# Comparing `tmp/opal-server-0.7.5.tar.gz` & `tmp/opal_server-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-server-0.7.5.tar", last modified: Wed Mar 13 16:42:10 2024, max compression
+gzip compressed data, was "opal_server-0.7.6.tar", last modified: Tue Apr 30 17:18:49 2024, max compression
```

## Comparing `opal-server-0.7.5.tar` & `opal_server-0.7.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.916286 opal-server-0.7.5/
--rw-r--r--   0 roekatz    (501) staff       (20)    10188 2024-03-13 16:42:10.916004 opal-server-0.7.5/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.908712 opal-server-0.7.5/opal_server/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-05-29 10:10:14.000000 opal-server-0.7.5/opal_server/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11162 2024-03-13 14:22:17.000000 opal-server-0.7.5/opal_server/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.910837 opal-server-0.7.5/opal_server/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5303 2023-06-20 17:01:29.000000 opal-server-0.7.5/opal_server/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6171 2024-03-06 13:35:27.000000 opal-server-0.7.5/opal_server/data/data_update_publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15201 2024-03-06 13:35:27.000000 opal-server-0.7.5/opal_server/git_fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/loadlimiting.py
--rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.911099 opal-server-0.7.5/opal_server/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/policy/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.911307 opal-server-0.7.5/opal_server/policy/bundles/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/policy/bundles/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4447 2023-05-29 10:10:14.000000 opal-server-0.7.5/opal_server/policy/bundles/api.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.912373 opal-server-0.7.5/opal_server/policy/watcher/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-server-0.7.5/opal_server/policy/watcher/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4529 2023-06-20 17:01:29.000000 opal-server-0.7.5/opal_server/policy/watcher/callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6422 2023-06-20 17:01:29.000000 opal-server-0.7.5/opal_server/policy/watcher/factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4767 2023-06-27 11:27:39.000000 opal-server-0.7.5/opal_server/policy/watcher/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.913262 opal-server-0.7.5/opal_server/policy/webhook/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/policy/webhook/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5690 2024-03-06 13:35:27.000000 opal-server-0.7.5/opal_server/policy/webhook/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-05-29 10:10:14.000000 opal-server-0.7.5/opal_server/policy/webhook/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/policy/webhook/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8009 2024-03-06 13:35:27.000000 opal-server-0.7.5/opal_server/pubsub.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1404 2023-10-04 11:07:26.000000 opal-server-0.7.5/opal_server/redis.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.914931 opal-server-0.7.5/opal_server/scopes/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/scopes/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12784 2024-03-06 13:35:27.000000 opal-server-0.7.5/opal_server/scopes/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-05-29 10:10:14.000000 opal-server-0.7.5/opal_server/scopes/loader.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1325 2023-05-09 07:59:18.000000 opal-server-0.7.5/opal_server/scopes/scope_repository.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8442 2024-03-06 13:35:27.000000 opal-server-0.7.5/opal_server/scopes/service.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3104 2024-03-06 13:35:27.000000 opal-server-0.7.5/opal_server/scopes/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.915429 opal-server-0.7.5/opal_server/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1423 2023-05-09 07:59:18.000000 opal-server-0.7.5/opal_server/security/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal-server-0.7.5/opal_server/security/jwks.py
--rw-r--r--   0 roekatz    (501) staff       (20)    17714 2024-03-06 13:35:27.000000 opal-server-0.7.5/opal_server/server.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-06-18 09:47:49.000000 opal-server-0.7.5/opal_server/statistics.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-03-13 16:42:10.915638 opal-server-0.7.5/opal_server.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)    10188 2024-03-13 16:42:10.000000 opal-server-0.7.5/opal_server.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1246 2024-03-13 16:42:10.000000 opal-server-0.7.5/opal_server.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-03-13 16:42:10.000000 opal-server-0.7.5/opal_server.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2024-03-13 16:42:10.000000 opal-server-0.7.5/opal_server.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      527 2024-03-13 16:42:10.000000 opal-server-0.7.5/opal_server.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-03-13 16:42:10.000000 opal-server-0.7.5/opal_server.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-03-13 16:42:10.916336 opal-server-0.7.5/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2979 2022-12-08 13:40:17.000000 opal-server-0.7.5/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.207912 opal_server-0.7.6/
+-rw-r--r--   0 roekatz    (501) staff       (20)    10196 2024-04-30 17:18:49.207451 opal_server-0.7.6/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.202300 opal_server-0.7.6/opal_server/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11336 2024-04-30 12:59:10.000000 opal_server-0.7.6/opal_server/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.203740 opal_server-0.7.6/opal_server/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5303 2023-06-20 17:01:29.000000 opal_server-0.7.6/opal_server/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4004 2024-04-30 13:01:51.000000 opal_server-0.7.6/opal_server/data/data_update_publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    15201 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/git_fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/loadlimiting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.203872 opal_server-0.7.6/opal_server/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/policy/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.204103 opal_server-0.7.6/opal_server/policy/bundles/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/policy/bundles/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4447 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/policy/bundles/api.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.204701 opal_server-0.7.6/opal_server/policy/watcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/policy/watcher/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4529 2023-06-20 17:01:29.000000 opal_server-0.7.6/opal_server/policy/watcher/callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6662 2024-04-30 12:59:10.000000 opal_server-0.7.6/opal_server/policy/watcher/factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4767 2023-06-27 11:27:39.000000 opal_server-0.7.6/opal_server/policy/watcher/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.205297 opal_server-0.7.6/opal_server/policy/webhook/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/policy/webhook/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5690 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/policy/webhook/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/policy/webhook/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/policy/webhook/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8009 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/pubsub.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1404 2023-10-04 11:07:26.000000 opal_server-0.7.6/opal_server/redis.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.206198 opal_server-0.7.6/opal_server/scopes/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/scopes/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12784 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/scopes/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/scopes/loader.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1325 2023-05-09 07:59:18.000000 opal_server-0.7.6/opal_server/scopes/scope_repository.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8442 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/scopes/service.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3104 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/scopes/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.206642 opal_server-0.7.6/opal_server/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1423 2023-05-09 07:59:18.000000 opal_server-0.7.6/opal_server/security/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/security/jwks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    17339 2024-04-30 13:01:51.000000 opal_server-0.7.6/opal_server/server.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-06-18 09:47:49.000000 opal_server-0.7.6/opal_server/statistics.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.206885 opal_server-0.7.6/opal_server.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)    10196 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1246 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      497 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-04-30 17:18:49.207975 opal_server-0.7.6/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     3031 2024-04-30 13:01:51.000000 opal_server-0.7.6/setup.py
```

### Comparing `opal-server-0.7.5/PKG-INFO` & `opal_server-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.7.5
+Version: 0.7.6
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
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
 Requires-Dist: click<9,>=8.1.3
 Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5
 Requires-Dist: gitpython<4,>=3.1.32
 Requires-Dist: pyjwt[crypto]<3,>=2.1.0
 Requires-Dist: websockets<11,>=10.3
 Requires-Dist: slowapi<1,>=0.1.5
 Requires-Dist: pygit2<2,>=1.13.3
 Requires-Dist: asgiref<4,>=3.5.2
 Requires-Dist: redis<5,>=4.3.4
