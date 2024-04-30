# Comparing `tmp/opal-common-0.7.5.tar.gz` & `tmp/opal_common-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-common-0.7.5.tar", last modified: Wed Mar 13 16:42:10 2024, max compression
+gzip compressed data, was "opal_common-0.7.6.tar", last modified: Tue Apr 30 17:18:48 2024, max compression
```

## Comparing `opal-common-0.7.5.tar` & `opal_common-0.7.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.340041 opal-common-0.7.5/
--rw-r--r--   0 roekatz    (501) staff       (20)     9956 2024-03-13 16:42:10.339728 opal-common-0.7.5/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.318410 opal-common-0.7.5/opal_common/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3070 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/async_utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.321382 opal-common-0.7.5/opal_common/authentication/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/authentication/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1477 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/authentication/authz.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3267 2023-05-09 07:59:18.000000 opal-common-0.7.5/opal_common/authentication/casting.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4990 2023-10-04 11:07:26.000000 opal-common-0.7.5/opal_common/authentication/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4669 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/authentication/signer.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.321832 opal-common-0.7.5/opal_common/authentication/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/authentication/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    17336 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/authentication/tests/jwt_signer_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      958 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/authentication/types.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4225 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/authentication/verifier.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.323042 opal-common-0.7.5/opal_common/cli/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/cli/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6657 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/cli/commands.py
--rw-r--r--   0 roekatz    (501) staff       (20)      702 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/cli/docs.py
--rw-r--r--   0 roekatz    (501) staff       (20)      167 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/cli/typer_app.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.324311 opal-common-0.7.5/opal_common/confi/
--rw-r--r--   0 roekatz    (501) staff       (20)       21 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/confi/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2278 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/confi/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    14044 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/confi/confi.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2836 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/confi/types.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7139 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/config.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1492 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/corn_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6045 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/emport.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.325302 opal-common-0.7.5/opal_common/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)       90 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/engine/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      576 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/engine/parsing.py
--rw-r--r--   0 roekatz    (501) staff       (20)      593 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/engine/paths.py
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/engine/py.typed
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.326355 opal-common-0.7.5/opal_common/fetcher/
--rw-r--r--   0 roekatz    (501) staff       (20)      143 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.327601 opal-common-0.7.5/opal_common/fetcher/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/engine/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2653 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/engine/base_fetching_engine.py
--rw-r--r--   0 roekatz    (501) staff       (20)      296 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/engine/core_callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1536 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/engine/fetch_worker.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8602 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/fetcher/engine/fetching_engine.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1191 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/events.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2548 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/fetcher/fetch_provider.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3030 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/fetcher_register.py
--rw-r--r--   0 roekatz    (501) staff       (20)      116 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/logger.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.328299 opal-common-0.7.5/opal_common/fetcher/providers/
--rw-r--r--   0 roekatz    (501) staff       (20)       67 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/providers/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1710 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3570 2024-02-28 15:15:55.000000 opal-common-0.7.5/opal_common/fetcher/providers/http_fetch_provider.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.329333 opal-common-0.7.5/opal_common/fetcher/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/fetcher/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1918 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/fetcher/tests/failure_handler_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4289 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/fetcher/tests/http_fetch_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2141 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/fetcher/tests/rpc_fetch_test.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.332040 opal-common-0.7.5/opal_common/git/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/git/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5461 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/git/branch_tracker.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15724 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/git/bundle_maker.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1887 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/git/bundle_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8684 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/git/commit_viewer.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7948 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/git/diff_viewer.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1580 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/git/env.py
--rw-r--r--   0 roekatz    (501) staff       (20)      299 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/git/exceptions.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8535 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/git/repo_cloner.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4237 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/git/tar_file_to_local_git_extractor.py
--rw-r--r--   0 roekatz    (501) staff       (20)      182 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/http.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1908 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/logger.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.333217 opal-common-0.7.5/opal_common/logging/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/logging/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      412 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/logging/decorators.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1166 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/logging/filter.py
--rw-r--r--   0 roekatz    (501) staff       (20)      616 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/logging/formatter.py
--rw-r--r--   0 roekatz    (501) staff       (20)      700 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/logging/intercept.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1355 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/logging/thirdparty.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3520 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/middleware.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.333762 opal-common-0.7.5/opal_common/monitoring/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/monitoring/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1546 2024-03-13 14:12:20.000000 opal-common-0.7.5/opal_common/monitoring/apm.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1446 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/monitoring/metrics.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4067 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/paths.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.335484 opal-common-0.7.5/opal_common/schemas/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/schemas/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7140 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/schemas/data.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1387 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/schemas/policy.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1767 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/schemas/policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)      508 2023-04-04 11:14:44.000000 opal-common-0.7.5/opal_common/schemas/scopes.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1573 2023-05-23 16:26:33.000000 opal-common-0.7.5/opal_common/schemas/security.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2398 2023-07-17 14:14:01.000000 opal-common-0.7.5/opal_common/schemas/store.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1438 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/schemas/webhook.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.335947 opal-common-0.7.5/opal_common/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      799 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/security/sslcontext.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3294 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/security/tarsafe.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.336752 opal-common-0.7.5/opal_common/sources/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/sources/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11637 2023-10-04 11:07:26.000000 opal-common-0.7.5/opal_common/sources/api_policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/sources/base_policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4238 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/sources/git_policy_source.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.337331 opal-common-0.7.5/opal_common/synchronization/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/synchronization/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1307 2023-10-04 11:07:26.000000 opal-common-0.7.5/opal_common/synchronization/expiring_redis_lock.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2990 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/synchronization/named_lock.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.338131 opal-common-0.7.5/opal_common/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     9622 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/tests/path_utils_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      539 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/tests/test_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1223 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/tests/url_utils_test.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.338925 opal-common-0.7.5/opal_common/topics/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/topics/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2371 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/topics/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7127 2024-03-06 13:35:27.000000 opal-common-0.7.5/opal_common/topics/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1054 2023-05-29 10:10:14.000000 opal-common-0.7.5/opal_common/topics/utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)      988 2022-12-08 13:40:17.000000 opal-common-0.7.5/opal_common/urls.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8371 2023-06-20 17:01:29.000000 opal-common-0.7.5/opal_common/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.339266 opal-common-0.7.5/opal_common.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     9956 2024-03-13 16:42:10.000000 opal-common-0.7.5/opal_common.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     3366 2024-03-13 16:42:10.000000 opal-common-0.7.5/opal_common.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-03-13 16:42:10.000000 opal-common-0.7.5/opal_common.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      505 2024-03-13 16:42:10.000000 opal-common-0.7.5/opal_common.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-03-13 16:42:10.000000 opal-common-0.7.5/opal_common.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-03-13 16:42:10.340092 opal-common-0.7.5/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2601 2022-12-08 13:40:17.000000 opal-common-0.7.5/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.529060 opal_common-0.7.6/
+-rw-r--r--   0 roekatz    (501) staff       (20)    10034 2024-04-30 17:18:48.528689 opal_common-0.7.6/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.515323 opal_common-0.7.6/opal_common/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3574 2024-04-30 13:01:51.000000 opal_common-0.7.6/opal_common/async_utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.517116 opal_common-0.7.6/opal_common/authentication/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1477 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/authz.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3329 2024-04-30 13:01:51.000000 opal_common-0.7.6/opal_common/authentication/casting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4990 2023-10-04 11:07:26.000000 opal_common-0.7.6/opal_common/authentication/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4669 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/signer.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.517557 opal_common-0.7.6/opal_common/authentication/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    17336 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/tests/jwt_signer_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      950 2024-04-30 16:48:47.000000 opal_common-0.7.6/opal_common/authentication/types.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4225 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/authentication/verifier.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.518771 opal_common-0.7.6/opal_common/cli/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/cli/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6657 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/cli/commands.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      702 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/cli/docs.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      167 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/cli/typer_app.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.519354 opal_common-0.7.6/opal_common/confi/
+-rw-r--r--   0 roekatz    (501) staff       (20)       21 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/confi/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2278 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/confi/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    14044 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/confi/confi.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2836 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/confi/types.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7139 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/config.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1492 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/corn_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6045 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/emport.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.519868 opal_common-0.7.6/opal_common/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)       90 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/engine/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      576 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/engine/parsing.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      593 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/engine/paths.py
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/engine/py.typed
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.520471 opal_common-0.7.6/opal_common/fetcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)      143 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.521104 opal_common-0.7.6/opal_common/fetcher/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/engine/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2653 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/engine/base_fetching_engine.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      296 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/engine/core_callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1536 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/engine/fetch_worker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8602 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/fetcher/engine/fetching_engine.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1191 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/events.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2548 2024-03-26 18:21:06.000000 opal_common-0.7.6/opal_common/fetcher/fetch_provider.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3030 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/fetcher_register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      116 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/logger.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.521522 opal_common-0.7.6/opal_common/fetcher/providers/
+-rw-r--r--   0 roekatz    (501) staff       (20)       67 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/providers/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1710 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3570 2024-02-28 15:15:55.000000 opal_common-0.7.6/opal_common/fetcher/providers/http_fetch_provider.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.522064 opal_common-0.7.6/opal_common/fetcher/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/fetcher/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1918 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/fetcher/tests/failure_handler_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4289 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/fetcher/tests/http_fetch_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2141 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/fetcher/tests/rpc_fetch_test.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.523494 opal_common-0.7.6/opal_common/git/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/git/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5461 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/branch_tracker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    15724 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/git/bundle_maker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1887 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/bundle_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8684 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/commit_viewer.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7948 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/git/diff_viewer.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1580 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/env.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      299 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/git/exceptions.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8535 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/git/repo_cloner.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4237 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/git/tar_file_to_local_git_extractor.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      182 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/http.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1908 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/logger.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.524285 opal_common-0.7.6/opal_common/logging/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      412 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/decorators.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1166 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/filter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      616 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/logging/formatter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      700 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/intercept.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1355 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/logging/thirdparty.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3520 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/middleware.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.524642 opal_common-0.7.6/opal_common/monitoring/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/monitoring/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1546 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/monitoring/apm.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1446 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/monitoring/metrics.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4067 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/paths.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.525734 opal_common-0.7.6/opal_common/schemas/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/schemas/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7140 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/schemas/data.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1387 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/schemas/policy.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1767 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/schemas/policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      508 2023-04-04 11:14:44.000000 opal_common-0.7.6/opal_common/schemas/scopes.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1573 2023-05-23 16:26:33.000000 opal_common-0.7.6/opal_common/schemas/security.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2398 2023-07-17 14:14:01.000000 opal_common-0.7.6/opal_common/schemas/store.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1438 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/schemas/webhook.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.526099 opal_common-0.7.6/opal_common/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      799 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/security/sslcontext.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3294 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/security/tarsafe.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.526622 opal_common-0.7.6/opal_common/sources/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/sources/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11747 2024-04-30 12:59:10.000000 opal_common-0.7.6/opal_common/sources/api_policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/sources/base_policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4238 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/sources/git_policy_source.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.527045 opal_common-0.7.6/opal_common/synchronization/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/synchronization/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1307 2023-10-04 11:07:26.000000 opal_common-0.7.6/opal_common/synchronization/expiring_redis_lock.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2990 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/synchronization/named_lock.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.527590 opal_common-0.7.6/opal_common/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     9622 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/tests/path_utils_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      539 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/tests/test_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1223 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/tests/url_utils_test.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.528117 opal_common-0.7.6/opal_common/topics/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/topics/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2371 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/topics/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7127 2024-03-19 14:53:02.000000 opal_common-0.7.6/opal_common/topics/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1054 2023-05-29 10:10:14.000000 opal_common-0.7.6/opal_common/topics/utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      988 2022-12-08 13:40:17.000000 opal_common-0.7.6/opal_common/urls.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8578 2024-04-30 12:59:10.000000 opal_common-0.7.6/opal_common/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:48.528311 opal_common-0.7.6/opal_common.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)    10034 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     3366 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      515 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-04-30 17:18:48.000000 opal_common-0.7.6/opal_common.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-04-30 17:18:48.529104 opal_common-0.7.6/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2653 2024-04-30 13:01:51.000000 opal_common-0.7.6/setup.py
```

### Comparing `opal-common-0.7.5/PKG-INFO` & `opal_common-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.7.5
+Version: 0.7.6
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp<4,>=3.9.2
 Requires-Dist: click<9,>=8.1.3
