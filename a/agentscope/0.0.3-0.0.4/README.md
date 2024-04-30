# Comparing `tmp/agentscope-0.0.3.tar.gz` & `tmp/agentscope-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentscope-0.0.3.tar", last modified: Wed Apr  3 10:22:54 2024, max compression
+gzip compressed data, was "agentscope-0.0.4.tar", last modified: Tue Apr 30 09:48:10 2024, max compression
```

## Comparing `agentscope-0.0.3.tar` & `agentscope-0.0.4.tar`

### file list

```diff
@@ -1,123 +1,140 @@
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.059185 agentscope-0.0.3/
--rw-r--r--   0 pxc        (502) staff       (20)    20637 2024-03-27 12:19:57.000000 agentscope-0.0.3/LICENSE
--rw-r--r--   0 pxc        (502) staff       (20)    22430 2024-04-03 10:22:54.058112 agentscope-0.0.3/PKG-INFO
--rw-r--r--   0 pxc        (502) staff       (20)    17712 2024-04-03 10:07:59.000000 agentscope-0.0.3/README.md
--rw-r--r--   0 pxc        (502) staff       (20)     3589 2024-03-27 12:19:57.000000 agentscope-0.0.3/pyproject.toml
--rw-r--r--   0 pxc        (502) staff       (20)       38 2024-04-03 10:22:54.059276 agentscope-0.0.3/setup.cfg
--rw-r--r--   0 pxc        (502) staff       (20)     2876 2024-04-03 10:17:20.000000 agentscope-0.0.3/setup.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:53.994984 agentscope-0.0.3/src/
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.003397 agentscope-0.0.3/src/agentscope/
--rw-r--r--   0 pxc        (502) staff       (20)      356 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     6434 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/_init.py
--rw-r--r--   0 pxc        (502) staff       (20)     2261 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/_runtime.py
--rw-r--r--   0 pxc        (502) staff       (20)       77 2024-04-03 10:08:40.000000 agentscope-0.0.3/src/agentscope/_version.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.008517 agentscope-0.0.3/src/agentscope/agents/
--rw-r--r--   0 pxc        (502) staff       (20)      572 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/agents/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     8263 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/agents/agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     3192 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/agents/dialog_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     7238 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/agents/dict_dialog_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)      546 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/agents/operator.py
--rw-r--r--   0 pxc        (502) staff       (20)    11512 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/agents/react_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)    24390 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/agents/rpc_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     1926 2024-03-29 10:49:20.000000 agentscope-0.0.3/src/agentscope/agents/text_to_image_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     3495 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/agents/user_agent.py
--rw-r--r--   0 pxc        (502) staff       (20)     1395 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/constants.py
--rw-r--r--   0 pxc        (502) staff       (20)     5379 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/file_manager.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.009508 agentscope-0.0.3/src/agentscope/memory/
--rw-r--r--   0 pxc        (502) staff       (20)      200 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/memory/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     2313 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/memory/memory.py
--rw-r--r--   0 pxc        (502) staff       (20)     9381 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/memory/temporary_memory.py
--rw-r--r--   0 pxc        (502) staff       (20)    12899 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/message.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.013268 agentscope-0.0.3/src/agentscope/models/
--rw-r--r--   0 pxc        (502) staff       (20)     4960 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     1747 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/models/config.py
--rw-r--r--   0 pxc        (502) staff       (20)    18952 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/dashscope_model.py
--rw-r--r--   0 pxc        (502) staff       (20)    11877 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/gemini_model.py
--rw-r--r--   0 pxc        (502) staff       (20)     9505 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/model.py
--rw-r--r--   0 pxc        (502) staff       (20)    14770 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/ollama_model.py
--rw-r--r--   0 pxc        (502) staff       (20)    15637 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/openai_model.py
--rw-r--r--   0 pxc        (502) staff       (20)     8299 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/post_model.py
--rw-r--r--   0 pxc        (502) staff       (20)     4879 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/models/response.py
--rw-r--r--   0 pxc        (502) staff       (20)     5007 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/msghub.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.014603 agentscope-0.0.3/src/agentscope/pipelines/
--rw-r--r--   0 pxc        (502) staff       (20)      520 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/pipelines/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     5435 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/pipelines/functional.py
--rw-r--r--   0 pxc        (502) staff       (20)     8182 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/pipelines/pipeline.py
--rw-r--r--   0 pxc        (502) staff       (20)     6533 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/prompt.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.015995 agentscope-0.0.3/src/agentscope/rpc/
--rw-r--r--   0 pxc        (502) staff       (20)      775 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/rpc/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     4150 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/rpc/rpc_agent_client.py
--rw-r--r--   0 pxc        (502) staff       (20)     1271 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/rpc/rpc_agent_pb2.py
--rw-r--r--   0 pxc        (502) staff       (20)     2406 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/rpc/rpc_agent_pb2_grpc.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.017915 agentscope-0.0.3/src/agentscope/service/
--rw-r--r--   0 pxc        (502) staff       (20)     1683 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/__init__.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.018581 agentscope-0.0.3/src/agentscope/service/execute_code/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/execute_code/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)    14781 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/execute_code/exec_python.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.020835 agentscope-0.0.3/src/agentscope/service/file/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/file/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     6125 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/file/common.py
--rw-r--r--   0 pxc        (502) staff       (20)     2320 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/file/json.py
--rw-r--r--   0 pxc        (502) staff       (20)     1921 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/file/text.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.021582 agentscope-0.0.3/src/agentscope/service/retrieval/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/retrieval/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     2908 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/retrieval/retrieval_from_list.py
--rw-r--r--   0 pxc        (502) staff       (20)      926 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/retrieval/similarity.py
--rw-r--r--   0 pxc        (502) staff       (20)     6009 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/service/service_factory.py
--rw-r--r--   0 pxc        (502) staff       (20)      911 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/service_response.py
--rw-r--r--   0 pxc        (502) staff       (20)      204 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/service_status.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.022609 agentscope-0.0.3/src/agentscope/service/sql_query/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/sql_query/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     2350 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/sql_query/mongodb.py
--rw-r--r--   0 pxc        (502) staff       (20)     2922 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/sql_query/mysql.py
--rw-r--r--   0 pxc        (502) staff       (20)     2263 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/sql_query/sqlite.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.023306 agentscope-0.0.3/src/agentscope/service/text_processing/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/text_processing/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     3177 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/service/text_processing/summarization.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.024812 agentscope-0.0.3/src/agentscope/service/web_search/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/web_search/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     6711 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/service/web_search/search.py
--rw-r--r--   0 pxc        (502) staff       (20)     8694 2024-03-29 10:49:20.000000 agentscope-0.0.3/src/agentscope/service/web_search/web_digest.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.028085 agentscope-0.0.3/src/agentscope/utils/
--rw-r--r--   0 pxc        (502) staff       (20)      315 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/utils/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     5827 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/utils/common.py
--rw-r--r--   0 pxc        (502) staff       (20)     7795 2024-04-03 10:07:59.000000 agentscope-0.0.3/src/agentscope/utils/logging_utils.py
--rw-r--r--   0 pxc        (502) staff       (20)    19513 2024-03-29 10:20:14.000000 agentscope-0.0.3/src/agentscope/utils/monitor.py
--rw-r--r--   0 pxc        (502) staff       (20)     5149 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/utils/token_utils.py
--rw-r--r--   0 pxc        (502) staff       (20)     5463 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/utils/tools.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.029397 agentscope-0.0.3/src/agentscope/web/
--rw-r--r--   0 pxc        (502) staff       (20)      116 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     3102 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/_app.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:53.998188 agentscope-0.0.3/src/agentscope/web/static/
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.032927 agentscope-0.0.3/src/agentscope/web/static/css/
--rw-r--r--   0 pxc        (502) staff       (20)   155751 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/bootstrap.min.css
--rw-r--r--   0 pxc        (502) staff       (20)      614 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/colors.css
--rw-r--r--   0 pxc        (502) staff       (20)     2948 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/components.css
--rw-r--r--   0 pxc        (502) staff       (20)      208 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/fonts.css
--rw-r--r--   0 pxc        (502) staff       (20)     4807 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/home.css
--rw-r--r--   0 pxc        (502) staff       (20)     6675 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/run.css
--rw-r--r--   0 pxc        (502) staff       (20)     1129 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/css/size.css
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.036516 agentscope-0.0.3/src/agentscope/web/static/fonts/
--rw-r--r--   0 pxc        (502) staff       (20)    11860 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/fonts/KRYPTON.ttf
--rw-r--r--   0 pxc        (502) staff       (20)   169108 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/fonts/OSWALD.ttf
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.045429 agentscope-0.0.3/src/agentscope/web/static/htmls/
--rw-r--r--   0 pxc        (502) staff       (20)      368 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/htmls/agent-chat-item.html
--rw-r--r--   0 pxc        (502) staff       (20)      330 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/htmls/user-chat-item.html
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.050545 agentscope-0.0.3/src/agentscope/web/static/js/
--rw-r--r--   0 pxc        (502) staff       (20)   193910 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/bootstrap-table.min.js
--rw-r--r--   0 pxc        (502) staff       (20)   122129 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 pxc        (502) staff       (20)     7162 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/home.js
--rw-r--r--   0 pxc        (502) staff       (20)   137490 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/jquery-3.3.1.min.js
--rw-r--r--   0 pxc        (502) staff       (20)     7339 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/run.js
--rw-r--r--   0 pxc        (502) staff       (20)   177905 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/static/js/socket.io.js
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.053417 agentscope-0.0.3/src/agentscope/web/studio/
--rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/studio/__init__.py
--rw-r--r--   0 pxc        (502) staff       (20)     9329 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/studio/studio.py
--rw-r--r--   0 pxc        (502) staff       (20)     6073 2024-03-27 12:19:57.000000 agentscope-0.0.3/src/agentscope/web/studio/utils.py
-drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-03 10:22:54.005261 agentscope-0.0.3/src/agentscope.egg-info/
--rw-r--r--   0 pxc        (502) staff       (20)    22430 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/PKG-INFO
--rw-r--r--   0 pxc        (502) staff       (20)     3629 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/SOURCES.txt
--rw-r--r--   0 pxc        (502) staff       (20)        1 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/dependency_links.txt
--rw-r--r--   0 pxc        (502) staff       (20)       67 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/entry_points.txt
--rw-r--r--   0 pxc        (502) staff       (20)     1218 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/requires.txt
--rw-r--r--   0 pxc        (502) staff       (20)       11 2024-04-03 10:22:53.000000 agentscope-0.0.3/src/agentscope.egg-info/top_level.txt
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.661181 agentscope-0.0.4/
+-rw-r--r--   0 pxc        (502) staff       (20)    20637 2024-03-27 12:19:57.000000 agentscope-0.0.4/LICENSE
+-rw-r--r--   0 pxc        (502) staff       (20)    27097 2024-04-30 09:48:10.660324 agentscope-0.0.4/PKG-INFO
+-rw-r--r--   0 pxc        (502) staff       (20)    22177 2024-04-30 09:47:49.000000 agentscope-0.0.4/README.md
+-rw-r--r--   0 pxc        (502) staff       (20)     3589 2024-03-27 12:19:57.000000 agentscope-0.0.4/pyproject.toml
+-rw-r--r--   0 pxc        (502) staff       (20)       38 2024-04-30 09:48:10.661282 agentscope-0.0.4/setup.cfg
+-rw-r--r--   0 pxc        (502) staff       (20)     3014 2024-04-30 09:27:49.000000 agentscope-0.0.4/setup.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.430311 agentscope-0.0.4/src/
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.454766 agentscope-0.0.4/src/agentscope/
+-rw-r--r--   0 pxc        (502) staff       (20)      444 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     7037 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/_init.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2261 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/_runtime.py
+-rw-r--r--   0 pxc        (502) staff       (20)       77 2024-04-30 09:47:49.000000 agentscope-0.0.4/src/agentscope/_version.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.486338 agentscope-0.0.4/src/agentscope/agents/
+-rw-r--r--   0 pxc        (502) staff       (20)      624 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/agents/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)    14932 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/agents/agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3263 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/agents/dialog_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     7281 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/agents/dict_dialog_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)      546 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/agents/operator.py
+-rw-r--r--   0 pxc        (502) staff       (20)    10106 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/agents/react_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)    27503 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/agents/rpc_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1926 2024-03-29 10:49:20.000000 agentscope-0.0.4/src/agentscope/agents/text_to_image_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3495 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/agents/user_agent.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1395 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/constants.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2771 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/exception.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5320 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/file_manager.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.491497 agentscope-0.0.4/src/agentscope/memory/
+-rw-r--r--   0 pxc        (502) staff       (20)      200 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/memory/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2313 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/memory/memory.py
+-rw-r--r--   0 pxc        (502) staff       (20)     9381 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/memory/temporary_memory.py
+-rw-r--r--   0 pxc        (502) staff       (20)    13457 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/message.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.513098 agentscope-0.0.4/src/agentscope/models/
+-rw-r--r--   0 pxc        (502) staff       (20)     4628 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/models/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1747 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/models/config.py
+-rw-r--r--   0 pxc        (502) staff       (20)    29715 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/models/dashscope_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)    11938 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/models/gemini_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)    10171 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/models/model.py
+-rw-r--r--   0 pxc        (502) staff       (20)    14900 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/models/ollama_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)    15976 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/models/openai_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)     8688 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/models/post_model.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2629 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/models/response.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5011 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/msghub.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.528814 agentscope-0.0.4/src/agentscope/parsers/
+-rw-r--r--   0 pxc        (502) staff       (20)      513 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/parsers/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1610 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/parsers/code_block_parser.py
+-rw-r--r--   0 pxc        (502) staff       (20)     7217 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/parsers/json_object_parser.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2102 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/parsers/parser_base.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5109 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/parsers/tagged_content_parser.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.538681 agentscope-0.0.4/src/agentscope/pipelines/
+-rw-r--r--   0 pxc        (502) staff       (20)      644 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/pipelines/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5435 2024-03-29 10:20:14.000000 agentscope-0.0.4/src/agentscope/pipelines/functional.py
+-rw-r--r--   0 pxc        (502) staff       (20)     8182 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/pipelines/pipeline.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6587 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/prompt.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.548154 agentscope-0.0.4/src/agentscope/rpc/
+-rw-r--r--   0 pxc        (502) staff       (20)      775 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/rpc/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     4266 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/rpc/rpc_agent_client.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1271 2024-04-03 10:07:59.000000 agentscope-0.0.4/src/agentscope/rpc/rpc_agent_pb2.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2406 2024-04-03 10:07:59.000000 agentscope-0.0.4/src/agentscope/rpc/rpc_agent_pb2_grpc.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.551334 agentscope-0.0.4/src/agentscope/service/
+-rw-r--r--   0 pxc        (502) staff       (20)     2101 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/__init__.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.555053 agentscope-0.0.4/src/agentscope/service/execute_code/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/execute_code/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)    14781 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/execute_code/exec_python.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1861 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/execute_code/exec_shell.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.566574 agentscope-0.0.4/src/agentscope/service/file/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/file/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     7915 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/file/common.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2320 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/file/json.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1921 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/file/text.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.568621 agentscope-0.0.4/src/agentscope/service/retrieval/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/retrieval/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2908 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/retrieval/retrieval_from_list.py
+-rw-r--r--   0 pxc        (502) staff       (20)      926 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/retrieval/similarity.py
+-rw-r--r--   0 pxc        (502) staff       (20)      911 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/service_response.py
+-rw-r--r--   0 pxc        (502) staff       (20)      204 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/service_status.py
+-rw-r--r--   0 pxc        (502) staff       (20)    24734 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/service_toolkit.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.574101 agentscope-0.0.4/src/agentscope/service/sql_query/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/sql_query/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2350 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/sql_query/mongodb.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2925 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/sql_query/mysql.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2266 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/sql_query/sqlite.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.575030 agentscope-0.0.4/src/agentscope/service/text_processing/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/service/text_processing/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3177 2024-03-29 10:20:14.000000 agentscope-0.0.4/src/agentscope/service/text_processing/summarization.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.583666 agentscope-0.0.4/src/agentscope/service/web/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/web/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     8811 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/web/arxiv.py
+-rw-r--r--   0 pxc        (502) staff       (20)     2339 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/web/download.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6711 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/web/search.py
+-rw-r--r--   0 pxc        (502) staff       (20)     8720 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/service/web/web_digest.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.592111 agentscope-0.0.4/src/agentscope/utils/
+-rw-r--r--   0 pxc        (502) staff       (20)      315 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/utils/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5778 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/utils/common.py
+-rw-r--r--   0 pxc        (502) staff       (20)     7765 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/utils/logging_utils.py
+-rw-r--r--   0 pxc        (502) staff       (20)    21077 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/utils/monitor.py
+-rw-r--r--   0 pxc        (502) staff       (20)     5149 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/utils/token_utils.py
+-rw-r--r--   0 pxc        (502) staff       (20)     7840 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/utils/tools.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.593808 agentscope-0.0.4/src/agentscope/web/
+-rw-r--r--   0 pxc        (502) staff       (20)      116 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3102 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/_app.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.438873 agentscope-0.0.4/src/agentscope/web/static/
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.605901 agentscope-0.0.4/src/agentscope/web/static/css/
+-rw-r--r--   0 pxc        (502) staff       (20)   155751 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/css/bootstrap.min.css
+-rw-r--r--   0 pxc        (502) staff       (20)      614 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/css/colors.css
+-rw-r--r--   0 pxc        (502) staff       (20)     2948 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/css/components.css
+-rw-r--r--   0 pxc        (502) staff       (20)      208 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/css/fonts.css
+-rw-r--r--   0 pxc        (502) staff       (20)     4807 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/css/home.css
+-rw-r--r--   0 pxc        (502) staff       (20)     6675 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/css/run.css
+-rw-r--r--   0 pxc        (502) staff       (20)     1129 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/css/size.css
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.611005 agentscope-0.0.4/src/agentscope/web/static/fonts/
+-rw-r--r--   0 pxc        (502) staff       (20)    11860 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/fonts/KRYPTON.ttf
+-rw-r--r--   0 pxc        (502) staff       (20)   169108 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/fonts/OSWALD.ttf
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.621843 agentscope-0.0.4/src/agentscope/web/static/htmls/
+-rw-r--r--   0 pxc        (502) staff       (20)      368 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/htmls/agent-chat-item.html
+-rw-r--r--   0 pxc        (502) staff       (20)      330 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/htmls/user-chat-item.html
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.633265 agentscope-0.0.4/src/agentscope/web/static/js/
+-rw-r--r--   0 pxc        (502) staff       (20)   193910 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/js/bootstrap-table.min.js
+-rw-r--r--   0 pxc        (502) staff       (20)   122129 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 pxc        (502) staff       (20)     7162 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/js/home.js
+-rw-r--r--   0 pxc        (502) staff       (20)   137490 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0 pxc        (502) staff       (20)     7339 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/js/run.js
+-rw-r--r--   0 pxc        (502) staff       (20)   177905 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/static/js/socket.io.js
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.638329 agentscope-0.0.4/src/agentscope/web/studio/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-03-27 12:19:57.000000 agentscope-0.0.4/src/agentscope/web/studio/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)       90 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/web/studio/constants.py
+-rw-r--r--   0 pxc        (502) staff       (20)    10549 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/web/studio/studio.py
+-rw-r--r--   0 pxc        (502) staff       (20)     6464 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/web/studio/utils.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.653171 agentscope-0.0.4/src/agentscope/web/workstation/
+-rw-r--r--   0 pxc        (502) staff       (20)        0 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/web/workstation/__init__.py
+-rw-r--r--   0 pxc        (502) staff       (20)     3131 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/web/workstation/workflow.py
+-rw-r--r--   0 pxc        (502) staff       (20)    10877 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/web/workstation/workflow_dag.py
+-rw-r--r--   0 pxc        (502) staff       (20)    26576 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/web/workstation/workflow_node.py
+-rw-r--r--   0 pxc        (502) staff       (20)     1086 2024-04-30 09:27:49.000000 agentscope-0.0.4/src/agentscope/web/workstation/workflow_utils.py
+drwxr-xr-x   0 pxc        (502) staff       (20)        0 2024-04-30 09:48:10.470979 agentscope-0.0.4/src/agentscope.egg-info/
+-rw-r--r--   0 pxc        (502) staff       (20)    27097 2024-04-30 09:48:10.000000 agentscope-0.0.4/src/agentscope.egg-info/PKG-INFO
+-rw-r--r--   0 pxc        (502) staff       (20)     4240 2024-04-30 09:48:10.000000 agentscope-0.0.4/src/agentscope.egg-info/SOURCES.txt
+-rw-r--r--   0 pxc        (502) staff       (20)        1 2024-04-30 09:48:10.000000 agentscope-0.0.4/src/agentscope.egg-info/dependency_links.txt
+-rw-r--r--   0 pxc        (502) staff       (20)      122 2024-04-30 09:48:10.000000 agentscope-0.0.4/src/agentscope.egg-info/entry_points.txt
+-rw-r--r--   0 pxc        (502) staff       (20)     1254 2024-04-30 09:48:10.000000 agentscope-0.0.4/src/agentscope.egg-info/requires.txt
+-rw-r--r--   0 pxc        (502) staff       (20)       11 2024-04-30 09:48:10.000000 agentscope-0.0.4/src/agentscope.egg-info/top_level.txt
```

### Comparing `agentscope-0.0.3/LICENSE` & `agentscope-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/PKG-INFO` & `agentscope-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agentscope
-Version: 0.0.3
+Version: 0.0.4
 Summary: AgentScope: A Flexible yet Robust Multi-Agent Platform.
 Home-page: https://github.com/modelscope/agentscope
-Download-URL: https://github.com/modelscope/agentscope/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/modelscope/agentscope/archive/v0.0.4.tar.gz
 Author: SysML team of Alibaba Tongyi Lab 
 Author-email: gaodawei.gdw@alibaba-inc.com
 License: Apache License 2.0
 Keywords: deep-learning,multi agents,agents
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -49,14 +49,15 @@
 Requires-Dist: openai>=1.3.0; extra == "distribute"
 Requires-Dist: ollama>=0.1.7; extra == "distribute"
 Requires-Dist: google-generativeai>=0.4.0; extra == "distribute"
 Requires-Dist: grpcio==1.60.0; extra == "distribute"
 Requires-Dist: grpcio-tools==1.60.0; extra == "distribute"
 Requires-Dist: protobuf==4.25.0; extra == "distribute"
 Requires-Dist: expiringdict; extra == "distribute"
+Requires-Dist: dill; extra == "distribute"
 Provides-Extra: dev
 Requires-Dist: docstring_parser; extra == "dev"
 Requires-Dist: loguru==0.6.0; extra == "dev"
 Requires-Dist: tiktoken; extra == "dev"
 Requires-Dist: Pillow; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: chardet; extra == "dev"
@@ -90,38 +91,42 @@
 Requires-Dist: openai>=1.3.0; extra == "full"
 Requires-Dist: ollama>=0.1.7; extra == "full"
 Requires-Dist: google-generativeai>=0.4.0; extra == "full"
 Requires-Dist: grpcio==1.60.0; extra == "full"
 Requires-Dist: grpcio-tools==1.60.0; extra == "full"
 Requires-Dist: protobuf==4.25.0; extra == "full"
 Requires-Dist: expiringdict; extra == "full"
+Requires-Dist: dill; extra == "full"
 Requires-Dist: docker; extra == "full"
 Requires-Dist: pymongo; extra == "full"
 Requires-Dist: pymysql; extra == "full"
 Requires-Dist: beautifulsoup4; extra == "full"
