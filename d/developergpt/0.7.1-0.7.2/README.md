# Comparing `tmp/developergpt-0.7.1.tar.gz` & `tmp/developergpt-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.7.1.tar", last modified: Sun Apr 28 19:24:19 2024, max compression
+gzip compressed data, was "developergpt-0.7.2.tar", last modified: Tue Apr 30 00:30:13 2024, max compression
```

## Comparing `developergpt-0.7.1.tar` & `developergpt-0.7.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:19.203080 developergpt-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-28 19:24:10.000000 developergpt-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 19:24:10.000000 developergpt-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-04-28 19:24:19.203080 developergpt-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-04-28 19:24:10.000000 developergpt-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:19.199080 developergpt-0.7.1/developergpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/few_shot_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/gemini_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-28 19:24:10.000000 developergpt-0.7.1/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:19.203080 developergpt-0.7.1/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 19:24:19.000000 developergpt-0.7.1/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 19:24:19.203080 developergpt-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-28 19:24:10.000000 developergpt-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:19.203080 developergpt-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 19:24:10.000000 developergpt-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-28 19:24:10.000000 developergpt-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 19:24:10.000000 developergpt-0.7.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:13.267089 developergpt-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 00:30:05.000000 developergpt-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 00:30:05.000000 developergpt-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-04-30 00:30:13.267089 developergpt-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-30 00:30:05.000000 developergpt-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:13.267089 developergpt-0.7.2/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/anthropic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/few_shot_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/gemini_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-30 00:30:05.000000 developergpt-0.7.2/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:13.267089 developergpt-0.7.2/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 00:30:13.000000 developergpt-0.7.2/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:30:13.267089 developergpt-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-30 00:30:05.000000 developergpt-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:13.267089 developergpt-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:30:05.000000 developergpt-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 00:30:05.000000 developergpt-0.7.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 00:30:05.000000 developergpt-0.7.2/tests/test_cli.py
```

### Comparing `developergpt-0.7.1/LICENSE` & `developergpt-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.1/PKG-INFO` & `developergpt-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.7.1
+Version: 0.7.2
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -17,14 +17,15 @@
 Requires-Dist: inquirer
 Requires-Dist: prompt_toolkit
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: llama-cpp-python
 Requires-Dist: huggingface-hub>=0.22.2
 Requires-Dist: minijinja
+Requires-Dist: anthropic>=0.23.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -32,29 +33,30 @@
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: autopep8; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
 DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
 As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
-Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
+Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
 | Model(s)                   | Source                                                                                                                       | Details                                                  |
 | -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
 | **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
 | **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
 | **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
 | **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
 | **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
 | **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
@@ -132,14 +134,26 @@
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
+#### Using Hugging Face Inference API Open LLMs
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+See https://huggingface.co/docs/api-inference/index for more details. 
+
+```bash
+# [OPTIONAL] set Hugging Face token (using zsh for example)
+$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+
+# reload the environment (or just quit and open a new terminal)
+$ source ~/.zshenv
+```
+
 #### Using Mistral-7B-Instruct (Offline)
 To use Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
 ```bash
 developergpt --offline chat
 ```
 
 #### Using OpenAI GPT LLMs
@@ -151,39 +165,43 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Hugging Face Inference API Open LLMs
-To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
-See https://huggingface.co/docs/api-inference/index for more details. 
+#### Using Anthropic LLMs
+To use Anthropic Claude LLMs, you will need an Anthropic API key.
 
+1. Get your own Anthropic API Key: https://www.anthropic.com/api
+2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
 ```bash
-# [OPTIONAL] set Hugging Face token (using zsh for example)
-# You only need to do this once
-$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+# set Anthropic API Key (using zsh for example)
+$ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-### Usage and Cost 
-#### Mistral-7B-Instruct (llama.cpp)
-Mistral-7B-Instruct is free to use and runs locally on-device.
 
+### Usage and Cost 
 #### Google Gemini
 As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
+#### Hugging Face Hosted Open LLMs 
+As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
+
+#### Mistral-7B-Instruct (llama.cpp)
+Mistral-7B-Instruct is free to use and runs locally on-device.
+
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
-#### Hugging Face Hosted Open LLMs 
-As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
+#### Anthropic Claude LLMs
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. Based on preliminary testing, using DeveloperGPT with Claude Haiku should cost less than 10 cents per day with regular usage. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini Pro API free tier.
```

