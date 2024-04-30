# Comparing `tmp/django_codemod-2.1.8.tar.gz` & `tmp/django_codemod-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_codemod-2.1.8.tar", max compression
+gzip compressed data, was "django_codemod-2.1.9.tar", max compression
```

## Comparing `django_codemod-2.1.8.tar` & `django_codemod-2.1.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1068 2023-12-11 04:10:19.415606 django_codemod-2.1.8/LICENSE
--rw-r--r--   0        0        0    10088 2023-12-11 04:10:19.415606 django_codemod-2.1.8/README.md
--rw-r--r--   0        0        0     3614 2023-12-11 04:10:20.487605 django_codemod-2.1.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-12-11 04:10:20.487605 django_codemod-2.1.8/src/django_codemod/__init__.py
--rw-r--r--   0        0        0     8609 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/cli.py
--rw-r--r--   0        0        0      710 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/commands.py
--rw-r--r--   0        0        0      448 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/constants.py
--rw-r--r--   0        0        0      116 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/feature_flags.py
--rw-r--r--   0        0        0     3656 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/path_utils.py
--rw-r--r--   0        0        0        0 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/utils/__init__.py
--rw-r--r--   0        0        0     1346 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/utils/calls.py
--rw-r--r--   0        0        0     3367 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/__init__.py
--rw-r--r--   0        0        0     5979 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/admin.py
--rw-r--r--   0        0        0    14896 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/base.py
--rw-r--r--   0        0        0      379 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/core.py
--rw-r--r--   0        0        0     1223 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/crypto.py
--rw-r--r--   0        0        0     1107 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/decorators.py
--rw-r--r--   0        0        0     1042 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/encoding.py
--rw-r--r--   0        0        0     1431 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/exceptions.py
--rw-r--r--   0        0        0      699 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/forms.py
--rw-r--r--   0        0        0      415 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/html.py
--rw-r--r--   0        0        0     3240 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/http.py
--rw-r--r--   0        0        0      413 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/lru_cache.py
--rw-r--r--   0        0        0     7923 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/models.py
--rw-r--r--   0        0        0      390 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/os_utils.py
--rw-r--r--   0        0        0      422 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/paginator.py
--rw-r--r--   0        0        0     1116 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/postgres_fields.py
--rw-r--r--   0        0        0      648 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/shortcuts.py
--rw-r--r--   0        0        0     4000 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/signals.py
--rw-r--r--   0        0        0     1339 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/template_context.py
--rw-r--r--   0        0        0     5774 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/template_tags.py
--rw-r--r--   0        0        0     1259 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/timezone.py
--rw-r--r--   0        0        0     1654 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/translations.py
--rw-r--r--   0        0        0     4185 2023-12-11 04:10:19.419606 django_codemod-2.1.8/src/django_codemod/visitors/urls.py
--rw-r--r--   0        0        0        0 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/__init__.py
--rw-r--r--   0        0        0     6313 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/test_cli.py
--rwxr-xr-x   0        0        0      737 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/test_e2e.sh
--rw-r--r--   0        0        0     6959 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/test_path_utils.py
--rw-r--r--   0        0        0        0 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/__init__.py
--rw-r--r--   0        0        0      484 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/base.py
--rw-r--r--   0        0        0     7083 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_admin.py
--rw-r--r--   0        0        0    14132 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_base.py
--rw-r--r--   0        0        0      951 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_core.py
--rw-r--r--   0        0        0     2264 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_crypto.py
--rw-r--r--   0        0        0     1894 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_decorators.py
--rw-r--r--   0        0        0     1704 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_encoding.py
--rw-r--r--   0        0        0     2071 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_exceptions.py
--rw-r--r--   0        0        0      954 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_forms.py
--rw-r--r--   0        0        0      559 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_html.py
--rw-r--r--   0        0        0     5449 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_http.py
--rw-r--r--   0        0        0      531 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_lru_cache.py
--rw-r--r--   0        0        0    11946 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_models.py
--rw-r--r--   0        0        0      514 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_os_utils.py
--rw-r--r--   0        0        0     1351 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_paginator.py
--rw-r--r--   0        0        0     2560 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_postgres_fields.py
--rw-r--r--   0        0        0      671 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_shortcuts.py
--rw-r--r--   0        0        0     4248 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_signals.py
--rw-r--r--   0        0        0     1957 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_template_context.py
--rw-r--r--   0        0        0     4713 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_template_tags.py
--rw-r--r--   0        0        0     2409 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_timezone.py
--rw-r--r--   0        0        0     4501 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_translations.py
--rw-r--r--   0        0        0     6971 2023-12-11 04:10:19.419606 django_codemod-2.1.8/tests/visitors/test_urls.py
--rw-r--r--   0        0        0    11610 1970-01-01 00:00:00.000000 django_codemod-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-05 23:24:41.576313 django_codemod-2.1.9/LICENSE
+-rw-r--r--   0        0        0    10088 2024-01-05 23:24:41.576313 django_codemod-2.1.9/README.md
+-rw-r--r--   0        0        0     3614 2024-01-05 23:24:42.756319 django_codemod-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-01-05 23:24:42.756319 django_codemod-2.1.9/src/django_codemod/__init__.py
+-rw-r--r--   0        0        0     8609 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/cli.py
+-rw-r--r--   0        0        0      710 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/commands.py
+-rw-r--r--   0        0        0      448 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/constants.py
+-rw-r--r--   0        0        0      116 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/feature_flags.py
+-rw-r--r--   0        0        0     3656 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/path_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/utils/__init__.py
+-rw-r--r--   0        0        0     1346 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/utils/calls.py
+-rw-r--r--   0        0        0     3367 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/__init__.py
+-rw-r--r--   0        0        0     5979 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/admin.py
+-rw-r--r--   0        0        0    14896 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/base.py
+-rw-r--r--   0        0        0      379 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/core.py
+-rw-r--r--   0        0        0     1223 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/crypto.py
+-rw-r--r--   0        0        0     1107 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/decorators.py
+-rw-r--r--   0        0        0     1042 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/encoding.py
+-rw-r--r--   0        0        0     1431 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/exceptions.py
+-rw-r--r--   0        0        0      699 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/forms.py
+-rw-r--r--   0        0        0      415 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/html.py
+-rw-r--r--   0        0        0     3240 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/http.py
+-rw-r--r--   0        0        0      413 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/lru_cache.py
+-rw-r--r--   0        0        0     7923 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/models.py
+-rw-r--r--   0        0        0      390 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/os_utils.py
+-rw-r--r--   0        0        0      422 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/paginator.py
+-rw-r--r--   0        0        0     1116 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/postgres_fields.py
+-rw-r--r--   0        0        0      648 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/shortcuts.py
+-rw-r--r--   0        0        0     4000 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/signals.py
+-rw-r--r--   0        0        0     1339 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/template_context.py
+-rw-r--r--   0        0        0     5774 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/template_tags.py
+-rw-r--r--   0        0        0     1259 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/timezone.py
+-rw-r--r--   0        0        0     1654 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/translations.py
+-rw-r--r--   0        0        0     4185 2024-01-05 23:24:41.580313 django_codemod-2.1.9/src/django_codemod/visitors/urls.py
+-rw-r--r--   0        0        0        0 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     6313 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/test_cli.py
+-rwxr-xr-x   0        0        0      737 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/test_e2e.sh
+-rw-r--r--   0        0        0     6959 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/test_path_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/__init__.py
+-rw-r--r--   0        0        0      484 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/base.py
+-rw-r--r--   0        0        0     7155 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_admin.py
+-rw-r--r--   0        0        0    14276 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_base.py
+-rw-r--r--   0        0        0      951 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_core.py
+-rw-r--r--   0        0        0     2264 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_crypto.py
+-rw-r--r--   0        0        0     1894 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_decorators.py
+-rw-r--r--   0        0        0     1704 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_encoding.py
+-rw-r--r--   0        0        0     2071 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_exceptions.py
+-rw-r--r--   0        0        0      954 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_forms.py
+-rw-r--r--   0        0        0      559 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_html.py
+-rw-r--r--   0        0        0     5521 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_http.py
+-rw-r--r--   0        0        0      531 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_lru_cache.py
+-rw-r--r--   0        0        0    12018 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_models.py
+-rw-r--r--   0        0        0      514 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_os_utils.py
+-rw-r--r--   0        0        0     1375 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_paginator.py
+-rw-r--r--   0        0        0     2632 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_postgres_fields.py
+-rw-r--r--   0        0        0      671 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_shortcuts.py
+-rw-r--r--   0        0        0     4296 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_signals.py
+-rw-r--r--   0        0        0     1957 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_template_context.py
+-rw-r--r--   0        0        0     4809 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_template_tags.py
+-rw-r--r--   0        0        0     2457 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_timezone.py
+-rw-r--r--   0        0        0     4501 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_translations.py
+-rw-r--r--   0        0        0     6971 2024-01-05 23:24:41.580313 django_codemod-2.1.9/tests/visitors/test_urls.py
+-rw-r--r--   0        0        0    11610 1970-01-01 00:00:00.000000 django_codemod-2.1.9/PKG-INFO
```

### Comparing `django_codemod-2.1.8/LICENSE` & `django_codemod-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/README.md` & `django_codemod-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/pyproject.toml` & `django_codemod-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-codemod"
-version = "2.1.8"
+version = "2.1.9"
 description = "A command line tool to automatically fix Django deprecations."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "codemod", "libCST"]
 repository = "https://github.com/browniebroke/django-codemod"
 documentation = "https://django-codemod.readthedocs.io"
