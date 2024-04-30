# Comparing `tmp/lionagi-0.1.1.tar.gz` & `tmp/lionagi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lionagi-0.1.1.tar", last modified: Sun Apr 21 00:58:00 2024, max compression
+gzip compressed data, was "lionagi-0.1.2.tar", last modified: Tue Apr 30 11:58:02 2024, max compression
```

## Comparing `lionagi-0.1.1.tar` & `lionagi-0.1.2.tar`

### file list

```diff
@@ -1,243 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.141428 lionagi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 00:57:39.000000 lionagi-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-21 00:58:00.141428 lionagi-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-21 00:57:39.000000 lionagi-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-21 00:57:39.000000 lionagi-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.113428 lionagi-0.1.1/lionagi/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.113428 lionagi-0.1.1/lionagi/core/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.113428 lionagi-0.1.1/lionagi/core/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/agent/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.113428 lionagi-0.1.1/lionagi/core/branch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18010 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/executable_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/flow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/direct/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/cot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/react.py
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/select.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/sentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/vote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/execute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/base_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/branch_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/instruction_map_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/neo4j_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/structure_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/flow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/baseflow.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/mono_chat_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/flow/monoflow/
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/ReAct.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/chat_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/followup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/flow/polyflow/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/polyflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/polyflow/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/form/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/action_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/field_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/scored_form.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/mail/mail_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/mail/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/messages/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/core/session/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38111 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/core/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/tool/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/tool/tool_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/directive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/directive/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/ast_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/base_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/sandbox_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/script_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/directive/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/directive/template_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/template_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/template_/base_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/function_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/tool_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/experimental/work/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/work_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/autogen_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/autogen_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/autogen_/autogen_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/langchain_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/langchain_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/langchain_/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/langchain_/langchain_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/get_index.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/llama_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/node_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/textnode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/pydantic_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/pydantic_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/pydantic_/pydantic_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/transformers_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/transformers_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/transformers_/install_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/chunker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/chunker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/chunker/chunk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.133428 lionagi-0.1.1/lionagi/integrations/config/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/mlx_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/oai_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/ollama_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/openrouter_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.133428 lionagi-0.1.1/lionagi/integrations/loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/loader/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/loader/load_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.133428 lionagi-0.1.1/lionagi/integrations/provider/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/litellm.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/mistralai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/mlx_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/oai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.133428 lionagi-0.1.1/lionagi/integrations/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25785 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/storage_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/to_excel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34577 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    23535 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    49096 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_func_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_knowledge_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    25007 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17353 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/sys_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/lions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/lions/coder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/add_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/base_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/coder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/lions/researcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/lions/researcher/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/finhub_.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/google_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/wiki_.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/yfinance_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/tests/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.141428 lionagi-0.1.1/lionagi/tests/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    20782 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_func_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_sys_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.141428 lionagi-0.1.1/lionagi/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_base_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_chat_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_mail_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_session_base_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_tool_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.141428 lionagi-0.1.1/lionagi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-21 00:57:39.000000 lionagi-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 00:58:00.141428 lionagi-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-21 00:57:39.000000 lionagi-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.500678 lionagi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 11:57:47.000000 lionagi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-30 11:58:02.500678 lionagi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-30 11:57:47.000000 lionagi-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 11:57:47.000000 lionagi-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.460678 lionagi-0.1.2/lionagi/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.460678 lionagi-0.1.2/lionagi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.464678 lionagi-0.1.2/lionagi/core/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/agent/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.464678 lionagi-0.1.2/lionagi/core/branch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18010 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/executable_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/flow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.464678 lionagi-0.1.2/lionagi/core/direct/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/cot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/react.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/vote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/execute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/base_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/branch_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/instruction_map_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/neo4j_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/structure_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/baseflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/mono_chat_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/flow/monoflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/ReAct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/chat_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/followup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/flow/polyflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/polyflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/polyflow/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/form/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/action_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/scored_form.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/mail/mail_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/mail/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/messages/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/session/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38111 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/tool/tool_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/directive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/directive/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/ast_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/sandbox_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/script_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/directive/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/directive/template_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/template_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/template_/base_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/report/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/report/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/function_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/tool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/experimental/validator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/validator/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/experimental/work/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/async_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/work_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/experimental/work2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/work.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/work_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/integrations/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/integrations/bridge/autogen_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/autogen_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/autogen_/autogen_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/integrations/bridge/langchain_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/langchain_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/langchain_/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/langchain_/langchain_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/get_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/llama_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/node_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/textnode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/bridge/pydantic_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/pydantic_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/pydantic_/pydantic_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/bridge/transformers_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/transformers_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/transformers_/install_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/chunker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/chunker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/chunker/chunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/mlx_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/oai_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/ollama_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/openrouter_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/loader/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/loader/load_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.488678 lionagi-0.1.2/lionagi/integrations/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/litellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/mistralai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/mlx_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/oai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.488678 lionagi-0.1.2/lionagi/integrations/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25785 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/storage_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/structure_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34577 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23535 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49096 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_func_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_knowledge_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25007 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17353 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/sys_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/lions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/lions/coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/add_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/lions/researcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/lions/researcher/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/finhub_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/google_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/wiki_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/yfinance_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.496678 lionagi-0.1.2/lionagi/tests/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.496678 lionagi-0.1.2/lionagi/tests/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20782 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_func_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_sys_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.496678 lionagi-0.1.2/lionagi/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.500678 lionagi-0.1.2/lionagi/tests/test_core/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/generic/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_base_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_chat_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_mail_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_session_base_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_tool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.500678 lionagi-0.1.2/lionagi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 11:57:47.000000 lionagi-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:58:02.500678 lionagi-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-30 11:57:47.000000 lionagi-0.1.2/setup.py
```

### Comparing `lionagi-0.1.1/LICENSE` & `lionagi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/PKG-INFO` & `lionagi-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lionagi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Towards automated general intelligence.
 Author: HaiyangLi
 Author-email: Haiyang Li <ocean@lionagi.ai>
 License: MIT License
         
         Copyright (c) 2023 HaiyangLi quantocean.li@gmail.com
```

### Comparing `lionagi-0.1.1/README.md` & `lionagi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/agent/base_agent.py` & `lionagi-0.1.2/lionagi/core/agent/base_agent.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/branch/base.py` & `lionagi-0.1.2/lionagi/core/branch/base.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/branch/branch.py` & `lionagi-0.1.2/lionagi/core/branch/branch.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/branch/flow_mixin.py` & `lionagi-0.1.2/lionagi/core/branch/flow_mixin.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/branch/util.py` & `lionagi-0.1.2/lionagi/core/branch/util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/direct/cot.py` & `lionagi-0.1.2/lionagi/core/direct/cot.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/direct/plan.py` & `lionagi-0.1.2/lionagi/core/direct/plan.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/direct/predict.py` & `lionagi-0.1.2/lionagi/core/direct/predict.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/direct/react.py` & `lionagi-0.1.2/lionagi/core/direct/react.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/direct/score.py` & `lionagi-0.1.2/lionagi/core/direct/score.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/direct/select.py` & `lionagi-0.1.2/lionagi/core/direct/select.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/direct/utils.py` & `lionagi-0.1.2/lionagi/core/direct/utils.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/direct/vote.py` & `lionagi-0.1.2/lionagi/core/direct/vote.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/execute/base_executor.py` & `lionagi-0.1.2/lionagi/core/execute/base_executor.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/execute/branch_executor.py` & `lionagi-0.1.2/lionagi/core/execute/branch_executor.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/execute/instruction_map_executor.py` & `lionagi-0.1.2/lionagi/core/execute/instruction_map_executor.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/execute/neo4j_executor.py` & `lionagi-0.1.2/lionagi/core/execute/neo4j_executor.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/execute/structure_executor.py` & `lionagi-0.1.2/lionagi/core/execute/structure_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         """
         Process the pending incoming mails and perform the corresponding actions.
         """
         for key in list(self.pending_ins.keys()):
             while self.pending_ins[key]:
                 mail: BaseMail = self.pending_ins[key].popleft()
                 try:
-                    if mail == "end":
+                    if mail.category == "end":
                         self.execute_stop = True
                         return
                     next_nodes = await self._handle_mail(mail)
                     self._send_mail(next_nodes, mail)
                 except Exception as e:
                     raise ValueError(f"Error handling mail: {e}") from e
 
@@ -308,7 +308,27 @@
         """
         if not self.acyclic:
             raise ValueError("Structure is not acyclic")
 
         while not self.execute_stop:
             await self.forward()
             await AsyncUtil.sleep(refresh_time)
+
+    def to_excel(self, structure_name, dir="structure_storage"):
+        """
+        Exports the current structure to an Excel file using a specified structure name and directory.
+
+        This method utilizes the `to_excel` function from the `lionagi.integrations.storage.to_excel` module,
+        saving the current structure instance into an Excel file format. The Excel file will contain details
+        about nodes, edges, and other relevant data as separate sheets within the file.
+
+        Args:
+            structure_name (str): The name to assign to the structure within the Excel file. This name is
+                                  used as part of the file naming convention.
+            dir (str, optional): The directory where the Excel file will be saved. Defaults to "structure_storage".
+
+        Raises:
+            Exception: Propagates any exceptions raised by the `to_excel` function, which might occur during
+                       the file writing process or data formatting.
+        """
+        from lionagi.integrations.storage.to_excel import to_excel
+        to_excel(self, structure_name, dir)
```

### Comparing `lionagi-0.1.1/lionagi/core/flow/monoflow/ReAct.py` & `lionagi-0.1.2/lionagi/core/flow/monoflow/ReAct.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,17 @@
         """
         if tools and isinstance(tools, list) and isinstance(tools[0], (Callable, Tool)):
             self.branch.tool_manager.register_tools(tools)
 
         if not self.branch.tool_manager.has_tools:
             raise ValueError("No tools found. You need to register tools.")
 
