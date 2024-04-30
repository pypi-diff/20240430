# Comparing `tmp/baseplate-2.7.0a1.tar.gz` & `tmp/baseplate-2.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseplate-2.7.0a1.tar", last modified: Mon Mar 18 15:57:59 2024, max compression
+gzip compressed data, was "baseplate-2.7.0b1.tar", max compression
```

## Comparing `baseplate-2.7.0a1.tar` & `baseplate-2.7.0b1.tar`

### file list

```diff
@@ -1,326 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.757557 baseplate-2.7.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.713557 baseplate-2.7.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.721557 baseplate-2.7.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    26307 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-18 15:57:59.757557 baseplate-2.7.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.721557 baseplate-2.7.0a1/baseplate/
--rw-r--r--   0 runner    (1001) docker     (127)    26348 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.725557 baseplate-2.7.0a1/baseplate/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/kombu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.725557 baseplate-2.7.0a1/baseplate/clients/memcache/
--rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/memcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/memcache/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/redis_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14716 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/clients/thrift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.725557 baseplate-2.7.0a1/baseplate/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.725557 baseplate-2.7.0a1/baseplate/frameworks/pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/frameworks/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/frameworks/pyramid/csrf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.725557 baseplate-2.7.0a1/baseplate/frameworks/queue_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/frameworks/queue_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/frameworks/queue_consumer/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/frameworks/queue_consumer/kombu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.725557 baseplate-2.7.0a1/baseplate/frameworks/thrift/
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/frameworks/thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/frameworks/thrift/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.729557 baseplate-2.7.0a1/baseplate/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    17148 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/edgecontext.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/file_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.729557 baseplate-2.7.0a1/baseplate/lib/live_data/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/live_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/live_data/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/live_data/zookeeper.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/message_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    19944 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/prometheus_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.729557 baseplate-2.7.0a1/baseplate/lib/ratelimit/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/ratelimit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.729557 baseplate-2.7.0a1/baseplate/lib/ratelimit/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/ratelimit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/ratelimit/backends/memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/ratelimit/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/ratelimit/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17956 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lib/thrift_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.729557 baseplate-2.7.0a1/baseplate/lint/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lint/db_query_string_format_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/lint/example_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.729557 baseplate-2.7.0a1/baseplate/observers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/observers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/observers/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/observers/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/observers/metrics_tagged.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/observers/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/observers/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)    22594 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/observers/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.733557 baseplate-2.7.0a1/baseplate/server/
--rw-r--r--   0 runner    (1001) docker     (127)    18542 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/einhorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/monkey.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/queue_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/reloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/runtime_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/thrift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.733557 baseplate-2.7.0a1/baseplate/sidecars/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/sidecars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/sidecars/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/sidecars/live_data_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/sidecars/secrets_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/sidecars/trace_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.733557 baseplate-2.7.0a1/baseplate/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.733557 baseplate-2.7.0a1/baseplate/testing/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/testing/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/testing/lib/file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/testing/lib/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.733557 baseplate-2.7.0a1/baseplate/thrift/
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/thrift/BaseplateService.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/thrift/BaseplateServiceV2.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/thrift/baseplate.thrift
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/thrift/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/baseplate/thrift/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.721557 baseplate-2.7.0a1/baseplate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-18 15:57:59.000000 baseplate-2.7.0a1/baseplate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-03-18 15:57:59.000000 baseplate-2.7.0a1/baseplate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 15:57:59.000000 baseplate-2.7.0a1/baseplate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-18 15:57:59.000000 baseplate-2.7.0a1/baseplate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 15:57:59.000000 baseplate-2.7.0a1/baseplate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-18 15:57:59.000000 baseplate-2.7.0a1/baseplate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-18 15:57:59.000000 baseplate-2.7.0a1/baseplate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.733557 baseplate-2.7.0a1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/bin/baseplate-healthcheck
--rwxr-xr-x   0 runner    (1001) docker     (127)      466 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/bin/baseplate-script
--rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/bin/baseplate-serve
--rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/bin/baseplate-shell
--rwxr-xr-x   0 runner    (1001) docker     (127)      567 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/bin/baseplate-tshell
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.737557 baseplate-2.7.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.737557 baseplate-2.7.0a1/docs/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.737557 baseplate-2.7.0a1/docs/api/baseplate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.737557 baseplate-2.7.0a1/docs/api/baseplate/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/cassandra.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/kombu.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/memcache.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/redis.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/redis_cluster.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/requests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/sqlalchemy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/clients/thrift.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.737557 baseplate-2.7.0a1/docs/api/baseplate/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/frameworks/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/frameworks/pyramid.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.737557 baseplate-2.7.0a1/docs/api/baseplate/frameworks/queue_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/frameworks/queue_consumer/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/frameworks/queue_consumer/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/frameworks/queue_consumer/kombu.rst
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/frameworks/thrift.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.741557 baseplate-2.7.0a1/docs/api/baseplate/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/crypto.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/edgecontext.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/file_watcher.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/live_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/message_queue.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/random.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/ratelimit.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/retry.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/secrets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/service_discovery.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/lib/thrift_pool.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.741557 baseplate-2.7.0a1/docs/api/baseplate/observers/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/observers/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/observers/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/observers/sentry.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/observers/statsd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/observers/tagged_statsd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/observers/timeout.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/baseplate/observers/tracing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/library.rst
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/api/observability-framework.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.741557 baseplate-2.7.0a1/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/cli/healthcheck.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/cli/script.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/cli/serve.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/cli/shell.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/config_dictof_example.ini
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/config_dictof_spec_example.ini
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/config_example.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.741557 baseplate-2.7.0a1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/guide/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/guide/startup.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    96286 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/images/baseplate.png
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/docs/lint/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/lint/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/secrets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/docs/tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/docs/tutorial/chapter1/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter1/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/docs/tutorial/chapter2/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter2/helloworld.ini
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter2/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/docs/tutorial/chapter3/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter3/helloworld.ini
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter3/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter3/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/docs/tutorial/chapter4/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter4/helloworld.ini
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter4/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/chapter4/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/docs/watched_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/pylint_baseplate_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-18 15:57:59.757557 baseplate-2.7.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.745557 baseplate-2.7.0a1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/data/file_watcher_tests.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.749557 baseplate-2.7.0a1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/cassandra_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.749557 baseplate-2.7.0a1/tests/integration/live_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/live_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/live_data/writer_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/live_data/zookeeper_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/memcache_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/message_queue_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/pyramid_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/ratelimit_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/redis_cluster_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/redis_testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/redis_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/requests_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/sqlalchemy_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/test.thrift
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.749557 baseplate-2.7.0a1/tests/integration/test_thrift/
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/test_thrift/TestService.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/test_thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/test_thrift/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/test_thrift/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23297 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/thrift_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/timeout_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/integration/tracing_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.749557 baseplate-2.7.0a1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.749557 baseplate-2.7.0a1/tests/unit/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/cassandra_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/kombu_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    18814 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/memcache_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/redis_cluster_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/redis_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/requests_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/sqlalchemy_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/clients/thrift_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    13228 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/core_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.749557 baseplate-2.7.0a1/tests/unit/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.749557 baseplate-2.7.0a1/tests/unit/frameworks/pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/frameworks/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/frameworks/pyramid/csrf_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/frameworks/pyramid/http_server_prom_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.749557 baseplate-2.7.0a1/tests/unit/frameworks/queue_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/frameworks/queue_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28081 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/frameworks/queue_consumer/kafka_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    22153 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/frameworks/queue_consumer/kombu_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/frameworks/thrift_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.753557 baseplate-2.7.0a1/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/config_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/crypto_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/datetime_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.753557 baseplate-2.7.0a1/tests/unit/lib/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/events/publisher_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/events/queue_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/file_watcher_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/log_formatter_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15438 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/metrics_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/random_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/ratelimit_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/retry_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.753557 baseplate-2.7.0a1/tests/unit/lib/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/secrets/store_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/secrets/vault_csi_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/service_discovery_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lib/thrift_pool_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.753557 baseplate-2.7.0a1/tests/unit/lint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lint/db_query_string_format_plugin_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/lint/example_plugin_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.753557 baseplate-2.7.0a1/tests/unit/observers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/observers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/observers/metrics_tagged_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/observers/metrics_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/observers/sentry_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.753557 baseplate-2.7.0a1/tests/unit/observers/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/observers/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/observers/tracing/publisher_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/observers/tracing_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.757557 baseplate-2.7.0a1/tests/unit/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/server/einhorn_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/server/monkey_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/server/queue_consumer_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/server/server_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:59.757557 baseplate-2.7.0a1/tests/unit/sidecars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/sidecars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/sidecars/live_data_watcher_loader_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-03-18 15:57:48.000000 baseplate-2.7.0a1/tests/unit/sidecars/live_data_watcher_tests.py
+-rw-r--r--   0        0        0     1476 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/LICENSE
+-rw-r--r--   0        0        0     2784 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/README.md
+-rw-r--r--   0        0        0    26348 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/baseplate/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/baseplate/clients/__init__.py
+-rw-r--r--   0        0        0    16053 2024-04-30 19:26:16.034084 baseplate-2.7.0b1/baseplate/clients/cassandra.py
+-rw-r--r--   0        0        0    11682 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/kombu.py
+-rw-r--r--   0        0        0    16132 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/memcache/__init__.py
+-rw-r--r--   0        0        0     8464 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/memcache/lib.py
+-rw-r--r--   0        0        0    14548 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/redis.py
+-rw-r--r--   0        0        0    22396 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/redis_cluster.py
+-rw-r--r--   0        0        0    17110 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/requests.py
+-rw-r--r--   0        0        0    13557 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/sqlalchemy.py
+-rw-r--r--   0        0        0    15350 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/clients/thrift.py
+-rw-r--r--   0        0        0      162 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/__init__.py
+-rw-r--r--   0        0        0    16283 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/pyramid/__init__.py
+-rw-r--r--   0        0        0     5341 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/pyramid/csrf.py
+-rw-r--r--   0        0        0        0 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/__init__.py
+-rw-r--r--   0        0        0    24917 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/kafka.py
+-rw-r--r--   0        0        0    18799 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/kombu.py
+-rw-r--r--   0        0        0    10209 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/thrift/__init__.py
+-rw-r--r--   0        0        0     2627 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/frameworks/thrift/command.py
+-rw-r--r--   0        0        0     1827 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/__init__.py
+-rw-r--r--   0        0        0     1730 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/_requests.py
+-rw-r--r--   0        0        0    17148 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/config.py
+-rw-r--r--   0        0        0     5390 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/crypto.py
+-rw-r--r--   0        0        0     1016 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/datetime.py
+-rw-r--r--   0        0        0      447 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/edgecontext.py
+-rw-r--r--   0        0        0      490 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/errors.py
+-rw-r--r--   0        0        0     3964 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/events.py
+-rw-r--r--   0        0        0     7004 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/file_watcher.py
+-rw-r--r--   0        0        0      120 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/live_data/__init__.py
+-rw-r--r--   0        0        0     3277 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/live_data/writer.py
+-rw-r--r--   0        0        0     3724 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/live_data/zookeeper.py
+-rw-r--r--   0        0        0      697 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/log_formatter.py
+-rw-r--r--   0        0        0     5653 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/message_queue.py
+-rw-r--r--   0        0        0    19944 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/metrics.py
+-rw-r--r--   0        0        0     1621 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/prometheus_metrics.py
+-rw-r--r--   0        0        0     3250 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/random.py
+-rw-r--r--   0        0        0      290 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/__init__.py
+-rw-r--r--   0        0        0      868 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/__init__.py
+-rw-r--r--   0        0        0     2660 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/memcache.py
+-rw-r--r--   0        0        0     2560 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/redis.py
+-rw-r--r--   0        0        0     2765 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/ratelimit/ratelimit.py
+-rw-r--r--   0        0        0     4217 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/retry.py
+-rw-r--r--   0        0        0    17956 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/secrets.py
+-rw-r--r--   0        0        0     3904 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/service_discovery.py
+-rw-r--r--   0        0        0    10377 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lib/thrift_pool.py
+-rw-r--r--   0        0        0      250 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lint/__init__.py
+-rw-r--r--   0        0        0     3481 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lint/db_query_string_format_plugin.py
+-rw-r--r--   0        0        0     2675 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/lint/example_plugin.py
+-rw-r--r--   0        0        0        0 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/__init__.py
+-rw-r--r--   0        0        0      578 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/logging.py
+-rw-r--r--   0        0        0     5918 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/metrics.py
+-rw-r--r--   0        0        0     7971 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/metrics_tagged.py
+-rw-r--r--   0        0        0     5687 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/sentry.py
+-rw-r--r--   0        0        0     2703 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/timeout.py
+-rw-r--r--   0        0        0    22594 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/observers/tracing.py
+-rw-r--r--   0        0        0       71 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/py.typed
+-rw-r--r--   0        0        0    18997 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/__main__.py
+-rw-r--r--   0        0        0     2166 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/einhorn.py
+-rw-r--r--   0        0        0     2704 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/healthcheck.py
+-rw-r--r--   0        0        0      581 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/monkey.py
+-rw-r--r--   0        0        0      971 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/net.py
+-rw-r--r--   0        0        0     3358 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/prometheus.py
+-rw-r--r--   0        0        0    12793 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/queue_consumer.py
+-rw-r--r--   0        0        0     1944 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/reloader.py
+-rw-r--r--   0        0        0    10523 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/runtime_monitor.py
+-rw-r--r--   0        0        0     2730 2024-04-30 19:26:16.038084 baseplate-2.7.0b1/baseplate/server/thrift.py
+-rw-r--r--   0        0        0     1733 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/server/wsgi.py
+-rw-r--r--   0        0        0     1924 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/__init__.py
+-rw-r--r--   0        0        0     8097 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/event_publisher.py
+-rw-r--r--   0        0        0    10475 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/live_data_watcher.py
+-rw-r--r--   0        0        0    15929 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/secrets_fetcher.py
+-rw-r--r--   0        0        0     6678 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/sidecars/trace_publisher.py
+-rw-r--r--   0        0        0        0 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/testing/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/testing/lib/__init__.py
+-rw-r--r--   0        0        0     1409 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/testing/lib/file_watcher.py
+-rw-r--r--   0        0        0     1250 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/testing/lib/secrets.py
+-rw-r--r--   0        0        0     8857 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/BaseplateService.py
+-rw-r--r--   0        0        0     9586 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/BaseplateServiceV2.py
+-rw-r--r--   0        0        0       76 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/__init__.py
+-rw-r--r--   0        0        0     8232 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/baseplate.thrift
+-rw-r--r--   0        0        0      472 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/constants.py
+-rw-r--r--   0        0        0    13730 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/baseplate/thrift/ttypes.py
+-rwxr-xr-x   0        0        0      138 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-healthcheck
+-rwxr-xr-x   0        0        0      453 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-script
+-rwxr-xr-x   0        0        0      461 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-serve
+-rwxr-xr-x   0        0        0      451 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-shell
+-rwxr-xr-x   0        0        0      554 2024-04-30 19:26:16.042084 baseplate-2.7.0b1/bin/baseplate-tshell
+-rw-r--r--   0        0        0     3323 2024-04-30 19:26:16.046085 baseplate-2.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5270 1970-01-01 00:00:00.000000 baseplate-2.7.0b1/PKG-INFO
```

### Comparing `baseplate-2.7.0a1/LICENSE` & `baseplate-2.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/PKG-INFO` & `baseplate-2.7.0b1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,26 @@
 Metadata-Version: 2.1
 Name: baseplate
