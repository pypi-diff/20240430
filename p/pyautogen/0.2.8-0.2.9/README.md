# Comparing `tmp/pyautogen-0.2.8.tar.gz` & `tmp/pyautogen-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautogen-0.2.8.tar", last modified: Tue Jan 23 16:17:50 2024, max compression
+gzip compressed data, was "pyautogen-0.2.9.tar", last modified: Sun Jan 28 00:57:54 2024, max compression
```

## Comparing `pyautogen-0.2.8.tar` & `pyautogen-0.2.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.830402 pyautogen-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-01-23 16:17:26.000000 pyautogen-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-01-23 16:17:26.000000 pyautogen-0.2.8/LICENSE-CODE
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-01-23 16:17:50.830402 pyautogen-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-01-23 16:17:26.000000 pyautogen-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.822403 pyautogen-0.2.8/autogen/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agent_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.822403 pyautogen-0.2.8/autogen/agentchat/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/assistant_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.826403 pyautogen-0.2.8/autogen/agentchat/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32658 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/agent_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.826403 pyautogen-0.2.8/autogen/agentchat/contrib/capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/capabilities/agent_capability.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/capabilities/teachability.py
--rw-r--r--   0 runner    (1001) docker     (127)    23884 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/compressible_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/gpt_assistant_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/llava_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19271 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/math_user_proxy_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/multimodal_conversable_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    18282 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/qdrant_retrieve_user_proxy_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/retrieve_assistant_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/retrieve_user_proxy_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/text_analyzer_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    16171 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/contrib/web_surfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    92289 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/conversable_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    21196 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/groupchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/agentchat/user_proxy_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/browser_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.826403 pyautogen-0.2.8/autogen/cache/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/cache/abstract_cache_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/cache/cache_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/cache/disk_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/cache/redis_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    27755 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/code_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.826403 pyautogen-0.2.8/autogen/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/function_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.826403 pyautogen-0.2.8/autogen/oai/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32003 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/oai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    53077 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/oai/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    27838 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/oai/openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15495 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/retrieve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/token_count_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-23 16:17:26.000000 pyautogen-0.2.8/autogen/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.830402 pyautogen-0.2.8/pyautogen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-01-23 16:17:50.000000 pyautogen-0.2.8/pyautogen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-01-23 16:17:50.000000 pyautogen-0.2.8/pyautogen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 16:17:50.000000 pyautogen-0.2.8/pyautogen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-23 16:17:50.000000 pyautogen-0.2.8/pyautogen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-23 16:17:50.000000 pyautogen-0.2.8/pyautogen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-23 16:17:26.000000 pyautogen-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 16:17:50.830402 pyautogen-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-23 16:17:26.000000 pyautogen-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:17:50.830402 pyautogen-0.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-01-23 16:17:26.000000 pyautogen-0.2.8/test/test_browser_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17053 2024-01-23 16:17:26.000000 pyautogen-0.2.8/test/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    13813 2024-01-23 16:17:26.000000 pyautogen-0.2.8/test/test_function_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-01-23 16:17:26.000000 pyautogen-0.2.8/test/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-23 16:17:26.000000 pyautogen-0.2.8/test/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-01-23 16:17:26.000000 pyautogen-0.2.8/test/test_retrieve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-23 16:17:26.000000 pyautogen-0.2.8/test/test_token_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.817724 pyautogen-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-01-28 00:57:36.000000 pyautogen-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-01-28 00:57:36.000000 pyautogen-0.2.9/LICENSE-CODE
+-rw-r--r--   0 runner    (1001) docker     (127)    16515 2024-01-28 00:57:54.817724 pyautogen-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-01-28 00:57:36.000000 pyautogen-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.809724 pyautogen-0.2.9/autogen/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agent_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.809724 pyautogen-0.2.9/autogen/agentchat/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/assistant_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.813724 pyautogen-0.2.9/autogen/agentchat/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32658 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/agent_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.813724 pyautogen-0.2.9/autogen/agentchat/contrib/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/capabilities/agent_capability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/capabilities/teachability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23884 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/compressible_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/gpt_assistant_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/llava_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19271 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/math_user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/multimodal_conversable_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18282 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/qdrant_retrieve_user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/retrieve_assistant_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/retrieve_user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/text_analyzer_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16171 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/contrib/web_surfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93077 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/conversable_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25614 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/groupchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/agentchat/user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/browser_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.813724 pyautogen-0.2.9/autogen/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/cache/abstract_cache_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/cache/cache_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/cache/disk_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/cache/redis_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27755 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/code_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.813724 pyautogen-0.2.9/autogen/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/function_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.813724 pyautogen-0.2.9/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32003 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/oai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53077 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/oai/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27838 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/oai/openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15495 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/retrieve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/token_count_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-28 00:57:36.000000 pyautogen-0.2.9/autogen/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.813724 pyautogen-0.2.9/pyautogen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16515 2024-01-28 00:57:54.000000 pyautogen-0.2.9/pyautogen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-01-28 00:57:54.000000 pyautogen-0.2.9/pyautogen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 00:57:54.000000 pyautogen-0.2.9/pyautogen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-28 00:57:54.000000 pyautogen-0.2.9/pyautogen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-28 00:57:54.000000 pyautogen-0.2.9/pyautogen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-28 00:57:36.000000 pyautogen-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 00:57:54.817724 pyautogen-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-28 00:57:36.000000 pyautogen-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 00:57:54.817724 pyautogen-0.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-01-28 00:57:36.000000 pyautogen-0.2.9/test/test_browser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-01-28 00:57:36.000000 pyautogen-0.2.9/test/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13813 2024-01-28 00:57:36.000000 pyautogen-0.2.9/test/test_function_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-01-28 00:57:36.000000 pyautogen-0.2.9/test/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-28 00:57:36.000000 pyautogen-0.2.9/test/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-01-28 00:57:36.000000 pyautogen-0.2.9/test/test_retrieve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-28 00:57:36.000000 pyautogen-0.2.9/test/test_token_count.py
```

### Comparing `pyautogen-0.2.8/LICENSE` & `pyautogen-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/LICENSE-CODE` & `pyautogen-0.2.9/LICENSE-CODE`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/PKG-INFO` & `pyautogen-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautogen
-Version: 0.2.8
+Version: 0.2.9
 Summary: Enabling Next-Gen LLM Applications via Multi-Agent Conversation Framework
 Home-page: https://github.com/microsoft/autogen
 Author: AutoGen
 Author-email: auto-gen@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,16 @@
 # AutoGen
 [📚 Cite paper](#related-papers).
 <!-- <p align="center">
     <img src="https://github.com/microsoft/autogen/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p> -->
 
+:warning: Jan 23: **Breaking Change in Latest Release v0.2.8** `use_docker` defaults to `True` for code-execution. See [blog post](https://microsoft.github.io/autogen/blog/2024/01/23/Code-execution-in-docker) for details and [FAQ](https://microsoft.github.io/autogen/docs/FAQ#agents-are-throwing-due-to-docker-not-running-how-can-i-resolve-this) for troubleshooting any issues.
+
 :fire: Dec 31: [AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation Framework](https://arxiv.org/abs/2308.08155) is selected by [TheSequence: My Five Favorite AI Papers of 2023](https://thesequence.substack.com/p/my-five-favorite-ai-papers-of-2023).
 
 <!-- :fire: Nov 24: pyautogen [v0.2](https://github.com/microsoft/autogen/releases/tag/v0.2.0) is released with many updates and new features compared to v0.1.1. It switches to using openai-python v1. Please read the [migration guide](https://microsoft.github.io/autogen/docs/Installation#python). -->
 
 <!-- :fire: Nov 11: OpenAI's Assistants are available in AutoGen and interoperatable with other AutoGen agents! Checkout our [blogpost](https://microsoft.github.io/autogen/blog/2023/11/13/OAI-assistants) for details and examples. -->
 
 :fire: Nov 8: AutoGen is selected into [Open100: Top 100 Open Source achievements](https://www.benchcouncil.org/evaluation/opencs/annual.html) 35 days after spinoff.
```

