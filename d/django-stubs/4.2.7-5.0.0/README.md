# Comparing `tmp/django-stubs-4.2.7.tar.gz` & `tmp/django_stubs-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stubs-4.2.7.tar", last modified: Tue Dec  5 19:02:17 2023, max compression
+gzip compressed data, was "django_stubs-5.0.0.tar", last modified: Tue Apr 30 10:03:06 2024, max compression
```

## Comparing `django-stubs-4.2.7.tar` & `django_stubs-5.0.0.tar`

### file list

```diff
@@ -1,839 +1,834 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.278337 django-stubs-4.2.7/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-4.2.7/LICENSE.md
--rw-r--r--   0 marti     (1000) marti      (121)    16619 2023-12-05 19:02:17.278337 django-stubs-4.2.7/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)    15361 2023-12-05 19:01:16.000000 django-stubs-4.2.7/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.098339 django-stubs-4.2.7/django-stubs/
--rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.098339 django-stubs-4.2.7/django-stubs/apps/
--rw-r--r--   0 marti     (1000) marti      (121)       78 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/apps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1094 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/apps/config.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1963 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/apps/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.098339 django-stubs-4.2.7/django-stubs/conf/
--rw-r--r--   0 marti     (1000) marti      (121)     1434 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/conf/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    17261 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/conf/global_settings.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.098339 django-stubs-4.2.7/django-stubs/conf/locale/
--rw-r--r--   0 marti     (1000) marti      (121)       50 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/conf/locale/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.101672 django-stubs-4.2.7/django-stubs/conf/urls/
--rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/conf/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      231 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/conf/urls/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/conf/urls/static.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.101672 django-stubs-4.2.7/django-stubs/contrib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.105006 django-stubs-4.2.7/django-stubs/contrib/admin/
--rw-r--r--   0 marti     (1000) marti      (121)     1157 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      313 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/actions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1078 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/admin/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2167 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/admin/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3887 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/filters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      237 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5534 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/admin/helpers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.105006 django-stubs-4.2.7/django-stubs/contrib/admin/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1052 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/admin/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    16305 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4088 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/admin/sites.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.108339 django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1981 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/admin_list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      690 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/admin_modify.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      503 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/admin_urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      605 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/log.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1629 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/tests.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4121 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/admin/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.108339 django-stubs-4.2.7/django-stubs/contrib/admin/views/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      374 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/views/autocomplete.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      383 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admin/views/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3126 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/admin/views/main.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5664 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/admin/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.108339 django-stubs-4.2.7/django-stubs/contrib/admindocs/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admindocs/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admindocs/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      478 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admindocs/middleware.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admindocs/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admindocs/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1018 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/admindocs/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.115006 django-stubs-4.2.7/django-stubs/contrib/auth/
--rw-r--r--   0 marti     (1000) marti      (121)     1272 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      560 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/auth/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1891 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/backends.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1572 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/auth/base_user.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      662 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      955 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/contrib/auth/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3962 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/auth/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.115006 django-stubs-4.2.7/django-stubs/contrib/auth/handlers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/handlers/modwsgi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2417 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/auth/hashers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.115006 django-stubs-4.2.7/django-stubs/contrib/auth/management/
--rw-r--r--   0 marti     (1000) marti      (121)      406 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/auth/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.118339 django-stubs-4.2.7/django-stubs/contrib/auth/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/management/commands/changepassword.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      194 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.118339 django-stubs-4.2.7/django-stubs/contrib/auth/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1228 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4789 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/auth/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2081 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/password_validation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      735 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/contrib/auth/tokens.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/auth/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      153 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/auth/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2550 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/auth/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.118339 django-stubs-4.2.7/django-stubs/contrib/contenttypes/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      655 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       76 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      414 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3851 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1421 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.118339 django-stubs-4.2.7/django-stubs/contrib/contenttypes/management/
--rw-r--r--   0 marti     (1000) marti      (121)     1305 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.118339 django-stubs-4.2.7/django-stubs/contrib/contenttypes/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      363 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.118339 django-stubs-4.2.7/django-stubs/contrib/contenttypes/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1040 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/contenttypes/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.121672 django-stubs-4.2.7/django-stubs/contrib/flatpages/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      259 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.121672 django-stubs-4.2.7/django-stubs/contrib/flatpages/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      402 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       81 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/sitemaps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.121672 django-stubs-4.2.7/django-stubs/contrib/flatpages/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      484 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/flatpages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.125006 django-stubs-4.2.7/django-stubs/contrib/gis/
--rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.125006 django-stubs-4.2.7/django-stubs/contrib/gis/admin/
--rw-r--r--   0 marti     (1000) marti      (121)      872 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1215 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/gis/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      272 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/admin/widgets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       67 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.125006 django-stubs-4.2.7/django-stubs/contrib/gis/db/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.125006 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.128339 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1443 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      836 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1408 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/operations.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.128339 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      251 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      867 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      333 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1268 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      699 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.128339 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      226 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      254 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      444 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      287 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      893 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1440 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.131672 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      351 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/const.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      360 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      931 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2320 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      340 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.135005 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      835 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      127 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      417 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      451 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      941 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1345 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1103 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      656 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.135005 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)      834 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6184 2023-10-23 19:46:47.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6848 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2955 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/proxy.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.135005 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/sql/
--rw-r--r--   0 marti     (1000) marti      (121)      166 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/db/models/sql/conversion.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      866 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/feeds.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.138339 django-stubs-4.2.7/django-stubs/contrib/gis/forms/
--rw-r--r--   0 marti     (1000) marti      (121)      642 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      808 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/gis/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      951 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.141672 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/
--rw-r--r--   0 marti     (1000) marti      (121)     1070 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      137 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      574 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/datasource.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      324 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/driver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      688 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/envelope.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/error.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      947 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/feature.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1460 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/field.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4844 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/geometries.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      304 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/geomtype.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1741 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/layer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      858 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/libgdal.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.141672 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1036 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      961 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1077 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      970 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1053 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      614 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.145005 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/raster/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/raster/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1565 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/raster/band.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/raster/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/raster/const.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2395 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/raster/source.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2193 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/contrib/gis/gdal/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.145005 django-stubs-4.2.7/django-stubs/contrib/gis/geoip2/
--rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geoip2/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1202 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geoip2/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       99 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geoip2/resources.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       97 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geometry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.148339 django-stubs-4.2.7/django-stubs/contrib/gis/geos/
--rw-r--r--   0 marti     (1000) marti      (121)      883 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      604 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/collections.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1252 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       36 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/error.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      276 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/factory.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5320 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/geometry.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      453 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/io.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      896 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/libgeos.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      766 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/linestring.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1126 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/mutable_list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      816 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/point.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      713 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/polygon.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prepared.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.151672 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/
--rw-r--r--   0 marti     (1000) marti      (121)     4249 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      795 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      474 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      792 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/io.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/misc.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      553 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      434 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      609 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/topology.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1343 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/contrib/gis/measure.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/ptr.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.151672 django-stubs-4.2.7/django-stubs/contrib/gis/serializers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      493 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/serializers/geojson.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      244 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.151672 django-stubs-4.2.7/django-stubs/contrib/gis/sitemaps/
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      328 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/sitemaps/kml.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      352 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.155005 django-stubs-4.2.7/django-stubs/contrib/gis/utils/
--rw-r--r--   0 marti     (1000) marti      (121)      436 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2526 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/utils/layermapping.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/gis/utils/ogrinfo.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      320 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/utils/ogrinspect.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      199 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/utils/srs.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      202 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/gis/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.155005 django-stubs-4.2.7/django-stubs/contrib/humanize/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/humanize/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/humanize/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.155005 django-stubs-4.2.7/django-stubs/contrib/humanize/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/humanize/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      859 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/humanize/templatetags/humanize.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.158338 django-stubs-4.2.7/django-stubs/contrib/messages/
--rw-r--r--   0 marti     (1000) marti      (121)      715 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1294 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/api.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      349 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.158338 django-stubs-4.2.7/django-stubs/contrib/messages/storage/
--rw-r--r--   0 marti     (1000) marti      (121)      168 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/messages/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      906 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      463 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/storage/cookie.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      228 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/storage/fallback.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      468 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/storage/session.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       44 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/messages/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      427 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/messages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.161672 django-stubs-4.2.7/django-stubs/contrib/postgres/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.161672 django-stubs-4.2.7/django-stubs/contrib/postgres/aggregates/
--rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/aggregates/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      668 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/aggregates/general.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       29 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/aggregates/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      617 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/aggregates/statistics.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      270 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      847 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/constraints.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      459 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/expressions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.161672 django-stubs-4.2.7/django-stubs/contrib/postgres/fields/
--rw-r--r--   0 marti     (1000) marti      (121)      759 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1942 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/fields/array.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/fields/citext.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      764 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/fields/hstore.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      376 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/fields/jsonb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2480 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/fields/ranges.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/fields/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.165005 django-stubs-4.2.7/django-stubs/contrib/postgres/forms/
--rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2299 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/forms/array.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      478 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/forms/hstore.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      207 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/forms/jsonb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1504 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/forms/ranges.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      223 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4041 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/indexes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      631 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2045 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3845 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/search.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      230 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      707 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/postgres/validators.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.165005 django-stubs-4.2.7/django-stubs/contrib/redirects/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/redirects/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/redirects/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/redirects/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/redirects/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.165005 django-stubs-4.2.7/django-stubs/contrib/redirects/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/redirects/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      150 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/redirects/models.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.168338 django-stubs-4.2.7/django-stubs/contrib/sessions/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.168338 django-stubs-4.2.7/django-stubs/contrib/sessions/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1869 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/backends/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/backends/cached_db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      549 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      239 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/backends/file.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/backends/signed_cookies.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      734 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/base_session.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      210 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.168338 django-stubs-4.2.7/django-stubs/contrib/sessions/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.168338 django-stubs-4.2.7/django-stubs/contrib/sessions/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      155 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      447 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.168338 django-stubs-4.2.7/django-stubs/contrib/sessions/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      243 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      337 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sessions/serializers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.171672 django-stubs-4.2.7/django-stubs/contrib/sitemaps/
--rw-r--r--   0 marti     (1000) marti      (121)     1909 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sitemaps/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.171672 django-stubs-4.2.7/django-stubs/contrib/sitemaps/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sitemaps/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.171672 django-stubs-4.2.7/django-stubs/contrib/sitemaps/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      694 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.175005 django-stubs-4.2.7/django-stubs/contrib/sites/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sites/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sites/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       69 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sites/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/sites/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      289 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/sites/management.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sites/managers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      209 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sites/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.175005 django-stubs-4.2.7/django-stubs/contrib/sites/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sites/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      605 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/sites/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      307 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/sites/requests.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      221 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/sites/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.175005 django-stubs-4.2.7/django-stubs/contrib/staticfiles/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      263 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2489 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/finders.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1815 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/handlers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.175005 django-stubs-4.2.7/django-stubs/contrib/staticfiles/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.178338 django-stubs-4.2.7/django-stubs/contrib/staticfiles/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1055 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       87 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2245 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/storage.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/testing.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/staticfiles/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.178338 django-stubs-4.2.7/django-stubs/contrib/syndication/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/syndication/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      131 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/contrib/syndication/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1889 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/contrib/syndication/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.178338 django-stubs-4.2.7/django-stubs/core/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/asgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.178338 django-stubs-4.2.7/django-stubs/core/cache/
--rw-r--r--   0 marti     (1000) marti      (121)      686 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/cache/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.181672 django-stubs-4.2.7/django-stubs/core/cache/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/cache/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4121 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/cache/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      634 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/cache/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/cache/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      259 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/cache/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      226 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/cache/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      908 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/cache/backends/memcached.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/cache/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.185005 django-stubs-4.2.7/django-stubs/core/checks/
--rw-r--r--   0 marti     (1000) marti      (121)      652 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/async_checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      529 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/caches.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.185005 django-stubs-4.2.7/django-stubs/core/checks/compatibility/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/compatibility/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      256 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/checks/compatibility/django_4_0.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      229 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/database.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      268 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/checks/files.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1084 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/messages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/model_checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1837 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/checks/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.185005 django-stubs-4.2.7/django-stubs/core/checks/security/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/security/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2087 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/checks/security/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      514 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/checks/security/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/security/sessions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      565 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/checks/templates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      625 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/translation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      706 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/checks/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1968 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.188338 django-stubs-4.2.7/django-stubs/core/files/
--rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/files/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1613 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/files/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      359 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/files/images.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/files/locks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      130 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/files/move.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.191671 django-stubs-4.2.7/django-stubs/core/files/storage/
--rw-r--r--   0 marti     (1000) marti      (121)      724 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/files/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/core/files/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      910 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/files/storage/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      509 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/files/storage/handler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      884 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/files/storage/memory.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      338 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/files/storage/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/files/temp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1446 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/core/files/uploadedfile.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3017 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/files/uploadhandler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      736 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/files/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.191671 django-stubs-4.2.7/django-stubs/core/handlers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2129 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/handlers/asgi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1220 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/handlers/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      770 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/handlers/exception.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1435 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/handlers/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.191671 django-stubs-4.2.7/django-stubs/core/mail/
--rw-r--r--   0 marti     (1000) marti      (121)     1714 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/core/mail/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.195005 django-stubs-4.2.7/django-stubs/core/mail/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/mail/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      670 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/core/mail/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      303 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/mail/backends/console.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/mail/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/mail/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/mail/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      395 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/mail/backends/smtp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4658 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/mail/message.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/mail/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.195005 django-stubs-4.2.7/django-stubs/core/management/
--rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3784 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1178 2023-10-23 19:46:47.000000 django-stubs-4.2.7/django-stubs/core/management/color.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.201671 django-stubs-4.2.7/django-stubs/core/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      179 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/check.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      503 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/compilemessages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/createcachetable.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      155 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/dbshell.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      568 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/diffsettings.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      153 2023-10-23 19:46:47.000000 django-stubs-4.2.7/django-stubs/core/management/commands/dumpdata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      220 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/flush.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      880 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/inspectdb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2347 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/loaddata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2320 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/makemessages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      847 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/core/management/commands/makemigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      643 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/migrate.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      617 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      111 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/sendtestemail.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      319 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/shell.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      371 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/showmigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      184 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/sqlflush.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      203 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/sqlmigrate.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       83 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/sqlsequencereset.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      405 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/squashmigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/startapp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/management/commands/startproject.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/test.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/commands/testserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/sql.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1033 2023-10-23 19:46:47.000000 django-stubs-4.2.7/django-stubs/core/management/templates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      850 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/management/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2272 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/paginator.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.205005 django-stubs-4.2.7/django-stubs/core/serializers/
--rw-r--r--   0 marti     (1000) marti      (121)     1193 2023-10-23 19:46:47.000000 django-stubs-4.2.7/django-stubs/core/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3435 2023-10-23 19:46:47.000000 django-stubs-4.2.7/django-stubs/core/serializers/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/serializers/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/serializers/jsonl.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      490 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/serializers/python.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      831 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/serializers/pyyaml.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2321 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/core/serializers/xml_serializer.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.205005 django-stubs-4.2.7/django-stubs/core/servers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/servers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1165 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/servers/basehttp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      139 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1846 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/signing.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4435 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/core/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/core/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.205005 django-stubs-4.2.7/django-stubs/db/
--rw-r--r--   0 marti     (1000) marti      (121)     1047 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.205005 django-stubs-4.2.7/django-stubs/db/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.208338 django-stubs-4.2.7/django-stubs/db/backends/base/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5488 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/backends/base/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      555 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/base/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1301 2023-10-23 19:46:47.000000 django-stubs-4.2.7/django-stubs/db/backends/base/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5709 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1870 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/base/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     7157 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/base/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4384 2023-10-23 19:46:47.000000 django-stubs-4.2.7/django-stubs/db/backends/base/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/base/validation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3134 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/ddl_references.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.208338 django-stubs-4.2.7/django-stubs/db/backends/dummy/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/dummy/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      924 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/dummy/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      176 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/dummy/features.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.211671 django-stubs-4.2.7/django-stubs/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2491 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      473 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      734 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      255 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3812 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      568 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2872 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      902 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      354 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/mysql/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.215005 django-stubs-4.2.7/django-stubs/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2711 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      546 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      373 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1923 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      351 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3990 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      924 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      308 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/oracle/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.215005 django-stubs-4.2.7/django-stubs/db/backends/postgresql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/postgresql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1441 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/backends/postgresql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      524 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/postgresql/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/postgresql/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2256 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/backends/postgresql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      304 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/postgresql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      529 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/postgresql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      809 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/postgresql/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       63 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.218338 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1052 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      322 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      205 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1014 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/backends/sqlite3/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2896 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.221671 django-stubs-4.2.7/django-stubs/db/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/autodetector.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      664 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1739 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/executor.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2404 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/migrations/graph.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/loader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1161 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/db/migrations/migration.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.221671 django-stubs-4.2.7/django-stubs/db/migrations/operations/
--rw-r--r--   0 marti     (1000) marti      (121)     1159 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/migrations/operations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1522 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/migrations/operations/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1251 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/migrations/operations/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5188 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/db/migrations/operations/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1932 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/migrations/operations/special.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      974 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/migrations/operations/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      290 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/optimizer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/questioner.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      886 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/db/migrations/recorder.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/serializer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4952 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/migrations/state.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      195 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1235 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/migrations/writer.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.225005 django-stubs-4.2.7/django-stubs/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)     4584 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      782 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4661 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       96 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/models/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2288 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/db/models/constraints.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3733 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/deletion.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1921 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/enums.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10469 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/expressions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.228338 django-stubs-4.2.7/django-stubs/db/models/fields/
--rw-r--r--   0 marti     (1000) marti      (121)    21759 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4009 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/db/models/fields/files.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3594 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/fields/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/models/fields/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      161 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/models/fields/proxy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    11783 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/fields/related.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6523 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/fields/related_descriptors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1393 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/models/fields/related_lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4727 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/fields/reverse_related.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.231671 django-stubs-4.2.7/django-stubs/db/models/functions/
--rw-r--r--   0 marti     (1000) marti      (121)     3407 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/functions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      567 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/functions/comparison.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1393 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/functions/datetime.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1222 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/models/functions/math.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/models/functions/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4746 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/functions/text.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      988 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/functions/window.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2266 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/db/models/indexes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6022 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     7787 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/manager.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5288 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10861 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/query.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3285 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/db/models/query_utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      908 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/db/models/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.231671 django-stubs-4.2.7/django-stubs/db/models/sql/
--rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6767 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/sql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/models/sql/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1791 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/models/sql/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     9568 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/sql/query.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1619 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/db/models/sql/subqueries.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2245 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/models/sql/where.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      473 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/db/models/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2178 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/db/transaction.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2120 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/db/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.231671 django-stubs-4.2.7/django-stubs/dispatch/
--rw-r--r--   0 marti     (1000) marti      (121)      116 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/dispatch/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1251 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/dispatch/dispatcher.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.235005 django-stubs-4.2.7/django-stubs/forms/
--rw-r--r--   0 marti     (1000) marti      (121)     4083 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2898 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/forms/boundfield.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    20629 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3220 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/forms/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3902 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/forms/formsets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    12162 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/forms/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1191 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/forms/renderers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2479 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/forms/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10440 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.235005 django-stubs-4.2.7/django-stubs/http/
--rw-r--r--   0 marti     (1000) marti      (121)     1332 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/http/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      108 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/http/cookie.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1979 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/http/multipartparser.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     8732 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/http/request.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5813 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/http/response.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.238338 django-stubs-4.2.7/django-stubs/middleware/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/middleware/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1063 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/middleware/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/middleware/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      968 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/middleware/common.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1816 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/middleware/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      339 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/middleware/gzip.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      369 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/middleware/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/middleware/locale.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      645 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/middleware/security.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1514 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.241671 django-stubs-4.2.7/django-stubs/template/
--rw-r--r--   0 marti     (1000) marti      (121)      756 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.245004 django-stubs-4.2.7/django-stubs/template/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      935 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/template/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/backends/django.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      402 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/template/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      931 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/template/backends/jinja2.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/backends/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5631 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/template/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3368 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/template/context.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      631 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3483 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/defaultfilters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6912 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/defaulttags.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2224 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/template/engine.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3244 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/library.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      670 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/template/loader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2289 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/template/loader_tags.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.245004 django-stubs-4.2.7/django-stubs/template/loaders/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/loaders/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       88 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/loaders/app_directories.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/loaders/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      554 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/loaders/cached.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      518 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/loaders/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      323 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/loaders/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2434 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/template/response.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1246 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/template/smartif.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      648 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/template/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.245004 django-stubs-4.2.7/django-stubs/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      629 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/templatetags/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3492 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/templatetags/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      410 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/templatetags/l10n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1123 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/templatetags/static.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1076 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/templatetags/tz.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.248338 django-stubs-4.2.7/django-stubs/test/
--rw-r--r--   0 marti     (1000) marti      (121)      890 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/test/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     9606 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/test/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1372 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/test/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6591 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/test/runner.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      539 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/test/selenium.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1307 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/test/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10502 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/test/testcases.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6312 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/test/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.251671 django-stubs-4.2.7/django-stubs/urls/
--rw-r--r--   0 marti     (1000) marti      (121)     1578 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      857 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/urls/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1465 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/urls/conf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      778 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/urls/converters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      102 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/urls/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4722 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/urls/resolvers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/urls/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.265004 django-stubs-4.2.7/django-stubs/utils/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/_os.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1487 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/utils/archive.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      230 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/asyncio.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2872 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/autoreload.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      591 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/baseconv.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1287 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1300 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/connection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      570 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/crypto.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4674 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/utils/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2045 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/utils/dateformat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      505 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/dateparse.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/dates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      557 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/utils/datetime_safe.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      606 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/utils/deconstruct.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      876 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1776 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/utils/deprecation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/duration.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3195 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/utils/encoding.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2803 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/utils/feedgenerator.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1850 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/utils/formats.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4252 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/utils/functional.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       66 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/hashable.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2485 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/utils/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1283 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/inspect.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/ipv6.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       61 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/itercompat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      714 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/jslex.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1742 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/utils/log.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      242 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/lorem_ipsum.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      312 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/module_loading.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      319 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/numberformat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      917 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/regex_helper.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      589 2023-06-29 17:05:25.000000 django-stubs-4.2.7/django-stubs/utils/safestring.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/termcolors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2069 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/utils/text.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      423 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/timesince.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2011 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/timezone.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/topological_sort.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.265004 django-stubs-4.2.7/django-stubs/utils/translation/
--rw-r--r--   0 marti     (1000) marti      (121)     2033 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/translation/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/utils/translation/reloader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      335 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/translation/template.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      801 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/translation/trans_null.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2965 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/utils/translation/trans_real.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      986 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/tree.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      518 2023-06-27 17:49:10.000000 django-stubs-4.2.7/django-stubs/utils/version.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      424 2023-12-05 19:01:16.000000 django-stubs-4.2.7/django-stubs/utils/xmlutils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.268338 django-stubs-4.2.7/django-stubs/views/
--rw-r--r--   0 marti     (1000) marti      (121)       39 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3125 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/views/debug.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.268338 django-stubs-4.2.7/django-stubs/views/decorators/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/decorators/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      347 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/views/decorators/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/decorators/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      162 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/decorators/common.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      427 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/decorators/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      259 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/views/decorators/debug.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      146 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/decorators/gzip.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      718 2023-06-02 14:08:54.000000 django-stubs-4.2.7/django-stubs/views/decorators/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/decorators/vary.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      807 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/views/defaults.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.271671 django-stubs-4.2.7/django-stubs/views/generic/
--rw-r--r--   0 marti     (1000) marti      (121)      797 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/generic/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2416 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/views/generic/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4561 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/views/generic/dates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.7/django-stubs/views/generic/detail.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3507 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/views/generic/edit.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1963 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/views/generic/list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1042 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/views/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      465 2023-10-18 16:41:31.000000 django-stubs-4.2.7/django-stubs/views/static.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.278337 django-stubs-4.2.7/django_stubs.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)    16619 2023-12-05 19:02:17.000000 django-stubs-4.2.7/django_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)    30513 2023-12-05 19:02:17.000000 django-stubs-4.2.7/django_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-12-05 19:02:17.000000 django-stubs-4.2.7/django_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-12-05 19:02:17.000000 django-stubs-4.2.7/django_stubs.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       32 2023-12-05 19:02:17.000000 django-stubs-4.2.7/django_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.275004 django-stubs-4.2.7/mypy_django_plugin/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/mypy_django_plugin/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     4295 2023-06-27 17:49:10.000000 django-stubs-4.2.7/mypy_django_plugin/config.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.275004 django-stubs-4.2.7/mypy_django_plugin/django/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/mypy_django_plugin/django/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)    22208 2023-10-18 16:41:31.000000 django-stubs-4.2.7/mypy_django_plugin/django/context.py
--rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.7/mypy_django_plugin/errorcodes.py
--rw-r--r--   0 marti     (1000) marti      (121)       89 2023-06-27 17:49:10.000000 django-stubs-4.2.7/mypy_django_plugin/exceptions.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.275004 django-stubs-4.2.7/mypy_django_plugin/lib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/mypy_django_plugin/lib/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     2831 2023-12-05 19:01:16.000000 django-stubs-4.2.7/mypy_django_plugin/lib/fullnames.py
--rw-r--r--   0 marti     (1000) marti      (121)    16996 2023-12-05 19:01:16.000000 django-stubs-4.2.7/mypy_django_plugin/lib/helpers.py
--rw-r--r--   0 marti     (1000) marti      (121)    15293 2023-12-05 19:01:16.000000 django-stubs-4.2.7/mypy_django_plugin/main.py
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/mypy_django_plugin/py.typed
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.278337 django-stubs-4.2.7/mypy_django_plugin/transformers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)    10130 2023-10-23 19:46:47.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/fields.py
--rw-r--r--   0 marti     (1000) marti      (121)     1787 2023-06-27 17:49:10.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/forms.py
--rw-r--r--   0 marti     (1000) marti      (121)     1313 2023-06-27 17:49:10.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/functional.py
--rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/init_create.py
--rw-r--r--   0 marti     (1000) marti      (121)    24685 2023-12-05 19:01:16.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/managers.py
--rw-r--r--   0 marti     (1000) marti      (121)     8113 2023-12-05 19:01:16.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/manytomany.py
--rw-r--r--   0 marti     (1000) marti      (121)     1938 2023-06-27 17:49:10.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/meta.py
--rw-r--r--   0 marti     (1000) marti      (121)    48193 2023-12-05 19:01:16.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/models.py
--rw-r--r--   0 marti     (1000) marti      (121)     2821 2023-12-05 19:01:16.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/orm_lookups.py
--rw-r--r--   0 marti     (1000) marti      (121)    13235 2023-10-23 19:46:47.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/querysets.py
--rw-r--r--   0 marti     (1000) marti      (121)     2048 2023-06-27 17:49:10.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/request.py
--rw-r--r--   0 marti     (1000) marti      (121)     2495 2023-06-27 17:49:10.000000 django-stubs-4.2.7/mypy_django_plugin/transformers/settings.py
--rw-r--r--   0 marti     (1000) marti      (121)     1453 2023-10-18 16:41:31.000000 django-stubs-4.2.7/pyproject.toml
--rw-r--r--   0 marti     (1000) marti      (121)       38 2023-12-05 19:02:17.278337 django-stubs-4.2.7/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     2264 2023-12-05 19:01:16.000000 django-stubs-4.2.7/setup.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:02:17.278337 django-stubs-4.2.7/tests/
--rw-r--r--   0 marti     (1000) marti      (121)     5744 2023-10-18 16:41:31.000000 django-stubs-4.2.7/tests/test_error_handling.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1075 2023-06-02 14:08:54.000000 django_stubs-5.0.0/LICENSE.md
+-rw-r--r--   0 marti     (1000) marti     (1000)    16027 2024-04-30 10:03:06.921465 django_stubs-5.0.0/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti     (1000)    14648 2024-04-30 10:01:49.000000 django_stubs-5.0.0/README.md
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/
+-rw-r--r--   0 marti     (1000) marti     (1000)      224 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/apps/
+-rw-r--r--   0 marti     (1000) marti     (1000)       78 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/apps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1125 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/apps/config.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1970 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/apps/registry.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/conf/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1545 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/conf/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    17238 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/conf/global_settings.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/conf/locale/
+-rw-r--r--   0 marti     (1000) marti     (1000)       50 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/conf/locale/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/conf/urls/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1073 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/conf/urls/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      231 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/conf/urls/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      193 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/conf/urls/static.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/contrib/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admin/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1203 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      313 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/actions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      136 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1078 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/admin/checks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2167 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/admin/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      251 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4313 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/filters.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      237 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/forms.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5570 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/helpers.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admin/migrations/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1052 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/admin/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    16634 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/options.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4347 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/sites.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1981 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_list.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      690 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_modify.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      503 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_urls.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      605 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      441 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/log.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1629 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/tests.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4488 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admin/views/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/views/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      374 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/views/autocomplete.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      383 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/views/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3177 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/views/main.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5651 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admindocs/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      129 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      478 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/middleware.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       60 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/urls.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      840 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1018 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1735 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      560 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/auth/admin.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       68 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1891 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/backends.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1592 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/base_user.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      398 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/checks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      662 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      955 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/auth/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3962 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/auth/forms.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/handlers/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/handlers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      198 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/handlers/modwsgi.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2614 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/hashers.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/management/
+-rw-r--r--   0 marti     (1000) marti     (1000)      406 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/auth/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/management/commands/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      125 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/management/commands/changepassword.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      194 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      818 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/migrations/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1228 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4693 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2114 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/password_validation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      120 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/signals.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      735 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/contrib/auth/tokens.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       60 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/urls.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      153 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/auth/validators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2550 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/auth/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/contenttypes/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      655 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/admin.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       76 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      414 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/checks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3851 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/fields.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1421 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/forms.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1305 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/commands/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      363 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/contenttypes/migrations/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1040 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      213 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/flatpages/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      259 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/admin.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      129 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      136 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/forms.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      293 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/flatpages/migrations/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      402 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       81 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/sitemaps.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/flatpages/templatetags/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      484 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       60 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/urls.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      309 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/admin/
+-rw-r--r--   0 marti     (1000) marti     (1000)      724 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/admin/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      261 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/admin/options.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      272 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/admin/widgets.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       67 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/db/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      200 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1443 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      836 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1408 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/operations.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      251 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      867 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      333 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1268 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      699 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      226 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      254 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      444 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      287 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      727 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1440 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      826 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      399 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      351 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      189 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/const.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      407 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      360 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      765 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2320 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      247 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      340 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      182 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      835 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      127 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      417 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      451 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      775 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1345 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1103 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      656 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/
+-rw-r--r--   0 marti     (1000) marti     (1000)      834 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      800 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/aggregates.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     6433 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/fields.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     6939 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/functions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2955 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      345 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/proxy.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/sql/
+-rw-r--r--   0 marti     (1000) marti     (1000)      166 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/sql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      829 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/sql/conversion.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      866 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/feeds.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/forms/
+-rw-r--r--   0 marti     (1000) marti     (1000)      642 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      808 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/gis/forms/fields.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      952 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/forms/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1070 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      137 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      574 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/datasource.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      324 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/driver.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      688 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/envelope.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      200 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/error.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      947 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/feature.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1460 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/field.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4844 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/geometries.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      304 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/geomtype.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1741 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/layer.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      858 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/libgdal.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1036 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      961 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1077 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      970 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1053 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      614 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1565 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/band.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      225 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      252 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/const.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2395 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/source.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2193 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/srs.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/
+-rw-r--r--   0 marti     (1000) marti     (1000)      106 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1202 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       99 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/resources.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       97 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geometry.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/geos/
+-rw-r--r--   0 marti     (1000) marti     (1000)      883 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      185 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      604 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/collections.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1252 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/coordseq.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       36 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/error.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      310 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/factory.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5385 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/geometry.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      453 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/io.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      896 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/libgeos.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      766 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/linestring.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1126 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/mutable_list.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      816 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/point.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      713 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/polygon.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      737 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prepared.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/
+-rw-r--r--   0 marti     (1000) marti     (1000)     4249 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      795 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      474 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      792 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/geom.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3014 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/io.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      232 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/misc.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      789 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      434 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      496 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      609 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/topology.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1343 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/gis/measure.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      252 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/ptr.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/serializers/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/serializers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      493 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/serializers/geojson.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      244 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/sitemaps/
+-rw-r--r--   0 marti     (1000) marti     (1000)      138 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/sitemaps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      328 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/sitemaps/kml.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      352 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/sitemaps/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/utils/
+-rw-r--r--   0 marti     (1000) marti     (1000)      436 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2561 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/layermapping.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      129 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/ogrinfo.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      320 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/ogrinspect.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      199 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/srs.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      202 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/humanize/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/humanize/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      128 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/humanize/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/humanize/templatetags/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/humanize/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      859 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/humanize/templatetags/humanize.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/messages/
+-rw-r--r--   0 marti     (1000) marti     (1000)      690 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/messages/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1294 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/api.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      193 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/messages/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      120 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/constants.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      225 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      349 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/messages/storage/
+-rw-r--r--   0 marti     (1000) marti     (1000)      168 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      906 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      463 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/cookie.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      228 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/fallback.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      468 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/session.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       44 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      427 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/messages/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/postgres/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/
+-rw-r--r--   0 marti     (1000) marti     (1000)      864 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2208 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/general.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      822 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      910 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/statistics.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      270 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1320 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/constraints.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      459 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/expressions.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/
+-rw-r--r--   0 marti     (1000) marti     (1000)      759 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2399 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/array.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      385 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/citext.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1013 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/hstore.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       99 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/jsonb.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3182 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/ranges.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      106 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/
+-rw-r--r--   0 marti     (1000) marti     (1000)      604 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2299 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/array.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      478 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/hstore.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1537 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/ranges.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      223 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/functions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4041 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/indexes.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      877 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2045 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4829 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/search.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      152 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      383 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/signals.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      177 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      707 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/validators.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/redirects/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      185 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/admin.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      129 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      379 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/redirects/migrations/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      150 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/models.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/sessions/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      128 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1892 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      280 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/cache.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      286 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/cached_db.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      549 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/db.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      239 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/file.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      100 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/signed_cookies.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      677 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/base_session.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      210 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/exceptions.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/sessions/management/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/sessions/management/commands/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      155 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      447 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/sessions/migrations/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      243 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      157 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/serializers.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/sitemaps/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1741 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sitemaps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      128 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sitemaps/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      694 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/sitemaps/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/sites/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      138 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/admin.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       69 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      247 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/sites/checks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      289 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/sites/management.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      247 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/managers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      209 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/sites/migrations/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      605 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/sites/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      375 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sites/requests.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      221 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/staticfiles/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      120 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      391 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/checks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2496 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/finders.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1815 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/handlers.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1170 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      206 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      120 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2355 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/storage.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      100 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/testing.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      152 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/urls.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      345 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      216 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/syndication/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/syndication/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      131 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/syndication/apps.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1889 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/syndication/views.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       98 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/asgi.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/cache/
+-rw-r--r--   0 marti     (1000) marti     (1000)      697 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/cache/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/cache/backends/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4184 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      634 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/db.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      182 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      259 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/filebased.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      226 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      776 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/memcached.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2296 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/redis.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      198 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/cache/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/checks/
+-rw-r--r--   0 marti     (1000) marti     (1000)      652 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      265 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/async_checks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      529 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/caches.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/checks/compatibility/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/compatibility/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      256 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/checks/compatibility/django_4_0.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      229 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/database.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      268 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/checks/files.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1084 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/messages.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      389 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/model_checks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1889 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/checks/registry.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/checks/security/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/security/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2087 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/checks/security/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      514 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/checks/security/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      577 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/security/sessions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      565 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/checks/templates.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      625 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/translation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      706 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/urls.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1968 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/exceptions.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/files/
+-rw-r--r--   0 marti     (1000) marti     (1000)       68 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1897 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/files/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      359 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/images.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      296 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/locks.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      130 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/move.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/files/storage/
+-rw-r--r--   0 marti     (1000) marti     (1000)      724 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/files/storage/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1073 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/core/files/storage/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      910 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/files/storage/filesystem.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      509 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/files/storage/handler.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      884 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/files/storage/memory.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      338 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/files/storage/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      100 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/temp.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1535 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/files/uploadedfile.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3017 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/uploadhandler.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      736 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/handlers/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/handlers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2473 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/handlers/asgi.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1353 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/handlers/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      770 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/handlers/exception.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1265 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/handlers/wsgi.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/mail/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1714 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/core/mail/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/mail/backends/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      670 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      303 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/console.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      103 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      128 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/filebased.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      103 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      454 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/smtp.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4034 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/mail/message.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       95 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.891465 django_stubs-5.0.0/django-stubs/core/management/
+-rw-r--r--   0 marti     (1000) marti     (1000)      945 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/management/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3804 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/management/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1178 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/core/management/color.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.891465 django_stubs-5.0.0/django-stubs/core/management/commands/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      179 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/check.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      503 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/compilemessages.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      284 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/createcachetable.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      155 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/dbshell.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      568 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/diffsettings.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      153 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/core/management/commands/dumpdata.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      220 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/flush.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      944 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/management/commands/inspectdb.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2347 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/loaddata.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2320 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/makemessages.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      847 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/management/commands/makemigrations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      643 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/migrate.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       85 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/management/commands/optimizemigration.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      617 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/runserver.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      111 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/sendtestemail.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      319 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/shell.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      371 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/showmigrations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      184 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/sqlflush.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      203 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/sqlmigrate.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       83 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/sqlsequencereset.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      405 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/squashmigrations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      225 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/startapp.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      225 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/startproject.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      232 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/test.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       85 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/testserver.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      488 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/sql.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1033 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/core/management/templates.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      850 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2516 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/paginator.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/core/serializers/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1193 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/core/serializers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3195 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/serializers/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      577 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/serializers/json.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      398 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/serializers/jsonl.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      490 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/serializers/python.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      831 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/serializers/pyyaml.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2355 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/serializers/xml_serializer.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/core/servers/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/servers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1459 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/servers/basehttp.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      139 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/signals.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2656 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/signing.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4626 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/validators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       98 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/wsgi.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1047 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/backends/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/backends/base/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/base/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5434 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/base/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      555 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/base/client.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1301 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/db/backends/base/creation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5747 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/base/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1870 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/base/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     7157 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/base/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4499 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/base/schema.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      389 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/base/validation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3183 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/ddl_references.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/backends/dummy/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/dummy/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      924 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/dummy/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      176 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/dummy/features.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/backends/mysql/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2491 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      473 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/client.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      734 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/compiler.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      255 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/creation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3812 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      568 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2872 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      902 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/schema.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      354 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/validation.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.898132 django_stubs-5.0.0/django-stubs/db/backends/oracle/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2718 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      546 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/client.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      373 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/creation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1874 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      398 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/functions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      351 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3990 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      924 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/schema.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      511 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      308 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/validation.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.898132 django_stubs-5.0.0/django-stubs/db/backends/postgresql/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1441 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      524 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/client.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      208 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/creation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2256 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      304 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      529 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      809 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/schema.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       63 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/signals.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.898132 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1052 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      441 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/client.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      322 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/creation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      205 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/features.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      432 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1014 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/operations.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      215 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/schema.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2930 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.901465 django_stubs-5.0.0/django-stubs/db/migrations/
+-rw-r--r--   0 marti     (1000) marti     (1000)      265 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2830 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/autodetector.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      664 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1770 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/migrations/executor.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2404 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/graph.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1960 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/loader.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1161 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/db/migrations/migration.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.901465 django_stubs-5.0.0/django-stubs/db/migrations/operations/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1159 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1522 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1251 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/fields.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5188 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1965 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/special.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      974 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      290 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/optimizer.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1109 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/questioner.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      887 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/migrations/recorder.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1835 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/serializer.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4952 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/state.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      195 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1235 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/writer.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.901465 django_stubs-5.0.0/django-stubs/db/models/
+-rw-r--r--   0 marti     (1000) marti     (1000)     4647 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      821 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/aggregates.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4692 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       96 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/models/constants.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2994 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/constraints.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3733 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/deletion.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2021 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/enums.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    10469 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/expressions.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/db/models/fields/
+-rw-r--r--   0 marti     (1000) marti     (1000)    22400 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4525 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/files.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1766 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/generated.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3929 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/json.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      515 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/fields/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      161 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/fields/proxy.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    12081 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/related.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     6978 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/related_descriptors.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1393 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/fields/related_lookups.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4804 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/reverse_related.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/db/models/functions/
+-rw-r--r--   0 marti     (1000) marti     (1000)     3407 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      567 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/comparison.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1393 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/datetime.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1222 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/functions/math.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      100 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/functions/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4746 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/text.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      988 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/window.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2266 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/db/models/indexes.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     6017 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     8022 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/manager.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5288 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/options.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    11068 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/query.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3549 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/query_utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      908 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/db/models/signals.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/db/models/sql/
+-rw-r--r--   0 marti     (1000) marti     (1000)      284 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/sql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     6753 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/sql/compiler.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      286 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/models/sql/constants.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1791 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/sql/datastructures.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     9563 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/sql/query.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1619 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/models/sql/subqueries.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2259 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/sql/where.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      551 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2178 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/db/transaction.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2120 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/dispatch/
+-rw-r--r--   0 marti     (1000) marti     (1000)      116 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/dispatch/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1453 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/dispatch/dispatcher.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/forms/
+-rw-r--r--   0 marti     (1000) marti     (1000)     4083 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2940 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/boundfield.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    20466 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/fields.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3164 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/forms.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3902 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/forms/formsets.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    12164 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/models.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1191 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/forms/renderers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2479 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/forms/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    10519 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.908132 django_stubs-5.0.0/django-stubs/http/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1332 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/http/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      108 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/http/cookie.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2007 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/http/multipartparser.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     8951 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/http/request.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5834 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/http/response.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.908132 django_stubs-5.0.0/django-stubs/middleware/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1063 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/middleware/cache.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      387 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/clickjacking.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      968 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/common.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1794 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/middleware/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      339 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/gzip.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      369 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/http.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      417 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/locale.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      645 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/security.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1807 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.908132 django_stubs-5.0.0/django-stubs/template/
+-rw-r--r--   0 marti     (1000) marti     (1000)      756 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.908132 django_stubs-5.0.0/django-stubs/template/backends/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      974 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/template/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1062 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/backends/django.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      402 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      931 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/backends/jinja2.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      215 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/backends/utils.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     5561 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/template/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3368 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/template/context.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      631 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3540 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/template/defaultfilters.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     6912 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/defaulttags.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2224 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/engine.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      511 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3244 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/library.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      670 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/template/loader.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2289 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/template/loader_tags.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.911465 django_stubs-5.0.0/django-stubs/template/loaders/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       88 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/app_directories.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      488 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      554 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/cached.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      518 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/filesystem.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      323 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2434 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/response.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1246 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/smartif.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      648 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.911465 django_stubs-5.0.0/django-stubs/templatetags/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      629 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/cache.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3492 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      410 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/l10n.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1123 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/static.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1039 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/templatetags/tz.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.911465 django_stubs-5.0.0/django-stubs/test/
+-rw-r--r--   0 marti     (1000) marti     (1000)      890 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/test/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)    13259 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/client.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1345 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/html.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     6645 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/runner.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      539 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/test/selenium.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1307 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/test/signals.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     9605 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/testcases.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     6346 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.911465 django_stubs-5.0.0/django-stubs/urls/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1578 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/urls/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      922 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/urls/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1851 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/urls/conf.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      996 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/urls/converters.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      102 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/urls/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4668 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/urls/resolvers.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      157 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/urls/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.914798 django_stubs-5.0.0/django-stubs/utils/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      286 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/_os.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1487 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/utils/archive.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      230 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/asyncio.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2872 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/autoreload.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1287 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/cache.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1101 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/choices.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1300 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/connection.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      570 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/crypto.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4759 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/datastructures.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2005 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/dateformat.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      505 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/dateparse.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      156 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/dates.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      640 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/deconstruct.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1155 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1829 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/deprecation.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      198 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/duration.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3195 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/utils/encoding.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2803 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/utils/feedgenerator.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1850 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/utils/formats.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4231 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/functional.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       66 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/hashable.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2510 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/html.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1307 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/http.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      483 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/inspect.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      175 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/ipv6.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)       61 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/itercompat.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      714 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/jslex.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1742 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/utils/log.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      242 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/lorem_ipsum.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      312 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/module_loading.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      319 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/numberformat.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      917 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/regex_helper.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      589 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/utils/safestring.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      627 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/termcolors.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2392 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/text.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      423 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/timesince.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1557 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/timezone.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/django-stubs/utils/translation/
+-rw-r--r--   0 marti     (1000) marti     (1000)     2033 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/translation/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      286 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/translation/reloader.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      335 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/translation/template.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      801 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/translation/trans_null.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3000 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/translation/trans_real.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      986 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/tree.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      518 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/version.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      424 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/utils/xmlutils.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/django-stubs/views/
+-rw-r--r--   0 marti     (1000) marti     (1000)       39 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      323 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3125 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/views/debug.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/django-stubs/views/decorators/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      347 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/views/decorators/cache.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      274 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/clickjacking.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      162 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/common.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      427 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      361 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/decorators/debug.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      146 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/gzip.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      718 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/views/decorators/http.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      218 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/vary.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      807 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/views/defaults.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/django-stubs/views/generic/
+-rw-r--r--   0 marti     (1000) marti     (1000)      797 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/generic/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     2428 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/generic/base.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     4561 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/views/generic/dates.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1109 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/generic/detail.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     3393 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/generic/edit.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1963 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/views/generic/list.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)     1091 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti     (1000)      502 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/static.pyi
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/django_stubs.egg-info/
+-rw-r--r--   0 marti     (1000) marti     (1000)    16027 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti     (1000)    30353 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)        1 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)      151 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)       32 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/mypy_django_plugin/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     4784 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/config.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/mypy_django_plugin/django/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/django/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)    22288 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/django/context.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      227 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/errorcodes.py
+-rw-r--r--   0 marti     (1000) marti     (1000)       89 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/exceptions.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/mypy_django_plugin/lib/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/lib/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     3087 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/lib/fullnames.py
+-rw-r--r--   0 marti     (1000) marti     (1000)    17822 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/lib/helpers.py
+-rw-r--r--   0 marti     (1000) marti     (1000)    15367 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/main.py
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/py.typed
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/mypy_django_plugin/transformers/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)    11307 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/fields.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     1787 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/forms.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     1313 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/functional.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     3104 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/init_create.py
+-rw-r--r--   0 marti     (1000) marti     (1000)    25150 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/managers.py
+-rw-r--r--   0 marti     (1000) marti     (1000)    10079 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/manytomany.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     1938 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/meta.py
+-rw-r--r--   0 marti     (1000) marti     (1000)    49032 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/models.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     2821 2023-12-05 19:01:16.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/orm_lookups.py
+-rw-r--r--   0 marti     (1000) marti     (1000)    13235 2023-10-23 19:46:47.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/querysets.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     2048 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/request.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     2495 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/settings.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     1841 2024-04-30 10:01:49.000000 django_stubs-5.0.0/pyproject.toml
+-rw-r--r--   0 marti     (1000) marti     (1000)       38 2024-04-30 10:03:06.921465 django_stubs-5.0.0/setup.cfg
+-rw-r--r--   0 marti     (1000) marti     (1000)     2348 2024-04-30 10:01:49.000000 django_stubs-5.0.0/setup.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/tests/
+-rw-r--r--   0 marti     (1000) marti     (1000)     7607 2024-04-30 10:01:49.000000 django_stubs-5.0.0/tests/test_error_handling.py
```

### Comparing `django-stubs-4.2.7/LICENSE.md` & `django_stubs-5.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/PKG-INFO` & `django_stubs-5.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 4.2.7
+Version: 5.0.0
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
+Project-URL: Funding, https://github.com/sponsors/typeddjango
 Project-URL: Release notes, https://github.com/typeddjango/django-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
-Requires-Dist: django-stubs-ext>=4.2.7
+Requires-Dist: asgiref
+Requires-Dist: django-stubs-ext>=5.0.0
 Requires-Dist: tomli; python_version < "3.11"
 Requires-Dist: typing-extensions
-Requires-Dist: types-pytz
 Requires-Dist: types-PyYAML
 Provides-Extra: compatible-mypy
-Requires-Dist: mypy~=1.7.0; extra == "compatible-mypy"
+Requires-Dist: mypy~=1.10.0; extra == "compatible-mypy"
+Provides-Extra: redis
+Requires-Dist: redis; extra == "redis"
 
 <img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 [![StackOverflow](https://shields.io/badge/ask-stackoverflow-orange?logo=stackoverflow)](https://stackoverflow.com/questions/tagged/django-stubs)
@@ -70,24 +73,25 @@
 [tool.django-stubs]
 django_settings_module = "myproject.settings"
 ```
 
 Two things happening here:
 
 1. We need to explicitly list our plugin to be loaded by `mypy`
-2. Our plugin also requires `django` settings module (what you put into `DJANGO_SETTINGS_MODULE` variable) to be specified
+2. You can either specify `django_settings_module` as seen above, or let `django_stubs` use the `DJANGO_SETTINGS_MODULE` variable from your environment.
 
 This fully working [typed boilerplate](https://github.com/wemake-services/wemake-django-template) can serve you as an example.
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 5.0.0          | 1.10.x       | 5.0            | 4.2, 4.1               | 3.8 - 3.12     |
 | 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
@@ -126,15 +130,15 @@
 django-stubs has a few settings, which you can list in:
 
 * `pyproject.toml`, under the table `[tool.django-stubs]`
 * `mypy.ini` under the table `[mypy.plugins.django-stubs]`
 
 The supported settings are:
 
-- `django_settings_module`, a string.
+- `django_settings_module`, a string, default to `os.getenv(DJANGO_SETTINGS_MODULE)`.
 
   Specify the import path of your settings module, the same as Django’s [`DJANGO_SETTINGS_MODULE` environment variable](https://docs.djangoproject.com/en/stable/topics/settings/#designating-the-settings).
 
 - `strict_settings`, a boolean, default `true`.
 
   Set to `false` if using dynamic settings, as [described below](https://github.com/typeddjango/django-stubs#how-to-use-a-custom-library-to-handle-django-settings).
 
@@ -207,62 +211,14 @@
 
 class AuthenticatedHttpRequest(HttpRequest):
     user: MyUser
 ```
 
 And then use `AuthenticatedHttpRequest` instead of the standard `HttpRequest` for when you know that the user is authenticated. For example in views using the `@login_required` decorator.
 
-### My QuerySet methods are returning Any rather than my Model
-
-If you are using `MyQuerySet.as_manager()`:
-
-Example:
-
-```python
-from django.db import models
-
-class MyModelQuerySet(models.QuerySet):
-    pass
-
-
-class MyModel(models.Model):
-    bar = models.IntegerField()
-    objects = MyModelQuerySet.as_manager()
-
-
-def use_my_model() -> int:
-    foo = MyModel.objects.get(id=1) # Should now be `MyModel`
-    return foo.xyz # Gives an error
-```
-
-Or if you're using `Manager.from_queryset`:
-
-Example:
-
-```python
-from django.db import models
-
-
-class MyModelQuerySet(models.QuerySet):
-    pass
-
-
-MyModelManager = models.Manager.from_queryset(MyModelQuerySet)
-
-
-class MyModel(models.Model):
-    bar = models.IntegerField()
-    objects = MyModelManager()
-
-
-def use_my_model() -> int:
-    foo = MyModel.objects.get(id=1) # Should now be `MyModel`
-    return foo.xyz # Gives an error
-```
-
 ### Why am I getting incompatible return type errors on my custom managers?
 
 If you declare your custom managers without generics and override built-in
 methods you might see an error message about incompatible error messages,
 something like this:
 
 ```python
@@ -383,15 +339,15 @@
 ```
 
 So, mypy would not like this code:
 
 ```python
 from django.conf import settings
 
-settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_SETTING'
+settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_VALUE'
 ```
 
 To handle this corner case we have a special setting `strict_settings` (`True` by default),
 you can switch it to `False` to always return `Any` and not raise any errors if runtime settings module has the given value,
 for example `pyproject.toml`:
 
 ```toml
@@ -406,15 +362,15 @@
 strict_settings = false
 ```
 
 And then:
 
 ```python
 # Works:
-reveal_type(settings.EXISTS_IN_RUNTIME)  # N: Any
+reveal_type(settings.EXISTS_AT_RUNTIME)  # N: Any
 
 # Errors:
 reveal_type(settings.MISSING)  # E: 'Settings' object has no attribute 'MISSING'
 ```
 
 ## Related projects
```

### Comparing `django-stubs-4.2.7/README.md` & `django_stubs-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,24 +35,25 @@
 [tool.django-stubs]
 django_settings_module = "myproject.settings"
 ```
 
 Two things happening here:
 
 1. We need to explicitly list our plugin to be loaded by `mypy`
-2. Our plugin also requires `django` settings module (what you put into `DJANGO_SETTINGS_MODULE` variable) to be specified
+2. You can either specify `django_settings_module` as seen above, or let `django_stubs` use the `DJANGO_SETTINGS_MODULE` variable from your environment.
 
 This fully working [typed boilerplate](https://github.com/wemake-services/wemake-django-template) can serve you as an example.
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 5.0.0          | 1.10.x       | 5.0            | 4.2, 4.1               | 3.8 - 3.12     |
 | 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
@@ -91,15 +92,15 @@
 django-stubs has a few settings, which you can list in:
 
 * `pyproject.toml`, under the table `[tool.django-stubs]`
 * `mypy.ini` under the table `[mypy.plugins.django-stubs]`
 
 The supported settings are:
 
-- `django_settings_module`, a string.
+- `django_settings_module`, a string, default to `os.getenv(DJANGO_SETTINGS_MODULE)`.
 
   Specify the import path of your settings module, the same as Django’s [`DJANGO_SETTINGS_MODULE` environment variable](https://docs.djangoproject.com/en/stable/topics/settings/#designating-the-settings).
 
 - `strict_settings`, a boolean, default `true`.
 
   Set to `false` if using dynamic settings, as [described below](https://github.com/typeddjango/django-stubs#how-to-use-a-custom-library-to-handle-django-settings).
 
@@ -172,62 +173,14 @@
 
 class AuthenticatedHttpRequest(HttpRequest):
     user: MyUser
 ```
 
 And then use `AuthenticatedHttpRequest` instead of the standard `HttpRequest` for when you know that the user is authenticated. For example in views using the `@login_required` decorator.
 
-### My QuerySet methods are returning Any rather than my Model
-
-If you are using `MyQuerySet.as_manager()`:
-
-Example:
-
-```python
-from django.db import models
-
-class MyModelQuerySet(models.QuerySet):
-    pass
-
-
-class MyModel(models.Model):
-    bar = models.IntegerField()
-    objects = MyModelQuerySet.as_manager()
-
-
-def use_my_model() -> int:
-    foo = MyModel.objects.get(id=1) # Should now be `MyModel`
-    return foo.xyz # Gives an error
-```
-
-Or if you're using `Manager.from_queryset`:
-
-Example:
-
-```python
-from django.db import models
-
-
-class MyModelQuerySet(models.QuerySet):
-    pass
-
-
-MyModelManager = models.Manager.from_queryset(MyModelQuerySet)
-
-
-class MyModel(models.Model):
-    bar = models.IntegerField()
-    objects = MyModelManager()
-
-
-def use_my_model() -> int:
-    foo = MyModel.objects.get(id=1) # Should now be `MyModel`
-    return foo.xyz # Gives an error
-```
-
 ### Why am I getting incompatible return type errors on my custom managers?
 
 If you declare your custom managers without generics and override built-in
 methods you might see an error message about incompatible error messages,
 something like this:
 
 ```python
@@ -348,15 +301,15 @@
 ```
 
 So, mypy would not like this code:
 
 ```python
 from django.conf import settings
 
-settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_SETTING'
+settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_VALUE'
 ```
 
 To handle this corner case we have a special setting `strict_settings` (`True` by default),
 you can switch it to `False` to always return `Any` and not raise any errors if runtime settings module has the given value,
 for example `pyproject.toml`:
 
 ```toml
@@ -371,15 +324,15 @@
 strict_settings = false
 ```
 
 And then:
 
 ```python
 # Works:
-reveal_type(settings.EXISTS_IN_RUNTIME)  # N: Any
+reveal_type(settings.EXISTS_AT_RUNTIME)  # N: Any
 
 # Errors:
 reveal_type(settings.MISSING)  # E: 'Settings' object has no attribute 'MISSING'
 ```
 
 ## Related projects
```

### Comparing `django-stubs-4.2.7/django-stubs/apps/config.pyi` & `django_stubs-5.0.0/django-stubs/apps/config.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 class AppConfig:
     name: str
     module: types.ModuleType | None
     apps: Apps | None
     label: str
     verbose_name: _StrOrPromise
     path: str
-    models_module: str | None
+    models_module: types.ModuleType | None
     # Default auto_field is a cached_property on the base, but is usually subclassed as a str
     # If not subclassing with a str, a type ignore[override] is needed
     models: dict[str, type[Model]]
+    default: bool
     default_auto_field: str | _Getter[str]
     def __init__(self, app_name: str, app_module: types.ModuleType | None) -> None: ...
     @classmethod
     def create(cls, entry: str) -> AppConfig: ...
     def get_model(self, model_name: str, require_ready: bool = ...) -> type[Model]: ...
     def get_models(self, include_auto_created: bool = ..., include_swapped: bool = ...) -> Iterator[type[Model]]: ...
     def import_models(self) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/apps/registry.pyi` & `django_stubs-5.0.0/django-stubs/apps/registry.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     apps_ready: bool
     ready_event: threading.Event
     loading: bool
     _pending_operations: dict[tuple[str, str], list]
     models_ready: bool
     ready: bool
     def __init__(self, installed_apps: Iterable[AppConfig | str] | None = ...) -> None: ...
-    def populate(self, installed_apps: Iterable[AppConfig | str] = ...) -> None: ...
+    def populate(self, installed_apps: Iterable[AppConfig | str] | None = ...) -> None: ...
     def check_apps_ready(self) -> None: ...
     def check_models_ready(self) -> None: ...
     def get_app_configs(self) -> Iterable[AppConfig]: ...
     def get_app_config(self, app_label: str) -> AppConfig: ...
     # it's not possible to support it in plugin properly now
     def get_models(self, include_auto_created: bool = ..., include_swapped: bool = ...) -> list[type[Model]]: ...
     def get_model(self, app_label: str, model_name: str | None = ..., require_ready: bool = ...) -> type[Any]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/conf/__init__.pyi` & `django_stubs-5.0.0/django-stubs/conf/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from typing import Any, Literal
+from typing import Any, Literal, type_check_only
 
 from django.utils.functional import LazyObject
 from typing_extensions import Self
 
 # explicit dependency on standard settings to make it loaded
 from . import global_settings  # noqa: F401
 
 ENVIRONMENT_VARIABLE: Literal["DJANGO_SETTINGS_MODULE"]
 DEFAULT_STORAGE_ALIAS: Literal["default"]
 STATICFILES_STORAGE_ALIAS: Literal["staticfiles"]
 
+# RemovedInDjango60Warning.
+FORMS_URLFIELD_ASSUME_HTTPS_DEPRECATED_MSG: str
+
 # required for plugin to be able to distinguish this specific instance of LazySettings from others
+@type_check_only
 class _DjangoConfLazyObject(LazyObject):
     def __getattr__(self, item: Any) -> Any: ...
 
 class LazySettings(_DjangoConfLazyObject):
     SETTINGS_MODULE: str
     @property
     def configured(self) -> bool: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/conf/global_settings.pyi` & `django_stubs-5.0.0/django-stubs/conf/global_settings.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Sequence
 from re import Pattern
 
 # This is defined here as a do-nothing function because we can't import
 # django.utils.translation -- that module depends on the settings.
-from typing import Any, Literal, Protocol
+from typing import Any, Literal, Protocol, type_check_only
 
 from typing_extensions import TypeAlias
 
 _Admins: TypeAlias = list[tuple[str, str]]
 
 ####################
 # CORE             #
@@ -36,15 +36,14 @@
 # https://en.wikipedia.org/wiki/List_of_tz_zones_by_name (although not all
 # systems may support all possibilities). When USE_TZ is True, this is
 # interpreted as the default user time zone.
 TIME_ZONE: str
 
 # If you set this to True, Django will use timezone-aware datetimes.
 USE_TZ: bool
-USE_DEPRECATED_PYTZ: bool
 
 # Language code for this installation. All choices can be found here:
 # http://www.i18nguy.com/unicode/language-identifiers.html
 LANGUAGE_CODE: str
 
 # Languages we provide translations for, out of the box.
 LANGUAGES: list[tuple[str, str]]
@@ -62,18 +61,14 @@
 LANGUAGE_COOKIE_AGE: int | None
 LANGUAGE_COOKIE_DOMAIN: str | None
 LANGUAGE_COOKIE_PATH: str
 LANGUAGE_COOKIE_HTTPONLY: bool
 LANGUAGE_COOKIE_SAMESITE: Literal["Lax", "Strict", "None", False] | None
 LANGUAGE_COOKIE_SECURE: bool
 
-# If you set this to True, Django will format dates, numbers and calendars
-# according to user current locale.
-USE_L10N: bool
-
 # Not-necessarily-technical managers of the site. They get broken link
 # notifications and other various emails.
 MANAGERS: _Admins
 
 # Default charset to use for all HttpResponse objects, if a
 # MIME type isn't manually specified. These are used to construct the
 # Content-Type header.
@@ -82,14 +77,15 @@
 # Email address that error messages come from.
 SERVER_EMAIL: str
 
 # Database connection info. If left empty, will default to the dummy backend.
 DATABASES: dict[str, dict[str, Any]]
 
 # Classes used to implement DB routing behavior.
+@type_check_only
 class Router(Protocol):
     def allow_migrate(self, db: str, app_label: str, **hints: Any) -> bool | None: ...
 
 DATABASE_ROUTERS: list[str | Router]
 
 # The email backend to use. For possible shortcuts see django.core.mail.
 # The default is to use the SMTP backend.
@@ -119,14 +115,19 @@
 INSTALLED_APPS: list[str]
 
 TEMPLATES: list[dict[str, Any]]
 
 # Default form rendering class.
 FORM_RENDERER: str
 
+# RemovedInDjango60Warning: It's a transitional setting helpful in early
+# adoption of "https" as the new default value of forms.URLField.assume_scheme.
+# Set to True to assume "https" during the Django 5.x release cycle.
+FORMS_URLFIELD_ASSUME_HTTPS: bool
+
 # Default email address to use for various automated correspondence from
 # the site managers.
 DEFAULT_FROM_EMAIL: str
 
 # Subject-line prefix for email messages send with django.core.mail.mail_admins
 # or ...mail_managers.  Make sure to include the trailing space.
 EMAIL_SUBJECT_PREFIX: str
@@ -429,18 +430,14 @@
 CSRF_COOKIE_SECURE: bool
 CSRF_COOKIE_HTTPONLY: bool
 CSRF_COOKIE_SAMESITE: Literal["Lax", "Strict", "None", False]
 CSRF_HEADER_NAME: str
 CSRF_TRUSTED_ORIGINS: list[str]
 CSRF_USE_SESSIONS: bool
 
-# Whether to mask CSRF cookie value. It's a transitional setting helpful in
-# migrating multiple instance of the same project to Django 4.1+.
-CSRF_COOKIE_MASKED: bool
-
 ############
 # MESSAGES #
 ############
 
 # Class to use as messages backend
 MESSAGE_STORAGE: str
 
@@ -498,15 +495,15 @@
 STATICFILES_FINDERS: list[str]
 
 ##############
 # MIGRATIONS #
 ##############
 
 # Migration module overrides for apps, by app label.
-MIGRATION_MODULES: dict[str, str]
+MIGRATION_MODULES: dict[str, str | None]
 
 #################
 # SYSTEM CHECKS #
 #################
 
 # List of all issues generated by system checks that should be silenced. Light
 # issues like warnings, infos or debugs will not generate a message. Silencing
```

### Comparing `django-stubs-4.2.7/django-stubs/conf/urls/__init__.pyi` & `django_stubs-5.0.0/django-stubs/conf/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 from .filters import ListFilter as ListFilter
 from .filters import RelatedFieldListFilter as RelatedFieldListFilter
 from .filters import RelatedOnlyFieldListFilter as RelatedOnlyFieldListFilter
 from .filters import SimpleListFilter as SimpleListFilter
 from .options import HORIZONTAL as HORIZONTAL
 from .options import VERTICAL as VERTICAL
 from .options import ModelAdmin as ModelAdmin
+from .options import ShowFacets as ShowFacets
 from .options import StackedInline as StackedInline
 from .options import TabularInline as TabularInline
 from .sites import AdminSite as AdminSite
 from .sites import site as site
 
 def autodiscover() -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/checks.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/checks.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/decorators.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/filters.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/filters.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,126 @@
 from collections.abc import Callable, Iterable, Iterator
-from typing import Any
+from datetime import date, datetime
+from typing import Any, ClassVar
 
 from django.contrib.admin.options import ModelAdmin
+from django.contrib.admin.views.main import ChangeList
+from django.db.models.aggregates import Count
 from django.db.models.base import Model
 from django.db.models.fields import Field
 from django.db.models.fields.related import RelatedField
 from django.db.models.query import QuerySet
+from django.db.models.query_utils import Q
 from django.http.request import HttpRequest
+from django.utils.datastructures import _ListOrTuple
 from django.utils.functional import _StrOrPromise
+from django.utils.safestring import SafeString
+from typing_extensions import TypedDict
+
+class _ListFilterChoices(TypedDict):
+    selected: bool
+    query_string: str
+    display: _StrOrPromise
 
 class ListFilter:
     title: _StrOrPromise | None
     template: str
-    used_parameters: Any
+    request: HttpRequest
+    used_parameters: dict[str, bool | datetime | str]
     def __init__(
         self, request: HttpRequest, params: dict[str, str], model: type[Model], model_admin: ModelAdmin
     ) -> None: ...
     def has_output(self) -> bool: ...
-    def choices(self, changelist: Any) -> Iterator[dict[str, Any]]: ...
+    def choices(self, changelist: ChangeList) -> Iterator[_ListFilterChoices]: ...
     def queryset(self, request: HttpRequest, queryset: QuerySet) -> QuerySet | None: ...
     def expected_parameters(self) -> list[str | None]: ...
 
-class SimpleListFilter(ListFilter):
+class FacetsMixin:
+    def get_facet_counts(self, pk_attname: str, filtered_qs: QuerySet[Model]) -> dict[str, Count]: ...
+    def get_facet_queryset(self, changelist: ChangeList) -> dict[str, int]: ...
+
+class SimpleListFilter(FacetsMixin, ListFilter):
     parameter_name: str | None
-    lookup_choices: Any
+    lookup_choices: list[tuple[str, _StrOrPromise]]
     def value(self) -> str | None: ...
-    def lookups(self, request: HttpRequest, model_admin: ModelAdmin) -> Iterable[tuple[Any, str]] | None: ...
-    def choices(self, changelist: Any) -> Iterator[dict[str, Any]]: ...
+    def lookups(self, request: HttpRequest, model_admin: ModelAdmin) -> Iterable[tuple[str, _StrOrPromise]] | None: ...
 
-class FieldListFilter(ListFilter):
+class FieldListFilter(FacetsMixin, ListFilter):
+    list_separator: ClassVar[str]
     field: Field
     field_path: str
-    title: str
+    title: _StrOrPromise
     def __init__(
         self,
         field: Field,
         request: HttpRequest,
         params: dict[str, str],
         model: type[Model],
         model_admin: ModelAdmin,
         field_path: str,
     ) -> None: ...
     @classmethod
-    def register(cls, test: Callable, list_filter_class: type[FieldListFilter], take_priority: bool = ...) -> None: ...
+    def register(
+        cls, test: Callable[[Field], Any], list_filter_class: type[FieldListFilter], take_priority: bool = ...
+    ) -> None: ...
     @classmethod
     def create(
         cls,
         field: Field,
         request: HttpRequest,
         params: dict[str, str],
         model: type[Model],
         model_admin: ModelAdmin,
         field_path: str,
     ) -> FieldListFilter: ...
 
 class RelatedFieldListFilter(FieldListFilter):
-    used_parameters: dict[Any, Any]
     lookup_kwarg: str
     lookup_kwarg_isnull: str
-    lookup_val: Any
-    lookup_val_isnull: Any
-    lookup_choices: Any
-    lookup_title: str
-    title: str
-    empty_value_display: Any
+    lookup_val: str | None
+    lookup_val_isnull: str | None
+    lookup_choices: list[tuple[str, _StrOrPromise]]
+    lookup_title: _StrOrPromise
+    empty_value_display: SafeString
     @property
     def include_empty_choice(self) -> bool: ...
+    def field_admin_ordering(
+        self, field: RelatedField, request: HttpRequest, model_admin: ModelAdmin
+    ) -> _ListOrTuple[str]: ...
     def field_choices(
         self, field: RelatedField, request: HttpRequest, model_admin: ModelAdmin
-    ) -> list[tuple[str, str]]: ...
-    def choices(self, changelist: Any) -> Iterator[dict[str, Any]]: ...
+    ) -> list[tuple[str, _StrOrPromise]]: ...
 
 class BooleanFieldListFilter(FieldListFilter):
     lookup_kwarg: str
     lookup_kwarg2: str
-    lookup_val: Any
-    lookup_val2: Any
-    def choices(self, changelist: Any) -> Iterator[dict[str, Any]]: ...
+    lookup_val: str | None
+    lookup_val2: str | None
 
 class ChoicesFieldListFilter(FieldListFilter):
-    title: str
-    used_parameters: dict[Any, Any]
     lookup_kwarg: str
     lookup_kwarg_isnull: str
-    lookup_val: Any
-    lookup_val_isnull: Any
-    def choices(self, changelist: Any) -> Iterator[dict[str, Any]]: ...
+    lookup_val: str | None
+    lookup_val_isnull: str | None
 
 class DateFieldListFilter(FieldListFilter):
-    field_generic: Any
-    date_params: Any
-    lookup_kwarg_since: Any
-    lookup_kwarg_until: Any
-    links: Any
-    lookup_kwarg_isnull: Any
-    def choices(self, changelist: Any) -> Iterator[dict[str, Any]]: ...
+    field_generic: str
+    date_params: dict[str, str]
+    lookup_kwarg_since: str
+    lookup_kwarg_until: str
+    links: tuple[tuple[_StrOrPromise, dict[str, bool | date | datetime]], ...]
+    lookup_kwarg_isnull: str
 
 class AllValuesFieldListFilter(FieldListFilter):
-    title: str
-    used_parameters: dict[Any, Any]
     lookup_kwarg: str
     lookup_kwarg_isnull: str
-    lookup_val: Any
-    lookup_val_isnull: Any
-    empty_value_display: str
+    lookup_val: str | None
+    lookup_val_isnull: str | None
+    empty_value_display: SafeString
     lookup_choices: QuerySet
-    def choices(self, changelist: Any) -> Iterator[dict[str, Any]]: ...
 
-class RelatedOnlyFieldListFilter(RelatedFieldListFilter):
-    lookup_kwarg: str
-    lookup_kwarg_isnull: str
-    lookup_val: Any
-    lookup_val_isnull: Any
-    title: str
-    used_parameters: dict[Any, Any]
+class RelatedOnlyFieldListFilter(RelatedFieldListFilter): ...
 
 class EmptyFieldListFilter(FieldListFilter):
     lookup_kwarg: str
-    lookup_val: Any
-    def choices(self, changelist: Any) -> Iterator[dict[str, Any]]: ...
+    lookup_val: str | None
+    def get_lookup_condition(self) -> Q: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/helpers.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/helpers.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
-from typing import Any
+from typing import Any, type_check_only
 
 from django import forms
 from django.contrib.admin.options import ModelAdmin
 from django.db.models import Model
 from django.db.models.fields import AutoField
 from django.forms import BaseForm
 from django.forms.boundfield import BoundField
@@ -15,16 +15,15 @@
 
 ACTION_CHECKBOX_NAME: str
 
 class ActionForm(forms.Form):
     action: Any
     select_across: Any
 
-checkbox: Any
-
+@type_check_only
 class _PrepopulatedDict(TypedDict):
     field: BoundField
     dependencies: list[BoundField]
 
 class AdminForm:
     prepopulated_fields: list[_PrepopulatedDict]
     model_admin: ModelAdmin | None
@@ -88,14 +87,15 @@
     is_first: bool
     is_checkbox: bool
     is_readonly: bool
     def __init__(self, form: ModelForm, field: str, is_first: bool) -> None: ...
     def label_tag(self) -> SafeString: ...
     def errors(self) -> SafeString: ...
 
+@type_check_only
 class _FieldDictT(TypedDict):
     name: str
     label: str
     help_text: str
     field: Callable[[Model], Any] | str
 
 class AdminReadonlyField:
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/models.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/options.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/options.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import enum
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
-from typing import Any, Generic, Literal, TypeVar
+from typing import Any, Generic, Literal, TypeVar, type_check_only
 
 from django import forms
 from django.contrib.admin.filters import FieldListFilter, ListFilter
 from django.contrib.admin.models import LogEntry
 from django.contrib.admin.sites import AdminSite
 from django.contrib.admin.views.main import ChangeList
 from django.contrib.auth.forms import AdminPasswordChangeForm
@@ -33,46 +34,54 @@
 from django.utils.datastructures import _ListOrTuple
 from django.utils.functional import _StrOrPromise
 from django.utils.safestring import SafeString
 from typing_extensions import TypeAlias, TypedDict
 
 IS_POPUP_VAR: str
 TO_FIELD_VAR: str
+IS_FACETS_VAR: str
 HORIZONTAL: Literal[1]
 VERTICAL: Literal[2]
 
 _Direction: TypeAlias = Literal[1, 2]
 
+class ShowFacets(enum.Enum):
+    NEVER: str
+    ALLOW: str
+    ALWAYS: str
+
 def get_content_type_for_model(obj: type[Model] | Model) -> ContentType: ...
 def get_ul_class(radio_style: int) -> str: ...
 
 class IncorrectLookupParameters(Exception): ...
 
 FORMFIELD_FOR_DBFIELD_DEFAULTS: Any
 csrf_protect_m: Any
 
 _FieldGroups: TypeAlias = Sequence[str | Sequence[str]]
 
+@type_check_only
 class _OptionalFieldOpts(TypedDict, total=False):
     classes: Sequence[str]
     description: _StrOrPromise
 
+@type_check_only
 class _FieldOpts(_OptionalFieldOpts, total=True):
     fields: _FieldGroups
 
 # Workaround for mypy issue, a Sequence type should be preferred here.
 # https://github.com/python/mypy/issues/8921
 # _FieldsetSpec = Sequence[Tuple[Optional[str], _FieldOpts]]
 _FieldsetSpec: TypeAlias = _ListOrTuple[tuple[_StrOrPromise | None, _FieldOpts]]
 _ListFilterT: TypeAlias = (
     type[ListFilter]
-    | Field
+    | Field[Any, Any]
     | str
-    | tuple[Field | str, type[FieldListFilter]]
-    | list[Field | str | type[FieldListFilter]]
+    | tuple[Field[Any, Any] | str, type[FieldListFilter]]
+    | list[Field[Any, Any] | str | type[FieldListFilter]]
 )
 
 # Generic type specifically for models, for use in BaseModelAdmin and subclasses
 # https://github.com/typeddjango/django-stubs/issues/482
 _ModelT = TypeVar("_ModelT", bound=Model)
 _DisplayT: TypeAlias = _ListOrTuple[str | Callable[[_ModelT], str | bool]]
 
@@ -87,23 +96,22 @@
     filter_horizontal: _ListOrTuple[str]
     radio_fields: Mapping[str, _Direction]
     prepopulated_fields: dict[str, Sequence[str]]
     formfield_overrides: Mapping[type[Field], Mapping[str, Any]]
     readonly_fields: _ListOrTuple[str]
     ordering: _ListOrTuple[str] | None
     sortable_by: _ListOrTuple[str] | None
-    view_on_site: bool | Callable[[_ModelT], str]
     show_full_result_count: bool
     checks_class: Any
     model: type[_ModelT]
     opts: Options[_ModelT]
     admin_site: AdminSite
     def __init__(self) -> None: ...
     def check(self, **kwargs: Any) -> list[CheckMessage]: ...
-    def formfield_for_dbfield(self, db_field: Field, request: HttpRequest, **kwargs: Any) -> FormField | None: ...
+    def formfield_for_dbfield(self, db_field: Field, request: HttpRequest, **kwargs: Any) -> FormField: ...
     def formfield_for_choice_field(self, db_field: Field, request: HttpRequest, **kwargs: Any) -> TypedChoiceField: ...
     def get_field_queryset(self, db: str | None, db_field: RelatedField, request: HttpRequest) -> QuerySet | None: ...
     def formfield_for_foreignkey(
         self, db_field: ForeignKey, request: HttpRequest, **kwargs: Any
     ) -> ModelChoiceField: ...
     def formfield_for_manytomany(
         self, db_field: ManyToManyField, request: HttpRequest, **kwargs: Any
@@ -115,43 +123,46 @@
     def get_fields(self, request: HttpRequest, obj: _ModelT | None = ...) -> _FieldGroups: ...
     def get_fieldsets(self, request: HttpRequest, obj: _ModelT | None = ...) -> _FieldsetSpec: ...
     def get_inlines(self, request: HttpRequest, obj: _ModelT | None) -> list[type[InlineModelAdmin]]: ...
     def get_ordering(self, request: HttpRequest) -> _ListOrTuple[str]: ...
     def get_readonly_fields(self, request: HttpRequest, obj: _ModelT | None = ...) -> _ListOrTuple[str]: ...
     def get_prepopulated_fields(self, request: HttpRequest, obj: _ModelT | None = ...) -> dict[str, Sequence[str]]: ...
     def get_queryset(self, request: HttpRequest) -> QuerySet[_ModelT]: ...
-    def get_sortable_by(self, request: HttpRequest) -> _DisplayT: ...
-    def lookup_allowed(self, lookup: str, value: str) -> bool: ...
+    def get_sortable_by(self, request: HttpRequest) -> _DisplayT[_ModelT]: ...
+    def lookup_allowed(self, lookup: str, value: str, request: HttpRequest | None = ...) -> bool: ...
     def to_field_allowed(self, request: HttpRequest, to_field: str) -> bool: ...
     def has_add_permission(self, request: HttpRequest) -> bool: ...
     def has_change_permission(self, request: HttpRequest, obj: _ModelT | None = ...) -> bool: ...
     def has_delete_permission(self, request: HttpRequest, obj: _ModelT | None = ...) -> bool: ...
     def has_view_permission(self, request: HttpRequest, obj: _ModelT | None = ...) -> bool: ...
     def has_view_or_change_permission(self, request: HttpRequest, obj: _ModelT | None = ...) -> bool: ...
     def has_module_permission(self, request: HttpRequest) -> bool: ...
+    @property
+    def view_on_site(self) -> Callable[[_ModelT], str] | bool: ...
 
 _ModelAdmin = TypeVar("_ModelAdmin", bound=ModelAdmin)
 _ActionCallable: TypeAlias = Callable[[_ModelAdmin, HttpRequest, QuerySet[_ModelT]], HttpResponseBase | None]
 
 class ModelAdmin(BaseModelAdmin[_ModelT]):
-    list_display: _DisplayT
-    list_display_links: _DisplayT | None
+    list_display: _DisplayT[_ModelT]
+    list_display_links: _DisplayT[_ModelT] | None
     list_filter: _ListOrTuple[_ListFilterT]
     list_select_related: bool | _ListOrTuple[str]
     list_per_page: int
     list_max_show_all: int
     list_editable: _ListOrTuple[str]
     search_fields: _ListOrTuple[str]
     search_help_text: _StrOrPromise | None
     date_hierarchy: str | None
     save_as: bool
     save_as_continue: bool
     save_on_top: bool
     paginator: type
     preserve_filters: bool
+    show_facets: ShowFacets
     inlines: _ListOrTuple[type[InlineModelAdmin]]
     add_form_template: _TemplateForResponseT | None
     change_form_template: _TemplateForResponseT | None
     change_list_template: _TemplateForResponseT | None
     delete_confirmation_template: _TemplateForResponseT | None
     delete_selected_confirmation_template: _TemplateForResponseT | None
     object_history_template: _TemplateForResponseT | None
@@ -196,16 +207,16 @@
     def log_deletion(self, request: HttpRequest, object: _ModelT, object_repr: str) -> LogEntry: ...
     def action_checkbox(self, obj: _ModelT) -> SafeString: ...
     def get_actions(self, request: HttpRequest) -> dict[str, tuple[Callable[..., str], str, str] | None]: ...
     def get_action_choices(
         self, request: HttpRequest, default_choices: list[tuple[str, str]] = ...
     ) -> list[tuple[str, str]]: ...
     def get_action(self, action: Callable | str) -> tuple[Callable[..., str], str, str] | None: ...
-    def get_list_display(self, request: HttpRequest) -> _DisplayT: ...
-    def get_list_display_links(self, request: HttpRequest, list_display: _DisplayT) -> _DisplayT: ...
+    def get_list_display(self, request: HttpRequest) -> _DisplayT[_ModelT]: ...
+    def get_list_display_links(self, request: HttpRequest, list_display: _DisplayT[_ModelT]) -> _DisplayT[_ModelT]: ...
     def get_list_filter(self, request: HttpRequest) -> _ListOrTuple[_ListFilterT]: ...
     def get_list_select_related(self, request: HttpRequest) -> bool | _ListOrTuple[str]: ...
     def get_search_fields(self, request: HttpRequest) -> _ListOrTuple[str]: ...
     def get_search_results(
         self, request: HttpRequest, queryset: QuerySet, search_term: str
     ) -> tuple[QuerySet[_ModelT], bool]: ...
     def get_preserved_filters(self, request: HttpRequest) -> str: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/sites.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/sites.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from collections.abc import Callable, Iterable
-from typing import Any
+from typing import Any, TypeVar
 
 from django.apps.config import AppConfig
+from django.contrib.admin.models import LogEntry
 from django.contrib.admin.options import ModelAdmin
 from django.contrib.auth.forms import AuthenticationForm
 from django.core.checks import CheckMessage
 from django.db.models.base import Model
 from django.db.models.query import QuerySet
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse
@@ -20,19 +21,18 @@
 
     all_sites: WeakSet[AdminSite]
 else:
     from collections.abc import MutableSet
 
     all_sites: MutableSet[AdminSite]
 
+_ViewType = TypeVar("_ViewType", bound=Callable[..., HttpResponse])
+_ModelT = TypeVar("_ModelT", bound=Model)
 _ActionCallback: TypeAlias = Callable[[ModelAdmin, HttpRequest, QuerySet], TemplateResponse | None]
 
-class AlreadyRegistered(Exception): ...
-class NotRegistered(Exception): ...
-
 class AdminSite:
     site_title: _StrOrPromise
     site_header: _StrOrPromise
     index_title: _StrOrPromise
     site_url: str | None
     login_form: type[AuthenticationForm] | None
     index_template: str | None
@@ -55,21 +55,22 @@
         self,
         model_or_iterable: type[Model] | Iterable[type[Model]],
         admin_class: type[ModelAdmin] | None = ...,
         **options: Any,
     ) -> None: ...
     def unregister(self, model_or_iterable: type[Model] | Iterable[type[Model]]) -> None: ...
     def is_registered(self, model: type[Model]) -> bool: ...
+    def get_model_admin(self, model: type[_ModelT]) -> ModelAdmin[_ModelT]: ...
     def add_action(self, action: _ActionCallback, name: str | None = ...) -> None: ...
     def disable_action(self, name: str) -> None: ...
-    def get_action(self, name: str) -> Callable: ...
+    def get_action(self, name: str) -> _ActionCallback: ...
     @property
     def actions(self) -> Iterable[tuple[str, _ActionCallback]]: ...
     def has_permission(self, request: HttpRequest) -> bool: ...
-    def admin_view(self, view: Callable, cacheable: bool = ...) -> Callable: ...
+    def admin_view(self, view: _ViewType, cacheable: bool = ...) -> _ViewType: ...
     def get_urls(self) -> list[URLResolver | URLPattern]: ...
     @property
     def urls(self) -> tuple[list[URLResolver | URLPattern], str, str]: ...
     def each_context(self, request: HttpRequest) -> dict[str, Any]: ...
     def password_change(self, request: HttpRequest, extra_context: dict[str, Any] | None = ...) -> TemplateResponse: ...
     def password_change_done(
         self, request: HttpRequest, extra_context: dict[str, Any] | None = ...
@@ -81,11 +82,12 @@
     def get_app_list(self, request: HttpRequest, app_label: str | None = ...) -> list[Any]: ...
     def index(self, request: HttpRequest, extra_context: dict[str, Any] | None = ...) -> TemplateResponse: ...
     def app_index(
         self, request: HttpRequest, app_label: str, extra_context: dict[str, Any] | None = ...
     ) -> TemplateResponse: ...
     def autocomplete_view(self, request: HttpRequest) -> HttpResponse: ...
     def catch_all_view(self, request: HttpRequest, url: str) -> HttpResponse: ...
+    def get_log_entries(self, request: HttpRequest) -> QuerySet[LogEntry]: ...
 
 class DefaultAdminSite(LazyObject): ...
 
 site: AdminSite
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/admin_list.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/admin_modify.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_modify.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/templatetags/base.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/tests.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/tests.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/utils.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/utils.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import datetime
 from collections import defaultdict
 from collections.abc import Callable, Iterable, Sequence
-from typing import Any, Literal, TypeVar, overload
+from typing import Any, Literal, TypeVar, overload, type_check_only
 from uuid import UUID
 
 from _typeshed import Unused
 from django.contrib.admin.options import BaseModelAdmin
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth.forms import AdminPasswordChangeForm
 from django.db.models.base import Model
 from django.db.models.deletion import Collector
 from django.db.models.fields import Field, reverse_related
 from django.db.models.options import Options
 from django.db.models.query import QuerySet
+from django.db.models.query_utils import Q
 from django.forms.forms import BaseForm
 from django.forms.formsets import BaseFormSet
 from django.http.request import HttpRequest
 from django.utils.datastructures import _IndexableCollection
 from typing_extensions import TypedDict
 
 _T = TypeVar("_T")
 
 class FieldIsAForeignKeyColumnName(Exception): ...
 
 def lookup_spawns_duplicates(opts: Options, lookup_path: str) -> bool: ...
-def prepare_lookup_value(key: str, value: datetime.datetime | str) -> bool | datetime.datetime | str: ...
+def get_last_value_from_parameters(parameters: dict[str, list[str] | str], key: str) -> str | None: ...
+def prepare_lookup_value(
+    key: str, value: list[bool | datetime.datetime | str] | datetime.datetime | str, separator: str
+) -> list[bool | datetime.datetime | str] | bool | datetime.datetime | str: ...
+def build_q_object_from_lookup_parameters(parameters: dict[str, list[str]]) -> Q: ...
 def quote(s: int | str | UUID) -> str: ...
 def unquote(s: str) -> str: ...
 def flatten(fields: Any) -> list[Callable | str]: ...
 def flatten_fieldsets(fieldsets: Any) -> list[Callable | str]: ...
 def get_deleted_objects(
     objs: Sequence[Model | None] | QuerySet[Model], request: HttpRequest, admin_site: AdminSite
 ) -> tuple[list[str], dict[str, int], set[str], list[str]]: ...
@@ -55,14 +60,15 @@
     ) -> QuerySet[Model]: ...
     @overload
     def nested(self, format_callback: None = None) -> list[Model]: ...
     @overload
     def nested(self, format_callback: Callable[[Model], _T]) -> list[_T]: ...
     def can_fast_delete(self, *args: Unused, **kwargs: Unused) -> Literal[False]: ...
 
+@type_check_only
 class _ModelFormatDict(TypedDict):
     verbose_name: str
     verbose_name_plural: str
 
 def model_format_dict(obj: Model | type[Model] | QuerySet | Options[Model]) -> _ModelFormatDict: ...
 def model_ngettext(obj: Options | QuerySet, n: int | None = ...) -> str: ...
 def lookup_field(
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/views/main.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/views/main.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     can_show_all: bool
     multi_page: bool
     paginator: Any
     def get_results(self, request: HttpRequest) -> None: ...
     def get_ordering_field(self, field_name: Callable | str) -> Expression | str | None: ...
     def get_ordering(self, request: HttpRequest, queryset: QuerySet) -> list[Expression | str]: ...
     def get_ordering_field_columns(self) -> dict[int, Literal["desc", "asc"]]: ...
-    def get_queryset(self, request: HttpRequest) -> QuerySet: ...
+    def get_queryset(self, request: HttpRequest, exclude_parameters: list[str | None] | None = ...) -> QuerySet: ...
     filter_specs: list[ListFilter]
     has_filters: bool
     has_active_filters: bool
     clear_all_filters_qs: str
     def apply_select_related(self, qs: QuerySet) -> QuerySet: ...
     def has_related_field_in_list_display(self) -> bool: ...
     def url_for_result(self, result: Model) -> str: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admin/widgets.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admin/widgets.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from collections.abc import Iterable, Mapping, Sequence
 from typing import Any
 
 from django import forms
 from django.contrib.admin.sites import AdminSite
 from django.core.files.base import File
-from django.db.models.fields import _FieldChoices
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel
 from django.forms.models import ModelChoiceIterator
 from django.forms.widgets import _OptAttrs
+from django.utils.choices import _Choices
 from django.utils.functional import _StrOrPromise
 
 class FilteredSelectMultiple(forms.SelectMultiple):
     verbose_name: _StrOrPromise
     is_stacked: bool
     def __init__(
         self,
         verbose_name: _StrOrPromise,
         is_stacked: bool,
         attrs: _OptAttrs | None = ...,
-        choices: _FieldChoices = ...,
+        choices: _Choices = ...,
     ) -> None: ...
 
 class AdminDateWidget(forms.DateInput):
     def __init__(self, attrs: _OptAttrs | None = ..., format: str | None = ...) -> None: ...
 
 class AdminTimeWidget(forms.TimeInput):
     def __init__(self, attrs: _OptAttrs | None = ..., format: str | None = ...) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admindocs/utils.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admindocs/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/admindocs/views.pyi` & `django_stubs-5.0.0/django-stubs/contrib/admindocs/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,22 @@
 BACKEND_SESSION_KEY: str
 HASH_SESSION_KEY: str
 REDIRECT_FIELD_NAME: str
 
 def load_backend(path: str) -> ModelBackend: ...
 def get_backends() -> list[ModelBackend]: ...
 def authenticate(request: HttpRequest | None = ..., **credentials: Any) -> AbstractBaseUser | None: ...
+async def aauthenticate(request: HttpRequest | None = ..., **credentials: Any) -> AbstractBaseUser | None: ...
 def login(
     request: HttpRequest, user: AbstractBaseUser | None, backend: type[ModelBackend] | str | None = ...
 ) -> None: ...
+async def alogin(
+    request: HttpRequest, user: AbstractBaseUser | None, backend: type[ModelBackend] | str | None = ...
+) -> None: ...
 def logout(request: HttpRequest) -> None: ...
+async def alogout(request: HttpRequest) -> None: ...
 def get_user_model() -> type[AbstractBaseUser]: ...
 def get_user(request: HttpRequest | Client) -> AbstractBaseUser | AnonymousUser: ...
+async def aget_user(request: HttpRequest | Client) -> AbstractBaseUser | AnonymousUser: ...
 def get_permission_codename(action: str, opts: Options) -> str: ...
 def update_session_auth_hash(request: HttpRequest, user: AbstractBaseUser) -> None: ...
-
-default_app_config: str
+async def aupdate_session_auth_hash(request: HttpRequest, user: AbstractBaseUser) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/admin.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/admin.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/backends.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/backends.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/base_user.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/base_user.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,23 @@
 class AbstractBaseUser(models.Model):
     REQUIRED_FIELDS: ClassVar[list[str]]
 
     password = models.CharField(max_length=128)
     last_login = models.DateTimeField(blank=True, null=True)
     is_active: bool | BooleanField[bool | Combinable, bool]
 
-    class Meta:
-        abstract: Literal[True]
     def get_username(self) -> str: ...
     def natural_key(self) -> tuple[str]: ...
     @property
     def is_anonymous(self) -> Literal[False]: ...
     @property
     def is_authenticated(self) -> Literal[True]: ...
     def set_password(self, raw_password: str | None) -> None: ...
     def check_password(self, raw_password: str) -> bool: ...
+    async def acheck_password(self, raw_password: str) -> bool: ...
     def set_unusable_password(self) -> None: ...
     def has_usable_password(self) -> bool: ...
     def get_session_auth_hash(self) -> str: ...
     @classmethod
     def get_email_field_name(cls) -> str: ...
     @classmethod
     @overload
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/context_processors.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/decorators.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/forms.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/hashers.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/hashers.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from collections.abc import Callable
 from typing import Any
 
 UNUSABLE_PASSWORD_PREFIX: str
 UNUSABLE_PASSWORD_SUFFIX_LENGTH: int
 
 def is_password_usable(encoded: str | None) -> bool: ...
+def verify_password(password: str | None, encoded: str, preferred: str = ...) -> tuple[bool, bool]: ...
 def check_password(password: str | None, encoded: str, setter: Callable | None = ..., preferred: str = ...) -> bool: ...
+async def acheck_password(
+    password: str | None, encoded: str, setter: Callable | None = ..., preferred: str = ...
+) -> bool: ...
 def make_password(password: str | None, salt: str | None = ..., hasher: str | BasePasswordHasher = ...) -> str: ...
 def get_hashers() -> list[BasePasswordHasher]: ...
 def get_hashers_by_algorithm() -> dict[str, BasePasswordHasher]: ...
 def reset_hashers(**kwargs: Any) -> None: ...
 def get_hasher(algorithm: str | BasePasswordHasher = ...) -> BasePasswordHasher: ...
 def identify_hasher(encoded: str) -> BasePasswordHasher: ...
 def mask_hash(hash: str, show: int = ..., char: str = ...) -> str: ...
@@ -22,17 +26,17 @@
     memory_cost: int
     parallelism: int
     digest: Any
     iterations: int
     salt_entropy: int
     def salt(self) -> str: ...
     def verify(self, password: str, encoded: str) -> bool: ...
-    def encode(self, password: str, salt: str) -> Any: ...
+    def encode(self, password: str, salt: str) -> str: ...
     def decode(self, encoded: str) -> dict[str, Any]: ...
-    def safe_summary(self, encoded: str) -> Any: ...
+    def safe_summary(self, encoded: str) -> dict[str, Any]: ...
     def must_update(self, encoded: str) -> bool: ...
     def harden_runtime(self, password: str, encoded: str) -> None: ...
 
 class PBKDF2PasswordHasher(BasePasswordHasher):
     def encode(self, password: str, salt: str, iterations: int | None = ...) -> str: ...
     def decode(self, encoded: str) -> dict[str, str | int]: ...
 
@@ -51,9 +55,7 @@
     def decode(self, encoded: str) -> dict[str, str]: ...
 
 class UnsaltedSHA1PasswordHasher(BasePasswordHasher):
     def decode(self, encoded: str) -> dict[str, str | None]: ...
 
 class UnsaltedMD5PasswordHasher(BasePasswordHasher):
     def decode(self, encoded: str) -> dict[str, str | None]: ...
-
-class CryptPasswordHasher(BasePasswordHasher): ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/middleware.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/middleware.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.http.request import HttpRequest
 from django.utils.deprecation import MiddlewareMixin
 
 def get_user(request: HttpRequest) -> AnonymousUser | AbstractBaseUser: ...
+async def auser(request: HttpRequest) -> AnonymousUser | AbstractBaseUser: ...
 
 class AuthenticationMiddleware(MiddlewareMixin):
     def process_request(self, request: HttpRequest) -> None: ...
 
 class RemoteUserMiddleware(MiddlewareMixin):
     header: str
     force_logout_if_no_header: bool
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/mixins.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/models.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/models.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -57,16 +57,14 @@
     ) -> QuerySet[_T]: ...
 
 class PermissionsMixin(models.Model):
     is_superuser = models.BooleanField()
     groups = models.ManyToManyField(Group)
     user_permissions = models.ManyToManyField(Permission)
 
-    class Meta:
-        abstract: Literal[True]
     def get_user_permissions(self, obj: _AnyUser | None = ...) -> set[str]: ...
     def get_group_permissions(self, obj: _AnyUser | None = ...) -> set[str]: ...
     def get_all_permissions(self, obj: _AnyUser | None = ...) -> set[str]: ...
     def has_perm(self, perm: str, obj: _AnyUser | None = ...) -> bool: ...
     def has_perms(self, perm_list: Iterable[str], obj: _AnyUser | None = ...) -> bool: ...
     def has_module_perms(self, app_label: str) -> bool: ...
 
@@ -82,16 +80,14 @@
     date_joined = models.DateTimeField()
 
     objects: ClassVar[UserManager[Self]]
 
     EMAIL_FIELD: str
     USERNAME_FIELD: str
 
-    class Meta:
-        abstract: Literal[True]
     def get_full_name(self) -> str: ...
     def get_short_name(self) -> str: ...
     def email_user(
         self, subject: _StrOrPromise, message: _StrOrPromise, from_email: str = ..., **kwargs: Any
     ) -> None: ...
 
 class User(AbstractUser): ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/password_validation.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/password_validation.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from collections.abc import Mapping, Sequence
 from pathlib import Path, PosixPath
-from typing import Any, Protocol
+from typing import Any, Protocol, type_check_only
 
 from django.db.models.base import Model
 from typing_extensions import TypeAlias
 
 _UserModel: TypeAlias = Model
 
+@type_check_only
 class PasswordValidator(Protocol):
-    def validate(self, __password: str, __user: _UserModel | None = ...) -> None: ...
+    def validate(self, password: str, user: _UserModel | None = ..., /) -> None: ...
     def get_help_text(self) -> str: ...
 
 def get_default_password_validators() -> list[PasswordValidator]: ...
 def get_password_validators(validator_config: Sequence[Mapping[str, Any]]) -> list[PasswordValidator]: ...
 def validate_password(
     password: str, user: _UserModel | None = ..., password_validators: Sequence[PasswordValidator] | None = ...
 ) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/tokens.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/tokens.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/auth/views.pyi` & `django_stubs-5.0.0/django-stubs/contrib/auth/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/contenttypes/admin.pyi` & `django_stubs-5.0.0/django-stubs/contrib/contenttypes/admin.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/contenttypes/fields.pyi` & `django_stubs-5.0.0/django-stubs/contrib/contenttypes/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/contenttypes/forms.pyi` & `django_stubs-5.0.0/django-stubs/contrib/contenttypes/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/contenttypes/management/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/contenttypes/models.pyi` & `django_stubs-5.0.0/django-stubs/contrib/contenttypes/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/admin/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/admin/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,11 +4,9 @@
 from django.contrib.admin import ModelAdmin as ModelAdmin
 from django.contrib.admin import StackedInline as StackedInline
 from django.contrib.admin import TabularInline as TabularInline
 from django.contrib.admin import action as action
 from django.contrib.admin import autodiscover as autodiscover
 from django.contrib.admin import register as register
 from django.contrib.admin import site as site
-from django.contrib.gis.admin.options import GeoModelAdmin as GeoModelAdmin
 from django.contrib.gis.admin.options import GISModelAdmin as GISModelAdmin
-from django.contrib.gis.admin.options import OSMGeoAdmin as OSMGeoAdmin
 from django.contrib.gis.admin.widgets import OpenLayersWidget as OpenLayersWidget
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/features.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/models.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/base/operations.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/features.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/operations.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/mysql/schema.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/models.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/models.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 from typing import Any, ClassVar
 
-from django.contrib.gis.db import models
 from django.contrib.gis.db.backends.base.models import SpatialRefSysMixin
-from django.db.models.manager import Manager
+from django.db import models
 from typing_extensions import Self
 
-class OracleGeometryColumns(models.Model):
-    table_name: Any
-    column_name: Any
+class SpatialiteGeometryColumns(models.Model):
+    f_table_name: Any
+    f_geometry_column: Any
+    coord_dimension: Any
     srid: Any
-    objects: ClassVar[Manager[Self]]
+    spatial_index_enabled: Any
+    type: Any
+    objects: ClassVar[models.Manager[Self]]
 
-    class Meta:
-        app_label: str
-        db_table: str
-        managed: bool
     @classmethod
     def table_name_col(cls) -> Any: ...
     @classmethod
     def geom_col_name(cls) -> Any: ...
 
-class OracleSpatialRefSys(models.Model, SpatialRefSysMixin):
-    cs_name: Any
+class SpatialiteSpatialRefSys(models.Model, SpatialRefSysMixin):
     srid: Any
-    auth_srid: Any
     auth_name: Any
-    wktext: Any
-    cs_bounds: Any
-    objects: ClassVar[Manager[Self]]
+    auth_srid: Any
+    ref_sys_name: Any
+    proj4text: Any
+    srtext: Any
+    objects: ClassVar[models.Manager[Self]]
 
-    class Meta:
-        app_label: str
-        db_table: str
-        managed: bool
     @property
     def wkt(self) -> Any: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/operations.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/oracle/schema.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/postgis/operations.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/base.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/models.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/models.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 from typing import Any, ClassVar
 
 from django.contrib.gis.db.backends.base.models import SpatialRefSysMixin
 from django.db import models
 from typing_extensions import Self
 
-class SpatialiteGeometryColumns(models.Model):
+class PostGISGeometryColumns(models.Model):
+    f_table_catalog: Any
+    f_table_schema: Any
     f_table_name: Any
     f_geometry_column: Any
     coord_dimension: Any
     srid: Any
-    spatial_index_enabled: Any
     type: Any
     objects: ClassVar[models.Manager[Self]]
 
-    class Meta:
-        app_label: str
-        db_table: str
-        managed: bool
     @classmethod
     def table_name_col(cls) -> Any: ...
     @classmethod
     def geom_col_name(cls) -> Any: ...
 
-class SpatialiteSpatialRefSys(models.Model, SpatialRefSysMixin):
+class PostGISSpatialRefSys(models.Model, SpatialRefSysMixin):
     srid: Any
     auth_name: Any
     auth_srid: Any
-    ref_sys_name: Any
-    proj4text: Any
     srtext: Any
+    proj4text: Any
     objects: ClassVar[models.Manager[Self]]
 
-    class Meta:
-        app_label: str
-        db_table: str
-        managed: bool
     @property
     def wkt(self) -> Any: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/backends/utils.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/models/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/models/aggregates.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/models/fields.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/fields.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,17 @@
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
     Polygon,
 )
 from django.core.validators import _ValidatorCallable
-from django.db.models.expressions import Combinable
-from django.db.models.fields import Field, _ErrorMessagesMapping, _FieldChoices
+from django.db.models.expressions import Combinable, Expression
+from django.db.models.fields import NOT_PROVIDED, Field, _ErrorMessagesMapping
+from django.utils.choices import _Choices
 from django.utils.functional import _StrOrPromise
 
 # __set__ value type
 _ST = TypeVar("_ST")
 # __get__ return type
 _GT = TypeVar("_GT")
 
@@ -47,23 +48,25 @@
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[_ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
     def db_type(self, connection: Any) -> Any: ...
     def spheroid(self, connection: Any) -> Any: ...
     def units(self, connection: Any) -> Any: ...
@@ -91,23 +94,25 @@
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[_ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
     def formfield(  # type: ignore[override]
         self,
         *,
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/models/functions.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/functions.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,18 @@
 class BoundingCircle(OracleToleranceMixin, GeomOutputGeoFunc):
     def __init__(self, expression: Any, num_seg: int = ..., **extra: Any) -> None: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Centroid(OracleToleranceMixin, GeomOutputGeoFunc):
     arity: int
 
+class ClosestPoint(GeomOutputGeoFunc):
+    arity: int
+    geom_param_pos: tuple[int, int]
+
 class Difference(OracleToleranceMixin, GeomOutputGeoFunc):
     arity: int
     geom_param_pos: Any
 
 class DistanceResultMixin:
     @cached_property
     def output_field(self) -> DistanceField: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/models/lookups.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/db/models/sql/conversion.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/sql/conversion.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/feeds.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/feeds.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/forms/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/forms/fields.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/forms/widgets.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/forms/widgets.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 class OpenLayersWidget(BaseGeometryWidget):
     template_name: str
     map_srid: int
 
     class Media:
         css: Any
         js: Any
+
     def serialize(self, value: Any) -> Any: ...
     def deserialize(self, value: Any) -> Any: ...
 
 class OSMWidget(OpenLayersWidget):
     template_name: str
     default_lon: int
     default_lat: int
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/datasource.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/datasource.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/envelope.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/envelope.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/feature.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/feature.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/field.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/field.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/geometries.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/geometries.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/layer.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/layer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/libgdal.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/libgdal.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/ds.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/ds.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/generation.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/generation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/geom.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/raster.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/raster.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/prototypes/srs.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/srs.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/raster/band.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/band.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/raster/source.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/source.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/gdal/srs.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/srs.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geoip2/base.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/collections.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/collections.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/coordseq.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/geometry.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/geometry.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def valid_reason(self) -> str: ...
     def contains(self, other: GEOSGeometry) -> bool: ...
     def covers(self, other: GEOSGeometry) -> bool: ...
     def crosses(self, other: GEOSGeometry) -> bool: ...
     def disjoint(self, other: GEOSGeometry) -> bool: ...
     def equals(self, other: GEOSGeometry) -> bool: ...
     def equals_exact(self, other: GEOSGeometry, tolerance: float = ...) -> bool: ...
+    def equals_identical(self, other: GEOSGeometry) -> bool: ...
     def intersects(self, other: GEOSGeometry) -> bool: ...
     def overlaps(self, other: GEOSGeometry) -> bool: ...
     def relate_pattern(self, other: GEOSGeometry, pattern: str) -> bool: ...
     def touches(self, other: GEOSGeometry) -> bool: ...
     def within(self, other: GEOSGeometry) -> bool: ...
     @property
     def srid(self) -> int | None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/libgeos.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/libgeos.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/linestring.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/linestring.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/mutable_list.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/mutable_list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/point.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/point.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/polygon.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/polygon.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/prepared.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prepared.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/geom.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/io.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/io.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     def read(self, wkt: Any) -> Any: ...
 
 class _WKBReader(IOBase):
     ptr_type: Any
     destructor: Any
     def read(self, wkb: Any) -> Any: ...
 
+def default_trim_value() -> bool: ...
+
 class WKTWriter(IOBase):
     ptr_type: Any
     destructor: Any
     def __init__(self, dim: int = ..., trim: bool = ..., precision: Any | None = ...) -> None: ...
     def write(self, geom: Any) -> Any: ...
     @property
     def outdim(self) -> Any: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/geos/prototypes/topology.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/topology.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/measure.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/measure.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/gis/utils/layermapping.pyi` & `django_stubs-5.0.0/django-stubs/contrib/gis/utils/layermapping.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from collections.abc import Mapping
 from pathlib import Path
-from typing import Any, Protocol
+from typing import Any, Protocol, type_check_only
 
 from django.contrib.gis.gdal import DataSource, OGRGeomType
 from django.contrib.gis.gdal.field import Field as OGRField
 from django.contrib.gis.gdal.layer import Layer
 from django.db.backends.base.operations import BaseDatabaseOperations
 from django.db.models import Field, Model
 
 class LayerMapError(Exception): ...
 class InvalidString(LayerMapError): ...
 class InvalidDecimal(LayerMapError): ...
 class InvalidInteger(LayerMapError): ...
 class MissingForeignKey(LayerMapError): ...
 
+@type_check_only
 class _Writer(Protocol):
-    def write(self, __s: str) -> Any: ...
+    def write(self, s: str, /) -> Any: ...
 
 class LayerMapping:
     MULTI_TYPES: dict[int, OGRGeomType]
     FIELD_TYPES: dict[Field, OGRField | tuple[OGRField, ...]]
     ds: DataSource
     layer: Layer
     using: str
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/humanize/templatetags/humanize.pyi` & `django_stubs-5.0.0/django-stubs/contrib/humanize/templatetags/humanize.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/messages/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/messages/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -11,9 +11,7 @@
 from .constants import DEBUG as DEBUG
 from .constants import DEFAULT_LEVELS as DEFAULT_LEVELS
 from .constants import DEFAULT_TAGS as DEFAULT_TAGS
 from .constants import ERROR as ERROR
 from .constants import INFO as INFO
 from .constants import SUCCESS as SUCCESS
 from .constants import WARNING as WARNING
-
-default_app_config: str
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/messages/api.pyi` & `django_stubs-5.0.0/django-stubs/contrib/messages/api.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/messages/storage/base.pyi` & `django_stubs-5.0.0/django-stubs/contrib/messages/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/aggregates/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/__init__.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .general import ArrayAgg as ArrayAgg
 from .general import BitAnd as BitAnd
 from .general import BitOr as BitOr
+from .general import BitXor as BitXor
 from .general import BoolAnd as BoolAnd
 from .general import BoolOr as BoolOr
 from .general import JSONBAgg as JSONBAgg
 from .general import StringAgg as StringAgg
 from .statistics import Corr as Corr
 from .statistics import CovarPop as CovarPop
 from .statistics import RegrAvgX as RegrAvgX
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/constraints.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/base/client.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-from collections.abc import Sequence
+from collections.abc import Iterable, Sequence
+from typing import Any
 
-from django.db.models import Deferrable
-from django.db.models.constraints import BaseConstraint
-from django.db.models.expressions import Combinable
-from django.db.models.query_utils import Q
-from django.utils.functional import _StrOrPromise
+from django.db.backends.base.base import BaseDatabaseWrapper
 
-class ExclusionConstraint(BaseConstraint):
-    expressions: Sequence[tuple[str | Combinable, str]]
-    index_type: str
-    condition: Q | None
-    def __init__(
-        self,
-        *,
-        name: str,
-        expressions: Sequence[tuple[str | Combinable, str]],
-        index_type: str | None = ...,
-        condition: Q | None = ...,
-        deferrable: Deferrable | None = ...,
-        include: list[str] | tuple[str] | None = ...,
-        opclasses: list[str] | tuple[str] = ...,
-        violation_error_message: _StrOrPromise | None = ...,
-    ) -> None: ...
+class BaseDatabaseClient:
+    executable_name: str | None
+    connection: BaseDatabaseWrapper
+    def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
+    @classmethod
+    def settings_to_cmd_args_env(
+        cls,
+        settings_dict: dict[str, Any],
+        parameters: Iterable[str],
+    ) -> tuple[Sequence[str], dict[str, str] | None]: ...
+    def runshell(self, parameters: Iterable[str]) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/fields/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/fields/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/fields/array.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/generated.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,48 @@
-from collections.abc import Iterable, Sequence
-from typing import Any, TypeVar
+from typing import Any, Iterable, Literal
 
 from django.core.validators import _ValidatorCallable
-from django.db.models import Field, Transform
-from django.db.models.expressions import Combinable
-from django.db.models.fields import _ErrorMessagesDict, _ErrorMessagesMapping, _FieldChoices
-from django.db.models.fields.mixins import CheckFieldDefaultMixin
+from django.db import models
+from django.db.backends.base.base import BaseDatabaseWrapper
+from django.db.models.expressions import Expression
+from django.db.models.fields import _ErrorMessagesMapping
+from django.db.models.sql import Query
+from django.utils.choices import _Choices
+from django.utils.datastructures import DictWrapper
 from django.utils.functional import _StrOrPromise
 
-# __set__ value type
-_ST = TypeVar("_ST")
-# __get__ return type
-_GT = TypeVar("_GT")
+class GeneratedField(models.Field):
+    generated: Literal[True]
+    db_returning: Literal[True]
+    _query: Query | None
+    output_field: models.Field | None
 
-class ArrayField(CheckFieldDefaultMixin, Field[_ST, _GT]):
-    _pyi_private_set_type: Sequence[Any] | Combinable
-    _pyi_private_get_type: list[Any]
-
-    empty_strings_allowed: bool
-    default_error_messages: _ErrorMessagesDict
-    base_field: Field
-    size: int | None
-    default_validators: Sequence[_ValidatorCallable]
-    from_db_value: Any
     def __init__(
         self,
-        base_field: Field,
-        size: int | None = ...,
         *,
+        expression: Expression,
+        output_field: models.Field,
+        db_persist: bool | None = ...,
         verbose_name: _StrOrPromise | None = ...,
         name: str | None = ...,
         primary_key: bool = ...,
-        max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
-        db_index: bool = ...,
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[_ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
+        **kwargs: Any,
     ) -> None: ...
-    @property
-    def description(self) -> str: ...  # type: ignore[override]
-    def get_transform(self, name: Any) -> type[Transform] | None: ...
+    def generated_sql(self, connection: BaseDatabaseWrapper) -> tuple[str, Any]: ...
+    def db_type_parameters(self, connection: BaseDatabaseWrapper) -> DictWrapper: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/fields/ranges.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/fields/ranges.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from typing import Any, ClassVar, Literal
+from typing import Any, ClassVar, Literal, TypeVar
 
+from _typeshed import Unused
+from django.contrib.postgres import forms
 from django.db import models
+from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.lookups import PostgresOperatorLookup
-from psycopg2.extras import DateRange, DateTimeTZRange, NumericRange, Range
+from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
+from psycopg2.extras import DateRange, DateTimeTZRange, NumericRange, Range  # type: ignore [import-untyped]
 
 class RangeBoundary(models.Expression):
     lower: str
     upper: str
     def __init__(self, inclusive_lower: bool = ..., inclusive_upper: bool = ...) -> None: ...
 
 class RangeOperators:
@@ -17,40 +21,49 @@
     OVERLAPS: Literal["&&"]
     FULLY_LT: Literal["<<"]
     FULLY_GT: Literal[">>"]
     NOT_LT: Literal["&>"]
     NOT_GT: Literal["&<"]
     ADJACENT_TO: Literal["-|-"]
 
-class RangeField(models.Field):
+_RangeT = TypeVar("_RangeT", bound=Range[Any])
+
+class RangeField(models.Field[Any, _RangeT]):
     empty_strings_allowed: bool
-    base_field: models.Field
-    range_type: type[Range]
+    base_field: type[models.Field]
+    range_type: type[_RangeT]
     def get_prep_value(self, value: Any) -> Any | None: ...
+    def get_placeholder(self, value: Unused, compiler: Unused, connection: BaseDatabaseWrapper) -> str: ...
     def to_python(self, value: Any) -> Any: ...
 
-class IntegerRangeField(RangeField):
-    def __get__(self, instance: Any, owner: Any) -> NumericRange: ...
-
-class BigIntegerRangeField(RangeField):
-    def __get__(self, instance: Any, owner: Any) -> NumericRange: ...
-
-class DecimalRangeField(RangeField):
-    def __get__(self, instance: Any, owner: Any) -> NumericRange: ...
-
-class DateTimeRangeField(RangeField):
-    def __get__(self, instance: Any, owner: Any) -> DateTimeTZRange: ...
-
-class DateRangeField(RangeField):
-    def __get__(self, instance: Any, owner: Any) -> DateRange: ...
+class IntegerRangeField(RangeField[NumericRange]):
+    base_field: type[models.IntegerField]
+    form_field: type[forms.IntegerRangeField]
+
+class BigIntegerRangeField(RangeField[NumericRange]):
+    base_field: type[models.BigIntegerField]
+    form_field: type[forms.IntegerRangeField]
+
+class DecimalRangeField(RangeField[NumericRange]):
+    base_field: type[models.DecimalField]
+    form_field: type[forms.DecimalRangeField]
+
+class DateTimeRangeField(RangeField[DateTimeTZRange]):
+    base_field: type[models.DecimalField]
+    form_field: type[forms.DecimalRangeField]
+
+class DateRangeField(RangeField[DateRange]):
+    base_field: type[models.DateField]
+    form_field: type[forms.DateRangeField]
 
 class DateTimeRangeContains(PostgresOperatorLookup): ...
 
 class RangeContainedBy(PostgresOperatorLookup):
     type_mapping: dict[str, str]
+    def process_lhs(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...  # type: ignore[override]
 
 class FullyLessThan(PostgresOperatorLookup): ...
 class FullGreaterThan(PostgresOperatorLookup): ...
 class NotLessThan(PostgresOperatorLookup): ...
 class NotGreaterThan(PostgresOperatorLookup): ...
 class AdjacentToLookup(PostgresOperatorLookup): ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/forms/array.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/forms/array.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/forms/ranges.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/forms/ranges.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 
 from django import forms
 from django.db.models.fields import _ErrorMessagesDict
 from django.forms.widgets import MultiWidget, _OptAttrs
-from psycopg2.extras import Range
+from psycopg2.extras import Range  # type: ignore [import-untyped]
 
 class RangeWidget(MultiWidget):
     def __init__(self, base_widget: forms.Widget | type[forms.Widget], attrs: _OptAttrs | None = ...) -> None: ...
     def decompress(self, value: Any) -> tuple[Any | None, Any | None]: ...
 
 class HiddenRangeWidget(RangeWidget):
     def __init__(self, attrs: _OptAttrs | None = ...) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/indexes.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/operations.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/search.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/search.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from typing import Any, ClassVar
 
+from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Expression, Field, FloatField, TextField
 from django.db.models.expressions import Combinable, CombinedExpression, Func
 from django.db.models.lookups import Lookup
+from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 from typing_extensions import Self, TypeAlias
 
 _Expression: TypeAlias = str | Combinable | SearchQueryCombinable
 
-class SearchVectorExact(Lookup): ...
+class SearchVectorExact(Lookup):
+    def process_rhs(self, qn: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
+    def as_sql(self, qn: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
+
 class SearchVectorField(Field): ...
 class SearchQueryField(Field): ...
 
 class SearchConfig(Expression):
     config: _Expression | None
     def __init__(self, config: _Expression) -> None: ...
     @classmethod
@@ -24,14 +29,21 @@
     config: _Expression | None
     function: str
     arg_joiner: str
     output_field: ClassVar[SearchVectorField]
     def __init__(
         self, *expressions: _Expression, config: _Expression | None = ..., weight: Any | None = ...
     ) -> None: ...
+    def as_sql(  # type: ignore[override]
+        self,
+        compiler: SQLCompiler,
+        connection: BaseDatabaseWrapper,
+        function: str | None = ...,
+        template: str | None = ...,
+    ) -> _AsSqlType: ...
 
 class CombinedSearchVector(SearchVectorCombinable, CombinedExpression):
     def __init__(
         self,
         lhs: Combinable,
         connector: str,
         rhs: Combinable,
@@ -55,14 +67,21 @@
         value: _Expression,
         output_field: Field | None = ...,
         *,
         config: _Expression | None = ...,
         invert: bool = ...,
         search_type: str = ...,
     ) -> None: ...
+    def as_sql(  # type: ignore[override]
+        self,
+        compiler: SQLCompiler,
+        connection: BaseDatabaseWrapper,
+        function: str | None = ...,
+        template: str | None = ...,
+    ) -> _AsSqlType: ...
     def __invert__(self) -> Self: ...  # type: ignore[override]
 
 class CombinedSearchQuery(SearchQueryCombinable, CombinedExpression):  # type: ignore[misc]
     def __init__(
         self,
         lhs: Combinable,
         connector: str,
@@ -97,14 +116,21 @@
         max_words: int | None = ...,
         min_words: int | None = ...,
         short_word: str | None = ...,
         highlight_all: bool | None = ...,
         max_fragments: int | None = ...,
         fragment_delimiter: str | None = ...,
     ) -> None: ...
+    def as_sql(  # type: ignore[override]
+        self,
+        compiler: SQLCompiler,
+        connection: BaseDatabaseWrapper,
+        function: str | None = ...,
+        template: str | None = ...,
+    ) -> _AsSqlType: ...
 
 class TrigramBase(Func):
     output_field: ClassVar[FloatField]
     def __init__(self, expression: _Expression, string: str, **extra: Any) -> None: ...
 
 class TrigramWordBase(Func):
     output_field: ClassVar[FloatField]
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/postgres/validators.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/validators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/sessions/backends/base.pyi` & `django_stubs-5.0.0/django-stubs/contrib/sessions/backends/base.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import Any
 
 VALID_KEY_CHARS: Any
 
 class CreateError(Exception): ...
 class UpdateError(Exception): ...
 
@@ -33,15 +33,15 @@
     @property
     def _session_key(self) -> str | None: ...
     @_session_key.setter
     def _session_key(self, value: str | None) -> None: ...
     def get_session_cookie_age(self) -> int: ...
     def get_expiry_age(self, **kwargs: Any) -> int: ...
     def get_expiry_date(self, **kwargs: Any) -> datetime: ...
-    def set_expiry(self, value: datetime | int | None) -> None: ...
+    def set_expiry(self, value: datetime | timedelta | int | None) -> None: ...
     def get_expire_at_browser_close(self) -> bool: ...
     def flush(self) -> None: ...
     def cycle_key(self) -> None: ...
     def exists(self, session_key: str) -> bool: ...
     def create(self) -> None: ...
     def save(self, must_create: bool = ...) -> None: ...
     def delete(self, session_key: str | None = ...) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/sessions/backends/db.pyi` & `django_stubs-5.0.0/django-stubs/contrib/sessions/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/sessions/base_session.pyi` & `django_stubs-5.0.0/django-stubs/contrib/sessions/base_session.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, Literal, TypeVar
+from typing import Any, TypeVar
 
 from django.contrib.sessions.backends.base import SessionBase
 from django.db import models
 
 _T = TypeVar("_T", bound=AbstractBaseSession)
 
 class BaseSessionManager(models.Manager[_T]):
@@ -12,12 +12,10 @@
 
 class AbstractBaseSession(models.Model):
     expire_date: datetime
     session_data: str
     session_key: str
     objects: Any
 
-    class Meta:
-        abstract: Literal[True]
     @classmethod
     def get_session_store_class(cls) -> type[SessionBase] | None: ...
     def get_decoded(self) -> dict[str, Any]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/sitemaps/__init__.pyi` & `django_stubs-5.0.0/django-stubs/contrib/sitemaps/__init__.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 
 from django.contrib.sites.models import Site
 from django.contrib.sites.requests import RequestSite
 from django.core.paginator import Paginator
 from django.db.models.base import Model
 from django.db.models.query import QuerySet
 
-PING_URL: str
-
-class SitemapNotFound(Exception): ...
-
-def ping_google(sitemap_url: str | None = ..., ping_url: str = ..., sitemap_uses_https: bool = ...) -> None: ...
-
 _ItemT = TypeVar("_ItemT")
 
 class Sitemap(Generic[_ItemT]):
     limit: int
     protocol: str | None
     i18n: bool
     languages: Sequence[str] | None
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/sitemaps/views.pyi` & `django_stubs-5.0.0/django-stubs/contrib/sitemaps/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/sites/models.pyi` & `django_stubs-5.0.0/django-stubs/contrib/sites/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/staticfiles/finders.pyi` & `django_stubs-5.0.0/django-stubs/contrib/staticfiles/finders.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     @overload
     def find(self, path: str, all: Literal[True]) -> list[str]: ...
     def list(self, ignore_patterns: Iterable[str] | None) -> Iterable[Any]: ...
 
 class FileSystemFinder(BaseFinder):
     locations: list[tuple[str, str]]
     storages: dict[str, Any]
-    def __init__(self, app_names: Sequence[str] = ..., *args: Any, **kwargs: Any) -> None: ...
+    def __init__(self, app_names: Sequence[str] | None = ..., *args: Any, **kwargs: Any) -> None: ...
     def find_location(self, root: str, path: str, prefix: str | None = ...) -> str | None: ...
     @overload
     def find(self, path: str, all: Literal[False] = ...) -> str | None: ...
     @overload
     def find(self, path: str, all: Literal[True]) -> list[str]: ...
     def list(self, ignore_patterns: Iterable[str] | None) -> Iterable[Any]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/staticfiles/handlers.pyi` & `django_stubs-5.0.0/django-stubs/contrib/staticfiles/handlers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi` & `django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from typing import Any
 
 from django.core.files.storage import Storage
 from django.core.management.base import BaseCommand
+from django.utils.functional import cached_property
 
 class Command(BaseCommand):
     copied_files: Any
     symlinked_files: Any
     unmodified_files: Any
     post_processed_files: Any
     storage: Any
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
-    @property
+    @cached_property
     def local(self) -> bool: ...
     interactive: Any
     verbosity: Any
     symlink: Any
     clear: Any
     dry_run: Any
     ignore_patterns: Any
     post_process: Any
     def set_options(self, **options: Any) -> None: ...
     def collect(self) -> dict[str, list[str]]: ...
+    def handle(self, **options: Any) -> str | None: ...
     def log(self, msg: str, level: int = ...) -> None: ...
     def is_local_storage(self) -> bool: ...
     def clear_dir(self, path: str) -> None: ...
     def delete_file(self, path: str, prefixed_path: str, source_storage: Storage) -> bool: ...
     def link_file(self, path: str, prefixed_path: str, source_storage: Storage) -> None: ...
     def copy_file(self, path: str, prefixed_path: str, source_storage: Storage) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/staticfiles/storage.pyi` & `django_stubs-5.0.0/django-stubs/contrib/staticfiles/storage.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import Callable, Iterator
+from re import Match
 from typing import Any
 
 from django.core.files.base import File
 from django.core.files.storage import FileSystemStorage, Storage
 from django.utils._os import _PathCompatible
 from django.utils.functional import LazyObject
 from typing_extensions import TypeAlias
@@ -19,32 +20,34 @@
     default_template: str
     max_post_process_passes: int
     support_js_module_import_aggregation: bool
     patterns: Any
     hashed_files: Any
     keep_intermediate_files: bool
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
-    def file_hash(self, name: str, content: File = ...) -> str: ...
+    def file_hash(self, name: str, content: File | None = ...) -> str | None: ...
     def hashed_name(self, name: str, content: File | None = ..., filename: str | None = ...) -> str: ...
     def url(self, name: str, force: bool = ...) -> str: ...
-    def url_converter(self, name: str, hashed_files: dict[str, Any], template: str = ...) -> Callable: ...
+    def url_converter(
+        self, name: str, hashed_files: dict[str, Any], template: str | None = ...
+    ) -> Callable[[Match], str]: ...
     def post_process(self, paths: dict[str, Any], dry_run: bool = ..., **options: Any) -> _PostProcessT: ...
     def clean_name(self, name: str) -> str: ...
     def hash_key(self, name: str) -> str: ...
     def stored_name(self, name: str) -> str: ...
 
 class ManifestFilesMixin(HashedFilesMixin):
     manifest_version: str
     manifest_name: str
     manifest_strict: bool
     keep_intermediate_files: bool
     manifest_storage: Storage | None
     hashed_files: dict[str, str]
     manifest_hash: str
-    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
+    def __init__(self, *args: Any, manifest_storage: Storage | None = ..., **kwargs: Any) -> None: ...
     def read_manifest(self) -> str: ...
     def load_manifest(self) -> dict[str, Any]: ...
     def save_manifest(self) -> None: ...
     def post_process(self, *args: Any, **kwargs: Any) -> _PostProcessT: ...
     def stored_name(self, name: str) -> str: ...
 
 class ManifestStaticFilesStorage(ManifestFilesMixin, StaticFilesStorage): ...  # type: ignore[misc]
```

### Comparing `django-stubs-4.2.7/django-stubs/contrib/syndication/views.pyi` & `django_stubs-5.0.0/django-stubs/contrib/syndication/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/cache/__init__.pyi` & `django_stubs-5.0.0/django-stubs/core/cache/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .backends.base import BaseCache as BaseCache
 from .backends.base import CacheKeyWarning as CacheKeyWarning
 from .backends.base import InvalidCacheBackendError as InvalidCacheBackendError
 from .backends.base import InvalidCacheKey as InvalidCacheKey
 
 DEFAULT_CACHE_ALIAS: str
 
-class CacheHandler(BaseConnectionHandler):
+class CacheHandler(BaseConnectionHandler[BaseCache]):
     settings_name: str
     exception_class: type[Exception]
     def create_connection(self, alias: str) -> BaseCache: ...
     def all(self, initialized_only: bool = ...) -> list[BaseCache]: ...
 
 def close_caches(**kwargs: Any) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/cache/backends/base.pyi` & `django_stubs-5.0.0/django-stubs/core/cache/backends/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import Callable, Iterable, Iterator
+from re import Pattern
 from typing import Any
 
 from django.core.exceptions import ImproperlyConfigured
 
 class InvalidCacheBackendError(ImproperlyConfigured): ...
 class CacheKeyWarning(RuntimeWarning): ...
 class InvalidCacheKey(ValueError): ...
@@ -62,8 +63,10 @@
     def incr_version(self, key: Any, delta: int = ..., version: int | None = ...) -> int: ...
     async def aincr_version(self, key: Any, delta: int = ..., version: int | None = ...) -> int: ...
     def decr_version(self, key: Any, delta: int = ..., version: int | None = ...) -> int: ...
     async def adecr_version(self, key: Any, delta: int = ..., version: int | None = ...) -> int: ...
     def close(self, **kwargs: Any) -> None: ...
     async def aclose(self, **kwargs: Any) -> None: ...
 
+memcached_error_chars_re: Pattern[str]
+
 def memcache_key_warnings(key: str) -> Iterator[str]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/cache/backends/db.pyi` & `django_stubs-5.0.0/django-stubs/core/cache/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/cache/backends/memcached.pyi` & `django_stubs-5.0.0/django-stubs/core/cache/backends/memcached.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,14 @@
         params: dict[str, Any],
         library: ModuleType,
         value_not_found_exception: type[BaseException],
     ) -> None: ...
     @property
     def client_servers(self) -> Sequence[str]: ...
 
-class MemcachedCache(BaseMemcachedCache):
-    def __init__(self, server: str | Sequence[str], params: dict[str, Any]) -> None: ...
-
 class PyLibMCCache(BaseMemcachedCache):
     def __init__(self, server: str | Sequence[str], params: dict[str, Any]) -> None: ...
     @property
     def client_servers(self) -> list[str]: ...
 
 class PyMemcacheCache(BaseMemcachedCache):
     def __init__(self, server: str | Sequence[str], params: dict[str, Any]) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/__init__.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/caches.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/caches.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/messages.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/messages.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/registry.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/registry.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Callable, Iterable, Sequence
-from typing import Any, Protocol, TypeVar, overload
+from typing import Any, Protocol, TypeVar, overload, type_check_only
 
 from django.apps.config import AppConfig
 from django.core.checks.messages import CheckMessage
 
 class Tags:
     admin: str
     async_support: str
@@ -16,35 +16,37 @@
     signals: str
     sites: str
     staticfiles: str
     templates: str
     translation: str
     urls: str
 
+@type_check_only
 class _CheckCallable(Protocol):
     def __call__(
         self,
         *,
         app_configs: Sequence[AppConfig] | None,
         databases: Sequence[str] | None,
         **kwargs: Any,
     ) -> Iterable[CheckMessage]: ...
 
 _C = TypeVar("_C", bound=_CheckCallable)
 
+@type_check_only
 class _ProcessedCheckCallable(Protocol[_C]):
     tags: Sequence[str]
     __call__: _C
 
 class CheckRegistry:
     registered_checks: set[_ProcessedCheckCallable]
     deployment_checks: set[_ProcessedCheckCallable]
     def __init__(self) -> None: ...
     @overload
-    def register(self, __check: _C) -> _ProcessedCheckCallable[_C]: ...
+    def register(self, check: _C, /) -> _ProcessedCheckCallable[_C]: ...
     @overload
     def register(self, *tags: str, **kwargs: Any) -> Callable[[_C], _ProcessedCheckCallable[_C]]: ...
     def run_checks(
         self,
         app_configs: Sequence[AppConfig] | None = ...,
         tags: Sequence[str] | None = ...,
         include_deployment_checks: bool = ...,
```

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/security/base.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/security/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/security/csrf.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/security/csrf.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/security/sessions.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/security/sessions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/templates.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/templates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/translation.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/translation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/checks/urls.pyi` & `django_stubs-5.0.0/django-stubs/core/checks/urls.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/exceptions.pyi` & `django_stubs-5.0.0/django-stubs/core/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/files/base.pyi` & `django_stubs-5.0.0/django-stubs/template/loader_tags.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,68 @@
-from collections.abc import Iterator
-from types import TracebackType
-from typing import IO, AnyStr, type_check_only
-
-from django.core.files.utils import FileProxyMixin
-from django.utils.functional import cached_property
-from typing_extensions import Self
-
-class File(FileProxyMixin[AnyStr], IO[AnyStr]):
-    DEFAULT_CHUNK_SIZE: int
-    file: IO[AnyStr] | None
-    name: str | None
-    mode: str
-    def __init__(self, file: IO[AnyStr] | None, name: str | None = ...) -> None: ...
-    def __bool__(self) -> bool: ...
-    def __len__(self) -> int: ...
-    @cached_property
-    def size(self) -> int: ...
-    def chunks(self, chunk_size: int | None = ...) -> Iterator[AnyStr]: ...
-    def multiple_chunks(self, chunk_size: int | None = ...) -> bool | None: ...
-    def __iter__(self) -> Iterator[AnyStr]: ...
-    def __enter__(self) -> Self: ...
-    def __exit__(
+import collections
+from typing import Any
+
+from django.template.base import FilterExpression, NodeList, Origin, Parser, Token
+from django.template.context import Context
+from django.utils.safestring import SafeString
+
+from .base import Node, Template
+
+register: Any
+BLOCK_CONTEXT_KEY: str
+
+class BlockContext:
+    blocks: collections.defaultdict[str, list[BlockNode]]
+    def __init__(self) -> None: ...
+    def add_blocks(self, blocks: dict[str, BlockNode]) -> None: ...
+    def pop(self, name: str) -> BlockNode: ...
+    def push(self, name: str, block: BlockNode) -> None: ...
+    def get_block(self, name: str) -> BlockNode: ...
+
+class BlockNode(Node):
+    context: Context
+    name: str
+    nodelist: NodeList
+    origin: Origin
+    parent: Node | None
+    token: Token
+    def __init__(self, name: str, nodelist: NodeList, parent: Node | None = ...) -> None: ...
+    def render(self, context: Context) -> SafeString: ...
+    def super(self) -> SafeString: ...
+
+class ExtendsNode(Node):
+    origin: Origin
+    token: Token
+    must_be_first: bool
+    context_key: str
+    nodelist: NodeList
+    parent_name: FilterExpression | Node
+    template_dirs: list[Any] | None
+    blocks: dict[str, BlockNode]
+    def __init__(
+        self, nodelist: NodeList, parent_name: FilterExpression | Node, template_dirs: list[Any] | None = ...
+    ) -> None: ...
+    def find_template(self, template_name: str, context: Context) -> Template: ...
+    def get_parent(self, context: Context) -> Template: ...
+    def render(self, context: Context) -> Any: ...
+
+class IncludeNode(Node):
+    origin: Origin
+    token: Token
+    context_key: str
+    template: FilterExpression
+    extra_context: dict[str, FilterExpression]
+    isolated_context: bool
+    def __init__(
         self,
-        exc_type: type[BaseException] | None,
-        exc_value: BaseException | None,
-        exc_tb: TracebackType | None,
+        template: FilterExpression,
+        *args: Any,
+        extra_context: Any | None = ...,
+        isolated_context: bool = ...,
+        **kwargs: Any,
     ) -> None: ...
-    def open(self, mode: str | None = ...) -> Self: ...
-    def close(self) -> None: ...
-    @type_check_only
-    def __next__(self) -> AnyStr: ...
-
-class ContentFile(File[AnyStr]):
-    file: IO[AnyStr]
-    def __init__(self, content: AnyStr, name: str | None = ...) -> None: ...
-    def __bool__(self) -> bool: ...
-    def open(self, mode: str | None = ...) -> Self: ...
-    def close(self) -> None: ...
-    def write(self, data: AnyStr) -> int: ...
-
-def endswith_cr(line: bytes | str) -> bool: ...
-def endswith_lf(line: bytes | str) -> bool: ...
-def equals_lf(line: bytes | str) -> bool: ...
+    def render(self, context: Context) -> SafeString: ...
+
+def do_block(parser: Parser, token: Token) -> BlockNode: ...
+def construct_relative_path(current_template_name: str | None, relative_name: str) -> str: ...
+def do_extends(parser: Parser, token: Token) -> ExtendsNode: ...
+def do_include(parser: Parser, token: Token) -> IncludeNode: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/files/storage/__init__.pyi` & `django_stubs-5.0.0/django-stubs/core/files/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/files/storage/base.pyi` & `django_stubs-5.0.0/django-stubs/core/files/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/files/storage/filesystem.pyi` & `django_stubs-5.0.0/django-stubs/core/files/storage/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/files/storage/memory.pyi` & `django_stubs-5.0.0/django-stubs/core/files/storage/memory.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/files/uploadedfile.pyi` & `django_stubs-5.0.0/django-stubs/core/files/uploadedfile.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self,
         file: IO,
         field_name: str | None,
         name: str | None,
         content_type: str | None,
         size: int | None,
         charset: str | None,
-        content_type_extra: dict[str, str] = ...,
+        content_type_extra: dict[str, str] | None = ...,
     ) -> None: ...
+    def open(self, mode: str | None = ...) -> Self: ...  # type: ignore[override]
 
 class SimpleUploadedFile(InMemoryUploadedFile):
     def __init__(self, name: str, content: bytes | None, content_type: str = ...) -> None: ...
     @classmethod
     def from_dict(cls, file_dict: dict[str, str | bytes]) -> Self: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/files/uploadhandler.pyi` & `django_stubs-5.0.0/django-stubs/core/files/uploadhandler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/files/utils.pyi` & `django_stubs-5.0.0/django-stubs/core/files/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/handlers/asgi.pyi` & `django_stubs-5.0.0/django-stubs/core/handlers/asgi.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from collections.abc import Awaitable, Callable, Iterator, Mapping, Sequence
+from logging import Logger
 from typing import IO, Any, TypeVar
 
 from django.core.handlers import base
 from django.http.request import HttpRequest, _ImmutableQueryDict
 from django.http.response import HttpResponseBase
 from django.urls.resolvers import ResolverMatch, URLResolver
 from django.utils.datastructures import MultiValueDict
 from django.utils.functional import cached_property
 from typing_extensions import TypeAlias
 
 _ReceiveCallback: TypeAlias = Callable[[], Awaitable[Mapping[str, Any]]]
 
 _SendCallback: TypeAlias = Callable[[Mapping[str, Any]], Awaitable[None]]
 
+logger: Logger
+
+def get_script_prefix(scope: Mapping[str, Any]) -> str: ...
+
 class ASGIRequest(HttpRequest):
     body_receive_timeout: int
     scope: Mapping[str, Any]
     resolver_match: ResolverMatch | None
     script_name: str | None
     path_info: str
     path: str
@@ -38,18 +43,22 @@
     def __init__(self) -> None: ...
     async def __call__(
         self,
         scope: dict[str, Any],
         receive: _ReceiveCallback,
         send: _SendCallback,
     ) -> None: ...
+    async def handle(
+        self, scope: dict[str, Any], receive: _ReceiveCallback, send: _SendCallback
+    ) -> HttpResponseBase | None: ...
+    async def listen_for_disconnect(self, receive: _ReceiveCallback) -> None: ...
+    async def run_get_response(self, request: HttpRequest) -> HttpResponseBase: ...
     async def read_body(self, receive: _ReceiveCallback) -> IO[bytes]: ...
     def create_request(
         self, scope: Mapping[str, Any], body_file: IO[bytes]
     ) -> tuple[ASGIRequest, None] | tuple[None, HttpResponseBase]: ...
     def handle_uncaught_exception(
         self, request: HttpRequest, resolver: URLResolver, exc_info: Any
     ) -> HttpResponseBase: ...
     async def send_response(self, response: HttpResponseBase, send: _SendCallback) -> None: ...
     @classmethod
     def chunk_bytes(cls, data: Sequence[_T]) -> Iterator[tuple[Sequence[_T], bool]]: ...
-    def get_script_prefix(self, scope: Mapping[str, Any]) -> str: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/handlers/base.pyi` & `django_stubs-5.0.0/django-stubs/core/handlers/base.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from collections.abc import Awaitable, Callable
+from logging import Logger
 from typing import Any
 
+import _typeshed
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse, HttpResponseBase
 from django.urls.resolvers import ResolverMatch
 
+logger: Logger
+
 class BaseHandler:
     def load_middleware(self, is_async: bool = ...) -> None: ...
     def adapt_method_mode(
         self,
         is_async: bool,
         method: Callable[[HttpRequest], HttpResponseBase | Awaitable[HttpResponseBase]],
         method_is_async: bool | None = ...,
@@ -17,7 +21,9 @@
     ) -> Callable[[HttpRequest], HttpResponseBase | Awaitable[HttpResponseBase]]: ...
     def get_response(self, request: HttpRequest) -> HttpResponseBase: ...
     async def get_response_async(self, request: HttpRequest) -> HttpResponseBase: ...
     def resolve_request(self, request: HttpRequest) -> ResolverMatch: ...
     def check_response(self, response: HttpResponseBase, callback: Any, name: str | None = ...) -> None: ...
     def make_view_atomic(self, view: Callable[..., HttpResponseBase]) -> Callable[..., HttpResponseBase]: ...
     def process_exception_by_middleware(self, exception: Exception, request: HttpRequest) -> HttpResponse: ...
+
+def reset_urlconf(sender: _typeshed.Unused, **kwargs: Any) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/handlers/exception.pyi` & `django_stubs-5.0.0/django-stubs/core/handlers/exception.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/handlers/wsgi.pyi` & `django_stubs-5.0.0/django-stubs/core/handlers/wsgi.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 import sys
-from io import BytesIO
+from io import BytesIO, IOBase
 from typing import Any
 
-from django.contrib.sessions.backends.base import SessionBase
 from django.core.handlers import base
 from django.http import HttpRequest
 from django.http.response import HttpResponseBase
 
 if sys.version_info >= (3, 11):
     from wsgiref.types import StartResponse, WSGIEnvironment
 else:
     from _typeshed.wsgi import StartResponse, WSGIEnvironment
 
-class LimitedStream:
-    stream: BytesIO
-    remaining: int
-    buffer: bytes
-    buf_size: int
-    def __init__(self, stream: BytesIO, limit: int, buf_size: int = ...) -> None: ...
+class LimitedStream(IOBase):
+    limit: int
+    def __init__(self, stream: BytesIO, limit: int) -> None: ...
     def read(self, size: int | None = ...) -> bytes: ...
     def readline(self, size: int | None = ...) -> bytes: ...
 
 class WSGIRequest(HttpRequest):
     environ: WSGIEnvironment
-    session: SessionBase
-    encoding: Any
     def __init__(self, environ: WSGIEnvironment) -> None: ...
 
 class WSGIHandler(base.BaseHandler):
     request_class: type[WSGIRequest]
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def __call__(
         self,
```

### Comparing `django-stubs-4.2.7/django-stubs/core/mail/__init__.pyi` & `django_stubs-5.0.0/django-stubs/core/mail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/mail/backends/base.pyi` & `django_stubs-5.0.0/django-stubs/core/mail/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/mail/message.pyi` & `django_stubs-5.0.0/django-stubs/core/mail/message.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from collections.abc import Sequence
-from email import charset as Charset
-from email._policybase import Policy
 from email.message import Message
 from email.mime.base import MIMEBase
 from email.mime.message import MIMEMessage
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from typing import Any, overload
 
@@ -23,48 +21,30 @@
 def forbid_multi_line_headers(name: str, val: str, encoding: str) -> tuple[str, str]: ...
 def sanitize_address(addr: tuple[str, str] | str, encoding: str) -> str: ...
 
 class MIMEMixin:
     def as_string(self, unixfrom: bool = ..., linesep: str = ...) -> str: ...
     def as_bytes(self, unixfrom: bool = ..., linesep: str = ...) -> bytes: ...
 
-class SafeMIMEMessage(MIMEMixin, MIMEMessage):  # type: ignore[misc]
-    defects: list[Any]
-    epilogue: Any
-    policy: Policy
-    preamble: Any
-    def __setitem__(self, name: str, val: str) -> None: ...
+class SafeMIMEMessage(MIMEMixin, MIMEMessage): ...  # type: ignore[misc]
 
 class SafeMIMEText(MIMEMixin, MIMEText):  # type: ignore[misc]
-    defects: list[Any]
-    epilogue: None
-    policy: Policy
-    preamble: None
     encoding: str
     def __init__(self, _text: str, _subtype: str = ..., _charset: str = ...) -> None: ...
-    def __setitem__(self, name: str, val: str) -> None: ...
-    def set_payload(
-        self, payload: list[Message] | str | bytes, charset: str | Charset.Charset | None = ...
-    ) -> None: ...
 
 class SafeMIMEMultipart(MIMEMixin, MIMEMultipart):  # type: ignore[misc]
-    defects: list[Any]
-    epilogue: None
-    policy: Policy
-    preamble: None
     encoding: str
     def __init__(
         self,
         _subtype: str = ...,
         boundary: Any | None = ...,
         _subparts: Any | None = ...,
         encoding: str = ...,
         **_params: Any,
     ) -> None: ...
-    def __setitem__(self, name: str, val: str) -> None: ...
 
 _AttachmentContent: TypeAlias = bytes | EmailMessage | Message | SafeMIMEText | str
 _AttachmentTuple: TypeAlias = (
     tuple[str, _AttachmentContent] | tuple[str | None, _AttachmentContent, str] | tuple[str, _AttachmentContent, None]
 )
 
 class EmailMessage:
```

### Comparing `django-stubs-4.2.7/django-stubs/core/management/__init__.pyi` & `django_stubs-5.0.0/django-stubs/core/management/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Any
 
 from .base import BaseCommand as BaseCommand
 from .base import CommandError as CommandError
+from .base import CommandParser as CommandParser
+from .base import handle_default_options as handle_default_options
 
 def find_commands(management_dir: str) -> list[str]: ...
 def load_command_class(app_name: str, name: str) -> BaseCommand: ...
 def get_commands() -> dict[str, str]: ...
 def call_command(command_name: BaseCommand | str, *args: Any, **options: Any) -> str: ...
 
 class ManagementUtility:
```

### Comparing `django-stubs-4.2.7/django-stubs/core/management/base.pyi` & `django_stubs-5.0.0/django-stubs/core/management/base.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.apps.config import AppConfig
 from django.core.management.color import Style
 from django.utils.datastructures import _ListOrTuple
 
 ALL_CHECKS: Literal["__all__"]
 
 class CommandError(Exception):
+    returncode: int
     def __init__(self, *args: Any, returncode: int = ..., **kwargs: Any) -> None: ...
 
 class SystemCheckError(CommandError): ...
 
 class CommandParser(ArgumentParser):
     missing_args_message: str | None
     called_from_command_line: bool | None
```

### Comparing `django-stubs-4.2.7/django-stubs/core/management/color.pyi` & `django_stubs-5.0.0/django-stubs/core/management/color.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/management/commands/diffsettings.pyi` & `django_stubs-5.0.0/django-stubs/core/management/commands/diffsettings.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/management/commands/inspectdb.pyi` & `django_stubs-5.0.0/django-stubs/contrib/postgres/constraints.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,34 @@
-from collections.abc import Iterable
-from typing import Any
+from collections.abc import Iterable, Sequence
 
-from django.core.management.base import BaseCommand
-from django.db.backends.base.base import BaseDatabaseWrapper
+from django.db.backends.base.schema import BaseDatabaseSchemaEditor
+from django.db.models import Deferrable
+from django.db.models.base import Model
+from django.db.models.constraints import BaseConstraint
+from django.db.models.expressions import Combinable
+from django.db.models.indexes import IndexExpression
+from django.db.models.query_utils import Q
+from django.utils.functional import _StrOrPromise
 
-class Command(BaseCommand):
-    db_module: str
+class ExclusionConstraintExpression(IndexExpression): ...
 
-    def handle(self, **options: Any) -> None: ...
-    def handle_inspection(self, options: dict[str, Any]) -> Iterable[str]: ...
-    def normalize_col_name(
-        self, col_name: str, used_column_names: list[str], is_relation: bool
-    ) -> tuple[str, dict[str, str], list[str]]: ...
-    def get_field_type(
-        self, connection: BaseDatabaseWrapper, table_name: str, row: Any
-    ) -> tuple[str, dict[str, Any], list[str]]: ...
-    def get_meta(
+class ExclusionConstraint(BaseConstraint):
+    template: str
+    expressions: Sequence[tuple[str | Combinable, str]]
+    index_type: str
+    condition: Q | None
+    def __init__(
         self,
-        table_name: str,
-        constraints: Any,
-        column_to_field_name: Any,
-        is_view: bool,
-        is_partition: bool,
-        comment: str | None,
-    ) -> list[str]: ...
+        *,
+        name: str,
+        expressions: Sequence[tuple[str | Combinable, str]],
+        index_type: str | None = ...,
+        condition: Q | None = ...,
+        deferrable: Deferrable | None = ...,
+        include: list[str] | tuple[str] | None = ...,
+        violation_error_code: str | None = ...,
+        violation_error_message: _StrOrPromise | None = ...,
+    ) -> None: ...
+    def check_supported(self, schema_editor: BaseDatabaseSchemaEditor) -> None: ...
+    def validate(
+        self, model: type[Model], instance: Model, exclude: Iterable[str] | None = ..., using: str = ...
+    ) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/management/commands/loaddata.pyi` & `django_stubs-5.0.0/django-stubs/core/management/commands/loaddata.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/management/commands/makemessages.pyi` & `django_stubs-5.0.0/django-stubs/core/management/commands/makemessages.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/management/commands/makemigrations.pyi` & `django_stubs-5.0.0/django-stubs/core/management/commands/makemigrations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/management/commands/migrate.pyi` & `django_stubs-5.0.0/django-stubs/core/management/commands/migrate.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/management/commands/runserver.pyi` & `django_stubs-5.0.0/django-stubs/core/management/commands/runserver.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/management/templates.pyi` & `django_stubs-5.0.0/django-stubs/core/management/templates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/management/utils.pyi` & `django_stubs-5.0.0/django-stubs/core/management/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/paginator.pyi` & `django_stubs-5.0.0/django-stubs/core/paginator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from collections.abc import Iterable, Iterator, Sequence, Sized
-from typing import ClassVar, Generic, Protocol, TypeVar, overload
+from typing import ClassVar, Generic, Protocol, TypeVar, overload, type_check_only
 
+from django.db.models.fields import _ErrorMessagesDict
 from django.utils.functional import _StrPromise, cached_property
 
 class UnorderedObjectListWarning(RuntimeWarning): ...
 class InvalidPage(Exception): ...
 class PageNotAnInteger(InvalidPage): ...
 class EmptyPage(InvalidPage): ...
 
 _T = TypeVar("_T")
 
+@type_check_only
 class _SupportsPagination(Protocol[_T], Sized, Iterable):
     @overload
-    def __getitem__(self, __index: int) -> _T: ...
+    def __getitem__(self, index: int, /) -> _T: ...
     @overload
-    def __getitem__(self, __index: slice) -> _SupportsPagination[_T]: ...
+    def __getitem__(self, index: slice, /) -> _SupportsPagination[_T]: ...
 
 class Paginator(Generic[_T]):
     ELLIPSIS: ClassVar[_StrPromise]
+    default_error_messages: ClassVar[_ErrorMessagesDict]
+    error_messages: _ErrorMessagesDict
     object_list: _SupportsPagination[_T]
     per_page: int
     orphans: int
     allow_empty_first_page: bool
     def __init__(
         self,
         object_list: _SupportsPagination[_T],
         per_page: int | str,
         orphans: int = ...,
         allow_empty_first_page: bool = ...,
+        error_messages: _ErrorMessagesDict | None = ...,
     ) -> None: ...
     def __iter__(self) -> Iterator[Page[_T]]: ...
     def validate_number(self, number: int | float | str) -> int: ...
     def get_page(self, number: int | float | str | None) -> Page[_T]: ...
     def page(self, number: int | str) -> Page[_T]: ...
     @cached_property
     def count(self) -> int: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/serializers/__init__.pyi` & `django_stubs-5.0.0/django-stubs/core/serializers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/serializers/base.pyi` & `django_stubs-5.0.0/django-stubs/core/serializers/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 from collections.abc import Collection, Iterable, Sequence
 from typing import IO, Any
 
-from _typeshed import ReadableBuffer
 from django.db.models.base import Model
 from django.db.models.fields import Field
 from django.db.models.fields.related import ForeignKey, ManyToManyField
 
 DEFER_FIELD: object
 
-class PickleSerializer:
-    protocol: int
-    def __init__(self, protocol: int | None = ...) -> None: ...
-    def dumps(self, obj: Any) -> bytes: ...
-    def loads(self, data: ReadableBuffer) -> Any: ...
-
 class SerializerDoesNotExist(KeyError): ...
 class SerializationError(Exception): ...
 
 class DeserializationError(Exception):
     @classmethod
     def WithData(
         cls, original_exc: Exception, model: str, fk: int | str, field_value: Sequence[str] | str | None
@@ -71,15 +64,15 @@
     options: dict[str, Any]
     stream: IO[str] | IO[bytes]
     def __init__(self, stream_or_string: bytes | str | IO[bytes] | IO[str], **options: Any) -> None: ...
     def __iter__(self) -> Deserializer: ...
     def __next__(self) -> Any: ...
 
 class DeserializedObject:
-    object: Any
+    object: Model
     m2m_data: dict[str, Sequence[Any]] | None
     deferred_fields: dict[Field, Any]
     def __init__(
         self,
         obj: Model,
         m2m_data: dict[str, Sequence[Any]] | None = ...,
         deferred_fields: dict[Field, Any] | None = ...,
```

### Comparing `django-stubs-4.2.7/django-stubs/core/serializers/json.pyi` & `django_stubs-5.0.0/django-stubs/core/serializers/json.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/serializers/pyyaml.pyi` & `django_stubs-5.0.0/django-stubs/core/serializers/pyyaml.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/core/serializers/xml_serializer.pyi` & `django_stubs-5.0.0/django-stubs/core/serializers/xml_serializer.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import IO, Any
-from xml.sax.expatreader import ExpatParser as _ExpatParser
+from xml.sax.expatreader import ExpatParser as _ExpatParser  # type: ignore[import-not-found]
 
 from django.core.serializers import base
 
 class Serializer(base.Serializer):
     def indent(self, level: int) -> None: ...
     xml: Any
     def start_serialization(self) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/servers/basehttp.pyi` & `django_stubs-5.0.0/django-stubs/core/servers/basehttp.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import socketserver
 from io import BytesIO
-from typing import Any
+from typing import Any, Callable
 from wsgiref import simple_server
 
 from django.core.handlers.wsgi import WSGIHandler, WSGIRequest
 
+def get_internal_wsgi_application() -> WSGIHandler: ...
+def is_broken_pipe_error() -> bool: ...
+
 class WSGIServer(simple_server.WSGIServer):
     request_queue_size: int
     address_family: Any
     allow_reuse_address: Any
     def __init__(self, *args: Any, ipv6: bool = ..., allow_reuse_address: bool = ..., **kwargs: Any) -> None: ...
     def handle_error(self, request: Any, client_address: Any) -> None: ...
 
@@ -28,8 +31,16 @@
     def log_message(self, format: str, *args: Any) -> None: ...
     def get_environ(self) -> dict[str, str]: ...
     raw_requestline: bytes
     requestline: str
     request_version: str
     def handle(self) -> None: ...
 
-def get_internal_wsgi_application() -> WSGIHandler: ...
+def run(
+    addr: str | bytes | bytearray,
+    port: int,
+    wsgi_handler: WSGIHandler,
+    ipv6: bool = ...,
+    threading: bool = ...,
+    on_bind: Callable[[str], None] | None = ...,
+    server_cls: type[WSGIServer] = ...,
+) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/core/signing.pyi` & `django_stubs-5.0.0/django-stubs/core/signing.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,76 @@
 from datetime import timedelta
-from typing import Any, Protocol
+from typing import Any, Protocol, overload, type_check_only
+
+from typing_extensions import deprecated
+
+BASE62_ALPHABET: str
 
 class BadSignature(Exception): ...
 class SignatureExpired(BadSignature): ...
 
+def b62_encode(s: int) -> str: ...
+def b62_decode(s: str) -> int: ...
 def b64_encode(s: bytes) -> bytes: ...
 def b64_decode(s: bytes) -> bytes: ...
-def base64_hmac(salt: str, value: bytes | str, key: bytes | str, algorithm: str = ...) -> str: ...
+def base64_hmac(salt: bytes | str, value: bytes | str, key: bytes | str, algorithm: str = ...) -> str: ...
 def get_cookie_signer(salt: str = ...) -> TimestampSigner: ...
-
+@type_check_only
 class Serializer(Protocol):
     def dumps(self, obj: Any) -> bytes: ...
     def loads(self, data: bytes) -> Any: ...
 
 class JSONSerializer:
     def dumps(self, obj: Any) -> bytes: ...
     def loads(self, data: bytes) -> Any: ...
 
 def dumps(
     obj: Any,
     key: bytes | str | None = ...,
-    salt: str = ...,
+    salt: bytes | str = ...,
     serializer: type[Serializer] = ...,
     compress: bool = ...,
 ) -> str: ...
 def loads(
     s: str,
     key: bytes | str | None = ...,
-    salt: str = ...,
+    salt: bytes | str = ...,
     serializer: type[Serializer] = ...,
     max_age: int | timedelta | None = ...,
+    fallback_keys: list[str | bytes] | None = ...,
 ) -> Any: ...
 
 class Signer:
-    key: str
+    key: bytes | str
+    fallback_keys: list[bytes | str]
     sep: str
-    salt: str
+    salt: bytes | str
     algorithm: str
+    @overload
+    def __init__(
+        self,
+        *,
+        key: bytes | str | None = ...,
+        sep: str = ...,
+        salt: bytes | str | None = ...,
+        algorithm: str | None = ...,
+        fallback_keys: list[bytes | str] | None = ...,
+    ) -> None: ...
+    @overload
+    @deprecated("Passing positional arguments to Signer is deprecated and will be removed in Django 5.1")
     def __init__(
         self,
+        *args: Any,
         key: bytes | str | None = ...,
         sep: str = ...,
-        salt: str | None = ...,
+        salt: bytes | str | None = ...,
         algorithm: str | None = ...,
+        fallback_keys: list[bytes | str] | None = ...,
     ) -> None: ...
-    def signature(self, value: bytes | str) -> str: ...
+    def signature(self, value: bytes | str, key: bytes | str | None = ...) -> str: ...
     def sign(self, value: str) -> str: ...
     def unsign(self, signed_value: str) -> str: ...
     def sign_object(
         self,
         obj: Any,
         serializer: type[Serializer] = ...,
         compress: bool = ...,
```

### Comparing `django-stubs-4.2.7/django-stubs/core/validators.pyi` & `django_stubs-5.0.0/django-stubs/core/validators.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     domain_re: str
     tld_re: str
     host_re: str
     schemes: Sequence[str]
     unsafe_chars: frozenset[str]
     max_length: int
     def __init__(self, schemes: Sequence[str] | None = ..., **kwargs: Any) -> None: ...
-    def __call__(self, value: str) -> None: ...
+    def __call__(self, value: Any) -> None: ...
 
 integer_validator: RegexValidator
 
 def validate_integer(value: float | str | None) -> None: ...
 
 class EmailValidator(_Deconstructible):
     message: _StrOrPromise
@@ -85,23 +85,28 @@
 
 validate_comma_separated_integer_list: RegexValidator
 
 class BaseValidator(_Deconstructible):
     message: _StrOrPromise
     code: str
     limit_value: Any
-    def __init__(self, limit_value: Any, message: _StrOrPromise | None = ...) -> None: ...
+    def __init__(self, limit_value: Any | Callable[[], Any], message: _StrOrPromise | None = ...) -> None: ...
     def __call__(self, value: Any) -> None: ...
     def compare(self, a: Any, b: Any) -> bool: ...
     def clean(self, x: Any) -> Any: ...
     def __eq__(self, other: object) -> bool: ...
 
 class MaxValueValidator(BaseValidator): ...
 class MinValueValidator(BaseValidator): ...
-class StepValueValidator(BaseValidator): ...
+
+class StepValueValidator(BaseValidator):
+    offset: int | None
+    def __init__(
+        self, limit_value: Any | Callable[[], Any], message: _StrOrPromise | None = ..., offset: int | None = ...
+    ) -> None: ...
 
 class MinLengthValidator(BaseValidator):
     def clean(self, x: Sized) -> int: ...
 
 class MaxLengthValidator(BaseValidator):
     def clean(self, x: Sized) -> int: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/__init__.pyi` & `django_stubs-5.0.0/django-stubs/db/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/base/base.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/base/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 
 logger: Logger
 
 _ExecuteWrapper: TypeAlias = Callable[
     [Callable[[str, Any, bool, dict[str, Any]], Any], str, Any, bool, dict[str, Any]], Any
 ]
 
-def timezone_constructor(tzname: str) -> tzinfo: ...
-
 class BaseDatabaseWrapper:
     data_types: dict[str, str]
     data_types_suffix: dict[str, str]
     data_type_check_constraints: dict[str, str]
     vendor: str
     display_name: str
     SchemaEditorClass: type[BaseDatabaseSchemaEditor]
```

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/base/client.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/oracle/client.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from collections.abc import Iterable, Sequence
+from collections.abc import Iterable
 from typing import Any
 
-from django.db.backends.base.base import BaseDatabaseWrapper
+from django.db.backends.base.client import BaseDatabaseClient
+from django.db.backends.oracle.base import DatabaseWrapper
 
-class BaseDatabaseClient:
-    executable_name: str | None
-    connection: BaseDatabaseWrapper
-    def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
+class DatabaseClient(BaseDatabaseClient):
+    connection: DatabaseWrapper
+    executable_name: str
+    wrapper_name: str
+    @staticmethod
+    def connect_string(settings_dict: dict[str, Any]) -> str: ...
     @classmethod
     def settings_to_cmd_args_env(
-        cls,
-        settings_dict: dict[str, Any],
-        parameters: Iterable[str],
-    ) -> tuple[Sequence[str], dict[str, str] | None]: ...
-    def runshell(self, parameters: Iterable[str]) -> None: ...
+        cls, settings_dict: dict[str, Any], parameters: Iterable[str]
+    ) -> tuple[list[str], None]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/base/creation.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/base/creation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/base/features.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/base/features.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,14 @@
     requires_casted_case_in_updates: bool
     supports_partial_indexes: bool
     supports_functions_in_partial_indexes: bool
     supports_covering_indexes: bool
     supports_expression_indexes: bool
     collate_as_index_expression: bool
     allows_multiple_constraints_on_same_fields: bool
-    supports_boolean_expr_in_select_clause: bool
     supports_comparing_boolean_expr: bool
     supports_json_field: bool
     can_introspect_json_field: bool
     supports_primitives_in_json_field: bool
     has_native_json_field: bool
     has_json_operators: bool
     supports_json_field_contains: bool
@@ -138,8 +137,10 @@
     django_test_skips: dict[str, set[str]]
     connection: BaseDatabaseWrapper
     def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
     @cached_property
     def supports_explaining_query_execution(self) -> bool: ...
     @cached_property
     def supports_transactions(self) -> bool: ...
+    @cached_property
+    def supports_boolean_expr_in_select_clause(self) -> bool: ...
     def allows_group_by_selected_pks_on_model(self, model: type[Model]) -> bool: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/base/introspection.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/base/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/base/operations.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/base/schema.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/base/schema.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.ddl_references import Statement
 from django.db.models.base import Model
 from django.db.models.constraints import BaseConstraint
 from django.db.models.fields import Field
 from django.db.models.indexes import Index
+from django.db.models.sql.compiler import _AsSqlType
 from typing_extensions import Self
 
 logger: Logger
 
 class BaseDatabaseSchemaEditor(AbstractContextManager[Any]):
     sql_create_table: str
     sql_rename_table: str
@@ -72,14 +73,15 @@
     def table_sql(self, model: type[Model]) -> tuple[str, list[Any]]: ...
     def column_sql(
         self, model: type[Model], field: Field, include_default: bool = ...
     ) -> tuple[None, None] | tuple[str, list[Any]]: ...
     def skip_default(self, field: Any) -> bool: ...
     def skip_default_on_alter(self, field: Any) -> bool: ...
     def prepare_default(self, value: Any) -> Any: ...
+    def db_default_sql(self, field: Field) -> _AsSqlType: ...
     def effective_default(self, field: Field) -> int | str: ...
     def quote_value(self, value: Any) -> str: ...
     def create_model(self, model: type[Model]) -> None: ...
     def delete_model(self, model: type[Model]) -> None: ...
     def add_index(self, model: type[Model], index: Index) -> None: ...
     def remove_index(self, model: type[Model], index: Index) -> None: ...
     def rename_index(self, model: type[Model], old_index: Index, new_index: Index) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/ddl_references.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/ddl_references.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Sequence
-from typing import Any, Protocol
+from typing import Any, Protocol, type_check_only
 
+@type_check_only
 class _QuoteCallable(Protocol):
     """Get rid of `cannot assign to method`"""
 
-    def __call__(self, __column: str) -> str: ...
+    def __call__(self, column: str, /) -> str: ...
 
 class Reference:
     def references_table(self, table: Any) -> bool: ...
     def references_column(self, table: Any, column: Any) -> bool: ...
     def rename_table_references(self, old_table: Any, new_table: Any) -> None: ...
     def rename_column_references(self, table: Any, old_column: Any, new_column: Any) -> None: ...
 
@@ -31,18 +32,19 @@
     table: str
     quote_name: _QuoteCallable
     col_suffixes: Sequence[str]
     def __init__(
         self, table: str, columns: list[str], quote_name: _QuoteCallable, col_suffixes: Sequence[str] = ...
     ) -> None: ...
 
+@type_check_only
 class _NameCallable(Protocol):
     """Get rid of `cannot assign to method`"""
 
-    def __call__(self, __table: str, __columns: list[str], __suffix: str) -> str: ...
+    def __call__(self, table: str, columns: list[str], suffix: str, /) -> str: ...
 
 class IndexName(TableColumns):
     columns: list[str]
     table: str
     suffix: str
     create_index_name: _NameCallable
     def __init__(self, table: str, columns: list[str], suffix: str, create_index_name: _NameCallable) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/dummy/base.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/dummy/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/mysql/base.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/mysql/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/mysql/compiler.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/mysql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/mysql/features.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/mysql/introspection.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/mysql/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/mysql/operations.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/mysql/schema.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/oracle/base.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/oracle/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,14 @@
     def get_new_connection(self, conn_params: Any) -> Any: ...
     pattern_ops: Any
     def init_connection_state(self) -> None: ...
     def create_cursor(self, name: Any | None = ...) -> Any: ...
     def check_constraints(self, table_names: Any | None = ...) -> None: ...
     def is_usable(self) -> Any: ...
     @property
-    def cx_oracle_version(self) -> Any: ...
-    @property
     def oracle_version(self) -> Any: ...
 
 class OracleParam:
     force_bytes: Any
     input_size: Any
     def __init__(self, param: Any, cursor: Any, strings_only: bool = ...) -> None: ...
 
@@ -64,15 +62,16 @@
     def bind_parameter(self, cursor: Any) -> Any: ...
     def __getattr__(self, key: Any) -> Any: ...
     def __setattr__(self, key: Any, value: Any) -> None: ...
 
 class FormatStylePlaceholderCursor:
     charset: str
     cursor: Any
-    def __init__(self, connection: Any) -> None: ...
+    database: BaseDatabaseWrapper
+    def __init__(self, connection: Any, database: BaseDatabaseWrapper) -> None: ...
     def execute(self, query: Any, params: Any | None = ...) -> Any: ...
     def executemany(self, query: Any, params: Any | None = ...) -> Any: ...
     def close(self) -> None: ...
     def var(self, *args: Any) -> Any: ...
     def arrayvar(self, *args: Any) -> Any: ...
     def __getattr__(self, attr: Any) -> Any: ...
     def __iter__(self) -> Iterator[Any]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/oracle/features.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/oracle/features.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -42,10 +42,9 @@
     supports_over_clause: bool
     supports_frame_range_fixed_distance: bool
     supports_ignore_conflicts: bool
     max_query_params: Any
     supports_partial_indexes: bool
     supports_slicing_ordering_in_compound: bool
     allows_multiple_constraints_on_same_fields: bool
-    supports_boolean_expr_in_select_clause: bool
     supports_primitives_in_json_field: bool
     supports_json_field_contains: bool
```

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/oracle/operations.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/oracle/schema.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/postgresql/base.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/postgresql/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/postgresql/client.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/postgresql/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/postgresql/features.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/postgresql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/postgresql/operations.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/postgresql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/postgresql/schema.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/postgresql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/sqlite3/base.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/sqlite3/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/sqlite3/operations.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/sqlite3/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/backends/utils.pyi` & `django_stubs-5.0.0/django-stubs/db/backends/utils.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
 from collections.abc import Generator, Iterator, Mapping, Sequence
 from contextlib import contextmanager
 from decimal import Decimal
 from logging import Logger
 from types import TracebackType
-from typing import Any, Literal, Protocol, overload
+from typing import Any, Literal, Protocol, overload, type_check_only
 from uuid import UUID
 
 from typing_extensions import Self, TypeAlias
 
 logger: Logger
 
 # Protocol matching psycopg2.sql.Composable, to avoid depending psycopg2
+@type_check_only
 class _Composable(Protocol):
     def as_string(self, context: Any) -> str: ...
     def __add__(self, other: Self) -> _Composable: ...
     def __mul__(self, n: int) -> _Composable: ...
 
 _ExecuteQuery: TypeAlias = str | _Composable
```

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/autodetector.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/autodetector.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/exceptions.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/executor.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/executor.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from collections.abc import Sequence
-from typing import Protocol
+from typing import Protocol, type_check_only
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.migrations.migration import Migration
 
 from .loader import MigrationLoader
 from .recorder import MigrationRecorder
 from .state import ProjectState
 
+@type_check_only
 class _ProgressCallbackT(Protocol):
-    def __call__(self, __action: str, __migration: Migration | None = ..., __fake: bool | None = ...) -> None: ...
+    def __call__(self, action: str, migration: Migration | None = ..., fake: bool | None = ..., /) -> None: ...
 
 class MigrationExecutor:
     connection: BaseDatabaseWrapper
     loader: MigrationLoader
     recorder: MigrationRecorder
     progress_callback: _ProgressCallbackT | None
     def __init__(
```

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/graph.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/graph.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/loader.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/loader.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/migration.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/migration.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/operations/__init__.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/operations/base.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/operations/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/operations/fields.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/operations/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/operations/models.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/operations/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/operations/special.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/operations/special.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Mapping, Sequence
-from typing import Any, Literal, Protocol
+from typing import Any, Literal, Protocol, type_check_only
 
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.migrations.state import StateApps
 from django.utils.datastructures import _ListOrTuple
 from typing_extensions import TypeAlias
 
 from .base import Operation
@@ -31,16 +31,17 @@
         state_operations: Sequence[Operation] | None = ...,
         hints: Mapping[str, Any] | None = ...,
         elidable: bool = ...,
     ) -> None: ...
     @property
     def reversible(self) -> bool: ...  # type: ignore[override]
 
+@type_check_only
 class _CodeCallable(Protocol):
-    def __call__(self, __state_apps: StateApps, __schema_editor: BaseDatabaseSchemaEditor) -> None: ...
+    def __call__(self, state_apps: StateApps, schema_editor: BaseDatabaseSchemaEditor, /) -> None: ...
 
 class RunPython(Operation):
     code: _CodeCallable
     reverse_code: _CodeCallable | None
     hints: Mapping[str, Any]
     def __init__(
         self,
```

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/operations/utils.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/operations/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/questioner.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/questioner.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/recorder.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/recorder.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class MigrationRecorder:
     class Migration(Model):
         app: Any
         name: Any
         applied: Any
         objects: ClassVar[Manager[Self]]
+
     connection: BaseDatabaseWrapper
     def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
     @property
     def migration_qs(self) -> QuerySet: ...
     def has_table(self) -> bool: ...
     def ensure_schema(self) -> None: ...
     def applied_migrations(self) -> dict[tuple[str, str], Migration]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/serializer.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/serializer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/state.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/state.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/migrations/writer.pyi` & `django_stubs-5.0.0/django-stubs/db/migrations/writer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/__init__.pyi` & `django_stubs-5.0.0/django-stubs/db/models/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 from .fields import SmallIntegerField as SmallIntegerField
 from .fields import TextField as TextField
 from .fields import TimeField as TimeField
 from .fields import URLField as URLField
 from .fields import UUIDField as UUIDField
 from .fields.files import FileField as FileField
 from .fields.files import ImageField as ImageField
+from .fields.generated import GeneratedField as GeneratedField
 from .fields.json import JSONField as JSONField
 from .fields.proxy import OrderWrt as OrderWrt
 from .fields.related import ForeignKey as ForeignKey
 from .fields.related import ForeignObject as ForeignObject
 from .fields.related import ForeignObjectRel as ForeignObjectRel
 from .fields.related import ManyToManyField as ManyToManyField
 from .fields.related import ManyToManyRel as ManyToManyRel
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/aggregates.pyi` & `django_stubs-5.0.0/django-stubs/db/models/aggregates.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from django.db.models.fields import IntegerField
 from django.db.models.functions.mixins import FixDurationInputMixin, NumericOutputFieldMixin
 
 class Aggregate(Func):
     filter_template: str
     filter: Any
     allow_distinct: bool
+    empty_result_set_value: int | None
     def __init__(self, *expressions: Any, distinct: bool = ..., filter: Any | None = ..., **extra: Any) -> None: ...
 
 class Avg(FixDurationInputMixin, NumericOutputFieldMixin, Aggregate): ...
 
 class Count(Aggregate):
     output_field: ClassVar[IntegerField]
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/base.pyi` & `django_stubs-5.0.0/django-stubs/db/models/base.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Collection, Iterable, Sequence
 from typing import Any, ClassVar, Final, TypeVar, overload
 
 from django.core.checks.messages import CheckMessage
 from django.core.exceptions import MultipleObjectsReturned as BaseMultipleObjectsReturned
 from django.core.exceptions import ObjectDoesNotExist, ValidationError
 from django.db.models import BaseConstraint, Field, QuerySet
-from django.db.models.manager import BaseManager, Manager
+from django.db.models.manager import Manager
 from django.db.models.options import Options
 from typing_extensions import Self
 
 _Self = TypeVar("_Self", bound=Model)
 
 class ModelStateFieldsCacheDescriptor:
     @overload
@@ -20,31 +20,30 @@
 class ModelState:
     db: str | None
     adding: bool
     fields_cache: ModelStateFieldsCacheDescriptor
 
 class ModelBase(type):
     @property
-    def _default_manager(cls: type[_Self]) -> BaseManager[_Self]: ...  # type: ignore[misc]
+    def _default_manager(cls: type[_Self]) -> Manager[_Self]: ...  # type: ignore[misc]
     @property
-    def _base_manager(cls: type[_Self]) -> BaseManager[_Self]: ...  # type: ignore[misc]
+    def _base_manager(cls: type[_Self]) -> Manager[_Self]: ...  # type: ignore[misc]
 
 class Model(metaclass=ModelBase):
     # Note: these two metaclass generated attributes don't really exist on the 'Model'
     # class, runtime they are only added on concrete subclasses of 'Model'. The
     # metaclass also sets up correct inheritance from concrete parent models exceptions.
     # Our mypy plugin aligns with this behaviour and will remove the 2 attributes below
     # and re-add them to correct concrete subclasses of 'Model'
     DoesNotExist: Final[type[ObjectDoesNotExist]]
     MultipleObjectsReturned: Final[type[BaseMultipleObjectsReturned]]
     # This 'objects' attribute will be deleted, via the plugin, in favor of managing it
     # to only exist on subclasses it exists on during runtime.
     objects: ClassVar[Manager[Self]]
 
-    class Meta: ...
     _meta: ClassVar[Options[Self]]
     pk: Any
     _state: ModelState
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     @classmethod
     def add_to_class(cls, name: str, value: Any) -> Any: ...
     @classmethod
@@ -68,36 +67,36 @@
     def validate_unique(self, exclude: Collection[str] | None = ...) -> None: ...
     def date_error_message(self, lookup_type: str, field_name: str, unique_for: str) -> ValidationError: ...
     def unique_error_message(self, model_class: type[Self], unique_check: Sequence[str]) -> ValidationError: ...
     def validate_constraints(self, exclude: Collection[str] | None = ...) -> None: ...
     def get_constraints(self) -> list[tuple[type[Model], Sequence[BaseConstraint]]]: ...
     def save(
         self,
-        force_insert: bool = ...,
+        force_insert: bool | tuple[ModelBase, ...] = ...,
         force_update: bool = ...,
         using: str | None = ...,
         update_fields: Iterable[str] | None = ...,
     ) -> None: ...
     async def asave(
         self,
-        force_insert: bool = ...,
+        force_insert: bool | tuple[ModelBase, ...] = ...,
         force_update: bool = ...,
         using: str | None = ...,
         update_fields: Iterable[str] | None = ...,
     ) -> None: ...
     def save_base(
         self,
         raw: bool = ...,
-        force_insert: bool = ...,
+        force_insert: bool | tuple[ModelBase, ...] = ...,
         force_update: bool = ...,
         using: str | None = ...,
         update_fields: Iterable[str] | None = ...,
     ) -> None: ...
-    def refresh_from_db(self, using: str | None = ..., fields: Sequence[str] | None = ...) -> None: ...
-    async def arefresh_from_db(self, using: str | None = ..., fields: Sequence[str] | None = ...) -> None: ...
+    def refresh_from_db(self, using: str | None = ..., fields: Iterable[str] | None = ...) -> None: ...
+    async def arefresh_from_db(self, using: str | None = ..., fields: Iterable[str] | None = ...) -> None: ...
     def serializable_value(self, field_name: str) -> Any: ...
     def prepare_database_save(self, field: Field) -> Any: ...
     def get_deferred_fields(self) -> set[str]: ...
     @classmethod
     def check(cls, **kwargs: Any) -> list[CheckMessage]: ...
     def __getstate__(self) -> dict: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/constraints.pyi` & `django_stubs-5.0.0/django-stubs/db/models/constraints.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -3,60 +3,81 @@
 from typing import Any, overload
 
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.models.base import Model
 from django.db.models.expressions import BaseExpression, Combinable
 from django.db.models.query_utils import Q
 from django.utils.functional import _StrOrPromise
-from typing_extensions import Self
+from typing_extensions import Self, deprecated
 
 class Deferrable(Enum):
     DEFERRED: str
     IMMEDIATE: str
 
 class BaseConstraint:
     name: str
+    violation_error_code: str | None
     violation_error_message: _StrOrPromise | None
     default_violation_error_message: _StrOrPromise
-    def __init__(self, name: str, violation_error_message: _StrOrPromise | None = ...) -> None: ...
+    @overload
+    def __init__(
+        self, *, name: str, violation_error_code: str | None = ..., violation_error_message: _StrOrPromise | None = ...
+    ) -> None: ...
+    @overload
+    @deprecated("Passing positional arguments to BaseConstraint is deprecated and will be removed in Django 6.0")
+    def __init__(
+        self,
+        *args: Any,
+        name: str | None = ...,
+        violation_error_code: str | None = ...,
+        violation_error_message: _StrOrPromise | None = ...,
+    ) -> None: ...
     def constraint_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
     def create_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
     def remove_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
     def deconstruct(self) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
     def clone(self) -> Self: ...
 
 class CheckConstraint(BaseConstraint):
     check: Q | BaseExpression
     def __init__(
-        self, *, check: Q | BaseExpression, name: str, violation_error_message: _StrOrPromise | None = ...
+        self,
+        *,
+        check: Q | BaseExpression,
+        name: str,
+        violation_error_code: str | None = ...,
+        violation_error_message: _StrOrPromise | None = ...,
     ) -> None: ...
 
 class UniqueConstraint(BaseConstraint):
     expressions: Sequence[BaseExpression | Combinable]
     fields: Sequence[str]
     condition: Q | None
     deferrable: Deferrable | None
 
     @overload
     def __init__(
         self,
         *expressions: str | BaseExpression | Combinable,
         fields: None = ...,
-        name: str,
+        name: str | None = ...,
         condition: Q | None = ...,
         deferrable: Deferrable | None = ...,
         include: Sequence[str] | None = ...,
         opclasses: Sequence[Any] = ...,
+        violation_error_code: str | None = ...,
         violation_error_message: _StrOrPromise | None = ...,
     ) -> None: ...
     @overload
     def __init__(
         self,
         *,
         fields: Sequence[str],
-        name: str,
+        name: str | None = ...,
         condition: Q | None = ...,
         deferrable: Deferrable | None = ...,
         include: Sequence[str] | None = ...,
         opclasses: Sequence[Any] = ...,
+        nulls_distinct: bool | None = ...,
+        violation_error_code: str | None = ...,
         violation_error_message: _StrOrPromise | None = ...,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/deletion.pyi` & `django_stubs-5.0.0/django-stubs/db/models/deletion.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/enums.pyi` & `django_stubs-5.0.0/django-stubs/db/models/enums.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import enum
 import sys
-from typing import Any, TypeVar
+from typing import Any, TypeVar, type_check_only
 
-from typing_extensions import Self
+from typing_extensions import Self, TypeAlias
 
 _Self = TypeVar("_Self")
 
 if sys.version_info >= (3, 11):
     _enum_property = enum.property
 else:
     _enum_property = property
@@ -25,35 +25,39 @@
     @property
     def choices(self) -> list[tuple[Any, str]]: ...
     @property
     def labels(self) -> list[str]: ...
     @property
     def values(self) -> list[Any]: ...
 
+ChoicesType: TypeAlias = ChoicesMeta
+
 class Choices(enum.Enum, metaclass=ChoicesMeta):
     @property
     def label(self) -> str: ...
     @_enum_property
     def value(self) -> Any: ...
     @property
     def do_not_call_in_templates(self) -> bool: ...
 
 # fake, to keep simulate class properties
+@type_check_only
 class _IntegerChoicesMeta(ChoicesMeta):
     @property
     def choices(self) -> list[tuple[int, str]]: ...
     @property
     def values(self) -> list[int]: ...
 
 class IntegerChoices(int, Choices, metaclass=_IntegerChoicesMeta):
     def __new__(cls, value: int) -> Self: ...
     @_enum_property
     def value(self) -> int: ...
 
 # fake, to keep simulate class properties
+@type_check_only
 class _TextChoicesMeta(ChoicesMeta):
     @property
     def choices(self) -> list[tuple[str, str]]: ...
     @property
     def values(self) -> list[str]: ...
 
 class TextChoices(str, Choices, metaclass=_TextChoicesMeta):
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/expressions.pyi` & `django_stubs-5.0.0/django-stubs/db/models/expressions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/fields/__init__.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 import decimal
 import uuid
 from collections.abc import Callable, Iterable, Mapping, Sequence
 from datetime import date, time, timedelta
 from datetime import datetime as real_datetime
-from typing import Any, ClassVar, Generic, Literal, Protocol, TypeVar, overload
+from typing import Any, ClassVar, Generic, Literal, Protocol, TypeVar, overload, type_check_only
 
 from django import forms
 from django.core import validators  # due to weird mypy.stubtest error
 from django.core.checks import CheckMessage
 from django.core.exceptions import FieldDoesNotExist as FieldDoesNotExist
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Model
-from django.db.models.expressions import Col, Combinable
+from django.db.models.expressions import Col, Combinable, Expression
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.db.models.query_utils import Q, RegisterLookupMixin
 from django.forms import Widget
+from django.utils.choices import BlankChoiceIterator, _Choice, _ChoiceNamedGroup, _Choices, _ChoicesCallable
 from django.utils.datastructures import DictWrapper
 from django.utils.functional import _Getter, _StrOrPromise, cached_property
 from typing_extensions import Self, TypeAlias
 
 class Empty: ...
 class NOT_PROVIDED: ...
 
 BLANK_CHOICE_DASH: list[tuple[str, str]]
 
-_Choice: TypeAlias = tuple[Any, Any]
-
-_ChoiceNamedGroup: TypeAlias = tuple[str, Iterable[_Choice]]
-_FieldChoices: TypeAlias = Iterable[_Choice | _ChoiceNamedGroup]
 _ChoicesList: TypeAlias = Sequence[_Choice] | Sequence[_ChoiceNamedGroup]
 _LimitChoicesTo: TypeAlias = Q | dict[str, Any]
 
 _F = TypeVar("_F", bound=Field, covariant=True)
 
-class _ChoicesCallable(Protocol):
-    def __call__(self) -> _FieldChoices: ...
-
+@type_check_only
 class _FieldDescriptor(Protocol[_F]):
     """
     Accessing fields of a model class (not instance) returns an object conforming to this protocol.
     Depending on field type this could be DeferredAttribute, ForwardManyToOneDescriptor, FileDescriptor, etc.
     """
 
     @property
@@ -138,14 +133,15 @@
     null: bool
     unique: bool
     editable: bool
     empty_strings_allowed: bool
     choices: _ChoicesList | None
     db_column: str | None
     db_comment: str | None
+    db_default: type[NOT_PROVIDED] | Expression
     column: str
     concrete: bool
     default: Any
     error_messages: _ErrorMessagesDict
     empty_values: Sequence[Any]
     creation_counter: int
     auto_creation_counter: int
@@ -168,22 +164,23 @@
         rel: ForeignObjectRel | None = ...,
         default: Any = ...,
         editable: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_tablespace: str | None = ...,
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         db_comment: str | None = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
     ) -> None: ...
     def __set__(self, instance: Any, value: _ST) -> None: ...
     # class access
     @overload
     def __get__(self, instance: None, owner: Any) -> _FieldDescriptor[Self]: ...
     # Model instance access
     @overload
@@ -219,15 +216,15 @@
     def clean(self, value: Any, model_instance: Model | None) -> Any: ...
     def get_choices(
         self,
         include_blank: bool = ...,
         blank_choice: _ChoicesList = ...,
         limit_choices_to: _LimitChoicesTo | None = ...,
         ordering: Sequence[str] = ...,
-    ) -> _ChoicesList: ...
+    ) -> BlankChoiceIterator | _ChoicesList: ...
     def _get_flatchoices(self) -> list[_Choice]: ...
     @property
     def flatchoices(self) -> list[_Choice]: ...
     def has_default(self) -> bool: ...
     def get_default(self) -> Any: ...
     def check(self, **kwargs: Any) -> list[CheckMessage]: ...
     def get_col(self, alias: str, output_field: Field | None = ...) -> Col: ...
@@ -276,18 +273,19 @@
         *,
         primary_key: bool = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
@@ -304,21 +302,22 @@
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         *,
@@ -333,21 +332,22 @@
         verbose_name: _StrOrPromise | None = ...,
         name: str | None = ...,
         primary_key: bool = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         *,
@@ -368,20 +368,21 @@
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         rel: ForeignObjectRel | None = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
@@ -399,21 +400,22 @@
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         *,
@@ -449,18 +451,19 @@
         unpack_ipv4: bool = ...,
         primary_key: bool = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
@@ -483,18 +486,19 @@
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
@@ -513,18 +517,19 @@
         *,
         primary_key: bool = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
@@ -547,20 +552,21 @@
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         rel: ForeignObjectRel | None = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
@@ -585,18 +591,19 @@
         primary_key: bool = ...,
         max_length: int = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/fields/files.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/files.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 from collections.abc import Callable, Iterable
-from typing import Any, Protocol, TypeVar, overload
+from typing import Any, Protocol, TypeVar, overload, type_check_only
 
 from django.core import validators  # due to weird mypy.stubtest error
 from django.core.files.base import File
 from django.core.files.images import ImageFile
 from django.core.files.storage import Storage
 from django.db.models.base import Model
-from django.db.models.fields import Field, _ErrorMessagesMapping, _FieldChoices
+from django.db.models.expressions import Expression
+from django.db.models.fields import NOT_PROVIDED, Field, _ErrorMessagesMapping
 from django.db.models.query_utils import DeferredAttribute
+from django.db.models.utils import AltersData
 from django.utils._os import _PathCompatible
+from django.utils.choices import _Choices
 from django.utils.functional import _StrOrPromise
 from typing_extensions import Self
 
-class FieldFile(File):
+class FieldFile(File, AltersData):
     instance: Model
     field: FileField
     storage: Storage
     name: str | None
     def __init__(self, instance: Model, field: FileField, name: str | None) -> None: ...
     file: Any
     @property
     def path(self) -> str: ...
     @property
     def url(self) -> str: ...
     @property
     def size(self) -> int: ...
+    def open(self, mode: str = ...) -> Self: ...  # type: ignore[override]
     def save(self, name: str, content: File, save: bool = ...) -> None: ...
     def delete(self, save: bool = ...) -> None: ...
     @property
     def closed(self) -> bool: ...
+    def __getstate__(self) -> dict[str, Any]: ...
+    def __setstate__(self, state: dict[str, Any]) -> None: ...
+    def __eq__(self, other: object) -> bool: ...
+    def __hash__(self) -> int: ...
 
 class FileDescriptor(DeferredAttribute):
     field: FileField
     def __set__(self, instance: Model, value: Any | None) -> None: ...
     def __get__(self, instance: Model | None, cls: type[Model] | None = ...) -> FieldFile | FileDescriptor: ...
 
 _M = TypeVar("_M", bound=Model, contravariant=True)
 
+@type_check_only
 class _UploadToCallable(Protocol[_M]):
-    def __call__(self, __instance: _M, __filename: str) -> _PathCompatible: ...
+    def __call__(self, instance: _M, filename: str, /) -> _PathCompatible: ...
 
 class FileField(Field):
     storage: Storage
     upload_to: _PathCompatible | _UploadToCallable
     def __init__(
         self,
         verbose_name: _StrOrPromise | None = ...,
@@ -52,21 +61,22 @@
         *,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | str = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/fields/json.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/json.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import json
 from collections.abc import Callable
-from typing import Any, ClassVar
+from typing import Any, ClassVar, TypeVar
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import lookups
+from django.db.models.expressions import Expression
 from django.db.models.fields import TextField
 from django.db.models.lookups import PostgresOperatorLookup, Transform
 from django.db.models.sql.compiler import SQLCompiler
 from django.utils.functional import _StrOrPromise
 from typing_extensions import Self
 
 from . import Field
 from .mixins import CheckFieldDefaultMixin
 
-class JSONField(CheckFieldDefaultMixin, Field):
+# __set__ value type
+_ST = TypeVar("_ST", contravariant=True, default=Any)
+# __get__ return type
+_GT = TypeVar("_GT", covariant=True, default=Any)
+
+class JSONField(CheckFieldDefaultMixin, Field[_ST, _GT]):
     encoder: type[json.JSONEncoder] | None
     decoder: type[json.JSONDecoder] | None
     def __init__(
         self,
         verbose_name: _StrOrPromise | None = ...,
         name: str | None = ...,
         encoder: type[json.JSONEncoder] | None = ...,
         decoder: type[json.JSONDecoder] | None = ...,
         **kwargs: Any,
     ) -> None: ...
+    def from_db_value(self, value: str | None, expression: Expression, connection: BaseDatabaseWrapper) -> Any: ...
 
 class DataContains(PostgresOperatorLookup): ...
 class ContainedBy(PostgresOperatorLookup): ...
 
 class HasKeyLookup(PostgresOperatorLookup):
     logical_operator: str | None
     def compile_json_path_final_key(self, key_transform: Any) -> str: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/fields/mixins.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/fields/related.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/related.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from collections.abc import Callable, Iterable, Sequence
 from typing import Any, Generic, Literal, TypeVar, overload
 from uuid import UUID
 
 from django.core import validators  # due to weird mypy.stubtest error
 from django.db.models.base import Model
-from django.db.models.expressions import Combinable
-from django.db.models.fields import Field, _AllLimitChoicesTo, _ErrorMessagesMapping, _FieldChoices, _LimitChoicesTo
+from django.db.models.expressions import Combinable, Expression
+from django.db.models.fields import NOT_PROVIDED, Field, _AllLimitChoicesTo, _ErrorMessagesMapping, _LimitChoicesTo
 from django.db.models.fields.mixins import FieldCacheMixin
 from django.db.models.fields.related_descriptors import ForwardManyToOneDescriptor as ForwardManyToOneDescriptor
 from django.db.models.fields.related_descriptors import ForwardOneToOneDescriptor as ForwardOneToOneDescriptor
 from django.db.models.fields.related_descriptors import ManyRelatedManager
 from django.db.models.fields.related_descriptors import ManyToManyDescriptor as ManyToManyDescriptor
 from django.db.models.fields.related_descriptors import ReverseManyToOneDescriptor as ReverseManyToOneDescriptor
 from django.db.models.fields.related_descriptors import ReverseOneToOneDescriptor as ReverseOneToOneDescriptor
 from django.db.models.fields.reverse_related import ForeignObjectRel as ForeignObjectRel
 from django.db.models.fields.reverse_related import ManyToManyRel as ManyToManyRel
 from django.db.models.fields.reverse_related import ManyToOneRel as ManyToOneRel
 from django.db.models.fields.reverse_related import OneToOneRel as OneToOneRel
 from django.db.models.query_utils import FilteredRelation, PathInfo, Q
+from django.utils.choices import _Choices
 from django.utils.functional import _StrOrPromise, cached_property
 from typing_extensions import Self
 
 RECURSIVE_RELATIONSHIP_CONSTANT: Literal["self"]
 
 def resolve_relation(scope_model: type[Model], relation: str | type[Model]) -> str | type[Model]: ...
 
@@ -52,20 +53,21 @@
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         rel: ForeignObjectRel | None = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_tablespace: str | None = ...,
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         db_comment: str | None = ...,
@@ -106,18 +108,19 @@
         name: str | None = ...,
         primary_key: bool = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         db_comment: str | None = ...,
     ) -> None: ...
@@ -162,21 +165,22 @@
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         db_comment: str | None = ...,
     ) -> None: ...
@@ -203,21 +207,22 @@
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
         null: bool = ...,
         db_index: bool = ...,
         default: Any = ...,
+        db_default: type[NOT_PROVIDED] | Expression | _ST = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         db_comment: str | None = ...,
     ) -> None: ...
@@ -269,27 +274,27 @@
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
-        choices: _FieldChoices | None = ...,
+        choices: _Choices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
         db_tablespace: str | None = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         db_comment: str | None = ...,
     ) -> None: ...
     # class access
     @overload
     def __get__(self, instance: None, owner: Any) -> ManyToManyDescriptor[_To, _Through]: ...
     # Model instance access
     @overload
-    def __get__(self, instance: Model, owner: Any) -> ManyRelatedManager[_To]: ...
+    def __get__(self, instance: Model, owner: Any) -> ManyRelatedManager[_To, _Through]: ...
     # non-Model instances
     @overload
     def __get__(self, instance: Any, owner: Any) -> Self: ...
     def get_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
     def get_reverse_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
     def contribute_to_related_class(self, cls: type[Model], related: RelatedField) -> None: ...
     def m2m_db_table(self) -> str: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/fields/related_descriptors.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/related_descriptors.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Callable, Iterable
-from typing import Any, Generic, NoReturn, TypeVar, overload
+from typing import Any, Generic, NoReturn, TypeVar, overload, type_check_only
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models.base import Model
 from django.db.models.fields import Field
 from django.db.models.fields.related import ForeignKey, ManyToManyField, RelatedField
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel, OneToOneRel
 from django.db.models.manager import BaseManager, Manager
@@ -11,15 +11,15 @@
 from django.db.models.query_utils import DeferredAttribute
 from django.utils.functional import cached_property
 from typing_extensions import Self
 
 _M = TypeVar("_M", bound=Model)
 _F = TypeVar("_F", bound=Field)
 _From = TypeVar("_From", bound=Model)
-_Through = TypeVar("_Through", bound=Model)
+_Through = TypeVar("_Through", bound=Model, default=Model)
 _To = TypeVar("_To", bound=Model)
 
 class ForeignKeyDeferredAttribute(DeferredAttribute):
     field: RelatedField
 
 class ForwardManyToOneDescriptor(Generic[_F]):
     field: _F
@@ -85,14 +85,15 @@
     @overload
     def __get__(self, instance: None, cls: Any = ...) -> Self: ...
     @overload
     def __get__(self, instance: Model, cls: Any = ...) -> RelatedManager[Any]: ...
     def __set__(self, instance: Any, value: Any) -> NoReturn: ...
 
 # Fake class, Django defines 'RelatedManager' inside a function body
+@type_check_only
 class RelatedManager(Manager[_M], Generic[_M]):
     related_val: tuple[int, ...]
     def add(self, *objs: _M | int, bulk: bool = ...) -> None: ...
     async def aadd(self, *objs: _M | int, bulk: bool = ...) -> None: ...
     def remove(self, *objs: _M | int, bulk: bool = ...) -> None: ...
     async def aremove(self, *objs: _M | int, bulk: bool = ...) -> None: ...
     def set(self, objs: QuerySet[_M] | Iterable[_M | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
@@ -120,29 +121,45 @@
     rel: ManyToManyRel  # type: ignore[assignment]
     field: ManyToManyField[_To, _Through]  # type: ignore[assignment]
     reverse: bool
     def __init__(self, rel: ManyToManyRel, reverse: bool = ...) -> None: ...
     @property
     def through(self) -> type[_Through]: ...
     @cached_property
-    def related_manager_cls(self) -> type[ManyRelatedManager[_To]]: ...  # type: ignore[override]
+    def related_manager_cls(self) -> type[ManyRelatedManager[_To, _Through]]: ...  # type: ignore[override]
     @overload  # type: ignore[override]
     def __get__(self, instance: None, cls: Any = ...) -> Self: ...
     @overload
-    def __get__(self, instance: Model, cls: Any = ...) -> ManyRelatedManager[_To]: ...
+    def __get__(self, instance: Model, cls: Any = ...) -> ManyRelatedManager[_To, _Through]: ...
 
 # Fake class, Django defines 'ManyRelatedManager' inside a function body
-class ManyRelatedManager(Manager[_M], Generic[_M]):
+@type_check_only
+class ManyRelatedManager(Manager[_To], Generic[_To, _Through]):
     related_val: tuple[int, ...]
-    def add(self, *objs: _M | int, bulk: bool = ...) -> None: ...
-    async def aadd(self, *objs: _M | int, bulk: bool = ...) -> None: ...
-    def remove(self, *objs: _M | int, bulk: bool = ...) -> None: ...
-    async def aremove(self, *objs: _M | int, bulk: bool = ...) -> None: ...
-    def set(self, objs: QuerySet[_M] | Iterable[_M | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
-    async def aset(self, objs: QuerySet[_M] | Iterable[_M | int], *, bulk: bool = ..., clear: bool = ...) -> None: ...
+    through: type[_Through]
+    def add(self, *objs: _To | int, bulk: bool = ..., through_defaults: dict[str, Any] | None = ...) -> None: ...
+    async def aadd(self, *objs: _To | int, bulk: bool = ..., through_defaults: dict[str, Any] | None = ...) -> None: ...
+    def remove(self, *objs: _To | int, bulk: bool = ...) -> None: ...
+    async def aremove(self, *objs: _To | int, bulk: bool = ...) -> None: ...
+    def set(
+        self,
+        objs: QuerySet[_To] | Iterable[_To | int],
+        *,
+        bulk: bool = ...,
+        clear: bool = ...,
+        through_defaults: dict[str, Any] | None = ...,
+    ) -> None: ...
+    async def aset(
+        self,
+        objs: QuerySet[_To] | Iterable[_To | int],
+        *,
+        bulk: bool = ...,
+        clear: bool = ...,
+        through_defaults: dict[str, Any] | None = ...,
+    ) -> None: ...
     def clear(self) -> None: ...
     async def aclear(self) -> None: ...
-    def __call__(self, *, manager: str) -> ManyRelatedManager[_M]: ...
+    def __call__(self, *, manager: str) -> ManyRelatedManager[_To, _Through]: ...
 
 def create_forward_many_to_many_manager(
-    superclass: type[BaseManager[_M]], rel: ManyToManyRel, reverse: bool
-) -> type[ManyRelatedManager[_M]]: ...
+    superclass: type[BaseManager[_To]], rel: ManyToManyRel, reverse: bool
+) -> type[ManyRelatedManager[_To, _Through]]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/fields/related_lookups.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/related_lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/fields/reverse_related.pyi` & `django_stubs-5.0.0/django-stubs/db/models/fields/reverse_related.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         related_name: str | None = ...,
         related_query_name: str | None = ...,
         limit_choices_to: _AllLimitChoicesTo | None = ...,
         parent_link: bool = ...,
         on_delete: Callable = ...,
     ) -> None: ...
     def get_related_field(self) -> Field: ...
+    def get_accessor_name(self, model: type[Model] | None = ...) -> str: ...
 
 class OneToOneRel(ManyToOneRel):
     field: OneToOneField
     def __init__(
         self,
         field: OneToOneField,
         to: type[Model] | str,
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/functions/__init__.pyi` & `django_stubs-5.0.0/django-stubs/db/models/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/functions/comparison.pyi` & `django_stubs-5.0.0/django-stubs/db/models/functions/comparison.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/functions/datetime.pyi` & `django_stubs-5.0.0/django-stubs/db/models/functions/datetime.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/functions/math.pyi` & `django_stubs-5.0.0/django-stubs/db/models/functions/math.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/functions/text.pyi` & `django_stubs-5.0.0/django-stubs/db/models/functions/text.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/functions/window.pyi` & `django_stubs-5.0.0/django-stubs/db/models/functions/window.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/indexes.pyi` & `django_stubs-5.0.0/django-stubs/db/models/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/lookups.pyi` & `django_stubs-5.0.0/django-stubs/db/models/lookups.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Iterable, Mapping
 from typing import Any, Generic, Literal, TypeVar
 
-from db.models import BooleanField
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.expressions import Expression, Func
+from django.db.models.fields import BooleanField
 from django.db.models.query_utils import RegisterLookupMixin
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType, _ParamT
 from django.utils.datastructures import OrderedSet
 from django.utils.functional import cached_property
 from typing_extensions import Self
 
 _T = TypeVar("_T")
@@ -67,16 +67,16 @@
 class FieldGetDbPrepValueIterableMixin(FieldGetDbPrepValueMixin):
     get_db_prep_lookup_value_is_iterable: Literal[True]
     def get_prep_lookup(self) -> Iterable[Any]: ...
     def resolve_expression_parameter(
         self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, sql: str, param: Any
     ) -> _AsSqlType: ...
 
-class PostgresOperatorLookup(FieldGetDbPrepValueMixin, Lookup[_T]):
-    postgres_operator: str
+class PostgresOperatorLookup(Lookup[_T]):
+    postgres_operator: str | None
     def as_postgresql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
 
 class Exact(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
 class IExact(BuiltinLookup[_T]): ...
 class GreaterThan(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
 class GreaterThanOrEqual(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
 class LessThan(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/manager.pyi` & `django_stubs-5.0.0/django-stubs/db/models/manager.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
-from collections.abc import AsyncIterator, Collection, Iterable, Iterator, MutableMapping, Sequence
+from collections.abc import AsyncIterator, Callable, Collection, Iterable, Iterator, MutableMapping, Sequence
 from typing import Any, Generic, NoReturn, TypeVar, overload
 
 from django.db.models.base import Model
 from django.db.models.expressions import Combinable, OrderBy
 from django.db.models.query import QuerySet, RawQuerySet
 from typing_extensions import Self
 
 from django_stubs_ext import ValuesQuerySet
 
 _T = TypeVar("_T", bound=Model, covariant=True)
 
 class BaseManager(Generic[_T]):
+    cache: Callable[[], Self]  # django-cacheops
     creation_counter: int
     auto_created: bool
     use_in_migrations: bool
     name: str
     model: type[_T]
     _db: str | None
     def __new__(cls, *args: Any, **kwargs: Any) -> Self: ...
@@ -64,17 +65,25 @@
     ) -> list[_T]: ...
     def bulk_update(self, objs: Iterable[_T], fields: Sequence[str], batch_size: int | None = ...) -> int: ...
     async def abulk_update(self, objs: Iterable[_T], fields: Sequence[str], batch_size: int | None = ...) -> int: ...
     def get_or_create(self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any) -> tuple[_T, bool]: ...
     async def aget_or_create(
         self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
     ) -> tuple[_T, bool]: ...
-    def update_or_create(self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any) -> tuple[_T, bool]: ...
+    def update_or_create(
+        self,
+        defaults: MutableMapping[str, Any] | None = ...,
+        create_defaults: MutableMapping[str, Any] | None = ...,
+        **kwargs: Any,
+    ) -> tuple[_T, bool]: ...
     async def aupdate_or_create(
-        self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
+        self,
+        defaults: MutableMapping[str, Any] | None = ...,
+        create_defaults: MutableMapping[str, Any] | None = ...,
+        **kwargs: Any,
     ) -> tuple[_T, bool]: ...
     def earliest(self, *fields: str | OrderBy) -> _T: ...
     async def aearliest(self, *fields: str | OrderBy) -> _T: ...
     def latest(self, *fields: str | OrderBy) -> _T: ...
     async def alatest(self, *fields: str | OrderBy) -> _T: ...
     def first(self) -> _T | None: ...
     async def afirst(self) -> _T | None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/options.pyi` & `django_stubs-5.0.0/django-stubs/db/models/options.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/query.pyi` & `django_stubs-5.0.0/django-stubs/db/models/query.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from collections.abc import AsyncIterator, Collection, Iterable, Iterator, MutableMapping, Reversible, Sequence, Sized
+from collections.abc import AsyncIterator, Collection, Iterable, Iterator, MutableMapping, Sequence, Sized
 from typing import Any, Generic, NamedTuple, TypeVar, overload
 
 from django.db.backends.utils import _ExecuteQuery
 from django.db.models import Manager
 from django.db.models.base import Model
 from django.db.models.expressions import Combinable, OrderBy
 from django.db.models.sql.query import Query, RawQuery
@@ -39,15 +39,15 @@
 
 class NamedValuesListIterable(ValuesListIterable[NamedTuple]):
     def __iter__(self) -> Iterator[NamedTuple]: ...
 
 class FlatValuesListIterable(BaseIterable[_Row]):
     def __iter__(self) -> Iterator[_Row]: ...
 
-class _QuerySet(Generic[_T, _Row], Collection[_Row], Reversible[_Row], Sized):
+class _QuerySet(Generic[_T, _Row], Iterable[_Row], Sized):
     model: type[_T]
     query: Query
     _iterable_class: type[BaseIterable]
     _result_cache: list[_Row] | None
     def __init__(
         self,
         model: type[Model] | None = ...,
@@ -94,17 +94,25 @@
     ) -> list[_T]: ...
     def bulk_update(self, objs: Iterable[_T], fields: Iterable[str], batch_size: int | None = ...) -> int: ...
     async def abulk_update(self, objs: Iterable[_T], fields: Iterable[str], batch_size: int | None = ...) -> int: ...
     def get_or_create(self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any) -> tuple[_T, bool]: ...
     async def aget_or_create(
         self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
     ) -> tuple[_T, bool]: ...
-    def update_or_create(self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any) -> tuple[_T, bool]: ...
+    def update_or_create(
+        self,
+        defaults: MutableMapping[str, Any] | None = ...,
+        create_defaults: MutableMapping[str, Any] | None = ...,
+        **kwargs: Any,
+    ) -> tuple[_T, bool]: ...
     async def aupdate_or_create(
-        self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
+        self,
+        defaults: MutableMapping[str, Any] | None = ...,
+        create_defaults: MutableMapping[str, Any] | None = ...,
+        **kwargs: Any,
     ) -> tuple[_T, bool]: ...
     def earliest(self, *fields: str | OrderBy) -> _Row: ...
     async def aearliest(self, *fields: str | OrderBy) -> _Row: ...
     def latest(self, *fields: str | OrderBy) -> _Row: ...
     async def alatest(self, *fields: str | OrderBy) -> _Row: ...
     def first(self) -> _Row | None: ...
     async def afirst(self) -> _Row | None: ...
@@ -174,15 +182,14 @@
     def ordered(self) -> bool: ...
     @property
     def db(self) -> str: ...
     def _fetch_all(self) -> None: ...
     def resolve_expression(self, *args: Any, **kwargs: Any) -> Any: ...
     def __iter__(self) -> Iterator[_Row]: ...
     def __aiter__(self) -> AsyncIterator[_Row]: ...
-    def __contains__(self, x: object) -> bool: ...
     @overload
     def __getitem__(self, i: int) -> _Row: ...
     @overload
     def __getitem__(self, s: slice) -> Self: ...
     def __reversed__(self) -> Iterator[_Row]: ...
 
 class RawQuerySet(Iterable[_T], Sized):
@@ -230,11 +237,12 @@
     def __getstate__(self) -> dict[str, Any]: ...
     def add_prefix(self, prefix: str) -> None: ...
     def get_current_prefetch_to(self, level: int) -> str: ...
     def get_current_to_attr(self, level: int) -> tuple[str, str]: ...
     def get_current_queryset(self, level: int) -> QuerySet | None: ...
 
 def prefetch_related_objects(model_instances: Iterable[_T], *related_lookups: str | Prefetch) -> None: ...
+async def aprefetch_related_objects(model_instances: Iterable[_T], *related_lookups: str | Prefetch) -> None: ...
 def get_prefetcher(instance: Model, through_attr: str, to_attr: str) -> tuple[Any, Any, bool, bool]: ...
 
 class InstanceCheckMeta(type): ...
 class EmptyQuerySet(metaclass=InstanceCheckMeta): ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/query_utils.pyi` & `django_stubs-5.0.0/django-stubs/db/models/query_utils.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import namedtuple
 from collections.abc import Collection, Iterable, Iterator, Mapping, Sequence
-from typing import Any, Literal, TypeVar
+from typing import Any, ClassVar, Literal, TypeVar
 
+from _typeshed import Incomplete
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.base import Model
 from django.db.models.expressions import BaseExpression
 from django.db.models.fields import Field
 from django.db.models.fields.mixins import FieldCacheMixin
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
@@ -36,24 +37,27 @@
         self,
         query: Query = ...,
         allow_joins: bool = ...,
         reuse: set[str] | None = ...,
         summarize: bool = ...,
         for_save: bool = ...,
     ) -> WhereNode: ...
+    def flatten(self) -> Iterator[Incomplete]: ...
+    def check(self, against: dict[str, Any], using: str = ...) -> bool: ...
     def deconstruct(self) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
 
 class DeferredAttribute:
     field: Field
     def __init__(self, field: Field) -> None: ...
+    def __get__(self, instance: Model | None, cls: type[Model] | None = None) -> Any: ...
 
 _R = TypeVar("_R", bound=type)
 
 class RegisterLookupMixin:
-    class_lookups: list[dict[Any, Any]]
+    class_lookups: ClassVar[dict[str, Any]]
     lookup_name: str
     @classmethod
     def get_lookups(cls) -> dict[str, Any]: ...
     def get_lookup(self, lookup_name: str) -> type[Lookup] | None: ...
     def get_transform(self, lookup_name: str) -> type[Transform] | None: ...
     @staticmethod
     def merge_dicts(dicts: Iterable[dict[str, Any]]) -> dict[str, Any]: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/signals.pyi` & `django_stubs-5.0.0/django-stubs/db/models/signals.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/sql/compiler.pyi` & `django_stubs-5.0.0/django-stubs/db/models/sql/compiler.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     annotation_col_map: Any
     klass_info: Any
     ordering_parts: Any
     def __init__(self, query: Query, connection: BaseDatabaseWrapper, using: str | None) -> None: ...
     col_count: int | None
     def setup_query(self, with_col_aliases: bool = ...) -> None: ...
     has_extra_select: Any
-    def pre_sql_setup(
-        self, with_col_aliases: bool = ...
-    ) -> tuple[
+    def pre_sql_setup(self, with_col_aliases: bool = ...) -> tuple[
         list[tuple[Expression, _AsSqlType, None]],
         list[tuple[Expression, tuple[str, _ParamsT, bool]]],
         list[_AsSqlType],
     ]: ...
     def get_group_by(
         self,
         select: list[tuple[BaseExpression, _AsSqlType, str | None]],
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/sql/datastructures.pyi` & `django_stubs-5.0.0/django-stubs/db/models/sql/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/sql/query.pyi` & `django_stubs-5.0.0/django-stubs/db/models/sql/query.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     select_for_update_nowait: bool
     select_for_update_skip_locked: bool
     select_for_update_of: tuple
     select_for_no_key_update: bool
     select_related: dict[str, Any] | bool
     max_depth: int
     values_select: tuple
-    annotation_select_mask: set[str] | None
+    annotation_select_mask: list[str] | None
     combinator: str | None
     combinator_all: bool
     combined_queries: tuple
     extra_select_mask: set[str] | None
     extra_tables: tuple
     extra_order_by: Sequence[Any]
     deferred_loading: tuple[set[str] | frozenset[str], bool]
@@ -195,15 +195,15 @@
     def extra_select(self) -> dict[str, Any]: ...
     def trim_start(self, names_with_path: list[tuple[str, list[PathInfo]]]) -> tuple[str, bool]: ...
     def is_nullable(self, field: Field) -> bool: ...
     def check_filterable(self, expression: Any) -> None: ...
     def build_lookup(self, lookups: Sequence[str], lhs: Expression | Query, rhs: Any) -> Lookup: ...
     def try_transform(self, lhs: Expression | Query, name: str) -> Transform: ...
     def join(
-        self, join: type[BaseTable | Join], reuse: str | None = ..., reuse_with_filtered_relation: bool = ...
+        self, join: BaseTable | Join, reuse: str | None = ..., reuse_with_filtered_relation: bool = ...
     ) -> str: ...
 
 class JoinPromoter:
     connector: str
     negated: bool
     effective_connector: str
     num_children: int
```

### Comparing `django-stubs-4.2.7/django-stubs/db/models/sql/subqueries.pyi` & `django_stubs-5.0.0/django-stubs/db/models/sql/subqueries.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/models/sql/where.pyi` & `django_stubs-5.0.0/django-stubs/db/models/sql/where.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Sequence
 from typing import Any
 
-from db.models import BooleanField
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.expressions import Expression
+from django.db.models.fields import BooleanField
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 from django.db.models.sql.query import Query
 from django.utils import tree
 from django.utils.functional import cached_property
 
 AND: str
 OR: str
```

### Comparing `django-stubs-4.2.7/django-stubs/db/transaction.pyi` & `django_stubs-5.0.0/django-stubs/db/transaction.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/db/utils.pyi` & `django_stubs-5.0.0/django-stubs/db/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/dispatch/dispatcher.pyi` & `django_stubs-5.0.0/django-stubs/dispatch/dispatcher.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,17 @@
         self, receiver: Callable, sender: object | None = ..., weak: bool = ..., dispatch_uid: Hashable | None = ...
     ) -> None: ...
     def disconnect(
         self, receiver: Callable | None = ..., sender: object | None = ..., dispatch_uid: str | None = ...
     ) -> bool: ...
     def has_listeners(self, sender: Any = ...) -> bool: ...
     def send(self, sender: Any, **named: Any) -> list[tuple[Callable, str | None]]: ...
+    async def asend(self, sender: Any, **named: Any) -> list[tuple[Callable, str | None]]: ...
     def send_robust(self, sender: Any, **named: Any) -> list[tuple[Callable, Exception | Any]]: ...
+    async def asend_robust(self, sender: Any, **named: Any) -> list[tuple[Callable, Exception | Any]]: ...
     def _live_receivers(self, sender: Any) -> list[Callable]: ...
 
 _F = TypeVar("_F", bound=Callable[..., Any])
 
 def receiver(
     signal: list[Signal] | tuple[Signal, ...] | Signal,
     *,
```

### Comparing `django-stubs-4.2.7/django-stubs/forms/__init__.pyi` & `django_stubs-5.0.0/django-stubs/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/forms/boundfield.pyi` & `django_stubs-5.0.0/django-stubs/forms/boundfield.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     def __getitem__(self, idx: slice) -> list[BoundWidget]: ...
     @property
     def errors(self) -> ErrorList: ...
     def as_widget(
         self, widget: Widget | None = ..., attrs: _AttrsT | None = ..., only_initial: bool = ...
     ) -> SafeString: ...
     def as_text(self, attrs: _AttrsT | None = ..., **kwargs: Any) -> SafeString: ...
+    def __html__(self) -> SafeString: ...
     def as_textarea(self, attrs: _AttrsT | None = ..., **kwargs: Any) -> SafeString: ...
     def as_hidden(self, attrs: _AttrsT | None = ..., **kwargs: Any) -> SafeString: ...
     @property
     def data(self) -> Any: ...
     def value(self) -> Any: ...
     def label_tag(
         self,
```

### Comparing `django-stubs-4.2.7/django-stubs/forms/fields.pyi` & `django_stubs-5.0.0/django-stubs/forms/fields.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 import datetime
 from collections.abc import Collection, Iterator, Sequence
 from decimal import Decimal
 from re import Pattern
-from typing import Any, Protocol
+from typing import Any, Protocol, type_check_only
 from uuid import UUID
 
 from django.core.files import File
 from django.core.validators import _ValidatorCallable
-from django.db.models.fields import (
-    _Choice,
-    _ChoiceNamedGroup,
-    _ChoicesCallable,
-    _ErrorMessagesDict,
-    _ErrorMessagesMapping,
-    _FieldChoices,
-)
+from django.db.models.fields import _ErrorMessagesDict, _ErrorMessagesMapping
 from django.forms.boundfield import BoundField
 from django.forms.forms import BaseForm
 from django.forms.widgets import Widget
+from django.utils.choices import CallableChoiceIterator, _Choices, _ChoicesCallable
 from django.utils.datastructures import _PropertyDescriptor
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 # Problem: attribute `widget` is always of type `Widget` after field instantiation.
 # However, on class level it can be set to `Type[Widget]` too.
 # If we annotate it as `Union[Widget, Type[Widget]]`, every code that uses field
@@ -303,41 +297,37 @@
         help_text: _StrOrPromise = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         show_hidden_initial: bool = ...,
         validators: Sequence[_ValidatorCallable] = ...,
         localize: bool = ...,
         disabled: bool = ...,
         label_suffix: str | None = ...,
+        assume_scheme: str | None = ...,
     ) -> None: ...
     def to_python(self, value: Any | None) -> str | None: ...
 
 class BooleanField(Field):
     def to_python(self, value: Any | None) -> bool: ...
     def validate(self, value: Any) -> None: ...
     def has_changed(self, initial: Any | None, data: Any | None) -> bool: ...
 
 class NullBooleanField(BooleanField):
     def to_python(self, value: Any | None) -> bool | None: ...  # type: ignore[override]
     def validate(self, value: Any) -> None: ...
 
-class CallableChoiceIterator:
-    choices_func: _ChoicesCallable
-    def __init__(self, choices_func: _ChoicesCallable) -> None: ...
-    def __iter__(self) -> Iterator[_Choice | _ChoiceNamedGroup]: ...
-
 class ChoiceField(Field):
     choices: _PropertyDescriptor[
-        _FieldChoices | _ChoicesCallable | CallableChoiceIterator,
-        _FieldChoices | CallableChoiceIterator,
+        _Choices | _ChoicesCallable | CallableChoiceIterator,
+        _Choices | CallableChoiceIterator,
     ]
     widget: _ClassLevelWidgetT
     def __init__(
         self,
         *,
-        choices: _FieldChoices | _ChoicesCallable = ...,
+        choices: _Choices | _ChoicesCallable = ...,
         required: bool = ...,
         widget: Widget | type[Widget] | None = ...,
         label: _StrOrPromise | None = ...,
         initial: Any | None = ...,
         help_text: _StrOrPromise = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         show_hidden_initial: bool = ...,
@@ -348,26 +338,27 @@
     ) -> None: ...
     # Real return type of `to_python` is `str`, but it results in errors when
     # subclassing `ModelChoiceField`: `# type: ignore[override]` is not inherited
     def to_python(self, value: Any | None) -> Any: ...
     def validate(self, value: Any) -> None: ...
     def valid_value(self, value: Any) -> bool: ...
 
+@type_check_only
 class _CoerceCallable(Protocol):
-    def __call__(self, __value: Any) -> Any: ...
+    def __call__(self, value: Any, /) -> Any: ...
 
 class TypedChoiceField(ChoiceField):
     coerce: _CoerceCallable
     empty_value: str | None
     def __init__(
         self,
         *,
         coerce: _CoerceCallable = ...,
         empty_value: str | None = ...,
-        choices: _FieldChoices | _ChoicesCallable = ...,
+        choices: _Choices | _ChoicesCallable = ...,
         required: bool = ...,
         widget: Widget | type[Widget] | None = ...,
         label: _StrOrPromise | None = ...,
         initial: Any | None = ...,
         help_text: _StrOrPromise = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         show_hidden_initial: bool = ...,
@@ -387,15 +378,15 @@
     coerce: _CoerceCallable
     empty_value: list[Any] | None
     def __init__(
         self,
         *,
         coerce: _CoerceCallable = ...,
         empty_value: list[Any] | None = ...,
-        choices: _FieldChoices | _ChoicesCallable = ...,
+        choices: _Choices | _ChoicesCallable = ...,
         required: bool = ...,
         widget: Widget | type[Widget] | None = ...,
         label: _StrOrPromise | None = ...,
         initial: Any | None = ...,
         help_text: _StrOrPromise = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         show_hidden_initial: bool = ...,
@@ -463,15 +454,15 @@
         self,
         path: str,
         *,
         match: str | None = ...,
         recursive: bool = ...,
         allow_files: bool = ...,
         allow_folders: bool = ...,
-        choices: _FieldChoices | _ChoicesCallable = ...,
+        choices: _Choices | _ChoicesCallable = ...,
         required: bool = ...,
         widget: Widget | type[Widget] | None = ...,
         label: _StrOrPromise | None = ...,
         initial: Any | None = ...,
         help_text: _StrOrPromise = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         show_hidden_initial: bool = ...,
```

### Comparing `django-stubs-4.2.7/django-stubs/forms/forms.pyi` & `django_stubs-5.0.0/django-stubs/forms/forms.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from collections.abc import Iterable, Iterator, Mapping, Sequence
+from collections.abc import Iterable, Iterator, Mapping
 from typing import Any, ClassVar
 
 from django.core.exceptions import ValidationError
 from django.forms.boundfield import BoundField
 from django.forms.fields import Field
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import ErrorDict, ErrorList, RenderableFormMixin, _DataT, _FilesT
 from django.forms.widgets import Media, MediaDefiningClass
 from django.utils.functional import _StrOrPromise, cached_property
 from django.utils.safestring import SafeString
 
 class DeclarativeFieldsMetaclass(MediaDefiningClass): ...
 
 class BaseForm(RenderableFormMixin):
-    class Meta:
-        fields: Sequence[str]
     default_renderer: BaseRenderer | type[BaseRenderer] | None
     field_order: Iterable[str] | None
     use_required_attribute: bool
     is_bound: bool
     data: _DataT
     files: _FilesT
     auto_id: bool | str
```

### Comparing `django-stubs-4.2.7/django-stubs/forms/formsets.pyi` & `django_stubs-5.0.0/django-stubs/forms/formsets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/forms/models.pyi` & `django_stubs-5.0.0/django-stubs/forms/models.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from collections.abc import Callable, Collection, Container, Iterator, Mapping, Sequence
 from typing import Any, ClassVar, Generic, Literal, TypeVar, overload
 from uuid import UUID
 
 from django.db import models
 from django.db.models import ForeignKey
 from django.db.models.base import Model
-from django.db.models.fields import _AllLimitChoicesTo, _ChoicesCallable, _FieldChoices, _LimitChoicesTo
+from django.db.models.fields import _AllLimitChoicesTo, _LimitChoicesTo
 from django.db.models.manager import Manager
 from django.db.models.query import QuerySet
-from django.forms.fields import CallableChoiceIterator, ChoiceField, Field, _ClassLevelWidgetT
+from django.forms.fields import ChoiceField, Field, _ClassLevelWidgetT
 from django.forms.forms import BaseForm, DeclarativeFieldsMetaclass
 from django.forms.formsets import BaseFormSet
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import ErrorList, _DataT, _FilesT
 from django.forms.widgets import Widget
-from django.utils.datastructures import _IndexableCollection, _ListOrTuple, _PropertyDescriptor
+from django.utils.choices import BaseChoiceIterator, CallableChoiceIterator, _Choices, _ChoicesCallable
+from django.utils.datastructures import _IndexableCollection, _PropertyDescriptor
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 ALL_FIELDS: Literal["__all__"]
 
-_Fields: TypeAlias = _ListOrTuple[str] | Literal["__all__"]
+_Fields: TypeAlias = Collection[str] | Literal["__all__"]
 _Widgets: TypeAlias = dict[str, type[Widget] | Widget]
 
 _Labels: TypeAlias = dict[str, str]
 _HelpTexts: TypeAlias = dict[str, str]
 _ErrorMessages: TypeAlias = dict[str, dict[str, str]]
 _FormFieldCallback: TypeAlias = Callable[[models.Field], Field]
 
@@ -122,15 +123,15 @@
         *,
         initial: Sequence[dict[str, Any]] | None = ...,
         **kwargs: Any,
     ) -> None: ...
     def initial_form_count(self) -> int: ...
     def get_queryset(self) -> _IndexableCollection[_M]: ...
     def save_new(self, form: _ModelFormT, commit: bool = ...) -> _M: ...
-    def save_existing(self, form: _ModelFormT, instance: _M, commit: bool = ...) -> _M: ...
+    def save_existing(self, form: _ModelFormT, obj: _M, commit: bool = ...) -> _M: ...
     def delete_existing(self, obj: _M, commit: bool = ...) -> None: ...
     saved_forms: list[_ModelFormT]
     def save_m2m(self) -> None: ...
     def save(self, commit: bool = ...) -> list[_M]: ...
     def clean(self) -> None: ...
     def validate_unique(self) -> None: ...
     def get_unique_error_message(self, unique_check: Sequence[str]) -> str: ...
@@ -238,71 +239,71 @@
     ) -> None: ...
     def clean(self, value: Any) -> Model: ...
     def has_changed(self, initial: Any, data: Any) -> bool: ...
 
 class ModelChoiceIteratorValue:
     def __init__(self, value: Any, instance: Model) -> None: ...
 
-class ModelChoiceIterator:
+class ModelChoiceIterator(BaseChoiceIterator):
     field: ModelChoiceField
     queryset: QuerySet
     def __init__(self, field: ModelChoiceField) -> None: ...
     def __iter__(self) -> Iterator[tuple[ModelChoiceIteratorValue | str, str]]: ...
     def __len__(self) -> int: ...
     def __bool__(self) -> bool: ...
     def choice(self, obj: Model) -> tuple[ModelChoiceIteratorValue, str]: ...
 
-class ModelChoiceField(ChoiceField):
+class ModelChoiceField(ChoiceField, Generic[_M]):
     disabled: bool
     help_text: _StrOrPromise
     required: bool
     show_hidden_initial: bool
     validators: list[Any]
     iterator: type[ModelChoiceIterator]
     empty_label: _StrOrPromise | None
-    queryset: QuerySet[models.Model] | None
+    queryset: QuerySet[_M] | None
     limit_choices_to: _AllLimitChoicesTo | None
     to_field_name: str | None
     def __init__(
         self,
-        queryset: None | Manager[models.Model] | QuerySet[models.Model],
+        queryset: Manager[_M] | QuerySet[_M] | None,
         *,
         empty_label: _StrOrPromise | None = ...,
         required: bool = ...,
         widget: Widget | type[Widget] | None = ...,
         label: _StrOrPromise | None = ...,
         initial: Any | None = ...,
         help_text: _StrOrPromise = ...,
         to_field_name: str | None = ...,
         limit_choices_to: _AllLimitChoicesTo | None = ...,
         blank: bool = ...,
         **kwargs: Any,
     ) -> None: ...
     def get_limit_choices_to(self) -> _LimitChoicesTo: ...
-    def label_from_instance(self, obj: Model) -> str: ...
+    def label_from_instance(self, obj: _M) -> str: ...
     choices: _PropertyDescriptor[
-        _FieldChoices | _ChoicesCallable | CallableChoiceIterator,
-        _FieldChoices | CallableChoiceIterator | ModelChoiceIterator,
+        _Choices | _ChoicesCallable | CallableChoiceIterator,
+        _Choices | CallableChoiceIterator | ModelChoiceIterator,
     ]
     def prepare_value(self, value: Any) -> Any: ...
-    def to_python(self, value: Any | None) -> Model | None: ...
-    def validate(self, value: Model | None) -> None: ...
+    def to_python(self, value: Any | None) -> _M | None: ...
+    def validate(self, value: _M | None) -> None: ...
     def has_changed(self, initial: Model | int | str | UUID | None, data: int | str | None) -> bool: ...
 
-class ModelMultipleChoiceField(ModelChoiceField):
+class ModelMultipleChoiceField(ModelChoiceField[_M]):
     disabled: bool
     empty_label: _StrOrPromise | None
     help_text: _StrOrPromise
     required: bool
     show_hidden_initial: bool
     widget: _ClassLevelWidgetT
     hidden_widget: type[Widget]
-    def __init__(self, queryset: None | Manager[Model] | QuerySet[Model], **kwargs: Any) -> None: ...
-    def to_python(self, value: Any) -> list[Model]: ...  # type: ignore[override]
-    def clean(self, value: Any) -> QuerySet[Model]: ...
+    def __init__(self, queryset: Manager[_M] | QuerySet[_M] | None, **kwargs: Any) -> None: ...
+    def to_python(self, value: Any) -> list[_M]: ...  # type: ignore[override]
+    def clean(self, value: Any) -> QuerySet[_M]: ...
     def prepare_value(self, value: Any) -> Any: ...
     def has_changed(self, initial: Collection[Any] | None, data: Collection[Any] | None) -> bool: ...  # type: ignore[override]
 
 def modelform_defines_fields(form_class: type[ModelForm]) -> bool: ...
 @overload
 def _get_foreign_key(  # type: ignore[overload-overlap]
     parent_model: type[Model], model: type[Model], fk_name: str | None = ..., can_fail: Literal[True] = ...
```

### Comparing `django-stubs-4.2.7/django-stubs/forms/renderers.pyi` & `django_stubs-5.0.0/django-stubs/forms/renderers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/forms/utils.pyi` & `django_stubs-5.0.0/django-stubs/forms/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/forms/widgets.pyi` & `django_stubs-5.0.0/django-stubs/forms/widgets.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import datetime
 from collections.abc import Iterable, Iterator, Mapping, Sequence
-from typing import Any, Literal, Protocol
+from typing import Any, Literal, Protocol, type_check_only
 
 from django.core.files.base import File
-from django.db.models.fields import _FieldChoices
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import _DataT, _FilesT
+from django.utils.choices import _Choices
 from django.utils.datastructures import _ListOrTuple
 from django.utils.safestring import SafeString
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 _OptAttrs: TypeAlias = dict[str, Any]
 
 class MediaOrderConflictWarning(RuntimeWarning): ...
 
 class Media:
     def __init__(
@@ -36,14 +36,15 @@
     needs_multipart_form: bool
     is_localized: bool
     is_required: bool
     supports_microseconds: bool
     attrs: _OptAttrs
     template_name: str
     def __init__(self, attrs: _OptAttrs | None = ...) -> None: ...
+    def __deepcopy__(self, memo: dict[int, Any]) -> Self: ...
     @property
     def is_hidden(self) -> bool: ...
     @property
     def media(self) -> Media: ...
     def subwidgets(self, name: str, value: Any, attrs: _OptAttrs = ...) -> Iterator[dict[str, Any]]: ...
     def format_value(self, value: Any) -> str | None: ...
     def get_context(self, name: str, value: Any, attrs: _OptAttrs | None) -> dict[str, Any]: ...
@@ -80,15 +81,15 @@
     render_value: bool
     input_type: str
     template_name: str
     def __init__(self, attrs: _OptAttrs | None = ..., render_value: bool = ...) -> None: ...
     def get_context(self, name: str, value: Any, attrs: _OptAttrs | None) -> dict[str, Any]: ...
 
 class HiddenInput(Input):
-    choices: _FieldChoices
+    choices: _Choices
     input_type: str
     template_name: str
 
 class MultipleHiddenInput(HiddenInput):
     template_name: str
 
 class FileInput(Input):
@@ -133,17 +134,17 @@
     template_name: str
 
 class TimeInput(DateTimeBaseInput):
     format_key: str
     template_name: str
 
 def boolean_check(v: Any) -> bool: ...
-
+@type_check_only
 class _CheckCallable(Protocol):
-    def __call__(self, __value: Any) -> bool: ...
+    def __call__(self, value: Any, /) -> bool: ...
 
 class CheckboxInput(Input):
     check_test: _CheckCallable
     input_type: str
     template_name: str
     def __init__(self, attrs: _OptAttrs | None = ..., check_test: _CheckCallable | None = ...) -> None: ...
 
@@ -151,16 +152,16 @@
     allow_multiple_selected: bool
     input_type: str | None
     template_name: str
     option_template_name: str | None
     add_id_index: bool
     checked_attribute: Any
     option_inherits_attrs: bool
-    choices: _FieldChoices
-    def __init__(self, attrs: _OptAttrs | None = ..., choices: _FieldChoices = ...) -> None: ...
+    choices: _Choices
+    def __init__(self, attrs: _OptAttrs | None = ..., choices: _Choices = ...) -> None: ...
     def subwidgets(self, name: str, value: Any, attrs: _OptAttrs = ...) -> Iterator[dict[str, Any]]: ...
     def options(self, name: str, value: list[str], attrs: _OptAttrs | None = ...) -> Iterator[dict[str, Any]]: ...
     def optgroups(
         self, name: str, value: list[str], attrs: _OptAttrs | None = ...
     ) -> list[tuple[str | None, list[dict[str, Any]], int | None]]: ...
     def get_context(self, name: str, value: Any, attrs: _OptAttrs | None) -> dict[str, Any]: ...
     def create_option(
```

### Comparing `django-stubs-4.2.7/django-stubs/http/__init__.pyi` & `django_stubs-5.0.0/django-stubs/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/http/multipartparser.pyi` & `django_stubs-5.0.0/django-stubs/http/multipartparser.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 class MultiPartParserError(Exception): ...
 class InputStreamExhausted(Exception): ...
 
 RAW: Literal["raw"]
 FILE: Literal["file"]
 FIELD: Literal["field"]
+FIELD_TYPES: frozenset[str]
 
 class MultiPartParser:
     def __init__(
         self,
         META: Mapping[str, Any],
         input_data: IO[bytes],
         upload_handlers: list[Any] | ImmutableList[Any],
```

### Comparing `django-stubs-4.2.7/django-stubs/http/request.pyi` & `django_stubs-5.0.0/django-stubs/http/request.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import datetime
 from collections.abc import Iterable, Mapping
 from io import BytesIO
 from re import Pattern
-from typing import Any, BinaryIO, Literal, NoReturn, TypeVar, overload
+from typing import Any, BinaryIO, Callable, Literal, NoReturn, TypeVar, overload, type_check_only
 
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.contrib.sessions.backends.base import SessionBase
 from django.contrib.sites.models import Site
 from django.core.files import uploadedfile, uploadhandler
 from django.urls import ResolverMatch
@@ -51,14 +52,16 @@
     _body: bytes
     _stream: BinaryIO
     # Attributes added by optional parts of Django
     # django.contrib.admin views:
     current_app: str
     # django.contrib.auth.middleware.AuthenticationMiddleware:
     user: AbstractBaseUser | AnonymousUser
+    # django.contrib.auth.middleware.AuthenticationMiddleware:
+    auser: Callable[[], AbstractBaseUser | AnonymousUser]
     # django.middleware.locale.LocaleMiddleware:
     LANGUAGE_CODE: str
     # django.contrib.sites.middleware.CurrentSiteMiddleware
     site: Site
     # django.contrib.sessions.middleware.SessionMiddleware
     session: SessionBase
     # The magic. If we instantiate HttpRequest directly somewhere, it has
@@ -71,15 +74,15 @@
     # (see comments in mypy.checkmember.type_object_type)
     # def __init__(self) -> None: ...
     def get_host(self) -> str: ...
     def get_port(self) -> str: ...
     def get_full_path(self, force_append_slash: bool = ...) -> str: ...
     def get_full_path_info(self, force_append_slash: bool = ...) -> str: ...
     def get_signed_cookie(
-        self, key: str, default: Any = ..., salt: str = ..., max_age: int | None = ...
+        self, key: str, default: Any = ..., salt: str = ..., max_age: int | datetime.timedelta | None = ...
     ) -> str | None: ...
     def get_raw_uri(self) -> str: ...
     def build_absolute_uri(self, location: str | None = ...) -> str: ...
     @property
     def scheme(self) -> str | None: ...
     def is_secure(self) -> bool: ...
     def is_ajax(self) -> bool: ...
@@ -99,14 +102,15 @@
     @cached_property
     def headers(self) -> HttpHeaders: ...
     @property
     def body(self) -> bytes: ...
     def _load_post_and_files(self) -> None: ...
     def accepts(self, media_type: str) -> bool: ...
 
+@type_check_only
 class _MutableHttpRequest(HttpRequest):
     GET: QueryDict  # type: ignore[assignment]
     POST: QueryDict  # type: ignore[assignment]
 
 _Z = TypeVar("_Z")
 
 class QueryDict(MultiValueDict[str, str]):
@@ -154,38 +158,39 @@
     def __setitem__(self, key: str | bytes, value: str | bytes) -> None: ...
     def __delitem__(self, key: str | bytes) -> None: ...
     def setlist(self, key: str | bytes, list_: Iterable[str | bytes]) -> None: ...
     def setlistdefault(self, key: str | bytes, default_list: list[str] | None = ...) -> list[str]: ...
     def appendlist(self, key: str | bytes, value: str | bytes) -> None: ...
     # Fake signature (because *args is used in source, but it fails with more that 1 argument)
     @overload
-    def pop(self, __key: str | bytes) -> str: ...
+    def pop(self, key: str | bytes, /) -> str: ...
     @overload
-    def pop(self, __key: str | bytes, __default: str | _Z = ...) -> str | _Z: ...
+    def pop(self, key: str | bytes, default: str | _Z = ..., /) -> str | _Z: ...
     def popitem(self) -> tuple[str, str]: ...
     def clear(self) -> None: ...
     def setdefault(self, key: str | bytes, default: str | bytes | None = ...) -> str: ...
     def copy(self) -> QueryDict: ...
     def urlencode(self, safe: str | None = ...) -> str: ...
 
+@type_check_only
 class _ImmutableQueryDict(QueryDict):
     _mutable: Literal[False]
     # def __init__(
     #     self, query_string: Optional[Union[str, bytes]] = ..., mutable: bool = ..., encoding: Optional[str] = ...
     # ) -> None: ...
     def __setitem__(self, key: str | bytes, value: str | bytes) -> NoReturn: ...
     def __delitem__(self, key: str | bytes) -> NoReturn: ...
     def setlist(self, key: str | bytes, list_: Iterable[str | bytes]) -> NoReturn: ...
     def setlistdefault(self, key: str | bytes, default_list: list[str] | None = ...) -> NoReturn: ...
     def appendlist(self, key: str | bytes, value: str | bytes) -> NoReturn: ...
     # Fake signature (because *args is used in source, but it fails with more that 1 argument)
     @overload
-    def pop(self, __key: str | bytes) -> NoReturn: ...
+    def pop(self, key: str | bytes, /) -> NoReturn: ...
     @overload
-    def pop(self, __key: str | bytes, __default: str | _Z = ...) -> NoReturn: ...
+    def pop(self, key: str | bytes, default: str | _Z = ..., /) -> NoReturn: ...
     def popitem(self) -> NoReturn: ...
     def clear(self) -> NoReturn: ...
     def setdefault(self, key: str | bytes, default: str | bytes | None = ...) -> NoReturn: ...
     def copy(self) -> QueryDict: ...  # type: ignore[override]
     def urlencode(self, safe: str | None = ...) -> str: ...
     # Fakes for convenience (for `request.GET` and `request.POST`). If dict
     # was created by Django, there is no chance to hit `List[object]` (empty list)
```

### Comparing `django-stubs-4.2.7/django-stubs/http/response.pyi` & `django_stubs-5.0.0/django-stubs/http/response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     def get(self, header: str, alternate: str) -> str: ...
     @overload
     def get(self, header: str, alternate: None = ...) -> str | None: ...
     def set_cookie(
         self,
         key: str,
         value: str = ...,
-        max_age: int | None = ...,
+        max_age: int | datetime.timedelta | None = ...,
         expires: str | datetime.datetime | None = ...,
         path: str = ...,
         domain: str | None = ...,
         secure: bool = ...,
         httponly: bool = ...,
         samesite: Literal["Lax", "Strict", "None", False] | None = ...,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/middleware/cache.pyi` & `django_stubs-5.0.0/django-stubs/middleware/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/middleware/common.pyi` & `django_stubs-5.0.0/django-stubs/middleware/common.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/middleware/csrf.pyi` & `django_stubs-5.0.0/django-stubs/middleware/csrf.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 invalid_token_chars_re: Pattern[str]
 
 REASON_BAD_ORIGIN: str
 REASON_NO_REFERER: str
 REASON_BAD_REFERER: str
 REASON_NO_CSRF_COOKIE: str
 REASON_CSRF_TOKEN_MISSING: str
-REASON_BAD_TOKEN: str
 REASON_MALFORMED_REFERER: str
 REASON_INSECURE_REFERER: str
 
 REASON_INCORRECT_LENGTH: str
 REASON_INVALID_CHARACTERS: str
 
 CSRF_SECRET_LENGTH: int
```

### Comparing `django-stubs-4.2.7/django-stubs/middleware/security.pyi` & `django_stubs-5.0.0/django-stubs/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/__init__.pyi` & `django_stubs-5.0.0/django-stubs/template/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/backends/base.pyi` & `django_stubs-5.0.0/django-stubs/template/backends/base.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Iterator, Mapping
-from typing import Any, Protocol
+from typing import Any, Protocol, type_check_only
 
 from django.http.request import HttpRequest
 from django.template.base import Context
 from django.utils.functional import cached_property
 from django.utils.safestring import SafeString
 
 class BaseEngine:
@@ -12,16 +12,17 @@
     app_dirs: bool
     def __init__(self, params: Mapping[str, Any]) -> None: ...
     @property
     def app_dirname(self) -> str | None: ...
     def from_string(self, template_code: str) -> _EngineTemplate: ...
     def get_template(self, template_name: str) -> _EngineTemplate: ...
     @cached_property
-    def template_dirs(self) -> tuple[str]: ...
+    def template_dirs(self) -> tuple[str, ...]: ...
     def iter_template_filenames(self, template_name: str) -> Iterator[str]: ...
 
+@type_check_only
 class _EngineTemplate(Protocol):
     def render(
         self,
         context: Context | dict[str, Any] | None = ...,
         request: HttpRequest | None = ...,
     ) -> SafeString: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/template/backends/django.pyi` & `django_stubs-5.0.0/django-stubs/template/backends/django.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/backends/jinja2.pyi` & `django_stubs-5.0.0/django-stubs/template/backends/jinja2.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/base.pyi` & `django_stubs-5.0.0/django-stubs/template/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,15 @@
     def __init__(
         self,
         template_string: Template | str,
         origin: Origin | None = ...,
         name: str | None = ...,
         engine: Engine | None = ...,
     ) -> None: ...
-    def __iter__(self) -> Iterator[Node]: ...
-    def render(self, context: Context | dict[str, Any] | None) -> SafeString: ...
+    def render(self, context: Context) -> SafeString: ...
     def compile_nodelist(self) -> NodeList: ...
     def get_exception_info(self, exception: Exception, token: Token) -> dict[str, Any]: ...
 
 def linebreak_iter(template_source: str) -> Iterator[int]: ...
 
 class Token:
     contents: str
```

### Comparing `django-stubs-4.2.7/django-stubs/template/context.pyi` & `django_stubs-5.0.0/django-stubs/template/context.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/context_processors.pyi` & `django_stubs-5.0.0/django-stubs/template/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/defaultfilters.pyi` & `django_stubs-5.0.0/django-stubs/template/defaultfilters.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 def wordcount(value: str) -> int: ...
 def wordwrap(value: str, arg: SafeString | int) -> str: ...
 def ljust(value: str, arg: SafeString | int) -> str: ...
 def rjust(value: str, arg: SafeString | int) -> str: ...
 def center(value: str, arg: SafeString | int) -> str: ...
 def cut(value: str, arg: str) -> str: ...
 def escape_filter(value: str) -> SafeString: ...
+def escapeseq(value: list[str]) -> list[SafeString]: ...
 def force_escape(value: str) -> SafeString: ...
 def linebreaks_filter(value: str, autoescape: bool = ...) -> SafeString: ...
 def linebreaksbr(value: str, autoescape: bool = ...) -> SafeString: ...
 def safe(value: str) -> SafeString: ...
 def safeseq(value: list[str]) -> list[SafeString]: ...
 def striptags(value: str) -> str: ...
 def dictsort(value: Any, arg: int | str) -> Any: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/template/defaulttags.pyi` & `django_stubs-5.0.0/django-stubs/template/defaulttags.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/engine.pyi` & `django_stubs-5.0.0/django-stubs/template/engine.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/library.pyi` & `django_stubs-5.0.0/django-stubs/template/library.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/loader.pyi` & `django_stubs-5.0.0/django-stubs/template/loader.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/loader_tags.pyi` & `django_stubs-5.0.0/django-stubs/templatetags/i18n.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,92 @@
-import collections
 from typing import Any
 
-from django.template.base import FilterExpression, NodeList, Origin, Parser, Token
+from django.template import Node
+from django.template.base import FilterExpression, NodeList, Parser, Token
 from django.template.context import Context
-from django.utils.safestring import SafeString
-
-from .base import Node, Template
 
 register: Any
-BLOCK_CONTEXT_KEY: str
 
-class BlockContext:
-    blocks: collections.defaultdict[str, list[BlockNode]]
-    def __init__(self) -> None: ...
-    def add_blocks(self, blocks: dict[str, BlockNode]) -> None: ...
-    def pop(self, name: str) -> BlockNode: ...
-    def push(self, name: str, block: BlockNode) -> None: ...
-    def get_block(self, name: str) -> BlockNode: ...
-
-class BlockNode(Node):
-    context: Context
-    name: str
-    nodelist: NodeList
-    origin: Origin
-    parent: Node | None
-    token: Token
-    def __init__(self, name: str, nodelist: NodeList, parent: Node | None = ...) -> None: ...
-    def render(self, context: Context) -> SafeString: ...
-    def super(self) -> SafeString: ...
-
-class ExtendsNode(Node):
-    origin: Origin
-    token: Token
-    must_be_first: bool
-    context_key: str
-    nodelist: NodeList
-    parent_name: FilterExpression | Node
-    template_dirs: list[Any] | None
-    blocks: dict[str, BlockNode]
+class GetAvailableLanguagesNode(Node):
+    variable: str
+    def __init__(self, variable: str) -> None: ...
+    def render(self, context: Context) -> str: ...
+
+class GetLanguageInfoNode(Node):
+    lang_code: FilterExpression
+    variable: str
+    def __init__(self, lang_code: FilterExpression, variable: str) -> None: ...
+    def render(self, context: Context) -> str: ...
+
+class GetLanguageInfoListNode(Node):
+    languages: FilterExpression
+    variable: str
+    def __init__(self, languages: FilterExpression, variable: str) -> None: ...
+    def get_language_info(self, language: Any) -> Any: ...
+    def render(self, context: Context) -> str: ...
+
+class GetCurrentLanguageNode(Node):
+    variable: str
+    def __init__(self, variable: str) -> None: ...
+    def render(self, context: Context) -> str: ...
+
+class GetCurrentLanguageBidiNode(Node):
+    variable: str
+    def __init__(self, variable: str) -> None: ...
+    def render(self, context: Context) -> str: ...
+
+class TranslateNode(Node):
+    noop: bool
+    asvar: str | None
+    message_context: FilterExpression | None
+    filter_expression: FilterExpression
     def __init__(
-        self, nodelist: NodeList, parent_name: FilterExpression | Node, template_dirs: list[Any] | None = ...
+        self,
+        filter_expression: FilterExpression,
+        noop: bool,
+        asvar: str | None = ...,
+        message_context: FilterExpression | None = ...,
     ) -> None: ...
-    def find_template(self, template_name: str, context: Context) -> Template: ...
-    def get_parent(self, context: Context) -> Template: ...
-    def render(self, context: Context) -> Any: ...
-
-class IncludeNode(Node):
-    origin: Origin
-    token: Token
-    context_key: str
-    template: FilterExpression
+    def render(self, context: Context) -> str: ...
+
+class BlockTranslateNode(Node):
     extra_context: dict[str, FilterExpression]
-    isolated_context: bool
+    singular: list[Token]
+    plural: list[Token]
+    countervar: str | None
+    counter: FilterExpression | None
+    message_context: FilterExpression | None
+    trimmed: bool
+    asvar: str | None
     def __init__(
         self,
-        template: FilterExpression,
-        *args: Any,
-        extra_context: Any | None = ...,
-        isolated_context: bool = ...,
-        **kwargs: Any,
+        extra_context: dict[str, FilterExpression],
+        singular: list[Token],
+        plural: list[Token] = ...,
+        countervar: str | None = ...,
+        counter: FilterExpression | None = ...,
+        message_context: FilterExpression | None = ...,
+        trimmed: bool = ...,
+        asvar: str | None = ...,
+        tag_name: str = ...,
     ) -> None: ...
-    def render(self, context: Context) -> SafeString: ...
+    def render_token_list(self, tokens: list[Token]) -> tuple[str, list[str]]: ...
+    def render(self, context: Context, nested: bool = ...) -> str: ...
 
-def do_block(parser: Parser, token: Token) -> BlockNode: ...
-def construct_relative_path(current_template_name: str | None, relative_name: str) -> str: ...
-def do_extends(parser: Parser, token: Token) -> ExtendsNode: ...
-def do_include(parser: Parser, token: Token) -> IncludeNode: ...
+class LanguageNode(Node):
+    nodelist: NodeList
+    language: FilterExpression
+    def __init__(self, nodelist: NodeList, language: FilterExpression) -> None: ...
+    def render(self, context: Context) -> str: ...
+
+def do_get_available_languages(parser: Parser, token: Token) -> GetAvailableLanguagesNode: ...
+def do_get_language_info(parser: Parser, token: Token) -> GetLanguageInfoNode: ...
+def do_get_language_info_list(parser: Parser, token: Token) -> GetLanguageInfoListNode: ...
+def language_name(lang_code: str) -> str: ...
+def language_name_translated(lang_code: str) -> str: ...
+def language_name_local(lang_code: str) -> str: ...
+def language_bidi(lang_code: str) -> bool: ...
+def do_get_current_language(parser: Parser, token: Token) -> GetCurrentLanguageNode: ...
+def do_get_current_language_bidi(parser: Parser, token: Token) -> GetCurrentLanguageBidiNode: ...
+def do_translate(parser: Parser, token: Token) -> TranslateNode: ...
+def do_block_translate(parser: Parser, token: Token) -> BlockTranslateNode: ...
+def language(parser: Parser, token: Token) -> LanguageNode: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/template/loaders/cached.pyi` & `django_stubs-5.0.0/django-stubs/template/loaders/cached.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/loaders/filesystem.pyi` & `django_stubs-5.0.0/django-stubs/template/loaders/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/response.pyi` & `django_stubs-5.0.0/django-stubs/template/response.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/smartif.pyi` & `django_stubs-5.0.0/django-stubs/template/smartif.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/template/utils.pyi` & `django_stubs-5.0.0/django-stubs/template/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/templatetags/cache.pyi` & `django_stubs-5.0.0/django-stubs/templatetags/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/templatetags/static.pyi` & `django_stubs-5.0.0/django-stubs/templatetags/static.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/templatetags/tz.pyi` & `django_stubs-5.0.0/django-stubs/templatetags/tz.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from datetime import datetime
+from datetime import datetime, tzinfo
 from typing import Any
 
 from django.template import Node
 from django.template.base import FilterExpression, NodeList, Parser, Token
-from django.utils.timezone import _TzInfoT
 
 register: Any
 
 class datetimeobject(datetime): ...
 
 def localtime(value: datetime | str | None) -> Any: ...
 def utc(value: datetime | str | None) -> Any: ...
-def do_timezone(value: datetime | str | None, arg: _TzInfoT | str | None) -> Any: ...
+def do_timezone(value: datetime | str | None, arg: tzinfo | str | None) -> Any: ...
 
 class LocalTimeNode(Node):
     nodelist: NodeList
     use_tz: bool
     def __init__(self, nodelist: NodeList, use_tz: bool) -> None: ...
 
 class TimezoneNode(Node):
```

### Comparing `django-stubs-4.2.7/django-stubs/test/__init__.pyi` & `django_stubs-5.0.0/django-stubs/test/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/test/client.pyi` & `django_stubs-5.0.0/django-stubs/test/testcases.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,302 +1,270 @@
-from collections.abc import Awaitable, Callable, Iterable, Iterator, Mapping
-from http.cookies import SimpleCookie
-from io import BytesIO, IOBase
-from json import JSONEncoder
-from re import Pattern
+import threading
+import unittest
+from collections.abc import Callable, Collection, Generator, Iterable, Iterator, Mapping, Sequence
+from contextlib import contextmanager
 from types import TracebackType
-from typing import Any, Generic, NoReturn, TypeVar
+from typing import Any, overload
 
-from django.contrib.auth.base_user import AbstractBaseUser
-from django.contrib.sessions.backends.base import SessionBase
-from django.core.handlers.asgi import ASGIRequest
-from django.core.handlers.base import BaseHandler
-from django.core.handlers.wsgi import WSGIRequest
-from django.http.request import HttpRequest
-from django.http.response import HttpResponseBase
+from django.core.exceptions import ImproperlyConfigured
+from django.core.handlers.wsgi import WSGIHandler
+from django.core.servers.basehttp import ThreadedWSGIServer, WSGIRequestHandler
+from django.db import connections as connections
+from django.db.backends.base.base import BaseDatabaseWrapper
+from django.db.models.base import Model
+from django.db.models.query import QuerySet, RawQuerySet
+from django.forms import BaseFormSet, Form
+from django.forms.fields import EmailField
+from django.http import HttpRequest
+from django.http.response import FileResponse, HttpResponseBase
 from django.template.base import Template
-from django.test.utils import ContextList
-from django.urls import ResolverMatch
-from typing_extensions import TypeAlias
-
-BOUNDARY: str
-MULTIPART_CONTENT: str
-CONTENT_TYPE_RE: Pattern[str]
-JSON_CONTENT_TYPE_RE: Pattern[str]
-
-class RedirectCycleError(Exception):
-    last_response: HttpResponseBase
-    redirect_chain: list[tuple[str, int]]
-    def __init__(self, message: str, last_response: HttpResponseBase) -> None: ...
-
-class FakePayload(IOBase):
-    read_started: bool
-    def __init__(self, initial_bytes: bytes | str | None = ...) -> None: ...
-    def __len__(self) -> int: ...
-    def read(self, size: int = ...) -> bytes: ...
-    def readline(self, size: int | None = ..., /) -> bytes: ...
-    def write(self, content: bytes | str) -> None: ...
-
-_T = TypeVar("_T")
-
-def closing_iterator_wrapper(iterable: Iterable[_T], close: Callable[[], Any]) -> Iterator[_T]: ...
-def conditional_content_removal(request: HttpRequest, response: HttpResponseBase) -> HttpResponseBase: ...
-
-class _WSGIResponse(HttpResponseBase):
-    wsgi_request: WSGIRequest
-
-class _ASGIResponse(HttpResponseBase):
-    asgi_request: ASGIRequest
-
-class ClientHandler(BaseHandler):
-    enforce_csrf_checks: bool
-    def __init__(self, enforce_csrf_checks: bool = ..., *args: Any, **kwargs: Any) -> None: ...
-    def __call__(self, environ: dict[str, Any]) -> _WSGIResponse: ...
-
-class AsyncClientHandler(BaseHandler):
-    enforce_csrf_checks: bool
-    def __init__(self, enforce_csrf_checks: bool = ..., *args: Any, **kwargs: Any) -> None: ...
-    async def __call__(self, scope: dict[str, Any]) -> _ASGIResponse: ...
-
-def encode_multipart(boundary: str, data: dict[str, Any]) -> bytes: ...
-def encode_file(boundary: str, key: str, file: Any) -> list[bytes]: ...
-
-_GetDataType: TypeAlias = (
-    Mapping[str, str | bytes | int | Iterable[str | bytes | int]]
-    | Iterable[tuple[str, str | bytes | int | Iterable[str | bytes | int]]]
-    | None
-)
-
-class _RequestFactory(Generic[_T]):
-    json_encoder: type[JSONEncoder]
-    defaults: dict[str, str]
-    cookies: SimpleCookie
-    errors: BytesIO
-    def __init__(
-        self, *, json_encoder: type[JSONEncoder] = ..., headers: Mapping[str, Any] | None = ..., **defaults: Any
+from django.test.client import AsyncClient, Client
+from django.test.html import Element
+from django.test.utils import CaptureQueriesContext, ContextList
+from django.utils.functional import classproperty
+from typing_extensions import Self
+
+def to_list(value: Any) -> list[Any]: ...
+def assert_and_parse_html(self: Any, html: str, user_msg: str, msg: str) -> Element: ...
+
+class _AssertNumQueriesContext(CaptureQueriesContext):
+    test_case: SimpleTestCase
+    num: int
+    def __init__(self, test_case: Any, num: Any, connection: BaseDatabaseWrapper) -> None: ...
+
+class _AssertTemplateUsedContext:
+    test_case: SimpleTestCase
+    template_name: str
+    rendered_templates: list[Template]
+    context: ContextList
+    def __init__(self, test_case: Any, template_name: Any) -> None: ...
+    def on_template_render(self, sender: Any, signal: Any, template: Any, context: Any, **kwargs: Any) -> None: ...
+    def test(self) -> None: ...
+    def message(self) -> str: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None: ...
-    def request(self, **request: Any) -> _T: ...
-    def get(
-        self,
-        path: str,
-        data: _GetDataType = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _T: ...
-    def post(
-        self,
-        path: str,
-        data: Any = ...,
-        content_type: str = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _T: ...
-    def head(
-        self, path: str, data: Any = ..., secure: bool = ..., *, headers: Mapping[str, Any] | None = ..., **extra: Any
-    ) -> _T: ...
-    def trace(self, path: str, secure: bool = ..., *, headers: Mapping[str, Any] | None = ..., **extra: Any) -> _T: ...
-    def options(
-        self,
-        path: str,
-        data: dict[str, str] | str = ...,
-        content_type: str = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _T: ...
-    def put(
-        self,
-        path: str,
-        data: Any = ...,
-        content_type: str = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _T: ...
-    def patch(
-        self,
-        path: str,
-        data: Any = ...,
-        content_type: str = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _T: ...
-    def delete(
-        self,
-        path: str,
-        data: Any = ...,
-        content_type: str = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _T: ...
-    def generic(
-        self,
-        method: str,
-        path: str,
-        data: Any = ...,
-        content_type: str | None = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _T: ...
-
-class RequestFactory(_RequestFactory[WSGIRequest]): ...
-class _AsyncRequestFactory(_RequestFactory[_T]): ...
-class AsyncRequestFactory(_AsyncRequestFactory[ASGIRequest]): ...
-
-# fakes to distinguish WSGIRequest and ASGIRequest
-class _MonkeyPatchedWSGIResponse(_WSGIResponse):
-    def json(self) -> Any: ...
-    request: dict[str, Any]
+
+class _AssertTemplateNotUsedContext(_AssertTemplateUsedContext): ...
+
+class _DatabaseFailure:
+    wrapped: Any
+    message: str
+    def __init__(self, wrapped: Any, message: str) -> None: ...
+    def __call__(self) -> None: ...
+
+class SimpleTestCase(unittest.TestCase):
+    client_class: type[Client]
     client: Client
-    templates: list[Template]
-    context: ContextList | dict[str, Any]
-    content: bytes
-    resolver_match: ResolverMatch
-    redirect_chain: list[tuple[str, int]]
-
-class _MonkeyPatchedASGIResponse(_ASGIResponse):
-    def json(self) -> Any: ...
-    request: dict[str, Any]
-    client: AsyncClient
-    templates: list[Template]
-    context: ContextList | dict[str, Any]
-    content: bytes
-    resolver_match: ResolverMatch
-    redirect_chain: list[tuple[str, int]]
-
-class ClientMixin:
-    def store_exc_info(self, **kwargs: Any) -> None: ...
-    def check_exception(self, response: HttpResponseBase) -> NoReturn: ...
-    @property
-    def session(self) -> SessionBase: ...
-    def login(self, **credentials: Any) -> bool: ...
-    def force_login(self, user: AbstractBaseUser, backend: str | None = ...) -> None: ...
-    def logout(self) -> None: ...
-
-class Client(ClientMixin, _RequestFactory[_MonkeyPatchedWSGIResponse]):
-    handler: ClientHandler
-    raise_request_exception: bool
-    exc_info: tuple[type[BaseException], BaseException, TracebackType] | None
-    extra: dict[str, Any] | None
-    headers: dict[str, Any]
-    def __init__(
+    async_client_class: type[AsyncClient]
+    async_client: AsyncClient
+    allow_database_queries: bool
+    # TODO: str -> Literal['__all__']
+    databases: set[str] | str
+    def __call__(self, result: unittest.TestResult | None = ...) -> None: ...
+    def settings(self, **kwargs: Any) -> Any: ...
+    def modify_settings(self, **kwargs: Any) -> Any: ...
+    def assertRedirects(
+        self,
+        response: HttpResponseBase,
+        expected_url: str,
+        status_code: int = ...,
+        target_status_code: int = ...,
+        msg_prefix: str = ...,
+        fetch_redirect_response: bool = ...,
+    ) -> None: ...
+    def assertURLEqual(
+        self,
+        url1: str | Any,  # Any for reverse_lazy() support
+        url2: str | Any,
+        msg_prefix: str = ...,
+    ) -> None: ...
+    def assertContains(
+        self,
+        response: HttpResponseBase,
+        text: bytes | int | str,
+        count: int | None = ...,
+        status_code: int = ...,
+        msg_prefix: str = ...,
+        html: bool = ...,
+    ) -> None: ...
+    def assertNotContains(
+        self,
+        response: HttpResponseBase,
+        text: bytes | str,
+        status_code: int = ...,
+        msg_prefix: str = ...,
+        html: bool = ...,
+    ) -> None: ...
+    def assertFormError(
+        self,
+        form: Form,
+        field: str | None,
+        errors: list[str] | str,
+        msg_prefix: str = ...,
+    ) -> None: ...
+    # assertFormsetError (lowercase "set") deprecated in Django 4.2
+    def assertFormsetError(
         self,
-        enforce_csrf_checks: bool = ...,
-        raise_request_exception: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **defaults: Any,
-    ) -> None: ...
-    def request(self, **request: Any) -> _MonkeyPatchedWSGIResponse: ...
-    def get(  # type: ignore[override]
-        self,
-        path: str,
-        data: _GetDataType = ...,
-        follow: bool = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _MonkeyPatchedWSGIResponse: ...
-    def post(  # type: ignore[override]
-        self,
-        path: str,
-        data: Any = ...,
-        content_type: str = ...,
-        follow: bool = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _MonkeyPatchedWSGIResponse: ...
-    def head(  # type: ignore[override]
-        self,
-        path: str,
-        data: Any = ...,
-        follow: bool = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _MonkeyPatchedWSGIResponse: ...
-    def options(  # type: ignore[override]
-        self,
-        path: str,
-        data: dict[str, str] | str = ...,
-        content_type: str = ...,
-        follow: bool = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _MonkeyPatchedWSGIResponse: ...
-    def put(  # type: ignore[override]
-        self,
-        path: str,
-        data: Any = ...,
-        content_type: str = ...,
-        follow: bool = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _MonkeyPatchedWSGIResponse: ...
-    def patch(  # type: ignore[override]
-        self,
-        path: str,
-        data: Any = ...,
-        content_type: str = ...,
-        follow: bool = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _MonkeyPatchedWSGIResponse: ...
-    def delete(  # type: ignore[override]
-        self,
-        path: str,
-        data: Any = ...,
-        content_type: str = ...,
-        follow: bool = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _MonkeyPatchedWSGIResponse: ...
-    def trace(  # type: ignore[override]
-        self,
-        path: str,
-        data: Any = ...,
-        follow: bool = ...,
-        secure: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **extra: Any,
-    ) -> _MonkeyPatchedWSGIResponse: ...
-
-class AsyncClient(ClientMixin, _AsyncRequestFactory[Awaitable[_MonkeyPatchedASGIResponse]]):
-    handler: AsyncClientHandler
-    raise_request_exception: bool
-    exc_info: Any
-    extra: dict[str, Any] | None
-    headers: dict[str, Any]
+        formset: BaseFormSet,
+        form_index: int | None,
+        field: str | None,
+        errors: list[str] | str,
+        msg_prefix: str = ...,
+    ) -> None: ...
+    def assertFormSetError(
+        self,
+        formset: BaseFormSet,
+        form_index: int | None,
+        field: str | None,
+        errors: list[str] | str,
+        msg_prefix: str = ...,
+    ) -> None: ...
+    def assertTemplateUsed(
+        self,
+        response: HttpResponseBase | str | None = ...,
+        template_name: str | None = ...,
+        msg_prefix: str = ...,
+        count: int | None = ...,
+    ) -> _AssertTemplateUsedContext | None: ...
+    def assertTemplateNotUsed(
+        self, response: HttpResponseBase | str = ..., template_name: str | None = ..., msg_prefix: str = ...
+    ) -> _AssertTemplateNotUsedContext | None: ...
+    def assertRaisesMessage(
+        self, expected_exception: type[Exception], expected_message: str, *args: Any, **kwargs: Any
+    ) -> Any: ...
+    def assertWarnsMessage(
+        self, expected_warning: type[Exception], expected_message: str, *args: Any, **kwargs: Any
+    ) -> Any: ...
+    def assertFieldOutput(
+        self,
+        fieldclass: type[EmailField],
+        valid: dict[str, str],
+        invalid: dict[str, list[str]],
+        field_args: Iterable[Any] | None = ...,
+        field_kwargs: Mapping[str, Any] | None = ...,
+        empty_value: str = ...,
+    ) -> Any: ...
+    def assertHTMLEqual(self, html1: str, html2: str, msg: str | None = ...) -> None: ...
+    def assertHTMLNotEqual(self, html1: str, html2: str, msg: str | None = ...) -> None: ...
+    def assertInHTML(self, needle: str, haystack: str, count: int | None = ..., msg_prefix: str = ...) -> None: ...
+    def assertJSONEqual(
+        self,
+        raw: str,
+        expected_data: dict[str, Any] | list[Any] | str | int | float | bool | None,
+        msg: str | None = ...,
+    ) -> None: ...
+    def assertJSONNotEqual(
+        self,
+        raw: str,
+        expected_data: dict[str, Any] | list[Any] | str | int | float | bool | None,
+        msg: str | None = ...,
+    ) -> None: ...
+    def assertXMLEqual(self, xml1: str, xml2: str, msg: str | None = ...) -> None: ...
+    def assertXMLNotEqual(self, xml1: str, xml2: str, msg: str | None = ...) -> None: ...
+
+class TransactionTestCase(SimpleTestCase):
+    reset_sequences: bool
+    available_apps: Any
+    fixtures: Any
+    multi_db: bool
+    serialized_rollback: bool
+    # assertQuerysetEqual (lowercase "set") deprecated in Django 4.2
+    def assertQuerysetEqual(
+        self,
+        qs: Iterator[Any] | list[Model] | QuerySet | RawQuerySet,
+        values: Collection[Any],
+        transform: Callable[[Model], Any] | type[str] = ...,
+        ordered: bool = ...,
+        msg: str | None = ...,
+    ) -> None: ...
+    def assertQuerySetEqual(
+        self,
+        qs: Iterator[Any] | list[Model] | QuerySet | RawQuerySet,
+        values: Collection[Any],
+        transform: Callable[[Model], Any] | type[str] | None = ...,
+        ordered: bool = ...,
+        msg: str | None = ...,
+    ) -> None: ...
+    @overload
+    def assertNumQueries(self, num: int, func: None = ..., *, using: str = ...) -> _AssertNumQueriesContext: ...
+    @overload
+    def assertNumQueries(
+        self, num: int, func: Callable[..., Any], *args: Any, using: str = ..., **kwargs: Any
+    ) -> None: ...
+
+class TestCase(TransactionTestCase):
+    @classmethod
+    def setUpTestData(cls) -> None: ...
+    @classmethod
+    @contextmanager
+    def captureOnCommitCallbacks(
+        cls, *, using: str = ..., execute: bool = ...
+    ) -> Generator[list[Callable[[], Any]], None, None]: ...
+
+class CheckCondition:
+    conditions: Sequence[tuple[Callable, str]]
+    def __init__(self, *conditions: tuple[Callable, str]) -> None: ...
+    def add_condition(self, condition: Callable, reason: str) -> CheckCondition: ...
+    def __get__(self, instance: None, cls: type[TransactionTestCase] | None = ...) -> bool: ...
+
+def skipIfDBFeature(*features: Any) -> Callable: ...
+def skipUnlessDBFeature(*features: Any) -> Callable: ...
+def skipUnlessAnyDBFeature(*features: Any) -> Callable: ...
+
+class QuietWSGIRequestHandler(WSGIRequestHandler): ...
+
+class FSFilesHandler(WSGIHandler):
+    application: Any
+    base_url: Any
+    def __init__(self, application: Any) -> None: ...
+    def file_path(self, url: Any) -> str: ...
+    def serve(self, request: HttpRequest) -> FileResponse: ...
+
+class _StaticFilesHandler(FSFilesHandler):
+    def get_base_dir(self) -> str: ...
+    def get_base_url(self) -> str: ...
+
+class _MediaFilesHandler(FSFilesHandler):
+    def get_base_dir(self) -> str: ...
+    def get_base_url(self) -> str: ...
+
+class LiveServerThread(threading.Thread):
+    host: str
+    port: int
+    is_ready: threading.Event
+    error: ImproperlyConfigured | None
+    static_handler: type[WSGIHandler]
+    connections_override: dict[str, BaseDatabaseWrapper]
     def __init__(
         self,
-        enforce_csrf_checks: bool = ...,
-        raise_request_exception: bool = ...,
-        *,
-        headers: Mapping[str, Any] | None = ...,
-        **defaults: Any,
+        host: str,
+        static_handler: type[WSGIHandler],
+        connections_override: dict[str, BaseDatabaseWrapper] = ...,
+        port: int = ...,
     ) -> None: ...
-    async def request(self, **request: Any) -> _MonkeyPatchedASGIResponse: ...
+    httpd: ThreadedWSGIServer
+    def terminate(self) -> None: ...
+
+class LiveServerTestCase(TransactionTestCase):
+    host: str
+    port: int
+    server_thread_class: type[Any]
+    server_thread: Any
+    static_handler: Any
+    @classproperty
+    def live_server_url(cls: Any) -> str: ...
+    @classproperty
+    def allowed_host(cls: Any) -> str: ...
+
+class SerializeMixin:
+    lockfile: Any
+    @classmethod
+    def setUpClass(cls) -> None: ...
+    @classmethod
+    def tearDownClass(cls) -> None: ...
+
+def connections_support_transactions(aliases: Iterable[str] | None = ...) -> bool: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/test/html.pyi` & `django_stubs-5.0.0/django-stubs/test/html.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 class RootElement(Element):
     def __init__(self) -> None: ...
 
 class HTMLParseError(Exception): ...
 
 class Parser(HTMLParser):
-    SELF_CLOSING_TAGS: Any
     root: Any
     open_tags: Any
     element_positions: Any
     def __init__(self) -> None: ...
     def error(self, msg: str) -> HTMLParseError: ...
     def format_position(self, position: Any = ..., element: Any = ...) -> str: ...
     @property
```

### Comparing `django-stubs-4.2.7/django-stubs/test/runner.pyi` & `django_stubs-5.0.0/django-stubs/test/runner.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     def check_subtest_picklable(self, test: Any, subtest: Any) -> None: ...
     def stop_if_failfast(self) -> None: ...
     def stop(self) -> None: ...
     def startTestRun(self) -> None: ...
     def stopTestRun(self) -> None: ...
     def startTest(self, test: Any) -> None: ...
     def stopTest(self, test: Any) -> None: ...
+    def addDuration(self, test: Any, elapsed: Any) -> None: ...
     def addError(self, test: Any, err: Any) -> None: ...
     def addFailure(self, test: Any, err: Any) -> None: ...
     def addSubTest(self, test: Any, subtest: Any, err: Any) -> None: ...
     def addSuccess(self, test: Any) -> None: ...
     def addSkip(self, test: Any, reason: Any) -> None: ...
     def addExpectedFailure(self, test: Any, err: Any) -> None: ...
     def addUnexpectedSuccess(self, test: Any) -> None: ...
@@ -78,14 +79,15 @@
     runner_class: Any
     subsuites: list[TestSuite]
     processes: int
     failfast: bool
     buffer: bool
     initial_settings: Any
     serialized_contents: Any
+    used_aliases: set[str] | None
     def __init__(
         self, subsuites: list[TestSuite], processes: int, failfast: bool = ..., buffer: bool = ...
     ) -> None: ...
     def run(self, result: Any) -> Any: ...  # type: ignore[override]
 
 class DiscoverRunner:
     test_suite: type[TestSuite]
@@ -128,40 +130,39 @@
         test_name_patterns: list[str] | None = ...,
         pdb: bool = ...,
         buffer: bool = ...,
         enable_faulthandler: bool = ...,
         timing: bool = ...,
         shuffle: int | Literal[False] = ...,
         logger: logging.Logger | None = ...,
+        durations: int | None = ...,
         **kwargs: Any,
     ) -> None: ...
     @classmethod
     def add_arguments(cls, parser: ArgumentParser) -> None: ...
     @property
     def shuffle_seed(self) -> int | None: ...
     def log(self, msg: str, level: int | None) -> None: ...
     def setup_test_environment(self, **kwargs: Any) -> None: ...
     def setup_shuffler(self) -> None: ...
     @contextmanager
     def load_with_patterns(self) -> Iterator[None]: ...
     def load_tests_for_label(self, label: str, discover_kwargs: dict[str, str]) -> TestSuite: ...
-    def build_suite(
-        self, test_labels: Sequence[str] = ..., extra_tests: list[Any] | None = ..., **kwargs: Any
-    ) -> TestSuite: ...
+    def build_suite(self, test_labels: Sequence[str] | None = ..., **kwargs: Any) -> TestSuite: ...
     def setup_databases(self, **kwargs: Any) -> list[tuple[BaseDatabaseWrapper, str, bool]]: ...
     def get_resultclass(self) -> type[TextTestResult] | None: ...
     def get_test_runner_kwargs(self) -> dict[str, Any]: ...
     def run_checks(self, databases: set[str]) -> None: ...
     def run_suite(self, suite: TestSuite, **kwargs: Any) -> TextTestResult: ...
     def teardown_databases(self, old_config: list[tuple[BaseDatabaseWrapper, str, bool]], **kwargs: Any) -> None: ...
     def teardown_test_environment(self, **kwargs: Any) -> None: ...
     def suite_result(self, suite: TestSuite, result: TextTestResult, **kwargs: Any) -> int: ...
     def _get_databases(self, suite: TestSuite) -> set[str]: ...
     def get_databases(self, suite: TestSuite) -> set[str]: ...
-    def run_tests(self, test_labels: list[str], extra_tests: list[Any] | None = ..., **kwargs: Any) -> int: ...
+    def run_tests(self, test_labels: list[str], **kwargs: Any) -> int: ...
 
 def is_discoverable(label: str) -> bool: ...
 def reorder_suite(
     suite: TestSuite, classes: tuple[type[TestCase], type[SimpleTestCase]], reverse: bool = ...
 ) -> TestSuite: ...
 def partition_suite_by_type(
     suite: TestSuite, classes: tuple[type[TestCase], type[SimpleTestCase]], bins: list[OrderedSet], reverse: bool = ...
```

### Comparing `django-stubs-4.2.7/django-stubs/test/selenium.pyi` & `django_stubs-5.0.0/django-stubs/test/selenium.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/test/signals.pyi` & `django_stubs-5.0.0/django-stubs/test/signals.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/test/utils.pyi` & `django_stubs-5.0.0/django-stubs/test/utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import decimal
 from collections.abc import Callable, Iterable, Iterator, Mapping
 from contextlib import AbstractContextManager, contextmanager
 from decimal import Decimal
 from io import StringIO
 from logging import Logger
 from types import TracebackType
-from typing import Any, Protocol, SupportsIndex, TypeVar
+from typing import Any, Protocol, SupportsIndex, TypeVar, type_check_only
 
 from django.apps.registry import Apps
 from django.conf import LazySettings, Settings
 from django.core.checks.registry import CheckRegistry
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.query_utils import RegisterLookupMixin
@@ -139,14 +139,15 @@
 @contextmanager
 def freeze_time(t: float) -> Iterator[None]: ...
 def tag(*tags: str) -> Callable[[_C], _C]: ...
 
 _Signature: TypeAlias = str
 _TestDatabase: TypeAlias = tuple[str, list[str]]
 
+@type_check_only
 class TimeKeeperProtocol(Protocol):
     @contextmanager
     def timed(self, name: Any) -> Iterator[None]: ...
     def print_results(self) -> None: ...
 
 def dependency_ordered(
     test_databases: Iterable[tuple[_Signature, _TestDatabase]], dependencies: Mapping[str, list[str]]
```

### Comparing `django-stubs-4.2.7/django-stubs/urls/__init__.pyi` & `django_stubs-5.0.0/django-stubs/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/urls/base.pyi` & `django_stubs-5.0.0/django-stubs/urls/base.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from collections.abc import Callable, Sequence
 from typing import Any, Literal
 
+from django.http.response import HttpResponse
 from django.urls.resolvers import ResolverMatch
 
 def resolve(path: str, urlconf: str | None = ...) -> ResolverMatch: ...
 def reverse(
-    viewname: Callable | str | None,
+    viewname: Callable[..., HttpResponse] | str | None,
     urlconf: str | None = ...,
     args: Sequence[Any] | None = ...,
     kwargs: dict[str, Any] | None = ...,
     current_app: str | None = ...,
 ) -> str: ...
 
 reverse_lazy: Any
```

### Comparing `django-stubs-4.2.7/django-stubs/urls/conf.pyi` & `django_stubs-5.0.0/django-stubs/urls/conf.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Callable, Sequence
 from types import ModuleType
-from typing import Any, overload
+from typing import Any, Coroutine, overload
 
 from django.urls import URLPattern, URLResolver, _AnyURL
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 from ..conf.urls import IncludedURLConf
 from ..http.response import HttpResponseBase
@@ -17,26 +17,40 @@
 
 # path()
 @overload
 def path(
     route: _StrOrPromise, view: Callable[..., HttpResponseBase], kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLPattern: ...
 @overload
+def path(
+    route: _StrOrPromise,
+    view: Callable[..., Coroutine[Any, Any, HttpResponseBase]],
+    kwargs: dict[str, Any] = ...,
+    name: str = ...,
+) -> URLPattern: ...
+@overload
 def path(route: _StrOrPromise, view: IncludedURLConf, kwargs: dict[str, Any] = ..., name: str = ...) -> URLResolver: ...
 @overload
 def path(
     route: _StrOrPromise, view: Sequence[URLResolver | str], kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLResolver: ...
 
 # re_path()
 @overload
 def re_path(
     route: _StrOrPromise, view: Callable[..., HttpResponseBase], kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLPattern: ...
 @overload
 def re_path(
+    route: _StrOrPromise,
+    view: Callable[..., Coroutine[Any, Any, HttpResponseBase]],
+    kwargs: dict[str, Any] = ...,
+    name: str = ...,
+) -> URLPattern: ...
+@overload
+def re_path(
     route: _StrOrPromise, view: IncludedURLConf, kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLResolver: ...
 @overload
 def re_path(
     route: _StrOrPromise, view: Sequence[URLResolver | str], kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLResolver: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/urls/resolvers.pyi` & `django_stubs-5.0.0/django-stubs/urls/resolvers.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections.abc import Callable, Iterator, Sequence
 from re import Pattern
 from types import ModuleType
 from typing import Any, overload
 
 from django.core.checks.messages import CheckMessage
 from django.urls import _AnyURL
-from django.urls.converters import UUIDConverter
 from django.utils.datastructures import MultiValueDict
 from django.utils.functional import cached_property
 from typing_extensions import TypeAlias
 
 class ResolverMatch:
     func: Callable
     args: tuple[Any, ...]
@@ -55,69 +54,69 @@
 
 class CheckURLMixin:
     def describe(self) -> str: ...
 
 class RegexPattern(CheckURLMixin):
     regex: LocaleRegexDescriptor
     name: str | None
-    converters: dict[Any, Any]
+    converters: dict[str, Any]
     def __init__(self, regex: str, name: str | None = ..., is_endpoint: bool = ...) -> None: ...
     def match(self, path: str) -> tuple[str, tuple, dict[str, str]] | None: ...
     def check(self) -> list[CheckMessage]: ...
 
 class RoutePattern(CheckURLMixin):
     regex: LocaleRegexDescriptor
     name: str | None
-    converters: dict[str, UUIDConverter]
+    converters: dict[str, Any]
     def __init__(self, route: str, name: str | None = ..., is_endpoint: bool = ...) -> None: ...
     def match(self, path: str) -> tuple[str, tuple, dict[str, int | str]] | None: ...
     def check(self) -> list[CheckMessage]: ...
 
 class LocalePrefixPattern:
     prefix_default_language: bool
-    converters: dict[Any, Any]
+    converters: dict[str, Any]
     def __init__(self, prefix_default_language: bool = ...) -> None: ...
     @property
     def regex(self) -> Pattern[str]: ...
     @property
     def language_prefix(self) -> str: ...
     def match(self, path: str) -> tuple[str, tuple, dict[str, Any]] | None: ...
     def check(self) -> list[CheckMessage]: ...
     def describe(self) -> str: ...
 
 class URLPattern:
     pattern: _Pattern
     callback: Callable
-    default_args: dict[str, str] | None
+    default_args: dict[str, Any]
     name: str | None
     def __init__(
         self,
         pattern: _Pattern,
         callback: Callable,
-        default_args: dict[str, str] | None = ...,
+        default_args: dict[str, Any] | None = ...,
         name: str | None = ...,
     ) -> None: ...
     def check(self) -> list[CheckMessage]: ...
     def resolve(self, path: str) -> ResolverMatch | None: ...
     @cached_property
     def lookup_str(self) -> str: ...
 
 class URLResolver:
     pattern: _Pattern
-    urlconf_name: str | None | Sequence[_AnyURL]
+    urlconf_name: str | Sequence[_AnyURL] | ModuleType
     callback: None
     default_kwargs: dict[str, Any]
     namespace: str | None
     app_name: str | None
     _local: Any
     _reverse_dict: MultiValueDict
     def __init__(
         self,
         pattern: _Pattern,
-        urlconf_name: str | None | Sequence[_AnyURL],
+        urlconf_name: str | Sequence[_AnyURL] | ModuleType,
         default_kwargs: dict[str, Any] | None = ...,
         app_name: str | None = ...,
         namespace: str | None = ...,
     ) -> None: ...
     @property
     def reverse_dict(self) -> MultiValueDict: ...
     @property
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/archive.pyi` & `django_stubs-5.0.0/django-stubs/utils/archive.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/autoreload.pyi` & `django_stubs-5.0.0/django-stubs/utils/autoreload.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/cache.pyi` & `django_stubs-5.0.0/django-stubs/utils/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/connection.pyi` & `django_stubs-5.0.0/django-stubs/utils/connection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/crypto.pyi` & `django_stubs-5.0.0/django-stubs/utils/crypto.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/datastructures.pyi` & `django_stubs-5.0.0/django-stubs/utils/datastructures.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from collections.abc import Collection, Iterable, Iterator, Mapping, MutableMapping, MutableSet
-from typing import Any, Generic, NoReturn, Protocol, TypeVar, overload
+from typing import Any, Generic, NoReturn, Protocol, TypeVar, overload, type_check_only
 
 from _typeshed import Incomplete
 from typing_extensions import Self, TypeAlias
 
 _K = TypeVar("_K")
 _V = TypeVar("_V")
 _Z = TypeVar("_Z")
 _I = TypeVar("_I", covariant=True)
 
 # Unfortunately, there's often check `if isinstance(var, (list, tuple))` in django
 # codebase. So we need sometimes to declare exactly list or tuple.
 _ListOrTuple: TypeAlias = list[_K] | tuple[_K, ...] | tuple[()]  # noqa: PYI047
 
+@type_check_only
 class _PropertyDescriptor(Generic[_K, _V]):
     """
     This helper property descriptor allows defining asynmetric getter/setters
     which mypy currently doesn't support with either:
 
         class HttpResponse:
             @property
@@ -31,15 +32,16 @@
             def _set_content(...): ...
             content = property(_get_content, _set_content)
     """
 
     def __get__(self, instance: Any, owner: Any | None) -> _V: ...
     def __set__(self, instance: Any, value: _K) -> None: ...
 
-class _IndexableCollection(Protocol[_I], Collection[_I]):
+@type_check_only
+class _IndexableCollection(Protocol[_I], Collection[_I]):  # noqa: PYI046
     @overload
     def __getitem__(self, index: int) -> _I: ...
     @overload
     def __getitem__(self, index: slice) -> Self: ...
 
 class OrderedSet(MutableSet[_K]):
     dict: dict[_K, None]
@@ -88,18 +90,19 @@
     def __deepcopy__(self, memo: MutableMapping[int, Incomplete]) -> Self: ...
 
 class ImmutableList(tuple[_V, ...]):
     warning: str
     def __new__(cls, *args: Any, warning: str = ..., **kwargs: Any) -> Self: ...
     def complain(self, *args: Any, **kwargs: Any) -> NoReturn: ...
 
+@type_check_only
 class _ItemCallable(Protocol[_V]):
     """Don't mess with arguments when assigning in class body in stub"""
 
-    def __call__(self, __value: _V) -> _V: ...
+    def __call__(self, value: _V, /) -> _V: ...
 
 class DictWrapper(dict[str, _V]):
     func: _ItemCallable[_V]
     prefix: str
     @overload
     def __init__(self, data: Mapping[str, _V], func: _ItemCallable[_V], prefix: str) -> None: ...
     @overload
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/dateformat.pyi` & `django_stubs-5.0.0/django-stubs/utils/dateformat.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from datetime import date
+from datetime import date, tzinfo
 from datetime import datetime as builtin_datetime
 from datetime import time as builtin_time
 from re import Pattern
 from typing import Any, Literal
 
-from django.utils.timezone import _TzInfoT
-
 re_formatchars: Pattern[str]
 re_escaped: Pattern[str]
 
 class Formatter:
     def format(self, formatstr: str) -> str: ...
 
 class TimeFormat(Formatter):
     data: builtin_datetime | builtin_time
-    timezone: _TzInfoT | None
+    timezone: tzinfo | None
     def __init__(self, obj: builtin_datetime | builtin_time) -> None: ...
     def a(self) -> str: ...
     def A(self) -> str: ...
     def e(self) -> str: ...
     def f(self) -> int | str: ...
     def g(self) -> int: ...
     def G(self) -> int: ...
@@ -30,15 +28,15 @@
     def s(self) -> str: ...
     def T(self) -> str: ...
     def u(self) -> str: ...
     def Z(self) -> int | Literal[""]: ...
 
 class DateFormat(TimeFormat):
     data: builtin_datetime | date | builtin_time  # type: ignore[assignment]
-    timezone: _TzInfoT | None
+    timezone: tzinfo | None
     year_days: Any
     def __init__(self, obj: builtin_datetime | builtin_time | date) -> None: ...
     def b(self) -> str: ...
     def c(self) -> str: ...
     def d(self) -> str: ...
     def D(self) -> str: ...
     def E(self) -> str: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/deprecation.pyi` & `django_stubs-5.0.0/django-stubs/utils/deprecation.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections.abc import Awaitable, Callable
-from typing import Any, Protocol
+from typing import Any, Protocol, type_check_only
 
 from django.http.request import HttpRequest
 from django.http.response import HttpResponseBase
 from typing_extensions import TypeAlias
 
-class RemovedInDjango50Warning(DeprecationWarning): ...
-class RemovedInDjango51Warning(PendingDeprecationWarning): ...
+class RemovedInDjango51Warning(DeprecationWarning): ...
+class RemovedInDjango60Warning(PendingDeprecationWarning): ...
 
-RemovedInNextVersionWarning: TypeAlias = RemovedInDjango50Warning
-RemovedAfterNextVersionWarning: TypeAlias = RemovedInDjango51Warning
+RemovedInNextVersionWarning: TypeAlias = RemovedInDjango51Warning
+RemovedAfterNextVersionWarning: TypeAlias = RemovedInDjango60Warning
 
 class warn_about_renamed_method:
     class_name: str
     old_method_name: str
     new_method_name: str
     deprecation_warning: type[DeprecationWarning]
     def __init__(
@@ -26,19 +26,21 @@
     def __new__(cls, name: Any, bases: Any, attrs: Any) -> type: ...
 
 class DeprecationInstanceCheck(type):
     alternative: str
     deprecation_warning: type[Warning]
     def __instancecheck__(self, instance: Any) -> bool: ...
 
+@type_check_only
 class _GetResponseCallable(Protocol):
-    def __call__(self, __request: HttpRequest) -> HttpResponseBase: ...
+    def __call__(self, request: HttpRequest, /) -> HttpResponseBase: ...
 
+@type_check_only
 class _AsyncGetResponseCallable(Protocol):
-    def __call__(self, __request: HttpRequest) -> Awaitable[HttpResponseBase]: ...
+    def __call__(self, request: HttpRequest, /) -> Awaitable[HttpResponseBase]: ...
 
 class MiddlewareMixin:
     sync_capable: bool
     async_capable: bool
 
     get_response: _GetResponseCallable | _AsyncGetResponseCallable
     def __init__(self, get_response: _GetResponseCallable | _AsyncGetResponseCallable) -> None: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/encoding.pyi` & `django_stubs-5.0.0/django-stubs/utils/encoding.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/feedgenerator.pyi` & `django_stubs-5.0.0/django-stubs/utils/feedgenerator.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/formats.pyi` & `django_stubs-5.0.0/django-stubs/utils/formats.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/functional.pyi` & `django_stubs-5.0.0/django-stubs/utils/functional.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from collections.abc import Callable, Sequence
+from collections.abc import Callable
 
 # Mypy has special handling for functools.cached_property, reuse typeshed's definition instead of defining our own
 from functools import cached_property as cached_property
-from typing import Any, Generic, Protocol, SupportsIndex, TypeVar, overload
+from typing import Any, Generic, Protocol, SupportsIndex, TypeVar, overload, type_check_only
 
 from django.db.models.base import Model
 from typing_extensions import Self, TypeAlias
 
 _T = TypeVar("_T")
 
 # Promise is only subclassed by a proxy class defined in the lazy function
@@ -16,30 +16,30 @@
     def __reduce__(self) -> tuple[Any, tuple[Any]]: ...
     def __lt__(self, other: Any) -> bool: ...
     def __mod__(self, rhs: Any) -> Any: ...
     def __add__(self, other: Any) -> Any: ...
     def __radd__(self, other: Any) -> Any: ...
     def __deepcopy__(self, memo: Any) -> Self: ...
 
-class _StrPromise(Promise, Sequence[str]):
-    def __add__(self, __s: str) -> str: ...
-    # Incompatible with Sequence.__contains__
-    def __contains__(self, __o: str) -> bool: ...  # type: ignore[override]
-    def __ge__(self, __x: str) -> bool: ...
-    def __getitem__(self, __i: SupportsIndex | slice) -> str: ...
-    def __gt__(self, __x: str) -> bool: ...
-    def __le__(self, __x: str) -> bool: ...
+@type_check_only
+class _StrPromise(Promise):
+    def __add__(self, s: str, /) -> str: ...
+    def __contains__(self, o: str, /) -> bool: ...
+    def __ge__(self, x: str, /) -> bool: ...
+    def __getitem__(self, i: SupportsIndex | slice, /) -> str: ...
+    def __gt__(self, x: str, /) -> bool: ...
+    def __le__(self, x: str, /) -> bool: ...
     # __len__ needed here because it defined abstract in Sequence[str]
     def __len__(self) -> int: ...
-    def __lt__(self, __x: str) -> bool: ...
-    def __mod__(self, __x: Any) -> str: ...
-    def __mul__(self, __n: SupportsIndex) -> str: ...
-    def __rmul__(self, __n: SupportsIndex) -> str: ...
+    def __lt__(self, x: str, /) -> bool: ...
+    def __mod__(self, x: Any, /) -> str: ...
+    def __mul__(self, n: SupportsIndex, /) -> str: ...
+    def __rmul__(self, n: SupportsIndex, /) -> str: ...
     # Mypy requires this for the attribute hook to take effect
-    def __getattribute__(self, __name: str) -> Any: ...
+    def __getattribute__(self, name: str, /) -> Any: ...
 
 _StrOrPromise: TypeAlias = str | _StrPromise  # noqa: PYI047
 _C = TypeVar("_C", bound=Callable)
 
 def lazy(func: _C, *resultclasses: Any) -> _C: ...
 def lazystr(text: Any) -> _StrPromise: ...
 def keep_lazy(*resultclasses: Any) -> Callable: ...
@@ -91,18 +91,19 @@
 
 class classproperty(Generic[_Get]):
     fget: Callable[[Any], _Get] | None
     def __init__(self, method: Callable[[Any], _Get] | None = ...) -> None: ...
     def __get__(self, instance: Any | None, cls: type[Any] | None = ...) -> _Get: ...
     def getter(self, method: Callable[[Any], _Get]) -> classproperty[_Get]: ...
 
-class _Getter(Protocol[_Get]):
+@type_check_only
+class _Getter(Protocol[_Get]):  # noqa: PYI046
     """Type fake to declare some read-only properties (until `property` builtin is generic)
 
     We can use something like `Union[_Getter[str], str]` in base class to avoid errors
     when redefining attribute with property or property with attribute.
     """
 
     @overload
-    def __get__(self, __instance: None, __typeobj: type[Any] | None) -> Self: ...
+    def __get__(self, instance: None, typeobj: type[Any] | None, /) -> Self: ...
     @overload
-    def __get__(self, __instance: Any, __typeobj: type[Any] | None) -> _Get: ...
+    def __get__(self, instance: Any, typeobj: type[Any] | None, /) -> _Get: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/html.pyi` & `django_stubs-5.0.0/django-stubs/utils/html.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from re import Pattern
 from typing import Any
 
 from _typeshed import Incomplete
 from django.utils.functional import SimpleLazyObject, _StrOrPromise
 from django.utils.safestring import SafeData, SafeString
 
+VOID_ELEMENTS: set[str]
+
 def escape(text: Any) -> SafeString: ...
 def escapejs(value: Any) -> SafeString: ...
 def json_script(value: Any, element_id: str | None = ..., encoder: type[JSONEncoder] | None = ...) -> SafeString: ...
 
 # conditional_escape could use a protocol to be more precise, see https://github.com/typeddjango/django-stubs/issues/1474
 def conditional_escape(text: _StrOrPromise | SafeData) -> SafeString: ...
 def format_html(format_string: str, *args: Any, **kwargs: Any) -> SafeString: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/http.pyi` & `django_stubs-5.0.0/django-stubs/utils/http.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 RFC1123_DATE: Pattern[str]
 RFC850_DATE: Pattern[str]
 ASCTIME_DATE: Pattern[str]
 RFC3986_GENDELIMS: str
 RFC3986_SUBDELIMS: str
 
 def urlencode(
-    query: Mapping[str, str | bytes | int | Iterable[str | bytes | int]]
-    | Iterable[tuple[str, str | bytes | int | Iterable[str | bytes | int]]]
-    | None,
+    query: (
+        Mapping[str, str | bytes | int | Iterable[str | bytes | int]]
+        | Iterable[tuple[str, str | bytes | int | Iterable[str | bytes | int]]]
+        | None
+    ),
     doseq: bool = ...,
 ) -> str: ...
 def http_date(epoch_seconds: float | None = ...) -> str: ...
 def parse_http_date(date: str) -> int: ...
 def parse_http_date_safe(date: str) -> int | None: ...
 def base36_to_int(s: str) -> int: ...
 def int_to_base36(i: int) -> str: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/jslex.pyi` & `django_stubs-5.0.0/django-stubs/utils/jslex.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/log.pyi` & `django_stubs-5.0.0/django-stubs/utils/log.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/regex_helper.pyi` & `django_stubs-5.0.0/django-stubs/utils/regex_helper.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/safestring.pyi` & `django_stubs-5.0.0/django-stubs/utils/safestring.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/termcolors.pyi` & `django_stubs-5.0.0/django-stubs/utils/termcolors.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from collections.abc import Callable, Mapping, Sequence
-from typing import Any
+from collections.abc import Callable, Sequence
+from typing import Any, Literal
 
-color_names: Sequence
-foreground: Mapping[str, str]
-background: Mapping[str, str]
-RESET: str
-opt_dict: Mapping[str, str]
+color_names: tuple[str, ...]
+foreground: dict[str, str]
+background: dict[str, str]
+RESET: Literal["0"]
+opt_dict: dict[str, str]
 
-def colorize(text: str | None = ..., opts: Sequence[str] = ..., **kwargs: Any) -> str: ...
-def make_style(opts: tuple = ..., **kwargs: Any) -> Callable: ...
+def colorize(text: str | None = ..., opts: Sequence[str] = ..., *, fg: str = ..., bg: str = ...) -> str: ...
+def make_style(opts: Sequence[str] = ..., *, fg: str = ..., bg: str = ...) -> Callable[[str | None], str]: ...
 
 NOCOLOR_PALETTE: str
 DARK_PALETTE: str
 LIGHT_PALETTE: str
 PALETTES: Any
 DEFAULT_PALETTE: str
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/text.pyi` & `django_stubs-5.0.0/django-stubs/utils/text.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 from collections.abc import Callable, Iterable, Iterator
 from io import BytesIO
-from re import Pattern
+from re import Match, Pattern
 from typing import ClassVar, TypeVar, overload
 
 from django.db.models.base import Model
 from django.utils.functional import SimpleLazyObject, _StrOrPromise
 
 _StrOrPromiseT = TypeVar("_StrOrPromiseT", bound=_StrOrPromise)
 _StrOrPromiseOrNoneT = TypeVar("_StrOrPromiseOrNoneT", bound=_StrOrPromise | None)
 
 def capfirst(x: _StrOrPromiseOrNoneT) -> _StrOrPromiseOrNoneT: ...
 
-re_words: Pattern[str]
+re_notag: Pattern[str]
+re_prt: Pattern[str]
+
+class WordsRegex:
+    @staticmethod
+    def search(text: str, pos: int) -> Match | FakeMatch: ...
+
+class FakeMatch:
+    def __init__(self, text: str, end: int) -> None: ...
+    def __getitem__(self, group: int) -> str | None: ...
+    def end(self, group: int = 0) -> int: ...
+
+re_words: type[WordsRegex]
 re_chars: Pattern[str]
 re_tag: Pattern[str]
 re_newlines: Pattern[str]
 re_camel_case: Pattern[str]
 
 def wrap(text: _StrOrPromiseT, width: int) -> _StrOrPromiseT: ...
+def add_truncation_text(text: str, truncate: str | None = ...) -> str: ...
 
 class Truncator(SimpleLazyObject):
     MAX_LENGTH_HTML: ClassVar[int]
     def __init__(self, text: Model | str) -> None: ...
-    def add_truncation_text(self, text: str, truncate: str | None = ...) -> str: ...
     def chars(self, num: int, truncate: str | None = ..., html: bool = ...) -> str: ...
     def words(self, num: int, truncate: str | None = ..., html: bool = ...) -> str: ...
 
 def get_valid_filename(name: _StrOrPromiseT) -> _StrOrPromiseT: ...
 @overload
 def get_text_list(list_: list[str], last_word: str = ...) -> str: ...
 @overload
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/timezone.pyi` & `django_stubs-5.0.0/django-stubs/utils/timezone.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,40 @@
 from contextlib import ContextDecorator
 from datetime import date, datetime, time, timedelta, timezone, tzinfo
 from types import TracebackType
-from typing import Any, Literal, overload
+from typing import Literal, overload
 
-import pytz
-from pytz import BaseTzInfo
-from typing_extensions import TypeAlias, TypeGuard
-
-_PytzTzInfoT: TypeAlias = pytz.tzinfo.BaseTzInfo | pytz._FixedOffset
-
-_TzInfoT: TypeAlias = _PytzTzInfoT | tzinfo
-
-utc: Any
+import zoneinfo  # type: ignore[import-not-found,unused-ignore]
 
 def get_fixed_timezone(offset: timedelta | int) -> timezone: ...
-def get_default_timezone() -> BaseTzInfo: ...
+def get_default_timezone() -> zoneinfo.ZoneInfo: ...
 def get_default_timezone_name() -> str: ...
-
-# Strictly speaking, it is possible to activate() a non-pytz timezone,
-# in which case BaseTzInfo is incorrect. However, this is unlikely,
-# so we use it anyway, to keep things ergonomic for most users.
-def get_current_timezone() -> BaseTzInfo: ...
+def get_current_timezone() -> zoneinfo.ZoneInfo: ...
 def get_current_timezone_name() -> str: ...
-def activate(timezone: _TzInfoT | str) -> None: ...
+def activate(timezone: tzinfo | str) -> None: ...
 def deactivate() -> None: ...
 
 class override(ContextDecorator):
-    timezone: str | _TzInfoT | None
-    old_timezone: _TzInfoT | None
-    def __init__(self, timezone: str | _TzInfoT | None) -> None: ...
+    timezone: str | tzinfo | None
+    old_timezone: tzinfo | None
+    def __init__(self, timezone: str | tzinfo | None) -> None: ...
     def __enter__(self) -> None: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None: ...
 
-def localtime(value: datetime | None = ..., timezone: _TzInfoT | None = ...) -> datetime: ...
-def localdate(value: datetime | None = ..., timezone: _TzInfoT | None = ...) -> date: ...
+def localtime(value: datetime | None = ..., timezone: tzinfo | None = ...) -> datetime: ...
+def localdate(value: datetime | None = ..., timezone: tzinfo | None = ...) -> date: ...
 def now() -> datetime: ...
 @overload
 def is_aware(value: time) -> Literal[False]: ...
 @overload
 def is_aware(value: datetime) -> bool: ...
 @overload
 def is_naive(value: time) -> Literal[True]: ...
 @overload
 def is_naive(value: datetime) -> bool: ...
-def make_aware(value: datetime, timezone: _TzInfoT | None = ..., is_dst: bool | None = ...) -> datetime: ...
-def make_naive(value: datetime, timezone: _TzInfoT | None = ...) -> datetime: ...
-def _is_pytz_zone(tz: _TzInfoT) -> TypeGuard[_PytzTzInfoT]: ...
+def make_aware(value: datetime, timezone: tzinfo | None = ...) -> datetime: ...
+def make_naive(value: datetime, timezone: tzinfo | None = ...) -> datetime: ...
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/translation/__init__.pyi` & `django_stubs-5.0.0/django-stubs/utils/translation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/translation/trans_null.pyi` & `django_stubs-5.0.0/django-stubs/utils/translation/trans_null.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/translation/trans_real.pyi` & `django_stubs-5.0.0/django-stubs/utils/translation/trans_real.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import gettext as gettext_module
 from collections.abc import Iterator
 from gettext import NullTranslations
 from re import Pattern
 
 # switch to tuple once https://github.com/python/mypy/issues/11098 is fixed
-from typing import Any, Literal, Protocol, TypeVar
+from typing import Any, Literal, Protocol, TypeVar, type_check_only
 
 from django.http.request import HttpRequest
 from typing_extensions import TypeAlias
 
 CONTEXT_SEPARATOR: Literal["\x04"]
 ACCEPT_LANGUAGE_HEADER_MAX_LENGTH: int
 
 accept_language_re: Pattern[str]
 language_code_re: Pattern[str]
 language_code_prefix_re: Pattern[str]
 
+@type_check_only
 class _PluralCallable(Protocol):
-    def __call__(self, __n: int) -> int: ...
+    def __call__(self, n: int, /) -> int: ...
 
 def reset_cache(*, setting: str, **kwargs: Any) -> None: ...
 
 # switch to tuple once https://github.com/python/mypy/issues/11098 is fixed
 _KeyT: TypeAlias = str | tuple[str, int]
 
 _Z = TypeVar("_Z")
```

### Comparing `django-stubs-4.2.7/django-stubs/utils/tree.pyi` & `django_stubs-5.0.0/django-stubs/utils/tree.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/utils/version.pyi` & `django_stubs-5.0.0/django-stubs/utils/version.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/views/debug.pyi` & `django_stubs-5.0.0/django-stubs/views/debug.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/views/decorators/http.pyi` & `django_stubs-5.0.0/django-stubs/views/decorators/http.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/views/defaults.pyi` & `django_stubs-5.0.0/django-stubs/views/defaults.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/views/generic/__init__.pyi` & `django_stubs-5.0.0/django-stubs/views/generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/views/generic/base.pyi` & `django_stubs-5.0.0/django-stubs/views/generic/base.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 from collections.abc import Callable, Sequence
-from typing import Any
+from typing import Any, Mapping
 
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse, HttpResponseBase
 from django.utils.functional import _Getter
 
 logger: logging.Logger
 
 class ContextMixin:
-    extra_context: dict[str, Any] | None
+    extra_context: Mapping[str, Any] | None
     def get_context_data(self, **kwargs: Any) -> dict[str, Any]: ...
 
 class View:
     http_method_names: Sequence[str]
     request: HttpRequest
     args: Any
     kwargs: Any
```

### Comparing `django-stubs-4.2.7/django-stubs/views/generic/dates.pyi` & `django_stubs-5.0.0/django-stubs/views/generic/dates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/views/generic/detail.pyi` & `django_stubs-5.0.0/django-stubs/views/generic/detail.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/views/generic/edit.pyi` & `django_stubs-5.0.0/django-stubs/views/generic/edit.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,11 @@
     object: _M
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse: ...
     def delete(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse: ...
     def get_success_url(self) -> str: ...
 
 class BaseDeleteView(Generic[_M, _ModelFormT], DeletionMixin[_M], FormMixin[_ModelFormT], BaseDetailView[_M]):
     object: _M
-    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
 
 class DeleteView(Generic[_M, _ModelFormT], SingleObjectTemplateResponseMixin, BaseDeleteView[_M, _ModelFormT]):
     object: _M
     template_name_suffix: str
-
-class DeleteViewCustomDeleteWarning(Warning): ...
```

### Comparing `django-stubs-4.2.7/django-stubs/views/generic/list.pyi` & `django_stubs-5.0.0/django-stubs/views/generic/list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/django-stubs/views/i18n.pyi` & `django_stubs-5.0.0/django-stubs/views/i18n.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections.abc import Callable
+from pathlib import Path
 from typing import Any
 
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse
 from django.utils.translation.trans_real import DjangoTranslation
 from django.views.generic import View
 
 LANGUAGE_QUERY_PARAMETER: str
 
+def builtin_template_path(name: str) -> Path: ...
 def set_language(request: HttpRequest) -> HttpResponse: ...
 def get_formats() -> dict[str, list[str] | int | str]: ...
 
-js_catalog_template: str
-
 class JavaScriptCatalog(View):
     head: Callable
     domain: str
     packages: list[str] | None
     translation: DjangoTranslation
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse: ...
     def get_paths(self, packages: list[str]) -> list[str]: ...
```

### Comparing `django-stubs-4.2.7/django_stubs.egg-info/PKG-INFO` & `django_stubs-5.0.0/django_stubs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 4.2.7
+Version: 5.0.0
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
+Project-URL: Funding, https://github.com/sponsors/typeddjango
 Project-URL: Release notes, https://github.com/typeddjango/django-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
-Requires-Dist: django-stubs-ext>=4.2.7
+Requires-Dist: asgiref
+Requires-Dist: django-stubs-ext>=5.0.0
 Requires-Dist: tomli; python_version < "3.11"
 Requires-Dist: typing-extensions
-Requires-Dist: types-pytz
 Requires-Dist: types-PyYAML
 Provides-Extra: compatible-mypy
-Requires-Dist: mypy~=1.7.0; extra == "compatible-mypy"
+Requires-Dist: mypy~=1.10.0; extra == "compatible-mypy"
+Provides-Extra: redis
+Requires-Dist: redis; extra == "redis"
 
 <img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 [![StackOverflow](https://shields.io/badge/ask-stackoverflow-orange?logo=stackoverflow)](https://stackoverflow.com/questions/tagged/django-stubs)
@@ -70,24 +73,25 @@
 [tool.django-stubs]
 django_settings_module = "myproject.settings"
 ```
 
 Two things happening here:
 
 1. We need to explicitly list our plugin to be loaded by `mypy`
-2. Our plugin also requires `django` settings module (what you put into `DJANGO_SETTINGS_MODULE` variable) to be specified
+2. You can either specify `django_settings_module` as seen above, or let `django_stubs` use the `DJANGO_SETTINGS_MODULE` variable from your environment.
 
 This fully working [typed boilerplate](https://github.com/wemake-services/wemake-django-template) can serve you as an example.
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 5.0.0          | 1.10.x       | 5.0            | 4.2, 4.1               | 3.8 - 3.12     |
 | 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
@@ -126,15 +130,15 @@
 django-stubs has a few settings, which you can list in:
 
 * `pyproject.toml`, under the table `[tool.django-stubs]`
 * `mypy.ini` under the table `[mypy.plugins.django-stubs]`
 
 The supported settings are:
 
-- `django_settings_module`, a string.
+- `django_settings_module`, a string, default to `os.getenv(DJANGO_SETTINGS_MODULE)`.
 
   Specify the import path of your settings module, the same as Django’s [`DJANGO_SETTINGS_MODULE` environment variable](https://docs.djangoproject.com/en/stable/topics/settings/#designating-the-settings).
 
 - `strict_settings`, a boolean, default `true`.
 
   Set to `false` if using dynamic settings, as [described below](https://github.com/typeddjango/django-stubs#how-to-use-a-custom-library-to-handle-django-settings).
 
@@ -207,62 +211,14 @@
 
 class AuthenticatedHttpRequest(HttpRequest):
     user: MyUser
 ```
 
 And then use `AuthenticatedHttpRequest` instead of the standard `HttpRequest` for when you know that the user is authenticated. For example in views using the `@login_required` decorator.
 
-### My QuerySet methods are returning Any rather than my Model
-
-If you are using `MyQuerySet.as_manager()`:
-
-Example:
-
-```python
-from django.db import models
-
-class MyModelQuerySet(models.QuerySet):
-    pass
-
-
-class MyModel(models.Model):
-    bar = models.IntegerField()
-    objects = MyModelQuerySet.as_manager()
-
-
-def use_my_model() -> int:
-    foo = MyModel.objects.get(id=1) # Should now be `MyModel`
-    return foo.xyz # Gives an error
-```
-
-Or if you're using `Manager.from_queryset`:
-
-Example:
-
-```python
-from django.db import models
-
-
-class MyModelQuerySet(models.QuerySet):
-    pass
-
-
-MyModelManager = models.Manager.from_queryset(MyModelQuerySet)
-
-
-class MyModel(models.Model):
-    bar = models.IntegerField()
-    objects = MyModelManager()
-
-
-def use_my_model() -> int:
-    foo = MyModel.objects.get(id=1) # Should now be `MyModel`
-    return foo.xyz # Gives an error
-```
-
 ### Why am I getting incompatible return type errors on my custom managers?
 
 If you declare your custom managers without generics and override built-in
 methods you might see an error message about incompatible error messages,
 something like this:
 
 ```python
@@ -383,15 +339,15 @@
 ```
 
 So, mypy would not like this code:
 
 ```python
 from django.conf import settings
 
-settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_SETTING'
+settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_VALUE'
 ```
 
 To handle this corner case we have a special setting `strict_settings` (`True` by default),
 you can switch it to `False` to always return `Any` and not raise any errors if runtime settings module has the given value,
 for example `pyproject.toml`:
 
 ```toml
@@ -406,15 +362,15 @@
 strict_settings = false
 ```
 
 And then:
 
 ```python
 # Works:
-reveal_type(settings.EXISTS_IN_RUNTIME)  # N: Any
+reveal_type(settings.EXISTS_AT_RUNTIME)  # N: Any
 
 # Errors:
 reveal_type(settings.MISSING)  # E: 'Settings' object has no attribute 'MISSING'
 ```
 
 ## Related projects
```

### Comparing `django-stubs-4.2.7/django_stubs.egg-info/SOURCES.txt` & `django_stubs-5.0.0/django_stubs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,14 @@
 django-stubs/contrib/postgres/fields/hstore.pyi
 django-stubs/contrib/postgres/fields/jsonb.pyi
 django-stubs/contrib/postgres/fields/ranges.pyi
 django-stubs/contrib/postgres/fields/utils.pyi
 django-stubs/contrib/postgres/forms/__init__.pyi
 django-stubs/contrib/postgres/forms/array.pyi
 django-stubs/contrib/postgres/forms/hstore.pyi
-django-stubs/contrib/postgres/forms/jsonb.pyi
 django-stubs/contrib/postgres/forms/ranges.pyi
 django-stubs/contrib/redirects/__init__.pyi
 django-stubs/contrib/redirects/admin.pyi
 django-stubs/contrib/redirects/apps.pyi
 django-stubs/contrib/redirects/middleware.pyi
 django-stubs/contrib/redirects/models.pyi
 django-stubs/contrib/redirects/migrations/__init__.pyi
@@ -290,17 +289,14 @@
 django-stubs/contrib/sessions/management/__init__.pyi
 django-stubs/contrib/sessions/management/commands/__init__.pyi
 django-stubs/contrib/sessions/management/commands/clearsessions.pyi
 django-stubs/contrib/sessions/migrations/__init__.pyi
 django-stubs/contrib/sitemaps/__init__.pyi
 django-stubs/contrib/sitemaps/apps.pyi
 django-stubs/contrib/sitemaps/views.pyi
-django-stubs/contrib/sitemaps/management/__init__.pyi
-django-stubs/contrib/sitemaps/management/commands/__init__.pyi
-django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
 django-stubs/contrib/sites/__init__.pyi
 django-stubs/contrib/sites/admin.pyi
 django-stubs/contrib/sites/apps.pyi
 django-stubs/contrib/sites/checks.pyi
 django-stubs/contrib/sites/management.pyi
 django-stubs/contrib/sites/managers.pyi
 django-stubs/contrib/sites/middleware.pyi
@@ -339,14 +335,15 @@
 django-stubs/core/cache/backends/__init__.pyi
 django-stubs/core/cache/backends/base.pyi
 django-stubs/core/cache/backends/db.pyi
 django-stubs/core/cache/backends/dummy.pyi
 django-stubs/core/cache/backends/filebased.pyi
 django-stubs/core/cache/backends/locmem.pyi
 django-stubs/core/cache/backends/memcached.pyi
+django-stubs/core/cache/backends/redis.pyi
 django-stubs/core/checks/__init__.pyi
 django-stubs/core/checks/async_checks.pyi
 django-stubs/core/checks/caches.pyi
 django-stubs/core/checks/database.pyi
 django-stubs/core/checks/files.pyi
 django-stubs/core/checks/messages.pyi
 django-stubs/core/checks/model_checks.pyi
@@ -405,14 +402,15 @@
 django-stubs/core/management/commands/dumpdata.pyi
 django-stubs/core/management/commands/flush.pyi
 django-stubs/core/management/commands/inspectdb.pyi
 django-stubs/core/management/commands/loaddata.pyi
 django-stubs/core/management/commands/makemessages.pyi
 django-stubs/core/management/commands/makemigrations.pyi
 django-stubs/core/management/commands/migrate.pyi
+django-stubs/core/management/commands/optimizemigration.pyi
 django-stubs/core/management/commands/runserver.pyi
 django-stubs/core/management/commands/sendtestemail.pyi
 django-stubs/core/management/commands/shell.pyi
 django-stubs/core/management/commands/showmigrations.pyi
 django-stubs/core/management/commands/sqlflush.pyi
 django-stubs/core/management/commands/sqlmigrate.pyi
 django-stubs/core/management/commands/sqlsequencereset.pyi
@@ -520,14 +518,15 @@
 django-stubs/db/models/options.pyi
 django-stubs/db/models/query.pyi
 django-stubs/db/models/query_utils.pyi
 django-stubs/db/models/signals.pyi
 django-stubs/db/models/utils.pyi
 django-stubs/db/models/fields/__init__.pyi
 django-stubs/db/models/fields/files.pyi
+django-stubs/db/models/fields/generated.pyi
 django-stubs/db/models/fields/json.pyi
 django-stubs/db/models/fields/mixins.pyi
 django-stubs/db/models/fields/proxy.pyi
 django-stubs/db/models/fields/related.pyi
 django-stubs/db/models/fields/related_descriptors.pyi
 django-stubs/db/models/fields/related_lookups.pyi
 django-stubs/db/models/fields/reverse_related.pyi
@@ -618,23 +617,22 @@
 django-stubs/urls/resolvers.pyi
 django-stubs/urls/utils.pyi
 django-stubs/utils/__init__.pyi
 django-stubs/utils/_os.pyi
 django-stubs/utils/archive.pyi
 django-stubs/utils/asyncio.pyi
 django-stubs/utils/autoreload.pyi
-django-stubs/utils/baseconv.pyi
 django-stubs/utils/cache.pyi
+django-stubs/utils/choices.pyi
 django-stubs/utils/connection.pyi
 django-stubs/utils/crypto.pyi
 django-stubs/utils/datastructures.pyi
 django-stubs/utils/dateformat.pyi
 django-stubs/utils/dateparse.pyi
 django-stubs/utils/dates.pyi
-django-stubs/utils/datetime_safe.pyi
 django-stubs/utils/deconstruct.pyi
 django-stubs/utils/decorators.pyi
 django-stubs/utils/deprecation.pyi
 django-stubs/utils/duration.pyi
 django-stubs/utils/encoding.pyi
 django-stubs/utils/feedgenerator.pyi
 django-stubs/utils/formats.pyi
@@ -652,15 +650,14 @@
 django-stubs/utils/numberformat.pyi
 django-stubs/utils/regex_helper.pyi
 django-stubs/utils/safestring.pyi
 django-stubs/utils/termcolors.pyi
 django-stubs/utils/text.pyi
 django-stubs/utils/timesince.pyi
 django-stubs/utils/timezone.pyi
-django-stubs/utils/topological_sort.pyi
 django-stubs/utils/tree.pyi
 django-stubs/utils/version.pyi
 django-stubs/utils/xmlutils.pyi
 django-stubs/utils/translation/__init__.pyi
 django-stubs/utils/translation/reloader.pyi
 django-stubs/utils/translation/template.pyi
 django-stubs/utils/translation/trans_null.pyi
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/config.py` & `django_stubs-5.0.0/mypy_django_plugin/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import configparser
+import os
 import sys
 import textwrap
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Dict, NoReturn, Optional
 
 if sys.version_info[:2] >= (3, 11):
@@ -10,30 +11,32 @@
 else:
     import tomli as tomllib
 
 INI_USAGE = """
 (config)
 ...
 [mypy.plugins.django-stubs]
-django_settings_module = str (required)
+django_settings_module = str (default: `os.getenv("DJANGO_SETTINGS_MODULE")`)
 strict_settings = bool (default: true)
 ...
 """
 TOML_USAGE = """
 (config)
 ...
 [tool.django-stubs]
-django_settings_module = str (required)
+django_settings_module = str (default: `os.getenv("DJANGO_SETTINGS_MODULE")`)
 strict_settings = bool (default: true)
 ...
 """
 INVALID_FILE = "mypy config file is not specified or found"
 COULD_NOT_LOAD_FILE = "could not load configuration file"
 MISSING_SECTION = "no section [{section}] found"
-MISSING_DJANGO_SETTINGS = "missing required 'django_settings_module' config"
+DJANGO_SETTINGS_ENV_VAR = "DJANGO_SETTINGS_MODULE"
+MISSING_DJANGO_SETTINGS = f"missing required 'django_settings_module' config.\
+ Either specify this config or set your `{DJANGO_SETTINGS_ENV_VAR}` env var"
 INVALID_BOOL_SETTING = "invalid {key!r}: the setting must be a boolean"
 
 
 def exit_with_error(msg: str, is_toml: bool = False) -> NoReturn:
     """Using mypy's argument parser, raise `SystemExit` to fail hard if validation fails.
 
     Considering that the plugin's startup duration is around double as long as mypy's, this aims to
@@ -76,18 +79,20 @@
             toml_exit(COULD_NOT_LOAD_FILE)
 
         try:
             config: Dict[str, Any] = data["tool"]["django-stubs"]
         except KeyError:
             toml_exit(MISSING_SECTION.format(section="tool.django-stubs"))
 
-        if "django_settings_module" not in config:
+        django_settings_module = config.get("django_settings_module") or os.getenv(DJANGO_SETTINGS_ENV_VAR)
+        if not django_settings_module:
             toml_exit(MISSING_DJANGO_SETTINGS)
 
-        self.django_settings_module = config["django_settings_module"]
+        self.django_settings_module = django_settings_module
+
         if not isinstance(self.django_settings_module, str):
             toml_exit("invalid 'django_settings_module': the setting must be a string")
 
         self.strict_settings = config.get("strict_settings", True)
         if not isinstance(self.strict_settings, bool):
             toml_exit(INVALID_BOOL_SETTING.format(key="strict_settings"))
 
@@ -99,18 +104,23 @@
         except OSError:
             exit_with_error(COULD_NOT_LOAD_FILE)
 
         section = "mypy.plugins.django-stubs"
         if not parser.has_section(section):
             exit_with_error(MISSING_SECTION.format(section=section))
 
-        if not parser.has_option(section, "django_settings_module"):
+        if parser.has_option(section, "django_settings_module"):
+            django_settings_module = parser.get(section, "django_settings_module").strip("'\"")
+        else:
+            django_settings_module = os.getenv(DJANGO_SETTINGS_ENV_VAR, "")
+
+        if not django_settings_module:
             exit_with_error(MISSING_DJANGO_SETTINGS)
 
-        self.django_settings_module = parser.get(section, "django_settings_module").strip("'\"")
+        self.django_settings_module = django_settings_module
 
         try:
             self.strict_settings = parser.getboolean(section, "strict_settings", fallback=True)
         except ValueError:
             exit_with_error(INVALID_BOOL_SETTING.format(key="strict_settings"))
 
     def to_json(self) -> Dict[str, Any]:
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/django/context.py` & `django_stubs-5.0.0/mypy_django_plugin/django/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,14 +365,17 @@
 
     def get_field_related_model_cls(self, field: Union["RelatedField[Any, Any]", ForeignObjectRel]) -> Type[Model]:
         if isinstance(field, RelatedField):
             related_model_cls = field.remote_field.model
         else:
             related_model_cls = field.field.model
 
+        if related_model_cls is None:
+            raise UnregisteredModelError
+
         if isinstance(related_model_cls, str):
             if related_model_cls == "self":  # type: ignore[unreachable]
                 # same model
                 related_model_cls = field.model
             elif "." not in related_model_cls:
                 # same file model
                 related_model_fullname = f"{field.model.__module__}.{related_model_cls}"
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/lib/helpers.py` & `django_stubs-5.0.0/mypy_django_plugin/lib/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     from_queryset_manager: str
     reverse_managers: Dict[str, str]
     baseform_bases: Dict[str, int]
     manager_bases: Dict[str, int]
     model_bases: Dict[str, int]
     queryset_bases: Dict[str, int]
     m2m_throughs: Dict[str, str]
+    m2m_managers: Dict[str, str]
 
 
 def get_django_metadata(model_info: TypeInfo) -> DjangoTypeMetadata:
     return cast(DjangoTypeMetadata, model_info.metadata.setdefault("django", {}))
 
 
 def get_django_metadata_bases(
@@ -77,14 +78,28 @@
     return lookup_fully_qualified_typeinfo(api, manager_fullname)
 
 
 def set_reverse_manager_info(model_info: TypeInfo, derived_from: str, fullname: str) -> None:
     get_django_metadata(model_info).setdefault("reverse_managers", {})[derived_from] = fullname
 
 
+def get_many_to_many_manager_info(
+    api: Union[TypeChecker, SemanticAnalyzer], *, to: TypeInfo, derived_from: str
+) -> Optional[TypeInfo]:
+    manager_fullname = get_django_metadata(to).get("m2m_managers", {}).get(derived_from)
+    if not manager_fullname:
+        return None
+
+    return lookup_fully_qualified_typeinfo(api, manager_fullname)
+
+
+def set_many_to_many_manager_info(to: TypeInfo, derived_from: str, manager_info: TypeInfo) -> None:
+    get_django_metadata(to).setdefault("m2m_managers", {})[derived_from] = manager_info.fullname
+
+
 class IncompleteDefnException(Exception):
     pass
 
 
 def lookup_fully_qualified_sym(fullname: str, all_modules: Dict[str, MypyFile]) -> Optional[SymbolTableNode]:
     if "." not in fullname:
         return None
@@ -185,14 +200,18 @@
     return arg_types[0]
 
 
 def make_optional(typ: MypyType) -> MypyType:
     return UnionType.make_union([typ, NoneTyp()])
 
 
+def is_optional(typ: MypyType) -> bool:
+    return isinstance(typ, UnionType) and any(isinstance(item, NoneTyp) for item in typ.items)
+
+
 # Duplicating mypy.semanal_shared.parse_bool because importing it directly caused ImportError (#1784)
 def parse_bool(expr: Expression) -> Optional[bool]:
     if isinstance(expr, NameExpr):
         if expr.fullname == "builtins.True":
             return True
         if expr.fullname == "builtins.False":
             return False
@@ -261,15 +280,15 @@
     classdef = ClassDef(name, Block([]))
     classdef.fullname = module + "." + name
 
     # make new TypeInfo
     new_typeinfo = TypeInfo(SymbolTable(), classdef, module)
     new_typeinfo.bases = bases
     calculate_mro(new_typeinfo)
-    new_typeinfo.calculate_metaclass_type()
+    new_typeinfo.metaclass_type = new_typeinfo.calculate_metaclass_type()
 
     classdef.info = new_typeinfo
 
     return new_typeinfo
 
 
 def add_new_class_for_module(
@@ -412,14 +431,17 @@
     sym = api.lookup_fully_qualified_or_none(fullnames.MANAGER_CLASS_FULLNAME)
     if sym is not None and isinstance(sym.node, TypeInfo):
         bases = get_django_metadata_bases(sym.node, "manager_bases")
         bases[fullname] = 1
 
 
 def is_abstract_model(model: TypeInfo) -> bool:
+    if model.fullname in fullnames.DJANGO_ABSTRACT_MODELS:
+        return True
+
     if not is_model_type(model):
         return False
 
     metadata = get_django_metadata(model)
     if metadata.get("is_abstract_model") is not None:
         return metadata["is_abstract_model"]
 
@@ -470,8 +492,8 @@
             api.defer()
     else:
         api.fail("Could not match lazy reference with any model", ctx)
     return None
 
 
 def is_model_type(info: TypeInfo) -> bool:
-    return info.metaclass_type is not None and info.metaclass_type.type.fullname == fullnames.MODEL_METACLASS_FULLNAME
+    return info.metaclass_type is not None and info.metaclass_type.type.has_base(fullnames.MODEL_METACLASS_FULLNAME)
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/main.py` & `django_stubs-5.0.0/mypy_django_plugin/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
 import sys
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 
+from mypy.build import PRI_MYPY
 from mypy.modulefinder import mypy_path
 from mypy.nodes import MypyFile, TypeInfo
 from mypy.options import Options
 from mypy.plugin import (
     AnalyzeTypeContext,
     AttributeContext,
     ClassDefContext,
@@ -95,15 +96,16 @@
     def _get_typeinfo_or_none(self, class_name: str) -> Optional[TypeInfo]:
         sym = self.lookup_fully_qualified(class_name)
         if sym is not None and isinstance(sym.node, TypeInfo):
             return sym.node
         return None
 
     def _new_dependency(self, module: str) -> Tuple[int, str, int]:
-        return 10, module, -1
+        fake_lineno = -1
+        return (PRI_MYPY, module, fake_lineno)
 
     def get_additional_deps(self, file: MypyFile) -> List[Tuple[int, str, int]]:
         # for settings
         if file.fullname == "django.conf" and self.django_context.django_settings_module:
             return [self._new_dependency(self.django_context.django_settings_module)]
 
         # for values / values_list
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/fields.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import TYPE_CHECKING, Any, Optional, Tuple, Union, cast
 
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models.fields import AutoField, Field
 from django.db.models.fields.related import RelatedField
 from django.db.models.fields.reverse_related import ForeignObjectRel
+from mypy.maptype import map_instance_to_supertype
 from mypy.nodes import AssignmentStmt, NameExpr, TypeInfo
 from mypy.plugin import FunctionContext
-from mypy.types import AnyType, Instance, ProperType, TypeOfAny, UnionType
+from mypy.types import AnyType, Instance, NoneType, ProperType, TypeOfAny, UninhabitedType, UnionType
 from mypy.types import Type as MypyType
 
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.exceptions import UnregisteredModelError
 from mypy_django_plugin.lib import fullnames, helpers
 from mypy_django_plugin.lib.helpers import parse_bool
 from mypy_django_plugin.transformers import manytomany
@@ -146,14 +147,33 @@
         is_set_nullable = parse_bool(primary_key_expr) or False
 
     set_type, get_type = get_field_descriptor_types(
         default_return_type.type,
         is_set_nullable=is_set_nullable or is_nullable,
         is_get_nullable=is_get_nullable or is_nullable,
     )
+
+    # reconcile set and get types with the base field class
+    base_field_type = next(base for base in default_return_type.type.mro if base.fullname == fullnames.FIELD_FULLNAME)
+    mapped_instance = map_instance_to_supertype(default_return_type, base_field_type)
+    mapped_set_type, mapped_get_type = mapped_instance.args
+
+    # bail if either mapped_set_type or mapped_get_type have type Never
+    if not (isinstance(mapped_set_type, UninhabitedType) or isinstance(mapped_get_type, UninhabitedType)):
+        # always replace set_type and get_type with (non-Any) mapped types
+        set_type = helpers.convert_any_to_type(mapped_set_type, set_type)
+        get_type = helpers.convert_any_to_type(mapped_get_type, get_type)
+
+        # the get_type must be optional if the field is nullable
+        if (is_get_nullable or is_nullable) and not (isinstance(get_type, NoneType) or helpers.is_optional(get_type)):
+            ctx.api.fail(
+                f"{default_return_type.type.name} is nullable but its generic get type parameter is not optional",
+                ctx.context,
+            )
+
     return helpers.reparametrize_instance(default_return_type, [set_type, get_type])
 
 
 def determine_type_of_array_field(ctx: FunctionContext, django_context: DjangoContext) -> MypyType:
     default_return_type = set_descriptor_types_for_field(ctx)
 
     base_field_arg_type = helpers.get_call_argument_type_by_name(ctx, "base_field")
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/forms.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/forms.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/functional.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/functional.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/init_create.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/init_create.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/managers.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,26 @@
     SymbolTableNode,
     TypeInfo,
     Var,
 )
 from mypy.plugin import AttributeContext, ClassDefContext, DynamicClassDefContext
 from mypy.semanal import SemanticAnalyzer
 from mypy.semanal_shared import has_placeholder
-from mypy.types import AnyType, CallableType, FunctionLike, Instance, Overloaded, ProperType, TypeOfAny, TypeVarType
+from mypy.types import (
+    AnyType,
+    CallableType,
+    FunctionLike,
+    Instance,
+    Overloaded,
+    ProperType,
+    TypeOfAny,
+    TypeVarType,
+    UnionType,
+    get_proper_type,
+)
 from mypy.types import Type as MypyType
 from mypy.typevars import fill_typevars
 
 from mypy_django_plugin.lib import fullnames, helpers
 
 MANAGER_METHODS_RETURNING_QUERYSET: Final = frozenset(
     (
@@ -270,14 +281,21 @@
         method_name = ctx.context.callee.name
     else:
         ctx.api.fail("Unable to resolve return type of queryset/manager method", ctx.context)
         return AnyType(TypeOfAny.from_error)
 
     if isinstance(ctx.type, Instance):
         return resolve_manager_method_from_instance(instance=ctx.type, method_name=method_name, ctx=ctx)
+    elif isinstance(ctx.type, UnionType) and all(isinstance(instance, Instance) for instance in ctx.type.items):
+        resolved = tuple(
+            resolve_manager_method_from_instance(instance=instance, method_name=method_name, ctx=ctx)
+            for instance in ctx.type.items
+            if isinstance(instance, Instance)
+        )
+        return get_proper_type(UnionType(resolved))
     else:
         ctx.api.fail(f'Unable to resolve return type of queryset/manager method "{method_name}"', ctx.context)
         return AnyType(TypeOfAny.from_error)
 
 
 def create_new_manager_class_from_from_queryset_method(ctx: DynamicClassDefContext) -> None:
     """
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/manytomany.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/manytomany.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import NamedTuple, Optional, Tuple, Union
 
 from mypy.checker import TypeChecker
 from mypy.nodes import AssignmentStmt, Expression, MemberExpr, NameExpr, StrExpr, TypeInfo
 from mypy.plugin import FunctionContext, MethodContext
 from mypy.semanal import SemanticAnalyzer
-from mypy.types import Instance, ProperType, UninhabitedType
+from mypy.types import Instance, ProperType, TypeVarType, UninhabitedType
 from mypy.types import Type as MypyType
 
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.lib import fullnames, helpers
 
 
 class M2MThrough(NamedTuple):
@@ -146,59 +146,92 @@
     if lazy_reference is not None:
         model_info = helpers.resolve_lazy_reference(lazy_reference, api=api, django_context=django_context, ctx=expr)
         if model_info is not None:
             return Instance(model_info, [])
     return None
 
 
-def get_related_manager_and_model(ctx: MethodContext) -> Optional[Tuple[Instance, Instance]]:
+def get_related_manager_and_model(ctx: MethodContext) -> Optional[Tuple[Instance, Instance, Instance]]:
+    """
+    Returns a 3-tuple consisting of:
+      1. A `ManyRelatedManager` instance
+      2. The first type parameter (_To) instance of 1. when it's a model
+      3. The second type parameter (_Through) instance of 1. when it's a model
+    When encountering a `ManyRelatedManager` that has populated its 2 first type
+    parameters with models. Otherwise `None` is returned.
+
+    For example: if given a `ManyRelatedManager[A, B]` where `A` and `B` are models the
+    following 3-tuple is returned: `(ManyRelatedManager[A, B], A, B)`.
+    """
     if (
         isinstance(ctx.default_return_type, Instance)
         and ctx.default_return_type.type.fullname == fullnames.MANY_RELATED_MANAGER
     ):
         # This is a call to '__get__' overload with a model instance of 'ManyToManyDescriptor'.
         # Returning a 'ManyRelatedManager'. Which we want to, just like Django, build from the
         # default manager of the related model.
         many_related_manager = ctx.default_return_type
-        # Require first type argument of 'ManyRelatedManager' to be a model
+        # Require first and second type argument of 'ManyRelatedManager' to be models
         if (
-            many_related_manager.args
+            len(many_related_manager.args) >= 2
             and isinstance(many_related_manager.args[0], Instance)
             and helpers.is_model_type(many_related_manager.args[0].type)
+            and isinstance(many_related_manager.args[1], Instance)
+            and helpers.is_model_type(many_related_manager.args[1].type)
         ):
-            return many_related_manager, many_related_manager.args[0]
+            return many_related_manager, many_related_manager.args[0], many_related_manager.args[1]
 
     return None
 
 
 def refine_many_to_many_related_manager(ctx: MethodContext) -> MypyType:
     """
     Updates the 'ManyRelatedManager' returned by e.g. 'ManyToManyDescriptor' to be a subclass
     of 'ManyRelatedManager' and the related model's default manager.
     """
     related_objects = get_related_manager_and_model(ctx)
     if related_objects is None:
         return ctx.default_return_type
 
-    many_related_manager, related_model_instance = related_objects
+    many_related_manager, related_model_instance, through_model_instance = related_objects
     checker = helpers.get_typechecker_api(ctx)
-    related_model_instance = related_model_instance.copy_modified()
-    related_manager_info = helpers.get_reverse_manager_info(
-        checker, related_model_instance.type, derived_from="_default_manager"
+    related_manager_info = helpers.get_many_to_many_manager_info(
+        checker, to=related_model_instance.type, derived_from="_default_manager"
     )
     if related_manager_info is None:
         default_manager_node = related_model_instance.type.names.get("_default_manager")
         if default_manager_node is None or not isinstance(default_manager_node.type, Instance):
             return ctx.default_return_type
 
+        # Create a reusable generic subclass that is generic over a 'through' model,
+        # explicitly declared it'd could have looked something like below
+        #
+        # class X(models.Model): ...
+        # _Through = TypeVar("_Through", bound=models.Model)
+        # class X_ManyRelatedManager(ManyRelatedManager[X, _Through], type(X._default_manager), Generic[_Through]): ...
+        _through_type_var = many_related_manager.type.defn.type_vars[1]
+        assert isinstance(_through_type_var, TypeVarType)
+        generic_to_many_related_manager = many_related_manager.copy_modified(
+            args=[
+                # Keep the same '_To' as the (parent) `ManyRelatedManager` instance
+                many_related_manager.args[0],
+                # But reset the '_Through' `TypeVar` declared for `ManyRelatedManager`
+                _through_type_var.copy_modified(),
+            ]
+        )
         related_manager_info = helpers.add_new_class_for_module(
             module=checker.modules[related_model_instance.type.module_name],
             name=f"{related_model_instance.type.name}_ManyRelatedManager",
-            bases=[many_related_manager, default_manager_node.type],
+            bases=[generic_to_many_related_manager, default_manager_node.type],
         )
+        # Reuse the '_Through' `TypeVar` from `ManyRelatedManager` in our subclass
+        related_manager_info.defn.type_vars = [_through_type_var.copy_modified()]
+        related_manager_info.add_type_vars()
         related_manager_info.metadata["django"] = {"related_manager_to_model": related_model_instance.type.fullname}
-        helpers.set_reverse_manager_info(
-            related_model_instance.type,
+        # Track the existence of our manager subclass, by tying it to model it operates on
+        helpers.set_many_to_many_manager_info(
+            to=related_model_instance.type,
             derived_from="_default_manager",
-            fullname=related_manager_info.fullname,
+            manager_info=related_manager_info,
         )
-    return Instance(related_manager_info, [])
+
+    return Instance(related_manager_info, [through_model_instance])
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/meta.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/meta.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/models.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from collections import deque
 from functools import cached_property
-from typing import Any, Dict, List, Optional, Type, Union, cast
+from typing import Any, Dict, Iterable, List, Optional, Type, Union, cast
 
 from django.db.models import Manager, Model
 from django.db.models.fields import DateField, DateTimeField, Field
-from django.db.models.fields.reverse_related import ManyToManyRel, OneToOneRel
+from django.db.models.fields.reverse_related import ForeignObjectRel, ManyToManyRel, OneToOneRel
 from mypy.checker import TypeChecker
 from mypy.nodes import (
     ARG_STAR2,
     MDEF,
     Argument,
     AssignmentStmt,
     CallExpr,
     Context,
     Expression,
     NameExpr,
     RefExpr,
+    Statement,
     StrExpr,
     SymbolTableNode,
     TypeInfo,
     Var,
 )
 from mypy.plugin import AnalyzeTypeContext, AttributeContext, CheckerPluginInterface, ClassDefContext
 from mypy.plugins import common
@@ -452,134 +454,132 @@
     def reverse_one_to_one_descriptor(self) -> TypeInfo:
         return self.lookup_typeinfo_or_incomplete_defn_error(fullnames.REVERSE_ONE_TO_ONE_DESCRIPTOR)
 
     @cached_property
     def many_to_many_descriptor(self) -> TypeInfo:
         return self.lookup_typeinfo_or_incomplete_defn_error(fullnames.MANY_TO_MANY_DESCRIPTOR)
 
-    def run_with_model_cls(self, model_cls: Type[Model]) -> None:
-        # add related managers
-        for relation in self.django_context.get_model_relations(model_cls):
-            attname = relation.get_accessor_name()
-            if attname is None or attname in self.model_classdef.info.names:
-                # No reverse accessor or already declared. Note that this would also leave any
-                # explicitly declared(i.e. non-inferred) reverse accessors alone
-                continue
+    def process_relation(self, relation: ForeignObjectRel) -> None:
+        attname = relation.get_accessor_name()
+        if attname is None or attname in self.model_classdef.info.names:
+            # No reverse accessor or already declared. Note that this would also leave any
+            # explicitly declared(i.e. non-inferred) reverse accessors alone
+            return
 
-            related_model_cls = self.django_context.get_field_related_model_cls(relation)
+        related_model_cls = self.django_context.get_field_related_model_cls(relation)
+        related_model_info = self.lookup_class_typeinfo_or_incomplete_defn_error(related_model_cls)
 
-            try:
-                related_model_info = self.lookup_class_typeinfo_or_incomplete_defn_error(related_model_cls)
-            except helpers.IncompleteDefnException as exc:
-                if not self.api.final_iteration:
-                    raise exc
-                else:
-                    continue
+        if isinstance(relation, OneToOneRel):
+            self.add_new_node_to_model_class(
+                attname,
+                Instance(
+                    self.reverse_one_to_one_descriptor,
+                    [Instance(self.model_classdef.info, []), Instance(related_model_info, [])],
+                ),
+            )
+            return
 
-            if isinstance(relation, OneToOneRel):
-                self.add_new_node_to_model_class(
-                    attname,
-                    Instance(
-                        self.reverse_one_to_one_descriptor,
-                        [Instance(self.model_classdef.info, []), Instance(related_model_info, [])],
-                    ),
-                )
-                continue
+        elif isinstance(relation, ManyToManyRel):
+            # TODO: 'relation' should be based on `TypeInfo` instead of Django runtime.
+            to_fullname = helpers.get_class_fullname(relation.remote_field.model)
+            to_model_info = self.lookup_typeinfo_or_incomplete_defn_error(to_fullname)
+            assert relation.through is not None
+            through_fullname = helpers.get_class_fullname(relation.through)
+            through_model_info = self.lookup_typeinfo_or_incomplete_defn_error(through_fullname)
+            self.add_new_node_to_model_class(
+                attname,
+                Instance(self.many_to_many_descriptor, [Instance(to_model_info, []), Instance(through_model_info, [])]),
+            )
+            return
+
+        related_manager_info = None
+        try:
+            related_manager_info = self.lookup_typeinfo_or_incomplete_defn_error(fullnames.RELATED_MANAGER_CLASS)
+            default_manager = related_model_info.names.get("_default_manager")
+            if not default_manager:
+                raise helpers.IncompleteDefnException()
+        except helpers.IncompleteDefnException as exc:
+            if not self.api.final_iteration:
+                raise exc
 
-            elif isinstance(relation, ManyToManyRel):
-                # TODO: 'relation' should be based on `TypeInfo` instead of Django runtime.
-                to_fullname = helpers.get_class_fullname(relation.remote_field.model)
-                to_model_info = self.lookup_typeinfo_or_incomplete_defn_error(to_fullname)
-                assert relation.through is not None
-                through_fullname = helpers.get_class_fullname(relation.through)
-                through_model_info = self.lookup_typeinfo_or_incomplete_defn_error(through_fullname)
+            # If a django model has a Manager class that cannot be
+            # resolved statically (if it is generated in a way where we
+            # cannot import it, like `objects = my_manager_factory()`),
+            # we fallback to the default related manager, so you at
+            # least get a base level of working type checking.
+            #
+            # See https://github.com/typeddjango/django-stubs/pull/993
+            # for more information on when this error can occur.
+            fallback_manager = self.get_or_create_manager_with_any_fallback(related_manager=True)
+            if fallback_manager is not None:
                 self.add_new_node_to_model_class(
-                    attname,
-                    Instance(
-                        self.many_to_many_descriptor, [Instance(to_model_info, []), Instance(through_model_info, [])]
-                    ),
+                    attname, Instance(fallback_manager, [Instance(related_model_info, [])])
                 )
+            related_model_fullname = related_model_cls.__module__ + "." + related_model_cls.__name__
+            self.ctx.api.fail(
+                (
+                    "Couldn't resolve related manager for relation "
+                    f"{relation.name!r} (from {related_model_fullname}."
+                    f"{relation.field})."
+                ),
+                self.ctx.cls,
+                code=MANAGER_MISSING,
+            )
+            return
 
-            else:
-                related_manager_info = None
-                try:
-                    related_manager_info = self.lookup_typeinfo_or_incomplete_defn_error(
-                        fullnames.RELATED_MANAGER_CLASS
-                    )
-                    default_manager = related_model_info.names.get("_default_manager")
-                    if not default_manager:
-                        raise helpers.IncompleteDefnException()
-                except helpers.IncompleteDefnException as exc:
-                    if not self.api.final_iteration:
-                        raise exc
-
-                    # If a django model has a Manager class that cannot be
-                    # resolved statically (if it is generated in a way where we
-                    # cannot import it, like `objects = my_manager_factory()`),
-                    # we fallback to the default related manager, so you at
-                    # least get a base level of working type checking.
-                    #
-                    # See https://github.com/typeddjango/django-stubs/pull/993
-                    # for more information on when this error can occur.
-                    fallback_manager = self.get_or_create_manager_with_any_fallback(related_manager=True)
-                    if fallback_manager is not None:
-                        self.add_new_node_to_model_class(
-                            attname, Instance(fallback_manager, [Instance(related_model_info, [])])
-                        )
-                    related_model_fullname = related_model_cls.__module__ + "." + related_model_cls.__name__
-                    self.ctx.api.fail(
-                        (
-                            "Couldn't resolve related manager for relation "
-                            f"{relation.name!r} (from {related_model_fullname}."
-                            f"{relation.field})."
-                        ),
-                        self.ctx.cls,
-                        code=MANAGER_MISSING,
-                    )
+        # Check if the related model has a related manager subclassed from the default manager
+        # TODO: Support other reverse managers than `_default_manager`
+        default_reverse_manager_info = helpers.get_reverse_manager_info(
+            self.api, model_info=related_model_info, derived_from="_default_manager"
+        )
+        if default_reverse_manager_info:
+            self.add_new_node_to_model_class(attname, Instance(default_reverse_manager_info, []))
+            return
 
-                    continue
+        # The reverse manager we're looking for doesn't exist. So we
+        # create it. The (default) reverse manager type is built from a
+        # RelatedManager and the default manager on the related model
+        parametrized_related_manager_type = Instance(related_manager_info, [Instance(related_model_info, [])])
+        default_manager_type = default_manager.type
+        assert default_manager_type is not None
+        assert isinstance(default_manager_type, Instance)
+        # When the default manager isn't custom there's no need to create a new type
+        # as `RelatedManager` has `models.Manager` as base
+        if default_manager_type.type.fullname == fullnames.MANAGER_CLASS_FULLNAME:
+            self.add_new_node_to_model_class(attname, parametrized_related_manager_type)
+            return
 
-                # Check if the related model has a related manager subclassed from the default manager
-                # TODO: Support other reverse managers than `_default_manager`
-                default_reverse_manager_info = helpers.get_reverse_manager_info(
-                    self.api, model_info=related_model_info, derived_from="_default_manager"
-                )
-                if default_reverse_manager_info:
-                    self.add_new_node_to_model_class(attname, Instance(default_reverse_manager_info, []))
-                    continue
+        # The reverse manager is based on the related model's manager, so it makes most sense to add the new
+        # related manager in that module
+        new_related_manager_info = helpers.add_new_class_for_module(
+            module=self.api.modules[related_model_info.module_name],
+            name=f"{related_model_cls.__name__}_RelatedManager",
+            bases=[parametrized_related_manager_type, default_manager_type],
+        )
+        new_related_manager_info.metadata["django"] = {"related_manager_to_model": related_model_info.fullname}
+        # Stash the new reverse manager type fullname on the related model, so we don't duplicate
+        # or have to create it again for other reverse relations
+        helpers.set_reverse_manager_info(
+            related_model_info,
+            derived_from="_default_manager",
+            fullname=new_related_manager_info.fullname,
+        )
+        self.add_new_node_to_model_class(attname, Instance(new_related_manager_info, []))
 
-                # The reverse manager we're looking for doesn't exist. So we
-                # create it. The (default) reverse manager type is built from a
-                # RelatedManager and the default manager on the related model
-                parametrized_related_manager_type = Instance(related_manager_info, [Instance(related_model_info, [])])
-                default_manager_type = default_manager.type
-                assert default_manager_type is not None
-                assert isinstance(default_manager_type, Instance)
-                # When the default manager isn't custom there's no need to create a new type
-                # as `RelatedManager` has `models.Manager` as base
-                if default_manager_type.type.fullname == fullnames.MANAGER_CLASS_FULLNAME:
-                    self.add_new_node_to_model_class(attname, parametrized_related_manager_type)
-                    continue
+    def run_with_model_cls(self, model_cls: Type[Model]) -> None:
+        # add related managers etc.
+        processing_incomplete = False
+        for relation in self.django_context.get_model_relations(model_cls):
+            try:
+                self.process_relation(relation)
+            except helpers.IncompleteDefnException:
+                processing_incomplete = True
 
-                # The reverse manager is based on the related model's manager, so it makes most sense to add the new
-                # related manager in that module
-                new_related_manager_info = helpers.add_new_class_for_module(
-                    module=self.api.modules[related_model_info.module_name],
-                    name=f"{related_model_cls.__name__}_RelatedManager",
-                    bases=[parametrized_related_manager_type, default_manager_type],
-                )
-                new_related_manager_info.metadata["django"] = {"related_manager_to_model": related_model_info.fullname}
-                # Stash the new reverse manager type fullname on the related model, so we don't duplicate
-                # or have to create it again for other reverse relations
-                helpers.set_reverse_manager_info(
-                    related_model_info,
-                    derived_from="_default_manager",
-                    fullname=new_related_manager_info.fullname,
-                )
-                self.add_new_node_to_model_class(attname, Instance(new_related_manager_info, []))
+        if processing_incomplete and not self.api.final_iteration:
+            raise helpers.IncompleteDefnException
 
 
 class AddExtraFieldMethods(ModelClassInitializer):
     def run_with_model_cls(self, model_cls: Type[Model]) -> None:
         # get_FOO_display for choices
         for field in self.django_context.get_model_fields(model_cls):
             if field.choices:
@@ -622,14 +622,36 @@
 class ProcessManyToManyFields(ModelClassInitializer):
     """
     Processes 'ManyToManyField()' fields and generates any implicit through tables that
     Django also generates. It won't do anything if the model is abstract or for fields
     where an explicit 'through' argument has been passed.
     """
 
+    def statements(self) -> Iterable[Statement]:
+        """
+        Returns class body statements from the current model and any of its bases that
+        is an abstract model. Statements from any concrete parent class or parents of
+        that concrete class will be skipped.
+        """
+        processed_models = set()
+        # Produce all statements from current class
+        model_bases = deque([self.model_classdef])
+        # Do a breadth first search over the current model and its bases, to find all
+        # abstract parent models that have not been "interrupted" by any concrete model.
+        while model_bases:
+            model = model_bases.popleft()
+            yield from model.defs.body
+            for base in model.info.bases:
+                # Only produce any additional statements from abstract model bases, as they
+                # simulate regular python inheritance. Avoid concrete models, and any of their
+                # parents, as they're handled differently by Django.
+                if helpers.is_abstract_model(base.type) and base.type.fullname not in processed_models:
+                    model_bases.append(base.type.defn)
+                    processed_models.add(base.type.fullname)
+
     def run(self) -> None:
         if self.is_model_abstract:
             # TODO: Create abstract through models?
             return
 
         # Start out by prefetching a couple of dependencies needed to be able to declare any
         # new, implicit, through model class.
@@ -638,34 +660,34 @@
         manager_info = self.lookup_typeinfo(fullnames.MANAGER_CLASS_FULLNAME)
         if model_base is None or fk_field is None or manager_info is None:
             raise helpers.IncompleteDefnException()
 
         from_pk = self.get_pk_instance(self.model_classdef.info)
         fk_set_type, fk_get_type = get_field_descriptor_types(fk_field, is_set_nullable=False, is_get_nullable=False)
 
-        for defn in self.model_classdef.defs.body:
+        for statement in self.statements():
             # Check if this part of the class body is an assignment from a 'ManyToManyField' call
             # <field> = ManyToManyField(...)
             if (
-                isinstance(defn, AssignmentStmt)
-                and len(defn.lvalues) == 1
-                and isinstance(defn.lvalues[0], NameExpr)
-                and isinstance(defn.rvalue, CallExpr)
-                and len(defn.rvalue.args) > 0  # Need at least the 'to' argument
-                and isinstance(defn.rvalue.callee, RefExpr)
-                and isinstance(defn.rvalue.callee.node, TypeInfo)
-                and defn.rvalue.callee.node.has_base(fullnames.MANYTOMANY_FIELD_FULLNAME)
+                isinstance(statement, AssignmentStmt)
+                and len(statement.lvalues) == 1
+                and isinstance(statement.lvalues[0], NameExpr)
+                and isinstance(statement.rvalue, CallExpr)
+                and len(statement.rvalue.args) > 0  # Need at least the 'to' argument
+                and isinstance(statement.rvalue.callee, RefExpr)
+                and isinstance(statement.rvalue.callee.node, TypeInfo)
+                and statement.rvalue.callee.node.has_base(fullnames.MANYTOMANY_FIELD_FULLNAME)
             ):
-                m2m_field_name = defn.lvalues[0].name
-                m2m_field_symbol = self.model_classdef.info.names.get(m2m_field_name)
+                m2m_field_name = statement.lvalues[0].name
+                m2m_field_symbol = self.model_classdef.info.get(m2m_field_name)
                 # The symbol referred to by the assignment expression is expected to be a variable
                 if m2m_field_symbol is None or not isinstance(m2m_field_symbol.node, Var):
                     continue
                 # Resolve argument information of the 'ManyToManyField(...)' call
-                args = self.resolve_many_to_many_arguments(defn.rvalue, context=defn)
+                args = self.resolve_many_to_many_arguments(statement.rvalue, context=statement)
                 if (
                     # Ignore calls without required 'to' argument, mypy will complain
                     args is None
                     or not isinstance(args.to.model, Instance)
                     # Call has explicit 'through=', no need to create any implicit through table
                     or args.through is not None
                 ):
@@ -734,20 +756,22 @@
                 other_pk = self.get_pk_instance(args.to.model.type)
                 helpers.add_new_sym_for_info(through_model, name=f"{to_name}_id", sym_type=other_pk.copy_modified())
                 # Add a manager named 'objects'
                 helpers.add_new_sym_for_info(
                     through_model,
                     name="objects",
                     sym_type=Instance(manager_info, [Instance(through_model, [])]),
+                    is_classvar=True,
                 )
                 # Also add manager as '_default_manager' attribute
                 helpers.add_new_sym_for_info(
                     through_model,
                     name="_default_manager",
                     sym_type=Instance(manager_info, [Instance(through_model, [])]),
+                    is_classvar=True,
                 )
 
     @cached_property
     def default_pk_instance(self) -> Instance:
         default_pk_field = self.lookup_typeinfo(self.django_context.settings.DEFAULT_AUTO_FIELD)
         if default_pk_field is None:
             raise helpers.IncompleteDefnException()
```

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/orm_lookups.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/querysets.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/querysets.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/request.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/request.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/mypy_django_plugin/transformers/settings.py` & `django_stubs-5.0.0/mypy_django_plugin/transformers/settings.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.7/pyproject.toml` & `django_stubs-5.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,49 @@
 [tool.black]
 target-version = ['py38']
 line-length = 120
 include = '\.pyi?$'
 
 [tool.codespell]
-ignore-words-list = "aadd,acount,nam"
+ignore-words-list = "aadd,acount,nam,asend"
+
+[tool.pyright]
+include = [
+    "django-stubs",
+    "ext/django_stubs_ext",
+    "mypy_django_plugin",
+    "scripts",
+    "tests",
+]
+exclude = [
+    ".github",
+    ".mypy_cache",
+    "build",
+]
+reportMissingTypeArgument = "warning"
+reportPrivateUsage = "none"
+stubPath = "."
+typeCheckingMode = "strict"
+
+pythonVersion = "3.8"
+pythonPlatform = "All"
+
 
 [tool.ruff]
 # Adds to default excludes: https://ruff.rs/docs/settings/#exclude
 extend-exclude = [
     ".*/",
     "django-source",
     "stubgen",
     "out",
 ]
 line-length = 120
 target-version = "py38"
+
+[tool.ruff.lint]
 # See Rules in Ruff documentation: https://beta.ruff.rs/docs/rules/
 select = [
     "B",        # bugbear
     "E",        # pycodestyle
     "F",        # pyflakes
     "INP",      # flake8-tidy-imports
     "W",        # pycodestyle
@@ -29,31 +53,31 @@
     "PYI",      # flake8-pyi
     "RUF100",   # Equivalent to flake8-noqa NQA103
     "PGH004",   # Equivalent to flake8-noqa NQA104
     "PGH003",   # Disallowed blanket `type: ignore` annotations.
 ]
 ignore = ["PYI021", "PYI024", "PYI041", "PYI043"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "*.pyi" = [
     "B",
     "E501",
     "E741",
     "E743",
     "F403", # Use wildcard import
     "F405",
     "F822",
     "F821",
 ]
 "tests/*.py" = ["INP001"]
 "ext/tests/*.py" = ["INP001"]
 "setup.py" = ["INP001"]
 
-[tool.ruff.flake8-tidy-imports.banned-api]
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
 "_typeshed.Self".msg = "Use typing_extensions.Self (PEP 673) instead."
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["django_stubs_ext", "mypy_django_plugin"]
 split-on-trailing-comma = false
 
 [build-system]
 requires = ["setuptools", "wheel"]
```

### Comparing `django-stubs-4.2.7/setup.py` & `django_stubs-5.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
     "django",
-    "django-stubs-ext>=4.2.7",
+    "asgiref",
+    "django-stubs-ext>=5.0.0",
     "tomli; python_version < '3.11'",
     # Types:
     "typing-extensions",
-    "types-pytz",
     "types-PyYAML",
 ]
 
 # Keep compatible-mypy major.minor version pinned to what we use in CI (requirements.txt)
 extras_require = {
-    "compatible-mypy": ["mypy~=1.7.0"],
+    "compatible-mypy": ["mypy~=1.10.0"],
+    "redis": ["redis"],
 }
 
 setup(
     name="django-stubs",
-    version="4.2.7",
+    version="5.0.0",
     description="Mypy stubs for Django",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Maksim Kurnikov",
@@ -63,15 +64,16 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
         "Framework :: Django",
-        "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
     ],
     project_urls={
+        "Funding": "https://github.com/sponsors/typeddjango",
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
 )
```

### Comparing `django-stubs-4.2.7/tests/test_error_handling.py` & `django_stubs-5.0.0/tests/test_error_handling.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+import os
 import tempfile
 import uuid
 from contextlib import contextmanager
 from typing import Any, Generator, List, Optional
+from unittest import mock
 
 import pytest
 
 from mypy_django_plugin.config import DjangoPluginConfig
 
 TEMPLATE = """
 (config)
 ...
 [mypy.plugins.django-stubs]
-django_settings_module = str (required)
+django_settings_module = str (default: `os.getenv("DJANGO_SETTINGS_MODULE")`)
 strict_settings = bool (default: true)
 ...
 (django-stubs) mypy: error: {}
 """
 
 TEMPLATE_TOML = """
 (config)
 ...
 [tool.django-stubs]
-django_settings_module = str (required)
+django_settings_module = str (default: `os.getenv("DJANGO_SETTINGS_MODULE")`)
 strict_settings = bool (default: true)
 ...
 (django-stubs) mypy: error: {}
 """
 
 
 @contextmanager
@@ -42,20 +44,22 @@
         pytest.param(
             ["[not-really-django-stubs]"],
             "no section [mypy.plugins.django-stubs] found",
             id="missing-section",
         ),
         pytest.param(
             ["[mypy.plugins.django-stubs]", "\tnot_django_not_settings_module = badbadmodule"],
-            "missing required 'django_settings_module' config",
+            "missing required 'django_settings_module' config.\
+ Either specify this config or set your `DJANGO_SETTINGS_MODULE` env var",
             id="missing-settings-module",
         ),
         pytest.param(
             ["[mypy.plugins.django-stubs]"],
-            "missing required 'django_settings_module' config",
+            "missing required 'django_settings_module' config.\
+ Either specify this config or set your `DJANGO_SETTINGS_MODULE` env var",
             id="no-settings-given",
         ),
         pytest.param(
             ["[mypy.plugins.django-stubs]", "django_settings_module = some.module", "strict_settings = bad"],
             "invalid 'strict_settings': the setting must be a boolean",
             id="missing-settings-module",
         ),
@@ -108,15 +112,16 @@
             id="missing django-stubs section",
         ),
         pytest.param(
             """
             [tool.django-stubs]
             not_django_not_settings_module = "badbadmodule"
             """,
-            "missing required 'django_settings_module' config",
+            "missing required 'django_settings_module' config.\
+ Either specify this config or set your `DJANGO_SETTINGS_MODULE` env var",
             id="missing django_settings_module",
         ),
         pytest.param(
             "tool.django-stubs]",
             "could not load configuration file",
             id="invalid toml",
         ),
@@ -168,7 +173,44 @@
         ]
     )
     with write_to_file(config_file_contents) as filename:
         config = DjangoPluginConfig(filename)
 
     assert config.django_settings_module == "my.module"
     assert config.strict_settings is (boolean_value.lower() == "true")
+
+
+@pytest.mark.parametrize("boolean_value", ["true", "false"])
+def test_correct_toml_configuration_with_django_setting_from_env(boolean_value: str) -> None:
+    config_file_contents = f"""
+    [tool.django-stubs]
+    some_other_setting = "setting"
+    strict_settings = {boolean_value}
+    """
+    django_settings_env_value = "my.module"
+
+    with write_to_file(config_file_contents, suffix=".toml") as filename:
+        with mock.patch.dict(os.environ, {"DJANGO_SETTINGS_MODULE": django_settings_env_value}):
+            config = DjangoPluginConfig(filename)
+
+    assert config.django_settings_module == django_settings_env_value
+    assert config.strict_settings is (boolean_value == "true")
+
+
+@pytest.mark.parametrize("boolean_value", ["true", "True", "false", "False"])
+def test_correct_configuration_with_django_setting_from_env(boolean_value) -> None:
+    """Django settings module gets extracted given valid configuration."""
+    config_file_contents = "\n".join(
+        [
+            "[mypy.plugins.django-stubs]",
+            "some_other_setting = setting",
+            f"strict_settings = {boolean_value}",
+        ]
+    )
+    django_settings_env_value = "my.module"
+
+    with write_to_file(config_file_contents) as filename:
+        with mock.patch.dict(os.environ, {"DJANGO_SETTINGS_MODULE": django_settings_env_value}):
+            config = DjangoPluginConfig(filename)
+
+    assert config.django_settings_module == django_settings_env_value
+    assert config.strict_settings is (boolean_value.lower() == "true")
```

