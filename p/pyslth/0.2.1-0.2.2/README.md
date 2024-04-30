# Comparing `tmp/pyslth-0.2.1.tar.gz` & `tmp/pyslth-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.2.1.tar", last modified: Mon Apr 29 14:24:42 2024, max compression
+gzip compressed data, was "pyslth-0.2.2.tar", last modified: Tue Apr 30 09:07:39 2024, max compression
```

## Comparing `pyslth-0.2.1.tar` & `pyslth-0.2.2.tar`

### file list

```diff
@@ -1,79 +1,84 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.971407 pyslth-0.2.1/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.1/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-29 14:24:42.971204 pyslth-0.2.1/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.941921 pyslth-0.2.1/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1752 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-29 14:24:42.000000 pyslth-0.2.1/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.1/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-29 14:24:42.971465 pyslth-0.2.1/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-29 14:24:23.000000 pyslth-0.2.1/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.948090 pyslth-0.2.1/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.1/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.2.1/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.948700 pyslth-0.2.1/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.1/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.1/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20281 2024-04-28 00:16:11.000000 pyslth-0.2.1/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.2.1/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25161 2024-04-29 14:14:17.000000 pyslth-0.2.1/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.949010 pyslth-0.2.1/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.949631 pyslth-0.2.1/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.1/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.1/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.952127 pyslth-0.2.1/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.1/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.2.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.2.1/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.2.1/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.1/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.2.1/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.1/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19803 2024-04-29 09:46:27.000000 pyslth-0.2.1/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.1/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.952608 pyslth-0.2.1/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.1/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11326 2024-04-28 13:32:26.000000 pyslth-0.2.1/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.2.1/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.952942 pyslth-0.2.1/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.954184 pyslth-0.2.1/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.956449 pyslth-0.2.1/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.2.1/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.1/slth/static/css/solid.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.958305 pyslth-0.2.1/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.1/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.1/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.1/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.1/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.970408 pyslth-0.2.1/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-29 14:24:31.000000 pyslth-0.2.1/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)    82788 2024-04-29 14:24:31.000000 pyslth-0.2.1/slth/static/js/lib.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-29 14:24:31.000000 pyslth-0.2.1/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/slth.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.1/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-29 14:24:42.970916 pyslth-0.2.1/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     2244 2024-04-28 00:37:31.000000 pyslth-0.2.1/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.1/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.1/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.1/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.1/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.2.1/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:39.016110 pyslth-0.2.2/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.2/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-30 09:07:39.015441 pyslth-0.2.2/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.937783 pyslth-0.2.2/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-30 09:07:38.000000 pyslth-0.2.2/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1928 2024-04-30 09:07:38.000000 pyslth-0.2.2/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-30 09:07:38.000000 pyslth-0.2.2/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-30 09:07:38.000000 pyslth-0.2.2/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-30 09:07:38.000000 pyslth-0.2.2/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.2/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-30 09:07:39.016572 pyslth-0.2.2/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-30 09:07:05.000000 pyslth-0.2.2/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.953560 pyslth-0.2.2/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.2/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.2.2/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.954230 pyslth-0.2.2/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.2/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.2/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20285 2024-04-29 21:30:56.000000 pyslth-0.2.2/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.2/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.2.2/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25161 2024-04-29 14:14:17.000000 pyslth-0.2.2/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.954579 pyslth-0.2.2/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.2/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.955816 pyslth-0.2.2/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.2/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.2/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.2/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.964028 pyslth-0.2.2/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.2.2/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.2/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.2.2/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.2.2/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.2.2/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.2/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.2/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.2.2/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.2/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.2/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19803 2024-04-29 09:46:27.000000 pyslth-0.2.2/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.2/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.968567 pyslth-0.2.2/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.2/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.2/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.2.2/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.969921 pyslth-0.2.2/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.973999 pyslth-0.2.2/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.2/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:38.996634 pyslth-0.2.2/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.2/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.2/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.2/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.2/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)      687 2024-04-29 21:33:32.000000 pyslth-0.2.2/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.2/slth/static/css/solid.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:39.000223 pyslth-0.2.2/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.2/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.2/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.2/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.2/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:39.014442 pyslth-0.2.2/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-30 09:07:02.000000 pyslth-0.2.2/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    83507 2024-04-30 09:07:02.000000 pyslth-0.2.2/slth/static/js/lib.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-30 09:07:02.000000 pyslth-0.2.2/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/js/slth.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.2/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-30 09:07:39.015078 pyslth-0.2.2/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     2281 2024-04-29 14:53:42.000000 pyslth-0.2.2/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.2/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.2/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.2/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.2/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.2.2/slth/views.py
```

### Comparing `pyslth-0.2.1/PKG-INFO` & `pyslth-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.1
+Version: 0.2.2
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.1/pyslth.egg-info/PKG-INFO` & `pyslth-0.2.2/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.1
+Version: 0.2.2
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.1/pyslth.egg-info/SOURCES.txt` & `pyslth-0.2.2/pyslth.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -35,21 +35,26 @@
 slth/migrations/0004_alter_profile_photo.py
 slth/migrations/0005_alter_profile_photo.py
 slth/migrations/0006_user.py
 slth/migrations/__init__.py
 slth/selenium/__init__.py
 slth/selenium/browser.py
 slth/static/index.html
+slth/static/css/.DS_Store
 slth/static/css/fontawesome.min.css
 slth/static/css/slth.css
 slth/static/css/solid.min.css
+slth/static/css/fonts/.DS_Store
 slth/static/css/fonts/Eina02-Bold.f8011405.ttf
 slth/static/css/fonts/Eina02-Regular.2e682693.ttf
 slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
 slth/static/css/fonts/fa-solid-900.woff2
+slth/static/css/fonts/rawline-400.woff
+slth/static/css/fonts/rawline-500i.woff
+slth/static/css/fonts/rawline-700.woff
 slth/static/images/logo.png
 slth/static/images/logo.svg
 slth/static/images/user.png
 slth/static/js/echarts.min.js
 slth/static/js/index.min.js
 slth/static/js/lib.min.js
 slth/static/js/peerjs.min.js
```

### Comparing `pyslth-0.2.1/setup.py` & `pyslth-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.2.1/slth/__init__.py` & `pyslth-0.2.2/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/components.py` & `pyslth-0.2.2/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/db/models.py` & `pyslth-0.2.2/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/endpoints.py` & `pyslth-0.2.2/slth/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
     def get(self):
         return IconSet()
 
 
 class Search(Endpoint):
     def get(self):
         key = '_options_'
-        options = self.cache.get(key)
+        options = self.cache.get(key, [])
         term = self.request.GET.get('term')
         if options is None and APPLICATON['dashboard']['search']:
             options = []
             for endpoint in APPLICATON['dashboard']['search']:
                 cls = ENDPOINTS[endpoint]
                 url = build_url(self.request, cls.get_api_url())
                 verbose_name = cls.get_metadata('verbose_name')
```

### Comparing `pyslth-0.2.1/slth/factory.py` & `pyslth-0.2.2/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/forms.py` & `pyslth-0.2.2/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/management/commands/integration_test.py` & `pyslth-0.2.2/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/management/commands/sync.py` & `pyslth-0.2.2/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/migrations/0001_initial.py` & `pyslth-0.2.2/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.2.2/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.2.2/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/migrations/0006_user.py` & `pyslth-0.2.2/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/models.py` & `pyslth-0.2.2/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/permissions.py` & `pyslth-0.2.2/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/queryset.py` & `pyslth-0.2.2/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/roles.py` & `pyslth-0.2.2/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/selenium/__init__.py` & `pyslth-0.2.2/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/selenium/browser.py` & `pyslth-0.2.2/slth/selenium/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
         time.sleep(seconds)
 
     def watch(self, e):
         self.save_screenshot("/tmp/test.png")
         if self.headless:
             raise e
         else:
+            breakpoint()
             raise e
 
     def print(self, message):
         if self.verbose:
             print(message)
 
     def debug(self, message):
@@ -204,16 +205,16 @@
             widgets = self.find_elements(By.CSS_SELECTOR, f'[data-label="{to_label_case(name)}"]')
             if widgets:
                 if widgets[0].tag_name.lower() == "select":
                     select = Select(widgets[0])
                     select.select_by_visible_text(value)
                 elif widgets[0].tag_name.lower() == "input":
                     widgets[0].send_keys(value)
-                    for i in range(0, 6):
-                        # print('Trying ({}) click at "{}"...'.format(i, value))
+                    for i in range(0, 10):
+                        print('Trying ({}) click at "{}"...'.format(i, value))
                         self.wait(0.5)
                         try:
                             super().find_element(By.CSS_SELECTOR, f'.autocomplete-item[data-label*="{to_label_case(value)}"]').click()
                             self.wait(0.5)
                             break
                         except WebDriverException:
                             pass