-Requires-Dist: cryptography<42,>=41.0.2
+Requires-Dist: cryptography<43,>=42.0.4
 Requires-Dist: gitpython<4,>=3.1.32
 Requires-Dist: loguru<1,>=0.6.0
 Requires-Dist: pyjwt[crypto]<3,>=2.4.0
 Requires-Dist: python-decouple<4,>=3.6
 Requires-Dist: tenacity<9,>=8.0.1
 Requires-Dist: datadog<1,>=0.44.0
-Requires-Dist: ddtrace<3,>=2
-Requires-Dist: charset-normalizer<3,>=2.0.12
+Requires-Dist: ddtrace<3,>=2.8.1
+Requires-Dist: certifi>=2023.7.22
+Requires-Dist: requests>=2.31.0
 Requires-Dist: idna<4,>=3.3
 Requires-Dist: typer<1,>=0.4.1
 Requires-Dist: fastapi<1,>=0.109.1
 Requires-Dist: fastapi_websocket_pubsub==0.3.7
 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0
+Requires-Dist: gunicorn<23,>=22.0.0
 Requires-Dist: pydantic[email]<2,>=1.9.1
 Requires-Dist: typing-extensions; python_version < "3.8"
 Requires-Dist: uvicorn[standard]<1,>=0.17.6
 Requires-Dist: fastapi-utils<1,>=0.2.1
 Requires-Dist: setuptools>=65.5.1
 
 <p  align="center">
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: opal-common Version: 0.7.5 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.6 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet ::
-WWW/HTTP :: WSGI Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp<4,>=3.9.2 Requires-Dist: click<9,>=8.1.3 Requires-Dist:
-cryptography<42,>=41.0.2 Requires-Dist: gitpython<4,>=3.1.32 Requires-Dist:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/
+HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
+Requires-Python: >=3.9 Description-Content-Type: text/markdown Requires-Dist:
+aiohttp<4,>=3.9.2 Requires-Dist: click<9,>=8.1.3 Requires-Dist:
+cryptography<43,>=42.0.4 Requires-Dist: gitpython<4,>=3.1.32 Requires-Dist:
 loguru<1,>=0.6.0 Requires-Dist: pyjwt[crypto]<3,>=2.4.0 Requires-Dist: python-
 decouple<4,>=3.6 Requires-Dist: tenacity<9,>=8.0.1 Requires-Dist:
-datadog<1,>=0.44.0 Requires-Dist: ddtrace<3,>=2 Requires-Dist: charset-
-normalizer<3,>=2.0.12 Requires-Dist: idna<4,>=3.3 Requires-Dist:
-typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
-fastapi_websocket_pubsub==0.3.7 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0 Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist: uvicorn
-[standard]<1,>=0.17.6 Requires-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist:
-setuptools>=65.5.1
+datadog<1,>=0.44.0 Requires-Dist: ddtrace<3,>=2.8.1 Requires-Dist:
+certifi>=2023.7.22 Requires-Dist: requests>=2.31.0 Requires-Dist: idna<4,>=3.3
+Requires-Dist: typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-
+Dist: fastapi_websocket_pubsub==0.3.7 Requires-Dist:
+fastapi_websocket_rpc<1,>=0.1.21 Requires-Dist: gunicorn<23,>=22.0.0 Requires-
+Dist: pydantic[email]<2,>=1.9.1 Requires-Dist: typing-extensions;
+python_version < "3.8" Requires-Dist: uvicorn[standard]<1,>=0.17.6 Requires-
+Dist: fastapi-utils<1,>=0.2.1 Requires-Dist: setuptools>=65.5.1
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
 _p_e_r_m_i_t___i_o_?_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_p_e_r_m_i_t___i_o_&_s_t_y_l_e_=_s_o_c_i_a_l_]## What is OPAL? OPAL is an
 administration layer for Policy Engines such as _O_p_e_n_ _P_o_l_i_c_y_ _A_g_e_n_t_ _(_O_P_A_), and