-        config = self.branch.tool_manager.parse_tool(tools=True, **kwargs)
+        if tools is None:
+            tools = True
+        config = self.branch.tool_manager.parse_tool(tools=tools, **kwargs)
         config["tool_parsed"] = True
         config["tool_choice"] = tool_choice
         return config
 
     async def _ReAct(
         self,
         instruction: Instruction | str | dict[str, dict | str],
```

### Comparing `lionagi-0.1.1/lionagi/core/flow/monoflow/chat.py` & `lionagi-0.1.2/lionagi/core/flow/monoflow/chat.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/flow/monoflow/chat_mixin.py` & `lionagi-0.1.2/lionagi/core/flow/monoflow/chat_mixin.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/flow/monoflow/followup.py` & `lionagi-0.1.2/lionagi/core/flow/monoflow/followup.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,17 @@
         """
         if tools and isinstance(tools, list) and isinstance(tools[0], (Callable, Tool)):
             self.branch.tool_manager.register_tools(tools)
 
         if not self.branch.tool_manager.has_tools:
             raise ValueError("No tools found. You need to register tools.")
 
-        config = self.branch.tool_manager.parse_tool(tools=True, **kwargs)
+        if tools is None:
+            tools = True
+        config = self.branch.tool_manager.parse_tool(tools=tools, **kwargs)
         config["tool_parsed"] = True
         config["tool_choice"] = tool_choice
         return config
 
     async def _followup(
         self,
         instruction: Instruction | str | dict[str, dict | str],
```

### Comparing `lionagi-0.1.1/lionagi/core/flow/polyflow/chat.py` & `lionagi-0.1.2/lionagi/core/flow/polyflow/chat.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/form/action_form.py` & `lionagi-0.1.2/lionagi/core/form/action_form.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/form/field_validator.py` & `lionagi-0.1.2/lionagi/core/form/field_validator.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/form/form.py` & `lionagi-0.1.2/lionagi/core/form/form.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/form/mixin.py` & `lionagi-0.1.2/lionagi/core/form/mixin.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/__init__.py` & `lionagi-0.1.2/lionagi/core/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/action.py` & `lionagi-0.1.2/lionagi/core/generic/action.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/component.py` & `lionagi-0.1.2/lionagi/core/generic/component.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""This module provides base components used in lionagi"""
+"""base components in lionagi"""
 
 from abc import ABC
 from functools import singledispatchmethod
-from typing import Any, TypeVar
-
+from typing import Any, TypeVar, Type
 from pydantic import AliasChoices, BaseModel, Field, ValidationError
 from pandas import DataFrame, Series
 
-from lionagi.libs import SysUtil, func_call, convert, ParseUtil, nested
+from lionagi.libs import SysUtil, convert, ParseUtil, nested, func_call
 
 
 T = TypeVar("T")
 
 
 class BaseComponent(BaseModel, ABC):
     """
@@ -24,231 +23,273 @@
 
     id_: str = Field(
         title="ID",
         default_factory=SysUtil.create_id,
         validation_alias=AliasChoices("node_id", "ID", "id"),
         description="A 32-char unique hash identifier for the node.",
     )
-
     timestamp: str = Field(
         default_factory=lambda: SysUtil.get_timestamp(sep=None),
         description="The timestamp of when the node was created.",
     )
 
+    extra_fields: dict[str, Any] = Field(
+        default_factory=dict,
+        validation_alias=AliasChoices(
+            "extra", "additional_fields", "schema_extra", "extra_schema"
+        ),
+        description="Additional fields for the component.",
+    )
+
     class Config:
         """Model configuration settings."""
 
         extra = "allow"
         arbitrary_types_allowed = True
         populate_by_name = True
-        validate_assignment = True
-        validate_return = True
-        str_strip_whitespace = True
+
+    @property
+    def class_name(self) -> str:
+        """
+        Retrieve the name of the class.
+
+        Returns:
+            str: The name of the class.
+        """
+        return self._class_name()
 
     @classmethod
-    def class_name(cls) -> str:
+    def _class_name(cls) -> str:
         """
         Retrieve the name of the class.
 
         Returns:
             str: The name of the class.
         """
         return cls.__name__
 
+    def to_json_str(self, *args, **kwargs) -> str:
+        """
+        Convert the component to a JSON string.
+
+        Returns:
+            str: The JSON string representation of the component.
+        """
+        dict_ = self.to_dict(*args, **kwargs)
+        return convert.to_str(dict_)
+
+    def to_dict(self, *args, **kwargs) -> dict[str, Any]:
+        """
+        Convert the component to a dictionary.
+
+        Returns:
+            dict[str, Any]: The dictionary representation of the component.
+        """
+        dict_ = self.model_dump(*args, by_alias=True, **kwargs)
+        for field_name in list(self.extra_fields.keys()):
+            if field_name not in dict_:
+                dict_[field_name] = getattr(self, field_name, None)
+        dict_.pop("extra_fields", None)
+        return dict_
+
+    def to_xml(self, *args, **kwargs) -> str:
+        """
+        Convert the component to an XML string.
+
+        Returns:
+            str: The XML string representation of the component.
+        """
+        import xml.etree.ElementTree as ET
+
+        root = ET.Element(self.__class__.__name__)
+
+        def convert(dict_obj: dict, parent: ET.Element) -> None:
+            for key, val in dict_obj.items():
+                if isinstance(val, dict):
+                    element = ET.SubElement(parent, key)
+                    convert(val, element)
+                else:
+                    element = ET.SubElement(parent, key)
+                    element.text = str(val)
+
+        convert(self.to_dict(*args, **kwargs), root)
+        return ET.tostring(root, encoding="unicode")
+
+    def to_pd_series(self, *args, pd_kwargs: dict | None = None, **kwargs) -> Series:
+        """
+        Convert the node to a Pandas Series.
+
+        Args:
+            pd_kwargs (dict | None): Additional keyword arguments for Pandas Series.
+
+        Returns:
+            Series: The Pandas Series representation of the node.
+        """
+        pd_kwargs = {} if pd_kwargs is None else pd_kwargs
+        dict_ = self.to_dict(*args, **kwargs)
+        return Series(dict_, **pd_kwargs)
+
+    def _add_field(
+        self,
+        field_name: str,
+        annotation: Any | Type | None = Any,
+        default: Any | None = None,
+        value: Any | None = None,
+        field: Any = None,
+        **kwargs,
+    ) -> None:
+        """
+        Add a field to the model after initialization.
+
+        Args:
+            field_name (str): The name of the field.
+            annotation (Any | Type | None): The type annotation for the field.
+            default (Any | None): The default value for the field.
+            value (Any | None): The initial value for the field.
+            field (Any): The Field object for the field.
+            **kwargs: Additional keyword arguments for the Field object.
+        """
+        field = field or Field(default=default, **kwargs)
+        self.extra_fields[field_name] = field
+        if annotation:
+            self.extra_fields[field_name].annotation = annotation
+
+        if not value and (a := self._get_field_attr(field_name, "default", None)):
+            value = a
+
+        self.__setattr__(field_name, value)
+
+    @property
+    def _all_fields(self):
+        return {**self.model_fields, **self.extra_fields}
+
     @property
     def _field_annotations(self) -> dict:
         """
         Return the annotations for each field in the model.
 
         Returns:
             dict: A dictionary mapping field names to their annotations.
         """
-        return self._get_field_annotation(list(self.model_fields.keys()))
 
-    def _get_field_attr(self, k: str, attr: str, default=False) -> Any:
+        return self._get_field_annotation(list(self._all_fields.keys()))
+
+    def _get_field_attr(self, k: str, attr: str, default: Any = False) -> Any:
         """
         Get the value of a field attribute.
 
         Args:
             k (str): The field name.
             attr (str): The attribute name.
-            default (Any): Default value to return if the attribute is not
-                found.
+            default (Any): Default value to return if the attribute is not found.
 
         Returns:
-            Any: The value of the field attribute, or the default value if not
-                found.
+            Any: The value of the field attribute, or the default value if not found.
 
         Raises:
             ValueError: If the field does not have the specified attribute.
         """
         try:
             if not self._field_has_attr(k, attr):
                 raise ValueError(f"field {k} has no attribute {attr}")
-            field = self.model_fields[k]
-            a = getattr(field, attr)
+
+            field = self._all_fields[k]
+            a = getattr(field, attr, None)
             if not a:
                 try:
                     a = field.json_schema_extra[attr]
                     return a
                 except Exception:
                     return None
             return a
         except Exception as e:
             if default is not False:
                 return default
             raise e
 
     @singledispatchmethod
-    def _get_field_annotation(self, field_name: str) -> Any:
+    def _get_field_annotation(self, field_name: Any) -> Any:
         """
         Get the annotation for a field.
 
         Args:
             field_name (str): The name of the field.
 
         Raises:
             TypeError: If the field_name is of an unsupported type.
         """
         raise TypeError(f"Unsupported type {type(field_name)}")
 
     @_get_field_annotation.register(str)
-    def _(self, field_name) -> dict[str, Any]:
+    def _(self, field_name: str) -> dict[str, Any]:
         """
         Get the annotation for a field as a dictionary.
 
         Args:
             field_name (str): The name of the field.
 
         Returns:
-            dict[str, Any]: A dictionary mapping the field name to its
-                annotation.
+            dict[str, Any]: A dictionary mapping the field name to its annotation.
         """
-        dict_ = {field_name: self.model_fields[field_name].annotation}
+        dict_ = {field_name: self._all_fields[field_name].annotation}
         for k, v in dict_.items():
             if "|" in str(v):
                 v = str(v)
                 v = v.split("|")
                 dict_[k] = func_call.lcall(v, convert.strip_lower)
             else:
                 dict_[k] = [v.__name__]
         return dict_
 
     @_get_field_annotation.register(list)
-    def _(self, field_name) -> dict[str, Any]:
-        """
-        Get the annotations for multiple fields as a dictionary.
-
-        Args:
-            field_name (list): A list or tuple of field names.
-
-        Returns:
-            dict[str, Any]: A dictionary mapping field names to their
-                annotations.
-        """
-        dict_ = {}
-        for i in field_name:
-            dict_.update(self._get_field_annotation(i))
-        return dict_
-
     @_get_field_annotation.register(tuple)
-    def _(self, field_name) -> dict[str, Any]:
+    def _(self, field_names: list | tuple) -> dict[str, Any]:
         """
         Get the annotations for multiple fields as a dictionary.
 
         Args:
-            field_name (tuple): A list or tuple of field names.
+            field_names (list | tuple): A list or tuple of field names.
 
         Returns:
-            dict[str, Any]: A dictionary mapping field names to their
-                annotations.
+            dict[str, Any]: A dictionary mapping field names to their annotations.
         """
         dict_ = {}
-        for i in field_name:
-            dict_.update(self._get_field_annotation(i))
+        for field_name in field_names:
+            dict_.update(self._get_field_annotation(field_name))
         return dict_
 
     def _field_has_attr(self, k: str, attr: str) -> bool:
         """
         Check if a field has a specific attribute.
 
         Args:
             k (str): The field name.
             attr (str): The attribute name.
 
         Returns:
             bool: True if the field has the attribute, False otherwise.
         """
-        field = self.model_fields.get(k, None)
+        field = self._all_fields.get(k, None)
         if field is None:
             raise ValueError(f"Field {k} not found in model fields.")
 
         a = attr in str(field)
         if not a:
             try:
                 a = (
-                    self.model_fields[k].json_schema_extra[attr] is not None
-                    and attr in self.model_fields[k].json_schema_extra
+                    self._all_fields[k].json_schema_extra[attr] is not None
+                    and attr in self._all_fields[k].json_schema_extra
                 )
                 return a if isinstance(a, bool) else False
             except Exception:
                 return False
         return a
 
-    def to_json_str(self, *args, **kwargs) -> str:
-        """
-        Convert the component to a JSON string.
-
-        Returns:
-            str: The JSON string representation of the component.
-        """
-        return self.model_dump_json(*args, by_alias=True, **kwargs)
-
-    def to_dict(self, *args, **kwargs) -> dict[str, Any]:
-        """
-        Convert the component to a dictionary.
-
-        Returns:
-            dict[str, Any]: The dictionary representation of the component.
-        """
-        return self.model_dump(*args, by_alias=True, **kwargs)
-
-    def to_xml(self) -> str:
-        """
-        Convert the component to an XML string.
-
-        Returns:
-            str: The XML string representation of the component.
-        """
-        import xml.etree.ElementTree as ET
-
-        root = ET.Element(self.__class__.__name__)
-
-        def convert(dict_obj, parent):
-            for key, val in dict_obj.items():
-                if isinstance(val, dict):
-                    element = ET.SubElement(parent, key)
-                    convert(val, element)
-                else:
-                    element = ET.SubElement(parent, key)
-                    element.text = str(val)
-
-        convert(self.to_dict(), root)
-        return ET.tostring(root, encoding="unicode")
-
-    def to_pd_series(self, *args, pd_kwargs: dict | None = None, **kwargs) -> Series:
-        """
-        Convert the node to a Pandas Series.
-
-        Returns:
-            Series: The Pandas Series representation of the node.
-        """
-        pd_kwargs = {} if pd_kwargs is None else pd_kwargs
-        dict_ = self.to_dict(*args, **kwargs)
-        return Series(dict_, **pd_kwargs)
+    def __str__(self):
+        return f"{self.__class__.__name__}({self.to_json_str()})"
 
 
 class BaseNode(BaseComponent):
     """
     Base class for creating node models.
 
     Attributes:
@@ -260,146 +301,182 @@
         default=None,
         validation_alias=AliasChoices("text", "page_content", "chunk_content", "data"),
         description="The optional content of the node.",
     )
 
     metadata: dict[str, Any] = Field(
         default_factory=dict,
-        alias="meta",
+        validation_alias="meta",
         description="Additional metadata for the node.",
     )
 
     @singledispatchmethod
     @classmethod
     def from_obj(cls, obj: Any, *args, **kwargs) -> T:
         """
         Create a node instance from an object.
 
         Args:
             obj (Any): The object to create the node from.
+            *args: Additional positional arguments.
+            **kwargs: Additional keyword arguments.
 
         Raises:
             NotImplementedError: If the object type is not supported.
         """
