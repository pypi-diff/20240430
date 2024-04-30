# Comparing `tmp/crawlee-0.0.3b5.tar.gz` & `tmp/crawlee-0.0.3b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.3b5.tar", max compression
+gzip compressed data, was "crawlee-0.0.3b6.tar", max compression
```

## Comparing `crawlee-0.0.3b5.tar` & `crawlee-0.0.3b6.tar`

### file list

```diff
@@ -1,77 +1,79 @@
--rw-r--r--   0        0        0    11355 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/LICENSE
--rw-r--r--   0        0        0       17 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/README.md
--rw-r--r--   0        0        0     6332 2024-04-29 08:12:43.086282 crawlee-0.0.3b5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0     3341 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3365 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1950 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     4668 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     2056 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0     1585 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15793 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9293 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      186 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    14678 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     5315 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2279 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0      815 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0       86 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/beautifulsoup_crawler/__init__.py
--rw-r--r--   0        0        0     4017 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
--rw-r--r--   0        0        0      462 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/beautifulsoup_crawler/types.py
--rw-r--r--   0        0        0     1246 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/configuration.py
--rw-r--r--   0        0        0       91 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7211 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     2683 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1303 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/events/types.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/http_clients/__init__.py
--rw-r--r--   0        0        0     1615 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/http_clients/base_http_client.py
--rw-r--r--   0        0        0     2031 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/http_clients/httpx_client.py
--rw-r--r--   0        0        0       38 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     3146 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      329 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/log_config.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/py.typed
--rw-r--r--   0        0        0     5506 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/request.py
--rw-r--r--   0        0        0      365 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/__init__.py
--rw-r--r--   0        0        0     5687 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/base_resource_client.py
--rw-r--r--   0        0        0     2980 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/base_resource_collection_client.py
--rw-r--r--   0        0        0    19714 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/dataset_client.py
--rw-r--r--   0        0        0     1819 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/dataset_collection_client.py
--rw-r--r--   0        0        0    20474 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/key_value_store_client.py
--rw-r--r--   0        0        0     1936 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/key_value_store_collection_client.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/py.typed
--rw-r--r--   0        0        0    22426 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/request_queue_client.py
--rw-r--r--   0        0        0     1912 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/resource_clients/request_queue_collection_client.py
--rw-r--r--   0        0        0       67 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/sessions/__init__.py
--rw-r--r--   0        0        0     2430 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/sessions/models.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/sessions/py.typed
--rw-r--r--   0        0        0     8155 2024-04-29 08:12:19.598260 crawlee-0.0.3b5/src/crawlee/sessions/session.py
--rw-r--r--   0        0        0    11695 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/sessions/session_pool.py
--rw-r--r--   0        0        0     1645 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      106 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storage_clients/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storage_clients/base_storage_client.py
--rw-r--r--   0        0        0    11477 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storage_clients/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storage_clients/py.typed
--rw-r--r--   0        0        0      150 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     7600 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15526 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     4999 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0     6489 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/models.py
--rw-r--r--   0        0        0        0 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2611 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2742 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25845 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0      630 2024-04-29 08:12:19.602259 crawlee-0.0.3b5/src/crawlee/types.py
--rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 crawlee-0.0.3b5/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/LICENSE
+-rw-r--r--   0        0        0       17 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/README.md
+-rw-r--r--   0        0        0     6386 2024-04-30 09:08:43.136986 crawlee-0.0.3b6/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0     3341 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1950 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     4668 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     5262 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/globs.py
+-rw-r--r--   0        0        0     2056 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0     1585 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      186 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    20483 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     5749 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2279 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0     2688 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0       86 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     5359 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      524 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0     1246 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/configuration.py
+-rw-r--r--   0        0        0      272 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/enqueue_strategy.py
+-rw-r--r--   0        0        0       91 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2683 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1303 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     1615 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     2031 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       38 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     3216 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/log_config.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/py.typed
+-rw-r--r--   0        0        0     6207 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/request.py
+-rw-r--r--   0        0        0      365 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/__init__.py
+-rw-r--r--   0        0        0     5687 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/base_resource_client.py
+-rw-r--r--   0        0        0     2980 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0        0        0    19714 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/dataset_client.py
+-rw-r--r--   0        0        0     1819 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/dataset_collection_client.py
+-rw-r--r--   0        0        0    20474 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/key_value_store_client.py
+-rw-r--r--   0        0        0     1936 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/resource_clients/key_value_store_collection_client.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/resource_clients/py.typed
+-rw-r--r--   0        0        0    22452 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/resource_clients/request_queue_client.py
+-rw-r--r--   0        0        0     1912 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/resource_clients/request_queue_collection_client.py
+-rw-r--r--   0        0        0       67 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8155 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0     1645 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      106 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_clients/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_clients/base_storage_client.py
+-rw-r--r--   0        0        0    11477 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_clients/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_clients/py.typed
+-rw-r--r--   0        0        0      150 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     7600 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15526 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     4999 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0     6489 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2593 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2775 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25883 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/types.py
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 crawlee-0.0.3b6/PKG-INFO
```

### Comparing `crawlee-0.0.3b5/LICENSE` & `crawlee-0.0.3b6/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/pyproject.toml` & `crawlee-0.0.3b6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.3b5"
+version = "0.0.3b6"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -58,27 +58,28 @@
 psutil = "^5.9.8"
 pydantic = "^2.6.3"
 pydantic-settings = "^2.2.1"
 pyee = "^11.1.0"
 python-dateutil = "^2.9.0"
 sortedcollections = "^2.1.0"
 typing-extensions = "^4.1.0"