### Comparing `developergpt-0.7.1/README.md` & `developergpt-0.7.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
 DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
 As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
-Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
+Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
 | Model(s)                   | Source                                                                                                                       | Details                                                  |
 | -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
 | **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
 | **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
 | **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
 | **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
 | **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
 | **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
@@ -96,14 +97,26 @@
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
+#### Using Hugging Face Inference API Open LLMs
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+See https://huggingface.co/docs/api-inference/index for more details. 
+
+```bash
+# [OPTIONAL] set Hugging Face token (using zsh for example)
+$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+
+# reload the environment (or just quit and open a new terminal)
+$ source ~/.zshenv
+```
+
 #### Using Mistral-7B-Instruct (Offline)
 To use Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
 ```bash
 developergpt --offline chat
 ```
 
 #### Using OpenAI GPT LLMs
@@ -115,39 +128,43 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Hugging Face Inference API Open LLMs
-To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
-See https://huggingface.co/docs/api-inference/index for more details. 
+#### Using Anthropic LLMs
+To use Anthropic Claude LLMs, you will need an Anthropic API key.
 
+1. Get your own Anthropic API Key: https://www.anthropic.com/api
+2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
 ```bash
-# [OPTIONAL] set Hugging Face token (using zsh for example)
-# You only need to do this once
-$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+# set Anthropic API Key (using zsh for example)
+$ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-### Usage and Cost 
-#### Mistral-7B-Instruct (llama.cpp)
-Mistral-7B-Instruct is free to use and runs locally on-device.
 
+### Usage and Cost 
 #### Google Gemini
 As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
+#### Hugging Face Hosted Open LLMs 
+As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
+
+#### Mistral-7B-Instruct (llama.cpp)
+Mistral-7B-Instruct is free to use and runs locally on-device.
+
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
-#### Hugging Face Hosted Open LLMs 
-As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
+#### Anthropic Claude LLMs
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. Based on preliminary testing, using DeveloperGPT with Claude Haiku should cost less than 10 cents per day with regular usage. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini Pro API free tier.
```

