# Comparing `tmp/kui-1.7.3.tar.gz` & `tmp/kui-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kui-1.7.3.tar", last modified: Fri Mar 29 08:20:17 2024, max compression
+gzip compressed data, was "kui-1.7.4.tar", last modified: Tue Apr 30 07:28:07 2024, max compression
```

## Comparing `kui-1.7.3.tar` & `kui-1.7.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0    11341 2024-03-29 08:19:57.865121 kui-1.7.3/LICENSE
--rw-r--r--   0        0        0      440 2024-03-29 08:19:57.865121 kui-1.7.3/README.md
--rw-r--r--   0        0        0        0 2024-03-29 08:19:57.865121 kui-1.7.3/kui/__init__.py
--rw-r--r--   0        0        0       63 2024-03-29 08:19:57.865121 kui-1.7.3/kui/__version__.py
--rw-r--r--   0        0        0     1718 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/__init__.py
--rw-r--r--   0        0        0     7401 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/applications.py
--rw-r--r--   0        0        0     2054 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/cors.py
--rw-r--r--   0        0        0     2382 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/exceptions.py
--rw-r--r--   0        0        0     2439 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/lifespan.py
--rw-r--r--   0        0        0     1470 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/openapi.py
--rw-r--r--   0        0        0     5230 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/parameters.py
--rw-r--r--   0        0        0     3756 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/requests.py
--rw-r--r--   0        0        0     2879 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/responses.py
--rw-r--r--   0        0        0      972 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/routing.py
--rw-r--r--   0        0        0     3177 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/templates.py
--rw-r--r--   0        0        0     4637 2024-03-29 08:19:57.865121 kui-1.7.3/kui/asgi/views.py
--rw-r--r--   0        0        0      304 2024-03-29 08:19:57.865121 kui-1.7.3/kui/cors.py
--rw-r--r--   0        0        0     3794 2024-03-29 08:19:57.865121 kui-1.7.3/kui/exceptions.py
--rw-r--r--   0        0        0      123 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/__init__.py
--rw-r--r--   0        0        0     9484 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/application.py
--rw-r--r--   0        0        0     1565 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/extra_docs.py
--rw-r--r--   0        0        0     1618 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/schema.py
--rw-r--r--   0        0        0     7726 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/specification.py
--rw-r--r--   0        0        0      224 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/templates/rapidoc.html
--rw-r--r--   0        0        0      743 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/templates/redoc.html
--rw-r--r--   0        0        0     1522 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/templates/swagger.html
--rw-r--r--   0        0        0     2061 2024-03-29 08:19:57.865121 kui-1.7.3/kui/openapi/types.py
--rw-r--r--   0        0        0    14959 2024-03-29 08:19:57.865121 kui-1.7.3/kui/parameters/__init__.py
--rw-r--r--   0        0        0     6775 2024-03-29 08:19:57.865121 kui-1.7.3/kui/parameters/field_functions.py
--rw-r--r--   0        0        0      960 2024-03-29 08:19:57.865121 kui-1.7.3/kui/parameters/fields.py
--rw-r--r--   0        0        0        0 2024-03-29 08:19:57.865121 kui-1.7.3/kui/py.typed
--rw-r--r--   0        0        0     2130 2024-03-29 08:19:57.869121 kui-1.7.3/kui/pydantic_compatible.py
--rw-r--r--   0        0        0     8449 2024-03-29 08:19:57.869121 kui-1.7.3/kui/responses.py
--rw-r--r--   0        0        0      429 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/__init__.py
--rw-r--r--   0        0        0       82 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/__main__.py
--rw-r--r--   0        0        0     1402 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/commands.py
--rw-r--r--   0        0        0      130 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/extensions/__init__.py
--rw-r--r--   0        0        0     2551 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/extensions/file.py
--rw-r--r--   0        0        0     3025 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/extensions/multimethod.py
--rw-r--r--   0        0        0    17666 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/routers.py
--rw-r--r--   0        0        0     3364 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/routes.py
--rw-r--r--   0        0        0     6234 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/tree.py
--rw-r--r--   0        0        0      439 2024-03-29 08:19:57.869121 kui-1.7.3/kui/routing/typing.py
--rw-r--r--   0        0        0     4075 2024-03-29 08:19:57.869121 kui-1.7.3/kui/security.py
--rw-r--r--   0        0        0     2783 2024-03-29 08:19:57.869121 kui-1.7.3/kui/status.py
--rw-r--r--   0        0        0     1250 2024-03-29 08:19:57.869121 kui-1.7.3/kui/templates.py
--rw-r--r--   0        0        0      757 2024-03-29 08:19:57.869121 kui-1.7.3/kui/utils/__init__.py
--rw-r--r--   0        0        0      856 2024-03-29 08:19:57.869121 kui-1.7.3/kui/utils/contextvars.py
--rw-r--r--   0        0        0      902 2024-03-29 08:19:57.869121 kui-1.7.3/kui/utils/importer.py
--rw-r--r--   0        0        0     1907 2024-03-29 08:19:57.869121 kui-1.7.3/kui/utils/inspect.py
--rw-r--r--   0        0        0     1647 2024-03-29 08:19:57.869121 kui-1.7.3/kui/utils/objects.py
--rw-r--r--   0        0        0      530 2024-03-29 08:19:57.869121 kui-1.7.3/kui/utils/pipe.py
--rw-r--r--   0        0        0     1139 2024-03-29 08:19:57.869121 kui-1.7.3/kui/utils/state.py
--rw-r--r--   0        0        0     1567 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/__init__.py
--rw-r--r--   0        0        0     5872 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/applications.py
--rw-r--r--   0        0        0     2031 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/cors.py
--rw-r--r--   0        0        0     2325 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/exceptions.py
--rw-r--r--   0        0        0     1428 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/openapi.py
--rw-r--r--   0        0        0     3932 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/parameters.py
--rw-r--r--   0        0        0     1835 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/requests.py
--rw-r--r--   0        0        0     2879 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/responses.py
--rw-r--r--   0        0        0      966 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/routing.py
--rw-r--r--   0        0        0     2884 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/templates.py
--rw-r--r--   0        0        0     2229 2024-03-29 08:19:57.869121 kui-1.7.3/kui/wsgi/views.py
--rw-r--r--   0        0        0     1962 2024-03-29 08:19:57.869121 kui-1.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 08:19:57.869121 kui-1.7.3/tests/asgi/__init__.py
--rw-r--r--   0        0        0     2416 2024-03-29 08:19:57.869121 kui-1.7.3/tests/asgi/test_application.py
--rw-r--r--   0        0        0     1338 2024-03-29 08:19:57.869121 kui-1.7.3/tests/asgi/test_cors.py
--rw-r--r--   0        0        0      506 2024-03-29 08:19:57.869121 kui-1.7.3/tests/asgi/test_lifespan.py
--rw-r--r--   0        0        0     7718 2024-03-29 08:19:57.869121 kui-1.7.3/tests/asgi/test_parameters.py
--rw-r--r--   0        0        0      838 2024-03-29 08:19:57.869121 kui-1.7.3/tests/asgi/test_response_convertors.py
--rw-r--r--   0        0        0     1318 2024-03-29 08:19:57.869121 kui-1.7.3/tests/asgi/test_views.py
--rw-r--r--   0        0        0    35105 2024-03-29 08:19:57.869121 kui-1.7.3/tests/openapi/test_application.py
--rw-r--r--   0        0        0      429 2024-03-29 08:19:57.869121 kui-1.7.3/tests/openapi/test_extra_docs.py
--rw-r--r--   0        0        0      247 2024-03-29 08:19:57.869121 kui-1.7.3/tests/routing/extensions/test_fileroutes.py
--rw-r--r--   0        0        0     3342 2024-03-29 08:19:57.869121 kui-1.7.3/tests/routing/extensions/test_multimethod.py
--rw-r--r--   0        0        0       88 2024-03-29 08:19:57.869121 kui-1.7.3/tests/routing/test_commands.py
--rw-r--r--   0        0        0     4559 2024-03-29 08:19:57.869121 kui-1.7.3/tests/routing/test_routes.py
--rw-r--r--   0        0        0     2444 2024-03-29 08:19:57.869121 kui-1.7.3/tests/routing/test_tree.py
--rw-r--r--   0        0        0      242 2024-03-29 08:19:57.869121 kui-1.7.3/tests/test_export_all.py
--rw-r--r--   0        0        0     4505 2024-03-29 08:19:57.869121 kui-1.7.3/tests/test_responses.py
--rw-r--r--   0        0        0     3032 2024-03-29 08:19:57.869121 kui-1.7.3/tests/test_security.py
--rw-r--r--   0        0        0        0 2024-03-29 08:19:57.869121 kui-1.7.3/tests/utils/__init__.py
--rw-r--r--   0        0        0      671 2024-03-29 08:19:57.869121 kui-1.7.3/tests/utils/test_importer.py
--rw-r--r--   0        0        0      170 2024-03-29 08:19:57.869121 kui-1.7.3/tests/utils/test_objects.py
--rw-r--r--   0        0        0      426 2024-03-29 08:19:57.869121 kui-1.7.3/tests/utils/test_state.py
--rw-r--r--   0        0        0     1290 2024-03-29 08:19:57.869121 kui-1.7.3/tests/wsgi/test_cors.py
--rw-r--r--   0        0        0     7125 2024-03-29 08:19:57.869121 kui-1.7.3/tests/wsgi/test_parameters.py
--rw-r--r--   0        0        0      783 2024-03-29 08:19:57.869121 kui-1.7.3/tests/wsgi/test_response_convertors.py
--rw-r--r--   0        0        0      453 2024-03-29 08:19:57.869121 kui-1.7.3/tests/wsgi/test_views.py
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 kui-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-04-30 07:27:51.401015 kui-1.7.4/LICENSE
+-rw-r--r--   0        0        0      313 2024-04-30 07:27:51.401015 kui-1.7.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 07:27:51.405015 kui-1.7.4/kui/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-30 07:27:51.405015 kui-1.7.4/kui/__version__.py
+-rw-r--r--   0        0        0     1718 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/__init__.py
+-rw-r--r--   0        0        0     7401 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/applications.py
+-rw-r--r--   0        0        0     2054 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/cors.py
+-rw-r--r--   0        0        0     2382 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/exceptions.py
+-rw-r--r--   0        0        0     2439 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/lifespan.py
+-rw-r--r--   0        0        0     1470 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/openapi.py
+-rw-r--r--   0        0        0     5230 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/parameters.py
+-rw-r--r--   0        0        0     3756 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/requests.py
+-rw-r--r--   0        0        0     2879 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/responses.py
+-rw-r--r--   0        0        0      972 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/routing.py
+-rw-r--r--   0        0        0     3177 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/templates.py
+-rw-r--r--   0        0        0     4637 2024-04-30 07:27:51.405015 kui-1.7.4/kui/asgi/views.py
+-rw-r--r--   0        0        0      304 2024-04-30 07:27:51.405015 kui-1.7.4/kui/cors.py
+-rw-r--r--   0        0        0     3794 2024-04-30 07:27:51.405015 kui-1.7.4/kui/exceptions.py
+-rw-r--r--   0        0        0      123 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/__init__.py
+-rw-r--r--   0        0        0     9484 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/application.py
+-rw-r--r--   0        0        0     1565 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/extra_docs.py
+-rw-r--r--   0        0        0     1618 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/schema.py
+-rw-r--r--   0        0        0     7726 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/specification.py
+-rw-r--r--   0        0        0      224 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/templates/rapidoc.html
+-rw-r--r--   0        0        0      743 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/templates/redoc.html
+-rw-r--r--   0        0        0     1522 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/templates/swagger.html
+-rw-r--r--   0        0        0     2061 2024-04-30 07:27:51.405015 kui-1.7.4/kui/openapi/types.py
+-rw-r--r--   0        0        0    14959 2024-04-30 07:27:51.405015 kui-1.7.4/kui/parameters/__init__.py
+-rw-r--r--   0        0        0     6295 2024-04-30 07:27:51.405015 kui-1.7.4/kui/parameters/field_functions.py
+-rw-r--r--   0        0        0      960 2024-04-30 07:27:51.405015 kui-1.7.4/kui/parameters/fields.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:27:51.405015 kui-1.7.4/kui/py.typed
+-rw-r--r--   0        0        0     2130 2024-04-30 07:27:51.405015 kui-1.7.4/kui/pydantic_compatible.py
+-rw-r--r--   0        0        0     8455 2024-04-30 07:27:51.405015 kui-1.7.4/kui/responses.py
+-rw-r--r--   0        0        0      429 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/__init__.py
+-rw-r--r--   0        0        0       82 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/__main__.py
+-rw-r--r--   0        0        0     1402 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/commands.py
+-rw-r--r--   0        0        0      130 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/extensions/__init__.py
+-rw-r--r--   0        0        0     2551 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/extensions/file.py
+-rw-r--r--   0        0        0     3025 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/extensions/multimethod.py
+-rw-r--r--   0        0        0    17666 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/routers.py
+-rw-r--r--   0        0        0     3364 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/routes.py
+-rw-r--r--   0        0        0     6234 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/tree.py
+-rw-r--r--   0        0        0      439 2024-04-30 07:27:51.405015 kui-1.7.4/kui/routing/typing.py
+-rw-r--r--   0        0        0     4075 2024-04-30 07:27:51.405015 kui-1.7.4/kui/security.py
+-rw-r--r--   0        0        0     2783 2024-04-30 07:27:51.405015 kui-1.7.4/kui/status.py
+-rw-r--r--   0        0        0     1250 2024-04-30 07:27:51.405015 kui-1.7.4/kui/templates.py
+-rw-r--r--   0        0        0      757 2024-04-30 07:27:51.405015 kui-1.7.4/kui/utils/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-30 07:27:51.405015 kui-1.7.4/kui/utils/contextvars.py
+-rw-r--r--   0        0        0      902 2024-04-30 07:27:51.405015 kui-1.7.4/kui/utils/importer.py
+-rw-r--r--   0        0        0     1907 2024-04-30 07:27:51.405015 kui-1.7.4/kui/utils/inspect.py
+-rw-r--r--   0        0        0     1647 2024-04-30 07:27:51.405015 kui-1.7.4/kui/utils/objects.py
+-rw-r--r--   0        0        0      530 2024-04-30 07:27:51.409015 kui-1.7.4/kui/utils/pipe.py
+-rw-r--r--   0        0        0     1139 2024-04-30 07:27:51.409015 kui-1.7.4/kui/utils/state.py
+-rw-r--r--   0        0        0     1567 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/__init__.py
+-rw-r--r--   0        0        0     5872 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/applications.py
+-rw-r--r--   0        0        0     2031 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/cors.py
+-rw-r--r--   0        0        0     2325 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/exceptions.py
+-rw-r--r--   0        0        0     1428 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/openapi.py
+-rw-r--r--   0        0        0     3932 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/parameters.py
+-rw-r--r--   0        0        0     1835 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/requests.py
+-rw-r--r--   0        0        0     2879 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/responses.py
+-rw-r--r--   0        0        0      966 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/routing.py
+-rw-r--r--   0        0        0     2884 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/templates.py
+-rw-r--r--   0        0        0     2229 2024-04-30 07:27:51.409015 kui-1.7.4/kui/wsgi/views.py
+-rw-r--r--   0        0        0     1962 2024-04-30 07:27:51.409015 kui-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 07:27:51.409015 kui-1.7.4/tests/asgi/__init__.py
+-rw-r--r--   0        0        0     2416 2024-04-30 07:27:51.409015 kui-1.7.4/tests/asgi/test_application.py
+-rw-r--r--   0        0        0     1338 2024-04-30 07:27:51.409015 kui-1.7.4/tests/asgi/test_cors.py
+-rw-r--r--   0        0        0      506 2024-04-30 07:27:51.409015 kui-1.7.4/tests/asgi/test_lifespan.py
+-rw-r--r--   0        0        0     7718 2024-04-30 07:27:51.409015 kui-1.7.4/tests/asgi/test_parameters.py
+-rw-r--r--   0        0        0      838 2024-04-30 07:27:51.409015 kui-1.7.4/tests/asgi/test_response_convertors.py
+-rw-r--r--   0        0        0     1318 2024-04-30 07:27:51.409015 kui-1.7.4/tests/asgi/test_views.py
+-rw-r--r--   0        0        0    35105 2024-04-30 07:27:51.409015 kui-1.7.4/tests/openapi/test_application.py
+-rw-r--r--   0        0        0      429 2024-04-30 07:27:51.409015 kui-1.7.4/tests/openapi/test_extra_docs.py
+-rw-r--r--   0        0        0      247 2024-04-30 07:27:51.409015 kui-1.7.4/tests/routing/extensions/test_fileroutes.py
+-rw-r--r--   0        0        0     3342 2024-04-30 07:27:51.409015 kui-1.7.4/tests/routing/extensions/test_multimethod.py
+-rw-r--r--   0        0        0       88 2024-04-30 07:27:51.409015 kui-1.7.4/tests/routing/test_commands.py
+-rw-r--r--   0        0        0     4559 2024-04-30 07:27:51.409015 kui-1.7.4/tests/routing/test_routes.py
+-rw-r--r--   0        0        0     2444 2024-04-30 07:27:51.409015 kui-1.7.4/tests/routing/test_tree.py
+-rw-r--r--   0        0        0      242 2024-04-30 07:27:51.409015 kui-1.7.4/tests/test_export_all.py
+-rw-r--r--   0        0        0     4505 2024-04-30 07:27:51.409015 kui-1.7.4/tests/test_responses.py
+-rw-r--r--   0        0        0     3032 2024-04-30 07:27:51.409015 kui-1.7.4/tests/test_security.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:27:51.409015 kui-1.7.4/tests/utils/__init__.py
+-rw-r--r--   0        0        0      671 2024-04-30 07:27:51.409015 kui-1.7.4/tests/utils/test_importer.py
+-rw-r--r--   0        0        0      170 2024-04-30 07:27:51.409015 kui-1.7.4/tests/utils/test_objects.py
+-rw-r--r--   0        0        0      426 2024-04-30 07:27:51.409015 kui-1.7.4/tests/utils/test_state.py
+-rw-r--r--   0        0        0     1290 2024-04-30 07:27:51.409015 kui-1.7.4/tests/wsgi/test_cors.py
+-rw-r--r--   0        0        0     7125 2024-04-30 07:27:51.409015 kui-1.7.4/tests/wsgi/test_parameters.py
+-rw-r--r--   0        0        0      783 2024-04-30 07:27:51.409015 kui-1.7.4/tests/wsgi/test_response_convertors.py
+-rw-r--r--   0        0        0      453 2024-04-30 07:27:51.409015 kui-1.7.4/tests/wsgi/test_views.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 kui-1.7.4/PKG-INFO
```

### Comparing `kui-1.7.3/LICENSE` & `kui-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/__init__.py` & `kui-1.7.4/kui/asgi/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/applications.py` & `kui-1.7.4/kui/asgi/applications.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/cors.py` & `kui-1.7.4/kui/asgi/cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/exceptions.py` & `kui-1.7.4/kui/asgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/lifespan.py` & `kui-1.7.4/kui/asgi/lifespan.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/openapi.py` & `kui-1.7.4/kui/asgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/parameters.py` & `kui-1.7.4/kui/asgi/parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/requests.py` & `kui-1.7.4/kui/asgi/requests.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/responses.py` & `kui-1.7.4/kui/asgi/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/routing.py` & `kui-1.7.4/kui/asgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/templates.py` & `kui-1.7.4/kui/asgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/asgi/views.py` & `kui-1.7.4/kui/asgi/views.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/exceptions.py` & `kui-1.7.4/kui/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/openapi/application.py` & `kui-1.7.4/kui/openapi/application.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/openapi/extra_docs.py` & `kui-1.7.4/kui/openapi/extra_docs.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/openapi/schema.py` & `kui-1.7.4/kui/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/openapi/specification.py` & `kui-1.7.4/kui/openapi/specification.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/openapi/templates/redoc.html` & `kui-1.7.4/kui/openapi/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/openapi/templates/swagger.html` & `kui-1.7.4/kui/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/openapi/types.py` & `kui-1.7.4/kui/openapi/types.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/parameters/__init__.py` & `kui-1.7.4/kui/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/parameters/field_functions.py` & `kui-1.7.4/kui/parameters/field_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,141 +15,133 @@
 def Path(
     default: Any = Undefined,
     *,
     default_factory: Optional[Callable[[], Any]] = None,
     alias: str | None = None,
     title: str | None = None,
     description: str | None = None,
-    exclusive: bool = False,
     **extra: Any,
 ) -> Any:
     """
     Used to provide extra information about a field.
 
     :param default: since this is replacing the field’s default, its first argument is used
       to set the default, use ellipsis (``...``) to indicate the field is required
     :param default_factory: callable that will be called when a default value is needed for this field
       If both `default` and `default_factory` are set, an error is raised.
     :param alias: the public name of the field
     :param title: can be any string, used in the schema
     :param description: can be any string, used in the schema
-    :param exclusive: decide whether this field receives all parameters
     :param **extra: any pydantic field kwargs
     """
     field_info = Field(
         default,
         default_factory=default_factory,
         alias=alias,
         title=title,
         description=description,
         **extra,
     )
