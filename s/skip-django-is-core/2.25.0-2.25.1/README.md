# Comparing `tmp/skip_django_is_core-2.25.0.tar.gz` & `tmp/skip_django_is_core-2.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip_django_is_core-2.25.0.tar", last modified: Fri Apr 19 10:34:33 2024, max compression
+gzip compressed data, was "skip_django_is_core-2.25.1.tar", last modified: Tue Apr 30 06:58:18 2024, max compression
```

## Comparing `skip_django_is_core-2.25.0.tar` & `skip_django_is_core-2.25.1.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.188297 skip_django_is_core-2.25.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-19 10:34:33.188297 skip_django_is_core-2.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/README
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.148296 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/field_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/http_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/rest_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/ui_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/ui_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.148296 skip_django_is_core-2.25.0/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/auth/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/cores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/commands/deleteexpiredexports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/0002_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.136296 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/background_serialization.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.156297 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/generic_views/table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.156297 skip_django_is_core-2.25.0/is_core/contrib/dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/cores.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.156297 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/cores.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.156297 skip_django_is_core-2.25.0/is_core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/exceptions/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.160297 skip_django_is_core-2.25.0/is_core/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/fieldset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/formsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13940 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.160297 skip_django_is_core-2.25.0/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/add_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/detail_views.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25711 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/form_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/generic_views/inlines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/generic_inline_form_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_form_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_objects_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_table_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/objects_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/table_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/models/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/paginators.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/static/is_core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/static/is_core/css/
--rw-r--r--   0 runner    (1001) docker     (127)   277370 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/css/app.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.172297 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   136822 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   747545 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   136516 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    92136 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    78460 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144714 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34052 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   204814 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   917575 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   204528 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   104280 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    80300 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    32357 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.eot
--rwxr-xr-x   0 runner    (1001) docker     (127)    95652 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)    56512 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)    35804 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.172297 skip_django_is_core-2.25.0/is_core/static/is_core/images/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/images/arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/images/cal.png
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/images/select-arrow.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.172297 skip_django_is_core-2.25.0/is_core/static/is_core/js/
--rw-r--r--   0 runner    (1001) docker     (127)  1054526 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.176297 skip_django_is_core-2.25.0/is_core/templates/is_core/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/500.html
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/error.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_field.html
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/inline_table.html
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/login_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/model_add_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/model_default_form.html
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/model_detail_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/responsive_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/responsive_inline_objects.html
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/stacked_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/tabular_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/tabular_inline_objects.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/add_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/base_table.html
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/default_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/detail_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/objects.html
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/readonly_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/readonly_fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/rest_documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/table.html
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/home.html
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/logged_out.html
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/bread_crumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/sub_menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/tabs_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templates/is_core/views/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/views/bulk-change-view.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/is_core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/data_generator_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/is_core/tests/factory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/factory/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/rest_generic_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/ui_generic_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/is_core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/field_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/is_core/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/views/csrf.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/views/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:34:33.188297 skip_django_is_core-2.25.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:34:32.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.776891 skip_django_is_core-2.25.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-30 06:58:18.776891 skip_django_is_core-2.25.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/README
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/cores/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/cores/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/cores/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/dynamo/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/dynamo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/elasticsearch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/elasticsearch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.740892 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.744892 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/field_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/http_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/rest_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/ui_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/ui_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.744892 skip_django_is_core-2.25.1/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/dj/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/auth/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/contrib/background_export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/cores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/contrib/background_export/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/contrib/background_export/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/management/commands/deleteexpiredexports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/contrib/background_export/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/migrations/0002_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.736891 skip_django_is_core-2.25.1/is_core/contrib/background_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/contrib/background_export/templates/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/templates/is_core/background_serialization.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/contrib/background_export/templates/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/templates/is_core/generic_views/table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/background_export/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.748891 skip_django_is_core-2.25.1/is_core/contrib/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/dynamo/cores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/dynamo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/dynamo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/dynamo/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.752891 skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/cores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.752891 skip_django_is_core-2.25.1/is_core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/exceptions/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.752891 skip_django_is_core-2.25.1/is_core/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/fieldset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/formsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.752891 skip_django_is_core-2.25.1/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/add_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/detail_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25711 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/form_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.756891 skip_django_is_core-2.25.1/is_core/generic_views/inlines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/inlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/inlines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/inlines/generic_inline_form_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/inlines/inline_form_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/inlines/inline_objects_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/inlines/inline_table_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/inlines/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/objects_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/generic_views/table_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.736891 skip_django_is_core-2.25.1/is_core/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.736891 skip_django_is_core-2.25.1/is_core/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.756891 skip_django_is_core-2.25.1/is_core/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.756891 skip_django_is_core-2.25.1/is_core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/models/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.756891 skip_django_is_core-2.25.1/is_core/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/rest/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/rest/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/rest/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/rest/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/rest/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.736891 skip_django_is_core-2.25.1/is_core/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.736891 skip_django_is_core-2.25.1/is_core/static/is_core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.756891 skip_django_is_core-2.25.1/is_core/static/is_core/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   277370 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/css/app.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.764891 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   136822 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   747545 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   136516 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    92136 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    78460 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144714 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34052 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   204814 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   917575 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   204528 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   104280 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    80300 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32357 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/icon-works-webfont.eot
+-rwxr-xr-x   0 runner    (1001) docker     (127)    95652 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/icon-works-webfont.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56512 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/icon-works-webfont.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35804 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/fonts/icon-works-webfont.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.764891 skip_django_is_core-2.25.1/is_core/static/is_core/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/images/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/images/cal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/images/select-arrow.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.764891 skip_django_is_core-2.25.1/is_core/static/is_core/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  1054526 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/static/is_core/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.736891 skip_django_is_core-2.25.1/is_core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.768891 skip_django_is_core-2.25.1/is_core/templates/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/error.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.768891 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/default_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/default_fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/default_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/inline_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/login_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/model_add_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/model_default_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/model_detail_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/responsive_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/responsive_inline_objects.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/stacked_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/tabular_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/forms/tabular_inline_objects.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.768891 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/add_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/base_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/default_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/detail_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/objects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/readonly_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/readonly_fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/rest_documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/logged_out.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.772891 skip_django_is_core-2.25.1/is_core/templates/is_core/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/menu/bread_crumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/menu/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/menu/sub_menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/menu/tabs_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.772891 skip_django_is_core-2.25.1/is_core/templates/is_core/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templates/is_core/views/bulk-change-view.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.772891 skip_django_is_core-2.25.1/is_core/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templatetags/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templatetags/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templatetags/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/templatetags/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.772891 skip_django_is_core-2.25.1/is_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/tests/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/tests/data_generator_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.772891 skip_django_is_core-2.25.1/is_core/tests/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/tests/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/tests/factory/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/tests/rest_generic_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/tests/ui_generic_test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.772891 skip_django_is_core-2.25.1/is_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/utils/field_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.772891 skip_django_is_core-2.25.1/is_core/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/views/csrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/is_core/views/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:58:18.776891 skip_django_is_core-2.25.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-30 06:58:15.000000 skip_django_is_core-2.25.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:58:18.776891 skip_django_is_core-2.25.1/skip_django_is_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-30 06:58:18.000000 skip_django_is_core-2.25.1/skip_django_is_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-30 06:58:18.000000 skip_django_is_core-2.25.1/skip_django_is_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:58:18.000000 skip_django_is_core-2.25.1/skip_django_is_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:58:18.000000 skip_django_is_core-2.25.1/skip_django_is_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 06:58:18.000000 skip_django_is_core-2.25.1/skip_django_is_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 06:58:18.000000 skip_django_is_core-2.25.1/skip_django_is_core.egg-info/top_level.txt
```

### Comparing `skip_django_is_core-2.25.0/LICENSE` & `skip_django_is_core-2.25.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/PKG-INFO` & `skip_django_is_core-2.25.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-is-core
-Version: 2.25.0
+Version: 2.25.1
 Summary: Information systems core.
 Home-page: https://github.com/skip-pay/django-is-core
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,admin,information systems,REST
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip_django_is_core-2.25.0/README.md` & `skip_django_is_core-2.25.1/README.md`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/__init__.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/cores/__init__.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/resources.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/cores/resources.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/core.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/dynamo/core.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/models.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/elasticsearch/models.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/forms/__init__.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0001_initial.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/models.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/models.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/dynamo.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/dynamo.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/elasticsearch.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/factories.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/factories.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/field_permissions.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/field_permissions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/http_exceptions.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/permissions.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/permissions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/rest.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/rest.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/rest_permissions.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/rest_permissions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/test_case.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/ui_ordering.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/ui_ordering.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/ui_permissions.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/ui_permissions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/utils.py` & `skip_django_is_core-2.25.1/example/dj/apps/issue_tracker/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/settings/base.py` & `skip_django_is_core-2.25.1/example/dj/settings/base.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/settings/settings.py` & `skip_django_is_core-2.25.1/example/dj/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/example/dj/wsgi.py` & `skip_django_is_core-2.25.1/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/actions.py` & `skip_django_is_core-2.25.1/is_core/actions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/auth/permissions.py` & `skip_django_is_core-2.25.1/is_core/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/auth/views.py` & `skip_django_is_core-2.25.1/is_core/auth/views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/config.py` & `skip_django_is_core-2.25.1/is_core/config.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/cores.py` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/cores.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/management/commands/deleteexpiredexports.py` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/management/commands/deleteexpiredexports.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/0001_initial.py` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/0002_migration.py` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/migrations/0002_migration.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/models.py` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/models.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/resource.py` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/resource.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/tasks.py` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/tasks.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/generic_views/table.html` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/templates/is_core/generic_views/table.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/background_export/views.py` & `skip_django_is_core-2.25.1/is_core/contrib/background_export/views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/dynamo/cores.py` & `skip_django_is_core-2.25.1/is_core/contrib/dynamo/cores.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/dynamo/views.py` & `skip_django_is_core-2.25.1/is_core/contrib/dynamo/views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/cores.py` & `skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/cores.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/filters.py` & `skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/views.py` & `skip_django_is_core-2.25.1/is_core/contrib/elasticsearch/views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/exceptions/response.py` & `skip_django_is_core-2.25.1/is_core/exceptions/response.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/boundfield.py` & `skip_django_is_core-2.25.1/is_core/forms/boundfield.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/fields.py` & `skip_django_is_core-2.25.1/is_core/forms/fields.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/fieldset.py` & `skip_django_is_core-2.25.1/is_core/forms/fieldset.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/forms.py` & `skip_django_is_core-2.25.1/is_core/forms/forms.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/formsets.py` & `skip_django_is_core-2.25.1/is_core/forms/formsets.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/generic.py` & `skip_django_is_core-2.25.1/is_core/forms/generic.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/models.py` & `skip_django_is_core-2.25.1/is_core/forms/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
                                                       itertools.chain(opts.exclude or (), readonly_exclude or ()))
 
     def _get_validation_exclusions(self):
         exclude = super(SmartModelForm, self)._get_validation_exclusions()
         for f in self.instance._meta.fields:
             field = f.name
             if field in self.readonly_fields and field not in exclude:
-                exclude.append(field)
+                exclude.add(field)
         return exclude
 
 
 def get_model_fields(model, fields):
     model_fields = []
     for field in model._meta.fields + model._meta.many_to_many:
         if field.editable and (fields is None or field.name in fields):
```