### Comparing `pyautogen-0.2.8/README.md` & `pyautogen-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # AutoGen
 [📚 Cite paper](#related-papers).
 <!-- <p align="center">
     <img src="https://github.com/microsoft/autogen/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p> -->
 
+:warning: Jan 23: **Breaking Change in Latest Release v0.2.8** `use_docker` defaults to `True` for code-execution. See [blog post](https://microsoft.github.io/autogen/blog/2024/01/23/Code-execution-in-docker) for details and [FAQ](https://microsoft.github.io/autogen/docs/FAQ#agents-are-throwing-due-to-docker-not-running-how-can-i-resolve-this) for troubleshooting any issues.
+
 :fire: Dec 31: [AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation Framework](https://arxiv.org/abs/2308.08155) is selected by [TheSequence: My Five Favorite AI Papers of 2023](https://thesequence.substack.com/p/my-five-favorite-ai-papers-of-2023).
 
 <!-- :fire: Nov 24: pyautogen [v0.2](https://github.com/microsoft/autogen/releases/tag/v0.2.0) is released with many updates and new features compared to v0.1.1. It switches to using openai-python v1. Please read the [migration guide](https://microsoft.github.io/autogen/docs/Installation#python). -->
 
 <!-- :fire: Nov 11: OpenAI's Assistants are available in AutoGen and interoperatable with other AutoGen agents! Checkout our [blogpost](https://microsoft.github.io/autogen/blog/2023/11/13/OAI-assistants) for details and examples. -->
 
 :fire: Nov 8: AutoGen is selected into [Open100: Top 100 Open Source achievements](https://www.benchcouncil.org/evaluation/opencs/annual.html) 35 days after spinoff.
```

### Comparing `pyautogen-0.2.8/autogen/_pydantic.py` & `pyautogen-0.2.9/autogen/_pydantic.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agent_utils.py` & `pyautogen-0.2.9/autogen/agent_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/agent.py` & `pyautogen-0.2.9/autogen/agentchat/agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/assistant_agent.py` & `pyautogen-0.2.9/autogen/agentchat/assistant_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/agent_builder.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/agent_builder.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/capabilities/agent_capability.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/capabilities/agent_capability.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/capabilities/teachability.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/capabilities/teachability.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/compressible_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/compressible_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/gpt_assistant_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/gpt_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/img_utils.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/img_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/llava_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/llava_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/math_user_proxy_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/math_user_proxy_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/multimodal_conversable_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/multimodal_conversable_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/qdrant_retrieve_user_proxy_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/qdrant_retrieve_user_proxy_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/retrieve_assistant_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/retrieve_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/retrieve_user_proxy_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/retrieve_user_proxy_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/text_analyzer_agent.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/text_analyzer_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/contrib/web_surfer.py` & `pyautogen-0.2.9/autogen/agentchat/contrib/web_surfer.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/agentchat/conversable_agent.py` & `pyautogen-0.2.9/autogen/agentchat/conversable_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -755,24 +755,38 @@
     def reset_consecutive_auto_reply_counter(self, sender: Optional[Agent] = None):
         """Reset the consecutive_auto_reply_counter of the sender."""
         if sender is None:
             self._consecutive_auto_reply_counter.clear()
         else:
             self._consecutive_auto_reply_counter[sender] = 0
 
-    def clear_history(self, agent: Optional[Agent] = None):
+    def clear_history(self, recipient: Optional[Agent] = None, nr_messages_to_preserve: Optional[int] = None):
         """Clear the chat history of the agent.
 
         Args:
-            agent: the agent with whom the chat history to clear. If None, clear the chat history with all agents.
+            recipient: the agent with whom the chat history to clear. If None, clear the chat history with all agents.
+            nr_messages_to_preserve: the number of newest messages to preserve in the chat history.
         """
-        if agent is None:
-            self._oai_messages.clear()
+        if recipient is None:
+            if nr_messages_to_preserve:
+                for key in self._oai_messages:
+                    # Remove messages from history except last `nr_messages_to_preserve` messages.
+                    self._oai_messages[key] = self._oai_messages[key][-nr_messages_to_preserve:]
+            else:
+                self._oai_messages.clear()
         else:
-            self._oai_messages[agent].clear()
+            self._oai_messages[recipient].clear()
+            if nr_messages_to_preserve:
+                print(
+                    colored(
+                        "WARNING: `nr_preserved_messages` is ignored when clearing chat history with a specific agent.",
+                        "yellow",
+                    ),
+                    flush=True,
+                )
 
     def generate_oai_reply(
         self,
         messages: Optional[List[Dict]] = None,
         sender: Optional[Agent] = None,
         config: Optional[OpenAIWrapper] = None,
     ) -> Tuple[bool, Union[str, Dict, None]]:
```

### Comparing `pyautogen-0.2.8/autogen/agentchat/groupchat.py` & `pyautogen-0.2.9/autogen/agentchat/groupchat.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,23 +27,27 @@
     - speaker_selection_method: the method for selecting the next speaker. Default is "auto".
         Could be any of the following (case insensitive), will raise ValueError if not recognized:
         - "auto": the next speaker is selected automatically by LLM.
         - "manual": the next speaker is selected manually by user input.
         - "random": the next speaker is selected randomly.
         - "round_robin": the next speaker is selected in a round robin fashion, i.e., iterating in the same order as provided in `agents`.
     - allow_repeat_speaker: whether to allow the same speaker to speak consecutively. Default is True, in which case all speakers are allowed to speak consecutively. If allow_repeat_speaker is a list of Agents, then only those listed agents are allowed to repeat. If set to False, then no speakers are allowed to repeat.
+    - enable_clear_history: enable possibility to clear history of messages for agents manually by providing
+        "clear history" phrase in user prompt. This is experimental feature.
+        See description of GroupChatManager.clear_agents_history function for more info.
     """
 
     agents: List[Agent]
     messages: List[Dict]
     max_round: Optional[int] = 10
     admin_name: Optional[str] = "Admin"
     func_call_filter: Optional[bool] = True
     speaker_selection_method: Optional[str] = "auto"
     allow_repeat_speaker: Optional[Union[bool, List[Agent]]] = True
+    enable_clear_history: Optional[bool] = False
 
     _VALID_SPEAKER_SELECTION_METHODS = ["auto", "manual", "random", "round_robin"]
 
     @property
     def agent_names(self) -> List[str]:
         """Return the names of the agents in the group chat."""
         return [agent.name for agent in self.agents]
@@ -384,14 +388,22 @@
                     speaker = groupchat.agent_by_name(groupchat.admin_name)
                     reply = speaker.generate_reply(sender=self)
                 else:
                     # admin agent is not found in the participants
                     raise
             if reply is None:
                 break
+
+            # check for "clear history" phrase in reply and activate clear history function if found
+            if (
+                groupchat.enable_clear_history
+                and isinstance(reply, dict)
+                and "CLEAR HISTORY" in reply["content"].upper()
+            ):
+                reply["content"] = self.clear_agents_history(reply["content"], groupchat)
             # The speaker sends the message without requesting a reply
             speaker.send(reply, self, request_reply=False)
             message = self.last_message(speaker)
             if i == groupchat.max_round - 1:
                 groupchat.append(message, speaker)
         if self.client_cache is not None:
             for a in groupchat.agents:
@@ -460,7 +472,74 @@
         Raises:
             RuntimeError: if any async reply functions are registered.
         """
         super()._raise_exception_on_async_reply_functions()
 
         for agent in self._groupchat.agents:
             agent._raise_exception_on_async_reply_functions()
+
+    def clear_agents_history(self, reply: str, groupchat: GroupChat) -> str:
+        """Clears history of messages for all agents or selected one. Can preserve selected number of last messages.
+        That function is called when user manually provide "clear history" phrase in his reply.
+        When "clear history" is provided, the history of messages for all agents is cleared.
+        When "clear history <agent_name>" is provided, the history of messages for selected agent is cleared.
+        When "clear history <nr_of_messages_to_preserve>" is provided, the history of messages for all agents is cleared
+        except last <nr_of_messages_to_preserve> messages.
+        When "clear history <agent_name> <nr_of_messages_to_preserve>" is provided, the history of messages for selected
+        agent is cleared except last <nr_of_messages_to_preserve> messages.
+        Phrase "clear history" and optional arguments are cut out from the reply before it passed to the chat.
+
+        Args:
+            reply (str): Admin reply to analyse.
+            groupchat (GroupChat): GroupChat object.
+        """
+        # Split the reply into words
+        words = reply.split()
+        # Find the position of "clear" to determine where to start processing
+        clear_word_index = next(i for i in reversed(range(len(words))) if words[i].upper() == "CLEAR")
+        # Extract potential agent name and steps
+        words_to_check = words[clear_word_index + 2 : clear_word_index + 4]
+        nr_messages_to_preserve = None
+        agent_to_memory_clear = None
+
+        for word in words_to_check:
+            if word.isdigit():
+                nr_messages_to_preserve = int(word)
+            elif word[:-1].isdigit():  # for the case when number of messages is followed by dot or other sign
+                nr_messages_to_preserve = int(word[:-1])
+            else:
+                for agent in groupchat.agents:
+                    if agent.name == word:
+                        agent_to_memory_clear = agent
+                        break
+                    elif agent.name == word[:-1]:  # for the case when agent name is followed by dot or other sign
+                        agent_to_memory_clear = agent
+                        break
+        # clear history
+        if agent_to_memory_clear:
+            if nr_messages_to_preserve:
+                print(
+                    f"Clearing history for {agent_to_memory_clear.name} except last {nr_messages_to_preserve} messages."
+                )
+            else:
+                print(f"Clearing history for {agent_to_memory_clear.name}.")
+            agent_to_memory_clear.clear_history(nr_messages_to_preserve=nr_messages_to_preserve)
+        else:
+            if nr_messages_to_preserve:
+                print(f"Clearing history for all agents except last {nr_messages_to_preserve} messages.")
+                # clearing history for groupchat here
+                temp = groupchat.messages[-nr_messages_to_preserve:]
+                groupchat.messages.clear()
+                groupchat.messages.extend(temp)
+            else:
+                print("Clearing history for all agents.")
+                # clearing history for groupchat here
+                groupchat.messages.clear()
+            # clearing history for agents
+            for agent in groupchat.agents:
+                agent.clear_history(nr_messages_to_preserve=nr_messages_to_preserve)
+
+        # Reconstruct the reply without the "clear history" command and parameters
+        skip_words_number = 2 + int(bool(agent_to_memory_clear)) + int(bool(nr_messages_to_preserve))
+        reply = " ".join(words[:clear_word_index] + words[clear_word_index + skip_words_number :])
+
+        return reply
```

### Comparing `pyautogen-0.2.8/autogen/agentchat/user_proxy_agent.py` & `pyautogen-0.2.9/autogen/agentchat/user_proxy_agent.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/browser_utils.py` & `pyautogen-0.2.9/autogen/browser_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/cache/abstract_cache_base.py` & `pyautogen-0.2.9/autogen/cache/abstract_cache_base.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/cache/cache.py` & `pyautogen-0.2.9/autogen/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/cache/cache_factory.py` & `pyautogen-0.2.9/autogen/cache/cache_factory.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/cache/disk_cache.py` & `pyautogen-0.2.9/autogen/cache/disk_cache.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/cache/redis_cache.py` & `pyautogen-0.2.9/autogen/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/code_utils.py` & `pyautogen-0.2.9/autogen/code_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/function_utils.py` & `pyautogen-0.2.9/autogen/function_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/math_utils.py` & `pyautogen-0.2.9/autogen/math_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/oai/__init__.py` & `pyautogen-0.2.9/autogen/oai/__init__.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/oai/client.py` & `pyautogen-0.2.9/autogen/oai/client.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/oai/completion.py` & `pyautogen-0.2.9/autogen/oai/completion.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/oai/openai_utils.py` & `pyautogen-0.2.9/autogen/oai/openai_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/retrieve_utils.py` & `pyautogen-0.2.9/autogen/retrieve_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/autogen/token_count_utils.py` & `pyautogen-0.2.9/autogen/token_count_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/pyautogen.egg-info/PKG-INFO` & `pyautogen-0.2.9/pyautogen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautogen
-Version: 0.2.8
+Version: 0.2.9
 Summary: Enabling Next-Gen LLM Applications via Multi-Agent Conversation Framework
 Home-page: https://github.com/microsoft/autogen
 Author: AutoGen
 Author-email: auto-gen@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,16 @@
 # AutoGen
 [📚 Cite paper](#related-papers).
 <!-- <p align="center">
     <img src="https://github.com/microsoft/autogen/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p> -->
 
+:warning: Jan 23: **Breaking Change in Latest Release v0.2.8** `use_docker` defaults to `True` for code-execution. See [blog post](https://microsoft.github.io/autogen/blog/2024/01/23/Code-execution-in-docker) for details and [FAQ](https://microsoft.github.io/autogen/docs/FAQ#agents-are-throwing-due-to-docker-not-running-how-can-i-resolve-this) for troubleshooting any issues.
+
 :fire: Dec 31: [AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation Framework](https://arxiv.org/abs/2308.08155) is selected by [TheSequence: My Five Favorite AI Papers of 2023](https://thesequence.substack.com/p/my-five-favorite-ai-papers-of-2023).
 
 <!-- :fire: Nov 24: pyautogen [v0.2](https://github.com/microsoft/autogen/releases/tag/v0.2.0) is released with many updates and new features compared to v0.1.1. It switches to using openai-python v1. Please read the [migration guide](https://microsoft.github.io/autogen/docs/Installation#python). -->
 
 <!-- :fire: Nov 11: OpenAI's Assistants are available in AutoGen and interoperatable with other AutoGen agents! Checkout our [blogpost](https://microsoft.github.io/autogen/blog/2023/11/13/OAI-assistants) for details and examples. -->
 
 :fire: Nov 8: AutoGen is selected into [Open100: Top 100 Open Source achievements](https://www.benchcouncil.org/evaluation/opencs/annual.html) 35 days after spinoff.
```

### Comparing `pyautogen-0.2.8/pyautogen.egg-info/SOURCES.txt` & `pyautogen-0.2.9/pyautogen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/pyautogen.egg-info/requires.txt` & `pyautogen-0.2.9/pyautogen.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -43,14 +43,14 @@
 [test]
 coverage>=5.3
 ipykernel
 nbconvert
 nbformat
 pre-commit
 pytest-asyncio
-pytest>=6.1.1
+pytest<8,>=6.1.1
 
 [websurfer]
 beautifulsoup4
 markdownify
 pathvalidate
 pdfminer.six
```

### Comparing `pyautogen-0.2.8/pyproject.toml` & `pyautogen-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/setup.py` & `pyautogen-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         "test": [
             "coverage>=5.3",
             "ipykernel",
             "nbconvert",
             "nbformat",
             "pre-commit",
             "pytest-asyncio",
-            "pytest>=6.1.1",
+            "pytest>=6.1.1,<8",
         ],
         "blendsearch": ["flaml[blendsearch]"],
         "mathchat": ["sympy", "pydantic==1.10.9", "wolframalpha"],
         "retrievechat": ["chromadb", "sentence_transformers", "pypdf", "ipython"],
         "autobuild": ["chromadb", "sentence-transformers", "huggingface-hub"],
         "teachable": ["chromadb"],
         "lmm": ["replicate", "pillow"],
```

### Comparing `pyautogen-0.2.8/test/test_browser_utils.py` & `pyautogen-0.2.9/test/test_browser_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 import os
 import sys
 import requests
 import hashlib
 import re
+import math
 
 from agentchat.test_assistant_agent import KEY_LOC  # noqa: E402
 
 BLOG_POST_URL = "https://microsoft.github.io/autogen/blog/2023/04/21/LLM-tuning-math"
 BLOG_POST_TITLE = "Does Model and Inference Parameter Matter in LLM Applications? - A Case Study for MATH | AutoGen"
 BLOG_POST_STRING = "Large language models (LLMs) are powerful tools that can generate natural language texts for various applications, such as chatbots, summarization, translation, and more. GPT-4 is currently the state of the art LLM in the world. Is model selection irrelevant? What about inference parameters?"
 
@@ -74,15 +75,15 @@
     # Test that we can visit a page and find what we expect there
     top_viewport = browser.visit_page(BLOG_POST_URL)
     assert browser.viewport == top_viewport
     assert browser.page_title.strip() == BLOG_POST_TITLE.strip()
     assert BLOG_POST_STRING in browser.page_content
 
     # Check if page splitting works
-    approx_pages = int(len(browser.page_content) / viewport_size + 0.5)  # May be fewer, since it aligns to word breaks
+    approx_pages = math.ceil(len(browser.page_content) / viewport_size)  # May be fewer, since it aligns to word breaks
     assert len(browser.viewport_pages) <= approx_pages
     assert abs(len(browser.viewport_pages) - approx_pages) <= 1  # allow only a small deviation
     assert browser.viewport_pages[0][0] == 0
     assert browser.viewport_pages[-1][1] == len(browser.page_content)
 
     # Make sure we can reconstruct the full contents from the split pages
     buffer = ""
```

### Comparing `pyautogen-0.2.8/test/test_code.py` & `pyautogen-0.2.9/test/test_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,24 +355,26 @@
     # execute code which takes a long time
     exit_code, error, image = execute_code("import time; time.sleep(2)", timeout=1, use_docker=use_docker)
     assert exit_code and error == "Timeout" or WIN32
     assert isinstance(image, str) or docker is None or os.path.exists("/.dockerenv") or use_docker is False
 
 
 @pytest.mark.skipif(
-    sys.platform in ["win32"] or (not is_docker_running() and not in_docker_container()), reason="docker is not running"
+    sys.platform in ["win32"] or (not is_docker_running()) or in_docker_container(),
+    reason="docker is not running or in docker container already",
 )
 def test_execute_code_with_custom_filename_on_docker():
     exit_code, msg, image = execute_code("print('hello world')", filename="tmp/codetest.py", use_docker=True)
     assert exit_code == 0 and msg == "hello world\n", msg
     assert image == "python:tmp_codetest.py"
 
 
 @pytest.mark.skipif(
-    sys.platform in ["win32"] or (not is_docker_running() and not in_docker_container()), reason="docker is not running"
+    sys.platform in ["win32"] or (not is_docker_running()) or in_docker_container(),
+    reason="docker is not running or in docker container already",
 )
 def test_execute_code_with_misformed_filename_on_docker():
     exit_code, msg, image = execute_code(
         "print('hello world')", filename="tmp/codetest.py (some extra information)", use_docker=True
     )
     assert exit_code == 0 and msg == "hello world\n", msg
     assert image == "python:tmp_codetest.py__some_extra_information_"
```

### Comparing `pyautogen-0.2.8/test/test_function_utils.py` & `pyautogen-0.2.9/test/test_function_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/test/test_notebook.py` & `pyautogen-0.2.9/test/test_notebook.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/test/test_pydantic.py` & `pyautogen-0.2.9/test/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/test/test_retrieve_utils.py` & `pyautogen-0.2.9/test/test_retrieve_utils.py`

 * *Files identical despite different names*

### Comparing `pyautogen-0.2.8/test/test_token_count.py` & `pyautogen-0.2.9/test/test_token_count.py`

 * *Files identical despite different names*