-    return Annotated[Any, field_info, InPath(exclusive=exclusive)]
+    return Annotated[Any, field_info, InPath()]
 
 
 def Query(
     default: Any = Undefined,
     *,
     default_factory: Optional[Callable[[], Any]] = None,
     alias: str | None = None,
     title: str | None = None,
     description: str | None = None,
-    exclusive: bool = False,
     **extra: Any,
 ) -> Any:
     """
     Used to provide extra information about a field.
 
     :param default: since this is replacing the field’s default, its first argument is used
       to set the default, use ellipsis (``...``) to indicate the field is required
     :param default_factory: callable that will be called when a default value is needed for this field
       If both `default` and `default_factory` are set, an error is raised.
     :param alias: the public name of the field
     :param title: can be any string, used in the schema
     :param description: can be any string, used in the schema
-    :param exclusive: decide whether this field receives all parameters
     :param **extra: any pydantic field kwargs
     """
     field_info = Field(
         default,
         default_factory=default_factory,
         alias=alias,
         title=title,
         description=description,
         **extra,
     )
-    return Annotated[Any, field_info, InQuery(exclusive=exclusive)]
+    return Annotated[Any, field_info, InQuery()]
 
 
 def Header(
     default: Any = Undefined,
     *,
     default_factory: Optional[Callable[[], Any]] = None,
     alias: str | None = None,
     title: str | None = None,
     description: str | None = None,
-    exclusive: bool = False,
     **extra: Any,
 ) -> Any:
     """
     Used to provide extra information about a field.
 
     :param default: since this is replacing the field’s default, its first argument is used
       to set the default, use ellipsis (``...``) to indicate the field is required
     :param default_factory: callable that will be called when a default value is needed for this field
       If both `default` and `default_factory` are set, an error is raised.
     :param alias: the public name of the field
     :param title: can be any string, used in the schema
     :param description: can be any string, used in the schema
-    :param exclusive: decide whether this field receives all parameters
     :param **extra: any pydantic field kwargs
     """
     field_info = Field(
         default,
         default_factory=default_factory,
         alias=alias.lower() if alias else None,
         title=title,
         description=description,
         **extra,
     )
