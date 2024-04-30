# Comparing `tmp/djangorestframework-stubs-3.14.5.tar.gz` & `tmp/djangorestframework_stubs-3.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-stubs-3.14.5.tar", last modified: Tue Dec  5 19:21:07 2023, max compression
+gzip compressed data, was "djangorestframework_stubs-3.15.0.tar", last modified: Tue Apr 30 19:56:36 2024, max compression
```

## Comparing `djangorestframework-stubs-3.14.5.tar` & `djangorestframework_stubs-3.15.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.894677 djangorestframework-stubs-3.14.5/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/LICENSE.txt
--rw-r--r--   0 marti     (1000) marti      (121)     3529 2023-12-05 19:21:07.894677 djangorestframework-stubs-3.14.5/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     2113 2023-10-04 20:46:18.000000 djangorestframework-stubs-3.14.5/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.894677 djangorestframework-stubs-3.14.5/djangorestframework_stubs.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)     3529 2023-12-05 19:21:07.000000 djangorestframework-stubs-3.14.5/djangorestframework_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     3237 2023-12-05 19:21:07.000000 djangorestframework-stubs-3.14.5/djangorestframework_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-12-05 19:21:07.000000 djangorestframework-stubs-3.14.5/djangorestframework_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)      226 2023-12-05 19:21:07.000000 djangorestframework-stubs-3.14.5/djangorestframework_stubs.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       37 2023-12-05 19:21:07.000000 djangorestframework-stubs-3.14.5/djangorestframework_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.874677 djangorestframework-stubs-3.14.5/mypy_drf_plugin/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/mypy_drf_plugin/__init__.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.874677 djangorestframework-stubs-3.14.5/mypy_drf_plugin/lib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/mypy_drf_plugin/lib/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     2714 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/mypy_drf_plugin/lib/fullnames.py
--rw-r--r--   0 marti     (1000) marti      (121)      167 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/mypy_drf_plugin/lib/helpers.py
--rw-r--r--   0 marti     (1000) marti      (121)     1480 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.5/mypy_drf_plugin/main.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.874677 djangorestframework-stubs-3.14.5/mypy_drf_plugin/transformers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/mypy_drf_plugin/transformers/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)      355 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/mypy_drf_plugin/transformers/serializers.py
--rw-r--r--   0 marti     (1000) marti      (121)     1390 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/pyproject.toml
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.884677 djangorestframework-stubs-3.14.5/rest_framework-stubs/
--rw-r--r--   0 marti     (1000) marti      (121)      224 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       77 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1115 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authentication.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.888010 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/
--rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      168 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       73 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.888010 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.888010 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      453 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/management/commands/drf_create_token.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      337 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      552 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1901 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/compat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3144 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1560 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/documentation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3087 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    24960 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2147 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/filters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4456 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/generics.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.888010 djangorestframework-stubs-3.14.5/rest_framework-stubs/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.888010 djangorestframework-stubs-3.14.5/rest_framework-stubs/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      459 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/management/commands/generateschema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      726 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/metadata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1260 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      800 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/negotiation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5063 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/pagination.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1794 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/parsers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3078 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/permissions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     7105 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/relations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4736 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/renderers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3224 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/request.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1136 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/response.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      671 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/reverse.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/routers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.891343 djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/
--rw-r--r--   0 marti     (1000) marti      (121)      973 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2841 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/coreapi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2171 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/generators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      589 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/inspectors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3512 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/openapi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      261 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      411 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    12234 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4158 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/settings.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2776 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/status.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.891343 djangorestframework-stubs-3.14.5/rest_framework-stubs/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1991 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/templatetags/rest_framework.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5770 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/test.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1138 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/throttling.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      565 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/urlpatterns.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       89 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/urls.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:21:07.894677 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      133 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/breadcrumbs.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       54 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/encoders.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1051 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/field_mapping.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      498 2023-12-05 19:01:17.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/formatting.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      288 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      272 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/humanize_datetime.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      382 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/mediatypes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      703 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/model_meta.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      315 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/representation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3552 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/serializer_helpers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      145 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1169 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/versioning.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4726 2023-10-18 16:50:08.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1792 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.5/rest_framework-stubs/viewsets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      434 2023-12-05 19:21:07.894677 djangorestframework-stubs-3.14.5/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     2190 2023-12-05 19:20:37.000000 djangorestframework-stubs-3.14.5/setup.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.635208 djangorestframework_stubs-3.15.0/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1075 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/LICENSE.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)     3592 2024-04-30 19:56:36.635208 djangorestframework_stubs-3.15.0/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti     (1000)     2113 2023-10-04 20:46:18.000000 djangorestframework_stubs-3.15.0/README.md
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.635208 djangorestframework_stubs-3.15.0/djangorestframework_stubs.egg-info/
+-rw-r--r--   0 marti     (1000) marti     (1000)     3592 2024-04-30 19:56:36.000000 djangorestframework_stubs-3.15.0/djangorestframework_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti     (1000)     3237 2024-04-30 19:56:36.000000 djangorestframework_stubs-3.15.0/djangorestframework_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)        1 2024-04-30 19:56:36.000000 djangorestframework_stubs-3.15.0/djangorestframework_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)      227 2024-04-30 19:56:36.000000 djangorestframework_stubs-3.15.0/djangorestframework_stubs.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)       37 2024-04-30 19:56:36.000000 djangorestframework_stubs-3.15.0/djangorestframework_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.625208 djangorestframework_stubs-3.15.0/mypy_drf_plugin/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/mypy_drf_plugin/__init__.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.625208 djangorestframework_stubs-3.15.0/mypy_drf_plugin/lib/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/mypy_drf_plugin/lib/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     2714 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/mypy_drf_plugin/lib/fullnames.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      167 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/mypy_drf_plugin/lib/helpers.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     1480 2023-06-27 17:53:54.000000 djangorestframework_stubs-3.15.0/mypy_drf_plugin/main.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.625208 djangorestframework_stubs-3.15.0/mypy_drf_plugin/transformers/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/mypy_drf_plugin/transformers/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      355 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/mypy_drf_plugin/transformers/serializers.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     1420 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/pyproject.toml
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.628542 djangorestframework_stubs-3.15.0/rest_framework-stubs/
+-rw-r--r--   0 marti     (1000) marti     (1000)      278 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       77 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1115 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authentication.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.631875 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/
+-rw-r--r--   0 marti     (1000) marti     (1000)       24 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      168 2023-12-05 19:01:17.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/admin.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       73 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.631875 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/management/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.631875 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/management/commands/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      453 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/management/commands/drf_create_token.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      337 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      196 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      552 2023-12-05 19:01:17.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/views.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      103 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/checks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2039 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/compat.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3162 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1560 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/documentation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3087 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    25050 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/fields.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2234 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/filters.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4568 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/generics.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.631875 djangorestframework_stubs-3.15.0/rest_framework-stubs/management/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.631875 djangorestframework_stubs-3.15.0/rest_framework-stubs/management/commands/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      459 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/management/commands/generateschema.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      726 2023-06-02 14:08:55.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/metadata.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1260 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      800 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/negotiation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5063 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/pagination.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1794 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/parsers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3078 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/permissions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     7132 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/relations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4737 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/renderers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3336 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/request.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1248 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/response.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      673 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/reverse.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2660 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/routers.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.631875 djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/
+-rw-r--r--   0 marti     (1000) marti     (1000)      973 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2841 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/coreapi.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2171 2023-12-05 19:01:17.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/generators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      589 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/inspectors.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3567 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/openapi.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      261 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      411 2023-12-05 19:01:17.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/views.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    12565 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4158 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/settings.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2776 2023-12-05 19:01:17.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/status.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.631875 djangorestframework_stubs-3.15.0/rest_framework-stubs/templatetags/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2008 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/templatetags/rest_framework.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5778 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/test.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1138 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/throttling.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      565 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/urlpatterns.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       89 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/urls.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 19:56:36.635208 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      133 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/breadcrumbs.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      239 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/encoders.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1219 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/field_mapping.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      498 2023-12-05 19:01:17.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/formatting.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      288 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/html.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      272 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/humanize_datetime.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      274 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/json.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      382 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/mediatypes.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      703 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/model_meta.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      315 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/representation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3553 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/serializer_helpers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      145 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/urls.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2975 2023-03-15 16:53:40.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/validators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1170 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/versioning.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4726 2023-10-18 16:50:08.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/views.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1792 2023-06-02 14:08:55.000000 djangorestframework_stubs-3.15.0/rest_framework-stubs/viewsets.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      434 2024-04-30 19:56:36.635208 djangorestframework_stubs-3.15.0/setup.cfg
+-rw-r--r--   0 marti     (1000) marti     (1000)     2255 2024-04-30 19:55:44.000000 djangorestframework_stubs-3.15.0/setup.py
```

### Comparing `djangorestframework-stubs-3.14.5/LICENSE.txt` & `djangorestframework_stubs-3.15.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/PKG-INFO` & `djangorestframework_stubs-3.15.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: djangorestframework-stubs
-Version: 3.14.5
+Version: 3.15.0
 Summary: PEP-484 stubs for django-rest-framework
 Home-page: https://github.com/typeddjango/djangorestframework-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Release notes, https://github.com/typeddjango/djangorestframework-stubs/releases