-Version: 2.7.0a1
+Version: 2.7.0b1
 Summary: reddit's python service framework
 Home-page: https://github.com/reddit/baseplate.py
-Author: reddit
 License: BSD
-Project-URL: Documentation, https://baseplate.readthedocs.io/en/stable/
-Project-URL: Source, https://github.com/reddit/baseplate.py
-Description: # baseplate.py
-        
-        * [Documentation](https://baseplate.readthedocs.io/en/stable/)
-        * [Contribution Guidelines](https://github.com/reddit/baseplate.py/blob/develop/CONTRIBUTING.md)
-        
-        It's much easier to manage a bunch of services when they all have the same
-        shape: the way they're developed, the way they interact with the infrastructure
-        they run on, and the way they interact with each other. Baseplate is reddit's
-        specification for the common shape of our services. This library, Baseplate.py,
-        is the Python implementation of that specification.
-        
-        Baseplate.py glues together tooling for interacting with the reddit backend
-        ecosystem and spackles over things that are missing. It integrates with Apache
-        Thrift, Pyramid, and client libraries for many systems to transparently make
-        your applications observable.
-        
-        Baseplate applications transparently get:
-        
-        * Timing and request rate metrics using statsd
-        * Distributed tracing with Zipkin
-        * Error reporting and aggregation with Sentry
-        
-        And can take advantage of:
-        
-        * Integration with commonly used clients like: Thrift, SQLAlchemy,
-          cassandra-driver, pymemcache, redis-py, and Kombu
-        * Secrets securely pulled from Vault
-        
-        And many other things!
-        
-        # pre-commit
-        
-        * [Documentation](https://pre-commit.com/)
-        
-        This repo comes with pre-commit hooks that let you (on a voluntary basis)
-        enable pre-commit and/or pre-push hooks.
-        
-        Configuration can be found at the root of the directory in
-        `.pre-commit-config.yaml`. On its own, the configuration file doesn't do
-        anything. You either need to [run the hooks manually](https://pre-commit.com/#pre-commit-run)
-        or [install them](https://pre-commit.com/#pre-commit-install) so that they run
-        automatically on every commit or push.
-        
-        Currently, we run the `make fmt` target on commit and `make lint` / `pytest`
-        actions on push.
-        
-        Specific hooks can be [temporarily disabled](https://pre-commit.com/#temporarily-disabling-hooks).
-        
-        You can install hooks only for a specific step (i.e. [pre-push](https://pre-commit.com/#pre-commit-during-push)).
-        
-        ## Testing in Snoodev
-        
-        You can upgrade any service to use in development Baseplate code in Snoodev by
-        editing the requirements file for the service you would like to use for testing.
-        Update the the Baseplate requirement to pull from Github instead, like this:
-        
-        ```
-        diff --git a/requirements.txt b/requirements.txt
-        index aef8ad8..d32a078 100644
-        --- a/requirements.txt
-        +++ b/requirements.txt
-        -baseplate==2.5.7
-        +git+https://github.com/reddit/baseplate.py@<ref>#egg=baseplate
-        ```
-        
-        In this case the ref can be either a commit hash or a branch name. After making
-        this update you can check if the service works in Snoodev.
-        
-        > **Warning**
-        > Never deploy this change to production. Production should always use a Baseplate
-        > semantic version that has been tagged, and released.
-        
-Platform: UNKNOWN
+Author: reddit
+Requires-Python: >=3.8.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
 Provides-Extra: amqp
 Provides-Extra: cassandra
 Provides-Extra: cqlmapper
 Provides-Extra: kafka
 Provides-Extra: memcache
 Provides-Extra: prometheus
 Provides-Extra: pyramid
@@ -104,8 +28,104 @@
 Provides-Extra: redis-py-cluster
 Provides-Extra: refcycle
 Provides-Extra: requests
 Provides-Extra: s3fetcher
 Provides-Extra: sentry
 Provides-Extra: sql
 Provides-Extra: zookeeper
-Provides-Extra: all
+Requires-Dist: advocate (>=1.0.0,<2.0) ; extra == "requests"
+Requires-Dist: boto3 (>=1.28.27)
+Requires-Dist: cassandra-driver (>=3.29.0,<4.0) ; extra == "cassandra"
+Requires-Dist: confluent-kafka (>=2.3.0) ; extra == "kafka"
+Requires-Dist: gevent (>=23.9.1)
+Requires-Dist: kazoo (>=2.5.0,<3.0) ; extra == "zookeeper"
+Requires-Dist: kombu (>=5.3.3) ; extra == "amqp"
+Requires-Dist: objgraph (>=3.6.0) ; extra == "refcycle"
+Requires-Dist: posix-ipc (>=1.0.0,<2.0)
+Requires-Dist: prometheus-client (>=0.12.0)
+Requires-Dist: pymemcache (>=1.3.0,<1.4.4) ; extra == "memcache"
+Requires-Dist: pyramid (>=1.10.8,<2.0) ; extra == "pyramid"
+Requires-Dist: python-json-logger (>=2.0.5,<3.0)
+Requires-Dist: reddit-cqlmapper (>=0.3.0,<1.0) ; extra == "cqlmapper"
+Requires-Dist: redis (>=2.10.0,<4.0.0) ; extra == "redis"
+Requires-Dist: redis-py-cluster (>=2.1.2,<3.0.0) ; extra == "redis-py-cluster"
+Requires-Dist: requests (>=2.21.0,<3.0)
+Requires-Dist: sentry-sdk (>=1.35.0,<2.0) ; extra == "sentry"
+Requires-Dist: sqlalchemy (>=1.4.49,<2) ; extra == "sql"
+Requires-Dist: thrift-unofficial (>=0.19.0,<1.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
+Project-URL: Documentation, https://baseplate.readthedocs.io/en/stable/
+Project-URL: Repository, https://github.com/reddit/baseplate.py
+Description-Content-Type: text/markdown
+
+# baseplate.py
+
+* [Documentation](https://baseplate.readthedocs.io/en/stable/)
+* [Contribution Guidelines](https://github.com/reddit/baseplate.py/blob/develop/CONTRIBUTING.md)
+
+It's much easier to manage a bunch of services when they all have the same
+shape: the way they're developed, the way they interact with the infrastructure
+they run on, and the way they interact with each other. Baseplate is reddit's
+specification for the common shape of our services. This library, Baseplate.py,
+is the Python implementation of that specification.
+
+Baseplate.py glues together tooling for interacting with the reddit backend
+ecosystem and spackles over things that are missing. It integrates with Apache
+Thrift, Pyramid, and client libraries for many systems to transparently make
+your applications observable.
+
+Baseplate applications transparently get:
+
+* Timing and request rate metrics using statsd
+* Distributed tracing with Zipkin
+* Error reporting and aggregation with Sentry
+
+And can take advantage of:
+
+* Integration with commonly used clients like: Thrift, SQLAlchemy,
+  cassandra-driver, pymemcache, redis-py, and Kombu
+* Secrets securely pulled from Vault
+
+And many other things!
+
+# pre-commit
+
+* [Documentation](https://pre-commit.com/)
+
+This repo comes with pre-commit hooks that let you (on a voluntary basis)
+enable pre-commit and/or pre-push hooks.
+
+Configuration can be found at the root of the directory in
+`.pre-commit-config.yaml`. On its own, the configuration file doesn't do
+anything. You either need to [run the hooks manually](https://pre-commit.com/#pre-commit-run)
+or [install them](https://pre-commit.com/#pre-commit-install) so that they run
+automatically on every commit or push.
+
+Currently, we run the `make fmt` target on commit and `make lint` / `pytest`
+actions on push.
+
+Specific hooks can be [temporarily disabled](https://pre-commit.com/#temporarily-disabling-hooks).
+
+You can install hooks only for a specific step (i.e. [pre-push](https://pre-commit.com/#pre-commit-during-push)).
+
+## Testing in Snoodev
+
+You can upgrade any service to use in development Baseplate code in Snoodev by
+editing the requirements file for the service you would like to use for testing.
+Update the the Baseplate requirement to pull from Github instead, like this:
+
+```
+diff --git a/requirements.txt b/requirements.txt
+index aef8ad8..d32a078 100644
+--- a/requirements.txt
++++ b/requirements.txt
+-baseplate==2.5.7
++git+https://github.com/reddit/baseplate.py@<ref>#egg=baseplate
+```
+
+In this case the ref can be either a commit hash or a branch name. After making
+this update you can check if the service works in Snoodev.
+
+> **Warning**
+> Never deploy this change to production. Production should always use a Baseplate
+> semantic version that has been tagged, and released.
+
```

### Comparing `baseplate-2.7.0a1/README.md` & `baseplate-2.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/__init__.py` & `baseplate-2.7.0b1/baseplate/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/clients/__init__.py` & `baseplate-2.7.0b1/baseplate/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/clients/cassandra.py` & `baseplate-2.7.0b1/baseplate/clients/cassandra.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/clients/kombu.py` & `baseplate-2.7.0b1/baseplate/clients/kombu.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/clients/memcache/__init__.py` & `baseplate-2.7.0b1/baseplate/clients/memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/clients/memcache/lib.py` & `baseplate-2.7.0b1/baseplate/clients/memcache/lib.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/clients/redis.py` & `baseplate-2.7.0b1/baseplate/clients/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         super().__init__(connection_pool=connection_pool)
 
     def execute_command(self, *args: Any, **kwargs: Any) -> Any:
         command = args[0]
         trace_name = f"{self.context_name}.{command}"
 
         labels = {
-            f"{PROM_LABELS_PREFIX}_command": command,
+            f"{PROM_LABELS_PREFIX}_command": command.lower(),
             f"{PROM_LABELS_PREFIX}_client_name": self.redis_client_name,
             f"{PROM_LABELS_PREFIX}_database": self.connection_pool.connection_kwargs.get("db", ""),
             f"{PROM_LABELS_PREFIX}_type": "standalone",
         }
         with self.server_span.make_child(trace_name), ACTIVE_REQUESTS.labels(
             **labels
         ).track_inprogress():
```

### Comparing `baseplate-2.7.0a1/baseplate/clients/redis_cluster.py` & `baseplate-2.7.0b1/baseplate/clients/redis_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,16 +218,21 @@
     # pylint: disable=arguments-differ
     def get_node_by_slot(self, slot: int, read_command: bool = False) -> Dict[str, Any]:
         """Get a node from the slot.
 
         If the command is a read command we'll try to return a random node.
         If there are no replicas or this isn't a read command we'll return the primary.
         """
-        if read_command:
-            return random.choice(self.nodes.slots[slot])
+        try:
+            if read_command:
+                return random.choice(self.nodes.slots[slot])
+        except KeyError:
+            raise rediscluster.exceptions.SlotNotCoveredError(
+                f"Slot {slot} not covered by the cluster"
+            )
 
         # This isn't a read command, so return the primary (first node)
         return self.nodes.slots[slot][0]
 
 
 def cluster_pool_from_config(
     app_config: config.RawConfig, prefix: str = "rediscluster.", **kwargs: Any
@@ -440,15 +445,15 @@
         command = args[0]
         trace_name = f"{self.context_name}.{command}"
 
         with self.server_span.make_child(trace_name):
             start_time = perf_counter()
             success = "true"
             labels = {
-                f"{PROM_LABELS_PREFIX}_command": command,
+                f"{PROM_LABELS_PREFIX}_command": command.lower(),
                 f"{PROM_LABELS_PREFIX}_client_name": self.redis_client_name,
                 f"{PROM_LABELS_PREFIX}_database": self.connection_pool.connection_kwargs.get(
                     "db", ""
                 ),
                 f"{PROM_LABELS_PREFIX}_type": "cluster",
             }
```

### Comparing `baseplate-2.7.0a1/baseplate/clients/requests.py` & `baseplate-2.7.0b1/baseplate/clients/requests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/clients/sqlalchemy.py` & `baseplate-2.7.0b1/baseplate/clients/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/clients/thrift.py` & `baseplate-2.7.0b1/baseplate/clients/thrift.py`

 * *Files 7% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                 fn_name: _build_thrift_proxy_method(fn_name)
                 for fn_name in _enumerate_service_methods(client_cls)
                 if not (fn_name.startswith("__") and fn_name.endswith("__"))
             },
         )
 
     def report_runtime_metrics(self, batch: metrics.Client) -> None:
-        pool_name = self.client_cls.__name__
+        pool_name = self.client_cls.__qualname__
         self.max_connections_gauge.labels(pool_name).set(self.pool.size)
         self.active_connections_gauge.labels(pool_name).set(self.pool.checkedout)
         batch.gauge("pool.size").replace(self.pool.size)
         batch.gauge("pool.in_use").replace(self.pool.checkedout)
         # it's hard to report "open_and_available" currently because we can't
         # distinguish easily between available connection slots that aren't
         # instantiated and ones that have actual open connections.
@@ -296,15 +296,15 @@
                         exception_type = ""
                         baseplate_status = ""
                         baseplate_status_code = ""
                         exc_info = sys.exc_info()
                         if exc_info[0] is not None:
                             thrift_success = "false"
                             exception_type = exc_info[0].__name__
-                            current_exc = exc_info[1]
+                            current_exc: Any = exc_info[1]
                             try:
                                 # We want the following code to execute whenever the
                                 # service raises an instance of Baseplate's `Error` class.
                                 # Unfortunately, we cannot just rely on `isinstance` to do
                                 # what we want here because some services compile
                                 # Baseplate's thrift file on their own and import `Error`
                                 # from that. When this is done, `isinstance` will always
@@ -313,16 +313,25 @@
                                 # `current_exc` and just catch the `AttributeError` if the
                                 # `code` attribute is not present.
                                 # Note: if the error code was not originally defined in baseplate, or the
                                 # name associated with the error was overriden, this cannot reflect that
                                 # we will emit the status code in both cases
                                 # but the status will be blank in the first case, and the baseplate name
                                 # in the second
-                                baseplate_status_code = current_exc.code  # type: ignore
-                                baseplate_status = ErrorCode()._VALUES_TO_NAMES.get(current_exc.code, "")  # type: ignore
+                                #
+                                # Since this exception could be of any type, we may receive exceptions
+                                # that have a `code` property that is actually not from Baseplate's
+                                # `Error` class. In order to reduce (but not eliminate) the possibility
+                                # of metric explosion, we validate it against the expected type for a
+                                # proper Error code.
+                                if isinstance(current_exc.code, int):
+                                    baseplate_status_code = str(current_exc.code)
+                                    baseplate_status = ErrorCode()._VALUES_TO_NAMES.get(
+                                        current_exc.code, ""
+                                    )
                             except AttributeError:
                                 pass
 
                         REQUEST_LATENCY.labels(
                             thrift_method=name,
                             thrift_client_name=self.namespace,
                             thrift_success=thrift_success,
```

### Comparing `baseplate-2.7.0a1/baseplate/frameworks/pyramid/__init__.py` & `baseplate-2.7.0b1/baseplate/frameworks/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/frameworks/pyramid/csrf.py` & `baseplate-2.7.0b1/baseplate/frameworks/pyramid/csrf.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/frameworks/queue_consumer/kafka.py` & `baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import confluent_kafka
 
 from gevent.server import StreamServer
 from prometheus_client import Counter
 from prometheus_client import Gauge
 from prometheus_client import Histogram
+from typing_extensions import Self
 
 from baseplate import Baseplate
 from baseplate import RequestContext
 from baseplate.lib.prometheus_metrics import default_latency_buckets
 from baseplate.server.queue_consumer import HealthcheckCallback
 from baseplate.server.queue_consumer import make_simple_healthchecker
 from baseplate.server.queue_consumer import MessageHandler
@@ -264,15 +265,15 @@
         topics: Sequence[str],
         handler_fn: Handler,
         kafka_consume_batch_size: int = 1,
         message_unpack_fn: KafkaMessageDeserializer = json.loads,
         health_check_fn: Optional[HealthcheckCallback] = None,
         kafka_config: Optional[Dict[str, Any]] = None,
         prometheus_client_name: str = "",
-    ) -> "_BaseKafkaQueueConsumerFactory":
+    ) -> Self:
         """Return a new `_BaseKafkaQueueConsumerFactory`.
 
         This method will create the :py:class:`~confluent_kafka.Consumer` for you and is
         appropriate to use in most cases where you just need a basic consumer
         with sensible defaults.
 
         This method will also enforce naming standards for the Kafka consumer group
@@ -327,14 +328,18 @@
         consumer_config = {
             "bootstrap.servers": bootstrap_servers,
             "group.id": group_id,
             # reset the offset to the latest offset when no stored offset exists.
             # this means that when a new consumer group is created it will only
             # process new messages.
             "auto.offset.reset": "latest",
+            # Use the cooperative sticky assignor for consumer group rebalances.
+            # This *dramatically* reduces the time taken to rebalance the consumer group
+            # when the underlying topic metadata changes (leadership changes etc).
+            "partition.assignment.strategy": "cooperative-sticky",
         }
         consumer_config.update(cls._consumer_config())
         if kafka_config:
             consumer_config.update(kafka_config)
         consumer = confluent_kafka.Consumer(consumer_config)
 
         try:
```

### Comparing `baseplate-2.7.0a1/baseplate/frameworks/queue_consumer/kombu.py` & `baseplate-2.7.0b1/baseplate/frameworks/queue_consumer/kombu.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/frameworks/thrift/__init__.py` & `baseplate-2.7.0b1/baseplate/frameworks/thrift/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/frameworks/thrift/command.py` & `baseplate-2.7.0b1/baseplate/frameworks/thrift/command.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/__init__.py` & `baseplate-2.7.0b1/baseplate/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/_requests.py` & `baseplate-2.7.0b1/baseplate/lib/_requests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/config.py` & `baseplate-2.7.0b1/baseplate/lib/config.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/crypto.py` & `baseplate-2.7.0b1/baseplate/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/datetime.py` & `baseplate-2.7.0b1/baseplate/lib/datetime.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/events.py` & `baseplate-2.7.0b1/baseplate/lib/events.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/file_watcher.py` & `baseplate-2.7.0b1/baseplate/lib/file_watcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/live_data/writer.py` & `baseplate-2.7.0b1/baseplate/lib/live_data/writer.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/live_data/zookeeper.py` & `baseplate-2.7.0b1/baseplate/lib/live_data/zookeeper.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/log_formatter.py` & `baseplate-2.7.0b1/baseplate/lib/log_formatter.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/message_queue.py` & `baseplate-2.7.0b1/baseplate/lib/message_queue.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/metrics.py` & `baseplate-2.7.0b1/baseplate/lib/metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/prometheus_metrics.py` & `baseplate-2.7.0b1/baseplate/lib/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/random.py` & `baseplate-2.7.0b1/baseplate/lib/random.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/ratelimit/backends/__init__.py` & `baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/ratelimit/backends/memcache.py` & `baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/memcache.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/ratelimit/backends/redis.py` & `baseplate-2.7.0b1/baseplate/lib/ratelimit/backends/redis.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/ratelimit/ratelimit.py` & `baseplate-2.7.0b1/baseplate/lib/ratelimit/ratelimit.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/retry.py` & `baseplate-2.7.0b1/baseplate/lib/retry.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/secrets.py` & `baseplate-2.7.0b1/baseplate/lib/secrets.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/service_discovery.py` & `baseplate-2.7.0b1/baseplate/lib/service_discovery.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lib/thrift_pool.py` & `baseplate-2.7.0b1/baseplate/lib/thrift_pool.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lint/db_query_string_format_plugin.py` & `baseplate-2.7.0b1/baseplate/lint/db_query_string_format_plugin.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/lint/example_plugin.py` & `baseplate-2.7.0b1/baseplate/lint/example_plugin.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/observers/logging.py` & `baseplate-2.7.0b1/baseplate/observers/logging.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/observers/metrics.py` & `baseplate-2.7.0b1/baseplate/observers/metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/observers/metrics_tagged.py` & `baseplate-2.7.0b1/baseplate/observers/metrics_tagged.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/observers/sentry.py` & `baseplate-2.7.0b1/baseplate/observers/sentry.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/observers/timeout.py` & `baseplate-2.7.0b1/baseplate/observers/timeout.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/observers/tracing.py` & `baseplate-2.7.0b1/baseplate/observers/tracing.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/__init__.py` & `baseplate-2.7.0b1/baseplate/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,17 +294,22 @@
     server.start()
     try:
         shutdown_event.wait()
 
         SERVER_STATE.state = ServerLifecycle.SHUTTING_DOWN
 
         cfg = parse_config(config.server, {"drain_time": OptionalConfig(Timespan)})
+        # Default drain time across all baseplate language implementations
+        # which allows enough time for systems such as k8s to remove the
+        # server from the endpoints list.
+        drain_time_seconds = 5
         if cfg.drain_time:
-            logger.debug("Draining inbound requests...")
-            time.sleep(cfg.drain_time.total_seconds())
+            drain_time_seconds = cfg.drain_time.total_seconds()
+        logger.debug("Draining inbound requests...")
+        time.sleep(drain_time_seconds)
     finally:
         logger.debug("Gracefully shutting down...")
         server.stop()
         logger.info("Exiting")
 
 
 def load_and_run_script() -> None:
@@ -434,28 +439,33 @@
         try:
             # IPython 5.x+
             from traitlets.config.loader import Config
         except ImportError:
             # IPython 4 and below
             from IPython import Config
 
+        # test for UTC availability from the datetime package
+        import datetime as dt
+
+        datetime_exec = "now(datetime.UTC)" if getattr(dt, "UTC", False) else "utcnow()"
+
         ipython_config = Config()
         ipython_config.InteractiveShellApp.exec_lines = [
             # monkeypatch IPython's log-write() to enable formatted input logging, copying original code:
             # https://github.com/ipython/ipython/blob/a54bf00feb5182fa821bd5457897b3b30a313436/IPython/core/logger.py#L187-L201
             f"""
             ip = get_ipython()
             from functools import partial
             def log_write(self, data, kind="input", message_id="IEXC"):
                 import datetime, os
                 if self.log_active and data:
                     write = self.logfile.write
                     if kind=='input':
                         # Generate an RFC 5424 compliant syslog format
-                        write(f'<13>1 {{datetime.datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S.%fZ")}} {{os.uname().nodename}} baseplate-shell {{os.getpid()}} {{message_id}} - {{data}}')
+                        write(f'<13>1 {{datetime.datetime.{datetime_exec}.strftime("%Y-%m-%dT%H:%M:%S.%fZ")}} {{os.uname().nodename}} baseplate-shell {{os.getpid()}} {{message_id}} - {{data}}')
                     elif kind=='output' and self.log_output:
                         odata = u'\\n'.join([u'#[Out]# %s' % s
                                         for s in data.splitlines()])
                         write(u'%s\\n' % odata)
                     self.logfile.flush()
             ip.logger.logstop = None
             ip.logger.log_write = partial(log_write, ip.logger)
```

### Comparing `baseplate-2.7.0a1/baseplate/server/einhorn.py` & `baseplate-2.7.0b1/baseplate/server/einhorn.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/healthcheck.py` & `baseplate-2.7.0b1/baseplate/server/healthcheck.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/monkey.py` & `baseplate-2.7.0b1/baseplate/server/monkey.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/net.py` & `baseplate-2.7.0b1/baseplate/server/net.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/prometheus.py` & `baseplate-2.7.0b1/baseplate/server/prometheus.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/queue_consumer.py` & `baseplate-2.7.0b1/baseplate/server/queue_consumer.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/reloader.py` & `baseplate-2.7.0b1/baseplate/server/reloader.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/runtime_monitor.py` & `baseplate-2.7.0b1/baseplate/server/runtime_monitor.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/thrift.py` & `baseplate-2.7.0b1/baseplate/server/thrift.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/server/wsgi.py` & `baseplate-2.7.0b1/baseplate/server/wsgi.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/sidecars/__init__.py` & `baseplate-2.7.0b1/baseplate/sidecars/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/sidecars/event_publisher.py` & `baseplate-2.7.0b1/baseplate/sidecars/event_publisher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/sidecars/live_data_watcher.py` & `baseplate-2.7.0b1/baseplate/sidecars/live_data_watcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/sidecars/secrets_fetcher.py` & `baseplate-2.7.0b1/baseplate/sidecars/secrets_fetcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/sidecars/trace_publisher.py` & `baseplate-2.7.0b1/baseplate/sidecars/trace_publisher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/testing/lib/file_watcher.py` & `baseplate-2.7.0b1/baseplate/testing/lib/file_watcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/testing/lib/secrets.py` & `baseplate-2.7.0b1/baseplate/testing/lib/secrets.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/thrift/BaseplateService.py` & `baseplate-2.7.0b1/baseplate/thrift/BaseplateService.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/thrift/BaseplateServiceV2.py` & `baseplate-2.7.0b1/baseplate/thrift/BaseplateServiceV2.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/thrift/baseplate.thrift` & `baseplate-2.7.0b1/baseplate/thrift/baseplate.thrift`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/baseplate/thrift/ttypes.py` & `baseplate-2.7.0b1/baseplate/thrift/ttypes.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.7.0a1/bin/baseplate-tshell` & `baseplate-2.7.0b1/bin/baseplate-tshell`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!python
 
 # this is here and not just a console_script entry point because we want the
 # gevent monkeypatching to happen before any pieces of baseplate are imported
 # at all, as would happen if we were to have this code be in the baseplate
 # package.
 
 from gevent.monkey import patch_all
```