```

### Comparing `opal-common-0.7.5/opal_common/authentication/authz.py` & `opal_common-0.7.6/opal_common/authentication/authz.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/authentication/casting.py` & `opal_common-0.7.6/opal_common/authentication/casting.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     if passphrase is None:
         password = None
     else:
         password = passphrase.encode("utf-8")
 
     key_path = os.path.expanduser(value)
     if os.path.isfile(key_path):
-        raw_key = open(key_path, "rb").read()
+        with open(key_path, "rb") as file:
+            raw_key = file.read()
     else:
         raw_key = maybe_decode_multiline_key(value)
 
     if key_format == EncryptionKeyFormat.pem:
         return serialization.load_pem_private_key(
             raw_key, password=password, backend=default_backend()
         )
@@ -80,15 +81,16 @@
         return None
 
     if isinstance(value, PublicKey.__args__):
         return value
 
     key_path = os.path.expanduser(value)
     if os.path.isfile(key_path):
-        raw_key = open(key_path, "rb").read()
+        with open(key_path, "rb") as file:
+            raw_key = file.read()
     elif key_format == EncryptionKeyFormat.ssh:  # ssh key format is one line
         raw_key = to_bytes(value)
     else:
         raw_key = maybe_decode_multiline_key(value)
 
     if key_format == EncryptionKeyFormat.pem:
         return serialization.load_pem_public_key(raw_key, backend=default_backend())
