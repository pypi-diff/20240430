# Comparing `tmp/baseweb-0.2.1.tar.gz` & `tmp/baseweb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseweb-0.2.1.tar", last modified: Sat Apr 13 07:26:53 2024, max compression
+gzip compressed data, was "baseweb-0.3.0.tar", last modified: Tue Apr 30 20:42:10 2024, max compression
```

## Comparing `baseweb-0.2.1.tar` & `baseweb-0.3.0.tar`

### file list

```diff
@@ -1,123 +1,118 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.999029 baseweb-0.2.1/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.970221 baseweb-0.2.1/.github/
--rw-r--r--   0 xtof       (501) staff       (20)      995 2024-02-18 12:58:44.000000 baseweb-0.2.1/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1072 2024-01-17 08:54:40.000000 baseweb-0.2.1/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      189 2022-11-26 16:31:09.000000 baseweb-0.2.1/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1901 2024-04-13 07:26:52.998816 baseweb-0.2.1/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.971545 baseweb-0.2.1/baseweb/
--rw-r--r--   0 xtof       (501) staff       (20)      232 2024-04-13 07:25:45.000000 baseweb-0.2.1/baseweb/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1455 2023-10-31 18:48:41.000000 baseweb-0.2.1/baseweb/config.py
--rw-r--r--   0 xtof       (501) staff       (20)     2006 2023-10-31 18:49:02.000000 baseweb-0.2.1/baseweb/interface.py
--rw-r--r--   0 xtof       (501) staff       (20)      331 2023-10-31 18:49:11.000000 baseweb-0.2.1/baseweb/rest.py
--rw-r--r--   0 xtof       (501) staff       (20)      841 2023-10-31 18:49:29.000000 baseweb-0.2.1/baseweb/security.py
--rw-r--r--   0 xtof       (501) staff       (20)      482 2023-10-31 18:49:59.000000 baseweb-0.2.1/baseweb/socketio.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.975781 baseweb-0.2.1/baseweb/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.976270 baseweb-0.2.1/baseweb/static/css/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/css/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      287 2022-12-29 15:36:28.000000 baseweb-0.2.1/baseweb/static/css/main.css
--rw-rw-rw-   0 xtof       (501) staff       (20)     4773 2022-10-28 08:40:23.000000 baseweb-0.2.1/baseweb/static/css/process_diagram.css
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.977448 baseweb-0.2.1/baseweb/static/js/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/js/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      586 2023-05-03 12:25:47.000000 baseweb-0.2.1/baseweb/static/js/app.js
--rw-r--r--   0 xtof       (501) staff       (20)     1024 2024-02-28 19:30:19.000000 baseweb-0.2.1/baseweb/static/js/common.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.979745 baseweb-0.2.1/baseweb/static/js/components/
--rw-rw-rw-   0 xtof       (501) staff       (20)     8465 2023-01-12 13:14:07.000000 baseweb-0.2.1/baseweb/static/js/components/CollectionView.js
--rw-rw-rw-   0 xtof       (501) staff       (20)      730 2024-02-28 13:22:18.000000 baseweb-0.2.1/baseweb/static/js/components/LineChart.js
--rw-r--r--   0 xtof       (501) staff       (20)     4814 2022-12-29 15:51:31.000000 baseweb-0.2.1/baseweb/static/js/components/NavigationDrawer.js
--rw-r--r--   0 xtof       (501) staff       (20)      150 2024-02-17 17:20:33.000000 baseweb-0.2.1/baseweb/static/js/components/Page.js
--rw-r--r--   0 xtof       (501) staff       (20)      725 2024-02-17 17:25:08.000000 baseweb-0.2.1/baseweb/static/js/components/PageWithBanner.js
--rw-r--r--   0 xtof       (501) staff       (20)     1265 2024-02-17 17:29:54.000000 baseweb-0.2.1/baseweb/static/js/components/PageWithStatus.js
--rw-rw-rw-   0 xtof       (501) staff       (20)     1253 2024-02-28 20:13:23.000000 baseweb-0.2.1/baseweb/static/js/components/ProcessDiagram.js
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/js/components/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)       88 2022-12-28 12:15:48.000000 baseweb-0.2.1/baseweb/static/js/router.js
--rw-r--r--   0 xtof       (501) staff       (20)      639 2024-02-28 19:00:45.000000 baseweb-0.2.1/baseweb/static/js/socketio.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.979867 baseweb-0.2.1/baseweb/static/vendor/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.981379 baseweb-0.2.1/baseweb/static/vendor/css/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    13490 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/bootstrap-datetimepicker.css
--rw-r--r--   0 xtof       (501) staff       (20)     1571 2022-11-30 17:41:16.000000 baseweb-0.2.1/baseweb/static/vendor/css/highlight.js.github.css
--rw-r--r--   0 xtof       (501) staff       (20)     1363 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/roboto-material-icons.css
--rw-r--r--   0 xtof       (501) staff       (20)     9800 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/vfg.css
--rw-r--r--   0 xtof       (501) staff       (20)     7238 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/css/vue-multiselect.min.css
--rw-r--r--   0 xtof       (501) staff       (20)   210148 2022-12-25 18:19:16.000000 baseweb-0.2.1/baseweb/static/vendor/css/vuetify.min.css
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.983751 baseweb-0.2.1/baseweb/static/vendor/fonts/
--rw-r--r--   0 xtof       (501) staff       (20)    35588 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35468 2022-12-28 19:16:33.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35236 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35408 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    49168 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.996333 baseweb-0.2.1/baseweb/static/vendor/js/
--rw-r--r--   0 xtof       (501) staff       (20)   157843 2022-12-29 15:35:01.000000 baseweb-0.2.1/baseweb/static/vendor/js/Chart.min.js
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    39239 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js
--rwxr-xr-x   0 xtof       (501) staff       (20)    37045 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/bootstrap.min.js
--rw-r--r--   0 xtof       (501) staff       (20)   120762 2022-11-30 17:19:12.000000 baseweb-0.2.1/baseweb/static/vendor/js/highlight.min.js
--rw-r--r--   0 xtof       (501) staff       (20)     2730 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/html5shiv.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    40413 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/index.js.map
--rwxr-xr-x   0 xtof       (501) staff       (20)    97163 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/jquery.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    51465 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/moment.min.js
--rw-r--r--   0 xtof       (501) staff       (20)     4377 2022-08-27 14:55:53.000000 baseweb-0.2.1/baseweb/static/vendor/js/respond.min.js
--rw-r--r--   0 xtof       (501) staff       (20)   146329 2022-08-27 16:18:42.000000 baseweb-0.2.1/baseweb/static/vendor/js/socket.io.min.js.map
--rw-r--r--   0 xtof       (501) staff       (20)    43622 2022-08-27 16:18:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/socket.io.slim.js
--rw-r--r--   0 xtof       (501) staff       (20)     3526 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-chartjs.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    24240 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-chartjs.min.js.map
--rw-r--r--   0 xtof       (501) staff       (20)   115645 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-form-generator.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    43084 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-multiselect.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    30139 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-notification.js
--rw-r--r--   0 xtof       (501) staff       (20)    65289 2022-11-26 16:27:44.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue-router.js
--rw-r--r--   0 xtof       (501) staff       (20)   433738 2022-12-25 18:21:14.000000 baseweb-0.2.1/baseweb/static/vendor/js/vue.js
--rw-r--r--   0 xtof       (501) staff       (20)  1101513 2022-12-25 18:34:51.000000 baseweb-0.2.1/baseweb/static/vendor/js/vuetify.js
--rw-r--r--   0 xtof       (501) staff       (20)  1102711 2022-12-25 18:34:51.000000 baseweb-0.2.1/baseweb/static/vendor/js/vuetify.js.map
--rw-r--r--   0 xtof       (501) staff       (20)    25628 2022-11-26 16:27:44.000000 baseweb-0.2.1/baseweb/static/vendor/js/vuex.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.998187 baseweb-0.2.1/baseweb/templates/
--rw-r--r--   0 xtof       (501) staff       (20)      270 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/templates/404.html
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:54.000000 baseweb-0.2.1/baseweb/templates/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5798 2024-02-28 18:59:45.000000 baseweb-0.2.1/baseweb/templates/main.html
--rw-r--r--   0 xtof       (501) staff       (20)     1099 2022-12-28 10:02:38.000000 baseweb-0.2.1/baseweb/templates/manifest.json
--rw-r--r--   0 xtof       (501) staff       (20)      145 2022-12-28 11:17:50.000000 baseweb-0.2.1/baseweb/templates/store.js
--rw-r--r--   0 xtof       (501) staff       (20)      171 2023-10-31 18:50:47.000000 baseweb-0.2.1/baseweb/web.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.971776 baseweb-0.2.1/baseweb-demo/
--rw-r--r--   0 xtof       (501) staff       (20)     2110 2024-02-28 19:16:23.000000 baseweb-0.2.1/baseweb-demo/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972012 baseweb-0.2.1/baseweb-demo/pages/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-11-26 16:32:12.000000 baseweb-0.2.1/baseweb-demo/pages/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972110 baseweb-0.2.1/baseweb-demo/pages/components/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972208 baseweb-0.2.1/baseweb-demo/pages/components/CollectionView/
--rw-r--r--   0 xtof       (501) staff       (20)     1924 2024-02-18 13:05:47.000000 baseweb-0.2.1/baseweb-demo/pages/components/CollectionView/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972469 baseweb-0.2.1/baseweb-demo/pages/components/LineChart/
--rw-r--r--   0 xtof       (501) staff       (20)      164 2024-02-18 16:47:27.000000 baseweb-0.2.1/baseweb-demo/pages/components/LineChart/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972700 baseweb-0.2.1/baseweb-demo/pages/components/PageWithBanner/
--rw-r--r--   0 xtof       (501) staff       (20)      169 2022-12-28 10:58:50.000000 baseweb-0.2.1/baseweb-demo/pages/components/PageWithBanner/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.972936 baseweb-0.2.1/baseweb-demo/pages/components/PageWithStatus/
--rw-r--r--   0 xtof       (501) staff       (20)      169 2024-02-17 17:14:44.000000 baseweb-0.2.1/baseweb-demo/pages/components/PageWithStatus/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.973166 baseweb-0.2.1/baseweb-demo/pages/components/ProcessDiagram/
--rw-r--r--   0 xtof       (501) staff       (20)      244 2024-02-28 20:07:49.000000 baseweb-0.2.1/baseweb-demo/pages/components/ProcessDiagram/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-28 10:55:34.000000 baseweb-0.2.1/baseweb-demo/pages/components/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.973424 baseweb-0.2.1/baseweb-demo/pages/index/
--rw-r--r--   0 xtof       (501) staff       (20)     1313 2024-02-18 13:06:35.000000 baseweb-0.2.1/baseweb-demo/pages/index/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.973663 baseweb-0.2.1/baseweb-demo/pages/page1/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.2.1/baseweb-demo/pages/page1/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.973896 baseweb-0.2.1/baseweb-demo/pages/page2/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.2.1/baseweb-demo/pages/page2/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.974085 baseweb-0.2.1/baseweb-demo/pages/page3/
--rw-r--r--   0 xtof       (501) staff       (20)      311 2023-04-29 12:05:47.000000 baseweb-0.2.1/baseweb-demo/pages/page3/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.974313 baseweb-0.2.1/baseweb-demo/pages/page4/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-28 13:04:06.000000 baseweb-0.2.1/baseweb-demo/pages/page4/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.974568 baseweb-0.2.1/baseweb-demo/pages/page5/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-29 15:06:11.000000 baseweb-0.2.1/baseweb-demo/pages/page5/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.974800 baseweb-0.2.1/baseweb-demo/pages/protected_page/
--rw-r--r--   0 xtof       (501) staff       (20)     1227 2024-02-18 13:07:07.000000 baseweb-0.2.1/baseweb-demo/pages/protected_page/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.975042 baseweb-0.2.1/baseweb-demo/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-25 18:52:18.000000 baseweb-0.2.1/baseweb-demo/static/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.975654 baseweb-0.2.1/baseweb.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1901 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     3412 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)      114 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       21 2024-04-13 07:26:52.000000 baseweb-0.2.1/baseweb.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-13 07:26:52.999069 baseweb-0.2.1/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1702 2024-04-13 07:23:18.000000 baseweb-0.2.1/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-13 07:26:52.998422 baseweb-0.2.1/tests/
--rw-r--r--   0 xtof       (501) staff       (20)       84 2023-10-31 18:51:49.000000 baseweb-0.2.1/tests/test_placeholder.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.052123 baseweb-0.3.0/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.038890 baseweb-0.3.0/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)      995 2024-02-18 12:58:44.000000 baseweb-0.3.0/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1072 2024-01-17 08:54:40.000000 baseweb-0.3.0/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      189 2022-11-26 16:31:09.000000 baseweb-0.3.0/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1901 2024-04-30 20:42:10.051880 baseweb-0.3.0/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.039153 baseweb-0.3.0/baseweb/
+-rw-r--r--   0 xtof       (501) staff       (20)     5998 2024-04-30 20:41:27.000000 baseweb-0.3.0/baseweb/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.041808 baseweb-0.3.0/baseweb/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.042140 baseweb-0.3.0/baseweb/static/css/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/css/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      287 2022-12-29 15:36:28.000000 baseweb-0.3.0/baseweb/static/css/main.css
+-rw-rw-rw-   0 xtof       (501) staff       (20)     4773 2022-10-28 08:40:23.000000 baseweb-0.3.0/baseweb/static/css/process_diagram.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.042714 baseweb-0.3.0/baseweb/static/js/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/js/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      586 2023-05-03 12:25:47.000000 baseweb-0.3.0/baseweb/static/js/app.js
+-rw-r--r--   0 xtof       (501) staff       (20)     1024 2024-02-28 19:30:19.000000 baseweb-0.3.0/baseweb/static/js/common.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.043814 baseweb-0.3.0/baseweb/static/js/components/
+-rw-rw-rw-   0 xtof       (501) staff       (20)     8465 2023-01-12 13:14:07.000000 baseweb-0.3.0/baseweb/static/js/components/CollectionView.js
+-rw-rw-rw-   0 xtof       (501) staff       (20)      730 2024-02-28 13:22:18.000000 baseweb-0.3.0/baseweb/static/js/components/LineChart.js
+-rw-r--r--   0 xtof       (501) staff       (20)     4814 2022-12-29 15:51:31.000000 baseweb-0.3.0/baseweb/static/js/components/NavigationDrawer.js
+-rw-r--r--   0 xtof       (501) staff       (20)      150 2024-02-17 17:20:33.000000 baseweb-0.3.0/baseweb/static/js/components/Page.js
+-rw-r--r--   0 xtof       (501) staff       (20)      725 2024-02-17 17:25:08.000000 baseweb-0.3.0/baseweb/static/js/components/PageWithBanner.js
+-rw-r--r--   0 xtof       (501) staff       (20)     1265 2024-02-17 17:29:54.000000 baseweb-0.3.0/baseweb/static/js/components/PageWithStatus.js
+-rw-rw-rw-   0 xtof       (501) staff       (20)     1253 2024-02-28 20:13:23.000000 baseweb-0.3.0/baseweb/static/js/components/ProcessDiagram.js
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/js/components/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)       88 2022-12-28 12:15:48.000000 baseweb-0.3.0/baseweb/static/js/router.js
+-rw-r--r--   0 xtof       (501) staff       (20)      639 2024-02-28 19:00:45.000000 baseweb-0.3.0/baseweb/static/js/socketio.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.043907 baseweb-0.3.0/baseweb/static/vendor/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.044810 baseweb-0.3.0/baseweb/static/vendor/css/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/css/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    13490 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/css/bootstrap-datetimepicker.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1571 2022-11-30 17:41:16.000000 baseweb-0.3.0/baseweb/static/vendor/css/highlight.js.github.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1363 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/css/roboto-material-icons.css
+-rw-r--r--   0 xtof       (501) staff       (20)     9800 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/css/vfg.css
+-rw-r--r--   0 xtof       (501) staff       (20)     7238 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/css/vue-multiselect.min.css
+-rw-r--r--   0 xtof       (501) staff       (20)   210148 2022-12-25 18:19:16.000000 baseweb-0.3.0/baseweb/static/vendor/css/vuetify.min.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.045897 baseweb-0.3.0/baseweb/static/vendor/fonts/
+-rw-r--r--   0 xtof       (501) staff       (20)    35588 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35468 2022-12-28 19:16:33.000000 baseweb-0.3.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35236 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35408 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/fonts/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    49168 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.050703 baseweb-0.3.0/baseweb/static/vendor/js/
+-rw-r--r--   0 xtof       (501) staff       (20)   157843 2022-12-29 15:35:01.000000 baseweb-0.3.0/baseweb/static/vendor/js/Chart.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/js/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    39239 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js
+-rwxr-xr-x   0 xtof       (501) staff       (20)    37045 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/js/bootstrap.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)   120762 2022-11-30 17:19:12.000000 baseweb-0.3.0/baseweb/static/vendor/js/highlight.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)     2730 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/js/html5shiv.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    40413 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/js/index.js.map
+-rwxr-xr-x   0 xtof       (501) staff       (20)    97163 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/js/jquery.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    51465 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/js/moment.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)     4377 2022-08-27 14:55:53.000000 baseweb-0.3.0/baseweb/static/vendor/js/respond.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)   146329 2022-08-27 16:18:42.000000 baseweb-0.3.0/baseweb/static/vendor/js/socket.io.min.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)    43622 2022-08-27 16:18:54.000000 baseweb-0.3.0/baseweb/static/vendor/js/socket.io.slim.js
+-rw-r--r--   0 xtof       (501) staff       (20)     3526 2022-08-27 14:55:54.000000 baseweb-0.3.0/baseweb/static/vendor/js/vue-chartjs.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    24240 2022-08-27 14:55:54.000000 baseweb-0.3.0/baseweb/static/vendor/js/vue-chartjs.min.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)   115645 2022-08-27 14:55:54.000000 baseweb-0.3.0/baseweb/static/vendor/js/vue-form-generator.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    43084 2022-08-27 14:55:54.000000 baseweb-0.3.0/baseweb/static/vendor/js/vue-multiselect.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    30139 2022-08-27 14:55:54.000000 baseweb-0.3.0/baseweb/static/vendor/js/vue-notification.js
+-rw-r--r--   0 xtof       (501) staff       (20)    65289 2022-11-26 16:27:44.000000 baseweb-0.3.0/baseweb/static/vendor/js/vue-router.js
+-rw-r--r--   0 xtof       (501) staff       (20)   433738 2022-12-25 18:21:14.000000 baseweb-0.3.0/baseweb/static/vendor/js/vue.js
+-rw-r--r--   0 xtof       (501) staff       (20)  1101513 2022-12-25 18:34:51.000000 baseweb-0.3.0/baseweb/static/vendor/js/vuetify.js
+-rw-r--r--   0 xtof       (501) staff       (20)  1102711 2022-12-25 18:34:51.000000 baseweb-0.3.0/baseweb/static/vendor/js/vuetify.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)    25628 2022-11-26 16:27:44.000000 baseweb-0.3.0/baseweb/static/vendor/js/vuex.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.051451 baseweb-0.3.0/baseweb/templates/
+-rw-r--r--   0 xtof       (501) staff       (20)      270 2022-08-27 14:55:54.000000 baseweb-0.3.0/baseweb/templates/404.html
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:54.000000 baseweb-0.3.0/baseweb/templates/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5798 2024-04-30 20:24:03.000000 baseweb-0.3.0/baseweb/templates/main.html
+-rw-r--r--   0 xtof       (501) staff       (20)     1099 2022-12-28 10:02:38.000000 baseweb-0.3.0/baseweb/templates/manifest.json
+-rw-r--r--   0 xtof       (501) staff       (20)      145 2022-12-28 11:17:50.000000 baseweb-0.3.0/baseweb/templates/store.js
+-rw-r--r--   0 xtof       (501) staff       (20)      231 2024-04-30 13:42:09.000000 baseweb-0.3.0/baseweb/util.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.039275 baseweb-0.3.0/baseweb-demo/
+-rw-r--r--   0 xtof       (501) staff       (20)     2180 2024-04-30 20:32:06.000000 baseweb-0.3.0/baseweb-demo/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.039399 baseweb-0.3.0/baseweb-demo/pages/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-11-26 16:32:12.000000 baseweb-0.3.0/baseweb-demo/pages/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.039498 baseweb-0.3.0/baseweb-demo/pages/components/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.039597 baseweb-0.3.0/baseweb-demo/pages/components/CollectionView/
+-rw-r--r--   0 xtof       (501) staff       (20)     1857 2024-04-30 20:30:43.000000 baseweb-0.3.0/baseweb-demo/pages/components/CollectionView/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.039747 baseweb-0.3.0/baseweb-demo/pages/components/LineChart/
+-rw-r--r--   0 xtof       (501) staff       (20)      145 2024-04-30 20:30:43.000000 baseweb-0.3.0/baseweb-demo/pages/components/LineChart/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.039886 baseweb-0.3.0/baseweb-demo/pages/components/PageWithBanner/
+-rw-r--r--   0 xtof       (501) staff       (20)      150 2024-04-30 20:30:43.000000 baseweb-0.3.0/baseweb-demo/pages/components/PageWithBanner/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040006 baseweb-0.3.0/baseweb-demo/pages/components/PageWithStatus/
+-rw-r--r--   0 xtof       (501) staff       (20)      150 2024-04-30 20:30:43.000000 baseweb-0.3.0/baseweb-demo/pages/components/PageWithStatus/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040132 baseweb-0.3.0/baseweb-demo/pages/components/ProcessDiagram/
+-rw-r--r--   0 xtof       (501) staff       (20)      232 2024-04-30 20:30:43.000000 baseweb-0.3.0/baseweb-demo/pages/components/ProcessDiagram/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-04-30 15:36:20.000000 baseweb-0.3.0/baseweb-demo/pages/components/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040249 baseweb-0.3.0/baseweb-demo/pages/index/
+-rw-r--r--   0 xtof       (501) staff       (20)     1221 2024-04-30 20:30:37.000000 baseweb-0.3.0/baseweb-demo/pages/index/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040367 baseweb-0.3.0/baseweb-demo/pages/page1/
+-rw-r--r--   0 xtof       (501) staff       (20)      140 2024-04-30 20:30:37.000000 baseweb-0.3.0/baseweb-demo/pages/page1/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040484 baseweb-0.3.0/baseweb-demo/pages/page2/
+-rw-r--r--   0 xtof       (501) staff       (20)      140 2024-04-30 20:30:37.000000 baseweb-0.3.0/baseweb-demo/pages/page2/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040604 baseweb-0.3.0/baseweb-demo/pages/page3/
+-rw-r--r--   0 xtof       (501) staff       (20)      269 2024-04-30 20:30:37.000000 baseweb-0.3.0/baseweb-demo/pages/page3/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040718 baseweb-0.3.0/baseweb-demo/pages/page4/
+-rw-r--r--   0 xtof       (501) staff       (20)      140 2024-04-30 20:30:37.000000 baseweb-0.3.0/baseweb-demo/pages/page4/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040833 baseweb-0.3.0/baseweb-demo/pages/page5/
+-rw-r--r--   0 xtof       (501) staff       (20)      140 2024-04-30 20:30:37.000000 baseweb-0.3.0/baseweb-demo/pages/page5/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.040967 baseweb-0.3.0/baseweb-demo/pages/protected_page/
+-rw-r--r--   0 xtof       (501) staff       (20)     1052 2024-04-30 20:30:37.000000 baseweb-0.3.0/baseweb-demo/pages/protected_page/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.041097 baseweb-0.3.0/baseweb-demo/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-25 18:52:18.000000 baseweb-0.3.0/baseweb-demo/static/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.041680 baseweb-0.3.0/baseweb.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1901 2024-04-30 20:42:10.000000 baseweb-0.3.0/baseweb.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     3318 2024-04-30 20:42:10.000000 baseweb-0.3.0/baseweb.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-30 20:42:10.000000 baseweb-0.3.0/baseweb.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      114 2024-04-30 20:42:10.000000 baseweb-0.3.0/baseweb.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       21 2024-04-30 20:42:10.000000 baseweb-0.3.0/baseweb.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-30 20:42:10.052171 baseweb-0.3.0/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1702 2024-04-13 07:23:18.000000 baseweb-0.3.0/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-30 20:42:10.051588 baseweb-0.3.0/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)      107 2024-04-30 16:45:38.000000 baseweb-0.3.0/tests/test_placeholder.py
```

### Comparing `baseweb-0.2.1/.github/README.md` & `baseweb-0.3.0/.github/README.md`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/LICENSE.txt` & `baseweb-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/PKG-INFO` & `baseweb-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseweb
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Pythonic base for building interactive web applications
 Home-page: https://github.com/christophevg/baseweb
 Author: Christophe VG
 License: MIT
 Keywords: Flask Vue REST SocketIO
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
```

