# Comparing `tmp/django-ausleihe-0.2.1.tar.gz` & `tmp/django_ausleihe-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ausleihe-0.2.1.tar", last modified: Mon Mar  4 09:27:11 2024, max compression
+gzip compressed data, was "django_ausleihe-0.2.2.tar", last modified: Tue Apr 30 15:01:51 2024, max compression
```

## Comparing `django-ausleihe-0.2.1.tar` & `django_ausleihe-0.2.2.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.935477 django-ausleihe-0.2.1/
--rw-r--r--   0 u001439  (1517772900) 1422596844     1075 2022-11-14 09:45:36.000000 django-ausleihe-0.2.1/LICENSE
--rw-r--r--   0 u001439  (1517772900) 1422596844      184 2022-11-14 09:46:40.000000 django-ausleihe-0.2.1/MANIFEST.in
--rw-r--r--   0 u001439  (1517772900) 1422596844     1577 2024-03-04 09:27:11.935010 django-ausleihe-0.2.1/PKG-INFO
--rw-r--r--   0 u001439  (1517772900) 1422596844      723 2022-10-23 11:43:30.000000 django-ausleihe-0.2.1/README.md
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.890004 django-ausleihe-0.2.1/ausleihe/
--rw-r--r--   0 u001439  (1517772900) 1422596844        0 2022-10-22 21:33:17.000000 django-ausleihe-0.2.1/ausleihe/__init__.py
--rw-r--r--   0 u001439  (1517772900) 1422596844     1410 2022-11-16 06:45:42.000000 django-ausleihe-0.2.1/ausleihe/admin.py
--rw-r--r--   0 u001439  (1517772900) 1422596844      148 2022-10-22 21:33:17.000000 django-ausleihe-0.2.1/ausleihe/apps.py
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.893028 django-ausleihe-0.2.1/ausleihe/migrations/
--rw-r--r--   0 u001439  (1517772900) 1422596844     2639 2022-10-24 10:10:16.000000 django-ausleihe-0.2.1/ausleihe/migrations/0001_initial.py
--rw-r--r--   0 u001439  (1517772900) 1422596844     1427 2022-11-07 19:12:39.000000 django-ausleihe-0.2.1/ausleihe/migrations/0002_leihe.py
--rw-r--r--   0 u001439  (1517772900) 1422596844      766 2022-11-18 17:02:02.000000 django-ausleihe-0.2.1/ausleihe/migrations/0003_alter_orderings.py
--rw-r--r--   0 u001439  (1517772900) 1422596844      428 2022-11-18 17:02:52.000000 django-ausleihe-0.2.1/ausleihe/migrations/0004_alter_leihe_zurueckgebracht.py
--rw-r--r--   0 u001439  (1517772900) 1422596844        0 2022-10-22 21:33:17.000000 django-ausleihe-0.2.1/ausleihe/migrations/__init__.py
--rw-r--r--   0 u001439  (1517772900) 1422596844     4099 2022-11-24 16:27:26.000000 django-ausleihe-0.2.1/ausleihe/models.py
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.880624 django-ausleihe-0.2.1/ausleihe/static/
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.881055 django-ausleihe-0.2.1/ausleihe/static/ausleihe/
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.897510 django-ausleihe-0.2.1/ausleihe/static/ausleihe/js/
--rw-r--r--   0 u001439  (1517772900) 1422596844      388 2022-11-01 22:11:04.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/js/enter_next.js
--rw-r--r--   0 u001439  (1517772900) 1422596844      493 2024-01-02 12:27:18.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/js/helpers.js
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.881684 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.901204 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/
--rw-r--r--   0 u001439  (1517772900) 1422596844    16338 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap2.css
--rw-r--r--   0 u001439  (1517772900) 1422596844     8715 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap3.css
--rw-r--r--   0 u001439  (1517772900) 1422596844     9307 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap4.css
--rw-r--r--   0 u001439  (1517772900) 1422596844     9368 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap5.css
--rw-r--r--   0 u001439  (1517772900) 1422596844     8133 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.css
--rw-r--r--   0 u001439  (1517772900) 1422596844     8781 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.default.css
--rw-r--r--   0 u001439  (1517772900) 1422596844    11940 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.legacy.css
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.902319 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/
--rw-r--r--   0 u001439  (1517772900) 1422596844   118016 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/selectize.js
--rw-r--r--   0 u001439  (1517772900) 1422596844    66927 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/selectize.min.js
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.903912 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/standalone/
--rw-r--r--   0 u001439  (1517772900) 1422596844   118029 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/standalone/selectize.js
--rw-r--r--   0 u001439  (1517772900) 1422596844    66344 2022-10-02 16:01:15.000000 django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/standalone/selectize.min.js
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.882684 django-ausleihe-0.2.1/ausleihe/templates/
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.931022 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/
--rw-r--r--   0 u001439  (1517772900) 1422596844      595 2022-10-29 16:12:53.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_create.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     2835 2022-10-30 20:20:53.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_detail.html
--rw-r--r--   0 u001439  (1517772900) 1422596844      665 2022-10-30 13:30:39.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_edit.html
--rw-r--r--   0 u001439  (1517772900) 1422596844      599 2022-10-29 16:33:10.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_form.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1472 2024-01-02 12:12:22.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_list.html
--rw-r--r--   0 u001439  (1517772900) 1422596844       73 2022-10-22 21:53:30.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/base.html
--rw-r--r--   0 u001439  (1517772900) 1422596844      332 2022-10-30 13:48:13.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_autoren_links.html
--rw-r--r--   0 u001439  (1517772900) 1422596844      160 2022-10-31 17:52:26.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_common_css.html
--rw-r--r--   0 u001439  (1517772900) 1422596844      364 2022-10-31 17:50:47.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_common_js.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1112 2022-10-31 14:21:39.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_create.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     2806 2022-10-30 21:28:01.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_detail.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1059 2022-10-31 13:41:20.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_edit.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     3992 2022-11-01 22:12:56.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_form.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     2739 2024-01-02 12:38:17.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_list.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     2634 2022-11-14 18:43:48.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/home.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     2983 2022-11-14 19:12:11.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/leihe_list.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1475 2022-11-14 19:09:40.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/leihe_user_detail.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     2206 2022-11-14 09:14:12.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/leihe_user_suche.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1599 2022-11-13 17:07:47.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/medium_detail.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1046 2022-11-26 15:32:17.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/profil_unvollstaendig.html
--rw-r--r--   0 u001439  (1517772900) 1422596844      839 2022-10-30 13:12:31.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verlag_create.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     2732 2022-10-30 20:19:55.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verlag_detail.html
--rw-r--r--   0 u001439  (1517772900) 1422596844      727 2022-10-30 13:32:15.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verlag_edit.html
--rw-r--r--   0 u001439  (1517772900) 1422596844      364 2022-10-30 13:12:21.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verlag_form.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1455 2024-01-02 12:11:57.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verlag_list.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     6826 2024-02-25 14:31:32.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verleihen.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1903 2022-11-14 19:09:06.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verliehen_aktuell_table.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1033 2022-11-14 18:33:33.000000 django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verliehen_historisch_table.html
--rw-r--r--   0 u001439  (1517772900) 1422596844     1733 2022-11-15 18:03:11.000000 django-ausleihe-0.2.1/ausleihe/urls.py
--rw-r--r--   0 u001439  (1517772900) 1422596844    12694 2024-02-24 18:26:59.000000 django-ausleihe-0.2.1/ausleihe/views.py
-drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-03-04 09:27:11.934430 django-ausleihe-0.2.1/django_ausleihe.egg-info/
--rw-r--r--   0 u001439  (1517772900) 1422596844     1577 2024-03-04 09:27:11.000000 django-ausleihe-0.2.1/django_ausleihe.egg-info/PKG-INFO
--rw-r--r--   0 u001439  (1517772900) 1422596844     2593 2024-03-04 09:27:11.000000 django-ausleihe-0.2.1/django_ausleihe.egg-info/SOURCES.txt
--rw-r--r--   0 u001439  (1517772900) 1422596844        1 2024-03-04 09:27:11.000000 django-ausleihe-0.2.1/django_ausleihe.egg-info/dependency_links.txt
--rw-r--r--   0 u001439  (1517772900) 1422596844       60 2024-03-04 09:27:11.000000 django-ausleihe-0.2.1/django_ausleihe.egg-info/requires.txt
--rw-r--r--   0 u001439  (1517772900) 1422596844        9 2024-03-04 09:27:11.000000 django-ausleihe-0.2.1/django_ausleihe.egg-info/top_level.txt
--rw-r--r--   0 u001439  (1517772900) 1422596844       38 2024-03-04 09:27:11.935545 django-ausleihe-0.2.1/setup.cfg
--rw-r--r--   0 u001439  (1517772900) 1422596844     1266 2024-03-04 09:24:47.000000 django-ausleihe-0.2.1/setup.py
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.828967 django_ausleihe-0.2.2/
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1075 2022-11-14 09:45:36.000000 django_ausleihe-0.2.2/LICENSE
+-rw-r--r--   0 u001439  (1517772900) 1422596844      184 2022-11-14 09:46:40.000000 django_ausleihe-0.2.2/MANIFEST.in
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1577 2024-04-30 15:01:51.828429 django_ausleihe-0.2.2/PKG-INFO
+-rw-r--r--   0 u001439  (1517772900) 1422596844      723 2022-10-23 11:43:30.000000 django_ausleihe-0.2.2/README.md
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.683755 django_ausleihe-0.2.2/ausleihe/
+-rw-r--r--   0 u001439  (1517772900) 1422596844        0 2022-10-22 21:33:17.000000 django_ausleihe-0.2.2/ausleihe/__init__.py
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1410 2022-11-16 06:45:42.000000 django_ausleihe-0.2.2/ausleihe/admin.py
+-rw-r--r--   0 u001439  (1517772900) 1422596844      148 2022-10-22 21:33:17.000000 django_ausleihe-0.2.2/ausleihe/apps.py
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.691048 django_ausleihe-0.2.2/ausleihe/migrations/
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2639 2022-10-24 10:10:16.000000 django_ausleihe-0.2.2/ausleihe/migrations/0001_initial.py
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1427 2022-11-07 19:12:39.000000 django_ausleihe-0.2.2/ausleihe/migrations/0002_leihe.py
+-rw-r--r--   0 u001439  (1517772900) 1422596844      766 2022-11-18 17:02:02.000000 django_ausleihe-0.2.2/ausleihe/migrations/0003_alter_orderings.py
+-rw-r--r--   0 u001439  (1517772900) 1422596844      428 2022-11-18 17:02:52.000000 django_ausleihe-0.2.2/ausleihe/migrations/0004_alter_leihe_zurueckgebracht.py
+-rw-r--r--   0 u001439  (1517772900) 1422596844        0 2022-10-22 21:33:17.000000 django_ausleihe-0.2.2/ausleihe/migrations/__init__.py
+-rw-r--r--   0 u001439  (1517772900) 1422596844     4099 2022-11-24 16:27:26.000000 django_ausleihe-0.2.2/ausleihe/models.py
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.660372 django_ausleihe-0.2.2/ausleihe/static/
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.660912 django_ausleihe-0.2.2/ausleihe/static/ausleihe/
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.694129 django_ausleihe-0.2.2/ausleihe/static/ausleihe/js/
+-rw-r--r--   0 u001439  (1517772900) 1422596844      388 2022-11-01 22:11:04.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/js/enter_next.js
+-rw-r--r--   0 u001439  (1517772900) 1422596844      493 2024-01-02 12:27:18.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/js/helpers.js
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.661431 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.710982 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/
+-rw-r--r--   0 u001439  (1517772900) 1422596844    16338 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap2.css
+-rw-r--r--   0 u001439  (1517772900) 1422596844     8715 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap3.css
+-rw-r--r--   0 u001439  (1517772900) 1422596844     9307 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap4.css
+-rw-r--r--   0 u001439  (1517772900) 1422596844     9368 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap5.css
+-rw-r--r--   0 u001439  (1517772900) 1422596844     8133 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.css
+-rw-r--r--   0 u001439  (1517772900) 1422596844     8781 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.default.css
+-rw-r--r--   0 u001439  (1517772900) 1422596844    11940 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.legacy.css
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.728010 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/
+-rw-r--r--   0 u001439  (1517772900) 1422596844   118016 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/selectize.js
+-rw-r--r--   0 u001439  (1517772900) 1422596844    66927 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/selectize.min.js
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.745312 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/standalone/
+-rw-r--r--   0 u001439  (1517772900) 1422596844   118029 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/standalone/selectize.js
+-rw-r--r--   0 u001439  (1517772900) 1422596844    66344 2022-10-02 16:01:15.000000 django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/standalone/selectize.min.js
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.662299 django_ausleihe-0.2.2/ausleihe/templates/
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.824625 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/
+-rw-r--r--   0 u001439  (1517772900) 1422596844      595 2022-10-29 16:12:53.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_create.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2835 2022-10-30 20:20:53.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_detail.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      665 2022-10-30 13:30:39.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_edit.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      599 2022-10-29 16:33:10.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_form.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1472 2024-04-28 16:02:17.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_list.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844       73 2022-10-22 21:53:30.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/base.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      332 2022-10-30 13:48:13.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_autoren_links.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      160 2022-10-31 17:52:26.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_common_css.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      364 2022-10-31 17:50:47.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_common_js.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1112 2022-10-31 14:21:39.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_create.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2806 2022-10-30 21:28:01.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_detail.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1059 2022-10-31 13:41:20.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_edit.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     3992 2022-11-01 22:12:56.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_form.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2739 2024-04-28 16:01:58.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_list.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2615 2024-04-28 16:12:07.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/home.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1080 2024-04-28 16:00:59.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/leihe_list.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      982 2024-04-28 16:38:57.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/leihe_list_normal_table.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2349 2024-04-28 14:55:55.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/leihe_list_staff_table.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2586 2024-04-30 09:27:45.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/leihe_user_detail.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2214 2024-04-28 16:15:54.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/leihe_user_suche.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1599 2022-11-13 17:07:47.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/medium_detail.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1046 2022-11-26 15:32:17.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/profil_unvollstaendig.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      839 2022-10-30 13:12:31.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_create.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2732 2022-10-30 20:19:55.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_detail.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      727 2022-10-30 13:32:15.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_edit.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844      364 2022-10-30 13:12:21.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_form.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1455 2024-04-28 16:02:36.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_list.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     6834 2024-04-28 16:14:17.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verleihen.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2041 2024-04-28 16:37:49.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verliehen_aktuell_table.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1176 2024-04-28 16:37:38.000000 django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verliehen_historisch_table.html
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1733 2022-11-15 18:03:11.000000 django_ausleihe-0.2.2/ausleihe/urls.py
+-rw-r--r--   0 u001439  (1517772900) 1422596844    12933 2024-04-29 14:44:06.000000 django_ausleihe-0.2.2/ausleihe/views.py
+drwxr-xr-x   0 u001439  (1517772900) 1422596844        0 2024-04-30 15:01:51.827736 django_ausleihe-0.2.2/django_ausleihe.egg-info/
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1577 2024-04-30 15:01:51.000000 django_ausleihe-0.2.2/django_ausleihe.egg-info/PKG-INFO
+-rw-r--r--   0 u001439  (1517772900) 1422596844     2706 2024-04-30 15:01:51.000000 django_ausleihe-0.2.2/django_ausleihe.egg-info/SOURCES.txt
+-rw-r--r--   0 u001439  (1517772900) 1422596844        1 2024-04-30 15:01:51.000000 django_ausleihe-0.2.2/django_ausleihe.egg-info/dependency_links.txt
+-rw-r--r--   0 u001439  (1517772900) 1422596844       60 2024-04-30 15:01:51.000000 django_ausleihe-0.2.2/django_ausleihe.egg-info/requires.txt
+-rw-r--r--   0 u001439  (1517772900) 1422596844        9 2024-04-30 15:01:51.000000 django_ausleihe-0.2.2/django_ausleihe.egg-info/top_level.txt
+-rw-r--r--   0 u001439  (1517772900) 1422596844       38 2024-04-30 15:01:51.829052 django_ausleihe-0.2.2/setup.cfg
+-rw-r--r--   0 u001439  (1517772900) 1422596844     1266 2024-04-30 15:01:34.000000 django_ausleihe-0.2.2/setup.py
```

### Comparing `django-ausleihe-0.2.1/LICENSE` & `django_ausleihe-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/PKG-INFO` & `django_ausleihe-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ausleihe
-Version: 0.2.1
+Version: 0.2.2
 Summary: Django-App für die Ausleihe von Medien.
 Home-page: https://github.com/hutchison/django-ausleihe
 Author: Martin Darmüntzel
 Author-email: martin@trivialanalog.de
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-ausleihe-0.2.1/README.md` & `django_ausleihe-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/admin.py` & `django_ausleihe-0.2.2/ausleihe/admin.py`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/migrations/0001_initial.py` & `django_ausleihe-0.2.2/ausleihe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/migrations/0002_leihe.py` & `django_ausleihe-0.2.2/ausleihe/migrations/0002_leihe.py`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/migrations/0003_alter_orderings.py` & `django_ausleihe-0.2.2/ausleihe/migrations/0003_alter_orderings.py`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/models.py` & `django_ausleihe-0.2.2/ausleihe/models.py`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap2.css` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap2.css`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap3.css` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap4.css` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap5.css` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.css` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.css`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.default.css` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.default.css`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/css/selectize.legacy.css` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/css/selectize.legacy.css`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/selectize.js` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/selectize.js`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/selectize.min.js` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/selectize.min.js`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/standalone/selectize.js` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/standalone/selectize.js`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/static/ausleihe/selectize/js/standalone/selectize.min.js` & `django_ausleihe-0.2.2/ausleihe/static/ausleihe/selectize/js/standalone/selectize.min.js`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_create.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_create.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_detail.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_detail.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_edit.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_edit.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_form.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_form.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/autor_list.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/autor_list.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% extends "ausleihe/base.html" %}
 
 {% block content %}
 <div class="container">
   <nav aria-label="breadcrumb">
     <ol class="breadcrumb">
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:home' %}">Start</a></li>
-      <li class="breadcrumb-item" aria-current="page">{{ object_list.count }} <a href="{% url 'ausleihe:autor-list' %}"><strong>Autoren</strong></a></li>
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:buch-list' %}">Bücher</a></li>
+      <li class="breadcrumb-item" aria-current="page">{{ object_list.count }} <a href="{% url 'ausleihe:autor-list' %}"><strong>Autoren</strong></a></li>
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verlag-list' %}">Verlage</a></li>
       {% if perms.ausleihe.add_autor %}
       <li class="breadcrumb-item active" aria-current="page"><a href="{% url 'ausleihe:autor-create' %}">hinzufügen</a></li>
       {% endif %}
     </ol>
   </nav>
   <div class="row">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends "ausleihe/base.html" %} {% block content %}
    1. _S_t_a_r_t
