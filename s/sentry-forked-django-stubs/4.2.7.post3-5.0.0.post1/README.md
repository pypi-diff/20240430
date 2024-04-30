# Comparing `tmp/sentry-forked-django-stubs-4.2.7.post3.tar.gz` & `tmp/sentry_forked_django_stubs-5.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-forked-django-stubs-4.2.7.post3.tar", last modified: Wed Feb  7 19:18:29 2024, max compression
+gzip compressed data, was "sentry_forked_django_stubs-5.0.0.post1.tar", last modified: Tue Apr 30 13:25:05 2024, max compression
```

## Comparing `sentry-forked-django-stubs-4.2.7.post3.tar` & `sentry_forked_django_stubs-5.0.0.post1.tar`

### file list

```diff
@@ -1,839 +1,838 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.501494 sentry-forked-django-stubs-4.2.7.post3/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-02-07 19:18:29.501494 sentry-forked-django-stubs-4.2.7.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15935 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.377495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.377495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/apps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/apps/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/apps/registry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.377495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17261 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/global_settings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.377495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/locale/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/locale/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.377495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/urls/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/urls/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/urls/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/urls/static.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.377495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.381495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/forms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.381495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/sites.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.381495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/admin_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/admin_modify.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/admin_urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/log.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/tests.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.385495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/views/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/views/autocomplete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/views/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/views/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/widgets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.385495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/middleware.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.389495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/backends.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/base_user.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/context_processors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/forms.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.389495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/handlers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/handlers/modwsgi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/hashers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.389495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/management/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.389495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/management/commands/changepassword.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.389495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/password_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/tokens.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/validators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.389495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/forms.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.389495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/management/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.393495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.393495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.393495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/forms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.393495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/sitemaps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.393495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/templatetags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/flatpages/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.393495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.397495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/admin/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/admin/widgets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/apps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.397495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.397495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.397495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/operations.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.397495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.401495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.401495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/const.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.401495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.405495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/aggregates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/lookups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/proxy.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.405495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/sql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/sql/conversion.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/feeds.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.405495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/forms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/forms/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/forms/widgets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.409495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/datasource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/driver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/envelope.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/feature.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/field.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/geometries.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/geomtype.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/layer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/libgdal.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.409495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.409495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/raster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/raster/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/raster/band.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/raster/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/raster/const.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/raster/source.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/srs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.409495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geoip2/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geoip2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geoip2/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geoip2/resources.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geometry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.413495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/collections.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/coordseq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/io.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/libgeos.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/linestring.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/mutable_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/point.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/polygon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prepared.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.413495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/geom.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/io.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/topology.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/measure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/ptr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.413495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/serializers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/serializers/geojson.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/shortcuts.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.413495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/sitemaps/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/sitemaps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/sitemaps/kml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/sitemaps/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.417495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/utils/layermapping.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/utils/ogrinfo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/utils/ogrinspect.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/utils/srs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.417495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/humanize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/humanize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/humanize/apps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.417495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/humanize/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/humanize/templatetags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/humanize/templatetags/humanize.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.417495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/context_processors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.417495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/storage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/storage/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/storage/cookie.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/storage/fallback.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/storage/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.421495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.421495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/aggregates/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/aggregates/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/aggregates/general.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/aggregates/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/aggregates/statistics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/expressions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.425495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/array.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/citext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/hstore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/jsonb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/ranges.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.425495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/forms/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/forms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/forms/array.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/forms/hstore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/forms/jsonb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/forms/ranges.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/indexes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/lookups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/serializers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/validators.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.425495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/redirects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/redirects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/redirects/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/redirects/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/redirects/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.425495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/redirects/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/redirects/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/redirects/models.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.425495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/apps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.429495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/cached_db.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/db.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/file.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/signed_cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/base_session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.429495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.429495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.429495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/serializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.429495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/apps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.429495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.429495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.429495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/management.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/managers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.433495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/requests.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/shortcuts.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.433495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/finders.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/handlers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.433495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.433495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/storage.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.433495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/syndication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/syndication/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/syndication/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/syndication/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.437495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/asgi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.437495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.437495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/db.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/filebased.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/locmem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/memcached.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.437495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/async_checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/caches.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.441495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/compatibility/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/compatibility/django_4_0.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/database.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/files.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/messages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/model_checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/registry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.441495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/security/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/security/csrf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/security/sessions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/templates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/translation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.441495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/locks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/move.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.441495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/filesystem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/handler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/memory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/temp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/uploadedfile.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/uploadhandler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.445495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/asgi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/wsgi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.445495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.445495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/console.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/filebased.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/locmem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/smtp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.445495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/color.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.449495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/check.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/compilemessages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/createcachetable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/dbshell.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/diffsettings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/dumpdata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/flush.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/inspectdb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/loaddata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/makemessages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/makemigrations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/migrate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/runserver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/sendtestemail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/shell.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/showmigrations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/sqlflush.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/sqlmigrate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/sqlsequencereset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/squashmigrations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/startapp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/startproject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/test.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/testserver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/sql.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/templates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/paginator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.453495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/json.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/jsonl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/python.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/pyyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/xml_serializer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.453495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/servers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/servers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/servers/basehttp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/signing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/validators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/wsgi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.453495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.453495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.453495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/ddl_references.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.453495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/dummy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/dummy/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/dummy/features.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.457495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/compiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/validation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.457495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/validation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.461495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/signals.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.461495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.465494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/autodetector.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/graph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/migration.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.465494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/special.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/optimizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/questioner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/recorder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/state.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/writer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.465494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/aggregates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/deletion.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/expressions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.469494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/
--rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/files.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/json.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/related.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/related_descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/related_lookups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/reverse_related.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.469494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/comparison.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/math.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/text.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/window.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/indexes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/lookups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/manager.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/query_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/signals.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.469494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/compiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/datastructures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/subqueries.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/where.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.473494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/dispatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/dispatch/dispatcher.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.473494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/boundfield.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20670 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/forms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/formsets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/renderers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/widgets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.473494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/cookie.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/multipartparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.473494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/clickjacking.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/csrf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/gzip.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/locale.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/shortcuts.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.477495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.477495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/django.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/jinja2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/context_processors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/defaultfilters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/defaulttags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/engine.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/library.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loader_tags.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.481495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/app_directories.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/cached.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/filesystem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/locmem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/smartif.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.481495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/l10n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/static.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/tz.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.481495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/selenium.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/testcases.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.481495 sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/conf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/resolvers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.489494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/_os.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/archive.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/asyncio.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/autoreload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/baseconv.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/datastructures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/dateformat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/dateparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/dates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/datetime_safe.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/deconstruct.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/deprecation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/duration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/encoding.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/feedgenerator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/formats.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/functional.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/hashable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/inspect.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/ipv6.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/itercompat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/jslex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/log.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/lorem_ipsum.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/module_loading.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/numberformat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/regex_helper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/safestring.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/termcolors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/text.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/timesince.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/timezone.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/topological_sort.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.493494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/reloader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/template.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/trans_null.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/trans_real.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/xmlutils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.493494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/csrf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/debug.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.493494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/clickjacking.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/csrf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/gzip.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/vary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/defaults.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.493494 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/dates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/detail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/edit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/static.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.497494 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.497494 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/django/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.497494 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/lib/fullnames.py
--rw-r--r--   0 runner    (1001) docker     (127)    16996 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.501494 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/init_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    24685 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/manytomany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    48193 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/orm_lookups.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/querysets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.501494 sentry-forked-django-stubs-4.2.7.post3/sentry_forked_django_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-02-07 19:18:29.000000 sentry-forked-django-stubs-4.2.7.post3/sentry_forked_django_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30583 2024-02-07 19:18:29.000000 sentry-forked-django-stubs-4.2.7.post3/sentry_forked_django_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 19:18:29.000000 sentry-forked-django-stubs-4.2.7.post3/sentry_forked_django_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-07 19:18:29.000000 sentry-forked-django-stubs-4.2.7.post3/sentry_forked_django_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-07 19:18:29.000000 sentry-forked-django-stubs-4.2.7.post3/sentry_forked_django_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 19:18:29.501494 sentry-forked-django-stubs-4.2.7.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:18:29.501494 sentry-forked-django-stubs-4.2.7.post3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-02-07 19:18:16.000000 sentry-forked-django-stubs-4.2.7.post3/tests/test_error_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.359050 sentry_forked_django_stubs-5.0.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17120 2024-04-30 13:25:05.359050 sentry_forked_django_stubs-5.0.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15842 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.251050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.251050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/apps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/apps/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/apps/registry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.255050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17261 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/global_settings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.255050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/locale/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.255050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/urls/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/urls/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/urls/static.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.255050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.255050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.255050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/sites.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.259050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/admin_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/admin_modify.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/admin_urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/tests.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.259050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/views/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/views/autocomplete.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/views/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/views/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.259050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/middleware.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.263050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/backends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/base_user.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/forms.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.263050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/handlers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/handlers/modwsgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/hashers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.263050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.263050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/management/commands/changepassword.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.263050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/password_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/tokens.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.263050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/forms.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.263050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.267050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.267050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.267050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.267050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/sitemaps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.267050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/flatpages/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.267050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.267050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/admin/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/admin/widgets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.271050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.271050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.271050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/operations.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.271050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.271050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.275050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/const.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.275050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.275050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/aggregates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/proxy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.275050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/sql/conversion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/feeds.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.279050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/forms/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/forms/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.279050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/datasource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/driver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/envelope.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/feature.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/field.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/geometries.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/geomtype.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/layer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/libgdal.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.279050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.283050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/raster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/raster/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/raster/band.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/raster/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/raster/const.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/raster/source.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/srs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.283050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geoip2/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geoip2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geoip2/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geoip2/resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geometry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.283050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/coordseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/io.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/libgeos.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/linestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/mutable_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/point.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/polygon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prepared.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.287050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/geom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/io.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/topology.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/measure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/ptr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.287050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/serializers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/serializers/geojson.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.287050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/sitemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/sitemaps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/sitemaps/kml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/sitemaps/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.287050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/utils/layermapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/utils/ogrinfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/utils/ogrinspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/utils/srs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.287050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/humanize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/humanize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/humanize/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.287050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/humanize/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/humanize/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/humanize/templatetags/humanize.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.291050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.291050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/storage/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/storage/cookie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/storage/fallback.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/storage/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.291050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.295050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/aggregates/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/aggregates/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/aggregates/general.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/aggregates/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/aggregates/statistics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/constraints.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.295050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/citext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/hstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/jsonb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/ranges.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.295050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/forms/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/forms/hstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/forms/jsonb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/forms/ranges.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/indexes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/serializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/validators.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.295050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/redirects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/redirects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/redirects/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/redirects/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/redirects/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.295050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/redirects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/redirects/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/redirects/models.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.299050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.299050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/cached_db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/signed_cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/base_session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.299050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.299050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.299050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/serializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.299050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.299050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.299050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.303050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/management.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/managers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.303050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/requests.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.303050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/finders.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/handlers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.303050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.303050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/storage.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.303050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/syndication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/syndication/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/syndication/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/syndication/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.307050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/asgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.307050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.307050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/filebased.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/memcached.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.307050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/async_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/caches.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.307050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/compatibility/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/compatibility/django_4_0.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/files.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/messages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/model_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/registry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.307050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/security/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/security/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/security/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/templates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/translation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.311050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/locks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/move.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.311050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/filesystem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/memory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/temp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/uploadedfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/uploadhandler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.311050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/asgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/wsgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.311050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.315050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/console.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/filebased.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/smtp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.315050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/color.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.319050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/compilemessages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/createcachetable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/dbshell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/diffsettings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/dumpdata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/flush.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/inspectdb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/loaddata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/makemessages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/makemigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/migrate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/runserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/sendtestemail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/shell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/showmigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/sqlflush.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/sqlmigrate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/sqlsequencereset.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/squashmigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/startapp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/startproject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/testserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/sql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/templates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/paginator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.319050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/jsonl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/python.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/pyyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/xml_serializer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.319050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/servers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/servers/basehttp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/signing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/wsgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.319050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.319050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.323050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/ddl_references.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.323050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/dummy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/dummy/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/dummy/features.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.323050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/compiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/validation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.327050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/validation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.327050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/signals.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.327050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.331050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/autodetector.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/migration.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.331050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/special.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/optimizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/questioner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/recorder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/state.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/writer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.331050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/aggregates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/deletion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/expressions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.335050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)    21728 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/files.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/related.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/related_descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/related_lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/reverse_related.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.335050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/comparison.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/window.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/indexes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/query_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/signals.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.335050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/compiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/datastructures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/subqueries.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/where.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.335050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/dispatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/dispatch/dispatcher.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.339050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/boundfield.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20629 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/formsets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/renderers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.339050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/cookie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/multipartparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.339050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/clickjacking.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/gzip.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/locale.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.339050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.343050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/django.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/jinja2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/defaultfilters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/defaulttags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/engine.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/library.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loader_tags.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.343050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/app_directories.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/cached.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/filesystem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/smartif.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.343050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/l10n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/tz.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.343050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/selenium.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/testcases.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.347050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/conf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/resolvers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.351050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/_os.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/archive.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/asyncio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/autoreload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/baseconv.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/datastructures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/dateformat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/dateparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/dates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/datetime_safe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/deconstruct.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/deprecation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/duration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/encoding.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/feedgenerator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/formats.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/functional.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/hashable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/inspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/ipv6.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/itercompat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/jslex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/lorem_ipsum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/module_loading.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/numberformat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/regex_helper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/safestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/termcolors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/timesince.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/timezone.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/topological_sort.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.351050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/reloader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/template.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/trans_null.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/trans_real.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/xmlutils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.351050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/debug.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.355050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/clickjacking.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/gzip.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/vary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/defaults.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.355050 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/dates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/edit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/static.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.355050 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.355050 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/django/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.355050 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/lib/fullnames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.359050 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/init_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24664 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/manytomany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47970 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/orm_lookups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/querysets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.359050 sentry_forked_django_stubs-5.0.0.post1/sentry_forked_django_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17120 2024-04-30 13:25:05.000000 sentry_forked_django_stubs-5.0.0.post1/sentry_forked_django_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30537 2024-04-30 13:25:05.000000 sentry_forked_django_stubs-5.0.0.post1/sentry_forked_django_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:25:05.000000 sentry_forked_django_stubs-5.0.0.post1/sentry_forked_django_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 13:25:05.000000 sentry_forked_django_stubs-5.0.0.post1/sentry_forked_django_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 13:25:05.000000 sentry_forked_django_stubs-5.0.0.post1/sentry_forked_django_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:25:05.359050 sentry_forked_django_stubs-5.0.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:25:05.359050 sentry_forked_django_stubs-5.0.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-30 13:25:01.000000 sentry_forked_django_stubs-5.0.0.post1/tests/test_error_handling.py
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/LICENSE.md` & `sentry_forked_django_stubs-5.0.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/PKG-INFO` & `sentry_forked_django_stubs-5.0.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-forked-django-stubs
-Version: 4.2.7.post3
+Version: 5.0.0.post1
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -21,21 +21,21 @@
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
-Requires-Dist: django-stubs-ext>=4.2.7
+Requires-Dist: django-stubs-ext>=4.2.5
 Requires-Dist: tomli; python_version < "3.11"
 Requires-Dist: typing-extensions
 Requires-Dist: types-pytz
 Requires-Dist: types-PyYAML
 Provides-Extra: compatible-mypy
-Requires-Dist: mypy~=1.7.0; extra == "compatible-mypy"
+Requires-Dist: mypy~=1.6.0; extra == "compatible-mypy"
 
 sentry-forked-django-stubs
 ==========================
 
 ### new release
 
 make a new branch for the fork of an upstream tag:
@@ -47,15 +47,15 @@
 git checkout 1.2.3 -b sentry-1.2.3
 ```
 
 - cherry-pick the craft / release commit(s) into your branch from `master`
 - cherry-pick relevant commit(s) from previous releases
 
 releases are done through craft in the release.yml workflow -- make sure to
-target your particular branch with a `.#` release postfix (like `1.2.3.0`)
+target your particular branch with a `-#` release postfix (like `1.2.3-1`)
 
 ___
 
 <img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
@@ -102,15 +102,14 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
-| 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/README.md` & `sentry_forked_django_stubs-5.0.0.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 git checkout 1.2.3 -b sentry-1.2.3
 ```
 
 - cherry-pick the craft / release commit(s) into your branch from `master`
 - cherry-pick relevant commit(s) from previous releases
 
 releases are done through craft in the release.yml workflow -- make sure to
-target your particular branch with a `.#` release postfix (like `1.2.3.0`)
+target your particular branch with a `-#` release postfix (like `1.2.3-1`)
 
 ___
 
 <img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
@@ -67,15 +67,14 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
-| 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/apps/config.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/apps/config.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/apps/registry.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/apps/registry.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/global_settings.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/global_settings.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/conf/urls/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/conf/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/checks.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/checks.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/decorators.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/decorators.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Callable, Sequence
 from typing import Any, TypeVar, overload
 
 from django.contrib.admin import ModelAdmin
 from django.contrib.admin.sites import AdminSite
-from django.db.models import QuerySet
+from django.db.models import Combinable, QuerySet
 from django.db.models.base import Model
-from django.db.models.expressions import BaseExpression, Combinable
+from django.db.models.expressions import BaseExpression
 from django.http import HttpRequest, HttpResponseBase
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 _Model = TypeVar("_Model", bound=Model)
 _ModelAdmin = TypeVar("_ModelAdmin", bound=ModelAdmin)
 _Request = TypeVar("_Request", bound=HttpRequest)
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/filters.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/filters.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/helpers.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/helpers.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,16 @@
         has_view_permission: bool = ...,
     ) -> None: ...
     def __iter__(self) -> Iterator[InlineAdminForm]: ...
     def fields(self) -> Iterator[dict[str, dict[str, bool] | bool | Widget | str]]: ...
     def inline_formset_data(self) -> str: ...
     @property
     def forms(self) -> list[BaseForm]: ...
-    def non_form_errors(self) -> ErrorList: ...
+    @property
+    def non_form_errors(self) -> Callable[[], ErrorList]: ...
     @property
     def media(self) -> Media: ...
 
 class InlineAdminForm(AdminForm):
     formset: Any
     original: bool | None
     show_url: bool
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/options.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/options.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -70,30 +70,29 @@
     | tuple[Field | str, type[FieldListFilter]]
     | list[Field | str | type[FieldListFilter]]
 )
 
 # Generic type specifically for models, for use in BaseModelAdmin and subclasses
 # https://github.com/typeddjango/django-stubs/issues/482
 _ModelT = TypeVar("_ModelT", bound=Model)
-_DisplayT: TypeAlias = _ListOrTuple[str | Callable[[_ModelT], str | bool]]
 
 class BaseModelAdmin(Generic[_ModelT]):
-    autocomplete_fields: _ListOrTuple[str]
-    raw_id_fields: _ListOrTuple[str]
+    autocomplete_fields: Sequence[str]
+    raw_id_fields: Sequence[str]
     fields: _FieldGroups | None
-    exclude: _ListOrTuple[str] | None
+    exclude: Sequence[str] | None
     fieldsets: _FieldsetSpec | None
     form: type[forms.ModelForm[_ModelT]]
-    filter_vertical: _ListOrTuple[str]
-    filter_horizontal: _ListOrTuple[str]
+    filter_vertical: Sequence[str]
+    filter_horizontal: Sequence[str]
     radio_fields: Mapping[str, _Direction]
     prepopulated_fields: dict[str, Sequence[str]]
     formfield_overrides: Mapping[type[Field], Mapping[str, Any]]
-    readonly_fields: _ListOrTuple[str]
-    ordering: _ListOrTuple[str] | None
+    readonly_fields: Sequence[str]
+    ordering: Sequence[str] | None
     sortable_by: _ListOrTuple[str] | None
     view_on_site: bool | Callable[[_ModelT], str]
     show_full_result_count: bool
     checks_class: Any
     model: type[_ModelT]
     opts: Options[_ModelT]
     admin_site: AdminSite
@@ -104,55 +103,56 @@
     def get_field_queryset(self, db: str | None, db_field: RelatedField, request: HttpRequest) -> QuerySet | None: ...
     def formfield_for_foreignkey(
         self, db_field: ForeignKey, request: HttpRequest, **kwargs: Any
     ) -> ModelChoiceField: ...
     def formfield_for_manytomany(
         self, db_field: ManyToManyField, request: HttpRequest, **kwargs: Any
     ) -> ModelMultipleChoiceField | None: ...
-    def get_autocomplete_fields(self, request: HttpRequest) -> _ListOrTuple[str]: ...
+    def get_autocomplete_fields(self, request: HttpRequest) -> Sequence[str]: ...
     def get_view_on_site_url(self, obj: _ModelT | None = ...) -> str | None: ...
     def get_empty_value_display(self) -> SafeString: ...
-    def get_exclude(self, request: HttpRequest, obj: _ModelT | None = ...) -> _ListOrTuple[str] | None: ...
+    def get_exclude(self, request: HttpRequest, obj: _ModelT | None = ...) -> Sequence[str] | None: ...
     def get_fields(self, request: HttpRequest, obj: _ModelT | None = ...) -> _FieldGroups: ...
     def get_fieldsets(self, request: HttpRequest, obj: _ModelT | None = ...) -> _FieldsetSpec: ...
     def get_inlines(self, request: HttpRequest, obj: _ModelT | None) -> list[type[InlineModelAdmin]]: ...
-    def get_ordering(self, request: HttpRequest) -> _ListOrTuple[str]: ...
-    def get_readonly_fields(self, request: HttpRequest, obj: _ModelT | None = ...) -> _ListOrTuple[str]: ...
+    def get_ordering(self, request: HttpRequest) -> Sequence[str]: ...
+    def get_readonly_fields(self, request: HttpRequest, obj: _ModelT | None = ...) -> Sequence[str]: ...
     def get_prepopulated_fields(self, request: HttpRequest, obj: _ModelT | None = ...) -> dict[str, Sequence[str]]: ...
     def get_queryset(self, request: HttpRequest) -> QuerySet[_ModelT]: ...
-    def get_sortable_by(self, request: HttpRequest) -> _DisplayT: ...
+    def get_sortable_by(self, request: HttpRequest) -> Sequence[str]: ...
     def lookup_allowed(self, lookup: str, value: str) -> bool: ...
     def to_field_allowed(self, request: HttpRequest, to_field: str) -> bool: ...
     def has_add_permission(self, request: HttpRequest) -> bool: ...
     def has_change_permission(self, request: HttpRequest, obj: _ModelT | None = ...) -> bool: ...
     def has_delete_permission(self, request: HttpRequest, obj: _ModelT | None = ...) -> bool: ...
     def has_view_permission(self, request: HttpRequest, obj: _ModelT | None = ...) -> bool: ...
     def has_view_or_change_permission(self, request: HttpRequest, obj: _ModelT | None = ...) -> bool: ...
     def has_module_permission(self, request: HttpRequest) -> bool: ...
 
+_DisplayT: TypeAlias = _ListOrTuple[str | Callable[[_ModelT], str | bool]]
 _ModelAdmin = TypeVar("_ModelAdmin", bound=ModelAdmin)
 _ActionCallable: TypeAlias = Callable[[_ModelAdmin, HttpRequest, QuerySet[_ModelT]], HttpResponseBase | None]
 
 class ModelAdmin(BaseModelAdmin[_ModelT]):
     list_display: _DisplayT
     list_display_links: _DisplayT | None
     list_filter: _ListOrTuple[_ListFilterT]
-    list_select_related: bool | _ListOrTuple[str]
+    list_select_related: bool | Sequence[str]
     list_per_page: int
     list_max_show_all: int
-    list_editable: _ListOrTuple[str]
-    search_fields: _ListOrTuple[str]
+    list_editable: Sequence[str]
+    search_fields: Sequence[str]
     search_help_text: _StrOrPromise | None
     date_hierarchy: str | None
     save_as: bool
     save_as_continue: bool
     save_on_top: bool
     paginator: type
     preserve_filters: bool