### Comparing `baseweb-0.2.1/baseweb/static/css/process_diagram.css` & `baseweb-0.3.0/baseweb/static/css/process_diagram.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/app.js` & `baseweb-0.3.0/baseweb/static/js/app.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/common.js` & `baseweb-0.3.0/baseweb/static/js/common.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/components/CollectionView.js` & `baseweb-0.3.0/baseweb/static/js/components/CollectionView.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/components/LineChart.js` & `baseweb-0.3.0/baseweb/static/js/components/LineChart.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/components/NavigationDrawer.js` & `baseweb-0.3.0/baseweb/static/js/components/NavigationDrawer.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/components/PageWithBanner.js` & `baseweb-0.3.0/baseweb/static/js/components/PageWithBanner.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/components/PageWithStatus.js` & `baseweb-0.3.0/baseweb/static/js/components/PageWithStatus.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/components/ProcessDiagram.js` & `baseweb-0.3.0/baseweb/static/js/components/ProcessDiagram.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/js/socketio.js` & `baseweb-0.3.0/baseweb/static/js/socketio.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/css/bootstrap-datetimepicker.css` & `baseweb-0.3.0/baseweb/static/vendor/css/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/css/highlight.js.github.css` & `baseweb-0.3.0/baseweb/static/vendor/css/highlight.js.github.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/css/roboto-material-icons.css` & `baseweb-0.3.0/baseweb/static/vendor/css/roboto-material-icons.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/css/vfg.css` & `baseweb-0.3.0/baseweb/static/vendor/css/vfg.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/css/vue-multiselect.min.css` & `baseweb-0.3.0/baseweb/static/vendor/css/vue-multiselect.min.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/css/vuetify.min.css` & `baseweb-0.3.0/baseweb/static/vendor/css/vuetify.min.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf` & `baseweb-0.3.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf` & `baseweb-0.3.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf` & `baseweb-0.3.0/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf` & `baseweb-0.3.0/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `baseweb-0.3.0/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/Chart.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/bootstrap.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/highlight.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/html5shiv.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/index.js.map` & `baseweb-0.3.0/baseweb/static/vendor/js/index.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/jquery.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/moment.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/respond.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/socket.io.min.js.map` & `baseweb-0.3.0/baseweb/static/vendor/js/socket.io.min.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/socket.io.slim.js` & `baseweb-0.3.0/baseweb/static/vendor/js/socket.io.slim.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vue-chartjs.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/vue-chartjs.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vue-chartjs.min.js.map` & `baseweb-0.3.0/baseweb/static/vendor/js/vue-chartjs.min.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vue-form-generator.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/vue-form-generator.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vue-multiselect.min.js` & `baseweb-0.3.0/baseweb/static/vendor/js/vue-multiselect.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vue-notification.js` & `baseweb-0.3.0/baseweb/static/vendor/js/vue-notification.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vue-router.js` & `baseweb-0.3.0/baseweb/static/vendor/js/vue-router.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vue.js` & `baseweb-0.3.0/baseweb/static/vendor/js/vue.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vuetify.js` & `baseweb-0.3.0/baseweb/static/vendor/js/vuetify.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vuetify.js.map` & `baseweb-0.3.0/baseweb/static/vendor/js/vuetify.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/static/vendor/js/vuex.js` & `baseweb-0.3.0/baseweb/static/vendor/js/vuex.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/templates/main.html` & `baseweb-0.3.0/baseweb/templates/main.html`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb/templates/manifest.json` & `baseweb-0.3.0/baseweb/templates/manifest.json`

 * *Files identical despite different names*