+        if not isinstance(obj, (dict, str, list, Series, DataFrame, BaseModel)):
+            type_ = str(type(obj))
+            if "llama_index" in type_:
+                return cls.from_obj(obj.to_dict())
+            elif "langchain" in type_:
+                langchain_json = obj.to_json()
+                langchain_dict = {
+                    "lc_id": langchain_json["id"],
+                    **langchain_json["kwargs"],
+                }
+                return cls.from_obj(langchain_dict)
+
         raise NotImplementedError(f"Unsupported type: {type(obj)}")
 
     @from_obj.register(dict)
     @classmethod
-    def _from_dict(cls, obj, *args, **kwargs) -> T:
+    def _from_dict(cls, obj: dict, *args, **kwargs) -> T:
         """
         Create a node instance from a dictionary.
 
         Args:
             obj (dict): The dictionary to create the node from.
+            *args: Additional positional arguments.
+            **kwargs: Additional keyword arguments.
 
         Returns:
             T: The created node instance.
         """
         return cls.model_validate(obj, *args, **kwargs)
 
     @from_obj.register(str)
     @classmethod
-    def _from_str(cls, obj, *args, fuzzy_parse=False, **kwargs) -> T:
+    def _from_str(cls, obj: str, *args, fuzzy_parse: bool = False, **kwargs) -> T:
         """
         Create a node instance from a JSON string.
 
         Args:
             obj (str): The JSON string to create the node from.
+            *args: Additional positional arguments.
             fuzzy_parse (bool): Whether to perform fuzzy parsing.
+            **kwargs: Additional keyword arguments.
 
         Returns:
             T: The created node instance.
         """
         obj = ParseUtil.fuzzy_parse_json(obj) if fuzzy_parse else convert.to_dict(obj)
         try:
             return cls.from_obj(obj, *args, **kwargs)
         except ValidationError as e:
             raise ValueError(f"Invalid JSON for deserialization: {e}") from e
 
     @from_obj.register(list)
     @classmethod
-    def _from_list(cls, obj, *args, **kwargs) -> list[T]:
+    def _from_list(cls, obj: list, *args, **kwargs) -> list[T]:
         """
         Create a list of node instances from a list of objects.
 
         Args:
             obj (list): The list of objects to create nodes from.
+            *args: Additional positional arguments.
+            **kwargs: Additional keyword arguments.
 
         Returns:
             list[T]: The list of created node instances.
         """
         return [cls.from_obj(item, *args, **kwargs) for item in obj]
 
     @from_obj.register(Series)
     @classmethod
-    def _from_pd_series(cls, obj, *args, pd_kwargs=None, **kwargs) -> T:
+    def _from_pd_series(
+        cls, obj: Series, *args, pd_kwargs: dict | None = None, **kwargs
+    ) -> T:
         """
         Create a node instance from a Pandas Series.
 
         Args:
             obj (Series): The Pandas Series to create the node from.
+            *args: Additional positional arguments.
+            pd_kwargs (dict | None): Additional keyword arguments for Pandas Series.
+            **kwargs: Additional keyword arguments.
 
         Returns:
             T: The created node instance.
         """
-        if pd_kwargs is None:
-            pd_kwargs = {}
+        pd_kwargs = pd_kwargs or {}
         return cls.from_obj(obj.to_dict(**pd_kwargs), *args, **kwargs)
 
     @from_obj.register(DataFrame)
     @classmethod
-    def _from_pd_dataframe(cls, obj, *args, pd_kwargs=None, **kwargs) -> list[T]:
+    def _from_pd_dataframe(
+        cls, obj: DataFrame, *args, pd_kwargs: dict | None = None, **kwargs
+    ) -> list[T]:
         """
         Create a list of node instances from a Pandas DataFrame.
 
         Args:
             obj (DataFrame): The Pandas DataFrame to create nodes from.
+            *args: Additional positional arguments.
+            pd_kwargs (dict | None): Additional keyword arguments for Pandas DataFrame.
+            **kwargs: Additional keyword arguments.
 
         Returns:
             list[T]: The list of created node instances.
         """
         if pd_kwargs is None:
             pd_kwargs = {}
-        return [
-            cls.from_obj(row, *args, **pd_kwargs, **kwargs) for _, row in obj.iterrows()
-        ]
+
+        _objs = []
+        for index, row in obj.iterrows():
+            _obj = cls.from_obj(row, *args, **pd_kwargs, **kwargs)
+            _obj.metadata["df_index"] = index
+            _objs.append(_obj)
+
+        return _objs
 
     @from_obj.register(BaseModel)
     @classmethod
     def _from_base_model(cls, obj, pydantic_kwargs=None, **kwargs) -> T:
         """
         Create a node instance from a Pydantic BaseModel.
 
         Args:
             obj (BaseModel): The Pydantic BaseModel to create the node from.
 
         Returns:
             T: The created node instance.
         """
-        if pydantic_kwargs is None:
-            pydantic_kwargs = {"by_alias": True}
-
-        config_ = {}
+        pydantic_kwargs = pydantic_kwargs or {"by_alias": True}
         try:
-            config_ = obj.model_dump(**pydantic_kwargs)
-        except:
-            config_ = obj.dict(**pydantic_kwargs)
+            config_ = {}
+            try:
+                config_ = obj.model_dump(**pydantic_kwargs)
+            except:
+                config_ = obj.to_dict(**pydantic_kwargs)
+            else:
+                config_ = obj.dict(**pydantic_kwargs)
+        except Exception as e:
+            raise ValueError(f"Invalid Pydantic model for deserialization: {e}") from e
 
         return cls.from_obj(config_ | kwargs)
 
     def meta_get(
-        self, key: str, indices: list[str | int] = None, default: Any = None
+        self, key: str, indices: list[str | int] | None = None, default: Any = None
     ) -> Any:
         """
         Get a value from the metadata dictionary.
 
         Args:
             key (str): The key to retrieve the value for.
-            indices (list[str | int]): Optional list of indices for nested
-                retrieval.
+            indices (list[str | int] | None): Optional list of indices for nested retrieval.
             default (Any): The default value to return if the key is not found.
 
         Returns:
             Any: The retrieved value or the default value if not found.
         """
         if indices:
             return nested.nget(self.metadata, indices, default)
@@ -448,8 +525,8 @@
             overwrite (bool): Whether to overwrite existing keys with the new
                 values.
             **kwargs: Additional keyword arguments for the `nested.nmerge`
                 function.
         """
         self.metadata = nested.nmerge(
             [self.metadata, additional_metadata], overwrite=overwrite, **kwargs
-        )
+        )
```

### Comparing `lionagi-0.1.1/lionagi/core/generic/condition.py` & `lionagi-0.1.2/lionagi/core/generic/condition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from abc import ABC, abstractmethod
 from enum import Enum
+from typing import Callable
 from pydantic import BaseModel, Field
 
 
 class ConditionSource(str, Enum):
     """
     Enumeration for specifying the source type of a condition.
 
     Attributes:
         STRUCTURE: Represents a condition based on the structure.
         EXECUTABLE: Represents a condition that can be executed or evaluated.
     """
 
     STRUCTURE = "structure"
     EXECUTABLE = "executable"
+    RULE = "rule"
 
 
 class Condition(BaseModel, ABC):
     """
     Abstract base class for defining conditions associated with edges.
 
     Attributes:
```

### Comparing `lionagi-0.1.1/lionagi/core/generic/data_logger.py` & `lionagi-0.1.2/lionagi/core/generic/data_logger.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/edge.py` & `lionagi-0.1.2/lionagi/core/generic/edge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,109 +1,115 @@
 """
-Module for representing conditions and edges between nodes in a graph structure.
+Module for representing conditions and edges between nodes in a graph.
 
-This module provides the base for creating and managing edges that connect nodes
-within a graph. It includes support for conditional edges, allowing the dynamic
-evaluation of connections based on custom logic.
+This module provides the base for creating and managing edges that connect
+nodes within a graph. It includes support for conditional edges, allowing
+the dynamic evaluation of connections based on custom logic.
 """
 
 from typing import Any
 from pydantic import Field, field_validator
-from lionagi.core.generic.component import BaseComponent, BaseNode
-from lionagi.core.generic.condition import Condition
+from .component import BaseComponent
+from .condition import Condition
 
 
 class Edge(BaseComponent):
     """
     Represents an edge between two nodes, potentially with a condition.
 
     Attributes:
         head (str): The identifier of the head node of the edge.
         tail (str): The identifier of the tail node of the edge.
-        condition (Optional[Condition]): An optional condition that must be met
+        condition (Condition | None): Optional condition that must be met
             for the edge to be considered active.
-        label (Optional[str]): An optional label for the edge.
+        label (str | None): An optional label for the edge.
+        bundle (bool): A flag indicating if the edge is bundled.
 
     Methods:
-        check_condition: Evaluates if the condition associated with the edge is met.
+        check_condition: Evaluates if the condition is met.
+        string_condition: Retrieves the condition class source code.
     """
 
     head: str = Field(
         title="Head",
         description="The identifier of the head node of the edge.",
     )
     tail: str = Field(
         title="Tail",
         description="The identifier of the tail node of the edge.",
     )
     condition: Condition | None = Field(
         default=None,
-        description="An optional condition that must be met for the edge to be considered active.",
+        description="Optional condition that must be met for the edge "
+                    "to be considered active.",
     )
     label: str | None = Field(
         default=None,
         description="An optional label for the edge.",
     )
     bundle: bool = Field(
         default=False,
         description="A flag indicating if the edge is bundled.",
     )
 
     @field_validator("head", "tail", mode="before")
     def _validate_head_tail(cls, value):
         """
-        Validates the head and tail fields to ensure they are valid node identifiers.
+        Validates head and tail fields to ensure valid node identifiers.
 
         Args:
-            value: The value of the field being validated.
-            values: A dictionary of all other values on the model.
-            field: The model field being validated.
+            value (Any): The value of the field being validated.
 
         Returns:
-            The validated value, ensuring it is a valid identifier.
+            str: The validated value, ensuring it is a valid identifier.
 
         Raises:
             ValueError: If the validation fails.
         """
-        if isinstance(value, BaseNode):
+
+        if isinstance(value, BaseComponent):
             return value.id_
         return value
 
     def check_condition(self, obj: dict[str, Any]) -> bool:
         """
         Evaluates if the condition associated with the edge is met.
 
         Args:
-            obj (dict[str, Any]): The context object used for condition evaluation.
+            obj (dict[str, Any]): Context for condition evaluation.
 
         Returns:
             bool: True if the condition is met, False otherwise.
 
         Raises:
             ValueError: If the condition is not set.
         """
         if not self.condition:
             raise ValueError("The condition for the edge is not set.")
         return self.condition(obj)
 
     def string_condition(self):
         """
-        Retrieves the source code of the condition class associated with this edge as a string.
+        Retrieves the condition class source code as a string.
 
-        This method is useful for serialization and debugging, allowing the condition logic to be inspected or stored
-        in a human-readable format. It employs advanced introspection techniques to locate and extract the exact class
-        definition, handling edge cases like dynamically defined classes or classes defined in interactive environments.
+        This method is useful for serialization and debugging, allowing
+        the condition logic to be inspected or stored in a human-readable
+        format. It employs advanced introspection techniques to locate and
+        extract the exact class definition, handling edge cases like
+        dynamically defined classes or classes defined interactively.
 
         Returns:
-            str: The source code of the condition's class, if available. If the condition is None or the source code
-                cannot be located, this method returns None.
+            str | None: The condition class source code if available.
+                If the condition is None or the source code cannot be
+                located, this method returns None.
 
         Raises:
-            TypeError: If the source code of the condition's class cannot be found due to the class being defined in a
-                non-standard manner or in the interactive interpreter (__main__ context).
+            TypeError: If the condition class source code cannot be found
+                due to the class being defined in a non-standard manner or
+                in the interactive interpreter (__main__ context).
         """
         if self.condition is None:
             return
 
         import inspect, sys
 
         def new_getfile(object, _old_getfile=inspect.getfile):
@@ -135,28 +141,22 @@
         obj = self.condition.__class__
         cell_code = "".join(inspect.linecache.getlines(new_getfile(obj)))
         class_code = extract_symbols(cell_code, obj.__name__)[0][0]
         return class_code
 
     def __str__(self) -> str:
         """
-        Returns a simple string representation of the Relationship.
+        Returns a simple string representation of the Edge.
         """
-
         return (
             f"Edge (id_={self.id_}, from={self.head}, to={self.tail}, "
             f"label={self.label})"
         )
 
     def __repr__(self) -> str:
         """
-        Returns a detailed string representation of the Relationship.
-
-        Examples:
-            >>> edge = Relationship(source_node_id="node1", target_node_id="node2")
-            >>> repr(edge)
-            'Relationship(id_=None, from=node1, to=node2, content=None, metadata=None, label=None)'
+        Returns a detailed string representation of the Edge.
         """
         return (
             f"Edge(id_={self.id_}, from={self.head}, to={self.tail}, "
             f"label={self.label})"
         )