-   2. {{ object_list.count }} _AA_uu_tt_oo_rr_ee_nn
-   3. _B_Ã_¼_c_h_e_r
+   2. _B_Ã_¼_c_h_e_r
+   3. {{ object_list.count }} _AA_uu_tt_oo_rr_ee_nn
    4. _V_e_r_l_a_g_e
    5. {% if perms.ausleihe.add_autor %}
    6. _h_i_n_z_u_f_Ã_¼_g_e_n
    7. {% endif %}
 {% if object_list %}
 IIDD             NNaammee
 {{ autor.id }} _{_{_ _a_u_t_o_r_._v_o_r_n_a_m_e_ _}_}_ _{_{_ _a_u_t_o_r_._n_a_c_h_n_a_m_e_ _}_}
```

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_create.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_create.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_detail.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_detail.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_edit.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_edit.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_form.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_form.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/buch_list.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/buch_list.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 {% endblock js %}
 
 {% block content %}
 <div class="container">
   <nav aria-label="breadcrumb">
     <ol class="breadcrumb">
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:home' %}">Start</a></li>
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:autor-list' %}">Autoren</a></li>
       <li class="breadcrumb-item" aria-current="page">{{ object_list.count }} <a href="{% url 'ausleihe:buch-list' %}"><strong>Bücher</strong></a></li>
+      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:autor-list' %}">Autoren</a></li>
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verlag-list' %}">Verlage</a></li>
       {% if perms.ausleihe.add_buch %}
       <li class="breadcrumb-item active" aria-current="page"><a href="{% url 'ausleihe:buch-create' %}">hinzufügen</a></li>
       {% endif %}
     </ol>
   </nav>
   <div class="row">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends "ausleihe/base.html" %} {% load static %} {% block js %}
 {% endblock js %} {% block content %}
    1. _S_t_a_r_t
-   2. _A_u_t_o_r_e_n
-   3. {{ object_list.count }} _BB_?Ã_?¼_cc_hh_ee_rr
+   2. {{ object_list.count }} _BB_?Ã_?¼_cc_hh_ee_rr
+   3. _A_u_t_o_r_e_n
    4. _V_e_r_l_a_g_e
    5. {% if perms.ausleihe.add_buch %}
    6. _h_i_n_z_u_f_Ã_¼_g_e_n
    7. {% endif %}
 {% if object_list %}[Unknown INPUT type]
 MMeeddiiaatthheekknnrr.. TTiitteell      AAuuttoorreenn                  IISSBBNN      VVeerrllaagg      AAuussggaabbee
                                                            {% if
```

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/home.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/leihe_list_staff_table.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,66 @@
-{% extends "ausleihe/base.html" %}
-
-{% block content %}
-<div class="container">
-  <nav aria-label="breadcrumb">
-    <ol class="breadcrumb">
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:home' %}">Start</a></li>
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:buch-list' %}">Bücher</a></li>
-      {% if perms.ausleihe.add_leihe %}
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verleihen' %}">verleihen</a></li>
-      {% endif %}
-      {% if perms.ausleihe.view_leihe %}
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verliehen' %}">verliehen</a></li>
-      {% endif %}
-    </ol>
-  </nav>
-</div>
-
-<div class="container">
+<div class="{% if object_list %}container-fluid{% else %}container{% endif %}">
   <div class="row">
     <div class="col">