+tldextract = "^5.1.2"
 
 [tool.poetry.group.dev.dependencies]
 build = "~1.2.0"
 filelock = "~3.13.1"
 mypy = "~1.10.0"
 pre-commit = "~3.7.0"
 pydoc-markdown = "~4.8.2"
 pytest = "~8.2.0"
 pytest-asyncio = "~0.23.5"
 pytest-cov = "~5.0.0"
 pytest-only = "~2.1.0"
 pytest-timeout = "~2.3.0"
-pytest-xdist = "~3.5.0"
+pytest-xdist = "~3.6.0"
 respx = "~0.21.0"
 ruff = "~0.4.0"
 types-aiofiles = "^23.2.0.20240106"
 types-beautifulsoup4 = "^4.12.0.20240229"
 types-colorama = "~0.4.15.20240106"
 types-psutil = "~5.9.5.20240205"
 types-python-dateutil = "^2.9.0.20240316"
@@ -185,8 +186,12 @@
 [tool.mypy-scrapy]
 ignore_missing_imports = true
 
 [tool.mypy-sortedcollections]
 ignore_missing_imports = true
 
 [tool.coverage.report]
-exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
+exclude_lines = [
+    "pragma: no cover",
+    "if TYPE_CHECKING:",
+    "assert_never()"
+]
```

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.3b6/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/crypto.py` & `crawlee-0.0.3b6/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.3b6/src/crawlee/_utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/env_vars.py` & `crawlee-0.0.3b6/src/crawlee/_utils/env_vars.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/file.py` & `crawlee-0.0.3b6/src/crawlee/_utils/file.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.3b6/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/math.py` & `crawlee-0.0.3b6/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.3b6/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.3b6/src/crawlee/_utils/recurring_task.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/requests.py` & `crawlee-0.0.3b6/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/system.py` & `crawlee-0.0.3b6/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/_utils/wait.py` & `crawlee-0.0.3b6/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.3b6/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.3b6/src/crawlee/autoscaling/snapshotter.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.3b6/src/crawlee/autoscaling/system_status.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/autoscaling/types.py` & `crawlee-0.0.3b6/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.3b6/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 # Inspiration: https://github.com/apify/crawlee/blob/v3.7.3/packages/basic-crawler/src/internals/basic-crawler.ts
 from __future__ import annotations
 
+import tempfile
 from datetime import timedelta
 from functools import partial
 from logging import getLogger
-from typing import TYPE_CHECKING, Awaitable, Callable, Generic, Union, cast
+from typing import TYPE_CHECKING, AsyncGenerator, Awaitable, Callable, Generic, Sequence, Union, cast
 
 import httpx
-from typing_extensions import TypeVar
+from tldextract import TLDExtract
+from typing_extensions import TypeVar, assert_never
 
+from crawlee import Glob
 from crawlee._utils.wait import wait_for
 from crawlee.autoscaling import AutoscaledPool, ConcurrencySettings
 from crawlee.autoscaling.snapshotter import Snapshotter
 from crawlee.autoscaling.system_status import SystemStatus
 from crawlee.basic_crawler.context_pipeline import (
     ContextPipeline,
     ContextPipelineInitializationError,
+    ContextPipelineInterruptedError,
     RequestHandlerError,
 )
 from crawlee.basic_crawler.router import Router
-from crawlee.basic_crawler.types import BasicCrawlingContext, FinalStatistics, SendRequestFunction
+from crawlee.basic_crawler.types import (
+    BasicCrawlingContext,
+    FinalStatistics,
+    RequestHandlerRunResult,
+    SendRequestFunction,
+)
 from crawlee.configuration import Configuration
+from crawlee.enqueue_strategy import EnqueueStrategy
 from crawlee.events.local_event_manager import LocalEventManager
 from crawlee.http_clients.httpx_client import HttpxClient
 from crawlee.request import BaseRequestData, Request, RequestState
+from crawlee.storages.request_queue import RequestQueue
 
 if TYPE_CHECKING:
+    import re
+
     from crawlee.http_clients.base_http_client import BaseHttpClient, HttpResponse
     from crawlee.storages.request_provider import RequestProvider
 
-
 TCrawlingContext = TypeVar('TCrawlingContext', bound=BasicCrawlingContext, default=BasicCrawlingContext)
 ErrorHandler = Callable[[TCrawlingContext, Exception], Awaitable[Union[Request, None]]]
 FailedRequestHandler = Callable[[TCrawlingContext, Exception], Awaitable[None]]
 
 logger = getLogger(__name__)
 
 
@@ -51,18 +63,16 @@
     functionality themselves. If we want a crawler that already facilitates this functionality, we should consider using
     one of its subclasses.
     """
 
     def __init__(
         self,
         *,
-        request_provider: RequestProvider,
+        request_provider: RequestProvider | None = None,
         router: Callable[[TCrawlingContext], Awaitable[None]] | None = None,
-        # TODO: make request_provider optional (and instantiate based on configuration if None is supplied)
-        # https://github.com/apify/crawlee-py/issues/83
         http_client: BaseHttpClient | None = None,
         concurrency_settings: ConcurrencySettings | None = None,
         max_request_retries: int = 3,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta = timedelta(minutes=1),
         _context_pipeline: ContextPipeline[TCrawlingContext] | None = None,
     ) -> None:
@@ -85,15 +95,15 @@
             self._router = cast(Router[TCrawlingContext], router)
         elif router is not None:
             self._router = None
             self.router.default_handler(router)
 
         self._http_client = http_client or HttpxClient()
 
-        self._context_pipeline = _context_pipeline or ContextPipeline()
+        self._context_pipeline = (_context_pipeline or ContextPipeline()).compose(self._check_url_after_redirects)
 
         self._error_handler: ErrorHandler[TCrawlingContext] | None = None
         self._failed_request_handler: FailedRequestHandler[TCrawlingContext] | None = None
 
         self._max_request_retries = max_request_retries
 
         self._request_provider = request_provider
@@ -102,14 +112,16 @@
         self._request_handler_timeout = request_handler_timeout
         self._internal_timeout = (
             self._configuration.internal_timeout
             if self._configuration.internal_timeout is not None
             else max(2 * request_handler_timeout, timedelta(minutes=5))
         )
 
+        self._tld_extractor = TLDExtract(cache_dir=tempfile.TemporaryDirectory().name)
+
         self._event_manager = LocalEventManager()  # TODO: switch based on configuration
         # https://github.com/apify/crawlee-py/issues/83
         self._snapshotter = Snapshotter(self._event_manager)
         self._pool = AutoscaledPool(
             system_status=SystemStatus(self._snapshotter),
             is_finished_function=self.__is_finished_function,
             is_task_ready_function=self.__is_task_ready_function,
@@ -128,14 +140,21 @@
     @router.setter
     def router(self, router: Router[TCrawlingContext]) -> None:
         if self._router is not None:
             raise RuntimeError('A router is already set')
 
         self._router = router
 
+    async def get_request_provider(self) -> RequestProvider:
+        """Return the configured request provider. If none is configured, open and return the default request queue."""
+        if not self._request_provider:
+            self._request_provider = await RequestQueue.open()
+
+        return self._request_provider
+
     def error_handler(self, handler: ErrorHandler[TCrawlingContext]) -> ErrorHandler[TCrawlingContext]:
         """Decorator for configuring an error handler (called after a request handler error and before retrying)."""
         self._error_handler = handler
         return handler
 
     def failed_request_handler(
         self, handler: FailedRequestHandler[TCrawlingContext]
@@ -149,15 +168,16 @@
         requests: list[str | BaseRequestData],
         *,
         batch_size: int = 1000,
         wait_for_all_requests_to_be_added: bool = False,
         wait_time_between_batches: timedelta = timedelta(0),
     ) -> None:
         """Add requests to the underlying queue."""
-        await self._request_provider.add_requests_batched(
+        request_provider = await self.get_request_provider()
+        await request_provider.add_requests_batched(
             [
                 request if isinstance(request, BaseRequestData) else BaseRequestData.from_url(url=request)
                 for request in requests
             ],
             batch_size=batch_size,
             wait_for_all_requests_to_be_added=wait_for_all_requests_to_be_added,
             wait_time_between_batches=wait_time_between_batches,
@@ -178,32 +198,102 @@
         if max_request_retries is None:
             max_request_retries = self._max_request_retries
 
         return (
             not crawling_context.request.no_retry and (crawling_context.request.retry_count + 1) < max_request_retries
         )
 
+    async def _check_url_after_redirects(
+        self, crawling_context: TCrawlingContext
+    ) -> AsyncGenerator[TCrawlingContext, None]:
+        """Invoked at the end of the context pipeline to make sure that the `loaded_url` still matches enqueue_strategy.
+
+        This is done to filter out links that redirect outside of the crawled domain.
+        """
+        if crawling_context.request.loaded_url is not None and not self._check_enqueue_strategy(
+            crawling_context.request.enqueue_strategy,
+            origin_url=httpx.URL(crawling_context.request.url),
+            target_url=httpx.URL(crawling_context.request.loaded_url),
+        ):
+            raise ContextPipelineInterruptedError(
+                f'Skipping URL {crawling_context.request.loaded_url} (redirected from {crawling_context.request.url})'
+            )
+
+        yield crawling_context
+
+    def _check_enqueue_strategy(
+        self, strategy: EnqueueStrategy, *, target_url: httpx.URL, origin_url: httpx.URL
+    ) -> bool:
+        """Check if a URL matches the enqueue_strategy."""
+        if strategy == EnqueueStrategy.SAME_HOSTNAME:
+            return target_url.host == origin_url.host
+
+        if strategy == EnqueueStrategy.SAME_DOMAIN:
+            origin_domain = self._tld_extractor.extract_str(origin_url.host).domain
+            target_domain = self._tld_extractor.extract_str(target_url.host).domain
+            return origin_domain == target_domain
+
+        if strategy == EnqueueStrategy.SAME_ORIGIN:
+            return target_url.host == origin_url.host and target_url.scheme == origin_url.scheme
+
+        if strategy == EnqueueStrategy.ALL:
+            return True
+
+        assert_never()
+
+    def _check_url_patterns(
+        self,
+        target_url: httpx.URL,
+        include: Sequence[re.Pattern | Glob] | None,
+        exclude: Sequence[re.Pattern | Glob] | None,
+    ) -> bool:
+        """Check if a URL matches configured include/exclude patterns."""
+        # If the URL matches any `exclude` pattern, reject it
+        for pattern in exclude or ():
+            if isinstance(pattern, Glob):
+                pattern = pattern.regexp  # noqa: PLW2901
+
+            if pattern.match(str(target_url)) is not None:
+                return False
+
+        # If there are no `include` patterns and the URL passed all `exclude` patterns, accept the URL
+        if include is None:
+            return True
+
+        # If the URL matches any `include` pattern, accept it
+        for pattern in include:
+            if isinstance(pattern, Glob):
+                pattern = pattern.regexp  # noqa: PLW2901
+
+            if pattern.match(str(target_url)) is not None:
+                return True
+
+        # The URL does not match any `include` pattern - reject it
+        return False
+
     async def _handle_request_error(self, crawling_context: TCrawlingContext, error: Exception) -> None:
+        request_provider = await self.get_request_provider()
+
         if self._should_retry_request(crawling_context):
             request = crawling_context.request
             request.retry_count += 1
 
             if self._error_handler:
                 try:
                     new_request = await self._error_handler(crawling_context, error)
                 except Exception as e:
                     raise UserDefinedErrorHandlerError('Exception thrown in user-defined request error handler') from e
                 else:
                     if new_request is not None:
                         request = new_request
 
-            await self._request_provider.reclaim_request(request)
+            await request_provider.reclaim_request(request)
         else:
             await wait_for(
-                lambda: self._request_provider.mark_request_as_handled(crawling_context.request),
+                lambda: request_provider.mark_request_as_handled(crawling_context.request),
                 timeout=self._internal_timeout,
                 timeout_message='Marking request as handled timed out after '
                 f'{self._internal_timeout.total_seconds()} seconds',
                 logger=logger,
                 max_retries=3,
             )
             await self._handle_failed_request(crawling_context, error)
@@ -219,50 +309,91 @@
 
     def _prepare_send_request_function(self) -> SendRequestFunction:
         async def send_request(url: str, *, method: str = 'get', headers: dict[str, str] | None = None) -> HttpResponse:
             return await self._http_client.send_request(url, method=method, headers=httpx.Headers(headers))
 
         return send_request
 
+    async def _commit_request_handler_result(
+        self, context: BasicCrawlingContext, result: RequestHandlerRunResult
+    ) -> None:
+        request_provider = await self.get_request_provider()
+        origin = httpx.URL(context.request.loaded_url or context.request.url)
+
+        for call in result.add_requests_calls:
+            requests = list[BaseRequestData]()
+
+            for request in call['requests']:
+                if (limit := call.get('limit')) is not None and len(requests) >= limit:
+                    break
+
+                request_model = request if isinstance(request, BaseRequestData) else BaseRequestData.from_url(request)
+                destination = httpx.URL(request_model.url)
+                if destination.is_relative_url:
+                    base_url = httpx.URL(call.get('base_url', origin))
+                    request_model.url = str(base_url.join(destination))
+
+                if self._check_enqueue_strategy(
+                    call.get('strategy', EnqueueStrategy.ALL), target_url=destination, origin_url=origin
+                ) and self._check_url_patterns(destination, call.get('include', None), call.get('exclude', None)):
+                    requests.append(request_model)
+
+            await request_provider.add_requests_batched(
+                requests=requests,
+                wait_for_all_requests_to_be_added=False,
+            )
+
     async def __is_finished_function(self) -> bool:
-        return await self._request_provider.is_finished()
+        request_provider = await self.get_request_provider()
+        return await request_provider.is_finished()
 
     async def __is_task_ready_function(self) -> bool:
-        return not await self._request_provider.is_empty()
+        request_provider = await self.get_request_provider()
+        return not await request_provider.is_empty()
 
     async def __run_task_function(self) -> None:
+        request_provider = await self.get_request_provider()
+
         request = await wait_for(
-            lambda: self._request_provider.fetch_next_request(),
+            lambda: request_provider.fetch_next_request(),
             timeout=self._internal_timeout,
             timeout_message=f'Fetching next request failed after {self._internal_timeout.total_seconds()} seconds',
             logger=logger,
             max_retries=3,
         )
 
         if request is None:
             return
 
         # TODO: fetch session from the session pool
         # https://github.com/apify/crawlee-py/issues/110
 
-        crawling_context = BasicCrawlingContext(request=request, send_request=self._prepare_send_request_function())
+        result = RequestHandlerRunResult()
+
+        crawling_context = BasicCrawlingContext(
+            request=request,
+            send_request=self._prepare_send_request_function(),
+            add_requests=result.add_requests,
+        )
 
         try:
             request.state = RequestState.REQUEST_HANDLER
 
             await wait_for(
                 lambda: self.__run_request_handler(crawling_context),
                 timeout=self._request_handler_timeout,
                 timeout_message='Request handler timed out after '
                 f'{self._request_handler_timeout.total_seconds()} seconds',
                 logger=logger,
             )
 
+            await self._commit_request_handler_result(crawling_context, result)
+
             await wait_for(
-                lambda: self._request_provider.mark_request_as_handled(crawling_context.request),
+                lambda: request_provider.mark_request_as_handled(crawling_context.request),
                 timeout=self._internal_timeout,
                 timeout_message='Marking request as handled timed out after '
                 f'{self._internal_timeout.total_seconds()} seconds',
                 logger=logger,
                 max_retries=3,
             )
 
@@ -293,30 +424,41 @@
                 logger.exception(
                     'An exception occurred during handling of failed request. This places the crawler '
                     'and its underlying storages into an unknown state and crawling will be terminated.',
                     exc_info=secondary_error,
                 )
                 request.state = RequestState.ERROR
                 raise
+        except ContextPipelineInterruptedError as interruped_error:
+            logger.debug('The context pipeline was interrupted', exc_info=interruped_error)
+
+            await wait_for(
+                lambda: request_provider.mark_request_as_handled(crawling_context.request),
+                timeout=self._internal_timeout,
+                timeout_message='Marking request as handled timed out after '
+                f'{self._internal_timeout.total_seconds()} seconds',
+                logger=logger,
+                max_retries=3,
+            )
         except ContextPipelineInitializationError as initialization_error:
             if self._should_retry_request(crawling_context):
                 logger.debug(
                     'An exception occured during the initialization of crawling context, a retry is in order',
                     exc_info=initialization_error,
                 )
 
                 request = crawling_context.request
                 request.retry_count += 1
                 request.state = RequestState.DONE
-                await self._request_provider.reclaim_request(request)
+                await request_provider.reclaim_request(request)
             else:
                 logger.exception('Request failed and reached maximum retries', exc_info=initialization_error)
 
                 await wait_for(
-                    lambda: self._request_provider.mark_request_as_handled(crawling_context.request),
+                    lambda: request_provider.mark_request_as_handled(crawling_context.request),
                     timeout=self._internal_timeout,
                     timeout_message='Marking request as handled timed out after '
                     f'{self._internal_timeout.total_seconds()} seconds',
                     logger=logger,
                     max_retries=3,
                 )
         except Exception as internal_error:
```