+Project-URL: Funding, https://github.com/sponsors/typeddjango
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: django-stubs>=4.2.7
+Requires-Dist: django-stubs>=5.0.0
 Requires-Dist: typing-extensions>=3.10.0
 Requires-Dist: requests>=2.0.0
 Requires-Dist: types-requests>=0.1.12
 Requires-Dist: types-PyYAML>=5.4.3
 Provides-Extra: compatible-mypy
-Requires-Dist: mypy~=1.7.0; extra == "compatible-mypy"
+Requires-Dist: mypy~=1.10.0; extra == "compatible-mypy"
 Requires-Dist: django-stubs[compatible-mypy]; extra == "compatible-mypy"
 Provides-Extra: coreapi
 Requires-Dist: coreapi>=2.0.0; extra == "coreapi"
 Provides-Extra: markdown
 Requires-Dist: types-Markdown>=0.1.5; extra == "markdown"
 
 <img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
```

### Comparing `djangorestframework-stubs-3.14.5/README.md` & `djangorestframework_stubs-3.15.0/README.md`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/djangorestframework_stubs.egg-info/PKG-INFO` & `djangorestframework_stubs-3.15.0/djangorestframework_stubs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: djangorestframework-stubs
-Version: 3.14.5
+Version: 3.15.0
 Summary: PEP-484 stubs for django-rest-framework
 Home-page: https://github.com/typeddjango/djangorestframework-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Release notes, https://github.com/typeddjango/djangorestframework-stubs/releases
+Project-URL: Funding, https://github.com/sponsors/typeddjango
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: django-stubs>=4.2.7
+Requires-Dist: django-stubs>=5.0.0
 Requires-Dist: typing-extensions>=3.10.0
 Requires-Dist: requests>=2.0.0
 Requires-Dist: types-requests>=0.1.12
 Requires-Dist: types-PyYAML>=5.4.3
 Provides-Extra: compatible-mypy
-Requires-Dist: mypy~=1.7.0; extra == "compatible-mypy"
+Requires-Dist: mypy~=1.10.0; extra == "compatible-mypy"
 Requires-Dist: django-stubs[compatible-mypy]; extra == "compatible-mypy"
 Provides-Extra: coreapi
 Requires-Dist: coreapi>=2.0.0; extra == "coreapi"
 Provides-Extra: markdown
 Requires-Dist: types-Markdown>=0.1.5; extra == "markdown"
 
 <img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
```