-Requires-Dist: opal-common==0.7.5
-Requires-Dist: charset-normalizer<3,>=2.0.12
+Requires-Dist: opal-common==0.7.6
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
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.7.5 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.6 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
-:: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist:
-click<9,>=8.1.3 Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5
-Requires-Dist: gitpython<4,>=3.1.32 Requires-Dist: pyjwt[crypto]<3,>=2.1.0
-Requires-Dist: websockets<11,>=10.3 Requires-Dist: slowapi<1,>=0.1.5 Requires-
-Dist: pygit2<2,>=1.13.3 Requires-Dist: asgiref<4,>=3.5.2 Requires-Dist:
-redis<5,>=4.3.4 Requires-Dist: opal-common==0.7.5 Requires-Dist: charset-
-normalizer<3,>=2.0.12 Requires-Dist: idna<4,>=3.3 Requires-Dist:
-typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
-fastapi_websocket_pubsub==0.3.7 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0 Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist: uvicorn
-[standard]<1,>=0.17.6 Requires-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist:
-setuptools>=65.5.1
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP
+Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python:
+>=3.9 Description-Content-Type: text/markdown Requires-Dist: click<9,>=8.1.3
+Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5 Requires-Dist:
+gitpython<4,>=3.1.32 Requires-Dist: pyjwt[crypto]<3,>=2.1.0 Requires-Dist:
+websockets<11,>=10.3 Requires-Dist: slowapi<1,>=0.1.5 Requires-Dist:
+pygit2<2,>=1.13.3 Requires-Dist: asgiref<4,>=3.5.2 Requires-Dist:
+redis<5,>=4.3.4 Requires-Dist: opal-common==0.7.6 Requires-Dist: idna<4,>=3.3
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

