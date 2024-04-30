# Comparing `tmp/pyslth-0.2.0.tar.gz` & `tmp/pyslth-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.2.0.tar", last modified: Mon Apr 29 09:48:27 2024, max compression
+gzip compressed data, was "pyslth-0.2.1.tar", last modified: Mon Apr 29 14:24:42 2024, max compression
```

## Comparing `pyslth-0.2.0.tar` & `pyslth-0.2.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.694618 pyslth-0.2.0/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.0/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-29 09:48:27.694371 pyslth-0.2.0/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.666019 pyslth-0.2.0/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-29 09:48:27.000000 pyslth-0.2.0/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1752 2024-04-29 09:48:27.000000 pyslth-0.2.0/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-29 09:48:27.000000 pyslth-0.2.0/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-29 09:48:27.000000 pyslth-0.2.0/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-29 09:48:27.000000 pyslth-0.2.0/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.0/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-29 09:48:27.694681 pyslth-0.2.0/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-29 09:47:38.000000 pyslth-0.2.0/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.672004 pyslth-0.2.0/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.0/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.2.0/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.672686 pyslth-0.2.0/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.0/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.0/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20281 2024-04-28 00:16:11.000000 pyslth-0.2.0/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.0/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.2.0/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.2.0/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.673225 pyslth-0.2.0/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.0/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.673945 pyslth-0.2.0/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.0/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.0/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.0/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.676920 pyslth-0.2.0/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.2.0/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.0/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.2.0/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.2.0/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.2.0/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.0/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.0/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.2.0/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.0/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.0/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19803 2024-04-29 09:46:27.000000 pyslth-0.2.0/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.0/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.677519 pyslth-0.2.0/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.0/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11326 2024-04-28 13:32:26.000000 pyslth-0.2.0/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.2.0/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.678061 pyslth-0.2.0/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.679488 pyslth-0.2.0/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.681824 pyslth-0.2.0/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.2.0/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.0/slth/static/css/solid.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.683820 pyslth-0.2.0/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.0/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.0/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.0/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.0/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.693454 pyslth-0.2.0/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-29 09:48:10.000000 pyslth-0.2.0/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)    81969 2024-04-29 09:48:10.000000 pyslth-0.2.0/slth/static/js/lib.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-29 09:48:10.000000 pyslth-0.2.0/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/js/slth.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.0/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 09:48:27.694009 pyslth-0.2.0/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     2244 2024-04-28 00:37:31.000000 pyslth-0.2.0/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.0/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.0/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-27 15:06:10.000000 pyslth-0.2.0/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.0/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.2.0/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.971407 pyslth-0.2.1/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.1/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-29 14:24:42.971204 pyslth-0.2.1/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.941921 pyslth-0.2.1/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1752 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.1/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-29 14:24:42.971465 pyslth-0.2.1/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-29 14:24:23.000000 pyslth-0.2.1/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.948090 pyslth-0.2.1/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.1/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.2.1/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.948700 pyslth-0.2.1/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.1/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.1/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20281 2024-04-28 00:16:11.000000 pyslth-0.2.1/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.2.1/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25161 2024-04-29 14:14:17.000000 pyslth-0.2.1/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.949010 pyslth-0.2.1/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.949631 pyslth-0.2.1/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.1/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.1/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.952127 pyslth-0.2.1/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.1/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.2.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.2.1/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.2.1/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.1/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.2.1/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.1/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19803 2024-04-29 09:46:27.000000 pyslth-0.2.1/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.1/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.952608 pyslth-0.2.1/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.1/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11326 2024-04-28 13:32:26.000000 pyslth-0.2.1/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.2.1/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.952942 pyslth-0.2.1/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.954184 pyslth-0.2.1/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.956449 pyslth-0.2.1/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.2.1/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.1/slth/static/css/solid.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.958305 pyslth-0.2.1/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.1/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.1/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.1/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.1/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.970408 pyslth-0.2.1/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-29 14:24:31.000000 pyslth-0.2.1/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    82788 2024-04-29 14:24:31.000000 pyslth-0.2.1/slth/static/js/lib.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-29 14:24:31.000000 pyslth-0.2.1/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/slth.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.970916 pyslth-0.2.1/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     2244 2024-04-28 00:37:31.000000 pyslth-0.2.1/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.1/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.1/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.1/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.2.1/slth/views.py
```

### Comparing `pyslth-0.2.0/PKG-INFO` & `pyslth-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.0
+Version: 0.2.1
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.0/pyslth.egg-info/PKG-INFO` & `pyslth-0.2.1/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.0
+Version: 0.2.1
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.0/pyslth.egg-info/SOURCES.txt` & `pyslth-0.2.1/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/setup.py` & `pyslth-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.2.0/slth/__init__.py` & `pyslth-0.2.1/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/components.py` & `pyslth-0.2.1/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/db/models.py` & `pyslth-0.2.1/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/endpoints.py` & `pyslth-0.2.1/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/factory.py` & `pyslth-0.2.1/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/forms.py` & `pyslth-0.2.1/slth/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,14 @@
         if name in self._actions:
             cls = ENDPOINTS[self._actions[name]]
             if cls.instantiate(self.request, self).check_permission():
                 data.update(action=cls.get_api_metadata(self.request, absolute_url(self.request)))
         return data
     
     def post(self):
-
         field_name = self.request.GET.get('on_change')
         if field_name:
             return self.on_change(field_name)
 
         data = {}
         errors = {}
         inline_fields = {name: field for name, field in self.fields.items() if isinstance(field, InlineFormField) or isinstance(field, InlineModelField)}
