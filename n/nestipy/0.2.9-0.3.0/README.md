# Comparing `tmp/nestipy-0.2.9.tar.gz` & `tmp/nestipy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.2.9.tar", max compression
+gzip compressed data, was "nestipy-0.3.0.tar", max compression
```

## Comparing `nestipy-0.2.9.tar` & `nestipy-0.3.0.tar`

### file list

```diff
@@ -1,119 +1,203 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.2.9/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy-0.2.9/README.md
--rw-r--r--   0        0        0      766 2024-04-29 13:27:48.293591 nestipy-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.2.9/src/nestipy/__init__.py
--rw-r--r--   0        0        0     1151 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-27 15:32:43.416679 nestipy-0.2.9/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.2.9/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0      978 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/config/__init__.py
--rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     2957 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/decorator/class_.py
--rw-r--r--   0        0        0     1204 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/decorator/method.py
--rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/exception/__init__.py
--rw-r--r--   0        0        0      732 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/exception/decorator.py
--rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/exception/http.py
--rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/exception/interface.py
--rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/exception/message.py
--rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/exception/meta.py
--rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/exception/status.py
--rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/guards/__init__.py
--rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/guards/can_activate.py
--rw-r--r--   0        0        0      332 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/guards/decorator.py
--rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/guards/meta.py
--rw-r--r--   0        0        0      719 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/helpers/__init__.py
--rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/http_/__init__.py
--rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/http_/multipart.py
--rw-r--r--   0        0        0     5076 2024-04-29 13:05:25.109202 nestipy-0.2.9/src/nestipy/common/http_/request.py
--rw-r--r--   0        0        0     4989 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/http_/response.py
--rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/http_/test.py
--rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/http_/upload_file.py
--rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/http_/websocket.py
--rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/interceptor/__init__.py
--rw-r--r--   0        0        0      489 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/interceptor/decorator.py
--rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/interceptor/interface.py
--rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/interceptor/meta.py
--rw-r--r--   0        0        0      168 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/middleware/__init__.py
--rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/middleware/cors.py
--rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/middleware/interface.py
--rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/middleware/meta.py
--rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/template/__init__.py
--rw-r--r--   0        0        0      274 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/template/decorator.py
--rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/template/interface.py
--rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/template/meta.py
--rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/common/utils.py
--rw-r--r--   0        0        0      933 2024-04-29 11:25:01.889396 nestipy-0.2.9/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-29 12:59:37.017620 nestipy-0.2.9/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.2.9/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.2.9/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.2.9/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/adapter/__init__.py
--rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/adapter/blacksheep_adapter.py
--rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/adapter/fastapi_adapter.py
--rw-r--r--   0        0        0     5666 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/adapter/http_adapter.py
--rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/constant.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/context/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/context/argument_host.py
--rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/context/execution_context.py
--rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/context/http_argument_host.py
--rw-r--r--   0        0        0      730 2024-04-27 15:32:43.416679 nestipy-0.2.9/src/nestipy/core/discover.py
--rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/exception/__init__.py
--rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.156372 nestipy-0.2.9/src/nestipy/core/exception/processor.py
--rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/guards/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/guards/processor.py
--rw-r--r--   0        0        0     3847 2024-04-29 11:49:41.852686 nestipy-0.2.9/src/nestipy/core/instance_loader.py
--rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/interceptor/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/interceptor/processor.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/meta/__init__.py
--rw-r--r--   0        0        0      380 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/meta/controller_metadata_creator.py
--rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/meta/metadata_creator.py
--rw-r--r--   0        0        0      771 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/meta/module_metadata_creator.py
--rw-r--r--   0        0        0      374 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/meta/provider_metadata_creator.py
--rw-r--r--   0        0        0      162 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/middleware/__init__.py
--rw-r--r--   0        0        0     3949 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/middleware/executor.py
--rw-r--r--   0        0        0     8889 2024-04-27 15:32:43.416679 nestipy-0.2.9/src/nestipy/core/nestipy_application.py
--rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/nestipy_factory.py
--rw-r--r--   0        0        0       64 2024-04-29 11:24:26.410705 nestipy-0.2.9/src/nestipy/core/on_destroy.py
--rw-r--r--   0        0        0       60 2024-04-29 11:24:33.962421 nestipy-0.2.9/src/nestipy/core/on_init.py
--rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      608 2024-04-27 15:32:43.416679 nestipy-0.2.9/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.2.9/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.2.9/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.2.9/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/router/__init__.py
--rw-r--r--   0        0        0     2879 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/router/route_explorer.py
--rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/router/route_extractor.py
--rw-r--r--   0        0        0     7920 2024-04-27 15:32:43.416679 nestipy-0.2.9/src/nestipy/core/router/router_proxy.py
--rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/template/__init__.py
--rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/template/minimal_jinja.py
--rw-r--r--   0        0        0     1457 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/core/template/processor.py
--rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/__init__.py
--rw-r--r--   0        0        0     1533 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/decorator.py
--rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/graphql_adapter.py
--rw-r--r--   0        0        0     1111 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/graphql_asgi.py
--rw-r--r--   0        0        0     1871 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/graphql_explorer.py
--rw-r--r--   0        0        0      547 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/graphql_module.py
--rw-r--r--   0        0        0     4326 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/graphql_proxy.py
--rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/meta.py
--rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/playground/graphql-playground-default.html
--rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/playground/graphql-playground-graphiql.html
--rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/pubsub.py
--rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/strawberry/__init__.py
--rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/strawberry/strawberry_adapter.py
--rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/strawberry/strawberry_asgi.py
--rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/graphql/test.py
--rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/openapi/__init__.py
--rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/openapi/constant.py
--rw-r--r--   0        0        0     3139 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/openapi/decorator.py
--rw-r--r--   0        0        0     1500 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/openapi/document_builder.py
--rw-r--r--   0        0        0      423 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/openapi/explorer.py
--rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/openapi/swagger.html
--rw-r--r--   0        0        0     2195 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/openapi/swagger_module.py
--rw-r--r--   0        0        0     2728 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/openapi/test.py
--rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/types_/__init__.py
--rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/types_/handler.py
--rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/types_/http.py
--rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/websocket/__init__.py
--rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/websocket/adapter.py
--rw-r--r--   0        0        0      716 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/websocket/decorator.py
--rw-r--r--   0        0        0     4517 2024-04-26 12:17:55.160372 nestipy-0.2.9/src/nestipy/websocket/proxy.py
--rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 nestipy-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-29 14:09:07.000292 nestipy-0.3.0/README.md
+-rw-r--r--   0        0        0      681 2024-04-30 15:13:45.376071 nestipy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.3.0/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1553 2024-04-30 12:37:23.938864 nestipy-0.3.0/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.3.0/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0      978 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      719 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     5299 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     5321 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0      248 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0     3276 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/middleware/session.py
+-rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      933 2024-04-29 14:09:07.020292 nestipy-0.3.0/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0     1179 2024-04-29 14:53:26.309598 nestipy-0.3.0/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.3.0/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.3.0/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.3.0/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0      730 2024-04-29 14:09:07.020292 nestipy-0.3.0/src/nestipy/core/discover.py
+-rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.3.0/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     3847 2024-04-30 15:13:45.376071 nestipy-0.3.0/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3949 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     8889 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0       64 2024-04-29 14:09:07.020292 nestipy-0.3.0/src/nestipy/core/on_destroy.py
+-rw-r--r--   0        0        0       60 2024-04-29 14:09:07.020292 nestipy-0.3.0/src/nestipy/core/on_init.py
+-rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-29 14:09:07.020292 nestipy-0.3.0/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.3.0/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.3.0/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.3.0/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     2879 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     8298 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      231 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/dynamic_module/__init__.py
+-rw-r--r--   0        0        0     3512 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/dynamic_module/builder.py
+-rw-r--r--   0        0        0      139 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/dynamic_module/module/__init__.py
+-rw-r--r--   0        0        0      517 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/dynamic_module/module/consumer.py
+-rw-r--r--   0        0        0      251 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/dynamic_module/module/interface.py
+-rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1111 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      547 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4326 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0      952 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/ioc/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/ioc/annotation.py
+-rw-r--r--   0        0        0    14115 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/ioc/container.py
+-rw-r--r--   0        0        0     1485 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/ioc/context_container.py
+-rw-r--r--   0        0        0     2054 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/ioc/dependency.py
+-rw-r--r--   0        0        0      885 2024-04-30 15:13:45.380071 nestipy-0.3.0/src/nestipy/ioc/meta.py
+-rw-r--r--   0        0        0     3013 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/ioc/middleware.py
+-rw-r--r--   0        0        0      877 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/ioc/provider.py
+-rw-r--r--   0        0        0       56 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/ioc/utils.py
+-rw-r--r--   0        0        0      458 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/__init__.py
+-rw-r--r--   0        0        0     1673 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/class_.py
+-rw-r--r--   0        0        0      508 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/container.py
+-rw-r--r--   0        0        0      710 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/decorator.py
+-rw-r--r--   0        0        0     1004 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/dependency.py
+-rw-r--r--   0        0        0      236 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/module.py
+-rw-r--r--   0        0        0       88 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/provider_token.py
+-rw-r--r--   0        0        0      688 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/reflect.py
+-rw-r--r--   0        0        0      107 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/metadata/route.py
+-rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     3144 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1502 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      423 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0       44 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/__init__.py
+-rw-r--r--   0        0        0     4684 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/common.py
+-rw-r--r--   0        0        0     1325 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/__init__.py
+-rw-r--r--   0        0        0     1757 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/common.py
+-rw-r--r--   0        0        0     1855 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/contents.py
+-rw-r--r--   0        0        0      633 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/generate.py
+-rw-r--r--   0        0        0     3196 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/jinja.py
+-rw-r--r--   0        0        0     1894 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/md.py
+-rw-r--r--   0        0        0     3065 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/texts.py
+-rw-r--r--   0        0        0    21375 2024-04-30 15:13:45.384071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
+-rw-r--r--   0        0        0     4250 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
+-rw-r--r--   0        0        0      103 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
+-rw-r--r--   0        0        0      890 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
+-rw-r--r--   0        0        0      610 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
+-rw-r--r--   0        0        0      730 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
+-rw-r--r--   0        0        0      322 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      284 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
+-rw-r--r--   0        0        0      207 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
+-rw-r--r--   0        0        0      571 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
+-rw-r--r--   0        0        0      873 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
+-rw-r--r--   0        0        0      480 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
+-rw-r--r--   0        0        0      492 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
+-rw-r--r--   0        0        0     1335 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
+-rw-r--r--   0        0        0      929 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
+-rw-r--r--   0        0        0      224 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
+-rw-r--r--   0        0        0      429 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
+-rw-r--r--   0        0        0      286 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
+-rw-r--r--   0        0        0      889 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
+-rw-r--r--   0        0        0      933 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
+-rw-r--r--   0        0        0      843 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
+-rw-r--r--   0        0        0      561 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      383 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
+-rw-r--r--   0        0        0      326 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
+-rw-r--r--   0        0        0      817 2024-04-30 15:13:45.388071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
+-rw-r--r--   0        0        0     1007 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
+-rw-r--r--   0        0        0      616 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
+-rw-r--r--   0        0        0      857 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
+-rw-r--r--   0        0        0     2250 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
+-rw-r--r--   0        0        0     1155 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
+-rw-r--r--   0        0        0      475 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
+-rw-r--r--   0        0        0      638 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
+-rw-r--r--   0        0        0      170 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
+-rw-r--r--   0        0        0      548 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
+-rw-r--r--   0        0        0      670 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
+-rw-r--r--   0        0        0      156 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
+-rw-r--r--   0        0        0      754 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
+-rw-r--r--   0        0        0      670 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
+-rw-r--r--   0        0        0        0 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2844 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/utils/source.py
+-rw-r--r--   0        0        0      878 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/utils/web.py
+-rw-r--r--   0        0        0     9579 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/v2.py
+-rw-r--r--   0        0        0     9667 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/openapi_docs/v3.py
+-rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2199 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     2676 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.3.0/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4517 2024-04-30 15:13:45.392071 nestipy-0.3.0/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 nestipy-0.3.0/PKG-INFO
```

### Comparing `nestipy-0.2.9/LICENSE` & `nestipy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/README.md` & `nestipy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/pyproject.toml` & `nestipy-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.2.9"
+version = "0.3.0"
 description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -13,17 +13,14 @@
 python-socketio = "^5.11.1"
 blacksheep = "^2.0.7"
 aiofiles = "^23.2.1"
 fastapi = "^0.110.0"
 uvicorn = { extras = ["standard"], version = "^0.29.0" }
 strawberry-graphql = "^0.225.0"
 ujson = "^5.9.0"