### Comparing `crawlee-0.0.3b5/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.3b6/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     """
 
     def __init__(self, wrapped_exception: Exception, crawling_context: BasicCrawlingContext) -> None:
         self.wrapped_exception = wrapped_exception
         self.crawling_context = crawling_context
 
 
+class ContextPipelineInterruptedError(Exception):
+    """May be thrown in the initialization phase of a middleware to signal that the request should not be processed."""
+
+
 class ContextPipelineFinalizationError(Exception):
     """Wraps an exception thrown in the finalization step of a context pipeline middleware.
 
     We may not have the complete context at this point, so only `BasicCrawlingContext` is provided.
     """
 
     def __init__(self, wrapped_exception: Exception, crawling_context: BasicCrawlingContext) -> None:
@@ -81,14 +85,16 @@
             for member in reversed(chain):
                 if member._middleware:  # noqa: SLF001
                     middleware_instance = member._middleware(crawling_context)  # noqa: SLF001
                     try:
                         result = await middleware_instance.__anext__()
                     except StopAsyncIteration as e:
                         raise RuntimeError('The middleware did not yield') from e
+                    except ContextPipelineInterruptedError:
+                        raise
                     except Exception as e:
                         raise ContextPipelineInitializationError(e, crawling_context) from e
 
                     crawling_context = result
                     cleanup_stack.append(middleware_instance)
 
             try:
@@ -97,14 +103,16 @@
                 raise RequestHandlerError(e, crawling_context) from e
         finally:
             for middleware_instance in reversed(cleanup_stack):
                 try:
                     result = await middleware_instance.__anext__()
                 except StopAsyncIteration:  # noqa: PERF203
                     pass
+                except ContextPipelineInterruptedError as e:
+                    raise RuntimeError('Invalid state - pipeline interrupted in the finalization step') from e
                 except Exception as e:
                     raise ContextPipelineFinalizationError(e, crawling_context) from e
                 else:
                     raise RuntimeError('The middleware yielded more than once')
 
     def compose(
         self,
```

### Comparing `crawlee-0.0.3b5/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.3b6/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py` & `crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from __future__ import annotations
 
 import asyncio
 from datetime import timedelta
-from typing import TYPE_CHECKING, AsyncGenerator, Awaitable, Callable, Iterable, Literal
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Callable, Iterable, Literal
 
 import httpx
+from typing_extensions import Unpack
 
 from crawlee.basic_crawler.basic_crawler import BasicCrawler
 from crawlee.basic_crawler.context_pipeline import ContextPipeline
 from crawlee.beautifulsoup_crawler.types import BeautifulSoupCrawlingContext
+from crawlee.enqueue_strategy import EnqueueStrategy
 from crawlee.http_clients.httpx_client import HttpxClient
 from crawlee.http_crawler.types import HttpCrawlingContext
+from crawlee.request import BaseRequestData
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
     from crawlee.autoscaling.autoscaled_pool import ConcurrencySettings
-    from crawlee.basic_crawler.types import BasicCrawlingContext
+    from crawlee.basic_crawler.types import AddRequestsFunctionKwargs, BasicCrawlingContext
     from crawlee.configuration import Configuration
     from crawlee.storages.request_provider import RequestProvider
 
 
 class BeautifulSoupCrawler(BasicCrawler[BeautifulSoupCrawlingContext]):
     """A crawler that fetches the request URL using `httpx` and parses the result with `BeautifulSoup`."""
 
     def __init__(
         self,
         *,
         parser: Literal['html.parser', 'lxml', 'xml', 'html5lib'] = 'lxml',
-        request_provider: RequestProvider,
+        request_provider: RequestProvider | None = None,
         router: Callable[[BeautifulSoupCrawlingContext], Awaitable[None]] | None = None,
         concurrency_settings: ConcurrencySettings | None = None,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta | None = None,
         additional_http_error_status_codes: Iterable[int] = (),
         ignore_http_error_status_codes: Iterable[int] = (),
     ) -> None:
@@ -79,19 +82,53 @@
             **basic_crawler_kwargs,  # type: ignore
         )
 
     async def _make_http_request(self, context: BasicCrawlingContext) -> AsyncGenerator[HttpCrawlingContext, None]:
         result = await self._http_client.crawl(context.request)
 
         yield HttpCrawlingContext(
-            request=context.request, send_request=context.send_request, http_response=result.http_response
+            request=context.request,
+            send_request=context.send_request,
+            add_requests=context.add_requests,
+            http_response=result.http_response,
         )
 
     async def _parse_http_response(
         self, context: HttpCrawlingContext
     ) -> AsyncGenerator[BeautifulSoupCrawlingContext, None]:
-        from bs4 import BeautifulSoup
+        from bs4 import BeautifulSoup, Tag
 
         soup = await asyncio.to_thread(lambda: BeautifulSoup(context.http_response.read(), self._parser))
+
+        async def enqueue_links(
+            *,
+            selector: str = 'a',
+            label: str | None = None,
+            user_data: dict[str, Any] | None = None,
+            **kwargs: Unpack[AddRequestsFunctionKwargs],
+        ) -> None:
+            requests = list[BaseRequestData]()
+            user_data = user_data or {}
+
+            link: Tag
+            for link in soup.find_all(selector):
+                link_user_data = user_data
+
+                if label is not None:
+                    link_user_data.setdefault('label', label)
+
+                if (href := link.attrs.get('href')) is not None:
+                    requests.append(BaseRequestData.from_url(href, user_data=link_user_data))
+
+            uses_patterns = 'include' in kwargs or 'exclude' in kwargs
+            kwargs.setdefault('strategy', EnqueueStrategy.SAME_HOSTNAME if uses_patterns else EnqueueStrategy.ALL)
+
+            await context.add_requests(requests, **kwargs)
+
         yield BeautifulSoupCrawlingContext(
-            request=context.request, send_request=context.send_request, http_response=context.http_response, soup=soup
+            request=context.request,
+            send_request=context.send_request,
+            add_requests=context.add_requests,
+            enqueue_links=enqueue_links,
+            http_response=context.http_response,
+            soup=soup,
         )