```

### Comparing `django_codemod-2.1.8/src/django_codemod/cli.py` & `django_codemod-2.1.9/src/django_codemod/cli.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/commands.py` & `django_codemod-2.1.9/src/django_codemod/commands.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/path_utils.py` & `django_codemod-2.1.9/src/django_codemod/path_utils.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/utils/calls.py` & `django_codemod-2.1.9/src/django_codemod/utils/calls.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/__init__.py` & `django_codemod-2.1.9/src/django_codemod/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/admin.py` & `django_codemod-2.1.9/src/django_codemod/visitors/admin.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/base.py` & `django_codemod-2.1.9/src/django_codemod/visitors/base.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/crypto.py` & `django_codemod-2.1.9/src/django_codemod/visitors/crypto.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/decorators.py` & `django_codemod-2.1.9/src/django_codemod/visitors/decorators.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/encoding.py` & `django_codemod-2.1.9/src/django_codemod/visitors/encoding.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/exceptions.py` & `django_codemod-2.1.9/src/django_codemod/visitors/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/forms.py` & `django_codemod-2.1.9/src/django_codemod/visitors/forms.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/http.py` & `django_codemod-2.1.9/src/django_codemod/visitors/http.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/models.py` & `django_codemod-2.1.9/src/django_codemod/visitors/models.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/postgres_fields.py` & `django_codemod-2.1.9/src/django_codemod/visitors/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/shortcuts.py` & `django_codemod-2.1.9/src/django_codemod/visitors/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/signals.py` & `django_codemod-2.1.9/src/django_codemod/visitors/signals.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/template_context.py` & `django_codemod-2.1.9/src/django_codemod/visitors/template_context.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/template_tags.py` & `django_codemod-2.1.9/src/django_codemod/visitors/template_tags.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/timezone.py` & `django_codemod-2.1.9/src/django_codemod/visitors/timezone.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/translations.py` & `django_codemod-2.1.9/src/django_codemod/visitors/translations.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/src/django_codemod/visitors/urls.py` & `django_codemod-2.1.9/src/django_codemod/visitors/urls.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/test_cli.py` & `django_codemod-2.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/test_e2e.sh` & `django_codemod-2.1.9/tests/test_e2e.sh`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/test_path_utils.py` & `django_codemod-2.1.9/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_admin.py` & `django_codemod-2.1.9/tests/visitors/test_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,43 +15,49 @@
             ("from django.contrib.admin import *", "TabularInline"),
             ("from django.contrib import *", "admin.TabularInline"),
             ("from django.contrib.admin import *", "StackedInline"),
             ("from django.contrib import *", "admin.StackedInline"),
         ]
     )
     def test_noop_import_star(self, import_line: str, base_class: str) -> None:
-        before = after = f"""
+        before = (
+            after
+        ) = f"""
             {import_line}
 
             class MyInlineInline(InlineMixin, {base_class}):
 
                 def has_add_permission(self, request):
                     if somethings:
                         return False
                     return super().has_add_permission(request)
         """
         self.assertCodemod(before, after)
 
     def test_model_admin_base_class(self) -> None:
         """Doesn't modify if base class doesn't match."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.contrib import admin
 
             class MyAdmin(admin.ModelAdmin):
 
                 def has_add_permission(self, request):
                     if somethings:
                         return False
                     return super().has_add_permission(request)
         """
         self.assertCodemod(before, after)
 
     def test_no_base_class(self) -> None:
         """Doesn't modify if there is no base class."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.contrib import admin
 
             class MyCustomStuff:
 
                 def has_add_permission(self, request):
                     if somethings:
                         return False
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_base.py` & `django_codemod-2.1.9/tests/visitors/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -274,50 +274,58 @@
 
             better_func()
             something(func="test")
         """
         self.assertCodemod(before, after)
 
     def test_avoid_try_import(self) -> None:
-        before = after = """
+        before = (
+            after
+        ) = """
             try:
                 from django.dummy.module import func
             except:
                 from django.dummy.other_module import better_func as func
 
             result = func()
         """
         with pytest.raises(SkipFile):
             self.assertCodemod(before, after)
 
     @pytest.mark.usefixtures("parent_module_import_enabled")
     def test_avoid_try_import_parent(self) -> None:
-        before = after = """
+        before = (
+            after
+        ) = """
             try:
                 from django.dummy import module
             except:
                 from django.dummy import other_module as module
 
             result = module.func()
         """
         with pytest.raises(SkipFile):
             self.assertCodemod(before, after)
 
     @pytest.mark.usefixtures("parent_module_import_enabled")
     def test_parent_import_star(self) -> None:
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.dummy import *
 
             result = module.func()
         """
         self.assertCodemod(before, after)
 
     @pytest.mark.usefixtures("parent_module_import_enabled")
     def test_parent_import_not_matches(self) -> None:
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.ymmud import other_module
 
             result = other_module.other_func()
         """
         self.assertCodemod(before, after)
 
 
@@ -403,15 +411,17 @@
             result = django_module.other_func()
         """
         self.assertCodemod(before, after)
 
     @pytest.mark.usefixtures("parent_module_import_enabled")
     def test_parent_module_noop(self) -> None:
         """Parent module imported, but other function used."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.dummy import module
 
             result = module.other_func()
         """
         self.assertCodemod(before, after)
 
     def test_already_imported(self) -> None:
@@ -462,15 +472,17 @@
             from django.dummy.other_module import func
 
             result = func()
         """
         self.assertCodemod(before, after)
 
     def test_avoid_try_import(self) -> None:
-        before = after = """
+        before = (
+            after
+        ) = """
             try:
                 from django.dummy.module import func
             except:
                 from django.dummy.other_module import better_func as func
 
             result = func()
         """
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_core.py` & `django_codemod-2.1.9/tests/visitors/test_core.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_crypto.py` & `django_codemod-2.1.9/tests/visitors/test_crypto.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_decorators.py` & `django_codemod-2.1.9/tests/visitors/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_encoding.py` & `django_codemod-2.1.9/tests/visitors/test_encoding.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_exceptions.py` & `django_codemod-2.1.9/tests/visitors/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_forms.py` & `django_codemod-2.1.9/tests/visitors/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_html.py` & `django_codemod-2.1.9/tests/visitors/test_html.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_http.py` & `django_codemod-2.1.9/tests/visitors/test_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,23 +98,27 @@
 
 
 class TestHttpRequestXReadLinesTransformer(BaseVisitorTest):
     transformer = HttpRequestXReadLinesTransformer
 
     def test_noop_wrong_name(self) -> None:
         """Don't replace calls for name other than `request` or `req`."""
-        before = after = """
+        before = (
+            after
+        ) = """
             for line in r.xreadlines():
                 print(line)
         """
         self.assertCodemod(before, after)
 
     def test_noop_function_call(self) -> None:
         """Don't replace calls for name other than `request` or `req`."""
-        before = after = """
+        before = (
+            after
+        ) = """
             for line in xreadlines(r):
                 print(line)
         """
         self.assertCodemod(before, after)
 
     @parameterized.expand(["req", "request"])
     def test_simple_substitution(self, variable_name) -> None:
@@ -165,15 +169,17 @@
         self.assertCodemod(before, after)
 
 
 class TestCookieDateTransformer(BaseVisitorTest):
     transformer = CookieDateTransformer
 
     def test_noop(self):
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.utils.http import http_date
 
             http_date(12345)
         """
         self.assertCodemod(before, after)
 
     def test_basic(self):
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_lru_cache.py` & `django_codemod-2.1.9/tests/visitors/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_models.py` & `django_codemod-2.1.9/tests/visitors/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,17 @@
         [
             ("from django.db import *",),
             ("from django.db.models import *",),
         ]
     )
     def test_noop_import_star(self, import_str: str) -> None:
         """Should not try to replace if import star is used."""
-        before = after = f"""
+        before = (
+            after
+        ) = f"""
             {import_str}
 
             class MyModel(models.Model):
 
                 @models.permalink
                 def url(self):
                     return ('guitarist_detail', [self.slug])
@@ -346,24 +348,28 @@
         self.assertCodemod(before, after)
 
 
 class TestNullBooleanFieldTransformer(BaseVisitorTest):
     transformer = NullBooleanFieldTransformer
 
     def test_noop_models(self) -> None:
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.db import models
 
             class MyThing(models.Model):
                 is_active = models.BooleanField()
         """
         self.assertCodemod(before, after)
 
     def test_noop_fields(self) -> None:
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.db.models import BooleanField, Model
 
             class MyThing(Model):
                 is_active = BooleanField()
         """
         self.assertCodemod(before, after)
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_os_utils.py` & `django_codemod-2.1.9/tests/visitors/test_os_utils.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_paginator.py` & `django_codemod-2.1.9/tests/visitors/test_paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 
 class TestQuerySetPaginatorTransformer(BaseVisitorTest):
     transformer = QuerySetPaginatorTransformer
 
     def test_noop(self) -> None:
         """Test when nothing should change."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.core.paginator import Paginator
 
             paginator_instance = Paginator([], 5)
         """
 
         self.assertCodemod(before, after)
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_postgres_fields.py` & `django_codemod-2.1.9/tests/visitors/test_postgres_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class TestFloatRangeModelFieldTransformer(BaseVisitorTest):
     transformer = FloatRangeModelFieldTransformer
 
     def test_noop(self) -> None:
         """Test when nothing should change."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.contrib.postgres.fields import DecimalRangeField
 
             some_range = DecimalRangeField()
         """
 
         self.assertCodemod(before, after)
 
@@ -36,15 +38,17 @@
 
 
 class TestFloatRangeFormFieldTransformer(BaseVisitorTest):
     transformer = FloatRangeFormFieldTransformer
 
     def test_noop(self) -> None:
         """Test when nothing should change."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.contrib.postgres.forms import DecimalRangeField
 
             some_range = DecimalRangeField()
         """
 
         self.assertCodemod(before, after)
 
@@ -65,15 +69,17 @@
 
 
 class TestJSONModelFieldTransformer(BaseVisitorTest):
     transformer = JSONModelFieldTransformer
 
     def test_noop(self) -> None:
         """Test when nothing should change."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.db.models import JSONField
 
             field = JSONField()
         """
 
         self.assertCodemod(before, after)
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_shortcuts.py` & `django_codemod-2.1.9/tests/visitors/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_signals.py` & `django_codemod-2.1.9/tests/visitors/test_signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,33 @@
         "m2m_changed",
         "pre_migrate",
         "post_migrate",
     ]
 
     @parameterized.expand(DJANGO_SIGNAL_NAMES)
     def test_noop(self, signal_name):
-        before = after = f"""
+        before = (
+            after
+        ) = f"""
             from django.db.models.signals import {signal_name}
 
             {signal_name}.disconnect(
                 receiver=some_handler,
                 sender=MyModel,
                 dispatch_uid='something-unique',
             )
         """
 
         self.assertCodemod(before, after)
 
     @parameterized.expand(DJANGO_SIGNAL_NAMES)
     def test_noop_import_star(self, signal_name):
-        before = after = f"""
+        before = (
+            after
+        ) = f"""
             from django.db.models.signals import *
 
             {signal_name}.disconnect(receiver=some_handler, sender=MyModel, weak=True)
         """
 
         self.assertCodemod(before, after)
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_template_context.py` & `django_codemod-2.1.9/tests/visitors/test_template_context.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_template_tags.py` & `django_codemod-2.1.9/tests/visitors/test_template_tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 
 class TestAssignmentTagTransformer(BaseVisitorTest):
     transformer = AssignmentTagTransformer
 
     def test_noop(self) -> None:
         """Test when nothing should change."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django import template
 
             register = template.Library()
 
 
             @register.simple_tag
             def some_tag():
@@ -26,27 +28,31 @@
         [
             ("from django import contrib",),
             ("from django.template import Engine",),
         ]
     )
     def test_noop_not_imported(self, import_line: str) -> None:
         """Test when import is missing."""
-        before = after = f"""
+        before = (
+            after
+        ) = f"""
             {import_line}
 
             @register.assignment_tag
             def some_tag():
                 return "Hello"
         """
 
         self.assertCodemod(before, after)
 
     def test_noop_import_star(self) -> None:
         """Test when imported as star import."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django import *
 
             register = template.Library()
 
 
             @register.assignment_tag
             def some_tag():
@@ -128,15 +134,17 @@
                 return "Hello"
         """
 
         self.assertCodemod(before, after)
 
     def test_noop_content_star_import(self) -> None:
         """Test when Library class is imported as star import."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from django.template import *
 
             register = Library()
 
 
             @register.assignment_tag
             def some_tag():
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_timezone.py` & `django_codemod-2.1.9/tests/visitors/test_timezone.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 
 class TestFixedOffsetTransformer(BaseVisitorTest):
     transformer = FixedOffsetTransformer
 
     def test_noop(self) -> None:
         """Test when nothing should change."""
-        before = after = """
+        before = (
+            after
+        ) = """
             from datetime import timedelta, timezone
 
             timezone(offset=timedelta(minutes=60))
         """
 
         self.assertCodemod(before, after)
 
@@ -72,13 +74,15 @@
 
             tz_info = timezone(timedelta(minutes=60), "example")
         """
 
         self.assertCodemod(before, after)
 
     def test_issue_421(self) -> None:
-        before = after = """
+        before = (
+            after
+        ) = """
         from django.utils import timezone
 
         now = timezone.now()
         """
         self.assertCodemod(before, after)
```

### Comparing `django_codemod-2.1.8/tests/visitors/test_translations.py` & `django_codemod-2.1.9/tests/visitors/test_translations.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/tests/visitors/test_urls.py` & `django_codemod-2.1.9/tests/visitors/test_urls.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.1.8/PKG-INFO` & `django_codemod-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codemod
-Version: 2.1.8
+Version: 2.1.9
 Summary: A command line tool to automatically fix Django deprecations.
 Home-page: https://github.com/browniebroke/django-codemod
 License: MIT
 Keywords: django,codemod,libCST
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-codemod Version: 2.1.8 Summary: A command
+Metadata-Version: 2.1 Name: django-codemod Version: 2.1.9 Summary: A command
 line tool to automatically fix Django deprecations. Home-page: https://
 github.com/browniebroke/django-codemod License: MIT Keywords:
 django,codemod,libCST Author: Bruno Alla Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

