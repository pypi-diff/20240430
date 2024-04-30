# Comparing `tmp/sd_prompt_reader-1.3.4.post2.tar.gz` & `tmp/sd_prompt_reader-1.3.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_prompt_reader-1.3.4.post2.tar", max compression
+gzip compressed data, was "sd_prompt_reader-1.3.5b1.tar", max compression
```

## Comparing `sd_prompt_reader-1.3.4.post2.tar` & `sd_prompt_reader-1.3.5b1.tar`

### file list

```diff
@@ -1,73 +1,75 @@
--rw-r--r--   0        0        0     1066 2023-04-09 14:16:43.184257 sd_prompt_reader-1.3.4.post2/LICENSE
--rw-r--r--   0        0        0    13355 2023-10-25 18:38:08.596050 sd_prompt_reader-1.3.4.post2/README.md
--rw-r--r--   0        0        0      987 2024-01-25 14:02:27.118416 sd_prompt_reader-1.3.4.post2/pyproject.toml
--rw-r--r--   0        0        0    10244 2024-01-17 23:14:20.642139 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/.DS_Store
--rw-r--r--   0        0        0      119 2023-09-11 15:13:17.041022 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/__init__.py
--rw-r--r--   0        0        0       24 2024-01-25 14:05:05.299096 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/__version__.py
--rw-r--r--   0        0        0    32741 2023-10-02 20:15:05.632806 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/app.py
--rw-r--r--   0        0        0     4464 2023-09-30 12:48:42.979786 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/button.py
--rw-r--r--   0        0        0     4600 2023-10-02 20:06:25.709709 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/constants.py
--rw-r--r--   0        0        0      374 2023-09-11 15:13:17.044406 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/ctkdnd.py
--rw-r--r--   0        0        0     6148 2024-01-17 23:14:20.644389 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/.DS_Store
--rw-r--r--   0        0        0      368 2023-09-11 15:13:17.044644 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/__init__.py
--rw-r--r--   0        0        0     3923 2024-01-05 22:27:28.387407 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/a1111.py
--rw-r--r--   0        0        0     1919 2023-09-30 12:48:42.981511 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/base_format.py
--rw-r--r--   0        0        0    20143 2023-10-19 23:08:55.736498 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/comfyui.py
--rw-r--r--   0        0        0      979 2023-12-23 08:22:21.119741 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/drawthings.py
--rw-r--r--   0        0        0     2713 2023-09-30 12:48:42.983302 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/easydiffusion.py
--rw-r--r--   0        0        0     1377 2023-09-30 12:48:42.983887 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/fooocus.py
--rw-r--r--   0        0        0     6161 2023-09-30 12:56:12.845232 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/invokeai.py
--rw-r--r--   0        0        0     1362 2023-09-30 12:48:42.985073 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/novelai.py
--rw-r--r--   0        0        0     1851 2023-12-11 12:47:28.807988 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/swarmui.py
--rw-r--r--   0        0        0    10053 2023-12-23 08:24:50.341227 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/image_data_reader.py
--rw-r--r--   0        0        0     6126 2023-09-30 23:12:04.290329 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/parameter_viewer.py
--rw-r--r--   0        0        0    19582 2023-09-30 12:48:42.987332 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/prompt_viewer.py
--rw-r--r--   0        0        0     6148 2023-09-20 15:11:02.029930 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/.DS_Store
--rw-r--r--   0        0        0      119 2023-09-11 15:13:17.048711 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/__init__.py
--rw-r--r--   0        0        0     3239 2023-08-29 22:10:08.112057 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/check_circle_24.png
--rw-r--r--   0        0        0     2076 2023-08-29 22:10:08.112671 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/check_circle_24_alpha.png
--rw-r--r--   0        0        0     1293 2023-08-29 22:10:08.113243 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/cleaning_services_24.png
--rw-r--r--   0        0        0     1036 2023-08-29 22:10:08.113737 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/cleaning_services_24_alpha.png
--rw-r--r--   0        0        0      602 2023-08-29 22:10:08.114163 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/content_copy_20.png
--rw-r--r--   0        0        0      550 2023-08-29 22:10:08.114647 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/content_copy_20_alpha.png
--rw-r--r--   0        0        0      739 2023-08-29 22:10:08.115173 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/content_copy_24.png
--rw-r--r--   0        0        0      621 2023-08-29 22:10:08.115591 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/content_copy_24_alpha.png
--rw-r--r--   0        0        0      751 2023-08-29 22:10:08.116121 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/description_24.png
--rw-r--r--   0        0        0      637 2023-08-29 22:10:08.116635 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/description_24_alpha.png
--rw-r--r--   0        0        0     1226 2023-08-29 22:10:08.117090 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/edit_24.png
--rw-r--r--   0        0        0      905 2023-08-29 22:10:08.117558 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/edit_24_alpha.png
--rw-r--r--   0        0        0     2016 2023-08-29 22:10:08.117987 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/edit_off_24.png
--rw-r--r--   0        0        0     1368 2023-08-29 22:10:08.118427 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/edit_off_24_alpha.png
--rw-r--r--   0        0        0     3062 2023-08-29 22:10:08.118883 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/error_24.png
--rw-r--r--   0        0        0     1964 2023-08-29 22:10:08.119345 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/error_24_alpha.png
--rw-r--r--   0        0        0      589 2023-08-29 22:10:08.119873 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/expand_more_24.png
--rw-r--r--   0        0        0      585 2023-08-29 22:10:08.120398 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/expand_more_24_alpha.png
--rw-r--r--   0        0        0     4510 2023-08-29 22:10:08.120632 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/gray.json
--rw-r--r--   0        0        0  1377264 2023-08-29 22:10:08.128049 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/icon.icns
--rw-r--r--   0        0        0   612157 2023-08-29 22:10:08.132165 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/icon.ico
--rw-r--r--   0        0        0   810239 2023-08-29 22:10:08.136339 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/icon.png
--rw-r--r--   0        0        0     3042 2023-08-29 22:10:08.136928 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/info_24.png
--rw-r--r--   0        0        0     1966 2023-08-29 22:10:08.137427 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/info_24_alpha.png
--rw-r--r--   0        0        0     1683 2023-08-29 22:10:08.138125 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/lightbulb_20.png
--rw-r--r--   0        0        0     1453 2023-08-29 22:10:08.138711 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/lightbulb_20_alpha.png
--rw-r--r--   0        0        0     1426 2023-08-29 22:10:08.139223 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/mop_24.png
--rw-r--r--   0        0        0     1109 2023-08-29 22:10:08.139580 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/mop_24_alpha.png
--rw-r--r--   0        0        0     1740 2023-08-29 22:10:08.139870 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/place_item_48.png
--rw-r--r--   0        0        0     1334 2023-08-29 22:10:08.140198 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/place_item_48_alpha.png
--rw-r--r--   0        0        0     1241 2023-08-29 22:10:08.140544 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/save_24.png
--rw-r--r--   0        0        0      946 2023-08-29 22:10:08.140887 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/save_24_alpha.png
--rw-r--r--   0        0        0     1619 2023-08-29 22:10:08.141189 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/sort_by_alpha_20.png
--rw-r--r--   0        0        0     1377 2023-08-29 22:10:08.141490 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png
--rw-r--r--   0        0        0     2732 2023-08-29 22:10:08.141811 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/update_24.png
--rw-r--r--   0        0        0     1937 2023-08-29 22:10:08.142161 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/update_24_alpha.png
--rw-r--r--   0        0        0      632 2023-09-11 15:13:17.048912 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/view_sidebar_20.png
--rw-r--r--   0        0        0      615 2023-09-11 15:13:17.049108 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/view_sidebar_20_alpha.png
--rw-r--r--   0        0        0      560 2023-09-11 15:13:17.049302 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/view_week_20.png
--rw-r--r--   0        0        0      545 2023-09-11 15:13:17.049498 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/view_week_20_alpha.png
--rw-r--r--   0        0        0     2258 2023-08-29 22:10:08.144127 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/warning_24.png
--rw-r--r--   0        0        0     1658 2023-08-29 22:10:08.144441 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/warning_24_alpha.png
--rw-r--r--   0        0        0     2913 2023-10-02 20:06:25.710878 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/status_bar.py
--rw-r--r--   0        0        0     3985 2023-09-30 12:48:42.988373 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/textbox.py
--rw-r--r--   0        0        0     1167 2023-09-30 12:48:42.988731 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/update_checker.py
--rw-r--r--   0        0        0     4200 2023-09-30 12:48:42.989399 sd_prompt_reader-1.3.4.post2/sd_prompt_reader/utility.py
--rw-r--r--   0        0        0    14299 1970-01-01 00:00:00.000000 sd_prompt_reader-1.3.4.post2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-09 14:16:43.184257 sd_prompt_reader-1.3.5b1/LICENSE
+-rw-r--r--   0        0        0    16866 2024-04-30 16:03:46.478493 sd_prompt_reader-1.3.5b1/README.md
+-rw-r--r--   0        0        0     1033 2024-04-30 16:00:45.792394 sd_prompt_reader-1.3.5b1/pyproject.toml
+-rw-r--r--   0        0        0    10244 2024-04-30 15:41:51.274726 sd_prompt_reader-1.3.5b1/sd_prompt_reader/.DS_Store
+-rw-r--r--   0        0        0      119 2023-09-11 15:13:17.041022 sd_prompt_reader-1.3.5b1/sd_prompt_reader/__init__.py
+-rw-r--r--   0        0        0       20 2024-04-30 16:09:22.373493 sd_prompt_reader-1.3.5b1/sd_prompt_reader/__version__.py
+-rw-r--r--   0        0        0    33371 2024-04-24 20:33:49.648741 sd_prompt_reader-1.3.5b1/sd_prompt_reader/app.py
+-rw-r--r--   0        0        0     4464 2023-09-30 12:48:42.979786 sd_prompt_reader-1.3.5b1/sd_prompt_reader/button.py
+-rw-r--r--   0        0        0    12829 2024-04-23 19:14:30.193577 sd_prompt_reader-1.3.5b1/sd_prompt_reader/cli.py
+-rw-r--r--   0        0        0     4997 2024-03-21 13:25:50.368703 sd_prompt_reader-1.3.5b1/sd_prompt_reader/constants.py
+-rw-r--r--   0        0        0      374 2023-09-11 15:13:17.044406 sd_prompt_reader-1.3.5b1/sd_prompt_reader/ctkdnd.py
+-rw-r--r--   0        0        0     6148 2024-04-25 20:30:42.459491 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/.DS_Store
+-rw-r--r--   0        0        0      404 2024-03-21 13:25:50.369729 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/__init__.py
+-rw-r--r--   0        0        0     4208 2024-03-21 15:43:32.269504 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/a1111.py
+-rw-r--r--   0        0        0     2601 2024-04-23 19:14:30.193953 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/base_format.py
+-rw-r--r--   0        0        0    20917 2024-04-24 20:26:31.436939 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/comfyui.py
+-rw-r--r--   0        0        0     1004 2024-03-21 13:25:50.372554 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/drawthings.py
+-rw-r--r--   0        0        0     2738 2024-03-21 13:25:50.373098 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/easydiffusion.py
+-rw-r--r--   0        0        0     1402 2024-03-21 13:25:50.373744 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/fooocus.py
+-rw-r--r--   0        0        0     6178 2024-04-25 09:51:40.283772 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/invokeai.py
+-rw-r--r--   0        0        0     4464 2024-04-30 15:51:30.127491 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/novelai.py
+-rw-r--r--   0        0        0     1876 2024-03-21 13:25:50.375371 sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/swarmui.py
+-rw-r--r--   0        0        0    13157 2024-04-30 15:51:30.109283 sd_prompt_reader-1.3.5b1/sd_prompt_reader/image_data_reader.py
+-rw-r--r--   0        0        0     2401 2024-04-23 19:14:30.194590 sd_prompt_reader-1.3.5b1/sd_prompt_reader/logger.py
+-rw-r--r--   0        0        0     6126 2023-09-30 23:12:04.290329 sd_prompt_reader-1.3.5b1/sd_prompt_reader/parameter_viewer.py
+-rw-r--r--   0        0        0    19582 2023-09-30 12:48:42.987332 sd_prompt_reader-1.3.5b1/sd_prompt_reader/prompt_viewer.py
+-rw-r--r--   0        0        0     6148 2023-09-20 15:11:02.029930 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/.DS_Store
+-rw-r--r--   0        0        0      119 2023-09-11 15:13:17.048711 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/__init__.py
+-rw-r--r--   0        0        0     3239 2023-08-29 22:10:08.112057 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/check_circle_24.png
+-rw-r--r--   0        0        0     2076 2023-08-29 22:10:08.112671 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/check_circle_24_alpha.png
+-rw-r--r--   0        0        0     1293 2023-08-29 22:10:08.113243 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/cleaning_services_24.png
+-rw-r--r--   0        0        0     1036 2023-08-29 22:10:08.113737 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/cleaning_services_24_alpha.png
+-rw-r--r--   0        0        0      602 2023-08-29 22:10:08.114163 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/content_copy_20.png
+-rw-r--r--   0        0        0      550 2023-08-29 22:10:08.114647 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/content_copy_20_alpha.png
+-rw-r--r--   0        0        0      739 2023-08-29 22:10:08.115173 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/content_copy_24.png
+-rw-r--r--   0        0        0      621 2023-08-29 22:10:08.115591 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/content_copy_24_alpha.png
+-rw-r--r--   0        0        0      751 2023-08-29 22:10:08.116121 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/description_24.png
+-rw-r--r--   0        0        0      637 2023-08-29 22:10:08.116635 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/description_24_alpha.png
+-rw-r--r--   0        0        0     1226 2023-08-29 22:10:08.117090 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/edit_24.png
+-rw-r--r--   0        0        0      905 2023-08-29 22:10:08.117558 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/edit_24_alpha.png
+-rw-r--r--   0        0        0     2016 2023-08-29 22:10:08.117987 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/edit_off_24.png
+-rw-r--r--   0        0        0     1368 2023-08-29 22:10:08.118427 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/edit_off_24_alpha.png
+-rw-r--r--   0        0        0     3062 2023-08-29 22:10:08.118883 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/error_24.png
+-rw-r--r--   0        0        0     1964 2023-08-29 22:10:08.119345 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/error_24_alpha.png
+-rw-r--r--   0        0        0      589 2023-08-29 22:10:08.119873 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/expand_more_24.png
+-rw-r--r--   0        0        0      585 2023-08-29 22:10:08.120398 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/expand_more_24_alpha.png
+-rw-r--r--   0        0        0     4510 2023-08-29 22:10:08.120632 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/gray.json
+-rw-r--r--   0        0        0  1377264 2023-08-29 22:10:08.128049 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/icon.icns
+-rw-r--r--   0        0        0   612157 2023-08-29 22:10:08.132165 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/icon.ico
+-rw-r--r--   0        0        0   810239 2023-08-29 22:10:08.136339 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/icon.png
+-rw-r--r--   0        0        0     3042 2023-08-29 22:10:08.136928 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/info_24.png
+-rw-r--r--   0        0        0     1966 2023-08-29 22:10:08.137427 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/info_24_alpha.png
+-rw-r--r--   0        0        0     1683 2023-08-29 22:10:08.138125 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/lightbulb_20.png
+-rw-r--r--   0        0        0     1453 2023-08-29 22:10:08.138711 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/lightbulb_20_alpha.png
+-rw-r--r--   0        0        0     1426 2023-08-29 22:10:08.139223 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/mop_24.png
+-rw-r--r--   0        0        0     1109 2023-08-29 22:10:08.139580 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/mop_24_alpha.png
+-rw-r--r--   0        0        0     1740 2023-08-29 22:10:08.139870 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/place_item_48.png
+-rw-r--r--   0        0        0     1334 2023-08-29 22:10:08.140198 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/place_item_48_alpha.png
+-rw-r--r--   0        0        0     1241 2023-08-29 22:10:08.140544 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/save_24.png
+-rw-r--r--   0        0        0      946 2023-08-29 22:10:08.140887 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/save_24_alpha.png
+-rw-r--r--   0        0        0     1619 2023-08-29 22:10:08.141189 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/sort_by_alpha_20.png
+-rw-r--r--   0        0        0     1377 2023-08-29 22:10:08.141490 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png
+-rw-r--r--   0        0        0     2732 2023-08-29 22:10:08.141811 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/update_24.png
+-rw-r--r--   0        0        0     1937 2023-08-29 22:10:08.142161 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/update_24_alpha.png
+-rw-r--r--   0        0        0      632 2023-09-11 15:13:17.048912 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/view_sidebar_20.png
+-rw-r--r--   0        0        0      615 2023-09-11 15:13:17.049108 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/view_sidebar_20_alpha.png
+-rw-r--r--   0        0        0      560 2023-09-11 15:13:17.049302 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/view_week_20.png
+-rw-r--r--   0        0        0      545 2023-09-11 15:13:17.049498 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/view_week_20_alpha.png
+-rw-r--r--   0        0        0     2258 2023-08-29 22:10:08.144127 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/warning_24.png
+-rw-r--r--   0        0        0     1658 2023-08-29 22:10:08.144441 sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/warning_24_alpha.png
+-rw-r--r--   0        0        0     2917 2024-03-21 13:25:50.376674 sd_prompt_reader-1.3.5b1/sd_prompt_reader/status_bar.py
+-rw-r--r--   0        0        0     3985 2023-09-30 12:48:42.988373 sd_prompt_reader-1.3.5b1/sd_prompt_reader/textbox.py
+-rw-r--r--   0        0        0     1171 2024-03-21 13:25:50.377123 sd_prompt_reader-1.3.5b1/sd_prompt_reader/update_checker.py
+-rw-r--r--   0        0        0     4323 2024-03-21 13:25:50.377815 sd_prompt_reader-1.3.5b1/sd_prompt_reader/utility.py
+-rw-r--r--   0        0        0    17806 1970-01-01 00:00:00.000000 sd_prompt_reader-1.3.5b1/PKG-INFO
```

### Comparing `sd_prompt_reader-1.3.4.post2/LICENSE` & `sd_prompt_reader-1.3.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/README.md` & `sd_prompt_reader-1.3.5b1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui.
     <br>
   <p>
     <a href="#features">Features</a> •
     <a href="#supported-formats">Supported Formats</a> •
     <a href="#download">Download</a> •
     <a href="#usage">Usage</a> •