```

### Comparing `crawlee-0.0.3b5/src/crawlee/configuration.py` & `crawlee-0.0.3b6/src/crawlee/configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/events/event_manager.py` & `crawlee-0.0.3b6/src/crawlee/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.3b6/src/crawlee/events/local_event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/events/types.py` & `crawlee-0.0.3b6/src/crawlee/events/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/http_clients/base_http_client.py` & `crawlee-0.0.3b6/src/crawlee/http_clients/base_http_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/http_clients/httpx_client.py` & `crawlee-0.0.3b6/src/crawlee/http_clients/httpx_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/http_crawler/http_crawler.py` & `crawlee-0.0.3b6/src/crawlee/http_crawler/http_crawler.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class HttpCrawler(BasicCrawler[HttpCrawlingContext]):
     """A crawler that fetches the request URL using `httpx`."""
 
     def __init__(
         self,
         *,
-        request_provider: RequestProvider,
+        request_provider: RequestProvider | None = None,
         router: Callable[[HttpCrawlingContext], Awaitable[None]] | None = None,
         concurrency_settings: ConcurrencySettings | None = None,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta | None = None,
         additional_http_error_status_codes: Iterable[int] = (),
         ignore_http_error_status_codes: Iterable[int] = (),
     ) -> None:
@@ -72,9 +72,10 @@
         self, crawling_context: BasicCrawlingContext
     ) -> AsyncGenerator[HttpCrawlingContext, None]:
         result = await self._http_client.crawl(crawling_context.request)
 
         yield HttpCrawlingContext(
             request=crawling_context.request,
             send_request=crawling_context.send_request,
+            add_requests=crawling_context.add_requests,
             http_response=result.http_response,
         )
```

### Comparing `crawlee-0.0.3b5/src/crawlee/log_config.py` & `crawlee-0.0.3b6/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/request.py` & `crawlee-0.0.3b6/src/crawlee/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from enum import Enum
 from typing import Annotated, Any
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Self
 
 from crawlee._utils.requests import compute_unique_key, unique_key_to_request_id
+from crawlee.enqueue_strategy import EnqueueStrategy
 
 
 class BaseRequestData(BaseModel):
     """Data needed to create a new crawling request."""
 
     model_config = ConfigDict(populate_by_name=True)
 
@@ -34,15 +35,15 @@
 
     method: str = 'get'
 
     payload: str | None = None
 
     headers: Annotated[dict[str, str] | None, Field(default_factory=dict)] = None
 
-    user_data: Annotated[dict[str, Any] | None, Field(alias='userData')] = None
+    user_data: Annotated[dict[str, Any], Field(alias='userData', default_factory=dict)]
     """Custom user data assigned to the request. Use this to save any request related data to the
     request's scope, keeping them accessible on retries, failures etc.
     """
 
     retry_count: Annotated[int, Field(alias='retryCount')] = 0
 
     no_retry: Annotated[bool, Field(alias='noRetry')] = False