-      {% if aktuell_verliehen %}
-      <h4>aktuell entliehen</h4>
+      {% if object_list %}
       <table class="table">
         <thead>
           <tr>
-            <th>Mediatheknr.</th>
-            <th>enthält</th>
+            <th>#</th>
+            <th>dazugehörige Medien</th>
+            <th>Nutzer</th>
             <th>Anfang</th>
             <th>Ende</th>
             <th>Δ</th>
+            <th>verliehen von</th>
+            {% if perms.ausleihe.change_leihe %}
+            <th>zurücknehmen</th>
+            {% endif %}
           </tr>
         </thead>
         <tbody>
-          {% for leihe in aktuell_verliehen %}
+          {% for leihe in object_list %}
           <tr>
             <td>
               <a href="{% url 'ausleihe:medium-detail' leihe.medium.id %}">{{ leihe.medium }}</a>
             </td>
             <td>
               {% if leihe.medium.buecher.exists %}
-              {% for buch in leihe.medium.buecher.all %}
-              {% if forloop.last %}
-              <a href="{% url 'ausleihe:buch-detail' buch.id %}">📘 {{ buch }}</a>
-              {% else %}
-              <a href="{% url 'ausleihe:buch-detail' buch.id %}">📘 {{ buch }}</a>, 
-              {% endif %}
-              {% endfor %}
+              📚 {{ leihe.medium.buecher.all|join:", " }}
               {% endif %}
             </td>