### Comparing `developergpt-0.7.1/developergpt/cli.py` & `developergpt-0.7.2/developergpt/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
 DeveloperGPT by luo-anthony
 """
 
 import os
 import subprocess
 import sys
-from functools import wraps
 from typing import Optional
 
 import click
 import google.generativeai as genai
 import inquirer
+from anthropic import Anthropic
 from google.generativeai import GenerativeModel
 from llama_cpp import Llama
 from openai import OpenAI
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.shortcuts import CompleteStyle
 from rich.console import Console
 
 from developergpt import (
+    anthropic_adapter,
     config,
     gemini_adapter,
     huggingface_adapter,
     openai_adapter,
     utils,
 )
 
@@ -36,15 +37,15 @@
     "--temperature",
     default=0.2,
     help="The temperature of the model response for chat (higher means more creative, lower means more predictable)",
 )
 @click.option(
     "--model",
     default="gemini",
-    help=f"The LLM to use. Options: f{', '.join(config.SUPPORTED_MODELS)}",
+    help=f"The LLM to use. Options: {', '.join(config.SUPPORTED_MODELS)}",
 )
 @click.option(
     "--offline",
     is_flag=True,
     default=False,
     help=f"Use DeveloperGPT with a quantized LLM running on-device (offline). Options: {', '.join(config.OFFLINE_MODELS)}",
 )
@@ -65,15 +66,15 @@
         console.print(
             """[bold red]No internet connection. """
             """Please check your internet connection or use --offline mode.[/bold red]"""
         )
         sys.exit(-1)
 
     ctx.ensure_object(dict)
-    client: Optional[OpenAI | Llama] = None
+    client: Optional[OpenAI | Llama | Anthropic] = None
     if offline or model in config.OFFLINE_MODELS:
         console.print(
             f"""[bold yellow]Using quantized {' '.join(config.LLAMA_CPP_MODEL_MAP[model])} running on-device (offline)."""
         )
         repo, llm_file, chat_format = config.LLAMA_CPP_MODEL_MAP[model]
         common_llama_args = {
             "n_ctx": config.OFFLINE_MODEL_CTX,
@@ -112,14 +113,17 @@
         )
         console.print(
             f"[bold yellow]Using {config.HF_MODEL_MAP[model]} via Hugging Face Inference API."
         )
     elif model in config.GOOGLE_MODEL_MAP:
         api_key = config.get_environ_key(config.GOOGLE_API_KEY, console)
         genai.configure(api_key=api_key)
+    elif model in config.ANTHROPIC_MODEL_MAP:
+        api_key = config.get_environ_key(config.ANTHROPIC_API_KEY, console)
+        client = Anthropic(api_key=api_key)
 
     ctx.obj["temperature"] = temperature
     ctx.obj["model"] = model
     ctx.obj["offline"] = offline
     ctx.obj["client"] = client
 
 
@@ -144,14 +148,16 @@
         if instruct_model:
             input_messages = []
         else:
             input_messages = huggingface_adapter.BASE_INPUT_CHAT_MSGS
     elif model in config.GOOGLE_MODEL_MAP:
         gemini_model = GenerativeModel(config.GOOGLE_MODEL_MAP[model])
         chat_session = gemini_model.start_chat()
+    elif model in config.ANTHROPIC_MODEL_MAP:
+        input_messages = []
     else:
         return
 
     console.print("[gray]Type 'quit' to exit the chat[/gray]")
     while True:
         if not user_input:
             user_input = utils.prompt_user_input(
@@ -185,25 +191,35 @@
         elif model in config.GOOGLE_MODEL_MAP:
             gemini_adapter.get_model_chat_response(
                 user_input=user_input,
                 console=console,
                 chat_session=chat_session,
                 temperature=ctx.obj["temperature"],
             )
+        elif model in config.ANTHROPIC_MODEL_MAP:
+            client = ctx.obj["client"]
+            input_messages = anthropic_adapter.get_model_chat_response(
+                user_input=user_input,
+                console=console,
+                input_messages=input_messages,
+                temperature=ctx.obj["temperature"],
+                model=model,
+                client=client,
+            )
 
         user_input = None
 
 
-@main.command(help="Execute commands using natural language")
+@main.command(help="Natural language to terminal commands")
 @click.argument("user_input", nargs=-1)
 @click.option(
     "--fast",
     is_flag=True,
     default=False,
-    help="Get commands without command or argument explanations (less accurate)",
+    help="Get commands without explanations (may be less accurate)",
 )
 @click.pass_context
 def cmd(ctx, user_input, fast):
     """
     Natural Language to Terminal Commands
     """
     input_request = "\nDesired Command Request: "
@@ -254,14 +270,22 @@
         elif model in config.GOOGLE_MODEL_MAP:
             model_output = gemini_adapter.model_command(
                 user_input=user_input,
                 console=console,
                 fast_mode=fast,
                 model=model,
             )
+        elif model in config.ANTHROPIC_MODEL_MAP:
+            model_output = anthropic_adapter.model_command(
+                user_input=user_input,
+                console=console,
+                fast_mode=fast,
+                model=model,
+                client=ctx.obj["client"],
+            )
 
         user_input = None  # clear input for next iteration
 
         commands = utils.print_command_response(model_output, console, fast)
         if not commands:
             continue
```

### Comparing `developergpt-0.7.1/developergpt/config.py` & `developergpt-0.7.2/developergpt/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,26 +28,30 @@
 ZEPHYR = "zephyr"
 GEMMA = "gemma"
 GEMMA_BASE = "gemma-base"
 GEMINI = "gemini"
 MISTRAL_Q6 = "mistral-q6"
 MISTRAL_Q4 = "mistral-q4"
 MISTRAL_HF = "mistral"
+SONNET = "sonnet"
+HAIKU = "haiku"
 BLOOM = "bloom"  # not supported due to poor performance
 SUPPORTED_MODELS = set(
     [
         GPT35,
         GPT4,
         GEMINI,
         ZEPHYR,
         MISTRAL_Q6,
         MISTRAL_Q4,
         MISTRAL_HF,
         GEMMA,
         GEMMA_BASE,
+        SONNET,
+        HAIKU,
     ]
 )
 OFFLINE_MODEL_CTX = 4000
 OFFLINE_MODELS = set([MISTRAL_Q6, MISTRAL_Q4])
 OFFLINE_MODEL_CACHE_DIR = os.path.expanduser("~/.cache/developergpt")
 
 LLAMA_CPP_MODEL_MAP = {
@@ -64,14 +68,19 @@
 }
 
 OPENAI_MODEL_MAP = {
     GPT35: "gpt-3.5-turbo",
     GPT4: "gpt-4-turbo",
 }
 
+ANTHROPIC_MODEL_MAP = {
+    SONNET: "claude-3-sonnet-20240229",
+    HAIKU: "claude-3-haiku-20240307",
+}
+
 HF_MODEL_MAP = {
     ZEPHYR: "HuggingFaceH4/zephyr-7b-beta",
     GEMMA: "google/gemma-1.1-7b-it",
     GEMMA_BASE: "google/gemma-7b",
     MISTRAL_HF: "mistralai/Mistral-7B-Instruct-v0.2",
     BLOOM: "bigscience/bloom",
 }
@@ -86,14 +95,15 @@
 }
 
 ### API Key Constants ###
 
 GOOGLE_API_KEY = "GOOGLE_API_KEY"
 OPEN_AI_API_KEY = "OPENAI_API_KEY"
 HUGGING_FACE_API_KEY = "HUGGING_FACE_API_KEY"
+ANTHROPIC_API_KEY = "ANTHROPIC_API_KEY"
 
 ### General Configuration ###
 
 USER_PLATFORM = platform.platform()
 CMD_TEMP = 0.01
```

### Comparing `developergpt-0.7.1/developergpt/few_shot_prompts.py` & `developergpt-0.7.2/developergpt/few_shot_prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 from datetime import datetime
 
+from developergpt import config
+
+CHAT_SYS_MSG = f"""
+You are DeveloperGPT, a helpful personal assistant for a programmer working on a {config.USER_PLATFORM} machine. 
+Your task is to assist the programmer with any programming-related tasks they may have. 
+This could include providing advice on how to approach a programming problem, suggesting tools or libraries to use for a particular task, 
+helping to troubleshoot errors or bugs in code, answering general programming questions, and providing code snippets or examples.
+
+Please keep your answers short and concise and use a suitable format for printing on the terminal. 
+If you provide code snippets, use ```<language> to specify the language. 
+"""
+
+CMD_SYS_MSG = f"""
+As an assistant for a programmer on a {config.USER_PLATFORM} machine, your task is to provide the appropriate command-line commands to execute a user request.
+"""
+
 JSON_CMD_FORMAT = """
 {
     "input": "<user input>",
     "error": 0,
     "commands": [
         {
             "seq": <Order of Command>,
```