```

### Comparing `pyslth-0.2.1/slth/serializer.py` & `pyslth-0.2.2/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/css/fontawesome.min.css` & `pyslth-0.2.2/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/css/fonts/Eina02-Bold.f8011405.ttf` & `pyslth-0.2.2/slth/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/css/fonts/Eina02-Regular.2e682693.ttf` & `pyslth-0.2.2/slth/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `pyslth-0.2.2/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.2.2/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/css/solid.min.css` & `pyslth-0.2.2/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/images/logo.png` & `pyslth-0.2.2/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/images/logo.svg` & `pyslth-0.2.2/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/images/user.png` & `pyslth-0.2.2/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/js/echarts.min.js` & `pyslth-0.2.2/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/js/index.min.js` & `pyslth-0.2.2/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/js/lib.min.js` & `pyslth-0.2.2/slth/static/js/lib.min.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 import {
     j as t,
-    c as H,
-    r as M
+    c as W,
+    r as C
 } from "./react.min.js";
 
 function De(e) {
     function n(r) {
-        navigator.clipboard.writeText(r), K('Icon "' + r + '" copied to clipboard!')
+        navigator.clipboard.writeText(r), Z('Icon "' + r + '" copied to clipboard!')
     }
     const a = {
         display: "inline-block",
         width: 150,
         textAlign: "center",
         cursor: "pointer"
     };
@@ -38,24 +38,24 @@
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function k(e) {
+function b(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
 
-function se(e) {
+function ce(e) {
     function n() {
         const a = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
@@ -64,64 +64,64 @@
         };
         return e.primary && (a.backgroundColor = "#1351b4", a.color = "white"), e.default && (a.color = "#1351b4", a.border = "solid 1px #1351b4"), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(k, {
+            children: t.jsx(b, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
 const qe = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
-function Ae(e) {
+function Be(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
-            backgroundColor: e.isError ? "#e52207" : "black",
+            backgroundColor: e.isError ? "#e52207" : "#1151b3",
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
-            padding: 10
+            padding: 15
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(k, {
+            children: [t.jsx(b, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
     return n()
 }
 
-function K(e, n = !1) {
+function Z(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(Ae, {
+    a.classList.add("message"), W.createRoot(document.body.appendChild(a)).render(t.jsx(Be, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
-function fe() {
+function ge() {
     document.querySelectorAll(".message").forEach(function(e) {
         e.remove()
     })
 }
 
-function ie(e) {
+function le(e) {
     function n() {
         const a = {
             color: "#155bcb",
             backgroundColor: "#d4e5ff",
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
@@ -136,117 +136,117 @@
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function Le(e) {
-    return ge(e.data)
+function Ae(e) {
+    return xe(e.data)
 }
 
-function B(e) {
+function L(e) {
     return e.replace("/app/", "/api/")
 }
 
-function F(e) {
+function H(e) {
     return e.replace("/api/", "/app/")
 }
 
-function D(e, n, a, r) {
-    const o = localStorage.getItem("token");
+function E(e, n, a, r) {
+    const d = localStorage.getItem("token");
     var i = {
         Accept: "application/json"
     };
-    o && (i.Authorization = "Token " + o);
-    const l = B(n);
-    var d = {
+    d && (i.Authorization = "Token " + d);
+    const o = L(n);
+    var s = {
         method: e,
         headers: new Headers(i),
         ajax: 1
     };
-    r && (d.body = r);
+    r && (s.body = r);
     var c = null,
         u = null;
-    fetch(l, d).then(function(s) {
-        if (c = s, u = c.headers.get("Content-Type"), u == "application/json") return s.text();
-        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return s.arrayBuffer();
-        s.text()
-    }).then(s => {
+    fetch(o, s).then(function(l) {
+        if (c = l, u = c.headers.get("Content-Type"), u == "application/json") return l.text();
+        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return l.arrayBuffer();
+        l.text()
+    }).then(l => {
         if (u == "application/json") {
-            var m = JSON.parse(s || "{}");
-            typeof m == "object" && m.type == "redirect" ? document.location.href = F(m.url) : a && a(m, c)
+            var m = JSON.parse(l || "{}");
+            typeof m == "object" && m.type == "redirect" ? document.location.href = H(m.url) : a && a(m, c)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var y = window.URL.createObjectURL(new Blob([new Uint8Array(s)], {
+            var x = window.URL.createObjectURL(new Blob([new Uint8Array(l)], {
                     type: u
                 })),
                 v = document.createElement("a");
-            v.href = y, u.indexOf("excel") >= 0 ? v.download = "Download.xls" : u.indexOf("pdf") >= 0 ? v.download = "Download.pdf" : u.indexOf("zip") >= 0 ? v.download = "Download.zip" : u.indexOf("json") >= 0 ? v.download = "Download.json" : u.indexOf("csv") >= 0 ? v.download = "Download.csv" : u.indexOf("png") >= 0 && (v.download = "Download.png"), document.body.appendChild(v), v.click(), a && a({}, c)
-        } else a && a(s, c)
+            v.href = x, u.indexOf("excel") >= 0 ? v.download = "Download.xls" : u.indexOf("pdf") >= 0 ? v.download = "Download.pdf" : u.indexOf("zip") >= 0 ? v.download = "Download.zip" : u.indexOf("json") >= 0 ? v.download = "Download.json" : u.indexOf("csv") >= 0 ? v.download = "Download.csv" : u.indexOf("png") >= 0 && (v.download = "Download.png"), document.body.appendChild(v), v.click(), a && a({}, c)
+        } else a && a(l, c)
     })
 }
 
-function ge(e) {
+function xe(e) {
     e.store && Object.keys(e.store).map(function(n) {
         e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
-    }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = F(e.redirect)) : e.message && K(e.message)
+    }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = H(e.redirect)) : e.message && Z(e.message)
 }
 
 function U(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
     if (typeof e == "number") {
         var n = e.toString().split(".");
         return n.length == 1 ? e.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".") : (n[0] = n[0].toString().replace(/\B(?=(\d{3})+(?!\d))/g, "."), n[1] = n[1].substring(0, 2), n[1].length == 1 && (n[1] = n[1] + "0"), n[0] + "," + n[1])
     }
     if (typeof e == "string") {
-        if (e.length == 7 && e[0] == "#") return t.jsx(x, {
+        if (e.length == 7 && e[0] == "#") return t.jsx(y, {
             data: {
                 type: "color",
                 value: e
             }
         });
         if (e.length == 19 && e[13] == ":" && e[16] == ":") {
             var n = e.split(" "),
                 a = n[0],
                 r = n[1];
             return r == "00:00:00" ? a : a + " " + r
         }
         return e
     }
-    return typeof e == "object" && e.type ? t.jsx(x, {
+    return typeof e == "object" && e.type ? t.jsx(y, {
         data: e
     }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : t.jsx("ul", {
         style: {
             padding: 0
         },
-        children: e.map(function(o) {
+        children: e.map(function(d) {
             return t.jsx("li", {
-                children: o
+                children: d
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
-function xe() {
-    document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ne, {}))
+function ye() {
+    document.querySelector(".layer") == null && W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ne, {}))
 }
 
-function ye(e, n) {
-    fe(), xe(), window.reloader = n;
+function pe(e, n) {
+    ge(), ye(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {
-        url: B(e)
+    W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {
+        url: L(e)
     }))
 }
 
-function Be(e) {
-    fe(), xe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Re, {
-        url: B(e)
+function Le(e) {
+    ge(), ye(), W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Re, {
+        url: L(e)
     }))
 }
 
 function V(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
@@ -272,85 +272,85 @@
             V()
         },
         style: n
     })
 }
 
 function Oe(e) {
-    const [n, a] = M.useState(null), [r, o] = M.useState(0);
-    M.useEffect(() => {
-        i(B(e.url)), document.querySelector(".layer").style.display = "block"
+    const [n, a] = C.useState(null), [r, d] = C.useState(0);
+    C.useEffect(() => {
+        i(L(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
     function i(c) {
-        D("GET", B(c), function(u) {
-            a(u), o(r + 1)
+        E("GET", L(c), function(u) {
+            a(u), d(r + 1)
         })
     }
 
-    function l() {
+    function o() {
         const c = {
             textAlign: "right",
             cursor: "pointer"
         };
         if (n) return t.jsxs("div", {
             children: [t.jsx("div", {
                 style: c,
-                children: t.jsx(k, {
+                children: t.jsx(b, {
                     icon: "x",
                     onClick: () => V()
                 })
-            }), t.jsx(x, {
+            }), t.jsx(y, {
                 data: n
             })]
         })
     }
-    const d = {
+    const s = {
         minWidth: "50%",
         display: n ? "block" : "none",
         maxWidth: "90%",
         top: window.scrollY + 40
     };
     return t.jsx("dialog", {
-        style: d,
-        children: l()
+        style: s,
+        children: o()
     }, r)
 }
 
 function Re(e) {
     var n = Math.random();
-    M.useEffect(() => {
+    C.useEffect(() => {
         document.querySelector(".layer").style.display = "block";
         var r = document.getElementById(n);
         r.style.top = document.documentElement.scrollTop + 100
     }, []);
 
     function a() {
         const r = {
                 minWidth: "50%",
                 display: "block",
                 maxWidth: "90%",
                 top: window.scrollY + 40
             },
-            o = {
+            d = {
                 float: "right",
                 cursor: "pointer",
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
-                style: o,
-                children: t.jsx(k, {
+                style: d,
+                children: t.jsx(b, {
                     icon: "x",
                     onClick: () => V()
                 })
             }), t.jsx("iframe", {
-                src: B(e.url),
+                src: L(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
                 }
             })]
         })
@@ -358,85 +358,85 @@
     return a()
 }
 
 function w(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
-function N(e) {
+function O(e) {
     const n = e.id || Math.random(),
-        [a, r] = M.useState(e.data.name);
+        [a, r] = C.useState(e.data.name);
 
-    function o(d) {
-        d.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(d)) : e.data.modal == !1 ? window.load(F(e.data.url)) : ye(e.data.url)
+    function d(s) {
+        s.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(s)) : e.data.modal == !1 ? window.load(H(e.data.url)) : pe(e.data.url)
     }
 
     function i() {
-        return e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(k, {
+        return e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(b, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(k, {
+            children: [t.jsx(b, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
 
-    function l() {
-        var d = {
+    function o() {
+        var s = {
             padding: 12,
             textDecoration: "none",
             borderRadius: 5,
             margin: 5
         };
-        return e.primary && (d.backgroundColor = "#1351b4", d.color = "white"), e.default && (d.border = "solid 1px #1351b4", d.color = "#1351b4"), e.style && Object.keys(e.style).map(function(c) {
-            d[c] = e.style[c]
+        return e.primary && (s.backgroundColor = "#1351b4", s.color = "white"), e.default && (s.border = "solid 1px #1351b4", s.color = "#1351b4"), e.style && Object.keys(e.style).map(function(c) {
+            s[c] = e.style[c]
         }), t.jsx("a", {
             id: n,
-            href: F(e.data.url) || "#",
-            onClick: o,
-            style: d,
+            href: H(e.data.url) || "#",
+            onClick: d,
+            style: s,
             "data-label": w(e.data.name),
             children: i()
         })
     }
-    return l()
+    return o()
 }
 
-function X(e) {
+function Q(e) {
     function n(i) {
-        var l = i.target.parentNode.querySelector(".dropdown");
-        return l == null && (l = i.target.parentNode.parentNode.querySelector(".dropdown")), l == null && (l = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), l
+        var o = i.target.parentNode.querySelector(".dropdown");
+        return o == null && (o = i.target.parentNode.parentNode.querySelector(".dropdown")), o == null && (o = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), o
     }
 
     function a(i) {
-        const l = i.target.getBoundingClientRect(),
-            d = n(i);
-        document.querySelectorAll(".dropdown").forEach(c => c.style.display = "none"), d.style.left = l.left - 150 + l.width + "px", d.style.display = "block"
+        const o = i.target.getBoundingClientRect(),
+            s = n(i);
+        document.querySelectorAll(".dropdown").forEach(c => c.style.display = "none"), s.style.left = o.left - 150 + o.width + "px", s.style.display = "block"
     }
 
     function r(i) {
-        const l = n(i);
-        l.style.display = "none"
+        const o = n(i);
+        o.style.display = "none"
     }
 
-    function o() {
+    function d() {
         const i = {
                 padding: 0,
                 position: "absolute",
                 width: 150,
                 left: 0,
                 textAlign: "center",
                 backgroundColor: "white",
                 boxShadow: "15px 15px 10px -15px #DDD",
                 display: "none"
             },
-            l = {
+            o = {
                 listStyleType: "none",
                 padding: 10
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 onClick: a,
                 style: {
@@ -444,59 +444,59 @@
                 },
                 "data-label": w(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: i,
                 onMouseLeave: r,
                 className: "dropdown",
-                children: e.actions.map(d => t.jsx("li", {
-                    style: l,
-                    children: t.jsx(N, {
-                        data: d,
+                children: e.actions.map(s => t.jsx("li", {
+                    style: o,
+                    children: t.jsx(O, {
+                        data: s,
                         style: {
                             padding: 0
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
-    return o()
+    return d()
 }
 
-function z({
+function P({
     id: e,
     href: n,
     modal: a,
     imodal: r,
-    children: o,
+    children: d,
     onClick: i,
-    dataLabel: l,
-    style: d
+    dataLabel: o,
+    style: s
 }) {
-    const c = n && n.indexOf("/media/") < 0 ? F(n) : n;
+    const c = n && n.indexOf("/media/") < 0 ? H(n) : n;
 
     function u(m) {
-        m.preventDefault(), a ? ye(c) : r ? Be(c) : window.load(c)
+        m.preventDefault(), a ? pe(c) : r ? Le(c) : window.load(c)
     }
 
-    function s() {
+    function l() {
         return t.jsx("a", {
             id: e,
             onClick: i || u,
             href: c || "#",
-            "data-label": w(l),
-            style: d,
-            children: o
+            "data-label": w(o),
+            style: s,
+            children: d
         })
     }
-    return s()
+    return l()
 }
 
-function J(e) {
+function $(e) {
     function n() {
         const r = {
             display: "grid",
             gridGap: 0,
             gridTemplateColumns: "repeat(auto-fit, minmax(" + (e.width || 200) + "px, 1fr))",
             alignItems: e.alignItems || "end"
         };
@@ -504,26 +504,26 @@
             style: r,
             children: e.children
         })
     }
     return n()
 }
 
-function $(e) {
+function J(e) {
     function n() {
         return e.data.url ? t.jsx(_e, {
             data: e.data
-        }) : t.jsx(pe, {
+        }) : t.jsx(ve, {
             data: e.data
         })
     }
     return n()
 }
 
-function pe(e) {
+function ve(e) {
     function n() {
         const a = {
             minWidth: e.width + "%",
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsxs("div", {
@@ -534,68 +534,68 @@
         })
     }
     return n()
 }
 
 function _e(e) {
     const n = Math.random(),
-        [a, r] = M.useState(e.data);
+        [a, r] = C.useState(e.data);
 
-    function o(l) {
-        D("GET", l, function(d) {
-            r(d)
+    function d(o) {
+        E("GET", o, function(s) {
+            r(s)
         })
     }
 
     function i() {
-        return window[n] = () => o(e.data.url), t.jsx("div", {
+        return window[n] = () => d(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
-            children: t.jsx(pe, {
+            children: t.jsx(ve, {
                 data: a,
                 width: 100
             })
         })
     }
     return i()
 }
 
-function ve(e) {
+function be(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 verticalAlign: "center",
                 textAlign: "right",
                 lineHeight: "3rem"
             },
             children: e.data.map(function(a) {
-                return t.jsx(N, {
+                return t.jsx(O, {
                     data: a,
                     default: !0,
                     compact: !0
                 }, Math.random())
             })
         })
     }
     return n()
 }
 
-function be(e) {
+function we(e) {
     function n() {
         return e.data.map(function(a) {
-            if (Array.isArray(a)) return t.jsx(J, {
+            if (Array.isArray(a)) return t.jsx($, {
                 width: 300,
                 alignItems: "start",
-                children: a.map(r => t.jsx($, {
+                children: a.map(r => t.jsx(J, {
                     data: r,
                     width: 100 / a.length
                 }, Math.random()))
             }, Math.random());
             if (a.label != "ID" && a.label != e.exclude) return t.jsx("div", {
-                children: t.jsx($, {
+                children: t.jsx(J, {
                     data: a,
                     width: 100
                 })
             }, Math.random())
         })
     }
     return n()
@@ -610,198 +610,210 @@
         return t.jsx("h3", {
             style: i,
             children: e.data.title
         })
     }
 
     function a() {
-        return t.jsx(be, {
+        return t.jsx(we, {
             data: e.data.data
         })
     }
 
     function r() {
-        return t.jsx(ve, {
+        return t.jsx(be, {
             data: e.data.actions
         })
     }
 
-    function o() {
+    function d() {
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
-    return o()
+    return d()
 }
 
 function ze(e) {
     function n() {
-        const l = {
+        const o = {
             paddingTop: 15,
             marginBottom: 10,
             color: "#1151b3"
         };
         return t.jsx("div", {
-            style: l,
+            style: o,
             children: t.jsx("strong", {
                 children: e.data.title
             })
         })
     }
 
     function a() {
-        return t.jsx(be, {
+        return t.jsx(we, {
             data: e.data.data,
             exclude: e.data.data[1].label
         })
     }
 
     function r() {
-        const l = {
+        const o = {
                 position: "absolute",
                 width: 140,
                 marginLeft: -128,
                 display: "flex",
                 justifyContent: "space-between",
                 marginTop: 10,
                 alignItems: "flex-end"
             },
-            d = {
+            s = {
                 maxWidth: 100
             },
             c = {
                 width: 20,
                 height: 20,
                 border: "3px solid #1151b3",
                 backgroundColor: "white",
                 borderRadius: "50%"
             };
         return t.jsxs("div", {
-            style: l,
+            style: o,
             children: [t.jsx("div", {
-                style: d,
+                style: s,
                 children: e.data.data[1].value
             }), t.jsx("div", {
                 style: c
             })]
         })
     }
 
-    function o() {
-        return t.jsx(ve, {
+    function d() {
+        return t.jsx(be, {
             data: e.data.actions
         })
     }
 
     function i() {
-        const l = {
+        const o = {
                 borderBottom: "solid 1px #DDD",
                 padding: 0,
                 borderBottomStyle: "dashed",
                 marginLeft: 140,
                 borderLeft: "3px solid #1151b3",
                 marginBottom: -10
             },
-            d = {
+            s = {
                 marginLeft: 20
             };
         return t.jsxs("div", {
-            style: l,
+            style: o,
             children: [r(), t.jsxs("div", {
-                style: d,
-                children: [n(), a(), o()]
+                style: s,
+                children: [n(), a(), d()]
             })]
         })
     }
     return i()
 }
 
 function He(e) {
     const n = Math.random(),
-        [a, r] = M.useState(e.data);
+        [a, r] = C.useState(e.data);
 
-    function o() {
-        return t.jsx(we, {
+    function d() {
+        return t.jsx(je, {
             data: a
         })
     }
 
     function i() {
+        const u = {
+            backgroundColor: "white",
+            padding: 15,
+            marginBottom: 15
+        };
+        return t.jsx("div", {
+            style: u,
+            children: o()
+        })
+    }
+
+    function o() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
-        }) : a.data.map(function(c) {
-            return Array.isArray(c) ? t.jsx(J, {
+        }) : a.data.map(function(u) {
+            return Array.isArray(u) ? t.jsx($, {
                 width: 300,
-                children: c.map(u => t.jsx($, {
-                    data: u,
-                    width: 100 / c.length
+                children: u.map(l => t.jsx(J, {
+                    data: l,
+                    width: 100 / u.length
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
-                children: t.jsx($, {
-                    data: c,
+                children: t.jsx(J, {
+                    data: u,
                     width: 100
                 })
             }, Math.random())
-        }) : t.jsx(x, {
+        }) : t.jsx(y, {
             data: a.data
         })
     }
 
-    function l(c) {
-        D("GET", c, function(u) {
-            r(u)
+    function s(u) {
+        E("GET", u, function(l) {
+            r(l)
         })
     }
 
-    function d() {
-        return e.data.url ? (window[n] = () => l(e.data.url), t.jsxs("div", {
+    function c() {
+        return e.data.url ? (window[n] = () => s(e.data.url), t.jsxs("div", {
             className: e.data.url && "reloadable",
             id: n,
-            children: [o(), i()]
+            children: [d(), i()]
         })) : t.jsxs("div", {
-            children: [o(), i()]
+            children: [d(), i()]
         })
     }
-    return d()
+    return c()
 }
 
 function Pe(e) {
     const n = Math.random(),
-        [a, r] = M.useState(e.data.actions);
+        [a, r] = C.useState(e.data.actions);
 
-    function o() {
-        const d = e.data.url.indexOf("?") < 0 ? "?" : "&";
-        return e.data.url + d + "only=actions"
+    function d() {
+        const s = e.data.url.indexOf("?") < 0 ? "?" : "&";
+        return e.data.url + s + "only=actions"
     }
 
     function i() {
-        D("GET", o(), function(d) {
-            r(d)
+        E("GET", d(), function(s) {
+            r(s)
         })
     }
 
-    function l() {
+    function o() {
         return window[n] = () => i(), t.jsx("div", {
             className: "reloadable",
             id: n,
-            children: a.map(function(d) {
-                return t.jsx(N, {
-                    data: d,
+            children: a.map(function(s) {
+                return t.jsx(O, {
+                    data: s,
                     default: !0
                 }, Math.random())
             })
         })
     }
-    return l()
+    return o()
 }
 
 function We(e) {
     function n() {
         const a = {
                 display: "flex",
                 justifyContent: "space-between",
@@ -820,15 +832,15 @@
                 data: e.data
             })]
         })
     }
     return n()
 }
 
-function we(e) {
+function je(e) {
     function n() {
         const a = {
                 display: "flex",
                 justifyContent: "space-between",
                 alignItems: "baseline"
             },
             r = {
@@ -838,17 +850,17 @@
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h2", {
                 style: r,
                 "data-label": w(e.data.title),
                 children: e.data.title
             }), e.data.actions.length > 0 && t.jsx("div", {
-                children: e.data.actions.map(function(o) {
-                    return t.jsx(N, {
-                        data: o,
+                children: e.data.actions.map(function(d) {
+                    return t.jsx(O, {
+                        data: d,
                         default: !0
                     }, Math.random())
                 })
             })]
         })
     }
     return n()
@@ -858,44 +870,44 @@
     function n() {
         return t.jsx(We, {
             data: e.data
         })
     }
 
     function a() {
-        return e.data.data.map(function(o, i) {
-            return t.jsx(x, {
-                data: o
+        return e.data.data.map(function(d, i) {
+            return t.jsx(y, {
+                data: d
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
         })
     }
     return r()
 }
 
 function Ue(e) {
     function n() {
-        return t.jsx(we, {
+        return t.jsx(je, {
             data: e.data
         })
     }
 
     function a() {
-        const o = {
+        const d = {
             backgroundColor: "white"
         };
-        return e.data.data.map(function(i, l) {
+        return e.data.data.map(function(i, o) {
             return t.jsx("div", {
-                style: o,
-                children: t.jsx(x, {
+                style: d,
+                children: t.jsx(y, {
                     data: i
                 }, Math.random())
             })
         })
     }
 
     function r() {
@@ -903,187 +915,187 @@
             children: [n(), a()]
         })
     }
     return r()
 }
 
 function Ve(e) {
-    const [n, a] = M.useState(0);
+    const [n, a] = C.useState(0);
 
     function r() {
         return t.jsx("div", {
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20
             },
-            children: e.data.map(function(o, i) {
-                return t.jsx(z, {
-                    href: o.url,
+            children: e.data.map(function(d, i) {
+                return t.jsx(P, {
+                    href: d.url,
                     style: {
                         padding: 5,
                         fontWeight: n == i ? "bold" : "normal",
                         borderBottom: n == i ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
-                    onClick: function(l) {
-                        l.preventDefault(), a(i), e.loadContent(o.url)
+                    onClick: function(o) {
+                        o.preventDefault(), a(i), e.loadContent(d.url)
                     },
-                    dataLabel: w(o.title),
-                    children: o.title
+                    dataLabel: w(d.title),
+                    children: d.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
-function Je(e) {
+function $e(e) {
     var n = Math.random();
-    const [a, r] = M.useState(e.data.data[0]);
+    const [a, r] = C.useState(e.data.data[0]);
 
-    function o() {
+    function d() {
         return e.data.title != "Top" && t.jsx("h2", {
             "data-label": w(e.data.title),
             children: e.data.title
         })
     }
 
     function i() {
         return t.jsx(Ve, {
             data: e.data.data,
             loadContent: c
         })
     }
 
-    function l() {
-        var s = {
+    function o() {
+        var l = {
             ...a
         };
-        s.title = null;
+        l.title = null;
         const m = {
             padding: 0
         };
         return t.jsx("div", {
             style: m,
-            children: t.jsx(x, {
-                data: s
+            children: t.jsx(y, {
+                data: l
             }, Math.random())
         })
     }
 
-    function d() {
-        const s = {
+    function s() {
+        const l = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
-            style: s
+            style: l
         })
     }
 
-    function c(s) {
-        D("GET", s, function(m) {
+    function c(l) {
+        E("GET", l, function(m) {
             r(m)
         })
     }
 
     function u() {
         return window[n] = () => c(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [o(), i(), l(), d()]
+            children: [d(), i(), o(), s()]
         })
     }
     return u()
 }
 
-function $e() {
+function Je() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
 
-function A({
+function q({
     id: e,
     onClick: n,
     icon: a,
     label: r,
-    display: o,
+    display: d,
     primary: i,
-    compact: l,
-    spin: d
+    compact: o,
+    spin: s
 }) {
     function c() {
-        return a ? l || !r ? t.jsx(k, {
+        return a ? o || !r ? t.jsx(b, {
             icon: a
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(Ie, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(k, {
+            }), t.jsx(b, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
 
     function u() {
-        const s = {
+        const l = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
-            display: o || "block",
+            display: d || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return i ? (s.backgroundColor = "#1351b4", s.color = "white") : (s.border = "solid 1px #1351b4", s.color = "#1351b4"), t.jsx("a", {
+        return i ? (l.backgroundColor = "#1351b4", l.color = "white") : (l.border = "solid 1px #1351b4", l.color = "#1351b4"), t.jsx("a", {
             id: e,
-            style: s,
+            style: l,
             "data-label": w(r || a),
             onClick: m => {
-                m.preventDefault(), a && d && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
+                m.preventDefault(), a && s && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
             },
             children: c()
         })
     }
     return u()
 }
 const Ye = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
     Y = {
         padding: 15,
-        border: "solid 1px #CCC",
+        border: "solid 1px #d9d9d9",
         borderRadius: 5
     };
 
-function ne(e) {
+function ae(e) {
     if (e) {
         const a = [".png", ".jpeg", ".jpeg", ".gif"];
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
-function je(e, n) {
+function ke(e, n) {
     var a = new FormData(e);
-    D("POST", n, Ze, a)
+    E("POST", n, Ze, a)
 }
 
 function Xe(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
@@ -1107,17 +1119,17 @@
     else if (r.tagName == "SELECT") {
         if (r.style.display != "none") r.dispatchEvent(new CustomEvent("customchange", {
             detail: {
                 value: n
             }
         }));
         else
-            for (var o = 0; o < r.options.length; o++)
-                if (r.options[o].value == n) {
-                    r.selectedIndex = o;
+            for (var d = 0; d < r.options.length; d++)
+                if (r.options[d].value == n) {
+                    r.selectedIndex = d;
                     break
                 }
     }
 }
 
 function Ze(e) {
     if (e) {
@@ -1137,15 +1149,15 @@
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(k, {
+                children: [t.jsx(b, {
                     icon: "circle-check",
                     style: {
                         color: "#155bcb",
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
@@ -1165,15 +1177,15 @@
             marginTop: 2,
             marginBottom: 2,
             padding: 8
         };
         return t.jsxs("div", {
             style: a,
             id: e.id,
-            children: [t.jsx(k, {
+            children: [t.jsx(b, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
@@ -1193,436 +1205,439 @@
                 children: e.text
             })
         })
     }
     return n()
 }
 
-function Q(e) {
+function K(e) {
     const n = e.data.name + Math.random();
 
     function a() {
-        const d = {
+        const s = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
         return e.data.action && (e.data.action.modal = !0), t.jsxs("div", {
-            style: d,
+            style: s,
             children: [t.jsx("label", {
                 className: e.data.required ? "bold" : "",
                 children: e.data.label
-            }), e.data.action && t.jsx(N, {
+            }), e.data.action && t.jsx(O, {
                 data: e.data.action,
                 style: {
                     padding: 0
                 }
             })]
         })
     }
 
     function r() {
-        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Ye.indexOf(e.data.type) >= 0 ? t.jsx(ce, {
+        return e.data.type == "datetime" && (e.data.type = "datetime-local"), Ye.indexOf(e.data.type) >= 0 ? t.jsx(ue, {
             data: e.data
-        }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ue, {
+        }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(he, {
             data: e.data
-        }) : t.jsx(ae, {
+        }) : t.jsx(re, {
             data: e.data
         }) : t.jsx(it, {
             data: e.data
-        }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ue, {
+        }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(he, {
             data: e.data
-        }) : t.jsx(ae, {
+        }) : t.jsx(re, {
             data: e.data
-        }) : t.jsx(ke, {
+        }) : t.jsx(Se, {
             data: e.data
-        }) : e.data.type == "decimal" ? t.jsx(ce, {
+        }) : e.data.type == "decimal" ? t.jsx(ue, {
             data: e.data
         }) : e.data.type == "boolean" ? t.jsx(rt, {
             data: e.data
         }) : e.data.type == "textarea" ? t.jsx(at, {
             data: e.data
         }) : t.jsx("span", {
             children: e.data.name
         })
     }
 
-    function o() {
+    function d() {
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
 
-    function l() {
-        const d = {
+    function o() {
+        const s = {
             display: e.data.type == "hidden" ? "none" : "flex",
             flexDirection: "column",
             padding: 5
         };
         return t.jsxs("div", {
             id: n,
             className: "form-group " + e.data.name,
-            style: d,
-            children: [a(), r(), i(), o()]
+            style: s,
+            children: [a(), r(), i(), d()]
         })
     }
-    return l()
+    return o()
 }
 
-function ce(e) {
+function ue(e) {
     var n = "";
     const a = e.data.name + Math.random();
-    e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), M.useEffect(() => {
-        function l(u, s, m) {
-            var y = m.target,
-                v = y.value.replace(/\D/g, ""),
-                j = y.value.length > s ? 1 : 0;
-            VMasker(y).unMask(), VMasker(y).maskPattern(u[j]), y.value = VMasker.toPattern(v, u[j])
+    e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), C.useEffect(() => {
+        function o(u, l, m) {
+            var x = m.target,
+                v = x.value.replace(/\D/g, ""),
+                j = x.value.length > l ? 1 : 0;
+            VMasker(x).unMask(), VMasker(x).maskPattern(u[j]), x.value = VMasker.toPattern(v, u[j])
         }
         if (e.data.mask) {
-            var d = document.getElementById(a);
-            if (e.data.mask == "decimal") VMasker(d).maskMoney({
+            var s = document.getElementById(a);
+            if (e.data.mask == "decimal") VMasker(s).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
             });
             else if (e.data.mask.indexOf("|") > 0) {
                 var c = e.data.mask.split("|");
-                VMasker(d).maskPattern(c[0]), d.addEventListener("input", l.bind(void 0, c, 14), !1)
-            } else VMasker(d).maskPattern(e.data.mask)
+                VMasker(s).maskPattern(c[0]), s.addEventListener("input", o.bind(void 0, c, 14), !1)
+            } else VMasker(s).maskPattern(e.data.mask)
         }
     }, []);
 
-    function r(l) {
-        je(l.target.closest("form"), e.data.onchange)
+    function r(o) {
+        ke(o.target.closest("form"), e.data.onchange)
     }
 
-    function o(l) {
-        if (e.data.type == "file" && l.target.files) {
-            let c = l.target.files[0];
-            var d = new FileReader;
-            d.onload = function(u) {
-                if (ne(c.name)) {
+    function d(o) {
+        if (e.data.type == "file" && o.target.files) {
+            let c = o.target.files[0];
+            var s = new FileReader;
+            s.onload = function(u) {
+                if (ae(c.name)) {
                     const v = "display" + a;
-                    var s = document.createElement("img");
-                    s.id = l.target.id + "img", s.style.width = "200px", s.style.display = "block", s.style.margin = "auto", s.style.marginTop = "20px", s.onload = function(j) {
-                        const I = e.data.width > e.data.height ? e.data.width / s.width : e.data.height / s.height;
-                        var T = document.createElement("canvas");
-                        const q = T.getContext("2d");
-                        T.height = T.width * (s.height / s.width);
-                        const C = document.createElement("canvas"),
-                            P = C.getContext("2d");
-                        C.width = s.width * I, C.height = s.height * I, P.drawImage(s, 0, 0, C.width, C.height), q.drawImage(C, 0, 0, C.width * I, C.height * I, 0, 0, T.width, T.height), C.toBlob(function(h) {
-                            const g = new DataTransfer;
-                            g.items.add(new File([h], c.name)), l.target.files = g.files
+                    var l = document.createElement("img");
+                    l.id = o.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(j) {
+                        const D = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
+                        var M = document.createElement("canvas");
+                        const B = M.getContext("2d");
+                        M.height = M.width * (l.height / l.width);
+                        const S = document.createElement("canvas"),
+                            F = S.getContext("2d");
+                        S.width = l.width * D, S.height = l.height * D, F.drawImage(l, 0, 0, S.width, S.height), B.drawImage(S, 0, 0, S.width * D, S.height * D, 0, 0, M.width, M.height), S.toBlob(function(h) {
+                            const f = new DataTransfer;
+                            f.items.add(new File([h], c.name)), o.target.files = f.files
                         });
-                        var p = document.getElementById(v);
-                        p == null ? (p = document.createElement("div"), p.id = v) : p.removeChild(p.childNodes[0]), p.appendChild(s), l.target.parentNode.appendChild(p)
-                    }, s.src = u.target.result
+                        var I = document.getElementById(v);
+                        I == null ? (I = document.createElement("div"), I.id = v) : I.removeChild(I.childNodes[0]), I.appendChild(l), o.target.parentNode.appendChild(I)
+                    }, l.src = u.target.result
                 }
                 const m = document.getElementById("fileinfo" + a);
-                var y = c.size / 1024;
-                y < 1024 ? y = parseInt(y) + " Kb" : y = (y / 1024).toFixed(2) + " Mb", m.innerHTML = c.name + " / " + y, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + y + ". Por favor, adicione um arquivo menor.")
-            }, d.readAsDataURL(c)
+                var x = c.size / 1024;
+                x < 1024 ? x = parseInt(x) + " Kb" : x = (x / 1024).toFixed(2) + " Mb", m.innerHTML = c.name + " / " + x, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + x + ". Por favor, adicione um arquivo menor.")
+            }, s.readAsDataURL(c)
         }
     }
 
     function i() {
-        var l = e.data.type;
-        if (l == "datetime" && (l = "datetime-regional"), l == "decimal" && (l = "text"), l == "file") {
+        var o = e.data.type;
+        if (o == "datetime" && (o = "datetime-regional"), o == "decimal" && (o = "text"), o == "file") {
             const u = {
                 alignContent: "center",
                 height: 75,
                 padding: 5,
                 maxWidth: "100%",
                 margin: "auto"
             };
-            var d = null;
-            return e.data.extensions && e.data.extensions.length > 0 && (d = e.data.extensions.map(s => "." + s).join(", ")), t.jsxs(t.Fragment, {
+            var s = null;
+            return e.data.extensions && e.data.extensions.length > 0 && (s = e.data.extensions.map(l => "." + l).join(", ")), t.jsxs(t.Fragment, {
                 children: [t.jsxs("div", {
                     style: {
                         display: window.innerWidth < 800 ? "block" : "flex",
                         justifyContent: "space-between",
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10,
                         textAlign: "center"
                     },
                     children: [t.jsx("div", {
                         style: u,
-                        children: t.jsx(k, {
+                        children: t.jsx(b, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
                                 color: "#1351b4"
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
-                        children: [e.data.value && ne(e.data.value) && t.jsx("div", {
+                        children: [e.data.value && ae(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
                             },
                             children: t.jsx("img", {
                                 src: e.data.value,
                                 height: 50
                             })
-                        }), e.data.value && !ne(e.data.value) && t.jsx("div", {
+                        }), e.data.value && !ae(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
                             },
                             children: e.data.value
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
-                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(s => "." + s).join(" ou "), "."]
+                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(l => "." + l).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
-                        children: t.jsx(A, {
+                        children: t.jsx(q, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
-                    type: l,
+                    type: o,
                     name: e.data.name,
                     id: a,
                     "data-label": w(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
-                    onChange: o,
+                    onChange: d,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
-                    accept: d
+                    accept: s
                 })]
             })
         } else {
             var c = Y;
-            return l == "color" && (c = {
+            return o == "color" && (c = {
                 ...Y
             }, c.width = "100%", c.backgroundColor = "white", c.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
-                type: l,
+                type: o,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
                 "data-label": w(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
-                onChange: o,
+                onChange: d,
                 style: c
             })
         }
     }
     return i()
 }
 
-function ke(e) {
+function Se(e) {
     var n = [];
-    Array.isArray(e.data.value) ? e.data.value.forEach(function(p, h) {
+    Array.isArray(e.data.value) ? e.data.value.forEach(function(h, f) {
         n.push({
-            id: p.id,
-            value: p.label
+            id: h.id,
+            value: h.label
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
-        o = Array.isArray(e.data.value),
-        [i, l] = M.useState(!1),
-        [d, c] = M.useState(null);
+        d = Array.isArray(e.data.value),
+        [i, o] = C.useState(!1),
+        [s, c] = C.useState(null);
     var u = !1;
-    M.useEffect(() => {
-        q(n), document.getElementById(a).addEventListener("customchange", function(p) {
-            q(p.detail.value), reactTriggerChange(document.getElementById(e.data.name))
+    let l;
+    C.useEffect(() => {
+        S(n), document.getElementById(a).addEventListener("customchange", function(h) {
+            S(h.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
-    function s() {
-        const p = document.getElementById(a);
-        if (o) {
-            const h = {
+    function m() {
+        const h = document.getElementById(a);
+        if (d) {
+            const f = {
                     padding: 5,
                     display: "inline"
                 },
                 g = {
                     cursor: "pointer",
                     marginRight: 5
                 },
-                f = {
+                p = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [p == null && n.map((b, S) => t.jsxs("div", {
-                    style: h,
+                children: [h == null && n.map((k, N) => t.jsxs("div", {
+                    style: f,
                     children: [t.jsx("span", {
-                        onClick: () => C(S),
+                        onClick: () => F(N),
                         style: g,
-                        children: t.jsx(k, {
+                        children: t.jsx(b, {
                             icon: "trash-can",
-                            style: f
+                            style: p
                         })
-                    }), b.value]
-                }, Math.random())), p != null && Array.from(p.options).map((b, S) => t.jsxs("div", {
-                    style: h,
+                    }), k.value]
+                }, Math.random())), h != null && Array.from(h.options).map((k, N) => t.jsxs("div", {
+                    style: f,
                     children: [t.jsx("span", {
-                        onClick: () => C(S),
+                        onClick: () => F(N),
                         style: g,
-                        children: t.jsx(k, {
+                        children: t.jsx(b, {
                             icon: "trash-can",
-                            style: f
+                            style: p
                         })
-                    }), b.innerHTML]
+                    }), k.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
-    function m(p) {
+    function x(h) {
         c([])
     }
 
-    function y() {
+    function v() {
         return t.jsx("select", {
-            onChange: m,
+            onChange: x,
             id: a,
             name: e.data.name,
-            multiple: o,
+            multiple: d,
             readOnly: !0,
             style: {
                 display: "contents"
             }
         })
     }
 
-    function v() {
-        const p = {
+    function j() {
+        const h = {
                 ...Y,
                 ...e.style || {}
             },
-            h = {
+            f = {
                 padding: 0,
                 margin: 0,
-                border: "solid 1px #CCC",
+                border: "solid 1px #d9d9d9",
                 marginTop: -1,
                 borderRadius: 5,
                 maxHeight: 150,
                 overflowY: "auto"
             };
-        h.position = "absolute", h.backgroundColor = "white";
+        f.position = "absolute", f.backgroundColor = "white";
         const g = document.getElementById(r);
         if (g) {
-            let E = null,
-                O = g,
-                W = null;
-            for (; !W && (O = O.parentElement) instanceof HTMLElement;) O.matches("dialog") && (W = O);
-            E = W;
-            const _ = g.getBoundingClientRect();
-            var f = _.top + _.height,
-                b = _.left;
-            if (E) {
-                const G = E.getBoundingClientRect();
-                f = f - G.top, b = b - G.left
-            } else f += window.scrollY, b += window.scrollX;
-            h.width = _.width, h.top = f, h.left = b
+            let T = null,
+                z = g,
+                G = null;
+            for (; !G && (z = z.parentElement) instanceof HTMLElement;) z.matches("dialog") && (G = z);
+            T = G;
+            const R = g.getBoundingClientRect();
+            var p = R.top + R.height,
+                k = R.left;
+            if (T) {
+                const X = T.getBoundingClientRect();
+                p = p - X.top, k = k - X.left
+            } else p += window.scrollY, k += window.scrollX;
+            f.width = R.width, f.top = p, f.left = k
         }
-        const S = {
+        const N = {
                 cursor: "pointer",
                 padding: 10
             },
-            ee = !o && n.length > 0 && n[0].value || "";
+            te = !d && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
             children: [t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
-                onFocus: E => {
-                    E.target.select(), T(E)
+                onFocus: T => {
+                    T.target.select(), B(T)
                 },
-                onChange: T,
-                onMouseLeave: j,
-                onBlur: j,
-                defaultValue: ee,
-                style: p,
-                "data-label": w(e.data.label)
-            }), d && i && t.jsxs("ul", {
+                onChange: B,
+                onMouseLeave: D,
+                onBlur: D,
+                defaultValue: te,
                 style: h,
-                onMouseLeave: I,
-                onMouseEnter: function(E) {
+                "data-label": w(e.data.label)
+            }), s && i && t.jsxs("ul", {
+                style: f,
+                onMouseLeave: M,
+                onMouseEnter: function(T) {
                     u = !0
                 },
-                children: [d.length == 0 && t.jsx("li", {
-                    style: S,
+                children: [s.length == 0 && t.jsx("li", {
+                    style: N,
                     children: "Nenhuma opção encontrada."
-                }), d.map(E => t.jsx("li", {
+                }), s.map(T => t.jsx("li", {
                     onClick: () => {
-                        l(!1), e.onSelect ? e.onSelect(E) : q(E)
+                        o(!1), e.onSelect ? e.onSelect(T) : S(T)
                     },
-                    style: S,
+                    style: N,
                     className: "autocomplete-item",
-                    "data-label": w(E.value),
-                    children: E.value
+                    "data-label": w(T.value),
+                    children: T.value
                 }, Math.random()))]
             })]
         })
     }
 
-    function j(p) {
+    function D(h) {
         u = !1, setTimeout(function() {
-            I(p)
+            M(h)
         }, 250)
     }
 
-    function I(p) {
-        const h = document.getElementById(a),
+    function M(h) {
+        const f = document.getElementById(a),
             g = document.getElementById(r);
-        o || h.options.length > 0 && g.value != h.options[0].innerHTML && (h.innerHTML = "", g.value = "", l(!1)), p.target.tagName == "UL" ? l(!1) : u || l(!1)
+        d || f.options.length > 0 && g.value != f.options[0].innerHTML && (f.innerHTML = "", g.value = "", o(!1)), h.target.tagName == "UL" ? o(!1) : u || o(!1)
     }
 
-    function T(p) {
-        const h = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-        l(!0), D("GET", e.data.choices + h + "term=" + p.target.value, function(f) {
-            c(f)
-        })
+    function B(h) {
+        clearTimeout(l), l = setTimeout(function() {
+            const f = e.data.choices.indexOf("?") < 0 ? "?" : "&";
+            o(!0), E("GET", e.data.choices + f + "term=" + h.target.value, function(p) {
+                c(p)
+            })
+        }, 1e3)
     }
 
-    function q(p) {
-        const h = document.getElementById(a),
+    function S(h) {
+        const f = document.getElementById(a),
             g = document.getElementById(r);
-        h.innerHTML == null && (h.innerHTML = ""), Array.isArray(p) ? h.innerHTML = p.map(f => `<option selected value="${f.id}">${f.value}</option>`).join("") : o ? (h.innerHTML += `<option selected value="${p.id}">${p.value}</option>`, g.value = "") : (h.innerHTML = `<option selected value="${p.id}">${p.value}</option>`, g.value = p.value), e.data.onchange && je(g.closest("form"), e.data.onchange)
+        f.innerHTML == null && (f.innerHTML = ""), Array.isArray(h) ? f.innerHTML = h.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : d ? (f.innerHTML += `<option selected value="${h.id}">${h.value}</option>`, g.value = "") : (f.innerHTML = `<option selected value="${h.id}">${h.value}</option>`, g.value = h.value), e.data.onchange && ke(g.closest("form"), e.data.onchange)
     }
 
-    function C(p) {
-        const h = document.getElementById(a);
-        var g = Array.from(h.options);
-        h.innerHTML = g.slice(0, p).concat(g.slice(p + 1)).map(f => `<option selected value="${f.value}">${f.innerHTML}</option>`).join(""), c([])
+    function F(h) {
+        const f = document.getElementById(a);
+        var g = Array.from(f.options);
+        f.innerHTML = g.slice(0, h).concat(g.slice(h + 1)).map(p => `<option selected value="${p.value}">${p.innerHTML}</option>`).join(""), c([])
     }
 
-    function P() {
+    function I() {
         return t.jsxs(t.Fragment, {
-            children: [s(), y(), v()]
+            children: [m(), v(), j()]
         })
     }
-    return P()
+    return I()
 }
 
 function at(e) {
     function n() {
         var a = {
             ...Y
         };
@@ -1641,103 +1656,103 @@
     var n = e.data;
     return n.choices = [{
         id: !0,
         value: "Sim"
     }, {
         id: !1,
         value: "Não"
-    }], t.jsx(ae, {
+    }], t.jsx(re, {
         data: n
     })
 }
 
-function ae(e) {
+function re(e) {
     var n = Math.random(),
         a = e.data;
 
-    function r(d) {
-        return a.value != null ? a.value == d.id ? !0 : a.value.id == d.id : !1
+    function r(s) {
+        return a.value != null ? a.value == s.id ? !0 : a.value.id == s.id : !1
     }
 
-    function o(d) {
-        var c = document.getElementById(d);
+    function d(s) {
+        var c = document.getElementById(s);
         a.checked && (c.checked = !1)
     }
 
-    function i(d) {
-        var c = document.getElementById(d);
+    function i(s) {
+        var c = document.getElementById(s);
         a.checked = c.checked
     }
 
-    function l() {
+    function o() {
         return t.jsx("div", {
             className: "radio-group",
-            children: a.choices.map((d, c) => t.jsxs("div", {
+            children: a.choices.map((s, c) => t.jsxs("div", {
                 style: {
                     paddingTop: 10
                 },
                 children: [t.jsx("input", {
                     id: a.name + n + c,
                     type: "radio",
                     name: a.name,
-                    defaultValue: d.id,
-                    defaultChecked: r(d),
-                    "data-label": w(d.value),
+                    defaultValue: s.id,
+                    defaultChecked: r(s),
+                    "data-label": w(s.value),
                     onClick: function() {
-                        o(a.name + n + c)
+                        d(a.name + n + c)
                     },
                     onMouseEnter: function() {
                         i(a.name + n + c)
                     }
                 }), t.jsx("label", {
                     htmlFor: a.name + n + c,
-                    children: d.value
+                    children: s.value
                 })]
             }, n + c))
         })
     }
-    return l()
+    return o()
 }
 
-function ue(e) {
+function he(e) {
     var n = Math.random(),
         a = e.data;
 
     function r(i) {
-        var l = !1;
+        var o = !1;
         if (a.value)
-            for (var d = 0; d < a.value.length; d++) {
-                var c = a.value[d];
-                (c == i.id || c.id == i.id) && (l = !0)
+            for (var s = 0; s < a.value.length; s++) {
+                var c = a.value[s];
+                (c == i.id || c.id == i.id) && (o = !0)
             }
-        return l
+        return o
     }
 
-    function o() {
+    function d() {
         return t.jsx("div", {
             className: "checkbox-group",
-            children: a.choices.map((i, l) => t.jsxs("div", {
+            children: a.choices.map((i, o) => t.jsxs("div", {
                 style: {
                     paddingTop: 10
                 },
                 children: [t.jsx("input", {
-                    id: a.name + n + l,
+                    id: a.name + n + o,
                     type: "checkbox",
                     name: a.name,
                     defaultValue: i.id,
                     defaultChecked: r(i),
                     "data-label": w(i.value)
                 }), t.jsx("label", {
-                    htmlFor: a.name + n + l,
+                    htmlFor: a.name + n + o,
                     children: i.value
                 })]
-            }, n + l))
+            }, n + o))
         })
     }
-    return o()
+    return d()
 }
 
 function it(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
@@ -1755,203 +1770,203 @@
 }
 
 function lt(e) {
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
-    function o() {
+    function d() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
-            children: t.jsxs(ie, {
+            children: t.jsxs(le, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
-                children: [t.jsx(A, {
+                children: [t.jsx(q, {
                     primary: !0,
                     icon: "pen-clip",
                     onClick: () => i(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
-                }), t.jsx(A, {
+                }), t.jsx(q, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => i(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
         })
     }
 
     function i(c) {
         const u = document.querySelector("input[name=" + r.name + "]"),
-            s = document.getElementById("inline-form-" + n),
+            l = document.getElementById("inline-form-" + n),
             m = document.getElementById("show-" + n),
-            y = document.getElementById("hide-" + n);
-        s.style.display = c ? "block" : "none", m.style.display = c ? "none" : "inline", y.style.display = c ? "inline" : "none", c ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+            x = document.getElementById("hide-" + n);
+        l.style.display = c ? "block" : "none", m.style.display = c ? "none" : "inline", x.style.display = c ? "inline" : "none", c ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
-    function l() {
+    function o() {
         const c = {
             display: r.value ? "block" : "none"
         };
         return e.data.required && (c.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
             className: "fieldset-inline-forms",
             style: c,
             id: "inline-form-" + n,
             children: e.data.value.map(function(u) {
-                return t.jsx(le, {
+                return t.jsx(oe, {
                     data: u
                 }, Math.random())
             })
         })
     }
 
-    function d() {
+    function s() {
         const c = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: c,
                 "data-label": w(e.data.label),
                 children: e.data.label
-            }), o(), l()]
+            }), d(), o()]
         })
     }
-    return d()
+    return s()
 }
 
 function ot(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
-    function r(s, m) {
-        const y = n;
+    function r(l, m) {
+        const x = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
-            id: "form-" + y + "-" + a,
-            children: [t.jsx(le, {
-                data: s
+            id: "form-" + x + "-" + a,
+            children: [t.jsx(oe, {
+                data: l
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
-                children: [t.jsx(A, {
+                children: [t.jsx(q, {
                     primary: !0,
                     icon: "plus",
                     onClick: () => i(),
-                    id: "extra-add-" + y + "-",
+                    id: "extra-add-" + x + "-",
                     display: m
-                }), t.jsx(A, {
+                }), t.jsx(q, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => l(y),
+                    onClick: () => o(x),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
-    function o() {
-        const s = d(),
-            m = s.length > 0 ? "none" : "inline";
+    function d() {
+        const l = s(),
+            m = l.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = m;
-        for (var y = 0; y < n; y++) {
-            var v = document.getElementById("extra-add-" + y + "-");
+        for (var x = 0; x < n; x++) {
+            var v = document.getElementById("extra-add-" + x + "-");
             v.style.display = "none"
         }
-        if (s.length > 0) {
-            var v = document.getElementById("extra-add-" + s[s.length - 1] + "-");
+        if (l.length > 0) {
+            var v = document.getElementById("extra-add-" + l[l.length - 1] + "-");
             v.style.display = "inline"
         }
     }
 
     function i() {
-        o();
-        var s = JSON.parse(JSON.stringify(e.data.template));
-        s.fields ? (s.fields.map(function(m) {
+        d();
+        var l = JSON.parse(JSON.stringify(e.data.template));
+        l.fields ? (l.fields.map(function(m) {
             m.name = m.name.replace("__n__", "__" + n + "__")
-        }), s.fields[0].value = 0) : s.fieldsets.map(function(m) {
-            m.fields.map(function(y) {
-                y.map(function(v) {
+        }), l.fields[0].value = 0) : l.fieldsets.map(function(m) {
+            m.fields.map(function(x) {
+                x.map(function(v) {
                     v.name = v.name.replace("__n__", "__" + n + "__")
-                }), y[0].value = 0
+                }), x[0].value = 0
             })
-        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(s, "inline")), setTimeout(o, 100)
+        }), W.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(l, "inline")), setTimeout(d, 100)
     }
 
-    function l(s) {
+    function o(l) {
         const m = e.data.template,
-            v = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + s + "__"),
+            v = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + l + "__"),
             j = document.querySelector("input[name=" + v + "]");
-        parseInt(j.value) == 0 ? j.value = "" : j.value = -parseInt(j.value), document.getElementById("form-" + s + "-" + a).style.display = "none", o()
+        parseInt(j.value) == 0 ? j.value = "" : j.value = -parseInt(j.value), document.getElementById("form-" + l + "-" + a).style.display = "none", d()
     }
 
-    function d() {
-        for (var s = [], m = 0; m < n; m++) document.getElementById("form-" + m + "-" + a).style.display == "block" && s.push(m);
-        return s
+    function s() {
+        for (var l = [], m = 0; m < n; m++) document.getElementById("form-" + m + "-" + a).style.display == "block" && l.push(m);
+        return l
     }
 
     function c() {
         return t.jsx("div", {
             id: "info-" + a,
-            children: t.jsx(ie, {
+            children: t.jsx(le, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
-                children: t.jsx(A, {
+                children: t.jsx(q, {
                     primary: !0,
                     icon: "add",
                     onClick: () => i(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
         })
     }
 
     function u() {
-        const s = {
+        const l = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: s,
+                style: l,
                 "data-label": w(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
-                children: [c(), e.data.value.map(function(m, y) {
-                    return r(m, y == e.data.value.length - 1 ? "inline" : "none")
+                children: [c(), e.data.value.map(function(m, x) {
+                    return r(m, x == e.data.value.length - 1 ? "inline" : "none")
                 })]
             })]
         })
     }
     return u()
 }
 
-function le(e) {
+function oe(e) {
     function n(r) {
         return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(lt, {
             data: r
         }, Math.random()) : t.jsx(ot, {
             data: r
-        }, Math.random()) : t.jsx(Q, {
+        }, Math.random()) : t.jsx(K, {
             data: r
         }, Math.random())
     }
 
     function a() {
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
@@ -1963,18 +1978,18 @@
                     "data-label": w(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), t.jsx("div", {
                     className: "fieldset-fields",
-                    children: r.fields.map(o => t.jsx("div", {
-                        children: o.map(i => t.jsx("div", {
+                    children: r.fields.map(d => t.jsx("div", {
+                        children: d.map(i => t.jsx("div", {
                             style: {
-                                width: 100 / o.length + "%",
+                                width: 100 / d.length + "%",
                                 display: i.type == "hidden" ? "none" : "inline-block"
                             },
                             children: n(i)
                         }, Math.random()))
                     }, Math.random()))
                 })]
             })
@@ -1983,118 +1998,141 @@
     return a()
 }
 
 function dt(e) {
     const n = Math.random();
 
     function a() {
-        const s = {
+        const l = {
             margin: 0,
             textAlign: "left"
         };
         return t.jsx("h1", {
-            style: s,
+            style: l,
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
 
-    function o() {
+    function d() {
         if (e.data.display) return t.jsxs(t.Fragment, {
-            children: [e.data.display.map(s => t.jsx(x, {
-                data: s
+            children: [e.data.display.map(l => t.jsx(y, {
+                data: l
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
             })]
         })
     }
 
     function i() {
-        return t.jsx(le, {
+        return t.jsx(oe, {
             data: e.data
         })
     }
 
-    function l() {
+    function o() {
         return t.jsxs("div", {
             style: {
                 marginTop: 20,
                 textAlign: "right"
             },
-            children: [t.jsx(A, {
+            children: [t.jsx(q, {
                 onClick: c,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
-            }), t.jsx(A, {
+            }), t.jsx(q, {
                 onClick: u,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
         })
     }
 
-    function d() {
+    function s() {
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
-                    padding: 20
+                    padding: 5
                 },
-                children: [a(), r(), o(), i(), l()]
+                children: [a(), r(), d(), i(), o()]
             })]
         })
     }
 
     function c() {
         V()
     }
 
-    function u(s) {
-        s.preventDefault();
+    function u(l) {
+        l.preventDefault();
         var m = document.getElementById(n),
-            y = new FormData(m);
-        D("POST", e.data.url, function(j) {
-            if (s.target.dataset.spinning && (s.target.querySelector("i.fa-spin").style.display = "none", s.target.querySelector("i.fa-" + s.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return V(), $e(), ge(j);
-            var I = j.text;
-            console.log(j), Object.keys(j.errors).map(function(T) {
-                if (T == "__all__") I = j.errors[T];
+            x = new FormData(m);
+        E("POST", e.data.url, function(j) {
+            if (l.target.dataset.spinning && (l.target.querySelector("i.fa-spin").style.display = "none", l.target.querySelector("i.fa-" + l.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return V(), Je(), xe(j);
+            var D = j.text;
+            console.log(j), Object.keys(j.errors).map(function(M) {
+                if (M == "__all__") D = j.errors[M];
                 else {
-                    const q = m.querySelector("#" + T + "_error");
-                    q.querySelector("span").innerHTML = j.errors[T], q.style.display = "block"
+                    const B = m.querySelector("#" + M + "_error");
+                    B.querySelector("span").innerHTML = j.errors[M], B.style.display = "block"
                 }
-            }), K(I, !0)
-        }, y)
+            }), Z(D, !0)
+        }, x)
     }
-    return d()
+    return s()
 }
 
 function st(e) {
+    function n() {
+        const a = {
+            backgroundColor: "#1351b4",
+            color: "white",
+            borderRadius: "50%",
+            minWidth: 13,
+            marginLeft: 2,
+            padding: 4,
+            fontSize: "70%",
+            display: "inline-block",
+            verticalAlign: "bottom",
+            marginBottom: 10,
+            lineHeight: 1
+        };
+        return t.jsx("div", {
+            style: a,
+            children: e.total
+        })
+    }
+    return n()
+}
+
+function ct(e) {
     e.data.id == null && (e.data.id = Math.random());
-    const [n, a] = M.useState(e.data);
+    const [n, a] = C.useState(e.data);
 
     function r() {
         const h = {
             margin: 0
         };
         return n.attrname ? t.jsx("h2", {
             style: h,
@@ -2103,15 +2141,15 @@
         }) : t.jsx("h1", {
             style: h,
             "data-label": w(n.title),
             children: n.title
         })
     }
 
-    function o() {
+    function d() {
         const h = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "center"
         };
         return t.jsxs("div", {
             style: h,
@@ -2125,500 +2163,504 @@
         })
     }
 
     function i(h) {
         document.getElementById("loader-" + e.data.id).style.display = h ? "block" : "none"
     }
 
-    function l() {
+    function o() {
         return n.subsets && t.jsx("div", {
             style: {
-                display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 paddingBottom: 20,
                 lineHeight: "2.5rem"
             },
-            children: n.subsets.map(function(h, g) {
-                var f = n.subset === h.name || !n.subset && g == 0;
-                return t.jsx(z, {
+            children: n.subsets.map(function(h, f) {
+                var g = n.subset === h.name || !n.subset && f == 0;
+                return t.jsxs(P, {
                     href: "#",
                     style: {
                         paddingBottom: 5,
                         paddingLeft: 15,
                         paddingRight: 15,
-                        fontWeight: f ? "bold" : "normal",
-                        borderBottom: f ? "solid 3px #2670e8" : "solid 3px #DDD",
+                        fontWeight: g ? "bold" : "normal",
+                        borderBottom: g ? "solid 3px #2670e8" : 0,
                         textDecoration: "none",
                         color: "#0c326f"
                     },
-                    onClick: function(b) {
-                        b.preventDefault(), d(h.name)
+                    onClick: function(p) {
+                        p.preventDefault(), s(h.name)
                     },
                     dataLabel: w(h.label),
-                    children: t.jsxs("div", {
-                        style: {
-                            display: "inline-block"
-                        },
-                        children: [h.label, " (", h.count, ")"]
-                    })
+                    children: [h.label, " ", t.jsx(st, {
+                        total: h.count + 1
+                    })]
                 }, Math.random())
             })
         })
     }
 
-    function d(h) {
-        const g = document.getElementById("subset-" + e.data.id);
-        g.value = h || "", C()
+    function s(h) {
+        const f = document.getElementById("subset-" + e.data.id);
+        f.value = h || "", S()
     }
 
-    function c(h, g, f) {
-        const b = document.getElementById("form-" + e.data.id);
-        b.querySelector("input[name=" + n.calendar.field + "__day]").value = h || "", b.querySelector("input[name=" + n.calendar.field + "__month]").value = g || "", b.querySelector("input[name=" + n.calendar.field + "__year]").value = f || "", C()
+    function c(h, f, g) {
+        const p = document.getElementById("form-" + e.data.id);
+        p.querySelector("input[name=" + n.calendar.field + "__day]").value = h || "", p.querySelector("input[name=" + n.calendar.field + "__month]").value = f || "", p.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", S()
     }
 
     function u() {
         if (n.calendar) {
-            const S = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
-                ee = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
-                E = {
+            const k = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
+                N = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
+                te = {
                     width: "100%",
                     borderSpacing: 0,
                     borderCollapse: "collapse",
                     marginTop: 15,
                     marginBottom: 15
                 },
-                O = {
+                T = {
                     marginLeft: "17",
                     textAlign: "right",
                     paddingRight: 2,
                     paddingTop: 2,
                     float: "right",
                     fontSize: "0.8rem"
                 },
-                W = {
+                z = {
                     verticalAlign: "top",
                     width: "14.2%",
                     height: 55,
                     border: "solid 1px #EEE"
                 },
-                _ = {
+                G = {
                     backgroundColor: "#1351b4",
                     borderRadius: "50%",
                     color: "white",
                     display: "block",
                     width: 30,
                     height: 30,
                     margin: "auto",
                     cursor: "pointer",
                     lineHeight: "2rem"
                 },
-                G = {
+                R = {
                     padding: 10,
                     textAlign: "center"
                 },
-                Te = {
+                X = {
                     display: "flex",
                     justifyContent: "space-between",
                     alignItems: "baseline"
                 },
                 Ee = new Date,
-                de = n.calendar.day ? new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day) : null;
+                se = n.calendar.day ? new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day) : null;
             for (var h = [
                     [],
                     [],
                     [],
                     [],
                     [],
                     []
-                ], g = n.calendar.month - 1, f = new Date(n.calendar.year, n.calendar.month - 1, 1); f.getDay() > 1;) f.setDate(f.getDate() - 1);
-            for (var b = 0;
-                (f.getMonth() <= g || h[b].length < 7) && (h[b].length == 7 && (b += 1), b != 5);) h[b].push({
-                date: f.getDate(),
-                total: n.calendar.total[f.toLocaleDateString("pt-BR")],
-                today: f.getDate() === Ee.getDate(),
-                selected: de ? f.getDate() == de.getDate() : !1
-            }), f.setDate(f.getDate() + 1);
+                ], f = n.calendar.month - 1, g = new Date(n.calendar.year, n.calendar.month - 1, 1); g.getDay() > 1;) g.setDate(g.getDate() - 1);
+            for (var p = 0;
+                (g.getMonth() <= f || h[p].length < 7) && (h[p].length == 7 && (p += 1), p != 5);) h[p].push({
+                date: g.getDate(),
+                total: n.calendar.total[g.toLocaleDateString("pt-BR")],
+                today: g.getDate() === Ee.getDate(),
+                selected: se ? g.getDate() == se.getDate() : !1
+            }), g.setDate(g.getDate() + 1);
             return t.jsxs("div", {
                 className: "calendar",
                 children: [t.jsxs("div", {
-                    style: Te,
+                    style: X,
                     children: [t.jsx("div", {
-                        children: t.jsx(se, {
+                        children: t.jsx(ce, {
                             default: !0,
                             icon: "arrow-left",
                             onClick: () => c(null, n.calendar.previous.month, n.calendar.previous.year)
                         })
                     }), t.jsxs("div", {
                         children: [t.jsxs("h3", {
                             align: "center",
                             style: {
                                 margin: 0
                             },
-                            children: [ee[n.calendar.month - 1], " ", n.calendar.year]
+                            children: [N[n.calendar.month - 1], " ", n.calendar.year]
                         }), n.calendar.day && t.jsxs("div", {
                             align: "center",
-                            className: O,
-                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(k, {
+                            className: T,
+                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(b, {
                                 default: !0,
                                 icon: "x",
                                 onClick: () => c(null, n.calendar.month, n.calendar.year),
                                 style: {
                                     marginLeft: 10,
                                     cursor: "pointer"
                                 }
                             })]
                         })]
                     }), t.jsx("div", {
-                        children: t.jsx(se, {
+                        children: t.jsx(ce, {
                             default: !0,
                             icon: "arrow-right",
                             onClick: () => c(null, n.calendar.next.month, n.calendar.next.year)
                         })
                     })]
                 }), t.jsxs("table", {
-                    style: E,
+                    style: te,
                     children: [t.jsx("thead", {
                         children: t.jsx("tr", {
-                            children: S.map(te => t.jsx("th", {
-                                children: te
+                            children: k.map(ne => t.jsx("th", {
+                                children: ne
                             }, Math.random()))
                         })
                     }), t.jsx("tbody", {
-                        children: h.map(te => t.jsx("tr", {
-                            children: te.map(L => t.jsxs("td", {
-                                style: W,
+                        children: h.map(ne => t.jsx("tr", {
+                            children: ne.map(A => t.jsxs("td", {
+                                style: z,
                                 children: [t.jsx("div", {
-                                    style: O,
-                                    children: L.today ? t.jsx("span", {
+                                    style: T,
+                                    children: A.today ? t.jsx("span", {
                                         style: {
                                             textDecoration: "underline"
                                         },
-                                        children: L.date
-                                    }) : L.date + L.today
-                                }), L.total && t.jsx("div", {
-                                    style: G,
-                                    onClick: () => c(L.date, n.calendar.month, n.calendar.year),
+                                        children: A.date
+                                    }) : A.date + A.today
+                                }), A.total && t.jsx("div", {
+                                    style: R,
+                                    onClick: () => c(A.date, n.calendar.month, n.calendar.year),
                                     children: t.jsx("div", {
-                                        style: _,
+                                        style: G,
                                         children: t.jsx("span", {
                                             style: {
-                                                textDecoration: L.selected ? "underline" : "normal"
+                                                textDecoration: A.selected ? "underline" : "normal"
                                             },
-                                            children: L.total
+                                            children: A.total
                                         })
                                     })
-                                }), !L.total && t.jsx("div", {
-                                    style: G,
+                                }), !A.total && t.jsx("div", {
+                                    style: R,
                                     children: " "
                                 })]
                             }, Math.random()))
                         }, Math.random()))
                     })]
                 })]
             })
         }
     }
 
-    function s(h) {
-        const g = {
+    function l(h) {
+        const f = {
             textAlign: "left",
             verticalAlign: "top",
+            backgroundColor: "#f0f0f0",
+            lineHeight: "3rem",
+            color: "#1351b4",
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
-            children: [h.map(function(f) {
-                return f.label != "ID" && t.jsx("th", {
-                    style: g,
-                    className: "bold",
-                    children: f.label
+            children: [h.map(function(g) {
+                return g.label != "ID" && t.jsx("th", {
+                    style: f,
+                    children: g.label
                 }, Math.random())
             }), t.jsx("th", {
-                style: g
+                style: f
             })]
         })
     }
 
     function m(h) {
-        const g = {
+        const f = {
                 borderBottom: "solid 1px #DDD",
                 padding: 5
             },
-            f = {
+            g = {
                 borderBottom: "solid 1px #DDD",
-                lineHeight: "3rem"
+                lineHeight: "3rem",
+                textAlign: "right"
             };
         return window.innerWidth < 800 ? t.jsxs("tr", {
             children: [t.jsx("td", {
-                style: g,
+                style: f,
                 children: h.title
             }, Math.random()), t.jsx("td", {
-                style: f,
+                style: g,
                 children: t.jsx("div", {
                     style: {
-                        verticalAlign: "center",
-                        textAlign: "right"
+                        verticalAlign: "center"
                     },
-                    children: h.actions.map(function(b) {
-                        return t.jsx(N, {
-                            data: b,
+                    children: h.actions.map(function(p) {
+                        return t.jsx(O, {
+                            data: p,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [h.data.map(function(b) {
-                return b.label != "ID" && t.jsx("td", {
-                    style: g,
-                    children: U(b.value)
+            children: [h.data.map(function(p) {
+                return p.label != "ID" && t.jsx("td", {
+                    style: f,
+                    children: U(p.value)
                 }, Math.random())
             }), t.jsx("td", {
-                style: f,
+                style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: h.actions.map(function(b) {
-                        return t.jsx(N, {
-                            data: b,
+                    children: h.actions.map(function(p) {
+                        return t.jsx(O, {
+                            data: p,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random())
     }
 
-    function y() {
-        return n.data.length > 0 ? n.renderer ? t.jsx(t.Fragment, {
+    function x() {
+        return n.data.length > 0 ? n.renderer ? t.jsx("div", {
+            style: {
+                marginBottom: 15
+            },
             children: n.data.map(function(h) {
-                return h.type = n.renderer, t.jsx(x, {
+                return h.type = n.renderer, t.jsx(y, {
                     data: h
                 }, Math.random())
             })
-        }) : v() : t.jsx(ie, {
+        }) : v() : t.jsx(le, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function v() {
         const h = {
                 width: "100%",
                 overflowX: "auto"
             },
-            g = {
+            f = {
                 width: "100%",
                 lineHeight: "2rem",
                 borderSpacing: 0
             };
         return t.jsx("div", {
             style: h,
             children: t.jsxs("table", {
-                style: g,
+                style: f,
                 children: [t.jsx("thead", {
-                    children: s(n.data[0].data)
+                    children: l(n.data[0].data)
                 }), t.jsx("tbody", {
-                    children: n.data.map(function(f) {
-                        return m(f)
+                    children: n.data.map(function(g) {
+                        return m(g)
                     })
                 })]
             })
         })
     }
 
     function j(h) {
-        const f = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        f.value = h, C()
+        const g = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
+        g.value = h, S()
     }
 
-    function I() {
+    function D() {
         const h = document.getElementById("form-" + e.data.id);
         if (h) {
-            const S = h.querySelector("input[name=page]");
-            S && (S.value = n.pagination.page.current)
+            const k = h.querySelector("input[name=page]");
+            k && (k.value = n.pagination.page.current)
         }
-        const g = {
+        const f = {
                 display: "flex",
                 justifyContent: "space-between",
                 lineHeight: "4rem",
                 alignItems: "baseline"
             },
-            f = {
+            g = {
                 display: "inline",
                 paddingRight: 10
             },
-            b = {
+            p = {
                 marginLeft: 10,
                 marginRight: 10,
                 height: "2.5rem",
                 paddingLeft: 5,
                 paddingRight: 5,
                 textAlign: "center"
             };
         return n.pagination.page.total > 1 && t.jsxs("div", {
-            style: g,
+            style: f,
             children: [t.jsxs("div", {
                 children: [t.jsxs("div", {
-                    style: f,
+                    style: g,
                     children: ["Exibir", t.jsx("select", {
-                        style: b,
+                        style: p,
                         name: "page_size",
                         onChange: () => j(1),
                         value: n.pagination.page.size,
-                        children: n.pagination.page.sizes.map(function(S) {
+                        children: n.pagination.page.sizes.map(function(k) {
                             return t.jsx("option", {
-                                children: S
+                                children: k
                             }, Math.random())
                         })
                     })]
                 }), t.jsx("div", {
-                    style: f,
+                    style: g,
                     children: "|"
                 }), t.jsxs("div", {
-                    style: f,
+                    style: g,
                     children: [n.pagination.start, " - ", n.pagination.end, " de ", n.total]
                 })]
             }), t.jsx("div", {
                 children: t.jsxs("div", {
-                    style: f,
+                    style: g,
                     children: [t.jsx("span", {
                         children: "Página"
                     }), t.jsx("input", {
                         type: "text",
                         name: "page",
                         defaultValue: n.pagination.page.current,
                         style: {
                             width: 30,
                             marginLeft: 10,
                             marginRight: 10,
                             height: "2rem",
                             textAlign: "center"
                         },
-                        onKeyDown: function(S) {
-                            S.key == "Enter" && (S.preventDefault(), j(S.target.value < 0 ? 1 : Math.min(S.target.value, n.pagination.page.total)))
+                        onKeyDown: function(k) {
+                            k.key == "Enter" && (k.preventDefault(), j(k.target.value < 0 ? 1 : Math.min(k.target.value, n.pagination.page.total)))
                         }
                     }), t.jsx("div", {
-                        style: f,
+                        style: g,
                         children: "|"
-                    }), n.pagination.page.previous && t.jsx(A, {
+                    }), n.pagination.page.previous && t.jsx(q, {
                         icon: "chevron-left",
                         default: !0,
                         display: "inline",
                         onClick: () => j(n.pagination.page.previous)
-                    }), n.pagination.page.next && t.jsx(A, {
+                    }), n.pagination.page.next && t.jsx(q, {
                         icon: "chevron-right",
                         default: !0,
                         display: "inline",
                         onClick: () => j(n.pagination.page.next)
                     })]
                 })
             })]
         })
     }
 
-    function T() {
+    function M() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
             children: n.actions.map(function(h) {
-                return t.jsx(N, {
+                return t.jsx(O, {
                     data: h,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
-    function q() {
-        const h = {},
-            g = n.search.length > 0,
-            f = n.filters.length > 0;
-        if (g || f) {
-            const b = {
+    function B() {
+        const h = {
+                backgroundColor: "#f8f8f8",
+                borderBottom: "solid 1px #DDD",
+                marginBottom: 10,
+                padding: 10
+            },
+            f = n.search.length > 0,
+            g = n.filters.length > 0;
+        if (f || g) {
+            const p = {
                 name: "q",
                 value: "",
                 mask: null,
                 type: "text",
                 label: "Palavras-chaves"
             };
-            return t.jsxs(t.Fragment, {
-                children: [t.jsxs(J, {
+            return t.jsxs("div", {
+                style: h,
+                children: [t.jsxs($, {
                     width: 250,
-                    children: [g && t.jsx("div", {
-                        style: h,
-                        children: t.jsx(Q, {
-                            data: b
+                    children: [f && t.jsx("div", {
+                        children: t.jsx(K, {
+                            data: p
                         })
-                    }), f && n.filters.map(function(S) {
-                        return S.type != "hidden" && t.jsx("div", {
-                            style: h,
-                            children: t.jsx(Q, {
-                                data: S
+                    }), g && n.filters.map(function(k) {
+                        return k.type != "hidden" && t.jsx("div", {
+                            children: t.jsx(K, {
+                                data: k
                             })
                         }, Math.random())
                     }), t.jsx("div", {
-                        style: h,
-                        children: t.jsx(A, {
-                            onClick: C,
+                        children: t.jsx(q, {
+                            onClick: S,
                             label: "Filtrar",
-                            default: !0
+                            icon: "filter",
+                            primary: !0
                         })
                     })]
-                }), f && n.filters.map(function(S) {
-                    return S.type == "hidden" && t.jsx("div", {
-                        style: h,
-                        children: t.jsx(Q, {
-                            data: S
+                }), g && n.filters.map(function(k) {
+                    return k.type == "hidden" && t.jsx("div", {
+                        children: t.jsx(K, {
+                            data: k
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function C() {
+    function S() {
         i(!0);
         var h;
-        const g = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? h = e.data.url + "&" + g : h = e.data.url + "?" + g, D("GET", h, function(f) {
-            a(f), i(!1)
+        const f = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
+        e.data.url.indexOf("?") > 0 ? h = e.data.url + "&" + f : h = e.data.url + "?" + f, E("GET", h, function(g) {
+            a(g), i(!1)
         })
     }
 
-    function P() {
+    function F() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [q(), n.bi.map(function(h) {
-                return t.jsx(J, {
+            children: [B(), n.bi.map(function(h) {
+                return t.jsx($, {
                     width: 300,
                     alignItems: "start",
-                    children: h.map(function(g) {
+                    children: h.map(function(f) {
                         return t.jsx("div", {
-                            children: t.jsx(x, {
-                                data: g
+                            children: t.jsx(y, {
+                                data: f
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs(t.Fragment, {
-            children: [T(), l(), q(), u(), y(), I()]
+            children: [M(), o(), B(), u(), x(), D()]
         })
     }
 
-    function p() {
-        window[e.data.id] = () => C();
+    function I() {
+        window[e.data.id] = () => S();
         const h = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable",
             id: e.data.id,
@@ -2627,99 +2669,99 @@
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
-                }), o(), P()]
+                }), d(), F()]
             })
         })
     }
-    return p()
+    return I()
 }
 
-function Z(e) {
+function ee(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
         if (r) {
-            var o = echarts.init(r);
-            o.setOption(e.option)
+            var d = echarts.init(r);
+            d.setOption(e.option)
         } else setTimeout(a, 1e3)
     }
     return setTimeout(a, 1e3), t.jsx("div", {
         id: n,
         style: {
             width: "100%",
             height: 300
         }
     })
 }
 
-function oe(e) {
+function de(e) {
     var n = [
         ["70%", "78%"],
         ["60%", "68%"],
         ["50%", "58%"],
         ["40%", "48%"],
         ["30%", "48%"],
         ["20%", "28%"],
         ["10%", "18%"]
     ];
 
     function a() {
-        return e.headers ? e.headers.slice(1).map(function(o, i) {
+        return e.headers ? e.headers.slice(1).map(function(d, i) {
             return {
-                name: o,
+                name: d,
                 type: "pie",
                 radius: n[i],
                 emphasis: {
                     label: {
                         show: !0,
-                        formatter: function(l) {
-                            return l.value.toLocaleString("pt-BR")
+                        formatter: function(o) {
+                            return o.value.toLocaleString("pt-BR")
                         },
                         fontWeight: "bold"
                     }
                 },
                 roseType: null,
-                data: e.rows.map(function(l) {
+                data: e.rows.map(function(o) {
                     return {
-                        name: l[0],
-                        value: l[i + 1]
+                        name: o[0],
+                        value: o[i + 1]
                     }
                 })
             }
         }) : {
             name: null,
             type: "pie",
             radius: e.donut ? ["25%", "65%"] : ["0%", "75%"],
             emphasis: {
                 label: {
                     show: !0,
-                    formatter: function(o) {
-                        return o.value.toLocaleString("pt-BR")
+                    formatter: function(d) {
+                        return d.value.toLocaleString("pt-BR")
                     },
                     fontWeight: "bold"
                 }
             },
             roseType: e.area ? "area" : null,
-            data: e.rows.map(function(o, i) {
+            data: e.rows.map(function(d, i) {
                 return {
-                    name: o[0],
-                    value: o[1]
+                    name: d[0],
+                    value: d[1]
                 }
             })
         }
     }
 
     function r() {
-        var o = {
+        var d = {
             tooltip: {
                 trigger: "item",
                 formatter: function(i) {
                     return `${i.name}: <b>${i.data.value.toLocaleString("pt-BR")}</b> (${i.percent.toLocaleString("pt-BR")}%)`
                 }
             },
             legend: {},
@@ -2727,91 +2769,91 @@
                 show: !0,
                 formatter(i) {
                     return i.name + " (" + i.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
-        return t.jsx(Z, {
-            option: o
+        return t.jsx(ee, {
+            option: d
         })
     }
     return r()
 }
 
-function ct(e) {
-    return t.jsx(oe, {
+function ut(e) {
+    return t.jsx(de, {
         donut: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function ut(e) {
-    return t.jsx(oe, {
+function ht(e) {
+    return t.jsx(de, {
         area: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function R(e) {
+function _(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
-        o = {
+        d = {
             type: "value"
         },
         i = {
             show: !0,
             feature: {
                 mark: {
                     show: !0
                 },
                 saveAsImage: {
                     show: !0
                 }
             }
         },
-        l = e.area ? {} : null;
+        o = e.area ? {} : null;
 
-    function d() {
+    function s() {
         return e.headers ? {
             type: "category",
             data: e.headers.slice(1)
         } : {
             type: "category",
-            data: e.rows.map(function(s) {
-                return s[0]
+            data: e.rows.map(function(l) {
+                return l[0]
             })
         }
     }
 
     function c() {
-        return e.headers ? e.rows.map(function(s) {
+        return e.headers ? e.rows.map(function(l) {
             return {
-                name: s[0],
-                data: s.slice(1),
+                name: l[0],
+                data: l.slice(1),
                 type: a,
                 stack: r,
-                areaStyle: l
+                areaStyle: o
             }
         }) : [{
             name: null,
-            data: e.rows.map(function(s) {
-                return s[1]
+            data: e.rows.map(function(l) {
+                return l[1]
             }),
             type: a,
             stack: r,
-            areaStyle: l
+            areaStyle: o
         }]
     }
 
     function u() {
-        var s = {
+        var l = {
             toolbox: i,
             tooltip: {
                 trigger: "axis",
                 axisPointer: {
                     type: "shadow"
                 },
                 formatter: function(m) {
@@ -2821,88 +2863,88 @@
             legend: {},
             label: {
                 show: !0,
                 formatter: function(m) {
                     return m.value.toLocaleString("pt-BR")
                 }
             },
-            xAxis: n ? o : d(),
-            yAxis: n ? d() : o,
+            xAxis: n ? d : s(),
+            yAxis: n ? s() : d,
             series: c()
         };
-        return t.jsx(Z, {
-            option: s
+        return t.jsx(ee, {
+            option: l
         })
     }
     return u()
 }
 
-function ht(e) {
-    return t.jsx(R, {
+function mt(e) {
+    return t.jsx(_, {
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function mt(e) {
-    return t.jsx(R, {
+function ft(e) {
+    return t.jsx(_, {
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function ft(e) {
-    return t.jsx(R, {
+function gt(e) {
+    return t.jsx(_, {
         area: !0,
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function gt(e) {
-    return t.jsx(R, {
+function xt(e) {
+    return t.jsx(_, {
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function xt(e) {
-    return t.jsx(R, {
+function yt(e) {
+    return t.jsx(_, {
         invert: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function yt(e) {
-    return t.jsx(R, {
+function pt(e) {
+    return t.jsx(_, {
         invert: !0,
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function pt(e) {
+function vt(e) {
     function n() {
         return e.headers ? [{
             type: "treemap",
             roam: "move",
             nodeClick: !0,
-            data: e.headers.slice(1).map(function(r, o) {
+            data: e.headers.slice(1).map(function(r, d) {
                 return {
                     name: r,
                     type: "pie",
                     children: e.rows.map(function(i) {
                         return {
                             name: i[0],
-                            value: i[o + 1]
+                            value: i[d + 1]
                         }
                     })
                 }
             })
         }] : [{
             type: "treemap",
             roam: "move",
@@ -2920,28 +2962,28 @@
         var r = {
             tooltip: {
                 trigger: "item"
             },
             legend: {},
             label: {
                 show: !0,
-                formatter(o) {
-                    return o.name + " (" + o.value.toLocaleString("pt-BR") + ")"
+                formatter(d) {
+                    return d.name + " (" + d.value.toLocaleString("pt-BR") + ")"
                 }
             },
             series: n()
         };
-        return t.jsx(Z, {
+        return t.jsx(ee, {
             option: r
         })
     }
     return a()
 }
 
-function vt(e) {
+function bt(e) {
     function n() {
         var a = {
             series: [{
                 type: "gauge",
                 startAngle: 0,
                 endAngle: 360,
                 min: 0,
@@ -2975,81 +3017,81 @@
                     }
                 },
                 data: [{
                     value: e.value
                 }]
             }]
         };
-        return t.jsx(Z, {
+        return t.jsx(ee, {
             option: a
         })
     }
     return n()
 }
 
-function he(e) {
+function me(e) {
     function n() {
         switch (e.type) {
             case "pie":
-                return t.jsx(oe, {
+                return t.jsx(de, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "polar":
-                return t.jsx(ut, {
+                return t.jsx(ht, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "donut":
-                return t.jsx(ct, {
+                return t.jsx(ut, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "bar":
-                return t.jsx(ht, {
+                return t.jsx(mt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "stacked_bar":
-                return t.jsx(gt, {
+                return t.jsx(xt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "column":
-                return t.jsx(xt, {
+                return t.jsx(yt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "stacked_column":
-                return t.jsx(yt, {
+                return t.jsx(pt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "tree_map":
-                return t.jsx(pt, {
+                return t.jsx(vt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "line":
-                return t.jsx(mt, {
+                return t.jsx(ft, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "area":
-                return t.jsx(ft, {
+                return t.jsx(gt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "progress":
-                return t.jsx(vt, {
+                return t.jsx(bt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             default:
-                return t.jsx(R, {
+                return t.jsx(_, {
                     headers: e.headers,
                     rows: e.rows
                 })
         }
     }
 
     function a() {
@@ -3063,127 +3105,127 @@
                 children: e.title
             }), n()]
         })
     }
     return a()
 }
 
-function bt(e) {
+function wt(e) {
     function n() {
-        for (var r = [], o = 0; o < e.data.series.length; o++) r.push([e.data.series[o][0], e.data.series[o][1]]);
-        return e.data.chart ? t.jsx(he, {
+        for (var r = [], d = 0; d < e.data.series.length; d++) r.push([e.data.series[d][0], e.data.series[d][1]]);
+        return e.data.chart ? t.jsx(me, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
                 "data-label": w(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%"
                 },
                 children: t.jsx("tbody", {
                     children: r.map(i => t.jsx("tr", {
-                        children: i.map((l, d) => d == 0 ? t.jsx("th", {
+                        children: i.map((o, s) => s == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left"
                             },
-                            children: l
+                            children: o
                         }, Math.random()) : t.jsx("td", {
-                            children: U(l)
+                            children: U(o)
                         }, Math.random()))
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
-        for (var r = [], o = [], i = Object.keys(e.data.series), l = [], d = 0; d < i.length; d++) {
-            d == 0 && r.push("");
-            for (var c = [i[d]], u = 0, s = 0; s < e.data.series[i[d]].length; s++) {
-                var m = e.data.series[i[d]];
-                d == 0 && r.push(m[s][0]), c.push(m[s][1]), u += m[s][1], i.length > 1 && (d == 0 ? l.push(m[s][1]) : l[s] += m[s][1], s > 0 && s == e.data.series[i[d]].length - 1 && (d == 0 ? l.push(u) : l[s + 1] += u))
+        for (var r = [], d = [], i = Object.keys(e.data.series), o = [], s = 0; s < i.length; s++) {
+            s == 0 && r.push("");
+            for (var c = [i[s]], u = 0, l = 0; l < e.data.series[i[s]].length; l++) {
+                var m = e.data.series[i[s]];
+                s == 0 && r.push(m[l][0]), c.push(m[l][1]), u += m[l][1], i.length > 1 && (s == 0 ? o.push(m[l][1]) : o[l] += m[l][1], l > 0 && l == e.data.series[i[s]].length - 1 && (s == 0 ? o.push(u) : o[l + 1] += u))
             }
-            c.length > 2 && (d == 0 && r.push("TOTAL"), c.push(u)), o.push(c)
+            c.length > 2 && (s == 0 && r.push("TOTAL"), c.push(u)), d.push(c)
         }
-        return e.data.chart ? t.jsx(he, {
+        return e.data.chart ? t.jsx(me, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
-            rows: o
+            rows: d
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
                 "data-label": w(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
                     width: "100%"
                 },
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: r.map(y => t.jsx("th", {
-                            children: y
+                        children: r.map(x => t.jsx("th", {
+                            children: x
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [o.map(y => t.jsx("tr", {
-                        children: y.map((v, j) => j == 0 ? t.jsx("th", {
+                    children: [d.map(x => t.jsx("tr", {
+                        children: x.map((v, j) => j == 0 ? t.jsx("th", {
                             children: v
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
                             style: {
-                                backgroundColor: j == y.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
+                                backgroundColor: j == x.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
                             },
                             children: U(v)
                         }, Math.random()))
-                    }, Math.random())), l.length > 0 && t.jsxs("tr", {
+                    }, Math.random())), o.length > 0 && t.jsxs("tr", {
                         children: [t.jsx("th", {
                             children: "TOTAL"
-                        }), l.map(y => t.jsxs("td", {
+                        }), o.map(x => t.jsxs("td", {
                             align: "center",
                             style: {
                                 backgroundColor: "var(--info-color)"
                             },
-                            children: [U(y), " "]
+                            children: [U(x), " "]
                         }, Math.random()))]
                     }, Math.random())]
                 })]
             })]
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
 }
-const Se = {
+const Ce = {
     primary: "#1351b4",
     success: "green",
     warning: "orange",
     info: "blue",
     danger: "red"
 };
 
-function wt(e) {
+function jt(e) {
     function n() {
         const a = {
             width: 30,
             height: 30,
             borderRadius: "50%",
             backgroundColor: e.data.value
         };
         return t.jsx("div", {
             style: a
         })
     }
     return n()
 }
 
-function jt() {
+function kt() {
     function e() {
         const i = {
             width: 150,
             height: 150,
             borderRadius: "50%",
             objectFit: "cover"
         };
@@ -3191,174 +3233,175 @@
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
                     style: i
                 })
             }), t.jsx("div", {
-                children: t.jsx(z, {
+                children: t.jsx(P, {
                     dataLabel: "Editar Perfil",
                     href: "/api/editprofile/",
                     style: {
                         textDecoration: "none"
                     },
                     children: window.application.menu.user
                 })
             })]
         })
     }
 
     function n(i) {
-        var l = i.target;
-        const d = l.querySelector(":scope > ul, :scope > li");
-        if (d) {
-            d.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(s) {
-                s.style.display = "block"
-            }) : l.querySelectorAll(":scope > ul, :scope > li").forEach(function(s) {
-                s.style.display = "none"
+        var o = i.target;
+        const s = o.querySelector(":scope > ul, :scope > li");
+        if (s) {
+            s.offsetParent === null ? o.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(l) {
+                l.style.display = "block"
+            }) : o.querySelectorAll(":scope > ul, :scope > li").forEach(function(l) {
+                l.style.display = "none"
             });
-            const c = l.querySelector(":scope > i.fa-solid.fa-chevron-right"),
-                u = l.querySelector(":scope > i.fa-solid.fa-chevron-up");
+            const c = o.querySelector(":scope > i.fa-solid.fa-chevron-right"),
+                u = o.querySelector(":scope > i.fa-solid.fa-chevron-up");
             return c && (c.classList.remove("fa-chevron-right"), c.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), i.preventDefault(), i.stopPropagation(), i.cancelBubble = !0, !1
         } else {
             const c = document.querySelector("aside");
             c.style.display = window.innerWidth < 800 ? "none" : "block"
         }
     }
 
-    function a(i, l) {
-        const d = {
-                display: l == 0 ? "block" : "none",
+    function a(i, o) {
+        const s = {
+                display: o == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 5,
                 paddingTop: 10,
                 paddingBottom: 10,
-                lineHeight: "2rem"
+                lineHeight: "2rem",
+                color: "#1351b4"
             },
             c = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return i.url ? t.jsx("li", {
-            style: d,
+            style: s,
             onClick: n,
-            children: t.jsxs(z, {
+            children: t.jsxs(P, {
                 href: i.url,
                 dataLabel: w(i.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [l == 0 && t.jsx(k, {
+                children: [o == 0 && t.jsx(b, {
                     icon: i.icon || "dot-circle",
                     style: c
                 }), i.label]
             })
         }, Math.random()) : i.items.length > 0 && t.jsxs("li", {
             onClick: n,
-            style: d,
+            style: s,
             "data-label": w(i.label),
-            children: [l == 0 && t.jsx(k, {
+            children: [o == 0 && t.jsx(b, {
                 icon: i.icon || "dot-circle",
                 style: c
-            }), i.label, t.jsx(k, {
+            }), i.label, t.jsx(b, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
                     display: "none",
                     paddingLeft: 15
                 },
                 children: i.items.map(function(u) {
-                    return a(u, l + 1)
+                    return a(u, o + 1)
                 })
             })]
         }, Math.random())
     }
 
     function r() {
         const i = {
             padding: 0
         };
         return window.application.menu.items.length > 0 && t.jsx("ul", {
             style: i,
-            children: window.application.menu.items.map(function(l) {
-                return a(l, 0)
+            children: window.application.menu.items.map(function(o) {
+                return a(o, 0)
             })
         })
     }
 
-    function o() {
+    function d() {
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
-    return o()
+    return d()
 }
 
-function kt(e) {
+function St(e) {
     var n;
 
     function a(i) {
-        const l = "=".repeat((4 - i.length % 4) % 4),
-            d = (i + l).replace(/\-/g, "+").replace(/_/g, "/"),
-            c = window.atob(d),
+        const o = "=".repeat((4 - i.length % 4) % 4),
+            s = (i + o).replace(/\-/g, "+").replace(/_/g, "/"),
+            c = window.atob(s),
             u = new Uint8Array(c.length);
-        for (let s = 0; s < c.length; ++s) u[s] = c.charCodeAt(s);
+        for (let l = 0; l < c.length; ++l) u[l] = c.charCodeAt(l);
         return u
     }
 
     function r() {
         "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(i) {
             if (i) {
-                const l = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
+                const o = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
                 i.pushManager.subscribe({
                     userVisibleOnly: !0,
-                    applicationServerKey: l
-                }).then(function(d) {
-                    if (console.log(d), n = JSON.stringify(d), console.log(n), d) {
+                    applicationServerKey: o
+                }).then(function(s) {
+                    if (console.log(s), n = JSON.stringify(s), console.log(n), s) {
                         alert("Notificação ativada com sucesso.");
                         var c = new FormData;
-                        c.append("subscription", n), D("POST", "/api/pushsubscribe/", function(u) {
+                        c.append("subscription", n), E("POST", "/api/pushsubscribe/", function(u) {
                             console.log(u)
                         }, c)
                     } else {
                         alert("Problema ao ativar notificações.");
                         return
                     }
-                }).catch(function(d) {
-                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", d)
+                }).catch(function(s) {
+                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", s)
                 })
             } else console.log("No registered service worker.")
         }).catch(function(i) {
             alert("Erro"), console.error("Service Worker Error", i)
         }) : alert("Push messaging is not supported")
     }
 
-    function o() {
-        return t.jsx(k, {
+    function d() {
+        return t.jsx(b, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer"
             }
         })
     }
-    return o()
+    return d()
 }
 
-function St(e) {
+function Ct(e) {
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
@@ -3376,96 +3419,96 @@
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 80
                 },
                 onClick: () => history.back(),
-                children: t.jsx(k, {
+                children: t.jsx(b, {
                     icon: "arrow-left",
                     style: r
                 })
             }), t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 20
                 },
                 onClick: () => window.scrollTo(0, 0),
-                children: t.jsx(k, {
+                children: t.jsx(b, {
                     icon: "arrow-up",
                     style: r
                 })
             })]
         })
     }
     return n()
 }
 
-function Ct(e) {
-    const [n, a] = M.useState(e.data);
-    window.loaddata = o => a(o);
+function Mt(e) {
+    const [n, a] = C.useState(e.data);
+    window.loaddata = d => a(d);
 
     function r() {
-        const o = {
+        const d = {
             minHeight: 400,
             margin: 20
         };
         return t.jsx("div", {
-            style: o,
+            style: d,
             id: "container",
-            children: t.jsx(x, {
+            children: t.jsx(y, {
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
-function Mt(e) {
-    M.useEffect(() => {
-        const u = localStorage.getItem("message");
-        u && (localStorage.removeItem("message"), K(u)), window.addEventListener("resize", () => {
-            const s = document.querySelector("aside");
-            s.style.display = window.innerWidth < 800 ? "none" : "block"
+function Tt(e) {
+    C.useEffect(() => {
+        const l = localStorage.getItem("message");
+        l && (localStorage.removeItem("message"), Z(l)), window.addEventListener("resize", () => {
+            const m = document.querySelector("aside");
+            m.style.display = window.innerWidth < 800 ? "none" : "block"
         })
     }, []);
 
     function a() {
-        const u = document.querySelector("aside");
-        u.style.display = u.style.display == "none" ? "block" : "none"
+        const l = document.querySelector("aside");
+        l.style.display = l.style.display == "none" ? "block" : "none"
     }
 
-    function r(u) {
-        u.preventDefault(), window.load(u.target.href)
+    function r(l) {
+        l.preventDefault(), window.load(l.target.href)
     }
 
-    function o() {
-        const u = {
+    function d() {
+        const l = {
                 display: "flex",
                 width: "100%",
                 justifyContent: "space-between",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 overflowX: "hidden"
             },
-            s = {
+            m = {
                 choices: "/api/search/",
                 help_text: null,
                 label: null,
                 mask: null,
                 name: "search",
                 required: !1,
                 type: "choice"
             };
         return e.data.navbar ? t.jsxs("div", {
-            style: u,
+            style: l,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [t.jsx(k, {
+                children: [t.jsx(b, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
@@ -3486,62 +3529,62 @@
                     display: "flex",
                     alignItems: "center"
                 },
                 children: [e.data.navbar.adder.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(X, {
+                    children: t.jsx(Q, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(k, {
+                        children: t.jsx(b, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(kt, {})
+                    children: t.jsx(St, {})
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(X, {
+                    children: t.jsx(Q, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(k, {
+                        children: t.jsx(b, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(X, {
+                    children: t.jsx(Q, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
-                        children: t.jsx(k, {
+                        children: t.jsx(b, {
                             icon: "gear"
                         })
                     })
-                }), window.innerWidth > 800 && t.jsx(ke, {
-                    data: s,
+                }), window.innerWidth > 800 && t.jsx(Se, {
+                    data: m,
                     style: {
                         padding: 10
                     },
-                    onSelect: m => document.location.href = F(m.id)
+                    onSelect: x => document.location.href = H(x.id)
                 }), e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(X, {
+                    children: t.jsx(Q, {
                         actions: e.data.navbar.usermenu,
                         position: {},
                         dataLabel: w(e.data.navbar.user),
                         children: e.data.navbar.user
                     })
                 })]
             })]
@@ -3552,72 +3595,88 @@
         return window.application.menu && t.jsx("aside", {
             style: {
                 flexGrow: 2,
                 maxWidth: "350px",
                 minWidth: "350px",
                 display: window.innerWidth < 800 ? "none" : "block"
             },
-            children: t.jsx(jt, {})
+            children: t.jsx(kt, {})
         })
     }
 
-    function l() {
+    function o() {
+        const l = {
+                margin: 15
+            },
+            m = {
+                color: "#1351b4"
+            };
+        return e.data.navbar && t.jsxs("div", {
+            style: l,
+            children: [t.jsx(b, {
+                icon: "home",
+                style: m
+            }), " Área Administrativa"]
+        })
+    }
+
+    function s() {
         return t.jsxs("main", {
             style: {
                 flexGrow: 6,
                 minWidth: "400px"
             },
-            children: [t.jsx(Ct, {
+            children: [o(), t.jsx(Mt, {
                 data: e.data.content
             }), t.jsx("footer", {
-                children: d()
-            }), t.jsx(St, {})]
+                children: c()
+            }), t.jsx(Ct, {})]
         })
     }
 
-    function d() {
+    function c() {
         return e.data.footer ? t.jsxs("div", {
             align: "center",
             children: [t.jsx("div", {
                 children: "Todos os direitos reservados"
             }), t.jsx("div", {
                 children: e.data.footer.version
             })]
         }) : null
     }
 
-    function c() {
+    function u() {
         return t.jsxs("div", {
             children: [t.jsx("header", {
-                children: o()
+                children: d()
             }), t.jsxs("div", {
                 style: {
                     overflowX: "hide",
                     width: "100%",
                     display: "flex",
                     overflow: "hidden",
                     minHeight: window.innerHeight - 70
                 },
-                children: [i(), l()]
+                children: [i(), s()]
             })]
         })
     }
-    return c()
+    return u()
 }
 
-function Tt(e) {
+function Et(e) {
     return t.jsx("img", {
         src: e.data.src,
         style: {
             width: "100%"
         }
     })
 }
 
-function Et(e) {
+function Dt(e) {
     const n = {
         width: "100%",
         textAlign: "center"
     };
     return t.jsx("div", {
         style: n,
         children: t.jsx("img", {
@@ -3627,39 +3686,39 @@
                 height: e.data.height,
                 borderRadius: e.data.round ? "50%" : 0
             }
         })
     })
 }
 
-function Dt(e) {
+function It(e) {
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
 
-function It(e) {
+function qt(e) {
     function n(i) {
-        return e.data.icon ? i.done ? t.jsx(k, {
+        return e.data.icon ? i.done ? t.jsx(b, {
             style: {
-                marginTop: 12
+                marginTop: 6
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
             style: {
-                marginTop: 12
+                marginTop: 6
             },
             children: i.number
         })
     }
 
     function a(i) {
         return {
@@ -3680,103 +3739,103 @@
             listStyleType: "none",
             display: "flex",
             justifyContent: "center",
             minWidth: i.length * 100
         }
     }
 
-    function o() {
+    function d() {
         const i = {
                 width: "100%",
                 margin: "auto",
                 overflowX: "auto",
                 "&::WebkitScrollbar": {
                     width: 0
                 }
             },
-            l = {
+            o = {
                 width: 100,
                 marginWidth: 100,
                 textAlign: "center"
             },
-            d = {
+            s = {
                 position: "relative",
                 borderBottom: "2px solid #1151b3",
                 top: -28,
                 width: 45,
                 left: 77
             };
         return t.jsx("div", {
             children: t.jsx("div", {
                 style: i,
                 children: t.jsx("ul", {
                     style: r(e.data.steps),
                     children: e.data.steps.map((c, u) => t.jsxs("li", {
-                        style: l,
+                        style: o,
                         children: [t.jsx("div", {
                             style: a(c),
                             children: n(c)
                         }), u < e.data.steps.length - 1 && t.jsx("div", {
-                            style: d
+                            style: s
                         }), t.jsx("div", {
                             children: c.name
                         })]
                     }, Math.random()))
                 })
             })
         })
     }
-    return o()
+    return d()
 }
 
-function qt(e) {
+function Bt(e) {
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
-            o = {
+            d = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
-                backgroundColor: Se[e.data.style]
+                backgroundColor: Ce[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
-                style: o,
+                style: d,
                 children: t.jsxs("span", {
                     style: r,
                     children: [e.data.value, "%"]
                 })
             })
         })
     }
     return n()
 }
 
 function At(e) {
     function n() {
-        return e.data.color = Se[e.data.style], t.jsx(Ce, {
+        return e.data.color = Ce[e.data.style], t.jsx(Me, {
             data: e.data
         })
     }
     return n()
 }
 
-function Ce(e) {
+function Me(e) {
     function n() {
         const a = {
             color: "white",
             width: "fit-content",
             borderRadius: 5,
             textWrap: "nowrap",
             padding: 10,
@@ -3793,28 +3852,29 @@
 
 function Lt(e) {
     function n() {
         const a = {
                 padding: 20,
                 marginLeft: -20,
                 marginRight: -20,
-                textAlign: "center"
+                textAlign: "center",
+                backgroundColor: "#f8f8f8"
             },
             r = {
                 padding: 20,
                 display: "inline-flex",
                 flexDirection: "column",
                 width: 250,
                 height: 250,
                 backgroundColor: "white",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
-            o = {
+            d = {
                 marginTop: 30,
                 fontSize: "3rem",
                 color: "#2670e8"
             },
             i = {
                 marginTop: 40,
                 fontWeight: "bold",
@@ -3825,35 +3885,35 @@
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
                 "data-label": w(e.data.title),
                 children: e.data.title
             }), t.jsx("div", {
-                children: e.data.items.map(l => t.jsxs(z, {
-                    href: l.url,
+                children: e.data.items.map(o => t.jsxs(P, {
+                    href: o.url,
                     style: r,
-                    dataLabel: l.label,
+                    dataLabel: o.label,
                     children: [t.jsx("div", {
-                        children: t.jsx(k, {
-                            style: o,
-                            icon: l.icon
+                        children: t.jsx(b, {
+                            style: d,
+                            icon: o.icon
                         })
                     }), t.jsx("div", {
                         style: i,
-                        children: l.label
+                        children: o.label
                     })]
                 }, Math.random()))
             })]
         }) : null
     }
     return n()
 }
 
-function Bt(e) {
+function Nt(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 backgroundColor: "black",
                 color: "white",
                 padding: "10px",
                 minHeight: "300px",
@@ -3865,46 +3925,46 @@
                 children: a
             }, Math.random()))
         })
     }
     return n()
 }
 
-function Nt(e) {
+function Ot(e) {
     function n() {
-        return e.data.url ? t.jsx(z, {
+        return e.data.url ? t.jsx(P, {
             href: e.data.url,
             imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(k, {
+            children: e.data.icon ? t.jsx(b, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
 }
 
-function Ot(e) {
+function Rt(e) {
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
 
-function Rt(e) {
+function _t(e) {
     const n = Math.random();
-    M.useEffect(() => {
+    C.useEffect(() => {
         new QRCode(document.getElementById(n), {
             text: e.data.text,
             width: 128,
             height: 128,
             colorDark: "#333333",
             colorLight: "#ffffff",
             correctLevel: QRCode.CorrectLevel.H
@@ -3915,29 +3975,29 @@
         return t.jsx("div", {
             id: n
         })
     }
     return a()
 }
 
-function _t(e) {
+function Ft(e) {
     function n() {
-        return t.jsx(J, {
+        return t.jsx($, {
             width: 400,
             children: e.data.items.map((a, r) => t.jsx("div", {
-                children: t.jsx(x, {
+                children: t.jsx(y, {
                     data: a
                 })
             }, Math.random()))
         })
     }
     return n()
 }
 
-function Ft(e) {
+function zt(e) {
     function n() {
         return t.jsxs("div", {
             children: [t.jsx("h2", {
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     fontSize: "12rem",
@@ -3946,133 +4006,133 @@
                 },
                 children: e.data.value
             })]
         })
     }
     return n()
 }
-var re, Me = {};
-const zt = "/api/application/",
-    me = localStorage.getItem("application");
+var ie, Te = {};
+const Ht = "/api/application/",
+    fe = localStorage.getItem("application");
 
-function x(e) {
-    const n = Me[e.data.type];
+function y(e) {
+    const n = Te[e.data.type];
     return n ? n(e.data) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
-x.register = function(e, n) {
-    Me[e] = n
+y.register = function(e, n) {
+    Te[e] = n
 };
-x.render = function(e) {
-    re = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/login/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
+y.render = function(e) {
+    ie = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/login/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-x.register("counter", e => t.jsx(Ft, {
+y.register("counter", e => t.jsx(zt, {
     data: e
 }));
-x.register("form", e => t.jsx(dt, {
+y.register("form", e => t.jsx(dt, {
     data: e
 }));
-x.register("queryset", e => t.jsx(st, {
+y.register("queryset", e => t.jsx(ct, {
     data: e
 }));
-x.register("fieldset", e => t.jsx(He, {
+y.register("fieldset", e => t.jsx(He, {
     data: e
 }));
-x.register("field", e => t.jsx($, {
+y.register("field", e => t.jsx(J, {
     data: e
 }));
-x.register("object", e => t.jsx(Ge, {
+y.register("object", e => t.jsx(Ge, {
     data: e
 }));
-x.register("section", e => t.jsx(Ue, {
+y.register("section", e => t.jsx(Ue, {
     data: e
 }));
-x.register("group", e => t.jsx(Je, {
+y.register("group", e => t.jsx($e, {
     data: e
 }));
-x.register("statistics", e => t.jsx(bt, {
+y.register("statistics", e => t.jsx(wt, {
     data: e
 }));
-x.register("image", e => t.jsx(Et, {
+y.register("image", e => t.jsx(Dt, {
     data: e
 }));
-x.register("banner", e => t.jsx(Tt, {
+y.register("banner", e => t.jsx(Et, {
     data: e
 }));
-x.register("map", e => t.jsx(Dt, {
+y.register("map", e => t.jsx(It, {
     data: e
 }));
-x.register("steps", e => t.jsx(It, {
+y.register("steps", e => t.jsx(qt, {
     data: e
 }));
-x.register("qrcode", e => t.jsx(Rt, {
+y.register("qrcode", e => t.jsx(_t, {
     data: e
 }));
-x.register("badge", e => t.jsx(Ce, {
+y.register("badge", e => t.jsx(Me, {
     data: e
 }));
-x.register("status", e => t.jsx(At, {
+y.register("status", e => t.jsx(At, {
     data: e
 }));
-x.register("progress", e => t.jsx(qt, {
+y.register("progress", e => t.jsx(Bt, {
     data: e
 }));
-x.register("color", e => t.jsx(wt, {
+y.register("color", e => t.jsx(jt, {
     data: e
 }));
-x.register("boxes", e => t.jsx(Lt, {
+y.register("boxes", e => t.jsx(Lt, {
     data: e
 }));
-x.register("shell", e => t.jsx(Bt, {
+y.register("shell", e => t.jsx(Nt, {
     data: e
 }));
-x.register("file_link", e => t.jsx(Nt, {
+y.register("file_link", e => t.jsx(Ot, {
     data: e
 }));
-x.register("file_viewer", e => t.jsx(Ot, {
+y.register("file_viewer", e => t.jsx(Rt, {
     data: e
 }));
-x.register("response", e => t.jsx(Le, {
+y.register("response", e => t.jsx(Ae, {
     data: e
 }));
-x.register("application", e => t.jsx(Mt, {
+y.register("application", e => t.jsx(Tt, {
     data: e
 }));
-x.register("iconset", e => t.jsx(De, {
+y.register("iconset", e => t.jsx(De, {
     data: e
 }));
-x.register("grid", e => t.jsx(_t, {
+y.register("grid", e => t.jsx(Ft, {
     data: e
 }));
-x.register("rows", e => t.jsx(Fe, {
+y.register("rows", e => t.jsx(Fe, {
     data: e
 }));
-x.register("timeline", e => t.jsx(ze, {
+y.register("timeline", e => t.jsx(ze, {
     data: e
 }));
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), me ? (window.application = JSON.parse(me), D("GET", B(e), function(n) {
-        window.application.content = n, re.render(t.jsx(x, {
+    }, "", e), fe ? (window.application = JSON.parse(fe), E("GET", L(e), function(n) {
+        window.application.content = n, ie.render(t.jsx(y, {
             data: window.application
         }, Math.random()))
-    })) : D("GET", zt, function(a) {
-        window.application = a, localStorage.setItem("application", JSON.stringify(window.application)), D("GET", B(e), function(r) {
-            window.application.content = r, re.render(t.jsx(x, {
+    })) : E("GET", Ht, function(a) {
+        window.application = a, localStorage.setItem("application", JSON.stringify(window.application)), E("GET", L(e), function(r) {
+            window.application.content = r, ie.render(t.jsx(y, {
                 data: window.application
             }, Math.random()))
         })
     })
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
-    }, "", e), D("GET", B(e), function(n) {
+    }, "", e), E("GET", L(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-x.render(H.createRoot(document.getElementById("root")));
+y.render(W.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.2.1/slth/static/js/peerjs.min.js` & `pyslth-0.2.2/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/js/qrcode.min.js` & `pyslth-0.2.2/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/js/react-trigger-change.js` & `pyslth-0.2.2/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/js/react.min.js` & `pyslth-0.2.2/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/js/vanilla-masker.js` & `pyslth-0.2.2/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/static/js/vanilla-masker.min.js` & `pyslth-0.2.2/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/statistics.py` & `pyslth-0.2.2/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/templates/index.html` & `pyslth-0.2.2/slth/templates/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html lang="pt">
 
 <head>
   <meta charset="UTF-8" />
-  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
   <title>{{ application.version }} {{ application.title }}</title>
   <link rel="stylesheet" href="/static/css/slth.css">
   <link rel="stylesheet" href="/static/css/fontawesome.min.css">
   <link rel="stylesheet" href="/static/css/solid.min.css">
   <script type="module" src="/static/js/vanilla-masker.min.js"></script>
   <script type="module" src="/static/js/react-trigger-change.js"></script>
   <!-- <script type="module" src="/static/js/qrcode.min.js"></script> -->
```

### Comparing `pyslth-0.2.1/slth/templates/service-worker.js` & `pyslth-0.2.2/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/tests.py` & `pyslth-0.2.2/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/urls.py` & `pyslth-0.2.2/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/utils.py` & `pyslth-0.2.2/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.1/slth/views.py` & `pyslth-0.2.2/slth/views.py`

 * *Files identical despite different names*