+    <a href="https://github.com/receyuki/comfyui-prompt-reader-node">ComfyUI Node</a> •
+    <a href="#cli">CLI</a> •
+    <a href="#api">API</a> •
     <a href="#faq">FAQ</a> •
     <a href="#credits">Credits</a>
   </p>
     <img src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/screenshot_v134.png">
 </div>
 
 >The SD Prompt Reader is now available as a ComfyUI node. Check out 
@@ -41,25 +44,29 @@
 - Edit or import prompt to images
 - Vertical orientation display and sorting by alphabet
 - Detect generation tool.
 - Multiple formats support.
 - Dark and light mode support.
 
 ## Supported Formats
-|                                                                          | PNG | JPEG | WEBP | TXT* |
-|--------------------------------------------------------------------------|:---:|:----:|:----:|:----:|
-| [A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) |  ✅  |  ✅   |  ✅   |  ✅   |
-| [Easy Diffusion](https://github.com/easydiffusion/easydiffusion)         |  ✅  |  ✅   |  ✅   |      |
-| [StableSwarmUI](https://github.com/Stability-AI/StableSwarmUI)*          |  ✅  |  ✅   |      |      |
-| [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)*               |  ✅  |  ✅   |      |      |
-| [InvokeAI](https://github.com/invoke-ai/InvokeAI)                        |  ✅  |      |      |      |
-| [ComfyUI](https://github.com/comfyanonymous/ComfyUI)*                    |  ✅  |      |      |      |
-| [NovelAI](https://novelai.net/)                                          |  ✅  |      |      |      |
-| [Draw Things](https://drawthings.ai/)                                    |  ✅  |      |      |      |
-| Naifu(4chan)                                                             |  ✅  |      |      |      |
+|                                                                                        | PNG | JPEG | WEBP | TXT* |
+|----------------------------------------------------------------------------------------|:---:|:----:|:----:|:----:|
+| [A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui)               |  ✅  |  ✅   |  ✅   |  ✅   |
+| [Easy Diffusion](https://github.com/easydiffusion/easydiffusion)                       |  ✅  |  ✅   |  ✅   |      |
+| [StableSwarmUI](https://github.com/Stability-AI/StableSwarmUI)*                        |  ✅  |  ✅   |      |      |
+| [StableSwarmUI (prior to 0.5.8-alpha)](https://github.com/Stability-AI/StableSwarmUI)* |  ✅  |  ✅   |      |      |
+| [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)*                             |  ✅  |  ✅   |      |      |
+| [InvokeAI](https://github.com/invoke-ai/InvokeAI)                                      |  ✅  |      |      |      |
+| [InvokeAI (prior to 2.3.5-post.2)](https://github.com/invoke-ai/InvokeAI)              |  ✅  |      |      |      |
+| [InvokeAI (prior to 1.15)](https://github.com/invoke-ai/InvokeAI)                      |  ✅  |      |      |      |
+| [ComfyUI](https://github.com/comfyanonymous/ComfyUI)*                                  |  ✅  |      |      |      |
+| [Draw Things](https://drawthings.ai/)                                                  |  ✅  |      |      |      |
+| [NovelAI (stealth pnginfo)](https://novelai.net/)                                      |  ✅  |      |      |      |
+| [NovelAI (legacy)](https://novelai.net/)                                               |  ✅  |      |      |      |
+| Naifu(4chan)                                                                           |  ✅  |      |      |      |
 
 \* Limitations apply. See [format limitations](#TXT).
 
 If you are using a tool or format that is not on this list, please help me to support your format 
 by uploading the original file generated by your tool to the issues, thx.
 
 For ComfyUI users, the SD Prompt Reader is now available as a ComfyUI node. 
@@ -165,30 +172,91 @@
 ***The SDXL workflow does not support editing. 
 If necessary, please remove prompts from image before edit.***  
 If the image's workflow includes multiple sets of SDXL prompts, 
 namely Clip G(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch to the multi-set prompt display mode as shown in the image below. 
 There are two interface options available for the multi-set prompt display mode, and you can switch between them using buttons.  
 ![comfyui_sdxl.png](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png)
 
+## CLI
+A CLI tool for reading, modifying, and clearing metadata is provided. 
+In order to use the CLI tool, please [install SD Prompt Reader via pip](#for-linux-users-not-regularly-tested).
+### Modes and Options
+#### Modes
+- Read Mode: Activated by `-r` or `--read` flag.
+- Write Mode: Activated by `-w` or `--write` flag.
+- Clear Mode: Activated by `-c` or `--clear` flag.
+#### General Options
+- `-i`, `--input-path`: Path to the input image file or directory containing image files, required parameter.
+- `-o`, `--output-path`: Path to the output file or directory where the processed files will be saved.
+- `-l`, `--log-level`: Specify the log verbosity level (e.g.DEBUG, INFO, WARN, ERROR).
+#### Read Options
+- `-f`, `--format-type`: Specifies the output metadata format, choices are "TXT" or "JSON". Default format is "TXT"
+#### Write Options
+- `-m`, `--metadata`: Provides a metadata file for writing.
+- `-p`, `--positive`: Provides a positive prompt string for writing.
+- `-n`, `--negative`: Provides a negative prompt string for writing.
+- `-s`, `--setting`: Provides a setting string for writing.
+### Basic Usage
+- If no output path is specified, the modified image will be saved in the current directory 
+with a suffix added to the original filename.  
+- To overwrite the source file, set the output path equal to the input path.
+- The write mode only supports modifications to a single image.
+#### Read Mode
+- Read metadata from an image.
+- Usage:  
+`sd-prompt-reader-cli [-r] -i <input_path> [--format-type <format>] [-o <output_path>]`
+- Examples:  
+`sd-prompt-reader-cli -i example.png`  
+`sd-prompt-reader-cli -i example.png -o metadata.txt`  
+`sd-prompt-reader-cli -r -i example.png -f TXT -o output_folder/`  
+`sd-prompt-reader-cli -r -i input_folder/ -f JSON -o output_folder/`
+#### Write Mode
+- Write metadata to an image.
+- Usage:  
+`sd-prompt-reader-cli -w -i <input_path> -m <metadata_path> [-o <output_path>]`
+- Examples:  
+`sd-prompt-reader-cli -w -i example.png -m new_metadata.txt`  
+`sd-prompt-reader-cli -w -i example.png -m new_metadata.txt -o output.png`  
+`sd-prompt-reader-cli -w -i example.png -m new_metadata.json -o output_folder/`
+#### Clear Mode
+- Remove all metadata from an image.
+- Usage:  
+`sd-prompt-reader-cli -c -i <input_path> [-o <output_path>]`
+- Examples:  
+`sd-prompt-reader-cli -c -i example.png`  
+`sd-prompt-reader-cli -c -i example.png -o output.png`  
+`sd-prompt-reader-cli -c -i example.png -o output_folder/`  
+`sd-prompt-reader-cli -c -i input_folder/ -o output_folder/`
+
+
+## API
+```Python
+from sd_prompt_reader.image_data_reader import ImageDataReader
+
+with open(image_path, "rb+") as f:
+   image_metadata = ImageDataReader(f)
+
+# WIP
+```
+
 ## Format Limitations
 ### TXT
 1. Importing txt file is only allowed in edit mode.
 2. Only A1111 format txt files are supported. You can use txt files generated by the A1111 webui or use the SD prompt reader to export txt from A1111 images
 ### StableSwarmUI
 StableSwarmUI is still in the Alpha testing phase, and its format may change in the future. I will keep track of upcoming updates of StableSwarmUI.
 ### ComfyUI
-***Support for comfyUI requires more testing. If you believe your image is not being displayed properly, please upload the original file generated by ComfyUI to the issues.***
-1. If there are multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means that there are multiple KSampler nodes in the flowchart.
-2. Due to the nature of ComfyUI, all nodes and flowcharts in the workflow are stored in the image, including those that are not being used. Also, a flowchart can have multiple branches, inputs and outputs.
+1. When custom nodes are used or when the workflow becomes overly complex, there is a high probability that metadata may not be correctly read. 
+This is because ComfyUI does not store metadata but only the complete workflow. SD Prompt Reader can only handle basic workflows.
+It is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
+2. If there are multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means that there are multiple KSampler nodes in the flowchart.
+3. Due to the nature of ComfyUI, all nodes and flowcharts in the workflow are stored in the image, including those that are not being used. Also, a flowchart can have multiple branches, inputs and outputs.
 (e.g. output hires. fixed image and original image simultaneously in a single flowchart)
 SD Prompt Reader will traverse all flowcharts and branches and display the longest branch with complete input and output.  
-3. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow)
-4. When custom nodes are used or when the workflow becomes overly complex, there is a high probability that metadata may not be correctly read. 
-This is because ComfyUI does not store metadata but only the complete workflow. 
-It is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
+4. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow)
 ### Easy Diffusion
 By default, Easy Diffusion does not write metadata to images. Please change the _Metadata format_ in settings to _embed_ to write the metadata to images
 ### Fooocus-MRE
 Since the original version of [Fooocus](https://github.com/lllyasviel/Fooocus) does not support writing metadata to image files, 
 SD Prompt Reader only supports images generated by [Fooocus MoonRide Edition](https://github.com/MoonRide303/Fooocus-MRE).
 
 ## FAQ
@@ -217,7 +285,8 @@
 - Gallery/Folder view
 - User preference
 
 ## Credits
 - Inspired by [Stable Diffusion web UI](https://github.com/AUTOMATIC1111/stable-diffusion-webui/)
 - App icon generated using Stable Diffusion with [IconsMI](https://huggingface.co/jvkape/IconsMI-AppIconsModelforSD)
 - Special thanks to [Azusachan](https://github.com/Azusachan) for providing SD server
+- The NovelAI stealth pnginfo parser is based on [the official metadata extraction script of NovelAI](https://github.com/NovelAI/novelai-image-metadata)
```

#### html2text {}

```diff
@@ -3,149 +3,189 @@
  _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_s_]_[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:
                                _b_l_a_c_k_][platform]
 
 [ç®ä½ä¸­æ](https://github.com/receyuki/stable-diffusion-prompt-reader/blob/
    master/README.zh-Hans.md) | [English](https://github.com/receyuki/stable-
  diffusion-prompt-reader/blob/master/README.md) A simple standalone viewer for
     reading prompt from Stable Diffusion generated image outside the webui.
-   _F_e_a_t_u_r_e_s â¢ _S_u_p_p_o_r_t_e_d_ _F_o_r_m_a_t_s â¢ _D_o_w_n_l_o_a_d â¢ _U_s_a_g_e â¢ _F_A_Q â¢ _C_r_e_d_i_t_s
+_F_e_a_t_u_r_e_s â¢ _S_u_p_p_o_r_t_e_d_ _F_o_r_m_a_t_s â¢ _D_o_w_n_l_o_a_d â¢ _U_s_a_g_e â¢ _C_o_m_f_y_U_I_ _N_o_d_e â¢ _C_L_I
+                          â¢ _A_P_I â¢ _F_A_Q â¢ _C_r_e_d_i_t_s
 [https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
                              screenshot_v134.png]
 >The SD Prompt Reader is now available as a ComfyUI node. Check out >the
 [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-
 node) for more information. ## Features - Support macOS, Windows and Linux. -
 Simple drag and drop interaction. - Copy prompt to clipboard. - Remove prompt
 from image. - Export prompt to text file. - Edit or import prompt to images -
 Vertical orientation display and sorting by alphabet - Detect generation tool.
 - Multiple formats support. - Dark and light mode support. ## Supported Formats
 | | PNG | JPEG | WEBP | TXT* | |-----------------------------------------------
----------------------------|:---:|:----:|:----:|:----:| | [A1111's webUI]
-(https://github.com/AUTOMATIC1111/stable-diffusion-webui) | â | â | â |
-â | | [Easy Diffusion](https://github.com/easydiffusion/easydiffusion) | â
-| â | â | | | [StableSwarmUI](https://github.com/Stability-AI/
-StableSwarmUI)* | â | â | | | | [Fooocus-MRE](https://github.com/
-MoonRide303/Fooocus-MRE)* | â | â | | | | [InvokeAI](https://github.com/
-invoke-ai/InvokeAI) | â | | | | | [ComfyUI](https://github.com/
-comfyanonymous/ComfyUI)* | â | | | | | [NovelAI](https://novelai.net/) | â
-| | | | | [Draw Things](https://drawthings.ai/) | â | | | | | Naifu(4chan) |
-â | | | | \* Limitations apply. See [format limitations](#TXT). If you are
-using a tool or format that is not on this list, please help me to support your
-format by uploading the original file generated by your tool to the issues,
-thx. For ComfyUI users, the SD Prompt Reader is now available as a ComfyUI
-node. The [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-
-prompt-reader-node) is a subproject of this project, and it is recommended to
-embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-
-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt
-Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within
-your workflow to ensure maximum compatibility. ## Download ### For Windows
-users Download executable from [GitHub Releases](https://github.com/receyuki/
-stable-diffusion-prompt-reader/releases/latest) ### For macOS users Download
-executable from [GitHub Releases](https://github.com/receyuki/stable-diffusion-
-prompt-reader/releases/latest) #### Install via Homebrew Cask You may also
-install SD Prompt Reader via [Homebrew](http://brew.sh/) cask. ```bash brew
-install --no-quarantine receyuki/sd-prompt-reader/sd-prompt-reader ``` The
-parameter `--no-quarantine` is used since the SD Prompt Reader is currently
-unsigned as I mentioned [here](https://github.com/receyuki/stable-diffusion-
-prompt-reader#sd-prompt-readerapp-is-damaged-and-cant-be-opened-you-should-
-move-it-to-the-trash) ### For Linux users (not regularly tested) ~~I'm pretty
-sure linux users can figure things out without an executable.~~ - The minimum
-version of Python required is 3.10 - Make sure you have the tkinter package
-installed in your Python. If not, install the python3-tk package with package
-managers. e.g. `sudo apt-get install python3-tk` for Debian-based distributions
-You can choose to install with pip or run it manually #### Install with pip or
-pipx ```bash pip install sd-prompt-reader ``` or ```bash pipx install sd-
-prompt-reader ``` To launch app just enter `sd-prompt-reader` in the terminal.
-#### Run source code manually 1. Clone this repo. ```bash git clone https://
-github.com/receyuki/stable-diffusion-prompt-reader.git ``` or download repo as
-a zip. 2. CD to the directory and install dependencies. ```bash cd stable-
-diffusion-prompt-reader pip install -r requirements.txt ``` 3. Run. ```bash
-python main.py ``` ## Usage ### Read prompt - Open the executable file (.exe or
-.app) and drag and drop the image into the window. OR - Right click on the
-image and select open with SD Prompt Reader OR - Drag and drop the image
-directly onto executable (.exe or .app). ### Export prompt to a text file -
-Click "Export" will generate a txt file alongside the image file. - To save to
-another location, click the expand arrow and click "select directory". !
-[export](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/
-images/export.png) ### Remove prompt from image - Click "Clear" will generate a
-new image file with suffix "_data_removed" alongside the original image file. -
-To save to another location, click the expand arrow and click "select
-directory". - To overwrite the original image file, click the expand arrow and
-click "overwrite the original image". ![remove](https://github.com/receyuki/
-stable-diffusion-prompt-reader/raw/master/images/remove.png) ### Edit image
-***Please note that the edited image will be written in A1111 format, it
-meaning that image in any format will become A1111 format after editing.*** -
-Click "Edit" to enter edit mode. - Edit the prompt directly in the textbox or
-import a metadata file in txt format. - Click "Save" will generate a edited
-image file with suffix "_edited" alongside the original image file. - To save
-to another location, click the expand arrow and click "select directory". - To
-overwrite the original image file, click the expand arrow and click "overwrite
-the original image". ![save](https://github.com/receyuki/stable-diffusion-
-prompt-reader/raw/master/images/save.png) ### Copy as single line prompt Copy
-image prompt and setting in a format that can be read by [Prompts from file or
-textbox](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/
-Features#prompts-from-file-or-textbox) The following parameters are supported:
-| Setting | Parameter | |-------------------------|----------------------| |
-Seed | --seed | | Variation seed strength | --subseed_strength | | Seed resize
-from | --seed_resize_from_h | | Seed resize from | --seed_resize_from_w | |
-Sampler | --sampler_name | | Steps | --steps | | CFG scale | --cfg_scale | |
-Size | --width | | Size | --height | | Face restoration | --restore_faces | -
-Click the expand arrow and click "single line prompt". - Paste it into the
-textbox below the webui script "Prompts from file or textbox". ![single line
-prompt](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/
-images/single_line_prompt.png) ### ComfyUI SDXL workflow ***The SDXL workflow
-does not support editing. If necessary, please remove prompts from image before
-edit.*** If the image's workflow includes multiple sets of SDXL prompts, namely
-Clip G(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch
-to the multi-set prompt display mode as shown in the image below. There are two
+-----------------------------------------|:---:|:----:|:----:|:----:| |
+[A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | â
+| â | â | â | | [Easy Diffusion](https://github.com/easydiffusion/
+easydiffusion) | â | â | â | | | [StableSwarmUI](https://github.com/
+Stability-AI/StableSwarmUI)* | â | â | | | | [StableSwarmUI (prior to
+0.5.8-alpha)](https://github.com/Stability-AI/StableSwarmUI)* | â | â | | |
+| [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)* | â | â | | |
+| [InvokeAI](https://github.com/invoke-ai/InvokeAI) | â | | | | | [InvokeAI
+(prior to 2.3.5-post.2)](https://github.com/invoke-ai/InvokeAI) | â | | | | |
+[InvokeAI (prior to 1.15)](https://github.com/invoke-ai/InvokeAI) | â | | | |
+| [ComfyUI](https://github.com/comfyanonymous/ComfyUI)* | â | | | | | [Draw
+Things](https://drawthings.ai/) | â | | | | | [NovelAI (stealth pnginfo)]
+(https://novelai.net/) | â | | | | | [NovelAI (legacy)](https://novelai.net/
+) | â | | | | | Naifu(4chan) | â | | | | \* Limitations apply. See [format
+limitations](#TXT). If you are using a tool or format that is not on this list,
+please help me to support your format by uploading the original file generated
+by your tool to the issues, thx. For ComfyUI users, the SD Prompt Reader is now
+available as a ComfyUI node. The [ComfyUI Prompt Reader Node](https://
+github.com/receyuki/comfyui-prompt-reader-node) is a subproject of this
+project, and it is recommended to embed the [Prompt Saver node](https://
+github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-
+generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/
+receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum
+compatibility. ## Download ### For Windows users Download executable from
+[GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/
+releases/latest) ### For macOS users Download executable from [GitHub Releases]
+(https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest)
+#### Install via Homebrew Cask You may also install SD Prompt Reader via
+[Homebrew](http://brew.sh/) cask. ```bash brew install --no-quarantine
+receyuki/sd-prompt-reader/sd-prompt-reader ``` The parameter `--no-quarantine`
+is used since the SD Prompt Reader is currently unsigned as I mentioned [here]
+(https://github.com/receyuki/stable-diffusion-prompt-reader#sd-prompt-
+readerapp-is-damaged-and-cant-be-opened-you-should-move-it-to-the-trash) ###
+For Linux users (not regularly tested) ~~I'm pretty sure linux users can figure
+things out without an executable.~~ - The minimum version of Python required is
+3.10 - Make sure you have the tkinter package installed in your Python. If not,
+install the python3-tk package with package managers. e.g. `sudo apt-get
+install python3-tk` for Debian-based distributions You can choose to install
+with pip or run it manually #### Install with pip or pipx ```bash pip install
+sd-prompt-reader ``` or ```bash pipx install sd-prompt-reader ``` To launch app
+just enter `sd-prompt-reader` in the terminal. #### Run source code manually 1.
+Clone this repo. ```bash git clone https://github.com/receyuki/stable-
+diffusion-prompt-reader.git ``` or download repo as a zip. 2. CD to the
+directory and install dependencies. ```bash cd stable-diffusion-prompt-reader
+pip install -r requirements.txt ``` 3. Run. ```bash python main.py ``` ## Usage
+### Read prompt - Open the executable file (.exe or .app) and drag and drop the
+image into the window. OR - Right click on the image and select open with SD
+Prompt Reader OR - Drag and drop the image directly onto executable (.exe or
+.app). ### Export prompt to a text file - Click "Export" will generate a txt
+file alongside the image file. - To save to another location, click the expand
+arrow and click "select directory". ![export](https://github.com/receyuki/
+stable-diffusion-prompt-reader/raw/master/images/export.png) ### Remove prompt
+from image - Click "Clear" will generate a new image file with suffix
+"_data_removed" alongside the original image file. - To save to another
+location, click the expand arrow and click "select directory". - To overwrite
+the original image file, click the expand arrow and click "overwrite the
+original image". ![remove](https://github.com/receyuki/stable-diffusion-prompt-
+reader/raw/master/images/remove.png) ### Edit image ***Please note that the
+edited image will be written in A1111 format, it meaning that image in any
+format will become A1111 format after editing.*** - Click "Edit" to enter edit
+mode. - Edit the prompt directly in the textbox or import a metadata file in
+txt format. - Click "Save" will generate a edited image file with suffix
+"_edited" alongside the original image file. - To save to another location,
+click the expand arrow and click "select directory". - To overwrite the
+original image file, click the expand arrow and click "overwrite the original
+image". ![save](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/
+master/images/save.png) ### Copy as single line prompt Copy image prompt and
+setting in a format that can be read by [Prompts from file or textbox](https://
+github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Features#prompts-from-
+file-or-textbox) The following parameters are supported: | Setting | Parameter
+| |-------------------------|----------------------| | Seed | --seed | |
+Variation seed strength | --subseed_strength | | Seed resize from | --
+seed_resize_from_h | | Seed resize from | --seed_resize_from_w | | Sampler | --
+sampler_name | | Steps | --steps | | CFG scale | --cfg_scale | | Size | --width
+| | Size | --height | | Face restoration | --restore_faces | - Click the expand
+arrow and click "single line prompt". - Paste it into the textbox below the
+webui script "Prompts from file or textbox". ![single line prompt](https://
+github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
+single_line_prompt.png) ### ComfyUI SDXL workflow ***The SDXL workflow does not
+support editing. If necessary, please remove prompts from image before edit.***
+If the image's workflow includes multiple sets of SDXL prompts, namely Clip G
+(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch to the
+multi-set prompt display mode as shown in the image below. There are two
 interface options available for the multi-set prompt display mode, and you can
 switch between them using buttons. ![comfyui_sdxl.png](https://github.com/
 receyuki/stable-diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png) ##
-Format Limitations ### TXT 1. Importing txt file is only allowed in edit mode.
-2. Only A1111 format txt files are supported. You can use txt files generated
-by the A1111 webui or use the SD prompt reader to export txt from A1111 images
-### StableSwarmUI StableSwarmUI is still in the Alpha testing phase, and its
-format may change in the future. I will keep track of upcoming updates of
-StableSwarmUI. ### ComfyUI ***Support for comfyUI requires more testing. If you
-believe your image is not being displayed properly, please upload the original
-file generated by ComfyUI to the issues.*** 1. If there are multiple sets of
-data (seed, steps, CFG, etc.) in the setting box, this means that there are
-multiple KSampler nodes in the flowchart. 2. Due to the nature of ComfyUI, all
-nodes and flowcharts in the workflow are stored in the image, including those
-that are not being used. Also, a flowchart can have multiple branches, inputs
-and outputs. (e.g. output hires. fixed image and original image simultaneously
-in a single flowchart) SD Prompt Reader will traverse all flowcharts and
-branches and display the longest branch with complete input and output. 3.
-[ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-
-reader#comfyui-sdxl-workflow) 4. When custom nodes are used or when the
-workflow becomes overly complex, there is a high probability that metadata may
-not be correctly read. This is because ComfyUI does not store metadata but only
-the complete workflow. It is recommended to embed the [Prompt Saver node]
-(https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--
-parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://
-github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure
-maximum compatibility. ### Easy Diffusion By default, Easy Diffusion does not
-write metadata to images. Please change the _Metadata format_ in settings to
-_embed_ to write the metadata to images ### Fooocus-MRE Since the original
-version of [Fooocus](https://github.com/lllyasviel/Fooocus) does not support
-writing metadata to image files, SD Prompt Reader only supports images
-generated by [Fooocus MoonRide Edition](https://github.com/MoonRide303/Fooocus-
-MRE). ## FAQ ### Malware Alert The false positive reported by some anti-
-malwares is caused by the packaging tool _pyinstaller_ which is a common issue
-for _pyinstaller_ users. I spent a lot of time trying to fix the Windows
-Defender false positive before, but I couldn't do it for every antivirus
-software. So, you can either trust Windows Defender or use the instruction for
-Linux users to use this app. ### "SD Prompt Reader.app" is damaged and can't be
-opened. You should move it to the Trash This is a very common macOS issue when
-you run unsigned non-appstore apps, and developers must pay $99 per year to
-Apple to eliminate this issue. You can choose to **Allow Apps from Anywhere**
-in **security & privacy** settings which can be dangerous. The way I prefer is
-to remove the quarantine attributes. 1. Open Terminal from the Applications
-folder. 2. Type in the following command and hit Enter. `xattr -r -
-d com.apple.quarantine /path/to/app.app` In my case it's `xattr -r -
+CLI A CLI tool for reading, modifying, and clearing metadata is provided. In
+order to use the CLI tool, please [install SD Prompt Reader via pip](#for-
+linux-users-not-regularly-tested). ### Modes and Options #### Modes - Read
+Mode: Activated by `-r` or `--read` flag. - Write Mode: Activated by `-w` or `-
+-write` flag. - Clear Mode: Activated by `-c` or `--clear` flag. #### General
+Options - `-i`, `--input-path`: Path to the input image file or directory
+containing image files, required parameter. - `-o`, `--output-path`: Path to
+the output file or directory where the processed files will be saved. - `-l`,
+`--log-level`: Specify the log verbosity level (e.g.DEBUG, INFO, WARN, ERROR).
+#### Read Options - `-f`, `--format-type`: Specifies the output metadata
+format, choices are "TXT" or "JSON". Default format is "TXT" #### Write Options
+- `-m`, `--metadata`: Provides a metadata file for writing. - `-p`, `--
+positive`: Provides a positive prompt string for writing. - `-n`, `--negative`:
+Provides a negative prompt string for writing. - `-s`, `--setting`: Provides a
+setting string for writing. ### Basic Usage - If no output path is specified,
+the modified image will be saved in the current directory with a suffix added
+to the original filename. - To overwrite the source file, set the output path
+equal to the input path. - The write mode only supports modifications to a
+single image. #### Read Mode - Read metadata from an image. - Usage: `sd-
+prompt-reader-cli [-r] -i [--format-type ] [-o ]` - Examples: `sd-prompt-
+reader-cli -i example.png` `sd-prompt-reader-cli -i example.png -
+o metadata.txt` `sd-prompt-reader-cli -r -i example.png -f TXT -
+o output_folder/` `sd-prompt-reader-cli -r -i input_folder/ -f JSON -
+o output_folder/` #### Write Mode - Write metadata to an image. - Usage: `sd-
+prompt-reader-cli -w -i -m [-o ]` - Examples: `sd-prompt-reader-cli -w -
+i example.png -m new_metadata.txt` `sd-prompt-reader-cli -w -i example.png -
+m new_metadata.txt -o output.png` `sd-prompt-reader-cli -w -i example.png -
+m new_metadata.json -o output_folder/` #### Clear Mode - Remove all metadata
+from an image. - Usage: `sd-prompt-reader-cli -c -i [-o ]` - Examples: `sd-
+prompt-reader-cli -c -i example.png` `sd-prompt-reader-cli -c -i example.png -
+o output.png` `sd-prompt-reader-cli -c -i example.png -o output_folder/` `sd-
+prompt-reader-cli -c -i input_folder/ -o output_folder/` ## API ```Python from
+sd_prompt_reader.image_data_reader import ImageDataReader with open(image_path,
+"rb+") as f: image_metadata = ImageDataReader(f) # WIP ``` ## Format
+Limitations ### TXT 1. Importing txt file is only allowed in edit mode. 2. Only
+A1111 format txt files are supported. You can use txt files generated by the
+A1111 webui or use the SD prompt reader to export txt from A1111 images ###
+StableSwarmUI StableSwarmUI is still in the Alpha testing phase, and its format
+may change in the future. I will keep track of upcoming updates of
+StableSwarmUI. ### ComfyUI 1. When custom nodes are used or when the workflow
+becomes overly complex, there is a high probability that metadata may not be
+correctly read. This is because ComfyUI does not store metadata but only the
+complete workflow. SD Prompt Reader can only handle basic workflows. It is
+recommended to embed the [Prompt Saver node](https://github.com/receyuki/
+comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the
+[ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-
+node) within your workflow to ensure maximum compatibility. 2. If there are
+multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means
+that there are multiple KSampler nodes in the flowchart. 3. Due to the nature
+of ComfyUI, all nodes and flowcharts in the workflow are stored in the image,
+including those that are not being used. Also, a flowchart can have multiple
+branches, inputs and outputs. (e.g. output hires. fixed image and original
+image simultaneously in a single flowchart) SD Prompt Reader will traverse all
+flowcharts and branches and display the longest branch with complete input and
+output. 4. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-
+diffusion-prompt-reader#comfyui-sdxl-workflow) ### Easy Diffusion By default,
+Easy Diffusion does not write metadata to images. Please change the _Metadata
+format_ in settings to _embed_ to write the metadata to images ### Fooocus-MRE
+Since the original version of [Fooocus](https://github.com/lllyasviel/Fooocus)
+does not support writing metadata to image files, SD Prompt Reader only
+supports images generated by [Fooocus MoonRide Edition](https://github.com/
+MoonRide303/Fooocus-MRE). ## FAQ ### Malware Alert The false positive reported
+by some anti-malwares is caused by the packaging tool _pyinstaller_ which is a
+common issue for _pyinstaller_ users. I spent a lot of time trying to fix the
+Windows Defender false positive before, but I couldn't do it for every
+antivirus software. So, you can either trust Windows Defender or use the
+instruction for Linux users to use this app. ### "SD Prompt Reader.app" is
+damaged and can't be opened. You should move it to the Trash This is a very
+common macOS issue when you run unsigned non-appstore apps, and developers must
+pay $99 per year to Apple to eliminate this issue. You can choose to **Allow
+Apps from Anywhere** in **security & privacy** settings which can be dangerous.
+The way I prefer is to remove the quarantine attributes. 1. Open Terminal from
+the Applications folder. 2. Type in the following command and hit Enter. `xattr
+-r -d com.apple.quarantine /path/to/app.app` In my case it's `xattr -r -
 d com.apple.quarantine /Applications/SD\ Prompt\ Reader.app` If you are still
 concerned about the security of the app you can use the instruction for Linux
 users to use this app. ## TODO - Batch image processing tool - Gallery/Folder
 view - User preference ## Credits - Inspired by [Stable Diffusion web UI]
 (https://github.com/AUTOMATIC1111/stable-diffusion-webui/) - App icon generated
 using Stable Diffusion with [IconsMI](https://huggingface.co/jvkape/IconsMI-
 AppIconsModelforSD) - Special thanks to [Azusachan](https://github.com/
-Azusachan) for providing SD server
+Azusachan) for providing SD server - The NovelAI stealth pnginfo parser is
+based on [the official metadata extraction script of NovelAI](https://
+github.com/NovelAI/novelai-image-metadata)
```

### Comparing `sd_prompt_reader-1.3.4.post2/pyproject.toml` & `sd_prompt_reader-1.3.5b1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sd-prompt-reader"
-version = "1.3.4.post2"
+version = "1.3.5b1"
 description = "A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui."
 authors = ["receyuki <receyuki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/receyuki/stable-diffusion-prompt-reader"
 repository = "https://github.com/receyuki/stable-diffusion-prompt-reader"
 documentation = "https://github.com/receyuki/stable-diffusion-prompt-reader"
@@ -20,11 +20,12 @@
 "Bug Tracker" = "https://github.com/receyuki/stable-diffusion-prompt-reader/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.scripts]
 sd-prompt-reader = "sd_prompt_reader.app:main"
+sd-prompt-reader-cli = "sd_prompt_reader.cli:cli"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/.DS_Store` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/.DS_Store`

 * *Files 9% similar despite different names*

```diff
@@ -253,32 +253,32 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 0011 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0002 a986 0000 000b 005f 005f 0070  ..........._._.p
+00001030: 0000 0002 cb27 0000 000b 005f 005f 0070  .....'....._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 c1ea aea4  moDDblob........
-00001060: 1ba2 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 b22c 9c38  moDDblob.....,.8
+00001060: a4f0 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 c1ea aea4 1ba2  dDblob..........
+00001080: 6444 626c 6f62 0000 0008 b22c 9c38 a4f0  dDblob.....,.8..
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0003 4000 0000 0006  comp......@.....
+000010b0: 636f 6d70 0000 0000 0003 6000 0000 0006  comp......`.....
 000010c0: 0066 006f 0072 006d 0061 0074 6c67 3153  .f.o.r.m.a.tlg1S
-000010d0: 636f 6d70 0000 0000 0001 a333 0000 0006  comp.......3....
+000010d0: 636f 6d70 0000 0000 0001 e06d 0000 0006  comp.......m....
 000010e0: 0066 006f 0072 006d 0061 0074 6d6f 4444  .f.o.r.m.a.tmoDD
-000010f0: 626c 6f62 0000 0008 9999 31e8 5ca4 c541  blob......1.\..A
+000010f0: 626c 6f62 0000 0008 380f 23f4 82f0 c541  blob....8.#....A
 00001100: 0000 0006 0066 006f 0072 006d 0061 0074  .....f.o.r.m.a.t
-00001110: 6d6f 6444 626c 6f62 0000 0008 9999 31e8  modDblob......1.
-00001120: 5ca4 c541 0000 0006 0066 006f 0072 006d  \..A.....f.o.r.m
+00001110: 6d6f 6444 626c 6f62 0000 0008 380f 23f4  modDblob....8.#.
+00001120: 82f0 c541 0000 0006 0066 006f 0072 006d  ...A.....f.o.r.m
 00001130: 0061 0074 7068 3153 636f 6d70 0000 0000  .a.tph1Scomp....
-00001140: 0002 4000 0000 0009 0072 0065 0073 006f  ..@......r.e.s.o
+00001140: 0002 a000 0000 0009 0072 0065 0073 006f  .........r.e.s.o
 00001150: 0075 0072 0063 0065 0073 6277 7370 626c  .u.r.c.e.sbwspbl
 00001160: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00001170: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00001180: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00001190: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 000011a0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 000011b0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/app.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,20 +26,23 @@
 from .image_data_reader import ImageDataReader
 from .parameter_viewer import ParameterViewer
 from .prompt_viewer import PromptViewer
 from .status_bar import StatusBar
 from .textbox import STkTextbox
 from .update_checker import UpdateChecker
 from .__version__ import VERSION
+from .logger import Logger
 
 
 class App(Tk):
     def __init__(self):
         super().__init__()
 
+        logger = Logger("SD_Prompt_Reader.App")
+        Logger.configure_global_logger("DEBUG")
         # window = TkinterDnD.Tk()
         # window = Tk()
         self.title("SD Prompt Reader")
         self.geometry("1280x600")
         # set_appearance_mode("Light")
         # deactivate_automatic_dpi_awareness()
         # set_widget_scaling(1)
@@ -477,31 +480,39 @@
         # open with in macOS
         self.createcommand("::tk::mac::OpenDocument", self.open_document_handler)
 
     def open_document_handler(self, *args):
         self.display_info(args[0], is_selected=True)
 
     def display_info(self, event, is_selected=False):
+        self.status_bar.unbind()
         # stop update thread when reading first image
         self.update_checker.close_thread()
         # selected or drag and drop
         if is_selected:
             if event == "":
                 return
             new_path = Path(event)
         else:
             new_path = Path(event.data.replace("}", "").replace("{", ""))
 
         # detect suffix and read
-        if new_path.suffix in SUPPORTED_FORMATS:
+        if new_path.suffix.lower() in SUPPORTED_FORMATS:
             self.file_path = new_path
             with open(self.file_path, "rb") as f:
                 self.image_data = ImageDataReader(f)
-                if not self.image_data.tool:
+                if (
+                    not self.image_data.tool
+                    or self.image_data.status.name == "FORMAT_ERROR"
+                ):
                     self.unsupported_format(MESSAGE["format_error"])
+                elif self.image_data.status.name == "COMFYUI_ERROR":
+                    self.unsupported_format(
+                        MESSAGE["comfyui_error"], url=URL["comfyui"], raw=True
+                    )
                 else:
                     self.readable = True
                     # insert prompt
                     if not self.image_data.is_sdxl:
                         self.positive_box.display(self.image_data.positive)
                         self.negative_box.display(self.image_data.negative)
                     else:
@@ -550,30 +561,35 @@
         else:
             self.unsupported_format(MESSAGE["suffix_error"], True)
             if self.button_edit.mode == EditMode.ON:
                 for box in self.boxes:
                     box.edit_off()
             self.button_edit.disable()
 
-    def unsupported_format(self, message, reset_image=False):
+    def unsupported_format(self, message, reset_image=False, url="", raw=False):
         self.readable = False
-        self.setting_box.text = message[0]
-        self.positive_box.display(message[0])
-        self.negative_box.display(message[0])
+        self.setting_box.text = ""
+        self.positive_box.display("")
+        self.negative_box.display("")
         self.setting_box_parameter.reset_text()
         for button in self.function_buttons:
             button.disable()
         self.positive_box.all_off()
         self.negative_box.all_off()
         if reset_image:
             self.image_label.configure(image=self.drop_image, text=MESSAGE["drop"][0])
             self.image = None
         else:
             self.button_edit.enable()
         self.status_bar.warning(message[-1])
+        if url:
+            self.status_bar.link(url)
+        if raw:
+            self.button_raw.enable()
+            self.button_export.enable()
 
     def resize_image(self, event=None):
         # resize image to window size
         if self.image:
             aspect_ratio = self.image.size[0] / self.image.size[1]
             # fix windows huge image problem under hidpi
             self.scaling = ScalingTracker.get_window_dpi_scaling(self)
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/button.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/button.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/constants.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 __copyright__ = "Copyright 2023"
 __email__ = "receyuki@gmail.com"
 
 from importlib import resources
 from pathlib import Path
 from . import resources as res
 
-RELEASE_URL = "https://api.github.com/repos/receyuki/stable-diffusion-prompt-reader/releases/latest"
 RESOURCE_DIR = str(resources.files(res))
 SUPPORTED_FORMATS = [".png", ".jpg", ".jpeg", ".webp"]
 COLOR_THEME = Path(RESOURCE_DIR, "gray.json")
 INFO_FILE = Path(RESOURCE_DIR, "info_24.png")
 ERROR_FILE = Path(RESOURCE_DIR, "error_24.png")
 WARNING_FILE = Path(RESOURCE_DIR, "warning_24.png")
 OK_FILE = Path(RESOURCE_DIR, "check_circle_24.png")
@@ -78,14 +77,18 @@
         "unsupported TXT format",
     ],
     "txt_imported": ["The TXT file has been successfully imported"],
     "edit": ["Edit mode", "View mode"],
     "sort": ["Ascending order", "Descending order", "Original order"],
     "view_prompt": ["Vertical orientation", "Horizontal orientation"],
     "view_setting": ["Simple mode", "Normal mode"],
+    "comfyui_error": [
+        "The ComfyUI workflow is overly complex, or unsupported custom nodes have been used",
+        "Failed to parse ComfyUI data, click here for more info",
+    ],
 }
 TOOLTIP = {
     "edit": "Edit image metadata",
     "save": "Save edited image",
     "clear": "Remove metadata from the image",
     "export": "Export metadata to a TXT file",
     "copy_raw": "Copy raw metadata to the clipboard",
@@ -93,14 +96,21 @@
     "copy_setting": "Copy setting to the clipboard",
     "sort": "Sort prompt lines in ascending or descending order",
     "view_prompt": "View prompt in vertical orientation",
     "view_setting": "View setting in simple mode",
     "view_separate": "View Clip G, Clip L and Refiner prompt in separate textbox",
     "view_tab": "View Clip G, Clip L and Refiner prompt in one textbox",
 }
+URL = {
+    "release": "https://api.github.com/repos/receyuki/stable-diffusion-prompt-reader/releases/latest",
+    "format": (
+        "https://github.com/receyuki/stable-diffusion-prompt-reader#supported-formats"
+    ),
+    "comfyui": "https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui",
+}
 DEFAULT_GRAY = "#8E8E93"
 ACCESSIBLE_GRAY = ("#6C6C70", "#AEAEB2")
 INACCESSIBLE_GRAY = ("gray60", "gray45")
 EDITABLE = ("gray10", "#DCE4EE")
 BUTTON_HOVER = ("gray86", "gray17")
 TOOLTIP_DELAY = 1.5
 BUTTON_WIDTH_L = 40
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/.DS_Store` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0000 ebd3 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0001 1118 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 b2d6 f7e8  moDDblob........
-00000160: 5ca4 c541 0000 000b 005f 005f 0070 0079  \..A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 08e0 c8d3  moDDblob........
+00000160: d1ec c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 b2d6 f7e8 5ca4  dDblob........\.
+00000180: 6444 626c 6f62 0000 0008 08e0 c8d3 d1ec  dDblob..........
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0001 3000 0000 0000  comp......0.....
+000001b0: 636f 6d70 0000 0000 0001 6000 0000 0000  comp......`.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/a1111.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/a1111.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 __filename__ = "a1111.py"
 __copyright__ = "Copyright 2023"
 __email__ = "receyuki@gmail.com"
 
 import re
 
 from ..format.base_format import BaseFormat
-from ..utility import add_quotes
+from ..utility import add_quotes, concat_strings
 
 
 class A1111(BaseFormat):
     PROMPT_MAPPING = {
         # "Model": ("sd_model", True),
         # "prompt",
         # "negative_prompt",
@@ -26,21 +26,24 @@
         "Face restoration": ("restore_faces", False),
     }
 
     SETTING_KEY = ["Model", "Sampler", "Seed", "CFG scale", "Steps", "Size"]
 
     def __init__(self, info: dict = None, raw: str = ""):
         super().__init__(info, raw)
+        self._extra = ""
+
+    def _process(self):
         if not self._raw:
-            self._raw = self._info.get("parameters")
+            self._raw = self._info.get("parameters", "")
+            self._extra = self._info.get("postprocessing", "")
         self._sd_format()
 
     def _sd_format(self):
-        if not self._raw:
-            self._raw = ""
+        if not self._raw and not self._extra:
             return
 
         steps_index = self._raw.find("\nSteps:")
         # w/ setting
         if steps_index != -1:
             self._positive = self._raw[:steps_index].strip()
             self._setting = self._raw[steps_index:].strip()
@@ -72,14 +75,18 @@
                 setting_dict[key] = value
 
         [self._width, self._height] = setting_dict.get("Size", "0x0").split("x")
 
         for p, s in zip(super().PARAMETER_KEY, A1111.SETTING_KEY):
             self._parameter[p] = setting_dict.get(s)
 
+        if self._extra:
+            self._raw = concat_strings(self._raw, self._extra)
+            self._setting = concat_strings(self._setting, self._extra)
+
     def prompt_to_line(self):
         if not self._setting:
             return ""
         single_line_prompt = "--prompt " + add_quotes(self._positive).replace("\n", "")
         if self._negative:
             single_line_prompt += " --negative_prompt " + add_quotes(
                 self._negative
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/comfyui.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/comfyui.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,20 +35,43 @@
         "",
     ]
 
     def __init__(
         self, info: dict = None, raw: str = "", width: int = None, height: int = None
     ):
         super().__init__(info, raw, width, height)
+        self._prompt = ""
+        self._workflow = ""
+
+    def parse(self):
+        try:
+            self._process()
+        except Exception as e:
+            self._logger.error(e)
+            self._status = self.Status.COMFYUI_ERROR
+            self._positive = ""
+            self._negative = ""
+            self._positive_sdxl = {}
+            self._negative_sdxl = {}
+            self._setting = ""
+            self._parameter = dict.fromkeys(BaseFormat.PARAMETER_KEY, "")
+            self._is_sdxl = False
+            self._raw = "\n".join([self._prompt, self._workflow])
+            return self._status
+        else:
+            self._status = self.Status.READ_SUCCESS
+            return self._status
+
+    def _process(self):
         self._comfy_png()
 
     def _comfy_png(self):
-        prompt = self._info.get("prompt", {})
-        workflow = self._info.get("workflow", {})
-        prompt_json = json.loads(prompt)
+        self._prompt = self._info.get("prompt", {})
+        self._workflow = self._info.get("workflow", {})
+        prompt_json = json.loads(str(self._prompt))
 
         # find end node of each flow
         end_nodes = list(
             filter(
                 lambda item: item[-1].get("class_type")
                 in ["SaveImage"] + ComfyUI.KSAMPLER_TYPES,
                 prompt_json.items(),
@@ -83,17 +106,17 @@
                 ]
                 + [
                     self._negative_sdxl.get(key).strip()
                     for key in sdxl_keys
                     if self._negative_sdxl.get(key)
                 ]
             )
-        self._raw += "\n" + str(prompt)
-        if workflow:
-            self._raw += "\n" + str(workflow)
+        self._raw += "\n" + str(self._prompt)
+        if self._workflow:
+            self._raw += "\n" + str(self._workflow)
 
         add_noise = (
             f"Add noise: {remove_quotes(longest_flow.get('add_noise'))}"
             if longest_flow.get("add_noise")
             else ""
         )
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/drawthings.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/drawthings.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 
 class DrawThings(BaseFormat):
     SETTING_KEY = ["model", "sampler", "seed", "scale", "steps", "size"]
 
     def __init__(self, info: dict = None, raw: str = ""):
         super().__init__(info, raw)
+
+    def _process(self):
         self._dt_format()
 
     def _dt_format(self):
         data_json = self.info
         self._tool = "Draw Things"
         self._positive = data_json.pop("c").strip()
         self._negative = data_json.pop("uc").strip()
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/easydiffusion.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/easydiffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         "guidance_scale",
         "num_inference_steps",
         "",
     ]
 
     def __init__(self, info: dict = None, raw: str = ""):
         super().__init__(info, raw)
+
+    def _process(self):
         if not self._raw:
             self._raw = str(self._info).replace("'", '"')
         self._ed_format()
 
     def _ed_format(self):
         data_json = json.loads(self._raw)
         ed = (
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/fooocus.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/fooocus.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         "cfg",
         "steps",
         "",
     ]
 
     def __init__(self, info: dict = None, raw: str = ""):
         super().__init__(info, raw)
+
+    def _process(self):
         self._fc_format()
 
     def _fc_format(self):
         data_json = self.info
         self._tool = "Fooocus"
         self._positive = data_json.get("prompt").strip()
         self._negative = data_json.get("negative_prompt").strip()
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/invokeai.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/invokeai.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,22 +34,24 @@
         "Size": "",
         "CFG scale": "C",
         "Sampler": "A",
     }
 
     def __init__(self, info: dict = None, raw: str = ""):
         super().__init__(info, raw)
+
+    def _process(self):
         if "invokeai_metadata" in self._info:
-            self._invoke_invoke_metadata()
-        elif "sd-metadata" in self._info:
             self._invoke_metadata()
+        elif "sd-metadata" in self._info:
+            self._invoke_sd_metadata()
         elif "Dream" in self._info:
             self._invoke_dream()
 
-    def _invoke_invoke_metadata(self):
+    def _invoke_metadata(self):
         data_json = json.loads(self._info.get("invokeai_metadata"))
         self._positive = data_json.pop("positive_prompt").strip()
         self._negative = data_json.pop("negative_prompt").strip()
         self._raw = "\n".join([self._positive, self._negative, str(data_json)])
         self._setting = remove_quotes(str(data_json)).strip("{ }")
         self._width = str(data_json.get("width"))
         self._height = str(data_json.get("height"))
@@ -78,15 +80,15 @@
                 case _:
                     self._parameter[p] = remove_quotes(
                         str((data_json.get(s[0]), data_json.get(s[1])))
                         if has_refiner
                         else str(data_json.get(s[0]))
                     )
 
-    def _invoke_metadata(self):
+    def _invoke_sd_metadata(self):
         data_json = json.loads(self._info.get("sd-metadata"))
         image = data_json.pop("image")
         prompt = (
             image.get("prompt")[0].get("prompt")
             if isinstance(image.get("prompt"), list)
             else image.get("prompt")
         )
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/format/swarmui.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/format/swarmui.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 class SwarmUI(BaseFormat):
     SETTING_KEY = ["model", "", "seed", "cfgscale", "steps", ""]
 
     def __init__(self, info: dict = None, raw: str = ""):
         super().__init__(info, raw)
         if not self._info:
             self._info = json.loads(self._raw)
+
+    def _process(self):
         self._ss_format()
 
     def _ss_format(self):
         data_json = self._info.get("sui_image_params")
         self._positive = data_json.get("prompt").strip()
         self._negative = data_json.get("negativeprompt").strip()
         self._raw = "\n".join([self._positive, self._negative, str(data_json)]).strip()
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/image_data_reader.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/image_data_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from xml.dom import minidom
 
 import piexif
 import piexif.helper
 from PIL import Image
 from PIL.PngImagePlugin import PngInfo
 
+from .logger import Logger
 from .constants import PARAMETER_PLACEHOLDER
 from .format import (
+    BaseFormat,
     A1111,
     EasyDiffusion,
     InvokeAI,
     NovelAI,
     ComfyUI,
     DrawThings,
     SwarmUI,
@@ -37,15 +39,18 @@
         self._raw = ""
         self._tool = ""
         self._parameter_key = ["model", "sampler", "seed", "cfg", "steps", "size"]
         self._parameter = dict.fromkeys(self._parameter_key, PARAMETER_PLACEHOLDER)
         self._is_txt = is_txt
         self._is_sdxl = False
         self._format = ""
+        self._props = ""
         self._parser = None
+        self._status = BaseFormat.Status.UNREAD
+        self._logger = Logger("SD_Prompt_Reader.ImageDataReader")
         self.read_data(file)
 
     def read_data(self, file):
         if self._is_txt:
             self._raw = file.read()
             self._parser = A1111(raw=self._raw)
             return
@@ -70,14 +75,17 @@
                         # a1111 png compatible format
                         else:
                             if "prompt" in self._info:
                                 self._tool = "ComfyUI\n(A1111 compatible)"
                             else:
                                 self._tool = "A1111 webUI"
                             self._parser = A1111(info=self._info)
+                    elif "postprocessing" in self._info:
+                        self._tool = "A1111 webUI\n(Postprocessing)"
+                        self._parser = A1111(info=self._info)
                     # easydiff png format
                     elif (
                         "negative_prompt" in self._info
                         or "Negative Prompt" in self._info
                     ):
                         self._tool = "Easy Diffusion"
                         self._parser = EasyDiffusion(info=self._info)
@@ -89,15 +97,15 @@
                     elif "sd-metadata" in self._info:
                         self._tool = "InvokeAI"
                         self._parser = InvokeAI(info=self._info)
                     # invokeai legacy dream format
                     elif "Dream" in self._info:
                         self._tool = "InvokeAI"
                         self._parser = InvokeAI(info=self._info)
-                    # novelai format
+                    # novelai legacy format
                     elif self._info.get("Software") == "NovelAI":
                         self._tool = "NovelAI"
                         self._parser = NovelAI(
                             info=self._info, width=self._width, height=self._height
                         )
                     # comfyui format
                     elif "prompt" in self._info:
@@ -108,169 +116,219 @@
                     # fooocus format
                     elif "Comment" in self._info:
                         try:
                             self._tool = "Fooocus"
                             self._parser = Fooocus(
                                 info=json.loads(self._info.get("Comment"))
                             )
-                        except:
-                            print("Fooocus format error")
+                        except Exception:
+                            self._logger.warn("Fooocus format error")
                     # drawthings format
                     elif "XML:com.adobe.xmp" in self._info:
                         try:
                             data = minidom.parseString(
                                 self._info.get("XML:com.adobe.xmp")
                             )
                             data_json = json.loads(
                                 data.getElementsByTagName("exif:UserComment")[0]
                                 .childNodes[1]
                                 .childNodes[1]
                                 .childNodes[0]
                                 .data
                             )
-                        except:
-                            print("Draw things format error")
+                        except Exception:
+                            self._logger.warn("Draw things format error")
+                            self._status = BaseFormat.Status.FORMAT_ERROR
                         else:
                             self._tool = "Draw Things"
                             self._parser = DrawThings(info=data_json)
+                    # novelai stealth pnginfo format
+                    elif f.mode == "RGBA":
+                        try:
+                            reader = NovelAI.LSBExtractor(f)
+                            magic = "stealth_pngcomp"
+                            read_magic = reader.get_next_n_bytes(len(magic)).decode(
+                                "utf-8"
+                            )
+                            assert (
+                                magic == read_magic
+                            ), "NovelAI stealth png info magic number error"
+                        except Exception as e:
+                            self._logger.warn(e)
+                            self._status = BaseFormat.Status.FORMAT_ERROR
+                        else:
+                            self._tool = "NovelAI"
+                            self._parser = NovelAI(extractor=reader)
                 elif f.format in ["JPEG", "WEBP"]:
                     # fooocus jpeg format
                     if "comment" in self._info:
                         try:
                             self._tool = "Fooocus"
                             self._parser = Fooocus(
                                 info=json.loads(self._info.get("comment"))
                             )
-                        except:
-                            print("Fooocus format error")
+                        except Exception:
+                            self._logger.warn("Fooocus format error")
+                            self._status = BaseFormat.Status.FORMAT_ERROR
                     else:
                         try:
                             exif = piexif.load(self._info.get("exif")) or {}
                             user_comment = exif.get("Exif").get(
                                 piexif.ExifIFD.UserComment
                             )
                         except TypeError:
-                            print("empty jpeg")
+                            self._logger.warn("Empty jpeg")
+                            self._status = BaseFormat.Status.FORMAT_ERROR
                         except Exception:
                             pass
                         else:
-                            # swarm format
-                            if "sui_image_params" in user_comment[8:].decode("utf-16"):
-                                self._tool = "StableSwarmUI"
-                                self._parser = SwarmUI(
-                                    raw=user_comment[8:].decode("utf-16")
-                                )
-                            else:
-                                self._raw = piexif.helper.UserComment.load(user_comment)
-                                # easydiff jpeg and webp format
-                                if self._raw[0] == "{":
-                                    self._tool = "Easy Diffusion"
-                                    self._parser = EasyDiffusion(raw=self._raw)
-                                # a1111 jpeg and webp format
+                            try:
+                                # swarm format
+                                if "sui_image_params" in user_comment[8:].decode(
+                                    "utf-16"
+                                ):
+                                    self._tool = "StableSwarmUI"
+                                    self._parser = SwarmUI(
+                                        raw=user_comment[8:].decode("utf-16")
+                                    )
                                 else:
-                                    self._tool = "A1111 webUI"
-                                    self._parser = A1111(raw=self._raw)
+                                    self._raw = piexif.helper.UserComment.load(
+                                        user_comment
+                                    )
+                                    # easydiff jpeg and webp format
+                                    if self._raw[0] == "{":
+                                        self._tool = "Easy Diffusion"
+                                        self._parser = EasyDiffusion(raw=self._raw)
+                                    # a1111 jpeg and webp format
+                                    else:
+                                        self._tool = "A1111 webUI"
+                                        self._parser = A1111(raw=self._raw)
+                            except Exception:
+                                self._status = BaseFormat.Status.FORMAT_ERROR
+            if self._tool and self._status == BaseFormat.Status.UNREAD:
+                self._logger.debug(f"Format: {self._tool}")
+                self._status = self._parser.parse()
+            self._logger.debug(f"Reading Status: {self._status.name}")
 
     @staticmethod
     def remove_data(image_file):
         with Image.open(image_file) as f:
             image_data = list(f.getdata())
             image_without_exif = Image.new(f.mode, f.size)
             image_without_exif.putdata(image_data)
             return image_without_exif
 
     @staticmethod
     def save_image(image_path, new_path, image_format, data=None):
         metadata = None
         if data:
-            match image_format:
+            match image_format.upper():
                 case "PNG":
                     metadata = PngInfo()
                     metadata.add_text("parameters", data)
-                case "JPEG" | "WEBP":
+                case "JPEG" | "JPG" | "WEBP":
                     metadata = piexif.dump(
                         {
                             "Exif": {
-                                piexif.ExifIFD.UserComment: piexif.helper.UserComment.dump(
-                                    data, encoding="unicode"
+                                piexif.ExifIFD.UserComment: (
+                                    piexif.helper.UserComment.dump(
+                                        data, encoding="unicode"
+                                    )
                                 )
                             },
                         }
                     )
 
         with Image.open(image_path) as f:
             try:
-                match image_format:
+                match image_format.upper():
                     case "PNG":
                         if data:
                             f.save(new_path, pnginfo=metadata)
                         else:
                             f.save(new_path)
-                    case "JPEG":
+                    case "JPEG" | "JPG":
                         f.save(new_path, quality="keep")
                         if data:
                             piexif.insert(metadata, str(new_path))
                     case "WEBP":
                         f.save(new_path, quality=100, lossless=True)
                         if data:
                             piexif.insert(metadata, str(new_path))
-            except:
+            except Exception:
                 print("Save error")
 
+    @staticmethod
+    def construct_data(positive, negative, setting):
+        return "\n".join(
+            filter(
+                None,
+                [
+                    f"{positive}" if positive else "",
+                    f"Negative prompt: {negative}" if negative else "",
+                    f"{setting}" if setting else "",
+                ],
+            )
+        )
+
     def prompt_to_line(self):
         return self._parser.prompt_to_line()
 
     @property
     def height(self):
-        return self._parser.height
+        return self._parser.height if self._tool else self._height
 
     @property
     def width(self):
-        return self._parser.width
+        return self._parser.width if self._tool else self._width
 
     @property
     def info(self):
         return self._info
 
     @property
     def positive(self):
-        return self._parser.positive
+        return self._parser.positive if self._tool else self._positive
 
     @property
     def negative(self):
-        return self._parser.negative
+        return self._parser.negative if self._tool else self._negative
 
     @property
     def positive_sdxl(self):
-        return self._parser.positive_sdxl
+        return self._parser.positive_sdxl if self._tool else self._positive_sdxl
 
     @property
     def negative_sdxl(self):
-        return self._parser.negative_sdxl
+        return self._parser.negative_sdxl if self._tool else self._negative_sdxl
 
     @property
     def setting(self):
-        return self._parser.setting
+        return self._parser.setting if self._tool else self._setting
 
     @property
     def raw(self):
-        return self._parser.raw
+        return self._parser.raw or self._raw
 
     @property
     def tool(self):
         return self._tool
 
     @property
     def parameter(self):
-        return self._parser.parameter
+        return self._parser.parameter if self._tool else self._parameter
 
     @property
     def format(self):
         return self._format
 
     @property
     def is_sdxl(self):
-        return self._parser.is_sdxl
+        return self._parser.is_sdxl if self._tool else self._is_sdxl
 
     @property
     def props(self):
-        return self._parser.props
+        return self._parser.props if self._tool else self._props
+
+    @property
+    def status(self):
+        return self._status
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/parameter_viewer.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/parameter_viewer.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/prompt_viewer.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/prompt_viewer.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/.DS_Store` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/.DS_Store`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/check_circle_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/check_circle_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/check_circle_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/check_circle_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/cleaning_services_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/cleaning_services_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/cleaning_services_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/cleaning_services_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/content_copy_20.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/content_copy_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/content_copy_20_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/content_copy_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/content_copy_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/content_copy_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/content_copy_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/content_copy_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/description_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/description_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/description_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/description_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/edit_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/edit_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/edit_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/edit_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/edit_off_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/edit_off_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/edit_off_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/edit_off_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/error_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/error_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/error_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/error_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/expand_more_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/expand_more_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/expand_more_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/expand_more_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/gray.json` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/gray.json`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/icon.icns` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/icon.icns`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/icon.ico` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/icon.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/icon.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/info_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/info_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/info_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/info_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/lightbulb_20.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/lightbulb_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/lightbulb_20_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/lightbulb_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/mop_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/mop_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/mop_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/mop_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/place_item_48.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/place_item_48.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/place_item_48_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/place_item_48_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/save_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/save_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/save_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/save_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/sort_by_alpha_20.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/sort_by_alpha_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/update_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/update_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/update_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/update_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/view_sidebar_20.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/view_sidebar_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/view_sidebar_20_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/view_sidebar_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/view_week_20.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/view_week_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/view_week_20_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/view_week_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/warning_24.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/warning_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/resources/warning_24_alpha.png` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/resources/warning_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/status_bar.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/status_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,23 +61,22 @@
             case "add suffix":
                 self.info(MESSAGE["suffix"][0])
             case "overwrite the original image":
                 self.info(MESSAGE["overwrite"][0])
             case "select directory":
                 self.info(MESSAGE["remove_select"][0])
 
-    def update(self, download_url):
-        self.status_label.configure(
-            image=self.available_updates_image, text=MESSAGE["update"][0]
-        )
-        self.status_label.bind(
-            "<Button-1>", lambda e: webbrowser.open_new(download_url)
-        )
+    def link(self, url, is_update=False):
+        if is_update:
+            self.status_label.configure(
+                image=self.available_updates_image, text=MESSAGE["update"][0]
+            )
+        self.status_label.bind("<Button-1>", lambda e: webbrowser.open_new(url))
 
-    def stop_update(self):
+    def unbind(self):
         self.status_label.unbind("<Button-1>")
 
     @staticmethod
     def add_margin(img, top, bottom, left, right):
         width, height = img.size
         new_width = width + right + left
         new_height = height + top + bottom
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/textbox.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/textbox.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/update_checker.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/update_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 
 import threading
 
 import requests
 from packaging import version
 
 from .__version__ import VERSION
-from .constants import RELEASE_URL
+from .constants import URL
 
 
 class UpdateChecker:
     def __init__(self, status_bar):
         self._update_check = True
         self.status_bar = status_bar
         self.update_thread = threading.Thread(target=self.check_update)
         self.update_thread.start()
 
     # check update from GitHub release
     def check_update(self):
         try:
-            response = requests.get(RELEASE_URL, timeout=3).json()
+            response = requests.get(URL["release"], timeout=3).json()
         except Exception:
             print("Github api connection error")
         else:
             latest = response["name"]
             if version.parse(latest) > version.parse(VERSION):
                 download_url = response["html_url"]
-                self.status_bar.update(download_url)
+                self.status_bar.link(download_url, is_update=True)
 
     # clean up threads that are no longer in use
     def close_thread(self):
         if self._update_check:
             self._update_check = False
-            self.status_bar.stop_update()
+            self.status_bar.unbind()
             self.update_thread.join()
```

### Comparing `sd_prompt_reader-1.3.4.post2/sd_prompt_reader/utility.py` & `sd_prompt_reader-1.3.5b1/sd_prompt_reader/utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         filetypes=(("image files", "*.png *.jpg *jpeg *.webp"),),
     )
 
 
 def copy_to_clipboard(status_bar, content):
     try:
         pyperclip.copy(content)
-    except:
+    except Exception:
         print("Copy error")
     else:
         status_bar.clipboard()
 
 
 def get_canvas_total_size(canvas):
     # Get the actual width and height of the canvas
@@ -143,8 +143,12 @@
 
 
 def remove_quotes(string):
     return str(string).replace('"', "").replace("'", "")
 
 
 def add_quotes(string):
-    return '"' + str(string) + '"'
+    return f'"{str(string)}"'
+
+
+def concat_strings(base, addition, separator=", "):
+    return f"{base}{separator}{addition}" if base else addition
```

### Comparing `sd_prompt_reader-1.3.4.post2/PKG-INFO` & `sd_prompt_reader-1.3.5b1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-prompt-reader
-Version: 1.3.4.post2
+Version: 1.3.5b1
 Summary: A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui.
 Home-page: https://github.com/receyuki/stable-diffusion-prompt-reader
 License: MIT
 Author: receyuki
 Author-email: receyuki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,17 @@
 A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui.
     <br>
   <p>
     <a href="#features">Features</a> •
     <a href="#supported-formats">Supported Formats</a> •
     <a href="#download">Download</a> •
     <a href="#usage">Usage</a> •
+    <a href="https://github.com/receyuki/comfyui-prompt-reader-node">ComfyUI Node</a> •
+    <a href="#cli">CLI</a> •
+    <a href="#api">API</a> •
     <a href="#faq">FAQ</a> •
     <a href="#credits">Credits</a>
   </p>
     <img src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/screenshot_v134.png">
 </div>
 
 >The SD Prompt Reader is now available as a ComfyUI node. Check out 
@@ -61,25 +64,29 @@
 - Edit or import prompt to images
 - Vertical orientation display and sorting by alphabet
 - Detect generation tool.
 - Multiple formats support.
 - Dark and light mode support.
 
 ## Supported Formats
-|                                                                          | PNG | JPEG | WEBP | TXT* |
-|--------------------------------------------------------------------------|:---:|:----:|:----:|:----:|
-| [A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) |  ✅  |  ✅   |  ✅   |  ✅   |
-| [Easy Diffusion](https://github.com/easydiffusion/easydiffusion)         |  ✅  |  ✅   |  ✅   |      |
-| [StableSwarmUI](https://github.com/Stability-AI/StableSwarmUI)*          |  ✅  |  ✅   |      |      |
-| [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)*               |  ✅  |  ✅   |      |      |
-| [InvokeAI](https://github.com/invoke-ai/InvokeAI)                        |  ✅  |      |      |      |
-| [ComfyUI](https://github.com/comfyanonymous/ComfyUI)*                    |  ✅  |      |      |      |
-| [NovelAI](https://novelai.net/)                                          |  ✅  |      |      |      |
-| [Draw Things](https://drawthings.ai/)                                    |  ✅  |      |      |      |
-| Naifu(4chan)                                                             |  ✅  |      |      |      |
+|                                                                                        | PNG | JPEG | WEBP | TXT* |
+|----------------------------------------------------------------------------------------|:---:|:----:|:----:|:----:|
+| [A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui)               |  ✅  |  ✅   |  ✅   |  ✅   |
+| [Easy Diffusion](https://github.com/easydiffusion/easydiffusion)                       |  ✅  |  ✅   |  ✅   |      |
+| [StableSwarmUI](https://github.com/Stability-AI/StableSwarmUI)*                        |  ✅  |  ✅   |      |      |
+| [StableSwarmUI (prior to 0.5.8-alpha)](https://github.com/Stability-AI/StableSwarmUI)* |  ✅  |  ✅   |      |      |
+| [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)*                             |  ✅  |  ✅   |      |      |
+| [InvokeAI](https://github.com/invoke-ai/InvokeAI)                                      |  ✅  |      |      |      |
+| [InvokeAI (prior to 2.3.5-post.2)](https://github.com/invoke-ai/InvokeAI)              |  ✅  |      |      |      |
+| [InvokeAI (prior to 1.15)](https://github.com/invoke-ai/InvokeAI)                      |  ✅  |      |      |      |
+| [ComfyUI](https://github.com/comfyanonymous/ComfyUI)*                                  |  ✅  |      |      |      |
+| [Draw Things](https://drawthings.ai/)                                                  |  ✅  |      |      |      |
+| [NovelAI (stealth pnginfo)](https://novelai.net/)                                      |  ✅  |      |      |      |
+| [NovelAI (legacy)](https://novelai.net/)                                               |  ✅  |      |      |      |
+| Naifu(4chan)                                                                           |  ✅  |      |      |      |
 
 \* Limitations apply. See [format limitations](#TXT).
 
 If you are using a tool or format that is not on this list, please help me to support your format 
 by uploading the original file generated by your tool to the issues, thx.
 
 For ComfyUI users, the SD Prompt Reader is now available as a ComfyUI node. 
@@ -185,30 +192,91 @@
 ***The SDXL workflow does not support editing. 
 If necessary, please remove prompts from image before edit.***  
 If the image's workflow includes multiple sets of SDXL prompts, 
 namely Clip G(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch to the multi-set prompt display mode as shown in the image below. 
 There are two interface options available for the multi-set prompt display mode, and you can switch between them using buttons.  
 ![comfyui_sdxl.png](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png)
 
+## CLI
+A CLI tool for reading, modifying, and clearing metadata is provided. 
+In order to use the CLI tool, please [install SD Prompt Reader via pip](#for-linux-users-not-regularly-tested).
+### Modes and Options
+#### Modes
+- Read Mode: Activated by `-r` or `--read` flag.
+- Write Mode: Activated by `-w` or `--write` flag.
+- Clear Mode: Activated by `-c` or `--clear` flag.
+#### General Options
+- `-i`, `--input-path`: Path to the input image file or directory containing image files, required parameter.
+- `-o`, `--output-path`: Path to the output file or directory where the processed files will be saved.
+- `-l`, `--log-level`: Specify the log verbosity level (e.g.DEBUG, INFO, WARN, ERROR).
+#### Read Options
+- `-f`, `--format-type`: Specifies the output metadata format, choices are "TXT" or "JSON". Default format is "TXT"
+#### Write Options
+- `-m`, `--metadata`: Provides a metadata file for writing.
+- `-p`, `--positive`: Provides a positive prompt string for writing.
+- `-n`, `--negative`: Provides a negative prompt string for writing.
+- `-s`, `--setting`: Provides a setting string for writing.
+### Basic Usage
+- If no output path is specified, the modified image will be saved in the current directory 
+with a suffix added to the original filename.  
+- To overwrite the source file, set the output path equal to the input path.
+- The write mode only supports modifications to a single image.
+#### Read Mode
+- Read metadata from an image.
+- Usage:  
+`sd-prompt-reader-cli [-r] -i <input_path> [--format-type <format>] [-o <output_path>]`
+- Examples:  
+`sd-prompt-reader-cli -i example.png`  
+`sd-prompt-reader-cli -i example.png -o metadata.txt`  
+`sd-prompt-reader-cli -r -i example.png -f TXT -o output_folder/`  
+`sd-prompt-reader-cli -r -i input_folder/ -f JSON -o output_folder/`
+#### Write Mode
+- Write metadata to an image.
+- Usage:  
+`sd-prompt-reader-cli -w -i <input_path> -m <metadata_path> [-o <output_path>]`
+- Examples:  
+`sd-prompt-reader-cli -w -i example.png -m new_metadata.txt`  
+`sd-prompt-reader-cli -w -i example.png -m new_metadata.txt -o output.png`  
+`sd-prompt-reader-cli -w -i example.png -m new_metadata.json -o output_folder/`
+#### Clear Mode
+- Remove all metadata from an image.
+- Usage:  
+`sd-prompt-reader-cli -c -i <input_path> [-o <output_path>]`
+- Examples:  
+`sd-prompt-reader-cli -c -i example.png`  
+`sd-prompt-reader-cli -c -i example.png -o output.png`  
+`sd-prompt-reader-cli -c -i example.png -o output_folder/`  
+`sd-prompt-reader-cli -c -i input_folder/ -o output_folder/`
+
+
+## API
+```Python
+from sd_prompt_reader.image_data_reader import ImageDataReader
+
+with open(image_path, "rb+") as f:
+   image_metadata = ImageDataReader(f)
+
+# WIP
+```
+
 ## Format Limitations
 ### TXT
 1. Importing txt file is only allowed in edit mode.
 2. Only A1111 format txt files are supported. You can use txt files generated by the A1111 webui or use the SD prompt reader to export txt from A1111 images
 ### StableSwarmUI
 StableSwarmUI is still in the Alpha testing phase, and its format may change in the future. I will keep track of upcoming updates of StableSwarmUI.
 ### ComfyUI
-***Support for comfyUI requires more testing. If you believe your image is not being displayed properly, please upload the original file generated by ComfyUI to the issues.***
-1. If there are multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means that there are multiple KSampler nodes in the flowchart.
-2. Due to the nature of ComfyUI, all nodes and flowcharts in the workflow are stored in the image, including those that are not being used. Also, a flowchart can have multiple branches, inputs and outputs.
+1. When custom nodes are used or when the workflow becomes overly complex, there is a high probability that metadata may not be correctly read. 
+This is because ComfyUI does not store metadata but only the complete workflow. SD Prompt Reader can only handle basic workflows.
+It is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
+2. If there are multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means that there are multiple KSampler nodes in the flowchart.
+3. Due to the nature of ComfyUI, all nodes and flowcharts in the workflow are stored in the image, including those that are not being used. Also, a flowchart can have multiple branches, inputs and outputs.
 (e.g. output hires. fixed image and original image simultaneously in a single flowchart)
 SD Prompt Reader will traverse all flowcharts and branches and display the longest branch with complete input and output.  
-3. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow)
-4. When custom nodes are used or when the workflow becomes overly complex, there is a high probability that metadata may not be correctly read. 
-This is because ComfyUI does not store metadata but only the complete workflow. 
-It is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
+4. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow)
 ### Easy Diffusion
 By default, Easy Diffusion does not write metadata to images. Please change the _Metadata format_ in settings to _embed_ to write the metadata to images
 ### Fooocus-MRE
 Since the original version of [Fooocus](https://github.com/lllyasviel/Fooocus) does not support writing metadata to image files, 
 SD Prompt Reader only supports images generated by [Fooocus MoonRide Edition](https://github.com/MoonRide303/Fooocus-MRE).
 
 ## FAQ
@@ -237,8 +305,9 @@
 - Gallery/Folder view
 - User preference
 
 ## Credits
 - Inspired by [Stable Diffusion web UI](https://github.com/AUTOMATIC1111/stable-diffusion-webui/)
 - App icon generated using Stable Diffusion with [IconsMI](https://huggingface.co/jvkape/IconsMI-AppIconsModelforSD)
 - Special thanks to [Azusachan](https://github.com/Azusachan) for providing SD server
+- The NovelAI stealth pnginfo parser is based on [the official metadata extraction script of NovelAI](https://github.com/NovelAI/novelai-image-metadata)
```

#### html2text {}

```diff
@@ -1,164 +1,204 @@
-Metadata-Version: 2.1 Name: sd-prompt-reader Version: 1.3.4.post2 Summary: A
-simple standalone viewer for reading prompt from Stable Diffusion generated
-image outside the webui. Home-page: https://github.com/receyuki/stable-
-diffusion-prompt-reader License: MIT Author: receyuki Author-email:
-receyuki@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Project-URL: Bug Tracker,
-https://github.com/receyuki/stable-diffusion-prompt-reader/issues Project-URL:
-Documentation, https://github.com/receyuki/stable-diffusion-prompt-reader
-Project-URL: Repository, https://github.com/receyuki/stable-diffusion-prompt-
-reader Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: sd-prompt-reader Version: 1.3.5b1 Summary: A simple
+standalone viewer for reading prompt from Stable Diffusion generated image
+outside the webui. Home-page: https://github.com/receyuki/stable-diffusion-
+prompt-reader License: MIT Author: receyuki Author-email: receyuki@gmail.com
+Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Project-URL: Bug Tracker, https://github.com/receyuki/stable-
+diffusion-prompt-reader/issues Project-URL: Documentation, https://github.com/
+receyuki/stable-diffusion-prompt-reader Project-URL: Repository, https://
+github.com/receyuki/stable-diffusion-prompt-reader Description-Content-Type:
+text/markdown
                                     [icon]
                  ************ SSttaabbllee DDiiffffuussiioonn PPrroommpptt RReeaaddeerr ************
  _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_s_]_[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:
                                _b_l_a_c_k_][platform]
 
 [ç®ä½ä¸­æ](https://github.com/receyuki/stable-diffusion-prompt-reader/blob/
    master/README.zh-Hans.md) | [English](https://github.com/receyuki/stable-
  diffusion-prompt-reader/blob/master/README.md) A simple standalone viewer for
     reading prompt from Stable Diffusion generated image outside the webui.
-   _F_e_a_t_u_r_e_s â¢ _S_u_p_p_o_r_t_e_d_ _F_o_r_m_a_t_s â¢ _D_o_w_n_l_o_a_d â¢ _U_s_a_g_e â¢ _F_A_Q â¢ _C_r_e_d_i_t_s
+_F_e_a_t_u_r_e_s â¢ _S_u_p_p_o_r_t_e_d_ _F_o_r_m_a_t_s â¢ _D_o_w_n_l_o_a_d â¢ _U_s_a_g_e â¢ _C_o_m_f_y_U_I_ _N_o_d_e â¢ _C_L_I
+                          â¢ _A_P_I â¢ _F_A_Q â¢ _C_r_e_d_i_t_s
 [https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
                              screenshot_v134.png]
 >The SD Prompt Reader is now available as a ComfyUI node. Check out >the
 [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-
 node) for more information. ## Features - Support macOS, Windows and Linux. -
 Simple drag and drop interaction. - Copy prompt to clipboard. - Remove prompt
 from image. - Export prompt to text file. - Edit or import prompt to images -
 Vertical orientation display and sorting by alphabet - Detect generation tool.
 - Multiple formats support. - Dark and light mode support. ## Supported Formats
 | | PNG | JPEG | WEBP | TXT* | |-----------------------------------------------
----------------------------|:---:|:----:|:----:|:----:| | [A1111's webUI]
-(https://github.com/AUTOMATIC1111/stable-diffusion-webui) | â | â | â |
-â | | [Easy Diffusion](https://github.com/easydiffusion/easydiffusion) | â
-| â | â | | | [StableSwarmUI](https://github.com/Stability-AI/
-StableSwarmUI)* | â | â | | | | [Fooocus-MRE](https://github.com/
-MoonRide303/Fooocus-MRE)* | â | â | | | | [InvokeAI](https://github.com/
-invoke-ai/InvokeAI) | â | | | | | [ComfyUI](https://github.com/
-comfyanonymous/ComfyUI)* | â | | | | | [NovelAI](https://novelai.net/) | â
-| | | | | [Draw Things](https://drawthings.ai/) | â | | | | | Naifu(4chan) |
-â | | | | \* Limitations apply. See [format limitations](#TXT). If you are
-using a tool or format that is not on this list, please help me to support your
-format by uploading the original file generated by your tool to the issues,
-thx. For ComfyUI users, the SD Prompt Reader is now available as a ComfyUI
-node. The [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-
-prompt-reader-node) is a subproject of this project, and it is recommended to
-embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-
-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt
-Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within
-your workflow to ensure maximum compatibility. ## Download ### For Windows
-users Download executable from [GitHub Releases](https://github.com/receyuki/
-stable-diffusion-prompt-reader/releases/latest) ### For macOS users Download
-executable from [GitHub Releases](https://github.com/receyuki/stable-diffusion-
-prompt-reader/releases/latest) #### Install via Homebrew Cask You may also
-install SD Prompt Reader via [Homebrew](http://brew.sh/) cask. ```bash brew
-install --no-quarantine receyuki/sd-prompt-reader/sd-prompt-reader ``` The
-parameter `--no-quarantine` is used since the SD Prompt Reader is currently
-unsigned as I mentioned [here](https://github.com/receyuki/stable-diffusion-
-prompt-reader#sd-prompt-readerapp-is-damaged-and-cant-be-opened-you-should-
-move-it-to-the-trash) ### For Linux users (not regularly tested) ~~I'm pretty
-sure linux users can figure things out without an executable.~~ - The minimum
-version of Python required is 3.10 - Make sure you have the tkinter package
-installed in your Python. If not, install the python3-tk package with package
-managers. e.g. `sudo apt-get install python3-tk` for Debian-based distributions
-You can choose to install with pip or run it manually #### Install with pip or
-pipx ```bash pip install sd-prompt-reader ``` or ```bash pipx install sd-
-prompt-reader ``` To launch app just enter `sd-prompt-reader` in the terminal.
-#### Run source code manually 1. Clone this repo. ```bash git clone https://
-github.com/receyuki/stable-diffusion-prompt-reader.git ``` or download repo as
-a zip. 2. CD to the directory and install dependencies. ```bash cd stable-
-diffusion-prompt-reader pip install -r requirements.txt ``` 3. Run. ```bash
-python main.py ``` ## Usage ### Read prompt - Open the executable file (.exe or
-.app) and drag and drop the image into the window. OR - Right click on the
-image and select open with SD Prompt Reader OR - Drag and drop the image
-directly onto executable (.exe or .app). ### Export prompt to a text file -
-Click "Export" will generate a txt file alongside the image file. - To save to
-another location, click the expand arrow and click "select directory". !
-[export](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/
-images/export.png) ### Remove prompt from image - Click "Clear" will generate a
-new image file with suffix "_data_removed" alongside the original image file. -
-To save to another location, click the expand arrow and click "select
-directory". - To overwrite the original image file, click the expand arrow and
-click "overwrite the original image". ![remove](https://github.com/receyuki/
-stable-diffusion-prompt-reader/raw/master/images/remove.png) ### Edit image
-***Please note that the edited image will be written in A1111 format, it
-meaning that image in any format will become A1111 format after editing.*** -
-Click "Edit" to enter edit mode. - Edit the prompt directly in the textbox or
-import a metadata file in txt format. - Click "Save" will generate a edited
-image file with suffix "_edited" alongside the original image file. - To save
-to another location, click the expand arrow and click "select directory". - To
-overwrite the original image file, click the expand arrow and click "overwrite
-the original image". ![save](https://github.com/receyuki/stable-diffusion-
-prompt-reader/raw/master/images/save.png) ### Copy as single line prompt Copy
-image prompt and setting in a format that can be read by [Prompts from file or
-textbox](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/
-Features#prompts-from-file-or-textbox) The following parameters are supported:
-| Setting | Parameter | |-------------------------|----------------------| |
-Seed | --seed | | Variation seed strength | --subseed_strength | | Seed resize
-from | --seed_resize_from_h | | Seed resize from | --seed_resize_from_w | |
-Sampler | --sampler_name | | Steps | --steps | | CFG scale | --cfg_scale | |
-Size | --width | | Size | --height | | Face restoration | --restore_faces | -
-Click the expand arrow and click "single line prompt". - Paste it into the
-textbox below the webui script "Prompts from file or textbox". ![single line
-prompt](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/
-images/single_line_prompt.png) ### ComfyUI SDXL workflow ***The SDXL workflow
-does not support editing. If necessary, please remove prompts from image before
-edit.*** If the image's workflow includes multiple sets of SDXL prompts, namely
-Clip G(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch
-to the multi-set prompt display mode as shown in the image below. There are two
+-----------------------------------------|:---:|:----:|:----:|:----:| |
+[A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | â
+| â | â | â | | [Easy Diffusion](https://github.com/easydiffusion/
+easydiffusion) | â | â | â | | | [StableSwarmUI](https://github.com/
+Stability-AI/StableSwarmUI)* | â | â | | | | [StableSwarmUI (prior to
+0.5.8-alpha)](https://github.com/Stability-AI/StableSwarmUI)* | â | â | | |
+| [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)* | â | â | | |
+| [InvokeAI](https://github.com/invoke-ai/InvokeAI) | â | | | | | [InvokeAI
+(prior to 2.3.5-post.2)](https://github.com/invoke-ai/InvokeAI) | â | | | | |
+[InvokeAI (prior to 1.15)](https://github.com/invoke-ai/InvokeAI) | â | | | |
+| [ComfyUI](https://github.com/comfyanonymous/ComfyUI)* | â | | | | | [Draw
+Things](https://drawthings.ai/) | â | | | | | [NovelAI (stealth pnginfo)]
+(https://novelai.net/) | â | | | | | [NovelAI (legacy)](https://novelai.net/
+) | â | | | | | Naifu(4chan) | â | | | | \* Limitations apply. See [format
+limitations](#TXT). If you are using a tool or format that is not on this list,
+please help me to support your format by uploading the original file generated
+by your tool to the issues, thx. For ComfyUI users, the SD Prompt Reader is now
+available as a ComfyUI node. The [ComfyUI Prompt Reader Node](https://
+github.com/receyuki/comfyui-prompt-reader-node) is a subproject of this
+project, and it is recommended to embed the [Prompt Saver node](https://
+github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-
+generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/
+receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum
+compatibility. ## Download ### For Windows users Download executable from
+[GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/
+releases/latest) ### For macOS users Download executable from [GitHub Releases]
+(https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest)
+#### Install via Homebrew Cask You may also install SD Prompt Reader via
+[Homebrew](http://brew.sh/) cask. ```bash brew install --no-quarantine
+receyuki/sd-prompt-reader/sd-prompt-reader ``` The parameter `--no-quarantine`
+is used since the SD Prompt Reader is currently unsigned as I mentioned [here]
+(https://github.com/receyuki/stable-diffusion-prompt-reader#sd-prompt-
+readerapp-is-damaged-and-cant-be-opened-you-should-move-it-to-the-trash) ###
+For Linux users (not regularly tested) ~~I'm pretty sure linux users can figure
+things out without an executable.~~ - The minimum version of Python required is
+3.10 - Make sure you have the tkinter package installed in your Python. If not,
+install the python3-tk package with package managers. e.g. `sudo apt-get
+install python3-tk` for Debian-based distributions You can choose to install
+with pip or run it manually #### Install with pip or pipx ```bash pip install
+sd-prompt-reader ``` or ```bash pipx install sd-prompt-reader ``` To launch app
+just enter `sd-prompt-reader` in the terminal. #### Run source code manually 1.
+Clone this repo. ```bash git clone https://github.com/receyuki/stable-
+diffusion-prompt-reader.git ``` or download repo as a zip. 2. CD to the
+directory and install dependencies. ```bash cd stable-diffusion-prompt-reader
+pip install -r requirements.txt ``` 3. Run. ```bash python main.py ``` ## Usage
+### Read prompt - Open the executable file (.exe or .app) and drag and drop the
+image into the window. OR - Right click on the image and select open with SD
+Prompt Reader OR - Drag and drop the image directly onto executable (.exe or
+.app). ### Export prompt to a text file - Click "Export" will generate a txt
+file alongside the image file. - To save to another location, click the expand
+arrow and click "select directory". ![export](https://github.com/receyuki/
+stable-diffusion-prompt-reader/raw/master/images/export.png) ### Remove prompt
+from image - Click "Clear" will generate a new image file with suffix
+"_data_removed" alongside the original image file. - To save to another
+location, click the expand arrow and click "select directory". - To overwrite
+the original image file, click the expand arrow and click "overwrite the
+original image". ![remove](https://github.com/receyuki/stable-diffusion-prompt-
+reader/raw/master/images/remove.png) ### Edit image ***Please note that the
+edited image will be written in A1111 format, it meaning that image in any
+format will become A1111 format after editing.*** - Click "Edit" to enter edit
+mode. - Edit the prompt directly in the textbox or import a metadata file in
+txt format. - Click "Save" will generate a edited image file with suffix
+"_edited" alongside the original image file. - To save to another location,
+click the expand arrow and click "select directory". - To overwrite the
+original image file, click the expand arrow and click "overwrite the original
+image". ![save](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/
+master/images/save.png) ### Copy as single line prompt Copy image prompt and
+setting in a format that can be read by [Prompts from file or textbox](https://
+github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Features#prompts-from-
+file-or-textbox) The following parameters are supported: | Setting | Parameter
+| |-------------------------|----------------------| | Seed | --seed | |
+Variation seed strength | --subseed_strength | | Seed resize from | --
+seed_resize_from_h | | Seed resize from | --seed_resize_from_w | | Sampler | --
+sampler_name | | Steps | --steps | | CFG scale | --cfg_scale | | Size | --width
+| | Size | --height | | Face restoration | --restore_faces | - Click the expand
+arrow and click "single line prompt". - Paste it into the textbox below the
+webui script "Prompts from file or textbox". ![single line prompt](https://
+github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
+single_line_prompt.png) ### ComfyUI SDXL workflow ***The SDXL workflow does not
+support editing. If necessary, please remove prompts from image before edit.***
+If the image's workflow includes multiple sets of SDXL prompts, namely Clip G
+(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch to the
+multi-set prompt display mode as shown in the image below. There are two
 interface options available for the multi-set prompt display mode, and you can
 switch between them using buttons. ![comfyui_sdxl.png](https://github.com/
 receyuki/stable-diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png) ##
-Format Limitations ### TXT 1. Importing txt file is only allowed in edit mode.
-2. Only A1111 format txt files are supported. You can use txt files generated
-by the A1111 webui or use the SD prompt reader to export txt from A1111 images
-### StableSwarmUI StableSwarmUI is still in the Alpha testing phase, and its
-format may change in the future. I will keep track of upcoming updates of
-StableSwarmUI. ### ComfyUI ***Support for comfyUI requires more testing. If you
-believe your image is not being displayed properly, please upload the original
-file generated by ComfyUI to the issues.*** 1. If there are multiple sets of
-data (seed, steps, CFG, etc.) in the setting box, this means that there are
-multiple KSampler nodes in the flowchart. 2. Due to the nature of ComfyUI, all
-nodes and flowcharts in the workflow are stored in the image, including those
-that are not being used. Also, a flowchart can have multiple branches, inputs
-and outputs. (e.g. output hires. fixed image and original image simultaneously
-in a single flowchart) SD Prompt Reader will traverse all flowcharts and
-branches and display the longest branch with complete input and output. 3.
-[ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-
-reader#comfyui-sdxl-workflow) 4. When custom nodes are used or when the
-workflow becomes overly complex, there is a high probability that metadata may
-not be correctly read. This is because ComfyUI does not store metadata but only
-the complete workflow. It is recommended to embed the [Prompt Saver node]
-(https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--
-parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://
-github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure
-maximum compatibility. ### Easy Diffusion By default, Easy Diffusion does not
-write metadata to images. Please change the _Metadata format_ in settings to
-_embed_ to write the metadata to images ### Fooocus-MRE Since the original
-version of [Fooocus](https://github.com/lllyasviel/Fooocus) does not support
-writing metadata to image files, SD Prompt Reader only supports images
-generated by [Fooocus MoonRide Edition](https://github.com/MoonRide303/Fooocus-
-MRE). ## FAQ ### Malware Alert The false positive reported by some anti-
-malwares is caused by the packaging tool _pyinstaller_ which is a common issue
-for _pyinstaller_ users. I spent a lot of time trying to fix the Windows
-Defender false positive before, but I couldn't do it for every antivirus
-software. So, you can either trust Windows Defender or use the instruction for
-Linux users to use this app. ### "SD Prompt Reader.app" is damaged and can't be
-opened. You should move it to the Trash This is a very common macOS issue when
-you run unsigned non-appstore apps, and developers must pay $99 per year to
-Apple to eliminate this issue. You can choose to **Allow Apps from Anywhere**
-in **security & privacy** settings which can be dangerous. The way I prefer is
-to remove the quarantine attributes. 1. Open Terminal from the Applications
-folder. 2. Type in the following command and hit Enter. `xattr -r -
-d com.apple.quarantine /path/to/app.app` In my case it's `xattr -r -
+CLI A CLI tool for reading, modifying, and clearing metadata is provided. In
+order to use the CLI tool, please [install SD Prompt Reader via pip](#for-
+linux-users-not-regularly-tested). ### Modes and Options #### Modes - Read
+Mode: Activated by `-r` or `--read` flag. - Write Mode: Activated by `-w` or `-
+-write` flag. - Clear Mode: Activated by `-c` or `--clear` flag. #### General
+Options - `-i`, `--input-path`: Path to the input image file or directory
+containing image files, required parameter. - `-o`, `--output-path`: Path to
+the output file or directory where the processed files will be saved. - `-l`,
+`--log-level`: Specify the log verbosity level (e.g.DEBUG, INFO, WARN, ERROR).
+#### Read Options - `-f`, `--format-type`: Specifies the output metadata
+format, choices are "TXT" or "JSON". Default format is "TXT" #### Write Options
+- `-m`, `--metadata`: Provides a metadata file for writing. - `-p`, `--
+positive`: Provides a positive prompt string for writing. - `-n`, `--negative`:
+Provides a negative prompt string for writing. - `-s`, `--setting`: Provides a
+setting string for writing. ### Basic Usage - If no output path is specified,
+the modified image will be saved in the current directory with a suffix added
+to the original filename. - To overwrite the source file, set the output path
+equal to the input path. - The write mode only supports modifications to a
+single image. #### Read Mode - Read metadata from an image. - Usage: `sd-
+prompt-reader-cli [-r] -i [--format-type ] [-o ]` - Examples: `sd-prompt-
+reader-cli -i example.png` `sd-prompt-reader-cli -i example.png -
+o metadata.txt` `sd-prompt-reader-cli -r -i example.png -f TXT -
+o output_folder/` `sd-prompt-reader-cli -r -i input_folder/ -f JSON -
+o output_folder/` #### Write Mode - Write metadata to an image. - Usage: `sd-
+prompt-reader-cli -w -i -m [-o ]` - Examples: `sd-prompt-reader-cli -w -
+i example.png -m new_metadata.txt` `sd-prompt-reader-cli -w -i example.png -
+m new_metadata.txt -o output.png` `sd-prompt-reader-cli -w -i example.png -
+m new_metadata.json -o output_folder/` #### Clear Mode - Remove all metadata
+from an image. - Usage: `sd-prompt-reader-cli -c -i [-o ]` - Examples: `sd-
+prompt-reader-cli -c -i example.png` `sd-prompt-reader-cli -c -i example.png -
+o output.png` `sd-prompt-reader-cli -c -i example.png -o output_folder/` `sd-
+prompt-reader-cli -c -i input_folder/ -o output_folder/` ## API ```Python from
+sd_prompt_reader.image_data_reader import ImageDataReader with open(image_path,
+"rb+") as f: image_metadata = ImageDataReader(f) # WIP ``` ## Format
+Limitations ### TXT 1. Importing txt file is only allowed in edit mode. 2. Only
+A1111 format txt files are supported. You can use txt files generated by the
+A1111 webui or use the SD prompt reader to export txt from A1111 images ###
+StableSwarmUI StableSwarmUI is still in the Alpha testing phase, and its format
+may change in the future. I will keep track of upcoming updates of
+StableSwarmUI. ### ComfyUI 1. When custom nodes are used or when the workflow
+becomes overly complex, there is a high probability that metadata may not be
+correctly read. This is because ComfyUI does not store metadata but only the
+complete workflow. SD Prompt Reader can only handle basic workflows. It is
+recommended to embed the [Prompt Saver node](https://github.com/receyuki/
+comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the
+[ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-
+node) within your workflow to ensure maximum compatibility. 2. If there are
+multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means
+that there are multiple KSampler nodes in the flowchart. 3. Due to the nature
+of ComfyUI, all nodes and flowcharts in the workflow are stored in the image,
+including those that are not being used. Also, a flowchart can have multiple
+branches, inputs and outputs. (e.g. output hires. fixed image and original
+image simultaneously in a single flowchart) SD Prompt Reader will traverse all
+flowcharts and branches and display the longest branch with complete input and
+output. 4. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-
+diffusion-prompt-reader#comfyui-sdxl-workflow) ### Easy Diffusion By default,
+Easy Diffusion does not write metadata to images. Please change the _Metadata
+format_ in settings to _embed_ to write the metadata to images ### Fooocus-MRE
+Since the original version of [Fooocus](https://github.com/lllyasviel/Fooocus)
+does not support writing metadata to image files, SD Prompt Reader only
+supports images generated by [Fooocus MoonRide Edition](https://github.com/
+MoonRide303/Fooocus-MRE). ## FAQ ### Malware Alert The false positive reported
+by some anti-malwares is caused by the packaging tool _pyinstaller_ which is a
+common issue for _pyinstaller_ users. I spent a lot of time trying to fix the
+Windows Defender false positive before, but I couldn't do it for every
+antivirus software. So, you can either trust Windows Defender or use the
+instruction for Linux users to use this app. ### "SD Prompt Reader.app" is
+damaged and can't be opened. You should move it to the Trash This is a very
+common macOS issue when you run unsigned non-appstore apps, and developers must
+pay $99 per year to Apple to eliminate this issue. You can choose to **Allow
+Apps from Anywhere** in **security & privacy** settings which can be dangerous.
+The way I prefer is to remove the quarantine attributes. 1. Open Terminal from
+the Applications folder. 2. Type in the following command and hit Enter. `xattr
+-r -d com.apple.quarantine /path/to/app.app` In my case it's `xattr -r -
 d com.apple.quarantine /Applications/SD\ Prompt\ Reader.app` If you are still
 concerned about the security of the app you can use the instruction for Linux
 users to use this app. ## TODO - Batch image processing tool - Gallery/Folder
 view - User preference ## Credits - Inspired by [Stable Diffusion web UI]
 (https://github.com/AUTOMATIC1111/stable-diffusion-webui/) - App icon generated
 using Stable Diffusion with [IconsMI](https://huggingface.co/jvkape/IconsMI-
 AppIconsModelforSD) - Special thanks to [Azusachan](https://github.com/
-Azusachan) for providing SD server
+Azusachan) for providing SD server - The NovelAI stealth pnginfo parser is
+based on [the official metadata extraction script of NovelAI](https://
+github.com/NovelAI/novelai-image-metadata)
```