@@ -52,20 +53,26 @@
     handled_at: Annotated[datetime | None, Field(alias='handledAt')] = None
 
     @classmethod
     def from_url(
         cls,
         url: str,
         *,
+        label: str | None = None,
         unique_key: str | None = None,
         **kwargs: Any,
     ) -> Self:
         """Create a new `RequestData` instance from a URL."""
         unique_key = unique_key or compute_unique_key(url)
-        return cls(url=url, unique_key=unique_key, **kwargs)
+        result = cls(url=url, unique_key=unique_key, **kwargs)
+
+        if label is not None:
+            result.user_data['label'] = label
+
+        return result
 
 
 class Request(BaseRequestData):
     """A crawling request (as returned from a request queue)."""
 
     id: str
 
@@ -76,66 +83,81 @@
     # https://github.com/apify/crawlee-py/issues/94
 
     @classmethod
     def from_url(
         cls,
         url: str,
         *,
+        label: str | None = None,
         unique_key: str | None = None,
         id: str | None = None,
         **kwargs: Any,
     ) -> Self:
         """Create a new `RequestData` instance from a URL."""
         unique_key = unique_key or compute_unique_key(url)
         id = id or unique_key_to_request_id(unique_key)
-        return cls(url=url, unique_key=unique_key, id=id, **kwargs)
+
+        result = cls(url=url, unique_key=unique_key, id=id, **kwargs)
+
+        if label is not None:
+            result.user_data['label'] = label
+
+        return result
 
     @classmethod
     def from_base_request_data(cls, base_request_data: BaseRequestData, *, id: str | None = None) -> Self:
         """Create a complete Request object based on a BaseRequestData instance."""
         return cls(**base_request_data.model_dump(), id=id or unique_key_to_request_id(base_request_data.unique_key))
 
     @property
-    def crawlee_data(self) -> CrawleeRequestData:
-        """Crawlee-specific configuration stored in the user_data."""
-        return CrawleeRequestData.model_validate(self.user_data.get('__crawlee', {}) if self.user_data else {})
-
-    @property
     def label(self) -> str | None:
         """A string used to differentiate between arbitrary request types."""
-        if self.user_data and 'label' in self.user_data:
+        if 'label' in self.user_data:
             return str(self.user_data['label'])
         return None
 
     @property
+    def crawlee_data(self) -> CrawleeRequestData:
+        """Crawlee-specific configuration stored in the user_data."""
+        return CrawleeRequestData.model_validate(self.user_data.get('__crawlee', {}))
+
+    @property
     def state(self) -> RequestState | None:
         """Crawlee-specific request handling state."""
         return self.crawlee_data.state
 
     @state.setter
     def state(self, new_state: RequestState) -> None:
-        if self.user_data is None:
-            self.user_data = {}
-
         self.user_data.setdefault('__crawlee', {})
         self.user_data['__crawlee']['state'] = new_state
 
     @property
     def max_retries(self) -> int | None:
         """Crawlee-specific limit on the number of retries of the request."""
         return self.crawlee_data.max_retries
 
     @max_retries.setter
     def max_retries(self, new_max_retries: int) -> None:
-        if self.user_data is None:
-            self.user_data = {}
-
         self.user_data.setdefault('__crawlee', {})
         self.user_data['__crawlee']['maxRetries'] = new_max_retries
 
+    @property
+    def enqueue_strategy(self) -> EnqueueStrategy:
+        """The strategy used when enqueueing the request."""
+        return (
+            EnqueueStrategy(self.crawlee_data.enqueue_strategy)
+            if self.crawlee_data.enqueue_strategy
+            else EnqueueStrategy.ALL
+        )
+
+    @enqueue_strategy.setter
+    def enqueue_strategy(self, new_enqueue_strategy: EnqueueStrategy) -> None:
+        self.user_data.setdefault('__crawlee', {})
+        self.user_data['__crawlee']['enqueueStrategy'] = str(new_enqueue_strategy)
+
 
 class RequestState(Enum):
     """Crawlee-specific request handling state."""
 
     UNPROCESSED = 0
     BEFORE_NAV = 1
     AFTER_NAV = 2
```

### Comparing `crawlee-0.0.3b5/src/crawlee/resource_clients/base_resource_client.py` & `crawlee-0.0.3b6/src/crawlee/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/resource_clients/base_resource_collection_client.py` & `crawlee-0.0.3b6/src/crawlee/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/resource_clients/dataset_client.py` & `crawlee-0.0.3b6/src/crawlee/resource_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/resource_clients/dataset_collection_client.py` & `crawlee-0.0.3b6/src/crawlee/resource_clients/dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/resource_clients/key_value_store_client.py` & `crawlee-0.0.3b6/src/crawlee/resource_clients/key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/resource_clients/key_value_store_collection_client.py` & `crawlee-0.0.3b6/src/crawlee/resource_clients/key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/resource_clients/request_queue_client.py` & `crawlee-0.0.3b6/src/crawlee/resource_clients/request_queue_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,14 +545,15 @@
             url=request.url,
             unique_key=request.unique_key,
             id=id,
             method=request.method,
             retry_count=request.retry_count,
             order_no=order_no,
             json_=json_request,
+            user_data={},
         )
 
     def _calculate_order_no(self, request: Request, forefront: bool | None) -> Decimal | None:
         if request.handled_at is not None:
             return None
 
         # Get the current timestamp in milliseconds