-nestipy-ioc = "^0.1.31"
-nestipy-metadata = "^0.1.1"
 minijinja = "^2.0.1"
-nestipy-dynamic-module = "0.1.7"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nestipy-0.2.9/src/nestipy/common/__init__.py` & `nestipy-0.3.0/src/nestipy/common/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # TODO: precise import
-from nestipy_ioc import ModuleProviderDict
+from nestipy.ioc import ModuleProviderDict
 
 from .config import ConfigModule, ConfigService
 from .decorator import Module, Controller, Injectable, Route, Get, Post, Patch, Put, Delete
 from .exception import HttpException, HttpStatusMessages, HttpStatus, UseFilters, Catch, ExceptionKey, ExceptionFilter
 from .guards import CanActivate, UseGuards
 from .http_ import Request, Response, Websocket, UploadFile
 from .interceptor import NestipyInterceptor, UseInterceptors
-from .middleware import cors, NestipyMiddleware
+from .middleware import cors, NestipyMiddleware, session, SessionOption
 from .template import Render, TemplateEngine
 
 __all__ = [
     "ConfigModule",
     "ConfigService",
     "Module",
     "Controller",
@@ -37,9 +37,11 @@
     "UploadFile",
     "NestipyInterceptor",
     "UseInterceptors",
     "cors",
     "NestipyMiddleware",
     "Render",
     "TemplateEngine",
-    "ModuleProviderDict"
+    "ModuleProviderDict",
+    "session",
+    "SessionOption"
 ]