```

### Comparing `pyslth-0.2.0/slth/management/commands/integration_test.py` & `pyslth-0.2.1/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/management/commands/sync.py` & `pyslth-0.2.1/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/migrations/0001_initial.py` & `pyslth-0.2.1/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.2.1/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.2.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/migrations/0006_user.py` & `pyslth-0.2.1/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/models.py` & `pyslth-0.2.1/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/permissions.py` & `pyslth-0.2.1/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/queryset.py` & `pyslth-0.2.1/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/roles.py` & `pyslth-0.2.1/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/selenium/__init__.py` & `pyslth-0.2.1/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/selenium/browser.py` & `pyslth-0.2.1/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/serializer.py` & `pyslth-0.2.1/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/css/fontawesome.min.css` & `pyslth-0.2.1/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/css/fonts/Eina02-Bold.f8011405.ttf` & `pyslth-0.2.1/slth/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/css/fonts/Eina02-Regular.2e682693.ttf` & `pyslth-0.2.1/slth/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `pyslth-0.2.1/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.2.1/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/css/slth.css` & `pyslth-0.2.1/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/css/solid.min.css` & `pyslth-0.2.1/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/images/logo.png` & `pyslth-0.2.1/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/images/logo.svg` & `pyslth-0.2.1/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/images/user.png` & `pyslth-0.2.1/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/js/echarts.min.js` & `pyslth-0.2.1/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/js/index.min.js` & `pyslth-0.2.1/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/js/lib.min.js` & `pyslth-0.2.1/slth/static/js/lib.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -136,56 +136,56 @@
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function Be(e) {
+function Le(e) {
     return ge(e.data)
 }
 
-function L(e) {
+function B(e) {
     return e.replace("/app/", "/api/")
 }
 
 function F(e) {
     return e.replace("/api/", "/app/")
 }
 
 function D(e, n, a, r) {
-    const d = localStorage.getItem("token");
+    const o = localStorage.getItem("token");
     var i = {
         Accept: "application/json"
     };
-    d && (i.Authorization = "Token " + d);
-    const l = L(n);
-    var s = {
+    o && (i.Authorization = "Token " + o);
+    const l = B(n);
+    var d = {
         method: e,
         headers: new Headers(i),
         ajax: 1
     };
-    r && (s.body = r);
-    var o = null,
+    r && (d.body = r);
+    var c = null,
         u = null;
-    fetch(l, s).then(function(c) {
-        if (o = c, u = o.headers.get("Content-Type"), u == "application/json") return c.text();
-        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return c.arrayBuffer();
-        c.text()
-    }).then(c => {
+    fetch(l, d).then(function(s) {
+        if (c = s, u = c.headers.get("Content-Type"), u == "application/json") return s.text();
+        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return s.arrayBuffer();
+        s.text()
+    }).then(s => {
         if (u == "application/json") {
-            var m = JSON.parse(c || "{}");
-            typeof m == "object" && m.type == "redirect" ? document.location.href = F(m.url) : a && a(m, o)
+            var m = JSON.parse(s || "{}");
+            typeof m == "object" && m.type == "redirect" ? document.location.href = F(m.url) : a && a(m, c)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var y = window.URL.createObjectURL(new Blob([new Uint8Array(c)], {
+            var y = window.URL.createObjectURL(new Blob([new Uint8Array(s)], {
                     type: u
                 })),
                 v = document.createElement("a");
-            v.href = y, u.indexOf("excel") >= 0 ? v.download = "Download.xls" : u.indexOf("pdf") >= 0 ? v.download = "Download.pdf" : u.indexOf("zip") >= 0 ? v.download = "Download.zip" : u.indexOf("json") >= 0 ? v.download = "Download.json" : u.indexOf("csv") >= 0 ? v.download = "Download.csv" : u.indexOf("png") >= 0 && (v.download = "Download.png"), document.body.appendChild(v), v.click(), a && a({}, o)
-        } else a && a(c, o)
+            v.href = y, u.indexOf("excel") >= 0 ? v.download = "Download.xls" : u.indexOf("pdf") >= 0 ? v.download = "Download.pdf" : u.indexOf("zip") >= 0 ? v.download = "Download.zip" : u.indexOf("json") >= 0 ? v.download = "Download.json" : u.indexOf("csv") >= 0 ? v.download = "Download.csv" : u.indexOf("png") >= 0 && (v.download = "Download.png"), document.body.appendChild(v), v.click(), a && a({}, c)
+        } else a && a(s, c)
     })
 }
 
 function ge(e) {
     e.store && Object.keys(e.store).map(function(n) {
         e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
     }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = F(e.redirect)) : e.message && K(e.message)
@@ -216,37 +216,37 @@
     }
     return typeof e == "object" && e.type ? t.jsx(x, {
         data: e
     }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : t.jsx("ul", {
         style: {
             padding: 0
         },
-        children: e.map(function(d) {
+        children: e.map(function(o) {
             return t.jsx("li", {
-                children: d
+                children: o
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
 function xe() {
     document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ne, {}))
 }
 
 function ye(e, n) {
     fe(), xe(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
     H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {
-        url: L(e)
+        url: B(e)
     }))
 }
 
-function Le(e) {
+function Be(e) {
     fe(), xe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Re, {
-        url: L(e)
+        url: B(e)
     }))
 }
 
 function V(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
@@ -272,50 +272,50 @@
             V()
         },
         style: n
     })
 }
 
 function Oe(e) {
-    const [n, a] = M.useState(null), [r, d] = M.useState(0);
+    const [n, a] = M.useState(null), [r, o] = M.useState(0);
     M.useEffect(() => {
-        i(L(e.url)), document.querySelector(".layer").style.display = "block"
+        i(B(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
-    function i(o) {
-        D("GET", L(o), function(u) {
-            a(u), d(r + 1)
+    function i(c) {
+        D("GET", B(c), function(u) {
+            a(u), o(r + 1)
         })
     }
 
     function l() {
-        const o = {
+        const c = {
             textAlign: "right",
             cursor: "pointer"
         };
         if (n) return t.jsxs("div", {
             children: [t.jsx("div", {
-                style: o,
+                style: c,
                 children: t.jsx(k, {
                     icon: "x",
                     onClick: () => V()
                 })
             }), t.jsx(x, {
                 data: n
             })]
         })
     }
-    const s = {
+    const d = {
         minWidth: "50%",
         display: n ? "block" : "none",
         maxWidth: "90%",
         top: window.scrollY + 40
     };
     return t.jsx("dialog", {
-        style: s,
+        style: d,
         children: l()
     }, r)
 }
 
 function Re(e) {
     var n = Math.random();
     M.useEffect(() => {
@@ -327,30 +327,30 @@
     function a() {
         const r = {
                 minWidth: "50%",
                 display: "block",
                 maxWidth: "90%",
                 top: window.scrollY + 40
             },
-            d = {
+            o = {
                 float: "right",
                 cursor: "pointer",
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
-                style: d,
+                style: o,
                 children: t.jsx(k, {
                     icon: "x",
                     onClick: () => V()
                 })
             }), t.jsx("iframe", {
-                src: L(e.url),
+                src: B(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
                 }
             })]
         })
@@ -362,45 +362,45 @@
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
 function N(e) {
     const n = e.id || Math.random(),
         [a, r] = M.useState(e.data.name);
 
-    function d(s) {
-        s.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(s)) : e.data.modal == !1 ? window.load(F(e.data.url)) : ye(e.data.url)
+    function o(d) {
+        d.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(d)) : e.data.modal == !1 ? window.load(F(e.data.url)) : ye(e.data.url)
     }
 
     function i() {
-        return e.data.icon ? e.compact || !e.data.name ? t.jsx(k, {
+        return e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(k, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(k, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
 
     function l() {
-        var s = {
+        var d = {
             padding: 12,
             textDecoration: "none",
             borderRadius: 5,
             margin: 5
         };
-        return e.primary && (s.backgroundColor = "#1351b4", s.color = "white"), e.default && (s.border = "solid 1px #1351b4", s.color = "#1351b4"), e.style && Object.keys(e.style).map(function(o) {
-            s[o] = e.style[o]
+        return e.primary && (d.backgroundColor = "#1351b4", d.color = "white"), e.default && (d.border = "solid 1px #1351b4", d.color = "#1351b4"), e.style && Object.keys(e.style).map(function(c) {
+            d[c] = e.style[c]
         }), t.jsx("a", {
             id: n,
             href: F(e.data.url) || "#",
-            onClick: d,
-            style: s,
+            onClick: o,
+            style: d,
             "data-label": w(e.data.name),
             children: i()
         })
     }
     return l()
 }
 
@@ -408,24 +408,24 @@
     function n(i) {
         var l = i.target.parentNode.querySelector(".dropdown");
         return l == null && (l = i.target.parentNode.parentNode.querySelector(".dropdown")), l == null && (l = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), l
     }
 
     function a(i) {
         const l = i.target.getBoundingClientRect(),
-            s = n(i);
-        document.querySelectorAll(".dropdown").forEach(o => o.style.display = "none"), s.style.left = l.left - 150 + l.width + "px", s.style.display = "block"
+            d = n(i);
+        document.querySelectorAll(".dropdown").forEach(c => c.style.display = "none"), d.style.left = l.left - 150 + l.width + "px", d.style.display = "block"
     }
 
     function r(i) {
         const l = n(i);
         l.style.display = "none"
     }
 
-    function d() {
+    function o() {
         const i = {
                 padding: 0,
                 position: "absolute",
                 width: 150,
                 left: 0,
                 textAlign: "center",
                 backgroundColor: "white",
@@ -444,56 +444,56 @@
                 },
                 "data-label": w(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: i,
                 onMouseLeave: r,
                 className: "dropdown",
-                children: e.actions.map(s => t.jsx("li", {
+                children: e.actions.map(d => t.jsx("li", {
                     style: l,
                     children: t.jsx(N, {
-                        data: s,
+                        data: d,
                         style: {
                             padding: 0
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
-    return d()
+    return o()
 }
 
 function z({
     id: e,
     href: n,
     modal: a,
     imodal: r,
-    children: d,
+    children: o,
     onClick: i,
     dataLabel: l,
-    style: s
+    style: d
 }) {
-    const o = n && n.indexOf("/media/") < 0 ? F(n) : n;
+    const c = n && n.indexOf("/media/") < 0 ? F(n) : n;
 
     function u(m) {
-        m.preventDefault(), a ? ye(o) : r ? Le(o) : window.load(o)
+        m.preventDefault(), a ? ye(c) : r ? Be(c) : window.load(c)
     }
 
-    function c() {
+    function s() {
         return t.jsx("a", {
             id: e,
             onClick: i || u,
-            href: o || "#",
+            href: c || "#",
             "data-label": w(l),
-            style: s,
-            children: d
+            style: d,
+            children: o
         })
     }
-    return c()
+    return s()
 }
 
 function J(e) {
     function n() {
         const r = {
             display: "grid",
             gridGap: 0,
@@ -536,22 +536,22 @@
     return n()
 }
 
 function _e(e) {
     const n = Math.random(),
         [a, r] = M.useState(e.data);
 
-    function d(l) {
-        D("GET", l, function(s) {
-            r(s)
+    function o(l) {
+        D("GET", l, function(d) {
+            r(d)
         })
     }
 
     function i() {
-        return window[n] = () => d(e.data.url), t.jsx("div", {
+        return window[n] = () => o(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
             children: t.jsx(pe, {
                 data: a,
                 width: 100
             })
         })
@@ -621,37 +621,40 @@
 
     function r() {
         return t.jsx(ve, {
             data: e.data.actions
         })
     }
 
-    function d() {
+    function o() {
         const i = {
             border: "solid 1px #DDD",
             padding: 10,
             borderStyle: "dashed"
         };
         return t.jsxs("div", {
             style: i,
             children: [n(), a(), r()]
         })
     }
-    return d()
+    return o()
 }
 
 function ze(e) {
     function n() {
         const l = {
-            marginTop: 5,
-            marginBottom: 5
+            paddingTop: 15,
+            marginBottom: 10,
+            color: "#1151b3"
         };
-        return t.jsx("h3", {
+        return t.jsx("div", {
             style: l,
-            children: e.data.title
+            children: t.jsx("strong", {
+                children: e.data.title
+            })
         })
     }
 
     function a() {
         return t.jsx(be, {
             data: e.data.data,
             exclude: e.data.data[1].label
@@ -664,135 +667,135 @@
                 width: 140,
                 marginLeft: -128,
                 display: "flex",
                 justifyContent: "space-between",
                 marginTop: 10,
                 alignItems: "flex-end"
             },
-            s = {
+            d = {
                 maxWidth: 100
             },
-            o = {
+            c = {
                 width: 20,
                 height: 20,
                 border: "3px solid #1151b3",
                 backgroundColor: "white",
                 borderRadius: "50%"
             };
         return t.jsxs("div", {
             style: l,
             children: [t.jsx("div", {
-                style: s,
+                style: d,
                 children: e.data.data[1].value
             }), t.jsx("div", {
-                style: o
+                style: c
             })]
         })
     }
 
-    function d() {
+    function o() {
         return t.jsx(ve, {
             data: e.data.actions
         })
     }
 
     function i() {
         const l = {
                 borderBottom: "solid 1px #DDD",
                 padding: 0,
                 borderBottomStyle: "dashed",
                 marginLeft: 140,
                 borderLeft: "3px solid #1151b3",
-                marginBottom: -5
+                marginBottom: -10
             },
-            s = {
+            d = {
                 marginLeft: 20
             };
         return t.jsxs("div", {
             style: l,
             children: [r(), t.jsxs("div", {
-                style: s,
-                children: [n(), a(), d()]
+                style: d,
+                children: [n(), a(), o()]
             })]
         })
     }
     return i()
 }
 
 function He(e) {
     const n = Math.random(),
         [a, r] = M.useState(e.data);
 
-    function d() {
+    function o() {
         return t.jsx(we, {
             data: a
         })
     }
 
     function i() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
-        }) : a.data.map(function(o) {
-            return Array.isArray(o) ? t.jsx(J, {
+        }) : a.data.map(function(c) {
+            return Array.isArray(c) ? t.jsx(J, {
                 width: 300,
-                children: o.map(u => t.jsx($, {
+                children: c.map(u => t.jsx($, {
                     data: u,
-                    width: 100 / o.length
+                    width: 100 / c.length
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
                 children: t.jsx($, {
-                    data: o,
+                    data: c,
                     width: 100
                 })
             }, Math.random())
         }) : t.jsx(x, {
             data: a.data
         })
     }
 
-    function l(o) {
-        D("GET", o, function(u) {
+    function l(c) {
+        D("GET", c, function(u) {
             r(u)
         })
     }
 
-    function s() {
+    function d() {
         return e.data.url ? (window[n] = () => l(e.data.url), t.jsxs("div", {
             className: e.data.url && "reloadable",
             id: n,
-            children: [d(), i()]
+            children: [o(), i()]
         })) : t.jsxs("div", {
-            children: [d(), i()]
+            children: [o(), i()]
         })
     }
-    return s()
+    return d()
 }
 
 function Pe(e) {
     const n = Math.random(),
         [a, r] = M.useState(e.data.actions);
 
-    function d() {
-        const s = e.data.url.indexOf("?") < 0 ? "?" : "&";
-        return e.data.url + s + "only=actions"
+    function o() {
+        const d = e.data.url.indexOf("?") < 0 ? "?" : "&";
+        return e.data.url + d + "only=actions"
     }
 
     function i() {
-        D("GET", d(), function(s) {
-            r(s)
+        D("GET", o(), function(d) {
+            r(d)
         })
     }
 
     function l() {
         return window[n] = () => i(), t.jsx("div", {
             className: "reloadable",
             id: n,
-            children: a.map(function(s) {
+            children: a.map(function(d) {
                 return t.jsx(N, {
-                    data: s,
+                    data: d,
                     default: !0
                 }, Math.random())
             })
         })
     }
     return l()
 }
@@ -835,17 +838,17 @@
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h2", {
                 style: r,
                 "data-label": w(e.data.title),
                 children: e.data.title
             }), e.data.actions.length > 0 && t.jsx("div", {
-                children: e.data.actions.map(function(d) {
+                children: e.data.actions.map(function(o) {
                     return t.jsx(N, {
-                        data: d,
+                        data: o,
                         default: !0
                     }, Math.random())
                 })
             })]
         })
     }
     return n()
@@ -855,17 +858,17 @@
     function n() {
         return t.jsx(We, {
             data: e.data
         })
     }
 
     function a() {
-        return e.data.data.map(function(d, i) {
+        return e.data.data.map(function(o, i) {
             return t.jsx(x, {
-                data: d
+                data: o
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
@@ -878,20 +881,20 @@
     function n() {
         return t.jsx(we, {
             data: e.data
         })
     }
 
     function a() {
-        const d = {
+        const o = {
             backgroundColor: "white"
         };
         return e.data.data.map(function(i, l) {
             return t.jsx("div", {
-                style: d,
+                style: o,
                 children: t.jsx(x, {
                     data: i
                 }, Math.random())
             })
         })
     }
 
@@ -911,95 +914,95 @@
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20
             },
-            children: e.data.map(function(d, i) {
+            children: e.data.map(function(o, i) {
                 return t.jsx(z, {
-                    href: d.url,
+                    href: o.url,
                     style: {
                         padding: 5,
                         fontWeight: n == i ? "bold" : "normal",
                         borderBottom: n == i ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(l) {
-                        l.preventDefault(), a(i), e.loadContent(d.url)
+                        l.preventDefault(), a(i), e.loadContent(o.url)
                     },
-                    dataLabel: w(d.title),
-                    children: d.title
+                    dataLabel: w(o.title),
+                    children: o.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
 function Je(e) {
     var n = Math.random();
     const [a, r] = M.useState(e.data.data[0]);
 
-    function d() {
+    function o() {
         return e.data.title != "Top" && t.jsx("h2", {
             "data-label": w(e.data.title),
             children: e.data.title
         })
     }
 
     function i() {
         return t.jsx(Ve, {
             data: e.data.data,
-            loadContent: o
+            loadContent: c
         })
     }
 
     function l() {
-        var c = {
+        var s = {
             ...a
         };
-        c.title = null;
+        s.title = null;
         const m = {
             padding: 0
         };
         return t.jsx("div", {
             style: m,
             children: t.jsx(x, {
-                data: c
+                data: s
             }, Math.random())
         })
     }
 
-    function s() {
-        const c = {
+    function d() {
+        const s = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
-            style: c
+            style: s
         })
     }
 
-    function o(c) {
-        D("GET", c, function(m) {
+    function c(s) {
+        D("GET", s, function(m) {
             r(m)
         })
     }
 
     function u() {
-        return window[n] = () => o(a.url), e.data.data.length > 0 && t.jsxs("div", {
+        return window[n] = () => c(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [d(), i(), l(), s()]
+            children: [o(), i(), l(), d()]
         })
     }
     return u()
 }
 
 function $e() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
@@ -1008,20 +1011,20 @@
 }
 
 function A({
     id: e,
     onClick: n,
     icon: a,
     label: r,
-    display: d,
+    display: o,
     primary: i,
     compact: l,
-    spin: s
+    spin: d
 }) {
-    function o() {
+    function c() {
         return a ? l || !r ? t.jsx(k, {
             icon: a
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(Ie, {
                 style: {
                     marginRight: 10,
                     display: "none"
@@ -1032,33 +1035,33 @@
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
 
     function u() {
-        const c = {
+        const s = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
-            display: d || "block",
+            display: o || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return i ? (c.backgroundColor = "#1351b4", c.color = "white") : (c.border = "solid 1px #1351b4", c.color = "#1351b4"), t.jsx("a", {
+        return i ? (s.backgroundColor = "#1351b4", s.color = "white") : (s.border = "solid 1px #1351b4", s.color = "#1351b4"), t.jsx("a", {
             id: e,
-            style: c,
+            style: s,
             "data-label": w(r || a),
             onClick: m => {
-                m.preventDefault(), a && s && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
+                m.preventDefault(), a && d && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
             },
-            children: o()
+            children: c()
         })
     }
     return u()
 }
 const Ye = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
     Y = {
         padding: 15,
@@ -1104,17 +1107,17 @@
     else if (r.tagName == "SELECT") {
         if (r.style.display != "none") r.dispatchEvent(new CustomEvent("customchange", {
             detail: {
                 value: n
             }
         }));
         else
-            for (var d = 0; d < r.options.length; d++)
-                if (r.options[d].value == n) {
-                    r.selectedIndex = d;
+            for (var o = 0; o < r.options.length; o++)
+                if (r.options[o].value == n) {
+                    r.selectedIndex = o;
                     break
                 }
     }
 }
 
 function Ze(e) {
     if (e) {
@@ -1194,21 +1197,21 @@
     return n()
 }
 
 function Q(e) {
     const n = e.data.name + Math.random();
 
     function a() {
-        const s = {
+        const d = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
         return e.data.action && (e.data.action.modal = !0), t.jsxs("div", {
-            style: s,
+            style: d,
             children: [t.jsx("label", {
                 className: e.data.required ? "bold" : "",
                 children: e.data.label
             }), e.data.action && t.jsx(N, {
                 data: e.data.action,
                 style: {
                     padding: 0
@@ -1239,120 +1242,122 @@
         }) : e.data.type == "textarea" ? t.jsx(at, {
             data: e.data
         }) : t.jsx("span", {
             children: e.data.name
         })
     }
 
-    function d() {
+    function o() {
         return t.jsx("div", {
             children: t.jsx(tt, {
                 id: e.data.name + "_error"
             })
         })
     }
 
     function i() {
         return e.data.help_text && t.jsx(nt, {
             text: e.data.help_text
         })
     }
 
     function l() {
-        const s = {
+        const d = {
             display: e.data.type == "hidden" ? "none" : "flex",
             flexDirection: "column",
             padding: 5
         };
         return t.jsxs("div", {
             id: n,
             className: "form-group " + e.data.name,
-            style: s,
-            children: [a(), r(), i(), d()]
+            style: d,
+            children: [a(), r(), i(), o()]
         })
     }
     return l()
 }
 
 function ce(e) {
     var n = "";
     const a = e.data.name + Math.random();
     e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), M.useEffect(() => {
-        function l(u, c, m) {
+        function l(u, s, m) {
             var y = m.target,
                 v = y.value.replace(/\D/g, ""),
-                j = y.value.length > c ? 1 : 0;
+                j = y.value.length > s ? 1 : 0;
             VMasker(y).unMask(), VMasker(y).maskPattern(u[j]), y.value = VMasker.toPattern(v, u[j])
         }
         if (e.data.mask) {
-            var s = document.getElementById(a);
-            if (e.data.mask == "decimal") VMasker(s).maskMoney({
+            var d = document.getElementById(a);
+            if (e.data.mask == "decimal") VMasker(d).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
             });
             else if (e.data.mask.indexOf("|") > 0) {
-                var o = e.data.mask.split("|");
-                VMasker(s).maskPattern(o[0]), s.addEventListener("input", l.bind(void 0, o, 14), !1)
-            } else VMasker(s).maskPattern(e.data.mask)
+                var c = e.data.mask.split("|");
+                VMasker(d).maskPattern(c[0]), d.addEventListener("input", l.bind(void 0, c, 14), !1)
+            } else VMasker(d).maskPattern(e.data.mask)
         }
     }, []);
 
     function r(l) {
         je(l.target.closest("form"), e.data.onchange)
     }
 
-    function d(l) {
+    function o(l) {
         if (e.data.type == "file" && l.target.files) {
-            let o = l.target.files[0];
-            var s = new FileReader;
-            s.onload = function(u) {
-                if (ne(o.name)) {
+            let c = l.target.files[0];
+            var d = new FileReader;
+            d.onload = function(u) {
+                if (ne(c.name)) {
                     const v = "display" + a;
-                    var c = document.createElement("img");
-                    c.id = l.target.id + "img", c.style.width = "200px", c.style.display = "block", c.style.margin = "auto", c.style.marginTop = "20px", c.onload = function(j) {
-                        const I = e.data.width > e.data.height ? e.data.width / c.width : e.data.height / c.height;
+                    var s = document.createElement("img");
+                    s.id = l.target.id + "img", s.style.width = "200px", s.style.display = "block", s.style.margin = "auto", s.style.marginTop = "20px", s.onload = function(j) {
+                        const I = e.data.width > e.data.height ? e.data.width / s.width : e.data.height / s.height;
                         var T = document.createElement("canvas");
                         const q = T.getContext("2d");
-                        T.height = T.width * (c.height / c.width);
+                        T.height = T.width * (s.height / s.width);
                         const C = document.createElement("canvas"),
                             P = C.getContext("2d");
-                        C.width = c.width * I, C.height = c.height * I, P.drawImage(c, 0, 0, C.width, C.height), q.drawImage(C, 0, 0, C.width * I, C.height * I, 0, 0, T.width, T.height), C.toBlob(function(h) {
+                        C.width = s.width * I, C.height = s.height * I, P.drawImage(s, 0, 0, C.width, C.height), q.drawImage(C, 0, 0, C.width * I, C.height * I, 0, 0, T.width, T.height), C.toBlob(function(h) {
                             const g = new DataTransfer;
-                            g.items.add(new File([h], o.name)), l.target.files = g.files
+                            g.items.add(new File([h], c.name)), l.target.files = g.files
                         });
                         var p = document.getElementById(v);
-                        p == null ? (p = document.createElement("div"), p.id = v) : p.removeChild(p.childNodes[0]), p.appendChild(c), l.target.parentNode.appendChild(p)
-                    }, c.src = u.target.result
+                        p == null ? (p = document.createElement("div"), p.id = v) : p.removeChild(p.childNodes[0]), p.appendChild(s), l.target.parentNode.appendChild(p)
+                    }, s.src = u.target.result
                 }
                 const m = document.getElementById("fileinfo" + a);
-                var y = o.size / 1024;
-                y < 1024 ? y = parseInt(y) + " Kb" : y = (y / 1024).toFixed(2) + " Mb", m.innerHTML = o.name + " / " + y, e.data.max_size && o.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + y + ". Por favor, adicione um arquivo menor.")
-            }, s.readAsDataURL(o)
+                var y = c.size / 1024;
+                y < 1024 ? y = parseInt(y) + " Kb" : y = (y / 1024).toFixed(2) + " Mb", m.innerHTML = c.name + " / " + y, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + y + ". Por favor, adicione um arquivo menor.")
+            }, d.readAsDataURL(c)
         }
     }
 
     function i() {
         var l = e.data.type;
         if (l == "datetime" && (l = "datetime-regional"), l == "decimal" && (l = "text"), l == "file") {
             const u = {
                 alignContent: "center",
                 height: 75,
-                padding: 30,
-                maxWidth: "100%"
+                padding: 5,
+                maxWidth: "100%",
+                margin: "auto"
             };
-            var s = null;
-            return e.data.extensions && e.data.extensions.length > 0 && (s = e.data.extensions.map(c => "." + c).join(", ")), t.jsxs(t.Fragment, {
+            var d = null;
+            return e.data.extensions && e.data.extensions.length > 0 && (d = e.data.extensions.map(s => "." + s).join(", ")), t.jsxs(t.Fragment, {
                 children: [t.jsxs("div", {
                     style: {
-                        display: "flex",
+                        display: window.innerWidth < 800 ? "block" : "flex",
                         justifyContent: "space-between",
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
-                        borderRadius: 10
+                        borderRadius: 10,
+                        textAlign: "center"
                     },
                     children: [t.jsx("div", {
                         style: u,
                         children: t.jsx(k, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
@@ -1373,54 +1378,55 @@
                             style: {
                                 textAlign: "center"
                             },
                             children: e.data.value
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
-                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(c => "." + c).join(" ou "), "."]
+                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(s => "." + s).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
+                        align: "center",
                         children: t.jsx(A, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: l,
                     name: e.data.name,
                     id: a,
                     "data-label": w(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
-                    onChange: d,
+                    onChange: o,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
-                    accept: s
+                    accept: d
                 })]
             })
         } else {
-            var o = Y;
-            return l == "color" && (o = {
+            var c = Y;
+            return l == "color" && (c = {
                 ...Y
-            }, o.width = "100%", o.backgroundColor = "white", o.height = 47.5), t.jsx("input", {
+            }, c.width = "100%", c.backgroundColor = "white", c.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
                 type: l,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
                 "data-label": w(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
-                onChange: d,
-                style: o
+                onChange: o,
+                style: c
             })
         }
     }
     return i()
 }
 
 function ke(e) {
@@ -1432,27 +1438,27 @@
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
-        d = Array.isArray(e.data.value),
+        o = Array.isArray(e.data.value),
         [i, l] = M.useState(!1),
-        [s, o] = M.useState(null);
+        [d, c] = M.useState(null);
     var u = !1;
     M.useEffect(() => {
         q(n), document.getElementById(a).addEventListener("customchange", function(p) {
             q(p.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
-    function c() {
+    function s() {
         const p = document.getElementById(a);
-        if (d) {
+        if (o) {
             const h = {
                     padding: 5,
                     display: "inline"
                 },
                 g = {
                     cursor: "pointer",
                     marginRight: 5
@@ -1483,23 +1489,23 @@
                     }), b.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
     function m(p) {
-        o([])
+        c([])
     }
 
     function y() {
         return t.jsx("select", {
             onChange: m,
             id: a,
             name: e.data.name,
-            multiple: d,
+            multiple: o,
             readOnly: !0,
             style: {
                 display: "contents"
             }
         })
     }
 
@@ -1534,15 +1540,15 @@
             } else f += window.scrollY, b += window.scrollX;
             h.width = _.width, h.top = f, h.left = b
         }
         const S = {
                 cursor: "pointer",
                 padding: 10
             },
-            ee = !d && n.length > 0 && n[0].value || "";
+            ee = !o && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
             children: [t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
                 onFocus: E => {
@@ -1550,24 +1556,24 @@
                 },
                 onChange: T,
                 onMouseLeave: j,
                 onBlur: j,
                 defaultValue: ee,
                 style: p,
                 "data-label": w(e.data.label)
-            }), s && i && t.jsxs("ul", {
+            }), d && i && t.jsxs("ul", {
                 style: h,
                 onMouseLeave: I,
                 onMouseEnter: function(E) {
                     u = !0
                 },
-                children: [s.length == 0 && t.jsx("li", {
+                children: [d.length == 0 && t.jsx("li", {
                     style: S,
                     children: "Nenhuma opção encontrada."
-                }), s.map(E => t.jsx("li", {
+                }), d.map(E => t.jsx("li", {
                     onClick: () => {
                         l(!1), e.onSelect ? e.onSelect(E) : q(E)
                     },
                     style: S,
                     className: "autocomplete-item",
                     "data-label": w(E.value),
                     children: E.value
@@ -1581,39 +1587,39 @@
             I(p)
         }, 250)
     }
 
     function I(p) {
         const h = document.getElementById(a),
             g = document.getElementById(r);
-        d || h.options.length > 0 && g.value != h.options[0].innerHTML && (h.innerHTML = "", g.value = "", l(!1)), p.target.tagName == "UL" ? l(!1) : u || l(!1)
+        o || h.options.length > 0 && g.value != h.options[0].innerHTML && (h.innerHTML = "", g.value = "", l(!1)), p.target.tagName == "UL" ? l(!1) : u || l(!1)
     }
 
     function T(p) {
         const h = e.data.choices.indexOf("?") < 0 ? "?" : "&";
         l(!0), D("GET", e.data.choices + h + "term=" + p.target.value, function(f) {
-            o(f)
+            c(f)
         })
     }
 
     function q(p) {
         const h = document.getElementById(a),
             g = document.getElementById(r);
-        h.innerHTML == null && (h.innerHTML = ""), Array.isArray(p) ? h.innerHTML = p.map(f => `<option selected value="${f.id}">${f.value}</option>`).join("") : d ? (h.innerHTML += `<option selected value="${p.id}">${p.value}</option>`, g.value = "") : (h.innerHTML = `<option selected value="${p.id}">${p.value}</option>`, g.value = p.value), e.data.onchange && je(g.closest("form"), e.data.onchange)
+        h.innerHTML == null && (h.innerHTML = ""), Array.isArray(p) ? h.innerHTML = p.map(f => `<option selected value="${f.id}">${f.value}</option>`).join("") : o ? (h.innerHTML += `<option selected value="${p.id}">${p.value}</option>`, g.value = "") : (h.innerHTML = `<option selected value="${p.id}">${p.value}</option>`, g.value = p.value), e.data.onchange && je(g.closest("form"), e.data.onchange)
     }
 
     function C(p) {
         const h = document.getElementById(a);
         var g = Array.from(h.options);
-        h.innerHTML = g.slice(0, p).concat(g.slice(p + 1)).map(f => `<option selected value="${f.value}">${f.innerHTML}</option>`).join(""), o([])
+        h.innerHTML = g.slice(0, p).concat(g.slice(p + 1)).map(f => `<option selected value="${f.value}">${f.innerHTML}</option>`).join(""), c([])
     }
 
     function P() {
         return t.jsxs(t.Fragment, {
-            children: [c(), y(), v()]
+            children: [s(), y(), v()]
         })
     }
     return P()
 }
 
 function at(e) {
     function n() {
@@ -1644,73 +1650,73 @@
     })
 }
 
 function ae(e) {
     var n = Math.random(),
         a = e.data;
 
-    function r(s) {
-        return a.value != null ? a.value == s.id ? !0 : a.value.id == s.id : !1
+    function r(d) {
+        return a.value != null ? a.value == d.id ? !0 : a.value.id == d.id : !1
     }
 
-    function d(s) {
-        var o = document.getElementById(s);
-        a.checked && (o.checked = !1)
+    function o(d) {
+        var c = document.getElementById(d);
+        a.checked && (c.checked = !1)
     }
 
-    function i(s) {
-        var o = document.getElementById(s);
-        a.checked = o.checked
+    function i(d) {
+        var c = document.getElementById(d);
+        a.checked = c.checked
     }
 
     function l() {
         return t.jsx("div", {
             className: "radio-group",
-            children: a.choices.map((s, o) => t.jsxs("div", {
+            children: a.choices.map((d, c) => t.jsxs("div", {
                 style: {
                     paddingTop: 10
                 },
                 children: [t.jsx("input", {
-                    id: a.name + n + o,
+                    id: a.name + n + c,
                     type: "radio",
                     name: a.name,
-                    defaultValue: s.id,
-                    defaultChecked: r(s),
-                    "data-label": w(s.value),
+                    defaultValue: d.id,
+                    defaultChecked: r(d),
+                    "data-label": w(d.value),
                     onClick: function() {
-                        d(a.name + n + o)
+                        o(a.name + n + c)
                     },
                     onMouseEnter: function() {
-                        i(a.name + n + o)
+                        i(a.name + n + c)
                     }
                 }), t.jsx("label", {
-                    htmlFor: a.name + n + o,
-                    children: s.value
+                    htmlFor: a.name + n + c,
+                    children: d.value
                 })]
-            }, n + o))
+            }, n + c))
         })
     }
     return l()
 }
 
 function ue(e) {
     var n = Math.random(),
         a = e.data;
 
     function r(i) {
         var l = !1;
         if (a.value)
-            for (var s = 0; s < a.value.length; s++) {
-                var o = a.value[s];
-                (o == i.id || o.id == i.id) && (l = !0)
+            for (var d = 0; d < a.value.length; d++) {
+                var c = a.value[d];
+                (c == i.id || c.id == i.id) && (l = !0)
             }
         return l
     }
 
-    function d() {
+    function o() {
         return t.jsx("div", {
             className: "checkbox-group",
             children: a.choices.map((i, l) => t.jsxs("div", {
                 style: {
                     paddingTop: 10
                 },
                 children: [t.jsx("input", {
@@ -1723,15 +1729,15 @@
                 }), t.jsx("label", {
                     htmlFor: a.name + n + l,
                     children: i.value
                 })]
             }, n + l))
         })
     }
-    return d()
+    return o()
 }
 
 function it(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
@@ -1749,15 +1755,15 @@
 }
 
 function lt(e) {
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
-    function d() {
+    function o() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
             children: t.jsxs(ie, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
                 children: [t.jsx(A, {
@@ -1773,68 +1779,68 @@
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
         })
     }
 
-    function i(o) {
+    function i(c) {
         const u = document.querySelector("input[name=" + r.name + "]"),
-            c = document.getElementById("inline-form-" + n),
+            s = document.getElementById("inline-form-" + n),
             m = document.getElementById("show-" + n),
             y = document.getElementById("hide-" + n);
-        c.style.display = o ? "block" : "none", m.style.display = o ? "none" : "inline", y.style.display = o ? "inline" : "none", o ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+        s.style.display = c ? "block" : "none", m.style.display = c ? "none" : "inline", y.style.display = c ? "inline" : "none", c ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
     function l() {
-        const o = {
+        const c = {
             display: r.value ? "block" : "none"
         };
-        return e.data.required && (o.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
+        return e.data.required && (c.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
             className: "fieldset-inline-forms",
-            style: o,
+            style: c,
             id: "inline-form-" + n,
             children: e.data.value.map(function(u) {
                 return t.jsx(le, {
                     data: u
                 }, Math.random())
             })
         })
     }
 
-    function s() {
-        const o = {
+    function d() {
+        const c = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: o,
+                style: c,
                 "data-label": w(e.data.label),
                 children: e.data.label
-            }), d(), l()]
+            }), o(), l()]
         })
     }
-    return s()
+    return d()
 }
 
 function ot(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
-    function r(c, m) {
+    function r(s, m) {
         const y = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
             id: "form-" + y + "-" + a,
             children: [t.jsx(le, {
-                data: c
+                data: s
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
                 children: [t.jsx(A, {
@@ -1849,55 +1855,55 @@
                     onClick: () => l(y),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
-    function d() {
-        const c = s(),
-            m = c.length > 0 ? "none" : "inline";
+    function o() {
+        const s = d(),
+            m = s.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = m;
         for (var y = 0; y < n; y++) {
             var v = document.getElementById("extra-add-" + y + "-");
             v.style.display = "none"
         }
-        if (c.length > 0) {
-            var v = document.getElementById("extra-add-" + c[c.length - 1] + "-");
+        if (s.length > 0) {
+            var v = document.getElementById("extra-add-" + s[s.length - 1] + "-");
             v.style.display = "inline"
         }
     }
 
     function i() {
-        d();
-        var c = JSON.parse(JSON.stringify(e.data.template));
-        c.fields ? (c.fields.map(function(m) {
+        o();
+        var s = JSON.parse(JSON.stringify(e.data.template));
+        s.fields ? (s.fields.map(function(m) {
             m.name = m.name.replace("__n__", "__" + n + "__")
-        }), c.fields[0].value = 0) : c.fieldsets.map(function(m) {
+        }), s.fields[0].value = 0) : s.fieldsets.map(function(m) {
             m.fields.map(function(y) {
                 y.map(function(v) {
                     v.name = v.name.replace("__n__", "__" + n + "__")
                 }), y[0].value = 0
             })
-        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(c, "inline")), setTimeout(d, 100)
+        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(s, "inline")), setTimeout(o, 100)
     }
 
-    function l(c) {
+    function l(s) {
         const m = e.data.template,
-            v = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + c + "__"),
+            v = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + s + "__"),
             j = document.querySelector("input[name=" + v + "]");
-        parseInt(j.value) == 0 ? j.value = "" : j.value = -parseInt(j.value), document.getElementById("form-" + c + "-" + a).style.display = "none", d()
+        parseInt(j.value) == 0 ? j.value = "" : j.value = -parseInt(j.value), document.getElementById("form-" + s + "-" + a).style.display = "none", o()
     }
 
-    function s() {
-        for (var c = [], m = 0; m < n; m++) document.getElementById("form-" + m + "-" + a).style.display == "block" && c.push(m);
-        return c
+    function d() {
+        for (var s = [], m = 0; m < n; m++) document.getElementById("form-" + m + "-" + a).style.display == "block" && s.push(m);
+        return s
     }
 
-    function o() {
+    function c() {
         return t.jsx("div", {
             id: "info-" + a,
             children: t.jsx(ie, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
                 children: t.jsx(A, {
@@ -1908,29 +1914,29 @@
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
         })
     }
 
     function u() {
-        const c = {
+        const s = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: c,
+                style: s,
                 "data-label": w(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
-                children: [o(), e.data.value.map(function(m, y) {
+                children: [c(), e.data.value.map(function(m, y) {
                     return r(m, y == e.data.value.length - 1 ? "inline" : "none")
                 })]
             })]
         })
     }
     return u()
 }
@@ -1957,18 +1963,18 @@
                     "data-label": w(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), t.jsx("div", {
                     className: "fieldset-fields",
-                    children: r.fields.map(d => t.jsx("div", {
-                        children: d.map(i => t.jsx("div", {
+                    children: r.fields.map(o => t.jsx("div", {
+                        children: o.map(i => t.jsx("div", {
                             style: {
-                                width: 100 / d.length + "%",
+                                width: 100 / o.length + "%",
                                 display: i.type == "hidden" ? "none" : "inline-block"
                             },
                             children: n(i)
                         }, Math.random()))
                     }, Math.random()))
                 })]
             })
@@ -1977,36 +1983,36 @@
     return a()
 }
 
 function dt(e) {
     const n = Math.random();
 
     function a() {
-        const c = {
+        const s = {
             margin: 0,
             textAlign: "left"
         };
         return t.jsx("h1", {
-            style: c,
+            style: s,
             children: e.data.title
         })
     }
 
     function r() {
         return e.data.info && t.jsx(et, {
             data: {
                 text: e.data.info
             }
         })
     }
 
-    function d() {
+    function o() {
         if (e.data.display) return t.jsxs(t.Fragment, {
-            children: [e.data.display.map(c => t.jsx(x, {
-                data: c
+            children: [e.data.display.map(s => t.jsx(x, {
+                data: s
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
             })]
         })
     }
@@ -2020,91 +2026,96 @@
     function l() {
         return t.jsxs("div", {
             style: {
                 marginTop: 20,
                 textAlign: "right"
             },
             children: [t.jsx(A, {
-                onClick: o,
+                onClick: c,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
             }), t.jsx(A, {
                 onClick: u,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
         })
     }
 
-    function s() {
+    function d() {
         return t.jsxs("form", {
             id: n,
             action: e.data.url,
             style: {
                 margin: "auto",
                 width: e.data.width,
                 backgroundColor: "white"
             },
             children: [t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [a(), r(), d(), i(), l()]
+                children: [a(), r(), o(), i(), l()]
             })]
         })
     }
 
-    function o() {
+    function c() {
         V()
     }
 
-    function u(c) {
-        c.preventDefault();
+    function u(s) {
+        s.preventDefault();
         var m = document.getElementById(n),
             y = new FormData(m);
         D("POST", e.data.url, function(j) {
-            if (c.target.dataset.spinning && (c.target.querySelector("i.fa-spin").style.display = "none", c.target.querySelector("i.fa-" + c.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return V(), $e(), ge(j);
+            if (s.target.dataset.spinning && (s.target.querySelector("i.fa-spin").style.display = "none", s.target.querySelector("i.fa-" + s.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return V(), $e(), ge(j);
             var I = j.text;
             console.log(j), Object.keys(j.errors).map(function(T) {
                 if (T == "__all__") I = j.errors[T];
                 else {
                     const q = m.querySelector("#" + T + "_error");
                     q.querySelector("span").innerHTML = j.errors[T], q.style.display = "block"
                 }
             }), K(I, !0)
         }, y)
     }
-    return s()
+    return d()
 }
 
 function st(e) {
     e.data.id == null && (e.data.id = Math.random());
     const [n, a] = M.useState(e.data);
 
     function r() {
+        const h = {
+            margin: 0
+        };
         return n.attrname ? t.jsx("h2", {
+            style: h,
             "data-label": w(n.title),
             children: n.title
         }) : t.jsx("h1", {
+            style: h,
             "data-label": w(n.title),
             children: n.title
         })
     }
 
-    function d() {
+    function o() {
         const h = {
             display: "flex",
             justifyContent: "space-between",
-            alignItems: "baseline"
+            alignItems: "center"
         };
         return t.jsxs("div", {
             style: h,
             children: [r(), t.jsx("i", {
                 id: "loader-" + e.data.id,
                 style: {
                     display: "none"
@@ -2138,34 +2149,34 @@
                         paddingRight: 15,
                         fontWeight: f ? "bold" : "normal",
                         borderBottom: f ? "solid 3px #2670e8" : "solid 3px #DDD",
                         textDecoration: "none",
                         color: "#0c326f"
                     },
                     onClick: function(b) {
-                        b.preventDefault(), s(h.name)
+                        b.preventDefault(), d(h.name)
                     },
                     dataLabel: w(h.label),
                     children: t.jsxs("div", {
                         style: {
                             display: "inline-block"
                         },
                         children: [h.label, " (", h.count, ")"]
                     })
                 }, Math.random())
             })
         })
     }
 
-    function s(h) {
+    function d(h) {
         const g = document.getElementById("subset-" + e.data.id);
         g.value = h || "", C()
     }
 
-    function o(h, g, f) {
+    function c(h, g, f) {
         const b = document.getElementById("form-" + e.data.id);
         b.querySelector("input[name=" + n.calendar.field + "__day]").value = h || "", b.querySelector("input[name=" + n.calendar.field + "__month]").value = g || "", b.querySelector("input[name=" + n.calendar.field + "__year]").value = f || "", C()
     }
 
     function u() {
         if (n.calendar) {
             const S = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
@@ -2232,88 +2243,88 @@
                 className: "calendar",
                 children: [t.jsxs("div", {
                     style: Te,
                     children: [t.jsx("div", {
                         children: t.jsx(se, {
                             default: !0,
                             icon: "arrow-left",
-                            onClick: () => o(null, n.calendar.previous.month, n.calendar.previous.year)
+                            onClick: () => c(null, n.calendar.previous.month, n.calendar.previous.year)
                         })
                     }), t.jsxs("div", {
                         children: [t.jsxs("h3", {
                             align: "center",
                             style: {
                                 margin: 0
                             },
                             children: [ee[n.calendar.month - 1], " ", n.calendar.year]
                         }), n.calendar.day && t.jsxs("div", {
                             align: "center",
                             className: O,
                             children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(k, {
                                 default: !0,
                                 icon: "x",
-                                onClick: () => o(null, n.calendar.month, n.calendar.year),
+                                onClick: () => c(null, n.calendar.month, n.calendar.year),
                                 style: {
                                     marginLeft: 10,
                                     cursor: "pointer"
                                 }
                             })]
                         })]
                     }), t.jsx("div", {
                         children: t.jsx(se, {
                             default: !0,
                             icon: "arrow-right",
-                            onClick: () => o(null, n.calendar.next.month, n.calendar.next.year)
+                            onClick: () => c(null, n.calendar.next.month, n.calendar.next.year)
                         })
                     })]
                 }), t.jsxs("table", {
                     style: E,
                     children: [t.jsx("thead", {
                         children: t.jsx("tr", {
                             children: S.map(te => t.jsx("th", {
                                 children: te
                             }, Math.random()))
                         })
                     }), t.jsx("tbody", {
                         children: h.map(te => t.jsx("tr", {
-                            children: te.map(B => t.jsxs("td", {
+                            children: te.map(L => t.jsxs("td", {
                                 style: W,
                                 children: [t.jsx("div", {
                                     style: O,
-                                    children: B.today ? t.jsx("span", {
+                                    children: L.today ? t.jsx("span", {
                                         style: {
                                             textDecoration: "underline"
                                         },
-                                        children: B.date
-                                    }) : B.date + B.today
-                                }), B.total && t.jsx("div", {
+                                        children: L.date
+                                    }) : L.date + L.today
+                                }), L.total && t.jsx("div", {
                                     style: G,
-                                    onClick: () => o(B.date, n.calendar.month, n.calendar.year),
+                                    onClick: () => c(L.date, n.calendar.month, n.calendar.year),
                                     children: t.jsx("div", {
                                         style: _,
                                         children: t.jsx("span", {
                                             style: {
-                                                textDecoration: B.selected ? "underline" : "normal"
+                                                textDecoration: L.selected ? "underline" : "normal"
                                             },
-                                            children: B.total
+                                            children: L.total
                                         })
                                     })
-                                }), !B.total && t.jsx("div", {
+                                }), !L.total && t.jsx("div", {
                                     style: G,
                                     children: " "
                                 })]
                             }, Math.random()))
                         }, Math.random()))
                     })]
                 })]
             })
         }
     }
 
-    function c(h) {
+    function s(h) {
         const g = {
             textAlign: "left",
             verticalAlign: "top",
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
             children: [h.map(function(f) {
@@ -2406,15 +2417,15 @@
                 borderSpacing: 0
             };
         return t.jsx("div", {
             style: h,
             children: t.jsxs("table", {
                 style: g,
                 children: [t.jsx("thead", {
-                    children: c(n.data[0].data)
+                    children: s(n.data[0].data)
                 }), t.jsx("tbody", {
                     children: n.data.map(function(f) {
                         return m(f)
                     })
                 })]
             })
         })
@@ -2616,29 +2627,29 @@
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
-                }), d(), P()]
+                }), o(), P()]
             })
         })
     }
     return p()
 }
 
 function Z(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
         if (r) {
-            var d = echarts.init(r);
-            d.setOption(e.option)
+            var o = echarts.init(r);
+            o.setOption(e.option)
         } else setTimeout(a, 1e3)
     }
     return setTimeout(a, 1e3), t.jsx("div", {
         id: n,
         style: {
             width: "100%",
             height: 300
@@ -2654,17 +2665,17 @@
         ["40%", "48%"],
         ["30%", "48%"],
         ["20%", "28%"],
         ["10%", "18%"]
     ];
 
     function a() {
-        return e.headers ? e.headers.slice(1).map(function(d, i) {
+        return e.headers ? e.headers.slice(1).map(function(o, i) {
             return {
-                name: d,
+                name: o,
                 type: "pie",
                 radius: n[i],
                 emphasis: {
                     label: {
                         show: !0,
                         formatter: function(l) {
                             return l.value.toLocaleString("pt-BR")
@@ -2683,32 +2694,32 @@
         }) : {
             name: null,
             type: "pie",
             radius: e.donut ? ["25%", "65%"] : ["0%", "75%"],
             emphasis: {
                 label: {
                     show: !0,
-                    formatter: function(d) {
-                        return d.value.toLocaleString("pt-BR")
+                    formatter: function(o) {
+                        return o.value.toLocaleString("pt-BR")
                     },
                     fontWeight: "bold"
                 }
             },
             roseType: e.area ? "area" : null,
-            data: e.rows.map(function(d, i) {
+            data: e.rows.map(function(o, i) {
                 return {
-                    name: d[0],
-                    value: d[1]
+                    name: o[0],
+                    value: o[1]
                 }
             })
         }
     }
 
     function r() {
-        var d = {
+        var o = {
             tooltip: {
                 trigger: "item",
                 formatter: function(i) {
                     return `${i.name}: <b>${i.data.value.toLocaleString("pt-BR")}</b> (${i.percent.toLocaleString("pt-BR")}%)`
                 }
             },
             legend: {},
@@ -2717,15 +2728,15 @@
                 formatter(i) {
                     return i.name + " (" + i.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
         return t.jsx(Z, {
-            option: d
+            option: o
         })
     }
     return r()
 }
 
 function ct(e) {
     return t.jsx(oe, {
@@ -2743,15 +2754,15 @@
     })
 }
 
 function R(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
-        d = {
+        o = {
             type: "value"
         },
         i = {
             show: !0,
             feature: {
                 mark: {
                     show: !0
@@ -2759,48 +2770,48 @@
                 saveAsImage: {
                     show: !0
                 }
             }
         },
         l = e.area ? {} : null;
 
-    function s() {
+    function d() {
         return e.headers ? {
             type: "category",
             data: e.headers.slice(1)
         } : {
             type: "category",
-            data: e.rows.map(function(c) {
-                return c[0]
+            data: e.rows.map(function(s) {
+                return s[0]
             })
         }
     }
 
-    function o() {
-        return e.headers ? e.rows.map(function(c) {
+    function c() {
+        return e.headers ? e.rows.map(function(s) {
             return {
-                name: c[0],
-                data: c.slice(1),
+                name: s[0],
+                data: s.slice(1),
                 type: a,
                 stack: r,
                 areaStyle: l
             }
         }) : [{
             name: null,
-            data: e.rows.map(function(c) {
-                return c[1]
+            data: e.rows.map(function(s) {
+                return s[1]
             }),
             type: a,
             stack: r,
             areaStyle: l
         }]
     }
 
     function u() {
-        var c = {
+        var s = {
             toolbox: i,
             tooltip: {
                 trigger: "axis",
                 axisPointer: {
                     type: "shadow"
                 },
                 formatter: function(m) {
@@ -2810,20 +2821,20 @@
             legend: {},
             label: {
                 show: !0,
                 formatter: function(m) {
                     return m.value.toLocaleString("pt-BR")
                 }
             },
-            xAxis: n ? d : s(),
-            yAxis: n ? s() : d,
-            series: o()
+            xAxis: n ? o : d(),
+            yAxis: n ? d() : o,
+            series: c()
         };
         return t.jsx(Z, {
-            option: c
+            option: s
         })
     }
     return u()
 }
 
 function ht(e) {
     return t.jsx(R, {
@@ -2876,22 +2887,22 @@
 
 function pt(e) {
     function n() {
         return e.headers ? [{
             type: "treemap",
             roam: "move",
             nodeClick: !0,
-            data: e.headers.slice(1).map(function(r, d) {
+            data: e.headers.slice(1).map(function(r, o) {
                 return {
                     name: r,
                     type: "pie",
                     children: e.rows.map(function(i) {
                         return {
                             name: i[0],
-                            value: i[d + 1]
+                            value: i[o + 1]
                         }
                     })
                 }
             })
         }] : [{
             type: "treemap",
             roam: "move",
@@ -2909,16 +2920,16 @@
         var r = {
             tooltip: {
                 trigger: "item"
             },
             legend: {},
             label: {
                 show: !0,
-                formatter(d) {
-                    return d.name + " (" + d.value.toLocaleString("pt-BR") + ")"
+                formatter(o) {
+                    return o.name + " (" + o.value.toLocaleString("pt-BR") + ")"
                 }
             },
             series: n()
         };
         return t.jsx(Z, {
             option: r
         })
@@ -3054,15 +3065,15 @@
         })
     }
     return a()
 }
 
 function bt(e) {
     function n() {
-        for (var r = [], d = 0; d < e.data.series.length; d++) r.push([e.data.series[d][0], e.data.series[d][1]]);
+        for (var r = [], o = 0; o < e.data.series.length; o++) r.push([e.data.series[o][0], e.data.series[o][1]]);
         return e.data.chart ? t.jsx(he, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
@@ -3070,42 +3081,42 @@
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%"
                 },
                 children: t.jsx("tbody", {
                     children: r.map(i => t.jsx("tr", {
-                        children: i.map((l, s) => s == 0 ? t.jsx("th", {
+                        children: i.map((l, d) => d == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left"
                             },
                             children: l
                         }, Math.random()) : t.jsx("td", {
                             children: U(l)
                         }, Math.random()))
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
-        for (var r = [], d = [], i = Object.keys(e.data.series), l = [], s = 0; s < i.length; s++) {
-            s == 0 && r.push("");
-            for (var o = [i[s]], u = 0, c = 0; c < e.data.series[i[s]].length; c++) {
-                var m = e.data.series[i[s]];
-                s == 0 && r.push(m[c][0]), o.push(m[c][1]), u += m[c][1], i.length > 1 && (s == 0 ? l.push(m[c][1]) : l[c] += m[c][1], c > 0 && c == e.data.series[i[s]].length - 1 && (s == 0 ? l.push(u) : l[c + 1] += u))
+        for (var r = [], o = [], i = Object.keys(e.data.series), l = [], d = 0; d < i.length; d++) {
+            d == 0 && r.push("");
+            for (var c = [i[d]], u = 0, s = 0; s < e.data.series[i[d]].length; s++) {
+                var m = e.data.series[i[d]];
+                d == 0 && r.push(m[s][0]), c.push(m[s][1]), u += m[s][1], i.length > 1 && (d == 0 ? l.push(m[s][1]) : l[s] += m[s][1], s > 0 && s == e.data.series[i[d]].length - 1 && (d == 0 ? l.push(u) : l[s + 1] += u))
             }
-            o.length > 2 && (s == 0 && r.push("TOTAL"), o.push(u)), d.push(o)
+            c.length > 2 && (d == 0 && r.push("TOTAL"), c.push(u)), o.push(c)
         }
         return e.data.chart ? t.jsx(he, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
-            rows: d
+            rows: o
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
                 "data-label": w(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
@@ -3114,15 +3125,15 @@
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: r.map(y => t.jsx("th", {
                             children: y
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [d.map(y => t.jsx("tr", {
+                    children: [o.map(y => t.jsx("tr", {
                         children: y.map((v, j) => j == 0 ? t.jsx("th", {
                             children: v
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
                             style: {
                                 backgroundColor: j == y.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
                             },
@@ -3194,64 +3205,64 @@
                 })
             })]
         })
     }
 
     function n(i) {
         var l = i.target;
-        const s = l.querySelector(":scope > ul, :scope > li");
-        if (s) {
-            s.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(c) {
-                c.style.display = "block"
-            }) : l.querySelectorAll(":scope > ul, :scope > li").forEach(function(c) {
-                c.style.display = "none"
+        const d = l.querySelector(":scope > ul, :scope > li");
+        if (d) {
+            d.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(s) {
+                s.style.display = "block"
+            }) : l.querySelectorAll(":scope > ul, :scope > li").forEach(function(s) {
+                s.style.display = "none"
             });
-            const o = l.querySelector(":scope > i.fa-solid.fa-chevron-right"),
+            const c = l.querySelector(":scope > i.fa-solid.fa-chevron-right"),
                 u = l.querySelector(":scope > i.fa-solid.fa-chevron-up");
-            return o && (o.classList.remove("fa-chevron-right"), o.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), i.preventDefault(), i.stopPropagation(), i.cancelBubble = !0, !1
+            return c && (c.classList.remove("fa-chevron-right"), c.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), i.preventDefault(), i.stopPropagation(), i.cancelBubble = !0, !1
         } else {
-            const o = document.querySelector("aside");
-            o.style.display = window.innerWidth < 800 ? "none" : "block"
+            const c = document.querySelector("aside");
+            c.style.display = window.innerWidth < 800 ? "none" : "block"
         }
     }
 
     function a(i, l) {
-        const s = {
+        const d = {
                 display: l == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 5,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem"
             },
-            o = {
+            c = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return i.url ? t.jsx("li", {
-            style: s,
+            style: d,
             onClick: n,
             children: t.jsxs(z, {
                 href: i.url,
                 dataLabel: w(i.label),
                 style: {
                     textDecoration: "none"
                 },
                 children: [l == 0 && t.jsx(k, {
                     icon: i.icon || "dot-circle",
-                    style: o
+                    style: c
                 }), i.label]
             })
         }, Math.random()) : i.items.length > 0 && t.jsxs("li", {
             onClick: n,
-            style: s,
+            style: d,
             "data-label": w(i.label),
             children: [l == 0 && t.jsx(k, {
                 icon: i.icon || "dot-circle",
-                style: o
+                style: c
             }), i.label, t.jsx(k, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
@@ -3274,146 +3285,197 @@
             style: i,
             children: window.application.menu.items.map(function(l) {
                 return a(l, 0)
             })
         })
     }
 
-    function d() {
+    function o() {
         const i = {
             padding: 25,
             height: "100%",
             borderRight: "solid 1px #EEE"
         };
         return t.jsxs("div", {
             style: i,
             children: [e(), r()]
         })
     }
-    return d()
+    return o()
 }
 
 function kt(e) {
     var n;
 
     function a(i) {
         const l = "=".repeat((4 - i.length % 4) % 4),
-            s = (i + l).replace(/\-/g, "+").replace(/_/g, "/"),
-            o = window.atob(s),
-            u = new Uint8Array(o.length);
-        for (let c = 0; c < o.length; ++c) u[c] = o.charCodeAt(c);
+            d = (i + l).replace(/\-/g, "+").replace(/_/g, "/"),
+            c = window.atob(d),
+            u = new Uint8Array(c.length);
+        for (let s = 0; s < c.length; ++s) u[s] = c.charCodeAt(s);
         return u
     }
 
     function r() {
         "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(i) {
             if (i) {
                 const l = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
                 i.pushManager.subscribe({
                     userVisibleOnly: !0,
                     applicationServerKey: l
-                }).then(function(s) {
-                    if (console.log(s), n = JSON.stringify(s), console.log(n), s) {
+                }).then(function(d) {
+                    if (console.log(d), n = JSON.stringify(d), console.log(n), d) {
                         alert("Notificação ativada com sucesso.");
-                        var o = new FormData;
-                        o.append("subscription", n), D("POST", "/api/pushsubscribe/", function(u) {
+                        var c = new FormData;
+                        c.append("subscription", n), D("POST", "/api/pushsubscribe/", function(u) {
                             console.log(u)
-                        }, o)
+                        }, c)
                     } else {
                         alert("Problema ao ativar notificações.");
                         return
                     }
-                }).catch(function(s) {
-                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", s)
+                }).catch(function(d) {
+                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", d)
                 })
             } else console.log("No registered service worker.")
         }).catch(function(i) {
             alert("Erro"), console.error("Service Worker Error", i)
         }) : alert("Push messaging is not supported")
     }
 
-    function d() {
+    function o() {
         return t.jsx(k, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer"
             }
         })
     }
-    return d()
+    return o()
 }
 
 function St(e) {
+    function n() {
+        if (window.innerWidth > 800) return;
+        const a = {
+                position: "fixed",
+                display: "flex",
+                width: 50,
+                height: 50,
+                backgroundColor: "#1151b3",
+                color: "white",
+                right: 10,
+                borderRadius: "50%",
+                cursor: "pointer"
+            },
+            r = {
+                paddingLeft: 14,
+                paddingTop: 12,
+                fontSize: "1.8rem"
+            };
+        return t.jsxs(t.Fragment, {
+            children: [t.jsx("div", {
+                style: {
+                    ...a,
+                    bottom: 80
+                },
+                onClick: () => history.back(),
+                children: t.jsx(k, {
+                    icon: "arrow-left",
+                    style: r
+                })
+            }), t.jsx("div", {
+                style: {
+                    ...a,
+                    bottom: 20
+                },
+                onClick: () => window.scrollTo(0, 0),
+                children: t.jsx(k, {
+                    icon: "arrow-up",
+                    style: r
+                })
+            })]
+        })
+    }
+    return n()
+}
+
+function Ct(e) {
     const [n, a] = M.useState(e.data);
-    window.loaddata = d => a(d);
+    window.loaddata = o => a(o);
 
     function r() {
-        const d = {
+        const o = {
             minHeight: 400,
             margin: 20
         };
         return t.jsx("div", {
-            style: d,
+            style: o,
             id: "container",
             children: t.jsx(x, {
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
-function Ct(e) {
+function Mt(e) {
     M.useEffect(() => {
-        const o = localStorage.getItem("message");
-        o && (localStorage.removeItem("message"), K(o)), window.addEventListener("resize", () => {
-            const u = document.querySelector("aside");
-            u.style.display = window.innerWidth < 800 ? "none" : "block"
+        const u = localStorage.getItem("message");
+        u && (localStorage.removeItem("message"), K(u)), window.addEventListener("resize", () => {
+            const s = document.querySelector("aside");
+            s.style.display = window.innerWidth < 800 ? "none" : "block"
         })
     }, []);
 
     function a() {
-        const o = document.querySelector("aside");
-        o.style.display = o.style.display == "none" ? "block" : "none"
+        const u = document.querySelector("aside");
+        u.style.display = u.style.display == "none" ? "block" : "none"
     }
 
-    function r() {
-        const o = {
+    function r(u) {
+        u.preventDefault(), window.load(u.target.href)
+    }
+
+    function o() {
+        const u = {
                 display: "flex",
                 width: "100%",
                 justifyContent: "space-between",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 overflowX: "hidden"
             },
-            u = {
+            s = {
                 choices: "/api/search/",
                 help_text: null,
                 label: null,
                 mask: null,
                 name: "search",
                 required: !1,
                 type: "choice"
             };
         return e.data.navbar ? t.jsxs("div", {
-            style: o,
+            style: u,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
                 children: [t.jsx(k, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
                 }), t.jsxs("a", {
-                    href: "/",
+                    href: "/app/dashboard/",
+                    onClick: r,
                     style: {
                         fontSize: "1.5rem",
                         textDecoration: "none"
                     },
                     children: [e.data.navbar.logo && t.jsx("img", {
                         src: e.data.navbar.logo,
                         height: 20
@@ -3462,19 +3524,19 @@
                         position: {},
                         dataLabel: "gear",
                         children: t.jsx(k, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && t.jsx(ke, {
-                    data: u,
+                    data: s,
                     style: {
                         padding: 10
                     },
-                    onSelect: c => document.location.href = F(c.id)
+                    onSelect: m => document.location.href = F(m.id)
                 }), e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.usermenu,
                         position: {},
@@ -3482,80 +3544,80 @@
                         children: e.data.navbar.user
                     })
                 })]
             })]
         }) : null
     }
 
-    function d() {
+    function i() {
         return window.application.menu && t.jsx("aside", {
             style: {
                 flexGrow: 2,
                 maxWidth: "350px",
                 minWidth: "350px",
                 display: window.innerWidth < 800 ? "none" : "block"
             },
             children: t.jsx(jt, {})
         })
     }
 
-    function i() {
+    function l() {
         return t.jsxs("main", {
             style: {
                 flexGrow: 6,
                 minWidth: "400px"
             },
-            children: [t.jsx(St, {
+            children: [t.jsx(Ct, {
                 data: e.data.content
             }), t.jsx("footer", {
-                children: l()
-            })]
+                children: d()
+            }), t.jsx(St, {})]
         })
     }
 
-    function l() {
+    function d() {
         return e.data.footer ? t.jsxs("div", {
             align: "center",
             children: [t.jsx("div", {
                 children: "Todos os direitos reservados"
             }), t.jsx("div", {
                 children: e.data.footer.version
             })]
         }) : null
     }
 
-    function s() {
+    function c() {
         return t.jsxs("div", {
             children: [t.jsx("header", {
-                children: r()
+                children: o()
             }), t.jsxs("div", {
                 style: {
                     overflowX: "hide",
                     width: "100%",
                     display: "flex",
                     overflow: "hidden",
                     minHeight: window.innerHeight - 70
                 },
-                children: [d(), i()]
+                children: [i(), l()]
             })]
         })
     }
-    return s()
+    return c()
 }
 
-function Mt(e) {
+function Tt(e) {
     return t.jsx("img", {
         src: e.data.src,
         style: {
             width: "100%"
         }
     })
 }
 
-function Tt(e) {
+function Et(e) {
     const n = {
         width: "100%",
         textAlign: "center"
     };
     return t.jsx("div", {
         style: n,
         children: t.jsx("img", {
@@ -3565,28 +3627,28 @@
                 height: e.data.height,
                 borderRadius: e.data.round ? "50%" : 0
             }
         })
     })
 }
 
-function Et(e) {
+function Dt(e) {
     return t.jsx("iframe", {
         width: e.data.width || "100%",
         height: e.data.height || "400px",
         id: "gmap_canvas",
         src: "https://maps.google.com/maps?q=" + e.data.latitude + "," + e.data.longitude + "&t=&z=13&ie=UTF8&iwloc=&output=embed",
         frameBorder: "0",
         scrolling: "no",
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
-function Dt(e) {
+function It(e) {
     function n(i) {
         return e.data.icon ? i.done ? t.jsx(k, {
             style: {
                 marginTop: 12
             },
             icon: e.data.icon
         }) : t.jsx("span", {
@@ -3597,18 +3659,18 @@
             },
             children: i.number
         })
     }
 
     function a(i) {
         return {
-            border: "2px solid " + (i.done ? "#1351b4" : "#EEE"),
+            border: "3px solid " + (i.done ? "#1351b4" : "#1151b3"),
             borderRadius: "50%",
             background: i.done ? "#1351b4" : "white",
-            color: i.done ? "white" : "black",
+            color: i.done ? "white" : "#1151b3",
             textAlign: "center",
             width: 50,
             height: 50,
             margin: "auto",
             fontSize: "1.5rem"
         }
     }
@@ -3618,94 +3680,94 @@
             listStyleType: "none",
             display: "flex",
             justifyContent: "center",
             minWidth: i.length * 100
         }
     }
 
-    function d() {
+    function o() {
         const i = {
                 width: "100%",
                 margin: "auto",
                 overflowX: "auto",
                 "&::WebkitScrollbar": {
                     width: 0
                 }
             },
             l = {
                 width: 100,
                 marginWidth: 100,
                 textAlign: "center"
             },
-            s = {
+            d = {
                 position: "relative",
-                borderBottom: "2px solid #EEE",
+                borderBottom: "2px solid #1151b3",
                 top: -28,
                 width: 45,
                 left: 77
             };
         return t.jsx("div", {
             children: t.jsx("div", {
                 style: i,
                 children: t.jsx("ul", {
                     style: r(e.data.steps),
-                    children: e.data.steps.map((o, u) => t.jsxs("li", {
+                    children: e.data.steps.map((c, u) => t.jsxs("li", {
                         style: l,
                         children: [t.jsx("div", {
-                            style: a(o),
-                            children: n(o)
+                            style: a(c),
+                            children: n(c)
                         }), u < e.data.steps.length - 1 && t.jsx("div", {
-                            style: s
+                            style: d
                         }), t.jsx("div", {
-                            children: o.name
+                            children: c.name
                         })]
                     }, Math.random()))
                 })
             })
         })
     }
-    return d()
+    return o()
 }
 
-function It(e) {
+function qt(e) {
     function n() {
         const a = {
                 display: "inline-block",
                 width: "100%",
                 backgroundColor: "#DDD",
                 borderRadius: 5,
                 marginTop: 5
             },
             r = {
                 marginLeft: 10
             },
-            d = {
+            o = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
                 backgroundColor: Se[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
-                style: d,
+                style: o,
                 children: t.jsxs("span", {
                     style: r,
                     children: [e.data.value, "%"]
                 })
             })
         })
     }
     return n()
 }
 
-function qt(e) {
+function At(e) {
     function n() {
         return e.data.color = Se[e.data.style], t.jsx(Ce, {
             data: e.data
         })
     }
     return n()
 }
@@ -3725,15 +3787,15 @@
             style: a,
             children: e.data.label
         })
     }
     return n()
 }
 
-function At(e) {
+function Lt(e) {
     function n() {
         const a = {
                 padding: 20,
                 marginLeft: -20,
                 marginRight: -20,
                 textAlign: "center"
             },
@@ -3744,15 +3806,15 @@
                 width: 250,
                 height: 250,
                 backgroundColor: "white",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
-            d = {
+            o = {
                 marginTop: 30,
                 fontSize: "3rem",
                 color: "#2670e8"
             },
             i = {
                 marginTop: 40,
                 fontWeight: "bold",
@@ -3769,15 +3831,15 @@
             }), t.jsx("div", {
                 children: e.data.items.map(l => t.jsxs(z, {
                     href: l.url,
                     style: r,
                     dataLabel: l.label,
                     children: [t.jsx("div", {
                         children: t.jsx(k, {
-                            style: d,
+                            style: o,
                             icon: l.icon
                         })
                     }), t.jsx("div", {
                         style: i,
                         children: l.label
                     })]
                 }, Math.random()))
@@ -3803,44 +3865,44 @@
                 children: a
             }, Math.random()))
         })
     }
     return n()
 }
 
-function Lt(e) {
+function Nt(e) {
     function n() {
         return e.data.url ? t.jsx(z, {
             href: e.data.url,
             imodal: !!e.data.modal,
             children: e.data.icon ? t.jsx(k, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
 }
 
-function Nt(e) {
+function Ot(e) {
     function n() {
         return t.jsx("iframe", {
             src: e.data.url,
             width: "100%",
             height: 500,
             style: {
                 border: 0
             }
         })
     }
     return n()
 }
 
-function Ot(e) {
+function Rt(e) {
     const n = Math.random();
     M.useEffect(() => {
         new QRCode(document.getElementById(n), {
             text: e.data.text,
             width: 128,
             height: 128,
             colorDark: "#333333",
@@ -3853,29 +3915,29 @@
         return t.jsx("div", {
             id: n
         })
     }
     return a()
 }
 
-function Rt(e) {
+function _t(e) {
     function n() {
         return t.jsx(J, {
             width: 400,
             children: e.data.items.map((a, r) => t.jsx("div", {
                 children: t.jsx(x, {
                     data: a
                 })
             }, Math.random()))
         })
     }
     return n()
 }
 
-function _t(e) {
+function Ft(e) {
     function n() {
         return t.jsxs("div", {
             children: [t.jsx("h2", {
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     fontSize: "12rem",
@@ -3885,30 +3947,30 @@
                 children: e.data.value
             })]
         })
     }
     return n()
 }
 var re, Me = {};
-const Ft = "/api/application/",
+const zt = "/api/application/",
     me = localStorage.getItem("application");
 
 function x(e) {
     const n = Me[e.data.type];
     return n ? n(e.data) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
 x.register = function(e, n) {
     Me[e] = n
 };
 x.render = function(e) {
     re = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/login/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-x.register("counter", e => t.jsx(_t, {
+x.register("counter", e => t.jsx(Ft, {
     data: e
 }));
 x.register("form", e => t.jsx(dt, {
     data: e
 }));
 x.register("queryset", e => t.jsx(st, {
     data: e
@@ -3927,90 +3989,90 @@
 }));
 x.register("group", e => t.jsx(Je, {
     data: e
 }));
 x.register("statistics", e => t.jsx(bt, {
     data: e
 }));
-x.register("image", e => t.jsx(Tt, {
+x.register("image", e => t.jsx(Et, {
     data: e
 }));
-x.register("banner", e => t.jsx(Mt, {
+x.register("banner", e => t.jsx(Tt, {
     data: e
 }));
-x.register("map", e => t.jsx(Et, {
+x.register("map", e => t.jsx(Dt, {
     data: e
 }));
-x.register("steps", e => t.jsx(Dt, {
+x.register("steps", e => t.jsx(It, {
     data: e
 }));
-x.register("qrcode", e => t.jsx(Ot, {
+x.register("qrcode", e => t.jsx(Rt, {
     data: e
 }));
 x.register("badge", e => t.jsx(Ce, {
     data: e
 }));
-x.register("status", e => t.jsx(qt, {
+x.register("status", e => t.jsx(At, {
     data: e
 }));
-x.register("progress", e => t.jsx(It, {
+x.register("progress", e => t.jsx(qt, {
     data: e
 }));
 x.register("color", e => t.jsx(wt, {
     data: e
 }));
-x.register("boxes", e => t.jsx(At, {
+x.register("boxes", e => t.jsx(Lt, {
     data: e
 }));
 x.register("shell", e => t.jsx(Bt, {
     data: e
 }));
-x.register("file_link", e => t.jsx(Lt, {
+x.register("file_link", e => t.jsx(Nt, {
     data: e
 }));
-x.register("file_viewer", e => t.jsx(Nt, {
+x.register("file_viewer", e => t.jsx(Ot, {
     data: e
 }));
-x.register("response", e => t.jsx(Be, {
+x.register("response", e => t.jsx(Le, {
     data: e
 }));
-x.register("application", e => t.jsx(Ct, {
+x.register("application", e => t.jsx(Mt, {
     data: e
 }));
 x.register("iconset", e => t.jsx(De, {
     data: e
 }));
-x.register("grid", e => t.jsx(Rt, {
+x.register("grid", e => t.jsx(_t, {
     data: e
 }));
 x.register("rows", e => t.jsx(Fe, {
     data: e
 }));
 x.register("timeline", e => t.jsx(ze, {
     data: e
 }));
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), me ? (window.application = JSON.parse(me), D("GET", L(e), function(n) {
+    }, "", e), me ? (window.application = JSON.parse(me), D("GET", B(e), function(n) {
         window.application.content = n, re.render(t.jsx(x, {
             data: window.application
         }, Math.random()))
-    })) : D("GET", Ft, function(a) {
-        window.application = a, localStorage.setItem("application", JSON.stringify(window.application)), D("GET", L(e), function(r) {
+    })) : D("GET", zt, function(a) {
+        window.application = a, localStorage.setItem("application", JSON.stringify(window.application)), D("GET", B(e), function(r) {
             window.application.content = r, re.render(t.jsx(x, {
                 data: window.application
             }, Math.random()))
         })
     })
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
-    }, "", e), D("GET", L(e), function(n) {
+    }, "", e), D("GET", B(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
 x.render(H.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.2.0/slth/static/js/peerjs.min.js` & `pyslth-0.2.1/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/js/qrcode.min.js` & `pyslth-0.2.1/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/js/react-trigger-change.js` & `pyslth-0.2.1/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/js/react.min.js` & `pyslth-0.2.1/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/js/vanilla-masker.js` & `pyslth-0.2.1/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/static/js/vanilla-masker.min.js` & `pyslth-0.2.1/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/statistics.py` & `pyslth-0.2.1/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/templates/index.html` & `pyslth-0.2.1/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/templates/service-worker.js` & `pyslth-0.2.1/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/tests.py` & `pyslth-0.2.1/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/urls.py` & `pyslth-0.2.1/slth/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import slth
 from django.apps import apps
 from django.conf import settings
 from django.urls import path, re_path
-from django.conf.urls.static import static
 from . import views
 
 urlpatterns = [
     # re_path(r'^(?P<path>.*)/$', views.dispatcher),
-] + static('media', document_root=settings.MEDIA_ROOT)
+]
 
 for app_label in settings.INSTALLED_APPS:
     try:
         app = apps.get_app_config(app_label.split('.')[-1])
         fromlist = app.module.__package__.split('.')
         if app_label != 'slth':
             __import__('{}.{}'.format(app_label, 'endpoints'), fromlist=fromlist)
```

### Comparing `pyslth-0.2.0/slth/utils.py` & `pyslth-0.2.1/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.0/slth/views.py` & `pyslth-0.2.1/slth/views.py`

 * *Files identical despite different names*