-            <td>{{ leihe.anfang }}</td>
-            <td>{{ leihe.ende|date:"l" }}, {{ leihe.ende }}</td>
             <td>
+              {% if perms.ausleihe.view_leihe %}
+              <a href="{% url 'ausleihe:verliehen-an' %}?username={{ leihe.nutzer.user }}">{{ leihe.nutzer }} ({{ leihe.nutzer.user }})</a>
+              {% else %}
+              {{ leihe.nutzer }} ({{ leihe.nutzer.user }})
+              {% endif %}
+            </td>
+            <td class="text-right">{{ leihe.anfang|date:"d.m.Y" }}</td>
+            <td class="text-right">{{ leihe.ende|date:"l" }}, {{ leihe.ende|date:"d.m.Y" }}</td>
+            <td class="text-right">
               {% if leihe.ist_ueberfaellig %}
               {% with leihe.differenz_heute as d %}
-              {{ d }} Tag{% if d != 1 %}e{% endif %} überfällig
+              <span class="text-danger">{{ d }}&thinsp;d überfällig</span>
               {% endwith %}
               {% else %}
               {% with leihe.differenz_heute as d %}
-              noch {{ d }} Tag{% if d != 1 %}e{% endif %}
+                noch {{ d }}&thinsp;d
               {% endwith %}
               {% endif %}
             </td>
+            <td>{{ leihe.verleiht_von.get_full_name }} ({{ leihe.verleiht_von }})</td>
+            {% if perms.ausleihe.change_leihe %}
+            <td>
+              <a class="btn btn-primary btn-sm" href="{% url 'ausleihe:zuruecknehmen' leihe.id %}">zurücknehmen</a>
+            </td>
+            {% endif %}
           </tr>
           {% endfor %}
         </tbody>
       </table>
       {% else %}
-      <p>Aktuell nichts entliehen.</p>
+      <p>Aktuell ist nichts verliehen.</p>
       {% endif %}
     </div>
   </div>
 </div>
-
-<div class="container">
-  <div class="row">
-    <div class="col">
-      {% include "ausleihe/verliehen_historisch_table.html" %}
-    </div>
-  </div>
-</div>
-{% endblock content %}
```

#### html2text {}

```diff
@@ -1,30 +1,17 @@
-{% extends "ausleihe/base.html" %} {% block content %}
-   1. _S_t_a_r_t
-   2. _B_Ã_¼_c_h_e_r
-   3. {% if perms.ausleihe.add_leihe %}
-   4. _v_e_r_l_e_i_h_e_n
-   5. {% endif %} {% if perms.ausleihe.view_leihe %}
-   6. _v_e_r_l_i_e_h_e_n
-   7. {% endif %}
-{% if aktuell_verliehen %}
-****** aakkttuueellll eennttlliieehheenn ******
-MMeeddiiaatthheekknnrr.. eenntthh?Ã?¤lltt                    AAnnffaanngg       EEnnddee             ?Î?
-                                                                       {% if
-                                                                       leihe.ist_ueberfaellig
-                                                                       %} {% with
-             {% if                                                     leihe.differenz_heute
-             leihe.medium.buecher.exists              {                as d %} {{ d }} Tag{%
-_{            %} {% for buch in           {            {                if d != 1 %}e{% endif
-_{            leihe.medium.buecher.all %} {            leihe.ende|date: %} Ã¼berfÃ¤llig {%
-_l_e_i_h_e_._m_e_d_i_u_m {% if forloop.last %} _ð____  leihe.anfang "l" }}, {        endwith %} {% else %}
-_}_}           _{_{_ _b_u_c_h_ _}_} {% else %} _ð____  }}           { leihe.ende }}  {% with
-             _{_{_ _b_u_c_h_ _}_}, {% endif %} {%                                leihe.differenz_heute
-             endfor %} {% endif %}                                     as d %} noch {{ d }}
-                                                                       Tag{% if d != 1 %}e{%
-                                                                       endif %} {% endwith %}
-                                                                       {% endif %}
+{% if object_list %}
+##            ddaazzuuggeehh?Ã?¶rriiggee MMeeddiieenn           NNuuttzzeerr                    AAnnffaanngg             EEnnddee             ?Î?                     vveerrlliieehheenn vvoonn                    zzuurr?Ã?¼cckknneehhmmeenn
+                                                                                                          {% if
+                                                                                                          leihe.ist_ueberfaellig
+                                            {% if                                        {                %} {% with
+             {% if                          perms.ausleihe.view_leihe                    {                leihe.differenz_heute
+_{            leihe.medium.buecher.exists %} %} _{_{_ _l_e_i_h_e_._n_u_t_z_e_r_ _}_}_ _(_{  {                  leihe.ende|date: as d %} {{ d }} d      {
+_{            ð {                         _{_ _l_e_i_h_e_._n_u_t_z_e_r_._u_s_e_r_ _}_}_)   {                  "l" }}, {        Ã¼berfÃ¤llig {%        {                                _z_u_r_Ã_¼_c_k_n_e_h_m_e_n
+_l_e_i_h_e_._m_e_d_i_u_m {                              {% else %} {              leihe.anfang|date: {                endwith %} {% else %}  leihe.verleiht_von.get_full_name
+_}_}           leihe.medium.buecher.all|join: { leihe.nutzer }} ({      "d.m.Y" }}         leihe.ende|date: {% with                }} ({{ leihe.verleiht_von }})
+             ", " }} {% endif %}            { leihe.nutzer.user }})                      "d.m.Y" }}       leihe.differenz_heute
+                                            {% endif %}                                                   as d %} noch {{ d }} d
+                                                                                                          {% endwith %} {% endif
+                                                                                                          %}
 {% else %}