```

### Comparing `nestipy-0.2.9/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/common/config/__init__.py` & `nestipy-0.3.0/src/nestipy/common/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import asdict
 from typing import Literal
 
 from nestipy.common.decorator import Module, Injectable
-from nestipy_dynamic_module import ConfigurableModuleBuilder
-from nestipy_ioc import ModuleProviderDict, Inject
-from nestipy_metadata import Reflect
+from nestipy.dynamic_module import ConfigurableModuleBuilder
+from nestipy.ioc import ModuleProviderDict, Inject
+from nestipy.metadata import Reflect
 
 Config = dict[Literal['folder'], str]
 ConfigurableModuleClass, CONFIG_MODULE_OPTION_TOKEN = ConfigurableModuleBuilder[Config]().set_method('for_root').build()
 
 
 @Injectable()
 class ConfigService:
```

### Comparing `nestipy-0.2.9/src/nestipy/common/decorator/class_.py` & `nestipy-0.3.0/src/nestipy/common/decorator/class_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import enum
 from typing import Type, Callable, Union
 
-from nestipy_dynamic_module import DynamicModule
-from nestipy_ioc import NestipyContainer, ModuleProviderDict
-from nestipy_metadata import ModuleMetadata, Reflect, RouteKey
+from nestipy.dynamic_module import DynamicModule
+from nestipy.ioc import NestipyContainer, ModuleProviderDict
+from nestipy.metadata import ModuleMetadata, Reflect, RouteKey
 
 
 class Scope(enum.Enum):
     Request = 'Request'
     Transient = 'Transient'
     Singleton = 'Singleton'
```

### Comparing `nestipy-0.2.9/src/nestipy/common/decorator/method.py` & `nestipy-0.3.0/src/nestipy/common/decorator/method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, Literal
 
-from nestipy_metadata import Reflect, RouteKey
+from nestipy.metadata import Reflect, RouteKey
 
 HTTPMethod = Literal['GET', 'POST', 'PUT', 'DELETE', 'PATCH', 'HEAD', 'OPTIONS', 'ALL', 'ANY']
 
 
 class Route:
     def __init__(self, path: str = '', method: list[HTTPMethod] = None, **kwargs):
         if method is None:
```

### Comparing `nestipy-0.2.9/src/nestipy/common/exception/decorator.py` & `nestipy-0.3.0/src/nestipy/common/exception/decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, Type, TYPE_CHECKING
 
-from nestipy_metadata import SetMetadata
+from nestipy.metadata import SetMetadata
 
 from nestipy.common.decorator import Injectable
 from .meta import ExceptionKey
 
 if TYPE_CHECKING:
     from .interface import ExceptionFilter
     from nestipy.common.exception.http import HttpException
```

### Comparing `nestipy-0.2.9/src/nestipy/common/exception/message.py` & `nestipy-0.3.0/src/nestipy/common/exception/message.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/common/exception/status.py` & `nestipy-0.3.0/src/nestipy/common/exception/status.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/common/helpers/__init__.py` & `nestipy-0.3.0/src/nestipy/common/helpers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Type
 
-from nestipy_ioc import ModuleProviderDict
-from nestipy_metadata import ModuleMetadata, Reflect
+from nestipy.ioc import ModuleProviderDict
+from nestipy.metadata import ModuleMetadata, Reflect
 
 
 class SpecialProviderExtractor:
 
     @classmethod
     def extract_special_providers(
             cls,
```

### Comparing `nestipy-0.2.9/src/nestipy/common/http_/multipart.py` & `nestipy-0.3.0/src/nestipy/common/http_/multipart.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/common/http_/request.py` & `nestipy-0.3.0/src/nestipy/common/http_/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from http import cookies as http_cookies
 from typing import Callable, Optional, Any
 from urllib.parse import parse_qsl
-from http import cookies as http_cookies
+
 import ujson
 from starlette.datastructures import UploadFile
 from starlette.requests import Request as StarletteRequest
 
 from .multipart import parse_content_header, parse_multipart_form, parse_url_encoded_form_data
 
 
@@ -91,14 +92,24 @@
 
     @property
     def client(self) -> list:
         if self._client is None:
             self._client = self.scope.get("client", ())
         return self._client
 
+    @property
+    def session(self) -> dict:
+        if self._session is None:
+            self._session = {}
+        return self._session
+
+    @session.setter
+    def session(self, session: dict):
+        self._session = session
+
     def set_body(self, body: str):
         self._body = body
 
     async def body(self) -> str:
         if self._body is None:
             body = b""
             while True:
@@ -144,15 +155,14 @@
                 )
             else:
                 self._form = None
         return self._form
 
     @property
     def cookies(self) -> dict[str, str]:
-        if not hasattr(self, "_cookies"):
+        if self._cookies is None:
             cookies: dict[str, str] = {}
             cookie_header = self.headers.get("cookie")
-
             if cookie_header:
                 cookies = cookie_parser(cookie_header)
             self._cookies = cookies
         return self._cookies
```

### Comparing `nestipy-0.2.9/src/nestipy/common/http_/response.py` & `nestipy-0.3.0/src/nestipy/common/http_/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if TYPE_CHECKING:
     from nestipy.common.template import TemplateEngine
 
 
 class Response:
     _status_code: int = 200
     _headers: set[tuple[str, str]] = set()
+    _cookies: set[tuple[str, str]] = set()
     _content: Union[bytes, None]
 
     def __init__(self, template_engine: "TemplateEngine" = None) -> None:
         self._headers = set()
         self._status_code = 200
         self._content = None
         self._stream_content = None
@@ -46,14 +47,19 @@
         return self
 
     def header(self, name: str, value: str) -> "Response":
         self._headers = set([(k, v) for k, v in self._headers if k.lower() != name.lower])
         self._headers.add((name, value))
         return self
 
+    def cookie(self, name: str, value: str) -> "Response":
+        self._cookies = set([(k, v) for k, v in self._cookies if k.lower() != name.lower])
+        self._cookies.add((name, value))
+        return self
+
     async def send(self, content: str, status_code: int = 200) -> "Response":
         await self.status(status_code)._write(content.encode())
         return self
 
     async def html(self, content: str, status_code: int = None):
         self.header("Content-Type", "text/html")
         self.header('max-age', '0')
@@ -136,13 +142,16 @@
 
     def content(self) -> Union[bytes, None]:
         return self._content
 
     def headers(self) -> set[tuple[str, str]]:
         return self._headers
 
+    def cookies(self) -> set[tuple[str, str]]:
+        return self._cookies
+
     def is_stream(self) -> bool:
         return self._stream_content is not None
 
     async def get_stream(self) -> AsyncIterator[bytes]:
         if self._stream_content is not None:
             yield self._stream_content()
```

### Comparing `nestipy-0.2.9/src/nestipy/common/http_/upload_file.py` & `nestipy-0.3.0/src/nestipy/common/http_/upload_file.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/common/middleware/cors.py` & `nestipy-0.3.0/src/nestipy/common/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/common/template/interface.py` & `nestipy-0.3.0/src/nestipy/common/template/interface.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/common/utils.py` & `nestipy-0.3.0/src/nestipy/common/utils.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/__init__.py` & `nestipy-0.3.0/src/nestipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/core/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8d832f66 (Mon Apr 29 11:25:01 2024 UTC)
+moddate:  0x03aa2f66 (Mon Apr 29 14:09:07 2024 UTC)
 files sz: 933
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `nestipy-0.2.9/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/adapter/blacksheep_adapter.py` & `nestipy-0.3.0/src/nestipy/core/adapter/blacksheep_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/adapter/fastapi_adapter.py` & `nestipy-0.3.0/src/nestipy/core/adapter/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/adapter/http_adapter.py` & `nestipy-0.3.0/src/nestipy/core/adapter/http_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Tuple, Any, Callable, Union, Type, TYPE_CHECKING
 
 from nestipy.common.exception.http import HttpException
 from nestipy.common.http_ import Request, Response, Websocket
 from nestipy.common.template import TemplateKey
 from nestipy.types_ import CallableHandler, NextFn, WebsocketHandler, MountHandler
 from nestipy.websocket.adapter import IoAdapter
-from nestipy_metadata import SetMetadata, Reflect
+from nestipy.metadata import SetMetadata, Reflect
 
 if TYPE_CHECKING:
     from nestipy.common.exception.interface import ExceptionFilter
     from nestipy.common.guards import CanActivate
     from nestipy.common.interceptor import NestipyInterceptor
```

### Comparing `nestipy-0.2.9/src/nestipy/core/context/argument_host.py` & `nestipy-0.3.0/src/nestipy/core/context/argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/context/execution_context.py` & `nestipy-0.3.0/src/nestipy/core/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/discover.py` & `nestipy-0.3.0/src/nestipy/core/discover.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/exception/processor.py` & `nestipy-0.3.0/src/nestipy/core/exception/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from nestipy.common.decorator import Injectable
 from nestipy.common.exception.http import HttpException
 from nestipy.common.exception.interface import ExceptionFilter
 from nestipy.common.exception.meta import ExceptionKey
 from nestipy.common.helpers import SpecialProviderExtractor
 from nestipy.core.constant import APP_FILTER
 from nestipy.core.context.argument_host import ArgumentHost
-from nestipy_ioc import NestipyContainer
-from nestipy_metadata import Reflect, ClassMetadata
+from nestipy.ioc import NestipyContainer
+from nestipy.metadata import Reflect, ClassMetadata
 
 
 @Injectable()
 class ExceptionFilterHandler(SpecialProviderExtractor):
     context: ArgumentHost = None
 
     def __init__(self, ):
```

### Comparing `nestipy-0.2.9/src/nestipy/core/guards/processor.py` & `nestipy-0.3.0/src/nestipy/core/guards/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from nestipy.common.decorator import Injectable
 from nestipy.common.guards.can_activate import CanActivate
 from nestipy.common.guards.meta import GuardKey
 from nestipy.common.helpers import SpecialProviderExtractor
 from nestipy.core.constant import APP_GUARD
 from nestipy.core.context.execution_context import ExecutionContext
-from nestipy_ioc import NestipyContainer
-from nestipy_metadata import ClassMetadata, Reflect
+from nestipy.ioc import NestipyContainer
+from nestipy.metadata import ClassMetadata, Reflect
 
 
 @Injectable()
 class GuardProcessor(SpecialProviderExtractor):
 
     def __init__(self):
         self.container = NestipyContainer.get_instance()
