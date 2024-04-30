# Comparing `tmp/immunoviewer-0.1.6.dev28.tar.gz` & `tmp/immunoviewer-0.2.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immunoviewer-0.1.6.dev28.tar", last modified: Tue Apr 30 15:12:09 2024, max compression
+gzip compressed data, was "immunoviewer-0.2.2.dev0.tar", last modified: Tue Apr 30 15:14:39 2024, max compression
```

## Comparing `immunoviewer-0.1.6.dev28.tar` & `immunoviewer-0.2.2.dev0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.055564 immunoviewer-0.1.6.dev28/
--rw-r--r--   0 vanijzen   (503) staff       (20)     8196 2024-04-29 12:50:44.000000 immunoviewer-0.1.6.dev28/.DS_Store
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.968906 immunoviewer-0.1.6.dev28/.github/
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.981236 immunoviewer-0.1.6.dev28/.github/workflows/
--rw-r--r--   0 vanijzen   (503) staff       (20)      342 2024-04-29 11:11:25.000000 immunoviewer-0.1.6.dev28/.github/workflows/push.yml
--rw-r--r--   0 vanijzen   (503) staff       (20)      767 2024-04-30 14:35:28.000000 immunoviewer-0.1.6.dev28/.github/workflows/release.yml
--rw-r--r--   0 vanijzen   (503) staff       (20)     3096 2024-04-12 07:04:08.000000 immunoviewer-0.1.6.dev28/.gitignore
--rw-r--r--   0 vanijzen   (503) staff       (20)      962 2024-04-29 08:33:00.000000 immunoviewer-0.1.6.dev28/Dockerfile
--rw-r--r--   0 vanijzen   (503) staff       (20)      849 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/LICENSE.md
--rw-r--r--   0 vanijzen   (503) staff       (20)     5933 2024-04-30 15:12:09.055436 immunoviewer-0.1.6.dev28/PKG-INFO
--rw-r--r--   0 vanijzen   (503) staff       (20)     2794 2023-05-04 15:54:42.000000 immunoviewer-0.1.6.dev28/README.md
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.986282 immunoviewer-0.1.6.dev28/client/
--rw-r--r--   0 vanijzen   (503) staff       (20)      297 2023-04-26 20:22:56.000000 immunoviewer-0.1.6.dev28/client/.gitignore
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.986617 immunoviewer-0.1.6.dev28/client/.vscode/
--rw-r--r--   0 vanijzen   (503) staff       (20)       75 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/.vscode/extensions.json
--rw-r--r--   0 vanijzen   (503) staff       (20)      630 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/README.md
--rw-r--r--   0 vanijzen   (503) staff       (20)      340 2023-04-26 17:08:39.000000 immunoviewer-0.1.6.dev28/client/index.html
--rw-r--r--   0 vanijzen   (503) staff       (20)   143490 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/package-lock.json
--rw-r--r--   0 vanijzen   (503) staff       (20)      630 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/package.json
--rw-r--r--   0 vanijzen   (503) staff       (20)       82 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/postcss.config.js
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.987885 immunoviewer-0.1.6.dev28/client/public/
--rw-rw-r--   0 vanijzen   (503) staff       (20)    15406 2024-04-25 06:42:54.000000 immunoviewer-0.1.6.dev28/client/public/favicon.ico
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.004025 immunoviewer-0.1.6.dev28/client/public/images/
--rw-r--r--   0 vanijzen   (503) staff       (20)     1085 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/fullpage_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2184 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/fullpage_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2225 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/fullpage_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1309 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/fullpage_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1062 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/home_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2091 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/home_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2138 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/home_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1258 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/home_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1918 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/next_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2358 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/next_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2411 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/next_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2027 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/next_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1933 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/previous_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2361 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/previous_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2413 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/previous_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2029 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/previous_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1731 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateleft_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2094 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateleft_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2036 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateleft_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1779 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateleft_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1800 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateright_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2158 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateright_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2039 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateright_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1812 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/rotateright_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1060 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomin_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2116 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomin_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2159 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomin_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1262 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomin_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)      977 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomout_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1926 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomout_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1997 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomout_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1153 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/public/images/zoomout_rest.png
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.004710 immunoviewer-0.1.6.dev28/client/src/
--rw-r--r--   0 vanijzen   (503) staff       (20)      119 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/App.vue
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.005419 immunoviewer-0.1.6.dev28/client/src/assets/
--rw-r--r--   0 vanijzen   (503) staff       (20)     2037 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/assets/base.css
--rw-r--r--   0 vanijzen   (503) staff       (20)      276 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/assets/logo.svg
--rw-r--r--   0 vanijzen   (503) staff       (20)      477 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/assets/main.css
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.971280 immunoviewer-0.1.6.dev28/client/src/components/
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.006555 immunoviewer-0.1.6.dev28/client/src/components/icons/
--rw-r--r--   0 vanijzen   (503) staff       (20)     1054 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconCommunity.vue
--rw-r--r--   0 vanijzen   (503) staff       (20)     1254 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconDocumentation.vue
--rw-r--r--   0 vanijzen   (503) staff       (20)     1977 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconEcosystem.vue
--rw-r--r--   0 vanijzen   (503) staff       (20)      288 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconSupport.vue
--rw-r--r--   0 vanijzen   (503) staff       (20)      913 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/components/icons/IconTooling.vue
--rw-r--r--   0 vanijzen   (503) staff       (20)       60 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/src/index.css
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.007069 immunoviewer-0.1.6.dev28/client/src/js/
--rw-r--r--   0 vanijzen   (503) staff       (20)    23862 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/js/openseadragon-scalebar.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   906910 2023-04-26 17:08:41.000000 immunoviewer-0.1.6.dev28/client/src/js/openseadragon.js
--rw-r--r--   0 vanijzen   (503) staff       (20)      773 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/src/main.js
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.007785 immunoviewer-0.1.6.dev28/client/src/router/
--rw-r--r--   0 vanijzen   (503) staff       (20)      297 2024-04-19 07:10:32.000000 immunoviewer-0.1.6.dev28/client/src/router/index.js
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.008020 immunoviewer-0.1.6.dev28/client/src/store/
--rw-r--r--   0 vanijzen   (503) staff       (20)     5359 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/src/store/index.js
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.008318 immunoviewer-0.1.6.dev28/client/src/views/
--rw-r--r--   0 vanijzen   (503) staff       (20)    11985 2024-04-29 07:35:34.000000 immunoviewer-0.1.6.dev28/client/src/views/SlideViewer.vue
--rw-r--r--   0 vanijzen   (503) staff       (20)      182 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/client/tailwind.config.js
--rw-r--r--   0 vanijzen   (503) staff       (20)      356 2023-04-26 21:40:47.000000 immunoviewer-0.1.6.dev28/client/vite.config.js
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.008991 immunoviewer-0.1.6.dev28/cloud-deploy/
--rw-r--r--   0 vanijzen   (503) staff       (20)      804 2024-04-29 08:23:59.000000 immunoviewer-0.1.6.dev28/cloud-deploy/Dockerfile
--rw-r--r--   0 vanijzen   (503) staff       (20)        0 2024-04-19 10:40:43.000000 immunoviewer-0.1.6.dev28/cloud-deploy/README.md
--rw-r--r--   0 vanijzen   (503) staff       (20)      324 2024-04-29 08:34:46.000000 immunoviewer-0.1.6.dev28/cloud-deploy/requirements.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      611 2024-04-29 08:59:06.000000 immunoviewer-0.1.6.dev28/environment.yml
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.009514 immunoviewer-0.1.6.dev28/img/
--rw-r--r--   0 vanijzen   (503) staff       (20)     6148 2023-04-27 16:52:22.000000 immunoviewer-0.1.6.dev28/img/.DS_Store
--rw-r--r--   0 vanijzen   (503) staff       (20)   552037 2023-04-27 16:52:09.000000 immunoviewer-0.1.6.dev28/img/screenshot.jpg
--rw-r--r--   0 vanijzen   (503) staff       (20)      230 2024-04-29 09:05:06.000000 immunoviewer-0.1.6.dev28/meta.yaml
--rw-r--r--   0 vanijzen   (503) staff       (20)     2372 2024-04-30 15:11:03.000000 immunoviewer-0.1.6.dev28/pyproject.toml
--rw-r--r--   0 vanijzen   (503) staff       (20)      322 2024-04-29 10:43:47.000000 immunoviewer-0.1.6.dev28/requirements.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)       94 2024-04-30 15:12:09.057393 immunoviewer-0.1.6.dev28/setup.cfg
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:08.973278 immunoviewer-0.1.6.dev28/src/
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.010945 immunoviewer-0.1.6.dev28/src/ImmunoViewer/
--rw-r--r--   0 vanijzen   (503) staff       (20)      205 2024-04-29 11:42:22.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/__init__.py
--rw-r--r--   0 vanijzen   (503) staff       (20)      426 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/_version.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.014724 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.030620 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/
--rw-r--r--   0 vanijzen   (503) staff       (20)      772 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-13d6bf50.css
--rw-r--r--   0 vanijzen   (503) staff       (20)   251090 2024-04-19 07:17:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-44b07d73.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   280297 2023-06-08 01:30:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js
--rw-r--r--   0 vanijzen   (503) staff       (20)      127 2023-06-08 01:30:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-73b8a8f8.css
--rw-r--r--   0 vanijzen   (503) staff       (20)      246 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-a4917311.css
--rw-r--r--   0 vanijzen   (503) staff       (20)   251142 2024-04-19 11:01:41.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-acc75342.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   256208 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-c345c42b.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   251142 2024-04-19 10:56:39.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-cac74aba.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   256213 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-d9842cde.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   252693 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-dfaf7abb.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   249629 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-2d6a5d9a.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   249719 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-7aec11c6.js
--rw-r--r--   0 vanijzen   (503) staff       (20)      678 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-e1bcd4c6.css
--rw-r--r--   0 vanijzen   (503) staff       (20)   249719 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-ec6e481a.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   123736 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-16c8f7df.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   399766 2024-04-19 10:56:39.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-1a44217b.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   399634 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-26efefc2.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   399766 2024-04-19 11:01:41.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-36ec0fef.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   731759 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-38ec41fb.css
--rw-r--r--   0 vanijzen   (503) staff       (20)   399684 2024-04-19 07:17:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-8ddde4e4.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   123736 2024-04-29 07:23:03.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-ab2b0f89.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   399624 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-d030ddc6.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   400172 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-d0c0c412.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   353701 2023-06-08 01:30:48.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-e299d4d6.js
--rw-r--r--   0 vanijzen   (503) staff       (20)   399634 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-e540ed02.js
--rw-r--r--   0 vanijzen   (503) staff       (20)     8285 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-f65d5671.css
--rw-r--r--   0 vanijzen   (503) staff       (20)  1280212 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot
--rw-r--r--   0 vanijzen   (503) staff       (20)   576748 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff
--rw-r--r--   0 vanijzen   (503) staff       (20)  1279992 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf
--rw-r--r--   0 vanijzen   (503) staff       (20)   396732 2024-04-26 14:34:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2
--rw-rw-r--   0 vanijzen   (503) staff       (20)    15406 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/favicon.ico
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.051618 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/
--rw-r--r--   0 vanijzen   (503) staff       (20)     1085 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2184 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2225 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1309 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1062 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2091 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2138 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1258 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1918 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2358 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2411 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2027 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1933 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2361 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2413 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2029 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1731 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2094 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2036 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1779 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1800 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2158 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2039 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1812 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1060 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2116 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     2159 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1262 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)      977 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_grouphover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1926 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_hover.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1997 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_pressed.png
--rw-r--r--   0 vanijzen   (503) staff       (20)     1153 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_rest.png
--rw-r--r--   0 vanijzen   (503) staff       (20)      432 2024-04-29 07:41:05.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/index.html
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.053062 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/
--rw-r--r--   0 vanijzen   (503) staff       (20)        0 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/__init__.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     2786 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/process_ome_tiff.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     2087 2024-04-19 07:10:04.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/process_tiff.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     2546 2024-04-26 13:29:28.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/server_helpers.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     5866 2024-04-30 13:27:01.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/server.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     2613 2024-04-30 14:20:49.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/watch_folder_docker.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     3730 2024-04-29 08:56:22.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer/watch_folder_watchdog.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2024-04-30 15:12:09.053866 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/
--rw-r--r--   0 vanijzen   (503) staff       (20)     5933 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/PKG-INFO
--rw-r--r--   0 vanijzen   (503) staff       (20)     6283 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/SOURCES.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)        1 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/dependency_links.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      121 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/entry_points.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      374 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/requires.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)       13 2024-04-30 15:12:08.000000 immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.532053 immunoviewer-0.2.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.492053 immunoviewer-0.2.2.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.496053 immunoviewer-0.2.2.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-30 15:14:39.532053 immunoviewer-0.2.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.496053 immunoviewer-0.2.2.dev0/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.496053 immunoviewer-0.2.2.dev0/client/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   143490 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/postcss.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.496053 immunoviewer-0.2.2.dev0/client/public/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.504053 immunoviewer-0.2.2.dev0/client/public/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/fullpage_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/fullpage_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/fullpage_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/fullpage_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/home_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/home_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/home_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/home_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/next_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/next_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/next_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/next_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/previous_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/previous_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/previous_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/previous_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/rotateleft_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/rotateleft_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/rotateleft_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/rotateleft_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/rotateright_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/rotateright_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/rotateright_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/rotateright_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/zoomin_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/zoomin_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/zoomin_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/zoomin_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/zoomout_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/zoomout_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/zoomout_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/public/images/zoomout_rest.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.504053 immunoviewer-0.2.2.dev0/client/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/App.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.504053 immunoviewer-0.2.2.dev0/client/src/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/assets/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/assets/main.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.492053 immunoviewer-0.2.2.dev0/client/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.504053 immunoviewer-0.2.2.dev0/client/src/components/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/components/icons/IconCommunity.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/components/icons/IconDocumentation.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/components/icons/IconEcosystem.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/components/icons/IconSupport.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/components/icons/IconTooling.vue
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/index.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.504053 immunoviewer-0.2.2.dev0/client/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    23862 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/js/openseadragon-scalebar.js
+-rw-r--r--   0 runner    (1001) docker     (127)   906910 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/js/openseadragon.js
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.504053 immunoviewer-0.2.2.dev0/client/src/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/router/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.508053 immunoviewer-0.2.2.dev0/client/src/store/
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/store/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.508053 immunoviewer-0.2.2.dev0/client/src/views/
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/src/views/SlideViewer.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/tailwind.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/client/vite.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.508053 immunoviewer-0.2.2.dev0/cloud-deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/cloud-deploy/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/cloud-deploy/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/cloud-deploy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.508053 immunoviewer-0.2.2.dev0/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/img/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)   552037 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/img/screenshot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 15:14:39.536053 immunoviewer-0.2.2.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.496053 immunoviewer-0.2.2.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.508053 immunoviewer-0.2.2.dev0/src/ImmunoViewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 15:14:39.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.508053 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.528053 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-13d6bf50.css
+-rw-r--r--   0 runner    (1001) docker     (127)   251090 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-44b07d73.js
+-rw-r--r--   0 runner    (1001) docker     (127)   280297 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-73b8a8f8.css
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-a4917311.css
+-rw-r--r--   0 runner    (1001) docker     (127)   251142 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-acc75342.js
+-rw-r--r--   0 runner    (1001) docker     (127)   256208 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-c345c42b.js
+-rw-r--r--   0 runner    (1001) docker     (127)   251142 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-cac74aba.js
+-rw-r--r--   0 runner    (1001) docker     (127)   256213 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-d9842cde.js
+-rw-r--r--   0 runner    (1001) docker     (127)   252693 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-dfaf7abb.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249629 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewerNew-2d6a5d9a.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249719 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewerNew-7aec11c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewerNew-e1bcd4c6.css
+-rw-r--r--   0 runner    (1001) docker     (127)   249719 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewerNew-ec6e481a.js
+-rw-r--r--   0 runner    (1001) docker     (127)   123736 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-16c8f7df.js
+-rw-r--r--   0 runner    (1001) docker     (127)   399766 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-1a44217b.js
+-rw-r--r--   0 runner    (1001) docker     (127)   399634 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-26efefc2.js
+-rw-r--r--   0 runner    (1001) docker     (127)   399766 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-36ec0fef.js
+-rw-r--r--   0 runner    (1001) docker     (127)   731759 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-38ec41fb.css
+-rw-r--r--   0 runner    (1001) docker     (127)   399684 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-8ddde4e4.js
+-rw-r--r--   0 runner    (1001) docker     (127)   123736 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-ab2b0f89.js
+-rw-r--r--   0 runner    (1001) docker     (127)   399624 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-d030ddc6.js
+-rw-r--r--   0 runner    (1001) docker     (127)   400172 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-d0c0c412.js
+-rw-r--r--   0 runner    (1001) docker     (127)   353701 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-e299d4d6.js
+-rw-r--r--   0 runner    (1001) docker     (127)   399634 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-e540ed02.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-f65d5671.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1280212 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   576748 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)  1279992 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   396732 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.532053 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/fullpage_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/fullpage_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/fullpage_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/fullpage_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/home_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/home_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/home_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/home_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/next_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/next_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/next_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/next_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/previous_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/previous_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/previous_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/previous_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateleft_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateleft_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateleft_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateleft_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateright_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateright_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateright_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateright_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomin_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomin_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomin_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomin_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomout_grouphover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomout_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomout_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomout_rest.png
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.532053 immunoviewer-0.2.2.dev0/src/ImmunoViewer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/helpers/process_ome_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/helpers/process_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/helpers/server_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/watch_folder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-30 15:14:26.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer/watch_folder_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:39.532053 immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-30 15:14:39.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-30 15:14:39.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:14:39.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-30 15:14:39.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 15:14:39.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 15:14:39.000000 immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/top_level.txt
```

### Comparing `immunoviewer-0.1.6.dev28/.DS_Store` & `immunoviewer-0.2.2.dev0/.DS_Store`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/.github/workflows/release.yml` & `immunoviewer-0.2.2.dev0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/.gitignore` & `immunoviewer-0.2.2.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/Dockerfile` & `immunoviewer-0.2.2.dev0/Dockerfile`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/LICENSE.md` & `immunoviewer-0.2.2.dev0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/PKG-INFO` & `immunoviewer-0.2.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImmunoViewer
-Version: 0.1.6.dev28
+Version: 0.2.2.dev0
 Summary: Explore and annotate your multi-channel large TIF files with this user-friendly viewer.
 Author-email: David van IJzendoorn <davidvanijzendoorn@gmail.com>
 License: Creative Commons Attribution-NonCommercial 4.0 International License
         
         Copyright (c) 2023 David van IJzendoorn
         
         This work is licensed under a Creative Commons Attribution-NonCommercial 4.0 International License.