### Comparing `skip_django_is_core-2.25.0/is_core/forms/patch.py` & `skip_django_is_core-2.25.1/is_core/forms/patch.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/utils.py` & `skip_django_is_core-2.25.1/is_core/forms/utils.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/forms/widgets.py` & `skip_django_is_core-2.25.1/is_core/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/add_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/add_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/base.py` & `skip_django_is_core-2.25.1/is_core/generic_views/base.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/detail_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/detail_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/form_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/form_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/inlines/base.py` & `skip_django_is_core-2.25.1/is_core/generic_views/inlines/base.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/inlines/generic_inline_form_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/inlines/generic_inline_form_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_form_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/inlines/inline_form_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_objects_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/inlines/inline_objects_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_table_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/inlines/inline_table_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/inlines/permissions.py` & `skip_django_is_core-2.25.1/is_core/generic_views/inlines/permissions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/mixins.py` & `skip_django_is_core-2.25.1/is_core/generic_views/mixins.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/objects_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/objects_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/generic_views/table_views.py` & `skip_django_is_core-2.25.1/is_core/generic_views/table_views.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/loading.py` & `skip_django_is_core-2.25.1/is_core/loading.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/django.mo` & `skip_django_is_core-2.25.1/is_core/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/django.po` & `skip_django_is_core-2.25.1/is_core/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/main.py` & `skip_django_is_core-2.25.1/is_core/main.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/menu.py` & `skip_django_is_core-2.25.1/is_core/menu.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/middleware.py` & `skip_django_is_core-2.25.1/is_core/middleware.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/models/patch.py` & `skip_django_is_core-2.25.1/is_core/models/patch.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/patterns.py` & `skip_django_is_core-2.25.1/is_core/patterns.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/rest/datastructures.py` & `skip_django_is_core-2.25.1/is_core/rest/datastructures.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/rest/filters.py` & `skip_django_is_core-2.25.1/is_core/rest/filters.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/rest/paginators.py` & `skip_django_is_core-2.25.1/is_core/rest/paginators.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/rest/resource.py` & `skip_django_is_core-2.25.1/is_core/rest/resource.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/site.py` & `skip_django_is_core-2.25.1/is_core/site.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/css/app.css` & `skip_django_is_core-2.25.1/is_core/static/is_core/css/app.css`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.eot` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.svg` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.ttf` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.woff` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.woff2` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.eot` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.svg` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.ttf` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.woff` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.woff2` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.eot` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.svg` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.ttf` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.woff` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.woff2` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.eot` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/icon-works-webfont.eot`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.svg` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/icon-works-webfont.svg`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.ttf` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/icon-works-webfont.ttf`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.woff` & `skip_django_is_core-2.25.1/is_core/static/is_core/fonts/icon-works-webfont.woff`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/images/arrow.png` & `skip_django_is_core-2.25.1/is_core/static/is_core/images/arrow.png`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/images/cal.png` & `skip_django_is_core-2.25.1/is_core/static/is_core/images/cal.png`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/images/select-arrow.png` & `skip_django_is_core-2.25.1/is_core/static/is_core/images/select-arrow.png`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/static/is_core/js/app.js` & `skip_django_is_core-2.25.1/is_core/static/is_core/js/app.js`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/base.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/base.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_field.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/default_field.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_fieldset.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/default_fieldset.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_form.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/default_form.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/inline_table.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/inline_table.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/model_default_form.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/model_default_form.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/responsive_inline_formset.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/responsive_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/responsive_inline_objects.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/responsive_inline_objects.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/stacked_inline_formset.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/stacked_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/tabular_inline_formset.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/tabular_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/tabular_inline_objects.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/forms/tabular_inline_objects.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/base_table.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/base_table.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/default_form.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/default_form.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/detail_form.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/detail_form.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/objects.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/objects.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/readonly_fieldset.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/generic_views/readonly_fieldset.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/logged_out.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/logged_out.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/login.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/login.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templates/is_core/menu/menu.html` & `skip_django_is_core-2.25.1/is_core/templates/is_core/menu/menu.html`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templatetags/forms.py` & `skip_django_is_core-2.25.1/is_core/templatetags/forms.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templatetags/menu.py` & `skip_django_is_core-2.25.1/is_core/templatetags/menu.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templatetags/permissions.py` & `skip_django_is_core-2.25.1/is_core/templatetags/permissions.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/templatetags/utils.py` & `skip_django_is_core-2.25.1/is_core/templatetags/utils.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/tests/crawler.py` & `skip_django_is_core-2.25.1/is_core/tests/crawler.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/tests/data_generator_test_case.py` & `skip_django_is_core-2.25.1/is_core/tests/data_generator_test_case.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/tests/factory/fields.py` & `skip_django_is_core-2.25.1/is_core/tests/factory/fields.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/tests/rest_generic_test_cases.py` & `skip_django_is_core-2.25.1/is_core/tests/rest_generic_test_cases.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/tests/ui_generic_test_cases.py` & `skip_django_is_core-2.25.1/is_core/tests/ui_generic_test_cases.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/utils/__init__.py` & `skip_django_is_core-2.25.1/is_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/utils/decorators.py` & `skip_django_is_core-2.25.1/is_core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/utils/field_api.py` & `skip_django_is_core-2.25.1/is_core/utils/field_api.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/is_core/utils/models.py` & `skip_django_is_core-2.25.1/is_core/utils/models.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/setup.py` & `skip_django_is_core-2.25.1/setup.py`

 * *Files identical despite different names*

### Comparing `skip_django_is_core-2.25.0/skip_django_is_core.egg-info/PKG-INFO` & `skip_django_is_core-2.25.1/skip_django_is_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-is-core
-Version: 2.25.0
+Version: 2.25.1
 Summary: Information systems core.
 Home-page: https://github.com/skip-pay/django-is-core
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,admin,information systems,REST
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip_django_is_core-2.25.0/skip_django_is_core.egg-info/SOURCES.txt` & `skip_django_is_core-2.25.1/skip_django_is_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

