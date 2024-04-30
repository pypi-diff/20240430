# Comparing `tmp/celery_starter-1.0.0.tar.gz` & `tmp/celery_starter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_starter-1.0.0.tar", last modified: Sun Apr 21 18:24:12 2024, max compression
+gzip compressed data, was "celery_starter-1.0.1.tar", last modified: Tue Apr 30 15:47:53 2024, max compression
```

## Comparing `celery_starter-1.0.0.tar` & `celery_starter-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 18:24:12.942511 celery_starter-1.0.0/
--rw-rw-rw-   0        0        0     1085 2024-04-16 14:24:28.000000 celery_starter-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       89 2024-04-16 22:07:38.000000 celery_starter-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2623 2024-04-21 18:24:12.939510 celery_starter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2024-04-16 22:32:31.000000 celery_starter-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 18:24:12.906510 celery_starter-1.0.0/celery_starter/
--rw-rw-rw-   0        0        0        0 2024-04-16 22:07:02.000000 celery_starter-1.0.0/celery_starter/__init__.py
--rw-rw-rw-   0        0        0      182 2024-04-16 22:16:28.000000 celery_starter-1.0.0/celery_starter/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:24:12.930513 celery_starter-1.0.0/celery_starter/management/
--rw-rw-rw-   0        0        0        0 2023-07-12 13:25:28.000000 celery_starter-1.0.0/celery_starter/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:24:12.937512 celery_starter-1.0.0/celery_starter/management/commands/
--rw-rw-rw-   0        0        0        0 2023-07-12 12:55:44.000000 celery_starter-1.0.0/celery_starter/management/commands/__init__.py
--rw-rw-rw-   0        0        0     2223 2024-04-16 22:08:17.000000 celery_starter-1.0.0/celery_starter/management/commands/_localization.py
--rw-rw-rw-   0        0        0     8212 2024-04-16 22:11:03.000000 celery_starter-1.0.0/celery_starter/management/commands/runcelery.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:24:12.939510 celery_starter-1.0.0/celery_starter.egg-info/
--rw-rw-rw-   0        0        0     2623 2024-04-21 18:24:12.000000 celery_starter-1.0.0/celery_starter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2024-04-21 18:24:12.000000 celery_starter-1.0.0/celery_starter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 18:24:12.000000 celery_starter-1.0.0/celery_starter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-21 18:24:12.000000 celery_starter-1.0.0/celery_starter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-21 18:24:12.000000 celery_starter-1.0.0/celery_starter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 18:24:12.943511 celery_starter-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1391 2024-04-17 08:18:26.000000 celery_starter-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.013289 celery_starter-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 15:47:48.000000 celery_starter-1.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.005289 celery_starter-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-30 15:47:48.000000 celery_starter-1.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 15:47:48.000000 celery_starter-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-30 15:47:48.000000 celery_starter-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-30 15:47:48.000000 celery_starter-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 15:47:48.000000 celery_starter-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-30 15:47:53.013289 celery_starter-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-30 15:47:48.000000 celery_starter-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-04-30 15:47:48.000000 celery_starter-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:47:53.013289 celery_starter-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.005289 celery_starter-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/src/celery_starter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/_localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/src/celery_starter/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/src/celery_starter/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/management/commands/runcelery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/src/celery_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 15:47:53.000000 celery_starter-1.0.1/src/celery_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/tests/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/management/commands/test_runcelery.py
```

### Comparing `celery_starter-1.0.0/celery_starter/management/commands/_localization.py` & `celery_starter-1.0.1/src/celery_starter/_localization.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import ctypes
-import locale
-import sys
-
-if sys.platform == 'win32':
-    localization = locale.windows_locale[ctypes.windll.kernel32.GetUserDefaultUILanguage()]
-else:
-    localization = 'ru_RU'
-
-command_help = """The command launching celery [worker, beat, flower]
- which are automatically restarted when any file is changed"""
-start_msg = 'Start celery (%s) [ worker %s%s] %s with function autoreload'
-debug_msg = ', in DEBUG mode'
-proj_name_help = 'The name of your django project.'
-beat_help = 'Excludes the beat server at startup.'
-flower_help = 'Excludes the flower server at startup.'
-debug_help = 'Displays information about successful/unsuccessful completion of processes.'
-log_level = 'Defines the logging level for celery worker/beat'
-log_file = 'Redirects the output to the console by default to a log file for celery worker/beat'
-celery_app_not_found = (
-    'The name of the celery app could not be found, pass the name manually as a positional parameter.'
-)
-
-if localization == 'ru_RU':
-    command_help = """Команда запускающая celery [worker, beat, flower]
-    которые автоматически перезапускаются при изменении любого файла"""
-    start_msg = 'Старт celery (%s) [ worker %s%s] %s с функцией autoreload'
-    debug_msg = ', в DEBUG режиме'
-    proj_name_help = 'Название вашего django проекта.'
-    beat_help = 'Исключает beat сервер при запуске.'
-    flower_help = 'Исключает flower сервер при запуске.'
-    debug_help = 'Отображает информацию о успешном/неудачном завершении процессов.'
-    log_level = 'Определяет уровень логирования для celery worker/beat'
-    log_file = 'Перенаправляет вывод в консоль по умолчанию в лог файл для celery worker/beat'
-    celery_app_not_found = """Не удалось найти название celery приложения,
- передайте название вручную, как позиционный параметр."""
+import ctypes
+import locale
+import sys
+
+if sys.platform == 'win32':
+    localization = locale.windows_locale[ctypes.windll.kernel32.GetUserDefaultUILanguage()]
+else:
+    localization = 'ru_RU'
+
+command_help = """The command launching celery [worker, beat, flower]
+ which are automatically restarted when any file is changed"""
+start_msg = 'Start celery (%s) [ worker %s%s] %s with function autoreload'
+debug_msg = ', in DEBUG mode'
+proj_name_help = 'The name of your django project.'
+beat_help = 'Excludes the beat server at startup.'
+flower_help = 'Excludes the flower server at startup.'
+debug_help = 'Displays information about successful/unsuccessful completion of processes.'
+log_level = 'Defines the logging level for celery worker/beat'
+log_file = 'Redirects the output to the console by default to a log file for celery worker/beat'
+celery_app_not_found = (
+    'The name of the celery app could not be found, pass the name manually as a positional parameter.'
+)
+
+if localization == 'ru_RU':
+    command_help = """Команда запускающая celery [worker, beat, flower]
+    которые автоматически перезапускаются при изменении любого файла"""
+    start_msg = 'Старт celery (%s) [ worker %s%s] %s с функцией autoreload'
+    debug_msg = ', в DEBUG режиме'
+    proj_name_help = 'Название вашего django проекта.'
+    beat_help = 'Исключает beat сервер при запуске.'
+    flower_help = 'Исключает flower сервер при запуске.'
+    debug_help = 'Отображает информацию о успешном/неудачном завершении процессов.'
+    log_level = 'Определяет уровень логирования для celery worker/beat'
+    log_file = 'Перенаправляет вывод в консоль по умолчанию в лог файл для celery worker/beat'
+    celery_app_not_found = """Не удалось найти название celery приложения,
+ передайте название вручную, как позиционный параметр."""
```