-Aktuell nichts entliehen.
+Aktuell ist nichts verliehen.
 {% endif %}
-{% include "ausleihe/verliehen_historisch_table.html" %}
-{% endblock content %}
```

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/leihe_list.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verliehen_aktuell_table.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,63 @@
-{% extends "ausleihe/base.html" %}
-
-{% block content %}
-<div class="container">
-  <nav aria-label="breadcrumb">
-    <ol class="breadcrumb">
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:home' %}">Start</a></li>
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:buch-list' %}">Bücher</a></li>
-      {% if perms.ausleihe.add_leihe %}
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verleihen' %}">verleihen</a></li>
+{% if aktuell_verliehen.exists %}
+<h4>aktuell entliehen</h4>
+<table class="table">
+  <thead>
+    <tr>
+      <th class="col-1">Mediatheknr.</th>
+      <th class="col-4">enthält</th>
+      <th class="text-right col-1">Anfang</th>
+      <th class="text-right col-2">Ende</th>
+      <th>Δ</th>
+      {% if perms.ausleihe.view_leihe %}
+      <th>verliehen von</th>
+      {% endif %}
+      {% if perms.ausleihe.change_leihe %}
+      <th>zurücknehmen</th>
       {% endif %}
+    </tr>
+  </thead>
+  <tbody>
+    {% for leihe in aktuell_verliehen %}
+    <tr>
+      <td>
+        <a href="{% url 'ausleihe:medium-detail' leihe.medium.id %}">{{ leihe.medium }}</a>
+      </td>
+      <td>
+        {% if leihe.medium.buecher.exists %}
+        {% for buch in leihe.medium.buecher.all %}
+        {% if forloop.last %}
+        <a href="{% url 'ausleihe:buch-detail' buch.id %}">📚 {{ buch }}</a>
+        {% else %}
+        <a href="{% url 'ausleihe:buch-detail' buch.id %}">📚 {{ buch }}</a>, 
+        {% endif %}
+        {% endfor %}
+        {% endif %}
+      </td>
+      <td class="text-right">{{ leihe.anfang|date:"d.m.Y" }}</td>
+      <td class="text-right">{{ leihe.ende|date:"l" }}, {{ leihe.ende|date:"d.m.Y" }}</td>
+      <td>
+        {% if leihe.ist_ueberfaellig %}
+        {% with leihe.differenz_heute as d %}
+        <span class="text-danger">{{ d }}&thinsp;d überfällig</span>
+        {% endwith %}
+        {% else %}
+        {% with leihe.differenz_heute as d %}
+        noch {{ d }}&thinsp;d
+        {% endwith %}
+        {% endif %}
+      </td>
       {% if perms.ausleihe.view_leihe %}
-      <li class="breadcrumb-item active" aria-current="page"><a href="{% url 'ausleihe:verliehen' %}"><strong>verliehen</strong></a></li>
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verliehen-an-suche' %}">nach Nutzer suchen</a></li>
+      <td>{{ leihe.verleiht_von.get_full_name }} ({{ leihe.verleiht_von }})</td>
       {% endif %}
-    </ol>
-  </nav>
-</div>
-<div class="{% if object_list %}container-fluid{% else %}container{% endif %}">
-  <div class="row">
-    <div class="col">
-      {% if object_list %}
-      <table class="table">
-        <thead>
-          <tr>
-            <th>Mediatheknr.</th>
-            <th>Nutzer</th>
-            <th>Anfang</th>
-            <th>Ende</th>
-            <th>Δ</th>
-            <th>verliehen von</th>
-            {% if perms.ausleihe.change_leihe %}
-            <th>zurücknehmen</th>
-            {% endif %}
-          </tr>
-        </thead>
-        <tbody>
-          {% for leihe in object_list %}
-          <tr>
-            <td>
-              <a href="{% url 'ausleihe:medium-detail' leihe.medium.id %}">{{ leihe.medium }}</a>
-            </td>
-            <td>
-              {% if perms.ausleihe.view_leihe %}
-              <a href="{% url 'ausleihe:verliehen-an' %}?username={{ leihe.nutzer.user }}">{{ leihe.nutzer }} ({{ leihe.nutzer.user }})</a>
-              {% else %}
-              {{ leihe.nutzer }} ({{ leihe.nutzer.user }})
-              {% endif %}
-            </td>
-            <td>{{ leihe.anfang }}</td>
-            <td>{{ leihe.ende|date:"l" }}, {{ leihe.ende }}</td>
-            <td>
-              {% if leihe.ist_ueberfaellig %}
-              {% with leihe.differenz_heute as d %}
-                {{ d }} Tag{% if d != 1 %}e{% endif %} überfällig
-              {% endwith %}
-              {% else %}
-              {% with leihe.differenz_heute as d %}
-                noch {{ d }} Tag{% if d != 1 %}e{% endif %}
-              {% endwith %}
-              {% endif %}
-            </td>
-            <td>{{ leihe.verleiht_von.get_full_name }} ({{ leihe.verleiht_von }})</td>
-            {% if perms.ausleihe.change_leihe %}
-            <td>
-              <a class="btn btn-primary btn-sm" href="{% url 'ausleihe:zuruecknehmen' leihe.id %}">zurücknehmen</a>
-            </td>
-            {% endif %}
-          </tr>
-          {% endfor %}
-        </tbody>
-      </table>
-      {% else %}
-      <p>Aktuell ist nichts verliehen.</p>
+      {% if perms.ausleihe.change_leihe %}
+      <td>
+        <a class="btn btn-primary btn-sm" href="{% url 'ausleihe:zuruecknehmen' leihe.id %}{% if username %}?username={{ username }}{% endif %}">zurücknehmen</a>
+      </td>
       {% endif %}
-    </div>
-  </div>
-</div>
-{% endblock content %}
+    </tr>
+    {% endfor %}
+  </tbody>
+</table>
+{% else %}
+<p>Aktuell nichts entliehen.</p>
+{% endif %}
```

