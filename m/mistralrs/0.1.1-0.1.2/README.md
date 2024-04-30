# Comparing `tmp/mistralrs-0.1.1.tar.gz` & `tmp/mistralrs-0.1.2.tar.gz`

## Comparing `mistralrs-0.1.1.tar` & `mistralrs-0.1.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0     1000     1000      794 2024-04-26 00:59:23.000000 mistralrs-0.1.1/mistralrs-lora/Cargo.toml
--rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs-0.1.1/mistralrs-lora/README.md
--rw-r--r--   0     1000     1000     2395 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-lora/src/layer.rs
--rw-r--r--   0     1000     1000     5657 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-lora/src/lib.rs
--rw-r--r--   0     1000     1000     9437 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-lora/src/loralinear.rs
--rw-r--r--   0     1000     1000     9937 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-lora/src/qloralinear.rs
--rw-r--r--   0     1000     1000     1809 2024-04-27 15:00:53.000000 mistralrs-0.1.1/mistralrs-core/Cargo.toml
--rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs-0.1.1/mistralrs-core/README.md
--rw-r--r--   0     1000     1000      133 2024-04-11 10:11:30.000000 mistralrs-0.1.1/mistralrs-core/src/aici/README.md
--rw-r--r--   0     1000     1000     6551 2024-04-11 10:11:30.000000 mistralrs-0.1.1/mistralrs-core/src/aici/bintokens.rs
--rw-r--r--   0     1000     1000      320 2024-04-11 10:11:30.000000 mistralrs-0.1.1/mistralrs-core/src/aici/bytes.rs
--rw-r--r--   0     1000     1000    15114 2024-04-11 10:11:30.000000 mistralrs-0.1.1/mistralrs-core/src/aici/cfg.rs
--rw-r--r--   0     1000     1000     9819 2024-04-11 10:11:30.000000 mistralrs-0.1.1/mistralrs-core/src/aici/lex.rs
--rw-r--r--   0     1000     1000      179 2024-04-11 10:11:30.000000 mistralrs-0.1.1/mistralrs-core/src/aici/mod.rs
--rw-r--r--   0     1000     1000     2447 2024-04-19 18:01:00.000000 mistralrs-0.1.1/mistralrs-core/src/aici/recognizer.rs
--rw-r--r--   0     1000     1000     1696 2024-04-12 01:34:41.000000 mistralrs-0.1.1/mistralrs-core/src/aici/rx.rs
--rw-r--r--   0     1000     1000     3094 2024-04-11 10:11:30.000000 mistralrs-0.1.1/mistralrs-core/src/aici/svob.rs
--rw-r--r--   0     1000     1000    17311 2024-04-19 18:01:00.000000 mistralrs-0.1.1/mistralrs-core/src/aici/toktree.rs
--rw-r--r--   0     1000     1000     2935 2024-04-25 14:28:35.000000 mistralrs-0.1.1/mistralrs-core/src/device_map.rs
--rw-r--r--   0     1000     1000    30518 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/engine/mod.rs
--rw-r--r--   0     1000     1000     7286 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-core/src/layers.rs
--rw-r--r--   0     1000     1000     7646 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/lib.rs
--rw-r--r--   0     1000     1000     8310 2024-04-25 00:00:52.000000 mistralrs-0.1.1/mistralrs-core/src/model_loader.rs
--rw-r--r--   0     1000     1000    10703 2024-04-27 09:46:04.000000 mistralrs-0.1.1/mistralrs-core/src/model_selected.rs
--rw-r--r--   0     1000     1000    15669 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/models/gemma.rs
--rw-r--r--   0     1000     1000    14022 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/models/llama.rs
--rw-r--r--   0     1000     1000    15585 2024-04-27 09:51:16.000000 mistralrs-0.1.1/mistralrs-core/src/models/mistral.rs
--rw-r--r--   0     1000     1000    20102 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/models/mixtral.rs
--rw-r--r--   0     1000     1000     2620 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-core/src/models/mod.rs
--rw-r--r--   0     1000     1000    14708 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/models/phi2.rs
--rw-r--r--   0     1000     1000    14527 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/models/phi3.rs
--rw-r--r--   0     1000     1000    19588 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-core/src/models/quantized_llama.rs
--rw-r--r--   0     1000     1000    10095 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-core/src/models/quantized_phi2.rs
--rw-r--r--   0     1000     1000    15130 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/models/qwen2.rs
--rw-r--r--   0     1000     1000     4424 2024-04-25 23:09:22.000000 mistralrs-0.1.1/mistralrs-core/src/pipeline/chat_template.rs
--rw-r--r--   0     1000     1000    14978 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/pipeline/ggml.rs
--rw-r--r--   0     1000     1000    17012 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/pipeline/gguf.rs
--rw-r--r--   0     1000     1000    19303 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-core/src/pipeline/loaders.rs
--rw-r--r--   0     1000     1000     9952 2024-04-27 14:43:53.000000 mistralrs-0.1.1/mistralrs-core/src/pipeline/macros.rs
--rw-r--r--   0     1000     1000    32323 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/pipeline/mod.rs
--rw-r--r--   0     1000     1000    12875 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/pipeline/normal.rs
--rw-r--r--   0     1000     1000     6358 2024-04-23 22:49:11.000000 mistralrs-0.1.1/mistralrs-core/src/prefix_cacher.rs
--rw-r--r--   0     1000     1000     1241 2024-04-26 13:13:55.000000 mistralrs-0.1.1/mistralrs-core/src/request.rs
--rw-r--r--   0     1000     1000     3848 2024-04-23 22:49:11.000000 mistralrs-0.1.1/mistralrs-core/src/response.rs
--rw-r--r--   0     1000     1000    10578 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/sampler.rs
--rw-r--r--   0     1000     1000     7286 2024-04-23 22:49:11.000000 mistralrs-0.1.1/mistralrs-core/src/scheduler.rs
--rw-r--r--   0     1000     1000    15888 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/sequence.rs
--rw-r--r--   0     1000     1000     7016 2024-04-27 10:11:41.000000 mistralrs-0.1.1/mistralrs-core/src/utils/mod.rs
--rw-r--r--   0     1000     1000     1716 2024-04-27 14:58:30.000000 mistralrs-0.1.1/mistralrs-core/src/utils/tokens.rs
--rw-r--r--   0     1000     1000     4799 2024-04-23 22:49:11.000000 mistralrs-0.1.1/mistralrs-core/src/utils/varbuilder_utils.rs
--rw-r--r--   0     1000     1000    11049 2024-04-06 02:02:23.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/classifier.rs
--rw-r--r--   0     1000     1000     1544 2024-04-23 22:49:11.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/config.rs
--rw-r--r--   0     1000     1000    24214 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/gemma.rs
--rw-r--r--   0     1000     1000    21882 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/llama.rs
--rw-r--r--   0     1000     1000    23588 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/mistral.rs
--rw-r--r--   0     1000     1000    28628 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/mixtral.rs
--rw-r--r--   0     1000     1000     4181 2024-04-25 18:24:04.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/mod.rs
--rw-r--r--   0     1000     1000    22218 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/phi2.rs
--rw-r--r--   0     1000     1000    21111 2024-04-27 02:47:50.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/phi3.rs
--rw-r--r--   0     1000     1000    34138 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-core/src/xlora_models/quantized_llama.rs
--rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 mistralrs-0.1.1/mistralrs-pyo3/Cargo.toml
--rw-r--r--   0     1000     1000      686 2024-03-08 12:45:25.000000 mistralrs-0.1.1/mistralrs-pyo3/.gitignore
--rw-r--r--   0     1000     1000     3516 2024-04-27 09:46:04.000000 mistralrs-0.1.1/mistralrs-pyo3/API.md
--rw-r--r--   0     1000     1000      819 2024-04-27 15:00:53.000000 mistralrs-0.1.1/mistralrs-pyo3/Cargo_template.toml
--rw-r--r--   0     1000     1000     3755 2024-04-27 10:12:38.000000 mistralrs-0.1.1/mistralrs-pyo3/README.md
--rw-r--r--   0     1000     1000     8231 2024-04-27 02:02:03.000000 mistralrs-0.1.1/mistralrs-pyo3/mistralrs.pyi
--rw-r--r--   0     1000     1000      530 2024-04-27 15:00:53.000000 mistralrs-0.1.1/mistralrs-pyo3/pyproject_template.toml
--rw-r--r--   0     1000     1000    28363 2024-04-26 13:56:27.000000 mistralrs-0.1.1/mistralrs-pyo3/src/lib.rs
--rw-r--r--   0     1000     1000      397 2024-04-25 14:28:35.000000 mistralrs-0.1.1/mistralrs-pyo3/src/message.rs
--rw-r--r--   0     1000     1000     1590 2024-04-23 22:49:11.000000 mistralrs-0.1.1/mistralrs-pyo3/src/stream.rs
--rw-r--r--   0     1000     1000     3058 2024-04-25 00:00:52.000000 mistralrs-0.1.1/mistralrs-pyo3/src/which.rs
--rwxr-xr-x   0     1000     1000     2044 2024-04-27 10:25:16.000000 mistralrs-0.1.1/mistralrs-pyo3/upload.py
--rw-r--r--   0     1000     1000    97009 2024-04-27 15:00:53.000000 mistralrs-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 mistralrs-0.1.1/Cargo.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 mistralrs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 mistralrs-0.1.1/PKG-INFO
+-rw-r--r--   0     1000     1000      794 2024-04-26 00:59:23.000000 mistralrs-0.1.2/mistralrs-lora/Cargo.toml
+-rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs-0.1.2/mistralrs-lora/README.md
+-rw-r--r--   0     1000     1000     2395 2024-04-26 13:56:27.000000 mistralrs-0.1.2/mistralrs-lora/src/layer.rs
+-rw-r--r--   0     1000     1000     5818 2024-04-28 01:11:39.000000 mistralrs-0.1.2/mistralrs-lora/src/lib.rs
+-rw-r--r--   0     1000     1000     9472 2024-04-28 22:09:55.000000 mistralrs-0.1.2/mistralrs-lora/src/loralinear.rs
+-rw-r--r--   0     1000     1000     9961 2024-04-28 22:10:05.000000 mistralrs-0.1.2/mistralrs-lora/src/qloralinear.rs
+-rw-------   0     1000     1000     1974 2024-04-30 09:44:59.000000 mistralrs-0.1.2/mistralrs-core/Cargo.toml
+-rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs-0.1.2/mistralrs-core/README.md
+-rw-r--r--   0     1000     1000      133 2024-04-11 10:11:30.000000 mistralrs-0.1.2/mistralrs-core/src/aici/README.md
+-rw-r--r--   0     1000     1000     6567 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/aici/bintokens.rs
+-rw-r--r--   0     1000     1000      320 2024-04-11 10:11:30.000000 mistralrs-0.1.2/mistralrs-core/src/aici/bytes.rs
+-rw-r--r--   0     1000     1000    15114 2024-04-11 10:11:30.000000 mistralrs-0.1.2/mistralrs-core/src/aici/cfg.rs
+-rw-r--r--   0     1000     1000     9819 2024-04-11 10:11:30.000000 mistralrs-0.1.2/mistralrs-core/src/aici/lex.rs
+-rw-r--r--   0     1000     1000      179 2024-04-11 10:11:30.000000 mistralrs-0.1.2/mistralrs-core/src/aici/mod.rs
+-rw-r--r--   0     1000     1000     2447 2024-04-19 18:01:00.000000 mistralrs-0.1.2/mistralrs-core/src/aici/recognizer.rs
+-rw-r--r--   0     1000     1000     1696 2024-04-12 01:34:41.000000 mistralrs-0.1.2/mistralrs-core/src/aici/rx.rs
+-rw-r--r--   0     1000     1000     3094 2024-04-11 10:11:30.000000 mistralrs-0.1.2/mistralrs-core/src/aici/svob.rs
+-rw-r--r--   0     1000     1000    17311 2024-04-19 18:01:00.000000 mistralrs-0.1.2/mistralrs-core/src/aici/toktree.rs
+-rw-r--r--   0     1000     1000     4667 2024-04-28 01:11:39.000000 mistralrs-0.1.2/mistralrs-core/src/device_map.rs
+-rw-r--r--   0     1000     1000    36507 2024-04-30 09:43:44.000000 mistralrs-0.1.2/mistralrs-core/src/engine/mod.rs
+-rw-r--r--   0     1000     1000     7663 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/layers.rs
+-rw-r--r--   0     1000     1000     7868 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/lib.rs
+-rw-r--r--   0     1000     1000     8310 2024-04-25 00:00:52.000000 mistralrs-0.1.2/mistralrs-core/src/model_loader.rs
+-rw-r--r--   0     1000     1000    10703 2024-04-27 09:46:04.000000 mistralrs-0.1.2/mistralrs-core/src/model_selected.rs
+-rw-r--r--   0     1000     1000    16512 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/gemma.rs
+-rw-r--r--   0     1000     1000    15309 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/llama.rs
+-rw-r--r--   0     1000     1000    17943 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/mistral.rs
+-rw-r--r--   0     1000     1000    22512 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/mixtral.rs
+-rw-r--r--   0     1000     1000     2620 2024-04-26 13:56:27.000000 mistralrs-0.1.2/mistralrs-core/src/models/mod.rs
+-rw-r--r--   0     1000     1000    15629 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/phi2.rs
+-rw-r--r--   0     1000     1000    17509 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/phi3.rs
+-rw-r--r--   0     1000     1000    19605 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/quantized_llama.rs
+-rw-r--r--   0     1000     1000    10138 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/quantized_phi2.rs
+-rw-r--r--   0     1000     1000    16101 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/models/qwen2.rs
+-rw-r--r--   0     1000     1000     5912 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/pipeline/chat_template.rs
+-rw-r--r--   0     1000     1000    13809 2024-04-30 09:43:17.000000 mistralrs-0.1.2/mistralrs-core/src/pipeline/ggml.rs
+-rw-r--r--   0     1000     1000    15835 2024-04-30 09:43:17.000000 mistralrs-0.1.2/mistralrs-core/src/pipeline/gguf.rs
+-rw-r--r--   0     1000     1000    20832 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/pipeline/loaders.rs
+-rw-r--r--   0     1000     1000    10912 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/pipeline/macros.rs
+-rw-r--r--   0     1000     1000    33649 2024-04-30 09:43:17.000000 mistralrs-0.1.2/mistralrs-core/src/pipeline/mod.rs
+-rw-r--r--   0     1000     1000    12269 2024-04-30 09:43:17.000000 mistralrs-0.1.2/mistralrs-core/src/pipeline/normal.rs
+-rw-r--r--   0     1000     1000     6358 2024-04-23 22:49:11.000000 mistralrs-0.1.2/mistralrs-core/src/prefix_cacher.rs
+-rw-r--r--   0     1000     1000     1250 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/request.rs
+-rw-r--r--   0     1000     1000     3848 2024-04-23 22:49:11.000000 mistralrs-0.1.2/mistralrs-core/src/response.rs
+-rw-r--r--   0     1000     1000    11276 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/sampler.rs
+-rw-r--r--   0     1000     1000     7286 2024-04-23 22:49:11.000000 mistralrs-0.1.2/mistralrs-core/src/scheduler.rs
+-rw-r--r--   0     1000     1000    15979 2024-04-30 09:43:17.000000 mistralrs-0.1.2/mistralrs-core/src/sequence.rs
+-rw-r--r--   0     1000     1000     7395 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/utils/mod.rs
+-rw-r--r--   0     1000     1000     1716 2024-04-27 14:58:30.000000 mistralrs-0.1.2/mistralrs-core/src/utils/tokens.rs
+-rw-r--r--   0     1000     1000     4799 2024-04-23 22:49:11.000000 mistralrs-0.1.2/mistralrs-core/src/utils/varbuilder_utils.rs
+-rw-r--r--   0     1000     1000    11049 2024-04-06 02:02:23.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/classifier.rs
+-rw-r--r--   0     1000     1000     1544 2024-04-23 22:49:11.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/config.rs
+-rw-r--r--   0     1000     1000    26714 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/gemma.rs
+-rw-r--r--   0     1000     1000    25200 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/llama.rs
+-rw-r--r--   0     1000     1000    27603 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/mistral.rs
+-rw-r--r--   0     1000     1000    32915 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/mixtral.rs
+-rw-r--r--   0     1000     1000     4305 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/mod.rs
+-rw-r--r--   0     1000     1000    24492 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/phi2.rs
+-rw-r--r--   0     1000     1000    25455 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/phi3.rs
+-rw-r--r--   0     1000     1000    34219 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-core/src/xlora_models/quantized_llama.rs
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 mistralrs-0.1.2/mistralrs-pyo3/Cargo.toml
+-rw-r--r--   0     1000     1000      686 2024-03-08 12:45:25.000000 mistralrs-0.1.2/mistralrs-pyo3/.gitignore
+-rw-r--r--   0     1000     1000     3516 2024-04-27 09:46:04.000000 mistralrs-0.1.2/mistralrs-pyo3/API.md
+-rw-r--r--   0     1000     1000      855 2024-04-30 09:44:59.000000 mistralrs-0.1.2/mistralrs-pyo3/Cargo_template.toml
+-rw-r--r--   0     1000     1000     3755 2024-04-27 10:12:38.000000 mistralrs-0.1.2/mistralrs-pyo3/README.md
+-rw-r--r--   0     1000     1000     8231 2024-04-27 02:02:03.000000 mistralrs-0.1.2/mistralrs-pyo3/mistralrs.pyi
+-rw-r--r--   0     1000     1000      530 2024-04-30 09:44:59.000000 mistralrs-0.1.2/mistralrs-pyo3/pyproject_template.toml
+-rw-r--r--   0     1000     1000    28680 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-pyo3/src/lib.rs
+-rw-r--r--   0     1000     1000      397 2024-04-25 14:28:35.000000 mistralrs-0.1.2/mistralrs-pyo3/src/message.rs
+-rw-r--r--   0     1000     1000     1672 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-pyo3/src/stream.rs
+-rw-r--r--   0     1000     1000     3114 2024-04-30 09:38:13.000000 mistralrs-0.1.2/mistralrs-pyo3/src/which.rs
+-rwxr-xr-x   0     1000     1000     2044 2024-04-27 10:25:16.000000 mistralrs-0.1.2/mistralrs-pyo3/upload.py
+-rw-r--r--   0     1000     1000    99219 2024-04-30 09:54:03.000000 mistralrs-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 mistralrs-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 mistralrs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 mistralrs-0.1.2/PKG-INFO
```

### Comparing `mistralrs-0.1.1/mistralrs-lora/Cargo.toml` & `mistralrs-0.1.2/mistralrs-lora/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-lora/src/layer.rs` & `mistralrs-0.1.2/mistralrs-lora/src/layer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-lora/src/lib.rs` & `mistralrs-0.1.2/mistralrs-lora/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -126,24 +126,25 @@
         false
     }
 }
 
 pub fn linear(
     d1: usize,
     d2: usize,
+    base_vb: crate::VarBuilder,
     vb: VarBuilder,
     lora_config: &[(String, LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     let prefix = vb.prefix();
     let module = prefix.split('.').last().unwrap();
 
     let linear_config = LoraLinearConfig::new(d1, d2);
-    let inner = candle_nn::linear(d1, d2, vb.clone())?;
+    let inner = candle_nn::linear(d1, d2, base_vb.clone())?;
 
     let target_modules = &lora_config[0].1.target_modules;
     for (_, cfg) in lora_config {
         if &cfg.target_modules != target_modules {
             candle_core::bail!("Expected all target modules to be the same.");
         }
     }
@@ -158,24 +159,25 @@
     *count += 1;
     Ok(Arc::new(lorainner))
 }
 
 pub fn linear_no_bias(
     d1: usize,
     d2: usize,
+    base_vb: crate::VarBuilder,
     vb: VarBuilder,
     lora_config: &[(String, LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     let prefix = vb.prefix();
     let module = prefix.split('.').last().unwrap();
 
     let linear_config = LoraLinearConfig::new(d1, d2);
-    let inner = candle_nn::linear_no_bias(d1, d2, vb.clone())?;
+    let inner = candle_nn::linear_no_bias(d1, d2, base_vb.clone())?;
 
     let target_modules = &lora_config[0].1.target_modules;
     for (_, cfg) in lora_config {
         if &cfg.target_modules != target_modules {
             candle_core::bail!("Expected all target modules to be the same.");
         }
     }
@@ -191,26 +193,28 @@
     Ok(Arc::new(lorainner))
 }
 
 fn get_maybe_topk_scalings(scalings: Tensor, layer: usize) -> Result<Tensor> {
     scalings.i((.., .., layer, ..))
 }
 
+#[allow(clippy::too_many_arguments)]
 pub fn linear_b(
     in_dim: usize,
     out_dim: usize,
     bias: bool,
+    base_vb: crate::VarBuilder,
     vb: crate::VarBuilder,
     lora_config: &[(String, LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     if bias {
-        linear(in_dim, out_dim, vb, lora_config, count, ord)
+        linear(in_dim, out_dim, base_vb, vb, lora_config, count, ord)
     } else {
-        linear_no_bias(in_dim, out_dim, vb, lora_config, count, ord)
+        linear_no_bias(in_dim, out_dim, base_vb, vb, lora_config, count, ord)
     }
 }
 
 pub fn get_lora_cfg(tensor: &QTensor) -> LoraLinearConfig {
     LoraLinearConfig::new(tensor.shape().dims()[1], tensor.shape().dims()[0])
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-lora/src/loralinear.rs` & `mistralrs-0.1.2/mistralrs-lora/src/loralinear.rs`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 let (mut w_base_layer, dtype) = (q.dequantize(&q.device())?, q.dtype());
                 for adapter in 0..self.scale_adapters.len() {
                     w_base_layer = (w_base_layer + self.get_delta_weight(adapter))?;
                 }
                 let new_w = QTensor::quantize(&w_base_layer, dtype)?;
                 self.old = QLinear::from_qparts(new_w, self.old.bias().cloned());
             }
-            QMatMul::Tensor(w_base_layer) => {
+            QMatMul::Tensor(w_base_layer) | QMatMul::TensorF16(w_base_layer) => {
                 let mut w_base_layer = w_base_layer.clone();
                 for adapter in 0..self.scale_adapters.len() {
                     w_base_layer = (w_base_layer + self.get_delta_weight(adapter))?;
                 }
                 self.old = QLinear::from_parts(w_base_layer, self.old.bias().cloned());
             }
         };
```

### Comparing `mistralrs-0.1.1/mistralrs-lora/src/qloralinear.rs` & `mistralrs-0.1.2/mistralrs-lora/src/qloralinear.rs`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             _ => unreachable!("Both adapters must be Either::Left or Either::Right."),
         }
     }
 
     fn merge_weights(&mut self) -> Result<()> {
         let (mut w_base_layer, dtype) = match &self.old {
             QMatMul::QTensor(q) => (q.dequantize(&q.device())?, q.dtype()),
-            QMatMul::Tensor(_) => unreachable!(),
+            QMatMul::Tensor(_) | QMatMul::TensorF16(_) => unreachable!(),
         };
         for adapter in 0..self.scale_adapters.len() {
             w_base_layer = (w_base_layer + self.get_delta_weight(adapter))?;
         }
         let new_w = QTensor::quantize(&w_base_layer, dtype)?;
         self.old = QMatMul::from_qtensor(new_w)?;
         self.merged = true;
```

### Comparing `mistralrs-0.1.1/mistralrs-core/Cargo.toml` & `mistralrs-0.1.2/mistralrs-core/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 dirs = "5.0.1"
 hf-hub = "0.3.2"
 thiserror = "1.0.57"
 tokenizers = "0.15.2"
 tqdm = "0.7.0"
 range-checked = { git = "https://github.com/EricLBuehler/range-checked.git", version = "0.1.0" }
 chrono = "0.4.34"
-mistralrs-lora = { version = "0.1.1", path = "../mistralrs-lora" }
+mistralrs-lora = { version = "0.1.2", path = "../mistralrs-lora" }
 minijinja = "1.0.12"
 either.workspace = true
 indexmap.workspace = true
 half = "2.4.0"
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 tracing.workspace = true
@@ -41,14 +41,20 @@
 cfgrammar = "0.13.3"
 lrtable = "0.13.3"
 galil-seiferas = "0.1.5"
 clap.workspace = true
 radix_trie = "0.2.1"
 bytemuck = "1.15.0"
 pyo3.workspace = true
+rayon = "1.10.0"
+tokio.workspace = true
+tokio-rayon = "2.1.0"
+rand_isaac = "0.3.0"
+futures.workspace = true
+indicatif = { version = "0.17.8", features = ["rayon"] }
 
 [features]
 cuda = ["candle-core/cuda", "candle-nn/cuda", "candle-transformers/cuda"]
 cudnn = ["candle-core/cudnn"]
 metal = ["candle-core/metal", "candle-nn/metal", "candle-transformers/metal"]
 flash-attn = ["cuda", "candle-transformers/flash-attn", "dep:candle-flash-attn"]
 accelerate = ["candle-core/accelerate", "candle-nn/accelerate", "candle-transformers/accelerate"]
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/aici/bintokens.rs` & `mistralrs-0.1.2/mistralrs-core/src/aici/bintokens.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 // Licensed under the MIT license
 
 use crate::aici::{bytes::TokRxInfo, toktree::TokTrie};
 use anyhow::{anyhow, bail, Result};
 use serde::{Deserialize, Serialize};
 use std::collections::{BTreeMap, HashMap};
 use tokenizers::{normalizers::Sequence, NormalizerWrapper, Tokenizer};
-use tracing::{error, warn};
+use tracing::{error, info};
 
 #[derive(Serialize, Deserialize)]
 pub struct ByteTokenizer {
     pub hf_model: String,
     pub hf_tokenizer: Tokenizer,
     pub eos_token: u32,
     pub vocab_size: u32,
@@ -151,15 +151,15 @@
                     };
 
                     res.token_bytes[tok_id as usize] = bytes;
                 } else {
                     panic!();
                 }
             } else {
-                warn!("missing token: {}", tok_id);
+                info!("⚠️ WARNING: missing token: {}", tok_id);
             }
         }
 
         Ok(res)
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/aici/cfg.rs` & `mistralrs-0.1.2/mistralrs-core/src/aici/cfg.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/aici/lex.rs` & `mistralrs-0.1.2/mistralrs-core/src/aici/lex.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/aici/recognizer.rs` & `mistralrs-0.1.2/mistralrs-core/src/aici/recognizer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/aici/rx.rs` & `mistralrs-0.1.2/mistralrs-core/src/aici/rx.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/aici/svob.rs` & `mistralrs-0.1.2/mistralrs-core/src/aici/svob.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/aici/toktree.rs` & `mistralrs-0.1.2/mistralrs-core/src/aici/toktree.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/engine/mod.rs` & `mistralrs-0.1.2/mistralrs-core/src/engine/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 use std::{
-    cell::RefCell,
     collections::{HashMap, VecDeque},
     iter::zip,
-    rc::Rc,
-    sync::{mpsc::Receiver, Mutex},
+    sync::{Arc, Mutex},
     time::{Instant, SystemTime, UNIX_EPOCH},
 };
+use tokio::sync::mpsc::Receiver;
 
 use crate::{
-    aici::{cfg::CfgParser, recognizer::StackRecognizer, rx::RecRx},
-    handle_seq_error_ok, handle_seq_error_stateaware_ok,
+    aici::{cfg::CfgParser, recognizer::StackRecognizer, rx::RecRx, toktree::TokTrie},
+    get_bias_if_not_allowed, handle_seq_error_ok, handle_seq_error_stateaware_ok,
     response::CompletionChoice,
-    CompletionResponse, RequestMessage,
+    sample_async, sampler, CompletionResponse, RequestMessage,
 };
-use candle_core::{quantized::GgmlDType, Result, Tensor};
-use tracing::warn;
+use candle_core::{quantized::GgmlDType, DType, Device, Result, Tensor};
+use futures::future;
+use rand::SeedableRng;
+use rand_isaac::Isaac64Rng;
+use tracing::info;
 
 use crate::{
     get_mut_arcmutex, handle_pipeline_forward_error, handle_seq_error,
     pipeline::Pipeline,
     prefix_cacher::PrefixCacheManager,
     request::Request,
     response::{
@@ -32,30 +34,30 @@
 };
 
 const SEED: u64 = 0;
 
 pub struct Engine {
     rx: Receiver<Request>,
     isq_rx: Receiver<GgmlDType>,
-    pipeline: Box<Mutex<dyn Pipeline>>,
+    pipeline: Arc<Mutex<dyn Pipeline>>,
     scheduler: Scheduler<VecDeque<Sequence>>,
     id: usize,
     truncate_sequence: bool,
     no_kv_cache: bool,
     prefix_cacher: PrefixCacheManager,
     is_debug: bool,
     disable_eos_stop: bool,
 }
 
 impl Engine {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         rx: Receiver<Request>,
         isq_rx: Receiver<GgmlDType>,
-        pipeline: Box<Mutex<dyn Pipeline>>,
+        pipeline: Arc<Mutex<dyn Pipeline>>,
         method: SchedulerMethod,
         truncate_sequence: bool,
         no_kv_cache: bool,
         no_prefix_cache: bool,
         prefix_cache_n: usize,
         disable_eos_stop: bool,
     ) -> Self {
@@ -78,87 +80,122 @@
             is_debug: std::env::var("RUST_LOG")
                 .unwrap_or_default()
                 .contains("debug"),
             disable_eos_stop,
         }
     }
 
-    pub fn run(&mut self) {
-        let mut last_run = Instant::now();
+    pub async fn run(&mut self) {
+        let rng = Arc::new(Mutex::new(Isaac64Rng::seed_from_u64(SEED)));
         let mut last_completion_ids: Vec<usize> = vec![];
         'lp: loop {
             while let Ok(request) = self.rx.try_recv() {
-                self.add_request(request);
+                self.add_request(request).await;
             }
+            let run_start = Instant::now();
             let mut scheduled = self.scheduler.schedule();
-            let mut pipeline = get_mut_arcmutex!(self.pipeline);
             if let Ok(dtype) = self.isq_rx.try_recv() {
-                if let Err(e) = pipeline.re_isq_model(dtype) {
-                    warn!("ISQ requantization failed: {e:?}");
+                if let Err(e) = get_mut_arcmutex!(self.pipeline).re_isq_model(dtype) {
+                    info!("⚠️ WARNING: ISQ requantization failed: {e:?}");
                 }
             }
 
             if scheduled.completion.len() > 0 {
                 let current_completion_ids: Vec<usize> =
                     scheduled.completion.iter().map(|seq| *seq.id()).collect();
-                // Run the completion seqs
-                if !self.no_kv_cache && last_completion_ids != current_completion_ids {
-                    Self::clone_in_cache(&mut *pipeline, &mut scheduled.completion);
-                }
-                let logits = pipeline.forward(&scheduled.completion, false);
-                let logits = handle_pipeline_forward_error!(
-                    "completion",
-                    logits,
-                    &mut scheduled.completion,
-                    pipeline,
-                    'lp,
-                    self.prefix_cacher
-                );
+                let logits = {
+                    let logits = {
+                        let mut pipeline = get_mut_arcmutex!(self.pipeline);
+                        // Run the completion seqs
+                        // Run the completion seqs
+                        if !self.no_kv_cache && last_completion_ids != current_completion_ids {
+                            Self::clone_in_cache(&mut *pipeline, &mut scheduled.completion);
+                        }
+                        pipeline.forward(&scheduled.completion, false)
+                    };
+                    let logits = handle_pipeline_forward_error!(
+                        "completion",
+                        logits,
+                        &mut scheduled.completion,
+                        self.pipeline,
+                        'lp,
+                        self.prefix_cacher
+                    );
 
-                if !self.no_kv_cache {
-                    Self::clone_out_cache(&mut *pipeline, &mut scheduled.completion);
-                } else {
-                    Self::set_none_cache(&mut *pipeline);
-                }
+                    {
+                        let mut pipeline = get_mut_arcmutex!(self.pipeline);
+                        if !self.no_kv_cache {
+                            Self::clone_out_cache(&mut *pipeline, &mut scheduled.completion);
+                        } else {
+                            Self::set_none_cache(&mut *pipeline);
+                        }
+                    }
+                    logits
+                };
 
+                let sampled_result = Self::sample_seqs(
+                    self.pipeline.clone(),
+                    &mut scheduled.completion,
+                    logits,
+                    &mut self.prefix_cacher,
+                    self.disable_eos_stop,
+                    rng.clone(),
+                )
+                .await;
                 handle_pipeline_forward_error!(
                     "sampling",
-                    Self::sample_seqs(&mut *pipeline, &mut scheduled.completion, logits, &mut self.prefix_cacher, self.disable_eos_stop),
+                    sampled_result,
                     &mut scheduled.completion,
-                    pipeline,
+                    self.pipeline,
                     'lp,
                     self.prefix_cacher
                 );
                 last_completion_ids = current_completion_ids;
             }
 
             if scheduled.prompt.len() > 0 {
-                // Run the prompt seqs
-                Self::set_none_cache(&mut *pipeline);
-                let logits = pipeline.forward(&scheduled.prompt, true);
+                let logits = {
+                    let mut pipeline = get_mut_arcmutex!(self.pipeline);
+
+                    // Run the prompt seqs
+                    Self::set_none_cache(&mut *pipeline);
+                    pipeline.forward(&scheduled.prompt, true)
+                };
                 let logits = handle_pipeline_forward_error!(
                     "prompt",
                     logits,
                     &mut scheduled.prompt,
-                    pipeline,
+                    self.pipeline,
                     'lp,
                     self.prefix_cacher
                 );
 
-                if !self.no_kv_cache {
-                    Self::clone_out_cache(&mut *pipeline, &mut scheduled.prompt);
-                } else {
-                    Self::set_none_cache(&mut *pipeline);
+                {
+                    let mut pipeline = get_mut_arcmutex!(self.pipeline);
+                    if !self.no_kv_cache {
+                        Self::clone_out_cache(&mut *pipeline, &mut scheduled.prompt);
+                    } else {
+                        Self::set_none_cache(&mut *pipeline);
+                    }
                 }
 
+                let sampled_result = Self::sample_seqs(
+                    self.pipeline.clone(),
+                    &mut scheduled.prompt,
+                    logits,
+                    &mut self.prefix_cacher,
+                    self.disable_eos_stop,
+                    rng.clone(),
+                )
+                .await;
                 handle_pipeline_forward_error!(
                     "sampling",
-                    Self::sample_seqs(&mut *pipeline, &mut scheduled.prompt, logits, &mut self.prefix_cacher,self.disable_eos_stop,),
+                    sampled_result,
                     &mut scheduled.prompt,
-                    pipeline,
+                    self.pipeline,
                     'lp,
                     self.prefix_cacher
                 );
 
                 for seq in scheduled.prompt.iter_mut() {
                     seq.set_state(SequenceState::RunningCompletion);
                     let now = SystemTime::now()
@@ -170,16 +207,15 @@
                     seq.prompt_tok_per_sec = prompt_tok_per_sec * 1000.;
                     seq.prompt_timestamp = Some(now);
                 }
                 last_completion_ids = vec![];
             }
 
             if self.is_debug {
-                let ms_from_last_run = last_run.elapsed().as_millis();
-                last_run = Instant::now();
+                let ms_from_last_run = run_start.elapsed().as_millis();
                 let total_len = scheduled.prompt.len() + scheduled.completion.len();
                 if total_len > 0 {
                     let prompt_lengths = scheduled
                         .prompt
                         .iter()
                         .map(|seq| seq.len().to_string())
                         .collect::<Vec<_>>()
@@ -196,54 +232,145 @@
                         "Prompt[{}] Completion[{}] - {}ms",
                         prompt_lengths,
                         completion_lengths,
                         ms_from_last_run
                     );
                 }
             }
-            drop(pipeline);
             if scheduled.prompt.len() == 0
                 && scheduled.completion.len() == 0
                 && self.scheduler.waiting_len() == 0
             {
                 // If there is nothing to do, sleep until a request comes in
-                if let Ok(request) = self.rx.recv() {
-                    self.add_request(request);
+                if let Some(request) = self.rx.recv().await {
+                    self.add_request(request).await;
                 }
             }
         }
     }
 
-    fn sample_seqs(
-        pipeline: &mut dyn Pipeline,
+    async fn sample_sequence(
+        logits: Tensor,
+        seq: &mut Sequence,
+        return_logprobs: bool,
+        repeat_last_n: usize,
+        tok_trie: Arc<TokTrie>,
+        rng: Arc<Mutex<Isaac64Rng>>,
+        use_async_pool: bool,
+    ) -> Result<sampler::Logprobs> {
+        let logits = logits.squeeze(0)?.squeeze(0)?.to_dtype(DType::F32)?;
+        let start_at = seq.get_toks().len().saturating_sub(repeat_last_n);
+
+        let sampler = seq.sampler();
+        let logits_clone = logits.clone();
+        let ctx_clone = seq.get_toks()[start_at..].to_vec();
+        let rng_clone = rng.clone();
+        let first_lobprobs_response = sample_async!(
+            use_async_pool,
+            sampler,
+            logits_clone,
+            ctx_clone,
+            return_logprobs,
+            rng_clone
+        );
+
+        let bias_if_not_allowed = match &mut seq.recognizer {
+            SequenceRecognizer::Regex(ref mut rx) => {
+                get_bias_if_not_allowed!(tok_trie, rx.as_mut(), first_lobprobs_response.token)
+            }
+            SequenceRecognizer::Cfg(ref mut cfg) => {
+                get_bias_if_not_allowed!(tok_trie, cfg.as_mut(), first_lobprobs_response.token)
+            }
+            SequenceRecognizer::None => None,
+        };
+        let second_logprobs_response = match bias_if_not_allowed {
+            Some(token_set) => {
+                let mut acc = vec![-f32::INFINITY; tok_trie.vocab_size()];
+                token_set.apply_to(&mut acc);
+                let new_logits = (logits + Tensor::from_slice(&acc, acc.len(), &Device::Cpu)?)?;
+
+                let ctx_clone = seq.get_toks()[start_at..].to_vec();
+                let rng_clone = rng.clone();
+                let sampler = seq.sampler();
+                sample_async!(
+                    use_async_pool,
+                    sampler,
+                    new_logits,
+                    ctx_clone,
+                    return_logprobs,
+                    rng_clone
+                )
+            }
+            None => first_lobprobs_response,
+        };
+
+        match seq.recognizer {
+            SequenceRecognizer::Regex(ref mut rx) => {
+                tok_trie.append_token(rx.as_mut(), second_logprobs_response.token);
+            }
+            SequenceRecognizer::Cfg(ref mut cfg) => {
+                tok_trie.append_token(cfg.as_mut(), second_logprobs_response.token);
+            }
+            SequenceRecognizer::None => {}
+        }
+        Ok(second_logprobs_response)
+    }
+    async fn sample_seqs(
+        pipeline: Arc<Mutex<dyn Pipeline>>,
         seqs: &mut [&mut Sequence],
         logits: Tensor,
         prefix_cacher: &mut PrefixCacheManager,
         disable_eos_stop: bool,
+        rng: Arc<Mutex<Isaac64Rng>>,
     ) -> Result<()> {
         let seqs_len = seqs.len();
-        let logits_seq = logits.chunk(seqs_len, 0).unwrap();
+        let logits_seq = logits.to_device(&Device::Cpu)?.chunk(seqs_len, 0)?;
         debug_assert_eq!(logits_seq.len(), seqs_len);
-        let eos_tok = pipeline.eos_tok().to_vec();
-        for (logits_per_seq, seq) in zip(logits_seq, seqs.iter_mut()) {
-            // Sample and extract next token
-            let return_logprobs = seq.return_logprobs();
-            let sampled = pipeline.sample(logits_per_seq, seq, return_logprobs);
+
+        let (tok_trie, repeat_last_n, eos_tok, max_seq_len, pipeline_name) = {
+            let pipeline = get_mut_arcmutex!(pipeline);
+            let repeat_last_n = pipeline.get_repeat_last_n();
+            let tok_trie = pipeline.tok_trie();
+            let eos_tok = pipeline.eos_tok().to_vec();
+            let max_seq_len = pipeline.get_max_seq_len();
+            let pipeline_name = pipeline.name();
+            (tok_trie, repeat_last_n, eos_tok, max_seq_len, pipeline_name)
+        };
+
+        let use_async_pool = seqs_len > 1;
+
+        let sampling_futures: Vec<_> = zip(logits_seq, seqs.iter_mut())
+            .map(|(logits_per_seq, seq)| {
+                let return_logprobs = seq.return_logprobs();
+                Self::sample_sequence(
+                    logits_per_seq,
+                    seq,
+                    return_logprobs,
+                    repeat_last_n,
+                    tok_trie.clone(),
+                    rng.clone(),
+                    use_async_pool,
+                )
+            })
+            .collect();
+        let sampled_vec = future::join_all(sampling_futures).await;
+
+        for (sampled, seq) in zip(sampled_vec, seqs.iter_mut()) {
             let next_token = handle_seq_error_stateaware_ok!(sampled, seq);
             let next_token_id = next_token.token;
 
             let eos_tok = if disable_eos_stop {
                 None
             } else {
                 Some(eos_tok.as_ref())
             };
-            let is_done = seq.is_done(next_token_id, eos_tok, pipeline.get_max_seq_len());
+            let is_done = seq.is_done(next_token_id, eos_tok, max_seq_len);
             seq.add_token(
                 next_token.clone(),
-                pipeline.tok_trie().decode(&[next_token_id]),
+                tok_trie.decode(&[next_token_id]),
                 &is_done,
             );
             // Handle streaming requests
             if seq.get_mut_group().is_streaming && seq.get_mut_group().is_chat {
                 let token_index = seq.get_toks().len();
                 let rate_limit_allowed = is_done.is_some() || token_index % 3 == 0;
 
@@ -268,47 +395,53 @@
                             },
                         });
 
                         if let Some(reason) = is_done {
                             prefix_cacher.add_sequence(seq);
                             prefix_cacher.evict_to_cpu()?;
                             seq.set_state(SequenceState::Done(reason));
-                            pipeline.reset_non_granular_state();
+                            get_mut_arcmutex!(pipeline).reset_non_granular_state();
                         }
 
                         if seq
                             .get_mut_group()
-                            .maybe_send_streaming_response(seq, pipeline.name())
+                            .maybe_send_streaming_response(seq, pipeline_name.clone())
+                            .await
                             .is_err()
                         {
                             // If we can't send the response, cancel the sequence
                             seq.set_state(SequenceState::Done(StopReason::Canceled));
-                            pipeline.reset_non_granular_state();
+                            get_mut_arcmutex!(pipeline).reset_non_granular_state();
                         }
                     }
                 }
             } else if let Some(reason) = is_done {
-                Self::finish_seq(pipeline, seq, reason, prefix_cacher)?;
-                pipeline.reset_non_granular_state();
+                Self::finish_seq(pipeline.clone(), seq, reason, prefix_cacher).await?;
+                get_mut_arcmutex!(pipeline).reset_non_granular_state();
             }
         }
 
         Ok(())
     }
 
-    fn finish_seq(
-        pipeline: &mut dyn Pipeline,
+    async fn finish_seq(
+        pipeline: Arc<Mutex<dyn Pipeline>>,
         seq: &mut Sequence,
         reason: StopReason,
         prefix_cacher: &mut PrefixCacheManager,
     ) -> Result<()> {
         seq.set_state(SequenceState::Done(reason));
+        let (tokenizer, pipeline_name) = {
+            let pipeline = get_mut_arcmutex!(pipeline);
+            let pipeline_name = pipeline.name();
+            let tokenizer = pipeline.tokenizer();
+            (tokenizer, pipeline_name)
+        };
 
         let logprobs = if seq.return_logprobs() {
-            let tokenizer = pipeline.tokenizer().clone();
             let mut logprobs = Vec::new();
             for logprob in seq.logprobs() {
                 let resp_logprob = ResponseLogprob {
                     token: handle_seq_error_ok!(
                         tokenizer.decode(&[logprob.token], false),
                         seq.responder()
                     ),
@@ -362,39 +495,45 @@
         }
 
         prefix_cacher.add_sequence(seq);
         prefix_cacher.evict_to_cpu()?;
 
         let group = seq.get_mut_group();
         if group.is_chat {
-            group.maybe_send_done_response(
-                ChatCompletionResponse {
-                    id: seq.id().to_string(),
-                    choices: group.get_choices().to_vec(),
-                    created: seq.creation_time(),
-                    model: pipeline.name(),
-                    system_fingerprint: SYSTEM_FINGERPRINT.to_string(),
-                    object: "chat.completion".to_string(),
-                    usage: group.get_usage(),
-                },
-                seq.responder(),
-            );
+            group
+                .maybe_send_done_response(
+                    ChatCompletionResponse {
+                        id: seq.id().to_string(),
+                        choices: group.get_choices().to_vec(),
+                        created: seq.creation_time(),
+                        model: pipeline_name,
+                        system_fingerprint: SYSTEM_FINGERPRINT.to_string(),
+                        object: "chat.completion".to_string(),
+                        usage: group.get_usage(),
+                    },
+                    seq.responder(),
+                )
+                .await
+                .map_err(candle_core::Error::msg)?;
         } else {
-            group.maybe_send_completion_done_response(
-                CompletionResponse {
-                    id: seq.id().to_string(),
-                    choices: group.get_completion_choices().to_vec(),
-                    created: seq.creation_time(),
-                    model: pipeline.name(),
-                    system_fingerprint: SYSTEM_FINGERPRINT.to_string(),
-                    object: "text_completion".to_string(),
-                    usage: group.get_usage(),
-                },
-                seq.responder(),
-            );
+            group
+                .maybe_send_completion_done_response(
+                    CompletionResponse {
+                        id: seq.id().to_string(),
+                        choices: group.get_completion_choices().to_vec(),
+                        created: seq.creation_time(),
+                        model: pipeline_name,
+                        system_fingerprint: SYSTEM_FINGERPRINT.to_string(),
+                        object: "text_completion".to_string(),
+                        usage: group.get_usage(),
+                    },
+                    seq.responder(),
+                )
+                .await
+                .map_err(candle_core::Error::msg)?;
         }
 
         Ok(())
     }
 
     /// Clone the cache FROM the sequences' cache TO the model cache. Only used for completion seqs.
     fn clone_in_cache(pipeline: &mut dyn Pipeline, seqs: &mut [&mut Sequence]) {
@@ -541,15 +680,15 @@
                 }
                 Ok(Some(Tensor::from_vec(logits_bias, vocab_size, &device)?))
             }
             None => Ok(None),
         }
     }
 
-    fn add_request(&mut self, request: Request) {
+    async fn add_request(&mut self, request: Request) {
         let is_chat = matches!(request.messages, RequestMessage::Chat(_));
         let echo_prompt = matches!(
             request.messages,
             RequestMessage::Completion {
                 echo_prompt: true,
                 ..
             }
@@ -564,25 +703,23 @@
                 .get_chat_template()
                 .has_chat_template()
         {
             request
                     .response
                     .send(Response::ValidationError(
                         "Received messages for a model which does not have a chat template. Either use a different model or pass a single string as the prompt".into(),
-                    )).expect("Expected receiver.");
+                    )).await.expect("Expected receiver.");
             return;
         }
 
         let mut force_tokens = None;
         let formatted_prompt = match request.messages {
             RequestMessage::Chat(messages) => {
-                handle_seq_error!(
-                    get_mut_arcmutex!(self.pipeline).apply_chat_template(messages, true),
-                    request.response
-                )
+                let template = get_mut_arcmutex!(self.pipeline).apply_chat_template(messages, true);
+                handle_seq_error!(template, request.response)
             }
             RequestMessage::Completion { text, .. } => text,
             RequestMessage::CompletionTokens(it) => {
                 let res = get_mut_arcmutex!(self.pipeline)
                     .tokenizer()
                     .decode(&it, false)
                     .expect("cannot decode completion tokens");
@@ -592,32 +729,33 @@
         };
         if formatted_prompt.is_empty() {
             request
                 .response
                 .send(Response::ValidationError(
                     "Received an empty prompt.".into(),
                 ))
+                .await
                 .expect("Expected receiver.");
             return;
         }
         let mut prompt = match force_tokens {
             Some(tks) => tks,
-            None => handle_seq_error!(
-                get_mut_arcmutex!(self.pipeline).tokenize_prompt(&formatted_prompt),
-                request.response
-            ),
+            None => {
+                let prompt = get_mut_arcmutex!(self.pipeline).tokenize_prompt(&formatted_prompt);
+                handle_seq_error!(prompt, request.response)
+            }
         };
 
         if prompt.len() > get_mut_arcmutex!(self.pipeline).get_max_seq_len() {
             if !self.truncate_sequence {
                 request
                     .response
                     .send(Response::ValidationError(
                         format!("Prompt sequence length is greater than {}, perhaps consider using `truncate_sequence`?", get_mut_arcmutex!(self.pipeline).get_max_seq_len()).into(),
-                    )).expect("Expected receiver.");
+                    )).await.expect("Expected receiver.");
                 return;
             } else {
                 let prompt_len = prompt.len();
                 let max_len = get_mut_arcmutex!(self.pipeline).get_max_seq_len();
                 let currently_over = prompt_len - max_len;
                 let sampling_max = if let Some(sampling_max) = request.sampling_params.max_len {
                     if currently_over + sampling_max >= prompt_len {
@@ -625,15 +763,15 @@
                     } else {
                         sampling_max
                     }
                 } else {
                     10
                 };
                 prompt = prompt[(currently_over + sampling_max)..].to_vec();
-                warn!("Prompt for request {} was {} tokens over the model maximum length. The last {} tokens were truncated to make space for generation.", request.id, currently_over, prompt_len - prompt.len());
+                info!("⚠️ WARNING: Prompt for request {} was {} tokens over the model maximum length. The last {} tokens were truncated to make space for generation.", request.id, currently_over, prompt_len - prompt.len());
             }
         }
         let prefill_cache = handle_seq_error!(
             self.prefix_cacher.search_for_matching_cache(&prompt),
             request.response
         );
 
@@ -644,38 +782,43 @@
             .unwrap_or(-1);
         let topp = request.sampling_params.top_p.unwrap_or(1.0);
         let num_hidden_layers = get_mut_arcmutex!(self.pipeline).num_hidden_layers();
 
         let (stop_toks, stop_strings) = match request.sampling_params.stop_toks {
             None => (vec![], vec![]),
             Some(StopTokens::Ids(ref i)) => {
-                let pipeline = get_mut_arcmutex!(self.pipeline);
-                let tok_trie = pipeline.tok_trie();
+                let tok_trie = {
+                    let pipeline = get_mut_arcmutex!(self.pipeline);
+                    pipeline.tok_trie()
+                };
                 for id in i {
                     // We can't use ` ` (space) as a stop token because other tokens like ` moon` start with a space.
                     if tok_trie.has_extensions(tok_trie.token(*id)) {
                         request
                             .response
                             .send(Response::ValidationError(
                                 format!("Stop token {:?} is also a prefix of other tokens and cannot be used as a stop token.", tok_trie.token_str(*id)).into(),
                             ))
-                            .expect("Expected receiver.");
+                            .await .expect("Expected receiver.");
                         return;
                     }
                 }
 
                 (i.clone(), vec![])
             }
             Some(StopTokens::Seqs(ref s)) => {
                 let mut stop_toks = Vec::new();
                 let mut stop_strings: Vec<String> = Vec::new();
 
-                let pipeline = get_mut_arcmutex!(self.pipeline);
-                let tok_trie = pipeline.tok_trie();
-                let tokenizer = pipeline.tokenizer();
+                let (tok_trie, tokenizer) = {
+                    let pipeline = get_mut_arcmutex!(self.pipeline);
+                    let tok_trie = pipeline.tok_trie();
+                    let tokenizer = pipeline.tokenizer();
+                    (tok_trie, tokenizer)
+                };
 
                 for stop_txt in s {
                     let encoded = tokenizer.encode(stop_txt.to_string(), false);
                     let toks = handle_seq_error!(encoded, request.response)
                         .get_ids()
                         .to_vec();
 
@@ -690,15 +833,15 @@
                     }
                 }
 
                 (stop_toks, stop_strings)
             }
         };
 
-        let group = Rc::new(RefCell::new(SequenceGroup::new(
+        let group = Arc::new(tokio::sync::Mutex::new(SequenceGroup::new(
             request.sampling_params.n_choices,
             request.is_streaming,
             is_chat,
             best_of,
         )));
         let now = SystemTime::now()
             .duration_since(UNIX_EPOCH)
@@ -708,22 +851,22 @@
             Ok(logits_bias) => logits_bias,
             Err(err) => {
                 request
                     .response
                     .send(Response::ValidationError(
                         format!("Failed creation of logits bias. {}", err).into(),
                     ))
+                    .await
                     .expect("Expected receiver.");
                 return;
             }
         };
         let tokenizer = get_mut_arcmutex!(self.pipeline).tokenizer();
 
         let sampler = Sampler::new(
-            SEED,
             Some(request.sampling_params.temperature.unwrap_or(1.0)),
             request.sampling_params.top_n_logprobs,
             tokenizer,
             request.sampling_params.frequency_penalty,
             request.sampling_params.presence_penalty,
             logits_bias,
             topk,
@@ -733,18 +876,31 @@
             Ok(recognizer) => recognizer,
             Err(err) => {
                 request
                     .response
                     .send(Response::ValidationError(
                         format!("Invalid grammar. {}", err).into(),
                     ))
+                    .await
                     .expect("Expected receiver.");
                 return;
             }
         };
+
+        if request.sampling_params.n_choices == 0 {
+            request
+                .response
+                .send(Response::ValidationError(
+                    "Number of choices must be greater than 0.".into(),
+                ))
+                .await
+                .expect("Expected receiver.");
+            return;
+        }
+
         // Add sequences
         for response_index in 0..request.sampling_params.n_choices {
             let seq = Sequence::new_waiting(
                 prompt.clone(),
                 self.id,
                 now.as_millis(),
                 num_hidden_layers,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/layers.rs` & `mistralrs-0.1.2/mistralrs-core/src/layers.rs`

 * *Files 13% similar despite different names*

```diff
@@ -9,25 +9,36 @@
 };
 
 use crate::models::phi3;
 
 #[derive(Debug, Clone)]
 pub struct RmsNorm {
     inner: candle_nn::RmsNorm<RmsNormNonQuantized>,
+    eps: f64,
+    weight: Tensor,
 }
 
 impl RmsNorm {
     pub fn new(size: usize, eps: f64, vb: VarBuilder) -> Result<Self> {
         let inner = candle_nn::rms_norm_non_quant(size, eps, vb)?;
-        Ok(Self { inner })
+        let w = inner.inner().weight().clone();
+        Ok(Self {
+            inner,
+            eps,
+            weight: w,
+        })
     }
 }
 
 impl Module for RmsNorm {
     fn forward(&self, x: &Tensor) -> Result<Tensor> {
+        if x.device().is_cpu() {
+            // Handle device mapping case
+            return candle_nn::ops::rms_norm(&x.contiguous()?, &self.weight, self.eps as f32);
+        }
         self.inner.forward(x)
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct QRmsNorm {
     inner: candle_nn::RmsNorm<RmsNormQuantized>,
@@ -122,67 +133,65 @@
                     1f32 / (scaled_params.short_factor[k]
                         * cfg.rope_theta.powf(i as f64 / dim as f64) as f32)
                 })
                 .collect();
             let inv_freq_len = inv_freq_long.len();
 
             let t = Tensor::arange(0u32, max_seq_len as u32, dev)?
-                .to_dtype(dtype)?
+                .to_dtype(DType::F32)?
                 .reshape((max_seq_len, 1))?;
 
             // Calculate sin,cos for long
-            let inv_freq_long =
-                Tensor::from_vec(inv_freq_long, (1, inv_freq_len), dev)?.to_dtype(dtype)?;
+            let inv_freq_long = Tensor::from_vec(inv_freq_long, (1, inv_freq_len), dev)?;
             let freqs_long = t.matmul(&inv_freq_long)?;
-            let long_sin = freqs_long.sin()?.mul(scaling_factor)?;
-            let long_cos = freqs_long.cos()?.mul(scaling_factor)?;
+            let long_sin = freqs_long.sin()?.mul(scaling_factor)?.to_dtype(dtype)?;
+            let long_cos = freqs_long.cos()?.mul(scaling_factor)?.to_dtype(dtype)?;
 
             // Calculate sin,cos for short
-            let inv_freq_short =
-                Tensor::from_vec(inv_freq_short, (1, inv_freq_len), dev)?.to_dtype(dtype)?;
+            let inv_freq_short = Tensor::from_vec(inv_freq_short, (1, inv_freq_len), dev)?;
             let freqs_short = t.matmul(&inv_freq_short)?;
-            let short_sin = freqs_short.sin()?.mul(scaling_factor)?;
-            let short_cos = freqs_short.cos()?.mul(scaling_factor)?;
+            let short_sin = freqs_short.sin()?.mul(scaling_factor)?.to_dtype(dtype)?;
+            let short_cos = freqs_short.cos()?.mul(scaling_factor)?.to_dtype(dtype)?;
 
             Ok(Self {
                 short_cos,
                 short_sin,
                 long_cos: Some(long_cos),
                 long_sin: Some(long_sin),
                 original_max_position_embeddings: cfg.original_max_position_embeddings,
             })
         } else {
             let inv_freq: Vec<_> = (0..dim)
                 .step_by(2)
                 .map(|i| 1f32 / cfg.rope_theta.powf(i as f64 / dim as f64) as f32)
                 .collect();
             let inv_freq_len = inv_freq.len();
-            let inv_freq = Tensor::from_vec(inv_freq, (1, inv_freq_len), dev)?.to_dtype(dtype)?;
+            let inv_freq = Tensor::from_vec(inv_freq, (1, inv_freq_len), dev)?;
             let t = Tensor::arange(0u32, max_seq_len as u32, dev)?
-                .to_dtype(dtype)?
+                .to_dtype(DType::F32)?
                 .reshape((max_seq_len, 1))?;
             let freqs = t.matmul(&inv_freq)?;
-            let sin = freqs.sin()?;
-            let cos = freqs.cos()?;
+            let sin = freqs.sin()?.to_dtype(dtype)?;
+            let cos = freqs.cos()?.to_dtype(dtype)?;
             Ok(Self {
                 short_cos: cos,
                 short_sin: sin,
                 long_cos: None,
                 long_sin: None,
                 original_max_position_embeddings: cfg.original_max_position_embeddings,
             })
         }
     }
 
     /// Returns (sin, cos) taking into account LongRope
-    fn get_long_or_short_sin_cos(&self, seqlen_offsets: &[usize]) -> (&Tensor, &Tensor) {
+    fn get_long_or_short_sin_cos(&self, position_ids: &[usize]) -> (&Tensor, &Tensor) {
         if self.long_cos.is_none() {
             return (&self.short_sin, &self.short_cos);
         }
-        let seq_len = seqlen_offsets.iter().max().unwrap() + 1;
+        let seq_len = position_ids.iter().max().unwrap() + 1;
         if seq_len > self.original_max_position_embeddings {
             (
                 self.long_sin.as_ref().unwrap(),
                 self.long_cos.as_ref().unwrap(),
             )
         } else {
             (&self.short_sin, &self.short_cos)
@@ -190,19 +199,20 @@
     }
 
     pub fn forward(
         &self,
         q: &Tensor,
         k: &Tensor,
         seqlen_offsets: &[usize],
+        position_ids: &[usize],
     ) -> Result<(Tensor, Tensor)> {
         let (_b_sz, _h, seq_len, _n_embd) = q.dims4()?;
         let mut q_embeds = Vec::new();
         let mut k_embeds = Vec::new();
-        let (sin, cos) = self.get_long_or_short_sin_cos(seqlen_offsets);
+        let (sin, cos) = self.get_long_or_short_sin_cos(position_ids);
         for offset in seqlen_offsets {
             let cos = cos.narrow(0, *offset, seq_len)?;
             let sin = sin.narrow(0, *offset, seq_len)?;
             let q_embed = candle_nn::rotary_emb::rope(&q.contiguous()?, &cos, &sin)?;
             let k_embed = candle_nn::rotary_emb::rope(&k.contiguous()?, &cos, &sin)?;
             q_embeds.push(q_embed);
             k_embeds.push(k_embed);
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/lib.rs` & `mistralrs-0.1.2/mistralrs-core/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #![deny(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use std::{
     cell::RefCell,
     error::Error,
     fs::OpenOptions,
     io::Write,
-    sync::{
-        mpsc::{channel, Sender},
-        Arc, Mutex,
-    },
+    sync::{Arc, Mutex},
     thread,
     time::{SystemTime, UNIX_EPOCH},
 };
+use tokio::sync::mpsc::{channel, Sender};
 
 use candle_core::quantized::GgmlDType;
 use engine::Engine;
 pub use mistralrs_lora::Ordering;
 pub use pipeline::Pipeline;
 
 mod aici;
@@ -47,14 +45,15 @@
 };
 pub use request::{Constraint, Request, RequestMessage};
 pub use response::Response;
 pub use response::*;
 pub use sampler::{SamplingParams, StopTokens, TopLogprob};
 pub use scheduler::SchedulerMethod;
 use serde::Serialize;
+use tokio::runtime::Runtime;
 
 /// The MistralRs struct handles sending requests to the engine.
 /// It is the core multi-threaded component of mistral.rs, and uses `mspc`
 /// `Sender` and `Receiver` primitives to send and receive requests to the
 /// engine.
 pub struct MistralRs {
     sender: Sender<Request>,
@@ -65,26 +64,26 @@
     next_request_id: Mutex<RefCell<usize>>,
 }
 
 /// The MistralRsBuilder takes the pipeline and a scheduler method and constructs
 /// an Engine and a MistralRs instance. The Engine runs on a separate thread, and the MistralRs
 /// instance stays on the calling thread.
 pub struct MistralRsBuilder {
-    pipeline: Box<Mutex<dyn Pipeline>>,
+    pipeline: Arc<Mutex<dyn Pipeline>>,
     method: SchedulerMethod,
     log: Option<String>,
     truncate_sequence: Option<bool>,
     no_kv_cache: Option<bool>,
     no_prefix_cache: Option<bool>,
     prefix_cache_n: Option<usize>,
     disable_eos_stop: Option<bool>,
 }
 
 impl MistralRsBuilder {
-    pub fn new(pipeline: Box<Mutex<dyn Pipeline>>, method: SchedulerMethod) -> Self {
+    pub fn new(pipeline: Arc<Mutex<dyn Pipeline>>, method: SchedulerMethod) -> Self {
         Self {
             pipeline,
             method,
             log: None,
             truncate_sequence: None,
             no_kv_cache: None,
             no_prefix_cache: None,
@@ -142,55 +141,59 @@
 
         let truncate_sequence = truncate_sequence.unwrap_or(false);
         let no_kv_cache = no_kv_cache.unwrap_or(false);
         let no_prefix_cache = no_prefix_cache.unwrap_or(false);
         let prefix_cache_n = prefix_cache_n.unwrap_or(16);
         let disable_eos_stop = disable_eos_stop.unwrap_or(false);
 
-        let (tx, rx) = channel();
-        let (isq_tx, isq_rx) = channel();
+        let (tx, rx) = channel(10_000);
+        let (isq_tx, isq_rx) = channel(10_000);
 
         let this = Arc::new(Self {
             sender: tx,
             sender_isq: isq_tx,
             log,
             id: pipeline.lock().unwrap().name(),
             creation_time: SystemTime::now()
                 .duration_since(UNIX_EPOCH)
                 .expect("Time travel has occurred!")
                 .as_secs(),
             next_request_id: Mutex::new(RefCell::new(0)),
         });
-
         thread::spawn(move || {
-            let mut engine = Engine::new(
-                rx,
-                isq_rx,
-                pipeline,
-                method,
-                truncate_sequence,
-                no_kv_cache,
-                no_prefix_cache,
-                prefix_cache_n,
-                disable_eos_stop,
-            );
-            engine.run();
+            let rt = Runtime::new().unwrap();
+            rt.block_on(async move {
+                let mut engine = Engine::new(
+                    rx,
+                    isq_rx,
+                    pipeline,
+                    method,
+                    truncate_sequence,
+                    no_kv_cache,
+                    no_prefix_cache,
+                    prefix_cache_n,
+                    disable_eos_stop,
+                );
+                engine.run().await;
+            });
         });
 
         this
     }
 
     pub fn get_sender(&self) -> Sender<Request> {
         self.sender.clone()
     }
 
     /// Send a request to re-ISQ the model. If the model was loaded as GGUF or GGML
     /// then nothing will happen.
     pub fn send_re_isq(&self, dtype: GgmlDType) {
-        self.sender_isq.send(dtype).expect("Engine is not present.")
+        self.sender_isq
+            .blocking_send(dtype)
+            .expect("Engine is not present.")
     }
 
     pub fn get_id(&self) -> String {
         self.id.clone()
     }
 
     pub fn get_creation_time(&self) -> u64 {
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/model_loader.rs` & `mistralrs-0.1.2/mistralrs-core/src/model_loader.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/model_selected.rs` & `mistralrs-0.1.2/mistralrs-core/src/model_selected.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/gemma.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/qwen2.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,163 +1,114 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-use std::sync::Arc;
-
-use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
-use candle_nn::{linear_b as linear, Activation, RotaryEmbedding, VarBuilder};
+use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
+use candle_nn::{linear, linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
 use mistralrs_lora::layer::QLinear;
+use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
+    layers::RmsNorm,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
-fn default_max_position_embeddings() -> usize {
-    4096
-}
-
-#[derive(serde::Deserialize, Debug, Clone)]
+#[derive(Debug, Clone, PartialEq, serde::Deserialize)]
 pub struct Config {
-    pub attention_bias: bool,
-    pub head_dim: usize,
-    // The code gemma configs include both hidden_act and hidden_activation.
-    pub hidden_act: Option<Activation>,
-    pub hidden_activation: Option<Activation>,
+    pub vocab_size: usize,
     pub hidden_size: usize,
     pub intermediate_size: usize,
-    pub num_attention_heads: usize,
     pub num_hidden_layers: usize,
+    pub num_attention_heads: usize,
     pub num_key_value_heads: usize,
-    pub rms_norm_eps: f64,
-    pub rope_theta: f64,
-    pub vocab_size: usize,
-
-    #[serde(default = "default_max_position_embeddings")]
     pub max_position_embeddings: usize,
+    pub sliding_window: usize,
+    pub max_window_layers: usize,
+    pub tie_word_embeddings: bool,
+    pub rope_theta: f64,
+    pub rms_norm_eps: f64,
+    pub use_sliding_window: bool,
+    pub hidden_act: Activation,
     pub use_flash_attn: bool,
 }
 
-impl Config {
-    pub fn hidden_act(&self) -> Result<Activation> {
-        match (self.hidden_act, self.hidden_activation) {
-            (None, Some(act)) | (Some(act), None) => Ok(act),
-            (Some(_), Some(_)) => {
-                candle_core::bail!("both hidden_act and hidden_activation are set")
-            }
-            (None, None) => candle_core::bail!("none of hidden_act and hidden_activation are set"),
-        }
-    }
-}
-
-#[derive(Debug, Clone)]
-struct RmsNorm {
-    weight: Tensor,
-    eps: f64,
-}
-
-impl RmsNorm {
-    fn new(dim: usize, eps: f64, vb: VarBuilder) -> Result<Self> {
-        let weight = vb.get(dim, "weight")?;
-        Ok(Self { weight, eps })
-    }
-}
-
-impl Module for RmsNorm {
-    fn forward(&self, x: &Tensor) -> Result<Tensor> {
-        let x_dtype = x.dtype();
-        let internal_dtype = match x_dtype {
-            DType::F16 | DType::BF16 => DType::F32,
-            d => d,
-        };
-        let hidden_size = x.dim(D::Minus1)?;
-        let x = x.to_dtype(internal_dtype)?;
-        let norm_x = (x.sqr()?.sum_keepdim(D::Minus1)? / hidden_size as f64)?;
-        let x_normed = x.broadcast_div(&(norm_x + self.eps)?.sqrt()?)?;
-        x_normed
-            .to_dtype(x_dtype)?
-            .broadcast_mul(&(&self.weight + 1.0)?)
-    }
-}
-
 #[derive(Debug, Clone)]
 #[allow(clippy::upper_case_acronyms)]
 struct MLP {
-    gate_proj: QLinear,
-    up_proj: QLinear,
-    down_proj: QLinear,
-    act_fn: candle_nn::Activation,
+    gate_proj: QMatMul,
+    up_proj: QMatMul,
+    down_proj: QMatMul,
+    act_fn: Activation,
 }
 
 impl MLP {
     fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let intermediate_sz = cfg.intermediate_size;
-        let gate_proj = linear(hidden_sz, intermediate_sz, false, vb.pp("gate_proj"))?;
-        let up_proj = linear(hidden_sz, intermediate_sz, false, vb.pp("up_proj"))?;
-        let down_proj = linear(intermediate_sz, hidden_sz, false, vb.pp("down_proj"))?;
+        let gate_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("gate_proj"))?;
+        let up_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("up_proj"))?;
+        let down_proj = linear_no_bias(intermediate_sz, hidden_sz, vb.pp("down_proj"))?;
         Ok(Self {
-            gate_proj: QLinear::from_linear(gate_proj),
-            up_proj: QLinear::from_linear(up_proj),
-            down_proj: QLinear::from_linear(down_proj),
-            act_fn: cfg.hidden_act()?,
+            gate_proj: QMatMul::Tensor(gate_proj.weight().clone()),
+            up_proj: QMatMul::Tensor(up_proj.weight().clone()),
+            down_proj: QMatMul::Tensor(down_proj.weight().clone()),
+            act_fn: cfg.hidden_act,
         })
     }
 }
 
 impl Module for MLP {
     fn forward(&self, xs: &Tensor) -> Result<Tensor> {
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
-        if self.gate_proj.is_quant() {
+        if matches!(self.gate_proj, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
         let lhs = xs.apply(&self.gate_proj)?.apply(&self.act_fn)?;
         let rhs = xs.apply(&self.up_proj)?;
         let mut res = (lhs * rhs)?.apply(&self.down_proj)?;
-        if self.gate_proj.is_quant() {
+        if matches!(self.gate_proj, QMatMul::QTensor(_)) {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
 struct Attention {
     q_proj: QLinear,
     k_proj: QLinear,
     v_proj: QLinear,
-    o_proj: QLinear,
+    o_proj: QMatMul,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let num_kv_groups = num_heads / num_kv_heads;
-        let head_dim = cfg.head_dim;
-        let bias = cfg.attention_bias;
-        let q_proj = linear(hidden_sz, num_heads * head_dim, bias, vb.pp("q_proj"))?;
-        let k_proj = linear(hidden_sz, num_kv_heads * head_dim, bias, vb.pp("k_proj"))?;
-        let v_proj = linear(hidden_sz, num_kv_heads * head_dim, bias, vb.pp("v_proj"))?;
-        let o_proj = linear(num_heads * head_dim, hidden_sz, bias, vb.pp("o_proj"))?;
+        let head_dim = hidden_sz / num_heads;
+        let q_proj = linear(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
+        let k_proj = linear(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
+        let v_proj = linear(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
+        let o_proj = linear_no_bias(num_heads * head_dim, hidden_sz, vb.pp("o_proj"))?;
         Ok(Self {
             q_proj: QLinear::from_linear(q_proj),
             k_proj: QLinear::from_linear(k_proj),
             v_proj: QLinear::from_linear(v_proj),
-            o_proj: QLinear::from_linear(o_proj),
+            o_proj: QMatMul::Tensor(o_proj.weight().clone()),
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
         })
@@ -257,23 +208,37 @@
     self_attn: Attention,
     mlp: MLP,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
-    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
-        let mlp = MLP::new(cfg, vb.pp("mlp"))?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+    fn new(
+        rotary_emb: Arc<RotaryEmbedding>,
+        cfg: &Config,
+        vb: VarBuilder,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+    ) -> Result<Self> {
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
+        )?;
+        let mlp = MLP::new(cfg, mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq))?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
             post_attention_layernorm,
         })
@@ -305,116 +270,159 @@
 
 #[derive(Debug)]
 pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
+    sliding_window: usize,
     dtype: DType,
-    hidden_size: usize,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Model {
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
+        let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let vb_l = vb_m.pp("layers");
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(RotaryEmbedding::new(
                 cfg.rope_theta as f32,
-                cfg.head_dim,
+                head_dim,
                 cfg.max_position_embeddings,
-                mapper.device_for(layer_idx).unwrap_or(vb.device()),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
                 is_gptx,
                 vb.dtype(),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = QMatMul::Tensor(embed_tokens.embeddings().clone());
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
-            lm_head,
-            device: vb.device().clone(),
+            lm_head: QMatMul::Tensor(lm_head.weight().clone()),
+            sliding_window: cfg.sliding_window,
+            device: real_device,
             dtype: vb.dtype(),
-            hidden_size: cfg.hidden_size,
             cache: Cache::new(cfg.num_hidden_layers, false),
-            max_seq_len: default_max_position_embeddings(),
+            max_seq_len: cfg.max_position_embeddings,
             mapper,
         })
     }
 
     fn prepare_decoder_attention_mask(
         &self,
         b_size: usize,
         tgt_len: usize,
         seqlen_offset: usize,
     ) -> Result<Tensor> {
+        // Sliding window mask?
         let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| (0..tgt_len).map(move |j| if i < j { f32::NEG_INFINITY } else { 0. }))
+            .flat_map(|i| {
+                (0..tgt_len).map(move |j| {
+                    if i < j || j + self.sliding_window < i {
+                        f32::NEG_INFINITY
+                    } else {
+                        0.
+                    }
+                })
+            })
             .collect();
         let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
         let mask = if seqlen_offset > 0 {
             let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
             Tensor::cat(&[&mask0, &mask], D::Minus1)?
         } else {
             mask
         };
         mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
             .to_dtype(self.dtype)
     }
 
+    fn calculate_past_kv_len(&mut self, seq_len: usize) -> Result<usize> {
+        let cache = self.cache.lock();
+        let kv_cache_1 = cache.first().unwrap();
+        if kv_cache_1.is_none() {
+            return Ok(0);
+        }
+        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
+        if k_cache_1.dims()[0] <= seq_len {
+            Ok(0)
+        } else {
+            let indexed = k_cache_1.i(seq_len)?;
+            let dims = indexed.dims();
+            Ok(dims[dims.len() - 2])
+        }
+    }
+
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
+        let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
-            let mask = self.prepare_decoder_attention_mask(b_size, seq_len, seqlen_offsets[0])?;
+            let mask =
+                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
             Some(mask)
         };
-        let xs = self.embed_tokens.forward(input_ids)?;
-        let mut xs = (xs * (self.hidden_size as f64).sqrt())?;
+        let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = self.cache.lock();
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
                 seqlen_offsets,
                 start_offsets_kernel.clone(),
                 &mut cache[i],
-            )?;
+            )?
         }
         let xs = xs.to_device(&self.device)?;
         let mut xs = xs.apply(&self.norm)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
         extract_logits(&xs.apply(&self.lm_head)?, context_lens)
@@ -424,14 +432,15 @@
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
         )
@@ -443,14 +452,15 @@
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
@@ -458,22 +468,22 @@
     }
     fn is_xlora(&self) -> bool {
         false
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(&mut self.lm_head);
-        for layer in &mut self.layers {
-            tensors.push(layer.self_attn.q_proj.inner());
-            tensors.push(layer.self_attn.k_proj.inner());
-            tensors.push(layer.self_attn.v_proj.inner());
-            tensors.push(layer.self_attn.o_proj.inner());
-            tensors.push(layer.mlp.down_proj.inner());
-            tensors.push(layer.mlp.gate_proj.inner());
-            tensors.push(layer.mlp.up_proj.inner());
+        tensors.push((&mut self.lm_head, None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((layer.self_attn.q_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.k_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.v_proj.inner(), Some(i)));
+            tensors.push((&mut layer.self_attn.o_proj, Some(i)));
+            tensors.push((&mut layer.mlp.down_proj, Some(i)));
+            tensors.push((&mut layer.mlp.gate_proj, Some(i)));
+            tensors.push((&mut layer.mlp.up_proj, Some(i)));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/llama.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/llama.rs`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,26 @@
     layers::RmsNorm,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv};
 
-pub const MAX_SEQ_LEN: usize = 4096;
-
 #[derive(Debug, Clone, Deserialize)]
 pub struct Config {
     pub hidden_size: usize,
     pub intermediate_size: usize,
     pub vocab_size: usize,
     pub num_hidden_layers: usize,
     pub num_attention_heads: usize,
     pub num_key_value_heads: usize,
     pub use_flash_attn: bool,
     pub rms_norm_eps: f64,
     pub rope_theta: f32,
+    pub max_position_embeddings: usize,
 }
 
 #[derive(Debug, Clone)]
 pub struct Cache {
     masks: HashMap<usize, Tensor>,
 }
 
@@ -64,14 +63,15 @@
     v_proj: QMatMul,
     o_proj: QMatMul,
     num_attention_heads: usize,
     num_key_value_heads: usize,
     head_dim: usize,
     use_flash_attn: bool,
     rotary_emb: Arc<RotaryEmbedding>,
+    max_seq_len: usize,
 }
 
 impl CausalSelfAttention {
     fn forward(
         &self,
         x: &Tensor,
         seqlen_offsets: &[usize],
@@ -116,23 +116,23 @@
                 .contiguous()?;
         }
 
         if let Some((cache_k, cache_v)) = &kv_cache[block_idx] {
             k = candle_nn::ops::kvconcat(cache_k, &k, 2)?.contiguous()?;
             v = candle_nn::ops::kvconcat(cache_v, &v, 2)?.contiguous()?;
             let k_seq_len = k.dims()[1];
-            if k_seq_len > MAX_SEQ_LEN {
+            if k_seq_len > self.max_seq_len {
                 k = k
-                    .narrow(D::Minus1, k_seq_len - MAX_SEQ_LEN, MAX_SEQ_LEN)?
+                    .narrow(D::Minus1, k_seq_len - self.max_seq_len, self.max_seq_len)?
                     .contiguous()?
             }
             let v_seq_len = v.dims()[1];
-            if v_seq_len > 2 * MAX_SEQ_LEN {
+            if v_seq_len > 2 * self.max_seq_len {
                 v = v
-                    .narrow(D::Minus1, v_seq_len - MAX_SEQ_LEN, MAX_SEQ_LEN)?
+                    .narrow(D::Minus1, v_seq_len - self.max_seq_len, self.max_seq_len)?
                     .contiguous()?
             }
         }
         kv_cache[block_idx] = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_attention_heads / self.num_key_value_heads)?.contiguous()?;
         let v = repeat_kv(v, self.num_attention_heads / self.num_key_value_heads)?.contiguous()?;
@@ -165,41 +165,33 @@
         let mut y = self.o_proj.forward(&y)?;
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             y = y.to_dtype(original_dtype)?;
         }
         Ok(y)
     }
 
-    fn load(vb: VarBuilder, cfg: &Config, is_gptx: bool) -> Result<Self> {
+    fn load(vb: VarBuilder, cfg: &Config, rope: Arc<RotaryEmbedding>) -> Result<Self> {
         let size_in = cfg.hidden_size;
         let size_q = (cfg.hidden_size / cfg.num_attention_heads) * cfg.num_attention_heads;
         let size_kv = (cfg.hidden_size / cfg.num_attention_heads) * cfg.num_key_value_heads;
         let q_proj = linear(size_in, size_q, vb.pp("q_proj"))?;
         let k_proj = linear(size_in, size_kv, vb.pp("k_proj"))?;
         let v_proj = linear(size_in, size_kv, vb.pp("v_proj"))?;
         let o_proj = linear(size_q, size_in, vb.pp("o_proj"))?;
-        let head_dim = cfg.hidden_size / cfg.num_attention_heads;
-        let rotary_emb = Arc::new(RotaryEmbedding::new(
-            cfg.rope_theta,
-            head_dim,
-            MAX_SEQ_LEN,
-            vb.device(),
-            is_gptx,
-            vb.dtype(),
-        )?);
         Ok(Self {
             q_proj: QMatMul::Tensor(q_proj.weight().clone()),
             k_proj: QMatMul::Tensor(k_proj.weight().clone()),
             v_proj: QMatMul::Tensor(v_proj.weight().clone()),
             o_proj: QMatMul::Tensor(o_proj.weight().clone()),
             num_attention_heads: cfg.num_attention_heads,
             num_key_value_heads: cfg.num_key_value_heads,
             head_dim: cfg.hidden_size / cfg.num_attention_heads,
             use_flash_attn: cfg.use_flash_attn,
-            rotary_emb,
+            rotary_emb: rope,
+            max_seq_len: cfg.max_position_embeddings,
         })
     }
 }
 
 fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: f32) -> Result<Tensor> {
     let shape = mask.shape();
     let on_true = Tensor::new(on_true, on_false.device())?.broadcast_as(shape.dims())?;
@@ -272,22 +264,37 @@
             cache,
         )? + residual)?;
         let residual = &x;
         let x = (self.mlp.forward(&self.rms_2.forward(&x)?)? + residual)?;
         Ok(x)
     }
 
-    fn load(vb: VarBuilder, cfg: &Config, is_gptx: bool) -> Result<Self> {
-        let attn = CausalSelfAttention::load(vb.pp("self_attn"), cfg, is_gptx)?;
-        let mlp = Mlp::load(vb.pp("mlp"), cfg)?;
-        let rms_1 = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+    fn load(
+        vb: VarBuilder,
+        cfg: &Config,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        rope: Arc<RotaryEmbedding>,
+    ) -> Result<Self> {
+        let attn = CausalSelfAttention::load(
+            mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
+            cfg,
+            rope,
+        )?;
+        let mlp = Mlp::load(mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq), cfg)?;
+        let rms_1 = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb.pp("input_layernorm"), false),
+        )?;
         let rms_2 = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_nm_device(vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             rms_1,
             attn,
             rms_2,
             mlp,
         })
@@ -324,64 +331,93 @@
                 start_offsets_kernel.clone(),
                 block_idx,
                 &mut cache,
                 &mut self.cache,
             )?;
         }
         let x = x.to_device(&self.device)?;
-        let mut x = self.ln_f.forward(&x)?.to_dtype(DType::F32)?;
+        let mut x = self.ln_f.forward(&x)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             x = x.to_dtype(DType::F32)?;
         }
         let logits = self.lm_head.forward(&x)?;
         extract_logits(&logits, context_lens)
     }
 
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
-        let device = vb.device();
-        let wte = embedding(cfg.vocab_size, cfg.hidden_size, vb.pp("model.embed_tokens"))?;
-        let lm_head = linear(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
-        let ln_f = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("model.norm"))?;
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let wte = embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb.pp("model.embed_tokens"), false),
+        )?;
+        let lm_head = linear(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
+        let ln_f = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb.pp("model.norm"), false),
+        )?;
+        let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let blocks: Vec<_> = (0..cfg.num_hidden_layers)
             .map(|i| {
+                let rotary_emb = Arc::new(
+                    RotaryEmbedding::new(
+                        cfg.rope_theta,
+                        head_dim,
+                        cfg.max_position_embeddings,
+                        mapper.device_for(i, false).unwrap_or(&real_device),
+                        is_gptx,
+                        vb.dtype(),
+                    )
+                    .expect("Failed to create RoPE"),
+                );
                 Block::load(
-                    mapper.set_device(i, vb.pp(&format!("model.layers.{i}"))),
+                    vb.pp(&format!("model.layers.{i}")),
                     cfg,
-                    is_gptx,
+                    &*mapper,
+                    i,
+                    loading_isq,
+                    rotary_emb,
                 )
                 .expect("Failed to load block.")
             })
             .collect();
 
         Ok(Self {
             wte,
             blocks,
             ln_f,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             cache: Cache::new()?,
             kv_cache: super::Cache::new(cfg.num_hidden_layers, false),
-            device: device.clone(),
+            device: real_device,
             mapper,
         })
     }
 }
 
 impl NormalModel for Llama {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
         )
@@ -393,37 +429,38 @@
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &super::Cache {
         &self.kv_cache
     }
     fn device(&self) -> &Device {
         &self.device
     }
     fn is_xlora(&self) -> bool {
         false
     }
     fn max_seq_len(&self) -> usize {
-        MAX_SEQ_LEN
+        self.blocks[0].attn.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(&mut self.lm_head);
-        for layer in &mut self.blocks {
-            tensors.push(&mut layer.attn.q_proj);
-            tensors.push(&mut layer.attn.k_proj);
-            tensors.push(&mut layer.attn.v_proj);
-            tensors.push(&mut layer.attn.o_proj);
-            tensors.push(&mut layer.mlp.c_fc1);
-            tensors.push(&mut layer.mlp.c_fc2);
-            tensors.push(&mut layer.mlp.c_proj);
+        tensors.push((&mut self.lm_head, None));
+        for (i, layer) in self.blocks.iter_mut().enumerate() {
+            tensors.push((&mut layer.attn.q_proj, Some(i)));
+            tensors.push((&mut layer.attn.k_proj, Some(i)));
+            tensors.push((&mut layer.attn.v_proj, Some(i)));
+            tensors.push((&mut layer.attn.o_proj, Some(i)));
+            tensors.push((&mut layer.mlp.c_fc1, Some(i)));
+            tensors.push((&mut layer.mlp.c_fc2, Some(i)));
+            tensors.push((&mut layer.mlp.c_proj, Some(i)));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/mistral.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/gemma.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,117 +1,167 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-/// Mistral LLM, https://github.com/mistralai/mistral-src
-use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
-use candle_nn::{linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
 use std::sync::Arc;
 
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
+use candle_nn::{linear_b as linear, Activation, RotaryEmbedding, VarBuilder};
+use mistralrs_lora::layer::QLinear;
+
 use crate::{
     device_map::DeviceMapper,
-    layers::RmsNorm,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
-#[derive(Debug, Clone, PartialEq)]
+fn default_max_position_embeddings() -> usize {
+    4096
+}
+
+#[derive(serde::Deserialize, Debug, Clone)]
 pub struct Config {
-    pub(crate) vocab_size: usize,
-    pub(crate) hidden_size: usize,
-    pub(crate) intermediate_size: usize,
-    pub(crate) num_hidden_layers: usize,
-    pub(crate) num_attention_heads: usize,
-    pub(crate) num_key_value_heads: usize,
-    pub(crate) hidden_act: Activation,
-    pub(crate) max_position_embeddings: usize,
-    pub(crate) rms_norm_eps: f64,
-    pub(crate) rope_theta: f64,
-    pub(crate) sliding_window: Option<usize>,
-    pub(crate) use_flash_attn: bool,
+    pub attention_bias: bool,
+    pub head_dim: usize,
+    // The code gemma configs include both hidden_act and hidden_activation.
+    pub hidden_act: Option<Activation>,
+    pub hidden_activation: Option<Activation>,
+    pub hidden_size: usize,
+    pub intermediate_size: usize,
+    pub num_attention_heads: usize,
+    pub num_hidden_layers: usize,
+    pub num_key_value_heads: usize,
+    pub rms_norm_eps: f64,
+    pub rope_theta: f64,
+    pub vocab_size: usize,
+
+    #[serde(default = "default_max_position_embeddings")]
+    pub max_position_embeddings: usize,
+    pub use_flash_attn: bool,
+}
+
+impl Config {
+    pub fn hidden_act(&self) -> Result<Activation> {
+        match (self.hidden_act, self.hidden_activation) {
+            (None, Some(act)) | (Some(act), None) => Ok(act),
+            (Some(_), Some(_)) => {
+                candle_core::bail!("both hidden_act and hidden_activation are set")
+            }
+            (None, None) => candle_core::bail!("none of hidden_act and hidden_activation are set"),
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
+struct RmsNorm {
+    weight: Tensor,
+    eps: f64,
+}
+
+impl RmsNorm {
+    fn new(dim: usize, eps: f64, vb: VarBuilder) -> Result<Self> {
+        let weight = vb.get(dim, "weight")?;
+        Ok(Self { weight, eps })
+    }
+}
+
+impl Module for RmsNorm {
+    fn forward(&self, x: &Tensor) -> Result<Tensor> {
+        let x_dtype = x.dtype();
+        let internal_dtype = match x_dtype {
+            DType::F16 | DType::BF16 => DType::F32,
+            d => d,
+        };
+        let hidden_size = x.dim(D::Minus1)?;
+        let x = x.to_dtype(internal_dtype)?;
+        let norm_x = (x.sqr()?.sum_keepdim(D::Minus1)? / hidden_size as f64)?;
+        let x_normed = x.broadcast_div(&(norm_x + self.eps)?.sqrt()?)?;
+        x_normed
+            .to_dtype(x_dtype)?
+            .broadcast_mul(&(&self.weight + 1.0)?)
+    }
 }
 
 #[derive(Debug, Clone)]
 #[allow(clippy::upper_case_acronyms)]
 struct MLP {
-    gate_proj: QMatMul,
-    up_proj: QMatMul,
-    down_proj: QMatMul,
-    act_fn: Activation,
+    gate_proj: QLinear,
+    up_proj: QLinear,
+    down_proj: QLinear,
+    act_fn: candle_nn::Activation,
 }
 
 impl MLP {
     fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let intermediate_sz = cfg.intermediate_size;
-        let gate_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("gate_proj"))?;
-        let up_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("up_proj"))?;
-        let down_proj = linear_no_bias(intermediate_sz, hidden_sz, vb.pp("down_proj"))?;
+        let gate_proj = linear(hidden_sz, intermediate_sz, false, vb.pp("gate_proj"))?;
+        let up_proj = linear(hidden_sz, intermediate_sz, false, vb.pp("up_proj"))?;
+        let down_proj = linear(intermediate_sz, hidden_sz, false, vb.pp("down_proj"))?;
         Ok(Self {
-            gate_proj: QMatMul::Tensor(gate_proj.weight().clone()),
-            up_proj: QMatMul::Tensor(up_proj.weight().clone()),
-            down_proj: QMatMul::Tensor(down_proj.weight().clone()),
-            act_fn: cfg.hidden_act,
+            gate_proj: QLinear::from_linear(gate_proj),
+            up_proj: QLinear::from_linear(up_proj),
+            down_proj: QLinear::from_linear(down_proj),
+            act_fn: cfg.hidden_act()?,
         })
     }
 }
 
 impl Module for MLP {
     fn forward(&self, xs: &Tensor) -> Result<Tensor> {
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
-        if matches!(self.gate_proj, QMatMul::QTensor(_)) {
+        if self.gate_proj.is_quant() {
             xs = xs.to_dtype(DType::F32)?;
         }
         let lhs = xs.apply(&self.gate_proj)?.apply(&self.act_fn)?;
         let rhs = xs.apply(&self.up_proj)?;
         let mut res = (lhs * rhs)?.apply(&self.down_proj)?;
-        if matches!(self.gate_proj, QMatMul::QTensor(_)) {
+        if self.gate_proj.is_quant() {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
 struct Attention {
-    q_proj: QMatMul,
-    k_proj: QMatMul,
-    v_proj: QMatMul,
-    o_proj: QMatMul,
+    q_proj: QLinear,
+    k_proj: QLinear,
+    v_proj: QLinear,
+    o_proj: QLinear,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
-    hidden_size: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let num_kv_groups = num_heads / num_kv_heads;
-        let head_dim = hidden_sz / num_heads;
-        let q_proj = linear_no_bias(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
-        let k_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
-        let v_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
-        let o_proj = linear_no_bias(num_heads * head_dim, hidden_sz, vb.pp("o_proj"))?;
+        let head_dim = cfg.head_dim;
+        let bias = cfg.attention_bias;
+        let q_proj = linear(hidden_sz, num_heads * head_dim, bias, vb.pp("q_proj"))?;
+        let k_proj = linear(hidden_sz, num_kv_heads * head_dim, bias, vb.pp("k_proj"))?;
+        let v_proj = linear(hidden_sz, num_kv_heads * head_dim, bias, vb.pp("v_proj"))?;
+        let o_proj = linear(num_heads * head_dim, hidden_sz, bias, vb.pp("o_proj"))?;
         Ok(Self {
-            q_proj: QMatMul::Tensor(q_proj.weight().clone()),
-            k_proj: QMatMul::Tensor(k_proj.weight().clone()),
-            v_proj: QMatMul::Tensor(v_proj.weight().clone()),
-            o_proj: QMatMul::Tensor(o_proj.weight().clone()),
+            q_proj: QLinear::from_linear(q_proj),
+            k_proj: QLinear::from_linear(k_proj),
+            v_proj: QLinear::from_linear(v_proj),
+            o_proj: QLinear::from_linear(o_proj),
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
-            hidden_size: hidden_sz,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
         })
     }
 
     fn forward(
         &mut self,
@@ -121,21 +171,21 @@
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
     ) -> Result<Tensor> {
         let (b_sz, q_len, _) = xs.dims3()?;
 
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
-        if matches!(self.q_proj, QMatMul::QTensor(_)) {
+        if self.q_proj.is_quant() {
             xs = xs.to_dtype(DType::F32)?;
         }
         let mut q = self.q_proj.forward(&xs)?;
         let mut k = self.k_proj.forward(&xs)?;
         let mut v = self.v_proj.forward(&xs)?;
-        if matches!(self.q_proj, QMatMul::QTensor(_)) {
+        if self.q_proj.is_quant() {
             q = q.to_dtype(original_dtype)?;
             k = k.to_dtype(original_dtype)?;
             v = v.to_dtype(original_dtype)?;
         }
 
         let mut q = q.reshape((b_sz * q_len, self.num_heads, self.head_dim))?;
         let mut k = k.reshape((b_sz * q_len, self.num_kv_heads, self.head_dim))?;
@@ -184,22 +234,22 @@
             let attn_weights = match attention_mask {
                 None => attn_weights,
                 Some(mask) => attn_weights.broadcast_add(mask)?,
             };
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
-        if matches!(self.q_proj, QMatMul::QTensor(_)) {
+        if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
             .transpose(1, 2)?
-            .reshape((b_sz, q_len, self.hidden_size))?
+            .reshape((b_sz, q_len, ()))?
             .apply(&self.o_proj)?;
-        if matches!(self.q_proj, QMatMul::QTensor(_)) {
+        if self.q_proj.is_quant() {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
@@ -207,23 +257,37 @@
     self_attn: Attention,
     mlp: MLP,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
-    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
-        let mlp = MLP::new(cfg, vb.pp("mlp"))?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+    fn new(
+        rotary_emb: Arc<RotaryEmbedding>,
+        cfg: &Config,
+        vb: VarBuilder,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+    ) -> Result<Self> {
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
+        )?;
+        let mlp = MLP::new(cfg, mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq))?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
             post_attention_layernorm,
         })
@@ -255,135 +319,115 @@
 
 #[derive(Debug)]
 pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
-    sliding_window: Option<usize>,
     dtype: DType,
+    hidden_size: usize,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Model {
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
-        let head_dim = cfg.hidden_size / cfg.num_attention_heads;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(RotaryEmbedding::new(
                 cfg.rope_theta as f32,
-                head_dim,
+                cfg.head_dim,
                 cfg.max_position_embeddings,
-                mapper.device_for(layer_idx).unwrap_or(vb.device()),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
                 is_gptx,
                 vb.dtype(),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = QMatMul::Tensor(embed_tokens.embeddings().clone());
         Ok(Self {
             embed_tokens,
             layers,
             norm,
-            lm_head: QMatMul::Tensor(lm_head.weight().clone()),
-            sliding_window: cfg.sliding_window,
-            device: vb.device().clone(),
+            lm_head,
+            device: real_device,
             dtype: vb.dtype(),
+            hidden_size: cfg.hidden_size,
             cache: Cache::new(cfg.num_hidden_layers, false),
-            max_seq_len: cfg.max_position_embeddings,
+            max_seq_len: default_max_position_embeddings(),
             mapper,
         })
     }
 
     fn prepare_decoder_attention_mask(
         &self,
         b_size: usize,
         tgt_len: usize,
         seqlen_offset: usize,
     ) -> Result<Tensor> {
-        // Sliding window mask
-        let sliding_window = self.sliding_window.unwrap_or(tgt_len + 1);
         let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
+            .flat_map(|i| (0..tgt_len).map(move |j| if i < j { f32::NEG_INFINITY } else { 0. }))
             .collect();
         let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
         let mask = if seqlen_offset > 0 {
             let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
             Tensor::cat(&[&mask0, &mask], D::Minus1)?
         } else {
             mask
         };
         mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
             .to_dtype(self.dtype)
     }
 
-    fn calculate_past_kv_len(&mut self, seq_len: usize) -> Result<usize> {
-        let cache = self.cache.lock();
-        let kv_cache_1 = cache.first().unwrap();
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        if k_cache_1.dims()[0] <= seq_len {
-            Ok(0)
-        } else {
-            let indexed = k_cache_1.i(seq_len)?;
-            let dims = indexed.dims();
-            Ok(dims[dims.len() - 2])
-        }
-    }
-
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
-        if seqlen_offsets.len() > b_size {
-            candle_core::bail!("Expected seqlen offsets have length equal to batch size.")
-        }
-
-        let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
+            let mask = self.prepare_decoder_attention_mask(b_size, seq_len, seqlen_offsets[0])?;
             Some(mask)
         };
-        let mut xs = self.embed_tokens.forward(input_ids)?;
+        let xs = self.embed_tokens.forward(input_ids)?;
+        let mut xs = (xs * (self.hidden_size as f64).sqrt())?;
         let mut cache = self.cache.lock();
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
@@ -406,14 +450,15 @@
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
         )
@@ -425,14 +470,15 @@
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
@@ -440,22 +486,22 @@
     }
     fn is_xlora(&self) -> bool {
         false
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(&mut self.lm_head);
-        for layer in &mut self.layers {
-            tensors.push(&mut layer.self_attn.q_proj);
-            tensors.push(&mut layer.self_attn.k_proj);
-            tensors.push(&mut layer.self_attn.v_proj);
-            tensors.push(&mut layer.self_attn.o_proj);
-            tensors.push(&mut layer.mlp.down_proj);
-            tensors.push(&mut layer.mlp.gate_proj);
-            tensors.push(&mut layer.mlp.up_proj);
+        tensors.push((&mut self.lm_head, None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((layer.self_attn.q_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.k_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.v_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.o_proj.inner(), Some(i)));
+            tensors.push((layer.mlp.down_proj.inner(), Some(i)));
+            tensors.push((layer.mlp.gate_proj.inner(), Some(i)));
+            tensors.push((layer.mlp.up_proj.inner(), Some(i)));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/mixtral.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/mixtral.rs`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     hidden_size: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
+    sliding_window: Option<usize>,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
@@ -70,14 +71,15 @@
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
             hidden_size: hidden_sz,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
+            sliding_window: Some(cfg.sliding_window),
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
@@ -117,20 +119,48 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
+        let (k, v, attn_mask) = match kv_cache.clone() {
+            None => (k, v, attention_mask.cloned()),
+            Some((mut prev_k, mut prev_v)) => {
+                let mut mask = attention_mask.cloned();
+                if let Some(sliding_window) = self.sliding_window {
+                    let kv_seq_len = prev_k.dim(2)?;
+                    if kv_seq_len > sliding_window {
+                        prev_k = prev_k.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        prev_v = prev_v.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        if let Some(ref mut mask) = mask {
+                            let mask_len = mask.dim(1)?;
+                            *mask = mask.narrow(
+                                1,
+                                mask_len - (sliding_window - 1),
+                                sliding_window - 1,
+                            )?;
+                            *mask = Tensor::cat(
+                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
+                                D::Minus1,
+                            )?;
+                        }
+                    }
+                }
+                let k = candle_nn::ops::kvconcat(&prev_k, &k, 2)?;
+                let v = candle_nn::ops::kvconcat(&prev_v, &v, 2)?;
+                (k, v, mask)
             }
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
@@ -141,17 +171,17 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
+            let attn_weights = match attn_mask {
                 None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
+                Some(mask) => attn_weights.broadcast_add(&mask)?,
             };
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
@@ -305,23 +335,40 @@
     self_attn: Attention,
     block_sparse_moe: SparseMoeBlock,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
-    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
-        let block_sparse_moe = SparseMoeBlock::new(cfg, vb.pp("block_sparse_moe"))?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+    fn new(
+        rotary_emb: Arc<RotaryEmbedding>,
+        cfg: &Config,
+        vb: VarBuilder,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+    ) -> Result<Self> {
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
+        )?;
+        let block_sparse_moe = SparseMoeBlock::new(
+            cfg,
+            mapper.set_device(layer_idx, vb.pp("block_sparse_moe"), loading_isq),
+        )?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             block_sparse_moe,
             input_layernorm,
             post_attention_layernorm,
         })
@@ -369,47 +416,63 @@
 
 impl Model {
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(RotaryEmbedding::new(
                 cfg.rope_theta as f32,
                 head_dim,
                 cfg.max_position_embeddings,
-                mapper.device_for(layer_idx).unwrap_or(vb.device()),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
                 is_gptx,
                 vb.dtype(),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             sliding_window: cfg.sliding_window,
-            device: vb.device().clone(),
+            device: real_device,
             dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
         })
     }
 
@@ -501,14 +564,15 @@
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
         )
@@ -520,14 +584,15 @@
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
@@ -535,25 +600,25 @@
     }
     fn is_xlora(&self) -> bool {
         false
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(&mut self.lm_head);
-        for layer in &mut self.layers {
-            tensors.push(&mut layer.self_attn.q_proj);
-            tensors.push(&mut layer.self_attn.k_proj);
-            tensors.push(&mut layer.self_attn.v_proj);
-            tensors.push(&mut layer.self_attn.o_proj);
-            tensors.push(&mut layer.block_sparse_moe.gate);
+        tensors.push((&mut self.lm_head, None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((&mut layer.self_attn.q_proj, Some(i)));
+            tensors.push((&mut layer.self_attn.k_proj, Some(i)));
+            tensors.push((&mut layer.self_attn.v_proj, Some(i)));
+            tensors.push((&mut layer.self_attn.o_proj, Some(i)));
+            tensors.push((&mut layer.block_sparse_moe.gate, Some(i)));
             for expert in &mut layer.block_sparse_moe.experts {
-                tensors.push(&mut expert.w1);
-                tensors.push(&mut expert.w2);
-                tensors.push(&mut expert.w3);
+                tensors.push((&mut expert.w1, Some(i)));
+                tensors.push((&mut expert.w2, Some(i)));
+                tensors.push((&mut expert.w3, Some(i)));
             }
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/mod.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/phi2.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/phi2.rs`

 * *Files 5% similar despite different names*

```diff
@@ -113,32 +113,22 @@
     let shape = mask.shape();
     let on_true = Tensor::new(on_true, on_false.device())?.broadcast_as(shape.dims())?;
     let m = mask.where_cond(&on_true, on_false)?;
     Ok(m)
 }
 
 impl Attention {
-    fn new(cfg: &Config, vb: VarBuilder, is_gptx: bool) -> Result<Self> {
+    fn new(cfg: &Config, vb: VarBuilder, rope: RotaryEmbedding) -> Result<Self> {
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads();
         let head_dim = cfg.head_dim();
         let q_proj = linear(cfg.hidden_size, num_heads * head_dim, vb.pp("q_proj"))?;
         let k_proj = linear(cfg.hidden_size, num_kv_heads * head_dim, vb.pp("k_proj"))?;
         let v_proj = linear(cfg.hidden_size, num_kv_heads * head_dim, vb.pp("v_proj"))?;
         let dense = linear(num_heads * head_dim, cfg.hidden_size, vb.pp("dense"))?;
-        // Alternative rope scalings are not supported.
-        let rotary_emb = RotaryEmbedding::new_partial(
-            cfg.rope_theta,
-            cfg.head_dim(),
-            (cfg.partial_rotary_factor * cfg.head_dim() as f64) as usize,
-            cfg.max_position_embeddings,
-            vb.device(),
-            is_gptx,
-            vb.dtype(),
-        )?;
         let (q_layernorm, k_layernorm) = if cfg.qk_layernorm {
             let q_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("q_layernorm"))?;
             let k_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("k_layernorm"))?;
             (Some(q_layernorm), Some(k_layernorm))
         } else {
             (None, None)
         };
@@ -146,15 +136,15 @@
         Ok(Self {
             q_proj: QLinear::from_linear(q_proj),
             k_proj: QLinear::from_linear(k_proj),
             v_proj: QLinear::from_linear(v_proj),
             dense: QLinear::from_linear(dense),
             q_layernorm,
             k_layernorm,
-            rotary_emb,
+            rotary_emb: rope,
             softmax_scale,
             num_heads,
             num_kv_heads,
             head_dim,
             use_flash_attn: cfg.use_flash_attn,
         })
     }
@@ -272,21 +262,32 @@
 struct DecoderLayer {
     self_attn: Attention,
     mlp: MLP,
     input_layernorm: LayerNorm,
 }
 
 impl DecoderLayer {
-    fn new(cfg: &Config, vb: VarBuilder, is_gptx: bool) -> Result<Self> {
-        let self_attn = Attention::new(cfg, vb.pp("self_attn"), is_gptx)?;
-        let mlp = MLP::new(cfg, vb.pp("mlp"))?;
+    fn new(
+        cfg: &Config,
+        vb: VarBuilder,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        rotary_emb: RotaryEmbedding,
+    ) -> Result<Self> {
+        let self_attn = Attention::new(
+            cfg,
+            mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
+            rotary_emb,
+        )?;
+        let mlp = MLP::new(cfg, mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq))?;
         let input_layernorm = layer_norm(
             cfg.hidden_size,
             cfg.layer_norm_eps,
-            vb.pp("input_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
         })
     }
@@ -322,41 +323,64 @@
 
 impl Model {
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
-        let embed_tokens = embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let final_layernorm = layer_norm(
             cfg.hidden_size,
             cfg.layer_norm_eps,
-            vb_m.pp("final_layernorm"),
+            mapper.set_nm_device(vb_m.pp("final_layernorm"), false),
         )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_m = vb_m.pp("layers");
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
+            // Alternative rope scalings are not supported.
+            let rotary_emb = RotaryEmbedding::new_partial(
+                cfg.rope_theta,
+                cfg.head_dim(),
+                (cfg.partial_rotary_factor * cfg.head_dim() as f64) as usize,
+                cfg.max_position_embeddings,
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
+                is_gptx,
+                vb.dtype(),
+            )?;
             let layer = DecoderLayer::new(
                 cfg,
-                mapper.set_device(layer_idx, vb_m.pp(layer_idx)),
-                is_gptx,
+                vb_m.pp(layer_idx),
+                &*mapper,
+                layer_idx,
+                loading_isq,
+                rotary_emb,
             )?;
             layers.push(layer)
         }
-        let lm_head = linear(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let lm_head = linear(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             final_layernorm,
             lm_head: QLinear::from_linear(lm_head),
             cache: Cache::new(cfg.num_hidden_layers, false),
-            device: vb.device().clone(),
+            device: real_device,
             max_seq_len: cfg.max_position_embeddings,
             mapper,
         })
     }
 
     pub fn forward(
         &mut self,
@@ -397,14 +421,15 @@
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
         )
@@ -416,14 +441,15 @@
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
@@ -431,21 +457,21 @@
     }
     fn is_xlora(&self) -> bool {
         false
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(self.lm_head.inner());
-        for layer in &mut self.layers {
-            tensors.push(layer.self_attn.q_proj.inner());
-            tensors.push(layer.self_attn.k_proj.inner());
-            tensors.push(layer.self_attn.v_proj.inner());
-            tensors.push(layer.self_attn.dense.inner());
-            tensors.push(layer.mlp.fc1.inner());
-            tensors.push(layer.mlp.fc2.inner());
+        tensors.push((self.lm_head.inner(), None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((layer.self_attn.q_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.k_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.v_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.dense.inner(), Some(i)));
+            tensors.push((layer.mlp.fc1.inner(), Some(i)));
+            tensors.push((layer.mlp.fc2.inner(), Some(i)));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/phi3.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/phi3.rs`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     pub rms_norm_eps: f64,
     pub rope_theta: f64,
     pub bos_token_id: Option<u32>,
     pub eos_token_id: Option<u32>,
     pub rope_scaling: Option<HashMap<String, Either<Vec<f32>, String>>>,
     pub max_position_embeddings: usize,
     pub use_flash_attn: bool,
+    pub sliding_window: Option<usize>,
     pub original_max_position_embeddings: usize,
 }
 
 impl Config {
     pub fn head_dim(&self) -> usize {
         self.hidden_size / self.num_attention_heads
     }
@@ -48,14 +49,15 @@
     o_proj: QMatMul,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<PhiRotaryEmbedding>,
     use_flash_attn: bool,
+    sliding_window: Option<usize>,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<PhiRotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let head_dim = cfg.head_dim();
@@ -67,23 +69,24 @@
             o_proj: QMatMul::Tensor(o_proj.weight().clone()),
             rotary_emb,
             num_heads,
             num_kv_heads,
             num_kv_groups: num_heads / num_kv_heads,
             head_dim,
             use_flash_attn: cfg.use_flash_attn,
+            sliding_window: cfg.sliding_window,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
-        _start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         kv_cache: &mut Option<(Tensor, Tensor)>,
     ) -> Result<Tensor> {
         let (b_sz, q_len, _) = xs.dims3()?;
 
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
         if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
@@ -108,22 +111,52 @@
         let k = k
             .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
             .transpose(1, 2)?;
         let v = v
             .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
             .transpose(1, 2)?;
 
-        let (q, k) = self.rotary_emb.forward(&q, &k, seqlen_offsets)?;
-
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = Tensor::cat(&[prev_k, &k], 2)?;
-                let v = Tensor::cat(&[prev_v, &v], 2)?;
-                (k, v)
+        let (q, k) = self
+            .rotary_emb
+            .forward(&q, &k, seqlen_offsets, position_ids)?;
+
+        let (k, v, attn_mask) = match kv_cache.clone() {
+            None => (k, v, attention_mask.cloned()),
+            Some((mut prev_k, mut prev_v)) => {
+                let mut mask = attention_mask.cloned();
+                if let Some(sliding_window) = self.sliding_window {
+                    let kv_seq_len = prev_k.dim(2)?;
+                    if kv_seq_len > sliding_window {
+                        prev_k = prev_k.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        prev_v = prev_v.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        if let Some(ref mut mask) = mask {
+                            let mask_len = mask.dim(1)?;
+                            *mask = mask.narrow(
+                                1,
+                                mask_len - (sliding_window - 1),
+                                sliding_window - 1,
+                            )?;
+                            *mask = Tensor::cat(
+                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
+                                D::Minus1,
+                            )?;
+                        }
+                    }
+                }
+                let k = Tensor::cat(&[prev_k, k], 2)?;
+                let v = Tensor::cat(&[prev_v, v], 2)?;
+                (k, v, mask)
             }
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
@@ -134,17 +167,17 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
+            let attn_weights = match attn_mask {
                 None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
+                Some(mask) => attn_weights.broadcast_add(&mask)?,
             };
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
@@ -206,49 +239,59 @@
     self_attn: Attention,
     mlp: Mlp,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
-    fn new(rotary_emb: Arc<PhiRotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
-        let mlp = Mlp::new(cfg, vb.pp("mlp"))?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+    fn new(
+        rotary_emb: Arc<PhiRotaryEmbedding>,
+        cfg: &Config,
+        vb: VarBuilder,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+    ) -> Result<Self> {
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
+        )?;
+        let mlp = Mlp::new(cfg, mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq))?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
             post_attention_layernorm,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         kv_cache: &mut Option<(Tensor, Tensor)>,
     ) -> Result<Tensor> {
         let residual = xs;
         let xs = self.input_layernorm.forward(xs)?;
-        let xs = self.self_attn.forward(
-            &xs,
-            attention_mask,
-            seqlen_offsets,
-            start_offsets_kernel,
-            kv_cache,
-        )?;
+        let xs =
+            self.self_attn
+                .forward(&xs, attention_mask, seqlen_offsets, position_ids, kv_cache)?;
         let xs = (xs + residual)?;
         let residual = &xs;
         let xs = xs.apply(&self.post_attention_layernorm)?.apply(&self.mlp)?;
         residual + xs
     }
 }
 
@@ -259,65 +302,94 @@
     norm: RmsNorm,
     lm_head: QMatMul,
     dtype: DType,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
+    sliding_window: Option<usize>,
 }
 
 impl Model {
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         _is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(PhiRotaryEmbedding::new(
                 vb.dtype(),
                 cfg,
-                mapper.device_for(layer_idx).unwrap_or(vb.device()),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
-            device: vb.device().clone(),
+            device: real_device,
             dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
+            sliding_window: cfg.sliding_window,
         })
     }
 
     fn prepare_decoder_attention_mask(
         &self,
         b_size: usize,
         tgt_len: usize,
         seqlen_offset: usize,
+        sliding_window: Option<usize>,
     ) -> Result<Tensor> {
+        // Sliding window mask
+        let sliding_window = sliding_window.unwrap_or(tgt_len + 1);
         let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| (0..tgt_len).map(move |j| if i < j { f32::NEG_INFINITY } else { 0. }))
+            .flat_map(|i| {
+                (0..tgt_len).map(move |j| {
+                    if i < j || j + sliding_window < i {
+                        f32::NEG_INFINITY
+                    } else {
+                        0.
+                    }
+                })
+            })
             .collect();
         let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
         let mask = if seqlen_offset > 0 {
             let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
             Tensor::cat(&[&mask0, &mask], D::Minus1)?
         } else {
             mask
@@ -342,75 +414,83 @@
         }
     }
 
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         context_lens: Vec<usize>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
         let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
+            let mask = self.prepare_decoder_attention_mask(
+                b_size,
+                seq_len,
+                past_key_values_length,
+                self.sliding_window,
+            )?;
             Some(mask)
         };
+        let position_ids_old = position_ids;
+        let mut position_ids = Vec::new();
+        for p in position_ids_old {
+            position_ids.push(*p + past_key_values_length);
+        }
+
         let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = self.cache.lock();
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
                 seqlen_offsets,
-                start_offsets_kernel.clone(),
+                &position_ids,
                 &mut cache[i],
             )?
         }
+        let xs = xs.to_device(&self.device)?;
         let mut xs = xs.apply(&self.norm)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
         extract_logits(&xs.apply(&self.lm_head)?, context_lens)
     }
 }
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        _start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
+        position_ids: Vec<usize>,
     ) -> Result<Tensor> {
-        self.forward(
-            input_ids,
-            seqlen_offsets,
-            start_offsets_kernel,
-            context_lens,
-        )
+        self.forward(input_ids, seqlen_offsets, &position_ids, context_lens)
     }
     fn xlora_forward(
         &mut self,
         _input_ids: &Tensor,
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
@@ -418,19 +498,19 @@
     }
     fn is_xlora(&self) -> bool {
         false
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(&mut self.lm_head);
-        for layer in &mut self.layers {
-            tensors.push(&mut layer.self_attn.qkv_proj);
-            tensors.push(&mut layer.self_attn.o_proj);
-            tensors.push(&mut layer.mlp.down_proj);
-            tensors.push(&mut layer.mlp.gate_up_proj);
+        tensors.push((&mut self.lm_head, None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((&mut layer.self_attn.qkv_proj, Some(i)));
+            tensors.push((&mut layer.self_attn.o_proj, Some(i)));
+            tensors.push((&mut layer.mlp.gate_up_proj, Some(i)));
+            tensors.push((&mut layer.mlp.down_proj, Some(i)));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/quantized_llama.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/quantized_llama.rs`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,18 @@
         let head_count_kv = md_get("llama.attention.head_count_kv")?.to_u32()? as usize;
         let block_count = md_get("llama.block_count")?.to_u32()? as usize;
         let embedding_length = md_get("llama.embedding_length")?.to_u32()? as usize;
         let rope_dim = md_get("llama.rope.dimension_count")?.to_u32()? as usize;
         // Strangely this value is generally 1e-6 in GGUF file but used to be 1e-5 by default.
         let rms_norm_eps = md_get("llama.attention.layer_norm_rms_epsilon")?.to_f32()?;
 
+        let max_seq_len = md_get("llama.context_length")
+            .and_then(|m| m.to_u64())
+            .unwrap_or(MAX_SEQ_LEN as u64) as usize;
+
         let rope_freq_base = md_get("llama.rope.freq_base")
             .and_then(|m| m.to_f32())
             .unwrap_or(10000f32);
         let head_dim = embedding_length / head_count;
         let tok_embeddings = ct.tensor(reader, "token_embd.weight", device)?;
         let tok_embeddings = tok_embeddings.dequantize(device)?;
         let norm = QRmsNorm::new(
@@ -315,20 +319,20 @@
             rms_norm_eps,
         )?;
         let output = ct.tensor(reader, "output.weight", device)?;
         let mut layers = Vec::with_capacity(block_count);
         let mapper = mapper.into_mapper(block_count, device)?;
         for layer_idx in 0..block_count {
             let prefix = format!("blk.{layer_idx}");
-            let device = mapper.device_for(layer_idx).unwrap_or(device);
+            let device = mapper.device_for(layer_idx, false).unwrap_or(device);
             let rotary = RotaryEmbedding::new_partial(
                 rope_freq_base,
                 head_dim,
                 rope_dim,
-                MAX_SEQ_LEN as usize,
+                max_seq_len,
                 device,
                 false,
                 DType::F32,
             )?;
             let neg_inf = Tensor::new(f32::NEG_INFINITY, device)?;
 
             let attention_wq = ct.tensor(reader, &format!("{prefix}.attn_q.weight"), device)?;
@@ -393,17 +397,15 @@
             tok_embeddings: Embedding::new(tok_embeddings, embedding_length),
             layers,
             norm,
             output: QMatMul::from_qtensor(output)?,
             masks: HashMap::new(),
             device: device.clone(),
             cache: Cache::new(block_count, false),
-            max_seq_len: md_get("llama.context_length")
-                .and_then(|m| m.to_u64())
-                .unwrap_or(MAX_SEQ_LEN as u64) as usize,
+            max_seq_len,
             mapper: Some(mapper),
         })
     }
 
     fn mask(&mut self, t: usize, device: &Device) -> Result<Tensor> {
         if let Some(mask) = self.masks.get(&t) {
             Ok(mask.clone())
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/quantized_phi2.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/quantized_phi2.rs`

 * *Files 2% similar despite different names*

```diff
@@ -132,23 +132,24 @@
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 fn precomput_freqs_cis(
     head_dim: usize,
     freq_base: f32,
     device: &Device,
+    max_seq_len: usize,
 ) -> Result<(Tensor, Tensor)> {
     let theta: Vec<_> = (0..head_dim)
         .step_by(2)
         .map(|i| 1f32 / freq_base.powf(i as f32 / head_dim as f32))
         .collect();
     let theta = Tensor::new(theta.as_slice(), device)?;
-    let idx_theta = Tensor::arange(0, MAX_SEQ_LEN as u32, device)?
+    let idx_theta = Tensor::arange(0, max_seq_len as u32, device)?
         .to_dtype(DType::F32)?
-        .reshape((MAX_SEQ_LEN, 1))?
+        .reshape((max_seq_len, 1))?
         .matmul(&theta.reshape((1, theta.elem_count()))?)?;
     let cos = idx_theta.cos()?;
     let sin = idx_theta.sin()?;
     Ok((cos, sin))
 }
 
 fn layer_norm(w: QTensor, b: QTensor, eps: f64) -> Result<LayerNorm> {
@@ -173,34 +174,33 @@
         // Parameter extraction from metadata.
         let head_count = md_get("phi2.attention.head_count")?.to_u32()? as usize;
         let head_count_kv = md_get("phi2.attention.head_count_kv")?.to_u32()? as usize;
         let block_count = md_get("phi2.block_count")?.to_u32()? as usize;
         let embedding_length = md_get("phi2.embedding_length")?.to_u32()? as usize;
         let rope_dim = md_get("phi2.rope.dimension_count")?.to_u32()? as usize;
         let ln_eps = md_get("phi2.attention.layer_norm_epsilon")?.to_f32()? as f64;
-        let (cos, sin) = precomput_freqs_cis(rope_dim, 10_000., device)?;
-        let neg_inf = Tensor::new(f32::NEG_INFINITY, device)?;
-
         let max_seq_len = md_get("phi2.context_length")
             .and_then(|m| m.to_u64())
             .unwrap_or(MAX_SEQ_LEN as u64) as usize;
+        let (cos, sin) = precomput_freqs_cis(rope_dim, 10_000., device, max_seq_len)?;
+        let neg_inf = Tensor::new(f32::NEG_INFINITY, device)?;
 
         let tok_embeddings = ct.tensor(reader, "token_embd.weight", device)?;
         let tok_embeddings = tok_embeddings.dequantize(device)?;
         let output_norm = layer_norm(
             ct.tensor(reader, "output_norm.weight", device)?,
             ct.tensor(reader, "output_norm.bias", device)?,
             ln_eps,
         )?;
         let output = QLinear::new(&ct, reader, "output", device)?;
         let mut layers = Vec::with_capacity(block_count);
         let mapper = mapper.into_mapper(block_count, device)?;
         for layer_idx in 0..block_count {
             let prefix = format!("blk.{layer_idx}");
-            let device = mapper.device_for(layer_idx).unwrap_or(device);
+            let device = mapper.device_for(layer_idx, false).unwrap_or(device);
 
             let ffn_up = QLinear::new(&ct, reader, &format!("{prefix}.ffn_up"), device)?;
             let ffn_down = QLinear::new(&ct, reader, &format!("{prefix}.ffn_down"), device)?;
             let mlp = Mlp { ffn_up, ffn_down };
             let attn_norm = layer_norm(
                 ct.tensor(reader, &format!("{prefix}.attn_norm.weight"), device)?,
                 ct.tensor(reader, &format!("{prefix}.attn_norm.bias"), device)?,
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/models/qwen2.rs` & `mistralrs-0.1.2/mistralrs-core/src/models/mistral.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
+/// Mistral LLM, https://github.com/mistralai/mistral-src
 use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
-use candle_nn::{linear, linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::layer::QLinear;
+use candle_nn::{linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
 use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
     layers::RmsNorm,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
-#[derive(Debug, Clone, PartialEq, serde::Deserialize)]
+#[derive(Debug, Clone, PartialEq)]
 pub struct Config {
-    pub vocab_size: usize,
-    pub hidden_size: usize,
-    pub intermediate_size: usize,
-    pub num_hidden_layers: usize,
-    pub num_attention_heads: usize,
-    pub num_key_value_heads: usize,
-    pub max_position_embeddings: usize,
-    pub sliding_window: usize,
-    pub max_window_layers: usize,
-    pub tie_word_embeddings: bool,
-    pub rope_theta: f64,
-    pub rms_norm_eps: f64,
-    pub use_sliding_window: bool,
-    pub hidden_act: Activation,
-    pub use_flash_attn: bool,
+    pub(crate) vocab_size: usize,
+    pub(crate) hidden_size: usize,
+    pub(crate) intermediate_size: usize,
+    pub(crate) num_hidden_layers: usize,
+    pub(crate) num_attention_heads: usize,
+    pub(crate) num_key_value_heads: usize,
+    pub(crate) hidden_act: Activation,
+    pub(crate) max_position_embeddings: usize,
+    pub(crate) rms_norm_eps: f64,
+    pub(crate) rope_theta: f64,
+    pub(crate) sliding_window: Option<usize>,
+    pub(crate) use_flash_attn: bool,
 }
 
 #[derive(Debug, Clone)]
 #[allow(clippy::upper_case_acronyms)]
 struct MLP {
     gate_proj: QMatMul,
     up_proj: QMatMul,
@@ -73,48 +70,52 @@
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
 struct Attention {
-    q_proj: QLinear,
-    k_proj: QLinear,
-    v_proj: QLinear,
+    q_proj: QMatMul,
+    k_proj: QMatMul,
+    v_proj: QMatMul,
     o_proj: QMatMul,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
+    hidden_size: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
+    sliding_window: Option<usize>,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let num_kv_groups = num_heads / num_kv_heads;
         let head_dim = hidden_sz / num_heads;
-        let q_proj = linear(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
-        let k_proj = linear(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
-        let v_proj = linear(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
+        let q_proj = linear_no_bias(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
+        let k_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
+        let v_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
         let o_proj = linear_no_bias(num_heads * head_dim, hidden_sz, vb.pp("o_proj"))?;
         Ok(Self {
-            q_proj: QLinear::from_linear(q_proj),
-            k_proj: QLinear::from_linear(k_proj),
-            v_proj: QLinear::from_linear(v_proj),
+            q_proj: QMatMul::Tensor(q_proj.weight().clone()),
+            k_proj: QMatMul::Tensor(k_proj.weight().clone()),
+            v_proj: QMatMul::Tensor(v_proj.weight().clone()),
             o_proj: QMatMul::Tensor(o_proj.weight().clone()),
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
+            hidden_size: hidden_sz,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
+            sliding_window: cfg.sliding_window,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
@@ -122,21 +123,21 @@
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
     ) -> Result<Tensor> {
         let (b_sz, q_len, _) = xs.dims3()?;
 
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
-        if self.q_proj.is_quant() {
+        if matches!(self.q_proj, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
         let mut q = self.q_proj.forward(&xs)?;
         let mut k = self.k_proj.forward(&xs)?;
         let mut v = self.v_proj.forward(&xs)?;
-        if self.q_proj.is_quant() {
+        if matches!(self.q_proj, QMatMul::QTensor(_)) {
             q = q.to_dtype(original_dtype)?;
             k = k.to_dtype(original_dtype)?;
             v = v.to_dtype(original_dtype)?;
         }
 
         let mut q = q.reshape((b_sz * q_len, self.num_heads, self.head_dim))?;
         let mut k = k.reshape((b_sz * q_len, self.num_kv_heads, self.head_dim))?;
@@ -154,20 +155,48 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
+        let (k, v, attn_mask) = match kv_cache.clone() {
+            None => (k, v, attention_mask.cloned()),
+            Some((mut prev_k, mut prev_v)) => {
+                let mut mask = attention_mask.cloned();
+                if let Some(sliding_window) = self.sliding_window {
+                    let kv_seq_len = prev_k.dim(2)?;
+                    if kv_seq_len > sliding_window {
+                        prev_k = prev_k.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        prev_v = prev_v.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        if let Some(ref mut mask) = mask {
+                            let mask_len = mask.dim(1)?;
+                            *mask = mask.narrow(
+                                1,
+                                mask_len - (sliding_window - 1),
+                                sliding_window - 1,
+                            )?;
+                            *mask = Tensor::cat(
+                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
+                                D::Minus1,
+                            )?;
+                        }
+                    }
+                }
+                let k = candle_nn::ops::kvconcat(&prev_k, &k, 2)?;
+                let v = candle_nn::ops::kvconcat(&prev_v, &v, 2)?;
+                (k, v, mask)
             }
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
@@ -178,29 +207,29 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
+            let attn_weights = match attn_mask {
                 None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
+                Some(mask) => attn_weights.broadcast_add(&mask)?,
             };
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
-        if self.q_proj.is_quant() {
+        if matches!(self.q_proj, QMatMul::QTensor(_)) {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
             .transpose(1, 2)?
-            .reshape((b_sz, q_len, ()))?
+            .reshape((b_sz, q_len, self.hidden_size))?
             .apply(&self.o_proj)?;
-        if self.q_proj.is_quant() {
+        if matches!(self.q_proj, QMatMul::QTensor(_)) {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
@@ -208,23 +237,37 @@
     self_attn: Attention,
     mlp: MLP,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
-    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
-        let mlp = MLP::new(cfg, vb.pp("mlp"))?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+    fn new(
+        rotary_emb: Arc<RotaryEmbedding>,
+        cfg: &Config,
+        vb: VarBuilder,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+    ) -> Result<Self> {
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
+        )?;
+        let mlp = MLP::new(cfg, mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq))?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
             post_attention_layernorm,
         })
@@ -256,79 +299,96 @@
 
 #[derive(Debug)]
 pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
-    sliding_window: usize,
+    sliding_window: Option<usize>,
     dtype: DType,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Model {
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
-        let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let head_dim = cfg.hidden_size / cfg.num_attention_heads;
+        let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(RotaryEmbedding::new(
                 cfg.rope_theta as f32,
                 head_dim,
                 cfg.max_position_embeddings,
-                mapper.device_for(layer_idx).unwrap_or(vb.device()),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
                 is_gptx,
                 vb.dtype(),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             sliding_window: cfg.sliding_window,
-            device: vb.device().clone(),
+            device: real_device,
             dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
         })
     }
 
     fn prepare_decoder_attention_mask(
         &self,
         b_size: usize,
         tgt_len: usize,
         seqlen_offset: usize,
     ) -> Result<Tensor> {
-        // Sliding window mask?
+        // Sliding window mask
+        let sliding_window = self.sliding_window.unwrap_or(tgt_len + 1);
         let mask: Vec<_> = (0..tgt_len)
             .flat_map(|i| {
                 (0..tgt_len).map(move |j| {
-                    if i < j || j + self.sliding_window < i {
+                    if i < j || j + sliding_window < i {
                         f32::NEG_INFINITY
                     } else {
                         0.
                     }
                 })
             })
             .collect();
@@ -363,14 +423,18 @@
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
+        if seqlen_offsets.len() > b_size {
+            candle_core::bail!("Expected seqlen offsets have length equal to batch size.")
+        }
+
         let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
             let mask =
                 self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
             Some(mask)
@@ -384,16 +448,17 @@
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
                 seqlen_offsets,
                 start_offsets_kernel.clone(),
                 &mut cache[i],
-            )?
+            )?;
         }
+        let xs = xs.to_device(&self.device)?;
         let mut xs = xs.apply(&self.norm)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
         extract_logits(&xs.apply(&self.lm_head)?, context_lens)
     }
 }
@@ -401,14 +466,15 @@
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
         )
@@ -420,14 +486,15 @@
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
@@ -435,22 +502,22 @@
     }
     fn is_xlora(&self) -> bool {
         false
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(&mut self.lm_head);
-        for layer in &mut self.layers {
-            tensors.push(layer.self_attn.q_proj.inner());
-            tensors.push(layer.self_attn.k_proj.inner());
-            tensors.push(layer.self_attn.v_proj.inner());
-            tensors.push(&mut layer.self_attn.o_proj);
-            tensors.push(&mut layer.mlp.down_proj);
-            tensors.push(&mut layer.mlp.gate_proj);
-            tensors.push(&mut layer.mlp.up_proj);
+        tensors.push((&mut self.lm_head, None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((&mut layer.self_attn.q_proj, Some(i)));
+            tensors.push((&mut layer.self_attn.k_proj, Some(i)));
+            tensors.push((&mut layer.self_attn.v_proj, Some(i)));
+            tensors.push((&mut layer.self_attn.o_proj, Some(i)));
+            tensors.push((&mut layer.mlp.down_proj, Some(i)));
+            tensors.push((&mut layer.mlp.up_proj, Some(i)));
+            tensors.push((&mut layer.mlp.gate_proj, Some(i)));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/pipeline/chat_template.rs` & `mistralrs-0.1.2/mistralrs-core/src/pipeline/chat_template.rs`

 * *Files 16% similar despite different names*

```diff
@@ -81,27 +81,69 @@
         match self.unk_token.as_ref()?.0 {
             Either::Left(ref lit) => Some(lit.clone()),
             Either::Right(ref added) => Some(added.content.clone()),
         }
     }
 }
 
-pub fn calculate_eos_tokens(chat_template: &ChatTemplate, tokenizer: &Tokenizer) -> Vec<u32> {
+pub fn calculate_eos_tokens(
+    chat_template: &ChatTemplate,
+    gen_conf: Option<GenerationConfig>,
+    tokenizer: &Tokenizer,
+) -> Vec<u32> {
     let mut eos_tok_ids = vec![chat_template.eos_tok()];
+    let mut bos_tok_ids = chat_template.bos_tok().map(|b| vec![b]).unwrap_or_default();
 
     for alternate in SUPPORTED_ALTERNATE_EOS {
         if tokenizer.get_vocab(true).get(alternate).is_some() {
             eos_tok_ids.push(alternate.to_string())
         }
     }
 
+    if let Some(gen_conf) = gen_conf {
+        let ids = match gen_conf.eos_token_id {
+            Either::Left(id) => vec![id],
+            Either::Right(ids) => ids,
+        };
+        for id in ids {
+            let s = tokenizer
+                .decode(&[id], false)
+                .unwrap_or_else(|_| panic!("Unable to decode id {id})"));
+            if !eos_tok_ids.contains(&s) {
+                eos_tok_ids.push(s);
+            }
+        }
+
+        let ids = match gen_conf.bos_token_id {
+            Either::Left(id) => vec![id],
+            Either::Right(ids) => ids,
+        };
+        for id in ids {
+            let s = tokenizer
+                .decode(&[id], false)
+                .unwrap_or_else(|_| panic!("Unable to decode id {id})"));
+            if !bos_tok_ids.contains(&s) {
+                bos_tok_ids.push(s);
+            }
+        }
+    }
+
+    let bos_render = bos_tok_ids
+        .iter()
+        .map(|val| format!("{:?}", val))
+        .collect::<Vec<String>>()
+        .join(", ");
+    let eos_render = eos_tok_ids
+        .iter()
+        .map(|val| format!("{:?}", val))
+        .collect::<Vec<String>>()
+        .join(", ");
+
     info!(
-        "bos_tok = {}, eos_tok = {:?}, unk_tok = {}",
-        chat_template.bos_tok().unwrap_or("`None`".to_string()),
-        eos_tok_ids,
+        "bos_toks = {bos_render}, eos_toks = {eos_render}, unk_tok = {}",
         chat_template.unk_tok().unwrap_or("`None`".to_string()),
     );
 
     let mut eos_toks = Vec::new();
     for eos_tok in eos_tok_ids {
         eos_toks.push(
             tokenizer
@@ -110,14 +152,23 @@
                 .copied()
                 .unwrap_or_else(|| panic!("Unable to extract `{eos_tok}` EOS token.")),
         )
     }
     eos_toks
 }
 
+#[allow(dead_code)]
+#[derive(Debug, Deserialize)]
+pub struct GenerationConfig {
+    #[serde(with = "either::serde_untagged")]
+    bos_token_id: Either<u32, Vec<u32>>,
+    #[serde(with = "either::serde_untagged")]
+    eos_token_id: Either<u32, Vec<u32>>,
+}
+
 pub fn apply_chat_template_to(
     messages: Vec<IndexMap<String, String>>,
     add_generation_prompt: bool,
     template: &str,
     bos_tok: Option<String>,
     eos_tok: &str,
     unk_tok: Option<String>,
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/pipeline/ggml.rs` & `mistralrs-0.1.2/mistralrs-core/src/pipeline/ggml.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,89 +2,47 @@
     calculate_inputs, get_model_paths, get_xlora_paths, Loader, ModelInputs, ModelKind, ModelPaths,
     Pipeline, TokenSource, XLoraPaths,
 };
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
 use crate::models::Cache;
 use crate::pipeline::chat_template::calculate_eos_tokens;
-use crate::pipeline::ChatTemplate;
+use crate::pipeline::{ChatTemplate, SimpleModelPaths};
 use crate::utils::varbuilder_utils::from_mmaped_safetensors;
-use crate::xlora_models::{NonGranularState, XLoraConfig};
+use crate::xlora_models::NonGranularState;
 use crate::{deserialize_chat_template, get_paths, DeviceMapMetadata};
 use crate::{
     models::quantized_llama::ModelWeights as QLlama, sequence::Sequence, utils::tokens::get_token,
     xlora_models::XLoraModelWeights as XLoraQLlama,
 };
 use anyhow::Result;
 use candle_core::quantized::{ggml_file, GgmlDType};
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
-use mistralrs_lora::{LoraConfig, Ordering};
+use mistralrs_lora::Ordering;
 use serde_json::Value;
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
 use std::sync::Mutex;
 use tokenizers::Tokenizer;
-use tracing::{info, warn};
+use tracing::info;
 
 enum Model {
     Llama(QLlama),
     XLoraLlama(XLoraQLlama),
 }
 
-pub struct MistralModelPaths<P> {
-    tokenizer_filename: P,
-    config_filename: P,
-    template_filename: P,
-    filenames: Vec<P>,
-    xlora_adapter_filenames: Option<Vec<(String, P)>>,
-    xlora_adapter_configs: Option<Vec<(String, LoraConfig)>>,
-    classifier_path: Option<P>,
-    classifier_config: Option<XLoraConfig>,
-    xlora_ordering: Option<Ordering>,
-}
-
-impl ModelPaths for MistralModelPaths<PathBuf> {
-    fn get_config_filename(&self) -> &PathBuf {
-        &self.config_filename
-    }
-    fn get_tokenizer_filename(&self) -> &PathBuf {
-        &self.tokenizer_filename
-    }
-    fn get_weight_filenames(&self) -> &[PathBuf] {
-        &self.filenames
-    }
-    fn get_adapter_filenames(&self) -> &Option<Vec<(String, PathBuf)>> {
-        &self.xlora_adapter_filenames
-    }
-    fn get_adapter_configs(&self) -> &Option<Vec<(String, LoraConfig)>> {
-        &self.xlora_adapter_configs
-    }
-    fn get_classifier_config(&self) -> &Option<XLoraConfig> {
-        &self.classifier_config
-    }
-    fn get_classifier_path(&self) -> &Option<PathBuf> {
-        &self.classifier_path
-    }
-    fn get_ordering(&self) -> &Option<Ordering> {
-        &self.xlora_ordering
-    }
-    fn get_template_filename(&self) -> &PathBuf {
-        &self.template_filename
-    }
-}
-
 pub struct GGMLPipeline {
     model: Model,
     config: GGMLSpecificConfig,
     tokenizer: Arc<Tokenizer>,
-    tok_trie: TokTrie,
+    tok_trie: Arc<TokTrie>,
     no_kv_cache: bool,
     chat_template: ChatTemplate,
     model_id: String,
     eos_tok: Vec<u32>,
     non_granular_state: Option<NonGranularState>,
     is_lora: bool,
 }
@@ -263,15 +221,15 @@
     fn download_model(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
         silent: bool,
     ) -> Result<Box<dyn ModelPaths>> {
         get_paths!(
-            MistralModelPaths,
+            SimpleModelPaths,
             &token_source,
             revision,
             self,
             self.quantized_model_id,
             self.quantized_filename,
             silent
         )
@@ -281,22 +239,22 @@
         &self,
         paths: &dyn ModelPaths,
         _dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Box<Mutex<dyn Pipeline + Send + Sync>>> {
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         if in_situ_quant.is_some() {
             anyhow::bail!(
                 "You are trying to in-situ quantize a GGUF model. This will not do anything."
             );
         }
         if !mapper.is_dummy() {
-            warn!("GGML models do not support device mapping. Device mapping will not work. Please consider using a GGUF model.");
+            info!("⚠️ WARNING: GGML models do not support device mapping. Device mapping will not work. Please consider using a GGUF model.");
         }
 
         let mut file = std::fs::File::open(paths.get_weight_filenames().first().unwrap())?;
         let model = ggml_file::Content::read(&mut file, device)
             .map_err(|e| e.with_path(paths.get_weight_filenames().first().unwrap()))?;
 
         let mut is_lora = false;
@@ -353,21 +311,21 @@
             }
             _ => unreachable!(),
         };
 
         let tokenizer =
             Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
 
-        let chat_template: ChatTemplate = deserialize_chat_template!(paths, self);
+        let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
-        Ok(Box::new(Mutex::new(GGMLPipeline {
+        Ok(Arc::new(Mutex::new(GGMLPipeline {
             model,
             config: self.config,
-            eos_tok: calculate_eos_tokens(&chat_template, &tokenizer),
-            tok_trie: build_tok_trie(tokenizer.clone()),
+            eos_tok: calculate_eos_tokens(&chat_template, gen_conf, &tokenizer),
+            tok_trie: build_tok_trie(tokenizer.clone()).into(),
             tokenizer: tokenizer.into(),
             no_kv_cache: self.no_kv_cache,
             chat_template,
             model_id: self.model_id.clone(),
             non_granular_state: self.tgt_non_granular_index.map(|tgt_non_granular_index| {
                 NonGranularState {
                     non_granular_index: Arc::new(Mutex::new(0)),
@@ -397,14 +355,15 @@
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full,
             context_lens,
+            position_ids: _, // NOTE(EricLBuehler): ignore, it is for phi3
         } = calculate_inputs(
             input_toks,
             is_prompt,
             self.is_xlora(),
             self.device(),
             self.no_kv_cache,
         )
@@ -473,16 +432,16 @@
     }
     fn get_chat_template(&self) -> &ChatTemplate {
         &self.chat_template
     }
     fn get_non_granular_state(&self) -> &Option<NonGranularState> {
         &None
     }
-    fn tok_trie(&self) -> &TokTrie {
-        &self.tok_trie
+    fn tok_trie(&self) -> Arc<TokTrie> {
+        self.tok_trie.clone()
     }
     fn re_isq_model(&mut self, _dtype: GgmlDType) -> Result<()> {
         anyhow::bail!(
             "You are trying to in-situ requantize a GGUF model. This will not do anything."
         )
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/pipeline/gguf.rs` & `mistralrs-0.1.2/mistralrs-core/src/pipeline/gguf.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,27 @@
     calculate_inputs, get_model_paths, get_xlora_paths, Loader, ModelInputs, ModelKind, ModelPaths,
     Pipeline, TokenSource, XLoraPaths,
 };
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
 use crate::models::Cache;
 use crate::pipeline::chat_template::calculate_eos_tokens;
-use crate::pipeline::ChatTemplate;
+use crate::pipeline::{ChatTemplate, SimpleModelPaths};
 use crate::utils::varbuilder_utils::from_mmaped_safetensors;
-use crate::xlora_models::{NonGranularState, XLoraConfig};
+use crate::xlora_models::NonGranularState;
 use crate::{deserialize_chat_template, get_paths, DeviceMapMetadata};
 use crate::{
     models::quantized_llama::ModelWeights as QLlama, models::quantized_phi2::ModelWeights as QPhi,
     sequence::Sequence, utils::tokens::get_token, xlora_models::XLoraModelWeights as XLoraQLlama,
 };
 use anyhow::{bail, Result};
 use candle_core::quantized::{gguf_file, GgmlDType};
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
-use mistralrs_lora::{LoraConfig, Ordering};
+use mistralrs_lora::Ordering;
 use serde_json::Value;
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
 use std::sync::Mutex;
@@ -31,61 +31,19 @@
 
 enum Model {
     Llama(QLlama),
     Phi2(QPhi),
     XLoraLlama(XLoraQLlama),
 }
 
-pub struct MistralModelPaths<P> {
-    tokenizer_filename: P,
-    config_filename: P,
-    template_filename: P,
-    filenames: Vec<P>,
-    xlora_adapter_filenames: Option<Vec<(String, P)>>,
-    xlora_adapter_configs: Option<Vec<(String, LoraConfig)>>,
-    classifier_path: Option<P>,
-    classifier_config: Option<XLoraConfig>,
-    xlora_ordering: Option<Ordering>,
-}
-
-impl ModelPaths for MistralModelPaths<PathBuf> {
-    fn get_config_filename(&self) -> &PathBuf {
-        &self.config_filename
-    }
-    fn get_tokenizer_filename(&self) -> &PathBuf {
-        &self.tokenizer_filename
-    }
-    fn get_weight_filenames(&self) -> &[PathBuf] {
-        &self.filenames
-    }
-    fn get_adapter_filenames(&self) -> &Option<Vec<(String, PathBuf)>> {
-        &self.xlora_adapter_filenames
-    }
-    fn get_adapter_configs(&self) -> &Option<Vec<(String, LoraConfig)>> {
-        &self.xlora_adapter_configs
-    }
-    fn get_classifier_config(&self) -> &Option<XLoraConfig> {
-        &self.classifier_config
-    }
-    fn get_classifier_path(&self) -> &Option<PathBuf> {
-        &self.classifier_path
-    }
-    fn get_ordering(&self) -> &Option<Ordering> {
-        &self.xlora_ordering
-    }
-    fn get_template_filename(&self) -> &PathBuf {
-        &self.template_filename
-    }
-}
-
 pub struct GGUFPipeline {
     model: Model,
     config: GGUFSpecificConfig,
     tokenizer: Arc<Tokenizer>,
-    tok_trie: TokTrie,
+    tok_trie: Arc<TokTrie>,
     no_kv_cache: bool,
     chat_template: ChatTemplate,
     model_id: String,
     eos_tok: Vec<u32>,
     non_granular_state: Option<NonGranularState>,
     is_lora: bool,
 }
@@ -297,15 +255,15 @@
     fn download_model(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
         silent: bool,
     ) -> Result<Box<dyn ModelPaths>> {
         get_paths!(
-            MistralModelPaths,
+            SimpleModelPaths,
             &token_source,
             revision,
             self,
             self.quantized_model_id,
             self.quantized_filename,
             silent
         )
@@ -315,15 +273,15 @@
         &self,
         paths: &dyn ModelPaths,
         _dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Box<Mutex<dyn Pipeline + Send + Sync>>> {
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         if in_situ_quant.is_some() {
             anyhow::bail!(
                 "You are trying to in-situ quantize a GGUF model. This will not do anything."
             );
         }
         let mut file = std::fs::File::open(paths.get_weight_filenames().first().unwrap())?;
         let model = gguf_file::Content::read(&mut file)
@@ -406,21 +364,21 @@
             }
             _ => unreachable!(),
         };
 
         let tokenizer =
             Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
 
-        let chat_template: ChatTemplate = deserialize_chat_template!(paths, self);
+        let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
-        Ok(Box::new(Mutex::new(GGUFPipeline {
+        Ok(Arc::new(Mutex::new(GGUFPipeline {
             model,
             config: self.config,
-            eos_tok: calculate_eos_tokens(&chat_template, &tokenizer),
-            tok_trie: build_tok_trie(tokenizer.clone()),
+            eos_tok: calculate_eos_tokens(&chat_template, gen_conf, &tokenizer),
+            tok_trie: build_tok_trie(tokenizer.clone()).into(),
             tokenizer: tokenizer.into(),
             no_kv_cache: self.no_kv_cache,
             chat_template,
             model_id: self.model_id.clone(),
             non_granular_state: self.tgt_non_granular_index.map(|tgt_non_granular_index| {
                 NonGranularState {
                     non_granular_index: Arc::new(Mutex::new(0)),
@@ -450,14 +408,15 @@
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full,
             context_lens,
+            position_ids: _, // NOTE(EricLBuehler): ignore, it is for phi3
         } = calculate_inputs(
             input_toks,
             is_prompt,
             self.is_xlora(),
             self.device(),
             self.no_kv_cache,
         )
@@ -530,16 +489,16 @@
     }
     fn get_chat_template(&self) -> &ChatTemplate {
         &self.chat_template
     }
     fn get_non_granular_state(&self) -> &Option<NonGranularState> {
         &None
     }
-    fn tok_trie(&self) -> &TokTrie {
-        &self.tok_trie
+    fn tok_trie(&self) -> Arc<TokTrie> {
+        self.tok_trie.clone()
     }
     fn re_isq_model(&mut self, _dtype: GgmlDType) -> Result<()> {
         anyhow::bail!(
             "You are trying to in-situ requantize a GGML model. This will not do anything."
         )
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/pipeline/loaders.rs` & `mistralrs-0.1.2/mistralrs-core/src/pipeline/loaders.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use std::{collections::HashMap, str::FromStr};
 
 use anyhow::Result;
+use candle_core::Device;
 use candle_nn::{Activation, VarBuilder};
 use either::Either;
 use mistralrs_lora::{LoraConfig, Ordering};
 use pyo3::pyclass;
 use serde::Deserialize;
 
 use super::{NormalModel, NormalModelLoader};
@@ -85,40 +86,48 @@
 impl NormalModelLoader for MistralLoader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(models::mistral::Model::new(
             &MistralBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraMistral::new(
             &MistralBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
 }
 
@@ -175,40 +184,48 @@
 impl NormalModelLoader for GemmaLoader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(models::gemma::Model::new(
             &GemmaBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraGemma::new(
             &GemmaBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
 }
 
@@ -221,14 +238,15 @@
     vocab_size: usize,
     num_hidden_layers: usize,
     num_attention_heads: usize,
     num_key_value_heads: Option<usize>,
     rms_norm_eps: f64,
     #[serde(default = "default_rope")]
     rope_theta: f32,
+    max_position_embeddings: usize,
 }
 
 fn default_rope() -> f32 {
     10_000.0
 }
 
 impl LlamaBasicConfig {
@@ -242,53 +260,62 @@
             num_attention_heads: basic_config.num_attention_heads,
             num_key_value_heads: basic_config
                 .num_key_value_heads
                 .unwrap_or(basic_config.num_attention_heads),
             rms_norm_eps: basic_config.rms_norm_eps,
             rope_theta: basic_config.rope_theta,
             use_flash_attn,
+            max_position_embeddings: basic_config.max_position_embeddings,
         })
     }
 }
 
 pub struct LlamaLoader;
 
 impl NormalModelLoader for LlamaLoader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(models::llama::Llama::new(
             &LlamaBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraLlama::new(
             &LlamaBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
 }
 
@@ -338,40 +365,48 @@
 impl NormalModelLoader for MixtralLoader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(models::mixtral::Model::new(
             &MixtralBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraMixtral::new(
             &MixtralBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
 }
 
@@ -421,40 +456,48 @@
 impl NormalModelLoader for Phi2Loader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(models::phi2::Model::new(
             &Phi2BasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraPhi2::new(
             &Phi2BasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
 }
 
@@ -475,14 +518,15 @@
     rms_norm_eps: f64,
     rope_theta: f64,
     bos_token_id: Option<u32>,
     eos_token_id: Option<u32>,
     rope_scaling: Option<HashMap<String, RopeScaling>>,
     max_position_embeddings: usize,
     original_max_position_embeddings: usize,
+    sliding_window: Option<usize>,
 }
 
 impl Phi3BasicConfig {
     fn deserialize(slice: &str, use_flash_attn: bool) -> Result<models::phi3::Config> {
         let basic_config: Self = serde_json::from_str(slice)?;
         Ok(models::phi3::Config {
             vocab_size: basic_config.vocab_size,
@@ -500,53 +544,62 @@
             rope_scaling: basic_config.rope_scaling.map(|s| {
                 s.into_iter()
                     .map(|(k, v)| (k, v.0))
                     .collect::<HashMap<_, _>>()
             }),
             original_max_position_embeddings: basic_config.original_max_position_embeddings,
             use_flash_attn,
+            sliding_window: basic_config.sliding_window,
         })
     }
 }
 
 pub struct Phi3Loader;
 
 impl NormalModelLoader for Phi3Loader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(models::phi3::Model::new(
             &Phi3BasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraPhi3::new(
             &Phi3BasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
 }
 
@@ -598,31 +651,37 @@
 impl NormalModelLoader for Qwen2Loader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(models::qwen2::Model::new(
             &Qwen2BasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             self.is_gptx(),
             mapper,
+            loading_isq,
+            device,
         )?))
     }
     fn load_xlora(
         &self,
         _config: &str,
         _use_flash_attn: bool,
         _vb: VarBuilder,
         _lora_config: &[(String, LoraConfig)],
         _xlora_config: Option<XLoraConfig>,
         _xlora_ordering: Ordering,
         _mapper: DeviceMapMetadata,
+        _loading_isq: bool,
+        _device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         todo!()
     }
     fn is_gptx(&self) -> bool {
         true
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/pipeline/macros.rs` & `mistralrs-0.1.2/mistralrs-core/src/pipeline/macros.rs`

 * *Files 3% similar despite different names*

```diff
@@ -62,22 +62,26 @@
 macro_rules! deserialize_chat_template {
     ($paths:expr, $this:ident) => {{
         use tracing::info;
 
         let template: ChatTemplate = serde_json::from_str(&fs::read_to_string(
             $paths.get_template_filename(),
         )?).unwrap();
+        let gen_conf: Option<$crate::pipeline::chat_template::GenerationConfig> = $paths.get_gen_conf_filename()
+            .map(|f| serde_json::from_str(&fs::read_to_string(
+                f
+            ).unwrap()).unwrap());
         #[derive(Debug, serde::Deserialize)]
         struct SpecifiedTemplate {
             chat_template: String,
             bos_token: Option<String>,
             eos_token: Option<String>,
         }
         match template.chat_template {
-            Some(_) => template,
+            Some(_) => (template, gen_conf),
             None => {
                 info!("`tokenizer_config.json` does not contain a chat template, attempting to use specified JINJA chat template.");
                 let mut deser: HashMap<String, Value> =
                     serde_json::from_str(&fs::read_to_string($paths.get_template_filename())?)
                         .unwrap();
                 match $this.chat_template.clone() {
                     Some(t) => {
@@ -114,15 +118,15 @@
                         deser.insert(
                             "chat_template".to_string(),
                             Value::Null,
                         );
                     }
                 };
                 let ser = serde_json::to_string_pretty(&deser).expect("Serialization of modified chat template failed.");
-                serde_json::from_str(&ser).unwrap()
+                (serde_json::from_str(&ser).unwrap(), gen_conf)
             }
         }
     }};
 }
 
 #[macro_export]
 macro_rules! get_paths {
@@ -167,48 +171,69 @@
             $this.model_id.clone(),
             &$this.xlora_model_id,
             &$token_source,
             revision.clone(),
             &$this.xlora_order,
         )?;
 
+        let gen_conf = if $crate::api_dir_list!(api, model_id)
+            .collect::<Vec<_>>()
+            .contains(&"generation_config.json".to_string())
+        {
+            Some($crate::api_get_file!(
+                api,
+                "generation_config.json",
+                model_id
+            ))
+        } else {
+            None
+        };
+
         let template_filename = $crate::api_get_file!(api, "tokenizer_config.json", model_id);
 
         Ok(Box::new($path_name {
             tokenizer_filename,
             config_filename,
             filenames,
             xlora_adapter_configs: adapter_configs,
             xlora_adapter_filenames: adapter_safetensors,
             classifier_path,
             classifier_config: xlora_config,
             xlora_ordering: xlora_order,
             template_filename,
+            gen_conf,
         }))
     }};
 }
 
 #[macro_export]
 macro_rules! normal_model_loader {
-    ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr) => {{
+    ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr, $loading_isq:expr, $real_device:expr) => {{
         let vb = from_mmaped_safetensors(
             $paths.get_weight_filenames().to_vec(),
             Vec::new(),
             $dtype.unwrap_or($default_dtype),
             $device,
             $silent,
         )?;
 
-        $loader.load(&$config, $use_flash_attn, vb, $mapper)?
+        $loader.load(
+            &$config,
+            $use_flash_attn,
+            vb,
+            $mapper,
+            $loading_isq,
+            $real_device,
+        )?
     }};
 }
 
 #[macro_export]
 macro_rules! xlora_model_loader {
-    ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr) => {{
+    ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr, $loading_isq:expr, $real_device:expr) => {{
         let mut safetensors_paths = $paths.get_weight_filenames().iter().collect::<Vec<_>>();
         safetensors_paths.push($paths.get_classifier_path().as_ref().unwrap());
         let vb = from_mmaped_safetensors(
             safetensors_paths
                 .iter()
                 .map(|x| (*x).to_owned())
                 .collect::<Vec<_>>(),
@@ -228,21 +253,23 @@
             &$config,
             $use_flash_attn,
             vb,
             $paths.get_adapter_configs().as_ref().unwrap(),
             Some($paths.get_classifier_config().as_ref().unwrap().clone()),
             $paths.get_ordering().as_ref().unwrap().clone(),
             $mapper,
+            $loading_isq,
+            $real_device,
         )?
     }};
 }
 
 #[macro_export]
 macro_rules! lora_model_loader {
-    ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr) => {{
+    ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr, $loading_isq:expr, $real_device:expr) => {{
         let mut safetensors_paths = $paths.get_weight_filenames().iter().collect::<Vec<_>>();
         safetensors_paths.push($paths.get_classifier_path().as_ref().unwrap());
         let vb = from_mmaped_safetensors(
             safetensors_paths
                 .iter()
                 .map(|x| (*x).to_owned())
                 .collect::<Vec<_>>(),
@@ -262,10 +289,12 @@
             &$config,
             $use_flash_attn,
             vb,
             $paths.get_adapter_configs().as_ref().unwrap(),
             None,
             $paths.get_ordering().as_ref().unwrap().clone(),
             $mapper,
+            $loading_isq,
+            $real_device,
         )?
     }};
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/pipeline/mod.rs` & `mistralrs-0.1.2/mistralrs-core/src/pipeline/mod.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 mod chat_template;
 mod ggml;
 mod gguf;
 mod loaders;
 mod macros;
 mod normal;
 use crate::aici::toktree::TokTrie;
+use crate::device_map::DeviceMapper;
 use crate::{api_dir_list, api_get_file, DeviceMapMetadata};
-use crate::{get_bias_if_not_allowed, sampler::Logprobs, sequence::SequenceRecognizer};
 use candle_core::quantized::{GgmlDType, QMatMul, QTensor};
 use candle_nn::VarBuilder;
 use chat_template::{apply_chat_template_to, ChatTemplate};
 use core::fmt;
 use either::Either;
 pub use ggml::{GGMLLoader, GGMLLoaderBuilder, GGMLSpecificConfig};
 pub use gguf::{GGUFLoader, GGUFLoaderBuilder, GGUFSpecificConfig};
 use hf_hub::{
     api::sync::{ApiBuilder, ApiRepo},
     Repo, RepoType,
 };
 use indexmap::IndexMap;
+use indicatif::{ParallelProgressIterator, ProgressBar, ProgressStyle};
 pub use loaders::{
     GemmaLoader, LlamaLoader, MistralLoader, MixtralLoader, NormalLoaderType, Phi2Loader,
     Phi3Loader, Qwen2Loader,
 };
 use mistralrs_lora::{LoraConfig, Ordering};
 pub use normal::{NormalLoader, NormalLoaderBuilder, NormalSpecificConfig};
+use rayon::iter::{IndexedParallelIterator, IntoParallelIterator, ParallelIterator};
 use std::path::Path;
+use std::sync::atomic::AtomicUsize;
 use std::sync::Arc;
 use std::{collections::HashMap, fs, iter::repeat, path::PathBuf, str::FromStr, sync::Mutex};
 use tokenizers::Tokenizer;
-use tqdm::Iter;
-use tracing::{info, warn};
+use tracing::info;
 
 use anyhow::Result;
 use candle_core::{DType, Device, Tensor};
 
 use crate::{
     get_mut_arcmutex,
     models::Cache,
@@ -49,14 +51,61 @@
     fn get_tokenizer_filename(&self) -> &PathBuf;
     fn get_template_filename(&self) -> &PathBuf;
     fn get_adapter_filenames(&self) -> &Option<Vec<(String, PathBuf)>>;
     fn get_adapter_configs(&self) -> &Option<Vec<(String, LoraConfig)>>;
     fn get_classifier_path(&self) -> &Option<PathBuf>;
     fn get_classifier_config(&self) -> &Option<XLoraConfig>;
     fn get_ordering(&self) -> &Option<Ordering>;
+    fn get_gen_conf_filename(&self) -> Option<&PathBuf>;
+}
+
+pub struct SimpleModelPaths<P> {
+    tokenizer_filename: P,
+    config_filename: P,
+    template_filename: P,
+    filenames: Vec<P>,
+    xlora_adapter_filenames: Option<Vec<(String, P)>>,
+    xlora_adapter_configs: Option<Vec<(String, LoraConfig)>>,
+    classifier_path: Option<P>,
+    classifier_config: Option<XLoraConfig>,
+    xlora_ordering: Option<Ordering>,
+    gen_conf: Option<P>,
+}
+
+impl ModelPaths for SimpleModelPaths<PathBuf> {
+    fn get_config_filename(&self) -> &PathBuf {
+        &self.config_filename
+    }
+    fn get_tokenizer_filename(&self) -> &PathBuf {
+        &self.tokenizer_filename
+    }
+    fn get_weight_filenames(&self) -> &[PathBuf] {
+        &self.filenames
+    }
+    fn get_adapter_filenames(&self) -> &Option<Vec<(String, PathBuf)>> {
+        &self.xlora_adapter_filenames
+    }
+    fn get_adapter_configs(&self) -> &Option<Vec<(String, LoraConfig)>> {
+        &self.xlora_adapter_configs
+    }
+    fn get_classifier_config(&self) -> &Option<XLoraConfig> {
+        &self.classifier_config
+    }
+    fn get_classifier_path(&self) -> &Option<PathBuf> {
+        &self.classifier_path
+    }
+    fn get_ordering(&self) -> &Option<Ordering> {
+        &self.xlora_ordering
+    }
+    fn get_template_filename(&self) -> &PathBuf {
+        &self.template_filename
+    }
+    fn get_gen_conf_filename(&self) -> Option<&PathBuf> {
+        self.gen_conf.as_ref()
+    }
 }
 
 #[derive(Debug, Clone)]
 /// The source of the HF token.
 pub enum TokenSource {
     Literal(String),
     EnvVar(String),
@@ -167,29 +216,29 @@
         &self,
         paths: &dyn ModelPaths,
         dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Box<Mutex<dyn Pipeline + Send + Sync>>>;
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>>;
 
     /// If `revision` is None, then it defaults to `main`.
     /// If `dtype` is None, then it defaults to the model default (usually BF16).
     #[allow(clippy::type_complexity, clippy::too_many_arguments)]
     fn load_model(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
         dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Box<Mutex<dyn Pipeline + Send + Sync>>> {
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         let paths = self.download_model(revision, token_source, silent)?;
         self._setup_model(&*paths, dtype, device, silent, mapper, in_situ_quant)
     }
 
     fn get_id(&self) -> &str;
     fn get_kind(&self) -> ModelKind;
 }
@@ -207,15 +256,15 @@
             .map_err(|e| anyhow::Error::msg(e.to_string()))?;
         Ok(encoding.get_ids().to_vec())
     }
     fn device(&self) -> &Device;
     fn num_hidden_layers(&self) -> usize;
     fn cache(&self) -> &Cache;
     fn tokenizer(&self) -> Arc<Tokenizer>;
-    fn tok_trie(&self) -> &TokTrie;
+    fn tok_trie(&self) -> Arc<TokTrie>;
     fn eos_tok(&self) -> &[u32];
     fn name(&self) -> String;
     fn get_max_seq_len(&self) -> usize;
     fn is_xlora(&self) -> bool;
     fn has_no_kv_cache(&self) -> bool;
     fn apply_chat_template(
         &self,
@@ -257,159 +306,143 @@
     fn reset_non_granular_state(&self) {
         if let Some(s) = self.get_non_granular_state().as_ref() {
             *self.cache().get_scalings_cache() = None;
             *get_mut_arcmutex!(s.non_granular_index) = 0;
         }
     }
     fn get_repeat_last_n(&self) -> usize;
-    fn sample(
-        &mut self,
-        logits: Tensor,
-        seq: &mut Sequence,
-        return_logprobs: bool,
-    ) -> Result<Logprobs> {
-        let logits = logits.squeeze(0)?.squeeze(0)?.to_dtype(DType::F32)?;
-        let start_at = seq
-            .get_toks()
-            .len()
-            .saturating_sub(self.get_repeat_last_n());
-        let ctxt = seq.get_toks()[start_at..].to_vec();
-
-        let first_lobprobs_response =
-            seq.sampler()
-                .sample(logits.clone(), Some(&ctxt), return_logprobs)?;
-
-        let bias_if_not_allowed = match &mut seq.recognizer {
-            SequenceRecognizer::Regex(ref mut rx) => {
-                get_bias_if_not_allowed!(self, rx.as_mut(), first_lobprobs_response.token)
-            }
-            SequenceRecognizer::Cfg(ref mut cfg) => {
-                get_bias_if_not_allowed!(self, cfg.as_mut(), first_lobprobs_response.token)
-            }
-            SequenceRecognizer::None => None,
-        };
-        let second_logprobs_response = match bias_if_not_allowed {
-            Some(token_set) => {
-                let mut acc = vec![-f32::INFINITY; self.tok_trie().vocab_size()];
-                token_set.apply_to(&mut acc);
-                let new_logits = (logits + Tensor::from_slice(&acc, acc.len(), self.device())?)?;
-
-                seq.sampler()
-                    .sample(new_logits, Some(&ctxt), return_logprobs)?
-            }
-            None => first_lobprobs_response,
-        };
 
-        match seq.recognizer {
-            SequenceRecognizer::Regex(ref mut rx) => {
-                self.tok_trie()
-                    .append_token(rx.as_mut(), second_logprobs_response.token);
-            }
-            SequenceRecognizer::Cfg(ref mut cfg) => {
-                self.tok_trie()
-                    .append_token(cfg.as_mut(), second_logprobs_response.token);
-            }
-            SequenceRecognizer::None => {}
-        }
-        Ok(second_logprobs_response)
-    }
     fn re_isq_model(&mut self, dtype: GgmlDType) -> Result<()>;
 }
 
 pub trait ConfigMarker {}
 
 pub trait NormalModelLoader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>>;
     #[allow(clippy::too_many_arguments)]
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>>;
     fn is_gptx(&self) -> bool;
 }
 
 pub trait NormalModel {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<usize>,
+        position_ids: Vec<usize>,
     ) -> candle_core::Result<Tensor>;
     #[allow(clippy::too_many_arguments)]
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
         context_lens: Vec<usize>,
+        position_ids: Vec<usize>,
     ) -> candle_core::Result<Tensor>;
     fn is_xlora(&self) -> bool;
     fn device(&self) -> &Device;
     fn cache(&self) -> &Cache;
     fn max_seq_len(&self) -> usize;
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul>;
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper);
     /// Quantize the model in-situ.
-    fn quantize(&mut self, dtype: GgmlDType) -> candle_core::Result<()> {
-        let tensors = self.get_tensors();
+    fn quantize(&mut self, dtype: GgmlDType, device: Device) -> candle_core::Result<()> {
+        let (tensors, mapper) = self.get_tensors();
         let total_tensors = tensors.len();
-        let mut n_quantized = 0;
-        info!("Applying in-situ quantization to {dtype:?}.");
-        for tensor in tensors.into_iter().tqdm() {
-            if let QMatMul::Tensor(t) = tensor {
-                n_quantized += 1;
-                *tensor = QMatMul::QTensor(Arc::new(QTensor::quantize(&*t, dtype)?));
-            }
+        let n_quantized = AtomicUsize::new(0);
+        info!(
+            "Applying in-situ quantization into {dtype:?} to {total_tensors} tensors in parallel."
+        );
+        let bar = ProgressBar::new(total_tensors as u64);
+        bar.set_style(
+            ProgressStyle::default_bar()
+                .template("[{elapsed_precise}] [{bar:40.cyan/blue}] {pos}/{len} ({eta})")
+                .unwrap()
+                .progress_chars("#>-"),
+        );
+
+        let mut devices = Vec::new();
+        for (_, layer) in &tensors {
+            let device = if let Some(layer) = layer {
+                mapper.device_for(*layer, false).unwrap_or(&device)
+            } else {
+                &device
+            };
+            devices.push(device.clone());
         }
-        info!("Applied in-situ quantization into {dtype:?} to {n_quantized} tensors out of {total_tensors} total tensors.");
+
+        tensors
+            .into_par_iter()
+            .zip(devices)
+            .progress_with(bar)
+            .for_each(|((tensor, _), device)| {
+                if let QMatMul::Tensor(t) = tensor {
+                    n_quantized.fetch_add(1, std::sync::atomic::Ordering::Relaxed);
+                    let t = t.to_device(&device).unwrap();
+                    *tensor = QMatMul::QTensor(Arc::new(QTensor::quantize(&t, dtype).unwrap()));
+                }
+            });
+        info!("Applied in-situ quantization into {dtype:?} to {n_quantized:?} tensors out of {total_tensors} total tensors.");
         Ok(())
     }
 }
 
 struct InputMetadata {
     input: Tensor,
     positions: Vec<usize>,
     positions_kernel: Tensor, // [bs, seq len]
     context_lens: Vec<usize>,
+    position_ids: Vec<usize>,
 }
 
 fn get_prompt_input(input_seqs: &[&mut Sequence], device: &Device) -> Result<InputMetadata> {
     let max_len = input_seqs
         .iter()
         .map(|seq| seq.len())
         .max()
         .expect("No sequences");
     let padding_tok = 0;
     // Pad each sequence by the padding token to the max len.
     let mut seqs_tensors = Vec::new();
     let mut seqlen_offsets = Vec::new();
     let mut context_lens = Vec::new();
+    let mut position_ids = Vec::new();
     for seq in input_seqs.iter() {
         let mut ctxt = seq.get_toks().to_vec();
         seqlen_offsets.push(0);
 
         ctxt.extend(repeat(padding_tok).take(max_len.saturating_sub(ctxt.len())));
         context_lens.push(seq.len() - 1);
+        position_ids.push(seq.len());
 
         seqs_tensors.push(Tensor::new(ctxt, device).unwrap().unsqueeze(0).unwrap());
     }
 
     let mut tmp = Vec::new();
     for pos in (0..seqs_tensors.len())
         .map(|_| (0..max_len).map(|x| x as i64).collect::<Vec<_>>())
@@ -419,14 +452,15 @@
     }
     let positions_kernel = Tensor::cat(&tmp, 0)?;
     Ok(InputMetadata {
         input: Tensor::cat(&seqs_tensors, 0).unwrap(),
         positions: seqlen_offsets,
         positions_kernel,
         context_lens,
+        position_ids,
     })
 }
 
 fn get_completion_input(
     input_seqs: &[&mut Sequence],
     device: &Device,
     no_kv_cache: bool,
@@ -434,19 +468,21 @@
     if no_kv_cache {
         return get_prompt_input(input_seqs, device);
     }
     // Pad each sequence by the padding token to the max len.
     let mut seqs_tensors = Vec::new();
     let mut seqlen_offsets = Vec::new();
     let mut context_lens = Vec::new();
+    let mut position_ids = Vec::new();
     for seq in input_seqs.iter() {
         let start_pos = seq.get_toks().len().saturating_sub(1);
         let ctxt = seq.get_toks()[start_pos..].to_vec();
         seqlen_offsets.push(start_pos);
         context_lens.push(0);
+        position_ids.push(seq.len());
 
         seqs_tensors.push(Tensor::new(ctxt, device).unwrap().unsqueeze(0).unwrap());
     }
     let mut tmp = Vec::new();
     for pos in (0..seqs_tensors.len())
         .map(|i| vec![*seqlen_offsets.get(i).unwrap() as i64])
         .collect::<Vec<_>>()
@@ -455,25 +491,27 @@
     }
     let positions_kernel = Tensor::cat(&tmp, 0)?;
     Ok(InputMetadata {
         input: Tensor::cat(&seqs_tensors, 0).unwrap(),
         positions: seqlen_offsets,
         positions_kernel,
         context_lens,
+        position_ids,
     })
 }
 
 struct ModelInputs {
     input_ids: Tensor,
     input_ids_full: Option<Tensor>,
     seqlen_offsets: Vec<usize>,
     seqlen_offsets_full: Option<Vec<usize>>,
     seqlen_offsets_kernel: Tensor,
     seqlen_offsets_kernel_full: Option<Tensor>,
     context_lens: Vec<usize>,
+    position_ids: Vec<usize>,
 }
 
 fn calculate_inputs(
     input_seqs: &[&mut Sequence],
     is_prompt: bool,
     is_xlora: bool,
     device: &Device,
@@ -481,77 +519,86 @@
 ) -> Result<ModelInputs> {
     if is_xlora && !is_prompt {
         let InputMetadata {
             input: input_ids_full,
             positions: seqlen_offsets_full,
             positions_kernel: seqlen_offsets_kernel_full,
             context_lens: _,
+            position_ids,
         } = get_prompt_input(input_seqs, device)?;
         let InputMetadata {
             input: input_ids,
             positions: seqlen_offsets,
             positions_kernel: seqlen_offsets_kernel,
             context_lens,
+            position_ids: _,
         } = get_completion_input(input_seqs, device, no_kv_cache)?;
         Ok(ModelInputs {
             input_ids,
             input_ids_full: Some(input_ids_full),
             seqlen_offsets,
             seqlen_offsets_full: Some(seqlen_offsets_full),
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full: Some(seqlen_offsets_kernel_full),
             context_lens,
+            position_ids,
         })
     } else if is_xlora && is_prompt {
         let InputMetadata {
             input: input_ids,
             positions: seqlen_offsets,
             positions_kernel: seqlen_offsets_kernel,
             context_lens,
+            position_ids,
         } = get_prompt_input(input_seqs, device)?;
         Ok(ModelInputs {
             input_ids: input_ids.clone(),
             input_ids_full: Some(input_ids),
             seqlen_offsets: seqlen_offsets.clone(),
             seqlen_offsets_full: Some(seqlen_offsets),
             seqlen_offsets_kernel: seqlen_offsets_kernel.clone(),
             seqlen_offsets_kernel_full: Some(seqlen_offsets_kernel),
             context_lens,
+            position_ids,
         })
     } else if is_prompt {
         let InputMetadata {
             input: input_ids,
             positions: seqlen_offsets,
             positions_kernel: seqlen_offsets_kernel,
             context_lens,
+            position_ids,
         } = get_prompt_input(input_seqs, device)?;
         Ok(ModelInputs {
             input_ids,
             input_ids_full: None,
             seqlen_offsets,
             seqlen_offsets_full: None,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full: None,
             context_lens,
+            position_ids,
         })
     } else {
         let InputMetadata {
             input: input_ids,
             positions: seqlen_offsets,
             positions_kernel: seqlen_offsets_kernel,
             context_lens,
+            position_ids,
         } = get_completion_input(input_seqs, device, no_kv_cache)?;
         Ok(ModelInputs {
             input_ids,
             input_ids_full: None,
             seqlen_offsets,
             seqlen_offsets_full: None,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full: None,
             context_lens,
+            position_ids,
         })
     }
 }
 
 pub fn extract_logits(logits: &Tensor, context_lens: Vec<usize>) -> candle_core::Result<Tensor> {
     let mut toks = Vec::new();
     for (dim, start) in logits.chunk(logits.dims()[0], 0)?.iter().zip(context_lens) {
@@ -587,44 +634,44 @@
         ));
         let model_id = Path::new(&xlora_id);
 
         let xlora_classifier = &api_dir_list!(api, model_id)
             .filter(|x| x.contains("xlora_classifier.safetensors"))
             .collect::<Vec<_>>();
         if xlora_classifier.len() != 1 {
-            warn!("Detected multiple X-LoRA classifiers: {xlora_classifier:?}");
-            warn!("Selected classifier: `{}`", &xlora_classifier[0]);
+            info!("⚠️ WARNING: Detected multiple X-LoRA classifiers: {xlora_classifier:?}");
+            info!("⚠️ WARNING: Selected classifier: `{}`", &xlora_classifier[0]);
         }
         let xlora_classifier = &xlora_classifier[0];
         let xlora_configs = &api_dir_list!(api, model_id)
             .filter(|x| x.contains("xlora_config.json"))
             .collect::<Vec<_>>();
         if xlora_configs.len() != 1 {
-            warn!("Detected multiple X-LoRA configs: {xlora_configs:?}");
+            info!("⚠️ WARNING: Detected multiple X-LoRA configs: {xlora_configs:?}");
         }
 
         let classifier_path = api_get_file!(api, xlora_classifier, Path::new(""));
 
         let mut xlora_config: Option<XLoraConfig> = None;
         let mut last_err: Option<serde_json::Error> = None;
         for (i, config_path) in xlora_configs.iter().enumerate() {
             if xlora_configs.len() != 1 {
-                warn!("Selecting config: `{}`", config_path);
+                info!("⚠️ WARNING: Selecting config: `{}`", config_path);
             }
             let config_path = api_get_file!(api, config_path, Path::new(""));
             let conf = fs::read_to_string(config_path)?;
             let deser: Result<XLoraConfig, serde_json::Error> = serde_json::from_str(&conf);
             match deser {
                 Ok(conf) => {
                     xlora_config = Some(conf);
                     break;
                 }
                 Err(e) => {
                     if i != xlora_configs.len() - 1 {
-                        warn!("Config is broken with error `{e}`");
+                        info!("⚠️ WARNING: Config is broken with error `{e}`");
                     }
                     last_err = Some(e);
                 }
             }
         }
         let xlora_config = xlora_config.unwrap_or_else(|| {
             panic!(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/pipeline/normal.rs` & `mistralrs-0.1.2/mistralrs-core/src/pipeline/normal.rs`

 * *Files 10% similar despite different names*

```diff
@@ -6,85 +6,43 @@
     calculate_inputs, get_model_paths, get_xlora_paths, Loader, ModelInputs, ModelKind, ModelPaths,
     NormalModel, NormalModelLoader, Pipeline, TokenSource, XLoraPaths,
 };
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
 use crate::models::Cache;
 use crate::pipeline::chat_template::calculate_eos_tokens;
-use crate::pipeline::ChatTemplate;
-use crate::xlora_models::{NonGranularState, XLoraConfig};
+use crate::pipeline::{ChatTemplate, SimpleModelPaths};
+use crate::xlora_models::NonGranularState;
 use crate::{
     deserialize_chat_template, get_paths, lora_model_loader, normal_model_loader,
     xlora_model_loader, DeviceMapMetadata,
 };
 use crate::{
     sequence::Sequence,
     utils::{tokens::get_token, varbuilder_utils::from_mmaped_safetensors},
 };
 use anyhow::Result;
 use candle_core::quantized::GgmlDType;
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
-use mistralrs_lora::{LoraConfig, Ordering};
+use mistralrs_lora::Ordering;
 use serde_json::Value;
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
 use std::sync::Mutex;
 use tokenizers::Tokenizer;
 use tracing::info;
 
-pub struct NormalModelPaths<P> {
-    tokenizer_filename: P,
-    config_filename: P,
-    template_filename: P,
-    filenames: Vec<P>,
-    xlora_adapter_filenames: Option<Vec<(String, P)>>,
-    xlora_adapter_configs: Option<Vec<(String, LoraConfig)>>,
-    classifier_path: Option<P>,
-    classifier_config: Option<XLoraConfig>,
-    xlora_ordering: Option<Ordering>,
-}
-
-impl ModelPaths for NormalModelPaths<PathBuf> {
-    fn get_config_filename(&self) -> &PathBuf {
-        &self.config_filename
-    }
-    fn get_tokenizer_filename(&self) -> &PathBuf {
-        &self.tokenizer_filename
-    }
-    fn get_weight_filenames(&self) -> &[PathBuf] {
-        &self.filenames
-    }
-    fn get_adapter_filenames(&self) -> &Option<Vec<(String, PathBuf)>> {
-        &self.xlora_adapter_filenames
-    }
-    fn get_adapter_configs(&self) -> &Option<Vec<(String, LoraConfig)>> {
-        &self.xlora_adapter_configs
-    }
-    fn get_classifier_config(&self) -> &Option<XLoraConfig> {
-        &self.classifier_config
-    }
-    fn get_classifier_path(&self) -> &Option<PathBuf> {
-        &self.classifier_path
-    }
-    fn get_ordering(&self) -> &Option<Ordering> {
-        &self.xlora_ordering
-    }
-    fn get_template_filename(&self) -> &PathBuf {
-        &self.template_filename
-    }
-}
-
 pub struct NormalPipeline {
     model: Box<dyn NormalModel + Send + Sync>,
     tokenizer: Arc<Tokenizer>,
-    tok_trie: TokTrie,
+    tok_trie: Arc<TokTrie>,
     config: NormalSpecificConfig,
     no_kv_cache: bool,
     chat_template: ChatTemplate,
     non_granular_state: Option<NonGranularState>,
     model_id: String,
     is_lora: bool,
     eos_tok: Vec<u32>,
@@ -226,15 +184,15 @@
     fn download_model(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
         silent: bool,
     ) -> Result<Box<dyn ModelPaths>> {
         get_paths!(
-            NormalModelPaths,
+            SimpleModelPaths,
             &token_source,
             revision,
             self,
             None,
             None,
             silent
         )
@@ -244,83 +202,97 @@
         &self,
         paths: &dyn ModelPaths,
         dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Box<Mutex<dyn Pipeline + Send + Sync>>> {
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         let config = std::fs::read_to_string(paths.get_config_filename())?;
-        let default_dtype = if device.is_cuda() {
+        let default_dtype = if device.is_cuda() && mapper.is_dummy() {
             DType::BF16
+        } else if !mapper.is_dummy() {
+            DType::F16
         } else {
             DType::F32
         };
 
         info!("Model config: {config}");
 
+        let load_device = if in_situ_quant.is_none() {
+            device.clone()
+        } else {
+            Device::Cpu
+        };
+
         let mut is_lora = false;
         let mut model = match self.kind {
             ModelKind::QuantizedGGUF => unreachable!(),
             ModelKind::QuantizedGGML => unreachable!(),
             ModelKind::Normal => normal_model_loader!(
                 paths,
                 dtype,
                 default_dtype,
-                device,
+                &load_device,
                 config,
                 self.inner,
                 self.config.use_flash_attn,
                 silent,
-                mapper
+                mapper,
+                in_situ_quant.is_some(),
+                device.clone()
             ),
             ModelKind::XLoraNormal => xlora_model_loader!(
                 paths,
                 dtype,
                 default_dtype,
-                device,
+                &load_device,
                 config,
                 self.inner,
                 self.config.use_flash_attn,
                 silent,
-                mapper
+                mapper,
+                in_situ_quant.is_some(),
+                device.clone()
             ),
             ModelKind::LoraNormal => {
                 is_lora = true;
                 lora_model_loader!(
                     paths,
                     dtype,
                     default_dtype,
-                    device,
+                    &load_device,
                     config,
                     self.inner,
                     self.config.use_flash_attn,
                     silent,
-                    mapper
+                    mapper,
+                    in_situ_quant.is_some(),
+                    device.clone()
                 )
             }
             ModelKind::XLoraGGUF => unreachable!(),
             ModelKind::XLoraGGML => unreachable!(),
             ModelKind::LoraGGUF => unreachable!(),
             ModelKind::LoraGGML => unreachable!(),
         };
 
         let tokenizer =
             Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
 
-        let chat_template: ChatTemplate = deserialize_chat_template!(paths, self);
+        let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
         if let Some(in_situ_quant) = in_situ_quant {
-            model.quantize(in_situ_quant)?;
+            model.quantize(in_situ_quant, device.clone())?;
         }
 
-        Ok(Box::new(Mutex::new(NormalPipeline {
+        Ok(Arc::new(Mutex::new(NormalPipeline {
             model,
-            eos_tok: calculate_eos_tokens(&chat_template, &tokenizer),
-            tok_trie: build_tok_trie(tokenizer.clone()),
+            eos_tok: calculate_eos_tokens(&chat_template, gen_conf, &tokenizer),
+            tok_trie: build_tok_trie(tokenizer.clone()).into(),
             tokenizer: tokenizer.into(),
             config: self.config,
             no_kv_cache: self.no_kv_cache,
             chat_template,
             non_granular_state: self.tgt_non_granular_index.map(|tgt_non_granular_index| {
                 NonGranularState {
                     non_granular_index: Arc::new(Mutex::new(0)),
@@ -351,39 +323,42 @@
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full,
             context_lens,
+            position_ids,
         } = calculate_inputs(
             input_toks,
             is_prompt,
             self.is_xlora(),
             self.device(),
             self.no_kv_cache,
         )
         .unwrap();
         match self.model.is_xlora() {
             false => self.model.forward(
                 &input_ids,
                 &seqlen_offsets,
                 seqlen_offsets_kernel,
                 context_lens,
+                position_ids,
             ),
             true => self.model.xlora_forward(
                 &input_ids,
                 input_ids_full.as_ref().unwrap_or(&input_ids),
                 &seqlen_offsets,
                 seqlen_offsets_full.as_ref().unwrap_or(&seqlen_offsets),
                 seqlen_offsets_kernel.clone(),
                 seqlen_offsets_kernel_full.unwrap_or(seqlen_offsets_kernel),
                 self.no_kv_cache,
                 &self.non_granular_state,
                 context_lens,
+                position_ids,
             ),
         }
     }
     fn device(&self) -> &Device {
         self.model.device()
     }
     fn num_hidden_layers(&self) -> usize {
@@ -415,14 +390,17 @@
     }
     fn get_chat_template(&self) -> &ChatTemplate {
         &self.chat_template
     }
     fn get_non_granular_state(&self) -> &Option<NonGranularState> {
         &self.non_granular_state
     }
-    fn tok_trie(&self) -> &TokTrie {
-        &self.tok_trie
+    fn tok_trie(&self) -> Arc<TokTrie> {
+        self.tok_trie.clone()
     }
     fn re_isq_model(&mut self, dtype: GgmlDType) -> Result<()> {
-        self.model.quantize(dtype).map_err(anyhow::Error::msg)
+        let device = self.device().clone();
+        self.model
+            .quantize(dtype, device)
+            .map_err(anyhow::Error::msg)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/prefix_cacher.rs` & `mistralrs-0.1.2/mistralrs-core/src/prefix_cacher.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/request.rs` & `mistralrs-0.1.2/mistralrs-core/src/request.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use indexmap::IndexMap;
 
 use crate::{response::Response, sampler::SamplingParams};
-use std::{fmt::Debug, sync::mpsc::Sender};
+use std::fmt::Debug;
+use tokio::sync::mpsc::Sender;
 
 #[derive(Clone)]
 /// Control the constraint with Regex or Yacc.
 pub enum Constraint {
     Regex(String),
     Yacc(String),
     None,
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/response.rs` & `mistralrs-0.1.2/mistralrs-core/src/response.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/sampler.rs` & `mistralrs-0.1.2/mistralrs-core/src/sampler.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-use std::{collections::HashMap, iter::zip, sync::Arc};
+use std::{
+    collections::HashMap,
+    iter::zip,
+    sync::{Arc, Mutex},
+};
 
 use candle_core::{bail, Device, Error, Result, Tensor, D};
 use pyo3::pyclass;
-use rand::{
-    distributions::{Distribution, WeightedIndex},
-    SeedableRng,
-};
+use rand::distributions::{Distribution, WeightedIndex};
+use rand_isaac::Isaac64Rng;
 use serde::{Deserialize, Serialize};
 use tokenizers::Tokenizer;
 
 #[derive(Clone, Debug)]
 /// Stop sequences or ids.
 pub enum StopTokens {
     Seqs(Vec<String>),
     Ids(Vec<u32>),
 }
 
-#[derive(Clone, Debug, Default)]
+#[derive(Clone, Debug)]
 /// Sampling params are used to control sampling.
 pub struct SamplingParams {
     pub temperature: Option<f64>,
     pub top_k: Option<usize>,
     pub top_p: Option<f64>,
     pub top_n_logprobs: usize,
     pub frequency_penalty: Option<f32>,
     pub presence_penalty: Option<f32>,
     pub stop_toks: Option<StopTokens>,
     pub max_len: Option<usize>,
     pub logits_bias: Option<HashMap<u32, f32>>,
     pub n_choices: usize,
 }
 
+impl Default for SamplingParams {
+    fn default() -> Self {
+        Self {
+            temperature: None,
+            top_k: None,
+            top_p: None,
+            top_n_logprobs: 0,
+            frequency_penalty: None,
+            presence_penalty: None,
+            stop_toks: None,
+            max_len: None,
+            logits_bias: None,
+            n_choices: 1,
+        }
+    }
+}
+
 /// Sampler for sampling.
 #[derive(Clone)]
 pub struct Sampler {
-    rng: rand::rngs::StdRng,
     temperature: Option<f64>,
     top_n_logprobs: usize,
     tokenizer: Arc<Tokenizer>,
     frequency_penalty: Option<f32>,
     presence_penalty: Option<f32>,
     logits_bias: Option<Tensor>,
     topk: i64,
@@ -64,15 +82,14 @@
     pub bytes: String,
     pub top_logprobs: Option<Vec<TopLogprob>>,
 }
 
 impl Sampler {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
-        seed: u64,
         temperature: Option<f64>,
         top_n_logprobs: usize,
         tokenizer: Arc<Tokenizer>,
         frequency_penalty: Option<f32>,
         presence_penalty: Option<f32>,
         logits_bias: Option<Tensor>,
         topk: i64,
@@ -80,15 +97,14 @@
     ) -> Self {
         let temperature = if temperature.map_or(true, |v| v < 1e-7) {
             None
         } else {
             temperature
         };
         Self {
-            rng: rand::rngs::StdRng::seed_from_u64(seed),
             temperature,
             top_n_logprobs,
             tokenizer,
             frequency_penalty,
             presence_penalty,
             logits_bias,
             topk,
@@ -118,28 +134,28 @@
             top_n_toks.push(argsort_indices[val]);
         }
 
         let mut bytes = Vec::new();
         for tok in &top_n_toks {
             bytes.push(
                 self.tokenizer
-                    .decode(&[*tok as u32], true)
+                    .decode(&[*tok as u32], false)
                     .map_err(|x| Error::Msg(x.to_string()))?,
             );
         }
         Ok(zip(bytes, zip(top_n_toks, top_n_logprobs))
             .map(|(bytes, (token, logprob))| TopLogprob {
                 token: token as u32,
                 logprob,
                 bytes,
             })
             .collect::<Vec<_>>())
     }
 
-    fn sample_argmax(&mut self, logits: Tensor, return_logprobs: bool) -> Result<Logprobs> {
+    fn sample_argmax(&self, logits: Tensor, return_logprobs: bool) -> Result<Logprobs> {
         let next_token = logits.argmax(D::Minus1)?.to_scalar::<u32>()?;
 
         let probs: Vec<f32> = logits.to_vec1()?;
 
         let argsort_indices = (0..probs.len()).collect::<Vec<_>>();
         let logprob = probs[next_token as usize].log(10.0);
 
@@ -151,52 +167,56 @@
 
         Ok(Logprobs {
             token: next_token,
             logprob,
             top_logprobs,
             bytes: self
                 .tokenizer
-                .decode(&[next_token], true)
+                .decode(&[next_token], false)
                 .map_err(|x| Error::Msg(x.to_string()))?,
         })
     }
 
     fn sample_multinomial(
-        &mut self,
+        &self,
         probs: &mut Vec<f32>,
         argsort_indices: Vec<usize>,
         return_logprobs: bool,
+        rng: Arc<Mutex<Isaac64Rng>>,
     ) -> Result<Logprobs> {
         let distr = WeightedIndex::new(&*probs).map_err(Error::wrap)?;
-        let next_token = distr.sample(&mut self.rng); // "Find the first item which has a weight *higher* than the chosen weight."
+
+        let mut mut_ref_rng = &mut *rng.lock().expect("could not lock rng mutex");
+        let next_token = distr.sample(&mut mut_ref_rng); // "Find the first item which has a weight *higher* than the chosen weight."
         let logprob = probs[next_token].log(10.0);
 
         let top_logprobs = if return_logprobs {
             Some(self.get_top_logprobs(probs, &argsort_indices)?)
         } else {
             None
         };
 
         Ok(Logprobs {
             token: next_token as u32,
             logprob,
             top_logprobs,
             bytes: self
                 .tokenizer
-                .decode(&[next_token.try_into().unwrap()], true)
+                .decode(&[next_token.try_into().unwrap()], false)
                 .map_err(|x| Error::Msg(x.to_string()))?,
         })
     }
 
     fn sample_topkp(
-        &mut self,
+        &self,
         probs: &mut Vec<f32>,
         top_k: i64,
         top_p: f32,
         return_logprobs: bool,
+        rng: Arc<Mutex<Isaac64Rng>>,
     ) -> Result<Logprobs> {
         let mut argsort_indices = (0..probs.len()).collect::<Vec<_>>();
 
         // Sort by descending probability.
         argsort_indices
             .sort_unstable_by(|&i, &j| probs[j].partial_cmp(&probs[i]).expect("No ordering."));
 
@@ -206,15 +226,15 @@
                 if index >= top_k as usize {
                     probs[*val] = 0.0;
                 }
             }
         }
 
         if top_p <= 0.0 || top_p >= 1.0 {
-            return self.sample_multinomial(probs, argsort_indices, return_logprobs);
+            return self.sample_multinomial(probs, argsort_indices, return_logprobs, rng);
         }
         // TOP P
 
         // top-p sampling (or "nucleus sampling") samples from the smallest set of
         // tokens that exceed probability top_p. This way we never sample tokens that
         // have very low probabilities and are less likely to go "off the rails".
 
@@ -225,15 +245,15 @@
                 probs[*index] = 0.0;
             } else {
                 cumsum += probs[*index];
             }
         }
 
         // Sample with clamped probabilities.
-        self.sample_multinomial(probs, argsort_indices, return_logprobs)
+        self.sample_multinomial(probs, argsort_indices, return_logprobs, rng)
     }
 
     fn apply_penalties(&self, mut logits: Vec<f32>, context: Option<&[u32]>) -> Result<Tensor> {
         if self.frequency_penalty.is_some() || self.presence_penalty.is_some() {
             if context.is_none() {
                 bail!("Must specify penalty context.");
             }
@@ -261,31 +281,39 @@
 
     /// Sample the provided tokens.
     ///
     /// If the temperature is `None`, argmax sampling is used. Otherwise, the selected sampling is used.
     /// With `top-p` sampling, if the `top-p` value is `<= 0.0` or `>= 1.0`, multinomial sampling is used.
     /// If `frequency_penalty.is_some()` or `presence_penalty.is_some()`, then `penalty_ctxt` must be provided.
     pub fn sample(
-        &mut self,
+        &self,
         logits: Tensor,
         penalty_ctxt: Option<&[u32]>,
         return_logprobs: bool,
+        rng: Arc<Mutex<Isaac64Rng>>,
     ) -> Result<Logprobs> {
         let logits = self.apply_penalties(logits.to_vec1()?, penalty_ctxt)?;
         let logits = match self.logits_bias {
             Some(ref bias) => (logits + bias)?,
             None => logits,
         };
         let next_token = match self.temperature {
             None => self.sample_argmax(logits, return_logprobs)?,
             Some(temperature) => {
                 let logits = (&logits / temperature)?;
                 let probs = candle_nn::ops::softmax_last_dim(&logits)?;
                 let mut probs: Vec<f32> = probs.to_vec1()?;
-                self.sample_topkp(&mut probs, self.topk, self.topp as f32, return_logprobs)?
+
+                self.sample_topkp(
+                    &mut probs,
+                    self.topk,
+                    self.topp as f32,
+                    return_logprobs,
+                    rng,
+                )?
             }
         };
         Ok(next_token)
     }
 }
 
 mod tests {
@@ -309,27 +337,21 @@
         Tokenizer::from_file(tokenizer_filename).unwrap()
     }
 
     #[test]
     fn test_argmax() {
         use super::Sampler;
         use candle_core::{Device, Tensor};
+        use rand::SeedableRng;
+        use rand_isaac::Isaac64Rng;
+        use std::sync::Arc;
+        use std::sync::Mutex;
 
-        let mut sampler = Sampler::new(
-            0,
-            None,
-            10,
-            get_tokenizer().into(),
-            None,
-            None,
-            None,
-            32,
-            0.1,
-        );
-
+        let sampler = Sampler::new(None, 10, get_tokenizer().into(), None, None, None, 32, 0.1);
         let logits = Tensor::arange(0f32, 1024f32, &Device::Cpu).unwrap();
-        let res = sampler.sample(logits, None, false).unwrap();
+        let rng = Arc::new(Mutex::new(Isaac64Rng::seed_from_u64(42)));
+        let res = sampler.sample(logits, None, false, rng).unwrap();
         assert_eq!(res.token, 1023);
         assert_eq!(res.top_logprobs, None);
         assert_eq!(res.logprob, 1023f64.log(10.) as f32)
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/scheduler.rs` & `mistralrs-0.1.2/mistralrs-core/src/scheduler.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/sequence.rs` & `mistralrs-0.1.2/mistralrs-core/src/sequence.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 use std::{
-    cell::{Cell, RefCell, RefMut},
-    rc::Rc,
-    sync::mpsc::{SendError, Sender},
+    cell::Cell,
+    sync::Arc,
     time::{SystemTime, UNIX_EPOCH},
 };
+use tokio::sync::{
+    mpsc::{error::SendError, Sender},
+    Mutex, MutexGuard,
+};
 
 use crate::{
     aici::{cfg::CfgParser, recognizer::StackRecognizer, rx::RecRx},
     response::CompletionChoice,
     CompletionResponse,
 };
 use crate::{
@@ -62,15 +65,15 @@
 }
 pub struct Sequence {
     // Metadata, const
     id: usize,
     prompt_len: usize,
     max_len: Option<usize>,
     timestamp: u128,
-    sampler: Sampler,
+    sampler: Arc<Sampler>,
     stop_tokens: Vec<u32>,
     stop_strings: Vec<String>,
     return_logprobs: bool,
     responder: Sender<Response>,
     response_index: usize,
     creation_time: u64,
     prefill_prompt_toks: Option<Vec<u32>>,
@@ -89,15 +92,15 @@
     completion_bytes: Vec<u8>,
     stream_idx: usize,
     pub recognizer: SequenceRecognizer,
 
     // GPU things
     pub prompt_tok_per_sec: f32,
     pub prompt_timestamp: Option<u128>,
-    group: Rc<RefCell<SequenceGroup>>,
+    group: Arc<Mutex<SequenceGroup>>,
     state: Cell<SequenceState>,
 }
 impl Sequence {
     #[allow(clippy::too_many_arguments)]
     pub fn new_waiting(
         tokens: Vec<u32>,
         id: usize,
@@ -106,15 +109,15 @@
         responder: Sender<Response>,
         sampler: Sampler,
         stop_tokens: Vec<u32>,
         stop_strings: Vec<String>,
         max_len: Option<usize>,
         return_logprobs: bool,
         is_xlora: bool,
-        group: Rc<RefCell<SequenceGroup>>,
+        group: Arc<Mutex<SequenceGroup>>,
         response_index: usize,
         creation_time: u64,
         recognizer: SequenceRecognizer,
         suffix: Option<String>,
         prefix: Option<String>,
     ) -> Self {
         let prompt_len = tokens.len();
@@ -128,15 +131,15 @@
             cache: vec![None; layers],
             xlora_cache: if is_xlora {
                 Some(vec![None; layers])
             } else {
                 None
             },
             responder,
-            sampler,
+            sampler: sampler.into(),
             stop_tokens,
             stop_strings,
             max_len,
             return_logprobs,
             prompt_tok_per_sec: 0.,
             prompt_timestamp: None,
             group,
@@ -232,16 +235,16 @@
         &mut self.scaling_cache
     }
 
     pub fn is_xlora(&self) -> bool {
         self.xlora_cache.is_some()
     }
 
-    pub fn sampler(&mut self) -> &mut Sampler {
-        &mut self.sampler
+    pub fn sampler(&mut self) -> Arc<Sampler> {
+        self.sampler.clone()
     }
 
     pub fn add_token(
         &mut self,
         tok: Logprobs,
         completion_bytes: Vec<u8>,
         is_done: &Option<StopReason>,
@@ -394,15 +397,15 @@
         self.update_time_info();
     }
 
     pub fn get_response_index(&self) -> usize {
         self.response_index
     }
 
-    pub fn get_mut_group(&self) -> RefMut<'_, SequenceGroup> {
+    pub fn get_mut_group(&self) -> MutexGuard<'_, SequenceGroup> {
         get_mut_group!(self)
     }
 
     pub fn add_streaming_chunk_choice_to_group(&self, chunk: ChunkChoice) {
         get_mut_group!(self).streaming_chunks.push(chunk);
     }
 }
@@ -471,27 +474,27 @@
                 * 1000.,
             total_time_sec: self.total_time as f32 / 1000.,
             total_completion_time_sec: self.total_completion_time as f32 / 1000.,
             total_prompt_time_sec: self.total_prompt_time as f32 / 1000.,
         }
     }
 
-    pub fn maybe_send_done_response(
+    pub async fn maybe_send_done_response(
         &self,
         response: ChatCompletionResponse,
         sender: Sender<Response>,
-    ) {
+    ) -> Result<(), SendError<Response>> {
         if self.choices.len() == self.n_choices {
-            sender
-                .send(Response::Done(response))
-                .expect("Expected receiver.");
+            sender.send(Response::Done(response)).await?;
         }
+
+        Ok(())
     }
 
-    pub fn maybe_send_streaming_response(
+    pub async fn maybe_send_streaming_response(
         &mut self,
         seq: &Sequence,
         model: String,
     ) -> Result<(), Box<SendError<Response>>> {
         if self.streaming_chunks.len() == self.n_choices && self.is_streaming {
             let mut swap_streaming_chunks = vec![];
 
@@ -501,24 +504,24 @@
                 .send(Response::Chunk(ChatCompletionChunkResponse {
                     id: seq.id.to_string(),
                     choices: swap_streaming_chunks,
                     created: seq.timestamp,
                     model: model.clone(),
                     system_fingerprint: SYSTEM_FINGERPRINT.to_string(),
                     object: "chat.completion.chunk".to_string(),
-                }))?;
+                }))
+                .await?;
         }
         Ok(())
     }
 
-    pub fn maybe_send_completion_done_response(
+    pub async fn maybe_send_completion_done_response(
         &self,
         response: CompletionResponse,
         sender: Sender<Response>,
-    ) {
+    ) -> Result<(), Box<SendError<Response>>> {
         if self.completion_choices.len() == self.n_choices {
-            sender
-                .send(Response::CompletionDone(response))
-                .expect("Expected receiver.");
+            sender.send(Response::CompletionDone(response)).await?;
         }
+        Ok(())
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/utils/mod.rs` & `mistralrs-0.1.2/mistralrs-core/src/utils/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ($fallible:expr, $response:expr) => {
         match $fallible {
             Ok(v) => v,
             Err(e) => {
                 use $crate::response::Response;
                 $response
                     .send(Response::InternalError(e.into()))
+                    .await
                     .expect("Expected receiver.");
                 return;
             }
         }
     };
 }
 
@@ -33,73 +34,62 @@
     ($fallible:expr, $response:expr) => {
         match $fallible {
             Ok(v) => v,
             Err(e) => {
                 use $crate::response::Response;
                 $response
                     .send(Response::InternalError(e.into()))
+                    .await
                     .expect("Expected receiver.");
                 return Ok(());
             }
         }
     };
 }
 
 #[macro_export]
-macro_rules! handle_seq_error_stateaware {
-    ($fallible:expr, $seq:expr) => {
-        match $fallible {
-            Ok(v) => v,
-            Err(e) => {
-                use $crate::response::Response;
-                use $crate::sequence::SequenceState;
-                $seq.responder()
-                    .send(Response::InternalError(e.into()))
-                    .expect("Expected receiver.");
-                $seq.set_state(SequenceState::Error);
-                return;
-            }
-        }
-    };
-}
-
-#[macro_export]
 macro_rules! handle_seq_error_stateaware_ok {
     ($fallible:expr, $seq:expr) => {
         match $fallible {
             Ok(v) => v,
             Err(e) => {
                 use $crate::response::Response;
                 use $crate::sequence::SequenceState;
                 $seq.responder()
                     .send(Response::InternalError(e.into()))
+                    .await
                     .expect("Expected receiver.");
                 $seq.set_state(SequenceState::Error);
                 return Ok(());
             }
         }
     };
 }
 
 #[macro_export]
 macro_rules! handle_pipeline_forward_error {
     ($stage: tt, $fallible:expr, $seq_slice:expr, $pipeline:expr, $label:tt, $prefix_cacher:expr) => {
         match $fallible {
             Ok(v) => v,
             Err(e) => {
+                let (tokenizer, pipeline_name) = {
+                    let pipeline = get_mut_arcmutex!($pipeline);
+                    let pipeline_name = pipeline.name();
+                    let tokenizer = pipeline.tokenizer();
+                    (tokenizer, pipeline_name)
+                };
                 use $crate::response::Response;
                 use $crate::sequence::SequenceState;
                 use $crate::Engine;
                 use $crate::response::SYSTEM_FINGERPRINT;
                 use tracing::error;
                 error!("{} - Model failed with error: {:?}", $stage, &e);
                 for seq in $seq_slice.iter_mut() {
                     // Step 1: Add all choices to groups
-                    let res = match $pipeline
-                        .tokenizer()
+                    let res = match tokenizer
                         .decode(&seq.get_toks()[seq.prompt_tokens()..], false)
                     {
                         Ok(v) => v,
                         Err(_) => "".to_string(),
                     };
 
                     if seq.get_mut_group().is_chat {
@@ -128,75 +118,98 @@
                     let group = seq.get_mut_group();
 
                     if group.is_chat {
                         let partial_completion_response = ChatCompletionResponse {
                             id: seq.id().to_string(),
                             choices: group.get_choices().to_vec(),
                             created: seq.creation_time(),
-                            model: $pipeline.name(),
+                            model: pipeline_name.clone(),
                             system_fingerprint: SYSTEM_FINGERPRINT.to_string(),
                             object: "chat.completion".to_string(),
                             usage: group.get_usage(),
                         };
 
                         seq.responder()
                             .send(Response::ModelError(
                                 e.to_string(),
                                 partial_completion_response
                             ))
+                            .await
                             .unwrap();
                     } else {
                         let partial_completion_response = CompletionResponse {
                             id: seq.id().to_string(),
                             choices: group.get_completion_choices().to_vec(),
                             created: seq.creation_time(),
-                            model: $pipeline.name(),
+                            model: pipeline_name.clone(),
                             system_fingerprint: SYSTEM_FINGERPRINT.to_string(),
                             object: "text_completion".to_string(),
                             usage: group.get_usage(),
                         };
 
                         seq.responder()
                             .send(Response::CompletionModelError(
                                 e.to_string(),
                                 partial_completion_response
                             ))
+                            .await
                             .unwrap();
                     }
                 }
                 for seq in $seq_slice.iter_mut() {
                     // Step 3: Set state - This cannot be done in Step 2 as `group` is locking the refcell
                     seq.set_state(SequenceState::Error);
                 }
 
-                Engine::set_none_cache(&mut *$pipeline);
+                Engine::set_none_cache(&mut *get_mut_arcmutex!($pipeline));
                 $prefix_cacher.evict_all_to_cpu().unwrap();
 
                 continue $label;
             }
         }
     };
 }
 
 #[macro_export]
 macro_rules! get_mut_group {
     ($this:expr) => {
         loop {
-            if let Ok(inner) = $this.group.try_borrow_mut() {
+            if let Ok(inner) = $this.group.try_lock() {
                 break inner;
             }
         }
     };
 }
 
 #[macro_export]
 macro_rules! get_bias_if_not_allowed {
-    ($pipeline:expr, $rx:expr, $next_token_id:expr) => {
-        if $pipeline.tok_trie().token_allowed($rx, $next_token_id) {
+    ($tok_trie:expr, $rx:expr, $next_token_id:expr) => {
+        if $tok_trie.token_allowed($rx, $next_token_id) {
             None
         } else {
-            let mut token_set = $pipeline.tok_trie().alloc_token_set();
-            $pipeline.tok_trie().compute_bias($rx, &mut token_set);
+            let mut token_set = $tok_trie.alloc_token_set();
+            $tok_trie.compute_bias($rx, &mut token_set);
             Some(token_set)
         }
     };
 }
+
+#[macro_export]
+macro_rules! sample_async {
+    (
+        $use_async_pool: expr,
+        $sampler: expr,
+        $logits: expr,
+        $ctx: expr,
+        $return_logprobs: expr,
+        $rng: expr
+     ) => {
+        if $use_async_pool {
+            tokio_rayon::spawn(move || {
+                $sampler.sample($logits, Some(&$ctx), $return_logprobs, $rng)
+            })
+            .await?
+        } else {
+            $sampler.sample($logits, Some(&$ctx), $return_logprobs, $rng)?
+        }
+    };
+}
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/utils/tokens.rs` & `mistralrs-0.1.2/mistralrs-core/src/utils/tokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/utils/varbuilder_utils.rs` & `mistralrs-0.1.2/mistralrs-core/src/utils/varbuilder_utils.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/classifier.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/classifier.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/config.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/config.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/gemma.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/gemma.rs`

 * *Files 8% similar despite different names*

```diff
@@ -57,46 +57,53 @@
     gate_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     up_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     down_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     act_fn: candle_nn::Activation,
 }
 
 impl MLP {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let intermediate_sz = cfg.intermediate_size;
         let gate_proj = linear(
             hidden_sz,
             intermediate_sz,
             false,
-            vb.pp("gate_proj"),
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let up_proj = linear(
             hidden_sz,
             intermediate_sz,
             false,
-            vb.pp("up_proj"),
+            mapper.set_device(layer_idx, vb.pp("up_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("up_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let down_proj = linear(
             intermediate_sz,
             hidden_sz,
             false,
-            vb.pp("down_proj"),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             gate_proj,
             up_proj,
@@ -156,60 +163,68 @@
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
 }
 
 impl Attention {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let num_kv_groups = num_heads / num_kv_heads;
         let head_dim = cfg.head_dim;
         let bias = cfg.attention_bias;
         let q_proj = linear(
             hidden_sz,
             num_heads * head_dim,
             bias,
-            vb.pp("q_proj"),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let k_proj = linear(
             hidden_sz,
             num_kv_heads * head_dim,
             bias,
-            vb.pp("k_proj"),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let v_proj = linear(
             hidden_sz,
             num_kv_heads * head_dim,
             bias,
-            vb.pp("v_proj"),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let o_proj = linear(
             num_heads * head_dim,
             hidden_sz,
             bias,
-            vb.pp("o_proj"),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             q_proj,
             k_proj,
@@ -339,31 +354,56 @@
     self_attn: Attention,
     mlp: MLP,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
-        let self_attn =
-            Attention::new(rotary_emb, cfg, vb.pp("self_attn"), lora_config, count, ord)?;
-        let mlp = MLP::new(cfg, vb.pp("mlp"), lora_config, count, ord)?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            vb.pp("self_attn"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let mlp = MLP::new(
+            cfg,
+            vb.pp("mlp"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
             post_attention_layernorm,
         })
@@ -416,46 +456,55 @@
     pub cache: Cache,
     pub max_seq_len: usize,
     xlora_classifier: Option<XLoraClassifier>,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl XLoraModel {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
         let mut count = 0;
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(RotaryEmbedding::new(
                 cfg.rope_theta as f32,
                 cfg.head_dim,
                 cfg.max_position_embeddings,
-                vb.device(),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
                 is_gptx,
                 vb.dtype(),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
         if xlora_config.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
@@ -479,22 +528,26 @@
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.mlp.up_proj)
                     .unwrap()
                     .merge_weights()?;
             }
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
         let lm_head = candle_nn::Linear::new(embed_tokens.embeddings().clone(), None);
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QLinear::from_linear(lm_head),
-            device: vb.device().clone(),
+            device: real_device,
             dtype: vb.dtype(),
             hidden_size: cfg.hidden_size,
             cache: Cache::new(cfg.num_hidden_layers, true),
             max_seq_len: default_max_position_embeddings(),
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
@@ -622,14 +675,15 @@
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
+                &context_lens,
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -685,28 +739,30 @@
 impl NormalModel for XLoraModel {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             start_offsets_kernel,
@@ -724,27 +780,48 @@
     }
     fn is_xlora(&self) -> bool {
         false
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(self.lm_head.inner());
-        for layer in &mut self.layers {
-            tensors.push(Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.gate_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.up_proj).unwrap().inner());
+        tensors.push((self.lm_head.inner(), None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.gate_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.up_proj).unwrap().inner(),
+                Some(i),
+            ));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
 
 impl ScalingsMaker for XLoraModel {
     fn dtype(&self) -> DType {
         self.dtype
     }
@@ -759,14 +836,15 @@
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
+        _context_lens: &[usize],
     ) -> Result<Tensor> {
         self.inner_forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             Some(scalings),
             is_full_pass,
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/llama.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/llama.rs`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
     layers::RmsNorm,
-    models::{
-        self, flash_attn,
-        llama::{Config, MAX_SEQ_LEN},
-        repeat_kv, LayerCaches,
-    },
+    models::{self, flash_attn, llama::Config, repeat_kv, LayerCaches},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
 
 #[derive(Debug, Clone)]
@@ -56,14 +52,15 @@
     v_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_attention_heads: usize,
     num_key_value_heads: usize,
     head_dim: usize,
     use_flash_attn: bool,
     rotary_emb: Arc<RotaryEmbedding>,
+    max_seq_len: usize,
 }
 
 impl CausalSelfAttention {
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &self,
         x: &Tensor,
@@ -127,23 +124,23 @@
                 .contiguous()?;
         }
 
         if let Some((cache_k, cache_v)) = &kv_cache[block_idx] {
             k = candle_nn::ops::kvconcat(cache_k, &k, 2)?.contiguous()?;
             v = candle_nn::ops::kvconcat(cache_v, &v, 2)?.contiguous()?;
             let k_seq_len = k.dims()[1];
-            if k_seq_len > MAX_SEQ_LEN {
+            if k_seq_len > self.max_seq_len {
                 k = k
-                    .narrow(D::Minus1, k_seq_len - MAX_SEQ_LEN, MAX_SEQ_LEN)?
+                    .narrow(D::Minus1, k_seq_len - self.max_seq_len, self.max_seq_len)?
                     .contiguous()?
             }
             let v_seq_len = v.dims()[1];
-            if v_seq_len > 2 * MAX_SEQ_LEN {
+            if v_seq_len > 2 * self.max_seq_len {
                 v = v
-                    .narrow(D::Minus1, v_seq_len - MAX_SEQ_LEN, MAX_SEQ_LEN)?
+                    .narrow(D::Minus1, v_seq_len - self.max_seq_len, self.max_seq_len)?
                     .contiguous()?
             }
         }
         kv_cache[block_idx] = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_attention_heads / self.num_key_value_heads)?.contiguous()?;
         let v = repeat_kv(v, self.num_attention_heads / self.num_key_value_heads)?.contiguous()?;
@@ -181,48 +178,76 @@
         )?;
         if self.q_proj.is_quant() {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 
+    #[allow(clippy::too_many_arguments)]
     fn load(
         vb: VarBuilder,
         cfg: &Config,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
-        is_gptx: bool,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        rope: Arc<RotaryEmbedding>,
     ) -> Result<Self> {
         let size_in = cfg.hidden_size;
         let size_q = (cfg.hidden_size / cfg.num_attention_heads) * cfg.num_attention_heads;
         let size_kv = (cfg.hidden_size / cfg.num_attention_heads) * cfg.num_key_value_heads;
-        let q_proj = linear(size_in, size_q, vb.pp("q_proj"), lora_config, count, ord)?;
-        let k_proj = linear(size_in, size_kv, vb.pp("k_proj"), lora_config, count, ord)?;
-        let v_proj = linear(size_in, size_kv, vb.pp("v_proj"), lora_config, count, ord)?;
-        let o_proj = linear(size_q, size_in, vb.pp("o_proj"), lora_config, count, ord)?;
-        let head_dim = cfg.hidden_size / cfg.num_attention_heads;
-        let rotary_emb = Arc::new(RotaryEmbedding::new(
-            cfg.rope_theta,
-            head_dim,
-            MAX_SEQ_LEN,
-            vb.device(),
-            is_gptx,
-            vb.dtype(),
-        )?);
+        let q_proj = linear(
+            size_in,
+            size_q,
+            mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), false),
+            lora_config,
+            count,
+            ord,
+        )?;
+        let k_proj = linear(
+            size_in,
+            size_kv,
+            mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), false),
+            lora_config,
+            count,
+            ord,
+        )?;
+        let v_proj = linear(
+            size_in,
+            size_kv,
+            mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), false),
+            lora_config,
+            count,
+            ord,
+        )?;
+        let o_proj = linear(
+            size_q,
+            size_in,
+            mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), false),
+            lora_config,
+            count,
+            ord,
+        )?;
         Ok(Self {
             q_proj,
             k_proj,
             v_proj,
             o_proj,
             num_attention_heads: cfg.num_attention_heads,
             num_key_value_heads: cfg.num_key_value_heads,
             head_dim: cfg.hidden_size / cfg.num_attention_heads,
             use_flash_attn: cfg.use_flash_attn,
-            rotary_emb,
+            rotary_emb: rope,
+            max_seq_len: cfg.max_position_embeddings,
         })
     }
 }
 
 fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: f32) -> Result<Tensor> {
     let shape = mask.shape();
     let on_true = Tensor::new(on_true, on_false.device())?.broadcast_as(shape.dims())?;
@@ -269,26 +294,54 @@
         )?;
         if self.c_fc1.is_quant() {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 
+    #[allow(clippy::too_many_arguments)]
     fn load(
         vb: VarBuilder,
         cfg: &Config,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let h_size = cfg.hidden_size;
         let i_size = cfg.intermediate_size;
-        let c_fc1 = linear(h_size, i_size, vb.pp("gate_proj"), lora_config, count, ord)?;
-        let c_fc2 = linear(h_size, i_size, vb.pp("up_proj"), lora_config, count, ord)?;
-        let c_proj = linear(i_size, h_size, vb.pp("down_proj"), lora_config, count, ord)?;
+        let c_fc1 = linear(
+            h_size,
+            i_size,
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), false),
+            lora_config,
+            count,
+            ord,
+        )?;
+        let c_fc2 = linear(
+            h_size,
+            i_size,
+            mapper.set_device(layer_idx, vb.pp("up_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("up_proj"), false),
+            lora_config,
+            count,
+            ord,
+        )?;
+        let c_proj = linear(
+            i_size,
+            h_size,
+            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
+            lora_config,
+            count,
+            ord,
+        )?;
         Ok(Self {
             c_fc1,
             c_fc2,
             c_proj,
         })
     }
 }
@@ -334,30 +387,56 @@
             scalings,
             global_scaling_weight,
             is_scaling_pass,
         )? + residual)?;
         Ok(x)
     }
 
+    #[allow(clippy::too_many_arguments)]
     fn load(
         vb: VarBuilder,
         cfg: &Config,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
-        is_gptx: bool,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        rope: Arc<RotaryEmbedding>,
     ) -> Result<Self> {
-        let attn =
-            CausalSelfAttention::load(vb.pp("self_attn"), cfg, lora_config, count, ord, is_gptx)?;
-        let mlp = Mlp::load(vb.pp("mlp"), cfg, lora_config, count, ord)?;
-        let rms_1 = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+        let attn = CausalSelfAttention::load(
+            vb.pp("self_attn"),
+            cfg,
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+            rope,
+        )?;
+        let mlp = Mlp::load(
+            vb.pp("mlp"),
+            cfg,
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let rms_1 = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let rms_2 = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             rms_1,
             attn,
             rms_2,
             mlp,
         })
@@ -417,15 +496,15 @@
                     .as_ref()
                     .map(|classifier| classifier.get_global_scaling_weight())
                     .unwrap_or(1.0),
                 is_scaling_pass,
             )?;
         }
         let x = x.to_device(&self.device)?;
-        self.ln_f.forward(&x)?.to_dtype(DType::F32)
+        self.ln_f.forward(&x)
     }
 
     #[allow(clippy::too_many_arguments)]
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
@@ -443,14 +522,15 @@
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
+                &context_lens,
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -507,31 +587,59 @@
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
-        let device = vb.device();
         let dtype = vb.dtype();
-        let wte = embedding(cfg.vocab_size, cfg.hidden_size, vb.pp("model.embed_tokens"))?;
-        let lm_head = candle_nn::linear(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
-        let ln_f = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("model.norm"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let wte = embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb.pp("model.embed_tokens"), false),
+        )?;
+        let lm_head = candle_nn::linear(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
+        let ln_f = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb.pp("model.norm"), false),
+        )?;
         let mut count = 0;
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
+        let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let mut blocks: Vec<_> = (0..cfg.num_hidden_layers)
             .map(|i| {
+                let rotary_emb = Arc::new(
+                    RotaryEmbedding::new(
+                        cfg.rope_theta,
+                        head_dim,
+                        cfg.max_position_embeddings,
+                        mapper.device_for(i, false).unwrap_or(&real_device),
+                        is_gptx,
+                        vb.dtype(),
+                    )
+                    .expect("Failed to create RoPE"),
+                );
                 Block::load(
-                    mapper.set_device(i, vb.pp(&format!("model.layers.{i}"))),
+                    vb.pp(&format!("model.layers.{i}")),
                     cfg,
                     lora_config,
                     &mut count,
                     &xlora_ordering,
-                    is_gptx,
+                    &*mapper,
+                    i,
+                    loading_isq,
+                    rotary_emb,
                 )
                 .expect("Failed to load block.")
             })
             .collect();
         if xlora_config.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
@@ -564,15 +672,15 @@
         Ok(Self {
             wte,
             blocks,
             ln_f,
             lm_head: QLinear::from_linear(lm_head),
             cache: Cache::new()?,
             kv_cache: models::Cache::new(cfg.num_hidden_layers, true),
-            device: device.clone(),
+            device: real_device,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             dtype,
             mapper,
         })
     }
@@ -581,28 +689,30 @@
 impl NormalModel for XLoraLlama {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             start_offsets_kernel,
@@ -618,29 +728,44 @@
     fn device(&self) -> &Device {
         &self.device
     }
     fn is_xlora(&self) -> bool {
         true
     }
     fn max_seq_len(&self) -> usize {
-        MAX_SEQ_LEN
+        self.blocks[0].attn.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(self.lm_head.inner());
-        for layer in &mut self.blocks {
-            tensors.push(Arc::get_mut(&mut layer.attn.q_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.attn.k_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.attn.v_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.attn.o_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.c_fc1).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.c_fc2).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.c_proj).unwrap().inner());
+        tensors.push((self.lm_head.inner(), None));
+        for (i, layer) in self.blocks.iter_mut().enumerate() {
+            tensors.push((
+                Arc::get_mut(&mut layer.attn.q_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.attn.k_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.attn.v_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.attn.o_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((Arc::get_mut(&mut layer.mlp.c_fc1).unwrap().inner(), Some(i)));
+            tensors.push((Arc::get_mut(&mut layer.mlp.c_fc2).unwrap().inner(), Some(i)));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.c_proj).unwrap().inner(),
+                Some(i),
+            ));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
 
 impl ScalingsMaker for XLoraLlama {
     fn dtype(&self) -> DType {
         self.dtype
     }
@@ -655,14 +780,15 @@
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
+        _context_lens: &[usize],
     ) -> Result<Tensor> {
         self.inner_forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             Some(scalings),
             is_full_pass,
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/mistral.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/mistral.rs`

 * *Files 14% similar despite different names*

```diff
@@ -24,43 +24,50 @@
     gate_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     up_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     down_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     act_fn: Activation,
 }
 
 impl MLP {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let intermediate_sz = cfg.intermediate_size;
         let gate_proj = linear_no_bias(
             hidden_sz,
             intermediate_sz,
-            vb.pp("gate_proj"),
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let up_proj = linear_no_bias(
             hidden_sz,
             intermediate_sz,
-            vb.pp("up_proj"),
+            mapper.set_device(layer_idx, vb.pp("up_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("up_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let down_proj = linear_no_bias(
             intermediate_sz,
             hidden_sz,
-            vb.pp("down_proj"),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             gate_proj,
             up_proj,
@@ -117,58 +124,67 @@
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
+    sliding_window: Option<usize>,
 }
 
 impl Attention {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let num_kv_groups = num_heads / num_kv_heads;
         let head_dim = hidden_sz / num_heads;
         let q_proj = linear_no_bias(
             hidden_sz,
             num_heads * head_dim,
-            vb.pp("q_proj"),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let k_proj = linear_no_bias(
             hidden_sz,
             num_kv_heads * head_dim,
-            vb.pp("k_proj"),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let v_proj = linear_no_bias(
             hidden_sz,
             num_kv_heads * head_dim,
-            vb.pp("v_proj"),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let o_proj = linear_no_bias(
             num_heads * head_dim,
             hidden_sz,
-            vb.pp("o_proj"),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             q_proj,
             k_proj,
@@ -176,14 +192,15 @@
             o_proj,
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
+            sliding_window: cfg.sliding_window,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &self,
         xs: &Tensor,
@@ -242,20 +259,48 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
+        let (k, v, attn_mask) = match kv_cache.clone() {
+            None => (k, v, attention_mask.cloned()),
+            Some((mut prev_k, mut prev_v)) => {
+                let mut mask = attention_mask.cloned();
+                if let Some(sliding_window) = self.sliding_window {
+                    let kv_seq_len = prev_k.dim(2)?;
+                    if kv_seq_len > sliding_window {
+                        prev_k = prev_k.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        prev_v = prev_v.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        if let Some(ref mut mask) = mask {
+                            let mask_len = mask.dim(1)?;
+                            *mask = mask.narrow(
+                                1,
+                                mask_len - (sliding_window - 1),
+                                sliding_window - 1,
+                            )?;
+                            *mask = Tensor::cat(
+                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
+                                D::Minus1,
+                            )?;
+                        }
+                    }
+                }
+                let k = candle_nn::ops::kvconcat(&prev_k, &k, 2)?;
+                let v = candle_nn::ops::kvconcat(&prev_v, &v, 2)?;
+                (k, v, mask)
             }
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
@@ -266,17 +311,17 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
+            let attn_weights = match attn_mask {
                 None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
+                Some(mask) => attn_weights.broadcast_add(&mask)?,
             };
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
@@ -298,31 +343,56 @@
     self_attn: Attention,
     mlp: MLP,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
-        let self_attn =
-            Attention::new(rotary_emb, cfg, vb.pp("self_attn"), lora_config, count, ord)?;
-        let mlp = MLP::new(cfg, vb.pp("mlp"), lora_config, count, ord)?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            vb.pp("self_attn"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let mlp = MLP::new(
+            cfg,
+            vb.pp("mlp"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
             post_attention_layernorm,
         })
@@ -375,47 +445,56 @@
     pub cache: Cache,
     pub max_seq_len: usize,
     xlora_classifier: Option<XLoraClassifier>,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl XLoraModel {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
         let mut count = 0;
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(RotaryEmbedding::new(
                 cfg.rope_theta as f32,
                 head_dim,
                 cfg.max_position_embeddings,
-                vb.device(),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
                 is_gptx,
                 vb.dtype(),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
         if xlora_config.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
@@ -439,23 +518,31 @@
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.mlp.up_proj)
                     .unwrap()
                     .merge_weights()?;
             }
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = candle_nn::linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = candle_nn::linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QLinear::from_linear(lm_head),
             sliding_window: cfg.sliding_window,
-            device: vb.device().clone(),
+            device: real_device,
             dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, true),
             max_seq_len: cfg.max_position_embeddings,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             mapper,
@@ -591,14 +678,15 @@
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
+                &context_lens,
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -654,28 +742,30 @@
 impl NormalModel for XLoraModel {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             start_offsets_kernel,
@@ -693,27 +783,48 @@
     }
     fn is_xlora(&self) -> bool {
         true
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(self.lm_head.inner());
-        for layer in &mut self.layers {
-            tensors.push(Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.gate_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.up_proj).unwrap().inner());
+        tensors.push((self.lm_head.inner(), None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.gate_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.up_proj).unwrap().inner(),
+                Some(i),
+            ));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
 
 impl ScalingsMaker for XLoraModel {
     fn dtype(&self) -> DType {
         self.dtype
     }
@@ -728,14 +839,15 @@
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
+        _context_lens: &[usize],
     ) -> Result<Tensor> {
         self.inner_forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             Some(scalings),
             is_full_pass,
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/mixtral.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/mixtral.rs`

 * *Files 10% similar despite different names*

```diff
@@ -28,58 +28,67 @@
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
+    sliding_window: Option<usize>,
 }
 
 impl Attention {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let num_kv_groups = num_heads / num_kv_heads;
         let head_dim = hidden_sz / num_heads;
         let q_proj = linear_no_bias(
             hidden_sz,
             num_heads * head_dim,
-            vb.pp("q_proj"),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let k_proj = linear_no_bias(
             hidden_sz,
             num_kv_heads * head_dim,
-            vb.pp("k_proj"),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let v_proj = linear_no_bias(
             hidden_sz,
             num_kv_heads * head_dim,
-            vb.pp("v_proj"),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let o_proj = linear_no_bias(
             num_heads * head_dim,
             hidden_sz,
-            vb.pp("o_proj"),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             q_proj,
             k_proj,
@@ -87,14 +96,15 @@
             o_proj,
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
+            sliding_window: Some(cfg.sliding_window),
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &mut self,
         xs: &Tensor,
@@ -153,20 +163,48 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
+        let (k, v, attn_mask) = match kv_cache.clone() {
+            None => (k, v, attention_mask.cloned()),
+            Some((mut prev_k, mut prev_v)) => {
+                let mut mask = attention_mask.cloned();
+                if let Some(sliding_window) = self.sliding_window {
+                    let kv_seq_len = prev_k.dim(2)?;
+                    if kv_seq_len > sliding_window {
+                        prev_k = prev_k.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        prev_v = prev_v.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        if let Some(ref mut mask) = mask {
+                            let mask_len = mask.dim(1)?;
+                            *mask = mask.narrow(
+                                1,
+                                mask_len - (sliding_window - 1),
+                                sliding_window - 1,
+                            )?;
+                            *mask = Tensor::cat(
+                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
+                                D::Minus1,
+                            )?;
+                        }
+                    }
+                }
+                let k = candle_nn::ops::kvconcat(&prev_k, &k, 2)?;
+                let v = candle_nn::ops::kvconcat(&prev_v, &v, 2)?;
+                (k, v, mask)
             }
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
@@ -177,17 +215,17 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
+            let attn_weights = match attn_mask {
                 None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
+                Some(mask) => attn_weights.broadcast_add(&mask)?,
             };
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
@@ -209,43 +247,50 @@
     w1: Arc<dyn LinearLayerLike + Send + Sync>,
     w2: Arc<dyn LinearLayerLike + Send + Sync>,
     w3: Arc<dyn LinearLayerLike + Send + Sync>,
     act_fn: Activation,
 }
 
 impl BlockSparseTop2MLP {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let intermediate_sz = cfg.intermediate_size;
         let w1 = linear_no_bias(
             hidden_sz,
             intermediate_sz,
-            vb.pp("w1"),
+            mapper.set_device(layer_idx, vb.pp("w1"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("w1"), false),
             lora_config,
             count,
             ord,
         )?;
         let w2 = linear_no_bias(
             intermediate_sz,
             hidden_sz,
-            vb.pp("w2"),
+            mapper.set_device(layer_idx, vb.pp("w2"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("w2"), false),
             lora_config,
             count,
             ord,
         )?;
         let w3 = linear_no_bias(
             hidden_sz,
             intermediate_sz,
-            vb.pp("w3"),
+            mapper.set_device(layer_idx, vb.pp("w3"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("w3"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             w1,
             w2,
@@ -298,33 +343,47 @@
 struct SparseMoeBlock {
     gate: Arc<dyn LinearLayerLike + Send + Sync>,
     experts: Vec<BlockSparseTop2MLP>,
     num_experts_per_tok: usize,
 }
 
 impl SparseMoeBlock {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let gate = linear_no_bias(
             cfg.hidden_size,
             cfg.num_local_experts,
-            vb.pp("gate"),
+            mapper.set_device(layer_idx, vb.pp("gate"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate"), false),
             lora_config,
             count,
             ord,
         )?;
         let mut experts = Vec::with_capacity(cfg.num_local_experts);
         let vb = vb.pp("experts");
         for idx in 0..cfg.num_local_experts {
-            let expert = BlockSparseTop2MLP::new(cfg, vb.pp(idx), lora_config, count, ord)?;
+            let expert = BlockSparseTop2MLP::new(
+                cfg,
+                vb.pp(idx),
+                lora_config,
+                count,
+                ord,
+                mapper,
+                layer_idx,
+                loading_isq,
+            )?;
             experts.push(expert)
         }
         Ok(SparseMoeBlock {
             gate,
             experts,
             num_experts_per_tok: cfg.num_experts_per_tok,
         })
@@ -419,32 +478,56 @@
     self_attn: Attention,
     block_sparse_moe: SparseMoeBlock,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
-        let self_attn =
-            Attention::new(rotary_emb, cfg, vb.pp("self_attn"), lora_config, count, ord)?;
-        let block_sparse_moe =
-            SparseMoeBlock::new(cfg, vb.pp("block_sparse_moe"), lora_config, count, ord)?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            vb.pp("self_attn"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let block_sparse_moe = SparseMoeBlock::new(
+            cfg,
+            vb.pp("block_sparse_moe"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             block_sparse_moe,
             input_layernorm,
             post_attention_layernorm,
         })
@@ -497,47 +580,56 @@
     dtype: DType,
     pub max_seq_len: usize,
     xlora_classifier: Option<XLoraClassifier>,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl XLoraModel {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
         let mut count = 0;
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(RotaryEmbedding::new(
                 cfg.rope_theta as f32,
                 head_dim,
                 cfg.max_position_embeddings,
-                vb.device(),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
                 is_gptx,
                 vb.dtype(),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
         if xlora_config.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
@@ -560,23 +652,31 @@
                 for expert in layer.block_sparse_moe.experts.iter_mut() {
                     Arc::get_mut(&mut expert.w1).unwrap().merge_weights()?;
                     Arc::get_mut(&mut expert.w2).unwrap().merge_weights()?;
                     Arc::get_mut(&mut expert.w3).unwrap().merge_weights()?;
                 }
             }
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = candle_nn::linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = candle_nn::linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             sliding_window: cfg.sliding_window,
-            device: vb.device().clone(),
+            device: real_device,
             dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             mapper,
@@ -704,14 +804,15 @@
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
+                &context_lens,
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -767,28 +868,30 @@
 impl NormalModel for XLoraModel {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             start_offsets_kernel,
@@ -806,34 +909,47 @@
     }
     fn is_xlora(&self) -> bool {
         true
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(&mut self.lm_head);
-        for layer in &mut self.layers {
-            tensors.push(Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner());
-            tensors.push(
+        tensors.push((&mut self.lm_head, None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
                 Arc::get_mut(&mut layer.block_sparse_moe.gate)
                     .unwrap()
                     .inner(),
-            );
+                Some(i),
+            ));
             for expert in &mut layer.block_sparse_moe.experts {
-                tensors.push(Arc::get_mut(&mut expert.w1).unwrap().inner());
-                tensors.push(Arc::get_mut(&mut expert.w2).unwrap().inner());
-                tensors.push(Arc::get_mut(&mut expert.w3).unwrap().inner());
+                tensors.push((Arc::get_mut(&mut expert.w1).unwrap().inner(), Some(i)));
+                tensors.push((Arc::get_mut(&mut expert.w2).unwrap().inner(), Some(i)));
+                tensors.push((Arc::get_mut(&mut expert.w3).unwrap().inner(), Some(i)));
             }
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
 
 impl ScalingsMaker for XLoraModel {
     fn dtype(&self) -> DType {
         self.dtype
     }
@@ -848,14 +964,15 @@
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
+        _context_lens: &[usize],
     ) -> Result<Tensor> {
         self.inner_forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             Some(scalings),
             is_full_pass,
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/mod.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -40,28 +40,30 @@
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
+        context_lens: &[usize],
     ) -> Result<Tensor>;
     fn get_cache(&self) -> &Cache;
 
     #[allow(clippy::too_many_arguments)]
     fn get_scalings(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: &Tensor,
         start_offsets_kernel_full: &Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
+        position_ids: &[usize],
     ) -> Result<Tensor> {
         let (b_size, _) = input_ids_full.dims2()?;
         let (_, seq_len) = input_ids.dims2()?;
 
         if let Some(ref non_granular_state) = non_granular_state {
             if let Some(scalings_cache) = &*self.get_cache().get_scalings_cache() {
                 return Ok(scalings_cache.clone());
@@ -83,14 +85,15 @@
                 input_ids_full,
                 seqlen_offsets_full,
                 start_offsets_kernel_full.clone(),
                 dummy_scalings,
                 true,
                 no_kv_cache,
                 Some(self.get_classifier().config.scaling_pass_value),
+                position_ids,
             )?;
 
             let mut new_cache = Vec::new();
             for _ in 0..self.get_cache().xlora_lock().len() {
                 new_cache.push(Some((
                     Tensor::zeros((1,), DType::U8, &Device::Cpu)?,
                     Tensor::zeros((1,), DType::U8, &Device::Cpu)?,
@@ -104,14 +107,15 @@
                 input_ids,
                 seqlen_offsets,
                 start_offsets_kernel.clone(),
                 dummy_scalings,
                 false,
                 no_kv_cache,
                 Some(self.get_classifier().config.scaling_pass_value),
+                position_ids,
             )?
         };
 
         let scalings = self.get_classifier().forward(hidden_states)?;
         if let Some(ref non_granular_state) = non_granular_state {
             if *get_mut_arcmutex!(non_granular_state.non_granular_index)
                 == non_granular_state.tgt_non_granular_index
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/phi2.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/phi2.rs`

 * *Files 16% similar despite different names*

```diff
@@ -29,33 +29,39 @@
 struct MLP {
     fc1: Arc<dyn LinearLayerLike + Send + Sync>,
     fc2: Arc<dyn LinearLayerLike + Send + Sync>,
     act: Activation,
 }
 
 impl MLP {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let fc1 = linear(
             cfg.hidden_size,
             cfg.intermediate_size,
-            vb.pp("fc1"),
+            mapper.set_device(layer_idx, vb.pp("fc1"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("fc1"), false),
             lora_config,
             count,
             ord,
         )?;
         let fc2 = linear(
             cfg.intermediate_size,
             cfg.hidden_size,
-            vb.pp("fc2"),
+            mapper.set_device(layer_idx, vb.pp("fc2"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("fc2"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             fc1,
             fc2,
@@ -125,67 +131,65 @@
     let shape = mask.shape();
     let on_true = Tensor::new(on_true, on_false.device())?.broadcast_as(shape.dims())?;
     let m = mask.where_cond(&on_true, on_false)?;
     Ok(m)
 }
 
 impl Attention {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
-        is_gptx: bool,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        rope: RotaryEmbedding,
     ) -> Result<Self> {
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads();
         let head_dim = cfg.head_dim();
         let q_proj = linear(
             cfg.hidden_size,
             num_heads * head_dim,
-            vb.pp("q_proj"),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("q_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let k_proj = linear(
             cfg.hidden_size,
             num_kv_heads * head_dim,
-            vb.pp("k_proj"),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("k_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let v_proj = linear(
             cfg.hidden_size,
             num_kv_heads * head_dim,
-            vb.pp("v_proj"),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("v_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let dense = linear(
             num_heads * head_dim,
             cfg.hidden_size,
-            vb.pp("dense"),
+            mapper.set_device(layer_idx, vb.pp("dense"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("dense"), false),
             lora_config,
             count,
             ord,
         )?;
-        // Alternative rope scalings are not supported.
-        let rotary_emb = RotaryEmbedding::new_partial(
-            cfg.rope_theta,
-            cfg.head_dim(),
-            (cfg.partial_rotary_factor * cfg.head_dim() as f64) as usize,
-            cfg.max_position_embeddings,
-            vb.device(),
-            is_gptx,
-            vb.dtype(),
-        )?;
         let (q_layernorm, k_layernorm) = if cfg.qk_layernorm {
             let q_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("q_layernorm"))?;
             let k_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("k_layernorm"))?;
             (Some(q_layernorm), Some(k_layernorm))
         } else {
             (None, None)
         };
@@ -193,15 +197,15 @@
         Ok(Self {
             q_proj,
             k_proj,
             v_proj,
             dense,
             q_layernorm,
             k_layernorm,
-            rotary_emb,
+            rotary_emb: rope,
             softmax_scale,
             num_heads,
             num_kv_heads,
             head_dim,
             use_flash_attn: cfg.use_flash_attn,
         })
     }
@@ -343,28 +347,51 @@
 struct DecoderLayer {
     self_attn: Attention,
     mlp: MLP,
     input_layernorm: LayerNorm,
 }
 
 impl DecoderLayer {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
-        is_gptx: bool,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        rope: RotaryEmbedding,
     ) -> Result<Self> {
-        let self_attn = Attention::new(cfg, vb.pp("self_attn"), lora_config, count, ord, is_gptx)?;
-        let mlp = MLP::new(cfg, vb.pp("mlp"), lora_config, count, ord)?;
+        let self_attn = Attention::new(
+            cfg,
+            vb.pp("self_attn"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+            rope,
+        )?;
+        let mlp = MLP::new(
+            cfg,
+            vb.pp("mlp"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
         let input_layernorm = layer_norm(
             cfg.hidden_size,
             cfg.layer_norm_eps,
-            vb.pp("input_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
         })
     }
@@ -410,42 +437,62 @@
     pub max_seq_len: usize,
     xlora_classifier: Option<XLoraClassifier>,
     dtype: DType,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Model {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
-        let embed_tokens = embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let final_layernorm = layer_norm(
             cfg.hidden_size,
             cfg.layer_norm_eps,
-            vb_m.pp("final_layernorm"),
+            mapper.set_nm_device(vb_m.pp("final_layernorm"), false),
         )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_m = vb_m.pp("layers");
         let mut count = 0;
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         for layer_idx in 0..cfg.num_hidden_layers {
+            // Alternative rope scalings are not supported.
+            let rotary_emb = RotaryEmbedding::new_partial(
+                cfg.rope_theta,
+                cfg.head_dim(),
+                (cfg.partial_rotary_factor * cfg.head_dim() as f64) as usize,
+                cfg.max_position_embeddings,
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
+                is_gptx,
+                vb.dtype(),
+            )?;
             let layer = DecoderLayer::new(
                 cfg,
-                mapper.set_device(layer_idx, vb_m.pp(layer_idx)),
+                vb_m.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
-                is_gptx,
+                &*mapper,
+                layer_idx,
+                loading_isq,
+                rotary_emb,
             )?;
             layers.push(layer)
         }
         if xlora_config.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
@@ -462,22 +509,26 @@
                     .unwrap()
                     .merge_weights()?;
 
                 Arc::get_mut(&mut layer.mlp.fc1).unwrap().merge_weights()?;
                 Arc::get_mut(&mut layer.mlp.fc2).unwrap().merge_weights()?;
             }
         }
-        let lm_head = candle_nn::linear(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let lm_head = candle_nn::linear(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             final_layernorm,
             lm_head: QLinear::from_linear(lm_head),
             cache: Cache::new(cfg.num_hidden_layers, true),
-            device: vb.device().clone(),
+            device: real_device,
             max_seq_len: cfg.max_position_embeddings,
             dtype: vb.dtype(),
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             mapper,
         })
@@ -555,14 +606,15 @@
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
+                &context_lens,
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -618,28 +670,30 @@
 impl NormalModel for Model {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             start_offsets_kernel,
@@ -657,26 +711,38 @@
     }
     fn is_xlora(&self) -> bool {
         true
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(self.lm_head.inner());
-        for layer in &mut self.layers {
-            tensors.push(Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.dense).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.fc1).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.fc2).unwrap().inner());
+        tensors.push((self.lm_head.inner(), None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.dense).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((Arc::get_mut(&mut layer.mlp.fc1).unwrap().inner(), Some(i)));
+            tensors.push((Arc::get_mut(&mut layer.mlp.fc2).unwrap().inner(), Some(i)));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
 
 impl ScalingsMaker for Model {
     fn dtype(&self) -> DType {
         self.dtype
     }
@@ -691,14 +757,15 @@
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
+        _context_lens: &[usize],
     ) -> Result<Tensor> {
         self.inner_forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             Some(scalings),
             is_full_pass,
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/phi3.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/phi3.rs`

 * *Files 17% similar despite different names*

```diff
@@ -27,64 +27,72 @@
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<PhiRotaryEmbedding>,
     use_flash_attn: bool,
+    sliding_window: Option<usize>,
 }
 
 impl Attention {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<PhiRotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let head_dim = cfg.head_dim();
         let op_size = num_heads * head_dim + 2 * num_kv_heads * head_dim;
         let qkv_proj = linear_no_bias(
             cfg.hidden_size,
             op_size,
-            vb.pp("qkv_proj"),
+            mapper.set_device(layer_idx, vb.pp("qkv_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("qkv_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let o_proj = linear_no_bias(
             num_heads * head_dim,
             cfg.hidden_size,
-            vb.pp("o_proj"),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             qkv_proj,
             o_proj,
             rotary_emb,
             num_heads,
             num_kv_heads,
             num_kv_groups: num_heads / num_kv_heads,
             head_dim,
             use_flash_attn: cfg.use_flash_attn,
+            sliding_window: cfg.sliding_window,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
-        _start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let (b_sz, q_len, _) = xs.dims3()?;
 
@@ -117,22 +125,52 @@
         let k = k
             .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
             .transpose(1, 2)?;
         let v = v
             .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
             .transpose(1, 2)?;
 
-        let (q, k) = self.rotary_emb.forward(&q, &k, seqlen_offsets)?;
-
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = Tensor::cat(&[prev_k, &k], 2)?;
-                let v = Tensor::cat(&[prev_v, &v], 2)?;
-                (k, v)
+        let (q, k) = self
+            .rotary_emb
+            .forward(&q, &k, seqlen_offsets, position_ids)?;
+
+        let (k, v, attn_mask) = match kv_cache.clone() {
+            None => (k, v, attention_mask.cloned()),
+            Some((mut prev_k, mut prev_v)) => {
+                let mut mask = attention_mask.cloned();
+                if let Some(sliding_window) = self.sliding_window {
+                    let kv_seq_len = prev_k.dim(2)?;
+                    if kv_seq_len > sliding_window {
+                        prev_k = prev_k.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        prev_v = prev_v.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        if let Some(ref mut mask) = mask {
+                            let mask_len = mask.dim(1)?;
+                            *mask = mask.narrow(
+                                1,
+                                mask_len - (sliding_window - 1),
+                                sliding_window - 1,
+                            )?;
+                            *mask = Tensor::cat(
+                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
+                                D::Minus1,
+                            )?;
+                        }
+                    }
+                }
+                let k = Tensor::cat(&[prev_k, k], 2)?;
+                let v = Tensor::cat(&[prev_v, v], 2)?;
+                (k, v, mask)
             }
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
@@ -143,17 +181,17 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
+            let attn_weights = match attn_mask {
                 None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
+                Some(mask) => attn_weights.broadcast_add(&mask)?,
             };
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if self.qkv_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
@@ -175,35 +213,41 @@
     gate_up_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     down_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     act_fn: candle_nn::Activation,
     i_size: usize,
 }
 
 impl Mlp {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
         let hidden_size = cfg.hidden_size;
         let i_size = cfg.intermediate_size;
         let gate_up_proj = linear_no_bias(
             hidden_size,
             2 * i_size,
-            vb.pp("gate_up_proj"),
+            mapper.set_device(layer_idx, vb.pp("gate_up_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate_up_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         let down_proj = linear_no_bias(
             i_size,
             hidden_size,
-            vb.pp("down_proj"),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
             lora_config,
             count,
             ord,
         )?;
         Ok(Self {
             gate_up_proj,
             down_proj,
@@ -251,31 +295,56 @@
     self_attn: Attention,
     mlp: Mlp,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
+    #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<PhiRotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
     ) -> Result<Self> {
-        let self_attn =
-            Attention::new(rotary_emb, cfg, vb.pp("self_attn"), lora_config, count, ord)?;
-        let mlp = Mlp::new(cfg, vb.pp("mlp"), lora_config, count, ord)?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            vb.pp("self_attn"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let mlp = Mlp::new(
+            cfg,
+            vb.pp("mlp"),
+            lora_config,
+            count,
+            ord,
+            mapper,
+            layer_idx,
+            loading_isq,
+        )?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
             post_attention_layernorm,
         })
@@ -283,27 +352,27 @@
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let residual = xs;
         let xs = self.input_layernorm.forward(xs)?;
         let xs = self.self_attn.forward(
             &xs,
             attention_mask,
             seqlen_offsets,
-            start_offsets_kernel,
+            position_ids,
             kv_cache,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
         let xs = (xs + residual)?;
         let residual = &xs;
@@ -324,46 +393,56 @@
     lm_head: QLinear,
     dtype: DType,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
     xlora_classifier: Option<XLoraClassifier>,
+    sliding_window: Option<usize>,
 }
 
 impl Model {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         lora_config: &[(String, LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         _is_gptx: bool,
         mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, vb.device())?;
         let mut count = 0;
         for layer_idx in 0..cfg.num_hidden_layers {
             let rotary_emb = Arc::new(PhiRotaryEmbedding::new(
                 vb.dtype(),
                 cfg,
-                mapper.device_for(layer_idx).unwrap_or(vb.device()),
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
-                mapper.set_device(layer_idx, vb_l.pp(layer_idx)),
+                vb_l.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
+                &*mapper,
+                layer_idx,
+                loading_isq,
             )?;
             layers.push(layer)
         }
         if xlora_config.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
@@ -378,40 +457,60 @@
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.mlp.gate_up_proj)
                     .unwrap()
                     .merge_weights()?;
             }
         }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = candle_nn::linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = candle_nn::linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QLinear::from_linear(lm_head),
-            device: vb.device().clone(),
+            device: real_device,
             dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, true),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
+            sliding_window: cfg.sliding_window,
         })
     }
 
     fn prepare_decoder_attention_mask(
         &self,
         b_size: usize,
         tgt_len: usize,
         seqlen_offset: usize,
+        sliding_window: Option<usize>,
     ) -> Result<Tensor> {
+        // Sliding window mask
+        let sliding_window = sliding_window.unwrap_or(tgt_len + 1);
         let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| (0..tgt_len).map(move |j| if i < j { f32::NEG_INFINITY } else { 0. }))
+            .flat_map(|i| {
+                (0..tgt_len).map(move |j| {
+                    if i < j || j + sliding_window < i {
+                        f32::NEG_INFINITY
+                    } else {
+                        0.
+                    }
+                })
+            })
             .collect();
         let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
         let mask = if seqlen_offset > 0 {
             let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
             Tensor::cat(&[&mask0, &mask], D::Minus1)?
         } else {
             mask
@@ -437,29 +536,39 @@
     }
 
     #[allow(clippy::too_many_arguments)]
     fn inner_forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         scalings: Option<Tensor>,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
         let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
+            let mask = self.prepare_decoder_attention_mask(
+                b_size,
+                seq_len,
+                past_key_values_length,
+                self.sliding_window,
+            )?;
             Some(mask)
         };
+        let position_ids_old = position_ids;
+        let mut position_ids = Vec::new();
+        for p in position_ids_old {
+            position_ids.push(*p + past_key_values_length);
+        }
+
         let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
@@ -475,24 +584,25 @@
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
                 seqlen_offsets,
-                start_offsets_kernel.clone(),
+                &position_ids,
                 &mut cache[i],
                 scalings.clone(),
                 self.xlora_classifier
                     .as_ref()
                     .map(|classifier| classifier.get_global_scaling_weight())
                     .unwrap_or(1.0),
                 is_scaling_pass,
             )?
         }
+        let xs = xs.to_device(&self.device)?;
         xs.apply(&self.norm)
     }
 
     #[allow(clippy::too_many_arguments)]
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
@@ -500,33 +610,35 @@
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
         context_lens: Vec<usize>,
+        position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
+                &position_ids,
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
-                        start_offsets_kernel_full,
+                        &position_ids,
                         Some(scalings),
                         true,
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
                 if self.lm_head.is_quant() {
@@ -535,15 +647,15 @@
                 extract_logits(&res.apply(&self.lm_head)?, context_lens)
             } else {
                 // is_full_pass=true is ok because no_kv_cache=false
                 let mut res = self
                     .inner_forward(
                         input_ids,
                         seqlen_offsets,
-                        start_offsets_kernel,
+                        &position_ids,
                         Some(scalings),
                         true,
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
                 if self.lm_head.is_quant() {
@@ -552,15 +664,15 @@
                 extract_logits(&res.apply(&self.lm_head)?, context_lens)
             }
         } else {
             let mut res = self
                 .inner_forward(
                     input_ids,
                     seqlen_offsets,
-                    start_offsets_kernel,
+                    &position_ids,
                     None,
                     false,
                     no_kv_cache,
                     None,
                 )?
                 .contiguous()?;
             if self.lm_head.is_quant() {
@@ -574,63 +686,78 @@
 impl NormalModel for Model {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
         _context_lens: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         context_lens: Vec<usize>,
+        position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             start_offsets_kernel,
             start_offsets_kernel_full,
             no_kv_cache,
             non_granular_state,
             context_lens,
+            position_ids,
         )
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
         &self.device
     }
     fn is_xlora(&self) -> bool {
         true
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
-    fn get_tensors(&mut self) -> Vec<&mut QMatMul> {
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push(self.lm_head.inner());
-        for layer in &mut self.layers {
-            tensors.push(Arc::get_mut(&mut layer.self_attn.qkv_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner());
-            tensors.push(Arc::get_mut(&mut layer.mlp.gate_up_proj).unwrap().inner());
+        tensors.push((self.lm_head.inner(), None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.qkv_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.gate_up_proj).unwrap().inner(),
+                Some(i),
+            ));
         }
-        tensors
+        (tensors, &*self.mapper)
     }
 }
 
 impl ScalingsMaker for Model {
     fn dtype(&self) -> DType {
         self.dtype
     }
@@ -640,24 +767,26 @@
     fn get_classifier(&self) -> &XLoraClassifier {
         self.xlora_classifier.as_ref().unwrap()
     }
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        _start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
+        context_lens: &[usize],
     ) -> Result<Tensor> {
+        // NOTE(EricLBuehler): hacky yes, but passing the context lens to start the position ids calculation works
         self.inner_forward(
             input_ids,
             seqlen_offsets,
-            start_offsets_kernel,
+            context_lens,
             Some(scalings),
             is_full_pass,
             no_kv_cache,
             is_scaling_pass,
         )
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-core/src/xlora_models/quantized_llama.rs` & `mistralrs-0.1.2/mistralrs-core/src/xlora_models/quantized_llama.rs`

 * *Files 1% similar despite different names*

```diff
@@ -456,32 +456,36 @@
         let rms_norm_eps = md_get("llama.attention.layer_norm_rms_epsilon")?.to_f32()?;
 
         let rope_freq_base = md_get("llama.rope.freq_base")
             .and_then(|m| m.to_f32())
             .unwrap_or(10000f32);
         let head_dim = embedding_length / head_count;
 
+        let max_seq_len = md_get("llama.context_length")
+            .and_then(|m| m.to_u64())
+            .unwrap_or(MAX_SEQ_LEN as u64) as usize;
+
         let tok_embeddings = ct.tensor(reader, "token_embd.weight", device)?;
         let tok_embeddings = tok_embeddings.dequantize(device)?;
         let norm = QRmsNorm::new(
             ct.tensor(reader, "output_norm.weight", device)?,
             rms_norm_eps,
         )?;
         let output = ct.tensor(reader, "output.weight", device)?;
         let mut layers = Vec::with_capacity(block_count);
         let mut count = 0;
         let mapper = mapper.into_mapper(block_count, device)?;
         for layer_idx in 0..block_count {
             let prefix = format!("blk.{layer_idx}");
-            let device = mapper.device_for(layer_idx).unwrap_or(device);
+            let device = mapper.device_for(layer_idx, false).unwrap_or(device);
             let rotary = RotaryEmbedding::new_partial(
                 rope_freq_base,
                 head_dim,
                 rope_dim,
-                MAX_SEQ_LEN as usize,
+                max_seq_len,
                 device,
                 false,
                 DType::F32,
             )?;
             let neg_inf = Tensor::new(f32::NEG_INFINITY, device)?;
 
             let attention_wq = ct.tensor(reader, &format!("{prefix}.attn_q.weight"), device)?;
@@ -668,17 +672,15 @@
             masks: HashMap::new(),
             device: device.clone(),
             cache: Cache::new(block_count, true),
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb.clone(), true)
                     .unwrap()
             }),
-            max_seq_len: md_get("llama.context_length")
-                .and_then(|m| m.to_u64())
-                .unwrap_or(MAX_SEQ_LEN as u64) as usize,
+            max_seq_len,
             mapper: Some(mapper),
         })
     }
 
     fn mask(&mut self, t: usize, device: &Device) -> Result<Tensor> {
         if let Some(mask) = self.masks.get(&t) {
             Ok(mask.clone())
@@ -783,14 +785,15 @@
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
+                &context_lens,
             )?;
 
             if no_kv_cache {
                 extract_logits(
                     &self
                         .inner_forward(
                             input_ids_full,
@@ -858,14 +861,15 @@
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
+        _context_lens: &[usize],
     ) -> Result<Tensor> {
         self.inner_forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             Some(scalings),
             is_full_pass,
```

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/Cargo.toml` & `mistralrs-0.1.2/mistralrs-pyo3/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.1", path = "../mistralrs-core" }
+mistralrs-core = { version = "0.1.2", path = "../mistralrs-core" }
 serde.workspace = true
 serde_json.workspace = true
 candle-core.workspace = true
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
 futures.workspace = true
+tokio.workspace = true
+tracing-subscriber.workspace = true
 
 [features]
 cuda = ["candle-core/cuda", "mistralrs-core/cuda"]
 cudnn = ["candle-core/cudnn", "mistralrs-core/cudnn"]
 metal = ["candle-core/metal", "mistralrs-core/metal"]
 flash-attn = ["cuda", "mistralrs-core/flash-attn"]
 accelerate = ["mistralrs-core/accelerate"]
```

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/.gitignore` & `mistralrs-0.1.2/mistralrs-pyo3/.gitignore`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/API.md` & `mistralrs-0.1.2/mistralrs-pyo3/API.md`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/Cargo_template.toml` & `mistralrs-0.1.2/mistralrs-pyo3/Cargo_template.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.1", path = "../mistralrs-core", features=["$feature_name"] }
+mistralrs-core = { version = "0.1.2", path = "../mistralrs-core", features=["$feature_name"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["$feature_name"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
 futures.workspace = true
+tracing-subscriber.workspace = true
```

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/README.md` & `mistralrs-0.1.2/mistralrs-pyo3/README.md`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/mistralrs.pyi` & `mistralrs-0.1.2/mistralrs-pyo3/mistralrs.pyi`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/pyproject_template.toml` & `mistralrs-0.1.2/mistralrs-pyo3/pyproject_template.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "$name"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/src/lib.rs` & `mistralrs-0.1.2/mistralrs-pyo3/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 use indexmap::IndexMap;
 use message::{Message, Role};
 use std::{
     cell::RefCell,
     collections::HashMap,
     fmt::Debug,
     str::FromStr,
-    sync::{mpsc::channel, Arc, Mutex},
+    sync::{Arc, Mutex},
 };
 use stream::ChatCompletionStreamer;
+use tokio::sync::mpsc::channel;
+use tracing_subscriber::{filter::LevelFilter, EnvFilter};
 
 use candle_core::Device;
 use mistralrs_core::{
     ChatCompletionResponse, CompletionResponse, Constraint, DeviceMapMetadata, GGMLLoaderBuilder,
     GGMLSpecificConfig, GGUFLoaderBuilder, GGUFSpecificConfig, Loader, MistralRs, MistralRsBuilder,
     NormalLoaderBuilder, NormalSpecificConfig, Request as _Request, RequestMessage, Response,
     SamplingParams, SchedulerMethod, StopTokens, TokenSource,
@@ -59,16 +61,16 @@
 
 fn parse_isq(s: &str) -> std::result::Result<GgmlDType, String> {
     match s {
         "Q4_0" => Ok(GgmlDType::Q4_0),
         "Q4_1" => Ok(GgmlDType::Q4_1),
         "Q5_0" => Ok(GgmlDType::Q5_0),
         "Q5_1" => Ok(GgmlDType::Q5_1),
-        "Q8_0" => Ok(GgmlDType::Q8_1),
-        "Q8_1" => Ok(GgmlDType::Q4_0),
+        "Q8_0" => Ok(GgmlDType::Q8_0),
+        "Q8_1" => Ok(GgmlDType::Q8_1),
         "Q2K" => Ok(GgmlDType::Q2K),
         "Q3K" => Ok(GgmlDType::Q3K),
         "Q4K" => Ok(GgmlDType::Q4K),
         "Q5K" => Ok(GgmlDType::Q5K),
         "Q6K" => Ok(GgmlDType::Q6K),
         "Q8K" => Ok(GgmlDType::Q8K),
         _ => Err(format!("GGML type {s} unknown")),
@@ -410,15 +412,15 @@
     }
 
     /// Send an OpenAI API compatible request, returning the result.
     fn send_chat_completion_request(
         &mut self,
         request: Py<ChatCompletionRequest>,
     ) -> PyResult<Either<ChatCompletionResponse, ChatCompletionStreamer>> {
-        let (tx, rx) = channel();
+        let (tx, mut rx) = channel(10_000);
         Python::with_gil(|py| {
             let request = request.bind(py).borrow();
             let stop_toks = request
                 .stop_seqs
                 .as_ref()
                 .map(|x| StopTokens::Seqs(x.to_vec()));
             let constraint = if request.grammar_type == Some("regex".to_string()) {
@@ -492,20 +494,20 @@
                 is_streaming: request.stream,
                 constraint,
                 suffix: None,
             };
 
             MistralRs::maybe_log_request(self.runner.clone(), format!("{request:?}"));
             let sender = self.runner.get_sender();
-            sender.send(model_request).unwrap();
+            sender.blocking_send(model_request).unwrap();
 
             if request.stream {
                 Ok(Either::Right(ChatCompletionStreamer::from_rx(rx)))
             } else {
-                let response = rx.recv().unwrap();
+                let response = rx.blocking_recv().unwrap();
 
                 match response {
                     Response::ValidationError(e) | Response::InternalError(e) => {
                         Err(PyValueError::new_err(e.to_string()))
                     }
                     Response::Done(response) => Ok(Either::Left(response)),
                     Response::ModelError(msg, _) => Err(PyValueError::new_err(msg.to_string())),
@@ -518,15 +520,15 @@
     }
 
     /// Send an OpenAI API compatible request, returning the result.
     fn send_completion_request(
         &mut self,
         request: Py<CompletionRequest>,
     ) -> PyResult<CompletionResponse> {
-        let (tx, rx) = channel();
+        let (tx, mut rx) = channel(10_000);
         Python::with_gil(|py| {
             let request = request.bind(py).borrow();
             let stop_toks = request
                 .stop_seqs
                 .as_ref()
                 .map(|x| StopTokens::Seqs(x.to_vec()));
             let constraint = if request.grammar_type == Some("regex".to_string()) {
@@ -580,16 +582,16 @@
                 is_streaming: false,
                 constraint,
                 suffix: request.suffix.clone(),
             };
 
             MistralRs::maybe_log_request(self.runner.clone(), format!("{request:?}"));
             let sender = self.runner.get_sender();
-            sender.send(model_request).unwrap();
-            let response = rx.recv().unwrap();
+            sender.blocking_send(model_request).unwrap();
+            let response = rx.blocking_recv().unwrap();
 
             match response {
                 Response::ValidationError(e) | Response::InternalError(e) => {
                     Err(PyValueError::new_err(e.to_string()))
                 }
                 Response::CompletionDone(response) => Ok(response),
                 Response::CompletionModelError(msg, _) => {
@@ -787,14 +789,19 @@
             grammar_type,
         })
     }
 }
 
 #[pymodule]
 fn mistralrs(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
+    let filter = EnvFilter::builder()
+        .with_default_directive(LevelFilter::INFO.into())
+        .from_env_lossy();
+    tracing_subscriber::fmt().with_env_filter(filter).init();
+
     m.add_class::<Runner>()?;
     m.add_class::<Which>()?;
     m.add_class::<ChatCompletionRequest>()?;
     m.add_class::<CompletionRequest>()?;
     m.add_class::<Message>()?;
     m.add_class::<Role>()?;
     m.add_class::<Architecture>()?;
```

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/src/stream.rs` & `mistralrs-0.1.2/mistralrs-pyo3/src/stream.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::sync::mpsc::Receiver;
+use tokio::sync::mpsc::Receiver;
 
 use mistralrs_core::{ChatCompletionChunkResponse, Response};
 use pyo3::{exceptions::PyValueError, pyclass, pymethods, PyRef, PyRefMut, PyResult};
 
 #[pyclass]
 pub struct ChatCompletionStreamer {
     rx: Receiver<Response>,
@@ -20,26 +20,28 @@
     fn __iter__(this: PyRef<'_, Self>) -> PyRef<'_, Self> {
         this
     }
     fn __next__(mut this: PyRefMut<'_, Self>) -> Option<PyResult<ChatCompletionChunkResponse>> {
         if this.is_done {
             return None;
         }
-        match this.rx.recv() {
-            Ok(resp) => match resp {
+        match this.rx.blocking_recv() {
+            Some(resp) => match resp {
                 Response::ModelError(msg, _) => Some(Err(PyValueError::new_err(msg.to_string()))),
                 Response::ValidationError(e) => Some(Err(PyValueError::new_err(e.to_string()))),
                 Response::InternalError(e) => Some(Err(PyValueError::new_err(e.to_string()))),
                 Response::Chunk(response) => {
                     if response.choices.iter().all(|x| x.finish_reason.is_some()) {
                         this.is_done = true;
                     }
                     Some(Ok(response))
                 }
                 Response::Done(_) => unreachable!(),
                 Response::CompletionDone(_) => unreachable!(),
                 Response::CompletionModelError(_, _) => unreachable!(),
             },
-            Err(e) => Some(Err(PyValueError::new_err(e.to_string()))),
+            None => Some(Err(PyValueError::new_err(
+                "Received none in ChatCompletionStreamer".to_string(),
+            ))),
         }
     }
 }
```

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/src/which.rs` & `mistralrs-0.1.2/mistralrs-pyo3/src/which.rs`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 #[derive(Debug, Clone)]
 pub enum Architecture {
     Mistral,
     Gemma,
     Mixtral,
     Llama,
     Phi2,
+    Phi3,
 }
 
 impl From<Architecture> for NormalLoaderType {
     fn from(value: Architecture) -> Self {
         match value {
             Architecture::Gemma => Self::Gemma,
             Architecture::Llama => Self::Llama,
             Architecture::Mistral => Self::Mistral,
             Architecture::Mixtral => Self::Mixtral,
             Architecture::Phi2 => Self::Phi2,
+            Architecture::Phi3 => Self::Phi3,
         }
     }
 }
 
 #[pyclass]
 #[derive(Clone)]
 pub enum Which {
```

### Comparing `mistralrs-0.1.1/mistralrs-pyo3/upload.py` & `mistralrs-0.1.2/mistralrs-pyo3/upload.py`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.1/Cargo.lock` & `mistralrs-0.1.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 dependencies = [
  "backtrace",
 ]
 
 [[package]]
+name = "arbitrary"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
+dependencies = [
+ "derive_arbitrary",
+]
+
+[[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "async-trait"
@@ -225,20 +234,14 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
-
-[[package]]
-name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bindgen_cuda"
 version = "0.1.5"
@@ -329,15 +332,15 @@
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "candle-core"
 version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#04f9b347a10f9775c5a21b7d3b1b0fae1c1ea214"
+source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
 dependencies = [
  "accelerate-src",
  "byteorder",
  "candle-kernels",
  "candle-metal-kernels",
  "cudarc",
  "gemm",
@@ -350,32 +353,32 @@
  "num_cpus",
  "rand",
  "rand_distr",
  "rayon",
  "safetensors",
  "thiserror",
  "yoke",
- "zip",
+ "zip 1.1.2",
 ]
 
 [[package]]
 name = "candle-flash-attn"
 version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#04f9b347a10f9775c5a21b7d3b1b0fae1c1ea214"
+source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
 dependencies = [
  "anyhow",
  "bindgen_cuda",
  "candle-core",
  "half",
 ]
 
 [[package]]
 name = "candle-kernels"
 version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#04f9b347a10f9775c5a21b7d3b1b0fae1c1ea214"
+source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
 dependencies = [
  "bindgen_cuda",
 ]
 
 [[package]]
 name = "candle-layer-norm"
 version = "0.0.1"
@@ -387,26 +390,26 @@
  "num_cpus",
  "rayon",
 ]
 
 [[package]]
 name = "candle-metal-kernels"
 version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#04f9b347a10f9775c5a21b7d3b1b0fae1c1ea214"
+source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
 dependencies = [
  "metal",
  "once_cell",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "candle-nn"
 version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#04f9b347a10f9775c5a21b7d3b1b0fae1c1ea214"
+source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-layer-norm",
  "candle-metal-kernels",
  "half",
  "intel-mkl-src",
@@ -417,15 +420,15 @@
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "candle-transformers"
 version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#04f9b347a10f9775c5a21b7d3b1b0fae1c1ea214"
+source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
 dependencies = [
  "accelerate-src",
  "byteorder",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
  "fancy-regex",
@@ -797,14 +800,25 @@
 [[package]]
 name = "defmac"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aafbece59594ed57696a1a69e8bb3ca1683fbc9cdb41d5c02726070b2cd8f19d"
 
 [[package]]
+name = "derive_arbitrary"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.60",
+]
+
+[[package]]
 name = "derive_builder"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d67778784b508018359cbc8696edb3db78160bab2c2a28ba7f56ef6932997f8"
 dependencies = [
  "derive_builder_macro 0.12.0",
 ]
@@ -989,41 +1003,41 @@
 [[package]]
 name = "fancy-regex"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "531e46835a22af56d1e3b66f04844bed63158bc094a628bec1d321d9b4c44bf2"
 dependencies = [
  "bit-set",
- "regex-automata",
- "regex-syntax",
+ "regex-automata 0.4.6",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "filetime"
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.4.1",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -1356,17 +1370,17 @@
  "num-traits",
  "rand",
  "rand_distr",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
 ]
 
 [[package]]
 name = "heck"
@@ -1546,14 +1560,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "763a5a8f45087d6bcea4222e7b72c291a054edf80e4ef6efd2a4979878c7bea3"
 dependencies = [
  "console",
  "instant",
  "number_prefix",
  "portable-atomic",
+ "rayon",
  "unicode-width",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1627,17 +1642,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
@@ -1655,17 +1670,17 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -1708,14 +1723,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62bb907fe88d54d8d9ce32a3cceab4218ed2f6b7d35617cafe9adf84e43919cb"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "matchers"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
+dependencies = [
+ "regex-automata 0.1.10",
+]
+
+[[package]]
 name = "matchit"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e7465ac9959cc2b1404e8e2367b43684a6d13790fe23056cc8c6c5a6b7bcb94"
 
 [[package]]
 name = "memchr"
@@ -1771,17 +1795,17 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "minijinja"
-version = "1.0.20"
+version = "1.0.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5c5e3d2b4c0a6832bd3d571f7c19a7c1c1f05f11a6e85ae1a29f76be5f9455"
+checksum = "55e877d961d4f96ce13615862322df7c0b6d169d40cab71a7ef3f9b9e594451e"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
@@ -1807,108 +1831,118 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mistralrs"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "anyhow",
  "candle-core",
  "mistralrs-core",
+ "tokio",
 ]
 
 [[package]]
 name = "mistralrs-bench"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "anyhow",
  "candle-core",
  "clap",
  "cli-table",
  "either",
  "mistralrs-core",
  "serde",
  "serde_json",
+ "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-core"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "bytemuck",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
  "candle-transformers",
  "cfgrammar",
  "chrono",
  "clap",
  "dirs",
  "either",
+ "futures",
  "galil-seiferas",
  "half",
  "hf-hub",
  "indexmap",
+ "indicatif",
  "intel-mkl-src",
  "lrtable",
  "minijinja",
  "mistralrs-lora",
  "pyo3",
  "radix_trie",
  "rand",
+ "rand_isaac",
  "range-checked",
- "regex-automata",
+ "rayon",
+ "regex-automata 0.4.6",
  "rustc-hash",
  "serde",
  "serde_json",
  "thiserror",
  "tokenizers",
+ "tokio",
+ "tokio-rayon",
  "tqdm",
  "tracing",
  "vob",
 ]
 
 [[package]]
 name = "mistralrs-lora"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-nn",
  "either",
  "intel-mkl-src",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "mistralrs-pyo3"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "either",
  "futures",
  "indexmap",
  "intel-mkl-src",
  "mistralrs-core",
  "pyo3",
  "serde",
  "serde_json",
+ "tokio",
+ "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-server"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "axum",
  "candle-core",
  "clap",
  "dyn-fmt",
@@ -2211,33 +2245,33 @@
 dependencies = [
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.5.1",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "parse-zoneinfo"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
@@ -2521,14 +2555,23 @@
 checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
+name = "rand_isaac"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fac4373cd91b4f55722c553fb0f286edbb81ef3ff6eec7b99d1898a4110a0b28"
+dependencies = [
+ "rand_core",
+]
+
+[[package]]
 name = "range-checked"
 version = "0.1.0"
 source = "git+https://github.com/EricLBuehler/range-checked.git#655349cc093fcd4965f35b25de394a24ff4b0c7b"
 
 [[package]]
 name = "raw-cpuid"
 version = "10.7.0"
@@ -2581,14 +2624,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
@@ -2599,31 +2651,46 @@
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata",
- "regex-syntax",
+ "regex-automata 0.4.6",
+ "regex-syntax 0.8.3",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
+dependencies = [
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-syntax"
+version = "0.6.29"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "ring"
 version = "0.17.8"
@@ -2702,17 +2769,17 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.33"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3cc72858054fcff6d7dea32df2aeaee6a7c24227366d7ea429aada2f26b16ad"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
@@ -2729,17 +2796,17 @@
  "rustls-webpki",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
@@ -2827,26 +2894,26 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -2969,17 +3036,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "sparsevec"
@@ -3196,15 +3263,15 @@
  "monostate",
  "onig",
  "paste",
  "rand",
  "rayon",
  "rayon-cond",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.8.3",
  "serde",
  "serde_json",
  "spm_precompiled",
  "thiserror",
  "unicode-normalization-alignments",
  "unicode-segmentation",
  "unicode_categories",
@@ -3234,14 +3301,24 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
+name = "tokio-rayon"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7cf33a76e0b1dd03b778f83244137bd59887abf25c0e87bc3e7071105f457693"
+dependencies = [
+ "rayon",
+ "tokio",
+]
+
+[[package]]
 name = "toml"
 version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
  "serde_spanned",
@@ -3372,18 +3449,22 @@
 
 [[package]]
 name = "tracing-subscriber"
 version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad0f048c97dbd9faa9b7df56362b8ebcaa52adb06b498c050d2f4e32f90a7a8b"
 dependencies = [
+ "matchers",
  "nu-ansi-term",
+ "once_cell",
+ "regex",
  "sharded-slab",
  "smallvec",
  "thread_local",
+ "tracing",
  "tracing-core",
  "tracing-log",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.17.0"
@@ -3439,17 +3520,17 @@
 name = "unicode-segmentation"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unicode_categories"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39ec24b3121d976906ece63c9daad25b85969647682eee313cb5779fdd69e14e"
 
@@ -3463,19 +3544,19 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "ureq"
-version = "2.9.6"
+version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
+checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
- "base64 0.21.7",
+ "base64 0.22.0",
  "flate2",
  "log",
  "native-tls",
  "once_cell",
  "rustls",
  "rustls-pki-types",
  "rustls-webpki",
@@ -3536,15 +3617,15 @@
  "axum",
  "mime_guess",
  "regex",
  "rust-embed",
  "serde",
  "serde_json",
  "utoipa",
- "zip",
+ "zip 0.6.6",
 ]
 
 [[package]]
 name = "uuid"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
@@ -3674,19 +3755,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
@@ -3837,17 +3918,17 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.6.6"
+version = "0.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
+checksum = "14b9415ee827af173ebb3f15f9083df5a122eb93572ec28741fb153356ea2578"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xattr"
 version = "1.3.1"
@@ -3937,7 +4018,19 @@
 checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
 dependencies = [
  "byteorder",
  "crc32fast",
  "crossbeam-utils",
  "flate2",
 ]
+
+[[package]]
+name = "zip"
+version = "1.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a23468b4a7a4e9e1e62812f8d1dd614f67f148e2b3faa72f4843bf00b573fd7"
+dependencies = [
+ "arbitrary",
+ "byteorder",
+ "crc32fast",
+ "crossbeam-utils",
+]
```

### Comparing `mistralrs-0.1.1/Cargo.toml` & `mistralrs-0.1.2/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["mistralrs-core", "mistralrs-lora", "mistralrs-pyo3"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 description = "Fast and easy LLM serving."
 homepage = "https://github.com/EricLBuehler/mistral.rs"
 repository = "https://github.com/EricLBuehler/mistral.rs"
 keywords = ["machine-learning"]
 categories = ["science"]
 license = "MIT"
@@ -19,15 +19,19 @@
 serde = "1.0.197"
 serde_json = "1.0.114"
 indexmap = { version = "2.2.5", features = ["serde"] }
 either = { version = "1.10.0", features = ["serde"] }
 accelerate-src = { version = "0.3.2" }
 intel-mkl-src = { version = "0.8.1", features = ["mkl-static-lp64-iomp"] }
 tracing = "0.1.40"
-tracing-subscriber = "0.3.18"
+tracing-subscriber = { version = "0.3.18", features = ["env-filter"] }
 futures = "0.3"
 clap = { version = "4.5.1", features = ["derive"] }
 pyo3 = { version = "0.21.0", features = ["full"] } # pyo3 = { version = "0.21.0", features = ["extension-module", "full"] }
+tokio = { version = "1.36.0", features = ["rt-multi-thread"] }
 
 [profile.profiling]
 inherits = "release"
 debug = true
+
+[profile.dev]
+opt-level = 3
```

### Comparing `mistralrs-0.1.1/pyproject.toml` & `mistralrs-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "mistralrs"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs-0.1.1/PKG-INFO` & `mistralrs-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistralrs
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Rust
 Summary: Fast and easy LLM serving.
```

