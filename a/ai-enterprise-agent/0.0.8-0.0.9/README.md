# Comparing `tmp/ai_enterprise_agent-0.0.8.tar.gz` & `tmp/ai_enterprise_agent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_enterprise_agent-0.0.8.tar", last modified: Wed Apr 24 22:29:16 2024, max compression
+gzip compressed data, was "ai_enterprise_agent-0.0.9.tar", last modified: Tue Apr 30 17:36:54 2024, max compression
```

## Comparing `ai_enterprise_agent-0.0.8.tar` & `ai_enterprise_agent-0.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.861020 ai_enterprise_agent-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-24 22:29:16.861020 ai_enterprise_agent-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/vector_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/open_api_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/orchestrator_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/sequential_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/simple_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/sql_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/vector_store_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.853021 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.857020 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/csv_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/ingestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/msft_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/pdf_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/txt_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.857020 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.857020 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/vector_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.857020 ai_enterprise_agent-0.0.8/ai_enterprise_agent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent/utils/fetch_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:29:16.861020 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 22:29:16.000000 ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:29:16.861020 ai_enterprise_agent-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-24 22:29:12.000000 ai_enterprise_agent-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.191993 ai_enterprise_agent-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-30 17:36:54.191993 ai_enterprise_agent-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.187993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.187993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/interface/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/interface/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/interface/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/interface/vector_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.187993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.187993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/open_api_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/orchestrator_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/sequential_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/simple_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/sql_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/vector_store_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.187993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chat_history/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chat_history/memory_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.191993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/msft_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/pdf_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/txt_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.191993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/llm/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/llm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/llm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.191993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.191993 ai_enterprise_agent-0.0.9/ai_enterprise_agent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent/utils/fetch_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:36:54.191993 ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-30 17:36:54.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-30 17:36:54.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:36:54.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-30 17:36:54.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 17:36:54.000000 ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 17:36:54.191993 ai_enterprise_agent-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-30 17:36:50.000000 ai_enterprise_agent-0.0.9/setup.py
```

### Comparing `ai_enterprise_agent-0.0.8/LICENSE` & `ai_enterprise_agent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/PKG-INFO` & `ai_enterprise_agent-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-enterprise-agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI Agent simplifies the implementation and use of generative AI with LangChain.
 Author: Author
 Author-email: autor@autor.com.br
 License: Apache 2.0 License
 Keywords: ai ai-agent agent assistant enterprise
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ai_enterprise_agent-0.0.8/README.md` & `ai_enterprise_agent-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/agent.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/agent.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/chat_history.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/interface/chat_history.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/interface/settings.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/interface/settings.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/chain.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/chain.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/open_api_chain.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/open_api_chain.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/orchestrator_chain.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/orchestrator_chain.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/sequential_chain.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/sequential_chain.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/simple_chain.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/simple_chain.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/sql_chain.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/sql_chain.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chains/vector_store_chain.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chains/vector_store_chain.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from typing import Any, Dict
 
 from langchain.chains.base import Chain
+from langchain.prompts import PromptTemplate
 from langchain_core.language_models.chat_models import BaseChatModel
+from langchain_core.output_parsers import StrOutputParser
+from langchain_core.runnables import RunnablePassthrough
 from langchain_core.vectorstores import VectorStore
 
 from ai_enterprise_agent.interface.chat_history import IChatHistoryService
 from ai_enterprise_agent.interface.settings import PROCESSING_TYPE, ISettings
 from ai_enterprise_agent.services.vector_store.vector_store import \
     VectorStoreFactory
 
@@ -30,19 +33,33 @@
   def __init__(self, config: ISettings, model: BaseChatModel, memory: IChatHistoryService):
     super().__init__()
     self.model = model
     self.memory = memory
     self.config = config
     self.vector_store = VectorStoreFactory.build(config=config, model=self.model)
 
-  def build_relevant_docs(self, question: str, k: int = 10):
-    return self.vector_store.similarity_search(query=question, k=k)
-
-  def chain(self):
-    pass
+  def build_relevant_docs(self, query: str, k: int = 10):
+    config = self.config.get('vector_store')
+    return self.vector_store.similarity_search(query=query, k=k, filters=config.get('custom_filters', None))
+
+  def chain(self, query: str):
+    context = self.build_relevant_docs(query)
+    template = """Use the following the context to answer the question at the end.
+    If you don't know the answer, just say that you don't know, don't try to make up an answer.
+    {context}
+    Question: {question}
+    Answer:"""
+    prompt = PromptTemplate.from_template(template)
+    return (
+      RunnablePassthrough.assign(context=lambda _: context)
+      | prompt
+      | self.model
+      | StrOutputParser()
+    )
 
   async def _call(self, input: Dict[str, Any]):
     question = input.get('question')
-    response = self.vector_store._call(question, False)
+    chain = self.chain(question)
+    response = chain.invoke(input={"question": question})
     if self.config.get('processing_type') == PROCESSING_TYPE.sequential:
-      return { self.output_key: response.get('result') }
-    return response.get('result')
+      return { self.output_key: response }
+    return response
```

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chat_history/memory.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory_chat_history.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chat_history/memory_chat_history.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/chat_history/memory_chat_redis.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/chat_history/memory_chat_redis.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/csv_loader.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/csv_loader.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/ingestion.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/ingestion.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/loader.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 from ai_enterprise_agent.services.vector_store.embedding import \
     EmbeddingFactory
 from ai_enterprise_agent.services.vector_store.vector_store import \
     VectorStoreFactory
 
 
 class CustomDocument(Document):
-  tags: Optional[str]
+  id: str
+  chat_thread_id: str
+  user: str
+  tags: str
 
 class Loader:
 
   @staticmethod
   def build(config: ISettings):
     llm_config = config.get('model')
     vector_store_config = config.get('vector_store')
@@ -33,16 +36,16 @@
     hashed_user_id = Loader.hash_user_id()
     return [CustomDocument(
       id=str(generate()),
       chat_thread_id=chat_uid,
       user=hashed_user_id,
       tags=tags,
       page_content=f"Header\nFilename:{file_name}\n{doc.page_content}",
-      metadata={"file": file_name},
-      embedding=embeddings.embed_query(text=doc.page_content),
+      metadata={"file": file_name, "tags": tags},
+      embedding=[],
     ) for doc in documents]
 
   @staticmethod
   def hash_user_id() -> str:
     value = 'aienterpriseagent'
     return hashlib.sha256(value.encode()).hexdigest()
```

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/msft_loader.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/msft_loader.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/pdf_loader.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/ingestion/txt_loader.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/ingestion/txt_loader.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/azure.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/llm/azure.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/google.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/llm/google.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/llm/model.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/llm/model.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/aws.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/aws.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Any, Iterable, List, Optional, Tuple, Type
 
-from langchain.chains.retrieval_qa.base import RetrievalQA
 from langchain_community.vectorstores.opensearch_vector_search import \
     OpenSearchVectorSearch
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.vectorstores import VectorStore
 from opensearchpy import AWSV4SignerAuth, RequestsHttpConnection
@@ -42,36 +41,32 @@
         http_auth=auth,
         timeout=100,
         use_ssl=True,
         verify_certs=True,
         connection_class=RequestsHttpConnection
     )
 
-  def similarity_search(self, query: str, k: int = 4, search_type: ISearchType = ISearchType.similarity) -> List[Document]:
+  def similarity_search(self, query: str, k: int = 4, search_type: ISearchType = ISearchType.similarity, filters:str = None) -> List[Document]:
     return self.vector_store.similarity_search(
       query=query,
       k=k,
-      search_type=search_type
+      search_type=search_type,
+      pre_filter=filters
     )
 
   def similarity_search_with_relevance_scores(self, query: str,  score_threshold: float, k: Optional[int]) -> List[Tuple[Document, float]]:
     return self.vector_store.similarity_search_with_relevance_scores(
       query=query,
       k=k,
       score_threshold=score_threshold,
     )
 
   def search(self, query: str, search_type: str, **kwargs: Any) -> List[Document]:
     return self.vector_store.search(query, search_type, **kwargs)
 