#### html2text {}

```diff
@@ -1,29 +1,18 @@
-{% extends "ausleihe/base.html" %} {% block content %}
-   1. _S_t_a_r_t
-   2. _B_Ã_¼_c_h_e_r
-   3. {% if perms.ausleihe.add_leihe %}
-   4. _v_e_r_l_e_i_h_e_n
-   5. {% endif %} {% if perms.ausleihe.view_leihe %}
-   6. _vv_ee_rr_ll_ii_ee_hh_ee_nn
-   7. _n_a_c_h_ _N_u_t_z_e_r_ _s_u_c_h_e_n
-   8. {% endif %}
-{% if object_list %}
-MMeeddiiaatthheekknnrr.. NNuuttzzeerr                    AAnnffaanngg       EEnnddee             ?Î?                     vveerrlliieehheenn vvoonn                    zzuurr?Ã?¼cckknneehhmmeenn
-                                                                     {% if
-                                                                     leihe.ist_ueberfaellig
-                                                                     %} {% with
-             {% if                                                   leihe.differenz_heute
-             perms.ausleihe.view_leihe              {                as d %} {{ d }} Tag{%
-_{            %} _{_{_ _l_e_i_h_e_._n_u_t_z_e_r_ _}_}_ _(_{  {            {                if d != 1 %}e{% endif  {
-_{            _{_ _l_e_i_h_e_._n_u_t_z_e_r_._u_s_e_r_ _}_}_)   {            leihe.ende|date: %} Ã¼berfÃ¤llig {%     {                                _z_u_r_Ã_¼_c_k_n_e_h_m_e_n
-_l_e_i_h_e_._m_e_d_i_u_m {% else %} {              leihe.anfang "l" }}, {        endwith %} {% else %}  leihe.verleiht_von.get_full_name
-_}_}           { leihe.nutzer }} ({      }}           { leihe.ende }}  {% with                }} ({{ leihe.verleiht_von }})
-             { leihe.nutzer.user }})                                 leihe.differenz_heute
-             {% endif %}                                             as d %} noch {{ d }}
-                                                                     Tag{% if d != 1 %}e{%
-                                                                     endif %} {% endwith %}
-                                                                     {% endif %}
+{% if aktuell_verliehen.exists %}
+****** aakkttuueellll eennttlliieehheenn ******
+MMeeddiiaatthheekknnrr.. eenntthh?Ã?¤lltt                    AAnnffaanngg             EEnnddee             ?Î?                     vveerrlliieehheenn vvoonn                    zzuurr?Ã?¼cckknneehhmmeenn
+                                                                             {% if
+                                                                             leihe.ist_ueberfaellig
+             {% if                                          {                %} {% with
+             leihe.medium.buecher.exists                    {                leihe.differenz_heute
+_{            %} {% for buch in           {                  leihe.ende|date: as d %} {{ d }} d      {
+_{            leihe.medium.buecher.all %} {                  "l" }}, {        Ã¼berfÃ¤llig {%        {                                _z_u_r_Ã_¼_c_k_n_e_h_m_e_n
+_l_e_i_h_e_._m_e_d_i_u_m {% if forloop.last %} _ð____  leihe.anfang|date: {                endwith %} {% else %}  leihe.verleiht_von.get_full_name
+_}_}           _{_{_ _b_u_c_h_ _}_} {% else %} _ð____  "d.m.Y" }}         leihe.ende|date: {% with                }} ({{ leihe.verleiht_von }})
+             _{_{_ _b_u_c_h_ _}_}, {% endif %} {%                     "d.m.Y" }}       leihe.differenz_heute
+             endfor %} {% endif %}                                           as d %} noch {{ d }} d
+                                                                             {% endwith %} {% endif
+                                                                             %}
 {% else %}
-Aktuell ist nichts verliehen.
+Aktuell nichts entliehen.
 {% endif %}
-{% endblock content %}
```

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/leihe_user_detail.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_list.html`

 * *Files 22% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 
 {% block content %}
 <div class="container">
   <nav aria-label="breadcrumb">
     <ol class="breadcrumb">
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:home' %}">Start</a></li>
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:buch-list' %}">Bücher</a></li>
-      {% if perms.ausleihe.add_leihe %}
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verleihen' %}">verleihen</a></li>
-      {% endif %}
-      {% if perms.ausleihe.view_leihe %}
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verliehen' %}">verliehen</a></li>
-      <li class="breadcrumb-item active" aria-current="page"><a href="{% url 'ausleihe:verliehen-an-suche' %}"><strong>nach Nutzer suchen</strong></a></li>
+      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:autor-list' %}">Autoren</a></li>
+      <li class="breadcrumb-item" aria-current="page">{{ object_list.count }} <a href="{% url 'ausleihe:verlag-list' %}"><strong>Verlage</strong></a></li>
+      {% if perms.ausleihe.add_verlag %}
+      <li class="breadcrumb-item active" aria-current="page"><a href="{% url 'ausleihe:verlag-create' %}">hinzufügen</a></li>
       {% endif %}
     </ol>
   </nav>
-  <h3>{{ nutzer }} ({{ nutzer.user }})</h3>
-</div>
-
-<div class="{% if perms.ausleihe.view_leihe and aktuell_verliehen %}container-fluid{% else %}container{% endif %}">
-  <div class="row">
-    <div class="col">
-      {% include "ausleihe/verliehen_aktuell_table.html" with username=nutzer.user %}
-    </div>
-  </div>
-</div>
-
-<div class="{% if perms.ausleihe.view_leihe and historisch_verliehen %}container-fluid{% else %}container{% endif %}">
   <div class="row">
     <div class="col">
-      {% include "ausleihe/verliehen_historisch_table.html" %}
+      {% if object_list %}
+      <table class="table">
+        <thead>
+          <tr>
+            <th>ID</th>
+            <th>Name</th>
+          </tr>
+        </thead>
+        <tbody>
+          {% for verlag in object_list %}
+          <tr>
+            <td>{{ verlag.id }}</td>
+            <td><a href="{% url 'ausleihe:verlag-detail' verlag.id %}">{{ verlag.name }}</a></td>
+          </tr>
+          {% endfor %}
+        </tbody>
+      </table>
+      {% else %}
+      <p>Bisher sind keine Verlage vorhanden.</p>
+      {% endif %}
     </div>
   </div>
 </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 {% extends "ausleihe/base.html" %} {% block content %}
    1. _S_t_a_r_t
    2. _B_Ã_¼_c_h_e_r
-   3. {% if perms.ausleihe.add_leihe %}
-   4. _v_e_r_l_e_i_h_e_n
-   5. {% endif %} {% if perms.ausleihe.view_leihe %}
-   6. _v_e_r_l_i_e_h_e_n
-   7. _nn_aa_cc_hh_ _NN_uu_tt_zz_ee_rr_ _ss_uu_cc_hh_ee_nn
-   8. {% endif %}
-******** {{{{ nnuuttzzeerr }}}} (({{{{ nnuuttzzeerr..uusseerr }}}})) ********
-{% include "ausleihe/verliehen_aktuell_table.html" with username=nutzer.user %}
-{% include "ausleihe/verliehen_historisch_table.html" %}
+   3. _A_u_t_o_r_e_n
+   4. {{ object_list.count }} _VV_ee_rr_ll_aa_gg_ee
+   5. {% if perms.ausleihe.add_verlag %}
+   6. _h_i_n_z_u_f_Ã_¼_g_e_n
+   7. {% endif %}
+{% if object_list %}
+IIDD              NNaammee
+{{ verlag.id }} _{_{_ _v_e_r_l_a_g_._n_a_m_e_ _}_}
+{% else %}
+Bisher sind keine Verlage vorhanden.
+{% endif %}
 {% endblock content %}
```

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/leihe_user_suche.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/leihe_user_suche.html`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
 {% block content %}
 <div class="container">
   <nav aria-label="breadcrumb">
     <ol class="breadcrumb">
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:home' %}">Start</a></li>
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:buch-list' %}">Bücher</a></li>
+      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verliehen' %}">aktuell verliehen</a></li>
       {% if perms.ausleihe.add_leihe %}
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verleihen' %}">verleihen</a></li>
       {% endif %}
       {% if perms.ausleihe.view_leihe %}
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verliehen' %}">verliehen</a></li>
       <li class="breadcrumb-item active" aria-current="page"><a href="{% url 'ausleihe:verliehen-an-suche' %}"><strong>nach Nutzer suchen</strong></a></li>
       {% endif %}
     </ol>
   </nav>
 </div>
 <div class="container">
   <div class="row">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 {% extends "ausleihe/base.html" %} {% load static sekizai_tags %} {% block css
 %} {% addtoblock "css" %}
 {% endaddtoblock %} {% endblock css %} {% block js %} {% addtoblock "js" %}
 {% endaddtoblock %} {% endblock %} {% block content %}
    1. _S_t_a_r_t
    2. _B_Ã_¼_c_h_e_r
-   3. {% if perms.ausleihe.add_leihe %}
-   4. _v_e_r_l_e_i_h_e_n
-   5. {% endif %} {% if perms.ausleihe.view_leihe %}
-   6. _v_e_r_l_i_e_h_e_n
+   3. _a_k_t_u_e_l_l_ _v_e_r_l_i_e_h_e_n
+   4. {% if perms.ausleihe.add_leihe %}
+   5. _v_e_r_l_e_i_h_e_n
+   6. {% endif %} {% if perms.ausleihe.view_leihe %}
    7. _nn_aa_cc_hh_ _NN_uu_tt_zz_ee_rr_ _ss_uu_cc_hh_ee_nn
    8. {% endif %}
 {% for n in nutzer %}
 {{ n }} ({{ n.user }})
 {% endfor %}
 AuswÃ¤hlen
 {% endblock content %}
```

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/medium_detail.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/medium_detail.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/profil_unvollstaendig.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/profil_unvollstaendig.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verlag_create.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_create.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verlag_detail.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verlag_edit.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verlag_edit.html`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verleihen.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verleihen.html`

 * *Files 1% similar despite different names*