```

### Comparing `opal-common-0.7.5/opal_common/authentication/deps.py` & `opal_common-0.7.6/opal_common/authentication/deps.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/authentication/signer.py` & `opal_common-0.7.6/opal_common/authentication/signer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/authentication/tests/jwt_signer_test.py` & `opal_common-0.7.6/opal_common/authentication/tests/jwt_signer_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/authentication/verifier.py` & `opal_common-0.7.6/opal_common/authentication/verifier.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/cli/commands.py` & `opal_common-0.7.6/opal_common/cli/commands.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/cli/docs.py` & `opal_common-0.7.6/opal_common/cli/docs.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/confi/cli.py` & `opal_common-0.7.6/opal_common/confi/cli.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/confi/confi.py` & `opal_common-0.7.6/opal_common/confi/confi.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/confi/types.py` & `opal_common-0.7.6/opal_common/confi/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/config.py` & `opal_common-0.7.6/opal_common/config.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/corn_utils.py` & `opal_common-0.7.6/opal_common/corn_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/emport.py` & `opal_common-0.7.6/opal_common/emport.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/engine/parsing.py` & `opal_common-0.7.6/opal_common/engine/parsing.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/engine/paths.py` & `opal_common-0.7.6/opal_common/engine/paths.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/engine/base_fetching_engine.py` & `opal_common-0.7.6/opal_common/fetcher/engine/base_fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/engine/fetch_worker.py` & `opal_common-0.7.6/opal_common/fetcher/engine/fetch_worker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/engine/fetching_engine.py` & `opal_common-0.7.6/opal_common/fetcher/engine/fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/events.py` & `opal_common-0.7.6/opal_common/fetcher/events.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/fetch_provider.py` & `opal_common-0.7.6/opal_common/fetcher/fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/fetcher_register.py` & `opal_common-0.7.6/opal_common/fetcher/fetcher_register.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py` & `opal_common-0.7.6/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/providers/http_fetch_provider.py` & `opal_common-0.7.6/opal_common/fetcher/providers/http_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/tests/failure_handler_test.py` & `opal_common-0.7.6/opal_common/fetcher/tests/failure_handler_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/tests/http_fetch_test.py` & `opal_common-0.7.6/opal_common/fetcher/tests/http_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/fetcher/tests/rpc_fetch_test.py` & `opal_common-0.7.6/opal_common/fetcher/tests/rpc_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/git/branch_tracker.py` & `opal_common-0.7.6/opal_common/git/branch_tracker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/git/bundle_maker.py` & `opal_common-0.7.6/opal_common/git/bundle_maker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/git/bundle_utils.py` & `opal_common-0.7.6/opal_common/git/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/git/commit_viewer.py` & `opal_common-0.7.6/opal_common/git/commit_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/git/diff_viewer.py` & `opal_common-0.7.6/opal_common/git/diff_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/git/env.py` & `opal_common-0.7.6/opal_common/git/env.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/git/repo_cloner.py` & `opal_common-0.7.6/opal_common/git/repo_cloner.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/git/tar_file_to_local_git_extractor.py` & `opal_common-0.7.6/opal_common/git/tar_file_to_local_git_extractor.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/logger.py` & `opal_common-0.7.6/opal_common/logger.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/logging/filter.py` & `opal_common-0.7.6/opal_common/logging/filter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/logging/formatter.py` & `opal_common-0.7.6/opal_common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/logging/intercept.py` & `opal_common-0.7.6/opal_common/logging/intercept.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/logging/thirdparty.py` & `opal_common-0.7.6/opal_common/logging/thirdparty.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/middleware.py` & `opal_common-0.7.6/opal_common/middleware.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/monitoring/apm.py` & `opal_common-0.7.6/opal_common/monitoring/apm.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/monitoring/metrics.py` & `opal_common-0.7.6/opal_common/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/paths.py` & `opal_common-0.7.6/opal_common/paths.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/schemas/data.py` & `opal_common-0.7.6/opal_common/schemas/data.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/schemas/policy.py` & `opal_common-0.7.6/opal_common/schemas/policy.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/schemas/policy_source.py` & `opal_common-0.7.6/opal_common/schemas/policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/schemas/security.py` & `opal_common-0.7.6/opal_common/schemas/security.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/schemas/store.py` & `opal_common-0.7.6/opal_common/schemas/store.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/schemas/webhook.py` & `opal_common-0.7.6/opal_common/schemas/webhook.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/security/sslcontext.py` & `opal_common-0.7.6/opal_common/security/sslcontext.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/security/tarsafe.py` & `opal_common-0.7.6/opal_common/security/tarsafe.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/sources/api_policy_source.py` & `opal_common-0.7.6/opal_common/sources/api_policy_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,28 @@
     def __init__(
         self,
         remote_source_url: str,
         local_clone_path: str,
         polling_interval: int = 0,
         token: Optional[str] = None,
         token_id: Optional[str] = None,
+        region: Optional[str] = None,
         bundle_server_type: Optional[PolicyBundleServerType] = None,
         policy_bundle_path=".",
         policy_bundle_git_add_pattern="*",
     ):
         super().__init__(
             remote_source_url=remote_source_url,
             local_clone_path=local_clone_path,
             polling_interval=polling_interval,
         )
         self.token = token
         self.token_id = token_id
         self.server_type = bundle_server_type