```

### Comparing `crawlee-0.0.3b5/src/crawlee/resource_clients/request_queue_collection_client.py` & `crawlee-0.0.3b6/src/crawlee/resource_clients/request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/sessions/models.py` & `crawlee-0.0.3b6/src/crawlee/sessions/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/sessions/session.py` & `crawlee-0.0.3b6/src/crawlee/sessions/session.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/sessions/session_pool.py` & `crawlee-0.0.3b6/src/crawlee/sessions/session_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/storage_client_manager.py` & `crawlee-0.0.3b6/src/crawlee/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/storage_clients/base_storage_client.py` & `crawlee-0.0.3b6/src/crawlee/storage_clients/base_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/storage_clients/memory_storage_client.py` & `crawlee-0.0.3b6/src/crawlee/storage_clients/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/storages/base_storage.py` & `crawlee-0.0.3b6/src/crawlee/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/storages/dataset.py` & `crawlee-0.0.3b6/src/crawlee/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.3b6/src/crawlee/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/storages/models.py` & `crawlee-0.0.3b6/src/crawlee/storages/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/src/crawlee/storages/request_list.py` & `crawlee-0.0.3b6/src/crawlee/storages/request_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from __future__ import annotations
 
 from collections import deque
-from typing import TYPE_CHECKING
+from datetime import timedelta
 
 from typing_extensions import override
 
 from crawlee.request import BaseRequestData, Request
 from crawlee.storages.request_provider import RequestProvider
 
-if TYPE_CHECKING:
-    from datetime import timedelta
-
 
 class RequestList(RequestProvider):
     """Represents a (potentially very large) list of URLs to crawl."""
 
     def __init__(self, sources: list[str | Request] | None = None, name: str | None = None) -> None:
         """Initialize the RequestList.
 
@@ -77,14 +74,14 @@
         return self._handled_count
 
     @override
     async def add_requests_batched(
         self,
         requests: list[BaseRequestData | Request],
         *,
-        batch_size: int,
-        wait_for_all_requests_to_be_added: bool,
-        wait_time_between_batches: timedelta,
+        batch_size: int = 1000,
+        wait_for_all_requests_to_be_added: bool = False,
+        wait_time_between_batches: timedelta = timedelta(seconds=1),
     ) -> None:
         self._sources.extend(
             request if isinstance(request, Request) else Request.from_base_request_data(request) for request in requests
         )
```

### Comparing `crawlee-0.0.3b5/src/crawlee/storages/request_provider.py` & `crawlee-0.0.3b6/src/crawlee/storages/request_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from datetime import timedelta
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from datetime import timedelta
-
     from crawlee.request import BaseRequestData, Request
     from crawlee.storages.models import RequestQueueOperationInfo
 
 
 class RequestProvider(ABC):
     """Provides access to a queue of crawling requests."""
 
@@ -54,17 +53,17 @@
         """Returns the number of handled requests."""
 
     @abstractmethod
     async def add_requests_batched(
         self,
         requests: list[BaseRequestData | Request],
         *,
-        batch_size: int,
-        wait_for_all_requests_to_be_added: bool,
-        wait_time_between_batches: timedelta,
+        batch_size: int = 1000,
+        wait_for_all_requests_to_be_added: bool = False,
+        wait_time_between_batches: timedelta = timedelta(seconds=1),
     ) -> None:
         """Adds requests to the queue in batches.
 
         By default, it will resolve after the initial batch is added, and continue adding the rest in background.
         You can configure the batch size via `batch_size` option and the sleep time in between the batches
         via `wait_time_between_batches`. If you want to wait for all batches to be added to the queue, you can use
         the `wait_for_all_requests_to_be_added` option.
```

### Comparing `crawlee-0.0.3b5/src/crawlee/storages/request_queue.py` & `crawlee-0.0.3b6/src/crawlee/storages/request_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,17 +204,17 @@
         return queue_operation_info
 
     @override
     async def add_requests_batched(
         self,
         requests: list[BaseRequestData | Request],
         *,
-        batch_size: int,
-        wait_for_all_requests_to_be_added: bool,
-        wait_time_between_batches: timedelta,
+        batch_size: int = 1000,
+        wait_for_all_requests_to_be_added: bool = False,
+        wait_time_between_batches: timedelta = timedelta(seconds=1),
     ) -> None:
         for request in requests:
             if isinstance(request, Request):
                 await self.add_request(request)
             else:
                 await self.add_request(Request.from_base_request_data(request))
```

### Comparing `crawlee-0.0.3b5/src/crawlee/types.py` & `crawlee-0.0.3b6/src/crawlee/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b5/PKG-INFO` & `crawlee-0.0.3b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.3b5
+Version: 0.0.3b6
 Summary: Crawlee for Python
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -30,14 +30,15 @@
 Requires-Dist: more_itertools (>=10.2.0,<11.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pyee (>=11.1.0,<12.0.0)
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: sortedcollections (>=2.1.0,<3.0.0)
+Requires-Dist: tldextract (>=5.1.2,<6.0.0)
 Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/crawlee-py/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://todo.com/
 Project-URL: Homepage, https://todo.com/
 Project-URL: Issue Tracker, https://github.com/apify/crawlee-py/issues
 Project-URL: Repository, https://github.com/apify/crawlee-py
```