```diff
@@ -85,19 +85,19 @@
 
 {% block content %}
 <div class="container">
   <nav aria-label="breadcrumb">
     <ol class="breadcrumb">
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:home' %}">Start</a></li>
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:buch-list' %}">Bücher</a></li>
+      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verliehen' %}">aktuell verliehen</a></li>
       {% if perms.ausleihe.add_leihe %}
       <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verleihen' %}"><strong>verleihen</strong></a></li>
       {% endif %}
       {% if perms.ausleihe.view_leihe %}
-      <li class="breadcrumb-item" aria-current="page"><a href="{% url 'ausleihe:verliehen' %}">verliehen</a></li>
       <li class="breadcrumb-item active" aria-current="page"><a href="{% url 'ausleihe:verliehen-an-suche' %}">nach Nutzer suchen</a></li>
       {% endif %}
     </ol>
   </nav>
 
   {% if errors.aktuell_ausgeliehen %}
   <div class="alert alert-danger" role="alert">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 {% extends "ausleihe/base.html" %} {% load static sekizai_tags %} {% block css
 %} {% addtoblock "css" %}
 {% endaddtoblock %} {% endblock css %} {% block js %} {% addtoblock "js" %}
 {% endaddtoblock %} {% endblock %} {% block content %}
    1. _S_t_a_r_t
    2. _B_Ã_¼_c_h_e_r
-   3. {% if perms.ausleihe.add_leihe %}
-   4. _vv_ee_rr_ll_ee_ii_hh_ee_nn
-   5. {% endif %} {% if perms.ausleihe.view_leihe %}
-   6. _v_e_r_l_i_e_h_e_n
+   3. _a_k_t_u_e_l_l_ _v_e_r_l_i_e_h_e_n
+   4. {% if perms.ausleihe.add_leihe %}
+   5. _vv_ee_rr_ll_ee_ii_hh_ee_nn
+   6. {% endif %} {% if perms.ausleihe.view_leihe %}
    7. _n_a_c_h_ _N_u_t_z_e_r_ _s_u_c_h_e_n
    8. {% endif %}
 {% if errors.aktuell_ausgeliehen %}
 Verleih nicht mÃ¶glich: das Medium ist aktuell ausgeliehen.
 {% endif %} {% if verleih_erfolgreich %}
 Bis zum {{ verliehen_bis }} an {{ verliehen_an }} verliehen.
 {% endif %}
```

### Comparing `django-ausleihe-0.2.1/ausleihe/templates/ausleihe/verliehen_historisch_table.html` & `django_ausleihe-0.2.2/ausleihe/templates/ausleihe/verliehen_historisch_table.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 {% if historisch_verliehen %}
 <h4>bisher entliehen</h4>
 <table class="table">
   <thead>
     <tr>
-      <th>Mediatheknr.</th>
-      <th>enthält</th>
-      <th>Anfang</th>
-      <th>Ende</th>
-      <th>Dauer</th>
+      <th class="col-1">Mediatheknr.</th>
+      <th class="col-4">enthält</th>
+      <th class="text-right col-1">Anfang</th>
+      <th class="text-right col-2">Ende</th>
+      <th>Δ</th>
     </tr>
   </thead>
   <tbody>
     {% for leihe in historisch_verliehen %}
     <tr>
       <td>
         <a href="{% url 'ausleihe:medium-detail' leihe.medium.id %}">{{ leihe.medium }}</a>
       </td>
       <td>
         {% if leihe.medium.buecher.exists %}
         {% for buch in leihe.medium.buecher.all %}
         {% if forloop.last %}
-        <a href="{% url 'ausleihe:buch-detail' buch.id %}">📘 {{ buch }}</a>
+        <a href="{% url 'ausleihe:buch-detail' buch.id %}">📚 {{ buch }}</a>
         {% else %}
-        <a href="{% url 'ausleihe:buch-detail' buch.id %}">📘 {{ buch }}</a>, 
+        <a href="{% url 'ausleihe:buch-detail' buch.id %}">📚 {{ buch }}</a>, 
         {% endif %}
         {% endfor %}
         {% endif %}
       </td>