+        self.region = region
         self.bundle_hash = None
         self.etag = None
         self.tmp_bundle_path = Path(policy_bundle_path)
         self.policy_bundle_git_add_pattern = policy_bundle_git_add_pattern
         self.tar_to_git = TarFileToLocalGitExtractor(
             self.local_clone_path,
             self.tmp_bundle_path,
@@ -132,15 +134,17 @@
             and token is not None
             and self.token_id is not None
         ):
             split_url = urlparse(self.remote_source_url)
             host = split_url.netloc
             path = split_url.path + "/" + path
 
-            return build_aws_rest_auth_headers(self.token_id, token, host, path)
+            return build_aws_rest_auth_headers(
+                self.token_id, token, host, path, self.region
+            )
         else:
             return {}
 
     async def fetch_policy_bundle_from_api_source(
         self, url: str, token: Optional[str]
     ) -> Tuple[Path, BundleHash, BundleHash]:
         """Fetches the bundle. May throw, in which case we retry again. Checks
```

### Comparing `opal-common-0.7.5/opal_common/sources/base_policy_source.py` & `opal_common-0.7.6/opal_common/sources/base_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/sources/git_policy_source.py` & `opal_common-0.7.6/opal_common/sources/git_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/synchronization/expiring_redis_lock.py` & `opal_common-0.7.6/opal_common/synchronization/expiring_redis_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/synchronization/named_lock.py` & `opal_common-0.7.6/opal_common/synchronization/named_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/tests/path_utils_test.py` & `opal_common-0.7.6/opal_common/tests/path_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/tests/test_utils.py` & `opal_common-0.7.6/opal_common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/tests/url_utils_test.py` & `opal_common-0.7.6/opal_common/tests/url_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/topics/listener.py` & `opal_common-0.7.6/opal_common/topics/listener.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/topics/publisher.py` & `opal_common-0.7.6/opal_common/topics/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/topics/utils.py` & `opal_common-0.7.6/opal_common/topics/utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/urls.py` & `opal_common-0.7.6/opal_common/urls.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/opal_common/utils.py` & `opal_common-0.7.6/opal_common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
     return dict([tup])
 
 
 def get_authorization_header(token: str) -> Tuple[str, str]:
     return "Authorization", f"Bearer {token}"
 
 
-def build_aws_rest_auth_headers(key_id: str, secret_key: str, host: str, path: str):
+def build_aws_rest_auth_headers(
+    key_id: str, secret_key: str, host: str, path: str, region: str
+):
     """Use the AWS signature algorithm (https://docs.aws.amazon.com/AmazonS3/la
     test/userguide/RESTAuthentication.html) to generate the hTTP headers.
 
     Args:
         key_id (str): Access key (aka user ID) of an account in the S3 service.
         secret_key (str): Secret key (aka password) of an account in the S3 service.
         host (str): S3 storage host