### Comparing `baseweb-0.2.1/baseweb-demo/__init__.py` & `baseweb-0.3.0/baseweb-demo/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-# ruff: noqa
-
 import logging
-
 import os
+from pathlib import Path
 
 from dotenv import load_dotenv, find_dotenv
 
 logger = logging.getLogger(__name__)
 
 # load the environment variables for this setup
 load_dotenv(find_dotenv())
 load_dotenv(find_dotenv(".env.local"))
 
-LOG_LEVEL = os.environ.get("LOG_LEVEL") or "INFO"
-
 # setup logging infrastructure
 
-# logging.getLogger("urllib3").setLevel(logging.WARN)
-
+LOG_LEVEL = os.environ.get("LOG_LEVEL") or "INFO"
 FORMAT  = "[%(asctime)s] [%(name)s] [%(process)d] [%(levelname)s] %(message)s"
 DATEFMT = "%Y-%m-%d %H:%M:%S %z"
 
 logging.basicConfig(level=LOG_LEVEL, format=FORMAT, datefmt=DATEFMT)
 formatter = logging.Formatter(FORMAT, DATEFMT)
 
-# adjust gunicorn logger to global level and formatting 
+# adjust other loggers to global level and formatting 
 logging.getLogger("gunicorn.error").handlers[0].setFormatter(formatter)
 logging.getLogger("gunicorn.error").setLevel(logging.INFO)
 logging.getLogger("engineio.client").setLevel(logging.WARN)
 logging.getLogger("engineio.server").setLevel(logging.WARN)
 logging.getLogger("socketio.client").setLevel(logging.WARN)
 logging.getLogger("socketio.server").setLevel(logging.WARN)