+Requires-Dist: feedparser; extra == "full"
 Requires-Dist: sphinx; extra == "full"
 Requires-Dist: sphinx-autobuild; extra == "full"
 Requires-Dist: sphinx_rtd_theme; extra == "full"
 Requires-Dist: myst-parser; extra == "full"
 Requires-Dist: sphinxcontrib-mermaid; extra == "full"
 Requires-Dist: pytest; extra == "full"
 Requires-Dist: pytest-cov; extra == "full"
 Requires-Dist: pre-commit; extra == "full"
+Requires-Dist: networkx; extra == "full"
 Requires-Dist: gradio==4.19.1; extra == "full"
 Requires-Dist: modelscope_studio==0.0.5; extra == "full"
+Requires-Dist: black; extra == "full"
 
 English | [**中文**](README_ZH.md)
 
 # AgentScope
 
 Start building LLM-empowered multi-agent applications in an easier way.
 
 [![](https://img.shields.io/badge/cs.MA-2402.14034-B31C1C?logo=arxiv&logoColor=B31C1C)](https://arxiv.org/abs/2402.14034)
 [![](https://img.shields.io/badge/python-3.9+-blue)](https://pypi.org/project/agentscope/)
-[![](https://img.shields.io/badge/pypi-v0.0.2-blue?logo=pypi)](https://pypi.org/project/agentscope/)
+[![](https://img.shields.io/badge/pypi-v0.0.4-blue?logo=pypi)](https://pypi.org/project/agentscope/)
 [![](https://img.shields.io/badge/Docs-English%7C%E4%B8%AD%E6%96%87-blue?logo=markdown)](https://modelscope.github.io/agentscope/#welcome-to-agentscope-tutorial-hub)
 [![](https://img.shields.io/badge/Docs-API_Reference-blue?logo=markdown)](https://modelscope.github.io/agentscope/)
 [![](https://img.shields.io/badge/ModelScope-Demos-4e29ff.svg?logo=data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjI0IDEyMS4zMyIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxwYXRoIGQ9Im0wIDQ3Ljg0aDI1LjY1djI1LjY1aC0yNS42NXoiIGZpbGw9IiM2MjRhZmYiIC8+Cgk8cGF0aCBkPSJtOTkuMTQgNzMuNDloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzYyNGFmZiIgLz4KCTxwYXRoIGQ9Im0xNzYuMDkgOTkuMTRoLTI1LjY1djIyLjE5aDQ3Ljg0di00Ny44NGgtMjIuMTl6IiBmaWxsPSIjNjI0YWZmIiAvPgoJPHBhdGggZD0ibTEyNC43OSA0Ny44NGgyNS42NXYyNS42NWgtMjUuNjV6IiBmaWxsPSIjMzZjZmQxIiAvPgoJPHBhdGggZD0ibTAgMjIuMTloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzM2Y2ZkMSIgLz4KCTxwYXRoIGQ9Im0xOTguMjggNDcuODRoMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzYyNGFmZiIgLz4KCTxwYXRoIGQ9Im0xOTguMjggMjIuMTloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzM2Y2ZkMSIgLz4KCTxwYXRoIGQ9Im0xNTAuNDQgMHYyMi4xOWgyNS42NXYyNS42NWgyMi4xOXYtNDcuODR6IiBmaWxsPSIjNjI0YWZmIiAvPgoJPHBhdGggZD0ibTczLjQ5IDQ3Ljg0aDI1LjY1djI1LjY1aC0yNS42NXoiIGZpbGw9IiMzNmNmZDEiIC8+Cgk8cGF0aCBkPSJtNDcuODQgMjIuMTloMjUuNjV2LTIyLjE5aC00Ny44NHY0Ny44NGgyMi4xOXoiIGZpbGw9IiM2MjRhZmYiIC8+Cgk8cGF0aCBkPSJtNDcuODQgNzMuNDloLTIyLjE5djQ3Ljg0aDQ3Ljg0di0yMi4xOWgtMjUuNjV6IiBmaWxsPSIjNjI0YWZmIiAvPgo8L3N2Zz4K)](https://modelscope.cn/studios?name=agentscope&page=1&sort=latest)
 
 [![](https://img.shields.io/badge/license-Apache--2.0-black)](./LICENSE)
 [![](https://img.shields.io/badge/Contribute-Welcome-green)](https://modelscope.github.io/agentscope/tutorial/contribute.html)
 
@@ -134,65 +139,73 @@
 |----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
 | <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> |
 
 ----
 
 ## News
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] We release **AgentScope** v0.0.2 now! In this new version,
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-30]** We release **AgentScope** v0.0.4 now!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-27]** [AgentScope Workstation](https://agentscope.aliyun.com/) is now online! You are welcome to try building your multi-agent application simply with our *drag-and-drop platform* and ask our *copilot* questions about AgentScope!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-19]** AgentScope supports Llama3 now! We provide [scripts](./examples/model_llama3) and example [model configuration](./examples/model_llama3) for quick set-up. Feel free to try llama3 in our examples!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-06]** We release **AgentScope** v0.0.3 now!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-06]** New examples [Gomoku](./examples/game_gomoku), [Conversation with ReAct Agent](./examples/conversation_with_react_agent), [Conversation with RAG Agent](./examples/conversation_with_RAG_agents) and [Distributed Parallel Search](./examples/distributed_search) are available now!
+
+- **[2024-03-19]** We release **AgentScope** v0.0.2 now! In this new version,
 AgentScope supports [ollama](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models)(A local CPU inference engine), [DashScope](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models) and Google [Gemini](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models) APIs.
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] New examples ["Autonomous Conversation with Mentions"](./examples/conversation_with_mentions) and ["Basic Conversation with LangChain library"](./examples/conversation_with_langchain) are available now!
+- **[2024-03-19]** New examples ["Autonomous Conversation with Mentions"](./examples/conversation_with_mentions) and ["Basic Conversation with LangChain library"](./examples/conversation_with_langchain) are available now!
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] The [Chinese tutorial](https://modelscope.github.io/agentscope/zh_CN/index.html) of AgentScope is online now!
+- **[2024-03-19]** The [Chinese tutorial](https://modelscope.github.io/agentscope/zh_CN/index.html) of AgentScope is online now!
 
-- [2024-02-27] We release **AgentScope v0.0.1** now, which is also
+- **[2024-02-27]** We release **AgentScope v0.0.1** now, which is also
 available in [PyPI](https://pypi.org/project/agentscope/)!
-- [2024-02-14] We release our paper "AgentScope: A Flexible yet Robust
+- **[2024-02-14]** We release our paper "AgentScope: A Flexible yet Robust
 Multi-Agent Platform" in [arXiv](https://arxiv.org/abs/2402.14034) now!
 
 ---
 
 ## What's AgentScope?
 
 AgentScope is an innovative multi-agent platform designed to empower developers
 to build multi-agent applications with large-scale models.
 It features three high-level capabilities:
 
 - 🤝 **Easy-to-Use**: Designed for developers, with [fruitful components](https://modelscope.github.io/agentscope/en/tutorial/204-service.html#),
-[comprehensive documentation](https://modelscope.github.io/agentscope/en/index.html), and broad compatibility.
+[comprehensive documentation](https://modelscope.github.io/agentscope/en/index.html), and broad compatibility. Besides, [AgentScope Workstation](https://agentscope.aliyun.com/) provides a *drag-and-drop programming platform* and a *copilot* for beginners of AgentScope!
 
 - ✅ **High Robustness**: Supporting customized fault-tolerance controls and
 retry mechanisms to enhance application stability.
 
 - 🚀 **Actor-Based Distribution**: Building distributed multi-agent
 applications in a centralized programming manner for streamlined development.
 
 **Supported Model Libraries**
 
 AgentScope provides a list of `ModelWrapper` to support both local model
 services and third-party model APIs.
 
-| API                    | Task            | Model Wrapper                                                                                                                   | Example Configuration                                                                       |
-|------------------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
-| OpenAI API             | Chat            | [`OpenAIChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-|                        | Embedding       | [`OpenAIEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-|                        | DALL·E          | [`OpenAIDALLEWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-| DashScope API          | Chat            | [`DashScopeChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)           | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-|                        | Image Synthesis | [`DashScopeImageSynthesisWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py) | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-|                        | Text Embedding  | [`DashScopeTextEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)  | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-| Gemini API             | Chat            | [`GeminiChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api)       |
-|                        | Embedding       | [`GeminiEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api)       |
-| ollama                 | Chat            | [`OllamaChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-|                        | Embedding       | [`OllamaEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-|                        | Generation      | [`OllamaGenerationWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)           | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-| Post Request based API | -               | [`PostAPIModelWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/post_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#post-request-api) |
+| API                    | Task            | Model Wrapper                                                                                                                   | Configuration                                                                      | Some Supported Models                         |
+|------------------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|-----------------------------------------------|
+| OpenAI API             | Chat            | [`OpenAIChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                 |[guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)  <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_chat_template.json)       | gpt-4, gpt-3.5-turbo, ...                     |
+|                        | Embedding       | [`OpenAIEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_embedding_template.json)       | text-embedding-ada-002, ...                   |
+|                        | DALL·E          | [`OpenAIDALLEWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_dall_e_template.json)       | dall-e-2, dall-e-3                            |
+| DashScope API          | Chat            | [`DashScopeChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)           | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_chat_template.json)    | qwen-plus, qwen-max, ...                      |
+|                        | Image Synthesis | [`DashScopeImageSynthesisWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py) | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)  <br>[template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_image_synthesis_template.json)    | wanx-v1                                       |
+|                        | Text Embedding  | [`DashScopeTextEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)  | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_text_embedding_template.json)    | text-embedding-v1, text-embedding-v2, ...     |
+|                        | Multimodal      | [`DashScopeMultiModalWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)     | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_multimodal_template.json)    | qwen-vl-max, qwen-vl-chat-v1, qwen-audio-chat |
+| Gemini API             | Chat            | [`GeminiChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/gemini_chat_template.json)       | gemini-pro, ...                               |
+|                        | Embedding       | [`GeminiEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/gemini_embedding_template.json)       | models/embedding-001, ...                     |
+| ollama                 | Chat            | [`OllamaChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_chat_template.json)       | llama3, llama2, Mistral, ...                  |
+|                        | Embedding       | [`OllamaEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_embedding_template.json)       | llama2, Mistral, ...                          |
+|                        | Generation      | [`OllamaGenerationWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)           | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_generate_template.json)       | llama2, Mistral, ...                          |
+| Post Request based API | -               | [`PostAPIModelWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/post_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#post-request-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/postapi_model_config_template.json) | -                                             |
 
 **Supported Local Model Deployment**
 
 AgentScope enables developers to rapidly deploy local model services using
 the following libraries.
 
 - [ollama (CPU inference)](https://github.com/modelscope/agentscope/blob/main/scripts/README.md#ollama)
@@ -208,14 +221,17 @@
 - Retrieval
 - Code Execution
 - File Operation
 - Text Processing
 
 **Example Applications**
 
+- Model
+  - <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>[Using Llama3 in AgentScope](./examples/model_llama3)
+
 - Conversation
   - [Basic Conversation](./examples/conversation_basic)
   - [Autonomous Conversation with Mentions](./examples/conversation_with_mentions)
   - [Self-Organizing Conversation](./examples/conversation_self_organizing)
   - [Basic Conversation with LangChain library](./examples/conversation_with_langchain)
   - [Conversation with ReAct Agent](./examples/conversation_with_react_agent)
   - [Conversation with RAG Agent](./examples/conversation_with_RAG_agents)
@@ -224,23 +240,24 @@
   - [Gomoku](./examples/game_gomoku)
   - [Werewolf](./examples/game_werewolf)
 
 - Distribution
   - [Distributed Conversation](./examples/distributed_basic)
   - [Distributed Debate](./examples/distributed_debate)
   - [Distributed Parallel Search](./examples/distributed_search)
+  - [Distributed Large Scale Simulation](./examples/distributed_simulation)
 
 More models, services and examples are coming soon!
 
 ## Installation
 
 AgentScope requires **Python 3.9** or higher.
 
-**_Note: This project is currently in active development, it's recommended to
-install AgentScope from source._**
+***Note: This project is currently in active development, it's recommended to
+install AgentScope from source.***
 
 ### From source
 
 - Install AgentScope in editable mode:
 
 ```bash
 # Pull the source code from GitHub
@@ -290,15 +307,15 @@
 ```
 
 Taking OpenAI Chat API as an example, the model configuration is as follows:
 
 ```python
 openai_model_config = {
     "config_name": "my_openai_config",             # The name to identify the config
-    "model_type": "openai",                        # The type to identify the model wrapper
+    "model_type": "openai_chat",                   # The type to identify the model wrapper
 
     # Detailed parameters into initialize the model wrapper
     "model_name": "gpt-4",                         # The used model in openai API, e.g. gpt-4, gpt-3.5-turbo, etc.
     "api_key": "xxx",                              # The API key for OpenAI API. If not set, env
                                                    # variable OPENAI_API_KEY will be used.
     "organization": "xxx",                         # The organization for OpenAI API. If not set, env
                                                    # variable OPENAI_ORGANIZATION will be used.
```

### Comparing `agentscope-0.0.3/README.md` & `agentscope-0.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AgentScope
 
 Start building LLM-empowered multi-agent applications in an easier way.
 
 [![](https://img.shields.io/badge/cs.MA-2402.14034-B31C1C?logo=arxiv&logoColor=B31C1C)](https://arxiv.org/abs/2402.14034)
 [![](https://img.shields.io/badge/python-3.9+-blue)](https://pypi.org/project/agentscope/)
-[![](https://img.shields.io/badge/pypi-v0.0.2-blue?logo=pypi)](https://pypi.org/project/agentscope/)
+[![](https://img.shields.io/badge/pypi-v0.0.4-blue?logo=pypi)](https://pypi.org/project/agentscope/)
 [![](https://img.shields.io/badge/Docs-English%7C%E4%B8%AD%E6%96%87-blue?logo=markdown)](https://modelscope.github.io/agentscope/#welcome-to-agentscope-tutorial-hub)
 [![](https://img.shields.io/badge/Docs-API_Reference-blue?logo=markdown)](https://modelscope.github.io/agentscope/)
 [![](https://img.shields.io/badge/ModelScope-Demos-4e29ff.svg?logo=data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjI0IDEyMS4zMyIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxwYXRoIGQ9Im0wIDQ3Ljg0aDI1LjY1djI1LjY1aC0yNS42NXoiIGZpbGw9IiM2MjRhZmYiIC8+Cgk8cGF0aCBkPSJtOTkuMTQgNzMuNDloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzYyNGFmZiIgLz4KCTxwYXRoIGQ9Im0xNzYuMDkgOTkuMTRoLTI1LjY1djIyLjE5aDQ3Ljg0di00Ny44NGgtMjIuMTl6IiBmaWxsPSIjNjI0YWZmIiAvPgoJPHBhdGggZD0ibTEyNC43OSA0Ny44NGgyNS42NXYyNS42NWgtMjUuNjV6IiBmaWxsPSIjMzZjZmQxIiAvPgoJPHBhdGggZD0ibTAgMjIuMTloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzM2Y2ZkMSIgLz4KCTxwYXRoIGQ9Im0xOTguMjggNDcuODRoMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzYyNGFmZiIgLz4KCTxwYXRoIGQ9Im0xOTguMjggMjIuMTloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzM2Y2ZkMSIgLz4KCTxwYXRoIGQ9Im0xNTAuNDQgMHYyMi4xOWgyNS42NXYyNS42NWgyMi4xOXYtNDcuODR6IiBmaWxsPSIjNjI0YWZmIiAvPgoJPHBhdGggZD0ibTczLjQ5IDQ3Ljg0aDI1LjY1djI1LjY1aC0yNS42NXoiIGZpbGw9IiMzNmNmZDEiIC8+Cgk8cGF0aCBkPSJtNDcuODQgMjIuMTloMjUuNjV2LTIyLjE5aC00Ny44NHY0Ny44NGgyMi4xOXoiIGZpbGw9IiM2MjRhZmYiIC8+Cgk8cGF0aCBkPSJtNDcuODQgNzMuNDloLTIyLjE5djQ3Ljg0aDQ3Ljg0di0yMi4xOWgtMjUuNjV6IiBmaWxsPSIjNjI0YWZmIiAvPgo8L3N2Zz4K)](https://modelscope.cn/studios?name=agentscope&page=1&sort=latest)
 
 [![](https://img.shields.io/badge/license-Apache--2.0-black)](./LICENSE)
 [![](https://img.shields.io/badge/Contribute-Welcome-green)](https://modelscope.github.io/agentscope/tutorial/contribute.html)
 
@@ -23,65 +23,73 @@
 |----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
 | <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> |
 
 ----
 
 ## News
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] We release **AgentScope** v0.0.2 now! In this new version,
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-30]** We release **AgentScope** v0.0.4 now!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-27]** [AgentScope Workstation](https://agentscope.aliyun.com/) is now online! You are welcome to try building your multi-agent application simply with our *drag-and-drop platform* and ask our *copilot* questions about AgentScope!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-19]** AgentScope supports Llama3 now! We provide [scripts](./examples/model_llama3) and example [model configuration](./examples/model_llama3) for quick set-up. Feel free to try llama3 in our examples!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-06]** We release **AgentScope** v0.0.3 now!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-06]** New examples [Gomoku](./examples/game_gomoku), [Conversation with ReAct Agent](./examples/conversation_with_react_agent), [Conversation with RAG Agent](./examples/conversation_with_RAG_agents) and [Distributed Parallel Search](./examples/distributed_search) are available now!
+
+- **[2024-03-19]** We release **AgentScope** v0.0.2 now! In this new version,
 AgentScope supports [ollama](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models)(A local CPU inference engine), [DashScope](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models) and Google [Gemini](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models) APIs.
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] New examples ["Autonomous Conversation with Mentions"](./examples/conversation_with_mentions) and ["Basic Conversation with LangChain library"](./examples/conversation_with_langchain) are available now!
+- **[2024-03-19]** New examples ["Autonomous Conversation with Mentions"](./examples/conversation_with_mentions) and ["Basic Conversation with LangChain library"](./examples/conversation_with_langchain) are available now!
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] The [Chinese tutorial](https://modelscope.github.io/agentscope/zh_CN/index.html) of AgentScope is online now!
+- **[2024-03-19]** The [Chinese tutorial](https://modelscope.github.io/agentscope/zh_CN/index.html) of AgentScope is online now!
 
-- [2024-02-27] We release **AgentScope v0.0.1** now, which is also
+- **[2024-02-27]** We release **AgentScope v0.0.1** now, which is also
 available in [PyPI](https://pypi.org/project/agentscope/)!
-- [2024-02-14] We release our paper "AgentScope: A Flexible yet Robust
+- **[2024-02-14]** We release our paper "AgentScope: A Flexible yet Robust
 Multi-Agent Platform" in [arXiv](https://arxiv.org/abs/2402.14034) now!
 
 ---
 
 ## What's AgentScope?
 
 AgentScope is an innovative multi-agent platform designed to empower developers
 to build multi-agent applications with large-scale models.
 It features three high-level capabilities:
 
 - 🤝 **Easy-to-Use**: Designed for developers, with [fruitful components](https://modelscope.github.io/agentscope/en/tutorial/204-service.html#),
-[comprehensive documentation](https://modelscope.github.io/agentscope/en/index.html), and broad compatibility.
+[comprehensive documentation](https://modelscope.github.io/agentscope/en/index.html), and broad compatibility. Besides, [AgentScope Workstation](https://agentscope.aliyun.com/) provides a *drag-and-drop programming platform* and a *copilot* for beginners of AgentScope!
 
 - ✅ **High Robustness**: Supporting customized fault-tolerance controls and
 retry mechanisms to enhance application stability.
 
 - 🚀 **Actor-Based Distribution**: Building distributed multi-agent
 applications in a centralized programming manner for streamlined development.
 
 **Supported Model Libraries**
 
 AgentScope provides a list of `ModelWrapper` to support both local model
 services and third-party model APIs.
 
-| API                    | Task            | Model Wrapper                                                                                                                   | Example Configuration                                                                       |
-|------------------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
-| OpenAI API             | Chat            | [`OpenAIChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-|                        | Embedding       | [`OpenAIEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-|                        | DALL·E          | [`OpenAIDALLEWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-| DashScope API          | Chat            | [`DashScopeChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)           | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-|                        | Image Synthesis | [`DashScopeImageSynthesisWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py) | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-|                        | Text Embedding  | [`DashScopeTextEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)  | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-| Gemini API             | Chat            | [`GeminiChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api)       |
-|                        | Embedding       | [`GeminiEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api)       |
-| ollama                 | Chat            | [`OllamaChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-|                        | Embedding       | [`OllamaEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-|                        | Generation      | [`OllamaGenerationWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)           | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-| Post Request based API | -               | [`PostAPIModelWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/post_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#post-request-api) |
+| API                    | Task            | Model Wrapper                                                                                                                   | Configuration                                                                      | Some Supported Models                         |
+|------------------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|-----------------------------------------------|
+| OpenAI API             | Chat            | [`OpenAIChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                 |[guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)  <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_chat_template.json)       | gpt-4, gpt-3.5-turbo, ...                     |
+|                        | Embedding       | [`OpenAIEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_embedding_template.json)       | text-embedding-ada-002, ...                   |
+|                        | DALL·E          | [`OpenAIDALLEWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_dall_e_template.json)       | dall-e-2, dall-e-3                            |
+| DashScope API          | Chat            | [`DashScopeChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)           | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_chat_template.json)    | qwen-plus, qwen-max, ...                      |
+|                        | Image Synthesis | [`DashScopeImageSynthesisWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py) | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)  <br>[template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_image_synthesis_template.json)    | wanx-v1                                       |
+|                        | Text Embedding  | [`DashScopeTextEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)  | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_text_embedding_template.json)    | text-embedding-v1, text-embedding-v2, ...     |
+|                        | Multimodal      | [`DashScopeMultiModalWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)     | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_multimodal_template.json)    | qwen-vl-max, qwen-vl-chat-v1, qwen-audio-chat |
+| Gemini API             | Chat            | [`GeminiChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/gemini_chat_template.json)       | gemini-pro, ...                               |
+|                        | Embedding       | [`GeminiEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/gemini_embedding_template.json)       | models/embedding-001, ...                     |
+| ollama                 | Chat            | [`OllamaChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_chat_template.json)       | llama3, llama2, Mistral, ...                  |
+|                        | Embedding       | [`OllamaEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_embedding_template.json)       | llama2, Mistral, ...                          |
+|                        | Generation      | [`OllamaGenerationWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)           | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_generate_template.json)       | llama2, Mistral, ...                          |
+| Post Request based API | -               | [`PostAPIModelWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/post_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#post-request-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/postapi_model_config_template.json) | -                                             |
 
 **Supported Local Model Deployment**
 
 AgentScope enables developers to rapidly deploy local model services using
 the following libraries.
 
 - [ollama (CPU inference)](https://github.com/modelscope/agentscope/blob/main/scripts/README.md#ollama)
@@ -97,14 +105,17 @@
 - Retrieval
 - Code Execution
 - File Operation
 - Text Processing
 
 **Example Applications**
 
+- Model
+  - <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>[Using Llama3 in AgentScope](./examples/model_llama3)
+
 - Conversation
   - [Basic Conversation](./examples/conversation_basic)
   - [Autonomous Conversation with Mentions](./examples/conversation_with_mentions)
   - [Self-Organizing Conversation](./examples/conversation_self_organizing)
   - [Basic Conversation with LangChain library](./examples/conversation_with_langchain)
   - [Conversation with ReAct Agent](./examples/conversation_with_react_agent)
   - [Conversation with RAG Agent](./examples/conversation_with_RAG_agents)
@@ -113,23 +124,24 @@
   - [Gomoku](./examples/game_gomoku)
   - [Werewolf](./examples/game_werewolf)
 
 - Distribution
   - [Distributed Conversation](./examples/distributed_basic)
   - [Distributed Debate](./examples/distributed_debate)
   - [Distributed Parallel Search](./examples/distributed_search)
+  - [Distributed Large Scale Simulation](./examples/distributed_simulation)
 
 More models, services and examples are coming soon!
 
 ## Installation
 
 AgentScope requires **Python 3.9** or higher.
 
-**_Note: This project is currently in active development, it's recommended to
-install AgentScope from source._**
+***Note: This project is currently in active development, it's recommended to
+install AgentScope from source.***
 
 ### From source
 
 - Install AgentScope in editable mode:
 
 ```bash
 # Pull the source code from GitHub
@@ -179,15 +191,15 @@
 ```
 
 Taking OpenAI Chat API as an example, the model configuration is as follows:
 
 ```python
 openai_model_config = {
     "config_name": "my_openai_config",             # The name to identify the config
-    "model_type": "openai",                        # The type to identify the model wrapper
+    "model_type": "openai_chat",                   # The type to identify the model wrapper
 
     # Detailed parameters into initialize the model wrapper
     "model_name": "gpt-4",                         # The used model in openai API, e.g. gpt-4, gpt-3.5-turbo, etc.
     "api_key": "xxx",                              # The API key for OpenAI API. If not set, env
                                                    # variable OPENAI_API_KEY will be used.
     "organization": "xxx",                         # The organization for OpenAI API. If not set, env
                                                    # variable OPENAI_ORGANIZATION will be used.
```

### Comparing `agentscope-0.0.3/pyproject.toml` & `agentscope-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/setup.py` & `agentscope-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,34 +18,41 @@
 URL = "https://github.com/modelscope/agentscope"
 
 rpc_requires = [
     "grpcio==1.60.0",
     "grpcio-tools==1.60.0",
     "protobuf==4.25.0",
     "expiringdict",
+    "dill",
 ]
 
 service_requires = [
     "docker",
     "pymongo",
     "pymysql",
     "beautifulsoup4",
+    "feedparser",
 ]
 
 doc_requires = [
     "sphinx",
     "sphinx-autobuild",
     "sphinx_rtd_theme",
     "myst-parser",
     "sphinxcontrib-mermaid",
 ]
 
 test_requires = ["pytest", "pytest-cov", "pre-commit"]
 
-gradio_requires = ["gradio==4.19.1", "modelscope_studio==0.0.5"]
+gradio_requires = [
+    "networkx",
+    "gradio==4.19.1",
+    "modelscope_studio==0.0.5",
+    "black",
+]
 
 # released requires
 minimal_requires = [
     "docstring_parser",
     "loguru==0.6.0",
     "tiktoken",
     "Pillow",
@@ -108,10 +115,11 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
     entry_points={
         "console_scripts": [
             "as_studio=agentscope.web.studio.studio:run_app",
+            "as_workflow=agentscope.web.workstation.workflow:main",
         ],
     },
 )
```

### Comparing `agentscope-0.0.3/src/agentscope/_init.py` & `agentscope-0.0.4/src/agentscope/_init.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,54 +22,63 @@
     model_configs: Optional[Union[dict, str, list]] = None,
     project: Optional[str] = None,
     name: Optional[str] = None,
     save_dir: str = _DEFAULT_DIR,
     save_log: bool = True,
     save_code: bool = True,
     save_api_invoke: bool = True,
+    use_monitor: bool = True,
     logger_level: LOG_LEVEL = _DEFAULT_LOG_LEVEL,
+    runtime_id: Optional[str] = None,
     agent_configs: Optional[Union[str, list, dict]] = None,
 ) -> Sequence[AgentBase]:
     """A unified entry to initialize the package, including model configs,
     runtime names, saving directories and logging settings.
 
     Args:
         model_configs (`Optional[Union[dict, str, list]]`, defaults to `None`):
             A dict, a list of dicts, or a path to a json file containing
             model configs.
         project (`Optional[str]`, defaults to `None`):
             The project name, which is used to identify the project.
         name (`Optional[str]`, defaults to `None`):
             The name for runtime, which is used to identify this runtime.
+        runtime_id (`Optional[str]`, defaults to `None`):
+            The id for runtime, which is used to identify this runtime. Use
+            `None` will generate a random id.
         save_dir (`str`, defaults to `./runs`):
             The directory to save logs, files, codes, and api invocations.
             If `dir` is `None`, when saving logs, files, codes, and api
             invocations, the default directory `./runs` will be created.
         save_log (`bool`, defaults to `False`):
             Whether to save logs locally.
         save_code (`bool`, defaults to `False`):
             Whether to save codes locally.
         save_api_invoke (`bool`, defaults to `False`):
             Whether to save api invocations locally, including model and web
             search invocation.
+        use_monitor (`bool`, defaults to `True`):
+            Whether to activate the monitor.
         logger_level (`LOG_LEVEL`, defaults to `"INFO"`):
             The logging level of logger.
         agent_configs (`Optional[Union[str, list, dict]]`, defaults to `None`):
             The config dict(s) of agents or the path to the config file,
             which can be loaded by json.loads(). One agent config should
             cover the required arguments to initialize a specific agent
             object, otherwise the default values will be used.
     """
     init_process(
         model_configs=model_configs,
         project=project,
         name=name,
+        runtime_id=runtime_id,
         save_dir=save_dir,
         save_api_invoke=save_api_invoke,
         save_log=save_log,
+        use_monitor=use_monitor,
         logger_level=logger_level,
     )
 
     # save init settings for subprocess
     _INIT_SETTINGS["model_configs"] = model_configs
     _INIT_SETTINGS["project"] = project
     _INIT_SETTINGS["name"] = name
@@ -113,14 +122,15 @@
     model_configs: Optional[Union[dict, str, list]] = None,
     project: Optional[str] = None,
     name: Optional[str] = None,
     runtime_id: Optional[str] = None,
     save_dir: str = _DEFAULT_DIR,
     save_api_invoke: bool = False,
     save_log: bool = False,
+    use_monitor: bool = True,
     logger_level: LOG_LEVEL = _DEFAULT_LOG_LEVEL,
 ) -> None:
     """An entry to initialize the package in a process.
 
     Args:
         project (`Optional[str]`, defaults to `None`):
             The project name, which is used to identify the project.
@@ -135,31 +145,36 @@
         save_api_invoke (`bool`, defaults to `False`):
             Whether to save api invocations locally, including model and web
             search invocation.
         model_configs (`Optional[Sequence]`, defaults to `None`):
             A sequence of pre-init model configs.
         save_log (`bool`, defaults to `False`):
             Whether to save logs locally.
+        use_monitor (`bool`, defaults to `True`):
+            Whether to activate the monitor.
         logger_level (`LOG_LEVEL`, defaults to `"INFO"`):
             The logging level of logger.
     """
-    # Init logger
-    dir_log = str(file_manager.dir_log) if save_log else None
-    setup_logger(dir_log, logger_level)
-
-    # Load model configs if needed
-    if model_configs is not None:
-        read_model_configs(model_configs)
-
     # Init the runtime
     if project is not None:
         _runtime.project = project
     if name is not None:
         _runtime.name = name
     if runtime_id is not None:
         _runtime.runtime_id = runtime_id
 
+    # Init logger
+    dir_log = str(file_manager.dir_log) if save_log else None
+    setup_logger(dir_log, logger_level)
+
+    # Load model configs if needed
+    if model_configs is not None:
+        read_model_configs(model_configs)
+
     # Init file manager and save configs by default
     file_manager.init(save_dir, save_api_invoke)
 
     # Init monitor
-    _ = MonitorFactory.get_monitor(db_path=file_manager.path_db)
+    _ = MonitorFactory.get_monitor(
+        db_path=file_manager.path_db,
+        impl_type="sqlite" if use_monitor else "dummy",
+    )
```

### Comparing `agentscope-0.0.3/src/agentscope/_runtime.py` & `agentscope-0.0.4/src/agentscope/_runtime.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/agents/__init__.py` & `agentscope-0.0.4/src/agentscope/agents/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 """ Import all agent related modules in the package. """
-from .agent import AgentBase
+from .agent import AgentBase, DistConf
 from .operator import Operator
 from .dialog_agent import DialogAgent
 from .dict_dialog_agent import DictDialogAgent
 from .user_agent import UserAgent
 from .text_to_image_agent import TextToImageAgent
-from .rpc_agent import RpcAgentServerLauncher
+from .rpc_agent import RpcAgent, RpcAgentServerLauncher
 from .react_agent import ReActAgent
 
 
 __all__ = [
     "AgentBase",
     "Operator",
     "DialogAgent",
     "DictDialogAgent",
     "TextToImageAgent",
     "UserAgent",
-    "RpcAgentServerLauncher",
     "ReActAgent",
+    "DistConf",
+    "RpcAgent",
+    "RpcAgentServerLauncher",
 ]
```

### Comparing `agentscope-0.0.3/src/agentscope/agents/agent.py` & `agentscope-0.0.4/src/agentscope/memory/temporary_memory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,250 +1,278 @@
 # -*- coding: utf-8 -*-
-""" Base class for Agent """
-
-from __future__ import annotations
-from abc import ABCMeta
+"""
+Memory module for conversation
+"""
+
+import json
+import os
+from typing import Iterable, Sequence
 from typing import Optional
-from typing import Sequence
 from typing import Union
-from typing import Any
-import uuid
-from loguru import logger
-
-from agentscope.agents.operator import Operator
-from agentscope.models import load_model_by_config_name
-from agentscope.memory import TemporaryMemory
-
+from typing import Callable
 
-class _RecordInitSettingMeta(ABCMeta):
-    """A wrapper to record the init args into `_init_settings` field."""
-
-    def __call__(cls, *args: tuple, **kwargs: dict) -> Any:
-        instance = super().__call__(*args, **kwargs)
-        instance._init_settings = {"args": args, "kwargs": kwargs}
-        return instance
+from loguru import logger
 
+from .memory import MemoryBase
+from ..models import load_model_by_config_name
+from ..service.retrieval.retrieval_from_list import retrieve_from_list
+from ..service.retrieval.similarity import Embedding
 
-class AgentBase(Operator, metaclass=_RecordInitSettingMeta):
-    """Base class for all agents.
 
-    All agents should inherit from this class and implement the `reply`
-    function.
+class TemporaryMemory(MemoryBase):
+    """
+    In-memory memory module, not writing to hard disk
     """
-
-    _version: int = 1
 
     def __init__(
         self,
-        name: str,
-        sys_prompt: Optional[str] = None,
-        model_config_name: str = None,
-        use_memory: bool = True,
-        memory_config: Optional[dict] = None,
+        config: Optional[dict] = None,
+        embedding_model: Union[str, Callable] = None,
     ) -> None:
-        r"""Initialize an agent from the given arguments.
-
-        Args:
-            name (`str`):
-                The name of the agent.
-            sys_prompt (`Optional[str]`):
-                The system prompt of the agent, which can be passed by args
-                or hard-coded in the agent.
-            model_config_name (`str`, defaults to None):
-                The name of the model config, which is used to load model from
-                configuration.
-            use_memory (`bool`, defaults to `True`):
-                Whether the agent has memory.
-            memory_config (`Optional[dict]`):
-                The config of memory.
-        """
-        self.name = name
-        self.memory_config = memory_config
-
-        if sys_prompt is not None:
-            self.sys_prompt = sys_prompt
+        super().__init__(config)
 
-        # TODO: support to receive a ModelWrapper instance
-        if model_config_name is not None:
-            self.model = load_model_by_config_name(model_config_name)
+        self._content = []
 
-        if use_memory:
-            self.memory = TemporaryMemory(memory_config)
+        # prepare embedding model if needed
+        if isinstance(embedding_model, str):
+            self.embedding_model = load_model_by_config_name(embedding_model)
         else:
-            self.memory = None
-
-        # The global unique id of this agent
-        self._agent_id = self.__class__.generate_agent_id()
+            self.embedding_model = embedding_model
 
-        # The audience of this agent, which means if this agent generates a
-        # response, it will be passed to all agents in the audience.
-        self._audience = None
-
-    @classmethod
-    def generate_agent_id(cls) -> str:
-        """Generate the agent_id of this agent instance"""
-        # TODO: change cls.__name__ into a global unique agent_type
-        return f"{cls.__name__}_{uuid.uuid4().hex}"
+    def add(
+        self,
+        memories: Union[Sequence[dict], dict, None],
+        embed: bool = False,
+    ) -> None:
+        if memories is None:
+            return
 
-    def reply(self, x: dict = None) -> dict:
-        """Define the actions taken by this agent.
+        if not isinstance(memories, list):
+            record_memories = [memories]
+        else:
+            record_memories = memories
 
-        Args:
-            x (`dict`, defaults to `None`):
-                Dialog history and some environment information
+        # if memory doesn't have id attribute, we skip the checking
+        memories_idx = set(_.id for _ in self._content if hasattr(_, "id"))
+        for memory_unit in record_memories:
+            # add to memory if it's new
+            if (
+                not hasattr(memory_unit, "id")
+                or memory_unit.id not in memories_idx
+            ):
+                if embed:
+                    if self.embedding_model:
+                        # TODO: embed only content or its string representation
+                        memory_unit.embedding = self.embedding_model(
+                            [memory_unit],
+                            return_embedding_only=True,
+                        )
+                    else:
+                        raise RuntimeError("Embedding model is not provided.")
+                self._content.append(memory_unit)
+
+    def delete(self, index: Union[Iterable, int]) -> None:
+        if self.size() == 0:
+            logger.warning(
+                "The memory is empty, and the delete operation is "
+                "skipping.",
+            )
+            return
 
-        Returns:
-            The agent's response to the input.
+        if isinstance(index, int):
+            index = [index]
 
-        Note:
-            Given that some agents are in an adversarial environment,
-            their input doesn't include the thoughts of other agents.
-        """
-        raise NotImplementedError(
-            f"Agent [{type(self).__name__}] is missing the required "
-            f'"reply" function.',
-        )
+        if isinstance(index, list):
+            index = set(index)
 
-    def load_from_config(self, config: dict) -> None:
-        """Load configuration for this agent.
+            invalid_index = [_ for _ in index if _ >= self.size() or _ < 0]
+            if len(invalid_index) > 0:
+                logger.warning(
+                    f"Skip delete operation for the invalid "
+                    f"index {invalid_index}",
+                )
 
-        Args:
-            config (`dict`): model configuration
-        """
+            self._content = [
+                _ for i, _ in enumerate(self._content) if i not in index
+            ]
+        else:
+            raise NotImplementedError(
+                "index type only supports {None, int, list}",
+            )
 
-    def export_config(self) -> dict:
-        """Return configuration of this agent.
+    def export(
+        self,
+        to_mem: bool = False,
+        file_path: Optional[str] = None,
+    ) -> Optional[list]:
+        """Export memory to json file"""
+        if to_mem:
+            return self._content
+
+        if to_mem is False and file_path is not None:
+            with open(file_path, "w", encoding="utf-8") as f:
+                json.dump(self._content, f, indent=4)
+        else:
+            raise NotImplementedError(
+                "file type only supports "
+                "{json, yaml, pkl}, default is json",
+            )
+        return None
 
-        Returns:
-            The configuration of current agent.
-        """
-        return {}
+    def load(
+        self,
+        memories: Union[str, dict, list],
+        overwrite: bool = False,
+    ) -> None:
+        if isinstance(memories, str):
+            if os.path.isfile(memories):
+                with open(memories, "r", encoding="utf-8") as f:
+                    self.add(json.load(f))
+            else:
+                try:
+                    load_memories = json.loads(memories)
+                    if not isinstance(load_memories, dict) and not isinstance(
+                        load_memories,
+                        list,
+                    ):
+                        logger.warning(
+                            "The memory loaded by json.loads is "
+                            "neither a dict nor a list, which may "
+                            "cause unpredictable errors.",
+                        )
+                except json.JSONDecodeError as e:
+                    raise json.JSONDecodeError(
+                        f"Cannot load [{memories}] via " f"json.loads.",
+                        e.doc,
+                        e.pos,
+                    )
+        else:
+            load_memories = memories
 
-    def load_memory(self, memory: Sequence[dict]) -> None:
-        r"""Load input memory."""
+        # overwrite the original memories after loading the new ones
+        if overwrite:
+            self.clear()
 
-    def __call__(self, *args: Any, **kwargs: Any) -> dict:
-        """Calling the reply function, and broadcast the generated
-        response to all audiences if needed."""
-        res = self.reply(*args, **kwargs)
+        self.add(load_memories)
 
-        # broadcast to audiences if needed
-        if self._audience is not None:
-            self._broadcast_to_audience(res)
+    def clear(self) -> None:
+        """Clean memory, depending on how the memory are stored"""
+        self._content = []
 
-        return res
+    def size(self) -> int:
+        """Returns the number of memory segments in memory."""
+        return len(self._content)
 
-    def speak(
+    def retrieve_by_embedding(
         self,
-        content: Union[str, dict],
-    ) -> None:
-        """Speak out the content generated by the agent."""
-        logger.chat(content)
-
-    def observe(self, x: Union[dict, Sequence[dict]]) -> None:
-        """Observe the input, store it in memory without response to it.
+        query: Union[str, Embedding],
+        metric: Callable[[Embedding, Embedding], float],
+        top_k: int = 1,
+        preserve_order: bool = True,
+        embedding_model: Callable[[Union[str, dict]], Embedding] = None,
+    ) -> list[dict]:
+        """Retrieve memory by their embeddings.
 
         Args:
-            x (`Union[dict, Sequence[dict]]`):
-                The input message to be recorded in memory.
+            query (`Union[str, Embedding]`):
+                Query string or embedding.
+            metric (`Callable[[Embedding, Embedding], float]`):
+                A metric to compute the relevance between embeddings of query
+                and memory. In default, higher relevance means better match,
+                and you can set `reverse` to `True` to reverse the order.
+            top_k (`int`, defaults to `1`):
+                The number of memory units to retrieve.
+            preserve_order (`bool`, defaults to `True`):
+                Whether to preserve the original order of the retrieved memory
+                units.
+            embedding_model (`Callable[[Union[str, dict]], Embedding]`, \
+                defaults to `None`):
+                A callable object to embed the memory unit. If not provided, it
+                will use the default embedding model.
+
+        Returns:
+            `list[dict]`: a list of retrieved memory units in
+            specific order.
         """
-        if self.memory:
-            self.memory.add(x)
 
-    def reset_audience(self, audience: Sequence[AgentBase]) -> None:
-        """Set the audience of this agent, which means if this agent
-        generates a response, it will be passed to all audiences.
+        retrieved_items = retrieve_from_list(
+            query,
+            self.get_embeddings(embedding_model or self.embedding_model),
+            metric,
+            top_k,
+            self.embedding_model,
+            preserve_order,
+        ).content
+
+        # obtain the corresponding memory item
+        response = []
+        for score, index, _ in retrieved_items:
+            response.append(
+                {
+                    "score": score,
+                    "index": index,
+                    "memory": self._content[index],
+                },
+            )
 
-        Args:
-            audience (`Sequence[AgentBase]`):
-                The audience of this agent, which will be notified when this
-                agent generates a response message.
-        """
-        # TODO: we leave the consideration of nested msghub for future.
-        #  for now we suppose one agent can only be in one msghub
-        self._audience = [_ for _ in audience if _ != self]
-
-    def clear_audience(self) -> None:
-        """Remove the audience of this agent."""
-        # TODO: we leave the consideration of nested msghub for future.
-        #  for now we suppose one agent can only be in one msghub
-        self._audience = None
+        return response
 
-    def rm_audience(
+    def get_embeddings(
         self,
-        audience: Union[Sequence[AgentBase], AgentBase],
-    ) -> None:
-        """Remove the given audience from the Sequence"""
-        if not isinstance(audience, Sequence):
-            audience = [audience]
-
-        for agent in audience:
-            if self._audience is not None and agent in self._audience:
-                self._audience.pop(self._audience.index(agent))
-            else:
-                logger.warning(
-                    f"Skip removing agent [{agent.name}] from the "
-                    f"audience for its inexistence.",
-                )
+        embedding_model: Callable[[Union[str, dict]], Embedding] = None,
+    ) -> list:
+        """Get embeddings of all memory units. If `embedding_model` is
+        provided, the memory units that doesn't have `embedding` attribute
+        will be embedded. Otherwise, its embedding will be `None`.
 
-    def _broadcast_to_audience(self, x: dict) -> None:
-        """Broadcast the input to all audiences."""
-        for agent in self._audience:
-            agent.observe(x)
-
-    @property
-    def agent_id(self) -> str:
-        """The unique id of this agent.
+        Args:
+            embedding_model
+                (`Callable[[Union[str, dict]], Embedding]`, defaults to
+                `None`):
+                Embedding model or embedding vector.
 
         Returns:
-            str: agent_id
+            `list[Union[Embedding, None]]`: List of embeddings or None.
         """
-        return self._agent_id
+        embeddings = []
+        for memory_unit in self._content:
+            if memory_unit.embedding is None and embedding_model is not None:
+                # embedding
+                # TODO: embed only content or its string representation
+                memory_unit.embedding = embedding_model(memory_unit)
+            embeddings.append(memory_unit.embedding)
+        return embeddings
 
-    def to_dist(
+    def get_memory(
         self,
-        host: str = "localhost",
-        port: int = None,
-        max_pool_size: int = 8192,
-        max_timeout_seconds: int = 1800,
-        launch_server: bool = True,
-        local_mode: bool = True,
-        lazy_launch: bool = True,
-    ) -> AgentBase:
-        """Convert current agent instance into a distributed version.
+        recent_n: Optional[int] = None,
+        filter_func: Optional[Callable[[int, dict], bool]] = None,
+    ) -> list:
+        """Retrieve memory.
 
         Args:
-            host (`str`, defaults to `"localhost"`):
-                Hostname of the rpc agent server.
-            port (`int`, defaults to `None`):
-                Port of the rpc agent server.
-            max_pool_size (`int`, defaults to `8192`):
-                Max number of task results that the server can accommodate.
-            max_timeout_seconds (`int`, defaults to `1800`):
-                Timeout for task results.
-            local_mode (`bool`, defaults to `True`):
-                Whether the started rpc server only listens to local
-                requests.
-            lazy_launch (`bool`, defaults to `True`):
-                Only launch the server when the agent is called.
-
-        Returns:
-            `AgentBase`: the wrapped agent instance with distributed
-            functionality
+            recent_n (`Optional[int]`, default `None`):
+                The last number of memories to return.
+            filter_func
+                (`Callable[[int, dict], bool]`, default to `None`):
+                The function to filter memories, which take the index and
+                memory unit as input, and return a boolean value.
         """
-        from .rpc_agent import RpcAgent
+        # extract the recent `recent_n` entries in memories
+        if recent_n is None:
+            memories = self._content
+        else:
+            if recent_n > self.size():
+                logger.warning(
+                    "The retrieved number of memories {} is "
+                    "greater than the total number of memories {"
+                    "}",
+                    recent_n,
+                    self.size(),
+                )
+            memories = self._content[-recent_n:]
+
+        # filter the memories
+        if filter_func is not None:
+            memories = [_ for i, _ in enumerate(memories) if filter_func(i, _)]
 
-        if issubclass(self.__class__, RpcAgent):
-            return self
-        return RpcAgent(
-            agent_class=self.__class__,
-            agent_configs=self._init_settings,
-            name=self.name,
-            host=host,
-            port=port,
-            max_pool_size=max_pool_size,
-            max_timeout_seconds=max_timeout_seconds,
-            launch_server=launch_server,
-            local_mode=local_mode,
-            lazy_launch=lazy_launch,
-            agent_id=self.agent_id,
-        )
+        return memories
```

### Comparing `agentscope-0.0.3/src/agentscope/agents/dialog_agent.py` & `agentscope-0.0.4/src/agentscope/agents/dialog_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
         if prompt_type is not None:
             logger.warning(
                 "The argument `prompt_type` is deprecated and "
                 "will be removed in the future.",
             )
 
+    # TODO change typing from dict to MSG
     def reply(self, x: dict = None) -> dict:
         """Reply function of the agent. Processes the input data,
         generates a prompt using the current dialogue memory and system
         prompt, and invokes the language model to produce a response. The
         response is then formatted and added to the dialogue memory.
 
         Args:
@@ -74,15 +75,17 @@
         # record the input if needed
         if self.memory:
             self.memory.add(x)
 
         # prepare prompt
         prompt = self.model.format(
             Msg("system", self.sys_prompt, role="system"),
-            self.memory and self.memory.get_memory(),  # type: ignore[arg-type]
+            self.memory
+            and self.memory.get_memory()
+            or x,  # type: ignore[arg-type]
         )
 
         # call llm and generate response
         response = self.model(prompt).text
         msg = Msg(self.name, response, role="assistant")
 
         # Print/speak the message in this agent's voice
```

### Comparing `agentscope-0.0.3/src/agentscope/agents/dict_dialog_agent.py` & `agentscope-0.0.4/src/agentscope/agents/dict_dialog_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,31 +81,28 @@
             model_config_name (`str`, defaults to None):
                 The name of the model config, which is used to load model from
                 configuration.
             use_memory (`bool`, defaults to `True`):
                 Whether the agent has memory.
             memory_config (`Optional[dict]`, defaults to `None`):
                 The config of memory.
-            parse_func (`Optional[Callable[..., Any]]`,
-            defaults to `parse_dict`):
+            parse_func (`Optional[Callable[..., Any]]`, defaults to `parse_dict`):
                 The function used to parse the model output,
                 e.g. `json.loads`, which is used to extract json from the
                 output.
-            fault_handler (`Optional[Callable[..., Any]]`,
-            defaults to `default_response`):
+            fault_handler (`Optional[Callable[..., Any]]`, defaults to `default_response`):
                 The function used to handle the fault when parse_func fails
                 to parse the model output.
             max_retries (`Optional[int]`, defaults to `None`):
                 The maximum number of retries when failed to parse the model
                 output.
-            prompt_type (`Optional[PromptType]`, defaults to
-            `PromptType.LIST`):
+            prompt_type (`Optional[PromptType]`, defaults to `PromptType.LIST`):
                 The type of the prompt organization, chosen from
                 `PromptType.LIST` or `PromptType.STRING`.
-        """
+        """  # noqa
         super().__init__(
             name=name,
             sys_prompt=sys_prompt,
             model_config_name=model_config_name,
             use_memory=use_memory,
             memory_config=memory_config,
         )
@@ -117,14 +114,15 @@
 
         if prompt_type is not None:
             logger.warning(
                 "The argument `prompt_type` is deprecated and "
                 "will be removed in the future.",
             )
 
+    # TODO change typing from dict to MSG
     def reply(self, x: dict = None) -> dict:
         """Reply function of the agent.
         Processes the input data, generates a prompt using the current
         dialogue memory and system prompt, and invokes the language
         model to produce a response. The response is then formatted
         and added to the dialogue memory.
 
@@ -146,15 +144,17 @@
         # record the input if needed
         if self.memory:
             self.memory.add(x)
 
         # prepare prompt
         prompt = self.model.format(
             Msg("system", self.sys_prompt, role="system"),
-            self.memory and self.memory.get_memory(),  # type: ignore[arg-type]
+            self.memory
+            and self.memory.get_memory()
+            or x,  # type: ignore[arg-type]
         )
 
         # call llm
         response = self.model(
             prompt,
             parse_func=self.parse_func,
             fault_handler=self.fault_handler,
```

### Comparing `agentscope-0.0.3/src/agentscope/agents/operator.py` & `agentscope-0.0.4/src/agentscope/agents/operator.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/agents/react_agent.py` & `agentscope-0.0.4/src/agentscope/agents/react_agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,36 @@
 # -*- coding: utf-8 -*-
 """An agent class that implements the ReAct algorithm. The agent will reason
 and act iteratively to solve problems. More details can be found in the paper
 https://arxiv.org/abs/2210.03629.
 """
-import json
-from typing import Tuple, List
+from typing import Any
 
+from loguru import logger
+
+from agentscope.exception import ResponseParsingError, FunctionCallError
 from agentscope.agents import AgentBase
 from agentscope.message import Msg
-from agentscope.models import ResponseParser, ResponseParsingError
-from agentscope.service import ServiceResponse, ServiceExecStatus
-
-
-DEFAULT_TOOL_PROMPT = """The following tool functions are available in the format of
-```
-{{index}}. {{function name}}: {{function description}}
-    {{argument1 name}} ({{argument type}}): {{argument description}}
-    {{argument2 name}} ({{argument type}}): {{argument description}}
-    ...
-```
-
-## Tool Functions:
-{function_prompt}
+from agentscope.parsers import MarkdownJsonDictParser
+from agentscope.service import ServiceToolkit
+from agentscope.service.service_toolkit import ServiceFunction
 
-## What You Should Do:
+INSTRUCTION_PROMPT = """## What You Should Do:
 1. First, analyze the current situation, and determine your goal.
 2. Then, check if your goal is already achieved. If so, try to generate a response. Otherwise, think about how to achieve it with the help of provided tool functions.
 3. Respond in the required format.
 
 ## Note:
 1. Fully understand the tool functions and their arguments before using them.
 2. You should decide if you need to use the tool functions, if not then return an empty list in "function" field.
 3. Make sure the types and values of the arguments you provided to the tool functions are correct.
 4. Don't take things for granted. For example, where you are, what's the time now, etc. You can try to use the tool functions to get information.
 5. If the function execution fails, you should analyze the error and try to solve it.
-
 """  # noqa
 
-TOOL_HINT_PROMPT = """
-## Response Format:
-You should respond with a JSON object in the following format, which can be loaded by `json.loads` in Python directly. If no tool function is used, the "function" field should be an empty list.
-{
-    "thought": "what you thought",
-    "speak": "what you said",
-    "function": [{"name": "{function name}", "arguments": {"{argument1 name}": xxx, "{argument2 name}": xxx}}]
-}"""  # noqa
-
-FUNCTION_RESULT_TITLE_PROMPT = """Execution Results:
-"""
-
-FUNCTION_RESULT_PROMPT = """{index}. {function_name}:
-    [EXECUTE STATUS]: {status}
-    [EXECUTE RESULT]: {result}
-"""
-
-ERROR_INFO_PROMPT = """Your response is not a JSON object, and cannot be parsed by `json.loads` in parse function:
-## Your Response:
-[YOUR RESPONSE BEGIN]
-{response}
-[YOUR RESPONSE END]
-
-## Error Information:
-{error_info}
-
-Analyze the reason, and re-correct your response in the correct format."""  # pylint: disable=all  # noqa
-
 
 class ReActAgent(AgentBase):
     """An agent class that implements the ReAct algorithm. More details refer
     to https://arxiv.org/abs/2210.03629.
 
     Note this is an example implementation of ReAct algorithm in AgentScope.
     We follow the idea within the paper, but the detailed prompt engineering
@@ -76,250 +38,220 @@
     their own needs.
     """
 
     def __init__(
         self,
         name: str,
         model_config_name: str,
-        tools: List[Tuple],
+        service_toolkit: ServiceToolkit = None,
         sys_prompt: str = "You're a helpful assistant. Your name is {name}.",
         max_iters: int = 10,
         verbose: bool = True,
+        **kwargs: Any,
     ) -> None:
         """Initialize the ReAct agent with the given name, model config name
         and tools.
 
         Args:
             name (`str`):
                 The name of the agent.
             sys_prompt (`str`):
                 The system prompt of the agent.
             model_config_name (`str`):
                 The name of the model config, which is used to load model from
                 configuration.
-            tools (`List[Tuple]`):
-                A list of tuples, each containing the name of a tool and the
-                tool's description in JSON schema format.
+            service_toolkit (`ServiceToolkit`):
+                A `ServiceToolkit` object that contains the tool functions.
             max_iters (`int`, defaults to `10`):
                 The maximum number of iterations of the reasoning-acting loops.
             verbose (`bool`, defaults to `True`):
-                Whether to print the output of the tools.
+                Whether to print the detailed information during reasoning and
+                acting steps. If `False`, only the content in speak field will
+                be print out.
         """
         super().__init__(
             name=name,
             sys_prompt=sys_prompt,
             model_config_name=model_config_name,
         )
 
-        self.tools = tools
+        # TODO: To compatible with the old version, which will be deprecated
+        #  soon
+        if "tools" in kwargs:
+            logger.warning(
+                "The argument `tools` will be deprecated soon. "
+                "Please use `service_toolkit` instead. Example refers to "
+                "https://github.com/modelscope/agentscope/blob/main/"
+                "examples/conversation_with_react_agent/code/"
+                "conversation_with_react_agent.py",
+            )
+
+            service_funcs = {}
+            for func, json_schema in kwargs["tools"]:
+                name = json_schema["function"]["name"]
+                service_funcs[name] = ServiceFunction(
+                    name=name,
+                    original_func=func,
+                    processed_func=func,
+                    json_schema=json_schema,
+                )
+
+            if service_toolkit is None:
+                service_toolkit = ServiceToolkit()
+                service_toolkit.service_funcs = service_funcs
+            else:
+                service_toolkit.service_funcs.update(service_funcs)
+
+        elif service_toolkit is None:
+            raise ValueError(
+                "The argument `service_toolkit` is required to initialize "
+                "the ReActAgent.",
+            )
+
+        self.service_toolkit = service_toolkit
         self.verbose = verbose
         self.max_iters = max_iters
 
-        func_prompt, self.func_name_mapping = self.prepare_funcs_prompt(tools)
-
-        # Prepare system prompt
-        tools_prompt = DEFAULT_TOOL_PROMPT.format(function_prompt=func_prompt)
+        if not sys_prompt.endswith("\n"):
+            sys_prompt = sys_prompt + "\n"
 
-        if sys_prompt.endswith("\n"):
-            self.sys_prompt = sys_prompt.format(name=self.name) + tools_prompt
-        else:
-            self.sys_prompt = (
-                sys_prompt.format(name=self.name) + "\n" + tools_prompt
-            )
+        self.sys_prompt = "\n".join(
+            [
+                # The brief intro of the role and target
+                sys_prompt.format(name=self.name),
+                # The instruction prompt for tools
+                self.service_toolkit.tools_instruction,
+                # The detailed instruction prompt for the agent
+                INSTRUCTION_PROMPT,
+            ],
+        )
 
         # Put sys prompt into memory
         self.memory.add(Msg("system", self.sys_prompt, role="system"))
 
+        # Initialize a parser object to formulate the response from the model
+        self.parser = MarkdownJsonDictParser(
+            content_hint={
+                "thought": "what you thought",
+                "speak": "what you speak",
+                "function": service_toolkit.tools_calling_format,
+            },
+            required_keys=["thought", "speak", "function"],
+        )
+
     def reply(self, x: dict = None) -> dict:
         """The reply function that achieves the ReAct algorithm.
         The more details please refer to https://arxiv.org/abs/2210.03629"""
 
-        if self.memory:
-            self.memory.add(x)
+        self.memory.add(x)
 
         for _ in range(self.max_iters):
             # Step 1: Thought
+            if self.verbose:
+                self.speak(f" ITER {_+1}, STEP 1: REASONING ".center(70, "#"))
 
-            self.speak(f" ITER {_+1}, STEP 1: REASONING ".center(70, "#"))
+            # Prepare hint to remind model what the response format is
+            # Won't be recorded in memory to save tokens
+            hint_msg = Msg(
+                "system",
+                self.parser.format_instruction,
+                role="system",
+            )
+            if self.verbose:
+                self.speak(hint_msg)
 
-            try:
-                hint_msg = Msg("system", TOOL_HINT_PROMPT, role="system")
-                self.memory.add(hint_msg)
+            # Prepare prompt for the model
+            prompt = self.model.format(self.memory.get_memory(), hint_msg)
 
-                # Generate LLM response
-                prompt = self.model.format(self.memory.get_memory())
+            # Generate and parse the response
+            try:
                 res = self.model(
                     prompt,
-                    parse_func=ResponseParser.to_dict,
+                    parse_func=self.parser.parse,
                     max_retries=1,
-                ).json
+                )
+
+                # Record the response in memory
+                msg_response = Msg(self.name, res.text, "assistant")
+                self.memory.add(msg_response)
+
+                # Print out the response
+                if self.verbose:
+                    self.speak(msg_response)
+                else:
+                    self.speak(
+                        Msg(self.name, res.parsed["speak"], "assistant"),
+                    )
+
+                # Skip the next steps if no need to call tools
+                # The parsed field is a dictionary
+                arg_function = res.parsed["function"]
+                if (
+                    isinstance(arg_function, str)
+                    and arg_function in ["[]", ""]
+                    or isinstance(arg_function, list)
+                    and len(arg_function) == 0
+                ):
+                    # Only the speak field is exposed to users or other agents
+                    return Msg(self.name, res.parsed["speak"], "assistant")
 
+            # Only catch the response parsing error and expose runtime
+            # errors to developers for debugging
             except ResponseParsingError as e:
-                # Record the wrong response from the model
-                response_msg = Msg(self.name, e.response.text, "assistant")
+                # Print out raw response from models for developers to debug
+                response_msg = Msg(self.name, e.raw_response, "assistant")
                 self.speak(response_msg)
 
                 # Re-correct by model itself
-                error_msg = Msg(
-                    "system",
-                    ERROR_INFO_PROMPT.format(
-                        parse_func=ResponseParser.to_dict,
-                        error_info=e.error_info,
-                        response=e.response.text,
-                    ),
-                    "system",
-                )
+                error_msg = Msg("system", str(e), "system")
                 self.speak(error_msg)
 
                 self.memory.add([response_msg, error_msg])
 
                 # Skip acting step to re-correct the response
                 continue
 
-            # Record the response in memory
-            msg_thought = Msg(self.name, res, role="assistant")
-
-            # To better display the response, we reformat it by json.dumps here
-            self.speak(
-                Msg(self.name, json.dumps(res, indent=4), role="assistant"),
-            )
-
-            if self.memory:
-                self.memory.add(msg_thought)
+            # Step 2: Acting
+            if self.verbose:
+                self.speak(f" ITER {_+1}, STEP 2: ACTING ".center(70, "#"))
 
-            # Skip the next steps if no need to call tools
-            if len(res.get("function", [])) == 0:
-                return msg_thought
-
-            # Step 2: Action
-
-            self.speak(f" ITER {_+1}, STEP 2: ACTION ".center(70, "#"))
-
-            # Execute functions
-            # TODO: check the provided arguments and re-correct them if needed
-            execute_results = []
-            for i, func in enumerate(res["function"]):
-                # Execute the function
-                func_res = self.execute_func(i, func)
-                execute_results.append(func_res)
-
-            # Prepare prompt for execution results
-            execute_results_prompt = "\n".join(
-                [
-                    FUNCTION_RESULT_PROMPT.format_map(res)
-                    for res in execute_results
-                ],
-            )
-            # Add title
-            execute_results_prompt = (
-                FUNCTION_RESULT_TITLE_PROMPT + execute_results_prompt
-            )
+            # Parse, check and execute the tool functions in service toolkit
+            try:
+                execute_results = self.service_toolkit.parse_and_call_func(
+                    res.parsed["function"],
+                )
 
-            # Note: Observing the execution results and generate response are
-            # finished in the next loop. We just put the execution results
-            # into memory, and wait for the next loop to generate response.
-
-            # Record execution results into memory as a message from the system
-            msg_res = Msg(
-                name="system",
-                content=execute_results_prompt,
-                role="system",
-            )
-            self.speak(msg_res)
-            if self.memory:
+                # Note: Observing the execution results and generate response
+                # are finished in the next reasoning step. We just put the
+                # execution results into memory, and wait for the next loop
+                # to generate response.
+
+                # Record execution results into memory as system message
+                msg_res = Msg("system", execute_results, "system")
+                self.speak(msg_res)
                 self.memory.add(msg_res)
 
-        return Msg(
+            except FunctionCallError as e:
+                # Catch the function calling error that can be handled by
+                # the model
+                error_msg = Msg("system", str(e), "system")
+                self.speak(error_msg)
+                self.memory.add(error_msg)
+
+        # Exceed the maximum iterations
+        hint_msg = Msg(
             "system",
-            "The agent has reached the maximum iterations.",
+            "You have failed to generate a response in the maximum "
+            "iterations. Now generate a reply by summarizing the current "
+            "situation.",
             role="system",
         )
+        if self.verbose:
+            self.speak(hint_msg)
 
-    def execute_func(self, index: int, func_call: dict) -> dict:
-        """Execute the tool function and return the result.
-
-        Args:
-            index (`int`):
-                The index of the tool function.
-            func_call (`dict`):
-                The function call dictionary with keys 'name' and 'arguments'.
-
-        Returns:
-            `ServiceResponse`: The execution results.
-        """
-        # Extract the function name and arguments
-        func_name = func_call["name"]
-        func_args = func_call["arguments"]
-
-        self.speak(f">>> Executing function {func_name} ...")
-
-        try:
-            func_res = self.func_name_mapping[func_name](**func_args)
-        except Exception as e:
-            func_res = ServiceResponse(
-                status=ServiceExecStatus.ERROR,
-                content=str(e),
-            )
-
-        self.speak(">>> END ")
-
-        status = (
-            "SUCCESS"
-            if func_res.status == ServiceExecStatus.SUCCESS
-            else "FAILED"
-        )
-
-        # return the result of the function
-        return {
-            "index": index + 1,
-            "function_name": func_name,
-            "status": status,
-            "result": func_res.content,
-        }
-
-    def prepare_funcs_prompt(self, tools: List[Tuple]) -> Tuple[str, dict]:
-        """Convert function descriptions from json schema format to
-        string prompt format.
-
-        Args:
-            tools (`List[Tuple]`):
-                The list of tool functions and their descriptions in JSON
-                schema format.
-
-        Returns:
-            `Tuple[str, dict]`:
-                The string prompt for the tool functions and a function name
-                mapping dict.
-
-            .. code-block:: python
-
-                {index}. {function name}: {function description}
-                    {argument name} ({argument type}): {argument description}
-                    ...
-
-        """
-        tools_prompt = []
-        func_name_mapping = {}
-        for i, (func, desc) in enumerate(tools):
-            func_name = desc["function"]["name"]
-            func_name_mapping[func_name] = func
-
-            func_desc = desc["function"]["description"]
-            args_desc = desc["function"]["parameters"]["properties"]
-
-            args_list = [f"{i + 1}. {func_name}: {func_desc}"]
-            for args_name, args_info in args_desc.items():
-                if "type" in args_info:
-                    args_line = (
-                        f'\t{args_name} ({args_info["type"]}): '
-                        f'{args_info.get("description", "")}'
-                    )
-                else:
-                    args_line = (
-                        f'\t{args_name}: {args_info.get("description", "")}'
-                    )
-                args_list.append(args_line)
-
-            func_prompt = "\n".join(args_list)
-            tools_prompt.append(func_prompt)
+        # Generate a reply by summarizing the current situation
+        prompt = self.model.format(self.memory.get_memory(), hint_msg)
+        res = self.model(prompt)
+        res_msg = Msg(self.name, res.text, "assistant")
+        self.speak(res_msg)
 
-        return "\n".join(tools_prompt), func_name_mapping
+        return res_msg
```

### Comparing `agentscope-0.0.3/src/agentscope/agents/rpc_agent.py` & `agentscope-0.0.4/src/agentscope/agents/rpc_agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 """ Base class for Rpc Agent """
 
-from multiprocessing import Process, Event, Pipe, cpu_count
+from multiprocessing import Process, Event, Pipe
 from multiprocessing.synchronize import Event as EventClass
 import socket
 import threading
 import json
-from typing import Any, Optional, Union, Type, Sequence
+import base64
+import traceback
+import asyncio
+from typing import Any, Type, Optional, Union, Sequence
 from concurrent import futures
 from loguru import logger
 
 try:
+    import dill
     import grpc
     from grpc import ServicerContext
+    from expiringdict import ExpiringDict
 except ImportError:
+    dill = None
     grpc = None
     ServicerContext = Any
-
-try:
-    from expiringdict import ExpiringDict
-except ImportError:
     ExpiringDict = None
 
 from agentscope._init import init_process, _INIT_SETTINGS
 from agentscope.agents.agent import AgentBase
 from agentscope.message import (
     Msg,
     PlaceholderMessage,
@@ -58,102 +60,96 @@
 
 class RpcAgent(AgentBase):
     """A wrapper to extend an AgentBase into a gRPC Client."""
 
     def __init__(
         self,
         name: str,
-        agent_class: Type[AgentBase],
-        agent_configs: Optional[dict] = None,
         host: str = "localhost",
         port: int = None,
-        launch_server: bool = True,
+        agent_class: Type[AgentBase] = None,
+        agent_configs: Optional[dict] = None,
         max_pool_size: int = 8192,
         max_timeout_seconds: int = 1800,
         local_mode: bool = True,
         lazy_launch: bool = True,
         agent_id: str = None,
-        create_with_agent_configs: bool = True,
+        connect_existing: bool = False,
     ) -> None:
         """Initialize a RpcAgent instance.
 
         Args:
-            name (`str`): Name of the agent.
-            agent_class (`Type[AgentBase]`):
-                The AgentBase subclass encapsulated by this wrapper.
-            agent_configs (`dict`, defaults to `None`): The args used to
-                initialize the agent_class.
-            host (`str`, defaults to `"localhost"`):
+            name (`str`): the name of the agent.
+            host (`str`, defaults to `localhost`):
                 Hostname of the rpc agent server.
             port (`int`, defaults to `None`):
                 Port of the rpc agent server.
-            launch_server (`bool`, defaults to `True`):
-                Whether to launch the gRPC agent server.
+            agent_class (`Type[AgentBase]`):
+                the AgentBase subclass of the source agent.
+            agent_configs (`dict`): The args used to
+                initialize the agent, generated by `_AgentMeta`.
             max_pool_size (`int`, defaults to `8192`):
                 Max number of task results that the server can accommodate.
             max_timeout_seconds (`int`, defaults to `1800`):
                 Timeout for task results.
             local_mode (`bool`, defaults to `True`):
                 Whether the started gRPC server only listens to local
                 requests.
             lazy_launch (`bool`, defaults to `True`):
                 Only launch the server when the agent is called.
             agent_id (`str`, defaults to `None`):
                 The agent id of this instance. If `None`, it will
                 be generated randomly.
-            create_with_agent_configs (`bool`, defaults to `True`):
-                Only takes effect when `agent_configs` is provided.
-                If true, create the agent instance for the agent with
-                provided `agent_configs`, otherwise uses the agent server's
-                default parameters.
+            connect_existing (`bool`, defaults to `False`):
+                Set to `True`, if the agent is already running on the agent
+                server.
         """
         super().__init__(name=name)
+        self.agent_class = agent_class
+        self.agent_configs = agent_configs
         self.host = host
         self.port = port
         self.server_launcher = None
         self.client = None
+        self.connect_existing = connect_existing
         if agent_id is not None:
             self._agent_id = agent_id
-        else:
-            self._agent_id = agent_class.generate_agent_id()
-        self.agent_class = agent_class
+        # if host and port are not provided, launch server locally
+        launch_server = port is None
         if launch_server:
+            self.host = "localhost"
             self.server_launcher = RpcAgentServerLauncher(
-                agent_class=agent_class,
-                agent_args=agent_configs["args"] if agent_configs else None,
-                agent_kwargs=(
-                    agent_configs["kwargs"] if agent_configs else None
-                ),
-                host=host,
+                host=self.host,
                 port=port,
                 max_pool_size=max_pool_size,
                 max_timeout_seconds=max_timeout_seconds,
                 local_mode=local_mode,
+                custom_agents=[agent_class],
             )
             if not lazy_launch:
                 self._launch_server()
         else:
             self.client = RpcAgentClient(
                 host=self.host,
                 port=self.port,
                 agent_id=self.agent_id,
             )
-            self.client.create_agent(
-                agent_configs if create_with_agent_configs else None,
-            )
+            if not self.connect_existing:
+                self.client.create_agent(agent_configs)
 
     def _launch_server(self) -> None:
         """Launch a rpc server and update the port and the client"""
         self.server_launcher.launch()
         self.port = self.server_launcher.port
         self.client = RpcAgentClient(
             host=self.host,
             port=self.port,
             agent_id=self.agent_id,
         )
+        self.client.create_agent(self.agent_configs)
 
     def reply(self, x: dict = None) -> dict:
         if self.client is None:
             self._launch_server()
         return PlaceholderMessage(
             name=self.name,
             content=None,
@@ -198,58 +194,50 @@
 
         # put itself as the first element of the returned list
         if including_self:
             generated_instances.append(self)
 
         # clone instances without agent server
         for _ in range(generated_instance_number):
+            new_agent_id = self.client.call_func("_clone_agent")
             generated_instances.append(
                 RpcAgent(
                     name=self.name,
-                    agent_class=self.agent_class,
                     host=self.host,
                     port=self.port,
-                    launch_server=False,
-                    create_with_agent_configs=False,
+                    agent_id=new_agent_id,
+                    connect_existing=True,
                 ),
             )
         return generated_instances
 
     def stop(self) -> None:
         """Stop the RpcAgent and the rpc server."""
         if self.server_launcher is not None:
             self.server_launcher.shutdown()
 
     def __del__(self) -> None:
         self.stop()
 
 
 def setup_rpc_agent_server(
-    agent_class: Type[AgentBase],
-    agent_args: tuple,
-    agent_kwargs: dict,
     host: str,
     port: int,
     init_settings: dict = None,
     start_event: EventClass = None,
     stop_event: EventClass = None,
     pipe: int = None,
     local_mode: bool = True,
     max_pool_size: int = 8192,
     max_timeout_seconds: int = 1800,
+    custom_agents: list = None,
 ) -> None:
     """Setup gRPC server rpc agent.
 
     Args:
-        agent_class (`Type[AgentBase]`):
-            A subclass of AgentBase.
-        agent_args (`tuple`): The args tuple used to initialize the
-            agent_class.
-        agent_kwargs (`dict`): The args dict used to initialize the
-            agent_class.
         host (`str`, defaults to `"localhost"`):
             Hostname of the rpc agent server.
         port (`int`):
             The socket port monitored by grpc server.
         init_settings (`dict`, defaults to `None`):
             Init settings for agentscope.init.
         start_event (`EventClass`, defaults to `None`):
@@ -262,67 +250,122 @@
             A pipe instance used to pass the actual port of the server.
         local_mode (`bool`, defaults to `None`):
             Only listen to local requests.
         max_pool_size (`int`, defaults to `8192`):
             Max number of task results that the server can accommodate.
         max_timeout_seconds (`int`, defaults to `1800`):
             Timeout for task results.
+        custom_agents (`list`, defaults to `None`):
+            A list of custom agent classes that are not in `agentscope.agents`.
+    """
+    asyncio.run(
+        setup_rpc_agent_server_async(
+            host=host,
+            port=port,
+            init_settings=init_settings,
+            start_event=start_event,
+            stop_event=stop_event,
+            pipe=pipe,
+            local_mode=local_mode,
+            max_pool_size=max_pool_size,
+            max_timeout_seconds=max_timeout_seconds,
+            custom_agents=custom_agents,
+        ),
+    )
+
+
+async def setup_rpc_agent_server_async(
+    host: str,
+    port: int,
+    init_settings: dict = None,
+    start_event: EventClass = None,
+    stop_event: EventClass = None,
+    pipe: int = None,
+    local_mode: bool = True,
+    max_pool_size: int = 8192,
+    max_timeout_seconds: int = 1800,
+    custom_agents: list = None,
+) -> None:
+    """Setup gRPC server rpc agent in an async way.
+
+    Args:
+        host (`str`, defaults to `"localhost"`):
+            Hostname of the rpc agent server.
+        port (`int`):
+            The socket port monitored by grpc server.
+        init_settings (`dict`, defaults to `None`):
+            Init settings for agentscope.init.
+        start_event (`EventClass`, defaults to `None`):
+            An Event instance used to determine whether the child process
+            has been started.
+        stop_event (`EventClass`, defaults to `None`):
+            The stop Event instance used to determine whether the child
+            process has been stopped.
+        pipe (`int`, defaults to `None`):
+            A pipe instance used to pass the actual port of the server.
+        local_mode (`bool`, defaults to `None`):
+            Only listen to local requests.
+        max_pool_size (`int`, defaults to `8192`):
+            Max number of task results that the server can accommodate.
+        max_timeout_seconds (`int`, defaults to `1800`):
+            Timeout for task results.
+        custom_agents (`list`, defaults to `None`):
+            A list of custom agent classes that are not in `agentscope.agents`.
     """
 
     if init_settings is not None:
         init_process(**init_settings)
-    servicer = RpcServerSideWrapper(
-        agent_class,
-        agent_args,
-        agent_kwargs,
+    servicer = AgentPlatform(
         host=host,
         port=port,
         max_pool_size=max_pool_size,
         max_timeout_seconds=max_timeout_seconds,
     )
+    # update agent registry
+    if custom_agents is not None:
+        for agent_class in custom_agents:
+            AgentBase.register_agent_class(agent_class=agent_class)
     while True:
         try:
             port = check_port(port)
             servicer.port = port
             logger.info(
-                f"Starting rpc server [{agent_class.__name__}] at port"
-                f" [{port}]...",
+                f"Starting rpc server at port [{port}]...",
             )
-            server = grpc.server(
-                futures.ThreadPoolExecutor(max_workers=cpu_count()),
+            server = grpc.aio.server(
+                futures.ThreadPoolExecutor(max_workers=None),
             )
             add_RpcAgentServicer_to_server(servicer, server)
             if local_mode:
                 server.add_insecure_port(f"localhost:{port}")
             else:
                 server.add_insecure_port(f"0.0.0.0:{port}")
-            server.start()
+            await server.start()
             break
         except OSError:
             logger.warning(
                 f"Failed to start rpc server at port [{port}]"
                 f"try another port",
             )
     logger.info(
-        f"rpc server [{agent_class.__name__}] at port [{port}] started "
-        "successfully",
+        f"rpc server at port [{port}] started successfully",
     )
     if start_event is not None:
         pipe.send(port)
         start_event.set()
-        stop_event.wait()
+        while not stop_event.is_set():
+            await asyncio.sleep(1)
         logger.info(
-            f"Stopping rpc server [{agent_class.__name__}] at port [{port}]",
+            f"Stopping rpc server at port [{port}]",
         )
-        server.stop(1.0).wait()
+        await server.stop(10.0)
     else:
-        server.wait_for_termination()
+        await server.wait_for_termination()
     logger.info(
-        f"rpc server [{agent_class.__name__}] at port [{port}] stopped "
-        "successfully",
+        f"rpc server at port [{port}] stopped successfully",
     )
 
 
 def find_available_port() -> int:
     """Get an unoccupied socket port number."""
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.bind(("", 0))
@@ -355,111 +398,113 @@
                 f"Port [{port}] is occupied, use [{new_port}] instead",
             )
             return new_port
     return port
 
 
 class RpcAgentServerLauncher:
-    """Launcher of rpc agent server."""
+    """The launcher of AgentPlatform (formerly RpcAgentServer)."""
 
     def __init__(
         self,
-        agent_class: Type[AgentBase] = None,
-        agent_args: tuple = (),
-        agent_kwargs: dict = None,
         host: str = "localhost",
         port: int = None,
         max_pool_size: int = 8192,
         max_timeout_seconds: int = 1800,
         local_mode: bool = False,
+        custom_agents: list = None,
+        agent_class: Type[AgentBase] = None,
+        agent_args: tuple = (),
+        agent_kwargs: dict = None,
     ) -> None:
         """Init a rpc agent server launcher.
 
         Args:
-            agent_class (`Type[AgentBase]`, defaults to `None`):
-                The AgentBase subclass encapsulated by this wrapper.
-            agent_args (`tuple`): The args tuple used to initialize the
-                agent_class.
-            agent_kwargs (`dict`): The args dict used to initialize the
-                agent_class.
             host (`str`, defaults to `"localhost"`):
                 Hostname of the rpc agent server.
             port (`int`, defaults to `None`):
                 Port of the rpc agent server.
             max_pool_size (`int`, defaults to `8192`):
                 Max number of task results that the server can accommodate.
             max_timeout_seconds (`int`, defaults to `1800`):
                 Timeout for task results.
             local_mode (`bool`, defaults to `False`):
                 Whether the started rpc server only listens to local
                 requests.
+            custom_agents (`list`, defaults to `None`):
+                A list of custom agent classes that are not in
+                `agentscope.agents`.
+            agent_class (`Type[AgentBase]`, deprecated):
+                The AgentBase subclass encapsulated by this wrapper.
+            agent_args (`tuple`, deprecated): The args tuple used to
+                initialize the agent_class.
+            agent_kwargs (`dict`, deprecated): The args dict used to
+                initialize the agent_class.
         """
-        self.agent_class = agent_class
-        self.agent_args = agent_args
-        self.agent_kwargs = agent_kwargs
         self.host = host
         self.port = check_port(port)
         self.max_pool_size = max_pool_size
         self.max_timeout_seconds = max_timeout_seconds
         self.local_mode = local_mode
         self.server = None
         self.stop_event = None
         self.parent_con = None
+        self.custom_agents = custom_agents
+        if (
+            agent_class is not None
+            or len(agent_args) > 0
+            or agent_kwargs is not None
+        ):
+            logger.warning(
+                "`agent_class`, `agent_args` and `agent_kwargs` is deprecated"
+                " in `RpcAgentServerLauncher`",
+            )
 
     def _launch_in_main(self) -> None:
         """Launch gRPC server in main-process"""
-        server_thread = threading.Thread(
-            target=setup_rpc_agent_server,
-            kwargs={
-                "agent_class": self.agent_class,
-                "agent_args": self.agent_args,
-                "agent_kwargs": self.agent_kwargs,
-                "host": self.host,
-                "port": self.port,
-                "max_pool_size": self.max_pool_size,
-                "max_timeout_seconds": self.max_timeout_seconds,
-                "local_mode": self.local_mode,
-            },
-        )
-        server_thread.start()
         logger.info(
-            f"Launch [{self.agent_class.__name__}] server at "
-            f"[{self.host}:{self.port}] success",
+            f"Launching agent server at [{self.host}:{self.port}]...",
+        )
+        asyncio.run(
+            setup_rpc_agent_server_async(
+                host=self.host,
+                port=self.port,
+                max_pool_size=self.max_pool_size,
+                max_timeout_seconds=self.max_timeout_seconds,
+                local_mode=self.local_mode,
+                custom_agents=self.custom_agents,
+            ),
         )
-        server_thread.join()
 
     def _launch_in_sub(self) -> None:
         """Launch gRPC server in sub-process."""
         self.stop_event = Event()
         self.parent_con, child_con = Pipe()
         start_event = Event()
         server_process = Process(
             target=setup_rpc_agent_server,
             kwargs={
-                "agent_class": self.agent_class,
-                "agent_args": self.agent_args,
-                "agent_kwargs": self.agent_kwargs,
                 "host": self.host,
                 "port": self.port,
                 "init_settings": _INIT_SETTINGS,
                 "start_event": start_event,
                 "stop_event": self.stop_event,
                 "pipe": child_con,
                 "max_pool_size": self.max_pool_size,
                 "max_timeout_seconds": self.max_timeout_seconds,
                 "local_mode": self.local_mode,
+                "custom_agents": self.custom_agents,
             },
         )
         server_process.start()
         self.port = self.parent_con.recv()
         start_event.wait()
         self.server = server_process
         logger.info(
-            f"Launch [{self.agent_class.__name__}] server at "
-            f"[{self.host}:{self.port}] success",
+            f"Launch agent server at [{self.host}:{self.port}] success",
         )
 
     def launch(self, in_subprocess: bool = True) -> None:
         """launch a rpc agent server.
 
         Args:
             in_subprocess (bool, optional): launch the server in subprocess.
@@ -482,99 +527,103 @@
             if self.stop_event is not None:
                 self.stop_event.set()
                 self.stop_event = None
             self.server.join()
             if self.server.is_alive():
                 self.server.kill()
                 logger.info(
-                    f"Rpc server [{self.agent_class.__name__}] at port"
-                    f" [{self.port}] is killed.",
+                    f"Agent server at port [{self.port}] is killed.",
                 )
             self.server = None
 
 
-class RpcServerSideWrapper(RpcAgentServicer):
-    """A wrapper to extend an AgentBase into a gRPC Servicer."""
+class AgentPlatform(RpcAgentServicer):
+    """A platform for agent to run on (formerly RpcServerSideWrapper)"""
 
     def __init__(
         self,
-        agent_class: Type[AgentBase],
-        agent_args: tuple,
-        agent_kwargs: dict,
         host: str = "localhost",
         port: int = None,
         max_pool_size: int = 8192,
         max_timeout_seconds: int = 1800,
     ):
-        """Init the service side wrapper.
+        """Init the AgentPlatform.
 
         Args:
-            agent_class (`Type[AgentBase]`): The AgentBase subclass
-                encapsulated by this wrapper.
-            agent_args (`tuple`): The args tuple used to initialize the
-                agent_class.
-            agent_kwargs (`dict`): The args dict used to initialize the
-                agent_class.
             host (`str`, defaults to "localhost"):
                 Hostname of the rpc agent server.
             port (`int`, defaults to `None`):
                 Port of the rpc agent server.
             max_pool_size (`int`, defaults to `8192`):
                 The max number of task results that the server can
                 accommodate. Note that the oldest result will be deleted
                 after exceeding the pool size.
             max_timeout_seconds (`int`, defaults to `1800`):
                 Timeout for task results. Note that expired results will be
                 deleted.
         """
-        self.agent_class = agent_class
-        self.agent_args = agent_args
-        self.agent_kwargs = agent_kwargs
         self.host = host
         self.port = port
         self.result_pool = ExpiringDict(
             max_len=max_pool_size,
             max_age_seconds=max_timeout_seconds,
         )
-        self.executor = futures.ThreadPoolExecutor(max_workers=cpu_count())
+        self.executor = futures.ThreadPoolExecutor(max_workers=None)
         self.task_id_lock = threading.Lock()
         self.agent_id_lock = threading.Lock()
         self.task_id_counter = 0
         self.agent_pool: dict[str, AgentBase] = {}
 
     def get_task_id(self) -> int:
         """Get the auto-increment task id."""
         with self.task_id_lock:
             self.task_id_counter += 1
             return self.task_id_counter
 
+    def agent_exists(self, agent_id: str) -> bool:
+        """Check whether the agent exists.
+
+        Args:
+            agent_id (`str`): the agent id.
+
+        Returns:
+            bool: whether the agent exists.
+        """
+        return agent_id in self.agent_pool
+
     def check_and_generate_agent(
         self,
         agent_id: str,
-        agent_configs: dict = None,
+        agent_configs: dict,
     ) -> None:
         """
         Check whether the agent exists, and create new agent instance
         for new agent.
 
         Args:
             agent_id (`str`): the agent id.
+            agent_configs (`dict`): configuration used to initialize the agent,
+                with three fields (generated in `_AgentMeta`):
+
+                .. code-block:: python
+
+                    {
+                        "class_name": {name of the agent}
+                        "args": {args in tuple type to init the agent}
+                        "kwargs": {args in dict type to init the agent}
+                    }
+
         """
         with self.agent_id_lock:
             if agent_id not in self.agent_pool:
-                if agent_configs is not None:
-                    agent_instance = self.agent_class(
-                        *agent_configs["args"],
-                        **agent_configs["kwargs"],
-                    )
-                else:
-                    agent_instance = self.agent_class(
-                        *self.agent_args,
-                        **self.agent_kwargs,
-                    )
+                agent_class_name = agent_configs["class_name"]
+                agent_instance = AgentBase.get_agent_class(agent_class_name)(
+                    *agent_configs["args"],
+                    **agent_configs["kwargs"],
+                )
                 agent_instance._agent_id = agent_id  # pylint: disable=W0212
                 self.agent_pool[agent_id] = agent_instance
                 logger.info(f"create agent instance [{agent_id}]")
 
     def check_and_delete_agent(self, agent_id: str) -> None:
         """
         Check whether the agent exists, and delete the agent instance
@@ -584,29 +633,34 @@
             agent_id (`str`): the agent id.
         """
         with self.agent_id_lock:
             if agent_id in self.agent_pool:
                 self.agent_pool.pop(agent_id)
                 logger.info(f"delete agent instance [{agent_id}]")
 
-    def call_func(self, request: RpcMsg, _: ServicerContext) -> RpcMsg:
+    def call_func(  # pylint: disable=W0236
+        self,
+        request: RpcMsg,
+        context: ServicerContext,
+    ) -> RpcMsg:
         """Call the specific servicer function."""
         if hasattr(self, request.target_func):
             if request.target_func not in ["_create_agent", "_get"]:
-                self.check_and_generate_agent(request.agent_id)
+                if not self.agent_exists(request.agent_id):
+                    return context.abort(
+                        grpc.StatusCode.INVALID_ARGUMENT,
+                        f"Agent [{request.agent_id}] not exists.",
+                    )
             return getattr(self, request.target_func)(request)
         else:
             # TODO: support other user defined method
             logger.error(f"Unsupported method {request.target_func}")
-            return RpcMsg(
-                value=Msg(
-                    name=self.agent_pool[request.agent_id].name,
-                    content=f"Unsupported method {request.target_func}",
-                    role="assistant",
-                ).serialize(),
+            return context.abort(
+                grpc.StatusCode.INVALID_ARGUMENT,
+                f"Unsupported method {request.target_func}",
             )
 
     def _reply(self, request: RpcMsg) -> RpcMsg:
         """Call function of RpcAgentService
 
         Args:
             request (`RpcMsg`):
@@ -682,18 +736,46 @@
         """Create a new agent instance for the agent_id.
 
         Args:
             request (RpcMsg): request message with a `agent_id` field.
         """
         self.check_and_generate_agent(
             request.agent_id,
-            agent_configs=json.loads(request.value) if request.value else None,
+            agent_configs=(
+                dill.loads(base64.b64decode(request.value))
+                if request.value
+                else None
+            ),
         )
         return RpcMsg()
 
+    def _clone_agent(self, request: RpcMsg) -> RpcMsg:
+        """Clone a new agent instance from the origin instance.
+
+        Args:
+            request (RpcMsg): The `agent_id` field is the agent_id of the
+            agent to be cloned.
+
+        Returns:
+            `RpcMsg`: The `value` field contains the agent_id of generated
+            agent.
+        """
+        agent_id = request.agent_id
+        with self.agent_id_lock:
+            if agent_id not in self.agent_pool:
+                raise ValueError(f"Agent [{agent_id}] not exists")
+            ori_agent = self.agent_pool[agent_id]
+        new_agent = ori_agent.__class__(
+            *ori_agent._init_settings["args"],  # pylint: disable=W0212
+            **ori_agent._init_settings["kwargs"],  # pylint: disable=W0212
+        )
+        with self.agent_id_lock:
+            self.agent_pool[new_agent.agent_id] = new_agent
+        return RpcMsg(value=new_agent.agent_id)
+
     def _delete_agent(self, request: RpcMsg) -> RpcMsg:
         """Delete the agent instance of the specific sesssion_id.
 
         Args:
             request (RpcMsg): request message with a `agent_id` field.
         """
         self.check_and_delete_agent(request.agent_id)
@@ -705,11 +787,21 @@
         agent_id: str,
         task_msg: dict = None,
     ) -> None:
         """Task processing."""
         if isinstance(task_msg, PlaceholderMessage):
             task_msg.update_value()
         cond = self.result_pool[task_id]
-        result = self.agent_pool[agent_id].reply(task_msg)
-        self.result_pool[task_id] = result
+        try:
+            result = self.agent_pool[agent_id].reply(task_msg)
+            self.result_pool[task_id] = result
+        except Exception:
+            error_msg = traceback.format_exc()
+            logger.error(f"Error in agent [{agent_id}]:\n{error_msg}")
+            self.result_pool[task_id] = Msg(
+                name="ERROR",
+                role="assistant",
+                __status="ERROR",
+                content=f"Error in agent [{agent_id}]:\n{error_msg}",
+            )
         with cond:
             cond.notify_all()
```

### Comparing `agentscope-0.0.3/src/agentscope/agents/text_to_image_agent.py` & `agentscope-0.0.4/src/agentscope/agents/text_to_image_agent.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/agents/user_agent.py` & `agentscope-0.0.4/src/agentscope/agents/user_agent.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/constants.py` & `agentscope-0.0.4/src/agentscope/constants.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/file_manager.py` & `agentscope-0.0.4/src/agentscope/file_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,16 +42,15 @@
             )
         return cls._instance
 
     def _get_and_create_subdir(self, subdir: str) -> str:
         """Get the path of the subdir and create the subdir if it does not
         exist."""
         path = os.path.join(self.dir, _runtime.runtime_id, subdir)
-        if not os.path.exists(path):
-            os.makedirs(path)
+        os.makedirs(path, exist_ok=True)
         return path
 
     def _get_file_path(self, file_name: str) -> str:
         """Get the path of the file."""
         return os.path.join(self.dir, _runtime.runtime_id, file_name)
 
     @property
@@ -85,16 +84,15 @@
         """The path to the sqlite db file."""
         return self._get_file_path(_DEFAULT_SQLITE_DB_PATH)
 
     def init(self, save_dir: str, save_api_invoke: bool = False) -> None:
         """Set the directory for saving files."""
         self.dir = save_dir
         runtime_dir = os.path.join(save_dir, _runtime.runtime_id)
-        if not os.path.exists(runtime_dir):
-            os.makedirs(runtime_dir)
+        os.makedirs(runtime_dir, exist_ok=True)
 
         self.save_api_invoke = save_api_invoke
 
         # Save the project and name to the runtime directory
         self._save_config()
 
     def _save_config(self) -> None:
```

### Comparing `agentscope-0.0.3/src/agentscope/memory/memory.py` & `agentscope-0.0.4/src/agentscope/memory/memory.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/message.py` & `agentscope-0.0.4/src/agentscope/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,28 +29,26 @@
 
         Args:
             name (`str`):
                 The name of who send the message. It's often used in
                 role-playing scenario to tell the name of the sender.
             content (`Any`):
                 The content of the message.
-            role (`Literal["system", "user", "assistant"]`,
-            defaults to "assistant"):
+            role (`Literal["system", "user", "assistant"]`, defaults to "assistant"):
                 The role of who send the message. It can be one of the
                 `"system"`, `"user"`, or `"assistant"`. Default to
                 `"assistant"`.
             url (`Optional[Union[list[str], str]]`, defaults to None):
                 A url to file, image, video, audio or website.
             timestamp (`Optional[str]`, defaults to None):
                 The timestamp of the message, if None, it will be set to
                 current time.
             **kwargs (`Any`):
                 Other attributes of the message.
-
-        """
+        """  # noqa
         # id and timestamp will be added to the object as its attributes
         # rather than items in dict
         self.id = uuid4().hex
         if timestamp is None:
             self.timestamp = _get_timestamp()
         else:
             self.timestamp = timestamp
@@ -110,22 +108,21 @@
                 The name of who send the message.
             content (`Any`):
                 The content of the message.
             role (`Literal["system", "user", "assistant"]`):
                 Used to identify the source of the message, e.g. the system
                 information, the user input, or the model response. This
                 argument is used to accommodate most Chat API formats.
-            url (`Optional[Union[list[str], str]]`, defaults to None):
+            url (`Optional[Union[list[str], str]]`, defaults to `None`):
                 A url to file, image, video, audio or website.
-            timestamp (`Optional[str]`, defaults to None):
+            timestamp (`Optional[str]`, defaults to `None`):
                 The timestamp of the message, if None, it will be set to
                 current time.
             **kwargs (`Any`):
                 Other attributes of the message.
-
         """
 
         if role is None:
             logger.warning(
                 "A new field `role` is newly added to the message. "
                 "Please specify the role of the message. Currently we use "
                 'a default "assistant" value.',
@@ -249,16 +246,15 @@
                 The name of who send the message. It's often used in
                 role-playing scenario to tell the name of the sender.
                 However, you can also only use `role` when calling openai api.
                 The usage of `name` refers to
                 https://cookbook.openai.com/examples/how_to_format_inputs_to_chatgpt_models.
             content (`Any`):
                 The content of the message.
-            role (`Literal["system", "user", "assistant"]`, defaults to
-            "assistant"):
+            role (`Literal["system", "user", "assistant"]`, defaults to "assistant"):
                 The role of the message, which can be one of the `"system"`,
                 `"user"`, or `"assistant"`.
             url (`Optional[Union[list[str], str]]`, defaults to None):
                 A url to file, image, video, audio or website.
             timestamp (`Optional[str]`, defaults to None):
                 The timestamp of the message, if None, it will be set to
                 current time.
@@ -270,15 +266,15 @@
             task_id (`int`, defaults to `None`):
                 The task id of the real message in the rpc server.
             client (`RpcAgentClient`, defaults to `None`):
                 An RpcAgentClient instance used to connect to the generator of
                 this placeholder.
             x (`dict`, defaults to `None`):
                 Input parameters used to call rpc methods on the client.
-        """
+        """  # noqa
         super().__init__(
             name=name,
             content=content,
             url=url,
             timestamp=timestamp,
             **kwargs,
         )
@@ -286,15 +282,19 @@
         self._is_placeholder = True
         if client is None:
             self._stub: ResponseStub = None
             self._host: str = host
             self._port: int = port
             self._task_id: int = task_id
         else:
-            self._stub = call_in_thread(client, x, "_reply")
+            self._stub = call_in_thread(
+                client,
+                x.serialize() if x is not None else "",
+                "_reply",
+            )
             self._host = client.host
             self._port = client.port
             self._task_id = None
 
     def __is_local(self, key: Any) -> bool:
         return (
             key in PlaceholderMessage.LOCAL_ATTRS or not self._is_placeholder
@@ -333,22 +333,34 @@
             # retrieve real message from rpc agent server
             self.__update_task_id()
             client = RpcAgentClient(self._host, self._port)
             result = client.call_func(
                 func_name="_get",
                 value=json.dumps({"task_id": self._task_id}),
             )
-            self.update(deserialize(result))
+            msg = deserialize(result)
+            status = msg.pop("__status", "OK")
+            if status == "ERROR":
+                raise RuntimeError(msg.content)
+            self.update(msg)
             # the actual value has been updated, not a placeholder any more
             self._is_placeholder = False
         return self
 
     def __update_task_id(self) -> None:
         if self._stub is not None:
-            resp = deserialize(self._stub.get_response())
+            try:
+                resp = deserialize(self._stub.get_response())
+            except Exception as e:
+                logger.error(
+                    f"Failed to get task_id: {self._stub.get_response()}",
+                )
+                raise ValueError(
+                    f"Failed to get task_id: {self._stub.get_response()}",
+                ) from e
             self._task_id = resp["task_id"]  # type: ignore[call-overload]
             self._stub = None
 
     def serialize(self) -> str:
         if self._is_placeholder:
             self.__update_task_id()
             return json.dumps(
```

### Comparing `agentscope-0.0.3/src/agentscope/models/__init__.py` & `agentscope-0.0.4/src/agentscope/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 import json
 from typing import Union, Type
 
 from loguru import logger
 
 from .config import _ModelConfig
 from .model import ModelWrapperBase
-from .response import (
-    ModelResponse,
-    ResponseParsingError,
-    ResponseParser,
-)
+from .response import ModelResponse
 from .post_model import (
     PostAPIModelWrapperBase,
     PostAPIChatWrapper,
 )
 from .openai_model import (
     OpenAIWrapperBase,
     OpenAIChatWrapper,
     OpenAIDALLEWrapper,
     OpenAIEmbeddingWrapper,
 )
 from .dashscope_model import (
     DashScopeChatWrapper,
     DashScopeImageSynthesisWrapper,
     DashScopeTextEmbeddingWrapper,
+    DashScopeMultiModalWrapper,
 )
 from .ollama_model import (
     OllamaChatWrapper,
     OllamaEmbeddingWrapper,
     OllamaGenerationWrapper,
 )
 from .gemini_model import (
@@ -37,68 +34,54 @@
     GeminiEmbeddingWrapper,
 )
 
 
 __all__ = [
     "ModelWrapperBase",
     "ModelResponse",
-    "ResponseParser",
-    "ResponseParsingError",
     "PostAPIModelWrapperBase",
     "PostAPIChatWrapper",
     "OpenAIWrapperBase",
     "OpenAIChatWrapper",
     "OpenAIDALLEWrapper",
     "OpenAIEmbeddingWrapper",
-    "load_model_by_config_name",
-    "read_model_configs",
-    "clear_model_configs",
     "DashScopeChatWrapper",
     "DashScopeImageSynthesisWrapper",
     "DashScopeTextEmbeddingWrapper",
+    "DashScopeMultiModalWrapper",
     "OllamaChatWrapper",
     "OllamaEmbeddingWrapper",
     "OllamaGenerationWrapper",
     "GeminiChatWrapper",
     "GeminiEmbeddingWrapper",
+    "load_model_by_config_name",
+    "read_model_configs",
+    "clear_model_configs",
 ]
 
 _MODEL_CONFIGS: dict[str, dict] = {}
 
 
 def _get_model_wrapper(model_type: str) -> Type[ModelWrapperBase]:
     """Get the specific type of model wrapper
 
     Args:
         model_type (`str`): The model type name.
 
     Returns:
         `Type[ModelWrapperBase]`: The corresponding model wrapper class.
     """
-    if model_type in ModelWrapperBase.type_registry:
-        return ModelWrapperBase.type_registry[  # type: ignore[return-value]
-            model_type
-        ]
-    elif model_type in ModelWrapperBase.registry:
-        return ModelWrapperBase.registry[  # type: ignore[return-value]
-            model_type
-        ]
-    elif model_type in ModelWrapperBase.deprecated_type_registry:
-        cls = ModelWrapperBase.deprecated_type_registry[model_type]
-        logger.warning(
-            f"Model type [{model_type}] will be deprecated in future releases,"
-            f" please use [{cls.model_type}] instead.",
-        )
-        return cls  # type: ignore[return-value]
-    else:
+    wrapper = ModelWrapperBase.get_wrapper(model_type=model_type)
+    if wrapper is None:
         logger.warning(
             f"Unsupported model_type [{model_type}],"
             "use PostApiModelWrapper instead.",
         )
         return PostAPIModelWrapperBase
+    return wrapper
 
 
 def load_model_by_config_name(config_name: str) -> ModelWrapperBase:
     """Load the model by config name."""
     if len(_MODEL_CONFIGS) == 0:
         raise ValueError(
             "No model configs loaded, please call "
@@ -145,28 +128,37 @@
     Returns:
         `dict`:
             The model configs.
     """
     if clear_existing:
         clear_model_configs()
 
+    cfgs = None
+
     if isinstance(configs, str):
         with open(configs, "r", encoding="utf-8") as f:
             cfgs = json.load(f)
 
     if isinstance(configs, dict):
         cfgs = [configs]
 
     if isinstance(configs, list):
         if not all(isinstance(_, dict) for _ in configs):
             raise ValueError(
                 "The model config unit should be a dict.",
             )
         cfgs = configs
 
+    if cfgs is None:
+        raise TypeError(
+            f"Invalid type of model_configs, it could be a dict, a list of "
+            f"dicts, or a path to a json file (containing a dict or a list "
+            f"of dicts), but got {type(configs)}",
+        )
+
     format_configs = _ModelConfig.format_configs(configs=cfgs)
 
     # check if name is unique
     for cfg in format_configs:
         if cfg.config_name in _MODEL_CONFIGS:
             logger.warning(
                 f"config_name [{cfg.config_name}] already exists.",
```

### Comparing `agentscope-0.0.3/src/agentscope/models/config.py` & `agentscope-0.0.4/src/agentscope/models/config.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/models/gemini_model.py` & `agentscope-0.0.4/src/agentscope/models/gemini_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         if api_key is None:
             raise ValueError(
                 "Google api_key must be provided or set as an "
                 "environment variable.",
             )
 
-        genai.configure(api_key=api_key)
+        genai.configure(api_key=api_key, **kwargs)
 
         self.model_name = model_name
 
         self._register_default_metrics()
 
     def _register_default_metrics(self) -> None:
         """Register the default metrics for the model."""
@@ -235,14 +235,16 @@
 
         Returns:
             `List[dict]`:
                 A list with one user message.
         """
         input_msgs = []
         for _ in args:
+            if _ is None:
+                continue
             if isinstance(_, MessageBase):
                 input_msgs.append(_)
             elif isinstance(_, list) and all(
                 isinstance(__, MessageBase) for __ in _
             ):
                 input_msgs.extend(_)
             else:
```

### Comparing `agentscope-0.0.3/src/agentscope/models/model.py` & `agentscope-0.0.4/src/agentscope/models/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 """The configuration file should contain one or a list of model configs,
 and each model config should follow the following format.
 
 .. code-block:: python
 
     {
         "config_name": "{config_name}",
-        "model_type": "openai" | "post_api" | ...,
+        "model_type": "openai_chat" | "post_api" | ...,
         ...
     }
 
 After that, you can specify model by {config_name}.
 
 Note:
     The parameters for different types of models are different. For OpenAI API,
     the format is:
 
         .. code-block:: python
 
             {
                 "config_name": "{id of your model}",
-                "model_type": "openai",
+                "model_type": "openai_chat",
                 "model_name": "{model_name_for_openai, e.g. gpt-3.5-turbo}",
                 "api_key": "{your_api_key}",
                 "organization": "{your_organization, if needed}",
                 "client_args": {
                     # ...
                 },
                 "generate_args": {
@@ -49,24 +49,26 @@
                 "generate_args": {
                     "temperature": 0.5,
                     # ...
                 }
             }
 
 """
+from __future__ import annotations
 import inspect
 import time
 from abc import ABCMeta
 from functools import wraps
-from typing import Sequence, Any, Callable, Union, List
+from typing import Sequence, Any, Callable, Union, List, Type
 
 from loguru import logger
 
 from agentscope.utils import QuotaExceededError
-from .response import ResponseParsingError, ModelResponse
+from .response import ModelResponse
+from ..exception import ResponseParsingError
 
 from ..file_manager import file_manager
 from ..message import MessageBase
 from ..utils import MonitorFactory
 from ..utils.monitor import get_full_name
 from ..utils.tools import _get_timestamp
 from ..constants import _DEFAULT_MAX_RETRIES
@@ -118,32 +120,27 @@
         for itr in range(1, max_retries + 1):
             # Call the model
             response = model_call(self, *args, **kwargs)
 
             # Parse the response if needed
             try:
                 return parse_func(response)
-            except Exception as e:
+            except ResponseParsingError as e:
                 if itr < max_retries:
                     logger.warning(
                         f"Fail to parse response ({itr}/{max_retries}):\n"
                         f"{response}.\n"
                         f"{e.__class__.__name__}: {e}",
                     )
                     time.sleep(_DEFAULT_RETRY_INTERVAL * itr)
                 else:
                     if fault_handler is not None and callable(fault_handler):
                         return fault_handler(response)
                     else:
-                        error_info = f"{e.__class__.__name__}: {e}"
-                        raise ResponseParsingError(
-                            parse_func=parse_func,
-                            error_info=error_info,
-                            response=response,
-                        ) from None
+                        raise
         return {}
 
     return checking_wrapper
 
 
 class _ModelWrapperMeta(ABCMeta):
     """A meta call to replace the model wrapper's __call__ function with
@@ -151,24 +148,24 @@
 
     def __new__(mcs, name: Any, bases: Any, attrs: Any) -> Any:
         if "__call__" in attrs:
             attrs["__call__"] = _response_parse_decorator(attrs["__call__"])
         return super().__new__(mcs, name, bases, attrs)
 
     def __init__(cls, name: Any, bases: Any, attrs: Any) -> None:
-        if not hasattr(cls, "registry"):
-            cls.registry = {}
-            cls.type_registry = {}
-            cls.deprecated_type_registry = {}
+        if not hasattr(cls, "_registry"):
+            cls._registry = {}
+            cls._type_registry = {}
+            cls._deprecated_type_registry = {}
         else:
-            cls.registry[name] = cls
+            cls._registry[name] = cls
             if hasattr(cls, "model_type"):
-                cls.type_registry[cls.model_type] = cls
+                cls._type_registry[cls.model_type] = cls
                 if hasattr(cls, "deprecated_model_type"):
-                    cls.deprecated_type_registry[
+                    cls._deprecated_type_registry[
                         cls.deprecated_model_type
                     ] = cls
         super().__init__(name, bases, attrs)
 
 
 class ModelWrapperBase(metaclass=_ModelWrapperMeta):
     """The base class for model wrapper."""
@@ -197,15 +194,32 @@
             config_name (`str`):
                 The id of the model, which is used to extract configuration
                 from the config file.
         """
         self.monitor = MonitorFactory.get_monitor()
 
         self.config_name = config_name
-        logger.info(f"Initialize model [{config_name}]")
+        logger.info(f"Initialize model by configuration [{config_name}]")
+
+    @classmethod
+    def get_wrapper(cls, model_type: str) -> Type[ModelWrapperBase]:
+        """Get the specific model wrapper"""
+        if model_type in cls._type_registry:
+            return cls._type_registry[model_type]  # type: ignore[return-value]
+        elif model_type in cls._registry:
+            return cls._registry[model_type]  # type: ignore[return-value]
+        elif model_type in cls._deprecated_type_registry:
+            deprecated_cls = cls._deprecated_type_registry[model_type]
+            logger.warning(
+                f"Model type [{model_type}] will be deprecated in future "
+                f"releases, please use [{deprecated_cls.model_type}] instead.",
+            )
+            return deprecated_cls  # type: ignore[return-value]
+        else:
+            return None  # type: ignore[return-value]
 
     def __call__(self, *args: Any, **kwargs: Any) -> ModelResponse:
         """Processing input with the model."""
         raise NotImplementedError(
             f"Model Wrapper [{type(self).__name__}]"
             f" is missing the required `__call__`"
             f" method.",
```

### Comparing `agentscope-0.0.3/src/agentscope/models/ollama_model.py` & `agentscope-0.0.4/src/agentscope/models/ollama_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
     def __init__(
         self,
         config_name: str,
         model_name: str,
         options: dict = None,
         keep_alive: str = "5m",
+        **kwargs: Any,
     ) -> None:
         """Initialize the model wrapper for Ollama API.
 
         Args:
             model_name (`str`):
                 The model name used in ollama API.
             options (`dict`, default `None`):
@@ -130,18 +131,18 @@
             },
             response=response,
         )
 
         # step3: monitor the response
         self.update_monitor(
             call_counter=1,
-            prompt_tokens=response["prompt_eval_count"],
-            completion_tokens=response["eval_count"],
-            total_tokens=response["prompt_eval_count"]
-            + response["eval_count"],
+            prompt_tokens=response.get("prompt_eval_count", 0),
+            completion_tokens=response.get("eval_count", 0),
+            total_tokens=response.get("prompt_eval_count", 0)
+            + response.get("eval_count", 0),
         )
 
         # step4: return response
         return ModelResponse(
             text=response["message"]["content"],
             raw=response,
         )
@@ -367,18 +368,18 @@
             },
             response=response,
         )
 
         # step4: monitor the response
         self.update_monitor(
             call_counter=1,
-            prompt_tokens=response["prompt_eval_count"],
-            completion_tokens=response["eval_count"],
-            total_tokens=response["prompt_eval_count"]
-            + response["eval_count"],
+            prompt_tokens=response.get("prompt_eval_count", 0),
+            completion_tokens=response.get("eval_count", 0),
+            total_tokens=response.get("prompt_eval_count", 0)
+            + response.get("eval_count", 0),
         )
 
         # step5: return response
         return ModelResponse(
             text=response["response"],
             raw=response,
         )
@@ -413,14 +414,16 @@
 
         Returns:
             `str`:
                 The formatted string prompt.
         """
         input_msgs = []
         for _ in args:
+            if _ is None:
+                continue
             if isinstance(_, MessageBase):
                 input_msgs.append(_)
             elif isinstance(_, list) and all(
                 isinstance(__, MessageBase) for __ in _
             ):
                 input_msgs.extend(_)
             else:
```

### Comparing `agentscope-0.0.3/src/agentscope/models/openai_model.py` & `agentscope-0.0.4/src/agentscope/models/openai_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,14 +344,21 @@
         )
 
         # step4: update monitor accordingly
         self.update_monitor(call_counter=1)
 
         # step5: return response
         raw_response = response.model_dump()
+        if "data" not in raw_response:
+            if "error" in raw_response:
+                error_msg = raw_response["error"]["message"]
+            else:
+                error_msg = raw_response
+            logger.error(f"Error in OpenAI API call:\n{error_msg}")
+            raise ValueError(f"Error in OpenAI API call:\n{error_msg}")
         images = raw_response["data"]
         # Get image urls as a list
         urls = [_["url"] for _ in images]
 
         if save_local:
             # Return local url if save_local is True
             urls = [file_manager.save_image(_) for _ in urls]
```

### Comparing `agentscope-0.0.3/src/agentscope/models/post_model.py` & `agentscope-0.0.4/src/agentscope/models/post_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             logger.error(json.dumps(request_kwargs, indent=4))
             raise RuntimeError(
                 f"Failed to call the model with {response.json()}",
             )
 
 
 class PostAPIChatWrapper(PostAPIModelWrapperBase):
-    """A post api model wrapper compatilble with openai chat, e.g., vLLM,
+    """A post api model wrapper compatible with openai chat, e.g., vLLM,
     FastChat."""
 
     model_type: str = "post_api_chat"
 
     def _parse_response(self, response: dict) -> ModelResponse:
         return ModelResponse(
             text=response["data"]["response"]["choices"][0]["message"][
@@ -210,21 +210,28 @@
                     f"of Msg objects, got {type(arg)}.",
                 )
 
         return messages
 
 
 class PostAPIDALLEWrapper(PostAPIModelWrapperBase):
-    """A post api model wrapper compatible with openai dalle"""
+    """A post api model wrapper compatible with openai dall_e"""
 
     model_type: str = "post_api_dall_e"
 
     deprecated_model_type: str = "post_api_dalle"
 
     def _parse_response(self, response: dict) -> ModelResponse:
+        if "data" not in response["data"]["response"]:
+            if "error" in response["data"]["response"]:
+                error_msg = response["data"]["response"]["error"]["message"]
+            else:
+                error_msg = response["data"]["response"]
+            logger.error(f"Error in API call:\n{error_msg}")
+            raise ValueError(f"Error in API call:\n{error_msg}")
         urls = [img["url"] for img in response["data"]["response"]["data"]]
         return ModelResponse(image_urls=urls)
 
     def format(
         self,
         *args: Union[MessageBase, Sequence[MessageBase]],
     ) -> Union[List[dict], str]:
```

### Comparing `agentscope-0.0.3/src/agentscope/msghub.py` & `agentscope-0.0.4/src/agentscope/msghub.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         announcement: Optional[Union[Sequence[dict], dict]] = None,
     ) -> None:
         """Initialize a msghub manager from the given arguments.
 
         Args:
             participants (`Sequence[AgentBase]`):
                 The Sequence of participants in the msghub.
-            announcement (`Optional[Union[list[dict], dict]]`, defaults to
-            `None`):
+            announcement
+                (`Optional[Union[list[dict], dict]]`, defaults to `None`):
                 The message that will be broadcast to all participants at
                 the first without requiring response.
         """
         self.participants = participants
         self.announcement = announcement
 
     def __enter__(self) -> MsgHubManager:
```

### Comparing `agentscope-0.0.3/src/agentscope/pipelines/functional.py` & `agentscope-0.0.4/src/agentscope/pipelines/functional.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/pipelines/pipeline.py` & `agentscope-0.0.4/src/agentscope/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/prompt.py` & `agentscope-0.0.4/src/agentscope/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         model: ModelWrapperBase,
         shrink_policy: ShrinkPolicy = ShrinkPolicy.TRUNCATE,
         max_length: Optional[int] = None,
         prompt_type: Optional[PromptType] = None,
         max_summary_length: int = 200,
         summarize_model: Optional[ModelWrapperBase] = None,
     ) -> None:
-        """
+        """Init PromptEngine.
 
         Args:
             model (`ModelWrapperBase`):
                 The target model for prompt engineering.
             shrink_policy (`ShrinkPolicy`, defaults to
             `ShrinkPolicy.TRUNCATE`):
                 The shrink policy for prompt engineering, defaults to
@@ -48,42 +48,48 @@
                 The max length of summary, if it is None, it will be set to the
                 max length of the model.
             summarize_model (`Optional[ModelWrapperBase]`, defaults to `None`):
                 The model used for summarization, if it is None, it will be
                 set to `model`.
 
         Note:
+
             1. TODO: Shrink function is still under development.
+
             2. If the argument `max_length` and `prompt_type` are not given,
             they will be set according to the given model.
+
             3. `shrink_policy` is used when the prompt is too long, it can
             be set to `ShrinkPolicy.TRUNCATE` or `ShrinkPolicy.SUMMARIZE`.
+
                 a. `ShrinkPolicy.TRUNCATE` will truncate the prompt to the
                 desired length.
+
                 b. `ShrinkPolicy.SUMMARIZE` will summarize partial of the
                 dialog history to save space. The summarization model
                 defaults to `model` if not given.
 
         Example:
+
             With prompt engine, we encapsulate different operations for
             string- and list-style prompt, and block the prompt engineering
             process from the user.
             As a user, you can just combine you prompt as follows.
 
-            ```python
-            # prepare the component
-            system_prompt = "You're a helpful assistant ..."
-            hint_prompt = "You should response in Json format."
-            prefix = "assistant: "
-
-            # initialize the prompt engine and join the prompt
-            engine = PromptEngine(model)
-            prompt = engine.join(system_prompt, memory.get_memory(),
-            hint_prompt, prefix)
-            ```
+            .. code-block:: python
+
+                # prepare the component
+                system_prompt = "You're a helpful assistant ..."
+                hint_prompt = "You should response in Json format."
+                prefix = "assistant: "
+
+                # initialize the prompt engine and join the prompt
+                engine = PromptEngine(model)
+                prompt = engine.join(system_prompt, memory.get_memory(),
+                hint_prompt, prefix)
         """
         self.model = model
         self.shrink_policy = shrink_policy
         self.max_length = max_length
 
         if prompt_type is None:
             if isinstance(model, OpenAIWrapperBase):
```

### Comparing `agentscope-0.0.3/src/agentscope/rpc/__init__.py` & `agentscope-0.0.4/src/agentscope/rpc/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     RpcAgentStub = Any
     add_RpcAgentServicer_to_server = Any
 
 
 __all__ = [
     "RpcAgentClient",
     "ResponseStub",
-    "call_in_thread",
     "RpcMsg",
     "RpcAgentServicer",
     "RpcAgentStub",
+    "call_in_thread",
     "add_RpcAgentServicer_to_server",
 ]
```

### Comparing `agentscope-0.0.3/src/agentscope/rpc/rpc_agent_client.py` & `agentscope-0.0.4/src/agentscope/rpc/rpc_agent_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # -*- coding: utf-8 -*-
 """ Client of rpc agent server """
 
-import json
 import threading
+import base64
 from typing import Any, Optional
 from loguru import logger
 
 try:
+    import dill
     import grpc
+    from grpc import RpcError
 except ImportError:
+    dill = None
     grpc = None
+    RpcError = None
 
 try:
     from agentscope.rpc.rpc_agent_pb2 import RpcMsg  # pylint: disable=E0611
     from agentscope.rpc.rpc_agent_pb2_grpc import RpcAgentStub
 except ModuleNotFoundError:
     RpcMsg = Any  # type: ignore[misc]
     RpcAgentStub = Any
@@ -59,26 +63,22 @@
                     target_func=func_name,
                     agent_id=self.agent_id,
                 ),
                 timeout=timeout,
             )
             return result_msg.value
 
-    def create_agent(self, agent_configs: Optional[dict]) -> None:
+    def create_agent(self, agent_configs: dict) -> None:
         """Create a new agent for this client."""
         try:
             if self.agent_id is None or len(self.agent_id) == 0:
                 return
             self.call_func(
-                func_name="_create_agent",
-                value=(
-                    None
-                    if agent_configs is None
-                    else json.dumps(agent_configs)
-                ),
+                "_create_agent",
+                base64.b64encode(dill.dumps(agent_configs)).decode("utf-8"),
             )
         except Exception as e:
             logger.error(
                 f"Fail to create agent with id [{self.agent_id}]: {e}",
             )
 
     def delete_agent(self) -> None:
@@ -113,32 +113,36 @@
             while self.response is None:
                 self.condition.wait()
             return self.response
 
 
 def call_in_thread(
     client: RpcAgentClient,
-    x: dict,
+    value: str,
     func_name: str,
 ) -> ResponseStub:
     """Call rpc function in a sub-thread.
 
     Args:
         client (`RpcAgentClient`): the rpc client.
-        x (`dict`): the value of the reqeust.
+        x (`str`): the value of the reqeust.
         func_name (`str`): the name of the function being called.
 
     Returns:
         `ResponseStub`: a stub to get the response.
     """
     stub = ResponseStub()
 
     def wrapper() -> None:
-        resp = client.call_func(
-            func_name=func_name,
-            value=x.serialize() if x is not None else "",
-        )
-        stub.set_response(resp)  # type: ignore[arg-type]
+        try:
+            resp = client.call_func(
+                func_name=func_name,
+                value=value,
+            )
+            stub.set_response(resp)  # type: ignore[arg-type]
+        except RpcError as e:
+            logger.error(f"Fail to call {func_name} in thread: {e}")
+            stub.set_response(str(e))
 
     thread = threading.Thread(target=wrapper)
     thread.start()
     return stub
```

### Comparing `agentscope-0.0.3/src/agentscope/rpc/rpc_agent_pb2.py` & `agentscope-0.0.4/src/agentscope/rpc/rpc_agent_pb2.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/rpc/rpc_agent_pb2_grpc.py` & `agentscope-0.0.4/src/agentscope/rpc/rpc_agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/__init__.py` & `agentscope-0.0.4/src/agentscope/service/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,75 @@
 # -*- coding: utf-8 -*-
 """ Import all service-related modules in the package."""
 from loguru import logger
 
 from .execute_code.exec_python import execute_python_code
+from .execute_code.exec_shell import execute_shell_command
 from .file.common import (
     create_file,
     delete_file,
     move_file,
     create_directory,
     delete_directory,
     move_directory,
+    list_directory_content,
+    get_current_directory,
 )
 from .file.text import read_text_file, write_text_file
 from .file.json import read_json_file, write_json_file
 from .sql_query.mysql import query_mysql
 from .sql_query.sqlite import query_sqlite
 from .sql_query.mongodb import query_mongodb
-from .web_search.search import bing_search, google_search
+from .web.search import bing_search, google_search
+from .web.arxiv import arxiv_search
 from .service_response import ServiceResponse
-from .service_factory import ServiceFactory
+from .service_toolkit import ServiceToolkit
+from .service_toolkit import ServiceFactory
 from .retrieval.similarity import cos_sim
 from .text_processing.summarization import summarization
 from .retrieval.retrieval_from_list import retrieve_from_list
 from .service_status import ServiceExecStatus
-from .web_search.web_digest import digest_webpage, load_web, parse_html_to_text
+from .web.web_digest import digest_webpage, load_web, parse_html_to_text
+from .web.download import download_from_url
 
 
 def get_help() -> None:
     """Get help message."""
     help_msg = f"The following service are available:\n{__all__}"
     logger.info(help_msg)
 
 
 __all__ = [
+    "ServiceResponse",
+    "ServiceExecStatus",
+    "ServiceToolkit",
+    "get_help",
     "execute_python_code",
+    "execute_shell_command",
     "create_file",
     "delete_file",
     "move_file",
     "create_directory",
     "delete_directory",
     "move_directory",
+    "list_directory_content",
+    "get_current_directory",
     "read_text_file",
     "write_text_file",
     "read_json_file",
     "write_json_file",
     "bing_search",
     "google_search",
+    "arxiv_search",
     "query_mysql",
     "query_sqlite",
     "query_mongodb",
-    "ServiceResponse",
-    "ServiceFactory",
     "cos_sim",
     "summarization",
     "retrieve_from_list",
-    "ServiceExecStatus",
     "digest_webpage",
     "load_web",
     "parse_html_to_text",
+    "download_from_url",
+    # to be deprecated
+    "ServiceFactory",
 ]
```

### Comparing `agentscope-0.0.3/src/agentscope/service/execute_code/exec_python.py` & `agentscope-0.0.4/src/agentscope/service/execute_code/exec_python.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/file/common.py` & `agentscope-0.0.4/src/agentscope/service/file/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 """ Common operators for file and directory. """
 import os
 import shutil
+from typing import List
 
 from agentscope.utils.common import write_file
 from agentscope.service.service_response import ServiceResponse
 from agentscope.service.service_status import ServiceExecStatus
 
 
 def create_file(file_path: str, content: str = "") -> ServiceResponse:
@@ -197,7 +198,65 @@
         )
     except Exception as e:
         error_message = f"{e.__class__.__name__}: {e}"
         return ServiceResponse(
             status=ServiceExecStatus.ERROR,
             content=error_message,
         )
+
+
+def list_directory_content(directory_path: str) -> ServiceResponse:
+    """
+    List the contents of a directory. i.e. ls -a
+
+    Args:
+        directory_path (`str`):
+            The path of the directory to show.
+
+    Returns:
+        `ServiceResponse`: The results contain a list of direcotry contents,
+        or an error message if any, including the error type.
+    """
+    if not os.path.exists(directory_path):
+        return ServiceResponse(
+            status=ServiceExecStatus.ERROR,
+            content="FileNotFoundError: The directory does not exist.",
+        )
+    if not os.path.isdir(directory_path):
+        return ServiceResponse(
+            status=ServiceExecStatus.ERROR,
+            content="FileNotFoundError: The path is not a directory",
+        )
+    try:
+        ls_result: List[str] = os.listdir(directory_path)
+        return ServiceResponse(
+            status=ServiceExecStatus.SUCCESS,
+            content=ls_result,
+        )
+    except Exception as e:
+        error_message = f"{e.__class__.__name__}: {e}"
+        return ServiceResponse(
+            status=ServiceExecStatus.ERROR,
+            content=error_message,
+        )
+
+
+def get_current_directory() -> ServiceResponse:
+    """
+    Get the current working directory path.
+
+    Returns:
+        `ServiceResponse`: The current working directory path, or an error
+        message if any, including the error type.
+    """
+    try:
+        cwd = os.getcwd()
+        return ServiceResponse(
+            status=ServiceExecStatus.SUCCESS,
+            content=cwd,
+        )
+    except Exception as e:
+        error_message = f"{e.__class__.__name__}: {e}"
+        return ServiceResponse(
+            status=ServiceExecStatus.ERROR,
+            content=error_message,
+        )
```

### Comparing `agentscope-0.0.3/src/agentscope/service/file/json.py` & `agentscope-0.0.4/src/agentscope/service/file/json.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/file/text.py` & `agentscope-0.0.4/src/agentscope/service/file/text.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/retrieval/retrieval_from_list.py` & `agentscope-0.0.4/src/agentscope/service/retrieval/retrieval_from_list.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/retrieval/similarity.py` & `agentscope-0.0.4/src/agentscope/service/retrieval/similarity.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/service_response.py` & `agentscope-0.0.4/src/agentscope/service/service_response.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/sql_query/mongodb.py` & `agentscope-0.0.4/src/agentscope/service/sql_query/mongodb.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/sql_query/mysql.py` & `agentscope-0.0.4/src/agentscope/service/sql_query/mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """query in Mysql """
 from typing import Optional
 from typing import Any
 
 from ..service_response import ServiceResponse
-from ...utils.common import if_change_database
+from ...utils.common import _if_change_database
 from ...service.service_status import ServiceExecStatus
 
 try:
     import pymysql
 except ImportError:
     pymysql = None
 
@@ -49,15 +49,15 @@
 
     Returns:
         `ServiceResponse`: A `ServiceResponse` object that contains
         execution results or error message.
     """
 
     # Check if the query is safe
-    if not allow_change_data and not if_change_database(query):
+    if not allow_change_data and not _if_change_database(query):
         raise ValueError(
             "Unsafe SQL query detected. Only SELECT statements are allowed. "
             "If you want to allow changing data in the database, "
             "set `allow_change_data` to `True`.",
         )
 
     # Limit the number of results by adding LIMIT keywords if necessary
@@ -76,15 +76,15 @@
             database=database,
             **kwargs,
         )
 
         cursor = conn.cursor()
         cursor.execute(query)
 
-        if if_change_database(query):
+        if _if_change_database(query):
             conn.commit()
 
         cursor.close()
         conn.close()
 
         # Fetch the results
         results = cursor.fetchall()
```

### Comparing `agentscope-0.0.3/src/agentscope/service/sql_query/sqlite.py` & `agentscope-0.0.4/src/agentscope/service/sql_query/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """ Query in sqlite """
 from typing import Optional
 from typing import Any
 
 from ...service.service_response import ServiceResponse
-from ...utils.common import if_change_database
+from ...utils.common import _if_change_database
 from ...service.service_status import ServiceExecStatus
 
 try:
     import sqlite3
 except ImportError:
     sqlite3 = None
 
@@ -35,15 +35,15 @@
 
     Returns:
         `ServiceResponse`: A `ServiceResponse` object that contains
         execution results or error message.
     """
 
     # Check if the query is safe
-    if not allow_change_data and not if_change_database(query):
+    if not allow_change_data and not _if_change_database(query):
         raise ValueError(
             "Unsafe SQL query detected. Only SELECT statements are allowed. "
             "If you want to allow changing data in the database, "
             "set `allow_change_data` to `True`.",
         )
 
     # Limit the number of results by adding LIMIT keywords if necessary
@@ -54,15 +54,15 @@
     try:
         conn = sqlite3.connect(database, **kwargs)
         cursor = conn.cursor()
         cursor.execute(query)
         results = cursor.fetchall()
 
         # commit the change if needed
-        if if_change_database(query):
+        if _if_change_database(query):
             conn.commit()
 
         cursor.close()
         conn.close()
 
         return ServiceResponse(
             status=ServiceExecStatus.SUCCESS,
```

### Comparing `agentscope-0.0.3/src/agentscope/service/text_processing/summarization.py` & `agentscope-0.0.4/src/agentscope/service/text_processing/summarization.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/web_search/search.py` & `agentscope-0.0.4/src/agentscope/service/web/search.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/service/web_search/web_digest.py` & `agentscope-0.0.4/src/agentscope/service/web/web_digest.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,16 @@
 
 def digest_webpage(
     web_text_or_url: str,
     model: ModelWrapperBase = None,
     html_selected_tags: Sequence[str] = ("h", "p", "li", "div", "a"),
     digest_prompt: str = DEFAULT_WEB_SYS_PROMPT,
 ) -> ServiceResponse:
-    """
+    """Digest the given webpage.
+
     Args:
         web_text_or_url (str): preprocessed web text or url to the web page
         model (ModelWrapperBase): the model to digest the web content
         html_selected_tags (Sequence[str]):
             the text in elements of `html_selected_tags` will
             be extracted and feed to the model
         digest_prompt (str): system prompt for the model to digest
```

### Comparing `agentscope-0.0.3/src/agentscope/utils/common.py` & `agentscope-0.0.4/src/agentscope/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 import re
 import signal
 import sys
 import tempfile
 import threading
 from typing import Any, Generator, Optional, Union
-from loguru import logger
 import requests
 
 from agentscope.service.service_response import ServiceResponse
 from agentscope.service.service_status import ServiceExecStatus
 
 
 @contextlib.contextmanager
@@ -153,22 +152,21 @@
         if headers:
             response = requests.get(url, params=params, headers=headers)
         else:
             response = requests.get(url, params=params)
         # This will raise an exception for HTTP error codes
         response.raise_for_status()
     except requests.RequestException as e:
-        logger.error(e)
         return str(e)
     # Parse the JSON response
     search_results = response.json()
     return search_results
 
 
-def if_change_database(sql_query: str) -> bool:
+def _if_change_database(sql_query: str) -> bool:
     """Check whether SQL query only contains SELECT query"""
     # Compile the regex pattern outside the function for better performance
     pattern_unsafe_sql = re.compile(
         r"\b(INSERT|UPDATE|DELETE|REPLACE|CREATE|ALTER|DROP|TRUNCATE|USE)\b",
         re.IGNORECASE,
     )
```

### Comparing `agentscope-0.0.3/src/agentscope/utils/logging_utils.py` & `agentscope-0.0.4/src/agentscope/utils/logging_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,15 @@
             filter=lambda record: record["level"].name != LEVEL_CHAT_SAVE,
             format=_level_format,
             enqueue=True,
             level=level,
         )
 
     if path_log is not None:
-        if not os.path.exists(path_log):
-            os.makedirs(path_log)
+        os.makedirs(path_log, exist_ok=True)
         path_log_file = os.path.join(path_log, "logging.log")
         path_chat_file = os.path.join(
             path_log,
             "logging.chat",
         )
 
         # save all logging into file
```

### Comparing `agentscope-0.0.3/src/agentscope/utils/monitor.py` & `agentscope-0.0.4/src/agentscope/utils/monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -240,56 +240,111 @@
         """
         self.message = f"Metric [{name}] exceeds quota."
         self.name = name
         super().__init__(self.message)
 
 
 @contextmanager
-def sqlite_transaction(db_path: str) -> Generator:
+def sqlite_transaction(db_path: str, timeout: float = 30.0) -> Generator:
     """Get a sqlite transaction cursor.
 
     Args:
         db_path (`str`): path to the sqlite db file
+        timeout (`float`): timeout of the connection
 
     Yields:
         `Generator`: a cursor with transaction
     """
-    conn = sqlite3.connect(db_path)
+    conn = sqlite3.connect(db_path, timeout=timeout)
     cursor = conn.cursor()
     try:
         conn.execute("BEGIN")
         yield cursor
         conn.commit()
     except Exception as e:
         conn.rollback()
         raise e
     finally:
         cursor.close()
         conn.close()
 
 
 @contextmanager
-def sqlite_cursor(db_path: str) -> Generator:
+def sqlite_cursor(db_path: str, timeout: float = 30.0) -> Generator:
     """Get a sqlite cursor.
 
     Args:
         db_path (`str`): path to the sqlite db file
+        timeout (`float`): timeout of the connection
 
     Yields:
         `Generator`: a cursor
     """
-    conn = sqlite3.connect(db_path)
+    conn = sqlite3.connect(db_path, timeout=timeout)
     cursor = conn.cursor()
     try:
         yield cursor
     finally:
         cursor.close()
         conn.close()
 
 
+class DummyMonitor(MonitorBase):
+    """A monitor that does nothing"""
+
+    def register(
+        self,
+        metric_name: str,
+        metric_unit: Optional[str] = None,
+        quota: Optional[float] = None,
+    ) -> bool:
+        return True
+
+    def exists(self, metric_name: str) -> bool:
+        return True
+
+    def add(self, metric_name: str, value: float) -> bool:
+        return True
+
+    def update(self, values: dict, prefix: Optional[str] = None) -> None:
+        return None
+
+    def clear(self, metric_name: str) -> bool:
+        return True
+
+    def remove(self, metric_name: str) -> bool:
+        return True
+
+    def get_value(self, metric_name: str) -> Optional[float]:
+        return 0.0
+
+    def get_unit(self, metric_name: str) -> Optional[str]:
+        return ""
+
+    def get_quota(self, metric_name: str) -> Optional[float]:
+        return 0.0
+
+    def set_quota(self, metric_name: str, quota: float) -> bool:
+        return True
+
+    def get_metric(self, metric_name: str) -> Optional[dict]:
+        return {}
+
+    def get_metrics(self, filter_regex: Optional[str] = None) -> dict:
+        return {}
+
+    def register_budget(
+        self,
+        model_name: str,
+        value: float,
+        prefix: Optional[str] = "local",
+    ) -> bool:
+        return True
+
+
 class SqliteMonitor(MonitorBase):
     """A monitor based on sqlite"""
 
     def __init__(
         self,
         db_path: str,
         table_name: str = _DEFAULT_MONITOR_TABLE_NAME,
@@ -640,14 +695,16 @@
 
         Returns:
             `MonitorBase`: the monitor instance.
         """
         if cls._instance is None:
             if impl_type is None or impl_type.lower() == "sqlite":
                 cls._instance = SqliteMonitor(db_path=db_path)
+            elif impl_type == "dummy":
+                cls._instance = DummyMonitor()
             else:
                 raise NotImplementedError(
                     "Monitor with type [{type}] is not implemented.",
                 )
         return cls._instance  # type: ignore[return-value]
 
     @classmethod
```

### Comparing `agentscope-0.0.3/src/agentscope/utils/token_utils.py` & `agentscope-0.0.4/src/agentscope/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/_app.py` & `agentscope-0.0.4/src/agentscope/web/_app.py`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/css/bootstrap.min.css` & `agentscope-0.0.4/src/agentscope/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/css/colors.css` & `agentscope-0.0.4/src/agentscope/web/static/css/colors.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/css/components.css` & `agentscope-0.0.4/src/agentscope/web/static/css/components.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/css/home.css` & `agentscope-0.0.4/src/agentscope/web/static/css/home.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/css/run.css` & `agentscope-0.0.4/src/agentscope/web/static/css/run.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/css/size.css` & `agentscope-0.0.4/src/agentscope/web/static/css/size.css`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/fonts/KRYPTON.ttf` & `agentscope-0.0.4/src/agentscope/web/static/fonts/KRYPTON.ttf`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/fonts/OSWALD.ttf` & `agentscope-0.0.4/src/agentscope/web/static/fonts/OSWALD.ttf`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/js/bootstrap-table.min.js` & `agentscope-0.0.4/src/agentscope/web/static/js/bootstrap-table.min.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/js/bootstrap.bundle.min.js` & `agentscope-0.0.4/src/agentscope/web/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/js/home.js` & `agentscope-0.0.4/src/agentscope/web/static/js/home.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/js/jquery-3.3.1.min.js` & `agentscope-0.0.4/src/agentscope/web/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/js/run.js` & `agentscope-0.0.4/src/agentscope/web/static/js/run.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/static/js/socket.io.js` & `agentscope-0.0.4/src/agentscope/web/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `agentscope-0.0.3/src/agentscope/web/studio/studio.py` & `agentscope-0.0.4/src/agentscope/web/studio/studio.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,52 +26,72 @@
     ResetException,
     check_uuid,
     send_msg,
     generate_image_from_name,
     audio2text,
     send_reset_msg,
     thread_local_data,
+    cycle_dots,
 )
+from agentscope.web.studio.constants import _SPEAK
 
 MAX_NUM_DISPLAY_MSG = 20
 FAIL_COUNT_DOWN = 30
 
 
 def init_uid_list() -> list:
     """Initialize an empty list for storing user IDs."""
     return []
 
 
 glb_history_dict = defaultdict(init_uid_list)
+glb_doing_signal_dict = defaultdict(init_uid_list)
 glb_signed_user = []
 
 
 def reset_glb_var(uid: str) -> None:
     """Reset global variables for a given user ID."""
     global glb_history_dict
+    global glb_doing_signal_dict
     glb_history_dict[uid] = init_uid_list()
+    glb_doing_signal_dict[uid] = init_uid_list()
 
 
 def get_chat(uid: str) -> list[list]:
     """Retrieve chat messages for a given user ID."""
     uid = check_uuid(uid)
     global glb_history_dict
+    global glb_doing_signal_dict
+
     line = get_chat_msg(uid=uid)
     # TODO: Optimize the display effect, currently there is a problem of
     #  output display jumping
     if line:
-        glb_history_dict[uid] += [line]
+        if line[1] and line[1]["text"] == _SPEAK:
+            line[1]["text"] = ""
+            glb_doing_signal_dict[uid] = line
+        else:
+            glb_history_dict[uid] += [line]
+            glb_doing_signal_dict[uid] = []
     dial_msg = []
     for line in glb_history_dict[uid]:
         _, msg = line
         if isinstance(msg, dict):
             dial_msg.append(line)
         else:
             # User chat, format: (msg, None)
             dial_msg.append(line)
+    if glb_doing_signal_dict[uid]:
+        if glb_doing_signal_dict[uid][1]:
+            text = cycle_dots(glb_doing_signal_dict[uid][1]["text"])
+            glb_doing_signal_dict[uid][1]["text"] = text
+            glb_doing_signal_dict[uid][1]["id"] = str(time.time())
+            glb_doing_signal_dict[uid][1]["flushing"] = False
+
+        dial_msg.append(glb_doing_signal_dict[uid])
     return dial_msg[-MAX_NUM_DISPLAY_MSG:]
 
 
 def send_audio(audio_term: str, uid: str) -> None:
     """Convert audio input to text and send as a chat message."""
     uid = check_uuid(uid)
     content = audio2text(audio_path=audio_term)
@@ -171,15 +191,26 @@
     # Save the current working directory
     # Change the current working directory to the directory where
     os.chdir(script_dir)
 
     def start_game(uid: str) -> None:
         """Start the main game loop."""
         thread_local_data.uid = uid
-        main = import_function_from_path(script_path, "main")
+        if script_path.endswith(".py"):
+            main = import_function_from_path(script_path, "main")
+        elif script_path.endswith(".json"):
+            from agentscope.web.workstation.workflow import (
+                start_workflow,
+                load_config,
+            )
+
+            config = load_config(script_path)
+            main = lambda: start_workflow(config)
+        else:
+            raise ValueError(f"Unrecognized file formats: {script_path}")
 
         while True:
             try:
                 main()
             except ResetException:
                 print(f"Reset Successfully：{uid} ")
             except Exception as e:
```

### Comparing `agentscope-0.0.3/src/agentscope/web/studio/utils.py` & `agentscope-0.0.4/src/agentscope/web/studio/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 
 def send_reset_msg(uid: Optional[str] = None) -> None:
     """Sends a reset message to the web UI."""
     uid = check_uuid(uid)
     global glb_uid_dict
     glb_queue_reset_msg = glb_uid_dict[uid]["glb_queue_reset_msg"]
     glb_queue_reset_msg.put([None, "**Reset**"])
+    send_player_input("**Reset**", uid)
 
 
 def get_reset_msg(uid: Optional[str] = None) -> None:
     """Retrieves a reset message from the queue, if available."""
     global glb_uid_dict
     glb_queue_reset_msg = glb_uid_dict[uid]["glb_queue_reset_msg"]
     if not glb_queue_reset_msg.empty():
@@ -182,20 +183,30 @@
         callback=callback,
     )
 
     result = rec.call(audio_path)
     return " ".join([s["text"] for s in result["output"]["sentence"]])
 
 
+def cycle_dots(text: str, num_dots: int = 3) -> str:
+    """display thinking dots before agent reply"""
+    current_dots = len(text) - len(text.rstrip("."))
+    next_dots = (current_dots + 1) % (num_dots + 1)
+    if next_dots == 0:
+        next_dots = 1
+    return text.rstrip(".") + "." * next_dots
+
+
 def user_input(
     prefix: str = "User input: ",
     timeout: Optional[int] = None,
 ) -> str:
     """get user input"""
     if hasattr(thread_local_data, "uid"):
+        get_reset_msg(uid=thread_local_data.uid)
         content = get_player_input(
             timeout=timeout,
             uid=thread_local_data.uid,
         )
     else:
         if timeout:
             from inputimeout import inputimeout, TimeoutOccurred
```

### Comparing `agentscope-0.0.3/src/agentscope.egg-info/PKG-INFO` & `agentscope-0.0.4/src/agentscope.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agentscope
-Version: 0.0.3
+Version: 0.0.4
 Summary: AgentScope: A Flexible yet Robust Multi-Agent Platform.
 Home-page: https://github.com/modelscope/agentscope
-Download-URL: https://github.com/modelscope/agentscope/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/modelscope/agentscope/archive/v0.0.4.tar.gz
 Author: SysML team of Alibaba Tongyi Lab 
 Author-email: gaodawei.gdw@alibaba-inc.com
 License: Apache License 2.0
 Keywords: deep-learning,multi agents,agents
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -49,14 +49,15 @@
 Requires-Dist: openai>=1.3.0; extra == "distribute"
 Requires-Dist: ollama>=0.1.7; extra == "distribute"
 Requires-Dist: google-generativeai>=0.4.0; extra == "distribute"
 Requires-Dist: grpcio==1.60.0; extra == "distribute"
 Requires-Dist: grpcio-tools==1.60.0; extra == "distribute"
 Requires-Dist: protobuf==4.25.0; extra == "distribute"
 Requires-Dist: expiringdict; extra == "distribute"
+Requires-Dist: dill; extra == "distribute"
 Provides-Extra: dev
 Requires-Dist: docstring_parser; extra == "dev"
 Requires-Dist: loguru==0.6.0; extra == "dev"
 Requires-Dist: tiktoken; extra == "dev"
 Requires-Dist: Pillow; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: chardet; extra == "dev"
@@ -90,38 +91,42 @@
 Requires-Dist: openai>=1.3.0; extra == "full"
 Requires-Dist: ollama>=0.1.7; extra == "full"
 Requires-Dist: google-generativeai>=0.4.0; extra == "full"
 Requires-Dist: grpcio==1.60.0; extra == "full"
 Requires-Dist: grpcio-tools==1.60.0; extra == "full"
 Requires-Dist: protobuf==4.25.0; extra == "full"
 Requires-Dist: expiringdict; extra == "full"
+Requires-Dist: dill; extra == "full"
 Requires-Dist: docker; extra == "full"
 Requires-Dist: pymongo; extra == "full"
 Requires-Dist: pymysql; extra == "full"
 Requires-Dist: beautifulsoup4; extra == "full"
+Requires-Dist: feedparser; extra == "full"
 Requires-Dist: sphinx; extra == "full"
 Requires-Dist: sphinx-autobuild; extra == "full"
 Requires-Dist: sphinx_rtd_theme; extra == "full"
 Requires-Dist: myst-parser; extra == "full"
 Requires-Dist: sphinxcontrib-mermaid; extra == "full"
 Requires-Dist: pytest; extra == "full"
 Requires-Dist: pytest-cov; extra == "full"
 Requires-Dist: pre-commit; extra == "full"
+Requires-Dist: networkx; extra == "full"
 Requires-Dist: gradio==4.19.1; extra == "full"
 Requires-Dist: modelscope_studio==0.0.5; extra == "full"
+Requires-Dist: black; extra == "full"
 
 English | [**中文**](README_ZH.md)
 
 # AgentScope
 
 Start building LLM-empowered multi-agent applications in an easier way.
 
 [![](https://img.shields.io/badge/cs.MA-2402.14034-B31C1C?logo=arxiv&logoColor=B31C1C)](https://arxiv.org/abs/2402.14034)
 [![](https://img.shields.io/badge/python-3.9+-blue)](https://pypi.org/project/agentscope/)
-[![](https://img.shields.io/badge/pypi-v0.0.2-blue?logo=pypi)](https://pypi.org/project/agentscope/)
+[![](https://img.shields.io/badge/pypi-v0.0.4-blue?logo=pypi)](https://pypi.org/project/agentscope/)
 [![](https://img.shields.io/badge/Docs-English%7C%E4%B8%AD%E6%96%87-blue?logo=markdown)](https://modelscope.github.io/agentscope/#welcome-to-agentscope-tutorial-hub)
 [![](https://img.shields.io/badge/Docs-API_Reference-blue?logo=markdown)](https://modelscope.github.io/agentscope/)
 [![](https://img.shields.io/badge/ModelScope-Demos-4e29ff.svg?logo=data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjI0IDEyMS4zMyIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxwYXRoIGQ9Im0wIDQ3Ljg0aDI1LjY1djI1LjY1aC0yNS42NXoiIGZpbGw9IiM2MjRhZmYiIC8+Cgk8cGF0aCBkPSJtOTkuMTQgNzMuNDloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzYyNGFmZiIgLz4KCTxwYXRoIGQ9Im0xNzYuMDkgOTkuMTRoLTI1LjY1djIyLjE5aDQ3Ljg0di00Ny44NGgtMjIuMTl6IiBmaWxsPSIjNjI0YWZmIiAvPgoJPHBhdGggZD0ibTEyNC43OSA0Ny44NGgyNS42NXYyNS42NWgtMjUuNjV6IiBmaWxsPSIjMzZjZmQxIiAvPgoJPHBhdGggZD0ibTAgMjIuMTloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzM2Y2ZkMSIgLz4KCTxwYXRoIGQ9Im0xOTguMjggNDcuODRoMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzYyNGFmZiIgLz4KCTxwYXRoIGQ9Im0xOTguMjggMjIuMTloMjUuNjV2MjUuNjVoLTI1LjY1eiIgZmlsbD0iIzM2Y2ZkMSIgLz4KCTxwYXRoIGQ9Im0xNTAuNDQgMHYyMi4xOWgyNS42NXYyNS42NWgyMi4xOXYtNDcuODR6IiBmaWxsPSIjNjI0YWZmIiAvPgoJPHBhdGggZD0ibTczLjQ5IDQ3Ljg0aDI1LjY1djI1LjY1aC0yNS42NXoiIGZpbGw9IiMzNmNmZDEiIC8+Cgk8cGF0aCBkPSJtNDcuODQgMjIuMTloMjUuNjV2LTIyLjE5aC00Ny44NHY0Ny44NGgyMi4xOXoiIGZpbGw9IiM2MjRhZmYiIC8+Cgk8cGF0aCBkPSJtNDcuODQgNzMuNDloLTIyLjE5djQ3Ljg0aDQ3Ljg0di0yMi4xOWgtMjUuNjV6IiBmaWxsPSIjNjI0YWZmIiAvPgo8L3N2Zz4K)](https://modelscope.cn/studios?name=agentscope&page=1&sort=latest)
 
 [![](https://img.shields.io/badge/license-Apache--2.0-black)](./LICENSE)
 [![](https://img.shields.io/badge/Contribute-Welcome-green)](https://modelscope.github.io/agentscope/tutorial/contribute.html)
 
@@ -134,65 +139,73 @@
 |----------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
 | <img src="https://gw.alicdn.com/imgextra/i1/O1CN01hhD1mu1Dd3BWVUvxN_!!6000000000238-2-tps-400-400.png" width="100" height="100"> | <img src="https://img.alicdn.com/imgextra/i2/O1CN01tuJ5971OmAqNg9cOw_!!6000000001747-0-tps-444-460.jpg" width="100" height="100"> |
 
 ----
 
 ## News
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] We release **AgentScope** v0.0.2 now! In this new version,
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-30]** We release **AgentScope** v0.0.4 now!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-27]** [AgentScope Workstation](https://agentscope.aliyun.com/) is now online! You are welcome to try building your multi-agent application simply with our *drag-and-drop platform* and ask our *copilot* questions about AgentScope!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-19]** AgentScope supports Llama3 now! We provide [scripts](./examples/model_llama3) and example [model configuration](./examples/model_llama3) for quick set-up. Feel free to try llama3 in our examples!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-06]** We release **AgentScope** v0.0.3 now!
+
+- <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>**[2024-04-06]** New examples [Gomoku](./examples/game_gomoku), [Conversation with ReAct Agent](./examples/conversation_with_react_agent), [Conversation with RAG Agent](./examples/conversation_with_RAG_agents) and [Distributed Parallel Search](./examples/distributed_search) are available now!
+
+- **[2024-03-19]** We release **AgentScope** v0.0.2 now! In this new version,
 AgentScope supports [ollama](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models)(A local CPU inference engine), [DashScope](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models) and Google [Gemini](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#supported-models) APIs.
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] New examples ["Autonomous Conversation with Mentions"](./examples/conversation_with_mentions) and ["Basic Conversation with LangChain library"](./examples/conversation_with_langchain) are available now!
+- **[2024-03-19]** New examples ["Autonomous Conversation with Mentions"](./examples/conversation_with_mentions) and ["Basic Conversation with LangChain library"](./examples/conversation_with_langchain) are available now!
 
-- ![new](https://img.alicdn.com/imgextra/i4/O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png)
-[2024-03-19] The [Chinese tutorial](https://modelscope.github.io/agentscope/zh_CN/index.html) of AgentScope is online now!
+- **[2024-03-19]** The [Chinese tutorial](https://modelscope.github.io/agentscope/zh_CN/index.html) of AgentScope is online now!
 
-- [2024-02-27] We release **AgentScope v0.0.1** now, which is also
+- **[2024-02-27]** We release **AgentScope v0.0.1** now, which is also
 available in [PyPI](https://pypi.org/project/agentscope/)!
-- [2024-02-14] We release our paper "AgentScope: A Flexible yet Robust
+- **[2024-02-14]** We release our paper "AgentScope: A Flexible yet Robust
 Multi-Agent Platform" in [arXiv](https://arxiv.org/abs/2402.14034) now!
 
 ---
 
 ## What's AgentScope?
 
 AgentScope is an innovative multi-agent platform designed to empower developers
 to build multi-agent applications with large-scale models.
 It features three high-level capabilities:
 
 - 🤝 **Easy-to-Use**: Designed for developers, with [fruitful components](https://modelscope.github.io/agentscope/en/tutorial/204-service.html#),
-[comprehensive documentation](https://modelscope.github.io/agentscope/en/index.html), and broad compatibility.
+[comprehensive documentation](https://modelscope.github.io/agentscope/en/index.html), and broad compatibility. Besides, [AgentScope Workstation](https://agentscope.aliyun.com/) provides a *drag-and-drop programming platform* and a *copilot* for beginners of AgentScope!
 
 - ✅ **High Robustness**: Supporting customized fault-tolerance controls and
 retry mechanisms to enhance application stability.
 
 - 🚀 **Actor-Based Distribution**: Building distributed multi-agent
 applications in a centralized programming manner for streamlined development.
 
 **Supported Model Libraries**
 
 AgentScope provides a list of `ModelWrapper` to support both local model
 services and third-party model APIs.
 
-| API                    | Task            | Model Wrapper                                                                                                                   | Example Configuration                                                                       |
-|------------------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
-| OpenAI API             | Chat            | [`OpenAIChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-|                        | Embedding       | [`OpenAIEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-|                        | DALL·E          | [`OpenAIDALLEWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)       |
-| DashScope API          | Chat            | [`DashScopeChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)           | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-|                        | Image Synthesis | [`DashScopeImageSynthesisWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py) | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-|                        | Text Embedding  | [`DashScopeTextEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)  | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)    |
-| Gemini API             | Chat            | [`GeminiChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api)       |
-|                        | Embedding       | [`GeminiEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api)       |
-| ollama                 | Chat            | [`OllamaChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-|                        | Embedding       | [`OllamaEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)            | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-|                        | Generation      | [`OllamaGenerationWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)           | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api)       |
-| Post Request based API | -               | [`PostAPIModelWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/post_model.py)                 | [link](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#post-request-api) |
+| API                    | Task            | Model Wrapper                                                                                                                   | Configuration                                                                      | Some Supported Models                         |
+|------------------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|-----------------------------------------------|
+| OpenAI API             | Chat            | [`OpenAIChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                 |[guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api)  <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_chat_template.json)       | gpt-4, gpt-3.5-turbo, ...                     |
+|                        | Embedding       | [`OpenAIEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_embedding_template.json)       | text-embedding-ada-002, ...                   |
+|                        | DALL·E          | [`OpenAIDALLEWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/openai_model.py)                | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#openai-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/openai_dall_e_template.json)       | dall-e-2, dall-e-3                            |
+| DashScope API          | Chat            | [`DashScopeChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)           | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_chat_template.json)    | qwen-plus, qwen-max, ...                      |
+|                        | Image Synthesis | [`DashScopeImageSynthesisWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py) | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api)  <br>[template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_image_synthesis_template.json)    | wanx-v1                                       |
+|                        | Text Embedding  | [`DashScopeTextEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)  | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_text_embedding_template.json)    | text-embedding-v1, text-embedding-v2, ...     |
+|                        | Multimodal      | [`DashScopeMultiModalWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/dashscope_model.py)     | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#dashscope-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/dashscope_multimodal_template.json)    | qwen-vl-max, qwen-vl-chat-v1, qwen-audio-chat |
+| Gemini API             | Chat            | [`GeminiChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/gemini_chat_template.json)       | gemini-pro, ...                               |
+|                        | Embedding       | [`GeminiEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/gemini_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#gemini-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/gemini_embedding_template.json)       | models/embedding-001, ...                     |
+| ollama                 | Chat            | [`OllamaChatWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_chat_template.json)       | llama3, llama2, Mistral, ...                  |
+|                        | Embedding       | [`OllamaEmbeddingWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)            | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_embedding_template.json)       | llama2, Mistral, ...                          |
+|                        | Generation      | [`OllamaGenerationWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/ollama_model.py)           | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#ollama-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/ollama_generate_template.json)       | llama2, Mistral, ...                          |
+| Post Request based API | -               | [`PostAPIModelWrapper`](https://github.com/modelscope/agentscope/blob/main/src/agentscope/models/post_model.py)                 | [guidance](https://modelscope.github.io/agentscope/en/tutorial/203-model.html#post-request-api) <br> [template](https://github.com/modelscope/agentscope/blob/main/examples/model_configs_template/postapi_model_config_template.json) | -                                             |
 
 **Supported Local Model Deployment**
 
 AgentScope enables developers to rapidly deploy local model services using
 the following libraries.
 
 - [ollama (CPU inference)](https://github.com/modelscope/agentscope/blob/main/scripts/README.md#ollama)
@@ -208,14 +221,17 @@
 - Retrieval
 - Code Execution
 - File Operation
 - Text Processing
 
 **Example Applications**
 
+- Model
+  - <img src="https://img.alicdn.com/imgextra/i3/O1CN01SFL0Gu26nrQBFKXFR_!!6000000007707-2-tps-500-500.png" alt="new" width="30" height="30"/>[Using Llama3 in AgentScope](./examples/model_llama3)
+
 - Conversation
   - [Basic Conversation](./examples/conversation_basic)
   - [Autonomous Conversation with Mentions](./examples/conversation_with_mentions)
   - [Self-Organizing Conversation](./examples/conversation_self_organizing)
   - [Basic Conversation with LangChain library](./examples/conversation_with_langchain)
   - [Conversation with ReAct Agent](./examples/conversation_with_react_agent)
   - [Conversation with RAG Agent](./examples/conversation_with_RAG_agents)
@@ -224,23 +240,24 @@
   - [Gomoku](./examples/game_gomoku)
   - [Werewolf](./examples/game_werewolf)
 
 - Distribution
   - [Distributed Conversation](./examples/distributed_basic)
   - [Distributed Debate](./examples/distributed_debate)
   - [Distributed Parallel Search](./examples/distributed_search)
+  - [Distributed Large Scale Simulation](./examples/distributed_simulation)
 
 More models, services and examples are coming soon!
 
 ## Installation
 
 AgentScope requires **Python 3.9** or higher.
 
-**_Note: This project is currently in active development, it's recommended to
-install AgentScope from source._**
+***Note: This project is currently in active development, it's recommended to
+install AgentScope from source.***
 
 ### From source
 
 - Install AgentScope in editable mode:
 
 ```bash
 # Pull the source code from GitHub
@@ -290,15 +307,15 @@
 ```
 
 Taking OpenAI Chat API as an example, the model configuration is as follows:
 
 ```python
 openai_model_config = {
     "config_name": "my_openai_config",             # The name to identify the config
-    "model_type": "openai",                        # The type to identify the model wrapper
+    "model_type": "openai_chat",                   # The type to identify the model wrapper
 
     # Detailed parameters into initialize the model wrapper
     "model_name": "gpt-4",                         # The used model in openai API, e.g. gpt-4, gpt-3.5-turbo, etc.
     "api_key": "xxx",                              # The API key for OpenAI API. If not set, env
                                                    # variable OPENAI_API_KEY will be used.
     "organization": "xxx",                         # The organization for OpenAI API. If not set, env
                                                    # variable OPENAI_ORGANIZATION will be used.
```

### Comparing `agentscope-0.0.3/src/agentscope.egg-info/SOURCES.txt` & `agentscope-0.0.4/src/agentscope.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 src/agentscope/__init__.py
 src/agentscope/_init.py
 src/agentscope/_runtime.py
 src/agentscope/_version.py
 src/agentscope/constants.py
+src/agentscope/exception.py
 src/agentscope/file_manager.py
 src/agentscope/message.py
 src/agentscope/msghub.py
 src/agentscope/prompt.py
 src/agentscope.egg-info/PKG-INFO
 src/agentscope.egg-info/SOURCES.txt
 src/agentscope.egg-info/dependency_links.txt
@@ -34,43 +35,51 @@
 src/agentscope/models/dashscope_model.py
 src/agentscope/models/gemini_model.py
 src/agentscope/models/model.py
 src/agentscope/models/ollama_model.py
 src/agentscope/models/openai_model.py
 src/agentscope/models/post_model.py
 src/agentscope/models/response.py
+src/agentscope/parsers/__init__.py
+src/agentscope/parsers/code_block_parser.py
+src/agentscope/parsers/json_object_parser.py
+src/agentscope/parsers/parser_base.py
+src/agentscope/parsers/tagged_content_parser.py
 src/agentscope/pipelines/__init__.py
 src/agentscope/pipelines/functional.py
 src/agentscope/pipelines/pipeline.py
 src/agentscope/rpc/__init__.py
 src/agentscope/rpc/rpc_agent_client.py
 src/agentscope/rpc/rpc_agent_pb2.py
 src/agentscope/rpc/rpc_agent_pb2_grpc.py
 src/agentscope/service/__init__.py
-src/agentscope/service/service_factory.py
 src/agentscope/service/service_response.py
 src/agentscope/service/service_status.py
+src/agentscope/service/service_toolkit.py
 src/agentscope/service/execute_code/__init__.py
 src/agentscope/service/execute_code/exec_python.py
+src/agentscope/service/execute_code/exec_shell.py
 src/agentscope/service/file/__init__.py
 src/agentscope/service/file/common.py
 src/agentscope/service/file/json.py
 src/agentscope/service/file/text.py
 src/agentscope/service/retrieval/__init__.py
 src/agentscope/service/retrieval/retrieval_from_list.py
 src/agentscope/service/retrieval/similarity.py
 src/agentscope/service/sql_query/__init__.py
 src/agentscope/service/sql_query/mongodb.py
 src/agentscope/service/sql_query/mysql.py
 src/agentscope/service/sql_query/sqlite.py
 src/agentscope/service/text_processing/__init__.py
 src/agentscope/service/text_processing/summarization.py
-src/agentscope/service/web_search/__init__.py
-src/agentscope/service/web_search/search.py
-src/agentscope/service/web_search/web_digest.py
+src/agentscope/service/web/__init__.py
+src/agentscope/service/web/arxiv.py
+src/agentscope/service/web/download.py
+src/agentscope/service/web/search.py
+src/agentscope/service/web/web_digest.py
 src/agentscope/utils/__init__.py
 src/agentscope/utils/common.py
 src/agentscope/utils/logging_utils.py
 src/agentscope/utils/monitor.py
 src/agentscope/utils/token_utils.py
 src/agentscope/utils/tools.py
 src/agentscope/web/__init__.py
@@ -89,9 +98,15 @@
 src/agentscope/web/static/js/bootstrap-table.min.js
 src/agentscope/web/static/js/bootstrap.bundle.min.js
 src/agentscope/web/static/js/home.js
 src/agentscope/web/static/js/jquery-3.3.1.min.js
 src/agentscope/web/static/js/run.js
 src/agentscope/web/static/js/socket.io.js
 src/agentscope/web/studio/__init__.py
+src/agentscope/web/studio/constants.py
 src/agentscope/web/studio/studio.py
-src/agentscope/web/studio/utils.py
+src/agentscope/web/studio/utils.py
+src/agentscope/web/workstation/__init__.py
+src/agentscope/web/workstation/workflow.py
+src/agentscope/web/workstation/workflow_dag.py
+src/agentscope/web/workstation/workflow_node.py
+src/agentscope/web/workstation/workflow_utils.py
```

### Comparing `agentscope-0.0.3/src/agentscope.egg-info/requires.txt` & `agentscope-0.0.4/src/agentscope.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 dashscope==1.14.1
 ollama>=0.1.7
 google-generativeai>=0.4.0
 grpcio==1.60.0
 grpcio-tools==1.60.0
 protobuf==4.25.0
 expiringdict
+dill
 
 [full]
 docstring_parser
 loguru==0.6.0
 tiktoken
 Pillow
 requests
@@ -72,21 +73,25 @@
 dashscope==1.14.1
 ollama>=0.1.7
 google-generativeai>=0.4.0
 grpcio==1.60.0
 grpcio-tools==1.60.0
 protobuf==4.25.0
 expiringdict
+dill
 docker
 pymongo
 pymysql
 beautifulsoup4
+feedparser
 sphinx
 sphinx-autobuild
 sphinx_rtd_theme
 myst-parser
 sphinxcontrib-mermaid
 pytest
 pytest-cov
 pre-commit
+networkx
 gradio==4.19.1
 modelscope_studio==0.0.5
+black
```

