# Comparing `tmp/spine_engine-0.23.4.tar.gz` & `tmp/spine_engine-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_engine-0.23.4.tar", last modified: Tue Apr 23 14:08:09 2024, max compression
+gzip compressed data, was "spine_engine-0.24.0.tar", last modified: Tue Apr 30 07:29:17 2024, max compression
```

## Comparing `spine_engine-0.23.4.tar` & `spine_engine-0.24.0.tar`

### file list

```diff
@@ -1,226 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.487058 spine_engine-0.23.4/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 14:08:02.000000 spine_engine-0.23.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 14:08:02.000000 spine_engine-0.23.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.459058 spine_engine-0.23.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 14:08:02.000000 spine_engine-0.23.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.459058 spine_engine-0.23.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-23 14:08:02.000000 spine_engine-0.23.4/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-23 14:08:02.000000 spine_engine-0.23.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 14:08:02.000000 spine_engine-0.23.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-23 14:08:02.000000 spine_engine-0.23.4/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-23 14:08:09.487058 spine_engine-0.23.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-23 14:08:02.000000 spine_engine-0.23.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 14:08:02.000000 spine_engine-0.23.4/bin/build_doc.bat
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 14:08:02.000000 spine_engine-0.23.4/bin/build_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 14:08:02.000000 spine_engine-0.23.4/bin/update_copyrights.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 14:08:02.000000 spine_engine-0.23.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/config/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_runner/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_runner/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/execution_manager_base/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/execution_manager_base/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/kernel_execution_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/kernel_execution_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/persistent_execution_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/persistent_execution_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/process_execution_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/process_execution_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/spine_repl/
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/spine_repl/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/load_project_items/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/load_project_items/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/executor/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/executor/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.463058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/multithread/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/multithread/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/thread_executor/
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/thread_executor/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/connection/
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/connection/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/executable_item_base/
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/executable_item_base/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_info/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_info/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_resource/
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_resource/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_specification/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_specification/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_specification_factory/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_specification_factory/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item_loader/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item_loader/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/spine_engine/
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/spine_engine/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/spine_engine_server/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/spine_engine_server/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/command_line_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/command_line_arguments/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/helpers/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/queue_logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/queue_logger/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/returning_process/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/returning_process/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/serialization/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/docs/source/autoapi/spine_engine/version/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/autoapi/spine_engine/version/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 14:08:02.000000 spine_engine-0.23.4/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.467058 spine_engine-0.23.4/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-04-23 14:08:02.000000 spine_engine-0.23.4/fig/eu-emblem-low-res.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-23 14:08:02.000000 spine_engine-0.23.4/fig/spineengine_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-23 14:08:02.000000 spine_engine-0.23.4/fig/spineengine_on_wht.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-04-23 14:08:02.000000 spine_engine-0.23.4/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-23 14:08:02.000000 spine_engine-0.23.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:08:09.487058 spine_engine-0.23.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.471058 spine_engine-0.23.4/spine_engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.471058 spine_engine-0.23.4/spine_engine/execution_managers/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17027 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/conda_kernel_spec_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/conda_kernel_spec_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/execution_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15105 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/kernel_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    30050 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/persistent_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/process_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/spine_repl.jl
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/execution_managers/spine_repl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/load_project_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.471058 spine_engine-0.23.4/spine_engine/multithread_executor/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/multithread_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/multithread_executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/multithread_executor/multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/multithread_executor/thread_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.475058 spine_engine-0.23.4/spine_engine/project_item/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/project_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/project_item/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/project_item/executable_item_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/project_item/project_item_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/project_item/project_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/project_item/project_item_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/project_item/project_item_specification_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/project_item_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.475058 spine_engine-0.23.4/spine_engine/server/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/certificate_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19693 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/engine_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/persistent_execution_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/ping_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/project_extractor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/project_remover_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/project_retriever_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/remote_execution_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/service_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/start_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.475058 spine_engine-0.23.4/spine_engine/server/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/util/event_data_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/util/server_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/server/util/zip_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/shared_memory_io_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    41739 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/spine_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.479058 spine_engine-0.23.4/spine_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/utils/command_line_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/utils/execution_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16898 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/utils/queue_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/utils/returning_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-23 14:08:02.000000 spine_engine-0.23.4/spine_engine/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 14:08:09.000000 spine_engine-0.23.4/spine_engine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.487058 spine_engine-0.23.4/spine_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-23 14:08:09.000000 spine_engine-0.23.4/spine_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-23 14:08:09.000000 spine_engine-0.23.4/spine_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:08:09.000000 spine_engine-0.23.4/spine_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:08:09.000000 spine_engine-0.23.4/spine_engine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-23 14:08:09.000000 spine_engine-0.23.4/spine_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 14:08:09.000000 spine_engine-0.23.4/spine_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.479058 spine_engine-0.23.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.479058 spine_engine-0.23.4/tests/execution_managers/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/execution_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/execution_managers/test_kernel_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/execution_managers/test_persistent_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/execution_managers/test_process_execution_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.455058 spine_engine-0.23.4/tests/mock_project_items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.479058 spine_engine-0.23.4/tests/mock_project_items/items_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/mock_project_items/items_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.479058 spine_engine-0.23.4/tests/mock_project_items/items_module/test_item/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/mock_project_items/items_module/test_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/mock_project_items/items_module/test_item/executable_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/mock_project_items/items_module/test_item/specification_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.479058 spine_engine-0.23.4/tests/project_item/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/project_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/project_item/test_ExecutableItem.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/project_item/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/project_item/test_project_item_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/helloworld.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/secfolder_for_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/secfolder_for_tests/allowEndpoints.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/secfolder_for_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/secfolder_for_tests/certificates/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/secfolder_for_tests/private_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/secfolder_for_tests/private_keys/client.key_secret
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/secfolder_for_tests/private_keys/server.key_secret
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/secfolder_for_tests/public_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/secfolder_for_tests/public_keys/client.key
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/secfolder_for_tests/public_keys/server.key
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/simple_importer.zip
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/test_EngineServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/test_PingService.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/test_ProjectExtractorService.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/test_ProjectRemoverService.py
--rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/test_RemoteExecutionService.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/test_start_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/util/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/local/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/local/project_local_data.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/local/specification_local_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.459058 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.483058 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/helloworld.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/helloworld2.json
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/projectforpackagingtests/input2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/test_EventDataConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/test_ServerMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/server/util/test_ZipHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/test_load_project_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    52384 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/test_spine_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:09.487058 spine_engine-0.23.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/utils/test_command_line_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/utils/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-23 14:08:02.000000 spine_engine-0.23.4/tests/utils/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 07:29:06.000000 spine_engine-0.24.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 07:29:06.000000 spine_engine-0.24.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-30 07:29:06.000000 spine_engine-0.24.0/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 07:29:06.000000 spine_engine-0.24.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 07:29:06.000000 spine_engine-0.24.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-30 07:29:06.000000 spine_engine-0.24.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-30 07:29:17.105780 spine_engine-0.24.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-30 07:29:06.000000 spine_engine-0.24.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-30 07:29:06.000000 spine_engine-0.24.0/bin/build_doc.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 07:29:06.000000 spine_engine-0.24.0/bin/build_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 07:29:06.000000 spine_engine-0.24.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/config/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_manager/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_runner/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/execution_manager_base/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/execution_manager_base/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/kernel_execution_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/kernel_execution_manager/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/persistent_execution_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/persistent_execution_manager/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/process_execution_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/process_execution_manager/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/spine_repl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/spine_repl/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/load_project_items/
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/load_project_items/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/executor/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/multithread/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/multithread/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/thread_executor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/thread_executor/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/connection/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/executable_item_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/executable_item_base/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_info/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_resource/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification_factory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification_factory/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item_loader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item_loader/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine_server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine_server/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/command_line_arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/command_line_arguments/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/helpers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/queue_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/queue_logger/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/returning_process/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/returning_process/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/serialization/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/version/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-04-30 07:29:06.000000 spine_engine-0.24.0/fig/eu-emblem-low-res.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-30 07:29:06.000000 spine_engine-0.24.0/fig/spineengine_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-30 07:29:06.000000 spine_engine-0.24.0/fig/spineengine_on_wht.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-04-30 07:29:06.000000 spine_engine-0.24.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-30 07:29:06.000000 spine_engine-0.24.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:29:17.105780 spine_engine-0.24.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.089780 spine_engine-0.24.0/spine_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.089780 spine_engine-0.24.0/spine_engine/execution_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/conda_kernel_spec_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/conda_kernel_spec_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/execution_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/kernel_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30262 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/persistent_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/process_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/spine_repl.jl
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/spine_repl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16252 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/jumpster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/load_project_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.093780 spine_engine-0.24.0/spine_engine/project_item/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28819 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/executable_item_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/project_item_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/project_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/project_item_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/project_item_specification_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.093780 spine_engine-0.24.0/spine_engine/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/certificate_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19731 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/engine_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/persistent_execution_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/ping_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/project_extractor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/project_remover_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/project_retriever_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/remote_execution_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/service_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/start_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.093780 spine_engine-0.24.0/spine_engine/server/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/util/event_data_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/util/server_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/util/zip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36567 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/spine_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/spine_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/command_line_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/execution_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17102 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/queue_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/returning_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 07:29:16.000000 spine_engine-0.24.0/spine_engine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/spine_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:29:16.000000 spine_engine-0.24.0/spine_engine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/tests/execution_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/execution_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/execution_managers/test_kernel_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/execution_managers/test_persistent_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/execution_managers/test_process_execution_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.073780 spine_engine-0.24.0/tests/mock_project_items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/tests/mock_project_items/items_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/mock_project_items/items_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/tests/mock_project_items/items_module/test_item/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/mock_project_items/items_module/test_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/mock_project_items/items_module/test_item/executable_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/mock_project_items/items_module/test_item/specification_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/project_item/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/project_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/project_item/test_ExecutableItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/project_item/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/project_item/test_project_item_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/secfolder_for_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/allowEndpoints.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/secfolder_for_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/certificates/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/secfolder_for_tests/private_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/private_keys/client.key_secret
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/private_keys/server.key_secret
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/secfolder_for_tests/public_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/public_keys/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/public_keys/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_EngineServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_PingService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_ProjectExtractorService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_ProjectRemoverService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_start_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/local/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/local/project_local_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/local/specification_local_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/helloworld.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/helloworld2.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/input2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/test_EventDataConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/test_ServerMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/test_ZipHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/zippedproject.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/test_load_project_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52129 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/test_spine_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/utils/test_command_line_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/utils/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/utils/test_serialization.py
```

### Comparing `spine_engine-0.23.4/.github/workflows/run_unit_tests.yml` & `spine_engine-0.24.0/.github/workflows/run_unit_tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,21 @@
     name: Unit tests
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [windows-latest, ubuntu-22.04]
         python-version: [3.8, 3.9, "3.10", 3.11]
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Version from Git tags
       run: git describe --tags
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Display Python version
       run:
          python -c "import sys; print(sys.version)"
     - name: Install additional packages for Linux
       if: runner.os == 'Linux'
@@ -34,15 +34,14 @@
     - name: Install dependencies
       env:
         PYTHONUTF8: 1
       run: |
         python -m pip install --upgrade pip
         pip install git+https://github.com/spine-tools/Spine-Database-API.git#egg=spinedb_api
         pip install .[dev]
-        pip install --no-deps git+https://github.com/spine-tools/spine-items.git#egg=spine_items
     - name: List packages
       run:
         pip list
     - name: Install python3 kernelspecs
       run: |
         pip install ipykernel
         python -m ipykernel install --user
@@ -53,8 +52,10 @@
         fi
         coverage run -m unittest discover --verbose
       shell: bash
     - name: Combine Coverage reports
       run:
         coverage combine
     - name: Upload coverage report to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
+      env:
+        CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `spine_engine-0.23.4/COPYING` & `spine_engine-0.24.0/COPYING`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/COPYING.LESSER` & `spine_engine-0.24.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/PKG-INFO` & `spine_engine-0.24.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: spine_engine
-Version: 0.23.4
+Version: 0.24.0
 Summary: A package to run Spine workflows.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/spine-engine
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12,>=3.8.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
-Requires-Dist: dagster<0.12.9,>=0.12.6
 Requires-Dist: pendulum<3.0.0
 Requires-Dist: protobuf<3.21.0
 Requires-Dist: networkx>2.5.1
 Requires-Dist: datapackage<1.16,>=1.15.2
 Requires-Dist: jupyter_client>=6.0
-Requires-Dist: spinedb_api>=0.30.5
+Requires-Dist: spinedb_api>=0.31.0
 Requires-Dist: pyzmq>=21.0
 Requires-Dist: markupsafe<2.1
 Provides-Extra: dev
 Requires-Dist: coverage[toml]; extra == "dev"
 
 # Spine Engine
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: spine_engine Version: 0.23.4 Summary: A package to
+Metadata-Version: 2.1 Name: spine_engine Version: 0.24.0 Summary: A package to
 run Spine workflows. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/spine-engine Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: <3.12,>=3.8.1 Description-Content-Type: text/markdown License-File:
-COPYING License-File: COPYING.LESSER Requires-Dist: dagster<0.12.9,>=0.12.6
-Requires-Dist: pendulum<3.0.0 Requires-Dist: protobuf<3.21.0 Requires-Dist:
-networkx>2.5.1 Requires-Dist: datapackage<1.16,>=1.15.2 Requires-Dist:
-jupyter_client>=6.0 Requires-Dist: spinedb_api>=0.30.5 Requires-Dist:
-pyzmq>=21.0 Requires-Dist: markupsafe<2.1 Provides-Extra: dev Requires-Dist:
-coverage[toml]; extra == "dev" # Spine Engine [![Python](https://
-img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)]
-(https://www.python.org/downloads/release/python-379/) [![Unit tests](https://
-github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)](https://
-github.com/spine-tools/spine-engine/actions?query=workflow%3A"Unit+tests") [!
-[codecov](https://codecov.io/gh/spine-tools/spine-engine/branch/master/graph/
-badge.svg)](https://codecov.io/gh/spine-tools/spine-engine) [![PyPI version]
-(https://badge.fury.io/py/spine-engine.svg)](https://badge.fury.io/py/spine-
-engine) A Python package to coordinate the execution of [Spine Toolbox](https:/
-/github.com/spine-tools/Spine-Toolbox) workflows.
+COPYING License-File: COPYING.LESSER Requires-Dist: pendulum<3.0.0 Requires-
+Dist: protobuf<3.21.0 Requires-Dist: networkx>2.5.1 Requires-Dist:
+datapackage<1.16,>=1.15.2 Requires-Dist: jupyter_client>=6.0 Requires-Dist:
+spinedb_api>=0.31.0 Requires-Dist: pyzmq>=21.0 Requires-Dist: markupsafe<2.1
+Provides-Extra: dev Requires-Dist: coverage[toml]; extra == "dev" # Spine
+Engine [![Python](https://img.shields.io/badge/python-
+3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/
+downloads/release/python-379/) [![Unit tests](https://github.com/spine-tools/
+spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/
+spine-engine/actions?query=workflow%3A"Unit+tests") [![codecov](https://
+codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://
+codecov.io/gh/spine-tools/spine-engine) [![PyPI version](https://badge.fury.io/
+py/spine-engine.svg)](https://badge.fury.io/py/spine-engine) A Python package
+to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/
+Spine-Toolbox) workflows.
                                 [Spine Engine]
 ## License Spine Engine is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
 the [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/
 by-sa/4.0/). ## Getting started ### Installation To install Spine Engine into
 an existing Python environment, run $ pip install spine_engine ### Dependencies
 Spine Engine installation will install [dagster](https://
```

### Comparing `spine_engine-0.23.4/README.md` & `spine_engine-0.24.0/README.md`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/Makefile` & `spine_engine-0.24.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/make.bat` & `spine_engine-0.24.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/config/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/config/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_manager/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_manager/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/execution_manager_base/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/execution_manager_base/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/kernel_execution_manager/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/kernel_execution_manager/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/persistent_execution_manager/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/persistent_execution_manager/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/process_execution_manager/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/process_execution_manager/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/execution_managers/spine_repl/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/spine_repl/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/load_project_items/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/load_project_items/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/executor/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/executor/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/multithread/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/multithread/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/multithread_executor/thread_executor/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/thread_executor/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/connection/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/connection/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/executable_item_base/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/executable_item_base/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_info/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_info/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_resource/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_resource/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_specification/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item/project_item_specification_factory/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification_factory/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/project_item_loader/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item_loader/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/spine_engine/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/spine_engine_server/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine_server/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/command_line_arguments/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/command_line_arguments/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/helpers/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/helpers/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/queue_logger/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/queue_logger/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/returning_process/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/returning_process/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/autoapi/spine_engine/utils/serialization/index.rst` & `spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/serialization/index.rst`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/docs/source/conf.py` & `spine_engine-0.24.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/fig/eu-emblem-low-res.jpg` & `spine_engine-0.24.0/fig/eu-emblem-low-res.jpg`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/fig/spineengine_logo.svg` & `spine_engine-0.24.0/fig/spineengine_logo.svg`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/fig/spineengine_on_wht.svg` & `spine_engine-0.24.0/fig/spineengine_on_wht.svg`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/pylintrc` & `spine_engine-0.24.0/pylintrc`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/pyproject.toml` & `spine_engine-0.24.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 classifiers = [
 	    "Programming Language :: Python :: 3",
 	    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
 	    "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8.1, <3.12"
 dependencies = [
-    # dagster >= 0.12.9 requires alembic that is incompatible with spinedb_api
-    "dagster>=0.12.6, <0.12.9",
     # dagster versions lower that 1.5.7 do not support pendulum >= 3.0.0
     "pendulum < 3.0.0",
     # https://developers.google.com/protocol-buffers/docs/news/2022-05-06#python-updates
     "protobuf<3.21.0",
     "networkx>2.5.1",
     "datapackage>=1.15.2, <1.16",
     "jupyter_client>=6.0",
-    "spinedb_api>=0.30.5",
+    "spinedb_api>=0.31.0",
     "pyzmq >=21.0",
     # dagster 0.12.8 requires Jinja2<3.0, which tries to import
     # soft_unicode, which has been removed in markupsafe 2.1
     "markupsafe < 2.1",
 ]
 
 [project.urls]
@@ -56,15 +54,16 @@
 	"fig*",
 	"tests*",
 ]
 
 [tool.coverage.run]
 source = ["spine_engine"]
 branch = true
+concurrency = ["multiprocessing", "thread"]
+disable_warnings = ["no-data-collected"]
 
 [tool.coverage.report]
 ignore_errors = true
 
 [tool.black]
 line-length = 120
-skip-string-normalization = true
 exclude = '\.git'
```

### Comparing `spine_engine-0.23.4/spine_engine/__init__.py` & `spine_engine-0.24.0/spine_engine/server/util/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-from .spine_engine import SpineEngine, SpineEngineState
-from .utils.helpers import ExecutionDirection, ItemExecutionFinishState
-from .version import __version__
+"""
+This package contains utility classes of remote server part of the Spine Engine.
+
+"""
```

### Comparing `spine_engine-0.23.4/spine_engine/config.py` & `spine_engine-0.24.0/spine_engine/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -30,16 +31,42 @@
 # GAMS
 GAMS_EXECUTABLE = _executable("gams")
 
 # Julia
 JULIA_EXECUTABLE = _executable("julia")
 
 # Python
+def is_frozen():
+    """Checks if we are currently running as frozen bundle.
+
+    Returns:
+        bool: True if we are frozen, False otherwise
+    """
+    return getattr(sys, "frozen", False)
+
+
+def is_pyinstaller_bundle():
+    """Checks if we are in a PyInstaller bundle.
+
+    Returns:
+        bool: True if the current bundle has been build by PyInstaller, False otherwise
+    """
+    return hasattr(sys, "_MEIPASS")
+
+
 PYTHON_EXECUTABLE = _executable("python" if _on_windows else "python3")
 _frozen = getattr(sys, "frozen", False)
 _path_to_executable = os.path.dirname(sys.executable if _frozen else __file__)
 APPLICATION_PATH = os.path.realpath(_path_to_executable)
-# Experimental Python interpreter shipped with Spine Toolbox installation bundle
-EMBEDDED_PYTHON = os.path.join(APPLICATION_PATH, "tools", "python.exe")
+# Python interpreter shipped with bundle
+BUNDLE_DIR = "Python"
+if is_frozen():
+    if is_pyinstaller_bundle():
+        EMBEDDED_PYTHON = os.path.join(sys._MEIPASS, BUNDLE_DIR, PYTHON_EXECUTABLE)
+    else:
+        EMBEDDED_PYTHON = os.path.join(APPLICATION_PATH, BUNDLE_DIR, PYTHON_EXECUTABLE)
+else:
+    EMBEDDED_PYTHON = None
+
 
 # Tool output directory name
 TOOL_OUTPUT_DIR = "output"
```

### Comparing `spine_engine-0.23.4/spine_engine/exception.py` & `spine_engine-0.24.0/spine_engine/exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/__init__.py` & `spine_engine-0.24.0/tests/project_item/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
-# Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
-# General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
-# option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+# Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
+# Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
+# any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
+
+"""
+Init file for tests.project_item package. Intentionally empty.
+
+"""
```

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/conda_kernel_spec_manager.py` & `spine_engine-0.24.0/spine_engine/execution_managers/conda_kernel_spec_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                     raise TraitError("CondaKernelSpecManager.kernelspec_path is not a directory.")
             self.log.debug("[nb_conda_kernels] Force conda_only=True as kernelspec_path is not None.")
             self.conda_only = True
 
         return new_value
 
     name_format = Unicode(
-        '{language} [conda env:{environment}]',
+        "{language} [conda env:{environment}]",
         config=True,
         help="""String name format; available field names within the string:
         '{0}' = Language
         '{1}' = Environment name
         '{conda_kernel}' = Dynamically built kernel name for conda environment
         '{display_name}' = Kernel displayed name (as defined in the kernel spec)
         '{environment}'  = Environment name (identical to '{1}')
@@ -102,23 +102,23 @@
 
     @staticmethod
     def clean_kernel_name(kname):
         """Replaces invalid characters in the Jupyter kernelname, with
         a bit of effort to preserve readability.
         """
         try:
-            kname.encode('ascii')
+            kname.encode("ascii")
         except UnicodeEncodeError:
             # Replace accented characters with unaccented equivalents
             import unicodedata
 
-            nfkd_form = unicodedata.normalize('NFKD', kname)
-            kname = u"".join([c for c in nfkd_form if not unicodedata.combining(c)])
+            nfkd_form = unicodedata.normalize("NFKD", kname)
+            kname = "".join([c for c in nfkd_form if not unicodedata.combining(c)])
         # Replace anything else, including spaces, with underscores
-        kname = re.sub(r'[^a-zA-Z0-9._\-]', '_', kname)
+        kname = re.sub(r"[^a-zA-Z0-9._\-]", "_", kname)
         return kname
 
     @property
     def _conda_info(self):
         """Get and parse the whole conda information output
 
         Caches the information for CACHE_TIMEOUT seconds, as this is
@@ -127,23 +127,23 @@
 
         expiry = self._conda_info_cache_expiry
         if expiry is None or expiry < time.time():
             self.log.debug("[nb_conda_kernels] refreshing conda info")
             # This is to make sure that subprocess can find 'conda' even if
             # it is a Windows batch file---which is the case in non-root
             # conda environments.
-            shell = self._conda_executable == 'conda' and sys.platform.startswith('win')
+            shell = self._conda_executable == "conda" and sys.platform.startswith("win")
             try:
                 # conda info --json uses the standard JSON escaping
                 # mechanism for non-ASCII characters. So it is always
                 # valid to decode here as 'ascii', since the JSON loads()
                 # method will recover any original Unicode for us.
                 p = subprocess.check_output([self._conda_executable, "info", "--json"], shell=shell).decode("ascii")
-                ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
-                result = ansi_escape.sub('', p)  # Remove ANSI Escape Sequences, such as ESC[0m
+                ansi_escape = re.compile(r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])")
+                result = ansi_escape.sub("", p)  # Remove ANSI Escape Sequences, such as ESC[0m
                 conda_info = json.loads(result)
             except Exception as err:
                 conda_info = None
                 self.log.error("Obtaining 'conda info --json' failed")
             self._conda_info_cache = conda_info
             self._conda_info_cache_expiry = time.time() + CACHE_TIMEOUT
         return self._conda_info_cache
@@ -151,49 +151,49 @@
     def _all_envs(self):
         """Find all of the environments we should be checking. We skip
         environments in the conda-bld directory as well as environments
         that match our env_filter regex. Returns a dict with canonical
         environment names as keys, and full paths as values.
         """
         conda_info = self._conda_info
-        envs = conda_info['envs']
-        base_prefix = conda_info['conda_prefix']
-        envs_prefix = join(base_prefix, 'envs')
-        build_prefix = join(base_prefix, 'conda-bld', '')
+        envs = conda_info["envs"]
+        base_prefix = conda_info["conda_prefix"]
+        envs_prefix = join(base_prefix, "envs")
+        build_prefix = join(base_prefix, "conda-bld", "")
         # Older versions of conda do not seem to include the base prefix
         # in the environment list, but we do want to scan that
         if base_prefix not in envs:
             envs.insert(0, base_prefix)
-        envs_dirs = conda_info['envs_dirs']
+        envs_dirs = conda_info["envs_dirs"]
         if not envs_dirs:
-            envs_dirs = [join(base_prefix, 'envs')]
+            envs_dirs = [join(base_prefix, "envs")]
         all_envs = {}
         for env_path in envs:
             if self.env_filter is not None:
                 if self._env_filter_regex.search(env_path):
                     continue
             if env_path == base_prefix:
-                env_name = 'root'
+                env_name = "root"
             elif env_path.startswith(build_prefix):
                 # Skip the conda-bld directory entirely
                 continue
             else:
                 env_base, env_name = split(env_path)
                 # Add a prefix to environments not found in the default
                 # environment location. The assumed convention is that a
                 # directory named 'envs' is a collection of environments
                 # as created by, say, conda or anaconda-project. The name
                 # of the parent directory, then, provides useful context.
-                if basename(env_base) == 'envs' and (env_base != envs_prefix or env_name in all_envs):
-                    env_name = u'{}-{}'.format(basename(dirname(env_base)), env_name)
+                if basename(env_base) == "envs" and (env_base != envs_prefix or env_name in all_envs):
+                    env_name = "{}-{}".format(basename(dirname(env_base)), env_name)
             # Further disambiguate, if necessary, with a counter.
             if env_name in all_envs:
                 base_name = env_name
                 for count in range(len(all_envs)):
-                    env_name = u'{}-{}'.format(base_name, count + 2)
+                    env_name = "{}-{}".format(base_name, count + 2)
                     if env_name not in all_envs:
                         break
             all_envs[env_name] = env_path
         return all_envs
 
     def _all_specs(self):
         """Find the all kernel specs in all environments.
@@ -205,86 +205,86 @@
         Caches the information for CACHE_TIMEOUT seconds, as this is
         relatively expensive.
         """
 
         all_specs = {}
         # We need to be able to find conda-run in the base conda environment
         # even if this package is not running there
-        conda_prefix = self._conda_info['conda_prefix']
+        conda_prefix = self._conda_info["conda_prefix"]
         all_envs = self._all_envs()
         for env_name, env_path in all_envs.items():
-            kspec_base = join(env_path, 'share', 'jupyter', 'kernels')
-            kspec_glob = glob.glob(join(kspec_base, '*', 'kernel.json'))
+            kspec_base = join(env_path, "share", "jupyter", "kernels")
+            kspec_glob = glob.glob(join(kspec_base, "*", "kernel.json"))
             for spec_path in kspec_glob:
                 try:
-                    with open(spec_path, 'rb') as fp:
+                    with open(spec_path, "rb") as fp:
                         data = fp.read()
-                    spec = json.loads(data.decode('utf-8'))
+                    spec = json.loads(data.decode("utf-8"))
                 except Exception as err:
                     self.log.error("[nb_conda_kernels] error loading %s:\n%s", spec_path, err)
                     continue
                 kernel_dir = dirname(spec_path).lower()
                 kernel_name = raw_kernel_name = basename(kernel_dir)
                 if self.kernelspec_path is not None and kernel_name.startswith("conda-"):
                     self.log.debug("[nb_conda_kernels] Skipping kernel spec %s", spec_path)
                     continue  # Ensure to skip dynamically added kernel spec within the environment prefix
                 # We're doing a few of these adjustments here to ensure that
                 # the naming convention is as close as possible to the previous
                 # versions of this package; particularly so that the tests
                 # pass without change.
-                if kernel_name in ('python2', 'python3'):
-                    kernel_name = 'py'
-                elif kernel_name == 'ir':
-                    kernel_name = 'r'
-                kernel_prefix = '' if env_name == 'root' else 'env-'
-                kernel_name = u'conda-{}{}-{}'.format(kernel_prefix, env_name, kernel_name)
+                if kernel_name in ("python2", "python3"):
+                    kernel_name = "py"
+                elif kernel_name == "ir":
+                    kernel_name = "r"
+                kernel_prefix = "" if env_name == "root" else "env-"
+                kernel_name = "conda-{}{}-{}".format(kernel_prefix, env_name, kernel_name)
                 # Replace invalid characters with dashes
                 kernel_name = self.clean_kernel_name(kernel_name)
 
-                display_prefix = spec['display_name']
-                if display_prefix.startswith('Python'):
-                    display_prefix = 'Python'
+                display_prefix = spec["display_name"]
+                if display_prefix.startswith("Python"):
+                    display_prefix = "Python"
                 display_name = self.name_format.format(
                     display_prefix,
                     env_name,
                     conda_kernel=kernel_name,
-                    display_name=spec['display_name'],
+                    display_name=spec["display_name"],
                     environment=env_name,
                     kernel=raw_kernel_name,
                     language=display_prefix,
                 )
                 if env_path == sys.prefix:
-                    display_name += ' *'
-                spec['display_name'] = display_name
+                    display_name += " *"
+                spec["display_name"] = display_name
                 if env_path != sys.prefix:
-                    spec['argv'] = RUNNER_COMMAND + [conda_prefix, env_path] + spec['argv']
-                metadata = spec.get('metadata', {})
-                metadata.update({'conda_env_name': env_name, 'conda_env_path': env_path})
-                spec['metadata'] = metadata
+                    spec["argv"] = RUNNER_COMMAND + [conda_prefix, env_path] + spec["argv"]
+                metadata = spec.get("metadata", {})
+                metadata.update({"conda_env_name": env_name, "conda_env_path": env_path})
+                spec["metadata"] = metadata
 
                 if self.kernelspec_path is not None:
                     # Install the kernel spec
                     try:
                         destination = self.install_kernel_spec(
                             kernel_dir, kernel_name=kernel_name, user=self._kernel_user, prefix=self._kernel_prefix
                         )
                         # Update the kernel spec
                         kernel_spec = join(destination, "kernel.json")
                         tmp_spec = spec.copy()
                         if env_path == sys.prefix:  # Add the conda runner to the installed kernel spec
-                            tmp_spec['argv'] = RUNNER_COMMAND + [conda_prefix, env_path] + spec['argv']
+                            tmp_spec["argv"] = RUNNER_COMMAND + [conda_prefix, env_path] + spec["argv"]
                         with open(kernel_spec, "w") as f:
                             json.dump(tmp_spec, f)
                     except OSError as error:
                         self.log.warning(
-                            u"[nb_conda_kernels] Fail to install kernel '{}'.".format(kernel_dir), exc_info=error
+                            "[nb_conda_kernels] Fail to install kernel '{}'.".format(kernel_dir), exc_info=error
                         )
 
                 # resource_dir is not part of the spec file, so it is added at the latest time
-                spec['resource_dir'] = abspath(kernel_dir)
+                spec["resource_dir"] = abspath(kernel_dir)
 
                 all_specs[kernel_name] = spec
 
         # Remove non-existing conda environments
         if self.kernelspec_path is not None:
             kernels_destination = self._get_destination_dir("", user=self._kernel_user, prefix=self._kernel_prefix)
             for folder in glob.glob(join(kernels_destination, "*", "kernel.json")):
@@ -359,15 +359,15 @@
         entries: "resource_dir" and "spec". This was added to fill out
         the full public interface to KernelManagerSpec.
         """
         res = {}
         for name, resource_dir in self.find_kernel_specs().items():
             try:
                 spec = self.get_kernel_spec(name)
-                res[name] = {'resource_dir': resource_dir, 'spec': spec.to_dict()}
+                res[name] = {"resource_dir": resource_dir, "spec": spec.to_dict()}
             except NoSuchKernel:
                 self.log.warning("Error loading kernelspec %r", name, exc_info=True)
         return res
 
     def remove_kernel_spec(self, name):
         """Remove a kernel spec directory by name.
```

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/conda_kernel_spec_runner.py` & `spine_engine-0.24.0/spine_engine/execution_managers/conda_kernel_spec_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,47 +14,47 @@
     from pipes import quote
 
 
 def exec_in_env(conda_prefix, env_path, *command):
     # Run the standard conda activation script, and print the
     # resulting environment variables to stdout for reading.
     is_current_env = env_path == sys.prefix
-    if sys.platform.startswith('win'):
+    if sys.platform.startswith("win"):
         if is_current_env:
             subprocess.Popen(list(command)).wait()
         else:
-            activate = os.path.join(conda_prefix, 'Scripts', 'activate.bat')
+            activate = os.path.join(conda_prefix, "Scripts", "activate.bat")
             ecomm = [
-                os.environ['COMSPEC'],
-                '/S',
-                '/U',
-                '/C',
-                '@echo',
-                'off',
-                '&&',
-                'chcp',
-                '65001',
-                '&&',
-                'call',
+                os.environ["COMSPEC"],
+                "/S",
+                "/U",
+                "/C",
+                "@echo",
+                "off",
+                "&&",
+                "chcp",
+                "65001",
+                "&&",
+                "call",
                 activate,
                 env_path,
-                '&&',
-                '@echo',
-                'CONDA_PREFIX=%CONDA_PREFIX%',
-                '&&',
+                "&&",
+                "@echo",
+                "CONDA_PREFIX=%CONDA_PREFIX%",
+                "&&",
             ] + list(command)
             subprocess.Popen(ecomm).wait()
     else:
         quoted_command = [quote(c) for c in command]
         if is_current_env:
             os.execvp(quoted_command[0], quoted_command)
         else:
-            activate = os.path.join(conda_prefix, 'bin', 'activate')
+            activate = os.path.join(conda_prefix, "bin", "activate")
             ecomm = ". '{}' '{}' && echo CONDA_PREFIX=$CONDA_PREFIX && exec {}".format(
-                activate, env_path, ' '.join(quoted_command)
+                activate, env_path, " ".join(quoted_command)
             )
-            ecomm = ['sh' if 'bsd' in sys.platform else 'bash', '-c', ecomm]
+            ecomm = ["sh" if "bsd" in sys.platform else "bash", "-c", ecomm]
             os.execvp(ecomm[0], ecomm)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     exec_in_env(*(sys.argv[1:]))
```

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/execution_manager_base.py` & `spine_engine-0.24.0/spine_engine/execution_managers/execution_manager_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/kernel_execution_manager.py` & `spine_engine-0.24.0/spine_engine/execution_managers/kernel_execution_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -83,16 +84,15 @@
         """Creates a new kernel manager for given kernel and group id if none exists.
         Starts the kernel if not started, and returns it.
 
         Args:
             kernel_name (str): The kernel
             group_id (str): Item group that will execute using this kernel
             logger (LoggerInterface): For logging
-            extra_switches (list, optional): List of additional switches to julia or python.
-                These come before the 'programfile'.
+            extra_switches (list, optional): List of additional switches for the kernel (i.e. Julia or Python)
             environment (str): "conda" to launch a Conda kernel spec. "" for a regular kernel spec
             `**kwargs`: optional. Keyword arguments passed to ``KernelManager.start_kernel()``
 
         Returns:
             KernelManager
         """
         server_ip = kwargs.pop("server_ip", "")
@@ -258,41 +258,40 @@
 
 
 class KernelExecutionManager(ExecutionManagerBase):
     def __init__(
         self,
         logger,
         kernel_name,
-        *commands,
+        commands,
         kill_completed=False,
         group_id=None,
         startup_timeout=60,
-        extra_switches=None,
         environment="",
+        extra_switches=None,
         **kwargs,
     ):
         """
         Args:
-            logger (LoggerInterface): For logging
-            kernel_name (str): The Kernel
-            *commands: Commands to execute in the kernel
+            logger (LoggerInterface): Logger instance
+            kernel_name (str): Kernel name
+            commands (list): Commands to execute in the kernel
             kill_completed (bool): Whether to kill completed persistent processes
             group_id (str, optional): Item group that will execute using this kernel
             startup_timeout (int, optional): How much to wait for the kernel, used in ``KernelClient.wait_for_ready()``
-            extra_switches (list, optional): List of additional switches to launch julia.
-                These come before the 'programfile'.
             environment (str): "conda" to launch a Conda kernel spec. "" for a regular kernel spec.
+            extra_switches (list, optional): List of additional switches for the kernel (i.e. Julia or Python)
             **kwargs (optional): Keyword arguments passed to ``KernelManager.start_kernel()``
         """
         super().__init__(logger)
         self._msg_head = dict(kernel_name=kernel_name)
         self._commands = commands
         self._cmd_failed = False
-        self.std_out = kwargs["stdout"] = open(os.devnull, 'w')
-        self.std_err = kwargs["stderr"] = open(os.devnull, 'w')
+        self.std_out = kwargs["stdout"] = open(os.devnull, "w")
+        self.std_err = kwargs["stderr"] = open(os.devnull, "w")
         # Don't show console when frozen
         kwargs["creationflags"] = subprocess.CREATE_NO_WINDOW if sys.platform == "win32" else 0
         self._kernel_manager = _kernel_manager_factory.new_kernel_manager(
             kernel_name, group_id, logger, extra_switches=extra_switches, environment=environment, **kwargs
         )
         self._kernel_client = self._kernel_manager.client() if self._kernel_manager is not None else None
         self._startup_timeout = startup_timeout
```

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/persistent_execution_manager.py` & `spine_engine-0.24.0/spine_engine/execution_managers/persistent_execution_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -141,23 +142,29 @@
         self.command_successful = False
         self._persistent = Popen(self._args + self._init_args(), **self._kwargs)
         threading.Thread(target=self._log_stdout, daemon=True).start()
         threading.Thread(target=self._log_stderr, daemon=True).start()
 
     def _log_stdout(self):
         """Puts stdout from the process into the queue (it will be consumed by issue_command())."""
-        for line in iter(self._persistent.stdout.readline, b''):
-            data = line.decode("UTF8", "replace").rstrip()
-            self._msg_queue.put(dict(type="stdout", data=data))
+        try:
+            for line in iter(self._persistent.stdout.readline, b""):
+                data = line.decode("UTF8", "replace").rstrip()
+                self._msg_queue.put(dict(type="stdout", data=data))
+        except ValueError:
+            pass
 
     def _log_stderr(self):
         """Puts stderr from the process into the queue (it will be consumed by issue_command())."""
-        for line in iter(self._persistent.stderr.readline, b''):
-            data = line.decode("UTF8", "replace").rstrip()
-            self._msg_queue.put(dict(type="stderr", data=data))
+        try:
+            for line in iter(self._persistent.stderr.readline, b""):
+                data = line.decode("UTF8", "replace").rstrip()
+                self._msg_queue.put(dict(type="stderr", data=data))
+        except ValueError:
+            pass
 
     def make_complete_command(self, cmd):
         lines = cmd.splitlines()
         cmd = os.linesep.join(lines)
         if len(lines) == 1:
             cmd += os.linesep
         try:
@@ -326,16 +333,16 @@
             receive (bool, optional): If True (the default) also receives the response and returns it.
 
         Returns:
             str or NoneType: response, or None if the ``receive`` argument is False
         """
         if not self.is_persistent_alive():
             raise PersistentIsDead()
-        req_args_sep = '\u001f'  # Unit separator
-        args_sep = '\u0091'  # Private Use 1
+        req_args_sep = "\u001f"  # Unit separator
+        args_sep = "\u0091"  # Private Use 1
         args = args_sep.join(args)
         msg = f"{request}{req_args_sep}{args}"
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             while True:
                 try:
                     s.connect(self._server_address)
                     break
@@ -562,15 +569,15 @@
     def new_persistent_manager(self, constructor, logger, args, group_id):
         """Creates a new persistent manager.
 
         Args:
             constructor (Callable): the persistent manager constructor
             logger (LoggerInterface)
             args (list): the arguments to launch the persistent process
-            group_id (str): item group that will execute using this persistent
+            group_id (str): Item group for sharing this persistent process
 
         Returns:
             PersistentManagerBase: persistent manager or None if factory has been closed
         """
         while not persistent_process_semaphore.acquire(timeout=0.5):
             if not self._factory_open:
                 return None
@@ -777,20 +784,20 @@
 
 class PersistentExecutionManagerBase(ExecutionManagerBase):
     """Base class for managing execution of commands on a persistent process."""
 
     def __init__(self, logger, args, commands, alias, kill_completed_processes, group_id=None):
         """
         Args:
-            logger (LoggerInterface): a logger instance
-            args (list): List of args to start the persistent process
-            commands (list): List of commands to execute in the persistent process
-            alias (str): an alias name for the manager
-            kill_completed_processes (bool): if True, the persistent process will be killed after execution
-            group_id (str, optional): item group that will execute using this kernel
+            logger (LoggerInterface): Logger instance
+            args (list): Program and cmd line args for the persistent process
+            commands (list): List of commands to execute in the persistent process (including the script cmd line args)
+            alias (str): Alias name for the manager
+            kill_completed_processes (bool): If True, the persistent process will be killed after execution
+            group_id (str, optional): Item group for sharing this persistent process
         """
         super().__init__(logger)
         self._args = args
         self._commands = commands
         self._alias = alias
         self._persistent_manager = _persistent_manager_factory.new_persistent_manager(
             self.persistent_manager_factory, logger, args, group_id
```

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/process_execution_manager.py` & `spine_engine-0.24.0/spine_engine/execution_managers/process_execution_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -18,21 +19,22 @@
 import subprocess
 from threading import Thread
 from .execution_manager_base import ExecutionManagerBase
 from ..utils.execution_resources import one_shot_process_semaphore
 
 
 class ProcessExecutionManager(ExecutionManagerBase):
-    def __init__(self, logger, program, *args, workdir=None):
+    def __init__(self, logger, program, args, workdir=None):
         """Class constructor.
 
         Args:
-            logger (LoggerInterface): a logger instance
-            program (str): Path to program to run in the subprocess (e.g. julia.exe)
-            *args: List of arguments for the program (e.g. path to script file)
+            logger (LoggerInterface): Logger instance
+            program (str): Path to program to run in the subprocess (e.g. 'path/to/julia')
+            args (list): List of arguments for the program (e.g. path to script file)
+            workdir (str): Work directory for the subprocess.Popen process
         """
         super().__init__(logger)
         self._process = None
         self._program = program
         self._args = args
         self._workdir = workdir
         self._stopped = False
@@ -41,43 +43,43 @@
         self._stopped = False
         cf = subprocess.CREATE_NO_WINDOW if sys.platform == "win32" else 0  # Don't show console when frozen
         with one_shot_process_semaphore:
             if self._stopped:
                 return 0
             try:
                 self._process = subprocess.Popen(
-                    [self._program, *self._args],
+                    [self._program] + self._args,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     cwd=self._workdir,
                     creationflags=cf,
                 )
             except OSError as e:
                 msg = dict(type="execution_failed_to_start", error=str(e), program=self._program)
                 self._logger.msg_standard_execution.emit(msg)
                 return 1
             msg = dict(type="execution_started", program=self._program, args=" ".join(self._args))
             self._logger.msg_standard_execution.emit(msg)
-            running = "# Running" + " ".join([self._program, *self._args])
+            running = "# Running" + " ".join([self._program] + self._args)
             self._logger.msg_standard_execution.emit({"type": "stdin", "data": running})
             Thread(target=self._log_stdout, args=(self._process.stdout,), daemon=True).start()
             Thread(target=self._log_stderr, args=(self._process.stderr,), daemon=True).start()
             return self._process.wait()
 
     def stop_execution(self):
         self._stopped = True
         if self._process is not None:
             self._process.terminate()
 
     def _log_stdout(self, stdout):
-        for line in iter(stdout.readline, b''):
+        for line in iter(stdout.readline, b""):
             line = line.decode("UTF8", "replace").strip()
             self._logger.msg_proc.emit(line)
             self._logger.msg_standard_execution.emit({"type": "stdout", "data": line})
         stdout.close()
 
     def _log_stderr(self, stderr):
-        for line in iter(stderr.readline, b''):
+        for line in iter(stderr.readline, b""):
             line = line.decode("UTF8", "replace").strip()
             self._logger.msg_proc_error.emit(line)
             self._logger.msg_standard_execution.emit({"type": "stderr", "data": line})
         stderr.close()
```

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/spine_repl.jl` & `spine_engine-0.24.0/spine_engine/execution_managers/spine_repl.jl`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/spine_engine/execution_managers/spine_repl.py` & `spine_engine-0.24.0/spine_engine/execution_managers/spine_repl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -27,16 +28,16 @@
 class SpineDBServer(socketserver.ThreadingMixIn, socketserver.TCPServer):
     allow_reuse_address = True
 
 
 class _RequestHandler(socketserver.BaseRequestHandler):
     def handle(self):
         data = self.request.recv(1024).decode("UTF8")
-        req_args_sep = '\u001f'  # Unit separator
-        args_sep = '\u0091'  # Private Use 1
+        req_args_sep = "\u001f"  # Unit separator
+        args_sep = "\u0091"  # Private Use 1
         request, args = data.split(req_args_sep)
         args = args.split(args_sep)
         handler = {
             "completions": completions,
             "add_history": add_history,
             "history_item": history_item,
             "is_complete": is_complete,
```

### Comparing `spine_engine-0.23.4/spine_engine/load_project_items.py` & `spine_engine-0.24.0/spine_engine/load_project_items.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,41 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-
-"""
-Functions to load project item modules.
-
-"""
-import pathlib
+""" Functions to load project item modules. """
 import importlib
-import importlib.util
 
 
 def load_item_specification_factories(items_package_name):
     """
     Loads the project item specification factories in given project item package.
 
     Args:
         items_package_name (str): name of the package that contains the project items
 
     Returns:
         dict: a map from item type to specification factory
     """
     items = importlib.import_module(items_package_name)
-    items_root = pathlib.Path(items.__file__).parent
-    factories = dict()
-    for child in items_root.iterdir():
-        if child.is_dir() and (
-            child.joinpath("specification_factory.py").exists()
-            or child.is_dir()
-            and child.joinpath("specification_factory.pyc").exists()
-        ):
-            spec = importlib.util.find_spec(f"{items_package_name}.{child.stem}.specification_factory")
-            m = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(m)
-            if hasattr(m, "SpecificationFactory"):
-                item_type = m.SpecificationFactory.item_type()
-                factories[item_type] = m.SpecificationFactory
-    return factories
+    return items.item_specification_factories()
 
 
 def load_executable_item_classes(items_package_name):
     """
     Loads the project item executable classes included in given project item package.
 
     Args:
         items_package_name (str): name of the package that contains the project items
 
     Returns:
         dict: a map from item type to the executable item class
     """
     items = importlib.import_module(items_package_name)
-    items_root = pathlib.Path(items.__file__).parent
-    classes = dict()
-    for child in items_root.iterdir():
-        if (
-            child.is_dir()
-            and child.joinpath("executable_item.py").exists()
-            or (child.is_dir() and child.joinpath("executable_item.pyc").exists())
-        ):
-            spec = importlib.util.find_spec(f"{items_package_name}.{child.stem}.executable_item")
-            m = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(m)
-            if hasattr(m, "ExecutableItem"):
-                item_class = m.ExecutableItem
-                item_type = item_class.item_type()
-                classes[item_type] = item_class
-    return classes
+    return items.executable_items()
```

### Comparing `spine_engine-0.23.4/spine_engine/multithread_executor/__init__.py` & `spine_engine-0.24.0/spine_engine/execution_managers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/multithread_executor/multithread.py` & `spine_engine-0.24.0/spine_engine/jumpster.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,318 +1,396 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-
 """
-Module contains MultithreadExecutor.
-
+In-house dagster replacement that also handles jumps.
 """
-
-import os
 import sys
-from dagster import check
-from dagster.core.execution.api import (
-    create_execution_plan,
-    inner_plan_execution_iterator,
-    ExecuteRunWithPlanIterable,
-    PlanExecutionContextManager,
-)
-from dagster.core.executor.base import Executor
-from dagster.core.execution.retries import RetryMode
-from dagster.core.execution.context.system import PlanOrchestrationContext
-from dagster.core.execution.plan.objects import StepFailureData
-from dagster.core.execution.plan.plan import ExecutionPlan
-from dagster.core.events import DagsterEvent, EngineEventData
-from dagster.core.errors import DagsterError
-from dagster.utils.timing import format_duration, time_execution_scope
-from dagster.utils.error import serializable_error_info_from_exc_info
-from .thread_executor import ThreadCrashException, ThreadEvent, ThreadSystemErrorEvent, execute_thread_command
-from ..spine_engine import ED
+import threading
+import queue
+from enum import Enum, unique
+from collections import namedtuple
+from .utils.helpers import serializable_error_info_from_exc_info, ExecutionDirection as ED
+
+
+@unique
+class JumpsterEventType(Enum):
+    STEP_START = 1
+    STEP_FAILURE = 2
+    STEP_FINISH = 3
+    OUTPUT_AVAILABLE = 4
+
+
+class PipelineDefinition:
+    def __init__(self, solid_defs, jumps):
+        self.solid_defs = solid_defs
+        self.jumps = jumps
+
+
+class DefinitionBase:
+    def __init__(self, item_name, direction):
+        self.item_name = item_name
+        self.direction = direction
+
+    @property
+    def key(self):
+        return (self.item_name, self.direction)
+
+
+class SolidDefinition(DefinitionBase):
+    def __init__(self, item_name, direction, input_defs, compute_fn):
+        super().__init__(item_name, direction)
+        self.input_defs = input_defs
+        self.compute_fn = compute_fn
+
+
+class InputDefinition(DefinitionBase):
+    pass
+
+
+class JumpsterEvent(DefinitionBase):
+    def __init__(self, event_type, item_name, direction, **kwargs):
+        super().__init__(item_name, direction)
+        self.event_type = event_type
+        for (key, value) in kwargs.items():
+            setattr(self, key, value)
+
+
+class Failure(BaseException):
+    """A failure"""
 
-DELEGATE_MARKER = "multithread_thread_init"
 
+class Output:
+    def __init__(self, value):
+        self.value = value
 
-class DagsterThreadError(DagsterError):
-    """An exception has occurred in one or more of the threads dagster manages.
+
+class Finalization:
+    def __init__(self, item_finish_state):
+        self.item_finish_state = item_finish_state
+
+
+class JumpsterThreadError(Exception):
+    """An exception has occurred in one or more of the threads jumpster manages.
     This error forwards the message and stack trace for all of the collected errors.
     """
 
     def __init__(self, *args, **kwargs):
-        from dagster.utils.error import SerializableErrorInfo
+        super().__init__()
+        self.thread_error_infos = kwargs.pop("thread_error_infos")
 
-        self.thread_error_infos = check.list_param(
-            kwargs.pop("thread_error_infos"), "thread_error_infos", SerializableErrorInfo
-        )
-        super(DagsterThreadError, self).__init__(*args, **kwargs)
 
+class MultithreadExecutor:
+    def __init__(self, pipeline_def, max_concurrent=None):
+        self._pipeline_def = pipeline_def
+        self._max_concurrent = max_concurrent if max_concurrent else 100  # TODO: How to determine a good amount?
+        self._output_value = {}
+        self._ready_to_execute = {}
+        self._in_flight = set()
+        self._steps_by_input_key = {}
+        for solid_def in self._pipeline_def.solid_defs:
+            step = Step(solid_def)
+            if step.is_ready_to_execute():
+                self._ready_to_execute[step.key] = step
+            else:
+                for input_def in solid_def.input_defs:
+                    self._steps_by_input_key.setdefault(input_def.key, []).append(step)
 
-class MultithreadExecutor(Executor):
-    def __init__(self, retries, max_concurrent=None):
-        self._retries = check.inst_param(retries, "retries", RetryMode)
-        max_concurrent = max_concurrent if max_concurrent else 100  # TODO: How to determine a good amount?
-        self.max_concurrent = check.int_param(max_concurrent, "max_concurrent")
-        self._forward_resources = {}
-        self._backward_resources = {}
+    def _is_complete(self):
+        return not self._in_flight and not self._ready_to_execute
 
-    @property
-    def retries(self):
-        return self._retries
+    def _get_steps_to_execute(self, limit):
+        steps = []
+        while self._ready_to_execute and len(steps) < limit:
+            key, step = self._ready_to_execute.popitem()
+            self._in_flight.add(key)
+            steps.append(step)
+        return steps
+
+    def _handle_event(self, event):
+        if event.event_type in (JumpsterEventType.STEP_FINISH, JumpsterEventType.STEP_FAILURE):
+            self._in_flight.discard(event.key)
+        elif event.event_type == JumpsterEventType.OUTPUT_AVAILABLE:
+            self._output_value[event.key] = event.output_value
+            steps = self._steps_by_input_key.get(event.key, ())
+            for step in steps:
+                step.inputs[event.key] = event.output_value
+                if step.is_ready_to_execute():
+                    self._ready_to_execute[step.key] = step
 
-    def execute(self, pipeline_context, execution_plan):
-        check.inst_param(pipeline_context, "pipeline_context", PlanOrchestrationContext)
-        check.inst_param(execution_plan, "execution_plan", ExecutionPlan)
-
-        limit = self.max_concurrent
-
-        yield DagsterEvent.engine_event(
-            pipeline_context,
-            "Executing steps using multithread executor (pid: {pid})".format(pid=os.getpid()),
-            event_specific_data=EngineEventData.in_process(os.getpid(), execution_plan.step_keys_to_execute),
-        )
-
-        with time_execution_scope() as timer_result:
-            with execution_plan.start(retry_mode=self.retries) as active_execution:
-                active_iters = {}
-                errors = {}
-                waiting = {}
-                iterating = {}
-                iterating_active = set()
-                iterating_failed = set()
-                jumps = pipeline_context.pipeline.get_definition().jumps
-                jump_by_source = {}
-                jump_by_solid_name = {}
-                for jump in jumps:
-                    jump_by_source[jump.source_solid] = jump
-                    non_nested_solid_names = set(jump.solid_names)
-                    for other_jump in jumps:
-                        if jump is other_jump:
+    def execute(self):
+        active_iters = {}
+        errors = {}
+        waiting = {}
+        iterating = {}
+        iterating_active = set()
+        iterating_failed = set()
+        jumps = self._pipeline_def.jumps
+        jump_by_source = {}
+        jump_by_item_name = {}
+        for jump in jumps:
+            jump_by_source[jump.source] = jump
+            non_nested_item_names = set(jump.item_names)
+            for other_jump in jumps:
+                if jump is other_jump:
+                    continue
+                if other_jump.item_names > jump.item_names:
+                    continue
+                non_nested_item_names -= other_jump.item_names
+            for item_name in non_nested_item_names:
+                jump_by_item_name[item_name] = jump
+        unfinished_jumps = set(jumps)
+        loop_iteration_counters = {}
+        step_by_key = {}
+        while not self._is_complete() or active_iters:
+            # start iterators
+            while len(active_iters) < self._max_concurrent:
+                candidate_steps = self._get_steps_to_execute(limit=(self._max_concurrent - len(active_iters)))
+                step_by_key.update({step.key: step for step in candidate_steps})
+                # Add all waiting steps
+                candidate_steps += list(waiting.values())
+                # Add iterating steps that don't depend on other pending iterating
+                iterating_skipped = set()
+                for key, step in iterating.items():
+                    dependency_keys = step.get_execution_dependency_keys()
+                    if dependency_keys & (iterating_active | iterating_skipped | iterating_failed):
+                        iterating_skipped.add(key)
+                        continue
+                    iterating_active.add(key)
+                    candidate_steps.append(step)
+                executable_steps = []
+                for step in candidate_steps:
+                    if step.direction == ED.BACKWARD:
+                        executable_steps.append(step)
+                        continue
+                    # Check if the step depends on any jumps that don't contain it
+                    predecessor_jumps = (jump for jump in unfinished_jumps if step.item_name not in jump.item_names)
+                    predecessor_item_names = {item for jump in predecessor_jumps for item in jump.item_names}
+                    predecessor_keys = {
+                        k
+                        for k, s in step_by_key.items()
+                        if s.direction == ED.FORWARD and s.item_name in predecessor_item_names
+                    }
+                    dependency_keys = step.get_execution_dependency_keys()
+                    if dependency_keys & predecessor_keys:
+                        if step.key not in iterating:
+                            waiting[step.key] = step
+                        continue
+                    waiting.pop(step.key, None)
+                    iterating.pop(step.key, None)
+                    executable_steps.append(step)
+                if not executable_steps:
+                    break
+                for step in executable_steps:
+                    active_iters[step.key] = execute_step_in_thread(step, errors)
+            # process active iterators
+            empty_iters = []
+            for key, step_iter in active_iters.items():
+                try:
+                    event_or_none = next(step_iter)
+                    if event_or_none is None:
+                        continue
+                    yield event_or_none
+                    self._handle_event(event_or_none)
+                    step = step_by_key[key]
+                    if step.direction == ED.BACKWARD:
+                        continue
+                    # Handle loops
+                    if event_or_none.event_type == JumpsterEventType.STEP_FAILURE:
+                        # Mark failed loops as finished
+                        iterating_active.discard(key)
+                        failed_jump = jump_by_item_name.get(step.item_name)
+                        if failed_jump is None:
                             continue
-                        if other_jump.solid_names > jump.solid_names:
+                        failed_item_names = failed_jump.item_names
+                        for jump in jumps:
+                            if jump.item_names & failed_item_names:
+                                unfinished_jumps.discard(jump)
+                                loop_iteration_counters.pop(jump, None)
+                        iterating_failed.add(step)
+                    elif event_or_none.event_type == JumpsterEventType.STEP_FINISH:
+                        # Process loop condition
+                        iterating_active.discard(key)
+                        jump = jump_by_source.get(step.item_name)
+                        if jump is None:
                             continue
-                        non_nested_solid_names -= other_jump.solid_names
-                    for solid_name in non_nested_solid_names:
-                        jump_by_solid_name[solid_name] = jump
-                unfinished_jumps = set(jumps)
-                loop_iteration_counters = {}
-                steps_by_key = {}
-                while not active_execution.is_complete or active_iters:
-                    # start iterators
-                    while len(active_iters) < limit:
-                        candidate_steps = active_execution.get_steps_to_execute(limit=(limit - len(active_iters)))
-                        steps_by_key.update({step.key: step for step in candidate_steps})
-                        # Add all waiting steps
-                        candidate_steps += list(waiting.values())
-                        # Add iterating steps that don't depend on other pending iterating
-                        iterating_skipped = set()
-                        for key, step in iterating.items():
-                            dependency_keys = step.get_execution_dependency_keys()
-                            if dependency_keys & (iterating_active | iterating_skipped | iterating_failed):
-                                iterating_skipped.add(key)
-                                continue
-                            iterating_active.add(key)
-                            candidate_steps.append(step)
-
-                        executable_steps = []
-                        for step in candidate_steps:
-                            # Check if the step depends on any jumps that don't contain it
-                            predecessor_jumps = (
-                                jump for jump in unfinished_jumps if step.solid_name not in jump.solid_names
-                            )
-                            predecessor_solid_names = {item for jump in predecessor_jumps for item in jump.solid_names}
-                            predecessor_keys = {
-                                key for key, step in steps_by_key.items() if step.solid_name in predecessor_solid_names
-                            }
-                            dependency_keys = step.get_execution_dependency_keys()
-                            if dependency_keys & predecessor_keys:
-                                if step.key not in iterating:
-                                    waiting[step.key] = step
-                                continue
-                            waiting.pop(step.key, None)
-                            iterating.pop(step.key, None)
-                            executable_steps.append(step)
-
-                        if not executable_steps:
-                            break
-
-                        for step in executable_steps:
-                            step_context = pipeline_context.for_step(step)
-                            active_iters[step.key] = self.execute_step_in_thread(
-                                pipeline_context.pipeline,
-                                step.key,
-                                step.solid_name,
-                                step_context,
-                                errors,
-                                active_execution.get_known_state(),
-                            )
-                    # process active iterators
-                    empty_iters = []
-                    for key, step_iter in active_iters.items():
-                        try:
-                            event_or_none = next(step_iter)
-                            if event_or_none is None:
-                                continue
-                            yield event_or_none
-                            try:
-                                active_execution.handle_event(event_or_none)
-                            except check.CheckError:
-                                # Bypass check errors on iterating steps
-                                if key in iterating_active:
-                                    pass
-                                else:
-                                    raise
-                            # Handle loops
-                            if event_or_none.is_step_failure:
-                                # Mark failed loops as finished
-                                iterating_active.discard(key)
-                                step = steps_by_key[key]
-                                failed_jump = jump_by_solid_name.get(step.solid_name)
-                                if failed_jump is None:
-                                    continue
-                                failed_solid_names = failed_jump.solid_names
-                                for jump in jumps:
-                                    if jump.solid_names & failed_solid_names:
-                                        unfinished_jumps.discard(jump)
-                                        loop_iteration_counters.pop(jump, None)
-                                iterating_failed.add(step)
-                            elif event_or_none.is_step_success:
-                                # Process loop condition
-                                iterating_active.discard(key)
-                                step = steps_by_key[key]
-                                jump = jump_by_source.get(step.solid_name)
-                                if jump is None:
-                                    continue
-                                forward_resources = self._forward_resources.get(jump.source_solid, [])
-                                backward_resources = self._backward_resources.get(jump.destination_solid, [])
-                                jump.receive_resources_from_source(forward_resources)
-                                jump.receive_resources_from_destination(backward_resources)
-                                iteration_counter = loop_iteration_counters.setdefault(jump, 1)
-                                if jump.is_condition_true(iteration_counter):
-                                    # Put all jump steps in the iterating bucket
-                                    for k, s in steps_by_key.items():
-                                        if s.solid_name in jump.solid_names:
-                                            iterating[k] = s
-                                    # Mark all nested jumps unfinished again
-                                    for solid_name in jump.solid_names:
-                                        nested_jump = jump_by_solid_name.get(solid_name)
-                                        if nested_jump is not None:
-                                            unfinished_jumps.add(nested_jump)
-
-                                    loop_iteration_counters[jump] += 1
-                                else:
-                                    unfinished_jumps.remove(jump)
-                                    del loop_iteration_counters[jump]
-
-                        except ThreadCrashException:
-                            serializable_error = serializable_error_info_from_exc_info(sys.exc_info())
-                            yield DagsterEvent.engine_event(
-                                pipeline_context,
-                                f"Multithread executor: thread for step {key} exited unexpectedly",
-                                EngineEventData.engine_error(serializable_error),
-                            )
-                            step_failure_event = DagsterEvent.step_failure_event(
-                                step_context=pipeline_context.for_step(active_execution.get_step_by_key(key)),
-                                step_failure_data=StepFailureData(error=serializable_error, user_failure_data=None),
-                            )
-                            active_execution.handle_event(step_failure_event)
-                            yield step_failure_event
-                            empty_iters.append(key)
-                        except StopIteration:
-                            empty_iters.append(key)
-                            # TODO: Anything about loops?
-                    # clear and mark complete finished iterators
-                    for key in empty_iters:
-                        del active_iters[key]
-                        active_execution.verify_complete(pipeline_context, key)
-
-                    # process skipped and abandoned steps
-                    for event in active_execution.plan_events_iterator(pipeline_context):
-                        yield event
-
-                errs = {tid: err for tid, err in errors.items() if err}
-                if errs:
-                    raise DagsterThreadError(
-                        "During multithread execution errors occurred in threads:\n{error_list}".format(
-                            error_list="\n".join(
-                                [
-                                    "In thread {tid}: {err}".format(tid=tid, err=err.to_string())
-                                    for tid, err in errs.items()
-                                ]
-                            )
-                        ),
-                        thread_error_infos=list(errs.values()),
+                        forward_resources = [
+                            r for stack in self._output_value.get((jump.source, ED.FORWARD), []) for r in stack
+                        ]
+                        backward_resources = self._output_value.get((jump.destination, ED.BACKWARD), [])
+                        jump.receive_resources_from_source(forward_resources)
+                        jump.receive_resources_from_destination(backward_resources)
+                        iteration_counter = loop_iteration_counters.setdefault(jump, 1)
+                        if jump.is_condition_true(iteration_counter):
+                            # Put all jump steps in the iterating bucket
+                            for k, s in step_by_key.items():
+                                if s.direction == ED.FORWARD and s.item_name in jump.item_names:
+                                    iterating[k] = s
+                            # Mark all nested jumps unfinished again
+                            for item_name in jump.item_names:
+                                nested_jump = jump_by_item_name.get(item_name)
+                                if nested_jump is not None:
+                                    unfinished_jumps.add(nested_jump)
+                            loop_iteration_counters[jump] += 1
+                        else:
+                            unfinished_jumps.remove(jump)
+                            del loop_iteration_counters[jump]
+                except ThreadCrashException:
+                    serializable_error = serializable_error_info_from_exc_info(sys.exc_info())
+                    step_failure_event = JumpsterEvent(JumpsterEventType.STEP_FAILURE, *key, error=serializable_error)
+                    self._handle_event(step_failure_event)
+                    yield step_failure_event
+                    empty_iters.append(key)
+                except StopIteration:
+                    empty_iters.append(key)
+                    # TODO: Anything about loops?
+            # clear and mark complete finished iterators
+            for key in empty_iters:
+                del active_iters[key]
+        errs = {tid: err for tid, err in errors.items() if err}
+        if errs:
+            raise JumpsterThreadError(
+                "During multithread execution errors occurred in threads:\n{error_list}".format(
+                    error_list="\n".join(
+                        ["In thread {tid}: {err}".format(tid=tid, err=err.to_string()) for tid, err in errs.items()]
                     )
+                ),
+                thread_error_infos=list(errs.values()),
+            )
 
-        yield DagsterEvent.engine_event(
-            pipeline_context,
-            "Multithread executor: parent process exiting after {duration} (pid: {pid})".format(
-                duration=format_duration(timer_result.millis), pid=os.getpid()
-            ),
-            event_specific_data=EngineEventData.multiprocess(os.getpid()),
-        )
 
-    def execute_step_in_thread(self, pipeline, step_key, solid_name, step_context, errors, known_state):
-        yield DagsterEvent.engine_event(
-            step_context, f"Spawning thread for {step_key}", EngineEventData(marker_start=DELEGATE_MARKER)
-        )
+class Step:
+    def __init__(self, solid_def):
+        self._solid_def = solid_def
+        self.inputs = {}
+        self._ready_once = False
 
-        command = ThreadExecutorChildThreadCommand(
-            step_context.run_config,
-            step_context.pipeline_run,
-            step_key,
-            step_context.instance,
-            pipeline,
-            self.retries,
-            known_state,
-        )
-        for ret in execute_thread_command(command):
-            if ret is None or isinstance(ret, DagsterEvent):
-                self._save_resources(command, solid_name)
-                yield ret
-            elif isinstance(ret, ThreadEvent):
-                if isinstance(ret, ThreadSystemErrorEvent):
-                    errors[ret.tid] = ret.error_info
-            else:
-                check.failed("Unexpected return value from thread {}".format(type(ret)))
+    @property
+    def item_name(self):
+        return self._solid_def.item_name
 
-    def _save_resources(self, command, solid_name):
-        for output_handle, outputs in command.output_capture.items():
-            if output_handle.output_name == f"{ED.BACKWARD}_output":
-                self._backward_resources[solid_name] = outputs
-            elif output_handle.output_name == f"{ED.FORWARD}_output":
-                self._forward_resources[solid_name] = [r for stack in outputs for r in stack]
-
-
-class ThreadExecutorChildThreadCommand:
-    def __init__(self, run_config, pipeline_run, step_key, instance, pipeline, retry_mode, known_state):
-        self.output_capture = {}
-        self._execution_plan = create_execution_plan(
-            pipeline=pipeline,
-            run_config=run_config,
-            mode=pipeline_run.mode,
-            step_keys_to_execute=[step_key],
-            known_state=known_state,
-        )
-        self._execution_context_manager = PlanExecutionContextManager(
-            pipeline=pipeline,
-            retry_mode=retry_mode,
-            execution_plan=self._execution_plan,
-            run_config=run_config,
-            pipeline_run=pipeline_run,
-            instance=instance,
-            output_capture=self.output_capture,
-        )
+    @property
+    def direction(self):
+        return self._solid_def.direction
+
+    @property
+    def key(self):
+        return self._solid_def.key
+
+    def is_ready_to_execute(self):
+        if self._ready_once:
+            return False
+        self._ready_once = len(self._solid_def.input_defs) == len(self.inputs)
+        return self._ready_once
 
     def execute(self):
-        return iter(
-            ExecuteRunWithPlanIterable(
-                execution_plan=self._execution_plan,
-                iterator=inner_plan_execution_iterator,
-                execution_context_manager=self._execution_context_manager,
-            )
+        inputs = {}
+        for input_def in self._solid_def.input_defs:
+            inputs.setdefault(input_def.direction, []).extend(self.inputs[input_def.key])
+        yield JumpsterEvent(JumpsterEventType.STEP_START, *self.key)
+        try:
+            for x in self._solid_def.compute_fn(inputs):
+                if isinstance(x, Output):
+                    yield JumpsterEvent(JumpsterEventType.OUTPUT_AVAILABLE, *self.key, output_value=x.value)
+                elif isinstance(x, Finalization):
+                    yield JumpsterEvent(JumpsterEventType.STEP_FINISH, *self.key, item_finish_state=x.item_finish_state)
+        except Exception as err:  # pylint: disable=broad-except
+            yield JumpsterEvent(JumpsterEventType.STEP_FAILURE, *self.key, error=err)
+
+    def get_execution_dependency_keys(self):
+        return set(input_def.key for input_def in self._solid_def.input_defs)
+
+
+def execute_pipeline_iterator(pipeline_def):
+    yield from MultithreadExecutor(pipeline_def).execute()
+
+
+# Thread execution stuff
+class ThreadDoneEvent(namedtuple("ThreadDoneEvent", "tid")):
+    pass
+
+
+class ThreadSystemErrorEvent(namedtuple("ThreadSystemErrorEvent", "tid error_info")):
+    pass
+
+
+class ThreadCrashException(Exception):
+    """Thrown when the thread crashes."""
+
+
+TICK = 20.0 * 1.0 / 1000.0
+"""The minimum interval at which to check for child process liveness -- default 20ms."""
+
+THREAD_DEAD_AND_QUEUE_EMPTY = "THREAD_DEAD_AND_QUEUE_EMPTY"
+"""Sentinel value."""
+
+
+def execute_step_in_thread(step, errors):
+    """Executes a Step in a new thread.
+
+    Args:
+        step (Step): step to execute
+    """
+    event_queue = queue.Queue()
+    thread = threading.Thread(target=_do_execute_step_in_thread, args=(event_queue, step))
+    thread.start()
+    completed_properly = False
+    while not completed_properly:
+        event = _poll_for_event(thread, event_queue)
+        if event == THREAD_DEAD_AND_QUEUE_EMPTY:
+            break
+        if event is None or isinstance(event, JumpsterEvent):
+            yield event
+        elif isinstance(event, (ThreadDoneEvent, ThreadSystemErrorEvent)):
+            completed_properly = True
+            if isinstance(event, ThreadSystemErrorEvent):
+                errors[event.tid] = event.error_info
+    if not completed_properly:
+        raise ThreadCrashException()
+    thread.join()
+
+
+def _poll_for_event(thread, event_queue):
+    try:
+        return event_queue.get(block=True, timeout=TICK)
+    except queue.Empty:
+        if not thread.is_alive():
+            # There is a possibility that after the last queue.get the
+            # thread created another event and then died. In that case
+            # we want to continue draining the queue.
+            try:
+                return event_queue.get(block=False)
+            except queue.Empty:
+                # If the queue empty we know that there are no more events
+                # and that the thread has died.
+                return THREAD_DEAD_AND_QUEUE_EMPTY
+    return None
+
+
+def _do_execute_step_in_thread(event_queue, step):
+    """Wraps the execution of a step.
+
+    Handles errors and communicates across a queue with the parent thread.
+
+    Args:
+        event_queue (Queue): event queue
+        step (Step): execution step
+    """
+    tid = threading.get_ident()
+    try:
+        for step_event in step.execute():
+            event_queue.put(step_event)
+        event_queue.put(ThreadDoneEvent(tid=tid))
+    except Exception:  # pylint: disable=broad-except
+        event_queue.put(
+            ThreadSystemErrorEvent(tid=tid, error_info=serializable_error_info_from_exc_info(sys.exc_info()))
         )
+    except Failure:
+        pass
```

### Comparing `spine_engine-0.23.4/spine_engine/project_item/__init__.py` & `spine_engine-0.24.0/spine_engine/project_item/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/project_item/connection.py` & `spine_engine-0.24.0/spine_engine/project_item/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-"""
-Provides connection classes for linking project items.
-
-"""
+""" Provides connection classes for linking project items. """
 from dataclasses import asdict, dataclass, field
 import os
 import subprocess
 import tempfile
 from contextlib import ExitStack
-from datapackage import Package
 from multiprocessing import Lock
+from datapackage import Package
 from spinedb_api import DatabaseMapping, SpineDBAPIError, SpineDBVersionError
 from spinedb_api.filters.scenario_filter import SCENARIO_FILTER_TYPE
-from spinedb_api.filters.tool_filter import TOOL_FILTER_TYPE
+from spinedb_api.filters.alternative_filter import ALTERNATIVE_FILTER_TYPE
 from spinedb_api.purge import purge_url
 from spine_engine.project_item.project_item_resource import (
     file_resource,
     make_cmd_line_arg,
     expand_cmd_line_args,
     labelled_resource_args,
 )
 from spine_engine.utils.helpers import (
-    resolve_python_interpreter,
+    resolve_current_python_interpreter,
     ItemExecutionFinishState,
     PartCount,
     ExecutionDirection as ED,
 )
 from spine_engine.utils.queue_logger import QueueLogger
 
 
+SUPPORTED_FILTER_TYPES = {ALTERNATIVE_FILTER_TYPE, SCENARIO_FILTER_TYPE}
+
+
 class ConnectionBase:
     """Base class for connections between two project items."""
 
     def __init__(self, source_name, source_position, destination_name, destination_position):
         """
         Args:
             source_name (str): source project item's name
@@ -160,56 +161,72 @@
     def make_logger(self, queue):
         self._logger = QueueLogger(queue, self.name, None, dict())
 
     def emit_flash(self):
         self._logger.flash.emit()
 
 
+DEFAULT_ENABLED_FILTER_TYPES = {ALTERNATIVE_FILTER_TYPE: False, SCENARIO_FILTER_TYPE: True}
+
+
 @dataclass
 class FilterSettings:
     """Filter settings for resource converting connections."""
 
     known_filters: dict = field(default_factory=dict)
     """mapping from resource labels and filter types to filter online statuses"""
     auto_online: bool = True
     """if True, set unknown filters automatically online"""
+    enabled_filter_types: dict = field(default_factory=DEFAULT_ENABLED_FILTER_TYPES.copy)
+
+    def __post_init__(self):
+        for resource, online_filters in self.known_filters.items():
+            supported_filters = {
+                filter_type: online
+                for filter_type, online in online_filters.items()
+                if filter_type in SUPPORTED_FILTER_TYPES
+            }
+            if supported_filters:
+                self.known_filters[resource] = supported_filters
 
     def has_filters(self):
         """Tests if there are filters.
 
         Returns:
             bool: True if filters of any type exists, False otherwise
         """
         for filters_by_type in self.known_filters.values():
-            for filters in filters_by_type.values():
-                if filters:
+            for filter_type, filters in filters_by_type.items():
+                if self.enabled_filter_types[filter_type] and filters:
                     return True
         return False
 
     def has_any_filter_online(self):
         """Tests in any filter is online.
 
         Returns:
             bool: True if any filter is online, False otherwise
         """
         for filters_by_type in self.known_filters.values():
-            for filters in filters_by_type.values():
-                if any(filters.values()):
+            for filter_type, filters in filters_by_type.items():
+                if self.enabled_filter_types[filter_type] and any(filters.values()):
                     return True
         return False
 
     def has_filter_online(self, filter_type):
         """Tests if any filter of given type is online.
 
         Args:
             filter_type (str): filter type to test
 
         Returns:
             bool: True if any filter of filter_type is online, False otherwise
         """
+        if not self.enabled_filter_types[filter_type]:
+            return False
         for filters_by_type in self.known_filters.values():
             if any(filters_by_type.get(filter_type, {}).values()):
                 return True
         return False
 
     def to_dict(self):
         """Stores the settings to a dict.
@@ -303,27 +320,40 @@
 
         Args:
             filter_type (str): filter type
 
         Returns:
             bool: True if online filters are required, False otherwise
         """
-        return self.options.get("require_" + filter_type, False)
+        return self._filter_settings.enabled_filter_types[filter_type] and self.options.get(
+            "require_" + filter_type, False
+        )
+
+    def is_filter_type_enabled(self, filter_type):
+        """Tests if filter type is enabled.
+
+        Args:
+            filter_type (str): filter type
+
+        Returns:
+            bool: True if filter type is enabled, False otherwise
+        """
+        return self._filter_settings.enabled_filter_types[filter_type]
 
     def notifications(self):
         """See base class."""
         notifications = []
-        for filter_type in (SCENARIO_FILTER_TYPE, TOOL_FILTER_TYPE):
+        for filter_type in (SCENARIO_FILTER_TYPE, ALTERNATIVE_FILTER_TYPE):
             filter_settings = self._filter_settings
             if self.require_filter_online(filter_type) and (
                 not filter_settings.has_filter_online(filter_type)
                 if filter_settings.has_filters()
                 else not filter_settings.auto_online
             ):
-                filter_name = {SCENARIO_FILTER_TYPE: "scenario", TOOL_FILTER_TYPE: "tool"}[filter_type]
+                filter_name = {SCENARIO_FILTER_TYPE: "scenario", ALTERNATIVE_FILTER_TYPE: "alternative"}[filter_type]
                 notifications.append(f"At least one {filter_name} filter must be active.")
         return notifications
 
     def receive_resources_from_source(self, resources):
         """See base class."""
         self._resources = {r for r in resources if r.type_ == "database" and r.filterable}
 
@@ -358,14 +388,16 @@
         return self._apply_use_memory_db(self._apply_use_datapackage(resources))
 
     def _do_purge_before_writing(self, resources):
         if self.purge_before_writing:
             to_urls = (r.url for r in resources if r.type_ == "database")
             for url in to_urls:
                 purge_url(url, self.purge_settings, self._logger)
+            return to_urls
+        return []
 
     def _apply_use_memory_db(self, resources):
         if not self.use_memory_db:
             return resources
         final_resources = []
         for r in resources:
             if r.type_ == "database":
@@ -408,30 +440,29 @@
         package_resource = file_resource(provider, package_path, label=f"datapackage@{provider}")
         package_resource.metadata = resources[0].metadata
         final_resources.append(package_resource)
         return final_resources
 
     def ready_to_execute(self):
         """See base class."""
-        for filter_type in (SCENARIO_FILTER_TYPE, TOOL_FILTER_TYPE):
+        for filter_type in (SCENARIO_FILTER_TYPE, ALTERNATIVE_FILTER_TYPE):
             if self.require_filter_online(filter_type) and not self._filter_settings.has_filter_online(filter_type):
                 return False
         return True
 
     def to_dict(self):
         """Returns a dictionary representation of this Connection.
 
         Returns:
             dict: serialized Connection
         """
         d = super().to_dict()
         if self.options:
             d["options"] = self.options.copy()
-        if self._filter_settings.has_filters():
-            d["filter_settings"] = self._filter_settings.to_dict()
+        d["filter_settings"] = self._filter_settings.to_dict()
         return d
 
     @staticmethod
     def _constructor_args_from_dict(connection_dict):
         """See base class."""
         kw_args = ConnectionBase._constructor_args_from_dict(connection_dict)
         kw_args["options"] = connection_dict.get("options")
@@ -458,15 +489,15 @@
             source_position (str): source anchor's position
             destination_name (str): destination project item's name
             destination_position (str): destination anchor's position
             options (dict, optional): any additional options
             filter_settings (FilterSettings, optional): filter settings
         """
         super().__init__(source_name, source_position, destination_name, destination_position, options, filter_settings)
-        self._enabled_filter_names = None
+        self._enabled_filter_values = None
         self._source_visited = False
 
     def visit_source(self):
         self._source_visited = True
 
     def visit_destination(self):
         if not self._source_visited:
@@ -480,54 +511,75 @@
 
         Args:
             resource_label (str): resource label
 
         Returns:
             dict: mapping from filter type to list of online filter names
         """
-        if self._enabled_filter_names is None:
-            self._prepare_enabled_filter_names()
-        return self._enabled_filter_names.get(resource_label)
+        if self._enabled_filter_values is None:
+            self._prepare_enabled_filter_values()
+        return self._enabled_filter_values.get(resource_label)
 
-    def _prepare_enabled_filter_names(self):
+    def _prepare_enabled_filter_values(self):
         """Reads filter information from database."""
-        self._enabled_filter_names = {}
+        self._enabled_filter_values = {}
         for resource in self._resources:
             url = resource.url
             if not url:
                 continue
             try:
-                db_map = DatabaseMapping(url)
+                with DatabaseMapping(url) as db_map:
+                    known_filters = self._filter_settings.known_filters.get(resource.label, {})
+                    enabled_filter_values = self._enabled_filter_values.setdefault(resource.label, {})
+                    if self._filter_settings.enabled_filter_types[SCENARIO_FILTER_TYPE]:
+                        enabled_scenarios = self._fetch_scenario_filter_values(db_map, known_filters)
+                        if enabled_scenarios:
+                            enabled_filter_values[SCENARIO_FILTER_TYPE] = enabled_scenarios
+                    if self._filter_settings.enabled_filter_types[ALTERNATIVE_FILTER_TYPE]:
+                        enabled_alternatives = self._fetch_alternative_filter_values(db_map, known_filters)
+                        if enabled_alternatives:
+                            enabled_filter_values[ALTERNATIVE_FILTER_TYPE] = enabled_alternatives
             except (SpineDBAPIError, SpineDBVersionError):
                 continue
-            try:
-                scenario_filter_settings = self._filter_settings.known_filters.get(resource.label, {}).get(
-                    SCENARIO_FILTER_TYPE, {}
-                )
-                available_scenarios = {row.name for row in db_map.query(db_map.scenario_sq)}
-                enabled_scenarios = set()
-                for name in available_scenarios:
-                    if scenario_filter_settings.get(name, self._filter_settings.auto_online):
-                        enabled_scenarios.add(name)
-                if enabled_scenarios:
-                    self._enabled_filter_names.setdefault(resource.label, {})[SCENARIO_FILTER_TYPE] = sorted(
-                        list(enabled_scenarios)
-                    )
-                tool_filter_settings = self._filter_settings.known_filters.get(resource.label, {}).get(
-                    TOOL_FILTER_TYPE, {}
-                )
-                available_tools = {row.name for row in db_map.query(db_map.tool_sq)}
-                enabled_tools = set()
-                for name in available_tools:
-                    if tool_filter_settings.get(name, self._filter_settings.auto_online):
-                        enabled_tools.add(name)
-                if enabled_tools:
-                    self._enabled_filter_names.setdefault(resource.label, {})[TOOL_FILTER_TYPE] = sorted(enabled_tools)
-            finally:
-                db_map.connection.close()
+
+    def _fetch_scenario_filter_values(self, db_map, known_filters):
+        """Fetches scenario names from database and picks the ones that are enabled by filter settings.
+
+        Args:
+            db_map (DatabaseMapping): database mapping
+            known_filters (dict): mapping from filter type to filter settings
+
+        Returns:
+            list of str: scenario filter values
+        """
+        filter_settings = known_filters.get(SCENARIO_FILTER_TYPE, {})
+        available_scenarios = {row.name for row in db_map.query(db_map.scenario_sq)}
+        enabled_scenarios = set()
+        for scenario_name in available_scenarios:
+            if filter_settings.get(scenario_name, self._filter_settings.auto_online):
+                enabled_scenarios.add(scenario_name)
+        return sorted(enabled_scenarios)
+
+    def _fetch_alternative_filter_values(self, db_map, known_filters):
+        """Fetches enabled alternative names from database.
+
+        Args:
+            db_map (DatabaseMapping): database mapping
+            known_filters (dict): mapping from filter type to filter settings
+
+        Returns:
+            list of list of str: alternative filter values
+        """
+        filter_settings = known_filters.get(ALTERNATIVE_FILTER_TYPE, {})
+        available_alternatives = {row.name for row in db_map.query(db_map.alternative_sq)}
+        enabled_alternatives = set()
+        for alternative_name in available_alternatives:
+            if filter_settings.get(alternative_name, self._filter_settings.auto_online):
+                enabled_alternatives.add(alternative_name)
+        return [list(enabled_alternatives)] if enabled_alternatives else []
 
     @classmethod
     def from_dict(cls, connection_dict):
         """Restores a connection from dictionary.
 
         Args:
             connection_dict (dict): connection dictionary
@@ -539,34 +591,32 @@
         return cls(**kw_args_from_dict)
 
 
 class Jump(ConnectionBase):
     """Represents a conditional jump between two project items."""
 
     def __init__(
-        self, source_name, source_position, destination_name, destination_position, condition=None, cmd_line_args=()
+        self, source_name, source_position, destination_name, destination_position, condition={}, cmd_line_args=()
     ):
         """
         Args:
             source_name (str): source project item's name
             source_position (str): source anchor's position
             destination_name (str): destination project item's name
             destination_position (str): destination anchor's position
             condition (dict): jump condition
         """
         super().__init__(source_name, source_position, destination_name, destination_position)
-        self.condition = condition if condition is not None else {"type": "python-script", "script": "exit(1)"}
+        default_condition = {"type": "python-script", "script": "exit(1)", "specification": ""}
+        self.condition = condition if condition else default_condition
         self._resources_from_source = set()
         self._resources_from_destination = set()
         self.cmd_line_args = list(cmd_line_args)
         self._engine = None
-        self.source_solid = None
-        self.destination_solid = None
         self.item_names = set()
-        self.solid_names = set()
 
     def set_engine(self, engine):
         self._engine = engine
 
     @property
     def resources(self):
         return self._resources_from_source | self._resources_from_destination
@@ -613,15 +663,15 @@
             return False
         with ExitStack() as stack:
             labelled_args = labelled_resource_args(self.resources, stack)
             expanded_args = expand_cmd_line_args(self.cmd_line_args + [jump_counter], labelled_args, self._logger)
             with tempfile.TemporaryFile("w+", encoding="utf-8") as script_file:
                 script_file.write(script)
                 script_file.seek(0)
-                python = resolve_python_interpreter("")
+                python = resolve_current_python_interpreter()
                 result = subprocess.run(
                     [python, "-", *expanded_args], encoding="utf-8", stdin=script_file, capture_output=True
                 )
                 if result.stdout:
                     self._logger.msg_proc.emit(result.stdout)
                 if result.stderr:
                     self._logger.msg_proc_error.emit(result.stderr)
@@ -674,13 +724,15 @@
 
     Args:
         disabled_filter_names (dict): disabled filter names with names stored as lists
 
     Returns:
         dict: known filters
     """
+    deprecated_types = {"tool_filter"}
     converted = {}
     for label, names_by_type in disabled_filter_names.items():
         converted_names_by_type = converted.setdefault(label, {})
         for filter_type, names in names_by_type.items():
-            converted_names_by_type[filter_type] = {name: False for name in names}
+            if filter_type not in deprecated_types:
+                converted_names_by_type[filter_type] = {name: False for name in names}
     return converted
```

### Comparing `spine_engine-0.23.4/spine_engine/project_item/executable_item_base.py` & `spine_engine-0.24.0/spine_engine/project_item/executable_item_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/project_item/project_item_info.py` & `spine_engine-0.24.0/spine_engine/project_item/project_item_info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -12,25 +13,28 @@
 Provides the ProjectItemInfo class.
 
 """
 
 
 class ProjectItemInfo:
     @staticmethod
-    def item_category():
+    def item_type():
         """
-        Returns the item category string, e.g., "Tools".
+        Returns the item type string, e.g., "Importer".
 
         Returns:
-            str: item's category
+            str: item's type
         """
         raise NotImplementedError()
 
     @staticmethod
-    def item_type():
+    def specification_icon(specification):
         """
-        Returns the item type string, e.g., "Importer".
+        Returns the specification icon resource path.
+
+        Args:
+            specification (ProjectItemSpecification): Item's specification
 
         Returns:
-            str: item's type
+            str: Path to the resource
         """
         raise NotImplementedError()
```

### Comparing `spine_engine-0.23.4/spine_engine/project_item/project_item_resource.py` & `spine_engine-0.24.0/spine_engine/project_item/project_item_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -69,15 +70,18 @@
                 "id": self._identifier,
                 "part_count": self.metadata.get("part_count", PartCount()),
                 "current": self.metadata.get("current"),
                 "precursors": self.metadata.get("precursors", set()),
             }
             db_server_manager_queue = self.metadata["db_server_manager_queue"]
             with closing_spine_db_server(
-                db_server_manager_queue, self.url, memory=self.metadata.get("memory", False), ordering=ordering
+                self.url,
+                memory=self.metadata.get("memory", False),
+                ordering=ordering,
+                server_manager_queue=db_server_manager_queue,
             ) as server_url:
                 if db_checkin:
                     SpineDBClient.from_server_url(server_url).db_checkin()
                 try:
                     yield server_url
                 finally:
                     if db_checkout:
@@ -151,21 +155,20 @@
         """Resource URL."""
         return self._url
 
     @url.setter
     def url(self, url):
         self._url = url
         self._parsed_url = urlparse(self._url)
-        self._filepath = url2pathname(self._parsed_url.path)
 
     @property
     def path(self):
         """Returns the resource path in the local syntax, as obtained from parsing the url."""
         if not self._filepath:
-            self._filepath = url2pathname(self._parsed_url.path)
+            self._filepath = url2pathname(self._parsed_url.path) if self._parsed_url.path else ""
         return self._filepath
 
     @property
     def scheme(self):
         """Returns the resource scheme, as obtained from parsing the url."""
         return self._parsed_url.scheme
```

### Comparing `spine_engine-0.23.4/spine_engine/project_item/project_item_specification.py` & `spine_engine-0.24.0/spine_engine/project_item/project_item_specification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Contains project item specification class.
-
-"""
+"""Contains project item specification class."""
 import json
-
 from spine_engine.utils.helpers import shorten, gather_leaf_data
 
 
 class ProjectItemSpecification:
     """
     Class to hold a project item specification.
 
     Attributes:
         item_type (str): type of the project item the specification is compatible with
         definition_file_path (str): specification's JSON file path
     """
 
-    def __init__(self, name, description=None, item_type="", item_category=""):
+    def __init__(self, name, description=None, item_type=""):
         """
         Args:
             name (str): specification name
             description (str): description
             item_type (str): Project item type
-            item_category (str): Project item category
         """
         self.name = name
         self.short_name = shorten(name)
         self.description = description
         self.item_type = item_type
-        self.item_category = item_category
         self.definition_file_path = ""
         self.plugin = None
 
     # TODO: Needed?
     def set_name(self, name):
         """Set object name and short name.
         Note: Check conflicts (e.g. name already exists)
```

### Comparing `spine_engine-0.23.4/spine_engine/project_item/project_item_specification_factory.py` & `spine_engine-0.24.0/spine_engine/project_item/project_item_specification_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/project_item_loader.py` & `spine_engine-0.24.0/spine_engine/project_item_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/__init__.py` & `spine_engine-0.24.0/tests/server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
-# Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
-# General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
-# option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+# Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
+# Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
+# any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
-This package contains Remote Server classes of the Spine Engine.
-
+Init file for spine_engine.tests.server package.
 """
```

### Comparing `spine_engine-0.23.4/spine_engine/server/certificate_creator.py` & `spine_engine-0.24.0/spine_engine/server/certificate_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/engine_server.py` & `spine_engine-0.24.0/spine_engine/server/engine_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -52,17 +53,17 @@
         super().__init__(target=self.serve, name="EngineServerThread")
         if sec_model == ServerSecurityModel.NONE:
             self._sec_model_state = ServerSecurityModel.NONE
         elif sec_model == ServerSecurityModel.STONEHOUSE:
             if not sec_folder:
                 raise ValueError("Path to security folder missing")
             base_dir = sec_folder
-            self.keys_dir = os.path.join(base_dir, 'certificates')
-            self.public_keys_dir = os.path.join(base_dir, 'public_keys')
-            self.secret_keys_dir = os.path.join(base_dir, 'private_keys')
+            self.keys_dir = os.path.join(base_dir, "certificates")
+            self.public_keys_dir = os.path.join(base_dir, "public_keys")
+            self.secret_keys_dir = os.path.join(base_dir, "private_keys")
             if not os.path.exists(self.keys_dir):
                 raise ValueError(f"Security folder: {self.keys_dir} does not exist")
             if not os.path.exists(self.public_keys_dir):
                 raise ValueError(f"Security folder: {self.public_keys_dir} does not exist")
             if not os.path.exists(self.secret_keys_dir):
                 raise ValueError(f"Security folder: {self.secret_keys_dir} does not exist")
             self._sec_folder = sec_folder
@@ -157,16 +158,16 @@
                     elif request.cmd() == "answer_prompt":
                         worker = workers.get(request.request_id(), None)  # Get DAG execution worker based on job Id
                         if not worker:
                             print(f"Worker for job_id:{request.request_id()} not found")
                             msg = f"Answering prompt failed. Worker for job_id:{request.request_id()} not found."
                             self.send_init_failed_reply(frontend, request.connection_id(), msg)
                             continue
-                        item_name, accepted = request.data()
-                        worker.answer_prompt(item_name, accepted)
+                        prompter_id, answer = request.data()
+                        worker.answer_prompt(prompter_id, answer)
                         continue
                     elif request.cmd() == "retrieve_project":
                         project_dir = project_dirs.get(request.request_id(), None)  # Get project dir based on job_id
                         if not project_dir:
                             print(f"Project for job_id:{request.request_id()} not found")
                             msg = (
                                 f"Retrieving project for job_id {request.request_id()} failed. "
@@ -333,15 +334,15 @@
                 auth.allow(ep)
                 allowed.append(ep)  # Just for printing
             except:
                 raise ValueError(f"Invalid IP address in allowEndpoints.txt:'{ep}'")
         allowed_str = "\n".join(allowed)
         print(f"StoneHouse security activated. Allowed endpoints ({len(allowed)}):\n{allowed_str}")
         # Tell the authenticator how to handle CURVE requests
-        auth.configure_curve(domain='*', location=zmq.auth.CURVE_ALLOW_ANY)
+        auth.configure_curve(domain="*", location=zmq.auth.CURVE_ALLOW_ANY)
         server_secret_file = os.path.join(self.secret_keys_dir, "server.key_secret")
         server_public, server_secret = zmq.auth.load_certificate(server_secret_file)
         frontend.curve_secretkey = server_secret
         frontend.curve_publickey = server_public
         frontend.curve_server = True  # must come before bind
         return auth
```

### Comparing `spine_engine-0.23.4/spine_engine/server/persistent_execution_service.py` & `spine_engine-0.24.0/spine_engine/server/persistent_execution_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -46,29 +47,29 @@
             retval = pm.make_complete_command(cmd) is not None
             retval_tuple = cmd_type, retval
         elif cmd_type == "issue_persistent_command":
             self.request.send_response(self.worker_socket, (cmd_type, str(pub_port)), (self.job_id, "in_progress"))
             for msg in pm.issue_command(cmd, add_history=True, catch_exception=False):
                 json_msg = json.dumps(msg)
                 self.push_socket.send(json_msg.encode("utf-8"))  # This blocks until somebody is pulling (receiving)
-            self.push_socket.send(b'END')
+            self.push_socket.send(b"END")
             retval_tuple = cmd_type, "ok"
         elif cmd_type == "get_completions":
             retval = pm.get_completions(cmd)
             retval_tuple = cmd_type, retval
         elif cmd_type == "get_history_item":
             text, prefix, backwards = cmd
             retval = pm.get_history_item(text, prefix, backwards)
             retval_tuple = cmd_type, retval
         elif cmd_type == "restart_persistent":
             self.request.send_response(self.worker_socket, (cmd_type, str(pub_port)), (self.job_id, "in_progress"))
             for msg in pm.restart_persistent():
                 json_msg = json.dumps(msg)
                 self.push_socket.send(json_msg.encode("utf-8"))
-            self.push_socket.send(b'END')
+            self.push_socket.send(b"END")
             retval_tuple = cmd_type, "ok"
         elif cmd_type == "interrupt_persistent":
             pm.interrupt_persistent()
             retval_tuple = cmd_type, "ok"
         elif cmd_type == "kill_persistent":
             pm.kill_process()
             retval_tuple = cmd_type, "ok"
```

### Comparing `spine_engine-0.23.4/spine_engine/server/ping_service.py` & `spine_engine-0.24.0/spine_engine/server/ping_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/project_extractor_service.py` & `spine_engine-0.24.0/spine_engine/server/project_extractor_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/project_remover_service.py` & `spine_engine-0.24.0/spine_engine/server/project_remover_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/project_retriever_service.py` & `spine_engine-0.24.0/spine_engine/server/project_retriever_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/remote_execution_service.py` & `spine_engine-0.24.0/spine_engine/server/remote_execution_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-
-"""
-Contains RemoteExecutionService class that executes a single DAG on the Spine Engine Server.
-"""
+""" Contains RemoteExecutionService class that executes a single DAG on the Spine Engine Server. """
 
 import os
 import threading
 import zmq
 from spine_engine import SpineEngine
 from spine_engine.utils.helpers import get_file_size
 from spine_engine.server.service_base import ServiceBase
@@ -151,17 +149,17 @@
             self.worker_socket, ("remote_execution_event", "completed"), (self.job_id, "completed")
         )
 
     def stop_engine(self):
         """Stops DAG execution."""
         self.engine.stop()
 
-    def answer_prompt(self, item_name, accepted):
+    def answer_prompt(self, prompter_id, answer):
         """Answers prompt."""
-        self.engine.answer_prompt(item_name, accepted)
+        self.engine.answer_prompt(prompter_id, answer)
 
     def close(self):
         """Cleans up sockets after worker is finished."""
         super().close()
         self.push_socket.close()
 
     @staticmethod
@@ -174,40 +172,36 @@
 
         Returns:
             dict: Converted input data
         """
         # Adjust project_dir to point to the local folder
         remote_folder = input_data["project_dir"]  # Project directory on client
         input_data["project_dir"] = local_project_dir  # Project directory on server
-        # Loop specs
-        specs_keys = input_data["specifications"].keys()
-        for specs_key in specs_keys:
+        for specs_key, spec_item in input_data["specifications"].items():
             spec_item = input_data["specifications"][specs_key]
-            i = 0
-            for specItemInfo in spec_item:
+            for i, item_info in enumerate(spec_item):
                 # Adjust definition_file_path in specs to point to the server folder
-                if "definition_file_path" in specItemInfo:
-                    original_def_file_path = specItemInfo["definition_file_path"]  # Absolute path on client machine
+                if "definition_file_path" in item_info:
+                    original_def_file_path = item_info["definition_file_path"]  # Absolute path on client machine
                     # Make sure path separators match the OS separator
                     original_def_file_path = original_def_file_path.replace("\\", os.path.sep)
                     # Remove part of definition file path that references client machine path to get
                     # a relative definition file path. Note: os.path.relpath() does not work because the output
                     # depends on OS. Note2: '/' must be added to remote folder here.
                     rel_def_file_path = original_def_file_path.replace(remote_folder + "/", "")
                     modified = os.path.join(local_project_dir, rel_def_file_path)  # Absolute path on server machine
                     input_data["specifications"][specs_key][i]["definition_file_path"] = modified
-                i += 1
                 # Modify Python executable path and kernel spec because those refer to paths on client's machine
-                if "execution_settings" in specItemInfo and specItemInfo["tooltype"] == "python":
-                    if specItemInfo["execution_settings"]["use_jupyter_console"]:
+                if "execution_settings" in item_info and item_info["tooltype"] == "python":
+                    if item_info["execution_settings"].get("use_jupyter_console", False):
                         # Replace kernel_spec_name with the default kernel spec 'python3' (must be available on server)
-                        specItemInfo["execution_settings"]["kernel_spec_name"] = "python3"
+                        item_info["execution_settings"]["kernel_spec_name"] = "python3"
                     else:
                         # Replace Python executable exec with "" because client's Python is not available on server
-                        specItemInfo["execution_settings"]["executable"] = ""
+                        item_info["execution_settings"]["executable"] = ""
         # Loop items
         items_keys = input_data["items"].keys()
         for items_key in items_keys:
             # Force execute in source dir
             if "execute_in_work" in input_data["items"][items_key]:
                 input_data["items"][items_key]["execute_in_work"] = False
         # Edit app settings dictionary
```

### Comparing `spine_engine-0.23.4/spine_engine/server/request.py` & `spine_engine-0.24.0/spine_engine/server/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/service_base.py` & `spine_engine-0.24.0/spine_engine/server/service_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/start_server.py` & `spine_engine-0.24.0/spine_engine/server/start_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/server/util/__init__.py` & `spine_engine-0.24.0/spine_engine/server/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
-This package contains utility classes of remote server part of the Spine Engine.
+This package contains Remote Server classes of the Spine Engine.
 
 """
```

### Comparing `spine_engine-0.23.4/spine_engine/server/util/event_data_converter.py` & `spine_engine-0.24.0/spine_engine/server/util/event_data_converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Contains static methods for converting event and data information to JSON format and back.
-"""
-
+"""Contains static methods for converting event and data information to JSON format and back."""
 import base64
 import json
 from spine_engine.spine_engine import ItemExecutionFinishState
+from spine_engine.utils.helpers import ExecutionDirection
 
 
 class EventDataConverter:
     @staticmethod
     def convert(event_type, data, b64encoding=False):
         """Converts a single event_type, data pair into a JSON string.
          Optionally, encodes data as base64.
@@ -89,14 +88,16 @@
             # We need to read the connection file to a JSON dictionary and insert that to data as a new key
             with open(data["connection_file"], "r") as fh:
                 try:
                     connection_file_dict = json.load(fh)
                     data["connection_file_dict"] = connection_file_dict
                 except json.decoder.JSONDecodeError:
                     print(f"Error loading connection file {data['connection_file']}. Invalid JSON.")
+        if "direction" in data.keys():
+            data["direction"] = str(data["direction"])  # Cast ExecutionDirection instance to string
         for key in data.keys():
             # Print warning if there are any tuples used as keys in the data dictionary.
             # Tuples are converted to lists by json.dumps(). Lists must be converted back to tuples
             # on client side (in fix_event_data()).
             if type(data[key]) == tuple:
                 print(f"[WARNING] Found tuple in message {event_type}: {data}. Fix this on client side.")
     return data
@@ -113,27 +114,47 @@
     """
     # Convert item_state str back to ItemExecutionFinishState. This was converted to str on server because
     # it is not JSON serializable
     if type(event[1]) == str:
         return event
     if "item_state" in event[1].keys():
         event[1]["item_state"] = convert_execution_finish_state(event[1]["item_state"])
+    if "direction" in event[1].keys():
+        event[1]["direction"] = convert_execution_direction(event[1]["direction"])
     return event
 
 
 def convert_execution_finish_state(state):
     """Transforms state string into an ItemExecutionFinishState enum.
 
     Args:
         state (str): State as string
 
     Returns:
         ItemExecutionFinishState: Enum if given str is valid, None otherwise.
     """
-    states = dict()
-    states["SUCCESS"] = ItemExecutionFinishState.SUCCESS
-    states["FAILURE"] = ItemExecutionFinishState.FAILURE
-    states["SKIPPED"] = ItemExecutionFinishState.SKIPPED
-    states["EXCLUDED"] = ItemExecutionFinishState.EXCLUDED
-    states["STOPPED"] = ItemExecutionFinishState.STOPPED
-    states["NEVER_FINISHED"] = ItemExecutionFinishState.NEVER_FINISHED
+    states = {
+        "SUCCESS": ItemExecutionFinishState.SUCCESS,
+        "FAILURE": ItemExecutionFinishState.FAILURE,
+        "SKIPPED": ItemExecutionFinishState.SKIPPED,
+        "EXCLUDED": ItemExecutionFinishState.EXCLUDED,
+        "STOPPED": ItemExecutionFinishState.STOPPED,
+        "NEVER_FINISHED": ItemExecutionFinishState.NEVER_FINISHED,
+    }
     return states.get(state, None)
+
+
+def convert_execution_direction(direction):
+    """Transforms direction string into an ExecutionDirection enum.
+
+    Args:
+        direction (str): Direction as string
+
+    Returns:
+        ExecutionDirection: Enum if given str is valid, None otherwise.
+    """
+    directions = {
+        "FORWARD": ExecutionDirection.FORWARD,
+        "BACKWARD": ExecutionDirection.BACKWARD,
+        "NONE": ExecutionDirection.NONE,
+    }
+    return directions.get(direction, None)
```

### Comparing `spine_engine-0.23.4/spine_engine/server/util/server_message.py` & `spine_engine-0.24.0/spine_engine/server/util/server_message.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -67,36 +68,36 @@
 
         Returns:
             str: The instance as a JSON string
         """
         jsonFileNames = self._getJSONFileNames()
         retStr = ""
         retStr += "{\n"
-        retStr += "   \"command\": \"" + self._command + "\",\n"
-        retStr += "   \"id\":\"" + self._id + "\",\n"
+        retStr += '   "command": "' + self._command + '",\n'
+        retStr += '   "id":"' + self._id + '",\n'
 
         if len(self._data) == 0:
-            retStr += "   \"data\":\"\",\n"
+            retStr += '   "data":"",\n'
         else:
-            retStr += "   \"data\":" + self._data + ",\n"
-        retStr += "   \"files\": " + jsonFileNames
+            retStr += '   "data":' + self._data + ",\n"
+        retStr += '   "files": ' + jsonFileNames
         retStr += "}"
         return retStr
 
     def _getJSONFileNames(self):
         fileNameCount = len(self._files)
         if fileNameCount == 0:
             return "{}\n"
-        retStr = '{\n'
+        retStr = "{\n"
         i = 0
         for fName in self._files:
             if i + 1 < fileNameCount:
-                retStr = retStr + "    \"name-" + str(i) + "\": \"" + fName + "\",\n"
+                retStr = retStr + '    "name-' + str(i) + '": "' + fName + '",\n'
             else:
-                retStr = retStr + "    \"name-" + str(i) + "\": \"" + fName + "\"\n"
+                retStr = retStr + '    "name-' + str(i) + '": "' + fName + '"\n'
             i += 1
         retStr = retStr + "    }\n"
         return retStr
 
     def to_bytes(self):
         """Converts this ServerMessage instance to a JSON and then to a bytes string.
 
@@ -119,11 +120,11 @@
         parsed_msg = json.loads(message.decode("utf-8"))  # Load JSON string into dictionary
         filenames = parsed_msg["files"]  # dict
         data = parsed_msg["data"]  # list
         parsed_filenames = list()
         if len(filenames) > 0:
             for f in filenames:
                 parsed_filenames.append(filenames[f])
-            msg = cls(parsed_msg['command'], parsed_msg['id'], data, parsed_filenames)
+            msg = cls(parsed_msg["command"], parsed_msg["id"], data, parsed_filenames)
         else:
-            msg = cls(parsed_msg['command'], parsed_msg['id'], data, None)
+            msg = cls(parsed_msg["command"], parsed_msg["id"], data, None)
         return msg
```

### Comparing `spine_engine-0.23.4/spine_engine/server/util/zip_handler.py` & `spine_engine-0.24.0/spine_engine/server/util/zip_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/spine_engine.py` & `spine_engine-0.24.0/spine_engine/spine_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,25 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-
-"""
-Contains the SpineEngine class for running Spine Toolbox DAGs.
-
-"""
+""" Contains the SpineEngine class for running Spine Toolbox DAGs. """
 from enum import Enum, unique
 import os
 import threading
 import multiprocessing as mp
 from itertools import product
 import networkx as nx
-from dagster import (
-    PipelineDefinition,
-    SolidDefinition,
-    InputDefinition,
-    OutputDefinition,
-    DependencyDefinition,
-    ModeDefinition,
-    Output,
-    Failure,
-    DagsterEventType,
-    default_executors,
-    AssetMaterialization,
-    execute_pipeline_iterator,
-)
 from spinedb_api import append_filter_config, name_from_dict
 from spinedb_api.spine_db_server import db_server_manager
 from spinedb_api.filters.tools import filter_config
 from spinedb_api.filters.scenario_filter import scenario_name_from_dict
 from spinedb_api.filters.execution_filter import execution_filter_config
 from .exception import EngineInitFailed
 from .execution_managers.persistent_execution_manager import (
@@ -53,17 +36,25 @@
     ItemExecutionFinishState,
     dag_edges,
     make_connections,
 )
 from .utils.execution_resources import one_shot_process_semaphore, persistent_process_semaphore
 from .utils.queue_logger import QueueLogger
 from .project_item_loader import ProjectItemLoader
-from .multithread_executor.executor import multithread_executor
+from .jumpster import (
+    execute_pipeline_iterator,
+    JumpsterEventType,
+    PipelineDefinition,
+    SolidDefinition,
+    InputDefinition,
+    Output,
+    Failure,
+    Finalization,
+)
 from .project_item.connection import Connection, Jump
-from .shared_memory_io_manager import shared_memory_io_manager
 
 
 @unique
 class SpineEngineState(Enum):
     SLEEPING = 1
     """Dare to wake it?"""
     RUNNING = 2
@@ -71,20 +62,14 @@
     FAILED = 4
     COMPLETED = 5
 
     def __str__(self):
         return str(self.name)
 
 
-class _JumpPipelineDefinition(PipelineDefinition):
-    def __init__(self, *args, jumps=None, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.jumps = jumps if jumps is not None else []
-
-
 class SpineEngine:
     """
     An engine for executing a Spine Toolbox DAG-workflow.
     """
 
     _resource_limit_lock = threading.Lock()
 
@@ -127,47 +112,41 @@
         connections = list(map(Connection.from_dict, connections))  # Deserialize connections
         project_item_loader = ProjectItemLoader()
         self._executable_item_classes = project_item_loader.load_executable_item_classes(items_module_name)
         required_items = required_items_for_execution(
             self._items, connections, self._executable_item_classes, self._execution_permits
         )
         self._connections = make_connections(connections, required_items)
-        self._connections_by_source = dict()
-        self._connections_by_destination = dict()
+        self._connections_by_source = {}
+        self._connections_by_destination = {}
         self._validate_and_sort_connections()
-        edges = dag_edges(self._connections)  # Mapping of a source node (item) to a list of destination nodes (items)
+        self._back_injectors = dag_edges(
+            self._connections
+        )  # Mapping of a source node (item) to a list of destination nodes (items)
         self._check_write_index()
         self._settings = AppSettings(settings if settings is not None else {})
         _set_resource_limits(self._settings, SpineEngine._resource_limit_lock)
         enable_persistent_process_creation()
         self._project_dir = project_dir
         if specifications is None:
             specifications = {}
         self._item_specifications = self._make_item_specifications(
             specifications, project_item_loader, items_module_name
         )
-        self._dag = make_dag(edges, self._execution_permits)
+        self._dag = make_dag(self._back_injectors, self._execution_permits)
         _validate_dag(self._dag)
-        self._dag_nodes = list(self._dag)  # Names of permitted items and their neighbors
+        self._item_names = list(self._dag)  # Names of permitted items and their neighbors
         if jumps is None:
             jumps = []
         self._jumps = list(map(Jump.from_dict, jumps))
         validate_jumps(self._jumps, self._dag)
         for x in self._connections + self._jumps:
             x.make_logger(self._queue)
         for x in self._jumps:
             x.set_engine(self)
-        # Mapping of item name to solid name
-        self._solids_by_items = {item_name: str(i) for i, item_name in enumerate(self._dag_nodes)}
-        # Mapping of solid name to item name
-        self._items_by_solids = {solid_name: item_name for item_name, solid_name in self._solids_by_items.items()}
-        # Same as edges but item names are swapped to solid names
-        self._back_injectors = {
-            self._solids_by_items[key]: [self._solids_by_items[x] for x in value] for key, value in edges.items()
-        }
         self._forth_injectors = inverted(self._back_injectors)
         self._pipeline = self._make_pipeline()
         self._state = SpineEngineState.SLEEPING
         self._debug = debug
         self._running_items = []
         self._prompt_queues = {}
         self._answered_prompts = {}
@@ -258,15 +237,16 @@
         return item_specifications
 
     def make_item(self, item_name, direction):
         """Recreates item from project item dictionary for a particular execution.
         Note that this method is called multiple times for each item:
         Once for the backward pipeline, and once for each filtered execution in the forward pipeline."""
         item_dict = self._items[item_name]
-        prompt_queue = self._prompt_queues[item_name] = mp.Queue()
+        prompt_queue = mp.Queue()
+        self._prompt_queues[id(prompt_queue)] = prompt_queue
         logger = QueueLogger(
             self._queue, item_name, prompt_queue, self._answered_prompts, silent=direction is ED.BACKWARD
         )
         return self.do_make_item(item_name, item_dict, logger)
 
     def do_make_item(self, item_name, item_dict, logger):
         item_type = item_dict["type"]
@@ -296,108 +276,72 @@
         while True:
             msg = self._queue.get()
             yield msg
             if msg[0] == "dag_exec_finished":
                 break
         self._thread.join()
 
-    def answer_prompt(self, item_name, accepted):
-        """Answers the prompt for the specified item, either accepting or rejecting it."""
-        self._prompt_queues[item_name].put(accepted)
+    def answer_prompt(self, prompter_id, answer):
+        """Answers the prompt for the specified prompter id."""
+        self._prompt_queues[prompter_id].put(answer)
 
     def wait(self):
         """Waits until engine execution has finished."""
         if self._thread.is_alive():
             self._thread.join()
 
     def run(self):
         """Starts db server manager the engine."""
         with db_server_manager() as self._db_server_manager_queue:
             self._do_run()
 
     def _do_run(self):
         """Runs this engine."""
         self._state = SpineEngineState.RUNNING
-        run_config = {
-            "loggers": {"console": {"config": {"log_level": "CRITICAL"}}},
-            "execution": {"multithread": {"config": {}}},
-        }
-        for event in execute_pipeline_iterator(self._pipeline, run_config=run_config):
+        for event in execute_pipeline_iterator(self._pipeline):
             self._process_event(event)
         if self._state == SpineEngineState.RUNNING:
             self._state = SpineEngineState.COMPLETED
         self._queue.put(("dag_exec_finished", str(self._state)))
 
     def _process_event(self, event):
         """Processes events from a pipeline.
 
         Args:
-            event (DagsterEvent): an event
+            event (JumpsterEvent): an event
         """
-        if event.event_type == DagsterEventType.STEP_START:
-            direction, _, solid_name = event.solid_name.partition("_")
-            item_name = self._items_by_solids[solid_name]
-            self._queue.put(('exec_started', {"item_name": item_name, "direction": direction}))
-        elif event.event_type == DagsterEventType.STEP_FAILURE and self._state != SpineEngineState.USER_STOPPED:
-            direction, _, solid_name = event.solid_name.partition("_")
-            item_name = self._items_by_solids[solid_name]
+        if event.event_type == JumpsterEventType.STEP_START:
+            self._queue.put(("exec_started", {"item_name": event.item_name, "direction": event.direction}))
+        elif event.event_type == JumpsterEventType.STEP_FAILURE and self._state != SpineEngineState.USER_STOPPED:
             self._state = SpineEngineState.FAILED
             self._queue.put(
                 (
-                    'exec_finished',
+                    "exec_finished",
                     {
-                        "item_name": item_name,
-                        "direction": direction,
+                        "item_name": event.item_name,
+                        "direction": event.direction,
                         "state": str(self._state),
                         "item_state": ItemExecutionFinishState.FAILURE,
                     },
                 )
             )
             if self._debug:
-                error = event.event_specific_data.error
+                error = event.error
                 print("Traceback (most recent call last):")
                 print("".join(error.stack + [error.message]))
                 print("(reported by SpineEngine in debug mode)")
-        elif event.event_type == DagsterEventType.STEP_SUCCESS:
-            # Notify Toolbox here when BACKWARD execution has finished
-            direction, _, solid_name = event.solid_name.partition("_")
-            if direction != "BACKWARD":
-                return
-            item_name = self._items_by_solids[solid_name]
-            if not self._execution_permits[item_name]:
-                item_finish_state = ItemExecutionFinishState.EXCLUDED
-            else:
-                item_finish_state = ItemExecutionFinishState.SUCCESS
+        elif event.event_type == JumpsterEventType.STEP_FINISH:
             self._queue.put(
                 (
-                    'exec_finished',
+                    "exec_finished",
                     {
-                        "item_name": item_name,
-                        "direction": direction,
+                        "item_name": event.item_name,
+                        "direction": event.direction,
                         "state": str(self._state),
-                        "item_state": item_finish_state,
-                    },
-                )
-            )
-        elif event.event_type == DagsterEventType.ASSET_MATERIALIZATION:
-            # Notify Toolbox here when FORWARD execution has finished
-            direction, _, solid_name = event.solid_name.partition("_")
-            if direction != "FORWARD":
-                return
-            item_name = self._items_by_solids[solid_name]
-            state_value = event.asset_key.path[0]
-            item_finish_state = ItemExecutionFinishState[state_value]
-            self._queue.put(
-                (
-                    'exec_finished',
-                    {
-                        "item_name": item_name,
-                        "direction": direction,
-                        "state": str(self._state),
-                        "item_state": item_finish_state,
+                        "item_state": event.item_finish_state,
                     },
                 )
             )
 
     def stop(self):
         """Stops the engine."""
         self._state = SpineEngineState.USER_STOPPED
@@ -407,148 +351,119 @@
         self._queue.put(("dag_exec_finished", str(self._state)))
 
     def _stop_item(self, item):
         """Stops given project item."""
         item.stop_execution()
         self._queue.put(
             (
-                'exec_finished',
+                "exec_finished",
                 {
                     "item_name": item.name,
-                    "direction": str(ED.FORWARD),
+                    "direction": ED.FORWARD,
                     "state": str(self._state),
                     "item_state": ItemExecutionFinishState.STOPPED,
                 },
             )
         )
 
     def _make_pipeline(self):
-        """Returns a _JumpPipelineDefinition for executing this engine.
+        """Returns a PipelineDefinition for executing this engine.
 
         Returns:
-            _JumpPipelineDefinition
+            PipelineDefinition
         """
         solid_defs = [
             make_solid_def(item_name)
-            for item_name in self._dag_nodes
+            for item_name in self._item_names
             for make_solid_def in (self._make_forward_solid_def, self._make_backward_solid_def)
         ]
-        dependencies = self._make_dependencies()
-        mode_defs = [
-            ModeDefinition(
-                executor_defs=default_executors + [multithread_executor],
-                resource_defs={"io_manager": shared_memory_io_manager},
-            )
-        ]
         self._complete_jumps()
-        return _JumpPipelineDefinition(
-            name="pipeline", solid_defs=solid_defs, dependencies=dependencies, mode_defs=mode_defs, jumps=self._jumps
-        )
+        return PipelineDefinition(solid_defs=solid_defs, jumps=self._jumps)
 
     def _complete_jumps(self):
         """Updates jumps with item and corresponding solid information."""
         for jump in self._jumps:
             src, dst = jump.source, jump.destination
             jump.item_names = {dst, src}
             for path in nx.all_simple_paths(self._dag, dst, src):
                 jump.item_names.update(path)
-            jump.solid_names = {f"{ED.FORWARD}_{self._solids_by_items[n]}" for n in jump.item_names}
-            jump.source_solid = f"{ED.FORWARD}_{self._solids_by_items[src]}"
-            jump.destination_solid = f"{ED.BACKWARD}_{self._solids_by_items[dst]}"
 
     def _make_backward_solid_def(self, item_name):
         """Returns a SolidDefinition for executing the given item in the backward sweep.
 
         Args:
             item_name (str): The project item that gets executed by the solid.
 
         Returns:
             SolidDefinition: solid's definition
         """
 
-        def compute_fn(context, inputs):
+        def compute_fn(inputs):
             if self.state() == SpineEngineState.USER_STOPPED:
-                context.log.error(f"compute_fn() FAILURE with item: {item_name} stopped by the user")
                 raise Failure()
-            context.log.info(f"Item Name: {item_name}")
             item = self.make_item(item_name, ED.BACKWARD)
             resources = item.output_resources(ED.BACKWARD)
             for r in resources:
                 r.metadata["db_server_manager_queue"] = self._db_server_manager_queue
-            yield Output(value=resources, output_name=f"{ED.BACKWARD}_output")
+            yield Output(value=resources)
+            yield Finalization(
+                item_finish_state=ItemExecutionFinishState.SUCCESS
+                if self._execution_permits[item_name]
+                else ItemExecutionFinishState.EXCLUDED
+            )
 
-        input_defs = []
-        output_defs = [OutputDefinition(name=f"{ED.BACKWARD}_output")]
-        return SolidDefinition(
-            name=f"{ED.BACKWARD}_{self._solids_by_items[item_name]}",
-            input_defs=input_defs,
-            compute_fn=compute_fn,
-            output_defs=output_defs,
-        )
+        return SolidDefinition(item_name=item_name, direction=ED.BACKWARD, input_defs=[], compute_fn=compute_fn)
 
     def _make_forward_solid_def(self, item_name):
         """Returns a SolidDefinition for executing the given item.
 
         Args:
             item_name (str)
 
         Returns:
             SolidDefinition
         """
 
-        def compute_fn(context, inputs):
+        def compute_fn(inputs):
             if self.state() == SpineEngineState.USER_STOPPED:
-                context.log.error(f"compute_fn() FAILURE with item: {item_name} stopped by the user")
                 raise Failure()
-            context.log.info(f"Item Name: {item_name}")
             for conn in self._connections_by_destination.get(item_name, []):
                 conn.visit_destination()
             # Split inputs into forward and backward resources based on prefix
             forward_resource_stacks = []
             backward_resources = []
-            for name, values in inputs.items():
-                if name.startswith(f"{ED.FORWARD}"):
+            for direction, values in inputs.items():
+                if direction == ED.FORWARD:
                     forward_resource_stacks += values
-                elif name.startswith(f"{ED.BACKWARD}"):
+                elif direction == ED.BACKWARD:
                     backward_resources += values
             item_finish_state, output_resource_stacks = self._execute_item(
-                context, item_name, forward_resource_stacks, backward_resources
+                item_name, forward_resource_stacks, backward_resources
             )
-            yield AssetMaterialization(asset_key=str(item_finish_state))
             if output_resource_stacks:
-                yield Output(value=output_resource_stacks, output_name=f"{ED.FORWARD}_output")
+                yield Output(value=output_resource_stacks)
             for conn in self._connections_by_source.get(item_name, []):
                 conn.visit_source()
+            yield Finalization(item_finish_state=item_finish_state)
 
         input_defs = [
-            InputDefinition(name=f"{ED.FORWARD}_input_from_{inj}")
-            for inj in self._forth_injectors.get(self._solids_by_items[item_name], [])
-        ] + [
-            InputDefinition(name=f"{ED.BACKWARD}_input_from_{inj}")
-            for inj in self._back_injectors.get(self._solids_by_items[item_name], [])
-        ]
-        output_defs = [OutputDefinition(name=f"{ED.FORWARD}_output")]
-        return SolidDefinition(
-            name=f"{ED.FORWARD}_{self._solids_by_items[item_name]}",
-            input_defs=input_defs,
-            compute_fn=compute_fn,
-            output_defs=output_defs,
-        )
+            InputDefinition(item_name=inj, direction=ED.FORWARD) for inj in self._forth_injectors.get(item_name, [])
+        ] + [InputDefinition(item_name=inj, direction=ED.BACKWARD) for inj in self._back_injectors.get(item_name, [])]
+        return SolidDefinition(item_name=item_name, direction=ED.FORWARD, input_defs=input_defs, compute_fn=compute_fn)
 
-    def _execute_item(self, context, item_name, forward_resource_stacks, backward_resources):
+    def _execute_item(self, item_name, forward_resource_stacks, backward_resources):
         """Executes the given item using the given forward resource stacks and backward resources.
         Returns list of output resource stacks.
 
         Called by ``_make_forward_solid_def.compute_fn``.
 
         For each element yielded by ``_filtered_resources_iterator``, spawns a thread that runs
         ``_execute_item_filtered``.
 
         Args:
-            context
             item_name (str)
             forward_resource_stacks (list(tuple(ProjectItemResource))): resources coming from predecessor items -
                 one tuple of ProjectItemResource per item, where each element in the tuple corresponds to a filtered
                 execution of the item.
             backward_resources (list(ProjectItemResource)): resources coming from successor items - just one
                 resource per item.
 
@@ -556,15 +471,14 @@
             ItemExecutionFinishState
             list(tuple(ProjectItemResource))
         """
         item = self.make_item(item_name, ED.NONE)
         if not item.ready_to_execute(self._settings):
             if not self._execution_permits[item_name]:
                 return ItemExecutionFinishState.EXCLUDED, []
-            context.log.error(f"compute_fn() FAILURE with '{item_name}', not ready for forward execution")
             return ItemExecutionFinishState.FAILURE, []
         success = [ItemExecutionFinishState.NEVER_FINISHED]
         output_resources_list = []
         threads = []
         resources_iterator = self._filtered_resources_iterator(
             item_name, forward_resource_stacks, backward_resources, self._timestamp
         )
@@ -580,15 +494,14 @@
                 )
                 threads.append(thread)
             for thread in threads:
                 thread.start()
             for thread in threads:
                 thread.join()
         if success[0] == ItemExecutionFinishState.FAILURE:
-            context.log.error(f"compute_fn() FAILURE with {item_name}, failed to execute")
             raise Failure()
         for resources in output_resources_list:
             for connection in self._connections_by_source.get(item_name, []):
                 connection.receive_resources_from_source(resources)
         return success[0], output_resources_list
 
     def _execute_item_filtered(
@@ -731,16 +644,16 @@
         connection = next(iter(c for c in connections if c.source == provider_name), None)
         if connection is None:
             raise RuntimeError("Logic error: no connection from resource provider")
         filters = connection.enabled_filters(resource_label)
         if filters is None:
             return []
         filter_configs_list = []
-        for filter_type, names in filters.items():
-            filter_configs = [filter_config(filter_type, name) for name in names]
+        for filter_type, values in filters.items():
+            filter_configs = [filter_config(filter_type, value) for value in values]
             if not filter_configs:
                 continue
             filter_configs_list.append(filter_configs)
         return list(product(*filter_configs_list))
 
     def _convert_backward_resources(self, item_name, resources):
         """Converts resources as they're being passed backwards to given item.
@@ -787,41 +700,14 @@
         for c in connections:
             resources_from_source = resources_by_provider.get(c.source)
             if resources_from_source is None:
                 continue
             resources_by_provider[c.source] = c.convert_forward_resources(resources_from_source)
         return [r for resources in resources_by_provider.values() for r in resources]
 
-    def _make_dependencies(self):
-        """
-        Returns a dictionary of dependencies according to the given dictionaries of injectors.
-
-        Returns:
-            dict: a dictionary to pass to the PipelineDefinition constructor as dependencies
-        """
-        forward_deps = {
-            f"{ED.FORWARD}_{n}": {
-                f"{ED.FORWARD}_input_from_{inj}": DependencyDefinition(f"{ED.FORWARD}_{inj}", f"{ED.FORWARD}_output")
-                for inj in injs
-            }
-            for n, injs in self._forth_injectors.items()
-        }
-        backward_deps = {
-            f"{ED.FORWARD}_{n}": {
-                f"{ED.BACKWARD}_input_from_{inj}": DependencyDefinition(f"{ED.BACKWARD}_{inj}", f"{ED.BACKWARD}_output")
-                for inj in injs
-            }
-            for n, injs in self._back_injectors.items()
-        }
-        deps = {}
-        for n in forward_deps.keys() | backward_deps.keys():
-            deps[n] = forward_deps.get(n, {})
-            deps[n].update(backward_deps.get(n, {}))
-        return deps
-
 
 def _make_filter_id(resource_filter_stack):
     """Builds filter id from resource filter stack.
 
     Args:
         resource_filter_stack (dict): mapping from resource to filter stack
```

### Comparing `spine_engine-0.23.4/spine_engine/utils/__init__.py` & `spine_engine-0.24.0/spine_engine/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/utils/command_line_arguments.py` & `spine_engine-0.24.0/spine_engine/utils/command_line_arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-
-"""
-Split command line arguments.
-
-"""
+""" Split command line arguments. """
 
 
 def split_cmdline_args(arg_string):
     """
     Splits a string of command line arguments into a list of tokens.
 
     Things in single ('') and double ("") quotes are kept as single tokens
@@ -35,13 +32,13 @@
     for character in arg_string:
         if character in ("'", '"') and not quoted_context:
             quoted_context = character
         elif character == quoted_context:
             quoted_context = False
         elif not character.isspace() or quoted_context:
             current_word = current_word + character
-        else:
+        elif current_word:
             tokens.append(current_word)
             current_word = ""
     if current_word:
         tokens.append(current_word)
     return tokens
```

### Comparing `spine_engine-0.23.4/spine_engine/utils/execution_resources.py` & `spine_engine-0.24.0/spine_engine/utils/execution_resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/utils/helpers.py` & `spine_engine-0.24.0/spine_engine/utils/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Helpers functions and classes.
-
-"""
+"""Helper functions and classes."""
 import collections
 import os
 import sys
 import datetime
 import itertools
 import time
 import json
 from pathlib import Path
 from enum import Enum, auto, unique
 import networkx
 from jupyter_client.kernelspec import find_kernel_specs
 from spinedb_api.spine_io.gdx_utils import find_gams_directory
-from ..config import PYTHON_EXECUTABLE, JULIA_EXECUTABLE, GAMS_EXECUTABLE, EMBEDDED_PYTHON
+from ..config import PYTHON_EXECUTABLE, JULIA_EXECUTABLE, GAMS_EXECUTABLE, EMBEDDED_PYTHON, is_frozen
 
 
 @unique
 class ExecutionDirection(Enum):
     FORWARD = auto()
     BACKWARD = auto()
     NONE = auto()
@@ -57,22 +55,18 @@
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super().__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class AppSettings:
-    """
-    A QSettings replacement.
-    """
+    """A QSettings replacement."""
 
     def __init__(self, settings):
         """
-        Init.
-
         Args:
             settings (dict)
         """
         self._settings = settings
 
     def value(self, key, defaultValue=""):
         return self._settings.get(key, defaultValue)
@@ -109,46 +103,82 @@
     """
     if conda_path != "":
         return conda_path
     conda_exe = os.environ.get("CONDA_EXE", "")
     return conda_exe
 
 
-def resolve_python_interpreter(python_path):
-    """If given python_path is empty, returns the
-    full path to Python interpreter depending on user's
-    settings and whether the app is frozen or not.
-    """
-    if python_path != "":
-        return python_path
-    if not getattr(sys, "frozen", False):
-        return sys.executable  # Use current Python
-    # We are frozen
+def resolve_python_interpreter(settings):
+    """Returns a path to Python interpreter in settings or the current executable if none is set.
+
+    Args:
+        settings (AppSettings): settings
+
+    Returns:
+        str: path to Python interpreter
+    """
+    path = settings.value("appSettings/pythonPath")
+    if path:
+        return path
+    return resolve_current_python_interpreter()
+
+
+def resolve_current_python_interpreter():
+    """Returns a path to current Python interpreter.
+
+    Returns:
+        str: path to Python interpreter
+    """
+    if not is_frozen():
+        return sys.executable
     path = resolve_executable_from_path(PYTHON_EXECUTABLE)
     if path != "":
-        return path  # Use Python from PATH
-    return EMBEDDED_PYTHON  # Use embedded <app_install_dir>/Tools/python.exe
+        return path
+    return EMBEDDED_PYTHON
+
+
+def resolve_julia_executable(settings):
+    """Returns path to Julia executable from settings, and, if not set, path to default Julia executable.
 
+    Args:
+        settings (AppSettings): application settings
 
-def resolve_julia_executable(julia_path):
-    """if given julia_path is empty, tries to find the path to Julia
-    in user's PATH env variable. If Julia is not found in PATH,
-    returns an empty string.
-
-    Note: In the long run, we should decide whether this is something we want to do
-    because adding julia-x.x./bin/ dir to the PATH is not recommended because this
-    also exposes some .dlls to other programs on user's (windows) system. I.e. it
-    may break other programs, and this is why the Julia installer does not
-    add (and does not even offer the chance to add) Julia to PATH.
+    Returns:
+        str: path to Julia executable
+    """
+    path = settings.value("appSettings/juliaPath")
+    if path:
+        return path
+    return resolve_default_julia_executable()
+
+
+def resolve_default_julia_executable():
+    """Returns path to default Julia executable.
+
+    Tries to find the path to Julia in user's PATH env variable.
+    If Julia is not found in PATH, returns an empty string.
+
+    Returns:
+        str: path to Julia executable
     """
-    if julia_path != "":
-        return julia_path
     return resolve_executable_from_path(JULIA_EXECUTABLE)
 
 
+def resolve_julia_project(settings):
+    """Returns path to Julia environment (project) from settings or an empty string if not available.
+
+    Args:
+        settings (AppSettings): application settings
+
+    Returns:
+        str: path to Julia environment
+    """
+    return settings.value("appSettings/juliaProjectPath")
+
+
 def resolve_gams_executable(gams_path):
     """If given gams_path is empty, tries to find the path to GAMS executable.
 
     If GAMS is not found, returns an empty string.
 
     Args:
         gams_path (str): current path to GAMS executable
@@ -197,42 +227,24 @@
     output = dict()
     for key, value_list in input_.items():
         for value in value_list:
             output.setdefault(value, list()).append(key)
     return output
 
 
-def get_julia_command(settings):
-    """
-    Args:
-        settings (QSettings, AppSettings)
-
-    Returns:
-        list of str: e.g. ["path/to/julia", "--project=path/to/project/"]
-    """
-    env = get_julia_env(settings)
-    if env is None:
-        return None
-    julia, project = env
-    command = [julia]
-    if project:
-        command.append(f"--project={project}")
-    return command
-
-
 def get_julia_env(settings):
     """
     Args:
         settings (QSettings, AppSettings)
 
     Returns:
-        tuple, NoneType: (julia_exe, julia_project), or None if none found
+        Union[tuple, None]: (julia_exe, julia_project), or None if none found
     """
-    use_julia_kernel = settings.value("appSettings/useJuliaKernel", defaultValue="2") == "2"
-    if use_julia_kernel:
+    use_jupyter_console = settings.value("appSettings/useJuliaKernel", defaultValue="0") == "2"
+    if use_jupyter_console:
         kernel_name = settings.value("appSettings/juliaKernel", defaultValue="")
         resource_dir = find_kernel_specs().get(kernel_name)
         if resource_dir is None:
             return None
         filepath = os.path.join(resource_dir, "kernel.json")
         with open(filepath, "r") as fh:
             try:
@@ -527,7 +539,11 @@
         return self._count == number
 
     def __deepcopy__(self, memo):
         return self
 
     def __repr__(self):
         return str(self._count)
+
+
+def serializable_error_info_from_exc_info(exc_info):
+    return exc_info
```

### Comparing `spine_engine-0.23.4/spine_engine/utils/queue_logger.py` & `spine_engine-0.24.0/spine_engine/utils/queue_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 The QueueLogger class.
 
 """
+import time
 
 
 class _MessageBase:
     def __init__(self, queue, item_name, event_type):
         self._queue = queue
         self._event_type = event_type
         self._item_name = item_name
@@ -66,25 +68,30 @@
         """Don't emit anything"""
 
     def connect(self, *args, **kwargs):
         """Don't connect anything"""
 
 
 class _Prompt(_MessageBase):
+    _PENDING = object()
+
     def __init__(self, queue, item_name, prompt_queue, answered_prompts):
         super().__init__(queue, item_name, "prompt")
         self._prompt_queue = prompt_queue
         self._answered_prompts = answered_prompts
 
-    def emit(self, prompt):
-        prompt = {"item_name": self._item_name, **prompt}
-        key = str(prompt)
+    def emit(self, prompt_data):
+        key = str(prompt_data)
         if key not in self._answered_prompts:
+            self._answered_prompts[key] = self._PENDING
+            prompt = {"prompter_id": id(self._prompt_queue), "data": prompt_data}
             self._queue.put(("prompt", prompt))
             self._answered_prompts[key] = self._prompt_queue.get()
+        while self._answered_prompts[key] is self._PENDING:
+            time.sleep(0.02)
         return self._answered_prompts[key]
 
 
 class _Flash(_MessageBase):
     def __init__(self, queue, item_name):
         super().__init__(queue, item_name, "flash")
```

### Comparing `spine_engine-0.23.4/spine_engine/utils/returning_process.py` & `spine_engine-0.24.0/spine_engine/utils/returning_process.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine/utils/serialization.py` & `spine_engine-0.24.0/spine_engine/utils/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/spine_engine.egg-info/PKG-INFO` & `spine_engine-0.24.0/spine_engine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: spine_engine
-Version: 0.23.4
+Version: 0.24.0
 Summary: A package to run Spine workflows.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/spine-engine
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12,>=3.8.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
-Requires-Dist: dagster<0.12.9,>=0.12.6
 Requires-Dist: pendulum<3.0.0
 Requires-Dist: protobuf<3.21.0
 Requires-Dist: networkx>2.5.1
 Requires-Dist: datapackage<1.16,>=1.15.2
 Requires-Dist: jupyter_client>=6.0
-Requires-Dist: spinedb_api>=0.30.5
+Requires-Dist: spinedb_api>=0.31.0
 Requires-Dist: pyzmq>=21.0
 Requires-Dist: markupsafe<2.1
 Provides-Extra: dev
 Requires-Dist: coverage[toml]; extra == "dev"
 
 # Spine Engine
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: spine_engine Version: 0.23.4 Summary: A package to
+Metadata-Version: 2.1 Name: spine_engine Version: 0.24.0 Summary: A package to
 run Spine workflows. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/spine-engine Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: <3.12,>=3.8.1 Description-Content-Type: text/markdown License-File:
-COPYING License-File: COPYING.LESSER Requires-Dist: dagster<0.12.9,>=0.12.6
-Requires-Dist: pendulum<3.0.0 Requires-Dist: protobuf<3.21.0 Requires-Dist:
-networkx>2.5.1 Requires-Dist: datapackage<1.16,>=1.15.2 Requires-Dist:
-jupyter_client>=6.0 Requires-Dist: spinedb_api>=0.30.5 Requires-Dist:
-pyzmq>=21.0 Requires-Dist: markupsafe<2.1 Provides-Extra: dev Requires-Dist:
-coverage[toml]; extra == "dev" # Spine Engine [![Python](https://
-img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)]
-(https://www.python.org/downloads/release/python-379/) [![Unit tests](https://
-github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)](https://
-github.com/spine-tools/spine-engine/actions?query=workflow%3A"Unit+tests") [!
-[codecov](https://codecov.io/gh/spine-tools/spine-engine/branch/master/graph/
-badge.svg)](https://codecov.io/gh/spine-tools/spine-engine) [![PyPI version]
-(https://badge.fury.io/py/spine-engine.svg)](https://badge.fury.io/py/spine-
-engine) A Python package to coordinate the execution of [Spine Toolbox](https:/
-/github.com/spine-tools/Spine-Toolbox) workflows.
+COPYING License-File: COPYING.LESSER Requires-Dist: pendulum<3.0.0 Requires-
+Dist: protobuf<3.21.0 Requires-Dist: networkx>2.5.1 Requires-Dist:
+datapackage<1.16,>=1.15.2 Requires-Dist: jupyter_client>=6.0 Requires-Dist:
+spinedb_api>=0.31.0 Requires-Dist: pyzmq>=21.0 Requires-Dist: markupsafe<2.1
+Provides-Extra: dev Requires-Dist: coverage[toml]; extra == "dev" # Spine
+Engine [![Python](https://img.shields.io/badge/python-
+3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/
+downloads/release/python-379/) [![Unit tests](https://github.com/spine-tools/
+spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/
+spine-engine/actions?query=workflow%3A"Unit+tests") [![codecov](https://
+codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://
+codecov.io/gh/spine-tools/spine-engine) [![PyPI version](https://badge.fury.io/
+py/spine-engine.svg)](https://badge.fury.io/py/spine-engine) A Python package
+to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/
+Spine-Toolbox) workflows.
                                 [Spine Engine]
 ## License Spine Engine is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
 the [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/
 by-sa/4.0/). ## Getting started ### Installation To install Spine Engine into
 an existing Python environment, run $ pip install spine_engine ### Dependencies
 Spine Engine installation will install [dagster](https://
```

### Comparing `spine_engine-0.23.4/spine_engine.egg-info/SOURCES.txt` & `spine_engine-0.24.0/spine_engine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-.coveragerc
 .gitattributes
 .gitignore
 COPYING
 COPYING.LESSER
 README.md
 dev-requirements.txt
 pylintrc
 pyproject.toml
 .github/pull_request_template.md
 .github/workflows/run_unit_tests.yml
 bin/build_doc.bat
 bin/build_doc.py
-bin/update_copyrights.py
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/autoapi/index.rst
 docs/source/autoapi/spine_engine/index.rst
@@ -52,17 +50,17 @@
 docs/source/autoapi/spine_engine/version/index.rst
 fig/eu-emblem-low-res.jpg
 fig/spineengine_logo.svg
 fig/spineengine_on_wht.svg
 spine_engine/__init__.py
 spine_engine/config.py
 spine_engine/exception.py
+spine_engine/jumpster.py
 spine_engine/load_project_items.py
 spine_engine/project_item_loader.py
-spine_engine/shared_memory_io_manager.py
 spine_engine/spine_engine.py
 spine_engine/version.py
 spine_engine.egg-info/PKG-INFO
 spine_engine.egg-info/SOURCES.txt
 spine_engine.egg-info/dependency_links.txt
 spine_engine.egg-info/not-zip-safe
 spine_engine.egg-info/requires.txt
@@ -72,18 +70,14 @@
 spine_engine/execution_managers/conda_kernel_spec_runner.py
 spine_engine/execution_managers/execution_manager_base.py
 spine_engine/execution_managers/kernel_execution_manager.py
 spine_engine/execution_managers/persistent_execution_manager.py
 spine_engine/execution_managers/process_execution_manager.py
 spine_engine/execution_managers/spine_repl.jl
 spine_engine/execution_managers/spine_repl.py
-spine_engine/multithread_executor/__init__.py
-spine_engine/multithread_executor/executor.py
-spine_engine/multithread_executor/multithread.py
-spine_engine/multithread_executor/thread_executor.py
 spine_engine/project_item/__init__.py
 spine_engine/project_item/connection.py
 spine_engine/project_item/executable_item_base.py
 spine_engine/project_item/project_item_info.py
 spine_engine/project_item/project_item_resource.py
 spine_engine/project_item/project_item_specification.py
 spine_engine/project_item/project_item_specification_factory.py
@@ -123,22 +117,20 @@
 tests/mock_project_items/items_module/test_item/executable_item.py
 tests/mock_project_items/items_module/test_item/specification_factory.py
 tests/project_item/__init__.py
 tests/project_item/test_ExecutableItem.py
 tests/project_item/test_connection.py
 tests/project_item/test_project_item_resource.py
 tests/server/__init__.py
-tests/server/helloworld.zip
-tests/server/simple_importer.zip
 tests/server/test_EngineServer.py
 tests/server/test_PingService.py
 tests/server/test_ProjectExtractorService.py
 tests/server/test_ProjectRemoverService.py
-tests/server/test_RemoteExecutionService.py
 tests/server/test_start_server.py
+tests/server/zippedproject.zip
 tests/server/secfolder_for_tests/allowEndpoints.txt
 tests/server/secfolder_for_tests/certificates/.gitignore
 tests/server/secfolder_for_tests/private_keys/client.key_secret
 tests/server/secfolder_for_tests/private_keys/server.key_secret
 tests/server/secfolder_for_tests/public_keys/client.key
 tests/server/secfolder_for_tests/public_keys/server.key
 tests/server/util/__init__.py
```

### Comparing `spine_engine-0.23.4/tests/__init__.py` & `spine_engine-0.24.0/tests/execution_managers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-
-"""
-Init file for tests package. Intentionally empty.
-
-"""
+"""Unit tests for ``execution_managers`` package."""
```

### Comparing `spine_engine-0.23.4/tests/execution_managers/__init__.py` & `spine_engine-0.24.0/spine_engine/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
-# Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
-# Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
-# any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+# Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
+# General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
+# option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-"""Unit tests for ``execution_managers`` package."""
+
+from .spine_engine import SpineEngine, SpineEngineState
+from .utils.helpers import ExecutionDirection, ItemExecutionFinishState
+from .version import __version__
```

### Comparing `spine_engine-0.23.4/tests/execution_managers/test_persistent_execution_manager.py` & `spine_engine-0.24.0/tests/execution_managers/test_persistent_execution_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/tests/execution_managers/test_process_execution_manager.py` & `spine_engine-0.24.0/tests/execution_managers/test_process_execution_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -11,60 +12,60 @@
 """Unit tests for ``process_execution_manager`` module."""
 import unittest
 from unittest.mock import MagicMock
 from tempfile import TemporaryDirectory
 from spine_engine.execution_managers.process_execution_manager import ProcessExecutionManager
 
 
-class TestStandardExecutionManager(unittest.TestCase):
+class TestProcessExecutionManager(unittest.TestCase):
     def test_run(self):
         logger = MagicMock()
         logger.msg_proc = MagicMock()
         logger.msg_proc.attach_mock(MagicMock(), "emit")
-        exec_manager = ProcessExecutionManager(logger, "python", "-c", "print('hello')")
+        exec_manager = ProcessExecutionManager(logger, "python", ["-c", "print('hello')"])
         ret = exec_manager.run_until_complete()
         logger.msg_proc.emit.assert_called_once()
         logger.msg_proc.emit.assert_called_with("hello")
         self.assertEqual(ret, 0)
 
     def test_run_with_error(self):
         logger = MagicMock()
         logger.msg_proc_error = MagicMock()
         logger.msg_proc_error.attach_mock(MagicMock(), "emit")
-        exec_manager = ProcessExecutionManager(logger, "python", "-c", "gibberish")
+        exec_manager = ProcessExecutionManager(logger, "python", ["-c", "gibberish"])
         ret = exec_manager.run_until_complete()
         logger.msg_proc_error.emit.assert_called_with("NameError: name 'gibberish' is not defined")
         self.assertEqual(ret, 1)
 
     def test_run_unknown_program(self):
         logger = MagicMock()
         logger.msg_proc = MagicMock()
         logger.msg_proc_error = MagicMock()
         logger.msg_standard_execution = MagicMock()
         logger.msg_proc.attach_mock(MagicMock(), "emit")
         logger.msg_proc_error.attach_mock(MagicMock(), "emit")
         logger.msg_standard_execution.attach_mock(MagicMock(), "emit")
-        exec_manager = ProcessExecutionManager(logger, "unknown_program")
+        exec_manager = ProcessExecutionManager(logger, "unknown_program", [])
         ret = exec_manager.run_until_complete()
         logger.msg_proc.emit.assert_not_called()
         logger.msg_proc_error.emit.assert_not_called()
         logger.msg_standard_execution.emit.assert_called_once()
         self.assertEqual(ret, 1)
 
     def test_run_with_workdir(self):
         logger = MagicMock()
         logger.msg_proc = MagicMock()
         logger.msg_proc.attach_mock(MagicMock(), "emit")
         logger.msg_proc_error = MagicMock()
         logger.msg_proc_error.attach_mock(MagicMock(), "emit")
         with TemporaryDirectory() as workdir:
             exec_manager = ProcessExecutionManager(
-                logger, "python", "-c", "import os; print(os.getcwd())", workdir=workdir
+                logger, "python", ["-c", "import os; print(os.getcwd())"], workdir=workdir
             )
             ret = exec_manager.run_until_complete()
         logger.msg_proc.emit.assert_called_once()
         logger.msg_proc.emit.assert_called_with(f"{workdir}")
         self.assertEqual(ret, 0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/project_item/test_ExecutableItem.py` & `spine_engine-0.24.0/tests/project_item/test_ExecutableItem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Toolbox.
 # Spine Toolbox is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/tests/project_item/test_connection.py` & `spine_engine-0.24.0/tests/project_item/test_connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-"""
-Uni tests for the ``connection`` module.
-
-"""
+""" Uni tests for the ``connection`` module. """
 import os.path
 from tempfile import TemporaryDirectory
 import unittest
 from unittest.mock import Mock
-from spinedb_api import DatabaseMapping, import_scenarios, import_tools, import_alternatives, import_object_classes
-from spine_engine.project_item.connection import Connection, FilterSettings, Jump, ResourceConvertingConnection
+from spinedb_api import DatabaseMapping, import_entity_classes, import_scenarios, import_alternatives
+from spine_engine.project_item.connection import Connection, FilterSettings, Jump
 from spine_engine.project_item.project_item_resource import database_resource
-from spine_engine.spine_engine import SpineEngine
 from spinedb_api.filters.scenario_filter import SCENARIO_FILTER_TYPE
-from spinedb_api.filters.tool_filter import TOOL_FILTER_TYPE
 
 
 class TestConnection(unittest.TestCase):
     def test_serialization_without_filters(self):
         connection = Connection("source", "bottom", "destination", "top", {"option": 23})
         connection_dict = connection.to_dict()
         restored = Connection.from_dict(connection_dict)
@@ -53,38 +49,33 @@
         self.assertTrue(connection.ready_to_execute())
 
     def test_require_filter_online(self):
         options = {"require_" + SCENARIO_FILTER_TYPE: True}
         filter_settings = FilterSettings({"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}}})
         connection = Connection("source", "bottom", "destination", "top", options, filter_settings)
         self.assertTrue(connection.require_filter_online(SCENARIO_FILTER_TYPE))
-        self.assertFalse(connection.require_filter_online(TOOL_FILTER_TYPE))
 
     def test_require_filter_online_default_value(self):
         filter_settings = FilterSettings({"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}}})
         connection = Connection("source", "bottom", "destination", "top", {}, filter_settings)
         self.assertIsNotNone(connection.require_filter_online(SCENARIO_FILTER_TYPE))
-        self.assertIsNotNone(connection.require_filter_online(TOOL_FILTER_TYPE))
         self.assertFalse(connection.require_filter_online(SCENARIO_FILTER_TYPE))
-        self.assertFalse(connection.require_filter_online(TOOL_FILTER_TYPE))
 
     def test_notification_when_filter_validation_fails(self):
-        options = {"require_" + SCENARIO_FILTER_TYPE: True, "require_" + TOOL_FILTER_TYPE: True}
+        options = {"require_" + SCENARIO_FILTER_TYPE: True}
         filter_settings = FilterSettings(auto_online=False)
         connection = Connection("source", "bottom", "destination", "top", options, filter_settings)
         self.assertEqual(
             connection.notifications(),
-            ["At least one scenario filter must be active.", "At least one tool filter must be active."],
+            ["At least one scenario filter must be active."],
         )
 
     def test_nothing_to_notify(self):
-        filter_settings = FilterSettings(
-            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}, TOOL_FILTER_TYPE: {"tool_1": True}}}
-        )
-        options = {"require_" + SCENARIO_FILTER_TYPE: True, "require_" + TOOL_FILTER_TYPE: True}
+        filter_settings = FilterSettings({"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}}})
+        options = {"require_" + SCENARIO_FILTER_TYPE: True}
         connection = Connection("source", "bottom", "destination", "top", options, filter_settings)
         self.assertEqual(connection.notifications(), [])
 
     def test_emtpy_notifications_when_scenario_filter_is_automatically_online(self):
         options = {"require_scenario_filter": True}
         connection = Connection("A", "bottom", "B", "top", options)
         notifications = connection.notifications()
@@ -94,15 +85,15 @@
 class TestConnectionWithDatabase(unittest.TestCase):
     def setUp(self):
         self._temp_dir = TemporaryDirectory()
         self._url = "sqlite:///" + os.path.join(self._temp_dir.name, "db.sqlite")
         self._db_map = DatabaseMapping(self._url, create=True)
 
     def tearDown(self):
-        self._db_map.connection.close()
+        self._db_map.close()
         self._temp_dir.cleanup()
 
     def test_serialization_with_filters(self):
         import_scenarios(self._db_map, ("my_scenario",))
         self._db_map.commit_session("Add test data.")
         filter_settings = FilterSettings(
             {"my_database": {"scenario_filter": {"my_scenario": False}}}, auto_online=False
@@ -132,54 +123,36 @@
         self._db_map.commit_session("Add test data.")
         filter_settings = FilterSettings({"my_database": {"scenario_filter": {"scenario_1": True}}}, auto_online=False)
         connection = Connection("source", "bottom", "destination", "top", filter_settings=filter_settings)
         resources = [database_resource("unit_test", self._url, "my_database", filterable=True)]
         connection.receive_resources_from_source(resources)
         self.assertEqual(connection.enabled_filters("my_database"), {"scenario_filter": ["scenario_1"]})
 
-    def test_enabled_tools_with_auto_enable_on(self):
-        import_tools(self._db_map, ("tool_1", "tool_2"))
-        self._db_map.commit_session("Add test data.")
-        filter_settings = FilterSettings({"my_database": {"tool_filter": {"tool_1": False}}})
-        connection = Connection("source", "bottom", "destination", "top", filter_settings=filter_settings)
-        resources = [database_resource("unit_test", self._url, "my_database", filterable=True)]
-        connection.receive_resources_from_source(resources)
-        self.assertEqual(connection.enabled_filters("my_database"), {"tool_filter": ["tool_2"]})
-
-    def test_enabled_tools_with_auto_enable_off(self):
-        import_tools(self._db_map, ("tool_1", "tool_2"))
-        self._db_map.commit_session("Add test data.")
-        filter_settings = FilterSettings({"my_database": {"tool_filter": {"tool_1": True}}}, auto_online=False)
-        connection = Connection("source", "bottom", "destination", "top", filter_settings=filter_settings)
-        resources = [database_resource("unit_test", self._url, "my_database", filterable=True)]
-        connection.receive_resources_from_source(resources)
-        self.assertEqual(connection.enabled_filters("my_database"), {"tool_filter": ["tool_1"]})
-
     def test_purge_data_before_writing(self):
         import_alternatives(self._db_map, ("my_alternative",))
-        import_object_classes(self._db_map, ("my_object_class",))
+        import_entity_classes(self._db_map, ("my_object_class",))
         self._db_map.commit_session("Add test data.")
-        self._db_map.connection.close()
+        self._db_map.close()
         connection = Connection(
             "source",
             "bottom",
             "destination",
             "top",
-            options={"purge_before_writing": True, "purge_settings": {"object_class": True}},
+            options={"purge_before_writing": True, "purge_settings": {"entity_class": True}},
         )
         resources = [database_resource("unit_test", self._url, "my_database")]
         connection.clean_up_backward_resources(resources)
         database_map = DatabaseMapping(self._url)
-        object_class_list = database_map.query(database_map.object_class_sq).all()
-        self.assertEqual(len(object_class_list), 0)
+        entity_class_list = database_map.query(database_map.entity_class_sq).all()
+        self.assertEqual(len(entity_class_list), 0)
         alternative_list = database_map.query(database_map.alternative_sq).all()
         self.assertEqual(len(alternative_list), 2)
         self.assertEqual(alternative_list[0].name, "Base")
         self.assertEqual(alternative_list[1].name, "my_alternative")
-        database_map.connection.close()
+        database_map.close()
 
 
 class TestJump(unittest.TestCase):
     def test_default_condition_prevents_jump(self):
         jump = Jump("source", "bottom", "destination", "top")
         self.assertFalse(jump.is_condition_true(1))
 
@@ -192,41 +165,14 @@
             "type": "python-script",
             "script": "\n".join(("import sys", "counter = int(sys.argv[1])", "exit(0 if counter == 23 else 1)")),
         }
         jump = Jump("source", "bottom", "destination", "top", condition)
         jump.make_logger(Mock())
         self.assertTrue(jump.is_condition_true(23))
 
-    @unittest.skip("Doesn't work in github actions: ModuleNotFoundError: No module named 'spine_items'")
-    def test_tool_spec_condition(self):
-        condition = {"type": "tool-specification", "specification": "loop_twice"}
-        jump = Jump("source", "bottom", "destination", "top", condition)
-        jump.make_logger(Mock())
-        with TemporaryDirectory() as temp_dir:
-            main_program_file_path = "script"
-            temp_file_path = os.path.join(temp_dir, main_program_file_path)
-            with open(temp_file_path, "w+") as program_file:
-                program_file.write('if ARGS[1] == "23" exit(0) else exit(1) end')
-            engine = SpineEngine(
-                settings={"appSettings/useJuliaKernel": "1"},
-                project_dir=temp_dir,
-                specifications={
-                    "Tool": [
-                        {
-                            "name": "loop_twice",
-                            "tooltype": "julia",
-                            "includes_main_path": temp_dir,
-                            "includes": [main_program_file_path],
-                        }
-                    ]
-                },
-            )
-            jump.prepare_condition(engine)
-            self.assertTrue(jump.is_condition_true(23))
-
     def test_dictionary(self):
         jump = Jump("source", "bottom", "destination", "top", {"type": "python-script", "script": "exit(23)"})
         jump_dict = jump.to_dict()
         new_jump = Jump.from_dict(jump_dict)
         self.assertEqual(new_jump.source, jump.source)
         self.assertEqual(new_jump.destination, jump.destination)
         self.assertEqual(new_jump.source_position, jump.source_position)
@@ -236,46 +182,59 @@
 
 class TestFilterSettings(unittest.TestCase):
     def test_has_filters_returns_false_when_no_filters_exist(self):
         settings = FilterSettings()
         self.assertFalse(settings.has_filters())
 
     def test_has_filters_returns_true_when_filters_exist(self):
-        settings = FilterSettings({"database@Data Store": {TOOL_FILTER_TYPE: {"tool_1": True}}})
+        settings = FilterSettings({"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}}})
         self.assertTrue(settings.has_filters())
 
+    def test_has_filters_returns_false_when_filter_type_is_disabled(self):
+        settings = FilterSettings(
+            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}}},
+            enabled_filter_types={SCENARIO_FILTER_TYPE: False},
+        )
+        self.assertFalse(settings.has_filters())
+
     def test_has_filters_online_returns_false_when_no_filters_exist(self):
         settings = FilterSettings()
         self.assertFalse(settings.has_filter_online(SCENARIO_FILTER_TYPE))
 
     def test_has_filters_online_returns_false_when_filters_are_offline(self):
-        settings = FilterSettings(
-            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}, TOOL_FILTER_TYPE: {"tool_1": False}}}
-        )
-        self.assertFalse(settings.has_filter_online(TOOL_FILTER_TYPE))
+        settings = FilterSettings({"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": False}}})
+        self.assertFalse(settings.has_filter_online(SCENARIO_FILTER_TYPE))
 
     def test_has_filters_online_returns_true_when_filters_are_online(self):
-        settings = FilterSettings(
-            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": False}, TOOL_FILTER_TYPE: {"tool_1": True}}}
-        )
-        self.assertTrue(settings.has_filter_online(TOOL_FILTER_TYPE))
+        settings = FilterSettings({"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}}})
+        self.assertTrue(settings.has_filter_online(SCENARIO_FILTER_TYPE))
 
     def test_has_filter_online_works_when_there_are_no_known_filters(self):
         settings = FilterSettings()
         self.assertFalse(settings.has_filter_online(SCENARIO_FILTER_TYPE))
-        self.assertFalse(settings.has_filter_online(TOOL_FILTER_TYPE))
+
+    def test_has_any_filter_online_returns_false_when_no_filters_exist(self):
+        settings = FilterSettings()
+        self.assertFalse(settings.has_any_filter_online())
+
+    def test_has_any_filter_online_returns_false_when_filter_type_is_disabled(self):
+        settings = FilterSettings(
+            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": True}}},
+            enabled_filter_types={SCENARIO_FILTER_TYPE: False},
+        )
+        self.assertFalse(settings.has_any_filter_online())
 
     def test_has_any_filter_online_returns_true_when_filters_are_online(self):
         settings = FilterSettings(
-            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": False}, TOOL_FILTER_TYPE: {"tool_1": True}}}
+            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": False, "scenario_2": True}}}
         )
         self.assertTrue(settings.has_any_filter_online())
 
     def test_has_any_filter_online_returns_false_when_all_filters_are_offline(self):
         settings = FilterSettings(
-            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": False}, TOOL_FILTER_TYPE: {"tool_1": False}}}
+            {"database@Data Store": {SCENARIO_FILTER_TYPE: {"scenario_1": False, "scenario_2": False}}}
         )
         self.assertFalse(settings.has_any_filter_online())
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/project_item/test_project_item_resource.py` & `spine_engine-0.24.0/tests/project_item/test_project_item_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -133,14 +134,25 @@
 
 
 class TestURLResource(unittest.TestCase):
     def test_schema_is_stored_in_metadata(self):
         resource = url_resource("project item", "sqlite:///path/do/db.sqlite", "my database", schema="my_schema")
         self.assertEqual(resource.metadata, {"schema": "my_schema"})
 
+    def test_url_setter_works_when_url_is_set_to_none(self):
+        resource = url_resource("project item", "sqlite:///path/do/db.sqlite", "my database")
+        resource.url = None
+        self.assertIsNone(resource.url)
+
+
+class TestTransientFileResource(unittest.TestCase):
+    def test_path_works_even_when_resource_has_no_url(self):
+        resource = transient_file_resource("Provider", "files@Provider")
+        self.assertEqual(resource.path, "")
+
 
 class TestGetSource(unittest.TestCase):
     def test_file_resource(self):
         resource = file_resource("project item", "/path/to/file")
         self.assertEqual(get_source(resource), str(Path("/", "path", "to", "file").resolve()))
 
     def test_url_resource(self):
@@ -170,9 +182,9 @@
         self.assertEqual(get_source_extras(resource), {"schema": None})
 
     def test_transient_file_resource(self):
         resource = transient_file_resource("project item", "non-existent")
         self.assertEqual(get_source_extras(resource), {})
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/server/__init__.py` & `spine_engine-0.24.0/tests/server/util/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-
-"""
-Init file for spine_engine.tests.server package.
-"""
```

### Comparing `spine_engine-0.23.4/tests/server/helloworld.zip` & `spine_engine-0.24.0/tests/server/zippedproject.zip`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/tests/server/test_EngineServer.py` & `spine_engine-0.24.0/tests/server/test_EngineServer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/tests/server/test_PingService.py` & `spine_engine-0.24.0/tests/server/test_PingService.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #####################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/tests/server/test_ProjectExtractorService.py` & `spine_engine-0.24.0/tests/server/test_ProjectExtractorService.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #####################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -42,45 +43,45 @@
 
     @mock.patch(
         "spine_engine.server.project_extractor_service.ProjectExtractorService.INTERNAL_PROJECT_DIR",
         new_callable=mock.PropertyMock,
     )
     def test_project_extraction(self, mock_proj_dir):
         mock_proj_dir.return_value = self._temp_dir.name
-        with open(os.path.join(str(Path(__file__).parent), "helloworld.zip"), "rb") as f:
+        with open(os.path.join(str(Path(__file__).parent), "zippedproject.zip"), "rb") as f:
             file_data = f.read()
-        msg = ServerMessage("prepare_execution", "1", json.dumps("helloworld"), ["helloworld.zip"])
+        msg = ServerMessage("prepare_execution", "1", json.dumps("project_name"), ["zippedproject.zip"])
         self.socket.send_multipart([msg.to_bytes(), file_data])
         response = self.socket.recv_multipart()
         response_msg = ServerMessage.parse(response[1])
         self.assertEqual("prepare_execution", response_msg.getCommand())
         self.assertTrue(len(response_msg.getId()) == 32)
         self.assertEqual("", response_msg.getData())
 
     def test_project_file_name_missing(self):
         """File name list in request is empty."""
-        with open(os.path.join(str(Path(__file__).parent), "helloworld.zip"), "rb") as f:
+        with open(os.path.join(str(Path(__file__).parent), "zippedproject.zip"), "rb") as f:
             file_data = f.read()
-        msg = ServerMessage("prepare_execution", "1", json.dumps("helloworld"), [])
+        msg = ServerMessage("prepare_execution", "1", json.dumps("project_name"), [])
         self.socket.send_multipart([msg.to_bytes(), file_data])
         response = self.socket.recv_multipart()
         self.check_correct_error_response(response[1], "Project ZIP file name missing")
 
     def test_project_name_missing(self):
         """Project name missing from request."""
-        with open(os.path.join(str(Path(__file__).parent), "helloworld.zip"), "rb") as f:
+        with open(os.path.join(str(Path(__file__).parent), "zippedproject.zip"), "rb") as f:
             data_file = f.read()
-        msg = ServerMessage("prepare_execution", "1", "", ["helloworld.zip"])
+        msg = ServerMessage("prepare_execution", "1", "", ["zippedproject.zip"])
         self.socket.send_multipart([msg.to_bytes(), data_file])
         response = self.socket.recv_multipart()
         self.check_correct_error_response(response[1], "Project name missing")
 
     def test_zip_file_missing(self):
         """Project zip-file missing from request."""
-        msg = ServerMessage("prepare_execution", "1", json.dumps("projekti"), ["helloworld.zip"])
+        msg = ServerMessage("prepare_execution", "1", json.dumps("project_name"), ["missing_zip_file.zip"])
         self.socket.send_multipart([msg.to_bytes()])
         response = self.socket.recv_multipart()
         self.check_correct_error_response(response[1], "Project ZIP file missing")
 
     def check_correct_error_response(self, response, expected_err_str):
         response_msg = ServerMessage.parse(response)
         self.assertEqual("prepare_execution", response_msg.getCommand())
```

### Comparing `spine_engine-0.23.4/tests/server/test_ProjectRemoverService.py` & `spine_engine-0.24.0/tests/server/test_ProjectRemoverService.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #####################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -34,17 +35,17 @@
         if not self.socket.closed:
             self.socket.close()
         if not self.context.closed:
             self.context.term()
 
     def test_remove_project_service(self):
         """Extracts a project into received_projects folder, then removes it using the ProjectRemoverService."""
-        with open(os.path.join(str(Path(__file__).parent), "helloworld.zip"), "rb") as f:
+        with open(os.path.join(str(Path(__file__).parent), "zippedproject.zip"), "rb") as f:
             file_data = f.read()
-        msg = ServerMessage("prepare_execution", "1", json.dumps("helloworld"), ["helloworld.zip"])
+        msg = ServerMessage("prepare_execution", "1", json.dumps("project_name"), ["zippedproject.zip"])
         self.socket.send_multipart([msg.to_bytes(), file_data])
         r1 = self.socket.recv_multipart()
         r1_msg = ServerMessage.parse(r1[1])
         self.assertEqual("prepare_execution", r1_msg.getCommand())
         self.assertTrue(len(r1_msg.getId()) == 32)
         self.assertEqual("", r1_msg.getData())
         job_id = r1_msg.getId()
```

### Comparing `spine_engine-0.23.4/tests/server/test_start_server.py` & `spine_engine-0.24.0/tests/server/test_start_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #####################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `spine_engine-0.23.4/tests/server/util/__init__.py` & `spine_engine-0.24.0/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
+
+"""
+Init file for tests package. Intentionally empty.
+
+"""
```

### Comparing `spine_engine-0.23.4/tests/server/util/projectforpackagingtests/.spinetoolbox/project.json` & `spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spine_engine-0.23.4/tests/server/util/test_EventDataConverter.py` & `spine_engine-0.24.0/tests/server/util/test_EventDataConverter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,148 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Unit tests for EventDataConverter class.
-"""
-
+"""Unit tests for EventDataConverter class."""
 import unittest
 from copy import deepcopy
 from spine_engine.spine_engine import ItemExecutionFinishState
 from spine_engine.server.util.event_data_converter import EventDataConverter
+from spine_engine.utils.helpers import ExecutionDirection
 
 
 class TestEventDataConverter(unittest.TestCase):
     def make_event_data(self):
         test_events = [
-            ('exec_started', {'item_name': 'helloworld', 'direction': 'BACKWARD'}),
-            ('exec_started', {'item_name': 'Data Connection 1', 'direction': 'BACKWARD'}),
+            ("exec_started", {"item_name": "helloworld", "direction": ExecutionDirection.BACKWARD}),
+            ("exec_started", {"item_name": "Data Connection 1", "direction": ExecutionDirection.BACKWARD}),
             (
-                'exec_finished',
+                "exec_finished",
                 {
-                    'item_name': 'helloworld',
-                    'direction': 'BACKWARD',
-                    'state': 'RUNNING',
-                    'item_state': ItemExecutionFinishState.SUCCESS,
+                    "item_name": "helloworld",
+                    "direction": ExecutionDirection.BACKWARD,
+                    "state": "RUNNING",
+                    "item_state": ItemExecutionFinishState.SUCCESS,
                 },
             ),
             (
-                'exec_finished',
+                "exec_finished",
                 {
-                    'item_name': 'Data Connection 1',
-                    'direction': 'BACKWARD',
-                    'state': 'RUNNING',
-                    'item_state': ItemExecutionFinishState.SUCCESS,
+                    "item_name": "Data Connection 1",
+                    "direction": ExecutionDirection.BACKWARD,
+                    "state": "RUNNING",
+                    "item_state": ItemExecutionFinishState.SUCCESS,
                 },
             ),
-            ('exec_started', {'item_name': 'Data Connection 1', 'direction': 'FORWARD'}),
+            ("exec_started", {"item_name": "Data Connection 1", "direction": ExecutionDirection.FORWARD}),
             (
-                'event_msg',
+                "event_msg",
                 {
-                    'item_name': 'Data Connection 1',
-                    'filter_id': '',
-                    'msg_type': 'msg_success',
-                    'msg_text': 'Executing Data Connection Data Connection 1 finished',
+                    "item_name": "Data Connection 1",
+                    "filter_id": "",
+                    "msg_type": "msg_success",
+                    "msg_text": "Executing Data Connection Data Connection 1 finished",
                 },
             ),
             (
-                'exec_finished',
+                "exec_finished",
                 {
-                    'item_name': 'Data Connection 1',
-                    'direction': 'FORWARD',
-                    'state': 'RUNNING',
-                    'item_state': ItemExecutionFinishState.SUCCESS,
+                    "item_name": "Data Connection 1",
+                    "direction": ExecutionDirection.FORWARD,
+                    "state": "RUNNING",
+                    "item_state": ItemExecutionFinishState.SUCCESS,
                 },
             ),
-            ('flash', {'item_name': 'from Data Connection 1 to helloworld'}),
-            ('exec_started', {'item_name': 'helloworld', 'direction': 'FORWARD'}),
+            ("flash", {"item_name": "from Data Connection 1 to helloworld"}),
+            ("exec_started", {"item_name": "helloworld", "direction": ExecutionDirection.FORWARD}),
             (
-                'event_msg',
+                "event_msg",
                 {
-                    'item_name': 'helloworld',
-                    'filter_id': '',
-                    'msg_type': 'msg',
-                    'msg_text': "*** Executing Tool specification <b>helloworld2</b> in <a style='color:#99CCFF;' title='C:\\data\\GIT\\SPINEENGINE\\spine_engine\\server\\received_projects\\helloworld__35bc62cea0324e8788144ce81342f4f1'href='file:///C:\\data\\GIT\\SPINEENGINE\\spine_engine\\server\\received_projects\\helloworld__35bc62cea0324e8788144ce81342f4f1'>source directory</a> ***",
+                    "item_name": "helloworld",
+                    "filter_id": "",
+                    "msg_type": "msg",
+                    "msg_text": "*** Executing Tool specification <b>helloworld2</b> in <a style='color:#99CCFF;' title='C:\\data\\GIT\\SPINEENGINE\\spine_engine\\server\\received_projects\\helloworld__35bc62cea0324e8788144ce81342f4f1'href='file:///C:\\data\\GIT\\SPINEENGINE\\spine_engine\\server\\received_projects\\helloworld__35bc62cea0324e8788144ce81342f4f1'>source directory</a> ***",
                 },
             ),
             (
-                'persistent_execution_msg',
+                "persistent_execution_msg",
                 {
-                    'item_name': 'helloworld',
-                    'filter_id': '',
-                    'type': 'persistent_started',
-                    'key': '6ceeb59271114fc2a0f787266f72dedc',
-                    'language': 'python',
+                    "item_name": "helloworld",
+                    "filter_id": "",
+                    "type": "persistent_started",
+                    "key": "6ceeb59271114fc2a0f787266f72dedc",
+                    "language": "python",
                 },
             ),
             (
-                'persistent_execution_msg',
-                {'item_name': 'helloworld', 'filter_id': '', 'type': 'stdin', 'data': '# Running python helloworld.py'},
+                "persistent_execution_msg",
+                {"item_name": "helloworld", "filter_id": "", "type": "stdin", "data": "# Running python helloworld.py"},
             ),
             (
-                'persistent_execution_msg',
-                {'item_name': 'helloworld', 'filter_id': '', 'type': 'stdout', 'data': 'helloo'},
+                "persistent_execution_msg",
+                {"item_name": "helloworld", "filter_id": "", "type": "stdout", "data": "helloo"},
             ),
             (
-                'event_msg',
+                "event_msg",
                 {
-                    'item_name': 'helloworld',
-                    'filter_id': '',
-                    'msg_type': 'msg',
-                    'msg_text': "*** Archiving output files to <a style='color:#BB99FF;' title='C:\\data\\GIT\\SPINEENGINE\\spine_engine\\server\\received_projects\\helloworld__35bc62cea0324e8788144ce81342f4f1\\.spinetoolbox\\items\\helloworld\\output\\2022-08-19T13.03.13' href='file:///C:\\data\\GIT\\SPINEENGINE\\spine_engine\\server\\received_projects\\helloworld__35bc62cea0324e8788144ce81342f4f1\\.spinetoolbox\\items\\helloworld\\output\\2022-08-19T13.03.13'>results directory</a> ***",
+                    "item_name": "helloworld",
+                    "filter_id": "",
+                    "msg_type": "msg",
+                    "msg_text": "*** Archiving output files to <a style='color:#BB99FF;' title='C:\\data\\GIT\\SPINEENGINE\\spine_engine\\server\\received_projects\\helloworld__35bc62cea0324e8788144ce81342f4f1\\.spinetoolbox\\items\\helloworld\\output\\2022-08-19T13.03.13' href='file:///C:\\data\\GIT\\SPINEENGINE\\spine_engine\\server\\received_projects\\helloworld__35bc62cea0324e8788144ce81342f4f1\\.spinetoolbox\\items\\helloworld\\output\\2022-08-19T13.03.13'>results directory</a> ***",
                 },
             ),
             (
-                'exec_finished',
+                "exec_finished",
                 {
-                    'item_name': 'helloworld',
-                    'direction': 'FORWARD',
-                    'state': 'RUNNING',
-                    'item_state': ItemExecutionFinishState.SUCCESS,
+                    "item_name": "helloworld",
+                    "direction": ExecutionDirection.FORWARD,
+                    "state": "RUNNING",
+                    "item_state": ItemExecutionFinishState.SUCCESS,
                 },
             ),
-            ('dag_exec_finished', 'COMPLETED'),
+            ("dag_exec_finished", "COMPLETED"),
         ]
         return test_events
 
     def test_convert(self):
         event_data = self.make_event_data()
         converted_events = list()
         for event in event_data:
             json_str = EventDataConverter.convert(event[0], event[1])
             converted_events.append(json_str)
         self.assertEqual(16, len(converted_events))
         # Check that item_state values are cast to strings i.e. ItemExecutionFinishState.SUCCESS -> "SUCCESS"
-        n = 0  # Counter for how many ItemExecutionFinishStates were cast to strings
+        item_execution_finish_states_converted = 0
+        # Check that direction values are cast to strings i.e. ExecutionDirection.FORWARD -> "FORWARD"
+        execution_direction_backward_converted = 0
+        execution_direction_forward_converted = 0
         for converted_event in converted_events:
-            if converted_event.startswith('{"event_type": "exec_finished"'):
+            if converted_event.startswith('{"event_type": "exec_started"'):
+                if '"direction": "BACKWARD"' in converted_event:
+                    execution_direction_backward_converted += 1
+                elif '"direction": "FORWARD"' in converted_event:
+                    execution_direction_forward_converted += 1
+            elif converted_event.startswith('{"event_type": "exec_finished"'):
                 self.assertTrue('"item_state": "SUCCESS"' in converted_event)
-                n += 1
-        self.assertEqual(4, n)
+                item_execution_finish_states_converted += 1
+                if '"direction": "BACKWARD"' in converted_event:
+                    execution_direction_backward_converted += 1
+                elif '"direction": "FORWARD"' in converted_event:
+                    execution_direction_forward_converted += 1
+        self.assertEqual(4, item_execution_finish_states_converted)
+        self.assertEqual(4, execution_direction_backward_converted)
+        self.assertEqual(4, execution_direction_forward_converted)
 
     def test_convert_deconvert(self):
         """Converts events, then deconverts them back."""
         event_data = self.make_event_data()
         expected_data = deepcopy(event_data)
         converted_events = list()
         for event in event_data:
@@ -141,9 +154,9 @@
             event_tuple = EventDataConverter.deconvert(conv_event.encode("utf-8"))
             deconverted_events.append(event_tuple)
         self.assertEqual(16, len(deconverted_events))
         # The converted & deconverted list must be equal to the original
         self.assertEqual(expected_data, deconverted_events)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/server/util/test_ServerMessage.py` & `spine_engine-0.24.0/tests/server/util/test_ServerMessage.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -17,157 +18,157 @@
 import json
 from spine_engine.server.util.server_message import ServerMessage
 
 
 class TestServerMessage(unittest.TestCase):
     def make_engine_data1(self):
         engine_data = {
-            'items': {
-                'T1': {
-                    'type': 'Tool',
-                    'description': '',
-                    'x': -81.09856329675559,
-                    'y': -7.8289158512399695,
-                    'specification': 'a',
-                    'execute_in_work': True,
-                    'cmd_line_args': [],
-                },
-                'DC1': {
-                    'type': 'Data Connection',
-                    'description': '',
-                    'x': -249.4143275244174,
-                    'y': -122.2554094109619,
-                    'file_references': [],
-                    'db_references': [],
-                    'db_credentials': {},
+            "items": {
+                "T1": {
+                    "type": "Tool",
+                    "description": "",
+                    "x": -81.09856329675559,
+                    "y": -7.8289158512399695,
+                    "specification": "a",
+                    "execute_in_work": True,
+                    "cmd_line_args": [],
+                },
+                "DC1": {
+                    "type": "Data Connection",
+                    "description": "",
+                    "x": -249.4143275244174,
+                    "y": -122.2554094109619,
+                    "file_references": [],
+                    "db_references": [],
+                    "db_credentials": {},
                 },
             },
-            'specifications': {
-                'Tool': [
+            "specifications": {
+                "Tool": [
                     {
-                        'name': 'a',
-                        'tooltype': 'python',
-                        'includes': ['a.py'],
-                        'description': '',
-                        'inputfiles': ['a.txt'],
-                        'inputfiles_opt': [],
-                        'outputfiles': [],
-                        'cmdline_args': [],
-                        'includes_main_path': '.',
-                        'execution_settings': {
-                            'env': '',
-                            'kernel_spec_name': 'python38',
-                            'use_jupyter_console': False,
-                            'executable': '',
+                        "name": "a",
+                        "tooltype": "python",
+                        "includes": ["a.py"],
+                        "description": "",
+                        "inputfiles": ["a.txt"],
+                        "inputfiles_opt": [],
+                        "outputfiles": [],
+                        "cmdline_args": [],
+                        "includes_main_path": ".",
+                        "execution_settings": {
+                            "env": "",
+                            "kernel_spec_name": "python38",
+                            "use_jupyter_console": False,
+                            "executable": "",
                         },
-                        'definition_file_path': 'C:\\Users\\ttepsa\\OneDrive - Teknologian Tutkimuskeskus VTT\\Documents\\SpineToolboxProjects\\remote test 2 dags\\.spinetoolbox\\specifications\\Tool\\a.json',
+                        "definition_file_path": "C:\\Users\\ttepsa\\OneDrive - Teknologian Tutkimuskeskus VTT\\Documents\\SpineToolboxProjects\\remote test 2 dags\\.spinetoolbox\\specifications\\Tool\\a.json",
                     }
                 ]
             },
-            'connections': [{'name': 'from DC1 to T1', 'from': ['DC1', 'right'], 'to': ['T1', 'left']}],
-            'jumps': [],
-            'execution_permits': {'T1': True, 'DC1': True},
-            'items_module_name': 'spine_items',
-            'settings': {
-                'engineSettings/remoteExecutionEnabled': 'true',
-                'engineSettings/remoteHost': '192.168.56.69',
-                'engineSettings/remotePort': 50001,
-                'engineSettings/remoteSecurityFolder': '',
-                'engineSettings/remoteSecurityModel': '',
+            "connections": [{"name": "from DC1 to T1", "from": ["DC1", "right"], "to": ["T1", "left"]}],
+            "jumps": [],
+            "execution_permits": {"T1": True, "DC1": True},
+            "items_module_name": "spine_items",
+            "settings": {
+                "engineSettings/remoteExecutionEnabled": "true",
+                "engineSettings/remoteHost": "192.168.56.69",
+                "engineSettings/remotePort": 50001,
+                "engineSettings/remoteSecurityFolder": "",
+                "engineSettings/remoteSecurityModel": "",
             },
-            'project_dir': 'C:/Users/ttepsa/OneDrive - Teknologian Tutkimuskeskus VTT/Documents/SpineToolboxProjects/remote test 2 dags',
+            "project_dir": "C:/Users/ttepsa/OneDrive - Teknologian Tutkimuskeskus VTT/Documents/SpineToolboxProjects/remote test 2 dags",
         }
         return engine_data
 
     def make_engine_data2(self):
         engine_data = {
-            'items': {
-                'Importer 1': {
-                    'type': 'Importer',
-                    'description': '',
-                    'x': 72.45758726309028,
-                    'y': -80.20321040425301,
-                    'specification': 'Importer 1 - pekka_units.xlsx - 0',
-                    'cancel_on_error': True,
-                    'purge_before_writing': True,
-                    'on_conflict': 'replace',
-                    'file_selection': [['<pekka data>/pekka_units.xlsx', True]],
-                },
-                'DS1': {
-                    'type': 'Data Store',
-                    'description': '',
-                    'x': 211.34193262411353,
-                    'y': -152.99750295508272,
-                    'url': {
-                        'dialect': 'sqlite',
-                        'username': '',
-                        'password': '',
-                        'host': '',
-                        'port': '',
-                        'database': {'type': 'path', 'relative': True, 'path': '.spinetoolbox/items/ds1/DS1.sqlite'},
+            "items": {
+                "Importer 1": {
+                    "type": "Importer",
+                    "description": "",
+                    "x": 72.45758726309028,
+                    "y": -80.20321040425301,
+                    "specification": "Importer 1 - pekka_units.xlsx - 0",
+                    "cancel_on_error": True,
+                    "purge_before_writing": True,
+                    "on_conflict": "replace",
+                    "file_selection": [["<pekka data>/pekka_units.xlsx", True]],
+                },
+                "DS1": {
+                    "type": "Data Store",
+                    "description": "",
+                    "x": 211.34193262411353,
+                    "y": -152.99750295508272,
+                    "url": {
+                        "dialect": "sqlite",
+                        "username": "",
+                        "password": "",
+                        "host": "",
+                        "port": "",
+                        "database": {"type": "path", "relative": True, "path": ".spinetoolbox/items/ds1/DS1.sqlite"},
                     },
                 },
-                'pekka data': {
-                    'type': 'Data Connection',
-                    'description': '',
-                    'x': -78.23453014184398,
-                    'y': -145.98354018912534,
-                    'file_references': [],
-                    'db_references': [],
-                    'db_credentials': {},
+                "pekka data": {
+                    "type": "Data Connection",
+                    "description": "",
+                    "x": -78.23453014184398,
+                    "y": -145.98354018912534,
+                    "file_references": [],
+                    "db_references": [],
+                    "db_credentials": {},
                 },
             },
-            'specifications': {
-                'Importer': [
+            "specifications": {
+                "Importer": [
                     {
-                        'name': 'Importer 1 - pekka_units.xlsx - 0',
-                        'item_type': 'Importer',
-                        'mapping': {
-                            'table_mappings': {
-                                'Sheet1': [
+                        "name": "Importer 1 - pekka_units.xlsx - 0",
+                        "item_type": "Importer",
+                        "mapping": {
+                            "table_mappings": {
+                                "Sheet1": [
                                     {
-                                        'map_type': 'ObjectClass',
-                                        'name': {'map_type': 'column', 'reference': 0},
-                                        'parameters': {'map_type': 'None'},
-                                        'skip_columns': [],
-                                        'read_start_row': 0,
-                                        'objects': {'map_type': 'column', 'reference': 1},
+                                        "map_type": "ObjectClass",
+                                        "name": {"map_type": "column", "reference": 0},
+                                        "parameters": {"map_type": "None"},
+                                        "skip_columns": [],
+                                        "read_start_row": 0,
+                                        "objects": {"map_type": "column", "reference": 1},
                                     }
                                 ]
                             },
-                            'table_options': {},
-                            'table_types': {'Sheet1': {'0': 'string', '1': 'string'}},
-                            'table_row_types': {},
-                            'selected_tables': ['Sheet1'],
-                            'source_type': 'ExcelConnector',
+                            "table_options": {},
+                            "table_types": {"Sheet1": {"0": "string", "1": "string"}},
+                            "table_row_types": {},
+                            "selected_tables": ["Sheet1"],
+                            "source_type": "ExcelConnector",
                         },
-                        'description': None,
-                        'definition_file_path': 'C:\\Users\\ttepsa\\OneDrive - Teknologian Tutkimuskeskus VTT\\Documents\\SpineToolboxProjects\\Simple Importer\\Importer 1 - pekka_units.xlsx - 0.json',
+                        "description": None,
+                        "definition_file_path": "C:\\Users\\ttepsa\\OneDrive - Teknologian Tutkimuskeskus VTT\\Documents\\SpineToolboxProjects\\Simple Importer\\Importer 1 - pekka_units.xlsx - 0.json",
                     }
                 ]
             },
-            'connections': [
+            "connections": [
                 {
-                    'name': 'from pekka data to Importer 1',
-                    'from': ['pekka data', 'right'],
-                    'to': ['Importer 1', 'left'],
+                    "name": "from pekka data to Importer 1",
+                    "from": ["pekka data", "right"],
+                    "to": ["Importer 1", "left"],
                 },
-                {'name': 'from Importer 1 to DS1', 'from': ['Importer 1', 'right'], 'to': ['DS1', 'left']},
+                {"name": "from Importer 1 to DS1", "from": ["Importer 1", "right"], "to": ["DS1", "left"]},
             ],
-            'jumps': [],
-            'execution_permits': {'Importer 1': True, 'DS1': True, 'pekka data': True},
-            'items_module_name': 'spine_items',
-            'settings': {
-                'engineSettings/remoteExecutionEnabled': 'true',
-                'engineSettings/remoteHost': '192.168.56.69',
-                'engineSettings/remotePort': 50001,
-                'engineSettings/remoteSecurityFolder': '',
-                'engineSettings/remoteSecurityModel': '',
+            "jumps": [],
+            "execution_permits": {"Importer 1": True, "DS1": True, "pekka data": True},
+            "items_module_name": "spine_items",
+            "settings": {
+                "engineSettings/remoteExecutionEnabled": "true",
+                "engineSettings/remoteHost": "192.168.56.69",
+                "engineSettings/remotePort": 50001,
+                "engineSettings/remoteSecurityFolder": "",
+                "engineSettings/remoteSecurityModel": "",
             },
-            'project_dir': 'C:/Users/ttepsa/OneDrive - Teknologian Tutkimuskeskus VTT/Documents/SpineToolboxProjects/Simple Importer',
+            "project_dir": "C:/Users/ttepsa/OneDrive - Teknologian Tutkimuskeskus VTT/Documents/SpineToolboxProjects/Simple Importer",
         }
         return engine_data
 
     def test_make_server_msg_and_parse1(self):
         """Engine data of DC -> Tool DAG"""
         engine_data = self.make_engine_data1()
         msg_data_json = json.dumps(engine_data)
@@ -221,9 +222,9 @@
         msg = ServerMessage.parse(jsonStr)
         self.assertEqual(msg.getCommand(), "execute")
         self.assertEqual(msg.getId(), "4")
         self.assertEqual(msg.getData(), {})
         self.assertEqual(len(msg.getFileNames()), 0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/server/util/test_ZipHandler.py` & `spine_engine-0.24.0/tests/server/util/test_ZipHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -26,15 +27,15 @@
         ZipHandler.package(src, dst, "packager_test_zip")
         zip_file = os.path.join(dst, "packager_test_zip.zip")
         self.assertTrue(os.path.isfile(zip_file))
         os.remove(zip_file)
         self.assertFalse(os.path.isfile(zip_file))
 
     def test_extract_and_delete_folder(self):
-        zip_file_path = str(Path(__file__).parent.parent / "helloworld.zip")
+        zip_file_path = str(Path(__file__).parent.parent / "zippedproject.zip")
         output_dir_path = str(Path(__file__).parent / "output")
         ZipHandler.extract(zip_file_path, output_dir_path)
         self.assertEqual(os.path.isdir(output_dir_path), True)
         ZipHandler.delete_folder(output_dir_path)
         self.assertEqual(os.path.isdir(output_dir_path), False)
 
     def test_extract_invalid_input(self):
```

### Comparing `spine_engine-0.23.4/tests/test_load_project_items.py` & `spine_engine-0.24.0/tests/test_load_project_items.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Unit tests for `load_project_items` module.
-
-"""
+"""Unit tests for `load_project_items` module."""
 import os.path
 import unittest
 import sys
 from spine_engine.load_project_items import load_executable_item_classes, load_item_specification_factories
 from spine_engine.project_item.executable_item_base import ExecutableItemBase
 from spine_engine.project_item.project_item_specification_factory import ProjectItemSpecificationFactory
 
@@ -40,9 +38,9 @@
     def test_load_item_specification_factories(self):
         factories = load_item_specification_factories("items_module")
         self.assertEqual(len(factories), 1)
         self.assertIn("TestItem", factories)
         self.assertTrue(issubclass(factories["TestItem"], ProjectItemSpecificationFactory))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/test_spine_engine.py` & `spine_engine-0.24.0/tests/test_spine_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for `spine_engine` module.
 
 Inspired from tests for spinetoolbox.ExecutionInstance and spinetoolbox.ResourceMap,
 and intended to supersede them.
-
 """
 import os.path
 import sys
 from tempfile import TemporaryDirectory
 import unittest
 from unittest.mock import MagicMock, NonCallableMagicMock, call, patch
-
-from spinedb_api import DatabaseMapping, import_scenarios, import_tools
+from spinedb_api import DatabaseMapping, import_scenarios
 from spinedb_api.filters.scenario_filter import scenario_filter_config
-from spinedb_api.filters.tool_filter import tool_filter_config
 from spinedb_api.filters.execution_filter import execution_filter_config
 from spinedb_api.filters.tools import clear_filter_configs
 from spine_engine.exception import EngineInitFailed
 from spine_engine.spine_engine import validate_single_jump
 from spine_engine.utils.helpers import make_dag
 from spine_engine import ExecutionDirection, SpineEngine, SpineEngineState, ItemExecutionFinishState
 from spine_engine.project_item.connection import Jump, Connection
@@ -62,30 +60,30 @@
         """
         if resources_forward is None:
             resources_forward = []
         if resources_backward is None:
             resources_backward = []
         item = NonCallableMagicMock()
         item.name = name
-        item.short_name = name.lower().replace(' ', '_')
+        item.short_name = name.lower().replace(" ", "_")
         item.execute.return_value = execute_outcome
         item.exclude_execution = MagicMock()
         for r in resources_forward + resources_backward:
             r.provider_name = item.name
         item.output_resources.side_effect = lambda direction: {
             ExecutionDirection.FORWARD: resources_forward,
             ExecutionDirection.BACKWARD: resources_backward,
         }[direction]
         return item
 
     @staticmethod
     def _default_forward_url_resource(url, predecessor_name):
         resource = _make_url_resource(url)
         resource.provider_name = predecessor_name
-        resource.metadata = {'filter_id': '', 'filter_stack': ()}
+        resource.metadata = {"filter_id": "", "filter_stack": ()}
         return resource
 
     @staticmethod
     def _default_backward_url_resource(url, item_name, successor_name, scenarios=None):
         resource = _make_url_resource(url)
         resource.provider_name = successor_name
         if scenarios is None:
@@ -276,19 +274,17 @@
         self._assert_resource_args(mock_item_c.execute.call_args_list, item_c_execute_calls)
         mock_item_c.exclude_execution.assert_not_called()
 
     def test_filter_stacks(self):
         """Tests filter stacks are properly applied."""
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
-            db_map = DatabaseMapping(url, create=True)
-            import_scenarios(db_map, (("scen1", True), ("scen2", True)))
-            import_tools(db_map, ("toolA",))
-            db_map.commit_session("Add test data.")
-            db_map.connection.close()
+            with DatabaseMapping(url, create=True) as db_map:
+                import_scenarios(db_map, (("scen1", True), ("scen2", True)))
+                db_map.commit_session("Add test data.")
             url_a_fw = _make_url_resource(url)
             url_b_fw1 = _make_url_resource("db:///url_b_fw")
             url_b_fw2 = _make_url_resource("db:///url_b_fw")
             url_c_bw = _make_url_resource("db:///url_c_bw")
             mock_item_a = self._mock_item("item_a", resources_forward=[url_a_fw], resources_backward=[])
             mock_item_b1 = self._mock_item("item_b", resources_forward=[url_b_fw1], resources_backward=[])
             mock_item_b2 = self._mock_item("item_b", resources_forward=[url_b_fw2], resources_backward=[])
@@ -304,63 +300,61 @@
                 "item_b": {"type": "TestItem"},
                 "item_c": {"type": "TestItem"},
             }
             connections = [
                 {
                     "from": ("item_a", "right"),
                     "to": ("item_b", "left"),
-                    "disabled_filters": {url_a_fw.label: {"scenario_filter": [], "tool_filter": []}},
+                    "disabled_filters": {url_a_fw.label: {"scenario_filter": []}},
                 },
                 {"from": ("item_b", "bottom"), "to": ("item_c", "left")},
             ]
             self._run_engine(items, connections, item_instances)
             item_a_execution_args = [[[], []]]
             self._assert_resource_args(mock_item_a.execute.call_args_list, item_a_execution_args)
             self.assertEqual(mock_item_a.filter_id, "")
             # Check that item_b has been executed two times, with the right filters
             expected_fw_resource1 = ProjectItemResource("item_a", "database", "label", url)
-            expected_filter_stack1 = (scenario_filter_config("scen1"), tool_filter_config("toolA"))
+            expected_filter_stack1 = (scenario_filter_config("scen1"),)
             expected_fw_resource1.metadata = {"filter_stack": expected_filter_stack1, "filter_id": ""}
             expected_bw_resource1 = self._default_backward_url_resource("db:///url_c_bw", "item_b", "item_c", ["scen1"])
             item_b_execution_args = [[[expected_fw_resource1], [expected_bw_resource1]]]
             self._assert_resource_args(mock_item_b1.execute.call_args_list, item_b_execution_args)
-            self.assertEqual(mock_item_b1.filter_id, "scen1, toolA - item_a")
+            self.assertEqual(mock_item_b1.filter_id, "scen1 - item_a")
             expected_fw_resource2 = ProjectItemResource("item_a", "database", "label", url)
-            expected_filter_stack2 = (scenario_filter_config("scen2"), tool_filter_config("toolA"))
+            expected_filter_stack2 = (scenario_filter_config("scen2"),)
             expected_fw_resource2.metadata = {"filter_stack": expected_filter_stack2, "filter_id": ""}
             expected_bw_resource2 = self._default_backward_url_resource("db:///url_c_bw", "item_b", "item_c", ["scen2"])
             item_b_execution_args = [[[expected_fw_resource2], [expected_bw_resource2]]]
             self._assert_resource_args(mock_item_b2.execute.call_args_list, item_b_execution_args)
-            self.assertEqual(mock_item_b2.filter_id, "scen2, toolA - item_a")
+            self.assertEqual(mock_item_b2.filter_id, "scen2 - item_a")
             # Check that item_c has been executed twice, with the right filters
             expected_fw_resource1 = ProjectItemResource("item_b", "database", "label", "db:///url_b_fw")
             expected_fw_resource1.metadata = {
                 "filter_stack": expected_filter_stack1,
-                "filter_id": "scen1, toolA - item_a",
+                "filter_id": "scen1 - item_a",
             }
             item_c_execution_args = [[[expected_fw_resource1], []]]
             self._assert_resource_args(mock_item_c1.execute.call_args_list, item_c_execution_args)
-            self.assertEqual(mock_item_c1.filter_id, "scen1, toolA - item_b")
+            self.assertEqual(mock_item_c1.filter_id, "scen1 - item_b")
             expected_fw_resource2 = ProjectItemResource("item_b", "database", "label", "db:///url_b_fw")
             expected_fw_resource2.metadata = {
                 "filter_stack": expected_filter_stack2,
-                "filter_id": "scen2, toolA - item_a",
+                "filter_id": "scen2 - item_a",
             }
             item_c_execution_args = [[[expected_fw_resource2], []]]
             self._assert_resource_args(mock_item_c2.execute.call_args_list, item_c_execution_args)
-            self.assertEqual(mock_item_c2.filter_id, "scen2, toolA - item_b")
+            self.assertEqual(mock_item_c2.filter_id, "scen2 - item_b")
 
     def test_parallel_execution_ends_when_no_output_resources_are_generated(self):
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
-            db_map = DatabaseMapping(url, create=True)
-            import_scenarios(db_map, (("scen1", True), ("scen2", True)))
-            import_tools(db_map, ("toolA",))
-            db_map.commit_session("Add test data.")
-            db_map.connection.close()
+            with DatabaseMapping(url, create=True) as db_map:
+                import_scenarios(db_map, (("scen1", True), ("scen2", True)))
+                db_map.commit_session("Add test data.")
             url_a_fw = _make_url_resource(url)
             url_c_bw = _make_url_resource("db:///url_c_bw")
             mock_item_a = self._mock_item("item_a", resources_forward=[url_a_fw], resources_backward=[])
             mock_item_b1 = self._mock_item("item_b", resources_forward=[], resources_backward=[])
             mock_item_b2 = self._mock_item("item_b", resources_forward=[], resources_backward=[])
             mock_item_c = self._mock_item("item_c", resources_forward=[], resources_backward=[url_c_bw])
             item_instances = {"item_a": [mock_item_a], "item_b": [mock_item_b1, mock_item_b2], "item_c": [mock_item_c]}
@@ -369,50 +363,48 @@
                 "item_b": {"type": "TestItem"},
                 "item_c": {"type": "TestItem"},
             }
             connections = [
                 {
                     "from": ("item_a", "right"),
                     "to": ("item_b", "left"),
-                    "resource_filters": {url_a_fw.label: {"scenario_filter": [1, 2], "tool_filter": [1]}},
+                    "resource_filters": {url_a_fw.label: {"scenario_filter": [1, 2]}},
                 },
                 {"from": ("item_b", "bottom"), "to": ("item_c", "left")},
             ]
             self._run_engine(items, connections, item_instances)
             item_a_execution_args = [[[], []]]
             self._assert_resource_args(mock_item_a.execute.call_args_list, item_a_execution_args)
             self.assertEqual(mock_item_a.filter_id, "")
             # Check that item_b has been executed two times, with the right filters
             expected_fw_resource1 = ProjectItemResource("item_a", "database", "label", url)
-            expected_filter_stack1 = (scenario_filter_config("scen1"), tool_filter_config("toolA"))
+            expected_filter_stack1 = (scenario_filter_config("scen1"),)
             expected_fw_resource1.metadata = {"filter_stack": expected_filter_stack1, "filter_id": ""}
             expected_bw_resource1 = self._default_backward_url_resource("db:///url_c_bw", "item_b", "item_c", ["scen1"])
             item_b_execution_args = [[[expected_fw_resource1], [expected_bw_resource1]]]
             self._assert_resource_args(mock_item_b1.execute.call_args_list, item_b_execution_args)
-            self.assertEqual(mock_item_b1.filter_id, "scen1, toolA - item_a")
+            self.assertEqual(mock_item_b1.filter_id, "scen1 - item_a")
             expected_fw_resource2 = ProjectItemResource("item_a", "database", "label", url)
-            expected_filter_stack2 = (scenario_filter_config("scen2"), tool_filter_config("toolA"))
+            expected_filter_stack2 = (scenario_filter_config("scen2"),)
             expected_fw_resource2.metadata = {"filter_stack": expected_filter_stack2, "filter_id": ""}
             expected_bw_resource2 = self._default_backward_url_resource("db:///url_c_bw", "item_b", "item_c", ["scen2"])
             item_b_execution_args = [[[expected_fw_resource2], [expected_bw_resource2]]]
             self._assert_resource_args(mock_item_b2.execute.call_args_list, item_b_execution_args)
-            self.assertEqual(mock_item_b2.filter_id, "scen2, toolA - item_a")
+            self.assertEqual(mock_item_b2.filter_id, "scen2 - item_a")
             # Check that item_c has been executed only once
             self._assert_resource_args(mock_item_c.execute.call_args_list, [[[], []]])
             self.assertEqual(mock_item_c.filter_id, "")
 
     def test_filter_stacks_and_multiple_file_output_resources(self):
         """Multiple file output resources should be combined correctly for a successor"""
         with TemporaryDirectory() as temp_dir:
             url = "sqlite:///" + os.path.join(temp_dir, "db.sqlite")
-            db_map = DatabaseMapping(url, create=True)
-            import_scenarios(db_map, (("scen1", True), ("scen2", True)))
-            import_tools(db_map, ("toolA",))
-            db_map.commit_session("Add test data.")
-            db_map.connection.close()
+            with DatabaseMapping(url, create=True) as db_map:
+                import_scenarios(db_map, (("scen1", True), ("scen2", True)))
+                db_map.commit_session("Add test data.")
             url_a_fw = _make_url_resource(url)
             file_b_fw_11 = ProjectItemResource("item_b", "file", "label_1")
             file_b_fw_12 = ProjectItemResource("item_b", "file", "label_1")
             file_b_fw_21 = ProjectItemResource("item_b", "file", "label_2")
             file_b_fw_22 = ProjectItemResource("item_b", "file", "label_2")
             url_c_bw = _make_url_resource("db:///url_c_bw")
             mock_item_a = self._mock_item("item_a", resources_forward=[url_a_fw], resources_backward=[])
@@ -434,79 +426,75 @@
                 "item_b": {"type": "TestItem"},
                 "item_c": {"type": "TestItem"},
             }
             connections = [
                 {
                     "from": ("item_a", "right"),
                     "to": ("item_b", "left"),
-                    "disabled_filters": {url_a_fw.label: {"scenario_filter": [], "tool_filter": []}},
+                    "disabled_filters": {url_a_fw.label: {"scenario_filter": []}},
                 },
                 {"from": ("item_b", "bottom"), "to": ("item_c", "left")},
             ]
             self._run_engine(items, connections, item_instances)
             item_a_execution_args = [[[], []]]
             self._assert_resource_args(mock_item_a.execute.call_args_list, item_a_execution_args)
             self.assertEqual(mock_item_a.filter_id, "")
             # Check that item_b has been executed two times, with the right filters
             expected_fw_resource1 = ProjectItemResource("item_a", "database", "label", url)
-            expected_filter_stack1 = (scenario_filter_config("scen1"), tool_filter_config("toolA"))
+            expected_filter_stack1 = (scenario_filter_config("scen1"),)
             expected_fw_resource1.metadata = {"filter_stack": expected_filter_stack1, "filter_id": ""}
             expected_bw_resource1 = self._default_backward_url_resource("db:///url_c_bw", "item_b", "item_c", ["scen1"])
             item_b_execution_args = [[[expected_fw_resource1], [expected_bw_resource1]]]
             self._assert_resource_args(mock_item_b1.execute.call_args_list, item_b_execution_args)
-            self.assertEqual(mock_item_b1.filter_id, "scen1, toolA - item_a")
+            self.assertEqual(mock_item_b1.filter_id, "scen1 - item_a")
             expected_fw_resource2 = ProjectItemResource("item_a", "database", "label", url)
-            expected_filter_stack2 = (scenario_filter_config("scen2"), tool_filter_config("toolA"))
+            expected_filter_stack2 = (scenario_filter_config("scen2"),)
             expected_fw_resource2.metadata = {"filter_stack": expected_filter_stack2, "filter_id": ""}
             expected_bw_resource2 = self._default_backward_url_resource("db:///url_c_bw", "item_b", "item_c", ["scen2"])
             item_b_execution_args = [[[expected_fw_resource2], [expected_bw_resource2]]]
             self._assert_resource_args(mock_item_b2.execute.call_args_list, item_b_execution_args)
-            self.assertEqual(mock_item_b2.filter_id, "scen2, toolA - item_a")
+            self.assertEqual(mock_item_b2.filter_id, "scen2 - item_a")
             # Check that item_c has been executed twice, with the right filters
             expected_fw_resource1 = ProjectItemResource("item_b", "file", "label_1")
             expected_fw_resource1.metadata = {
                 "filter_stack": expected_filter_stack1,
-                "filter_id": "scen1, toolA - item_a",
+                "filter_id": "scen1 - item_a",
             }
             expected_fw_resource2 = ProjectItemResource("item_b", "file", "label_2")
             expected_fw_resource2.metadata = {
                 "filter_stack": expected_filter_stack1,
-                "filter_id": "scen1, toolA - item_a",
+                "filter_id": "scen1 - item_a",
             }
             item_c_execution_args = [[[expected_fw_resource1, expected_fw_resource2], []]]
             self._assert_resource_args(mock_item_c1.execute.call_args_list, item_c_execution_args)
-            self.assertEqual(mock_item_c1.filter_id, "scen1, toolA - item_a")
+            self.assertEqual(mock_item_c1.filter_id, "scen1 - item_a")
             expected_fw_resource3 = ProjectItemResource("item_b", "file", "label_1")
             expected_fw_resource3.metadata = {
                 "filter_stack": expected_filter_stack2,
-                "filter_id": "scen2, toolA - item_a",
+                "filter_id": "scen2 - item_a",
             }
             expected_fw_resource4 = ProjectItemResource("item_b", "file", "label_2")
             expected_fw_resource4.metadata = {
                 "filter_stack": expected_filter_stack2,
-                "filter_id": "scen2, toolA - item_a",
+                "filter_id": "scen2 - item_a",
             }
             item_c_execution_args = [[[expected_fw_resource3, expected_fw_resource4], []]]
             self._assert_resource_args(mock_item_c2.execute.call_args_list, item_c_execution_args)
-            self.assertEqual(mock_item_c2.filter_id, "scen2, toolA - item_a")
+            self.assertEqual(mock_item_c2.filter_id, "scen2 - item_a")
 
     def test_merge_two_filtered_database_branches(self):
         with TemporaryDirectory() as temp_dir:
             urlA = "sqlite:///" + os.path.join(temp_dir, "dbA.sqlite")
-            db_map = DatabaseMapping(urlA, create=True)
-            import_scenarios(db_map, (("scenA1", True), ("scenA2", True)))
-            import_tools(db_map, ("toolA",))
-            db_map.commit_session("Add test data.")
-            db_map.connection.close()
+            with DatabaseMapping(urlA, create=True) as db_map:
+                import_scenarios(db_map, (("scenA1", True), ("scenA2", True)))
+                db_map.commit_session("Add test data.")
             urlB = "sqlite:///" + os.path.join(temp_dir, "dbB.sqlite")
-            db_map = DatabaseMapping(urlB, create=True)
-            import_scenarios(db_map, (("scenB1", True), ("scenB2", True)))
-            import_tools(db_map, ("toolB",))
-            db_map.commit_session("Add test data.")
-            db_map.connection.close()
+            with DatabaseMapping(urlB, create=True) as db_map:
+                import_scenarios(db_map, (("scenB1", True), ("scenB2", True)))
+                db_map.commit_session("Add test data.")
             url_a_fw = _make_url_resource(urlA)
             url_b_fw = _make_url_resource(urlB)
             mock_item_a = self._mock_item("item_a", resources_forward=[url_a_fw], resources_backward=[])
             mock_item_b = self._mock_item("item_b", resources_forward=[url_b_fw], resources_backward=[])
             mock_item_c1 = self._mock_item("item_c", resources_forward=[], resources_backward=[])
             mock_item_c2 = self._mock_item("item_c", resources_forward=[], resources_backward=[])
             mock_item_c3 = self._mock_item("item_c", resources_forward=[], resources_backward=[])
@@ -521,63 +509,59 @@
                 "item_b": {"type": "TestItem"},
                 "item_c": {"type": "TestItem"},
             }
             connections = [
                 {
                     "from": ("item_a", "right"),
                     "to": ("item_c", "left"),
-                    "disabled_filters": {url_a_fw.label: {"scenario_filter": [], "tool_filter": []}},
+                    "disabled_filters": {url_a_fw.label: {"scenario_filter": []}},
                 },
                 {
                     "from": ("item_b", "right"),
                     "to": ("item_c", "left"),
-                    "disabled_filters": {url_b_fw.label: {"scenario_filter": [], "tool_filter": []}},
+                    "disabled_filters": {url_b_fw.label: {"scenario_filter": []}},
                 },
             ]
             self._run_engine(items, connections, item_instances)
             item_a_execution_args = [[[], []]]
             self._assert_resource_args(mock_item_a.execute.call_args_list, item_a_execution_args)
             item_b_execution_args = [[[], []]]
             self._assert_resource_args(mock_item_b.execute.call_args_list, item_b_execution_args)
             # Check that item_c has been executed four times, with all combinations of item_a and item_b filters
             expected_fw_resource1 = ProjectItemResource("item_a", "database", "label", urlA)
-            expected_filter_stack1 = (scenario_filter_config("scenA1"), tool_filter_config("toolA"))
+            expected_filter_stack1 = (scenario_filter_config("scenA1"),)
             expected_fw_resource1.metadata = {"filter_stack": expected_filter_stack1, "filter_id": ""}
             expected_fw_resource2 = ProjectItemResource("item_b", "database", "label", urlB)
-            expected_filter_stack2 = (scenario_filter_config("scenB1"), tool_filter_config("toolB"))
+            expected_filter_stack2 = (scenario_filter_config("scenB1"),)
             expected_fw_resource2.metadata = {"filter_stack": expected_filter_stack2, "filter_id": ""}
             item_c_execution_args = [[[expected_fw_resource1, expected_fw_resource2], []]]
             self._assert_resource_args(mock_item_c1.execute.call_args_list, item_c_execution_args)
             expected_fw_resource3 = ProjectItemResource("item_b", "database", "label", urlB)
-            expected_filter_stack3 = (scenario_filter_config("scenB2"), tool_filter_config("toolB"))
+            expected_filter_stack3 = (scenario_filter_config("scenB2"),)
             expected_fw_resource3.metadata = {"filter_stack": expected_filter_stack3, "filter_id": ""}
             item_c_execution_args = [[[expected_fw_resource1, expected_fw_resource3], []]]
             self._assert_resource_args(mock_item_c2.execute.call_args_list, item_c_execution_args)
             expected_fw_resource4 = ProjectItemResource("item_a", "database", "label", urlA)
-            expected_filter_stack4 = (scenario_filter_config("scenA2"), tool_filter_config("toolA"))
+            expected_filter_stack4 = (scenario_filter_config("scenA2"),)
             expected_fw_resource4.metadata = {"filter_stack": expected_filter_stack4, "filter_id": ""}
             item_c_execution_args = [[[expected_fw_resource4, expected_fw_resource2], []]]
             self._assert_resource_args(mock_item_c3.execute.call_args_list, item_c_execution_args)
             item_c_execution_args = [[[expected_fw_resource4, expected_fw_resource3], []]]
             self._assert_resource_args(mock_item_c4.execute.call_args_list, item_c_execution_args)
 
     def test_merge_two_filtered_file_resource_branches(self):
         with TemporaryDirectory() as temp_dir:
             urlA = "sqlite:///" + os.path.join(temp_dir, "dbA.sqlite")
-            db_map = DatabaseMapping(urlA, create=True)
-            import_scenarios(db_map, (("scenA1", True), ("scenA2", True)))
-            import_tools(db_map, ("toolA",))
-            db_map.commit_session("Add test data.")
-            db_map.connection.close()
+            with DatabaseMapping(urlA, create=True) as db_map:
+                import_scenarios(db_map, (("scenA1", True), ("scenA2", True)))
+                db_map.commit_session("Add test data.")
             urlB = "sqlite:///" + os.path.join(temp_dir, "dbB.sqlite")
-            db_map = DatabaseMapping(urlB, create=True)
-            import_scenarios(db_map, (("scenB1", True), ("scenB2", True)))
-            import_tools(db_map, ("toolB",))
-            db_map.commit_session("Add test data.")
-            db_map.connection.close()
+            with DatabaseMapping(urlB, create=True) as db_map:
+                import_scenarios(db_map, (("scenB1", True), ("scenB2", True)))
+                db_map.commit_session("Add test data.")
             url_a_fw = _make_url_resource(urlA)
             url_b_fw = _make_url_resource(urlB)
             file_c_fw_11 = ProjectItemResource("item_c", "file", "label_1")
             file_c_fw_12 = ProjectItemResource("item_c", "file", "label_1")
             file_c_fw_21 = ProjectItemResource("item_c", "file", "label_2")
             file_c_fw_22 = ProjectItemResource("item_c", "file", "label_2")
             file_d_fw_11 = ProjectItemResource("item_d", "file", "label_3")
@@ -616,122 +600,122 @@
                 "item_d": {"type": "TestItem"},
                 "item_e": {"type": "TestItem"},
             }
             connections = [
                 {
                     "from": ("item_a", "right"),
                     "to": ("item_c", "left"),
-                    "resource_filters": {url_a_fw.label: {"scenario_filter": [1, 2], "tool_filter": [1]}},
+                    "resource_filters": {url_a_fw.label: {"scenario_filter": [1, 2]}},
                 },
                 {
                     "from": ("item_b", "right"),
                     "to": ("item_d", "left"),
-                    "resource_filters": {url_b_fw.label: {"scenario_filter": [1, 2], "tool_filter": [1]}},
+                    "resource_filters": {url_b_fw.label: {"scenario_filter": [1, 2]}},
                 },
                 {"from": ("item_c", "right"), "to": ("item_e", "left")},
                 {"from": ("item_d", "bottom"), "to": ("item_e", "top")},
             ]
             self._run_engine(items, connections, item_instances)
             item_a_execution_args = [[[], []]]
             self._assert_resource_args(mock_item_a.execute.call_args_list, item_a_execution_args)
             self.assertEqual(mock_item_a.filter_id, "")
             item_b_execution_args = [[[], []]]
             self._assert_resource_args(mock_item_b.execute.call_args_list, item_b_execution_args)
             self.assertEqual(mock_item_b.filter_id, "")
             # Check that item_c has been executed twice, with all combinations of item_a's filters
             expected_fw_resource1 = ProjectItemResource("item_a", "database", "label", urlA)
-            expected_filter_stack1 = (scenario_filter_config("scenA1"), tool_filter_config("toolA"))
+            expected_filter_stack1 = (scenario_filter_config("scenA1"),)
             expected_fw_resource1.metadata = {"filter_stack": expected_filter_stack1, "filter_id": ""}
             item_c_execution_args = [[[expected_fw_resource1], []]]
             self._assert_resource_args(mock_item_c1.execute.call_args_list, item_c_execution_args)
-            self.assertEqual(mock_item_c1.filter_id, "scenA1, toolA - item_a")
+            self.assertEqual(mock_item_c1.filter_id, "scenA1 - item_a")
             expected_fw_resource2 = ProjectItemResource("item_a", "database", "label", urlA)
-            expected_filter_stack2 = (scenario_filter_config("scenA2"), tool_filter_config("toolA"))
+            expected_filter_stack2 = (scenario_filter_config("scenA2"),)
             expected_fw_resource2.metadata = {"filter_stack": expected_filter_stack2, "filter_id": ""}
             item_c_execution_args = [[[expected_fw_resource2], []]]
             self._assert_resource_args(mock_item_c2.execute.call_args_list, item_c_execution_args)
-            self.assertEqual(mock_item_c2.filter_id, "scenA2, toolA - item_a")
+            self.assertEqual(mock_item_c2.filter_id, "scenA2 - item_a")
             # Check that item_d has been executed twice, with all combinations of item_b's filters
             expected_fw_resource3 = ProjectItemResource("item_b", "database", "label", urlB)
-            expected_filter_stack3 = (scenario_filter_config("scenB1"), tool_filter_config("toolB"))
+            expected_filter_stack3 = (scenario_filter_config("scenB1"),)
             expected_fw_resource3.metadata = {"filter_stack": expected_filter_stack3, "filter_id": ""}
             item_d_execution_args = [[[expected_fw_resource3], []]]
             self._assert_resource_args(mock_item_d1.execute.call_args_list, item_d_execution_args)
-            self.assertEqual(mock_item_d1.filter_id, "scenB1, toolB - item_b")
+            self.assertEqual(mock_item_d1.filter_id, "scenB1 - item_b")
             expected_fw_resource4 = ProjectItemResource("item_b", "database", "label", urlB)
-            expected_filter_stack4 = (scenario_filter_config("scenB2"), tool_filter_config("toolB"))
+            expected_filter_stack4 = (scenario_filter_config("scenB2"),)
             expected_fw_resource4.metadata = {"filter_stack": expected_filter_stack4, "filter_id": ""}
             item_d_execution_args = [[[expected_fw_resource4], []]]
             self._assert_resource_args(mock_item_d2.execute.call_args_list, item_d_execution_args)
-            self.assertEqual(mock_item_d2.filter_id, "scenB2, toolB - item_b")
+            self.assertEqual(mock_item_d2.filter_id, "scenB2 - item_b")
             # Check that item_e has been executed four times, with all combinations of item_c's and item_d's resources.
             expected_fw_resource5 = ProjectItemResource("item_c", "file", "label_1")
-            expected_filter_stack5 = (scenario_filter_config("scenA1"), tool_filter_config("toolA"))
+            expected_filter_stack5 = (scenario_filter_config("scenA1"),)
             expected_fw_resource5.metadata = {
                 "filter_stack": expected_filter_stack5,
-                "filter_id": "scenA1, toolA - item_a",
+                "filter_id": "scenA1 - item_a",
             }
             expected_fw_resource6 = ProjectItemResource("item_c", "file", "label_2")
             expected_fw_resource6.metadata = {
                 "filter_stack": expected_filter_stack5,
-                "filter_id": "scenA1, toolA - item_a",
+                "filter_id": "scenA1 - item_a",
             }
             expected_fw_resource7 = ProjectItemResource("item_d", "file", "label_3")
-            expected_filter_stack7 = (scenario_filter_config("scenB1"), tool_filter_config("toolB"))
+            expected_filter_stack7 = (scenario_filter_config("scenB1"),)
             expected_fw_resource7.metadata = {
                 "filter_stack": expected_filter_stack7,
-                "filter_id": "scenB1, toolB - item_b",
+                "filter_id": "scenB1 - item_b",
             }
             expected_fw_resource8 = ProjectItemResource("item_d", "file", "label_4")
             expected_fw_resource8.metadata = {
                 "filter_stack": expected_filter_stack7,
-                "filter_id": "scenB1, toolB - item_b",
+                "filter_id": "scenB1 - item_b",
             }
             item_e_execution_args = [
                 [[expected_fw_resource5, expected_fw_resource6, expected_fw_resource7, expected_fw_resource8], []]
             ]
             self._assert_resource_args(mock_item_e1.execute.call_args_list, item_e_execution_args)
-            self.assertEqual(mock_item_e1.filter_id, "scenA1, toolA - item_a & scenB1, toolB - item_b")
+            self.assertEqual(mock_item_e1.filter_id, "scenA1 - item_a & scenB1 - item_b")
             expected_fw_resource9 = ProjectItemResource("item_d", "file", "label_3")
-            expected_filter_stack9 = (scenario_filter_config("scenB2"), tool_filter_config("toolB"))
+            expected_filter_stack9 = (scenario_filter_config("scenB2"),)
             expected_fw_resource9.metadata = {
                 "filter_stack": expected_filter_stack9,
-                "filter_id": "scenB2, toolB - item_b",
+                "filter_id": "scenB2 - item_b",
             }
             expected_fw_resource10 = ProjectItemResource("item_d", "file", "label_4")
             expected_fw_resource10.metadata = {
                 "filter_stack": expected_filter_stack9,
-                "filter_id": "scenB2, toolB - item_b",
+                "filter_id": "scenB2 - item_b",
             }
             item_e_execution_args = [
                 [[expected_fw_resource5, expected_fw_resource6, expected_fw_resource9, expected_fw_resource10], []]
             ]
             self._assert_resource_args(mock_item_e2.execute.call_args_list, item_e_execution_args)
-            self.assertEqual(mock_item_e2.filter_id, "scenA1, toolA - item_a & scenB2, toolB - item_b")
+            self.assertEqual(mock_item_e2.filter_id, "scenA1 - item_a & scenB2 - item_b")
             expected_fw_resource11 = ProjectItemResource("item_c", "file", "label_1")
-            expected_filter_stack11 = (scenario_filter_config("scenA2"), tool_filter_config("toolA"))
+            expected_filter_stack11 = (scenario_filter_config("scenA2"),)
             expected_fw_resource11.metadata = {
                 "filter_stack": expected_filter_stack11,
-                "filter_id": "scenA2, toolA - item_a",
+                "filter_id": "scenA2 - item_a",
             }
             expected_fw_resource12 = ProjectItemResource("item_c", "file", "label_2")
             expected_fw_resource12.metadata = {
                 "filter_stack": expected_filter_stack11,
-                "filter_id": "scenA2, toolA - item_a",
+                "filter_id": "scenA2 - item_a",
             }
             item_e_execution_args = [
                 [[expected_fw_resource11, expected_fw_resource12, expected_fw_resource7, expected_fw_resource8], []]
             ]
             self._assert_resource_args(mock_item_e3.execute.call_args_list, item_e_execution_args)
-            self.assertEqual(mock_item_e3.filter_id, "scenA2, toolA - item_a & scenB1, toolB - item_b")
+            self.assertEqual(mock_item_e3.filter_id, "scenA2 - item_a & scenB1 - item_b")
             item_e_execution_args = [
                 [[expected_fw_resource11, expected_fw_resource12, expected_fw_resource9, expected_fw_resource10], []]
             ]
             self._assert_resource_args(mock_item_e4.execute.call_args_list, item_e_execution_args)
-            self.assertEqual(mock_item_e4.filter_id, "scenA2, toolA - item_a & scenB2, toolB - item_b")
+            self.assertEqual(mock_item_e4.filter_id, "scenA2 - item_a & scenB2 - item_b")
 
     def test_self_jump_succeeds(self):
         mock_item = self._mock_item("item", resources_forward=[], resources_backward=[])
         items = {"item": {"type": "TestItem"}}
         connections = []
         jumps = [Jump("item", "bottom", "item", "top", self._LOOP_TWICE).to_dict()]
         execution_permits = {"item": True}
@@ -746,104 +730,118 @@
         engine.make_item = lambda name, direction: mock_item
         engine.run()
         lock_1 = mock_item.execute.call_args_list[0].args[-1]
         lock_2 = mock_item.execute.call_args_list[1].args[-1]
         self.assertEqual(mock_item.execute.call_args_list, [call([], [], lock_1), call([], [], lock_2)])
         self.assertEqual(engine.state(), SpineEngineState.COMPLETED)
 
-    @unittest.skip("Hangs because something's not right in SpineDBServer")
     def test_jump_resources_get_passed_correctly(self):
-        resource_fw_a = _make_url_resource("db:///fw_a")
-        resource_bw_a = _make_url_resource("db:///bw_a")
-        item_a = self._mock_item("a", resources_forward=[resource_fw_a], resources_backward=[resource_bw_a])
-        resource_fw_b = _make_url_resource("db:///fw_b")
-        resource_bw_b = _make_url_resource("db:///bw_b")
-        item_b = self._mock_item("b", resources_forward=[resource_fw_b], resources_backward=[resource_bw_b])
-        resource_fw_c = _make_url_resource("db:///fw_c")
-        resource_bw_c = _make_url_resource("db:///bw_c")
-        item_c = self._mock_item("c", resources_forward=[resource_fw_c], resources_backward=[resource_bw_c])
-        resource_fw_d = _make_url_resource("db:///fw_d")
-        resource_bw_d = _make_url_resource("db:///bw_d")
-        item_d = self._mock_item("d", resources_forward=[resource_fw_d], resources_backward=[resource_bw_d])
-        item_instances = {"a": [item_a], "b": [item_b, item_b], "c": [item_c, item_c], "d": [item_d]}
-        items = {
-            "a": {"type": "TestItem"},
-            "b": {"type": "TestItem"},
-            "c": {"type": "TestItem"},
-            "d": {"type": "TestItem"},
-        }
-        connections = [
-            c.to_dict()
-            for c in (
-                Connection("a", "right", "b", "left"),
-                Connection("b", "bottom", "c", "top"),
-                Connection("c", "left", "d", "right"),
+        with TemporaryDirectory() as temp_dir:
+            url_fw_a = "sqlite:///" + os.path.join(temp_dir, "fw_a")
+            url_bw_a = "sqlite:///" + os.path.join(temp_dir, "bw_a")
+            url_fw_b = "sqlite:///" + os.path.join(temp_dir, "fw_b")
+            url_bw_b = "sqlite:///" + os.path.join(temp_dir, "bw_b")
+            url_fw_c = "sqlite:///" + os.path.join(temp_dir, "fw_c")
+            url_bw_c = "sqlite:///" + os.path.join(temp_dir, "bw_c")
+            url_fw_d = "sqlite:///" + os.path.join(temp_dir, "fw_d")
+            url_bw_d = "sqlite:///" + os.path.join(temp_dir, "bw_d")
+            resource_fw_a = _make_url_resource(url_fw_a)
+            resource_bw_a = _make_url_resource(url_bw_a)
+            item_a = self._mock_item("a", resources_forward=[resource_fw_a], resources_backward=[resource_bw_a])
+            resource_fw_b = _make_url_resource(url_fw_b)
+            resource_bw_b = _make_url_resource(url_bw_b)
+            item_b = self._mock_item("b", resources_forward=[resource_fw_b], resources_backward=[resource_bw_b])
+            resource_fw_c = _make_url_resource(url_fw_c)
+            resource_bw_c = _make_url_resource(url_bw_c)
+            item_c = self._mock_item("c", resources_forward=[resource_fw_c], resources_backward=[resource_bw_c])
+            resource_fw_d = _make_url_resource(url_fw_d)
+            resource_bw_d = _make_url_resource(url_bw_d)
+            item_d = self._mock_item("d", resources_forward=[resource_fw_d], resources_backward=[resource_bw_d])
+            item_instances = {"a": [item_a], "b": [item_b, item_b], "c": [item_c, item_c], "d": [item_d]}
+            items = {
+                "a": {"type": "TestItem"},
+                "b": {"type": "TestItem"},
+                "c": {"type": "TestItem"},
+                "d": {"type": "TestItem"},
+            }
+            connections = [
+                c.to_dict()
+                for c in (
+                    Connection("a", "right", "b", "left"),
+                    Connection("b", "bottom", "c", "top"),
+                    Connection("c", "left", "d", "right"),
+                )
+            ]
+            jumps = [Jump("c", "right", "b", "right", self._LOOP_TWICE).to_dict()]
+            self._run_engine(items, connections, item_instances, jumps=jumps)
+            self._assert_resource_args(
+                item_a.execute.call_args_list, [[[], [self._default_backward_url_resource(url_bw_b, "a", "b")]]]
+            )
+            self._assert_resource_args(
+                item_b.execute.call_args_list,
+                2
+                * [
+                    [
+                        [self._default_forward_url_resource(url_fw_a, "a")],
+                        [self._default_backward_url_resource(url_bw_c, "b", "c")],
+                    ]
+                ],
+            )
+            self._assert_resource_args(
+                item_c.execute.call_args_list,
+                2
+                * [
+                    [
+                        [self._default_forward_url_resource(url_fw_b, "b")],
+                        [self._default_backward_url_resource(url_bw_d, "c", "d")],
+                    ]
+                ],
+            )
+            self._assert_resource_args(
+                item_d.execute.call_args_list, [[[self._default_forward_url_resource(url_fw_c, "c")], []]]
             )
-        ]
-        jumps = [Jump("c", "right", "b", "right", self._LOOP_TWICE).to_dict()]
-        self._run_engine(items, connections, item_instances, jumps=jumps)
-        self._assert_resource_args(
-            item_a.execute.call_args_list, [[[], [self._default_backward_url_resource("db:///bw_b", "a", "b")]]]
-        )
-        self._assert_resource_args(
-            item_b.execute.call_args_list,
-            2
-            * [
-                [
-                    [self._default_forward_url_resource("db:///fw_a", "a")],
-                    [self._default_backward_url_resource("db:///bw_c", "b", "c")],
-                ]
-            ],
-        )
-        self._assert_resource_args(
-            item_c.execute.call_args_list,
-            2
-            * [
-                [
-                    [self._default_forward_url_resource("db:///fw_b", "b")],
-                    [self._default_backward_url_resource("db:///bw_d", "c", "d")],
-                ]
-            ],
-        )
-        self._assert_resource_args(
-            item_d.execute.call_args_list, [[[self._default_forward_url_resource("db:///fw_c", "c")], []]]
-        )
 
-    @unittest.skip("Hangs because something's not right in SpineDBServer")
     def test_nested_jump_with_inner_self_jump(self):
-        resource_fw_a = _make_url_resource("db:///fw_a")
-        resource_bw_a = _make_url_resource("db:///bw_a")
-        item_a = self._mock_item("a", resources_forward=[resource_fw_a], resources_backward=[resource_bw_a])
-        resource_fw_b = _make_url_resource("db:///fw_b")
-        resource_bw_b = _make_url_resource("db:///bw_b")
-        item_b = self._mock_item("b", resources_forward=[resource_fw_b], resources_backward=[resource_bw_b])
-        resource_fw_c = _make_url_resource("db:///fw_c")
-        resource_bw_c = _make_url_resource("db:///bw_c")
-        item_c = self._mock_item("c", resources_forward=[resource_fw_c], resources_backward=[resource_bw_c])
-        item_instances = {"a": 2 * [item_a], "b": 4 * [item_b], "c": 2 * [item_c]}
-        items = {"a": {"type": "TestItem"}, "b": {"type": "TestItem"}, "c": {"type": "TestItem"}}
-        connections = [
-            c.to_dict() for c in (Connection("a", "right", "b", "left"), Connection("b", "bottom", "c", "top"))
-        ]
-        jumps = [
-            Jump("c", "right", "a", "right", self._LOOP_TWICE).to_dict(),
-            Jump("b", "top", "b", "top", self._LOOP_TWICE).to_dict(),
-        ]
-        self._run_engine(items, connections, item_instances, jumps=jumps)
-        expected = 2 * [[[], [self._default_backward_url_resource("db:///bw_b", "a", "b")]]]
-        self._assert_resource_args(item_a.execute.call_args_list, expected)
-        expected = 4 * [
-            [
-                [self._default_forward_url_resource("db:///fw_a", "a")],
-                [self._default_backward_url_resource("db:///bw_c", "b", "c")],
+        with TemporaryDirectory() as temp_dir:
+            url_fw_a = "sqlite:///" + os.path.join(temp_dir, "fw_a")
+            url_bw_a = "sqlite:///" + os.path.join(temp_dir, "bw_a")
+            url_fw_b = "sqlite:///" + os.path.join(temp_dir, "fw_b")
+            url_bw_b = "sqlite:///" + os.path.join(temp_dir, "bw_b")
+            url_fw_c = "sqlite:///" + os.path.join(temp_dir, "fw_c")
+            url_bw_c = "sqlite:///" + os.path.join(temp_dir, "bw_c")
+            resource_fw_a = _make_url_resource(url_fw_a)
+            resource_bw_a = _make_url_resource(url_bw_a)
+            item_a = self._mock_item("a", resources_forward=[resource_fw_a], resources_backward=[resource_bw_a])
+            resource_fw_b = _make_url_resource(url_fw_b)
+            resource_bw_b = _make_url_resource(url_bw_b)
+            item_b = self._mock_item("b", resources_forward=[resource_fw_b], resources_backward=[resource_bw_b])
+            resource_fw_c = _make_url_resource(url_fw_c)
+            resource_bw_c = _make_url_resource(url_bw_c)
+            item_c = self._mock_item("c", resources_forward=[resource_fw_c], resources_backward=[resource_bw_c])
+            item_instances = {"a": 2 * [item_a], "b": 4 * [item_b], "c": 2 * [item_c]}
+            items = {"a": {"type": "TestItem"}, "b": {"type": "TestItem"}, "c": {"type": "TestItem"}}
+            connections = [
+                c.to_dict() for c in (Connection("a", "right", "b", "left"), Connection("b", "bottom", "c", "top"))
             ]
-        ]
-        self._assert_resource_args(item_b.execute.call_args_list, expected)
-        expected = 2 * [[[self._default_forward_url_resource("db:///fw_b", "b")], []]]
-        self._assert_resource_args(item_c.execute.call_args_list, expected)
+            jumps = [
+                Jump("c", "right", "a", "right", self._LOOP_TWICE).to_dict(),
+                Jump("b", "top", "b", "top", self._LOOP_TWICE).to_dict(),
+            ]
+            self._run_engine(items, connections, item_instances, jumps=jumps)
+            expected = 2 * [[[], [self._default_backward_url_resource(url_bw_b, "a", "b")]]]
+            self._assert_resource_args(item_a.execute.call_args_list, expected)
+            expected = 4 * [
+                [
+                    [self._default_forward_url_resource(url_fw_a, "a")],
+                    [self._default_backward_url_resource(url_bw_c, "b", "c")],
+                ]
+            ]
+            self._assert_resource_args(item_b.execute.call_args_list, expected)
+            expected = 2 * [[[self._default_forward_url_resource(url_fw_b, "b")], []]]
+            self._assert_resource_args(item_c.execute.call_args_list, expected)
 
     def _assert_resource_args(self, arg_packs, expected_packs):
         self.assertEqual(len(arg_packs), len(expected_packs))
         for pack, expected_pack in zip(arg_packs, expected_packs):
             self.assertEqual(len(pack), len(expected_pack))
             for args, expected in zip(pack[0], expected_pack):
                 self.assertEqual(len(args), len(expected))
@@ -863,9 +861,9 @@
         jump_to_check = jumps[0]
         try:
             validate_single_jump(jump_to_check, jumps, dag)
         except EngineInitFailed:
             self.fail("validate_single_jump shouldn't have raised")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/utils/test_command_line_args.py` & `spine_engine-0.24.0/tests/utils/test_command_line_args.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Unit tests for command line args module.
-
-"""
+""" Unit tests for command line args module. """
 
 import unittest
 from spine_engine.utils.command_line_arguments import split_cmdline_args
 
 
 class TestToolSpecification(unittest.TestCase):
     def test_split_cmdline_args(self):
@@ -28,11 +26,15 @@
         self.assertEqual(splitted, ["--input=data.dat", "-h", "5"])
         splitted = split_cmdline_args('--output="a long file name.txt"')
         self.assertEqual(splitted, ["--output=a long file name.txt"])
         splitted = split_cmdline_args("--file='file name with spaces.dat' -i 3")
         self.assertEqual(splitted, ["--file=file name with spaces.dat", "-i", "3"])
         splitted = split_cmdline_args("'quotation \"within\" a quotation'")
         self.assertEqual(splitted, ['quotation "within" a quotation'])
+        splitted = split_cmdline_args("  ")
+        self.assertEqual(splitted, [])
+        splitted = split_cmdline_args("-a  -b")
+        self.assertEqual(splitted, ["-a", "-b"])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/utils/test_helpers.py` & `spine_engine-0.24.0/tests/utils/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -183,9 +184,9 @@
         self.assertEqual(expected_output, output)
         s = 1024 * 1024 * 1024 * 2
         expected_output = "2.0 GB"
         output = get_file_size(s)
         self.assertEqual(expected_output, output)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.23.4/tests/utils/test_serialization.py` & `spine_engine-0.24.0/tests/utils/test_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ######################################################################################################################
 # Copyright (C) 2017-2022 Spine project consortium
+# Copyright Spine Engine contributors
 # This file is part of Spine Engine.
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
@@ -139,9 +140,9 @@
         self.assertTrue(path_in_dir(r"c:\path\to\file.xt", r"C:\path\\"))
 
     def test_unix_paths(self):
         self.assertTrue(path_in_dir("/path/to/my/file.dat", "/path/to"))
         self.assertFalse(path_in_dir("/path/to/my/file.dat", "/another/path"))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