```

### Comparing `nestipy-0.2.9/src/nestipy/core/instance_loader.py` & `nestipy-0.3.0/src/nestipy/core/instance_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 import typing
 from typing import Type, Any
 
-from nestipy_dynamic_module import DynamicModule, MiddlewareConsumer, NestipyModule
-from nestipy_ioc import NestipyContainer, ModuleProviderDict
-from nestipy_metadata import ModuleMetadata, Reflect
+from nestipy.dynamic_module import DynamicModule, MiddlewareConsumer, NestipyModule
+from nestipy.ioc import NestipyContainer, ModuleProviderDict
+from nestipy.metadata import ModuleMetadata, Reflect
 
 from .discover import DiscoverService
 from .on_destroy import OnDestroy
 from .on_init import OnInit
 from ..graphql.graphql_module import GraphqlModule
```

### Comparing `nestipy-0.2.9/src/nestipy/core/interceptor/processor.py` & `nestipy-0.3.0/src/nestipy/core/interceptor/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import TYPE_CHECKING
 
 from nestipy.common.decorator import Injectable
 from nestipy.common.helpers import SpecialProviderExtractor
 from nestipy.common.interceptor import NestipyInterceptor, InterceptorKey
 from nestipy.core.constant import APP_INTERCEPTOR
 from nestipy.core.context.execution_context import ExecutionContext
-from nestipy_ioc import NestipyContainer
-from nestipy_metadata import ClassMetadata, Reflect
+from nestipy.ioc import NestipyContainer
+from nestipy.metadata import ClassMetadata, Reflect
 
 if TYPE_CHECKING:
     from nestipy.types_.handler import NextFn
 
 
 @Injectable()
 class RequestInterceptor(NestipyInterceptor, SpecialProviderExtractor):
```

### Comparing `nestipy-0.2.9/src/nestipy/core/meta/metadata_creator.py` & `nestipy-0.3.0/src/nestipy/core/meta/metadata_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Type, Union
 
 from nestipy.common.utils import uniq_list
-from nestipy_dynamic_module import DynamicModule
-from nestipy_ioc import NestipyContainer
-from nestipy_metadata import ClassMetadata, ModuleMetadata, Reflect
+from nestipy.dynamic_module import DynamicModule
+from nestipy.ioc import NestipyContainer
+from nestipy.metadata import ClassMetadata, ModuleMetadata, Reflect
 
 
 class MetadataCreator(ABC):
 
     def __init__(self, module, global_data=None, is_root=False):
         self.module = self._dynamic_module_to_module(module)
         self.is_root = is_root
```

### Comparing `nestipy-0.2.9/src/nestipy/core/meta/module_metadata_creator.py` & `nestipy-0.3.0/src/nestipy/core/meta/module_metadata_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type
 
-from nestipy_metadata import ClassMetadata, ModuleMetadata, Reflect
+from nestipy.metadata import ClassMetadata, ModuleMetadata, Reflect
 
 from .metadata_creator import MetadataCreator
 
 
 class ModuleMetadataCreator(MetadataCreator):
     def _extract(self) -> list:
         return Reflect.get_metadata(self.module, ModuleMetadata.Imports, [])
```

### Comparing `nestipy-0.2.9/src/nestipy/core/middleware/executor.py` & `nestipy-0.3.0/src/nestipy/core/middleware/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import logging
 import re
 import traceback
 from typing import Callable, Any
 
-from nestipy_ioc import MiddlewareContainer, MiddlewareProxy
+from nestipy.ioc import MiddlewareContainer, MiddlewareProxy
 
 from nestipy.common.http_ import Request, Response
 from nestipy.common.middleware import NestipyMiddleware
 from nestipy.types_ import HTTPMethod
 
 
 def uniq_middleware_list(data: list[MiddlewareProxy]) -> list:
```

### Comparing `nestipy-0.2.9/src/nestipy/core/nestipy_application.py` & `nestipy-0.3.0/src/nestipy/core/nestipy_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import dataclasses
 import logging
 import os.path
 import traceback
 from typing import Type, Callable, Literal, Union, Any, TYPE_CHECKING
 
-from nestipy_dynamic_module import DynamicModule
-from nestipy_ioc import MiddlewareContainer, MiddlewareProxy, NestipyContainer, ModuleProviderDict
-from nestipy_metadata import ModuleMetadata, Reflect
+from nestipy.dynamic_module import DynamicModule
+from nestipy.ioc import MiddlewareContainer, MiddlewareProxy, NestipyContainer, ModuleProviderDict
+from nestipy.metadata import ModuleMetadata, Reflect
 from openapidocs.v3 import PathItem
 
 from nestipy.common.http_ import Response, Request
 from nestipy.common.middleware import NestipyMiddleware
 from nestipy.common.template import TemplateEngine, TemplateKey
 from nestipy.common.utils import uniq_list
 from nestipy.core.template import MinimalJinjaTemplateEngine
```

### Comparing `nestipy-0.2.9/src/nestipy/core/nestipy_factory.py` & `nestipy-0.3.0/src/nestipy/core/nestipy_factory.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.3.0/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/router/route_explorer.py` & `nestipy-0.3.0/src/nestipy/core/router/route_explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from inspect import isfunction, getmembers
 from typing import List, Type, Union
 
-from nestipy_ioc import MiddlewareContainer
-from nestipy_metadata import ModuleMetadata, Reflect, RouteKey
+from nestipy.ioc import MiddlewareContainer
+from nestipy.metadata import ModuleMetadata, Reflect, RouteKey
 from openapidocs.v3 import Parameter, ParameterLocation
 
 from nestipy.common.utils import deep_merge
 from nestipy.openapi.explorer import OpenApiExplorer
 from .route_extractor import RouteParamsExtractor
```

### Comparing `nestipy-0.2.9/src/nestipy/core/router/router_proxy.py` & `nestipy-0.3.0/src/nestipy/core/router/router_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import dataclasses
+import logging
 import traceback
 import typing
 from typing import Type, Union
 
