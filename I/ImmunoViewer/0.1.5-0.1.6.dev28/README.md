# Comparing `tmp/ImmunoViewer-0.1.5.tar.gz` & `tmp/immunoviewer-0.1.6.dev28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImmunoViewer-0.1.5.tar", last modified: Thu Apr 27 15:40:46 2023, max compression
+gzip compressed data, was "immunoviewer-0.1.6.dev28.tar", last modified: Tue Apr 30 15:12:09 2024, max compression
```

## Comparing `ImmunoViewer-0.1.5.tar` & `immunoviewer-0.1.6.dev28.tar`

### file list

```diff
@@ -1,64 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:40:46.247379 ImmunoViewer-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-27 15:40:46.247379 ImmunoViewer-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:40:46.247379 ImmunoViewer-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:40:46.235379 ImmunoViewer-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:40:46.235379 ImmunoViewer-0.1.5/src/ImmunoViewer/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:40:46.239379 ImmunoViewer-0.1.5/src/ImmunoViewer/client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:40:46.243379 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   280297 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/SlideViewer-73b8a8f8.css
--rw-r--r--   0 runner    (1001) docker     (123)   731759 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/index-38ec41fb.css
--rw-r--r--   0 runner    (1001) docker     (123)   353701 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/index-e299d4d6.js
--rw-r--r--   0 runner    (1001) docker     (123)  1280212 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot
--rw-r--r--   0 runner    (1001) docker     (123)   576748 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff
--rw-r--r--   0 runner    (1001) docker     (123)  1279992 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   396732 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:40:46.247379 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/fullpage_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/fullpage_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/fullpage_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/fullpage_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/home_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/home_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/home_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/home_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/next_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/next_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/next_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/next_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/previous_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/previous_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/previous_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/previous_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateleft_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateleft_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateleft_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateleft_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateright_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateright_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateright_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateright_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomin_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomin_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomin_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomin_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomout_grouphover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomout_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomout_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomout_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/client/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/process_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9247 2023-04-27 15:40:27.000000 ImmunoViewer-0.1.5/src/ImmunoViewer/tile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:40:46.239379 ImmunoViewer-0.1.5/src/ImmunoViewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-27 15:40:46.000000 ImmunoViewer-0.1.5/src/ImmunoViewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-27 15:40:46.000000 ImmunoViewer-0.1.5/src/ImmunoViewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:40:46.000000 ImmunoViewer-0.1.5/src/ImmunoViewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 15:40:46.000000 ImmunoViewer-0.1.5/src/ImmunoViewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 15:40:46.000000 ImmunoViewer-0.1.5/src/ImmunoViewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 15:40:46.000000 ImmunoViewer-0.1.5/src/ImmunoViewer.egg-info/top_level.txt
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.055564 immunoviewer-0.1.6.dev28/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     8196 2024-04-29 12:50:44.000000 immunoviewer-0.1.6.dev28/.DS_Store
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.968906 immunoviewer-0.1.6.dev28/.github/
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.981236 immunoviewer-0.1.6.dev28/.github/workflows/
+-rw-r--r--   0 vanijzen   (503) staff       (20)      342 2024-04-29 11:11:25.000000 immunoviewer-0.1.6.dev28/.github/workflows/push.yml
+-rw-r--r--   0 vanijzen   (503) staff       (20)      767 2024-04-30 14:35:28.000000 immunoviewer-0.1.6.dev28/.github/workflows/release.yml
+-rw-r--r--   0 vanijzen   (503) staff       (20)     3096 2024-04-12 07:04:08.000000 immunoviewer-0.1.6.dev28/.gitignore
+-rw-r--r--   0 vanijzen   (503) staff       (20)      962 2024-04-29 08:33:00.000000 immunoviewer-0.1.6.dev28/Dockerfile
+-rw-r--r--   0 vanijzen   (503) staff       (20)      849 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/LICENSE.md
+-rw-r--r--   0 vanijzen   (503) staff       (20)     5933 2024-04-30 15:12:09.055436 immunoviewer-0.1.6.dev28/PKG-INFO
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2794 2023-05-04 15:54:42.000000 immunoviewer-0.1.6.dev28/README.md
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.986282 immunoviewer-0.1.6.dev28/client/
+-rw-r--r--   0 vanijzen   (503) staff       (20)      297 2023-04-26 20:22:56.000000 immunoviewer-0.1.6.dev28/client/.gitignore
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.986617 immunoviewer-0.1.6.dev28/client/.vscode/
+-rw-r--r--   0 vanijzen   (503) staff       (20)       75 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/.vscode/extensions.json
+-rw-r--r--   0 vanijzen   (503) staff       (20)      630 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/README.md
+-rw-r--r--   0 vanijzen   (503) staff       (20)      340 2023-04-26 17:08:39.000000 immunoviewer-0.1.6.dev28/client/index.html
+-rw-r--r--   0 vanijzen   (503) staff       (20)   143490 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/package-lock.json
+-rw-r--r--   0 vanijzen   (503) staff       (20)      630 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/package.json
+-rw-r--r--   0 vanijzen   (503) staff       (20)       82 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/postcss.config.js
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.987885 immunoviewer-0.1.6.dev28/client/public/
+-rw-rw-r--   0 vanijzen   (503) staff       (20)    15406 2024-04-25 06:42:54.000000 immunoviewer-0.1.6.dev28/client/public/favicon.ico
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.004025 immunoviewer-0.1.6.dev28/client/public/images/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1085 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/fullpage_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2184 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/fullpage_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2225 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/fullpage_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1309 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/fullpage_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1062 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/home_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2091 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/home_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2138 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/home_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1258 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/home_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1918 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/next_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2358 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/next_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2411 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/next_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2027 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/next_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1933 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/previous_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2361 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/previous_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2413 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/previous_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2029 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/previous_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1731 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateleft_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2094 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateleft_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2036 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateleft_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1779 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateleft_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1800 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateright_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2158 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateright_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2039 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateright_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1812 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateright_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1060 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomin_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2116 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomin_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2159 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomin_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1262 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomin_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)      977 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomout_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1926 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomout_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1997 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomout_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1153 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomout_rest.png
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.004710 immunoviewer-0.1.6.dev28/client/src/
+-rw-r--r--   0 vanijzen   (503) staff       (20)      119 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/App.vue
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.005419 immunoviewer-0.1.6.dev28/client/src/assets/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2037 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/assets/base.css
+-rw-r--r--   0 vanijzen   (503) staff       (20)      276 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/assets/logo.svg
+-rw-r--r--   0 vanijzen   (503) staff       (20)      477 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/assets/main.css
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.971280 immunoviewer-0.1.6.dev28/client/src/components/
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.006555 immunoviewer-0.1.6.dev28/client/src/components/icons/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1054 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconCommunity.vue
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1254 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconDocumentation.vue
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1977 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconEcosystem.vue
+-rw-r--r--   0 vanijzen   (503) staff       (20)      288 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconSupport.vue
+-rw-r--r--   0 vanijzen   (503) staff       (20)      913 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconTooling.vue
+-rw-r--r--   0 vanijzen   (503) staff       (20)       60 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/src/index.css
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.007069 immunoviewer-0.1.6.dev28/client/src/js/
+-rw-r--r--   0 vanijzen   (503) staff       (20)    23862 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/js/openseadragon-scalebar.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   906910 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/js/openseadragon.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)      773 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/src/main.js
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.007785 immunoviewer-0.1.6.dev28/client/src/router/
+-rw-r--r--   0 vanijzen   (503) staff       (20)      297 2024-04-19 07:10:32.000000 immunoviewer-0.1.6.dev28/client/src/router/index.js
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.008020 immunoviewer-0.1.6.dev28/client/src/store/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     5359 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/src/store/index.js
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.008318 immunoviewer-0.1.6.dev28/client/src/views/
+-rw-r--r--   0 vanijzen   (503) staff       (20)    11985 2024-04-29 07:35:34.000000 immunoviewer-0.1.6.dev28/client/src/views/SlideViewer.vue
+-rw-r--r--   0 vanijzen   (503) staff       (20)      182 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/tailwind.config.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)      356 2023-04-26 21:40:47.000000 immunoviewer-0.1.6.dev28/client/vite.config.js
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.008991 immunoviewer-0.1.6.dev28/cloud-deploy/
+-rw-r--r--   0 vanijzen   (503) staff       (20)      804 2024-04-29 08:23:59.000000 immunoviewer-0.1.6.dev28/cloud-deploy/Dockerfile
+-rw-r--r--   0 vanijzen   (503) staff       (20)        0 2024-04-19 10:40:43.000000 immunoviewer-0.1.6.dev28/cloud-deploy/README.md
+-rw-r--r--   0 vanijzen   (503) staff       (20)      324 2024-04-29 08:34:46.000000 immunoviewer-0.1.6.dev28/cloud-deploy/requirements.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)      611 2024-04-29 08:59:06.000000 immunoviewer-0.1.6.dev28/environment.yml
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.009514 immunoviewer-0.1.6.dev28/img/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     6148 2023-04-27 16:52:22.000000 immunoviewer-0.1.6.dev28/img/.DS_Store
+-rw-r--r--   0 vanijzen   (503) staff       (20)   552037 2023-04-27 16:52:09.000000 immunoviewer-0.1.6.dev28/img/screenshot.jpg
+-rw-r--r--   0 vanijzen   (503) staff       (20)      230 2024-04-29 09:05:06.000000 immunoviewer-0.1.6.dev28/meta.yaml
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2372 2024-04-30 15:11:03.000000 immunoviewer-0.1.6.dev28/pyproject.toml
+-rw-r--r--   0 vanijzen   (503) staff       (20)      322 2024-04-29 10:43:47.000000 immunoviewer-0.1.6.dev28/requirements.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)       94 2024-04-30 15:12:09.057393 immunoviewer-0.1.6.dev28/setup.cfg
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.973278 immunoviewer-0.1.6.dev28/src/
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.010945 immunoviewer-0.1.6.dev28/src/ImmunoViewer/
+-rw-r--r--   0 vanijzen   (503) staff       (20)      205 2024-04-29 11:42:22.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/__init__.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)      426 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/_version.py
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.014724 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.030620 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/
+-rw-r--r--   0 vanijzen   (503) staff       (20)      772 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-13d6bf50.css
+-rw-r--r--   0 vanijzen   (503) staff       (20)   251090 2024-04-19 07:17:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-44b07d73.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   280297 2023-06-08 01:30:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)      127 2023-06-08 01:30:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-73b8a8f8.css
+-rw-r--r--   0 vanijzen   (503) staff       (20)      246 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-a4917311.css
+-rw-r--r--   0 vanijzen   (503) staff       (20)   251142 2024-04-19 11:01:41.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-acc75342.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   256208 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-c345c42b.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   251142 2024-04-19 10:56:39.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-cac74aba.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   256213 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-d9842cde.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   252693 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-dfaf7abb.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   249629 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-2d6a5d9a.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   249719 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-7aec11c6.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)      678 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-e1bcd4c6.css
+-rw-r--r--   0 vanijzen   (503) staff       (20)   249719 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-ec6e481a.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   123736 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-16c8f7df.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   399766 2024-04-19 10:56:39.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-1a44217b.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   399634 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-26efefc2.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   399766 2024-04-19 11:01:41.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-36ec0fef.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   731759 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-38ec41fb.css
+-rw-r--r--   0 vanijzen   (503) staff       (20)   399684 2024-04-19 07:17:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-8ddde4e4.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   123736 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-ab2b0f89.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   399624 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-d030ddc6.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   400172 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-d0c0c412.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   353701 2023-06-08 01:30:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-e299d4d6.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)   399634 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-e540ed02.js
+-rw-r--r--   0 vanijzen   (503) staff       (20)     8285 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-f65d5671.css
+-rw-r--r--   0 vanijzen   (503) staff       (20)  1280212 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot
+-rw-r--r--   0 vanijzen   (503) staff       (20)   576748 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff
+-rw-r--r--   0 vanijzen   (503) staff       (20)  1279992 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf
+-rw-r--r--   0 vanijzen   (503) staff       (20)   396732 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2
+-rw-rw-r--   0 vanijzen   (503) staff       (20)    15406 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/favicon.ico
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.051618 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1085 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2184 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2225 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1309 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1062 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2091 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2138 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1258 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1918 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2358 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2411 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2027 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1933 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2361 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2413 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2029 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1731 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2094 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2036 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1779 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1800 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2158 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2039 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1812 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1060 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2116 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2159 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1262 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)      977 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_grouphover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1926 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_hover.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1997 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_pressed.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1153 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_rest.png
+-rw-r--r--   0 vanijzen   (503) staff       (20)      432 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/index.html
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.053062 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/
+-rw-r--r--   0 vanijzen   (503) staff       (20)        0 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/__init__.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2786 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/process_ome_tiff.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2087 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/process_tiff.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2546 2024-04-26 13:29:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/server_helpers.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     5866 2024-04-30 13:27:01.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/server.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2613 2024-04-30 14:20:49.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/watch_folder_docker.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     3730 2024-04-29 08:56:22.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/watch_folder_watchdog.py
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.053866 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     5933 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/PKG-INFO
+-rw-r--r--   0 vanijzen   (503) staff       (20)     6283 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/SOURCES.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)        1 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/dependency_links.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)      121 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/entry_points.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)      374 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/requires.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)       13 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/top_level.txt
```

### Comparing `ImmunoViewer-0.1.5/README.md` & `immunoviewer-0.1.6.dev28/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,23 @@
     * [Install OpenSlide](#install-openslide)
     * [Install from GitHub](#install-from-github)
     * [Install from pip](#install-from-pip)
 * [Usage](#usage)  
     * [Folder structure](#folder-structure)
     * [Generate tiles](#generate-tiles)
     * [Run the viewer](#run-the-viewer)
+* [Acknowledgements](#acknowledgements)
 
 
 ## About ImmunoViewer
 
 ImmunoViewer is a convenient tool for viewing scanned TIF files, particularly those generated by the Keyence Immuno Fluorescence scanner. The viewer allows you to add annotations to the images and supports multi-channel images by saving channels as separate big TIF files. You can customize the color and signal intensity for each channel. We welcome your suggestions for additional features.
 
+<img src="https://github.com/davidvi/ImmunoViewer/raw/main/img/screenshot.jpg" height="500">  
+
 ## Installation
 
 ### Install OpenSlide
 
 ImmunoViewer requires OpenSlide to generate tiled images (not necessary for the viewer). If you use Conda to install ImmunoViewer, it will automatically install OpenSlide.
 
 To install OpenSlide using a Conda environment, run this command:
@@ -75,8 +78,12 @@
 
 ```bash
 ImmunoViewerServer -p [port (default is 5000)] -l [IP address (default = 0.0.0.0)] [data_directory]
 ```
 
 Now you can navigate to http://[IP address]:[port] in your web browser to access ImmunoViewer.
 
-If you leave the IP address to default (0.0.0.0) and the port is exposed to the network other people can also view your slides.  
+If you leave the IP address to default (0.0.0.0) and the port is exposed to the network other people can also view your slides.  
+
+## Acknowledgements 
+
+The script to tile big TIF files was adapted from the [OpenSlide-python repo](https://github.com/openslide/openslide-python).
```

### Comparing `ImmunoViewer-0.1.5/setup.py` & `immunoviewer-0.1.6.dev28/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,78 @@
-import setuptools
+[build-system]
+requires = [
+    "setuptools >= 65",
+    "setuptools_scm[toml]",
+    "wheel",
+]
+build-backend = "setuptools.build_meta"
 
-with open('README.md', 'r', encoding='utf-8') as fh:
-    long_description = fh.read()
+[project]
+name = "ImmunoViewer"
+license = {file = "LICENSE.md"}
+dynamic = ["version"]
+authors = [{ name = "David van IJzendoorn", email = "davidvanijzendoorn@gmail.com" }]
+description = "Explore and annotate your multi-channel large TIF files with this user-friendly viewer."
+keywords = ["big tif", "immuno", "viewer", "annotate", "annotation", "discover", "discovery", "image", "images", "tif", "tiff", "multi-channel", "multi c"]
+readme = "README.md"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Intended Audience :: End Users/Desktop",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3 :: Only",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "click~=8.1.3",
+    "contourpy~=1.0.7",
+    "cycler~=0.11.0",
+    "fonttools~=4.39.0",
+    "itsdangerous~=2.1.2",
+    "jinja2~=3.1.2",
+    "kiwisolver~=1.4.4",
+    "markupsafe~=2.1.2",
+    "matplotlib~=3.7.1",
+    "numpy~=1.24.2",
+    "pillow~=9.4.0",
+    "pyparsing~=3.0.9",
+    "werkzeug~=2.2.3",
+    "watchdog~=4.0.0",
+    "aicsimageio~=4.14.0",
+    "opencv-python~=4.7.0",
+    "gunicorn~=22.0.0",
+    "fastapi~=0.110.2",
+    "uvicorn~=0.29.0",
+    "pydantic-settings~=2.2.1"
+]
+requires-python = ">=3.8"
 
-setuptools.setup(
-    version='0.1.5',
-    name='ImmunoViewer',
-    author='David van IJzendoorn',
-    author_email='davidvanijzendoorn@gmail.com',
-    description='Explore and annotate your multi-channel large TIF files with this user-friendly viewer.',
-    keywords='big tif, immuno, viewer, annotate, annotation, discover, discovery, image, images, tif, tiff, multi-channel, multi c',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/davidvi/ImmunoViewer',
-    project_urls={
-        'Documentation': 'https://github.com/davidvi/ImmunoViewer',
-        'Bug Reports':
-        'https://github.com/davidvi/ImmunoViewer/issues',
-        'Source Code': 'https://github.com/davidvi/ImmunoViewer'
-    },
-    package_dir={'': 'src'},
-    package_data={
-        'ImmunoViewer': ['client/*', 'client/*/*']
-        },
-    packages=setuptools.find_packages(where='src'),
-    classifiers=[
-        # see https://pypi.org/classifiers/
-        'Development Status :: 5 - Production/Stable',
-
-        'Intended Audience :: Developers',
-        'Intended Audience :: End Users/Desktop',
-
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Programming Language :: Python :: 3 :: Only',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-        'flask==2.2.3',
-        'numpy==1.24.2',
-        'openslide-python==1.2.0',
-        'pillow==9.4.0',
-        'opencv-python==4.7.0.72',
-        'matplotlib==3.7.1',
-        'Flask-Cors==3.0.10',
-        ],
-    entry_points={
-    'console_scripts': [
-        'ImmunoViewerProcess=ImmunoViewer.process_folder:main',
-        'ImmunoViewerServer=ImmunoViewer.server:main',
-    ],
-},
-)
+[project.urls]
+"Homepage" = "https://github.com/davidvi/ImmunoViewer"
+"Source" = "https://github.com/davidvi/ImmunoViewer"
+"Bug Reports" = "https://github.com/davidvi/ImmunoViewer/issues"
+"Documentation" = "https://github.com/davidvi/ImmunoViewer"
+
+[project.scripts]
+ImmunoViewerWatch = "ImmunoViewer.watch_folder_docker:main"
+ImmunoViewerServe = "ImmunoViewer.server:main"
+
+[project.optional-dependencies]
+test = [
+    "pytest>=6.0",
+    "mock>=4.0"
+]
+
+[tool.setuptools_scm]
+write_to = "src/ImmunoViewer/_version.py"
+local_scheme = "no-local-version"
+
+[tool.setuptools.packages.find]
+where = ["src"]
```

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js` & `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/index-38ec41fb.css` & `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-38ec41fb.css`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/index-e299d4d6.js` & `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-e299d4d6.js`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot` & `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff` & `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf` & `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2` & `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/fullpage_grouphover.png` & `immunoviewer-0.1.6.dev28/client/public/images/fullpage_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/fullpage_hover.png` & `immunoviewer-0.1.6.dev28/client/public/images/fullpage_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/fullpage_pressed.png` & `immunoviewer-0.1.6.dev28/client/public/images/fullpage_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/fullpage_rest.png` & `immunoviewer-0.1.6.dev28/client/public/images/fullpage_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/home_grouphover.png` & `immunoviewer-0.1.6.dev28/client/public/images/home_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/home_hover.png` & `immunoviewer-0.1.6.dev28/client/public/images/home_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/home_pressed.png` & `immunoviewer-0.1.6.dev28/client/public/images/home_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/home_rest.png` & `immunoviewer-0.1.6.dev28/client/public/images/home_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/next_grouphover.png` & `immunoviewer-0.1.6.dev28/client/public/images/next_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/next_hover.png` & `immunoviewer-0.1.6.dev28/client/public/images/next_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/next_pressed.png` & `immunoviewer-0.1.6.dev28/client/public/images/next_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/next_rest.png` & `immunoviewer-0.1.6.dev28/client/public/images/next_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/previous_grouphover.png` & `immunoviewer-0.1.6.dev28/client/public/images/previous_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/previous_hover.png` & `immunoviewer-0.1.6.dev28/client/public/images/previous_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/previous_pressed.png` & `immunoviewer-0.1.6.dev28/client/public/images/previous_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/previous_rest.png` & `immunoviewer-0.1.6.dev28/client/public/images/previous_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateleft_grouphover.png` & `immunoviewer-0.1.6.dev28/client/public/images/rotateleft_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateleft_hover.png` & `immunoviewer-0.1.6.dev28/client/public/images/rotateleft_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateleft_pressed.png` & `immunoviewer-0.1.6.dev28/client/public/images/rotateleft_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateleft_rest.png` & `immunoviewer-0.1.6.dev28/client/public/images/rotateleft_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateright_grouphover.png` & `immunoviewer-0.1.6.dev28/client/public/images/rotateright_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateright_hover.png` & `immunoviewer-0.1.6.dev28/client/public/images/rotateright_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateright_pressed.png` & `immunoviewer-0.1.6.dev28/client/public/images/rotateright_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/rotateright_rest.png` & `immunoviewer-0.1.6.dev28/client/public/images/rotateright_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomin_grouphover.png` & `immunoviewer-0.1.6.dev28/client/public/images/zoomin_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomin_hover.png` & `immunoviewer-0.1.6.dev28/client/public/images/zoomin_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomin_pressed.png` & `immunoviewer-0.1.6.dev28/client/public/images/zoomin_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomin_rest.png` & `immunoviewer-0.1.6.dev28/client/public/images/zoomin_rest.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomout_grouphover.png` & `immunoviewer-0.1.6.dev28/client/public/images/zoomout_grouphover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomout_hover.png` & `immunoviewer-0.1.6.dev28/client/public/images/zoomout_hover.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomout_pressed.png` & `immunoviewer-0.1.6.dev28/client/public/images/zoomout_pressed.png`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.5/src/ImmunoViewer/client/images/zoomout_rest.png` & `immunoviewer-0.1.6.dev28/client/public/images/zoomout_rest.png`

 * *Files identical despite different names*