### Comparing `developergpt-0.7.1/developergpt/gemini_adapter.py` & `developergpt-0.7.2/developergpt/gemini_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.1/developergpt/huggingface_adapter.py` & `developergpt-0.7.2/developergpt/huggingface_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.1/developergpt/openai_adapter.py` & `developergpt-0.7.2/developergpt/openai_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,36 +12,28 @@
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from developergpt import config, few_shot_prompts, utils
 from developergpt.few_shot_prompts import (
+    CHAT_SYS_MSG,
+    CMD_SYS_MSG,
     INITIAL_USER_CMD_MSG,
     INITIAL_USER_CMD_MSG_FAST,
 )
 
 INITIAL_CHAT_SYSTEM_MSG = {
     "role": "system",
-    "content": f"""
-                You are DeveloperGPT, a helpful personal assistant for a programmer working on a {config.USER_PLATFORM} machine. 
-                Your task is to assist the programmer with any programming-related tasks they may have. 
-                This could include providing advice on how to approach a programming problem, suggesting tools or libraries to use for a particular task, 
-                helping to troubleshoot errors or bugs in code, answering general programming questions, and providing code snippets or examples.
-
-                Please keep your answers short and concise and use a suitable format for printing on the terminal. 
-                If you provide code snippets, use ```<language> to specify the language. 
-            """,
+    "content": CHAT_SYS_MSG,
 }
 
 INITIAL_CMD_SYSTEM_MSG = {
     "role": "system",
-    "content": f"""
-            As an assistant for a programmer on a {config.USER_PLATFORM} machine, your task is to provide the appropriate command-line commands to execute a user request.
-            """,
+    "content": CMD_SYS_MSG,
 }
 
 
 def format_user_request(
     user_request: str, platform: str = config.USER_PLATFORM
 ) -> dict:
     return {
```

### Comparing `developergpt-0.7.1/developergpt/utils.py` & `developergpt-0.7.2/developergpt/utils.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.1/developergpt.egg-info/PKG-INFO` & `developergpt-0.7.2/developergpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.7.1
+Version: 0.7.2
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -17,14 +17,15 @@
 Requires-Dist: inquirer
 Requires-Dist: prompt_toolkit
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: llama-cpp-python
 Requires-Dist: huggingface-hub>=0.22.2
 Requires-Dist: minijinja
+Requires-Dist: anthropic>=0.23.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -32,29 +33,30 @@
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: autopep8; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
 DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
 
 As of May 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
-Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
+Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
 | Model(s)                   | Source                                                                                                                       | Details                                                  |
 | -------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
 | **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                                   | Free (up to 15 requests/min), Google AI API Key Required |
 | **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
 | **Zephyr**                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
 | **Gemma, Gemma-Base**      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
 | **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
 | **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
 - `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
@@ -132,14 +134,26 @@
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
+#### Using Hugging Face Inference API Open LLMs
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
+See https://huggingface.co/docs/api-inference/index for more details. 
+
+```bash
+# [OPTIONAL] set Hugging Face token (using zsh for example)
+$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+
+# reload the environment (or just quit and open a new terminal)
+$ source ~/.zshenv
+```
+
 #### Using Mistral-7B-Instruct (Offline)
 To use Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
 ```bash
 developergpt --offline chat
 ```
 
 #### Using OpenAI GPT LLMs
@@ -151,39 +165,43 @@
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-#### Using Hugging Face Inference API Open LLMs
-To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
-See https://huggingface.co/docs/api-inference/index for more details. 
+#### Using Anthropic LLMs
+To use Anthropic Claude LLMs, you will need an Anthropic API key.
 
+1. Get your own Anthropic API Key: https://www.anthropic.com/api
+2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
 ```bash
-# [OPTIONAL] set Hugging Face token (using zsh for example)
-# You only need to do this once
-$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+# set Anthropic API Key (using zsh for example)
+$ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-### Usage and Cost 
-#### Mistral-7B-Instruct (llama.cpp)
-Mistral-7B-Instruct is free to use and runs locally on-device.
 
+### Usage and Cost 
 #### Google Gemini
 As of May 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
+#### Hugging Face Hosted Open LLMs 
+As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
+
+#### Mistral-7B-Instruct (llama.cpp)
+Mistral-7B-Instruct is free to use and runs locally on-device.
+
 #### OpenAI GPT
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
-#### Hugging Face Hosted Open LLMs 
-As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details. 
+#### Anthropic Claude LLMs
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. Based on preliminary testing, using DeveloperGPT with Claude Haiku should cost less than 10 cents per day with regular usage. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini Pro API free tier.
```

### Comparing `developergpt-0.7.1/developergpt.egg-info/SOURCES.txt` & `developergpt-0.7.2/developergpt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 developergpt/VERSION
 developergpt/__init__.py
 developergpt/__main__.py
+developergpt/anthropic_adapter.py
 developergpt/cli.py
 developergpt/config.py
 developergpt/few_shot_prompts.py
 developergpt/gemini_adapter.py
 developergpt/huggingface_adapter.py
 developergpt/openai_adapter.py
 developergpt/utils.py
```

### Comparing `developergpt-0.7.1/setup.py` & `developergpt-0.7.2/setup.py`

 * *Files identical despite different names*