+logging.getLogger("urllib3").setLevel(logging.WARN)
 
 logging.getLogger().handlers[0].setFormatter(formatter)
 
-# import baseweb server object to expose it from this application
-from baseweb.web import server
+# all set up, now get our server
 
-from baseweb.security import add_authenticator
+from baseweb import server
 
 def authenticator(scope, request, *args, **kwargs):
-  logger.debug("AUTH: scope:{} / request:{} / args:{} / kwargs:{}".format(
+  logger.debug("👀 scope:{} / request:{} / args:{} / kwargs:{}".format(
     scope, str(request), str(args), str(kwargs)
   ))
   return True
 
-add_authenticator(authenticator)
+server.authenticator = authenticator
+
+@server.socketio.on("connect")
+def on_connect():
+  logger.info("connect: {0}".format(server.request.sid))
 
-from baseweb.interface import register_component, register_static_folder
+@server.socketio.on("disconnect")
+def on_disconnect():
+  logger.info("disconnect: {0}".format(server.request.sid))
 
-HERE       = os.path.dirname(__file__)
-COMPONENTS = os.path.join(HERE, "components")
+HERE       = Path(__file__).resolve().parent
+COMPONENTS = HERE / "components"
 
-register_static_folder(os.path.join(HERE, "static"))
+server.register_component("app.js",        HERE)
+server.register_component("SourceView.js", COMPONENTS)
+server.register_component("logo.js",       COMPONENTS)
 
-register_component("app.js",        HERE)
-register_component("SourceView.js", COMPONENTS)
-register_component("logo.js",       COMPONENTS)
+server.app_static_folder = HERE / "static"
 
 from .pages            import index, page1, page2, page3, page4, page5
 from .pages            import protected_page
 from .pages.components import PageWithStatus, PageWithBanner, CollectionView
 from .pages.components import LineChart, ProcessDiagram
 
-logger.info("✅ all systems are go!")
+logger.info("✅ demo is ready")
```

### Comparing `baseweb-0.2.1/baseweb-demo/pages/components/CollectionView/__init__.py` & `baseweb-0.3.0/baseweb-demo/pages/components/CollectionView/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import os
 from datetime import datetime, timedelta
 import random
 
-from baseweb.interface import register_component
-
 from flask import request
 from flask_restful import Resource
 
-from baseweb.rest     import api
-from baseweb.security import authenticated
+from .... import server
 
 def random_date_between(start, end):
   delta = end - start
   int_delta = (delta.days * 24 * 3600) + delta.seconds
   return start + timedelta(seconds=random.randrange(int_delta))
 
 def random_date():
   return random_date_between(datetime.now(), datetime.now()+timedelta(days=1))
 
-register_component("CollectionView.js", os.path.dirname(__file__))
+server.register_component("CollectionView.js", os.path.dirname(__file__))
 
 # set up an in-memory collection of random names and provide a resource to
 # access them with query arguments, emulating a MongoDB collection
 
 first_names = [ "John", "Andy", "Joe" ]
 last_names  = [ "Johnson", "Smith", "Williams" ]
 data = [
@@ -31,15 +28,15 @@
     "name"    : random.choice(first_names) + " " + random.choice(last_names),
     "created" : random_date().isoformat(),
     "updated" : random_date().isoformat()
   } for index in range(100)
 ]
 
 class Collection(Resource):
-  @authenticated("app.collection.get")
+  @server.authenticated("app.collection.get")
   def get(self):
     start = int(request.args.get("start", 0))
     limit = int(request.args.get("limit", 5))
     sort  = request.args.get("sort", None)
     order = request.args.get("order", "asc")
     name  = request.args.get("name", None)
 
@@ -52,16 +49,16 @@
       selection.reverse()
 
     return { 
       "content"       : selection[start:start+limit],
       "totalElements" : len(data)
     }
     
-  @authenticated("app.collection.post")
+  @server.authenticated("app.collection.post")
   def post(self):
     return "ok"
 
-  @authenticated("app.collection.delete")
+  @server.authenticated("app.collection.delete")
   def delete(self):
     return "ok"
 
-api.add_resource(Collection, "/api/collection")
+server.api.add_resource(Collection, "/api/collection")
```

### Comparing `baseweb-0.2.1/baseweb-demo/pages/index/__init__.py` & `baseweb-0.3.0/baseweb-demo/pages/index/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 import logging
 
 import os
 
-from baseweb.interface import register_component
-
 from flask import request
 
 from flask_restful import Resource
 
-from baseweb.rest     import api
-from baseweb.socketio import socketio
-from baseweb.security import authenticated
+from ... import server
 
 logger = logging.getLogger(__name__)
 
 # register the Vue component for the UI
-register_component("index.js", os.path.dirname(__file__))
+server.register_component("index.js", os.path.dirname(__file__))
 
 # log all messages both to logging infrastructure and connected clients
 
 def log(msg):
   logger.info(msg)
-  socketio.emit("log", msg)
+  server.socketio.emit("log", msg)
 
 # set up socketio event handlers to handle events from the UI
 
-@socketio.on("hello")
-@authenticated("app.io.hello")
+@server.socketio.on("hello")
+@server.authenticated("app.io.hello")
 def on_hello(name):
   log("received hello from {0} ({1}) via socketio".format(name, request.sid))
   return "Hello {0} from socketio!".format(name)
 
 # set up a REST resource to handle requests from the UI
 
 class Hello(Resource):
-  @authenticated("app.hello.get")
+  @server.authenticated("app.hello.get")
   def get(self):
     name = request.args["name"]
     log("received hello from {0} via rest/get".format(name))
     return "Hello {0} from REST/GET".format(name)
     
-  @authenticated("app.hello.post")
+  @server.authenticated("app.hello.post")
   def post(self):
     name = request.get_json()["name"]
     log("received hello from {0} via rest/post".format(name))
     return "Hello {0} from REST/POST".format(name)
 
-api.add_resource(Hello, "/api/hello")
+server.api.add_resource(Hello, "/api/hello")
```

### Comparing `baseweb-0.2.1/baseweb-demo/pages/protected_page/__init__.py` & `baseweb-0.3.0/baseweb-demo/pages/protected_page/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,40 @@
 import os
 
-from baseweb.interface import register_component
-
-# setup OATK infrastructure
-
 from flask import Response
-from flask_restful import Resource, Api
-
-from baseweb.web       import server
-from baseweb.interface import register_external_script
-from baseweb.config    import app
+from flask_restful import Resource
 
 import oatk.js
 from oatk import OAuthToolkit
 
+from ... import server
+
 # register the Vue component for the UI
-register_component("protected_page.js", os.path.dirname(__file__))
+server.register_component("protected_page.js", os.path.dirname(__file__))
 
-# add discovery url and client_id from env
-app["oauth"] = {
+# expose discovery url and client_id settings loaded from from env
+server.settings["oauth"] = {
   "provider" : os.environ.get("OAUTH_PROVIDER"),
   "client_id": os.environ.get("OAUTH_CLIENT_ID")
 }
 
 # route for oatk.js from the oatk package
-@server.route("/oatk.js", methods=["GET"])
+@server.route("/oatk.js")
 def oatk_script():
   return Response(oatk.js.as_src(), mimetype="application/javascript")
 
 # and have it included in the HTML
-register_external_script("/oatk.js")
-
-# a protected API endpoint
-
-# API set up
-api = Api(server)
+server.register_external_script("/oatk.js")
 
-# setup oatk
-auth = OAuthToolkit()
-auth.using_provider(os.environ["OAUTH_PROVIDER"])
-auth.with_client_id(os.environ["OAUTH_CLIENT_ID"])
+# create an oauth protected API endpoint
+oauth = OAuthToolkit()
+oauth.using_provider(os.environ["OAUTH_PROVIDER"])
+oauth.with_client_id(os.environ["OAUTH_CLIENT_ID"])
 
 class HelloWorld(Resource):
-  @auth.authenticated
+  @oauth.authenticated
   def get(self):
     return {
       "message": "hello protected world"
     }
 
-api.add_resource(HelloWorld, "/api/protected/hello")
+server.api.add_resource(HelloWorld, "/api/protected/hello")
```

### Comparing `baseweb-0.2.1/baseweb.egg-info/PKG-INFO` & `baseweb-0.3.0/baseweb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseweb
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Pythonic base for building interactive web applications
 Home-page: https://github.com/christophevg/baseweb
 Author: Christophe VG
 License: MIT
 Keywords: Flask Vue REST SocketIO
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
```

### Comparing `baseweb-0.2.1/baseweb.egg-info/SOURCES.txt` & `baseweb-0.3.0/baseweb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 LICENSE.txt
 MANIFEST.in
 setup.py
 .github/README.md
 baseweb/__init__.py
-baseweb/config.py
-baseweb/interface.py
-baseweb/rest.py
-baseweb/security.py
-baseweb/socketio.py
-baseweb/web.py
+baseweb/util.py
 baseweb-demo/__init__.py
 baseweb-demo/pages/__init__.py
 baseweb-demo/pages/components/__init__.py
 baseweb-demo/pages/components/CollectionView/__init__.py
 baseweb-demo/pages/components/LineChart/__init__.py
 baseweb-demo/pages/components/PageWithBanner/__init__.py
 baseweb-demo/pages/components/PageWithStatus/__init__.py
```

### Comparing `baseweb-0.2.1/setup.py` & `baseweb-0.3.0/setup.py`

 * *Files identical despite different names*