-    inlines: _ListOrTuple[type[InlineModelAdmin]]
+    inlines: Sequence[type[InlineModelAdmin]]
     add_form_template: _TemplateForResponseT | None
     change_form_template: _TemplateForResponseT | None
     change_list_template: _TemplateForResponseT | None
     delete_confirmation_template: _TemplateForResponseT | None
     delete_selected_confirmation_template: _TemplateForResponseT | None
     object_history_template: _TemplateForResponseT | None
     popup_response_template: _TemplateForResponseT | None
@@ -198,17 +198,17 @@
     def get_actions(self, request: HttpRequest) -> dict[str, tuple[Callable[..., str], str, str] | None]: ...
     def get_action_choices(
         self, request: HttpRequest, default_choices: list[tuple[str, str]] = ...
     ) -> list[tuple[str, str]]: ...
     def get_action(self, action: Callable | str) -> tuple[Callable[..., str], str, str] | None: ...
     def get_list_display(self, request: HttpRequest) -> _DisplayT: ...
     def get_list_display_links(self, request: HttpRequest, list_display: _DisplayT) -> _DisplayT: ...
-    def get_list_filter(self, request: HttpRequest) -> _ListOrTuple[_ListFilterT]: ...
-    def get_list_select_related(self, request: HttpRequest) -> bool | _ListOrTuple[str]: ...
-    def get_search_fields(self, request: HttpRequest) -> _ListOrTuple[str]: ...
+    def get_list_filter(self, request: HttpRequest) -> Sequence[_ListFilterT]: ...
+    def get_list_select_related(self, request: HttpRequest) -> bool | Sequence[str]: ...
+    def get_search_fields(self, request: HttpRequest) -> Sequence[str]: ...
     def get_search_results(
         self, request: HttpRequest, queryset: QuerySet, search_term: str
     ) -> tuple[QuerySet[_ModelT], bool]: ...
     def get_preserved_filters(self, request: HttpRequest) -> str: ...
     def _get_edited_object_pks(self, request: HttpRequest, prefix: str) -> list[str]: ...
     def _get_list_editable_queryset(self, request: HttpRequest, prefix: str) -> QuerySet[_ModelT]: ...
     def construct_change_message(
@@ -261,15 +261,15 @@
     ) -> HttpResponse: ...
     def change_view(
         self, request: HttpRequest, object_id: str, form_url: str = ..., extra_context: dict[str, Any] | None = ...
     ) -> HttpResponse: ...
     def changelist_view(self, request: HttpRequest, extra_context: dict[str, Any] | None = ...) -> HttpResponse: ...
     def get_deleted_objects(
         self, objs: Sequence[_ModelT] | QuerySet[_ModelT], request: HttpRequest
-    ) -> tuple[list[str], dict[str, int], set[str], list[str]]: ...
+    ) -> tuple[list[Model], dict[str, int], set[str], list[str]]: ...
     def delete_view(
         self, request: HttpRequest, object_id: str, extra_context: dict[str, Any] | None = ...
     ) -> HttpResponse: ...
     def history_view(
         self, request: HttpRequest, object_id: str, extra_context: dict[str, Any] | None = ...
     ) -> HttpResponse: ...
     def get_formset_kwargs(
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/sites.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/sites.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/admin_list.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/admin_list.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/admin_modify.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/admin_modify.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/templatetags/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/templatetags/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/tests.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/tests.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/utils.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,66 @@
 import datetime
-from collections import defaultdict
 from collections.abc import Callable, Iterable, Sequence
-from typing import Any, Literal, TypeVar, overload
+from typing import Any, Literal, overload
 from uuid import UUID
 
-from _typeshed import Unused
 from django.contrib.admin.options import BaseModelAdmin
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth.forms import AdminPasswordChangeForm
 from django.db.models.base import Model
 from django.db.models.deletion import Collector
 from django.db.models.fields import Field, reverse_related
 from django.db.models.options import Options
 from django.db.models.query import QuerySet
 from django.forms.forms import BaseForm
 from django.forms.formsets import BaseFormSet
 from django.http.request import HttpRequest
 from django.utils.datastructures import _IndexableCollection
 from typing_extensions import TypedDict
 
-_T = TypeVar("_T")
-
 class FieldIsAForeignKeyColumnName(Exception): ...
 
 def lookup_spawns_duplicates(opts: Options, lookup_path: str) -> bool: ...
 def prepare_lookup_value(key: str, value: datetime.datetime | str) -> bool | datetime.datetime | str: ...
 def quote(s: int | str | UUID) -> str: ...
 def unquote(s: str) -> str: ...
 def flatten(fields: Any) -> list[Callable | str]: ...
 def flatten_fieldsets(fieldsets: Any) -> list[Callable | str]: ...
 def get_deleted_objects(
     objs: Sequence[Model | None] | QuerySet[Model], request: HttpRequest, admin_site: AdminSite
-) -> tuple[list[str], dict[str, int], set[str], list[str]]: ...
+) -> tuple[list[Model], dict[str, int], set[str], list[str]]: ...
 
 class NestedObjects(Collector):
-    edges: dict[Model, list[Model]]
-    protected: set[Model]
-    model_objs: defaultdict[str, set[Model]]
+    data: dict[type[Model], set[Model] | list[Model]]
+    dependencies: dict[Any, Any]
+    fast_deletes: list[Any]
+    field_updates: dict[Any, Any]
+    using: str
+    edges: Any
+    protected: Any
+    model_objs: Any
+    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def add_edge(self, source: Model | None, target: Model) -> None: ...
-    def collect(  # type: ignore[override]
-        self,
-        objs: _IndexableCollection[Model | None],
-        source: type[Model] | None = ...,
-        source_attr: str | None = ...,
-        *,
-        nullable: bool = ...,
-        collect_related: bool = ...,
-        reverse_dependency: bool = ...,
-        keep_parents: bool = ...,
-        fail_on_restricted: bool = ...,
-    ) -> None: ...
     def related_objects(
         self, related_model: type[Model], related_fields: Iterable[Field], objs: _IndexableCollection[Model]
     ) -> QuerySet[Model]: ...
-    @overload
-    def nested(self, format_callback: None = None) -> list[Model]: ...
-    @overload
-    def nested(self, format_callback: Callable[[Model], _T]) -> list[_T]: ...
-    def can_fast_delete(self, *args: Unused, **kwargs: Unused) -> Literal[False]: ...
+    def nested(self, format_callback: Callable = ...) -> list[Any]: ...
+    def can_fast_delete(self, *args: Any, **kwargs: Any) -> bool: ...
 
 class _ModelFormatDict(TypedDict):
     verbose_name: str
     verbose_name_plural: str
 
 def model_format_dict(obj: Model | type[Model] | QuerySet | Options[Model]) -> _ModelFormatDict: ...
 def model_ngettext(obj: Options | QuerySet, n: int | None = ...) -> str: ...
 def lookup_field(
     name: Callable | str, obj: Model, model_admin: BaseModelAdmin | None = ...
 ) -> tuple[Field | None, str | None, Any]: ...
 @overload