```

### Comparing `lionagi-0.1.1/lionagi/core/generic/mail.py` & `lionagi-0.1.2/lionagi/core/generic/mail.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/mailbox.py` & `lionagi-0.1.2/lionagi/core/generic/mailbox.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/node.py` & `lionagi-0.1.2/lionagi/core/generic/node.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/relation.py` & `lionagi-0.1.2/lionagi/core/generic/relation.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/signal.py` & `lionagi-0.1.2/lionagi/core/generic/signal.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/structure.py` & `lionagi-0.1.2/lionagi/core/generic/structure.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/transfer.py` & `lionagi-0.1.2/lionagi/core/generic/transfer.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/generic/work.py` & `lionagi-0.1.2/lionagi/core/generic/work.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/graph/graph.py` & `lionagi-0.1.2/lionagi/core/graph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
         from networkx import DiGraph
 
         g = DiGraph(**kwargs)
         for node_id, node in self.internal_nodes.items():
             node_info = node.to_dict()
             node_info.pop("id_")
-            node_info.update({"class_name": node.class_name()})
+            node_info.update({"class_name": node.class_name})
             g.add_node(node_id, **node_info)
 
         for _edge in list(self.internal_edges.values()):
             edge_info = _edge.to_dict()
             edge_info.pop("id_")
             edge_info.update({"class_name": _edge.__class__.__name__})
             source_node_id = edge_info.pop("head")
```

### Comparing `lionagi-0.1.1/lionagi/core/graph/tree.py` & `lionagi-0.1.2/lionagi/core/graph/tree.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/mail/mail_manager.py` & `lionagi-0.1.2/lionagi/core/mail/mail_manager.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/mail/schema.py` & `lionagi-0.1.2/lionagi/core/mail/schema.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/messages/schema.py` & `lionagi-0.1.2/lionagi/core/messages/schema.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/session/session.py` & `lionagi-0.1.2/lionagi/core/session/session.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/tool/tool.py` & `lionagi-0.1.2/lionagi/core/tool/tool.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/core/tool/tool_manager.py` & `lionagi-0.1.2/lionagi/core/tool/tool_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,23 +155,24 @@
             elif isinstance(tool, str):
                 if self.name_existed(tool):
                     tool: Tool = self.registry[tool]
                     return tool.schema_
                 else:
                     raise ValueError(f"Function {tool} is not registered.")
 
-        if isinstance(tools, bool):
-            tool_kwarg = {"tools": self.to_tool_schema_list()}
-            kwargs = tool_kwarg | kwargs
+        if tools:
+            if isinstance(tools, bool):
+                tool_kwarg = {"tools": self.to_tool_schema_list()}
+                kwargs = tool_kwarg | kwargs
 
-        else:
-            if not isinstance(tools, list):
-                tools = [tools]
-            tool_kwarg = {"tools": func_call.lcall(tools, tool_check)}
-            kwargs = tool_kwarg | kwargs
+            else:
+                if not isinstance(tools, list):
+                    tools = [tools]
+                tool_kwarg = {"tools": func_call.lcall(tools, tool_check)}
+                kwargs = tool_kwarg | kwargs
 
         return kwargs
 
 
 def func_to_tool(
     func_: Callable | list[Callable], parser=None, docstring_style="google"
 ):
```

### Comparing `lionagi-0.1.1/lionagi/experimental/directive/evaluator/ast_evaluator.py` & `lionagi-0.1.2/lionagi/experimental/directive/evaluator/ast_evaluator.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/directive/evaluator/base_evaluator.py` & `lionagi-0.1.2/lionagi/experimental/directive/evaluator/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/directive/evaluator/script_engine.py` & `lionagi-0.1.2/lionagi/experimental/directive/evaluator/script_engine.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/directive/parser/base_parser.py` & `lionagi-0.1.2/lionagi/experimental/directive/parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/directive/schema.py` & `lionagi-0.1.2/lionagi/experimental/directive/schema.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/directive/template_/base_template.py` & `lionagi-0.1.2/lionagi/experimental/directive/template_/base_template.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/tool/function_calling.py` & `lionagi-0.1.2/lionagi/experimental/tool/function_calling.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/tool/manual.py` & `lionagi-0.1.2/lionagi/experimental/tool/manual.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/tool/schema.py` & `lionagi-0.1.2/lionagi/experimental/tool/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
     @invoke.register
     async def _(self, kwargs: dict):
 
         out = None
 
         if self.pre_processor:
-            kwargs = await func_call.unified_call(self.pre_processor, kwargs)
+            kwargs = await func_call.call_handler(self.pre_processor, kwargs)
         try:
-            out = await func_call.unified_call(self.func, **kwargs)
+            out = await func_call.call_handler(self.func, **kwargs)
 
         except Exception as e:
             _logging.error(f"Error invoking function {self.func_name}: {e}")
             return None
 
         if self.post_processor:
-            return await func_call.unified_call(self.post_processor, out)
+            return await func_call.call_handler(self.post_processor, out)
 
         return out
 
     @invoke.register
     async def _(self, function_calls: FunctionCalling):
         return await self.invoke(function_calls.kwargs)
```

### Comparing `lionagi-0.1.1/lionagi/experimental/tool/tool_manager.py` & `lionagi-0.1.2/lionagi/experimental/tool/tool_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         name, kwargs = func_params
         if not self._has_name(name):
             raise ValueError(f"Function {name} is not registered.")
         tool = self.registry[name]
         func = tool.func
         parser = tool.parser
         try:
-            out = await func_call.unified_call(func, **kwargs)
+            out = await func_call.call_handler(func, **kwargs)
             return parser(out) if parser else out
 
         except Exception as e:
             raise ValueError(
                 f"Error when invoking function {name} with arguments {kwargs} with error message {e}"
             ) from e
```

### Comparing `lionagi-0.1.1/lionagi/experimental/work/schema.py` & `lionagi-0.1.2/lionagi/experimental/work2/schema.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/experimental/work/tests.py` & `lionagi-0.1.2/lionagi/experimental/work2/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .schema import Work, WorkStatus
-from ._logger import WorkLog
+from ..work.worklog import WorkLog
 from .work_function import WorkFunction
 
 import unittest
 from unittest.mock import AsyncMock, patch
 
 from lionagi.libs import func_call
```

### Comparing `lionagi-0.1.1/lionagi/experimental/work/work_function.py` & `lionagi-0.1.2/lionagi/experimental/work2/work_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import Field
 from functools import wraps
 from lionagi import logging as _logging
 from lionagi.libs import func_call
 from lionagi.core.generic import BaseComponent
 
 from .schema import Work, WorkStatus
-from ._logger import WorkLog
+from ..work.worklog import WorkLog
 from .worker import Worker
 
 
 class WorkFunction(BaseComponent):
     """Work function management and execution."""
 
     function: Callable