-from nestipy_ioc import NestipyContainer
-from nestipy_ioc import NestipyContextContainer
-from nestipy_metadata import NestipyContextProperty
 from openapidocs.v3 import Operation, PathItem
 from pydantic import BaseModel
 
 from nestipy.common.exception import HttpException
 from nestipy.common.exception.message import HttpStatusMessages
 from nestipy.common.exception.status import HttpStatus
 from nestipy.common.http_ import Request, Response
 from nestipy.common.utils import snakecase_to_camelcase
 from nestipy.core.exception.processor import ExceptionFilterHandler
 from nestipy.core.guards import GuardProcessor
 from nestipy.core.interceptor import RequestInterceptor
 from nestipy.core.middleware import MiddlewareExecutor
 from nestipy.core.template import TemplateRendererProcessor
+from nestipy.ioc import NestipyContainer
+from nestipy.ioc import RequestContextContainer
+from nestipy.metadata import NestipyContextProperty
 from nestipy.types_ import NextFn, CallableHandler
 from .route_explorer import RouteExplorer
 from ..adapter.http_adapter import HttpAdapter
 from ..context.execution_context import ExecutionContext
 
 
 class RouterProxy:
@@ -56,37 +57,42 @@
                     )
                     json_paths[path] = route_path
         paths = {}
         for path, op in json_paths.items():
             paths[path] = PathItem(**op)
         return paths
 
+    @classmethod
+    async def setup_context_data(cls, context_container: RequestContextContainer, req: "Request", res: "Response"):
+        context_container.set_value(NestipyContextProperty.request, req)
+        context_container.set_value(NestipyContextProperty.response, res)
+        context_container.set_value(NestipyContextProperty.params, req.path_params)
+        context_container.set_value(NestipyContextProperty.query_params, req.query_params)
+        context_container.set_value(NestipyContextProperty.headers, req.headers)
+        context_container.set_value(NestipyContextProperty.session, req.session)
+        context_container.set_value(NestipyContextProperty.cookies, req.cookies)
+        form_data = await req.form()
+        if form_data is not None:
+            context_container.set_value(NestipyContextProperty.body, form_data)
+        else:
+            json_data = await req.json()
+            context_container.set_value(NestipyContextProperty.body, json_data)
+
     def create_request_handler(
             self,
             module_ref: Type,
             controller: Union[object, Type],
             method_name: str
     ) -> CallableHandler:
 
         async def request_handler(req: "Request", res: "Response", next_fn: NextFn):
 
-            context_container = NestipyContextContainer.get_instance()
+            context_container = RequestContextContainer.get_instance()
             # setup container for query params, route params, request, response, session, etc..