-      <td>{{ leihe.anfang }}</td>
-      <td>{{ leihe.ende|date:"l" }}, {{ leihe.ende }}</td>
-      <td>{{ leihe.dauer }} Tage</td>
+      <td class="text-right">{{ leihe.anfang|date:"d.m.Y" }}</td>
+      <td class="text-right">{{ leihe.ende|date:"l" }}, {{ leihe.ende|date:"d.m.Y" }}</td>
+      <td>{{ leihe.dauer }}&thinsp;d</td>
     </tr>
     {% endfor %}
   </tbody>
 </table>
 {% else %}
 <p>Bisher nichts entliehen.</p>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% if historisch_verliehen %}
 ****** bbiisshheerr eennttlliieehheenn ******
-MMeeddiiaatthheekknnrr.. eenntthh?Ã?¤lltt                    AAnnffaanngg       EEnnddee             DDaauueerr
-             {% if
-             leihe.medium.buecher.exists              {
-_{            %} {% for buch in           {            {                {
-_{            leihe.medium.buecher.all %} {            leihe.ende|date: {
-_l_e_i_h_e_._m_e_d_i_u_m {% if forloop.last %} _ð____  leihe.anfang "l" }}, {        leihe.dauer
-_}_}           _{_{_ _b_u_c_h_ _}_} {% else %} _ð____  }}           { leihe.ende }}  }} Tage
-             _{_{_ _b_u_c_h_ _}_}, {% endif %} {%
+MMeeddiiaatthheekknnrr.. eenntthh?Ã?¤lltt                    AAnnffaanngg             EEnnddee             ?Î?
+             {% if                                          {
+             leihe.medium.buecher.exists                    {
+_{            %} {% for buch in           {                  leihe.ende|date: {
+_{            leihe.medium.buecher.all %} {                  "l" }}, {        {
+_l_e_i_h_e_._m_e_d_i_u_m {% if forloop.last %} _ð____  leihe.anfang|date: {                leihe.dauer
+_}_}           _{_{_ _b_u_c_h_ _}_} {% else %} _ð____  "d.m.Y" }}         leihe.ende|date: }} d
+             _{_{_ _b_u_c_h_ _}_}, {% endif %} {%                     "d.m.Y" }}
              endfor %} {% endif %}
 {% else %}
 Bisher nichts entliehen.
 {% endif %}
```

### Comparing `django-ausleihe-0.2.1/ausleihe/urls.py` & `django_ausleihe-0.2.2/ausleihe/urls.py`

 * *Files identical despite different names*

### Comparing `django-ausleihe-0.2.1/ausleihe/views.py` & `django_ausleihe-0.2.2/ausleihe/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.utils.http import urlencode
 from django.views import View
 from django.views.generic import DetailView, ListView
 from django.views.generic.base import TemplateView
 from django.views.generic.edit import CreateView, UpdateView
 
 from datetime import date, datetime, timedelta
-from fsmedhro_core.models import FachschaftUser
+from fsmedhro_core.models import FachschaftUser, Kontaktdaten
 
 from .models import (
     Autor,
     Buch,
     Leihe,
     Medium,
     Verlag,
@@ -346,19 +346,19 @@
             url = reverse("ausleihe:verliehen-an")
             parameter = urlencode({"username": username})
             return redirect(f"{url}?{parameter}")
         else:
             return redirect("ausleihe:verliehen")
 
 
-class LeiheList(LoginRequiredMixin, PermissionRequiredMixin, ListView):
-    permission_required = "ausleihe.view_leihe"
+class LeiheList(LoginRequiredMixin, ListView):
     queryset = Leihe.objects.prefetch_related(
         "medium",
-        "nutzer",
+        "medium__buecher",
+        "nutzer__user",
         "verleiht_von",
     ).filter(
         zurueckgebracht=False,
     ).order_by(
         "ende",
         "nutzer",
     )
@@ -368,22 +368,32 @@
     template_name = "ausleihe/leihe_user_detail.html"
     user_model = get_user_model()
 
     def get(self, request):
         username = request.GET.get("username", None)
 
         user = get_object_or_404(self.user_model, username=username)
-        fuser = get_object_or_404(FachschaftUser, user=user.id)
+        fuser = get_object_or_404(
+            FachschaftUser,
+            user=user.id
+        )
 
-        leihen = Leihe.objects.filter(nutzer=fuser)
+        kontaktdaten = Kontaktdaten.objects.filter(fachschaftuser=fuser)
+
+        leihen = Leihe.objects.filter(nutzer=fuser).prefetch_related(
+            "medium__buecher",
+            "nutzer__user",
+            "verleiht_von",
+        )
 
         context = {
             "nutzer": fuser,
             "aktuell_verliehen": leihen.filter(zurueckgebracht=False),
             "historisch_verliehen": leihen.filter(zurueckgebracht=True),
+            "kontaktdaten": kontaktdaten,
         }
 
         return render(request, self.template_name, context)
 
 
 class LeiheUserSuche(LoginRequiredMixin, PermissionRequiredMixin, TemplateView):
     permission_required = "ausleihe.view_leihe"
```

### Comparing `django-ausleihe-0.2.1/django_ausleihe.egg-info/PKG-INFO` & `django_ausleihe-0.2.2/django_ausleihe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ausleihe
-Version: 0.2.1
+Version: 0.2.2
 Summary: Django-App für die Ausleihe von Medien.
 Home-page: https://github.com/hutchison/django-ausleihe
 Author: Martin Darmüntzel
 Author-email: martin@trivialanalog.de
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-ausleihe-0.2.1/django_ausleihe.egg-info/SOURCES.txt` & `django_ausleihe-0.2.2/django_ausleihe.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 ausleihe/templates/ausleihe/buch_create.html
 ausleihe/templates/ausleihe/buch_detail.html
 ausleihe/templates/ausleihe/buch_edit.html
 ausleihe/templates/ausleihe/buch_form.html
 ausleihe/templates/ausleihe/buch_list.html
 ausleihe/templates/ausleihe/home.html
 ausleihe/templates/ausleihe/leihe_list.html
+ausleihe/templates/ausleihe/leihe_list_normal_table.html
+ausleihe/templates/ausleihe/leihe_list_staff_table.html
 ausleihe/templates/ausleihe/leihe_user_detail.html
 ausleihe/templates/ausleihe/leihe_user_suche.html
 ausleihe/templates/ausleihe/medium_detail.html
 ausleihe/templates/ausleihe/profil_unvollstaendig.html
 ausleihe/templates/ausleihe/verlag_create.html
 ausleihe/templates/ausleihe/verlag_detail.html
 ausleihe/templates/ausleihe/verlag_edit.html
```

### Comparing `django-ausleihe-0.2.1/setup.py` & `django_ausleihe-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-ausleihe',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     include_package_data=True,
     description='Django-App für die Ausleihe von Medien.',
     long_description=README,
     license='MIT License',
     url='https://github.com/hutchison/django-ausleihe',
     install_requires=[
```