```

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/autogen_/autogen_.py` & `lionagi-0.1.2/lionagi/integrations/bridge/autogen_/autogen_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/langchain_/documents.py` & `lionagi-0.1.2/lionagi/integrations/bridge/langchain_/documents.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/langchain_/langchain_bridge.py` & `lionagi-0.1.2/lionagi/integrations/bridge/langchain_/langchain_bridge.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/get_index.py` & `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/get_index.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py` & `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/llama_pack.py` & `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/llama_pack.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/node_parser.py` & `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/node_parser.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/reader.py` & `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/reader.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/textnode.py` & `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/textnode.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/bridge/transformers_/install_.py` & `lionagi-0.1.2/lionagi/integrations/bridge/transformers_/install_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/chunker/chunk.py` & `lionagi-0.1.2/lionagi/integrations/chunker/chunk.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/config/oai_configs.py` & `lionagi-0.1.2/lionagi/integrations/config/oai_configs.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/config/openrouter_configs.py` & `lionagi-0.1.2/lionagi/integrations/config/openrouter_configs.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/loader/load.py` & `lionagi-0.1.2/lionagi/integrations/loader/load.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/loader/load_util.py` & `lionagi-0.1.2/lionagi/integrations/loader/load_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/provider/litellm.py` & `lionagi-0.1.2/lionagi/integrations/provider/litellm.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/provider/mlx_service.py` & `lionagi-0.1.2/lionagi/integrations/provider/mlx_service.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/provider/oai.py` & `lionagi-0.1.2/lionagi/integrations/provider/oai.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/provider/ollama.py` & `lionagi-0.1.2/lionagi/integrations/provider/ollama.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/provider/openrouter.py` & `lionagi-0.1.2/lionagi/integrations/provider/openrouter.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/provider/services.py` & `lionagi-0.1.2/lionagi/integrations/provider/services.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/provider/transformers.py` & `lionagi-0.1.2/lionagi/integrations/provider/transformers.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/storage/neo4j.py` & `lionagi-0.1.2/lionagi/integrations/storage/neo4j.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/storage/storage_util.py` & `lionagi-0.1.2/lionagi/integrations/storage/storage_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,26 +25,26 @@
     """
     summary_list = []
     output = {}
 
     structure_output = {
         "id": structure.id_,
         "timestamp": structure.timestamp,
-        "type": structure.class_name(),
+        "type": structure.class_name,
     }
     summary_list.append(structure_output.copy())
-    structure_output["head_nodes"] = [i.id_ for i in structure.get_heads()]
+    structure_output["head_nodes"] = json.dumps([i.id_ for i in structure.get_heads()])
     # structure_output['nodes'] = json.dumps([i for i in structure.internal_nodes.keys()])
     # structure_output['edges'] = json.dumps([i for i in structure.internal_edges.keys()])
     output[structure_output["type"]] = [structure_output]
     for node in structure.internal_nodes.values():
         node_output = {
             "id": node.id_,
             "timestamp": node.timestamp,
-            "type": node.class_name(),
+            "type": node.class_name,
         }
         summary_list.append(node_output.copy())
         if isinstance(node, System) or isinstance(node, Instruction):
             node_output["content"] = json.dumps(node.content)
             node_output["sender"] = node.sender
             node_output["recipient"] = node.recipient
         elif isinstance(node, Tool):
@@ -282,8 +282,8 @@
         cls = ParseNode.convert_to_class(cls_code)
 
         init_params = {}
         for key in inspect.signature(cls.__init__).parameters.keys():
             if key == "self":
                 continue
             init_params[key] = args[key]
-        return cls(**init_params)
+        return cls(**init_params)
```

### Comparing `lionagi-0.1.1/lionagi/integrations/storage/to_csv.py` & `lionagi-0.1.2/lionagi/integrations/storage/to_csv.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/integrations/storage/to_excel.py` & `lionagi-0.1.2/lionagi/integrations/storage/to_excel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 import pandas as pd
 from lionagi.libs import SysUtil
 
 from lionagi.integrations.storage.storage_util import output_node_list, output_edge_list
 
 
-def _output_excel(
-    node_list, node_dict, edge_list, edge_cls_list, filename="structure_storage"
-):
+def _output_excel(node_list, node_dict, edge_list, edge_cls_list, structure_name, dir="structure_storage"):
     """
     Writes provided node and edge data into multiple sheets of a single Excel workbook.
 
     This helper function takes lists and dictionaries of nodes and edges, converts them into pandas DataFrames,
     and then writes each DataFrame to a distinct sheet in an Excel workbook. This includes a separate sheet
     for each type of node and edge, as well as edge conditions if they exist.
 
     Args:
         node_list (list): A list of dictionaries where each dictionary contains attributes of a single node.
         node_dict (dict): A dictionary of lists where each key represents a node type and the value is a list of
                           node attributes for nodes of that type.
         edge_list (list): A list of dictionaries where each dictionary contains attributes of a single edge.
         edge_cls_list (list): A list of dictionaries where each dictionary contains attributes of edge conditions.
-        filename (str): The base name for the output Excel file. The '.xlsx' extension will be added
+        structure_name (str): The base name for the output Excel file. The '.xlsx' extension will be added
                         automatically if not included.
 
     Returns:
         None: This function does not return a value but writes data directly to an Excel workbook.
 
     Raises:
         ImportError: If the required 'openpyxl' library is not installed, which is necessary for pandas to write Excel files.
     """
     SysUtil.check_import("openpyxl")
 
+    structure_id = ""
+
     tables = {"Nodes": pd.DataFrame(node_list), "Edges": pd.DataFrame(edge_list)}
     if edge_cls_list:
         tables["EdgesCondClass"] = pd.DataFrame(edge_cls_list)
     for i in node_dict:
+        if i == "StructureExecutor":
+            structure_node = node_dict[i][0]
+            structure_node["name"] = structure_name
+            structure_id = structure_node["id"]
         tables[i] = pd.DataFrame(node_dict[i])
 
-    filename = filename + ".xlsx"
+    import os
+    filepath = os.path.join(dir, f"{structure_name}_{structure_id}.xlsx")
+
+    if not os.path.exists(dir):
+        os.makedirs(dir)
 
-    with pd.ExcelWriter(filename) as writer:
+    with pd.ExcelWriter(filepath) as writer:
         for i in tables:
             tables[i].to_excel(writer, sheet_name=i, index=False)
 
 
-def to_excel(structure, filename="structure_storage"):
+def to_excel(structure, structure_name, dir="structure_storage"):
     """
     Converts a structure into a series of Excel sheets within a single workbook.
 
     This function processes the specified structure to extract detailed node and edge information,
     including conditions if applicable. These details are then saved into separate sheets within an
     Excel workbook for nodes, edges, and any edge conditions.
 
     Args:
         structure: An object representing the structure to be serialized. This should have methods
                    to return lists of nodes and edges suitable for output.
-        filename (str): The base name of the output Excel file. The '.xlsx' extension will be added
+        structure_name (str): The base name of the output Excel file. The '.xlsx' extension will be added
                         automatically if not included.
 
     Returns:
         None: This function does not return a value but outputs an Excel workbook with multiple sheets.
     """
     node_list, node_dict = output_node_list(structure)
     edge_list, edge_cls_list = output_edge_list(structure)
 