### Comparing `opal-server-0.7.5/opal_server/cli.py` & `opal_server-0.7.6/opal_server/cli.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/config.py` & `opal_server-0.7.6/opal_server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,19 @@
         description="Secret token to be sent to API bundle server",
     )
     POLICY_BUNDLE_SERVER_TOKEN_ID = confi.str(
         "POLICY_BUNDLE_SERVER_TOKEN_ID",
         None,
         description="The id of the secret token to be sent to API bundle server",
     )
+    POLICY_BUNDLE_SERVER_AWS_REGION = confi.str(
+        "POLICY_BUNDLE_SERVER_AWS_REGION",
+        "us-east-1",
+        description="The AWS region of the S3 bucket",
+    )
     POLICY_BUNDLE_TMP_PATH = confi.str(
         "POLICY_BUNDLE_TMP_PATH",
         "/tmp/bundle.tar.gz",
         description="Path for temp policy file, need to be writeable",
     )
     POLICY_BUNDLE_GIT_ADD_PATTERN = confi.str(
         "POLICY_BUNDLE_GIT_ADD_PATTERN",
```

### Comparing `opal-server-0.7.5/opal_server/data/api.py` & `opal_server-0.7.6/opal_server/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/git_fetcher.py` & `opal_server-0.7.6/opal_server/git_fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/loadlimiting.py` & `opal_server-0.7.6/opal_server/loadlimiting.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/policy/bundles/api.py` & `opal_server-0.7.6/opal_server/policy/bundles/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/policy/watcher/callbacks.py` & `opal_server-0.7.6/opal_server/policy/watcher/callbacks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/policy/watcher/factory.py` & `opal_server-0.7.6/opal_server/policy/watcher/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     branch_name: str = None,
     ssh_key: Optional[str] = None,
     polling_interval: int = None,
     request_timeout: int = None,
     policy_bundle_token: str = None,
     policy_bundle_token_id: str = None,
     policy_bundle_server_type: str = None,
+    policy_bundle_aws_region: str = None,
     extensions: Optional[List[str]] = None,
     bundle_ignore: Optional[List[str]] = None,
 ) -> BasePolicyWatcherTask:
     """Create a PolicyWatcherTask with Git / API policy source defined by env
     vars Load all the defaults from config if called without params.
 
     Args:
@@ -111,23 +112,27 @@
             )
         policy_bundle_token_id = load_conf_if_none(
             policy_bundle_token_id, opal_server_config.POLICY_BUNDLE_SERVER_TOKEN_ID
         )
         policy_bundle_server_type = load_conf_if_none(
             policy_bundle_server_type, opal_server_config.POLICY_BUNDLE_SERVER_TYPE
         )
+        policy_bundle_aws_region = load_conf_if_none(
+            policy_bundle_aws_region, opal_server_config.POLICY_BUNDLE_SERVER_AWS_REGION
+        )
         watcher = ApiPolicySource(
             remote_source_url=remote_source_url,
             local_clone_path=clone_path,
             polling_interval=polling_interval,
             token=policy_bundle_token,
             token_id=policy_bundle_token_id,
             bundle_server_type=policy_bundle_server_type,
             policy_bundle_path=opal_server_config.POLICY_BUNDLE_TMP_PATH,
             policy_bundle_git_add_pattern=opal_server_config.POLICY_BUNDLE_GIT_ADD_PATTERN,
+            region=policy_bundle_aws_region,
         )
     else:
         raise ValueError("Unknown value for OPAL_POLICY_SOURCE_TYPE")
     watcher.add_on_new_policy_callback(
         partial(
             publish_changed_directories,
             publisher=publisher,
```

### Comparing `opal-server-0.7.5/opal_server/policy/watcher/task.py` & `opal_server-0.7.6/opal_server/policy/watcher/task.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/policy/webhook/api.py` & `opal_server-0.7.6/opal_server/policy/webhook/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/policy/webhook/deps.py` & `opal_server-0.7.6/opal_server/policy/webhook/deps.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/policy/webhook/listener.py` & `opal_server-0.7.6/opal_server/policy/webhook/listener.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/publisher.py` & `opal_server-0.7.6/opal_server/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/pubsub.py` & `opal_server-0.7.6/opal_server/pubsub.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/redis.py` & `opal_server-0.7.6/opal_server/redis.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/scopes/api.py` & `opal_server-0.7.6/opal_server/scopes/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/scopes/loader.py` & `opal_server-0.7.6/opal_server/scopes/loader.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/scopes/scope_repository.py` & `opal_server-0.7.6/opal_server/scopes/scope_repository.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/scopes/service.py` & `opal_server-0.7.6/opal_server/scopes/service.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/scopes/task.py` & `opal_server-0.7.6/opal_server/scopes/task.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/security/api.py` & `opal_server-0.7.6/opal_server/security/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/security/jwks.py` & `opal_server-0.7.6/opal_server/security/jwks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server/server.py` & `opal_server-0.7.6/opal_server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,22 +346,15 @@
                     # only one worker gets here, the others block. in case the leader worker
                     # is terminated, another one will obtain the lock and become leader.
                     logger.info(
                         "leadership lock acquired, leader pid: {pid}",
                         pid=os.getpid(),
                     )
 
-                    if not opal_server_config.SCOPES:
-                        # bind data updater publishers to the leader worker
-                        asyncio.create_task(
-                            DataUpdatePublisher.mount_and_start_polling_updates(
-                                self.publisher, opal_server_config.DATA_CONFIG_SOURCES
-                            )
-                        )
-                    else:
+                    if opal_server_config.SCOPES:
                         await load_scopes(self._scopes)
 
                     if self.broadcast_keepalive is not None:
                         self.broadcast_keepalive.start()
                         if not self._init_policy_watcher:
                             # Wait on keepalive instead to keep leadership lock acquired
                             await self.broadcast_keepalive.wait_until_done()
```

### Comparing `opal-server-0.7.5/opal_server/statistics.py` & `opal_server-0.7.6/opal_server/statistics.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/opal_server.egg-info/PKG-INFO` & `opal_server-0.7.6/opal_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.7.5
+Version: 0.7.6
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
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
 Requires-Dist: click<9,>=8.1.3
 Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5
 Requires-Dist: gitpython<4,>=3.1.32
 Requires-Dist: pyjwt[crypto]<3,>=2.1.0
 Requires-Dist: websockets<11,>=10.3
 Requires-Dist: slowapi<1,>=0.1.5
 Requires-Dist: pygit2<2,>=1.13.3
 Requires-Dist: asgiref<4,>=3.5.2
 Requires-Dist: redis<5,>=4.3.4
-Requires-Dist: opal-common==0.7.5
-Requires-Dist: charset-normalizer<3,>=2.0.12
+Requires-Dist: opal-common==0.7.6
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
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.7.5 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.6 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
-:: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist:
-click<9,>=8.1.3 Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5
-Requires-Dist: gitpython<4,>=3.1.32 Requires-Dist: pyjwt[crypto]<3,>=2.1.0
-Requires-Dist: websockets<11,>=10.3 Requires-Dist: slowapi<1,>=0.1.5 Requires-
-Dist: pygit2<2,>=1.13.3 Requires-Dist: asgiref<4,>=3.5.2 Requires-Dist:
-redis<5,>=4.3.4 Requires-Dist: opal-common==0.7.5 Requires-Dist: charset-
-normalizer<3,>=2.0.12 Requires-Dist: idna<4,>=3.3 Requires-Dist:
-typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-Dist:
-fastapi_websocket_pubsub==0.3.7 Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<21,>=20.1.0 Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist: uvicorn
-[standard]<1,>=0.17.6 Requires-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist:
-setuptools>=65.5.1
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP
+Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python:
+>=3.9 Description-Content-Type: text/markdown Requires-Dist: click<9,>=8.1.3
+Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5 Requires-Dist:
+gitpython<4,>=3.1.32 Requires-Dist: pyjwt[crypto]<3,>=2.1.0 Requires-Dist:
+websockets<11,>=10.3 Requires-Dist: slowapi<1,>=0.1.5 Requires-Dist:
+pygit2<2,>=1.13.3 Requires-Dist: asgiref<4,>=3.5.2 Requires-Dist:
+redis<5,>=4.3.4 Requires-Dist: opal-common==0.7.6 Requires-Dist: idna<4,>=3.3
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

### Comparing `opal-server-0.7.5/opal_server.egg-info/SOURCES.txt` & `opal_server-0.7.6/opal_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.5/setup.py` & `opal_server-0.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,20 @@
     license=about.__license__,
     packages=find_packages(include=("opal_server*",)),
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
     install_requires=server_install_requires + about.get_install_requires(project_root),
     entry_points={
         "console_scripts": ["opal-server = opal_server.cli:cli"],
     },
 )
```