-            context_container.set_value(NestipyContextProperty.request, req)
-            context_container.set_value(NestipyContextProperty.response, res)
-            context_container.set_value(NestipyContextProperty.params, req.path_params)
-            context_container.set_value(NestipyContextProperty.query_params, req.query_params)
-            context_container.set_value(NestipyContextProperty.headers, req.headers)
-            form_data = await req.form()
-            if form_data is not None:
-                context_container.set_value(NestipyContextProperty.body, form_data)
-            else:
-                json_data = await req.json()
-                context_container.set_value(NestipyContextProperty.body, json_data)
-
+            await self.setup_context_data(context_container, req, res)
             # TODO: req.files
 
             container = NestipyContainer.get_instance()
             controller_method_handler = getattr(controller, method_name)
             execution_context = ExecutionContext(
                 self.router,
                 module_ref,
@@ -132,27 +138,28 @@
                 # process template rendering
                 if self._template_processor.can_process(controller_method_handler, result):
                     result = await res.html(self._template_processor.render())
                 # transform result to response
                 handler_response = await self._ensure_response(res, result)
 
             except Exception as e:
+                logging.error(e)
                 if not isinstance(e, HttpException):
                     tb = traceback.format_exc()
                     e = HttpException(HttpStatus.INTERNAL_SERVER_ERROR, str(e), str(tb))
 
                 # Call exception catch
                 exception_handler = await container.get(ExceptionFilterHandler)
                 result = await exception_handler.catch(e, execution_context)
                 if result:
                     handler_response = await self._ensure_response(res, result)
                 else:
                     handler_response = await self._ensure_response(res, await next_fn(e))
             finally:
-                #  reset context container
+                #  reset request context container
                 context_container.destroy()
             return handler_response
 
         return request_handler
 
     @classmethod
     async def _ensure_response(cls, res: "Response", result: Union["Response", str, dict, list]) -> "Response":
```

### Comparing `nestipy-0.2.9/src/nestipy/core/template/minimal_jinja.py` & `nestipy-0.3.0/src/nestipy/core/template/minimal_jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/core/template/processor.py` & `nestipy-0.3.0/src/nestipy/core/template/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, Callable, Any, TYPE_CHECKING
 
-from nestipy_metadata import Reflect
+from nestipy.metadata import Reflect
 
 from nestipy.common.template import TemplateEngine, TemplateKey
 from .minimal_jinja import MinimalJinjaTemplateEngine
 
 if TYPE_CHECKING:
     from nestipy.core.adapter.http_adapter import HttpAdapter
```

### Comparing `nestipy-0.2.9/src/nestipy/graphql/decorator.py` & `nestipy-0.3.0/src/nestipy/graphql/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, Union, Callable, Any
 
-from nestipy_metadata import Reflect
+from nestipy.metadata import Reflect
 
 from nestipy.graphql.meta import NestipyGraphqlKey
 
 
 class GraphQlDecorator:
     def __init__(self, graphql_type: str, value: Any = True, is_method: bool = True):
         self.graphql_type = graphql_type
```

### Comparing `nestipy-0.2.9/src/nestipy/graphql/graphql_adapter.py` & `nestipy-0.3.0/src/nestipy/graphql/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/graphql/graphql_asgi.py` & `nestipy-0.3.0/src/nestipy/graphql/graphql_asgi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from abc import abstractmethod
 
 import aiofiles
-from nestipy_ioc import NestipyContextContainer
-from nestipy_metadata import NestipyContextProperty
+from nestipy.ioc import RequestContextContainer
+from nestipy.metadata import NestipyContextProperty
 
 from nestipy.common.http_ import Request
 from nestipy.graphql.graphql_module import GraphqlOption
 
 
 class GraphqlAsgi:
     option: GraphqlOption = None
@@ -29,9 +29,9 @@
     @abstractmethod
     async def handle(self, scope: dict, receive, send):
         self._setup_request(scope, receive, send)
 
     @classmethod
     def _setup_request(cls, scope: dict, receive, send):
         req = Request(scope, receive, send)
-        NestipyContextContainer.get_instance().set_value(NestipyContextProperty.request, req)
+        RequestContextContainer.get_instance().set_value(NestipyContextProperty.request, req)
         pass
```

### Comparing `nestipy-0.2.9/src/nestipy/graphql/graphql_explorer.py` & `nestipy-0.3.0/src/nestipy/graphql/graphql_explorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inspect import getmembers, isfunction
 from typing import Union, Type
 
-from nestipy_metadata import ModuleMetadata, Reflect
+from nestipy.metadata import ModuleMetadata, Reflect
 from nestipy.graphql.meta import NestipyGraphqlKey
 
 
 class GraphqlExplorer:
 
     @classmethod
     def explore(cls, module_ref: Union[Type, object]) -> type[list[dict], list[dict], list[dict]]:
```

### Comparing `nestipy-0.2.9/src/nestipy/graphql/graphql_module.py` & `nestipy-0.3.0/src/nestipy/graphql/graphql_module.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 from typing import Literal
 
 from nestipy.common.decorator import Module
-from nestipy_dynamic_module import ConfigurableModuleBuilder
-from nestipy_ioc import Inject
+from nestipy.dynamic_module import ConfigurableModuleBuilder
+from nestipy.ioc import Inject
 
 
 @dataclasses.dataclass
 class GraphqlOption:
     url: str = '/graphql'
     ide: Literal['default', 'graphiql'] = 'default'
```

### Comparing `nestipy-0.2.9/src/nestipy/graphql/graphql_proxy.py` & `nestipy-0.3.0/src/nestipy/graphql/graphql_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union, Type, Callable
 
 from nestipy.core.guards import GuardProcessor
 from nestipy.graphql.graphql_adapter import GraphqlAdapter
-from nestipy_ioc import NestipyContainer
-from nestipy_ioc import NestipyContextContainer
-from nestipy_metadata import NestipyContextProperty
+from nestipy.ioc import NestipyContainer
+from nestipy.ioc import RequestContextContainer
+from nestipy.metadata import NestipyContextProperty
 
 from .graphql_explorer import GraphqlExplorer
 from .graphql_module import GraphqlModule, GraphqlOption
 from ..common import Request
 from ..core.adapter.http_adapter import HttpAdapter
 from ..core.context.execution_context import ExecutionContext
 
@@ -38,15 +38,15 @@
 
     def _create_graphql_query_handler(self, module_ref: Union[Type, object], meta: dict) -> tuple[str, Type, Callable]:
         resolver: Union[object, Type] = meta['class']
         method_name: str = meta['handler_name']
         method = getattr(resolver, method_name)
 
         async def graphql_handler(*_args, **kwargs):
-            context_container = NestipyContextContainer.get_instance()
+            context_container = RequestContextContainer.get_instance()
             context_container.set_value(NestipyContextProperty.args, kwargs)
             try:
                 # TODO: Refactor with routerProxy
                 # create execution context
                 execution_context = ExecutionContext(
                     self._adapter,
                     module_ref,
```

### Comparing `nestipy-0.2.9/src/nestipy/graphql/playground/graphql-playground-default.html` & `nestipy-0.3.0/src/nestipy/graphql/playground/graphql-playground-default.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/graphql/playground/graphql-playground-graphiql.html` & `nestipy-0.3.0/src/nestipy/graphql/playground/graphql-playground-graphiql.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/graphql/pubsub.py` & `nestipy-0.3.0/src/nestipy/graphql/pubsub.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/graphql/strawberry/__init__.py` & `nestipy-0.3.0/src/nestipy/graphql/strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/graphql/strawberry/strawberry_adapter.py` & `nestipy-0.3.0/src/nestipy/graphql/strawberry/strawberry_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/graphql/strawberry/strawberry_asgi.py` & `nestipy-0.3.0/src/nestipy/graphql/strawberry/strawberry_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/openapi/__init__.py` & `nestipy-0.3.0/src/nestipy/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/openapi/decorator.py` & `nestipy-0.3.0/src/nestipy/openapi/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import dataclasses
 from typing import Union, Optional, Any, Type
 
-from nestipy_metadata import SetMetadata
-from openapidocs.v3 import RequestBody, Response, Parameter
-from openapidocs.v3 import SecurityRequirement, MediaType, Schema
 from pydantic import TypeAdapter, BaseModel
 
+from nestipy.metadata import SetMetadata
+from .openapi_docs.v3 import RequestBody, Response, Parameter
+from .openapi_docs.v3 import SecurityRequirement, MediaType, Schema
+
 
 def ApiBody(body: Union[BaseModel, Type] = None, consumer: str = 'application/json'):
     content: dict = {}
     if dataclasses.is_dataclass(body):
         content: dict = TypeAdapter(body).json_schema()
     elif isinstance(body, BaseModel):
         content: dict = body.model_json_schema()
```

### Comparing `nestipy-0.2.9/src/nestipy/openapi/document_builder.py` & `nestipy-0.3.0/src/nestipy/openapi/document_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from openapidocs.v3 import Info, OpenAPI, Components, SecurityScheme, HTTPSecurity
+from .openapi_docs.v3 import Info, OpenAPI, Components, SecurityScheme, HTTPSecurity
 
 
 class DocumentBuilder:
     _info: dict = {}
     _security_schemes: dict = {}
     _schemas: dict = {}
     _instance: "DocumentBuilder" = None
```

### Comparing `nestipy-0.2.9/src/nestipy/openapi/swagger.html` & `nestipy-0.3.0/src/nestipy/openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/openapi/swagger_module.py` & `nestipy-0.3.0/src/nestipy/openapi/swagger_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import dataclasses
 import os.path
 from typing import TYPE_CHECKING
 
 import aiofiles
-from nestipy_metadata import Reflect
-from openapidocs.common import Serializer
-from openapidocs.v3 import OpenAPI
 
 from nestipy.common.http_ import Request, Response
+from nestipy.metadata import Reflect
 from .constant import OPENAPI_HANDLER_METADATA
+from .openapi_docs.common import Serializer
+from .openapi_docs.v3 import OpenAPI
 
 if TYPE_CHECKING:
     from ..core.nestipy_application import NestipyApplication
 
 
 @dataclasses.dataclass
 class _Document:
```

### Comparing `nestipy-0.2.9/src/nestipy/openapi/test.py` & `nestipy-0.3.0/src/nestipy/openapi/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import json
-
-from openapidocs.v3 import OpenAPI, Info, Response, Components, Schema, SecuritySchemeType
-from openapidocs.v3 import PathItem, Operation, SecurityRequirement, ValueType, SecurityScheme
-from openapidocs.v3 import Tag, HTTPSecurity, APIKeySecurity, ParameterLocation, Parameter
-from openapidocs.common import Serializer
-from dataclasses import asdict
+from .openapi_docs.common import Serializer
+from .openapi_docs.v3 import OpenAPI, Info, Response, Components, Schema, SecuritySchemeType
+from .openapi_docs.v3 import PathItem, Operation, SecurityRequirement, ValueType
+from .openapi_docs.v3 import Tag, HTTPSecurity, APIKeySecurity, ParameterLocation, Parameter
 
 open_api = OpenAPI(
     info=Info(
         title='Test openapi',
         description='This is the description',
         version='v1'
     ),
```

### Comparing `nestipy-0.2.9/src/nestipy/websocket/adapter.py` & `nestipy-0.3.0/src/nestipy/websocket/adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.9/src/nestipy/websocket/decorator.py` & `nestipy-0.3.0/src/nestipy/websocket/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Type
 
 from nestipy.common.decorator import Injectable
-from nestipy_metadata import SetMetadata
+from nestipy.metadata import SetMetadata
 
 GATEWAY_KEY = '__GATEWAY__'
 EVENT_KEY = '__GATEWAY_EVENT__'
 SUCCESS_EVENT_KEY = '__GATEWAY_SUCCESS_EVENT__'
 ERROR_EVENT_KEY = '__GATEWAY_ERROR_EVENT__'
```

### Comparing `nestipy-0.2.9/src/nestipy/websocket/proxy.py` & `nestipy-0.3.0/src/nestipy/websocket/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from typing import Type, Union, Callable, Any, TYPE_CHECKING
 
-from nestipy_ioc import NestipyContainer
-from nestipy_ioc import NestipyContextContainer
-from nestipy_metadata import NestipyContextProperty, Reflect, ModuleMetadata
+from nestipy.ioc import NestipyContainer
+from nestipy.ioc import RequestContextContainer
+from nestipy.metadata import NestipyContextProperty, Reflect, ModuleMetadata
 
 from .decorator import GATEWAY_KEY, EVENT_KEY, SUCCESS_EVENT_KEY, ERROR_EVENT_KEY
 from ..core.context.execution_context import ExecutionContext
 
 if TYPE_CHECKING:
     from ..core.adapter.http_adapter import HttpAdapter
 
@@ -57,15 +57,15 @@
             gateway: Type,
             method_name: str,
             namespace: str,
             event_name: Any
     ) -> Callable[..., Any]:
         async def io_handler(sid: Any, data: Any):
             io_adapter = self.adapter.get_io_adapter()
-            context_container = NestipyContextContainer.get_instance()
+            context_container = RequestContextContainer.get_instance()
             context_container.set_value(NestipyContextProperty.io_client, sid)
             context_container.set_value(NestipyContextProperty.io_data, data)
             context_container.set_value(NestipyContextProperty.io_server, io_adapter)
 
             container = NestipyContainer.get_instance()
             gateway_method = getattr(gateway, method_name)
             execution_context = ExecutionContext(
```

### Comparing `nestipy-0.2.9/PKG-INFO` & `nestipy-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.2.9
+Version: 0.3.0
 Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: minijinja (>=2.0.1,<3.0.0)
-Requires-Dist: nestipy-dynamic-module (==0.1.7)
-Requires-Dist: nestipy-ioc (>=0.1.31,<0.2.0)
-Requires-Dist: nestipy-metadata (>=0.1.1,<0.2.0)
 Requires-Dist: pyee (>=11.1.0,<12.0.0)
 Requires-Dist: python-socketio (>=5.11.1,<6.0.0)
 Requires-Dist: snakecase (>=1.0.1,<2.0.0)
 Requires-Dist: strawberry-graphql (>=0.225.0,<0.226.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,22 +1,20 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.2.9 Summary: Nestipy is a Python
+Metadata-Version: 2.1 Name: nestipy Version: 0.3.0 Summary: Nestipy is a Python
 framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: minijinja
-(>=2.0.1,<3.0.0) Requires-Dist: nestipy-dynamic-module (==0.1.7) Requires-Dist:
-nestipy-ioc (>=0.1.31,<0.2.0) Requires-Dist: nestipy-metadata (>=0.1.1,<0.2.0)
-Requires-Dist: pyee (>=11.1.0,<12.0.0) Requires-Dist: python-socketio
-(>=5.11.1,<6.0.0) Requires-Dist: snakecase (>=1.0.1,<2.0.0) Requires-Dist:
-strawberry-graphql (>=0.225.0,<0.226.0) Requires-Dist: ujson (>=5.9.0,<6.0.0)
-Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0) Description-Content-Type:
-text/markdown
+(>=2.0.1,<3.0.0) Requires-Dist: pyee (>=11.1.0,<12.0.0) Requires-Dist: python-
+socketio (>=5.11.1,<6.0.0) Requires-Dist: snakecase (>=1.0.1,<2.0.0) Requires-
+Dist: strawberry-graphql (>=0.225.0,<0.226.0) Requires-Dist: ujson
+(>=5.9.0,<6.0.0) Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
+Description-Content-Type: text/markdown
                                 [Nestipy Logo]
                           _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_L_i_c_e_n_s_e_]
 ## Description
 Nestipy is a Python framework built on top of FastAPI that follows the modular
 architecture of NestJS
 Under the hood, Nestipy makes use of _F_a_s_t_A_P_I, but also provides compatibility
 with a wide range of other libraries, like _B_l_a_c_k_s_h_e_e_p, allowing for easy use of
```