### Comparing `djangorestframework-stubs-3.14.5/djangorestframework_stubs.egg-info/SOURCES.txt` & `djangorestframework_stubs-3.15.0/djangorestframework_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/mypy_drf_plugin/lib/fullnames.py` & `djangorestframework_stubs-3.15.0/mypy_drf_plugin/lib/fullnames.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/mypy_drf_plugin/main.py` & `djangorestframework_stubs-3.15.0/mypy_drf_plugin/main.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/pyproject.toml` & `djangorestframework_stubs-3.15.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
+target-version = ["py38", "py39", "py310", "py311", "py312"]
 
 [tool.ruff]
 # Adds to default excludes: https://docs.astral.sh/ruff/settings/#exclude
 extend-exclude = [
     ".*/",
     "drf_source",
     "stubgen",
@@ -35,18 +36,17 @@
     "E501",
     "E741",
     "E743",
     "F403", # Use wildcard import
     "F405",
     "F822",
     "F821",
-    "PYI026",  # TODO fix these errors
     "PGH003",  # TODO fix these errors
-    "PYI002",  # TODO fix these errors
 ]
+"rest_framework-stubs/compat.pyi" = ["PYI042"]
 
 [tool.ruff.flake8-tidy-imports.banned-api]
 "_typeshed.Self".msg = "Use typing_extensions.Self (PEP 673) instead."
 
 [tool.ruff.isort]
 split-on-trailing-comma = false
 extra-standard-library = ["_typeshed"]
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/authentication.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/authentication.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/authtoken/views.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/authtoken/views.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/compat.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/compat.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 from typing import Any
 
 from django.db.models import QuerySet
+from typing_extensions import TypeAlias
 
 try:
     from django.contrib.postgres import fields as postgres_fields
 except ImportError:
-    postgres_fields = None  # type: ignore
+    postgres_fields: TypeAlias = None  # type: ignore[no-redef]
 try:
     import coreapi
 except ImportError:
-    coreapi = None
+    coreapi: TypeAlias = None  # type: ignore[no-redef]
 try:
     import uritemplate
 except ImportError:
-    uritemplate = None  # type: ignore
+    uritemplate: TypeAlias = None  # type: ignore[no-redef]
 try:
     import coreschema
 except ImportError:
-    coreschema = None
+    coreschema: TypeAlias = None  # type: ignore[no-redef]
 try:
     import yaml
 except ImportError:
-    yaml = None  # type: ignore
+    yaml: TypeAlias = None  # type: ignore[no-redef]
 try:
     import requests
 except ImportError:
-    requests = None  # type: ignore
+    requests: TypeAlias = None  # type: ignore[no-redef]
 try:
     import pygments
 except ImportError:
-    pygments = None
+    pygments: TypeAlias = None  # type: ignore[no-redef]
+
 try:
     import markdown
-    def apply_markdown(text: str) -> str: ...
-
-except ImportError:
-    apply_markdown = None  # type: ignore
-    markdown = None  # type: ignore
-
-if markdown is not None and pygments is not None:
     from markdown.preprocessors import Preprocessor
+    def apply_markdown(text: str) -> str: ...
 
     class CodeBlockPreprocessor(Preprocessor):
         pattern: Any
         formatter: Any
         def run(self, lines: list[str]) -> list[str]: ...
 
+except ImportError:
+    apply_markdown: TypeAlias = None  # type: ignore[no-redef]
+    markdown: TypeAlias = None  # type: ignore[no-redef]
+
 def pygments_css(style: Any) -> str | None: ...
 def pygments_highlight(text: str, lang: str, style: Any) -> Any: ...
 def md_filter_add_syntax_highlight(md: Any) -> bool: ...
 def unicode_http_header(value: str | bytes) -> str: ...
-def distinct(queryset: QuerySet, base: QuerySet | None) -> QuerySet: ...
 
 SHORT_SEPARATORS: tuple[str, str]
 LONG_SEPARATORS: tuple[str, str]
 INDENT_SEPARATORS: tuple[str, str]
 
 __all__ = [
     "coreapi",
@@ -69,12 +68,11 @@
     "apply_markdown",
     "Preprocessor",
     "CodeBlockPreprocessor",
     "pygments_css",
     "pygments_highlight",
     "md_filter_add_syntax_highlight",
     "unicode_http_header",
-    "distinct",
     "SHORT_SEPARATORS",
     "LONG_SEPARATORS",
     "INDENT_SEPARATORS",
 ]
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/decorators.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/decorators.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 class ViewSetAction(Protocol[_View]):
     detail: bool
     url_path: str
     url_name: str
     kwargs: Mapping[str, Any]
     mapping: MethodMapper
     __call__: _View
+    __name__: str
 
 def api_view(
     http_method_names: Sequence[str] | None = ...,
 ) -> Callable[[Callable[Concatenate[Request, _P], _RESP]], AsView[Callable[Concatenate[HttpRequest, _P], _RESP]]]: ...
 def renderer_classes(renderer_classes: Sequence[BaseRenderer | type[BaseRenderer]]) -> Callable[[_View], _View]: ...
 def parser_classes(parser_classes: Sequence[BaseParser | type[BaseParser]]) -> Callable[[_View], _View]: ...
 def authentication_classes(
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/documentation.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/documentation.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/exceptions.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/fields.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/fields.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import datetime
 import uuid
 from _typeshed import Incomplete
-from collections.abc import Callable, Generator, Iterable, Mapping, MutableMapping, Sequence
+from collections.abc import Callable, Generator, Iterable, Mapping, Sequence
 from decimal import Decimal
 from enum import Enum
 from json import JSONDecoder, JSONEncoder
+from logging import Logger
 from re import Pattern
 from typing import Any, ClassVar, Final, Generic, NoReturn, Protocol, TypeVar
 
 from django.core.files.base import File
 from django.db import models
 from django.forms import ImageField as DjangoImageField  # noqa: F401
 from django_stubs_ext import StrOrPromise
 from rest_framework.serializers import BaseSerializer
 from rest_framework.validators import Validator
 from typing_extensions import Self, TypeAlias
 
+logger: Logger
+
 class _Empty(Enum):
     sentinel = 0
 
 empty: Final = _Empty.sentinel
 
 class BuiltinSignatureError(Exception): ...
 
@@ -40,15 +43,14 @@
     end_option_group: bool
     label: StrOrPromise
     value: str
     display_text: StrOrPromise
 
 def is_simple_callable(obj: Callable) -> bool: ...
 def get_attribute(instance: Any, attrs: list[str] | None) -> Any: ...
-def set_value(dictionary: MutableMapping[str, Any], keys: Sequence[str], value: Any) -> None: ...
 def to_choices_dict(choices: Iterable[Any]) -> dict: ...
 def flatten_choices_dict(choices: dict[Any, Any]) -> dict: ...
 def iter_options(
     grouped_choices: dict, cutoff: int | None = ..., cutoff_text: StrOrPromise | None = ...
 ) -> Generator[Option, None, None]: ...
 def get_error_detail(exc_info: Any) -> Any: ...
 
@@ -99,14 +101,15 @@
         label: StrOrPromise | None = None,
         help_text: StrOrPromise | None = None,
         style: dict[str, Any] | None = None,
         error_messages: dict[str, StrOrPromise] | None = None,
         validators: Sequence[Validator[_VT]] | None = ...,
         allow_null: bool = ...,
     ) -> None: ...