-    return Annotated[Any, field_info, InHeader(exclusive=exclusive)]
+    return Annotated[Any, field_info, InHeader()]
 
 
 def Cookie(
     default: Any = Undefined,
     *,
     default_factory: Optional[Callable[[], Any]] = None,
     alias: str | None = None,
     title: str | None = None,
     description: str | None = None,
-    exclusive: bool = False,
     **extra: Any,
 ) -> Any:
     """
     Used to provide extra information about a field.
 
     :param default: since this is replacing the field’s default, its first argument is used
       to set the default, use ellipsis (``...``) to indicate the field is required
     :param default_factory: callable that will be called when a default value is needed for this field
       If both `default` and `default_factory` are set, an error is raised.
     :param alias: the public name of the field
     :param title: can be any string, used in the schema
     :param description: can be any string, used in the schema
-    :param exclusive: decide whether this field receives all parameters
     :param **extra: any pydantic field kwargs
     """
     field_info = Field(
         default,
         default_factory=default_factory,
         alias=alias,
         title=title,
         description=description,
         **extra,
     )
-    return Annotated[Any, field_info, InCookie(exclusive=exclusive)]
+    return Annotated[Any, field_info, InCookie()]
 
 
 def Body(
     default: Any = Undefined,
     *,
     default_factory: Optional[Callable[[], Any]] = None,
     alias: str | None = None,
```

### Comparing `kui-1.7.3/kui/parameters/fields.py` & `kui-1.7.4/kui/parameters/fields.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/pydantic_compatible.py` & `kui-1.7.4/kui/pydantic_compatible.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/responses.py` & `kui-1.7.4/kui/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class JSONResponseDocsMetaclass(abc.ABCMeta):
     def __getitem__(
         cls,
         parameters: typing.Tuple[
             int,
             typing.Dict[str, spec.Header | spec.Reference],
-            typing.Type[BaseModel] | spec.Schema | type,
+            typing.Type[BaseModel] | spec.Schema | typing.Any,
         ]
         | typing.Tuple[int, typing.Dict[str, spec.Header | spec.Reference]]
         | int,
     ) -> spec.Responses:
         """
         Use JSONResponse[status, headers, content] to describe response
         """
```

### Comparing `kui-1.7.3/kui/routing/commands.py` & `kui-1.7.4/kui/routing/commands.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/routing/extensions/file.py` & `kui-1.7.4/kui/routing/extensions/file.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/routing/extensions/multimethod.py` & `kui-1.7.4/kui/routing/extensions/multimethod.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/routing/routers.py` & `kui-1.7.4/kui/routing/routers.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/routing/routes.py` & `kui-1.7.4/kui/routing/routes.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/routing/tree.py` & `kui-1.7.4/kui/routing/tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/security.py` & `kui-1.7.4/kui/security.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/status.py` & `kui-1.7.4/kui/status.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/templates.py` & `kui-1.7.4/kui/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/utils/__init__.py` & `kui-1.7.4/kui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/utils/contextvars.py` & `kui-1.7.4/kui/utils/contextvars.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/utils/importer.py` & `kui-1.7.4/kui/utils/importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/utils/inspect.py` & `kui-1.7.4/kui/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/utils/objects.py` & `kui-1.7.4/kui/utils/objects.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/utils/pipe.py` & `kui-1.7.4/kui/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/utils/state.py` & `kui-1.7.4/kui/utils/state.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/__init__.py` & `kui-1.7.4/kui/wsgi/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/applications.py` & `kui-1.7.4/kui/wsgi/applications.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/cors.py` & `kui-1.7.4/kui/wsgi/cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/exceptions.py` & `kui-1.7.4/kui/wsgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/openapi.py` & `kui-1.7.4/kui/wsgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/parameters.py` & `kui-1.7.4/kui/wsgi/parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/requests.py` & `kui-1.7.4/kui/wsgi/requests.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/responses.py` & `kui-1.7.4/kui/wsgi/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/routing.py` & `kui-1.7.4/kui/wsgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/templates.py` & `kui-1.7.4/kui/wsgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/kui/wsgi/views.py` & `kui-1.7.4/kui/wsgi/views.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/pyproject.toml` & `kui-1.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kui"
-version = "1.7.3"
+version = "1.7.4"
 description = "An easy-to-use web framework."
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "baize<0.21.0,>=0.20.0",
     "pydantic>=1.10",
```

### Comparing `kui-1.7.3/tests/asgi/test_application.py` & `kui-1.7.4/tests/asgi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/asgi/test_cors.py` & `kui-1.7.4/tests/asgi/test_cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/asgi/test_parameters.py` & `kui-1.7.4/tests/asgi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/asgi/test_response_convertors.py` & `kui-1.7.4/tests/asgi/test_response_convertors.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/asgi/test_views.py` & `kui-1.7.4/tests/asgi/test_views.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/openapi/test_application.py` & `kui-1.7.4/tests/openapi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/routing/extensions/test_multimethod.py` & `kui-1.7.4/tests/routing/extensions/test_multimethod.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/routing/test_routes.py` & `kui-1.7.4/tests/routing/test_routes.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/routing/test_tree.py` & `kui-1.7.4/tests/routing/test_tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/test_responses.py` & `kui-1.7.4/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/test_security.py` & `kui-1.7.4/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/utils/test_importer.py` & `kui-1.7.4/tests/utils/test_importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/wsgi/test_cors.py` & `kui-1.7.4/tests/wsgi/test_cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/wsgi/test_parameters.py` & `kui-1.7.4/tests/wsgi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/tests/wsgi/test_response_convertors.py` & `kui-1.7.4/tests/wsgi/test_response_convertors.py`

 * *Files identical despite different names*

### Comparing `kui-1.7.3/PKG-INFO` & `kui-1.7.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: kui
-Version: 1.7.3
+Version: 1.7.4
 Summary: An easy-to-use web framework.
 License: Apache-2.0
 Author-email: abersheeran <me@abersheeran.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Project-URL: documentation, https://kui.aber.sh
 Project-URL: homepage, https://github.com/abersheeran/kui
 Project-URL: repository, https://github.com/abersheeran/kui
 Description-Content-Type: text/markdown
 
 # Kuí
 
-[![Codecov](https://img.shields.io/codecov/c/github/abersheeran/kui?style=flat-square)](https://codecov.io/gh/abersheeran/kui)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kui?label=Support%20Python%20Version&style=flat-square)](https://pypi.org/project/kui/)
 
 An easy-to-use web framework. Based on [baize](https://baize.aber.sh) and [pydantic](https://docs.pydantic.dev/).
 
 ## Install
 
 ```
```