@@ -75,14 +77,17 @@
     def getSignatureKey(key, dateStamp, regionName, serviceName):
         kDate = sign(("AWS4" + key).encode("utf-8"), dateStamp)
         kRegion = sign(kDate, regionName)
         kService = sign(kRegion, serviceName)
         kSigning = sign(kService, "aws4_request")
         return kSigning
 
+    # SHA256 of empty string.  This is needed when S3 request payload is empty.
+    SHA256_EMPTY = "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"
+
     t = datetime.utcnow()
     amzdate = t.strftime("%Y%m%dT%H%M%SZ")
     datestamp = t.strftime("%Y%m%d")
 
     canonical_headers = "host:" + host + "\n" + "x-amz-date:" + amzdate + "\n"
     signed_headers = "host;x-amz-date"
 
@@ -97,15 +102,14 @@
         + canonical_headers
         + "\n"
         + signed_headers
         + "\n"
         + payload_hash
     )
 
-    region = "us-east-1"
     algorithm = "AWS4-HMAC-SHA256"
     credential_scope = datestamp + "/" + region + "/" + "s3" + "/" + "aws4_request"
 
     string_to_sign = (
         algorithm
         + "\n"
         + amzdate
@@ -132,14 +136,15 @@
         + ", "
         + "Signature="
         + signature
     )
 
     return {
         "x-amz-date": amzdate,
+        "x-amz-content-sha256": SHA256_EMPTY,
         "Authorization": authorization_header,
     }
 
 
 def sorted_list_from_set(s: set) -> list:
     l = list(s)
     l.sort()
```

### Comparing `opal-common-0.7.5/opal_common.egg-info/PKG-INFO` & `opal_common-0.7.6/opal_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.7.5
+Version: 0.7.6
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp<4,>=3.9.2
 Requires-Dist: click<9,>=8.1.3
-Requires-Dist: cryptography<42,>=41.0.2
+Requires-Dist: cryptography<43,>=42.0.4
 Requires-Dist: gitpython<4,>=3.1.32
 Requires-Dist: loguru<1,>=0.6.0
 Requires-Dist: pyjwt[crypto]<3,>=2.4.0
 Requires-Dist: python-decouple<4,>=3.6
 Requires-Dist: tenacity<9,>=8.0.1
 Requires-Dist: datadog<1,>=0.44.0