+    def __class_getitem__(cls, *args: Any, **kwargs: Any) -> type[Self]: ...
     def bind(self, field_name: str, parent: BaseSerializer) -> None: ...
     @property
     def validators(self) -> list[Validator[_VT]]: ...
     @validators.setter
     def validators(self, validators: list[Validator[_VT]]) -> None: ...
     def get_validators(self) -> list[Validator[_VT]]: ...
     def get_initial(self) -> _VT | None: ...
@@ -177,15 +180,15 @@
     ) -> None: ...
 
 class EmailField(CharField): ...
 
 class RegexField(CharField):
     def __init__(
         self,
-        regex: str | Pattern,
+        regex: str | Pattern[str],
         *,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool | None = None,
         default: _DefaultInitial[StrOrPromise] = ...,
         initial: _DefaultInitial[str] = ...,
         source: str | None = None,
@@ -326,24 +329,26 @@
     max_digits: int | None
     decimal_places: int | None
     coerce_to_string: bool | None
     max_value: Decimal | int | float | None
     min_value: Decimal | int | float | None
     localize: bool
     rounding: str | None
+    normalize_output: bool
     max_whole_digits: int | None
     def __init__(
         self,
         max_digits: int | None,
         decimal_places: int | None,
         coerce_to_string: bool | None = None,
         max_value: Decimal | int | float | None = None,
         min_value: Decimal | int | float | None = None,
         localize: bool = ...,
         rounding: str | None = None,
+        normalize_output: bool = ...,
         *,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool | None = None,
         default: _DefaultInitial[Decimal] = ...,
         initial: _DefaultInitial[Decimal] = ...,
         source: str | None = None,
@@ -609,16 +614,16 @@
         help_text: StrOrPromise | None = None,
         style: dict[str, Any] | None = None,
         error_messages: dict[str, StrOrPromise] | None = None,
         validators: Sequence[Validator[list[Any]]] | None = ...,
         allow_null: bool = ...,
         child: Field = ...,
         allow_empty: bool = ...,
-        max_length: int = ...,
-        min_length: int = ...,
+        max_length: int | None = ...,
+        min_length: int | None = ...,
     ) -> None: ...
     def run_child_validation(self, data: list[Mapping[Any, Any]]) -> Any: ...
 
 class DictField(Field[dict[Any, Any], dict[Any, Any], dict[Any, Any], Any]):
     child: Field
     allow_empty: bool
     def __init__(
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/filters.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/filters.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 
 from django.db.models import Model, QuerySet
 from rest_framework.request import Request
 from rest_framework.views import APIView
 
 _MT = TypeVar("_MT", bound=Model)
 
+def search_smart_split(search_terms: list[str]) -> list[str]: ...
+
 class BaseFilterBackend:
     def filter_queryset(self, request: Request, queryset: QuerySet[_MT], view: APIView) -> QuerySet[_MT]: ...
     def get_schema_fields(self, view: APIView) -> list[Any]: ...
     def get_schema_operation_parameters(self, view: APIView) -> list[dict[str, Incomplete]]: ...
 
 class SearchFilter(BaseFilterBackend):
     search_param: str
     template: str
     lookup_prefixes: dict[str, str]
     search_title: str
     search_description: str
     def get_search_fields(self, view: APIView, request: Request) -> Incomplete: ...
     def get_search_terms(self, request: Request) -> list[str]: ...
-    def construct_search(self, field_name: str) -> str: ...
+    def construct_search(self, field_name: str, queryset: QuerySet) -> str: ...
     def must_call_distinct(self, queryset: QuerySet, search_fields: Incomplete) -> bool: ...
     def to_html(self, request: Request, queryset: QuerySet, view: APIView) -> str: ...
 
 class OrderingFilter(BaseFilterBackend):
     ordering_param: str
     ordering_fields: Sequence[str] | None
     ordering_title: str
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/generics.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/generics.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.db.models.query import QuerySet
 from rest_framework import mixins, views
 from rest_framework.filters import BaseFilterBackend
 from rest_framework.pagination import BasePagination
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.serializers import BaseSerializer
+from typing_extensions import Self
 
 _MT_co = TypeVar("_MT_co", bound=Model, covariant=True)
 _MT_inv = TypeVar("_MT_inv", bound=Model)
 
 def get_object_or_404(
     queryset: type[_MT_co] | Manager[_MT_co] | QuerySet[_MT_co], *filter_args: Any, **filter_kwargs: Any
 ) -> _MT_co: ...
@@ -33,14 +34,15 @@
 class GenericAPIView(views.APIView, UsesQuerySet[_MT_co]):
     queryset: QuerySet[_MT_co] | Manager[_MT_co] | None
     serializer_class: type[BaseSerializer] | None
     lookup_field: str
     lookup_url_kwarg: str | None
     filter_backends: Sequence[type[BaseFilterBackend | BaseFilterProtocol[_MT_co]]]
     pagination_class: type[BasePagination] | None
+    def __class_getitem__(cls, *args: Any, **kwargs: Any) -> type[Self]: ...
     def get_object(self) -> _MT_co: ...
     def get_serializer(self, *args: Any, **kwargs: Any) -> BaseSerializer[_MT_co]: ...
     def get_serializer_class(self) -> type[BaseSerializer[_MT_co]]: ...
     def get_serializer_context(self) -> dict[str, Any]: ...
     def filter_queryset(self, queryset: QuerySet[_MT_co]) -> QuerySet[_MT_co]: ...
     @property
     def paginator(self) -> BasePagination | None: ...
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/metadata.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/metadata.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/mixins.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/mixins.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/negotiation.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/negotiation.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/pagination.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/pagination.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/parsers.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/permissions.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/permissions.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/relations.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/relations.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     reverse: Callable
     lookup_field: str
     lookup_url_kwarg: str
     format: str | None
     view_name: str | None
     def __init__(
         self,
-        view_name: str,
+        view_name: str | None = ...,
         *,
         many: bool = ...,
         allow_empty: bool = ...,
         queryset: QuerySet[_MT] | Manager[_MT] | None = ...,
         html_cutoff: int | None = ...,
         html_cutoff_text: str = ...,
         read_only: bool = ...,
@@ -125,15 +125,15 @@
         validators: Sequence[Validator[_MT]] | None = ...,
         error_messages: dict[str, StrOrPromise] | None = ...,
         style: dict[str, str] | None = ...,
         lookup_field: str | None = ...,
         lookup_url_kwarg: str | None = ...,
         format: str | None = ...,
     ) -> None: ...
-    def get_object(self, view_name: str, *view_args: Any, **view_kwargs: Any) -> _MT: ...
+    def get_object(self, view_name: str, view_args: list[Any], view_kwargs: dict[str, Any]) -> _MT: ...
     def get_url(self, obj: Model, view_name: str, request: Request, format: str | None) -> str | None: ...
 
 class HyperlinkedIdentityField(HyperlinkedRelatedField): ...
 
 class SlugRelatedField(RelatedField[_MT, str, str]):
     slug_field: str | None
     def __init__(
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/renderers.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/renderers.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def show_form_for_method(self, view: APIView, method: str, request: Request, obj: Any) -> bool: ...
     def _get_serializer(
         self,
         serializer_class: type[BaseSerializer],
         view_instance: APIView,
         request: Request,
         *args: Incomplete,
-        **kwargs: Incomplete
+        **kwargs: Incomplete,
     ) -> BaseSerializer: ...
     def get_rendered_html_form(self, data: Any, view: APIView, method: str, request: Request) -> Any: ...
     def render_form_for_serializer(self, serializer: BaseSerializer) -> Any: ...
     def get_raw_data_form(self, data: Any, view: APIView, method: str, request: Request) -> forms.Form | None: ...
     def get_name(self, view: APIView) -> str: ...
     def get_description(self, view: APIView, status_code: int) -> str: ...
     def get_breadcrumbs(self, request: Request) -> list[tuple[str, str]]: ...
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/request.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/request.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from django.http.request import _ImmutableQueryDict
 from rest_framework.authentication import BaseAuthentication
 from rest_framework.authtoken.models import Token
 from rest_framework.negotiation import BaseContentNegotiation
 from rest_framework.parsers import BaseParser
 from rest_framework.versioning import BaseVersioning
 from rest_framework.views import APIView
+from typing_extensions import Self
 
 def is_form_media_type(media_type: str) -> bool: ...
 
 class override_method(AbstractContextManager[Request]):
     def __init__(self, view: APIView, request: Request, method: str) -> None: ...
     def __enter__(self) -> Request: ...
     def __exit__(
@@ -54,14 +55,15 @@
         self,
         request: HttpRequest,
         parsers: Sequence[BaseParser] | None = ...,
         authenticators: Sequence[BaseAuthentication] | None = ...,
         negotiator: BaseContentNegotiation | None = ...,
         parser_context: dict[str, Any] | None = ...,
     ) -> None: ...
+    def __class_getitem__(cls, *args: Any, **kwargs: Any) -> type[Self]: ...
     @property
     def content_type(self) -> str: ...  # type: ignore[override]
     @property
     def stream(self) -> Any: ...
     @property
     def query_params(self) -> _ImmutableQueryDict: ...
     @property
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/response.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/response.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from django.template.base import Template
 from django.template.response import SimpleTemplateResponse
 from django.test.utils import ContextList
 from django.urls import ResolverMatch
 from rest_framework.request import Request
 from rest_framework.test import APIClient
+from typing_extensions import Self
 
 class Response(SimpleTemplateResponse):
     data: Any
     exception: bool
     content_type: str | None
     _request: Request
     def __init__(
@@ -18,14 +19,15 @@
         data: Any = ...,
         status: int | None = ...,
         template_name: str | None = ...,
         headers: Mapping[str, str] | None = ...,
         exception: bool = ...,
         content_type: str | None = ...,
     ) -> None: ...
+    def __class_getitem__(cls, *args: Any, **kwargs: Any) -> type[Self]: ...
     @property
     def rendered_content(self) -> Any: ...
     def render(self) -> Any: ...
     @property
     def status_text(self) -> str: ...
 
 class _MonkeyPatchedResponse(Response):
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/reverse.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/reverse.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 def preserve_builtin_query_params(url: str, request: HttpRequest | None = ...) -> str: ...
 def reverse(
     viewname: str,
     args: Sequence[Any] | None = ...,
     kwargs: Mapping[str, Any] | None = ...,
     request: HttpRequest | None = ...,
     format: str | None = ...,
-    **extra: Any
+    **extra: Any,
 ) -> str: ...
 def _reverse(
     viewname: str,
     args: Sequence[Any] | None = ...,
     kwargs: Mapping[str, Any] | None = ...,
     request: HttpRequest | None = ...,
     format: str | None = ...,
-    **extra: Any
+    **extra: Any,
 ) -> str: ...
 
 reverse_lazy: Callable[..., str]
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/routers.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/routers.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -31,23 +31,24 @@
     renamed_methods: Iterable[str | Callable]
 
 class BaseRouter(metaclass=RenameRouterMethods):
     registry: list[tuple[str, type[ViewSetMixin], str]]
     def register(
         self, prefix: str, viewset: type[ViewSetMixin], basename: str | None = ..., base_name: str | None = ...
     ) -> None: ...
+    def is_already_registered(self, new_basename: str) -> bool: ...
     def get_default_basename(self, viewset: type[ViewSetMixin]) -> str: ...
     def get_urls(self) -> list[_AnyURL]: ...
     @property
     def urls(self) -> list[_AnyURL]: ...
 
 class SimpleRouter(BaseRouter):
     routes: list[Route | DynamicRoute]
     trailing_slash: str
-    def __init__(self, trailing_slash: bool = ...) -> None: ...
+    def __init__(self, trailing_slash: bool = ..., use_regex_path: bool = ...) -> None: ...
     def get_routes(self, viewset: type[ViewSetMixin]) -> list[Route]: ...
     def _get_dynamic_route(self, route: DynamicRoute, action: Any) -> Route: ...
     def get_method_map(self, viewset: type[ViewSetMixin], method_map: Mapping[str, str]) -> dict[str, str]: ...
     def get_lookup_regex(self, viewset: type[ViewSetMixin], lookup_prefix: str = ...) -> str: ...
 
 class APIRootView(views.APIView):
     _ignore_model_permissions: bool
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/__init__.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/coreapi.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/coreapi.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/generators.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/generators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/inspectors.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/inspectors.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/schemas/openapi.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/schemas/openapi.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     def get_filter_parameters(self, path: str, method: str) -> list[dict[str, Any]]: ...
     def allows_filters(self, path: str, method: str) -> bool: ...
     def get_pagination_parameters(self, path: str, method: str) -> list[dict[str, Any]]: ...
     def map_choicefield(self, field: Field) -> dict[str, Any]: ...
     def map_field(self, field: Field) -> dict[str, Any]: ...
     def map_serializer(self, serializer: BaseSerializer) -> dict[str, Any]: ...
     def map_field_validators(self, field: Any, schema: Any) -> None: ...
+    def get_field_name(self, field: Field) -> str: ...
     def get_paginator(self) -> type[BasePagination] | None: ...
     def map_parsers(self, path: str, method: str) -> list[str]: ...
     def map_renderers(self, path: str, method: str) -> list[str]: ...
     def get_serializer(self, path: str, method: str) -> BaseSerializer | None: ...
     def get_request_serializer(self, path: str, method: str) -> BaseSerializer | None: ...
     def get_response_serializer(self, path: str, method: str) -> BaseSerializer | None: ...
     def get_reference(self, serializer: BaseSerializer) -> dict[str, str]: ...
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/serializers.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/serializers.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from collections.abc import Callable, Iterable, Iterator, Mapping, MutableMapping, Sequence
+from collections.abc import Iterable, Iterator, Mapping, MutableMapping, Sequence
 from typing import Any, ClassVar, Generic, Literal, NoReturn, TypeVar
 
 from django.db import models
 from django.db.models import Manager, Model, QuerySet
 from django.utils.functional import cached_property
 from django_stubs_ext import StrOrPromise
 from rest_framework.exceptions import APIException as APIException
@@ -47,14 +47,15 @@
 from rest_framework.fields import RegexField as RegexField
 from rest_framework.fields import SerializerMethodField as SerializerMethodField
 from rest_framework.fields import SkipField as SkipField
 from rest_framework.fields import SlugField as SlugField
 from rest_framework.fields import TimeField as TimeField
 from rest_framework.fields import URLField as URLField
 from rest_framework.fields import UUIDField as UUIDField
+from rest_framework.fields import _DefaultInitial
 from rest_framework.fields import empty as empty
 from rest_framework.relations import Hyperlink as Hyperlink
 from rest_framework.relations import HyperlinkedIdentityField as HyperlinkedIdentityField
 from rest_framework.relations import HyperlinkedRelatedField as HyperlinkedRelatedField
 from rest_framework.relations import ManyRelatedField as ManyRelatedField
 from rest_framework.relations import PrimaryKeyRelatedField as PrimaryKeyRelatedField
 from rest_framework.relations import RelatedField as RelatedField
@@ -62,14 +63,15 @@
 from rest_framework.relations import StringRelatedField as StringRelatedField
 from rest_framework.utils.model_meta import FieldInfo, RelationInfo
 from rest_framework.utils.serializer_helpers import BindingDict, BoundField, ReturnDict, ReturnList
 from rest_framework.validators import BaseUniqueForValidator, UniqueTogetherValidator, Validator
 from typing_extensions import Self
 
 LIST_SERIALIZER_KWARGS: Sequence[str]
+LIST_SERIALIZER_KWARGS_REMOVE: Sequence[str]
 ALL_FIELDS: str
 
 _MT = TypeVar("_MT", bound=Model)  # Model Type
 _IN = TypeVar("_IN")  # Instance Type
 
 class BaseSerializer(Generic[_IN], Field[Any, Any, Any, _IN]):
     partial: bool
@@ -125,14 +127,15 @@
 class Serializer(
     BaseSerializer[_IN],
     metaclass=SerializerMetaclass,
 ):
     _declared_fields: dict[str, Field]
     default_error_messages: ClassVar[dict[str, StrOrPromise]]
     def get_initial(self) -> Any: ...
+    def set_value(self, dictionary: MutableMapping[str, Any], keys: Sequence[str], value: Any) -> None: ...
     @cached_property
     def fields(self) -> BindingDict: ...
     def get_fields(self) -> dict[str, Field]: ...
     def to_representation(self, instance: _IN) -> dict[str, Any]: ...
     def validate(self, attrs: Any) -> Any: ...
     def __iter__(self) -> Iterator[BoundField]: ...
     def __getitem__(self, key: str) -> BoundField: ...
@@ -172,14 +175,15 @@
         style: dict[str, Any] | None = None,
         error_messages: dict[str, StrOrPromise] | None = None,
         validators: Sequence[Validator[list[Any]]] | None = ...,
         allow_null: bool = ...,
         min_length: int | None = ...,
         max_length: int | None = ...,
     ) -> None: ...
+    def run_child_validation(self, data: Any) -> Any: ...
     def to_representation(self, data: Manager[Any] | Iterable[Any]) -> list[Any]: ...  # type: ignore[override]
     def get_initial(self) -> list[Mapping[Any, Any]]: ...
     def validate(self, attrs: Any) -> Any: ...
     @property
     def data(self) -> ReturnList: ...
     @property
     def errors(self) -> ReturnList: ...
@@ -198,27 +202,28 @@
     class Meta:
         model: type[_MT]  # type: ignore
         fields: Sequence[str] | Literal["__all__"]
         read_only_fields: Sequence[str] | None
         exclude: Sequence[str] | None
         depth: int | None
         extra_kwargs: dict[str, dict[str, Any]]
+
     def __init__(
         self,
         instance: None | _MT | Sequence[_MT] | QuerySet[_MT] | Manager[_MT] = ...,
         data: Any = ...,
         *,
         partial: bool = ...,
         many: bool = ...,
         context: dict[str, Any] = ...,
         read_only: bool = ...,
         write_only: bool = ...,
         required: bool | None = None,
-        default: _MT | Sequence[_MT] | Callable[[], _MT | Sequence[_MT]] = ...,
-        initial: _MT | Sequence[_MT] | Callable[[], _MT | Sequence[_MT]] = ...,
+        default: _DefaultInitial[_MT | Sequence[_MT]] = ...,
+        initial: _DefaultInitial[_MT | Sequence[_MT]] = ...,
         source: str | None = None,
         label: StrOrPromise | None = None,
         help_text: StrOrPromise | None = None,
         style: dict[str, Any] | None = None,
         error_messages: dict[str, StrOrPromise] | None = None,
         validators: Sequence[Validator[_MT]] | None = ...,
         allow_null: bool = ...,
@@ -229,32 +234,33 @@
     def save(self, **kwargs: Any) -> _MT: ...
     def get_field_names(self, declared_fields: Mapping[str, Field], info: FieldInfo) -> list[str]: ...
     def get_default_field_names(self, declared_fields: Mapping[str, Field], model_info: FieldInfo) -> list[str]: ...
     def build_field(
         self, field_name: str, info: FieldInfo, model_class: _MT, nested_depth: int
     ) -> tuple[type[Field], dict[str, Any]]: ...
     def build_standard_field(
-        self, field_name: str, model_field: type[models.Field]
+        self, field_name: str, model_field: models.Field
     ) -> tuple[type[Field], dict[str, Any]]: ...
     def build_relational_field(
         self, field_name: str, relation_info: RelationInfo
     ) -> tuple[type[Field], dict[str, Any]]: ...
     def build_nested_field(
         self, field_name: str, relation_info: RelationInfo, nested_depth: int
     ) -> tuple[type[Field], dict[str, Any]]: ...
     def build_property_field(self, field_name: str, model_class: _MT) -> tuple[type[Field], dict[str, Any]]: ...
     def build_url_field(self, field_name: str, model_class: _MT) -> tuple[type[Field], dict[str, Any]]: ...
     def build_unknown_field(self, field_name: str, model_class: _MT) -> NoReturn: ...
     def include_extra_kwargs(
         self, kwargs: MutableMapping[str, Any], extra_kwargs: MutableMapping[str, Any]
     ) -> MutableMapping[str, Any]: ...
     def get_extra_kwargs(self) -> dict[str, Any]: ...
+    def get_unique_together_constraints(self, model: _MT) -> Iterator[tuple[set[tuple[str, ...]], Manager[_MT]]]: ...
     def get_uniqueness_extra_kwargs(
         self, field_names: Iterable[str], declared_fields: Mapping[str, Field], extra_kwargs: dict[str, Any]
     ) -> tuple[dict[str, Any], dict[str, HiddenField]]: ...
     def _get_model_fields(
         self, field_names: Iterable[str], declared_fields: Mapping[str, Field], extra_kwargs: MutableMapping[str, Any]
     ) -> dict[str, models.Field]: ...
     def get_unique_together_validators(self) -> list[UniqueTogetherValidator]: ...
     def get_unique_for_date_validators(self) -> list[BaseUniqueForValidator]: ...
 
-class HyperlinkedModelSerializer(ModelSerializer): ...
+class HyperlinkedModelSerializer(ModelSerializer[_MT]): ...
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/settings.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/settings.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/status.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/status.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/templatetags/rest_framework.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/templatetags/rest_framework.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def form_for_link(link: Any) -> Incomplete: ...
 def render_markdown(markdown_text: Any) -> Incomplete: ...
 def get_pagination_html(pager: Any) -> Incomplete: ...
 def render_form(serializer: Any, template_pack: Any | None = ...) -> Incomplete: ...
 def render_field(field: Any, style: Any) -> Incomplete: ...
 def optional_login(request: Request) -> Incomplete: ...
 def optional_docs_login(request: Request) -> Incomplete: ...
-def optional_logout(request: Request, user: AnonymousUser | AbstractBaseUser) -> Incomplete: ...
+def optional_logout(request: Request, user: AnonymousUser | AbstractBaseUser, csrf_token: str) -> Incomplete: ...
 def add_query_param(request: Request, key: str, val: Any) -> Incomplete: ...
 def as_string(value: Any) -> str: ...
 def as_list_of_strings(value: Any) -> list[str]: ...
 def add_class(value: Any, css_class: Any) -> Incomplete: ...
 def format_value(value: Any) -> Incomplete: ...
 def items(value: Any) -> Incomplete: ...
 def data(value: Any) -> Incomplete: ...
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/test.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/test.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from django.test.client import RequestFactory as DjangoRequestFactory
 from rest_framework.authtoken.models import Token
 from rest_framework.request import Request
 from rest_framework.response import _MonkeyPatchedResponse
 from typing_extensions import TypeAlias
 
 _GetDataType: TypeAlias = (
-    Mapping[str, str | bytes | int | Iterable[str | bytes | int]]
-    | Iterable[tuple[str, str | bytes | int | Iterable[str | bytes | int]]]
+    Mapping[str, str | bytes | float | Iterable[str | bytes | float]]
+    | Iterable[tuple[str, str | bytes | float | Iterable[str | bytes | float]]]
     | None
 )
 
 def force_authenticate(
     request: HttpRequest, user: AnonymousUser | AbstractBaseUser | None = ..., token: Token | None = ...
 ) -> None: ...
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/throttling.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/throttling.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/urlpatterns.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/urlpatterns.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/field_mapping.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/field_mapping.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from _typeshed import Incomplete
 from collections.abc import MutableMapping, Sequence
-from typing import Any, Generic, TypeVar
+from typing import Any, Generic, Iterator, TypeVar
 
 from django.db import models
+from rest_framework.validators import UniqueValidator
 
 NUMERIC_FIELD_TYPES: Sequence[type[models.Field]]
 
 _K = TypeVar("_K", bound=type)
 _V = TypeVar("_V")
 
 class ClassLookupDict(Generic[_K, _V]):
     mapping: MutableMapping[type[_K], _V]
     def __init__(self, mapping: MutableMapping[type[_K], _V]) -> None: ...
     def __getitem__(self, key: _K) -> _V: ...
     def __setitem__(self, key: _K, value: _V) -> None: ...
 
 def needs_label(model_field: models.Field, field_name: str) -> bool: ...
 def get_detail_view_name(model: models.Model) -> str: ...
+def get_unique_validators(field_name: str, model_field: models.Field) -> Iterator[UniqueValidator]: ...
 def get_field_kwargs(field_name: str, model_field: models.Field) -> dict[str, Any]: ...
 def get_relation_kwargs(field_name: str, relation_info: Incomplete) -> dict[str, Any]: ...
 def get_nested_relation_kwargs(relation_info: Incomplete) -> dict[str, Any]: ...
 def get_url_kwargs(model_field: models.Model) -> dict[str, Any]: ...
 def get_unique_error_message(model_field: models.Field) -> str: ...
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/model_meta.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/model_meta.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/utils/serializer_helpers.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/utils/serializer_helpers.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self, __map: SupportsKeysAndGetItem[_KT, _VT], *, serializer: BaseSerializer) -> None: ...
     @overload
     def __init__(
         self: ReturnDict[str, _VT],
         __map: SupportsKeysAndGetItem[str, _VT],
         *,
         serializer: BaseSerializer,
-        **kwargs: _VT
+        **kwargs: _VT,
     ) -> None: ...
     @overload
     def __init__(self, __iterable: Iterable[tuple[_KT, _VT]], *, serializer: BaseSerializer) -> None: ...
     @overload
     def __init__(
         self: ReturnDict[str, _VT], __iterable: Iterable[tuple[str, _VT]], *, serializer: BaseSerializer, **kwargs: _VT
     ) -> None: ...
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/validators.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/validators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/versioning.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/versioning.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def reverse(
         self,
         viewname: str,
         args: Sequence[Any] | None = ...,
         kwargs: Mapping[str, Any] | None = ...,
         request: Request | None = ...,
         format: str | None = ...,
-        **extra: Any
+        **extra: Any,
     ) -> str: ...
     def is_allowed_version(self, version: str | None) -> bool: ...
 
 class AcceptHeaderVersioning(BaseVersioning):
     invalid_version_message: str
 
 class URLPathVersioning(BaseVersioning):
```

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/views.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/views.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/rest_framework-stubs/viewsets.pyi` & `djangorestframework_stubs-3.15.0/rest_framework-stubs/viewsets.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.5/setup.py` & `djangorestframework_stubs-3.15.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,31 +16,31 @@
     return result
 
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
-    "django-stubs>=4.2.7",
+    "django-stubs>=5.0.0",
     "typing-extensions>=3.10.0",
     "requests>=2.0.0",
     "types-requests>=0.1.12",
     "types-PyYAML>=5.4.3",
 ]
 
-# Keep compatible-mypy major.minor version pinned to what we use in CI (requirements.txt)
+# Keep compatible-mypy major.minor version pinned to what latest django-stubs release uses.
 extras_require = {
-    "compatible-mypy": ["mypy~=1.7.0", "django-stubs[compatible-mypy]"],
+    "compatible-mypy": ["mypy~=1.10.0", "django-stubs[compatible-mypy]"],
     "coreapi": ["coreapi>=2.0.0"],
     "markdown": ["types-Markdown>=0.1.5"],
 }
 
 setup(
     name="djangorestframework-stubs",
-    version="3.14.5",
+    version="3.15.0",
     description="PEP-484 stubs for django-rest-framework",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/typeddjango/djangorestframework-stubs",
     author="Maksim Kurnikov",
     author_email="maxim.kurnikov@gmail.com",
     maintainer="Marti Raudsepp",
@@ -60,9 +60,10 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
         "Framework :: Django",
     ],
     project_urls={
         "Release notes": "https://github.com/typeddjango/djangorestframework-stubs/releases",
+        "Funding": "https://github.com/sponsors/typeddjango",
     },
 )
```