```

### Comparing `immunoviewer-0.1.6.dev28/README.md` & `immunoviewer-0.2.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/README.md` & `immunoviewer-0.2.2.dev0/client/README.md`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/package-lock.json` & `immunoviewer-0.2.2.dev0/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/package.json` & `immunoviewer-0.2.2.dev0/client/package.json`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/favicon.ico` & `immunoviewer-0.2.2.dev0/client/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/fullpage_grouphover.png` & `immunoviewer-0.2.2.dev0/client/public/images/fullpage_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/fullpage_hover.png` & `immunoviewer-0.2.2.dev0/client/public/images/fullpage_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/fullpage_pressed.png` & `immunoviewer-0.2.2.dev0/client/public/images/fullpage_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/fullpage_rest.png` & `immunoviewer-0.2.2.dev0/client/public/images/fullpage_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/home_grouphover.png` & `immunoviewer-0.2.2.dev0/client/public/images/home_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/home_hover.png` & `immunoviewer-0.2.2.dev0/client/public/images/home_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/home_pressed.png` & `immunoviewer-0.2.2.dev0/client/public/images/home_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/home_rest.png` & `immunoviewer-0.2.2.dev0/client/public/images/home_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/next_grouphover.png` & `immunoviewer-0.2.2.dev0/client/public/images/next_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/next_hover.png` & `immunoviewer-0.2.2.dev0/client/public/images/next_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/next_pressed.png` & `immunoviewer-0.2.2.dev0/client/public/images/next_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/next_rest.png` & `immunoviewer-0.2.2.dev0/client/public/images/next_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/previous_grouphover.png` & `immunoviewer-0.2.2.dev0/client/public/images/previous_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/previous_hover.png` & `immunoviewer-0.2.2.dev0/client/public/images/previous_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/previous_pressed.png` & `immunoviewer-0.2.2.dev0/client/public/images/previous_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/previous_rest.png` & `immunoviewer-0.2.2.dev0/client/public/images/previous_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/rotateleft_grouphover.png` & `immunoviewer-0.2.2.dev0/client/public/images/rotateleft_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/rotateleft_hover.png` & `immunoviewer-0.2.2.dev0/client/public/images/rotateleft_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/rotateleft_pressed.png` & `immunoviewer-0.2.2.dev0/client/public/images/rotateleft_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/rotateleft_rest.png` & `immunoviewer-0.2.2.dev0/client/public/images/rotateleft_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/rotateright_grouphover.png` & `immunoviewer-0.2.2.dev0/client/public/images/rotateright_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/rotateright_hover.png` & `immunoviewer-0.2.2.dev0/client/public/images/rotateright_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/rotateright_pressed.png` & `immunoviewer-0.2.2.dev0/client/public/images/rotateright_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/rotateright_rest.png` & `immunoviewer-0.2.2.dev0/client/public/images/rotateright_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/zoomin_grouphover.png` & `immunoviewer-0.2.2.dev0/client/public/images/zoomin_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/zoomin_hover.png` & `immunoviewer-0.2.2.dev0/client/public/images/zoomin_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/zoomin_pressed.png` & `immunoviewer-0.2.2.dev0/client/public/images/zoomin_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/zoomin_rest.png` & `immunoviewer-0.2.2.dev0/client/public/images/zoomin_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/zoomout_grouphover.png` & `immunoviewer-0.2.2.dev0/client/public/images/zoomout_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/zoomout_hover.png` & `immunoviewer-0.2.2.dev0/client/public/images/zoomout_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/zoomout_pressed.png` & `immunoviewer-0.2.2.dev0/client/public/images/zoomout_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/public/images/zoomout_rest.png` & `immunoviewer-0.2.2.dev0/client/public/images/zoomout_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/assets/base.css` & `immunoviewer-0.2.2.dev0/client/src/assets/base.css`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/components/icons/IconCommunity.vue` & `immunoviewer-0.2.2.dev0/client/src/components/icons/IconCommunity.vue`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/components/icons/IconDocumentation.vue` & `immunoviewer-0.2.2.dev0/client/src/components/icons/IconDocumentation.vue`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/components/icons/IconEcosystem.vue` & `immunoviewer-0.2.2.dev0/client/src/components/icons/IconEcosystem.vue`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/components/icons/IconTooling.vue` & `immunoviewer-0.2.2.dev0/client/src/components/icons/IconTooling.vue`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/js/openseadragon-scalebar.js` & `immunoviewer-0.2.2.dev0/client/src/js/openseadragon-scalebar.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/js/openseadragon.js` & `immunoviewer-0.2.2.dev0/client/src/js/openseadragon.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/main.js` & `immunoviewer-0.2.2.dev0/client/src/main.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/store/index.js` & `immunoviewer-0.2.2.dev0/client/src/store/index.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/client/src/views/SlideViewer.vue` & `immunoviewer-0.2.2.dev0/client/src/views/SlideViewer.vue`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/cloud-deploy/Dockerfile` & `immunoviewer-0.2.2.dev0/cloud-deploy/Dockerfile`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/environment.yml` & `immunoviewer-0.2.2.dev0/environment.yml`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/img/.DS_Store` & `immunoviewer-0.2.2.dev0/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/img/screenshot.jpg` & `immunoviewer-0.2.2.dev0/img/screenshot.jpg`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/pyproject.toml` & `immunoviewer-0.2.2.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-13d6bf50.css` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-13d6bf50.css`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-44b07d73.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-44b07d73.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-4db2fbd9.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-acc75342.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-acc75342.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-c345c42b.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-c345c42b.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-cac74aba.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-cac74aba.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-d9842cde.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-d9842cde.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewer-dfaf7abb.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewer-dfaf7abb.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-2d6a5d9a.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewerNew-2d6a5d9a.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-7aec11c6.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewerNew-7aec11c6.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-e1bcd4c6.css` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewerNew-e1bcd4c6.css`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/SlideViewerNew-ec6e481a.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/SlideViewerNew-ec6e481a.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-16c8f7df.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-16c8f7df.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-1a44217b.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-1a44217b.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-26efefc2.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-26efefc2.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-36ec0fef.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-36ec0fef.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-38ec41fb.css` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-38ec41fb.css`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-8ddde4e4.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-8ddde4e4.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-ab2b0f89.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-ab2b0f89.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-d030ddc6.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-d030ddc6.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-d0c0c412.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-d0c0c412.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-e299d4d6.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-e299d4d6.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-e540ed02.js` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-e540ed02.js`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/index-f65d5671.css` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/index-f65d5671.css`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/materialdesignicons-webfont-67d24abe.eot`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/materialdesignicons-webfont-80bb28b3.woff`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/materialdesignicons-webfont-a58ecb54.ttf`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/assets/materialdesignicons-webfont-c1c004a9.woff2`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/favicon.ico` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/favicon.ico`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_grouphover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/fullpage_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_hover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/fullpage_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_pressed.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/fullpage_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/fullpage_rest.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/fullpage_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_grouphover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/home_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_hover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/home_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_pressed.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/home_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/home_rest.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/home_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_grouphover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/next_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_hover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/next_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_pressed.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/next_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/next_rest.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/next_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_grouphover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/previous_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_hover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/previous_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_pressed.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/previous_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/previous_rest.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/previous_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_grouphover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateleft_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_hover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateleft_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_pressed.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateleft_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateleft_rest.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateleft_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_grouphover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateright_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_hover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateright_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_pressed.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateright_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/rotateright_rest.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/rotateright_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_grouphover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomin_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_hover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomin_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_pressed.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomin_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomin_rest.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomin_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_grouphover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomout_grouphover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_hover.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomout_hover.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_pressed.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomout_pressed.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/client/images/zoomout_rest.png` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/client/images/zoomout_rest.png`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/process_ome_tiff.py` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/helpers/process_ome_tiff.py`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/process_tiff.py` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/helpers/process_tiff.py`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/helpers/server_helpers.py` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/helpers/server_helpers.py`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/server.py` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/server.py`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/watch_folder_docker.py` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/watch_folder_docker.py`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer/watch_folder_watchdog.py` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer/watch_folder_watchdog.py`

 * *Files identical despite different names*

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/PKG-INFO` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImmunoViewer
-Version: 0.1.6.dev28
+Version: 0.2.2.dev0
 Summary: Explore and annotate your multi-channel large TIF files with this user-friendly viewer.
 Author-email: David van IJzendoorn <davidvanijzendoorn@gmail.com>
 License: Creative Commons Attribution-NonCommercial 4.0 International License
         
         Copyright (c) 2023 David van IJzendoorn
         
         This work is licensed under a Creative Commons Attribution-NonCommercial 4.0 International License.
```

### Comparing `immunoviewer-0.1.6.dev28/src/ImmunoViewer.egg-info/SOURCES.txt` & `immunoviewer-0.2.2.dev0/src/ImmunoViewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