-Requires-Dist: ddtrace<3,>=2
-Requires-Dist: charset-normalizer<3,>=2.0.12
+Requires-Dist: ddtrace<3,>=2.8.1
+Requires-Dist: certifi>=2023.7.22
+Requires-Dist: requests>=2.31.0
 Requires-Dist: idna<4,>=3.3
 Requires-Dist: typer<1,>=0.4.1
 Requires-Dist: fastapi<1,>=0.109.1
 Requires-Dist: fastapi_websocket_pubsub==0.3.7
 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0
+Requires-Dist: gunicorn<23,>=22.0.0
 Requires-Dist: pydantic[email]<2,>=1.9.1
 Requires-Dist: typing-extensions; python_version < "3.8"
 Requires-Dist: uvicorn[standard]<1,>=0.17.6
 Requires-Dist: fastapi-utils<1,>=0.2.1
 Requires-Dist: setuptools>=65.5.1
 
 <p  align="center">
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: opal-common Version: 0.7.5 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.6 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet ::
-WWW/HTTP :: WSGI Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp<4,>=3.9.2 Requires-Dist: click<9,>=8.1.3 Requires-Dist:
-cryptography<42,>=41.0.2 Requires-Dist: gitpython<4,>=3.1.32 Requires-Dist:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/
+HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
+Requires-Python: >=3.9 Description-Content-Type: text/markdown Requires-Dist:
+aiohttp<4,>=3.9.2 Requires-Dist: click<9,>=8.1.3 Requires-Dist:
+cryptography<43,>=42.0.4 Requires-Dist: gitpython<4,>=3.1.32 Requires-Dist:
 loguru<1,>=0.6.0 Requires-Dist: pyjwt[crypto]<3,>=2.4.0 Requires-Dist: python-
 decouple<4,>=3.6 Requires-Dist: tenacity<9,>=8.0.1 Requires-Dist:
-datadog<1,>=0.44.0 Requires-Dist: ddtrace<3,>=2 Requires-Dist: charset-
-normalizer<3,>=2.0.12 Requires-Dist: idna<4,>=3.3 Requires-Dist:
-typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
-fastapi_websocket_pubsub==0.3.7 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0 Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist: uvicorn
-[standard]<1,>=0.17.6 Requires-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist:
-setuptools>=65.5.1
+datadog<1,>=0.44.0 Requires-Dist: ddtrace<3,>=2.8.1 Requires-Dist:
+certifi>=2023.7.22 Requires-Dist: requests>=2.31.0 Requires-Dist: idna<4,>=3.3
+Requires-Dist: typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-
+Dist: fastapi_websocket_pubsub==0.3.7 Requires-Dist:
+fastapi_websocket_rpc<1,>=0.1.21 Requires-Dist: gunicorn<23,>=22.0.0 Requires-
+Dist: pydantic[email]<2,>=1.9.1 Requires-Dist: typing-extensions;
+python_version < "3.8" Requires-Dist: uvicorn[standard]<1,>=0.17.6 Requires-
+Dist: fastapi-utils<1,>=0.2.1 Requires-Dist: setuptools>=65.5.1
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
 _p_e_r_m_i_t___i_o_?_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_p_e_r_m_i_t___i_o_&_s_t_y_l_e_=_s_o_c_i_a_l_]## What is OPAL? OPAL is an
 administration layer for Policy Engines such as _O_p_e_n_ _P_o_l_i_c_y_ _A_g_e_n_t_ _(_O_P_A_), and
```

### Comparing `opal-common-0.7.5/opal_common.egg-info/SOURCES.txt` & `opal_common-0.7.6/opal_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.5/setup.py` & `opal_common-0.7.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,16 +60,17 @@
     license=about.__license__,
     packages=find_packages(include=("opal_common*",)),
     classifiers=[
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
         "Topic :: Internet :: WWW/HTTP :: WSGI",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     install_requires=common_install_requires + about.get_install_requires(project_root),
 )
```