-  def _call(self, query, return_source_documents: bool = True):
-    retriever = self.vector_store.as_retriever()
-    qa = RetrievalQA.from_chain_type(self.model, chain_type="stuff", retriever=retriever, return_source_documents=return_source_documents)
-    return qa.invoke({"query": query})
-
   def add_documents(self, documents: List[Document]):
     self.vector_store.add_documents(documents=documents)
 
   def add_texts(
         self,
         texts: Iterable[str],
         metadatas: Optional[List[dict]] = None,
```

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/azure.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/azure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from typing import Any, Iterable, List, Optional, Tuple, Type
 
 from azure.search.documents.indexes.models import (SearchableField,
                                                    SearchField,
                                                    SearchFieldDataType,
                                                    SimpleField)
-from langchain.chains.retrieval_qa.base import RetrievalQA
 from langchain_community.vectorstores.azuresearch import AzureSearch
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.vectorstores import VectorStore
 
 from ai_enterprise_agent.interface.settings import VECTOR_STORE_TYPE, ISettings
 from ai_enterprise_agent.interface.vector_search import ISearchType
 from ai_enterprise_agent.services.vector_store.embedding import \
     EmbeddingFactory
 
 
+class CustomDocument(Document):
+  id: str
+  chat_thread_id: str
+  user: str
+  tags: str
+
 class AzureVectorSearch(VectorStore):
 
   def __init__(self, config: ISettings, model: BaseChatModel) -> None:
     super().__init__()
     self.config = config
     self.model = model
     self.vector_store = self.build()
@@ -29,14 +34,15 @@
     config = self.config.get('vector_store')
     embeddings = EmbeddingFactory.build(VECTOR_STORE_TYPE.azure_search, self.config)
 
     fields = [
       SimpleField(name='id', type=SearchFieldDataType.String, key=True, filterable=True),
       SearchableField(name=config.get('fields_content', 'content'), type=SearchFieldDataType.String),
       SearchField(name=config.get('fields_content_vector', 'content_vector'), type=SearchFieldDataType.Collection(SearchFieldDataType.Single), searchable=True, vector_search_dimensions=len(embeddings.embed_query("Text")), vector_search_profile_name=config.get('vector_search_profile_name')),
+      SearchableField(name='tags', type=SearchFieldDataType.String, searchable=True, filterable=True, sortable=True),
       SearchableField(name='metadata', type=SearchFieldDataType.String),
     ]
 
     return AzureSearch(
       azure_search_endpoint=config.get('endpoint'),
       azure_search_key=config.get('api_key'),
       index_name=config.get('index_name'),
@@ -48,31 +54,27 @@
     return self.vector_store.similarity_search(
       query=query,
       k=k,
       search_type=search_type,
       filters=filters
     )
 
-  def similarity_search_with_relevance_scores(self, query: str,  score_threshold: float, k: Optional[int]) -> List[Tuple[Document, float]]:
+  def similarity_search_with_relevance_scores(self, query: str,  score_threshold: float, k: Optional[int], **kwargs) -> List[Tuple[Document, float]]:
     return self.vector_store.similarity_search_with_relevance_scores(
       query=query,
       k=k,
       score_threshold=score_threshold,
+      **kwargs
     )
 
   def search(self, query: str, search_type: str = ISearchType.similarity, **kwargs: Any) -> List[Document]:
     return self.vector_store.search(query, search_type, **kwargs)
 
-  def _call(self, query, return_source_documents: bool = True):
-    retriever = self.vector_store.as_retriever()
-    qa = RetrievalQA.from_chain_type(self.model, chain_type="stuff", retriever=retriever, return_source_documents=return_source_documents)
-    return qa.invoke({"query": query})
-
-  def add_documents(self, documents: List[Document]):
-    self.vector_store.add_documents(documents=documents)
+  def add_documents(self, documents: List[CustomDocument]):
+    return self.vector_store.add_documents(documents=documents)
 
   def add_texts(
         self,
         texts: Iterable[str],
         metadatas: Optional[List[dict]] = None,
         **kwargs: Any,
     ) -> List[str]:
```

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/embedding.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/embedding.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/pinecone.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/pinecone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Any, Iterable, List, Optional, Tuple, Type
 
-from langchain.chains.retrieval_qa.base import RetrievalQA
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.vectorstores import VectorStore
 from langchain_pinecone.vectorstores import PineconeVectorStore
 
 from ai_enterprise_agent.interface.settings import VECTOR_STORE_TYPE, ISettings
@@ -22,35 +21,31 @@
     self.vector_store = self.build()
 
   def build(self):
     config = self.config('vector_store')
     embeddings = EmbeddingFactory.build(VECTOR_STORE_TYPE.pinecone, self.config)
     return PineconeVectorStore(pinecone_api_key=config.get('api_key'), embedding=embeddings, index_name=config.get('index_name'))
 
-  def similarity_search(self, query: str, k: int = 4) -> List[Document]:
+  def similarity_search(self, query: str, k: int = 4, filters:str = None) -> List[Document]:
     return self.vector_store.similarity_search(
       query=query,
       k=k,
+      filter=filters
     )
 
   def similarity_search_with_relevance_scores(self, query: str,  score_threshold: float, k: Optional[int]) -> List[Tuple[Document, float]]:
     return self.vector_store.similarity_search_with_relevance_scores(
       query=query,
       k=k,
       score_threshold=score_threshold,
     )
 
   def search(self, query: str, search_type: str = ISearchType.similarity, **kwargs: Any) -> List[Document]:
     return self.vector_store.search(query, search_type, **kwargs)
 
-  def _call(self, query, return_source_documents: bool = True):
-    retriever = self.vector_store.as_retriever()
-    qa = RetrievalQA.from_chain_type(self.model, chain_type="stuff", retriever=retriever, return_source_documents=return_source_documents)
-    return qa.invoke({"query": query})
-
   def add_documents(self, documents: List[Document]):
     self.vector_store.add_documents(documents=documents)
 
   def add_texts(
         self,
         texts: Iterable[str],
         metadatas: Optional[List[dict]] = None,
```

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/services/vector_store/vector_store.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/services/vector_store/vector_store.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent/utils/fetch_helper.py` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent/utils/fetch_helper.py`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/PKG-INFO` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-enterprise-agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI Agent simplifies the implementation and use of generative AI with LangChain.
 Author: Author
 Author-email: autor@autor.com.br
 License: Apache 2.0 License
 Keywords: ai ai-agent agent assistant enterprise
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/SOURCES.txt` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/ai_enterprise_agent.egg-info/requires.txt` & `ai_enterprise_agent-0.0.9/ai_enterprise_agent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.8/setup.py` & `ai_enterprise_agent-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='ai-enterprise-agent',
-    version='0.0.8',
+    version='0.0.9',
     license='Apache 2.0 License',
     author='Author',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='autor@autor.com.br',
     keywords='ai ai-agent agent assistant enterprise',
     description='AI Agent simplifies the implementation and use of generative AI with LangChain.',
```