-    _output_excel(node_list, node_dict, edge_list, edge_cls_list, filename)
+    _output_excel(node_list, node_dict, edge_list, edge_cls_list, structure_name, dir)
+
```

### Comparing `lionagi-0.1.1/lionagi/libs/ln_api.py` & `lionagi-0.1.2/lionagi/libs/ln_api.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_async.py` & `lionagi-0.1.2/lionagi/libs/ln_async.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_convert.py` & `lionagi-0.1.2/lionagi/libs/ln_convert.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_dataframe.py` & `lionagi-0.1.2/lionagi/libs/ln_dataframe.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_func_call.py` & `lionagi-0.1.2/lionagi/libs/ln_func_call.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_knowledge_graph.py` & `lionagi-0.1.2/lionagi/libs/ln_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_nested.py` & `lionagi-0.1.2/lionagi/libs/ln_nested.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_parse.py` & `lionagi-0.1.2/lionagi/libs/ln_parse.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_queue.py` & `lionagi-0.1.2/lionagi/libs/ln_queue.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_tokenizer.py` & `lionagi-0.1.2/lionagi/libs/ln_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/ln_validate.py` & `lionagi-0.1.2/lionagi/libs/ln_validate.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/libs/sys_util.py` & `lionagi-0.1.2/lionagi/libs/sys_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/lions/coder/add_feature.py` & `lionagi-0.1.2/lionagi/lions/coder/add_feature.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/lions/coder/coder.py` & `lionagi-0.1.2/lionagi/lions/coder/coder.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/lions/coder/util.py` & `lionagi-0.1.2/lionagi/lions/coder/util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/lions/researcher/data_source/finhub_.py` & `lionagi-0.1.2/lionagi/lions/researcher/data_source/finhub_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/lions/researcher/data_source/google_.py` & `lionagi-0.1.2/lionagi/lions/researcher/data_source/google_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/lions/researcher/data_source/wiki_.py` & `lionagi-0.1.2/lionagi/lions/researcher/data_source/wiki_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/lions/researcher/data_source/yfinance_.py` & `lionagi-0.1.2/lionagi/lions/researcher/data_source/yfinance_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/libs/test_api.py` & `lionagi-0.1.2/lionagi/tests/libs/test_api.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/libs/test_convert.py` & `lionagi-0.1.2/lionagi/tests/libs/test_convert.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/libs/test_field_validators.py` & `lionagi-0.1.2/lionagi/tests/libs/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/libs/test_func_call.py` & `lionagi-0.1.2/lionagi/tests/libs/test_func_call.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/libs/test_nested.py` & `lionagi-0.1.2/lionagi/tests/libs/test_nested.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/libs/test_parse.py` & `lionagi-0.1.2/lionagi/tests/libs/test_parse.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/libs/test_queue.py` & `lionagi-0.1.2/lionagi/tests/libs/test_queue.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/libs/test_sys_util.py` & `lionagi-0.1.2/lionagi/tests/libs/test_sys_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/test_core/test_base_branch.py` & `lionagi-0.1.2/lionagi/tests/test_core/test_base_branch.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/test_core/test_branch.py` & `lionagi-0.1.2/lionagi/tests/test_core/test_branch.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/test_core/test_chat_flow.py` & `lionagi-0.1.2/lionagi/tests/test_core/test_chat_flow.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/test_core/test_mail_manager.py` & `lionagi-0.1.2/lionagi/tests/test_core/test_mail_manager.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/test_core/test_prompts.py` & `lionagi-0.1.2/lionagi/tests/test_core/test_prompts.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/test_core/test_session.py` & `lionagi-0.1.2/lionagi/tests/test_core/test_session.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/test_core/test_session_base_util.py` & `lionagi-0.1.2/lionagi/tests/test_core/test_session_base_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi/tests/test_core/test_tool_manager.py` & `lionagi-0.1.2/lionagi/tests/test_core/test_tool_manager.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/lionagi.egg-info/PKG-INFO` & `lionagi-0.1.2/lionagi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lionagi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Towards automated general intelligence.
 Author: HaiyangLi
 Author-email: Haiyang Li <ocean@lionagi.ai>
 License: MIT License
         
         Copyright (c) 2023 HaiyangLi quantocean.li@gmail.com
```

### Comparing `lionagi-0.1.1/lionagi.egg-info/SOURCES.txt` & `lionagi-0.1.2/lionagi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -86,28 +86,41 @@
 lionagi/experimental/directive/evaluator/base_evaluator.py
 lionagi/experimental/directive/evaluator/sandbox_.py
 lionagi/experimental/directive/evaluator/script_engine.py
 lionagi/experimental/directive/parser/__init__.py
 lionagi/experimental/directive/parser/base_parser.py
 lionagi/experimental/directive/template_/__init__.py
 lionagi/experimental/directive/template_/base_template.py
+lionagi/experimental/report/__init__.py
+lionagi/experimental/report/form.py
+lionagi/experimental/report/report.py
+lionagi/experimental/report/util.py
 lionagi/experimental/tool/__init__.py
 lionagi/experimental/tool/function_calling.py
 lionagi/experimental/tool/manual.py
 lionagi/experimental/tool/schema.py
 lionagi/experimental/tool/tool_manager.py
 lionagi/experimental/tool/util.py
+lionagi/experimental/validator/__init__.py
+lionagi/experimental/validator/rule.py
+lionagi/experimental/validator/validator.py
 lionagi/experimental/work/__init__.py
-lionagi/experimental/work/_logger.py
-lionagi/experimental/work/exchange.py
+lionagi/experimental/work/async_queue.py
 lionagi/experimental/work/schema.py
-lionagi/experimental/work/tests.py
-lionagi/experimental/work/util.py
 lionagi/experimental/work/work_function.py
 lionagi/experimental/work/worker.py
+lionagi/experimental/work2/__init__.py
+lionagi/experimental/work2/form.py
+lionagi/experimental/work2/report.py
+lionagi/experimental/work2/schema.py
+lionagi/experimental/work2/tests.py
+lionagi/experimental/work2/util.py
+lionagi/experimental/work2/work.py
+lionagi/experimental/work2/work_function.py
+lionagi/experimental/work2/worker.py
 lionagi/integrations/__init__.py
 lionagi/integrations/bridge/__init__.py
 lionagi/integrations/bridge/autogen_/__init__.py
 lionagi/integrations/bridge/autogen_/autogen_.py
 lionagi/integrations/bridge/langchain_/__init__.py
 lionagi/integrations/bridge/langchain_/documents.py
 lionagi/integrations/bridge/langchain_/langchain_bridge.py
@@ -141,14 +154,15 @@
 lionagi/integrations/provider/ollama.py
 lionagi/integrations/provider/openrouter.py
 lionagi/integrations/provider/services.py
 lionagi/integrations/provider/transformers.py
 lionagi/integrations/storage/__init__.py
 lionagi/integrations/storage/neo4j.py
 lionagi/integrations/storage/storage_util.py
+lionagi/integrations/storage/structure_excel.py
 lionagi/integrations/storage/to_csv.py
 lionagi/integrations/storage/to_excel.py
 lionagi/libs/__init__.py
 lionagi/libs/ln_api.py
 lionagi/libs/ln_async.py
 lionagi/libs/ln_convert.py
 lionagi/libs/ln_dataframe.py
@@ -188,8 +202,10 @@
 lionagi/tests/test_core/test_base_branch.py
 lionagi/tests/test_core/test_branch.py
 lionagi/tests/test_core/test_chat_flow.py
 lionagi/tests/test_core/test_mail_manager.py
 lionagi/tests/test_core/test_prompts.py
 lionagi/tests/test_core/test_session.py
 lionagi/tests/test_core/test_session_base_util.py
-lionagi/tests/test_core/test_tool_manager.py
+lionagi/tests/test_core/test_tool_manager.py
+lionagi/tests/test_core/generic/__init__.py
+lionagi/tests/test_core/generic/test_component.py
```

### Comparing `lionagi-0.1.1/pyproject.toml` & `lionagi-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.1/setup.py` & `lionagi-0.1.2/setup.py`

 * *Files identical despite different names*