-def label_for_field(  # type: ignore[overload-overlap]
+def label_for_field(  # type: ignore[misc]
     name: Callable | str,
     model: type[Model],
     model_admin: BaseModelAdmin | None = ...,
     return_attr: Literal[True] = ...,
     form: BaseForm | None = ...,
 ) -> tuple[str, Callable | str | None]: ...
 @overload
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/views/main.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/views/main.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admin/widgets.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admin/widgets.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/admindocs/views.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/admindocs/views.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/admin.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/admin.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/backends.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/backends.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/base_user.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/base_user.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/context_processors.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/decorators.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/decorators.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/forms.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/forms.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/hashers.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/hashers.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/middleware.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/middleware.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/mixins.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/mixins.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/password_validation.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/password_validation.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/tokens.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/tokens.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/auth/views.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/auth/views.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/admin.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/admin.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/fields.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/forms.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/forms.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/management/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/contenttypes/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/contenttypes/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/admin/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/admin/options.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/admin/options.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/features.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/base/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/base/operations.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Any
 
-from django.utils.functional import cached_property
-
 class BaseSpatialOperations:
     postgis: bool
     spatialite: bool
     mysql: bool
     oracle: bool
     spatial_version: Any
     select: str
-    @cached_property
+    @property
     def select_extent(self) -> str: ...
     geography: bool
     geometry: bool
     disallowed_aggregates: Any
     geom_func_prefix: str
     function_names: Any
     unsupported_functions: set[str]
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/features.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/features.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from typing import Any
 
 from django.contrib.gis.db.backends.base.features import BaseSpatialFeatures
 from django.db.backends.mysql.features import DatabaseFeatures as MySQLDatabaseFeatures
-from django.utils.functional import cached_property
 
 class DatabaseFeatures(BaseSpatialFeatures, MySQLDatabaseFeatures):
     has_spatialrefsys_table: bool
     supports_add_srs_entry: bool
     supports_distance_geodetic: bool
     supports_length_geodetic: bool
     supports_area_geodetic: bool
     supports_transform: bool
     supports_null_geometries: bool
     supports_num_points_poly: bool
     @property
     def empty_intersection_returns_none(self) -> bool: ...
-    @cached_property
+    @property
     def supports_geometry_field_unique_index(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def django_test_skips(self) -> dict[str, Any]: ...  # type: ignore[override]
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from collections.abc import Callable
 from typing import Any
 
 from django.contrib.gis.db.backends.base.operations import BaseSpatialOperations
 from django.contrib.gis.db.backends.utils import SpatialOperator
 from django.contrib.gis.geos.geometry import GEOSGeometryBase
 from django.db.backends.mysql.operations import DatabaseOperations
-from django.utils.functional import cached_property
 
 class MySQLOperations(BaseSpatialOperations, DatabaseOperations):
     name: str
     geom_func_prefix: str
     Adapter: Any
-    @cached_property
+    @property
     def mariadb(self) -> bool: ...
-    @cached_property
+    @property
     def mysql(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def select(self) -> str: ...  # type: ignore[override]
-    @cached_property
+    @property
     def from_text(self) -> str: ...  # type: ignore[override]
-    @cached_property
+    @property
     def gis_operators(self) -> dict[str, SpatialOperator]: ...
     disallowed_aggregates: Any
-    @cached_property
+    @property
     def unsupported_functions(self) -> set[str]: ...  # type: ignore[override]
     def geo_db_type(self, f: Any) -> Any: ...
     def get_distance(self, f: Any, value: Any, lookup_type: Any) -> list[Any]: ...
     def get_geometry_converter(self, expression: Any) -> Callable[[Any, Any, Any], GEOSGeometryBase | None]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/mysql/schema.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/oracle/schema.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/postgis/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from typing import Any, Literal
 
 from django.contrib.gis.db.backends.base.operations import BaseSpatialOperations
 from django.contrib.gis.db.backends.utils import SpatialOperator
-from django.contrib.gis.db.models.fields import GeometryField
 from django.db.backends.postgresql.operations import DatabaseOperations
 from django.db.models import Func
-from django.utils.functional import cached_property
 
 BILATERAL: Literal["bilateral"]
 
 class PostGISOperator(SpatialOperator):
     geography: Any
     raster: bool | Literal["bilateral"]
     def __init__(self, geography: bool = ..., raster: bool | Literal["bilateral"] = ..., **kwargs: Any) -> None: ...
     def check_raster(self, lookup: Any, template_params: Any) -> Any: ...
 
 class ST_Polygon(Func):
     function: str
     def __init__(self, expr: Any) -> None: ...
-    @cached_property
-    def output_field(self) -> GeometryField: ...
+    @property
+    def output_field(self) -> Any: ...
 
 class PostGISOperations(BaseSpatialOperations, DatabaseOperations):
     name: str
     postgis: bool
     geography: bool
     geom_func_prefix: str
     Adapter: Any
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any
 
 from django.contrib.gis.db.backends.base.operations import BaseSpatialOperations
 from django.contrib.gis.db.backends.utils import SpatialOperator
 from django.db.backends.sqlite3.operations import DatabaseOperations
-from django.utils.functional import cached_property
 
 class SpatialiteNullCheckOperator(SpatialOperator): ...
 
 class SpatiaLiteOperations(BaseSpatialOperations, DatabaseOperations):
     name: str
     spatialite: bool
     Adapter: Any
@@ -15,15 +14,15 @@
     extent: str
     makeline: str
     unionagg: str
     gis_operators: Any
     disallowed_aggregates: Any
     select: str
     function_names: Any
-    @cached_property
+    @property
     def unsupported_functions(self) -> set[str]: ...  # type: ignore[override]
     @property
     def spatial_version(self) -> Any: ...
     def geo_db_type(self, f: Any) -> None: ...
     def get_distance(self, f: Any, value: Any, lookup_type: Any) -> Any: ...
     def geos_version(self) -> Any: ...
     def proj_version(self) -> Any: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/backends/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/backends/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/aggregates.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/fields.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/functions.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/functions.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,88 @@
-from typing import Any, ClassVar
+from typing import Any
 
-from django.contrib.gis.db.models.fields import GeometryField
-from django.contrib.gis.db.models.sql.conversion import AreaField, DistanceField
 from django.db.backends.base.base import BaseDatabaseWrapper
-from django.db.models import BinaryField, BooleanField, FloatField, Func, IntegerField, TextField
+from django.db.models import Func
 from django.db.models import Transform as StandardTransform
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
-from django.utils.functional import cached_property
 
 NUMERIC_TYPES: Any
 
 class GeoFuncMixin:
     geom_param_pos: Any
     @property
     def geo_field(self) -> Any: ...
 
 class GeoFunc(GeoFuncMixin, Func): ...
 
 class GeomOutputGeoFunc(GeoFunc):
-    @cached_property
-    def output_field(self) -> GeometryField: ...
+    @property
+    def output_field(self) -> Any: ...
 
 class SQLiteDecimalToFloatMixin:
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class OracleToleranceMixin:
     tolerance: float
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Area(OracleToleranceMixin, GeoFunc):
     arity: int
-    @cached_property
-    def output_field(self) -> AreaField: ...
+    @property
+    def output_field(self) -> Any: ...
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Azimuth(GeoFunc):
-    output_field: ClassVar[FloatField]
+    output_field: Any
     arity: int
     geom_param_pos: Any
 
 class AsGeoJSON(GeoFunc):
-    output_field: ClassVar[TextField]
+    output_field: Any
     def __init__(
         self, expression: Any, bbox: bool = ..., crs: bool = ..., precision: int = ..., **extra: Any
     ) -> None: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class AsGML(GeoFunc):
     geom_param_pos: Any
-    output_field: ClassVar[TextField]
+    output_field: Any
     def __init__(self, expression: Any, version: int = ..., precision: int = ..., **extra: Any) -> None: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class AsKML(GeoFunc):
-    output_field: ClassVar[TextField]
+    output_field: Any
     def __init__(self, expression: Any, precision: int = ..., **extra: Any) -> None: ...
 
 class AsSVG(GeoFunc):
-    output_field: ClassVar[TextField]
+    output_field: Any
     def __init__(self, expression: Any, relative: bool = ..., precision: int = ..., **extra: Any) -> None: ...
 
 class AsWKB(GeoFunc):
-    output_field: ClassVar[BinaryField]
+    output_field: Any
     arity: int
 
 class AsWKT(GeoFunc):
-    output_field: ClassVar[TextField]
+    output_field: Any
     arity: int
 
 class BoundingCircle(OracleToleranceMixin, GeomOutputGeoFunc):
     def __init__(self, expression: Any, num_seg: int = ..., **extra: Any) -> None: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Centroid(OracleToleranceMixin, GeomOutputGeoFunc):
     arity: int
 
 class Difference(OracleToleranceMixin, GeomOutputGeoFunc):
     arity: int
     geom_param_pos: Any
 
 class DistanceResultMixin:
-    @cached_property
-    def output_field(self) -> DistanceField: ...
+    @property
+    def output_field(self) -> Any: ...
     def source_is_geography(self) -> Any: ...
 
 class Distance(DistanceResultMixin, OracleToleranceMixin, GeoFunc):
     geom_param_pos: Any
     spheroid: Any
     def __init__(self, expr1: Any, expr2: Any, spheroid: Any | None = ..., **extra: Any) -> None: ...
     def as_postgresql(
@@ -96,71 +93,71 @@
 class Envelope(GeomOutputGeoFunc):
     arity: int
 
 class ForcePolygonCW(GeomOutputGeoFunc):
     arity: int
 
 class FromWKB(GeoFunc):
-    output_field: ClassVar[GeometryField]
+    output_field: Any
     arity: int
 
 class FromWKT(GeoFunc):
-    output_field: ClassVar[GeometryField]
+    output_field: Any
     arity: int
 
 class GeoHash(GeoFunc):
-    output_field: ClassVar[TextField]
+    output_field: Any
     def __init__(self, expression: Any, precision: Any | None = ..., **extra: Any) -> None: ...
     def as_mysql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class GeometryDistance(GeoFunc):
-    output_field: ClassVar[FloatField]
+    output_field: Any
     arity: int
     function: str
     arg_joiner: str
     geom_param_pos: Any
 
 class Intersection(OracleToleranceMixin, GeomOutputGeoFunc):
     arity: int
     geom_param_pos: Any
 
 class IsEmpty(GeoFuncMixin, StandardTransform):
     lookup_name: str
-    output_field: ClassVar[BooleanField]
+    output_field: Any
 
 class IsValid(OracleToleranceMixin, GeoFuncMixin, StandardTransform):
     lookup_name: str
-    output_field: ClassVar[BooleanField]
+    output_field: Any
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Length(DistanceResultMixin, OracleToleranceMixin, GeoFunc):
     spheroid: Any
     def __init__(self, expr1: Any, spheroid: bool = ..., **extra: Any) -> None: ...
     def as_postgresql(
         self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any
     ) -> _AsSqlType: ...
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class LineLocatePoint(GeoFunc):
-    output_field: ClassVar[FloatField]
+    output_field: Any
     arity: int
     geom_param_pos: Any
 
 class MakeValid(GeomOutputGeoFunc): ...
 
 class MemSize(GeoFunc):
-    output_field: ClassVar[IntegerField]
+    output_field: Any
     arity: int
 
 class NumGeometries(GeoFunc):
-    output_field: ClassVar[IntegerField]
+    output_field: Any
     arity: int
 
 class NumPoints(GeoFunc):
-    output_field: ClassVar[IntegerField]
+    output_field: Any
     arity: int
 
 class Perimeter(DistanceResultMixin, OracleToleranceMixin, GeoFunc):
     arity: int
     def as_postgresql(
         self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any
     ) -> _AsSqlType: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/lookups.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/db/models/sql/conversion.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/db/models/sql/conversion.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/feeds.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/feeds.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/forms/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/forms/fields.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/forms/widgets.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/datasource.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/datasource.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/envelope.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/envelope.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/feature.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/feature.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/field.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/field.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/geometries.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/geometries.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/layer.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/layer.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/ds.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/generation.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/geom.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/raster.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/prototypes/srs.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/raster/band.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/raster/band.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/raster/source.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/raster/source.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pathlib import Path
 from typing import Any
 
 from django.contrib.gis.gdal.driver import Driver
 from django.contrib.gis.gdal.raster.band import BandList
 from django.contrib.gis.gdal.raster.base import GDALRasterBase
 from django.contrib.gis.gdal.srs import SpatialReference
-from django.utils.functional import cached_property
 
 class TransformPoint(list[Sequence[float]]):
     indices: dict[str, tuple[int, int]]
     def __init__(self, raster: GDALRaster, prop: str) -> None: ...
     @property
     def x(self) -> float: ...
     @x.setter
@@ -23,19 +22,19 @@
 
 class GDALRaster(GDALRasterBase):
     destructor: Any
     def __init__(self, ds_input: str | Path | bytes | dict | c_void_p, write: bool = ...) -> None: ...
     def __del__(self) -> None: ...
     @property
     def vsi_buffer(self) -> bytes | None: ...
-    @cached_property
+    @property
     def is_vsi_based(self) -> bool: ...
     @property
     def name(self) -> str: ...
-    @cached_property
+    @property
     def driver(self) -> Driver: ...
     @property
     def width(self) -> int: ...
     @property
     def height(self) -> int: ...
     @property
     def srs(self) -> SpatialReference | None: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/gdal/srs.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/gdal/srs.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geoip2/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geoip2/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/collections.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/collections.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/coordseq.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/geometry.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/geometry.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+from collections.abc import Sequence
 from typing import Any
 
 from django.contrib.gis.gdal import CoordTransform, SpatialReference
 from django.contrib.gis.gdal.geometries import OGRGeometry
 from django.contrib.gis.geos.base import GEOSBase
 from django.contrib.gis.geos.coordseq import GEOSCoordSeq
 from django.contrib.gis.geos.mutable_list import ListMixin
 from django.contrib.gis.geos.point import Point
 from django.contrib.gis.geos.prepared import PreparedGeometry
-from django.utils.deconstruct import _Deconstructible
 from typing_extensions import Self
 
 class GEOSGeometryBase(GEOSBase):
     ptr_type: Any
     destructor: Any
     has_cs: bool
     def __init__(self, ptr: Any, cls: Any) -> None: ...
@@ -138,9 +138,10 @@
     def project(self, point: Point) -> float: ...
     def project_normalized(self, point: Point) -> float: ...
     @property
     def merged(self) -> GEOSGeometry: ...
     @property
     def closed(self) -> bool: ...
 
-class GEOSGeometry(_Deconstructible, GEOSGeometryBase, ListMixin):
+class GEOSGeometry(GEOSGeometryBase, ListMixin):
     def __init__(self, geo_input: Any, srid: int | None = ...) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/libgeos.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/libgeos.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/linestring.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/linestring.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/mutable_list.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/mutable_list.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/point.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/point.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/polygon.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/polygon.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prepared.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prepared.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/geom.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/io.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/io.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/predicates.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/geos/prototypes/topology.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/geos/prototypes/topology.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/measure.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/measure.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/gis/utils/layermapping.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/gis/utils/layermapping.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/humanize/templatetags/humanize.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/humanize/templatetags/humanize.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/api.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/api.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/messages/storage/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/messages/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/aggregates/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/aggregates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/constraints.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/constraints.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/fields/array.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/fields/array.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/forms/array.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/forms/array.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/forms/ranges.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/forms/ranges.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/indexes.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/indexes.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.backends.ddl_references import Statement
 from django.db.models import Func, Index, Model
 from django.db.models.expressions import BaseExpression, Combinable
 from django.db.models.query_utils import Q
 from django.utils.datastructures import _ListOrTuple
-from django.utils.functional import cached_property
 
 class PostgresIndex(Index):
-    @cached_property
+    @property
     def max_name_length(self) -> int: ...  # type: ignore[override]
     def create_sql(
         self, model: type[Model], schema_editor: BaseDatabaseSchemaEditor, using: str = ..., **kwargs: Any
     ) -> Statement: ...
     def check_supported(self, schema_editor: BaseDatabaseSchemaEditor) -> None: ...
     def get_with_params(self) -> Sequence[str]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/lookups.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/lookups.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/search.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/search.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Any, ClassVar
+from typing import Any
 
-from django.db.models import Expression, Field, FloatField, TextField
+from django.db.models import Expression, Field
 from django.db.models.expressions import Combinable, CombinedExpression, Func
 from django.db.models.lookups import Lookup
 from typing_extensions import Self, TypeAlias
 
 _Expression: TypeAlias = str | Combinable | SearchQueryCombinable
 
 class SearchVectorExact(Lookup): ...
@@ -20,15 +20,15 @@
 class SearchVectorCombinable:
     ADD: str
 
 class SearchVector(SearchVectorCombinable, Func):
     config: _Expression | None
     function: str
     arg_joiner: str
-    output_field: ClassVar[SearchVectorField]
+    output_field: Field
     def __init__(
         self, *expressions: _Expression, config: _Expression | None = ..., weight: Any | None = ...
     ) -> None: ...
 
 class CombinedSearchVector(SearchVectorCombinable, CombinedExpression):
     def __init__(
         self,
@@ -44,15 +44,14 @@
     BITOR: str
     def __or__(self, other: SearchQueryCombinable) -> Self: ...
     def __ror__(self, other: SearchQueryCombinable) -> Self: ...
     def __and__(self, other: SearchQueryCombinable) -> Self: ...
     def __rand__(self, other: SearchQueryCombinable) -> Self: ...
 
 class SearchQuery(SearchQueryCombinable, Func):  # type: ignore[misc]
-    output_field: ClassVar[SearchQueryField]
     SEARCH_TYPES: dict[str, str]
     def __init__(
         self,
         value: _Expression,
         output_field: Field | None = ...,
         *,
         config: _Expression | None = ...,
@@ -68,28 +67,27 @@
         connector: str,
         rhs: Combinable,
         config: _Expression | None,
         output_field: Field | None = ...,
     ) -> None: ...
 
 class SearchRank(Func):
-    output_field: ClassVar[FloatField]
     def __init__(
         self,
         vector: SearchVector | _Expression,
         query: SearchQuery | _Expression,
         weights: Any | None = ...,
         normalization: Any | None = ...,
         cover_density: bool = ...,
     ) -> None: ...
 
 class SearchHeadline(Func):
     function: str
     template: str
-    output_field: ClassVar[TextField]
+    output_field: Field
     def __init__(
         self,
         expression: _Expression,
         query: _Expression,
         *,
         config: _Expression | None = ...,
         start_sel: Any | None = ...,
@@ -99,19 +97,17 @@
         short_word: str | None = ...,
         highlight_all: bool | None = ...,
         max_fragments: int | None = ...,
         fragment_delimiter: str | None = ...,
     ) -> None: ...
 
 class TrigramBase(Func):
-    output_field: ClassVar[FloatField]
     def __init__(self, expression: _Expression, string: str, **extra: Any) -> None: ...
 
 class TrigramWordBase(Func):
-    output_field: ClassVar[FloatField]
     def __init__(self, string: str, expression: _Expression, **extra: Any) -> None: ...
 
 class TrigramSimilarity(TrigramBase): ...
 class TrigramDistance(TrigramBase): ...
 class TrigramWordDistance(TrigramWordBase): ...
 class TrigramStrictWordDistance(TrigramWordBase): ...
 class TrigramWordSimilarity(TrigramWordBase): ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/postgres/validators.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/postgres/validators.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from collections.abc import Iterable, Mapping
+from collections.abc import Iterable, Mapping, Sequence
 from typing import Any
 
 from django.core.validators import MaxLengthValidator, MaxValueValidator, MinLengthValidator, MinValueValidator
-from django.utils.deconstruct import _Deconstructible
 
 class ArrayMaxLengthValidator(MaxLengthValidator): ...
 class ArrayMinLengthValidator(MinLengthValidator): ...
 
-class KeysValidator(_Deconstructible):
+class KeysValidator:
     messages: dict[str, str]
     strict: bool
     def __init__(self, keys: Iterable[str], strict: bool = ..., messages: Mapping[str, str] | None = ...) -> None: ...
     def __call__(self, value: Any) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...  # fake
 
 class RangeMaxValueValidator(MaxValueValidator): ...
 class RangeMinValueValidator(MinValueValidator): ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/backends/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sessions/base_session.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sessions/base_session.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import datetime
-from typing import Any, ClassVar, Literal, TypeVar
+from typing import Any, Literal, TypeVar
 
 from django.contrib.sessions.backends.base import SessionBase
 from django.db import models
 
 _T = TypeVar("_T", bound=AbstractBaseSession)
 
 class BaseSessionManager(models.Manager[_T]):
     def encode(self, session_dict: dict[str, Any]) -> str: ...
     def save(self, session_key: str, session_dict: dict[str, Any], expire_date: datetime) -> _T: ...
 
 class AbstractBaseSession(models.Model):
     expire_date: datetime
     session_data: str
     session_key: str
-    objects: ClassVar[Any]
+    objects: Any
 
     class Meta:
         abstract: Literal[True]
     @classmethod
     def get_session_store_class(cls) -> type[SessionBase] | None: ...
     def get_decoded(self) -> dict[str, Any]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sitemaps/views.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sitemaps/views.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/sites/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/sites/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/finders.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/finders.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/handlers.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/handlers.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/staticfiles/storage.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/staticfiles/storage.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from django.utils._os import _PathCompatible
 from django.utils.functional import LazyObject
 from typing_extensions import TypeAlias
 
 _PostProcessT: TypeAlias = Iterator[tuple[str, str, bool] | tuple[str, None, RuntimeError]]
 
 class StaticFilesStorage(FileSystemStorage):
+    base_location: str
+    location: _PathCompatible
     def __init__(
         self, location: _PathCompatible | None = ..., base_url: str | None = ..., *args: Any, **kwargs: Any
     ) -> None: ...
     def path(self, name: _PathCompatible) -> str: ...
 
 class HashedFilesMixin:
     default_template: str
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/contrib/syndication/views.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/contrib/syndication/views.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/db.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/cache/backends/memcached.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/cache/backends/memcached.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/caches.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/caches.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/messages.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/messages.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/registry.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/registry.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/security/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/security/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/security/csrf.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/security/csrf.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/security/sessions.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/security/sessions.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/templates.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/templates.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/translation.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/translation.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/checks/urls.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/checks/urls.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/exceptions.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/base.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from collections.abc import Iterator
 from types import TracebackType
 from typing import IO, AnyStr, type_check_only
 
 from django.core.files.utils import FileProxyMixin
-from django.utils.functional import cached_property
 from typing_extensions import Self
 
 class File(FileProxyMixin[AnyStr], IO[AnyStr]):
     DEFAULT_CHUNK_SIZE: int
     file: IO[AnyStr] | None
-    name: str | None
+    name: str | None  # type: ignore[assignment]
     mode: str
     def __init__(self, file: IO[AnyStr] | None, name: str | None = ...) -> None: ...
     def __bool__(self) -> bool: ...
     def __len__(self) -> int: ...
-    @cached_property
+    @property
     def size(self) -> int: ...
     def chunks(self, chunk_size: int | None = ...) -> Iterator[AnyStr]: ...
     def multiple_chunks(self, chunk_size: int | None = ...) -> bool | None: ...
     def __iter__(self) -> Iterator[AnyStr]: ...
     def __enter__(self) -> Self: ...
     def __exit__(
         self,
@@ -29,14 +28,15 @@
     def open(self, mode: str | None = ...) -> Self: ...
     def close(self) -> None: ...
     @type_check_only
     def __next__(self) -> AnyStr: ...
 
 class ContentFile(File[AnyStr]):
     file: IO[AnyStr]
+    size: int
     def __init__(self, content: AnyStr, name: str | None = ...) -> None: ...
     def __bool__(self) -> bool: ...
     def open(self, mode: str | None = ...) -> Self: ...
     def close(self) -> None: ...
     def write(self, data: AnyStr) -> int: ...
 
 def endswith_cr(line: bytes | str) -> bool: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/storage/filesystem.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/storage/memory.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+from collections.abc import Sequence
+from typing import Any
+
 from django.utils._os import _PathCompatible
-from django.utils.deconstruct import _Deconstructible
-from django.utils.functional import cached_property
 
 from .base import Storage
 from .mixins import StorageSettingsMixin
 
-class FileSystemStorage(_Deconstructible, Storage, StorageSettingsMixin):
-    OS_OPEN_FLAGS: int
-
+class InMemoryStorage(Storage, StorageSettingsMixin):
     def __init__(
         self,
         location: _PathCompatible | None = ...,
         base_url: str | None = ...,
         file_permissions_mode: int | None = ...,
         directory_permissions_mode: int | None = ...,
     ) -> None: ...
-    @cached_property
+    @property
     def base_location(self) -> _PathCompatible: ...
-    @cached_property
+    @property
     def location(self) -> _PathCompatible: ...
-    @cached_property
+    @property
     def base_url(self) -> str: ...
-    @cached_property
+    @property
     def file_permissions_mode(self) -> int | None: ...
-    @cached_property
+    @property
     def directory_permissions_mode(self) -> int | None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...  # fake
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/uploadedfile.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/uploadedfile.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/uploadhandler.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/uploadhandler.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/files/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/files/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/asgi.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/asgi.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import IO, Any, TypeVar
 
 from django.core.handlers import base
 from django.http.request import HttpRequest, _ImmutableQueryDict
 from django.http.response import HttpResponseBase
 from django.urls.resolvers import ResolverMatch, URLResolver
 from django.utils.datastructures import MultiValueDict
-from django.utils.functional import cached_property
 from typing_extensions import TypeAlias
 
 _ReceiveCallback: TypeAlias = Callable[[], Awaitable[Mapping[str, Any]]]
 
 _SendCallback: TypeAlias = Callable[[Mapping[str, Any]], Awaitable[None]]
 
 class ASGIRequest(HttpRequest):
@@ -19,19 +18,19 @@
     resolver_match: ResolverMatch | None
     script_name: str | None
     path_info: str
     path: str
     method: str
     META: dict[str, Any]
     def __init__(self, scope: Mapping[str, Any], body_file: IO[bytes]) -> None: ...
-    @cached_property
+    @property
     def GET(self) -> _ImmutableQueryDict: ...  # type: ignore[override]
     POST: _ImmutableQueryDict
     FILES: MultiValueDict
-    @cached_property
+    @property
     def COOKIES(self) -> dict[str, str]: ...  # type: ignore[override]
 
 _T = TypeVar("_T")
 
 class ASGIHandler(base.BaseHandler):
     request_class: type[ASGIRequest]
     chunk_size: int
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/exception.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/exception.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/handlers/wsgi.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/handlers/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/backends/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/mail/message.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/mail/message.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from io import TextIOBase
 from typing import Any, Literal, TextIO
 
 from django.apps.config import AppConfig
 from django.core.management.color import Style
 from django.utils.datastructures import _ListOrTuple
 
-ALL_CHECKS: Literal["__all__"]
-
 class CommandError(Exception):
     def __init__(self, *args: Any, returncode: int = ..., **kwargs: Any) -> None: ...
 
 class SystemCheckError(CommandError): ...
 
 class CommandParser(ArgumentParser):
     missing_args_message: str | None
@@ -47,29 +45,27 @@
 class BaseCommand:
     help: str
     output_transaction: bool
     requires_migrations_checks: bool
     requires_system_checks: _ListOrTuple[str] | Literal["__all__"]
     base_stealth_options: tuple[str, ...]
     stealth_options: tuple[str, ...]
-    suppressed_base_arguments: set[str]
     stdout: OutputWrapper
     stderr: OutputWrapper
     style: Style
     def __init__(
         self,
         stdout: TextIO | None = ...,
         stderr: TextIO | None = ...,
         no_color: bool = ...,
         force_color: bool = ...,
     ) -> None: ...
     def get_version(self) -> str: ...
     def create_parser(self, prog_name: str, subcommand: str, **kwargs: Any) -> CommandParser: ...
     def add_arguments(self, parser: CommandParser) -> None: ...
-    def add_base_argument(self, parser: CommandParser, *args: Any, **kwargs: Any) -> None: ...
     def print_help(self, prog_name: str, subcommand: str) -> None: ...
     def run_from_argv(self, argv: list[str]) -> None: ...
     def execute(self, *args: Any, **options: Any) -> str | None: ...
     def check(
         self,
         app_configs: Sequence[AppConfig] | None = ...,
         tags: Sequence[str] | None = ...,
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/color.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/color.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/diffsettings.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/diffsettings.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,13 @@
 from typing import Any
 
 from django.core.management.base import BaseCommand
 
 def module_to_dict(module: Any, omittable: Callable[[str], bool] = ...) -> dict[str, str]: ...
 
 class Command(BaseCommand):
-    def handle(self, **options: Any) -> str: ...
     def output_hash(
         self, user_settings: dict[str, str], default_settings: dict[str, str], **options: Any
     ) -> list[str]: ...
     def output_unified(
         self, user_settings: dict[str, str], default_settings: dict[str, str], **options: Any
     ) -> list[str]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/inspectdb.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/inspectdb.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from collections.abc import Iterable
 from typing import Any
 
 from django.core.management.base import BaseCommand
 from django.db.backends.base.base import BaseDatabaseWrapper
 
 class Command(BaseCommand):
+    stealth_options: tuple[str]
     db_module: str
-
-    def handle(self, **options: Any) -> None: ...
     def handle_inspection(self, options: dict[str, Any]) -> Iterable[str]: ...
     def normalize_col_name(
         self, col_name: str, used_column_names: list[str], is_relation: bool
     ) -> tuple[str, dict[str, str], list[str]]: ...
     def get_field_type(
         self, connection: BaseDatabaseWrapper, table_name: str, row: Any
     ) -> tuple[str, dict[str, Any], list[str]]: ...
     def get_meta(
-        self,
-        table_name: str,
-        constraints: Any,
-        column_to_field_name: Any,
-        is_view: bool,
-        is_partition: bool,
-        comment: str | None,
+        self, table_name: str, constraints: Any, column_to_field_name: Any, is_view: Any, is_partition: Any
     ) -> list[str]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/loaddata.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/debug.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,76 @@
-import zipfile
-from collections.abc import Sequence
-from io import BufferedReader
-from typing import Callable, Literal
-
-from django.apps.config import AppConfig
-from django.core.management.base import BaseCommand
-from django.core.serializers.base import DeserializedObject
-from django.db.backends.base.base import BaseDatabaseWrapper
-from django.db.models.base import Model
-from django.utils.functional import cached_property
-from typing_extensions import TypeAlias
-
-has_bz2: bool
-has_lzma: bool
-
-READ_STDIN: str
-_ReadBinaryMode: TypeAlias = Literal["r", "rb"]
-
-class Command(BaseCommand):
-    missing_args_message: str
-    ignore: bool
-    using: str
-    app_label: str
-    verbosity: int
-    excluded_models: set[type[Model]]
-    excluded_apps: set[AppConfig]
-    format: str
-    fixture_count: int
-    loaded_object_count: int
-    fixture_object_count: int
-    models: set[type[Model]]
-    serialization_formats: list[str]
-    objs_with_deferred_fields: list[DeserializedObject]
-    @cached_property
-    def compression_formats(self) -> dict[str | None, tuple[Callable[[str, _ReadBinaryMode], BufferedReader]]]: ...
-    def reset_sequences(self, connection: BaseDatabaseWrapper, models: set[type[Model]]) -> None: ...
-    def loaddata(self, fixture_labels: Sequence[str]) -> None: ...
-    def save_obj(self, obj: DeserializedObject) -> bool: ...
-    def load_label(self, fixture_label: str) -> None: ...
-    def get_fixture_name_and_dirs(self, fixture_name: str) -> tuple[str, list[str]]: ...
-    def get_targets(self, fixture_name: str, ser_fmt: str | None, cmp_fmt: str | None) -> set[str]: ...
-    def find_fixture_files_in_dir(
-        self, fixture_dir: str, fixture_name: str, targets: set[str]
-    ) -> list[tuple[str, str, str]]: ...
-    def find_fixtures(self, fixture_label: str) -> list[tuple[str, str | None, str | None]]: ...
-    @cached_property
-    def fixture_dirs(self) -> list[str]: ...
-    def parse_name(self, fixture_name: str) -> tuple[str, str | None, str | None]: ...
-
-class SingleZipReader(zipfile.ZipFile):
-    # Incompatible override
-    #     zipfile.ZipFile.read(
-    #         self,
-    #         name: typing.Union[typing.Text, zipfile.ZipInfo],
-    #         pwd: Optional[bytes] = ...,
-    #     ) -> bytes: ...
-    def read(self) -> bytes: ...  # type: ignore[override]
-
-def humanize(dirname: str) -> str: ...
+import re
+from collections.abc import Callable, ItemsView, Iterator
+from pathlib import Path
+from types import TracebackType
+from typing import Any
+
+from django.http.request import HttpRequest, QueryDict
+from django.http.response import Http404, HttpResponse
+from django.template import Engine
+from django.utils.safestring import SafeString
+
+DEBUG_ENGINE: Engine
+
+class CallableSettingWrapper:
+    def __init__(self, callable_setting: Callable | type[Any]) -> None: ...
+
+class ExceptionCycleWarning(UserWarning): ...
+
+def technical_500_response(
+    request: HttpRequest,
+    exc_type: type[BaseException] | None,
+    exc_value: BaseException | None,
+    tb: TracebackType | None,
+    status_code: int = ...,
+) -> HttpResponse: ...
+def get_default_exception_reporter_filter() -> SafeExceptionReporterFilter: ...
+def get_exception_reporter_filter(request: HttpRequest | None) -> SafeExceptionReporterFilter: ...
+
+class SafeExceptionReporterFilter:
+    cleansed_substitute: str
+    hidden_settings: re.Pattern[str]
+    def cleanse_setting(self, key: int | str, value: Any) -> Any: ...
+    def get_safe_settings(self) -> dict[str, Any]: ...
+    def get_safe_request_meta(self, request: HttpRequest) -> dict[str, Any]: ...
+    def get_safe_cookies(self, request: HttpRequest) -> dict[str, Any]: ...
+    def is_active(self, request: HttpRequest | None) -> bool: ...
+    def get_cleansed_multivaluedict(self, request: HttpRequest, multivaluedict: QueryDict) -> QueryDict: ...
+    def get_post_parameters(self, request: HttpRequest | None) -> dict[str, Any]: ...
+    def cleanse_special_types(self, request: HttpRequest | None, value: Any) -> Any: ...
+    def get_traceback_frame_variables(self, request: Any, tb_frame: Any) -> ItemsView[str, Any]: ...
+
+class ExceptionReporter:
+    request: HttpRequest | None
+    filter: SafeExceptionReporterFilter
+    exc_type: type[BaseException] | None
+    exc_value: BaseException | None
+    tb: TracebackType | None
+    is_email: bool
+    template_info: Any | None
+    template_does_not_exist: bool
+    postmortem: Any | None
+    @property
+    def html_template_path(self) -> Path: ...
+    @property
+    def text_template_path(self) -> Path: ...
+    def __init__(
+        self,
+        request: HttpRequest | None,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        tb: TracebackType | None,
+        is_email: bool = ...,
+    ) -> None: ...
+    def get_traceback_data(self) -> dict[str, Any]: ...
+    def get_traceback_html(self) -> SafeString: ...
+    def get_traceback_text(self) -> SafeString: ...
+    def get_traceback_frames(self) -> list[Any]: ...
+    def get_exception_traceback_frames(
+        self, exc_value: BaseException | None, tb: TracebackType | None
+    ) -> Iterator[dict[str, Any]]: ...
+
+def technical_404_response(request: HttpRequest, exception: Http404) -> HttpResponse: ...
+def default_urlconf(request: HttpResponse | None) -> HttpResponse: ...
+def builtin_template_path(name: str) -> Path: ...
+def get_caller(request: HttpRequest) -> str: ...
+def get_exception_reporter_class(request: HttpRequest) -> ExceptionReporter: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/makemessages.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/makemessages.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-from re import Match, Pattern
+from re import Pattern
 from typing import Any
 
 from django.core.management.base import BaseCommand
-from django.utils.functional import cached_property
 
 plural_forms_re: Pattern[str]
 STATUS_OK: int
 NO_LOCALE_DIR: Any
 
 def check_programs(*programs: str) -> None: ...
-def is_valid_locale(locale: str) -> Match[str] | None: ...
 
 class TranslatableFile:
     dirpath: str
     file_name: str
     locale_dir: str
     def __init__(self, dirpath: str, file_name: str, locale_dir: str | None) -> None: ...
 
 class BuildFile:
     """
     Represent the state of a translatable file during the build process.
     """
 
-    command: BaseCommand
-    domain: str
-    translatable: TranslatableFile
     def __init__(self, command: BaseCommand, domain: str, translatable: TranslatableFile) -> None: ...
-    @cached_property
+    @property
     def is_templatized(self) -> bool: ...
-    @cached_property
+    @property
     def path(self) -> str: ...
-    @cached_property
+    @property
     def work_path(self) -> str: ...
     def preprocess(self) -> None: ...
     def postprocess_messages(self, msgs: str) -> str: ...
     def cleanup(self) -> None: ...
 
 def normalize_eols(raw_contents: str) -> str: ...
 def write_pot_file(potfile: str, msgs: str) -> None: ...
@@ -42,29 +37,7 @@
 class Command(BaseCommand):
     translatable_file_class: type[TranslatableFile]
     build_file_class: type[BuildFile]
     msgmerge_options: list[str]
     msguniq_options: list[str]
     msgattrib_options: list[str]
     xgettext_options: list[str]
-
-    domain: str
-    verbosity: int
-    symlinks: bool
-    ignore_patterns: list[str]
-    no_obsolete: bool
-    keep_pot: bool
-    extensions: set[str]
-    invoked_for_django: bool
-    locale_paths: list[str]
-    default_locale_path: str | None
-    @cached_property
-    def gettext_version(self) -> tuple[int, int] | tuple[int, int, int]: ...
-    @cached_property
-    def settings_available(self) -> bool: ...
-    def build_potfiles(self) -> list[str]: ...
-    def remove_potfiles(self) -> None: ...
-    def find_files(self, root: str) -> list[TranslatableFile]: ...
-    def process_files(self, file_list: list[TranslatableFile]) -> None: ...
-    def process_locale_dir(self, locale_dir: str, files: list[TranslatableFile]) -> None: ...
-    def write_po_file(self, potfile: str, locale: str) -> None: ...
-    def copy_plural_forms(self, msgs: str, locale: str) -> str: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/makemigrations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/makemigrations.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/commands/migrate.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/commands/migrate.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/templates.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/templates.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/management/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/management/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/paginator.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Iterable, Iterator, Sequence, Sized
 from typing import ClassVar, Generic, Protocol, TypeVar, overload
 
-from django.utils.functional import _StrPromise, cached_property
+from django.utils.functional import _StrPromise
 
 class UnorderedObjectListWarning(RuntimeWarning): ...
 class InvalidPage(Exception): ...
 class PageNotAnInteger(InvalidPage): ...
 class EmptyPage(InvalidPage): ...
 
 _T = TypeVar("_T")
@@ -29,17 +29,17 @@
         orphans: int = ...,
         allow_empty_first_page: bool = ...,
     ) -> None: ...
     def __iter__(self) -> Iterator[Page[_T]]: ...
     def validate_number(self, number: int | float | str) -> int: ...
     def get_page(self, number: int | float | str | None) -> Page[_T]: ...
     def page(self, number: int | str) -> Page[_T]: ...
-    @cached_property
+    @property
     def count(self) -> int: ...
-    @cached_property
+    @property
     def num_pages(self) -> int: ...
     @property
     def page_range(self) -> range: ...
     def get_elided_page_range(
         self, number: int | float | str = ..., *, on_each_side: int = ..., on_ends: int = ...
     ) -> Iterator[str | int]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/json.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/json.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/pyyaml.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/pyyaml.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/serializers/xml_serializer.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/serializers/xml_serializer.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/servers/basehttp.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/servers/basehttp.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/signing.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/signing.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/core/validators.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/core/validators.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 from collections.abc import Callable, Collection, Sequence, Sized
 from decimal import Decimal
 from re import Pattern, RegexFlag
 from typing import Any
 
 from django.core.files.base import File
-from django.utils.deconstruct import _Deconstructible
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 EMPTY_VALUES: Any
 
 _Regex: TypeAlias = str | Pattern[str]
 
 _ValidatorCallable: TypeAlias = Callable[[Any], None]  # noqa: PYI047
 
-class RegexValidator(_Deconstructible):
+class RegexValidator:
     regex: _Regex  # Pattern[str] on instance, but may be str on class definition
     message: _StrOrPromise
     code: str
     inverse_match: bool
     flags: int
     def __init__(
         self,
         regex: _Regex | None = ...,
         message: _StrOrPromise | None = ...,
         code: str | None = ...,
         inverse_match: bool | None = ...,
         flags: RegexFlag | None = ...,
     ) -> None: ...
     def __call__(self, value: Any) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class URLValidator(RegexValidator):
     ul: str
     ipv4_re: str
     ipv6_re: str
     hostname_re: str
     domain_re: str
     tld_re: str
     host_re: str
     schemes: Sequence[str]
     unsafe_chars: frozenset[str]
     max_length: int
     def __init__(self, schemes: Sequence[str] | None = ..., **kwargs: Any) -> None: ...
     def __call__(self, value: str) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 integer_validator: RegexValidator
 
 def validate_integer(value: float | str | None) -> None: ...
 
-class EmailValidator(_Deconstructible):
+class EmailValidator:
     message: _StrOrPromise
     code: str
     user_regex: Pattern[str]
     domain_regex: Pattern[str]
     literal_regex: Pattern[str]
     domain_allowlist: Sequence[str]
     def __init__(
@@ -60,14 +61,15 @@
         message: _StrOrPromise | None = ...,
         code: str | None = ...,
         allowlist: Sequence[str] | None = ...,
     ) -> None: ...
     def __call__(self, value: str | None) -> None: ...
     def validate_domain_part(self, domain_part: str) -> bool: ...
     def __eq__(self, other: object) -> bool: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 validate_email: EmailValidator
 slug_re: Pattern[str]
 validate_slug: RegexValidator
 slug_unicode_re: Pattern[str]
 validate_unicode_slug: RegexValidator
 
@@ -81,55 +83,66 @@
 def ip_address_validators(protocol: str, unpack_ipv4: bool) -> _IPValidator: ...
 def int_list_validator(
     sep: str = ..., message: _StrOrPromise | None = ..., code: str = ..., allow_negative: bool = ...
 ) -> RegexValidator: ...
 
 validate_comma_separated_integer_list: RegexValidator
 
-class BaseValidator(_Deconstructible):
+class BaseValidator:
     message: _StrOrPromise
     code: str
     limit_value: Any
     def __init__(self, limit_value: Any, message: _StrOrPromise | None = ...) -> None: ...
     def __call__(self, value: Any) -> None: ...
     def compare(self, a: Any, b: Any) -> bool: ...
     def clean(self, x: Any) -> Any: ...
     def __eq__(self, other: object) -> bool: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
-class MaxValueValidator(BaseValidator): ...
-class MinValueValidator(BaseValidator): ...
-class StepValueValidator(BaseValidator): ...
+class MaxValueValidator(BaseValidator):
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
+
+class MinValueValidator(BaseValidator):
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
+
+class StepValueValidator(BaseValidator):
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class MinLengthValidator(BaseValidator):
     def clean(self, x: Sized) -> int: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class MaxLengthValidator(BaseValidator):
     def clean(self, x: Sized) -> int: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
-class DecimalValidator(_Deconstructible):
+class DecimalValidator:
     messages: dict[str, str]
     max_digits: int | None
     decimal_places: int | None
     def __init__(self, max_digits: int | None, decimal_places: int | None) -> None: ...
     def __call__(self, value: Decimal) -> None: ...
     def __eq__(self, other: object) -> bool: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
-class FileExtensionValidator(_Deconstructible):
+class FileExtensionValidator:
     message: _StrOrPromise
     code: str
     allowed_extensions: Collection[str] | None
     def __init__(
         self,
         allowed_extensions: Collection[str] | None = ...,
         message: _StrOrPromise | None = ...,
         code: str | None = ...,
     ) -> None: ...
     def __call__(self, value: File) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 def get_available_image_extensions() -> Sequence[str]: ...
 def validate_image_file_extension(value: File) -> None: ...
 
-class ProhibitNullCharactersValidator(_Deconstructible):
+class ProhibitNullCharactersValidator:
     message: _StrOrPromise
     code: str
     def __init__(self, message: _StrOrPromise | None = ..., code: str | None = ...) -> None: ...
     def __call__(self, value: Any) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from django.db.backends.base.creation import BaseDatabaseCreation
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.db.backends.base.introspection import BaseDatabaseIntrospection
 from django.db.backends.base.operations import BaseDatabaseOperations
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.backends.base.validation import BaseDatabaseValidation
 from django.db.backends.utils import CursorDebugWrapper, CursorWrapper
-from django.utils.functional import cached_property
 from typing_extensions import Self, TypeAlias
 
 NO_DB_ALIAS: str
 RAN_DB_VERSION_CHECK: set[str]
 
 logger: Logger
 
@@ -62,17 +61,17 @@
     features: BaseDatabaseFeatures
     introspection: BaseDatabaseIntrospection
     ops: BaseDatabaseOperations
     validation: BaseDatabaseValidation
     operators: MutableMapping[str, str]
     def __init__(self, settings_dict: dict[str, Any], alias: str = ...) -> None: ...
     def ensure_timezone(self) -> bool: ...
-    @cached_property
+    @property
     def timezone(self) -> tzinfo | None: ...
-    @cached_property
+    @property
     def timezone_name(self) -> str: ...
     @property
     def queries_logged(self) -> bool: ...
     @property
     def queries(self) -> list[dict[str, str]]: ...
     def get_database_version(self) -> tuple[int, ...]: ...
     def check_database_version_supported(self) -> None: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/client.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/client.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/creation.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/creation.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/features.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/features.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections.abc import Sequence
 from typing import Any
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.base import Model
 from django.db.utils import DatabaseError, DataError
-from django.utils.functional import cached_property
 
 class BaseDatabaseFeatures:
     minimum_database_version: tuple[int, ...] | None
     gis_enabled: bool
     allows_group_by_lob: bool
     allows_group_by_selected_pks: bool
     allows_group_by_select_index: bool
@@ -134,12 +133,12 @@
     supports_unlimited_charfield: bool
     test_collations: dict[str, str | None]
     test_now_utc_template: str | None
     django_test_expected_failures: set[str]
     django_test_skips: dict[str, set[str]]
     connection: BaseDatabaseWrapper
     def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
-    @cached_property
+    @property
     def supports_explaining_query_execution(self) -> bool: ...
-    @cached_property
+    @property
     def supports_transactions(self) -> bool: ...
     def allows_group_by_selected_pks_on_model(self, model: type[Model]) -> bool: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/introspection.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/introspection.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/base/schema.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/base/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/ddl_references.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/ddl_references.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/dummy/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/dummy/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     def create_cursor(self, name: Any | None = ...) -> CursorWrapper: ...
     def disable_constraint_checking(self) -> Literal[True]: ...
     needs_rollback: Any
     def enable_constraint_checking(self) -> None: ...
     def check_constraints(self, table_names: Any | None = ...) -> None: ...
     def is_usable(self) -> bool: ...
     @property
-    def display_name(self) -> str: ...  # type: ignore[override]
+    def display_name(self) -> str: ...  # type: ignore [override]
     @property
-    def data_type_check_constraints(self) -> dict[str, str]: ...  # type: ignore[override]
+    def data_type_check_constraints(self) -> dict[str, str]: ...  # type: ignore [override]
     @property
     def mysql_server_data(self) -> dict[str, Any]: ...
     @property
     def mysql_server_info(self) -> str: ...
     @property
     def mysql_version(self) -> tuple[int, ...]: ...
     @property
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/compiler.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/features.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/features.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Any
 
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.db.backends.mysql.base import DatabaseWrapper
-from django.utils.functional import cached_property
 
 class DatabaseFeatures(BaseDatabaseFeatures):
     connection: DatabaseWrapper
     empty_fetchmany_value: Any
     allows_group_by_pk: bool
     related_fields_match_type: bool
     allow_sliced_subqueries_with_in: bool
@@ -38,51 +37,51 @@
     supports_order_by_nulls_modifier: bool
     order_by_nulls_first: bool
 
     # fake properties (until `property` is generic)
     supports_frame_range_fixed_distance: bool
     supports_table_check_constraints: bool
     can_return_rows_from_bulk_insert: bool
-    @cached_property
+    @property
     def allows_auto_pk_0(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def update_can_self_select(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def can_introspect_foreign_keys(self) -> bool: ...  # type: ignore[override]
-    @cached_property
-    def introspected_field_types(self) -> dict[str, str]: ...  # type: ignore[override]
-    @cached_property
+    @property
+    def introspected_field_types(self) -> dict[str, str]: ...  # type: ignore [override]
+    @property
     def can_return_columns_from_insert(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def has_zoneinfo_database(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def is_sql_auto_is_null_enabled(self) -> bool: ...
-    @cached_property
+    @property
     def supports_over_clause(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def supports_column_check_constraints(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def can_introspect_check_constraints(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def has_select_for_update_skip_locked(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def has_select_for_update_nowait(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def has_select_for_update_of(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def supports_explain_analyze(self) -> bool: ...
-    @cached_property
+    @property
     def supported_explain_formats(self) -> set[str]: ...  # type: ignore[override]
-    @cached_property
+    @property
     def supports_transactions(self) -> bool: ...
-    @cached_property
+    @property
     def ignores_table_name_case(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def supports_default_in_lead_lag(self) -> bool: ...  # type: ignore[override]
     @property
     def supports_json_field(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def can_introspect_json_field(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def supports_index_column_ordering(self) -> bool: ...  # type: ignore[override]
-    @cached_property
+    @property
     def supports_expression_indexes(self) -> bool: ...  # type: ignore[override]
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/introspection.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/introspection.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/mysql/schema.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/client.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/client.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/features.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/oracle/schema.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/base.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from io import IOBase
 from typing import Any
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.utils import CursorDebugWrapper as BaseCursorDebugWrapper
 from django.db.backends.utils import _ExecuteQuery
-from django.utils.functional import cached_property
 
 from .client import DatabaseClient
 from .creation import DatabaseCreation
 from .features import DatabaseFeatures
 from .introspection import DatabaseIntrospection
 from .operations import DatabaseOperations
 
@@ -31,13 +30,13 @@
 
     operators: dict[str, str]
     pattern_esc: str
     pattern_ops: dict[str, str]
 
     # PostgreSQL backend-specific attributes.
     _named_cursor_idx: int
-    @cached_property
+    @property
     def pg_version(self) -> int: ...
 
 class CursorDebugWrapper(BaseCursorDebugWrapper):
     def copy_expert(self, sql: _ExecuteQuery, file: IOBase, *args: Any) -> Any: ...
     def copy_to(self, file: IOBase, table: str, *args: Any, **kwargs: Any) -> Any: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/client.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/client.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/features.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/features.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Any
 
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.db.backends.postgresql.base import DatabaseWrapper
-from django.utils.functional import cached_property
 
 class DatabaseFeatures(BaseDatabaseFeatures):
     connection: DatabaseWrapper
     allows_group_by_selected_pks: bool
     can_return_columns_from_insert: bool
     can_return_rows_from_bulk_insert: bool
     has_real_datatype: bool
@@ -46,15 +45,15 @@
     json_key_contains_list_matching_requires_list: bool
     @property
     def is_postgresql_10(self) -> bool: ...
     @property
     def is_postgresql_11(self) -> bool: ...
     @property
     def is_postgresql_12(self) -> bool: ...
-    @cached_property
+    @property
     def is_postgresql_13(self) -> bool: ...
     has_brin_autosummarize: bool
     has_websearch_to_tsquery: bool
     supports_table_partitions: bool
     supports_covering_indexes: bool
     supports_covering_gist_indexes: bool
     supports_non_deterministic_collations: bool
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/postgresql/schema.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/postgresql/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/sqlite3/operations.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/sqlite3/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/backends/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/backends/utils.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -65,22 +65,22 @@
         sql: str | None = ...,
         params: _ExecuteParameters | Sequence[_ExecuteParameters] | None = ...,
         use_last_executed_query: bool = ...,
         many: bool = ...,
     ) -> Generator[None, None, None]: ...
 
 @overload
-def typecast_date(s: None | Literal[""]) -> None: ...  # type: ignore[overload-overlap]
+def typecast_date(s: None | Literal[""]) -> None: ...  # type: ignore[misc]
 @overload
 def typecast_date(s: str) -> datetime.date: ...
 @overload
-def typecast_time(s: None | Literal[""]) -> None: ...  # type: ignore[overload-overlap]
+def typecast_time(s: None | Literal[""]) -> None: ...  # type: ignore[misc]
 @overload
 def typecast_time(s: str) -> datetime.time: ...
 @overload
-def typecast_timestamp(s: None | Literal[""]) -> None: ...  # type: ignore[overload-overlap]
+def typecast_timestamp(s: None | Literal[""]) -> None: ...  # type: ignore[misc]
 @overload
 def typecast_timestamp(s: str) -> datetime.datetime: ...
 def split_identifier(identifier: str) -> tuple[str, str]: ...
 def truncate_name(identifier: str, length: int | None = ..., hash_len: int = ...) -> str: ...
 def format_number(value: Decimal | None, max_digits: int | None, decimal_places: int | None) -> str | None: ...
 def strip_quotes(table_name: str) -> str: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/autodetector.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/autodetector.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/exceptions.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/executor.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/executor.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/graph.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/graph.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/loader.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/loader.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/migration.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/migration.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/fields.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/special.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/special.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/operations/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/operations/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/questioner.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/questioner.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/recorder.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/recorder.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/serializer.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/serializer.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/state.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/state.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/migrations/writer.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/migrations/writer.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,27 @@
 from .deletion import SET_NULL as SET_NULL
 from .deletion import ProtectedError as ProtectedError
 from .deletion import RestrictedError as RestrictedError
 from .enums import Choices as Choices
 from .enums import IntegerChoices as IntegerChoices
 from .enums import TextChoices as TextChoices
 from .expressions import Case as Case
+from .expressions import Col as Col
+from .expressions import Combinable as Combinable
+from .expressions import CombinedExpression as CombinedExpression
 from .expressions import Exists as Exists
 from .expressions import Expression as Expression
 from .expressions import ExpressionList as ExpressionList
 from .expressions import ExpressionWrapper as ExpressionWrapper
 from .expressions import F as F
 from .expressions import Func as Func
 from .expressions import OrderBy as OrderBy
 from .expressions import OuterRef as OuterRef
+from .expressions import RawSQL as RawSQL
+from .expressions import Ref as Ref
 from .expressions import RowRange as RowRange
 from .expressions import Subquery as Subquery
 from .expressions import Value as Value
 from .expressions import ValueRange as ValueRange
 from .expressions import When as When
 from .expressions import Window as Window
 from .expressions import WindowFrame as WindowFrame
@@ -68,14 +73,16 @@
 from .fields import SlugField as SlugField
 from .fields import SmallAutoField as SmallAutoField
 from .fields import SmallIntegerField as SmallIntegerField
 from .fields import TextField as TextField
 from .fields import TimeField as TimeField
 from .fields import URLField as URLField
 from .fields import UUIDField as UUIDField
+from .fields.files import FieldFile as FieldFile
+from .fields.files import FileDescriptor as FileDescriptor
 from .fields.files import FileField as FileField
 from .fields.files import ImageField as ImageField
 from .fields.json import JSONField as JSONField
 from .fields.proxy import OrderWrt as OrderWrt
 from .fields.related import ForeignKey as ForeignKey
 from .fields.related import ForeignObject as ForeignObject
 from .fields.related import ForeignObjectRel as ForeignObjectRel
@@ -83,13 +90,15 @@
 from .fields.related import ManyToManyRel as ManyToManyRel
 from .fields.related import ManyToOneRel as ManyToOneRel
 from .fields.related import OneToOneField as OneToOneField
 from .fields.related import OneToOneRel as OneToOneRel
 from .indexes import Index as Index
 from .lookups import Lookup as Lookup
 from .lookups import Transform as Transform
+from .manager import BaseManager as BaseManager
 from .manager import Manager as Manager
 from .query import Prefetch as Prefetch
 from .query import QuerySet as QuerySet
+from .query import RawQuerySet as RawQuerySet
 from .query import prefetch_related_objects as prefetch_related_objects
 from .query_utils import FilteredRelation as FilteredRelation
 from .query_utils import Q as Q
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections.abc import Collection, Iterable, Sequence
 from typing import Any, ClassVar, Final, TypeVar, overload
 
 from django.core.checks.messages import CheckMessage
 from django.core.exceptions import MultipleObjectsReturned as BaseMultipleObjectsReturned
 from django.core.exceptions import ObjectDoesNotExist, ValidationError
-from django.db.models import BaseConstraint, Field, QuerySet
+from django.db.models import BaseConstraint, Field
 from django.db.models.manager import BaseManager, Manager
 from django.db.models.options import Options
 from typing_extensions import Self
 
 _Self = TypeVar("_Self", bound=Model)
 
 class ModelStateFieldsCacheDescriptor:
@@ -45,23 +45,14 @@
     pk: Any
     _state: ModelState
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     @classmethod
     def add_to_class(cls, name: str, value: Any) -> Any: ...
     @classmethod
     def from_db(cls, db: str | None, field_names: Collection[str], values: Collection[Any]) -> Self: ...
-    def _do_update(
-        self,
-        base_qs: QuerySet[Self],
-        using: str | None,
-        pk_val: Any,
-        values: Collection[tuple[Field, type[Model] | None, Any]],
-        update_fields: Iterable[str] | None,
-        forced_update: bool,
-    ) -> bool: ...
     def delete(self, using: Any = ..., keep_parents: bool = ...) -> tuple[int, dict[str, int]]: ...
     async def adelete(self, using: Any = ..., keep_parents: bool = ...) -> tuple[int, dict[str, int]]: ...
     def full_clean(
         self, exclude: Iterable[str] | None = ..., validate_unique: bool = ..., validate_constraints: bool = ...
     ) -> None: ...
     def clean(self) -> None: ...
     def clean_fields(self, exclude: Collection[str] | None = ...) -> None: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/constraints.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/constraints.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/deletion.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/deletion.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import defaultdict
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from typing import Any
 
 from django.db import IntegrityError
 from django.db.models.base import Model
 from django.db.models.fields import Field
 from django.db.models.options import Options
@@ -54,21 +53,20 @@
 
 class RestrictedError(IntegrityError):
     restricted_objects: set[Model]
     def __init__(self, msg: str, restricted_objects: set[Model]) -> None: ...
 
 class Collector:
     using: str
-    origin: Model | QuerySet[Model] | None
     data: dict[type[Model], set[Model] | list[Model]]
-    field_updates: defaultdict[tuple[Field, Any], list[Model]]
-    restricted_objects: defaultdict[Model, defaultdict[Field, set[Model]]]
-    fast_deletes: list[QuerySet[Model]]
-    dependencies: defaultdict[Model, set[Model]]
-    def __init__(self, using: str, origin: Model | QuerySet[Model] | None = None) -> None: ...
+    field_updates: Any
+    restricted_objects: Any
+    fast_deletes: Any
+    dependencies: Any
+    def __init__(self, using: str) -> None: ...
     def add(
         self,
         objs: _IndexableCollection[Model],
         source: type[Model] | None = ...,
         nullable: bool = ...,
         reverse_dependency: bool = ...,
     ) -> list[Model]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/expressions.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/expressions.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import datetime
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 from decimal import Decimal
 from typing import Any, ClassVar, Generic, Literal, TypeVar
 
 from django.db.backends.base.base import BaseDatabaseWrapper
-from django.db.models import Q, fields
+from django.db.models import Q
 from django.db.models.fields import Field
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.query import QuerySet
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 from django.db.models.sql.query import Query
-from django.utils.deconstruct import _Deconstructible
-from django.utils.functional import cached_property
 from typing_extensions import Self, TypeAlias
 
 class SQLiteNumericMixin:
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 _Numeric: TypeAlias = float | Decimal
 
@@ -61,37 +59,35 @@
     is_summary: bool
     filterable: bool
     window_compatible: bool
     def __init__(self, output_field: Field | None = ...) -> None: ...
     def get_db_converters(self, connection: BaseDatabaseWrapper) -> list[Callable]: ...
     def get_source_expressions(self) -> list[Any]: ...
     def set_source_expressions(self, exprs: Sequence[Combinable]) -> None: ...
-    @cached_property
+    @property
     def contains_aggregate(self) -> bool: ...
-    @cached_property
+    @property
     def contains_over_clause(self) -> bool: ...
-    @cached_property
+    @property
     def contains_column_references(self) -> bool: ...
-    @cached_property
-    def contains_subquery(self) -> bool: ...
     def resolve_expression(
         self,
         query: Any = ...,
         allow_joins: bool = ...,
         reuse: set[str] | None = ...,
         summarize: bool = ...,
         for_save: bool = ...,
     ) -> Self: ...
     @property
     def conditional(self) -> bool: ...
     @property
     def field(self) -> Field: ...
-    @cached_property
+    @property
     def output_field(self) -> Field: ...
-    @cached_property
+    @property
     def convert_value(self) -> Callable: ...
     def get_lookup(self, lookup: str) -> type[Lookup] | None: ...
     def get_transform(self, name: str) -> type[Transform] | None: ...
     def relabeled_clone(self, change_map: dict[str | None, str]) -> Self: ...
     def copy(self) -> Self: ...
     def get_group_by_cols(self) -> list[BaseExpression]: ...
     def get_source_fields(self) -> list[Field | None]: ...
@@ -108,30 +104,30 @@
         nulls_first: bool | None = ...,
         nulls_last: bool | None = ...,
     ) -> OrderBy: ...
     def reverse_ordering(self) -> BaseExpression: ...
     def flatten(self) -> Iterator[BaseExpression]: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
 
-class Expression(_Deconstructible, BaseExpression, Combinable): ...
+class Expression(BaseExpression, Combinable):
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class CombinedExpression(SQLiteNumericMixin, Expression):
     connector: str
     lhs: Combinable
     rhs: Combinable
     def __init__(self, lhs: Combinable, connector: str, rhs: Combinable, output_field: Field | None = ...) -> None: ...
 
 class DurationExpression(CombinedExpression):
     def compile(self, side: Combinable, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
 
 class TemporalSubtraction(CombinedExpression):
-    output_field: ClassVar[fields.DurationField]
     def __init__(self, lhs: Combinable, rhs: Combinable) -> None: ...
 
-class F(_Deconstructible, Combinable):
+class F(Combinable):
     name: str
     def __init__(self, name: str) -> None: ...
     def resolve_expression(
         self,
         query: Any = ...,
         allow_joins: bool = ...,
         reuse: set[str] | None = ...,
@@ -149,14 +145,15 @@
     def desc(
         self,
         *,
         nulls_first: bool | None = ...,
         nulls_last: bool | None = ...,
     ) -> OrderBy: ...
     def copy(self) -> F: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class ResolvedOuterRef(F):
     contains_aggregate: ClassVar[bool]
     contains_over_clause: ClassVar[bool]
 
 class OuterRef(F):
     contains_aggregate: ClassVar[bool]
@@ -178,18 +175,20 @@
         compiler: SQLCompiler,
         connection: BaseDatabaseWrapper,
         function: str | None = ...,
         template: str | None = ...,
         arg_joiner: str | None = ...,
         **extra_context: Any,
     ) -> _AsSqlType: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class Value(Expression):
     value: Any
     def __init__(self, value: Any, output_field: Field | None = ...) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class RawSQL(Expression):
     params: list[Any]
     sql: str
     def __init__(self, sql: str, params: Sequence[Any], output_field: Field | None = ...) -> None: ...
 
 class Star(Expression): ...
@@ -210,43 +209,45 @@
 class OrderByList(Func): ...
 
 _E = TypeVar("_E", bound=Q | Combinable)
 
 class ExpressionWrapper(Expression, Generic[_E]):
     def __init__(self, expression: _E, output_field: Field) -> None: ...
     expression: _E
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class NegatedExpression(ExpressionWrapper[_E]):
     def __init__(self, expression: _E) -> None: ...
     def __invert__(self) -> _E: ...  # type: ignore[override]
 
 class When(Expression):
     template: str
     condition: Any
     result: Any
     def __init__(self, condition: Any = ..., then: Any = ..., **lookups: Any) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class Case(Expression):
     template: str
     case_joiner: str
     cases: Any
     default: Any
     extra: Any
     def __init__(
         self, *cases: Any, default: Any | None = ..., output_field: Field | None = ..., **extra: Any
     ) -> None: ...
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class Subquery(BaseExpression, Combinable):
     template: str
     query: Query
     extra: dict[Any, Any]
     def __init__(self, queryset: Query | QuerySet, output_field: Field | None = ..., **extra: Any) -> None: ...
 
 class Exists(Subquery):
-    output_field: ClassVar[fields.BooleanField]
     def __init__(self, queryset: Query | QuerySet, **kwargs: Any) -> None: ...
 
 class OrderBy(Expression):
     template: str
     nulls_first: bool
     nulls_last: bool
     descending: bool
@@ -256,14 +257,15 @@
         expression: Expression | F | Subquery,
         descending: bool = ...,
         nulls_first: bool | None = ...,
         nulls_last: bool | None = ...,
     ) -> None: ...
     def asc(self) -> None: ...  # type: ignore[override]
     def desc(self) -> None: ...  # type: ignore[override]
+    def deconstruct(obj) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class Window(SQLiteNumericMixin, Expression):
     template: str
     contains_aggregate: bool
     contains_over_clause: bool
     partition_by: ExpressionList | None
     order_by: ExpressionList | None
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Model
 from django.db.models.expressions import Col, Combinable
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.db.models.query_utils import Q, RegisterLookupMixin
 from django.forms import Widget
 from django.utils.datastructures import DictWrapper
-from django.utils.functional import _Getter, _StrOrPromise, cached_property
+from django.utils.functional import _Getter, _StrOrPromise
 from typing_extensions import Self, TypeAlias
 
 class Empty: ...
 class NOT_PROVIDED: ...
 
 BLANK_CHOICE_DASH: list[tuple[str, str]]
 
@@ -171,27 +171,30 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
-        db_comment: str | None = ...,
     ) -> None: ...
     def __set__(self, instance: Any, value: _ST) -> None: ...
     # class access
     @overload
     def __get__(self, instance: None, owner: Any) -> _FieldDescriptor[Self]: ...
     # Model instance access
     @overload
-    def __get__(self, instance: object, owner: Any) -> _GT: ...
+    def __get__(self, instance: Model, owner: Any) -> _GT: ...
+    # non-Model instances
+    @overload
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def deconstruct(self) -> tuple[str, str, Sequence[Any], dict[str, Any]]: ...
     def set_attributes_from_name(self, name: str) -> None: ...
     def db_type_parameters(self, connection: BaseDatabaseWrapper) -> DictWrapper: ...
     def db_check(self, connection: BaseDatabaseWrapper) -> str | None: ...
     def db_type(self, connection: BaseDatabaseWrapper) -> str | None: ...
     def db_parameters(self, connection: BaseDatabaseWrapper) -> dict[str, str | None]: ...
     def pre_save(self, model_instance: Model, add: bool) -> Any: ...
@@ -205,15 +208,15 @@
         form_class: type[forms.Field] | None = ...,
         choices_form_class: type[forms.ChoiceField] | None = ...,
         **kwargs: Any,
     ) -> forms.Field: ...
     def save_form_data(self, instance: Model, data: Any) -> None: ...
     def contribute_to_class(self, cls: type[Model], name: str, private_only: bool = ...) -> None: ...
     def to_python(self, value: Any) -> Any: ...
-    @cached_property
+    @property
     def validators(self) -> list[validators._ValidatorCallable]: ...
     def run_validators(self, value: Any) -> None: ...
     def validate(self, value: Any, model_instance: Model | None) -> None: ...
     def clean(self, value: Any, model_instance: Model | None) -> Any: ...
     def get_choices(
         self,
         include_blank: bool = ...,
@@ -224,15 +227,15 @@
     def _get_flatchoices(self) -> list[_Choice]: ...
     @property
     def flatchoices(self) -> list[_Choice]: ...
     def has_default(self) -> bool: ...
     def get_default(self) -> Any: ...
     def check(self, **kwargs: Any) -> list[CheckMessage]: ...
     def get_col(self, alias: str, output_field: Field | None = ...) -> Col: ...
-    @cached_property
+    @property
     def cached_col(self) -> Col: ...
     def value_from_object(self, obj: Model) -> _GT: ...
     def get_attname(self) -> str: ...
     def get_attname_column(self) -> tuple[str, str]: ...
     def value_to_string(self, obj: Model) -> str: ...
 
 class IntegerField(Field[_ST, _GT]):
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/files.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/files.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.core.files.images import ImageFile
 from django.core.files.storage import Storage
 from django.db.models.base import Model
 from django.db.models.fields import Field, _ErrorMessagesMapping, _FieldChoices
 from django.db.models.query_utils import DeferredAttribute
 from django.utils._os import _PathCompatible
 from django.utils.functional import _StrOrPromise
+from typing_extensions import Self
 
 class FieldFile(File):
     instance: Model
     field: FileField
     storage: Storage
     name: str | None
     def __init__(self, instance: Model, field: FileField, name: str | None) -> None: ...
@@ -70,15 +71,18 @@
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
     # class access
     @overload
     def __get__(self, instance: None, owner: Any) -> FileDescriptor: ...
     # Model instance access
     @overload
-    def __get__(self, instance: object, owner: Any) -> Any: ...
+    def __get__(self, instance: Model, owner: Any) -> Any: ...
+    # non-Model instances
+    @overload
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def generate_filename(self, instance: Model | None, filename: _PathCompatible) -> str: ...
 
 class ImageFileDescriptor(FileDescriptor):
     field: ImageField
     def __set__(self, instance: Model, value: str | None) -> None: ...
 
 class ImageFieldFile(ImageFile, FieldFile):
@@ -95,9 +99,12 @@
         **kwargs: Any,
     ) -> None: ...
     # class access
     @overload
     def __get__(self, instance: None, owner: Any) -> ImageFileDescriptor: ...
     # Model instance access
     @overload
-    def __get__(self, instance: object, owner: Any) -> Any: ...
+    def __get__(self, instance: Model, owner: Any) -> Any: ...
+    # non-Model instances
+    @overload
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def update_dimension_fields(self, instance: Model, force: bool = ..., *args: Any, **kwargs: Any) -> None: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/json.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/json.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from collections.abc import Callable
-from typing import Any, ClassVar
+from typing import Any
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import lookups
-from django.db.models.fields import TextField
 from django.db.models.lookups import PostgresOperatorLookup, Transform
 from django.db.models.sql.compiler import SQLCompiler
 from django.utils.functional import _StrOrPromise
 from typing_extensions import Self
 
 from . import Field
 from .mixins import CheckFieldDefaultMixin
@@ -54,15 +53,14 @@
     postgres_nested_operator: str
     def __init__(self, key_name: Any, *args: Any, **kwargs: Any) -> None: ...
     def preprocess_lhs(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> Any: ...
 
 class KeyTextTransform(KeyTransform):
     postgres_operator: str
     postgres_nested_operator: str
-    output_field: ClassVar[TextField]
     @classmethod
     def from_lookup(cls, lookup: str) -> Self: ...
 
 KT: Callable[[str], KeyTextTransform]
 
 class KeyTransformTextLookupMixin:
     def __init__(self, key_transform: Any, *args: Any, **kwargs: Any) -> None: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/mixins.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/mixins.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/related.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/related.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 from django.db.models.fields.related_descriptors import ReverseManyToOneDescriptor as ReverseManyToOneDescriptor
 from django.db.models.fields.related_descriptors import ReverseOneToOneDescriptor as ReverseOneToOneDescriptor
 from django.db.models.fields.reverse_related import ForeignObjectRel as ForeignObjectRel
 from django.db.models.fields.reverse_related import ManyToManyRel as ManyToManyRel
 from django.db.models.fields.reverse_related import ManyToOneRel as ManyToOneRel
 from django.db.models.fields.reverse_related import OneToOneRel as OneToOneRel
 from django.db.models.query_utils import FilteredRelation, PathInfo, Q
-from django.utils.functional import _StrOrPromise, cached_property
+from django.utils.functional import _StrOrPromise
 from typing_extensions import Self
 
 RECURSIVE_RELATIONSHIP_CONSTANT: Literal["self"]
 
 def resolve_relation(scope_model: type[Model], relation: str | type[Model]) -> str | type[Model]: ...
 
+_M = TypeVar("_M", bound=Model)
 # __set__ value type
 _ST = TypeVar("_ST")
 # __get__ return type
 _GT = TypeVar("_GT")
 
 class RelatedField(FieldCacheMixin, Field[_ST, _GT]):
     one_to_many: bool
@@ -36,45 +37,15 @@
     many_to_many: bool
     many_to_one: bool
     opts: Any
 
     remote_field: ForeignObjectRel
     rel_class: type[ForeignObjectRel]
     swappable: bool
-    def __init__(
-        self,
-        related_name: str | None = ...,
-        related_query_name: str | None = ...,
-        limit_choices_to: _AllLimitChoicesTo | None = ...,
-        *,
-        verbose_name: _StrOrPromise | None = ...,
-        name: str | None = ...,
-        primary_key: bool = ...,
-        max_length: int | None = ...,
-        unique: bool = ...,
-        blank: bool = ...,
-        null: bool = ...,
-        db_index: bool = ...,
-        rel: ForeignObjectRel | None = ...,
-        default: Any = ...,
-        editable: bool = ...,
-        serialize: bool = ...,
-        unique_for_date: str | None = ...,
-        unique_for_month: str | None = ...,
-        unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
-        help_text: _StrOrPromise = ...,
-        db_column: str | None = ...,
-        db_tablespace: str | None = ...,
-        auto_created: bool = ...,
-        validators: Iterable[validators._ValidatorCallable] = ...,
-        error_messages: _ErrorMessagesMapping | None = ...,
-        db_comment: str | None = ...,
-    ) -> None: ...
-    @cached_property
+    @property
     def related_model(self) -> type[Model] | Literal["self"]: ...  # type: ignore[override]
     def get_forward_related_filter(self, obj: Model) -> dict[str, int | UUID]: ...
     def get_reverse_related_filter(self, obj: Model) -> Q: ...
     @property
     def swappable_setting(self) -> str | None: ...
     def set_attributes_from_rel(self) -> None: ...
     def do_related_class(self, other: type[Model], cls: type[Model]) -> None: ...
@@ -98,47 +69,51 @@
         rel: ForeignObjectRel | None = ...,
         related_name: str | None = ...,
         related_query_name: str | None = ...,
         limit_choices_to: _AllLimitChoicesTo | None = ...,
         parent_link: bool = ...,
         swappable: bool = ...,
         *,
+        db_constraint: bool = ...,
         verbose_name: _StrOrPromise | None = ...,
         name: str | None = ...,
         primary_key: bool = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
-        db_comment: str | None = ...,
     ) -> None: ...
     # class access
     @overload
     def __get__(self, instance: None, owner: Any) -> ForwardManyToOneDescriptor[Self]: ...
     # Model instance access
     @overload
-    def __get__(self, instance: object, owner: Any) -> _GT: ...
+    def __get__(self, instance: Model, owner: Any) -> _GT: ...
+    # non-Model instances
+    @overload
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def resolve_related_fields(self) -> list[tuple[Field, Field]]: ...
-    @cached_property
+    @property
     def related_fields(self) -> list[tuple[Field, Field]]: ...
-    @cached_property
+    @property
     def reverse_related_fields(self) -> list[tuple[Field, Field]]: ...
-    @cached_property
+    @property
     def local_related_fields(self) -> tuple[Field, ...]: ...
-    @cached_property
+    @property
     def foreign_related_fields(self) -> tuple[Field, ...]: ...
 
 class ForeignKey(ForeignObject[_ST, _GT]):
     _pyi_private_set_type: Any | Combinable
     _pyi_private_get_type: Any
 
     remote_field: ManyToOneRel
@@ -168,18 +143,18 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
-        db_comment: str | None = ...,
     ) -> None: ...
 
 class OneToOneField(ForeignKey[_ST, _GT]):
     _pyi_private_set_type: Any | Combinable
     _pyi_private_get_type: Any
 
     remote_field: OneToOneRel
@@ -209,30 +184,32 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
-        db_comment: str | None = ...,
     ) -> None: ...
     # class access
     @overload
     def __get__(self, instance: None, owner: Any) -> ForwardOneToOneDescriptor[Self]: ...
     # Model instance access
     @overload
-    def __get__(self, instance: object, owner: Any) -> _GT: ...
+    def __get__(self, instance: Model, owner: Any) -> _GT: ...
+    # non-Model instances
+    @overload
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
 
-_Through = TypeVar("_Through", bound=Model)
 _To = TypeVar("_To", bound=Model)
 
-class ManyToManyField(RelatedField[Any, Any], Generic[_To, _Through]):
+class ManyToManyField(RelatedField[Any, Any], Generic[_To, _M]):
     description: str
     has_null_arg: bool
     swappable: bool
 
     many_to_many: Literal[True]
     many_to_one: Literal[False]
     one_to_many: Literal[False]
@@ -243,15 +220,15 @@
     def __init__(
         self,
         to: type[_To] | str,
         related_name: str | None = ...,
         related_query_name: str | None = ...,
         limit_choices_to: _AllLimitChoicesTo | None = ...,
         symmetrical: bool | None = ...,
-        through: type[_Through] | str | None = ...,
+        through: type[_M] | str | None = ...,
         through_fields: tuple[str, str] | None = ...,
         db_constraint: bool = ...,
         db_table: str | None = ...,
         swappable: bool = ...,
         *,
         verbose_name: _StrOrPromise | None = ...,
         name: str | None = ...,
@@ -266,24 +243,27 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
-        db_comment: str | None = ...,
     ) -> None: ...
     # class access
     @overload
-    def __get__(self, instance: None, owner: Any) -> ManyToManyDescriptor[_To, _Through]: ...
+    def __get__(self, instance: None, owner: Any) -> ManyToManyDescriptor[_M]: ...
     # Model instance access
     @overload
-    def __get__(self, instance: object, owner: Any) -> ManyRelatedManager[_To]: ...
+    def __get__(self, instance: Model, owner: Any) -> ManyRelatedManager[_To]: ...
+    # non-Model instances
+    @overload
+    def __get__(self, instance: Any, owner: Any) -> Self: ...
     def get_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
     def get_reverse_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
     def contribute_to_related_class(self, cls: type[Model], related: RelatedField) -> None: ...
     def m2m_db_table(self) -> str: ...
     def m2m_column_name(self) -> str: ...
     def m2m_reverse_name(self) -> str: ...
     def m2m_reverse_field_name(self) -> str: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/related_descriptors.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/related_descriptors.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 from typing import Any, Generic, NoReturn, TypeVar, overload
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models.base import Model
 from django.db.models.fields import Field
 from django.db.models.fields.related import ForeignKey, ManyToManyField, RelatedField
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel, OneToOneRel
-from django.db.models.manager import BaseManager, Manager
+from django.db.models.manager import BaseManager, RelatedManager
 from django.db.models.query import QuerySet
 from django.db.models.query_utils import DeferredAttribute
-from django.utils.functional import cached_property
 from typing_extensions import Self
 
 _M = TypeVar("_M", bound=Model)
 _F = TypeVar("_F", bound=Field)
 _From = TypeVar("_From", bound=Model)
-_Through = TypeVar("_Through", bound=Model)
 _To = TypeVar("_To", bound=Model)
 
 class ForeignKeyDeferredAttribute(DeferredAttribute):
     field: RelatedField
 
 class ForwardManyToOneDescriptor(Generic[_F]):
     field: _F
     def __init__(self, field_with_rel: _F) -> None: ...
-    @cached_property
+    @property
     def RelatedObjectDoesNotExist(self) -> type[ObjectDoesNotExist]: ...
     def is_cached(self, instance: Model) -> bool: ...
     def get_queryset(self, **hints: Any) -> QuerySet: ...
     def get_prefetch_queryset(
         self, instances: list[Model], queryset: QuerySet | None = ...
     ) -> tuple[QuerySet, Callable, Callable, bool, str, bool]: ...
     def get_object(self, instance: Model) -> Model: ...
@@ -49,15 +47,15 @@
             place = OneToOneField(Place, related_name='restaurant')
 
     ``Place.restaurant`` is a ``ReverseOneToOneDescriptor`` instance.
     """
 
     related: OneToOneRel
     def __init__(self, related: OneToOneRel) -> None: ...
-    @cached_property
+    @property
     def RelatedObjectDoesNotExist(self) -> type[ObjectDoesNotExist]: ...
     def is_cached(self, instance: _From) -> bool: ...
     def get_queryset(self, **hints: Any) -> QuerySet[_To]: ...
     def get_prefetch_queryset(
         self, instances: list[_From], queryset: QuerySet[_To] | None = ...
     ) -> tuple[QuerySet[_To], Callable[..., Any], Callable[..., Any], bool, str, bool]: ...
     @overload
@@ -76,66 +74,48 @@
 
     ``Parent.children`` is a ``ReverseManyToOneDescriptor`` instance.
     """
 
     rel: ManyToOneRel
     field: ForeignKey
     def __init__(self, rel: ManyToOneRel) -> None: ...
-    @cached_property
+    @property
     def related_manager_cls(self) -> type[RelatedManager[Any]]: ...
     @overload
     def __get__(self, instance: None, cls: Any = ...) -> Self: ...
     @overload
-    def __get__(self, instance: Model, cls: Any = ...) -> RelatedManager[Any]: ...
+    def __get__(self, instance: Model, cls: Any = ...) -> type[RelatedManager[Any]]: ...
     def __set__(self, instance: Any, value: Any) -> NoReturn: ...
 
-# Fake class, Django defines 'RelatedManager' inside a function body
-class RelatedManager(Manager[_M], Generic[_M]):
-    related_val: tuple[int, ...]
-    def add(self, *objs: _M | int, bulk: bool = ...) -> None: ...
-    async def aadd(self, *objs: _M | int, bulk: bool = ...) -> None: ...
-    def remove(self, *objs: _M | int, bulk: bool = ...) -> None: ...
-    async def aremove(self, *objs: _M | int, bulk: bool = ...) -> None: ...
-    def set(self, objs: QuerySet[_M] | Iterable[_M | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
-    async def aset(self, objs: QuerySet[_M] | Iterable[_M | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
-    def clear(self) -> None: ...
-    async def aclear(self) -> None: ...
-    def __call__(self, *, manager: str) -> RelatedManager[_M]: ...
-
 def create_reverse_many_to_one_manager(
     superclass: type[BaseManager[_M]], rel: ManyToOneRel
 ) -> type[RelatedManager[_M]]: ...
 
-class ManyToManyDescriptor(ReverseManyToOneDescriptor, Generic[_To, _Through]):
+class ManyToManyDescriptor(ReverseManyToOneDescriptor, Generic[_M]):
     """
     In the example::
 
         class Pizza(Model):
             toppings = ManyToManyField(Topping, related_name='pizzas')
 
     ``Pizza.toppings`` and ``Topping.pizzas`` are ``ManyToManyDescriptor``
     instances.
     """
 
     # 'field' here is 'rel.field'
     rel: ManyToManyRel  # type: ignore[assignment]
-    field: ManyToManyField[_To, _Through]  # type: ignore[assignment]
+    field: ManyToManyField[Any, _M]  # type: ignore[assignment]
     reverse: bool
     def __init__(self, rel: ManyToManyRel, reverse: bool = ...) -> None: ...
     @property
-    def through(self) -> type[_Through]: ...
-    @cached_property
-    def related_manager_cls(self) -> type[ManyRelatedManager[_To]]: ...  # type: ignore[override]
-    @overload  # type: ignore[override]
-    def __get__(self, instance: None, cls: Any = ...) -> Self: ...
-    @overload
-    def __get__(self, instance: Model, cls: Any = ...) -> ManyRelatedManager[_To]: ...
+    def through(self) -> type[_M]: ...
+    @property
+    def related_manager_cls(self) -> type[ManyRelatedManager[Any]]: ...  # type: ignore[override]
 
-# Fake class, Django defines 'ManyRelatedManager' inside a function body
-class ManyRelatedManager(Manager[_M], Generic[_M]):
+class ManyRelatedManager(BaseManager[_M], Generic[_M]):
     related_val: tuple[int, ...]
     def add(self, *objs: _M | int, bulk: bool = ...) -> None: ...
     async def aadd(self, *objs: _M | int, bulk: bool = ...) -> None: ...
     def remove(self, *objs: _M | int, bulk: bool = ...) -> None: ...
     async def aremove(self, *objs: _M | int, bulk: bool = ...) -> None: ...
     def set(self, objs: QuerySet[_M] | Iterable[_M | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
     async def aset(self, objs: QuerySet[_M] | Iterable[_M | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/related_lookups.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/related_lookups.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/fields/reverse_related.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/fields/reverse_related.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from django.db.models.base import Model
 from django.db.models.fields import AutoField, Field, _AllLimitChoicesTo, _ChoicesList, _LimitChoicesTo
 from django.db.models.fields.related import ForeignKey, ForeignObject, ManyToManyField, OneToOneField
 from django.db.models.lookups import Lookup, StartsWith
 from django.db.models.query_utils import FilteredRelation, PathInfo
 from django.db.models.sql.where import WhereNode
-from django.utils.functional import cached_property
 
 from .mixins import FieldCacheMixin
 
 # Common note: `model` and `through` can be of type `str` when passed to `__init__`.
 # When parent's `contribute_to_class` is called (during startup),
 # strings are resolved to real model classes.
 # Thus `str` is acceptable in __init__, but instance attribute `model` is always
@@ -39,31 +38,31 @@
         to: type[Model] | str,
         related_name: str | None = ...,
         related_query_name: str | None = ...,
         limit_choices_to: _AllLimitChoicesTo | None = ...,
         parent_link: bool = ...,
         on_delete: Callable = ...,
     ) -> None: ...
-    @cached_property
+    @property
     def hidden(self) -> bool: ...
-    @cached_property
+    @property
     def name(self) -> str: ...
     @property
     def remote_field(self) -> ForeignObject: ...
     @property
     def target_field(self) -> AutoField: ...
-    @cached_property
+    @property
     def related_model(self) -> type[Model] | Literal["self"]: ...
-    @cached_property
+    @property
     def many_to_many(self) -> bool: ...
-    @cached_property
+    @property
     def many_to_one(self) -> bool: ...
-    @cached_property
+    @property
     def one_to_many(self) -> bool: ...
-    @cached_property
+    @property
     def one_to_one(self) -> bool: ...
     def get_lookup(self, lookup_name: str) -> type[Lookup] | None: ...
     def get_internal_type(self) -> str: ...
     @property
     def db_type(self) -> Any: ...
     # Yes, seems that `get_choices` will fail if `limit_choices_to=None`
     # and `self.limit_choices_to` is callable.
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 from .math import Power as Power
 from .math import Radians as Radians
 from .math import Round as Round
 from .math import Sign as Sign
 from .math import Sin as Sin
 from .math import Sqrt as Sqrt
 from .math import Tan as Tan
-from .text import MD5 as MD5
 from .text import SHA1 as SHA1
 from .text import SHA224 as SHA224
 from .text import SHA256 as SHA256
 from .text import SHA384 as SHA384
 from .text import SHA512 as SHA512
 from .text import Chr as Chr
 from .text import Concat as Concat
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/comparison.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/comparison.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, ClassVar
+from typing import Any
 
 from django.db.models import Func
 from django.db.models.fields import Field
 from django.db.models.fields.json import JSONField
 
 class Cast(Func):
     def __init__(self, expression: Any, output_field: str | Field) -> None: ...
@@ -12,11 +12,11 @@
 class Collate(Func):
     def __init__(self, expression: Any, collation: str) -> None: ...
 
 class Greatest(Func): ...
 
 class JSONObject(Func):
     def __init__(self, **fields: Any) -> None: ...
-    output_field: ClassVar[JSONField]
+    output_field: JSONField
 
 class Least(Func): ...
 class NullIf(Func): ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/datetime.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/datetime.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, ClassVar
+from typing import Any
 
 from django.db import models
 from django.db.models import Func, Transform
 
 class TimezoneMixin:
     tzinfo: Any
     def get_tzname(self) -> str | None: ...
 
 class Extract(TimezoneMixin, Transform):
     lookup_name: str
-    output_field: ClassVar[models.IntegerField]
+    output_field: models.IntegerField
     def __init__(
         self, expression: Any, lookup_name: str | None = ..., tzinfo: Any | None = ..., **extra: Any
     ) -> None: ...
 
 class ExtractYear(Extract): ...
 class ExtractIsoYear(Extract): ...
 class ExtractMonth(Extract): ...
@@ -23,29 +23,29 @@
 class ExtractIsoWeekDay(Extract): ...
 class ExtractQuarter(Extract): ...
 class ExtractHour(Extract): ...
 class ExtractMinute(Extract): ...
 class ExtractSecond(Extract): ...
 
 class Now(Func):
-    output_field: ClassVar[models.DateTimeField]
+    output_field: models.DateTimeField
 
 class TruncBase(TimezoneMixin, Transform):
     kind: str
     tzinfo: Any
 
 class Trunc(TruncBase): ...
 class TruncYear(TruncBase): ...
 class TruncQuarter(TruncBase): ...
 class TruncMonth(TruncBase): ...
 class TruncWeek(TruncBase): ...
 class TruncDay(TruncBase): ...
 
 class TruncDate(TruncBase):
-    output_field: ClassVar[models.DateField]
+    output_field: models.DateField
 
 class TruncTime(TruncBase):
-    output_field: ClassVar[models.TimeField]
+    output_field: models.TimeField
 
 class TruncHour(TruncBase): ...
 class TruncMinute(TruncBase): ...
 class TruncSecond(TruncBase): ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/math.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/math.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/text.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/text.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, ClassVar
+from typing import Any
 
 from django.db import models
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Func, Transform
 from django.db.models.expressions import Combinable, Expression, Value
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 
@@ -27,42 +27,41 @@
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
     def as_mysql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Concat(Func):
     def __init__(self, *expressions: Any, **extra: Any) -> None: ...
 
 class Left(Func):
-    output_field: ClassVar[models.CharField]
+    output_field: models.CharField
     def __init__(self, expression: Expression | str, length: Expression | int, **extra: Any) -> None: ...
     def get_substr(self) -> Substr: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Length(Transform):
-    output_field: ClassVar[models.IntegerField]
+    output_field: models.IntegerField
     def as_mysql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Lower(Transform): ...
 
 class LPad(Func):
-    output_field: ClassVar[models.CharField]
+    output_field: models.CharField
     def __init__(
         self, expression: Expression | str, length: Expression | int | None, fill_text: Expression = ..., **extra: Any
     ) -> None: ...
 
 class LTrim(Transform): ...
-class MD5(OracleHashMixin, Transform): ...
 
 class Ord(Transform):
-    output_field: ClassVar[models.IntegerField]
+    output_field: models.IntegerField
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
     def as_mysql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Repeat(Func):
-    output_field: ClassVar[models.CharField]
+    output_field: models.CharField
     def __init__(self, expression: Expression | str, number: Expression | int | None, **extra: Any) -> None: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Replace(Func):
     def __init__(self, expression: Combinable | str, text: Value, replacement: Value = ..., **extra: Any) -> None: ...
 
 class Reverse(Transform):
@@ -79,21 +78,21 @@
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class SHA256(MySQLSHA2Mixin, OracleHashMixin, PostgreSQLSHAMixin, Transform): ...
 class SHA384(MySQLSHA2Mixin, OracleHashMixin, PostgreSQLSHAMixin, Transform): ...
 class SHA512(MySQLSHA2Mixin, OracleHashMixin, PostgreSQLSHAMixin, Transform): ...
 
 class StrIndex(Func):
-    output_field: ClassVar[models.IntegerField]
+    output_field: models.IntegerField
     def as_postgresql(
         self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any
     ) -> _AsSqlType: ...
 
 class Substr(Func):
-    output_field: ClassVar[models.CharField]
+    output_field: models.CharField
     def __init__(
         self, expression: Expression | str, pos: Expression | int, length: Expression | int | None = ..., **extra: Any
     ) -> None: ...
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Trim(Transform): ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/functions/window.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/functions/window.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Any, ClassVar
+from typing import Any
 
 from django.db import models
 from django.db.models.expressions import Func
 
 class CumeDist(Func):
-    output_field: ClassVar[models.FloatField]
+    output_field: models.FloatField
 
 class DenseRank(Func):
-    output_field: ClassVar[models.IntegerField]
+    output_field: models.IntegerField
 
 class FirstValue(Func): ...
 
 class LagLeadFunction(Func):
     def __init__(self, expression: str | None, offset: int = ..., default: int | None = ..., **extra: Any) -> None: ...
 
 class Lag(LagLeadFunction): ...
@@ -19,17 +19,17 @@
 class Lead(LagLeadFunction): ...
 
 class NthValue(Func):
     def __init__(self, expression: str | None, nth: int = ..., **extra: Any) -> None: ...
 
 class Ntile(Func):
     def __init__(self, num_buckets: int = ..., **extra: Any) -> None: ...
-    output_field: ClassVar[models.IntegerField]
+    output_field: models.IntegerField
 
 class PercentRank(Func):
-    output_field: ClassVar[models.FloatField]
+    output_field: models.FloatField
 
 class Rank(Func):
-    output_field: ClassVar[models.IntegerField]
+    output_field: models.IntegerField
 
 class RowNumber(Func):
-    output_field: ClassVar[models.IntegerField]
+    output_field: models.IntegerField
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/indexes.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/indexes.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/lookups.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/lookups.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from collections.abc import Iterable, Mapping
 from typing import Any, Generic, Literal, TypeVar
 
-from db.models import BooleanField
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.expressions import Expression, Func
 from django.db.models.query_utils import RegisterLookupMixin
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType, _ParamT
 from django.utils.datastructures import OrderedSet
-from django.utils.functional import cached_property
 from typing_extensions import Self
 
 _T = TypeVar("_T")
 
 class Lookup(Generic[_T]):
     lookup_name: str
     prepare_rhs: bool
@@ -33,19 +31,17 @@
     ) -> _AsSqlType: ...
     def process_rhs(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def rhs_is_direct_value(self) -> bool: ...
     def relabeled_clone(self, relabels: Mapping[str, str]) -> Self: ...
     def get_group_by_cols(self) -> list[Expression]: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
-    @cached_property
-    def output_field(self) -> BooleanField: ...
-    @cached_property
+    @property
     def contains_aggregate(self) -> bool: ...
-    @cached_property
+    @property
     def contains_over_clause(self) -> bool: ...
     @property
     def is_summary(self) -> bool: ...
     @property
     def identity(self) -> tuple[type[Lookup], Any, Any]: ...
 
 class Transform(RegisterLookupMixin, Func):
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/manager.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/manager.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import datetime
 from collections.abc import AsyncIterator, Collection, Iterable, Iterator, MutableMapping, Sequence
 from typing import Any, Generic, NoReturn, TypeVar, overload
 
+from django.db.models import Combinable
 from django.db.models.base import Model
-from django.db.models.expressions import Combinable, OrderBy
 from django.db.models.query import QuerySet, RawQuerySet
 from typing_extensions import Self
 
 from django_stubs_ext import ValuesQuerySet
 
 _T = TypeVar("_T", bound=Model, covariant=True)
 
 class BaseManager(Generic[_T]):
     creation_counter: int
     auto_created: bool
     use_in_migrations: bool
     name: str
     model: type[_T]
     _db: str | None
-    def __new__(cls, *args: Any, **kwargs: Any) -> Self: ...
     def __init__(self) -> None: ...
-    def __class_getitem__(cls, *args: Any, **kwargs: Any) -> type[Self]: ...
     def deconstruct(
         self,
     ) -> tuple[bool, str | None, str | None, Sequence[Any] | None, dict[str, Any] | None]: ...
     def check(self, **kwargs: Any) -> list[Any]: ...
     @classmethod
     def from_queryset(cls, queryset_class: type[QuerySet[_T]], class_name: str | None = ...) -> type[Self]: ...
     @classmethod
@@ -32,15 +30,15 @@
     def contribute_to_class(self, cls: type[Model], name: str) -> None: ...
     def db_manager(self, using: str | None = ..., hints: dict[str, Model] | None = ...) -> Self: ...
     @property
     def db(self) -> str: ...
     def get_queryset(self) -> QuerySet[_T]: ...
     # NOTE: The following methods are in common with QuerySet, but note that the use of QuerySet as a return type
     # rather than a self-type (_QS), since Manager's QuerySet-like methods return QuerySets and not Managers.
-    def iterator(self, chunk_size: int | None = ...) -> Iterator[_T]: ...
+    def iterator(self, chunk_size: int = ...) -> Iterator[_T]: ...
     def aiterator(self, chunk_size: int = ...) -> AsyncIterator[_T]: ...
     def aggregate(self, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
     async def aaggregate(self, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
     def get(self, *args: Any, **kwargs: Any) -> _T: ...
     async def aget(self, *args: Any, **kwargs: Any) -> _T: ...
     def create(self, **kwargs: Any) -> _T: ...
     async def acreate(self, **kwargs: Any) -> _T: ...
@@ -68,24 +66,24 @@
     async def aget_or_create(
         self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
     ) -> tuple[_T, bool]: ...
     def update_or_create(self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any) -> tuple[_T, bool]: ...
     async def aupdate_or_create(
         self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
     ) -> tuple[_T, bool]: ...
-    def earliest(self, *fields: str | OrderBy) -> _T: ...
-    async def aearliest(self, *fields: str | OrderBy) -> _T: ...
-    def latest(self, *fields: str | OrderBy) -> _T: ...
-    async def alatest(self, *fields: str | OrderBy) -> _T: ...
+    def earliest(self, *fields: Any, field_name: Any | None = ...) -> _T: ...
+    async def aearliest(self, *fields: Any, field_name: Any | None = ...) -> _T: ...
+    def latest(self, *fields: Any, field_name: Any | None = ...) -> _T: ...
+    async def alatest(self, *fields: Any, field_name: Any | None = ...) -> _T: ...
     def first(self) -> _T | None: ...
     async def afirst(self) -> _T | None: ...
     def last(self) -> _T | None: ...
     async def alast(self) -> _T | None: ...
-    def in_bulk(self, id_list: Iterable[Any] | None = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
-    async def ain_bulk(self, id_list: Iterable[Any] | None = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
+    def in_bulk(self, id_list: Iterable[Any] = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
+    async def ain_bulk(self, id_list: Iterable[Any] = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
     def update(self, **kwargs: Any) -> int: ...
     async def aupdate(self, **kwargs: Any) -> int: ...
     def exists(self) -> bool: ...
     async def aexists(self) -> bool: ...
     def explain(self, *, format: Any | None = ..., **options: Any) -> str: ...
     async def aexplain(self, *, format: Any | None = ..., **options: Any) -> str: ...
     def contains(self, objs: Model) -> bool: ...
@@ -141,14 +139,27 @@
     def only(self, *fields: Any) -> QuerySet[_T]: ...
     def using(self, alias: str | None) -> QuerySet[_T]: ...
     @property
     def ordered(self) -> bool: ...
 
 class Manager(BaseManager[_T]): ...
 
+# Fake to make ManyToMany work
+class RelatedManager(Manager[_T]):
+    related_val: tuple[int, ...]
+    def add(self, *objs: _T | int, bulk: bool = ...) -> None: ...
+    async def aadd(self, *objs: _T | int, bulk: bool = ...) -> None: ...
+    def remove(self, *objs: _T | int, bulk: bool = ...) -> None: ...
+    async def aremove(self, *objs: _T | int, bulk: bool = ...) -> None: ...
+    def set(self, objs: QuerySet[_T] | Iterable[_T | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
+    async def aset(self, objs: QuerySet[_T] | Iterable[_T | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
+    def clear(self) -> None: ...
+    async def aclear(self) -> None: ...
+    def __call__(self, *, manager: str) -> RelatedManager[_T]: ...
+
 class ManagerDescriptor:
     manager: BaseManager
     def __init__(self, manager: BaseManager) -> None: ...
     @overload
     def __get__(self, instance: None, cls: type[Model] | None = ...) -> BaseManager: ...
     @overload
     def __get__(self, instance: Model, cls: type[Model] | None = ...) -> NoReturn: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/options.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/options.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from django.db.models.constraints import BaseConstraint, UniqueConstraint
 from django.db.models.fields import AutoField, Field
 from django.db.models.fields.related import ManyToManyField, OneToOneField
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.db.models.manager import Manager
 from django.db.models.query_utils import PathInfo
 from django.utils.datastructures import ImmutableList, _ListOrTuple
-from django.utils.functional import _StrOrPromise, cached_property
+from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 PROXY_PARENTS: object
 EMPTY_RELATION_TREE: Any
 IMMUTABLE_WARNING: str
 DEFAULT_NAMES: tuple[str, ...]
 
@@ -97,32 +97,32 @@
     def setup_pk(self, field: GenericForeignKey | Field[Any, Any]) -> None: ...
     def setup_proxy(self, target: type[Model]) -> None: ...
     def can_migrate(self, connection: BaseDatabaseWrapper | str) -> bool: ...
     @property
     def verbose_name_raw(self) -> str: ...
     @property
     def swapped(self) -> str | None: ...
-    @cached_property
+    @property
     def fields_map(self) -> dict[str, Field[Any, Any] | ForeignObjectRel]: ...
-    @cached_property
+    @property
     def managers(self) -> ImmutableList[Manager]: ...
-    @cached_property
+    @property
     def managers_map(self) -> dict[str, Manager]: ...
-    @cached_property
+    @property
     def base_manager(self) -> Manager: ...
-    @cached_property
+    @property
     def default_manager(self) -> Manager | None: ...
-    @cached_property
+    @property
     def fields(self) -> ImmutableList[Field[Any, Any]]: ...
     def get_field(self, field_name: str) -> Field | ForeignObjectRel | GenericForeignKey: ...
     def get_base_chain(self, model: type[Model]) -> list[type[Model]]: ...
     def get_parent_list(self) -> list[type[Model]]: ...
     def get_ancestor_link(self, ancestor: type[Model]) -> OneToOneField | None: ...
     def get_path_to_parent(self, parent: type[Model]) -> list[PathInfo]: ...
     def get_path_from_parent(self, parent: type[Model]) -> list[PathInfo]: ...
     def get_fields(
         self, include_parents: bool = ..., include_hidden: bool = ...
     ) -> list[Field[Any, Any] | ForeignObjectRel | GenericForeignKey]: ...
-    @cached_property
+    @property
     def total_unique_constraints(self) -> list[UniqueConstraint]: ...
-    @cached_property
+    @property
     def db_returning_fields(self) -> list[Field[Any, Any]]: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/query.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/query.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import datetime
 from collections.abc import AsyncIterator, Collection, Iterable, Iterator, MutableMapping, Reversible, Sequence, Sized
 from typing import Any, Generic, NamedTuple, TypeVar, overload
 
 from django.db.backends.utils import _ExecuteQuery
 from django.db.models import Manager
 from django.db.models.base import Model
-from django.db.models.expressions import Combinable, OrderBy
+from django.db.models.expressions import Combinable
 from django.db.models.sql.query import Query, RawQuery
-from django.utils.functional import cached_property
 from typing_extensions import Self, TypeAlias
 
 _T = TypeVar("_T", bound=Model, covariant=True)
 _Row = TypeVar("_Row", covariant=True)
 _QS = TypeVar("_QS", bound=_QuerySet)
 _TupleT = TypeVar("_TupleT", bound=tuple[Any, ...], covariant=True)
 
@@ -19,15 +18,14 @@
 REPR_OUTPUT_SIZE: int
 
 class BaseIterable(Generic[_Row]):
     queryset: QuerySet[Model]
     chunked_fetch: bool
     chunk_size: int
     def __init__(self, queryset: QuerySet[Model], chunked_fetch: bool = ..., chunk_size: int = ...) -> None: ...
-    def __aiter__(self) -> AsyncIterator[_Row]: ...
 
 class ModelIterable(Generic[_T], BaseIterable[_T]):
     def __iter__(self) -> Iterator[_T]: ...
 
 class RawModelIterable(BaseIterable[dict[str, Any]]):
     def __iter__(self) -> Iterator[dict[str, Any]]: ...
 
@@ -62,15 +60,15 @@
     def __class_getitem__(cls: type[_QS], item: type[_T]) -> type[_QS]: ...
     def __getstate__(self) -> dict[str, Any]: ...
     # Technically, the other QuerySet must be of the same type _T, but _T is covariant
     def __and__(self, other: _QuerySet[_T, _Row]) -> Self: ...
     def __or__(self, other: _QuerySet[_T, _Row]) -> Self: ...
     # IMPORTANT: When updating any of the following methods' signatures, please ALSO modify
     # the corresponding method in BaseManager.
-    def iterator(self, chunk_size: int | None = ...) -> Iterator[_Row]: ...
+    def iterator(self, chunk_size: int = ...) -> Iterator[_Row]: ...
     def aiterator(self, chunk_size: int = ...) -> AsyncIterator[_Row]: ...
     def aggregate(self, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
     async def aaggregate(self, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
     def get(self, *args: Any, **kwargs: Any) -> _Row: ...
     async def aget(self, *args: Any, **kwargs: Any) -> _Row: ...
     def create(self, **kwargs: Any) -> _T: ...
     async def acreate(self, **kwargs: Any) -> _T: ...
@@ -98,24 +96,24 @@
     async def aget_or_create(
         self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
     ) -> tuple[_T, bool]: ...
     def update_or_create(self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any) -> tuple[_T, bool]: ...
     async def aupdate_or_create(
         self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
     ) -> tuple[_T, bool]: ...
-    def earliest(self, *fields: str | OrderBy) -> _Row: ...
-    async def aearliest(self, *fields: str | OrderBy) -> _Row: ...
-    def latest(self, *fields: str | OrderBy) -> _Row: ...
-    async def alatest(self, *fields: str | OrderBy) -> _Row: ...
+    def earliest(self, *fields: Any, field_name: Any | None = ...) -> _Row: ...
+    async def aearliest(self, *fields: Any, field_name: Any | None = ...) -> _Row: ...
+    def latest(self, *fields: Any, field_name: Any | None = ...) -> _Row: ...
+    async def alatest(self, *fields: Any, field_name: Any | None = ...) -> _Row: ...
     def first(self) -> _Row | None: ...
     async def afirst(self) -> _Row | None: ...
     def last(self) -> _Row | None: ...
     async def alast(self) -> _Row | None: ...
-    def in_bulk(self, id_list: Iterable[Any] | None = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
-    async def ain_bulk(self, id_list: Iterable[Any] | None = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
+    def in_bulk(self, id_list: Iterable[Any] = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
+    async def ain_bulk(self, id_list: Iterable[Any] = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
     def delete(self) -> tuple[int, dict[str, int]]: ...
     async def adelete(self) -> tuple[int, dict[str, int]]: ...
     def update(self, **kwargs: Any) -> int: ...
     async def aupdate(self, **kwargs: Any) -> int: ...
     def exists(self) -> bool: ...
     async def aexists(self) -> bool: ...
     def explain(self, *, format: Any | None = ..., **options: Any) -> str: ...
@@ -202,20 +200,20 @@
     def __bool__(self) -> bool: ...
     @overload
     def __getitem__(self, k: int) -> _T: ...
     @overload
     def __getitem__(self, k: str) -> Any: ...
     @overload
     def __getitem__(self, k: slice) -> RawQuerySet[_T]: ...
-    @cached_property
+    @property
     def columns(self) -> list[str]: ...
     @property
     def db(self) -> str: ...
     def iterator(self) -> Iterator[_T]: ...
-    @cached_property
+    @property
     def model_fields(self) -> dict[str, str]: ...
     def prefetch_related(self, *lookups: Any) -> RawQuerySet[_T]: ...
     def resolve_model_init_order(self) -> tuple[list[str], list[int], list[tuple[str, int]]]: ...
     def using(self, alias: str | None) -> RawQuerySet[_T]: ...
 
 _QuerySetAny: TypeAlias = _QuerySet  # noqa: PYI047
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/query_utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/query_utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/signals.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/signals.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/compiler.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/compiler.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.utils import CursorWrapper
 from django.db.models.base import Model
 from django.db.models.expressions import BaseExpression, Expression
 from django.db.models.sql.query import Query
 from django.db.models.sql.subqueries import AggregateQuery, DeleteQuery, InsertQuery, UpdateQuery
-from django.utils.functional import cached_property
 from typing_extensions import TypeAlias
 
 _ParamT: TypeAlias = str | int
 
 _ParamsT: TypeAlias = list[_ParamT]
 _AsSqlType: TypeAlias = tuple[str, _ParamsT]
 
@@ -93,23 +92,23 @@
         results: Iterable[list[Sequence[Any]]] | None = ...,
         tuple_expected: bool = ...,
         chunked_fetch: bool = ...,
         chunk_size: int = ...,
     ) -> Iterator[Sequence[Any]]: ...
     def has_results(self) -> bool: ...
     @overload
-    def execute_sql(  # type: ignore[overload-overlap]
+    def execute_sql(  # type: ignore[misc]
         self, result_type: Literal["cursor"] = ..., chunked_fetch: bool = ..., chunk_size: int = ...
     ) -> CursorWrapper: ...
     @overload
     def execute_sql(
         self, result_type: Literal["no results"] | None = ..., chunked_fetch: bool = ..., chunk_size: int = ...
     ) -> None: ...
     @overload
-    def execute_sql(  # type: ignore[overload-overlap]
+    def execute_sql(  # type: ignore[misc]
         self, result_type: Literal["single"] = ..., chunked_fetch: bool = ..., chunk_size: int = ...
     ) -> Iterable[Sequence[Any]] | None: ...
     @overload
     def execute_sql(
         self, result_type: Literal["multi"] = ..., chunked_fetch: bool = ..., chunk_size: int = ...
     ) -> Iterable[list[Sequence[Any]]] | None: ...
     def as_subquery_condition(self, alias: str, columns: list[str], compiler: SQLCompiler) -> _AsSqlType: ...
@@ -126,17 +125,17 @@
     def as_sql(self) -> list[_AsSqlType]: ...  # type: ignore[override]
     def execute_sql(  # type: ignore[override]
         self, returning_fields: Sequence[str] | None = ...
     ) -> list[tuple[Any]]: ...  # 1-tuple
 
 class SQLDeleteCompiler(SQLCompiler):
     query: DeleteQuery
-    @cached_property
+    @property
     def single_alias(self) -> bool: ...
-    @cached_property
+    @property
     def contains_self_reference_subquery(self) -> bool: ...
     def as_sql(self) -> _AsSqlType: ...  # type: ignore[override]
 
 class SQLUpdateCompiler(SQLCompiler):
     query: UpdateQuery
     def as_sql(self) -> _AsSqlType: ...  # type: ignore[override]
     def execute_sql(self, result_type: Literal["cursor", "no results"]) -> int: ...  # type: ignore[override]
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/datastructures.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/query.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/query.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from django.db.models.expressions import BaseExpression, Combinable, Expression, OrderBy
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.options import Options
 from django.db.models.query_utils import PathInfo
 from django.db.models.sql.compiler import SQLCompiler
 from django.db.models.sql.datastructures import BaseTable, Join
 from django.db.models.sql.where import WhereNode
-from django.utils.functional import cached_property
 
 JoinInfo = namedtuple("JoinInfo", ("final_field", "targets", "opts", "joins", "path", "transform_function"))
 
 class RawQuery:
     high_mark: int | None
     low_mark: int | None
     params: Any
@@ -82,15 +81,15 @@
     extra: dict[str, Any]
     annotations: dict[str, Expression]
     def __init__(self, model: type[Model] | None, where: type[WhereNode] = ..., alias_cols: bool = ...) -> None: ...
     @property
     def output_field(self) -> Field: ...
     @property
     def has_select_fields(self) -> bool: ...
-    @cached_property
+    @property
     def base_table(self) -> str: ...
     def sql_with_params(self) -> tuple[str, tuple]: ...
     def __deepcopy__(self, memo: dict[int, Any]) -> Query: ...
     def get_compiler(self, using: str | None = ..., connection: BaseDatabaseWrapper | None = ...) -> SQLCompiler: ...
     def get_meta(self) -> Options: ...
     def clone(self) -> Query: ...
     def chain(self, klass: type[Query] | None = ...) -> Query: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/subqueries.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/subqueries.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/models/sql/where.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/models/sql/where.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from collections.abc import Sequence
 from typing import Any
 
-from db.models import BooleanField
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.expressions import Expression
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 from django.db.models.sql.query import Query
 from django.utils import tree
-from django.utils.functional import cached_property
 
 AND: str
 OR: str
 
 class WhereNode(tree.Node):
     connector: str
     negated: bool
@@ -21,19 +19,17 @@
     def split_having(self, negated: bool = ...) -> tuple[WhereNode | None, WhereNode | None]: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def get_group_by_cols(self, alias: str | None = ...) -> list[Expression]: ...
     def relabel_aliases(self, change_map: dict[str | None, str]) -> None: ...
     def clone(self) -> WhereNode: ...
     def relabeled_clone(self, change_map: dict[str | None, str]) -> WhereNode: ...
     def resolve_expression(self, *args: Any, **kwargs: Any) -> WhereNode: ...
-    @cached_property
-    def output_field(self) -> BooleanField: ...
-    @cached_property
+    @property
     def contains_aggregate(self) -> bool: ...
-    @cached_property
+    @property
     def contains_over_clause(self) -> bool: ...
     @property
     def is_summary(self) -> bool: ...
 
 class NothingNode:
     contains_aggregate: bool
     def as_sql(
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/transaction.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/transaction.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/db/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/db/utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from types import TracebackType
 from typing import Any
 
 from django.apps import AppConfig
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Model
 from django.utils.connection import BaseConnectionHandler
-from django.utils.functional import cached_property
 
 DEFAULT_DB_ALIAS: str
 DJANGO_VERSION_PICKLE_KEY: str
 
 class Error(Exception): ...
 class InterfaceError(Error): ...
 class DatabaseError(Error): ...
@@ -39,15 +38,15 @@
     def ensure_defaults(self, alias: str) -> None: ...
     def prepare_test_settings(self, alias: str) -> None: ...
     def create_connection(self, alias: str) -> BaseDatabaseWrapper: ...
     def close_all(self) -> None: ...
 
 class ConnectionRouter:
     def __init__(self, routers: Iterable[Any] | None = ...) -> None: ...
-    @cached_property
+    @property
     def routers(self) -> list[Any]: ...
     def db_for_read(self, model: type[Model], **hints: Any) -> str: ...
     def db_for_write(self, model: type[Model], **hints: Any) -> str: ...
     def allow_relation(self, obj1: Model, obj2: Model, **hints: Any) -> bool: ...
     def allow_migrate(self, db: str, app_label: str, **hints: Any) -> bool: ...
     def allow_migrate_model(self, db: str, model: type[Model]) -> bool: ...
     def get_migratable_models(
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/dispatch/dispatcher.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/dispatch/dispatcher.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/boundfield.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/boundfield.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, overload
 
 from django.forms.fields import Field
 from django.forms.forms import BaseForm
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import ErrorList
 from django.forms.widgets import Widget
-from django.utils.functional import _StrOrPromise, cached_property
+from django.utils.functional import _StrOrPromise
 from django.utils.safestring import SafeString
 from typing_extensions import TypeAlias
 
 _AttrsT: TypeAlias = dict[str, str | bool]
 
 class BoundField:
     form: BaseForm
@@ -18,15 +18,15 @@
     name: str
     html_name: str
     html_initial_name: str
     html_initial_id: str
     label: _StrOrPromise
     help_text: _StrOrPromise
     def __init__(self, form: BaseForm, field: Field, name: str) -> None: ...
-    @cached_property
+    @property
     def subwidgets(self) -> list[BoundWidget]: ...
     def __bool__(self) -> bool: ...
     def __iter__(self) -> Iterator[BoundWidget]: ...
     def __len__(self) -> int: ...
     @overload
     def __getitem__(self, idx: int | str) -> BoundWidget: ...
     @overload
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/fields.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/fields.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,14 @@
         help_text: _StrOrPromise = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         show_hidden_initial: bool = ...,
         validators: Sequence[_ValidatorCallable] = ...,
         localize: bool = ...,
         disabled: bool = ...,
         label_suffix: str | None = ...,
-        assume_scheme: str | None = ...,
     ) -> None: ...
     def to_python(self, value: Any | None) -> str | None: ...
 
 class BooleanField(Field):
     def to_python(self, value: Any | None) -> bool: ...
     def validate(self, value: Any) -> None: ...
     def has_changed(self, initial: Any | None, data: Any | None) -> bool: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/forms.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/forms.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from django.core.exceptions import ValidationError
 from django.forms.boundfield import BoundField
 from django.forms.fields import Field
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import ErrorDict, ErrorList, RenderableFormMixin, _DataT, _FilesT
 from django.forms.widgets import Media, MediaDefiningClass
-from django.utils.functional import _StrOrPromise, cached_property
+from django.utils.functional import _StrOrPromise
 from django.utils.safestring import SafeString
 
 class DeclarativeFieldsMetaclass(MediaDefiningClass): ...
 
 class BaseForm(RenderableFormMixin):
     class Meta:
         fields: Sequence[str]
@@ -61,15 +61,15 @@
     def template_name(self) -> str: ...
     def non_field_errors(self) -> ErrorList: ...
     def add_error(self, field: str | None, error: ValidationError | _StrOrPromise) -> None: ...
     def has_error(self, field: str | None, code: str | None = ...) -> bool: ...
     def full_clean(self) -> None: ...
     def clean(self) -> dict[str, Any] | None: ...
     def has_changed(self) -> bool: ...
-    @cached_property
+    @property
     def changed_data(self) -> list[str]: ...
     @property
     def media(self) -> Media: ...
     def is_multipart(self) -> bool: ...
     def hidden_fields(self) -> list[BoundField]: ...
     def visible_fields(self) -> list[BoundField]: ...
     def get_initial_for_field(self, field: Field, field_name: str) -> Any: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/formsets.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/formsets.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections.abc import Iterator, Mapping, Sequence, Sized
 from typing import Any, Generic, TypeVar
 
 from django.db.models.fields import _ErrorMessagesDict
 from django.forms.forms import BaseForm, Form
 from django.forms.utils import ErrorList, RenderableFormMixin, _DataT, _FilesT
 from django.forms.widgets import Media, Widget
-from django.utils.functional import cached_property
 
 TOTAL_FORM_COUNT: str
 INITIAL_FORM_COUNT: str
 MIN_NUM_FORM_COUNT: str
 MAX_NUM_FORM_COUNT: str
 ORDERING_FIELD_NAME: str
 DELETION_FIELD_NAME: str
@@ -62,19 +61,19 @@
         form_kwargs: dict[str, Any] | None = ...,
         error_messages: Mapping[str, str] | None = ...,
     ) -> None: ...
     def __iter__(self) -> Iterator[_F]: ...
     def __getitem__(self, index: int) -> _F: ...
     def __len__(self) -> int: ...
     def __bool__(self) -> bool: ...
-    @cached_property
+    @property
     def management_form(self) -> ManagementForm: ...
     def total_form_count(self) -> int: ...
     def initial_form_count(self) -> int: ...
-    @cached_property
+    @property
     def forms(self) -> list[_F]: ...
     def get_form_kwargs(self, index: int | None) -> dict[str, Any]: ...
     @property
     def initial_forms(self) -> list[_F]: ...
     @property
     def extra_forms(self) -> list[_F]: ...
     @property
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/models.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/models.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -300,14 +300,14 @@
     def to_python(self, value: Any) -> list[Model]: ...  # type: ignore[override]
     def clean(self, value: Any) -> QuerySet[Model]: ...
     def prepare_value(self, value: Any) -> Any: ...
     def has_changed(self, initial: Collection[Any] | None, data: Collection[Any] | None) -> bool: ...  # type: ignore[override]
 
 def modelform_defines_fields(form_class: type[ModelForm]) -> bool: ...
 @overload
-def _get_foreign_key(  # type: ignore[overload-overlap]
+def _get_foreign_key(  # type: ignore[misc]
     parent_model: type[Model], model: type[Model], fk_name: str | None = ..., can_fail: Literal[True] = ...
 ) -> ForeignKey | None: ...
 @overload
 def _get_foreign_key(
     parent_model: type[Model], model: type[Model], fk_name: str | None = ..., can_fail: Literal[False] = ...
 ) -> ForeignKey: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/renderers.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/renderers.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from typing import Any
 
 from django.http import HttpRequest
 from django.template.backends.base import BaseEngine
 from django.template.backends.django import DjangoTemplates as DjangoTemplatesR
 from django.template.backends.jinja2 import Jinja2 as Jinja2R
 from django.template.base import Template
-from django.utils.functional import cached_property
 
 def get_default_renderer() -> BaseRenderer: ...
 
 class BaseRenderer:
     form_template_name: str
     formset_template_name: str
     def get_template(self, template_name: str) -> Any: ...
     def render(self, template_name: str, context: dict[str, Any], request: HttpRequest | None = ...) -> str: ...
 
 class EngineMixin:
     def get_template(self, template_name: str) -> Any: ...
-    @cached_property
+    @property
     def engine(self) -> BaseEngine: ...
 
 class DjangoTemplates(EngineMixin, BaseRenderer):
     backend: type[DjangoTemplatesR]
 
 class Jinja2(EngineMixin, BaseRenderer):
-    @cached_property
+    @property
     def backend(self) -> type[Jinja2R]: ...
 
 class Jinja2DivFormRenderer(Jinja2):
     form_template_name: str
     formset_template_name: str
 
 class TemplatesSetting(BaseRenderer):
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/forms/widgets.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/multipartparser.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/multipartparser.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/request.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/request.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.contrib.sessions.backends.base import SessionBase
 from django.contrib.sites.models import Site
 from django.core.files import uploadedfile, uploadhandler
 from django.urls import ResolverMatch
 from django.utils.datastructures import CaseInsensitiveMapping, ImmutableList, MultiValueDict
-from django.utils.functional import cached_property
 from typing_extensions import Self, TypeAlias
 
 RAISE_ERROR: object
 host_validation_re: Pattern[str]
 
 class UnreadablePostError(OSError): ...
 class RawPostDataException(Exception): ...
@@ -23,22 +22,14 @@
 
 class HttpHeaders(CaseInsensitiveMapping[str]):
     HTTP_PREFIX: str
     UNPREFIXED_HEADERS: set[str]
     def __init__(self, environ: Mapping[str, Any]) -> None: ...
     @classmethod
     def parse_header_name(cls, header: str) -> str | None: ...
-    @classmethod
-    def to_wsgi_name(cls, header: str) -> str: ...
-    @classmethod
-    def to_asgi_name(cls, header: str) -> str: ...
-    @classmethod
-    def to_wsgi_names(cls, headers: Mapping[str, Any]) -> dict[str, Any]: ...
-    @classmethod
-    def to_asgi_names(cls, headers: Mapping[str, Any]) -> dict[str, Any]: ...
 
 class HttpRequest(BytesIO):
     GET: _ImmutableQueryDict
     POST: _ImmutableQueryDict
     COOKIES: dict[str, str]
     META: dict[str, Any]
     FILES: MultiValueDict[str, uploadedfile.UploadedFile]
@@ -87,20 +78,20 @@
     def encoding(self) -> str | None: ...
     @encoding.setter
     def encoding(self, val: str) -> None: ...
     @property
     def upload_handlers(self) -> UploadHandlerList: ...
     @upload_handlers.setter
     def upload_handlers(self, upload_handlers: UploadHandlerList) -> None: ...
-    @cached_property
+    @property
     def accepted_types(self) -> list[MediaType]: ...
     def parse_file_upload(
         self, META: Mapping[str, Any], post_data: BinaryIO
     ) -> tuple[QueryDict, MultiValueDict[str, uploadedfile.UploadedFile]]: ...
-    @cached_property
+    @property
     def headers(self) -> HttpHeaders: ...
     @property
     def body(self) -> bytes: ...
     def _load_post_and_files(self) -> None: ...
     def accepts(self, media_type: str) -> bool: ...
 
 class _MutableHttpRequest(HttpRequest):
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/http/response.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/http/response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from collections.abc import AsyncIterable, AsyncIterator, Iterable, Iterator
-from http.cookies import SimpleCookie
 from io import BytesIO
 from json import JSONEncoder
 from typing import Any, Literal, TypeVar, overload, type_check_only
 
+from django.http.cookie import SimpleCookie
 from django.utils.datastructures import CaseInsensitiveMapping, _PropertyDescriptor
 
 class BadHeaderError(ValueError): ...
 
 _Z = TypeVar("_Z")
 
 class ResponseHeaders(CaseInsensitiveMapping[str]):
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/cache.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/cache.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/common.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/common.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/csrf.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/csrf.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/middleware/security.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/shortcuts.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/shortcuts.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/base.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from collections.abc import Iterator, Mapping
 from typing import Any, Protocol
 
 from django.http.request import HttpRequest
 from django.template.base import Context
-from django.utils.functional import cached_property
 from django.utils.safestring import SafeString
 
 class BaseEngine:
     name: str
     dirs: list[str]
     app_dirs: bool
     def __init__(self, params: Mapping[str, Any]) -> None: ...
     @property
     def app_dirname(self) -> str | None: ...
     def from_string(self, template_code: str) -> _EngineTemplate: ...
     def get_template(self, template_name: str) -> _EngineTemplate: ...
-    @cached_property
+    @property
     def template_dirs(self) -> tuple[str]: ...
     def iter_template_filenames(self, template_name: str) -> Iterator[str]: ...
 
 class _EngineTemplate(Protocol):
     def render(
         self,
         context: Context | dict[str, Any] | None = ...,
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/django.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/django.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/backends/jinja2.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/backends/jinja2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from collections.abc import Callable
 from typing import Any
 
 from _typeshed import Incomplete
 from django.template.exceptions import TemplateSyntaxError
-from django.utils.functional import cached_property
 
 from .base import BaseEngine
 
 class Jinja2(BaseEngine):
     env: Any
     context_processors: list[str]
     def __init__(self, params: dict[str, Any]) -> None: ...
-    @cached_property
+    @property
     def template_context_processors(self) -> list[Callable]: ...
 
 class Origin:
     name: str
     template_name: str | None
     def __init__(self, name: str, template_name: str | None) -> None: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/context.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/context.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/context_processors.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/defaultfilters.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/defaultfilters.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/defaulttags.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/defaulttags.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/engine.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/engine.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections.abc import Callable, Sequence
 from typing import Any
 
 from django.template.base import Origin
 from django.template.library import Library
 from django.template.loaders.base import Loader
-from django.utils.functional import cached_property
 from django.utils.safestring import SafeString
 from typing_extensions import TypeAlias
 
 from .base import Template
 
 _Loader: TypeAlias = Any
 
@@ -37,19 +36,19 @@
         file_charset: str = ...,
         libraries: dict[str, str] | None = ...,
         builtins: list[str] | None = ...,
         autoescape: bool = ...,
     ) -> None: ...
     @staticmethod
     def get_default() -> Engine: ...
-    @cached_property
+    @property
     def template_context_processors(self) -> Sequence[Callable]: ...
     def get_template_builtins(self, builtins: list[str]) -> list[Library]: ...
     def get_template_libraries(self, libraries: dict[str, str]) -> dict[str, Library]: ...
-    @cached_property
+    @property
     def template_loaders(self) -> list[Loader]: ...
     def get_template_loaders(self, template_loaders: Sequence[_Loader]) -> list[Loader]: ...
     def find_template_loader(self, loader: _Loader) -> Loader: ...
     def find_template(
         self, name: str, dirs: None = ..., skip: list[Origin] | None = ...
     ) -> tuple[Template, Origin]: ...
     def from_string(self, template_code: str) -> Template: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/library.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/library.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loader.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loader.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loader_tags.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loader_tags.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/cached.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/cached.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/loaders/filesystem.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/loaders/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/response.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 _TemplateForResponseT: TypeAlias = _ListOrTuple[str] | Template | str
 
 class ContentNotRenderedError(Exception): ...
 
 class SimpleTemplateResponse(HttpResponse):
     content: Any
     closed: bool
-    cookies: SimpleCookie
+    cookies: SimpleCookie[str]
     status_code: int
     rendering_attrs: Any
     template_name: _TemplateForResponseT
     context_data: dict[str, Any] | None
     using: str | None
     def __init__(
         self,
@@ -46,15 +46,15 @@
     def __iter__(self) -> Iterator[Any]: ...
 
 class TemplateResponse(SimpleTemplateResponse):
     client: Client
     closed: bool
     context: RequestContext
     context_data: dict[str, Any] | None
-    cookies: SimpleCookie
+    cookies: SimpleCookie[str]
     csrf_cookie_set: bool
     json: functools.partial
     _request: HttpRequest
     status_code: int
     template_name: _TemplateForResponseT
     templates: list[Template]
     using: str | None
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/template/smartif.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/template/smartif.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/cache.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/cache.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/i18n.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/i18n.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/static.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/static.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/templatetags/tz.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/templatetags/tz.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/client.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections.abc import Awaitable, Callable, Iterable, Iterator, Mapping
-from http.cookies import SimpleCookie
 from io import BytesIO, IOBase
 from json import JSONEncoder
 from re import Pattern
 from types import TracebackType
 from typing import Any, Generic, NoReturn, TypeVar
 
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.sessions.backends.base import SessionBase
 from django.core.handlers.asgi import ASGIRequest
 from django.core.handlers.base import BaseHandler
 from django.core.handlers.wsgi import WSGIRequest
+from django.http.cookie import SimpleCookie
 from django.http.request import HttpRequest
 from django.http.response import HttpResponseBase
 from django.template.base import Template
 from django.test.utils import ContextList
 from django.urls import ResolverMatch
 from typing_extensions import TypeAlias
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/html.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/html.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/runner.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/runner.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/selenium.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/selenium.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/signals.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/signals.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/testcases.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/testcases.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -214,20 +214,20 @@
         ordered: bool = ...,
         msg: str | None = ...,
     ) -> None: ...
     def assertQuerySetEqual(
         self,
         qs: Iterator[Any] | list[Model] | QuerySet | RawQuerySet,
         values: Collection[Any],
-        transform: Callable[[Model], Any] | type[str] | None = ...,
+        transform: Callable[[Model], Any] | type[str] = ...,
         ordered: bool = ...,
         msg: str | None = ...,
     ) -> None: ...
     @overload
-    def assertNumQueries(self, num: int, func: None = ..., *, using: str = ...) -> _AssertNumQueriesContext: ...
+    def assertNumQueries(self, num: int, using: str = ...) -> _AssertNumQueriesContext: ...  # type: ignore[misc]
     @overload
     def assertNumQueries(
         self, num: int, func: Callable[..., Any], *args: Any, using: str = ..., **kwargs: Any
     ) -> None: ...
 
 class TestCase(TransactionTestCase):
     @classmethod
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/test/utils.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/test/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/conf.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/conf.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/converters.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/converters.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/urls/resolvers.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/urls/resolvers.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/archive.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/archive.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/autoreload.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/autoreload.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/baseconv.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/baseconv.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/cache.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/cache.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/connection.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/connection.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/crypto.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/crypto.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/datastructures.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/dateformat.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/dateformat.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/datetime_safe.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/datetime_safe.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/decorators.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/decorators.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/deprecation.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/deprecation.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/encoding.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/encoding.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 @overload
 def force_bytes(s: Any, encoding: str = ..., strings_only: bool = ..., errors: str = ...) -> bytes: ...
 @overload
 def iri_to_uri(iri: None) -> None: ...
 @overload
 def iri_to_uri(iri: str | Promise) -> str: ...
 @overload
-def uri_to_iri(uri: None) -> None: ...  # type: ignore[overload-overlap]
+def uri_to_iri(uri: None) -> None: ...  # type: ignore[misc]
 @overload
 def uri_to_iri(uri: Any) -> str: ...
 def escape_uri_path(path: str) -> str: ...
 def punycode(domain: str) -> str: ...
 def repercent_broken_unicode(path: bytes) -> bytes: ...
 @overload
 def filepath_to_uri(path: None) -> None: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/feedgenerator.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/feedgenerator.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/formats.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/formats.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 
 _T = TypeVar("_T")
 
 # Mypy considers this invalid (overlapping signatures), but thanks to implementation
 # details it works as expected (all values from Union are `localize`d to str,
 # while type of others is preserved)
 @overload
-def localize(  # type: ignore[overload-overlap]
+def localize(  # type: ignore[misc]
     value: builtin_datetime | date | time | Decimal | float | str, use_l10n: bool | None = ...
 ) -> str: ...
 @overload
 def localize(value: _T, use_l10n: bool | None = ...) -> _T: ...
 @overload
-def localize_input(  # type: ignore[overload-overlap]
+def localize_input(  # type: ignore[misc]
     value: builtin_datetime | date | time | Decimal | float | str, default: str | None = ...
 ) -> str: ...
 @overload
 def localize_input(value: _T, default: str | None = ...) -> _T: ...
 def sanitize_separators(value: _T) -> _T: ...
 def sanitize_strftime_format(fmt: str) -> str: ...
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/functional.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/functional.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/html.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/html.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/http.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/http.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/jslex.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/jslex.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/log.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/log.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/regex_helper.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/regex_helper.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/safestring.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/safestring.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/termcolors.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/termcolors.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/text.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/text.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from re import Pattern
 from typing import ClassVar, TypeVar, overload
 
 from django.db.models.base import Model
 from django.utils.functional import SimpleLazyObject, _StrOrPromise
 
 _StrOrPromiseT = TypeVar("_StrOrPromiseT", bound=_StrOrPromise)
-_StrOrPromiseOrNoneT = TypeVar("_StrOrPromiseOrNoneT", bound=_StrOrPromise | None)
 
-def capfirst(x: _StrOrPromiseOrNoneT) -> _StrOrPromiseOrNoneT: ...
+def capfirst(x: _StrOrPromiseT | None) -> _StrOrPromiseT | None: ...
 
 re_words: Pattern[str]
 re_chars: Pattern[str]
 re_tag: Pattern[str]
 re_newlines: Pattern[str]
 re_camel_case: Pattern[str]
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/timezone.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/timezone.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from pytz import BaseTzInfo
 from typing_extensions import TypeAlias, TypeGuard
 
 _PytzTzInfoT: TypeAlias = pytz.tzinfo.BaseTzInfo | pytz._FixedOffset
 
 _TzInfoT: TypeAlias = _PytzTzInfoT | tzinfo
 
+utc: Any
+
 def get_fixed_timezone(offset: timedelta | int) -> timezone: ...
 def get_default_timezone() -> BaseTzInfo: ...
 def get_default_timezone_name() -> str: ...
 
 # Strictly speaking, it is possible to activate() a non-pytz timezone,
 # in which case BaseTzInfo is incorrect. However, this is unlikely,
 # so we use it anyway, to keep things ergonomic for most users.
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/trans_null.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/trans_null.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/translation/trans_real.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/translation/trans_real.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/tree.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/tree.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/utils/version.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/utils/version.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/decorators/http.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/decorators/http.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/defaults.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/defaults.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/__init__.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/base.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/dates.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/dates.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/detail.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/detail.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/edit.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/edit.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/generic/list.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/generic/list.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/django-stubs/views/i18n.pyi` & `sentry_forked_django_stubs-5.0.0.post1/django-stubs/views/i18n.pyi`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/config.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/config.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/django/context.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/django/context.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/lib/fullnames.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/lib/fullnames.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 MANYTOMANY_FIELD_FULLNAME = "django.db.models.fields.related.ManyToManyField"
 DUMMY_SETTINGS_BASE_CLASS = "django.conf._DjangoConfLazyObject"
 AUTH_USER_MODEL_FULLNAME = "django.conf.settings.AUTH_USER_MODEL"
 
 QUERYSET_CLASS_FULLNAME = "django.db.models.query._QuerySet"
 BASE_MANAGER_CLASS_FULLNAME = "django.db.models.manager.BaseManager"
 MANAGER_CLASS_FULLNAME = "django.db.models.manager.Manager"
-RELATED_MANAGER_CLASS = "django.db.models.fields.related_descriptors.RelatedManager"
+RELATED_MANAGER_CLASS = "django.db.models.manager.RelatedManager"
 
 WITH_ANNOTATIONS_FULLNAME = "django_stubs_ext.WithAnnotations"
 ANNOTATIONS_FULLNAME = "django_stubs_ext.annotations.Annotations"
 
 BASEFORM_CLASS_FULLNAME = "django.forms.forms.BaseForm"
 FORM_CLASS_FULLNAME = "django.forms.forms.Form"
 MODELFORM_CLASS_FULLNAME = "django.forms.models.ModelForm"
@@ -30,16 +30,14 @@
 
 MANAGER_CLASSES = {
     MANAGER_CLASS_FULLNAME,
     BASE_MANAGER_CLASS_FULLNAME,
 }
 
 REVERSE_ONE_TO_ONE_DESCRIPTOR = "django.db.models.fields.related_descriptors.ReverseOneToOneDescriptor"
-MANY_TO_MANY_DESCRIPTOR = "django.db.models.fields.related_descriptors.ManyToManyDescriptor"
-MANY_RELATED_MANAGER = "django.db.models.fields.related_descriptors.ManyRelatedManager"
 RELATED_FIELDS_CLASSES = frozenset(
     (
         FOREIGN_OBJECT_FULLNAME,
         FOREIGN_KEY_FULLNAME,
         ONETOONE_FIELD_FULLNAME,
     )
 )
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/lib/helpers.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/lib/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,28 +63,14 @@
 
 def get_django_metadata_bases(
     model_info: TypeInfo, key: Literal["baseform_bases", "manager_bases", "queryset_bases"]
 ) -> Dict[str, int]:
     return get_django_metadata(model_info).setdefault(key, cast(Dict[str, int], {}))
 
 
-def get_reverse_manager_info(
-    api: Union[TypeChecker, SemanticAnalyzer], model_info: TypeInfo, derived_from: str
-) -> Optional[TypeInfo]:
-    manager_fullname = get_django_metadata(model_info).get("reverse_managers", {}).get(derived_from)
-    if not manager_fullname:
-        return None
-
-    return lookup_fully_qualified_typeinfo(api, manager_fullname)
-
-
-def set_reverse_manager_info(model_info: TypeInfo, derived_from: str, fullname: str) -> None:
-    get_django_metadata(model_info).setdefault("reverse_managers", {})[derived_from] = fullname
-
-
 class IncompleteDefnException(Exception):
     pass
 
 
 def lookup_fully_qualified_sym(fullname: str, all_modules: Dict[str, MypyFile]) -> Optional[SymbolTableNode]:
     if "." not in fullname:
         return None
@@ -412,15 +398,15 @@
     sym = api.lookup_fully_qualified_or_none(fullnames.MANAGER_CLASS_FULLNAME)
     if sym is not None and isinstance(sym.node, TypeInfo):
         bases = get_django_metadata_bases(sym.node, "manager_bases")
         bases[fullname] = 1
 
 
 def is_abstract_model(model: TypeInfo) -> bool:
-    if not is_model_type(model):
+    if model.metaclass_type is None or model.metaclass_type.type.fullname != fullnames.MODEL_METACLASS_FULLNAME:
         return False
 
     metadata = get_django_metadata(model)
     if metadata.get("is_abstract_model") is not None:
         return metadata["is_abstract_model"]
 
     meta = model.names.get("Meta")
@@ -467,11 +453,7 @@
         elif isinstance(api, SemanticAnalyzer) and not api.final_iteration:
             # Getting this far, where Django matched the reference but we still can't
             # find it, we want to defer
             api.defer()
     else:
         api.fail("Could not match lazy reference with any model", ctx)
     return None
-
-
-def is_model_type(info: TypeInfo) -> bool:
-    return info.metaclass_type is not None and info.metaclass_type.type.fullname == fullnames.MODEL_METACLASS_FULLNAME
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/main.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from mypy.types import Type as MypyType
 
 import mypy_django_plugin.transformers.orm_lookups
 from mypy_django_plugin.config import DjangoPluginConfig
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.exceptions import UnregisteredModelError
 from mypy_django_plugin.lib import fullnames, helpers
-from mypy_django_plugin.transformers import fields, forms, init_create, manytomany, meta, querysets, request, settings
+from mypy_django_plugin.transformers import fields, forms, init_create, meta, querysets, request, settings
 from mypy_django_plugin.transformers.functional import resolve_str_promise_attribute
 from mypy_django_plugin.transformers.managers import (
     create_new_manager_class_from_as_manager_method,
     create_new_manager_class_from_from_queryset_method,
     reparametrize_any_manager_hook,
     resolve_manager_method,
 )
@@ -184,20 +184,14 @@
                 return forms.extract_proper_type_for_get_form_class
 
         elif method_name == "get_form":
             info = self._get_typeinfo_or_none(class_fullname)
             if info and info.has_base(fullnames.FORM_MIXIN_CLASS_FULLNAME):
                 return forms.extract_proper_type_for_get_form
 
-        elif method_name == "__get__" and class_fullname in {
-            fullnames.MANYTOMANY_FIELD_FULLNAME,
-            fullnames.MANY_TO_MANY_DESCRIPTOR,
-        }:
-            return manytomany.refine_many_to_many_related_manager
-
         manager_classes = self._get_current_manager_bases()
 
         if method_name == "values":
             info = self._get_typeinfo_or_none(class_fullname)
             if info and info.has_base(fullnames.QUERYSET_CLASS_FULLNAME) or class_fullname in manager_classes:
                 return partial(querysets.extract_proper_type_queryset_values, django_context=self.django_context)
 
@@ -226,30 +220,35 @@
                 django_context=self.django_context,
             )
 
         return None
 
     def get_customize_class_mro_hook(self, fullname: str) -> Optional[Callable[[ClassDefContext], None]]:
         if fullname == fullnames.MODEL_CLASS_FULLNAME:
-            return None
+            return MetaclassAdjustments.adjust_model_class
 
         sym = self.lookup_fully_qualified(fullname)
         if (
             sym is not None
             and isinstance(sym.node, TypeInfo)
             and sym.node.has_base(fullnames.BASE_MANAGER_CLASS_FULLNAME)
         ):
             return reparametrize_any_manager_hook
         else:
             return None
 
     def get_base_class_hook(self, fullname: str) -> Optional[Callable[[ClassDefContext], None]]:
         # Base class is a Model class definition
         sym = self.lookup_fully_qualified(fullname)
-        if sym is not None and isinstance(sym.node, TypeInfo) and helpers.is_model_type(sym.node):
+        if (
+            sym is not None
+            and isinstance(sym.node, TypeInfo)
+            and sym.node.metaclass_type is not None
+            and sym.node.metaclass_type.type.fullname == fullnames.MODEL_METACLASS_FULLNAME
+        ):
             return partial(process_model_class, django_context=self.django_context)
 
         # Base class is a Manager class definition
         if fullname in self._get_current_manager_bases():
             return add_new_manager_base_hook
 
         # Base class is a Form class definition
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/fields.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/fields.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/forms.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/forms.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/functional.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/functional.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/init_create.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/init_create.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/managers.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,29 +105,27 @@
     base_that_has_method: TypeInfo,
     manager_instance: Instance,
     is_fallback_queryset: bool,
 ) -> CallableType:
     variables = method_type.variables
     ret_type = method_type.ret_type
 
-    if not is_fallback_queryset:
-        queryset_instance = Instance(queryset_info, manager_instance.args)
-    else:
-        # The fallback queryset inherits _QuerySet, which has two generics
-        # instead of the one exposed on QuerySet. That means that we need
-        # to add the model twice. In real code it's not possible to inherit
-        # from _QuerySet, as it doesn't exist at runtime, so this fix is
-        # only needed for plugin-generated querysets.
-        queryset_instance = Instance(queryset_info, [manager_instance.args[0], manager_instance.args[0]])
-
     # For methods on the manager that return a queryset we need to override the
     # return type to be the actual queryset class, not the base QuerySet that's
     # used by the typing stubs.
     if method_name in MANAGER_METHODS_RETURNING_QUERYSET:
-        ret_type = queryset_instance
+        if not is_fallback_queryset:
+            ret_type = Instance(queryset_info, manager_instance.args)
+        else:
+            # The fallback queryset inherits _QuerySet, which has two generics
+            # instead of the one exposed on QuerySet. That means that we need
+            # to add the model twice. In real code it's not possible to inherit
+            # from _QuerySet, as it doesn't exist at runtime, so this fix is
+            # only needed for pluign-generated querysets.
+            ret_type = Instance(queryset_info, [manager_instance.args[0], manager_instance.args[0]])
         variables = []
     args_types = method_type.arg_types[1:]
     if _has_compatible_type_vars(base_that_has_method):
         typed_var = manager_instance.args or queryset_info.bases[0].args
         if (
             typed_var
             and isinstance(typed_var[0], Instance)
@@ -136,15 +134,15 @@
             ret_type = _replace_type_var(ret_type, base_that_has_method.defn.type_vars[0].fullname, typed_var[0])
             args_types = [
                 _replace_type_var(arg_type, base_that_has_method.defn.type_vars[0].fullname, manager_instance.args[0])
                 for arg_type in args_types
             ]
     if base_that_has_method.self_type:
         # Manages -> Self returns
-        ret_type = _replace_type_var(ret_type, base_that_has_method.self_type.fullname, queryset_instance)
+        ret_type = _replace_type_var(ret_type, base_that_has_method.self_type.fullname, manager_instance)
 
     # Drop any 'self' argument as our manager is already initialized
     return method_type.copy_modified(
         arg_types=args_types,
         arg_kinds=method_type.arg_kinds[1:],
         arg_names=method_type.arg_names[1:],
         variables=variables,
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/manytomany.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/manytomany.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import NamedTuple, Optional, Tuple, Union
+from typing import NamedTuple, Optional, Union
 
 from mypy.checker import TypeChecker
 from mypy.nodes import AssignmentStmt, Expression, MemberExpr, NameExpr, StrExpr, TypeInfo
-from mypy.plugin import FunctionContext, MethodContext
+from mypy.plugin import FunctionContext
 from mypy.semanal import SemanticAnalyzer
 from mypy.types import Instance, ProperType, UninhabitedType
 from mypy.types import Type as MypyType
 
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.lib import fullnames, helpers
 
@@ -126,15 +126,18 @@
     django_context: DjangoContext,
 ) -> Optional[ProperType]:
     """
     Attempts to resolve an expression to a 'TypeInfo' instance. Any lazy reference
     argument(e.g. "<app_label>.<object_name>") to a Django model is also attempted.
     """
     if isinstance(expr, NameExpr) and isinstance(expr.node, TypeInfo):
-        if helpers.is_model_type(expr.node):
+        if (
+            expr.node.metaclass_type is not None
+            and expr.node.metaclass_type.type.fullname == fullnames.MODEL_METACLASS_FULLNAME
+        ):
             return Instance(expr.node, [])
 
     lazy_reference = None
     if isinstance(expr, StrExpr):
         lazy_reference = expr.value
     elif (
         isinstance(expr, MemberExpr)
@@ -144,61 +147,7 @@
         lazy_reference = django_context.settings.AUTH_USER_MODEL
 
     if lazy_reference is not None:
         model_info = helpers.resolve_lazy_reference(lazy_reference, api=api, django_context=django_context, ctx=expr)
         if model_info is not None:
             return Instance(model_info, [])
     return None
-
-
-def get_related_manager_and_model(ctx: MethodContext) -> Optional[Tuple[Instance, Instance]]:
-    if (
-        isinstance(ctx.default_return_type, Instance)
-        and ctx.default_return_type.type.fullname == fullnames.MANY_RELATED_MANAGER
-    ):
-        # This is a call to '__get__' overload with a model instance of 'ManyToManyDescriptor'.
-        # Returning a 'ManyRelatedManager'. Which we want to, just like Django, build from the
-        # default manager of the related model.
-        many_related_manager = ctx.default_return_type
-        # Require first type argument of 'ManyRelatedManager' to be a model
-        if (
-            many_related_manager.args
-            and isinstance(many_related_manager.args[0], Instance)
-            and helpers.is_model_type(many_related_manager.args[0].type)
-        ):
-            return many_related_manager, many_related_manager.args[0]
-
-    return None
-
-
-def refine_many_to_many_related_manager(ctx: MethodContext) -> MypyType:
-    """
-    Updates the 'ManyRelatedManager' returned by e.g. 'ManyToManyDescriptor' to be a subclass
-    of 'ManyRelatedManager' and the related model's default manager.
-    """
-    related_objects = get_related_manager_and_model(ctx)
-    if related_objects is None:
-        return ctx.default_return_type
-
-    many_related_manager, related_model_instance = related_objects
-    checker = helpers.get_typechecker_api(ctx)
-    related_model_instance = related_model_instance.copy_modified()
-    related_manager_info = helpers.get_reverse_manager_info(
-        checker, related_model_instance.type, derived_from="_default_manager"
-    )
-    if related_manager_info is None:
-        default_manager_node = related_model_instance.type.names.get("_default_manager")
-        if default_manager_node is None or not isinstance(default_manager_node.type, Instance):
-            return ctx.default_return_type
-
-        related_manager_info = helpers.add_new_class_for_module(
-            module=checker.modules[related_model_instance.type.module_name],
-            name=f"{related_model_instance.type.name}_ManyRelatedManager",
-            bases=[many_related_manager, default_manager_node.type],
-        )
-        related_manager_info.metadata["django"] = {"related_manager_to_model": related_model_instance.type.fullname}
-        helpers.set_reverse_manager_info(
-            related_model_instance.type,
-            derived_from="_default_manager",
-            fullname=related_manager_info.fullname,
-        )
-    return Instance(related_manager_info, [])
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/meta.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/meta.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/models.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import cached_property
 from typing import Any, Dict, List, Optional, Type, Union, cast
 
 from django.db.models import Manager, Model
 from django.db.models.fields import DateField, DateTimeField, Field
-from django.db.models.fields.reverse_related import ManyToManyRel, OneToOneRel
+from django.db.models.fields.reverse_related import ForeignObjectRel, OneToOneRel
 from mypy.checker import TypeChecker
 from mypy.nodes import (
     ARG_STAR2,
     MDEF,
     Argument,
     AssignmentStmt,
     CallExpr,
@@ -444,23 +444,31 @@
             default_manager_info = generated_manager_info
 
         default_manager = Instance(default_manager_info, [Instance(self.model_classdef.info, [])])
         self.add_new_node_to_model_class("_default_manager", default_manager, is_classvar=True)
 
 
 class AddReverseLookups(ModelClassInitializer):
-    @cached_property
-    def reverse_one_to_one_descriptor(self) -> TypeInfo:
-        return self.lookup_typeinfo_or_incomplete_defn_error(fullnames.REVERSE_ONE_TO_ONE_DESCRIPTOR)
+    def get_reverse_manager_info(self, model_info: TypeInfo, derived_from: str) -> Optional[TypeInfo]:
+        manager_fullname = helpers.get_django_metadata(model_info).get("reverse_managers", {}).get(derived_from)
+        if not manager_fullname:
+            return None
 
-    @cached_property
-    def many_to_many_descriptor(self) -> TypeInfo:
-        return self.lookup_typeinfo_or_incomplete_defn_error(fullnames.MANY_TO_MANY_DESCRIPTOR)
+        symbol = self.api.lookup_fully_qualified_or_none(manager_fullname)
+        if symbol is None or not isinstance(symbol.node, TypeInfo):
+            return None
+        return symbol.node
+
+    def set_reverse_manager_info(self, model_info: TypeInfo, derived_from: str, fullname: str) -> None:
+        helpers.get_django_metadata(model_info).setdefault("reverse_managers", {})[derived_from] = fullname
 
     def run_with_model_cls(self, model_cls: Type[Model]) -> None:
+        reverse_one_to_one_descriptor = self.lookup_typeinfo_or_incomplete_defn_error(
+            fullnames.REVERSE_ONE_TO_ONE_DESCRIPTOR
+        )
         # add related managers
         for relation in self.django_context.get_model_relations(model_cls):
             attname = relation.get_accessor_name()
             if attname is None or attname in self.model_classdef.info.names:
                 # No reverse accessor or already declared. Note that this would also leave any
                 # explicitly declared(i.e. non-inferred) reverse accessors alone
                 continue
@@ -475,35 +483,21 @@
                 else:
                     continue
 
             if isinstance(relation, OneToOneRel):
                 self.add_new_node_to_model_class(
                     attname,
                     Instance(
-                        self.reverse_one_to_one_descriptor,
+                        reverse_one_to_one_descriptor,
                         [Instance(self.model_classdef.info, []), Instance(related_model_info, [])],
                     ),
                 )
                 continue
 
-            elif isinstance(relation, ManyToManyRel):
-                # TODO: 'relation' should be based on `TypeInfo` instead of Django runtime.
-                to_fullname = helpers.get_class_fullname(relation.remote_field.model)
-                to_model_info = self.lookup_typeinfo_or_incomplete_defn_error(to_fullname)
-                assert relation.through is not None
-                through_fullname = helpers.get_class_fullname(relation.through)
-                through_model_info = self.lookup_typeinfo_or_incomplete_defn_error(through_fullname)
-                self.add_new_node_to_model_class(
-                    attname,
-                    Instance(
-                        self.many_to_many_descriptor, [Instance(to_model_info, []), Instance(through_model_info, [])]
-                    ),
-                )
-
-            else:
+            if isinstance(relation, ForeignObjectRel):
                 related_manager_info = None
                 try:
                     related_manager_info = self.lookup_typeinfo_or_incomplete_defn_error(
                         fullnames.RELATED_MANAGER_CLASS
                     )
                     default_manager = related_model_info.names.get("_default_manager")
                     if not default_manager:
@@ -536,16 +530,16 @@
                         code=MANAGER_MISSING,
                     )
 
                     continue
 
                 # Check if the related model has a related manager subclassed from the default manager
                 # TODO: Support other reverse managers than `_default_manager`
-                default_reverse_manager_info = helpers.get_reverse_manager_info(
-                    self.api, model_info=related_model_info, derived_from="_default_manager"
+                default_reverse_manager_info = self.get_reverse_manager_info(
+                    model_info=related_model_info, derived_from="_default_manager"
                 )
                 if default_reverse_manager_info:
                     self.add_new_node_to_model_class(attname, Instance(default_reverse_manager_info, []))
                     continue
 
                 # The reverse manager we're looking for doesn't exist. So we
                 # create it. The (default) reverse manager type is built from a
@@ -566,15 +560,15 @@
                     module=self.api.modules[related_model_info.module_name],
                     name=f"{related_model_cls.__name__}_RelatedManager",
                     bases=[parametrized_related_manager_type, default_manager_type],
                 )
                 new_related_manager_info.metadata["django"] = {"related_manager_to_model": related_model_info.fullname}
                 # Stash the new reverse manager type fullname on the related model, so we don't duplicate
                 # or have to create it again for other reverse relations
-                helpers.set_reverse_manager_info(
+                self.set_reverse_manager_info(
                     related_model_info,
                     derived_from="_default_manager",
                     fullname=new_related_manager_info.fullname,
                 )
                 self.add_new_node_to_model_class(attname, Instance(new_related_manager_info, []))
 
 
@@ -846,15 +840,16 @@
 
     def get_exception_bases(self, name: str) -> List[Instance]:
         bases = []
         for model_base in self.model_classdef.info.direct_base_classes():
             exception_base_sym = model_base.names.get(name)
             if (
                 # Base class is a Model
-                helpers.is_model_type(model_base)
+                model_base.metaclass_type is not None
+                and model_base.metaclass_type.type.fullname == fullnames.MODEL_METACLASS_FULLNAME
                 # But base class is not 'models.Model'
                 and model_base.fullname != fullnames.MODEL_CLASS_FULLNAME
                 # Base class also has a generated exception base e.g. 'DoesNotExist'
                 and exception_base_sym is not None
                 and exception_base_sym.plugin_generated
                 and isinstance(exception_base_sym.node, TypeInfo)
             ):
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/orm_lookups.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/orm_lookups.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 def typecheck_queryset_filter(ctx: MethodContext, django_context: DjangoContext) -> MypyType:
     # Expected formal arguments for filter methods are `*args` and `**kwargs`. We'll only typecheck
     # `**kwargs`, which means that `arg_names[1]` is what we're interested in.
 
     lookup_kwargs = ctx.arg_names[1] if len(ctx.arg_names) >= 2 else []
     provided_lookup_types = ctx.arg_types[1] if len(ctx.arg_types) >= 2 else []
 
-    if not isinstance(ctx.type, Instance) or not ctx.type.args or not isinstance(ctx.type.args[0], Instance):
+    assert isinstance(ctx.type, Instance)
+
+    if not ctx.type.args or not isinstance(ctx.type.args[0], Instance):
         return ctx.default_return_type
 
     model_cls_fullname = ctx.type.args[0].type.fullname
     model_cls = django_context.get_model_class_by_fullname(model_cls_fullname)
     if model_cls is None:
         return ctx.default_return_type
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/querysets.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/querysets.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/request.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/request.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/mypy_django_plugin/transformers/settings.py` & `sentry_forked_django_stubs-5.0.0.post1/mypy_django_plugin/transformers/settings.py`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/pyproject.toml` & `sentry_forked_django_stubs-5.0.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sentry-forked-django-stubs-4.2.7.post3/sentry_forked_django_stubs.egg-info/PKG-INFO` & `sentry_forked_django_stubs-5.0.0.post1/sentry_forked_django_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-forked-django-stubs
-Version: 4.2.7.post3
+Version: 5.0.0.post1
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -21,21 +21,21 @@
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
-Requires-Dist: django-stubs-ext>=4.2.7
+Requires-Dist: django-stubs-ext>=4.2.5
 Requires-Dist: tomli; python_version < "3.11"
 Requires-Dist: typing-extensions
 Requires-Dist: types-pytz
 Requires-Dist: types-PyYAML
 Provides-Extra: compatible-mypy
-Requires-Dist: mypy~=1.7.0; extra == "compatible-mypy"
+Requires-Dist: mypy~=1.6.0; extra == "compatible-mypy"
 
 sentry-forked-django-stubs
 ==========================
 
 ### new release
 
 make a new branch for the fork of an upstream tag:
@@ -47,15 +47,15 @@
 git checkout 1.2.3 -b sentry-1.2.3
 ```
 
 - cherry-pick the craft / release commit(s) into your branch from `master`
 - cherry-pick relevant commit(s) from previous releases
 
 releases are done through craft in the release.yml workflow -- make sure to
-target your particular branch with a `.#` release postfix (like `1.2.3.0`)
+target your particular branch with a `-#` release postfix (like `1.2.3-1`)
 
 ___
 
 <img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
@@ -102,15 +102,14 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
-| 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/sentry_forked_django_stubs.egg-info/SOURCES.txt` & `sentry_forked_django_stubs-5.0.0.post1/sentry_forked_django_stubs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,14 @@
 django-stubs/contrib/messages/storage/base.pyi
 django-stubs/contrib/messages/storage/cookie.pyi
 django-stubs/contrib/messages/storage/fallback.pyi
 django-stubs/contrib/messages/storage/session.pyi
 django-stubs/contrib/postgres/__init__.pyi
 django-stubs/contrib/postgres/apps.pyi
 django-stubs/contrib/postgres/constraints.pyi
-django-stubs/contrib/postgres/expressions.pyi
 django-stubs/contrib/postgres/functions.pyi
 django-stubs/contrib/postgres/indexes.pyi
 django-stubs/contrib/postgres/lookups.pyi
 django-stubs/contrib/postgres/operations.pyi
 django-stubs/contrib/postgres/search.pyi
 django-stubs/contrib/postgres/serializers.pyi
 django-stubs/contrib/postgres/signals.pyi
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/setup.py` & `sentry_forked_django_stubs-5.0.0.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
     "django",
-    "django-stubs-ext>=4.2.7",
+    "django-stubs-ext>=4.2.5",
     "tomli; python_version < '3.11'",
     # Types:
     "typing-extensions",
     "types-pytz",
     "types-PyYAML",
 ]
 
 # Keep compatible-mypy major.minor version pinned to what we use in CI (requirements.txt)
 extras_require = {
-    "compatible-mypy": ["mypy~=1.7.0"],
+    "compatible-mypy": ["mypy~=1.6.0"],
 }
 
 setup(
     name="sentry-forked-django-stubs",
-    version="4.2.7-3",
+    version="5.0.0-1",
     description="Mypy stubs for Django",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Maksim Kurnikov",
```

### Comparing `sentry-forked-django-stubs-4.2.7.post3/tests/test_error_handling.py` & `sentry_forked_django_stubs-5.0.0.post1/tests/test_error_handling.py`

 * *Files identical despite different names*

