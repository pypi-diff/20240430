# Comparing `tmp/reflex_antd-0.0.4.tar.gz` & `tmp/reflex_antd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_antd-0.0.4.tar", last modified: Tue Apr 23 05:06:24 2024, max compression
+gzip compressed data, was "reflex_antd-0.0.5.tar", last modified: Tue Apr 30 11:23:59 2024, max compression
```

## Comparing `reflex_antd-0.0.4.tar` & `reflex_antd-0.0.5.tar`

### file list

```diff
@@ -1,159 +1,158 @@
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 05:06:24.838097 reflex_antd-0.0.4/
--rwxrwxrwx   0 see       (1000) see       (1000)    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.4/LICENSE
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-23 05:06:24.831097 reflex_antd-0.0.4/PKG-INFO
--rwxrwxrwx   0 see       (1000) see       (1000)      336 2024-04-19 06:20:21.000000 reflex_antd-0.0.4/README.md
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 05:06:20.985904 reflex_antd-0.0.4/custom_components/
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 05:06:21.282740 reflex_antd-0.0.4/custom_components/reflex_antd/
--rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/__init__.py
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 05:06:24.796097 reflex_antd-0.0.4/custom_components/reflex_antd/antd/
--rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/__init__.py
--rwxrwxrwx   0 see       (1000) see       (1000)      679 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/affix.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3101 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/affix.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/alert.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5909 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/alert.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1028 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/anchor.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3655 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/anchor.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1549 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/auto_complete.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4382 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/auto_complete.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1025 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/avatar.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5934 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/avatar.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      825 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/badge.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6130 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/badge.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2697 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/base.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5912 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/base.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/breadcrumb.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5451 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/breadcrumb.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      922 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/button.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3644 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/button.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1318 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/calendar.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3605 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/calendar.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1366 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/card.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8612 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/card.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      814 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/carousel.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3386 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/carousel.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2282 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/cascader.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5957 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/cascader.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1269 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/checkbox.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6026 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/checkbox.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      935 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/collapse.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3580 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/collapse.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1439 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/color_picker.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4599 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/color_picker.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4993 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/date_picker.py
--rwxrwxrwx   0 see       (1000) see       (1000)    17831 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/date_picker.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      709 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/descriptions.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3597 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/descriptions.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/divider.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3200 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/divider.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1398 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/drawer.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4497 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/drawer.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1518 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/dropdown.py
--rwxrwxrwx   0 see       (1000) see       (1000)     7254 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/dropdown.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      340 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/empty.py
--rwxrwxrwx   0 see       (1000) see       (1000)     2839 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/empty.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      494 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/flex.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3049 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/flex.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/float_button.py
--rwxrwxrwx   0 see       (1000) see       (1000)     9924 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/float_button.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     3495 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/form.py
--rwxrwxrwx   0 see       (1000) see       (1000)    14023 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/form.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      907 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/grid.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5943 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/grid.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2234 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/icon.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4456 2024-04-17 06:35:31.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/icon.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      973 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/image.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5829 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/image.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1947 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/input.py
--rwxrwxrwx   0 see       (1000) see       (1000)    16141 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/input.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1565 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/input_number.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4745 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/input_number.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1645 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/layout.py
--rwxrwxrwx   0 see       (1000) see       (1000)    18024 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/layout.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1114 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/list.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8602 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/list.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1383 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/mentions.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4545 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/mentions.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/menu.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4675 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/menu.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4551 2024-04-17 07:26:07.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/message.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3176 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/message.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/modal.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4678 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/modal.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-04-17 08:26:56.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/notification.py
--rwxrwxrwx   0 see       (1000) see       (1000)     1169 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/pagination.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3794 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/pagination.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      972 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/popconfirm.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3709 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/popconfirm.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      473 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/popover.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4413 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/popover.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1039 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/progress.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4279 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/progress.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      941 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/qrcode.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3635 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/qrcode.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1221 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/radio.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8759 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/radio.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/rate.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3600 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/rate.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      545 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/result.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3263 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/result.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      850 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/segmented.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3432 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/segmented.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2862 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/select.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6924 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/select.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      575 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/skeleton.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3161 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/skeleton.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1272 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/slider.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4053 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/slider.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      755 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/space.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6085 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/space.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      588 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/spin.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3247 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/spin.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1213 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/statistic.py
--rwxrwxrwx   0 see       (1000) see       (1000)     9147 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/statistic.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1036 2024-04-17 04:22:47.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/steps.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3976 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/steps.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1042 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/switch.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3595 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/switch.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2690 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/table.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5782 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/table.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2108 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tabs.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5235 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tabs.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1063 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tag.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5717 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tag.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      566 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/timeline.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3170 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/timeline.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1352 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tooltip.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4395 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tooltip.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1237 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tour.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4192 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tour.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1997 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/transfer.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3910 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/transfer.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2609 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tree.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6180 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tree.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2869 2024-04-23 00:49:43.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tree_select.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6424 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/tree_select.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1763 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/typography.py
--rwxrwxrwx   0 see       (1000) see       (1000)    15437 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/typography.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1584 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/upload.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4500 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/upload.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-17 04:22:48.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/watermark.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3397 2024-04-17 06:35:32.000000 reflex_antd-0.0.4/custom_components/reflex_antd/antd/watermark.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)    23359 2024-04-23 05:04:07.000000 reflex_antd-0.0.4/custom_components/reflex_antd/base.py
--rwxrwxrwx   0 see       (1000) see       (1000)    11261 2024-04-17 06:35:23.000000 reflex_antd-0.0.4/custom_components/reflex_antd/base.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1919 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/constant.py
--rwxrwxrwx   0 see       (1000) see       (1000)      996 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/display.py
--rwxrwxrwx   0 see       (1000) see       (1000)      873 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/entry.py
--rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/feedback.py
--rwxrwxrwx   0 see       (1000) see       (1000)      289 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/general.py
--rwxrwxrwx   0 see       (1000) see       (1000)      145 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/helper.py
--rwxrwxrwx   0 see       (1000) see       (1000)      243 2024-04-17 04:22:46.000000 reflex_antd-0.0.4/custom_components/reflex_antd/layout.py
--rwxrwxrwx   0 see       (1000) see       (1000)      288 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/navigation.py
--rwxrwxrwx   0 see       (1000) see       (1000)     1654 2024-04-17 04:22:49.000000 reflex_antd-0.0.4/custom_components/reflex_antd/util.py
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 05:06:24.822098 reflex_antd-0.0.4/custom_components/reflex_antd.egg-info/
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-23 05:06:20.000000 reflex_antd-0.0.4/custom_components/reflex_antd.egg-info/PKG-INFO
--rwxrwxrwx   0 see       (1000) see       (1000)     6899 2024-04-23 05:06:20.000000 reflex_antd-0.0.4/custom_components/reflex_antd.egg-info/SOURCES.txt
--rwxrwxrwx   0 see       (1000) see       (1000)        1 2024-04-23 05:06:20.000000 reflex_antd-0.0.4/custom_components/reflex_antd.egg-info/dependency_links.txt
--rwxrwxrwx   0 see       (1000) see       (1000)       33 2024-04-23 05:06:20.000000 reflex_antd-0.0.4/custom_components/reflex_antd.egg-info/requires.txt
--rwxrwxrwx   0 see       (1000) see       (1000)       12 2024-04-23 05:06:20.000000 reflex_antd-0.0.4/custom_components/reflex_antd.egg-info/top_level.txt
--rwxrwxrwx   0 see       (1000) see       (1000)      794 2024-04-23 05:05:10.000000 reflex_antd-0.0.4/pyproject.toml
--rwxrwxrwx   0 see       (1000) see       (1000)       38 2024-04-23 05:06:24.838097 reflex_antd-0.0.4/setup.cfg
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:59.096709 reflex_antd-0.0.5/
+-rwxrwxrwx   0 see       (1000) see       (1000)    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.5/LICENSE
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-30 11:23:59.089708 reflex_antd-0.0.5/PKG-INFO
+-rwxrwxrwx   0 see       (1000) see       (1000)      336 2024-04-19 06:20:21.000000 reflex_antd-0.0.5/README.md
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:55.453099 reflex_antd-0.0.5/custom_components/
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:55.726139 reflex_antd-0.0.5/custom_components/reflex_antd/
+-rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/__init__.py
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:59.051708 reflex_antd-0.0.5/custom_components/reflex_antd/antd/
+-rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/__init__.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      679 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/affix.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3101 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/affix.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/alert.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5909 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/alert.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1028 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/anchor.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3655 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/anchor.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1549 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/auto_complete.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4382 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/auto_complete.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1025 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/avatar.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5934 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/avatar.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      825 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/badge.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6130 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/badge.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     3547 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/base.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/breadcrumb.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5451 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/breadcrumb.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      922 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/button.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3644 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/button.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1318 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/calendar.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3605 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/calendar.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1366 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/card.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8612 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/card.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      814 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/carousel.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3386 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/carousel.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2282 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/cascader.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5957 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/cascader.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1269 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/checkbox.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6026 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/checkbox.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      935 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/collapse.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3580 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/collapse.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1439 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/color_picker.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4599 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/color_picker.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4993 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/date_picker.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    17831 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/date_picker.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      709 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/descriptions.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3597 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/descriptions.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/divider.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3200 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/divider.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1398 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/drawer.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4497 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/drawer.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1518 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/dropdown.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     7254 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/dropdown.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      340 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/empty.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     2839 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/empty.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      494 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/flex.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3049 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/flex.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/float_button.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     9924 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/float_button.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     3495 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/form.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    14023 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/form.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      907 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/grid.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5943 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/grid.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2234 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/icon.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4456 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/icon.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      973 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/image.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5829 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/image.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1947 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/input.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    16141 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/input.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1565 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/input_number.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4745 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/input_number.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1645 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/layout.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    18024 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/layout.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1114 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/list.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8602 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/list.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1383 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/mentions.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4545 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/mentions.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2022 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/menu.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4675 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/menu.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4551 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/message.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3176 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/message.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/modal.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4678 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/modal.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/notification.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     1169 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/pagination.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3794 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/pagination.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      972 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/popconfirm.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3709 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/popconfirm.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      473 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/popover.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4413 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/popover.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1039 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/progress.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4279 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/progress.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      941 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/qrcode.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3635 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/qrcode.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1221 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/radio.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8759 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/radio.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/rate.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3600 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/rate.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      545 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/result.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3263 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/result.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      850 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/segmented.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3432 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/segmented.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2862 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/select.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6924 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/select.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      575 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/skeleton.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3161 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/skeleton.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1272 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/slider.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4053 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/slider.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      755 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/space.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6085 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/space.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      588 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/spin.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3247 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/spin.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1213 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/statistic.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     9147 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/statistic.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1036 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/steps.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3976 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/steps.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1042 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/switch.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3595 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/switch.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2690 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/table.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5782 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/table.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2108 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tabs.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5235 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tabs.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1063 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tag.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5717 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tag.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      566 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/timeline.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3170 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/timeline.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1352 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tooltip.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4395 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tooltip.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1237 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tour.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4192 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tour.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1997 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/transfer.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3910 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/transfer.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2609 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6180 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2869 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree_select.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6424 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree_select.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1763 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/typography.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    15437 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/typography.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1584 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/upload.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4500 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/upload.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/watermark.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3397 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/watermark.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)    24090 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/base.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    11261 2024-04-17 06:35:23.000000 reflex_antd-0.0.5/custom_components/reflex_antd/base.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1919 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/constant.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      996 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/display.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      873 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/entry.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/feedback.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      289 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/general.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      152 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/helper.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      243 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/layout.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      288 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/navigation.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     1654 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/util.py
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:59.079707 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-30 11:23:54.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/PKG-INFO
+-rwxrwxrwx   0 see       (1000) see       (1000)     6855 2024-04-30 11:23:55.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)        1 2024-04-30 11:23:54.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)       33 2024-04-30 11:23:54.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/requires.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)       12 2024-04-30 11:23:54.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/top_level.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)      794 2024-04-30 11:21:16.000000 reflex_antd-0.0.5/pyproject.toml
+-rwxrwxrwx   0 see       (1000) see       (1000)       38 2024-04-30 11:23:59.097707 reflex_antd-0.0.5/setup.cfg
```

### Comparing `reflex_antd-0.0.4/LICENSE` & `reflex_antd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/PKG-INFO` & `reflex_antd-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-antd
-Version: 0.0.4
+Version: 0.0.5
 Summary: Reflex custom component antd
 Author-email: seewind <seewindcn@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: source, https://github.com/seewindcn/reflex-antd
 Keywords: reflex,reflex-custom-components
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/affix.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/affix.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/affix.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/affix.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/alert.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/alert.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/alert.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/anchor.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/anchor.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/anchor.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/anchor.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/auto_complete.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/auto_complete.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/auto_complete.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/auto_complete.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/avatar.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/avatar.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/badge.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/badge.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/badge.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/base.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/input_number.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,47 @@
-from typing import Optional, Union, Dict
-from functools import lru_cache
-
-import reflex as rx
+from typing import Optional, Union, Dict, Any
 from reflex import Var, Component
-from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType
 
 
-from .. import base
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType
-
-
-class Locale(JsValue):
-
-    @property
-    def lang(self) -> str:
-        return self.value.replace("_", "")
-
-    def serialize(self) -> str:
-        return self.lang
-
-    def get_imports(self) -> imports.ImportDict:
-        return {
-            f'antd/locale/{self.value}': [imports.ImportVar(tag=self.lang, install=False, is_default=True)],
-        }
-
-
-class ConfigProvider(AntdComponent):
-    """Top level antd provider must be included in any app using antd components."""
-
-    tag = "ConfigProvider"
-    alias = "AntdConfigProvider"
-
-    auto_insert_space_in_button: Optional[Var[bool]]
-    component_disabled: Optional[Var[bool]]
-    component_size: Optional[Var[SizeType]]
-    csp: Optional[Var[ContainVar]]
-    direction: Optional[Var[str]]
-    get_popup_container: Optional[Var[JsValue]]
-    get_target_container: Optional[Var[JsValue]]
-    icon_prefix_cls: Optional[Var[str]]
-    locale: Optional[Var[Locale]]
-    popup_match_select_width: Optional[Var[Union[bool, int]]]
-    popup_overflow: Optional[Var[str]]
-    prefix_cls: Optional[Var[str]]
-    render_empty: Optional[Var[JsValue]]
-    theme: Optional[Var[Union[Dict, ContainVar]]]
-    virtual: Optional[Var[bool]]
-    warning: Optional[Var[Dict]]
-
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        """Create a new ConfigProvider component.
-
-        Returns:
-            A new ConfigProvider component.
-        """
-        if 'theme' not in props:
-            theme = Var.create('theme.styles.global.body.antd', _var_is_local=False)
-            props['theme'] = theme
-
-        return super().create(
-            *children,
-            **props
-        )
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        _imports.setdefault("/utils/theme.js", []).append(
-            imports.ImportVar(tag="theme", is_default=True),
-        )
-        return _imports
-
-    @staticmethod
-    @lru_cache(maxsize=None)
-    def _get_app_wrap_components() -> dict[tuple[int, str], Component]:
-        """ support app router """
-        if base.APP_ROUTER:
-            return {
-                (170, "AntdRegistryProvider"): antd_registry_provider(),
-            }
-        else:
-            return {}
-
-
-class AntdRegistryProvider(Component):
-    library = "@ant-design/nextjs-registry"
-    tag = "AntdRegistry"
+class InputNumber(AntdComponent):
+    tag = "InputNumber"
 
+    addon_after: Optional[Var[ReactNode]]
+    addon_before: Optional[Var[ReactNode]]
+    auto_focus: Optional[Var[bool]]
+    change_on_blur: Optional[Var[bool]]
+    change_on_wheel: Optional[Var[bool]]
+    controls: Optional[Var[Union[bool, ContainVar]]]
+    decimal_separator: Optional[Var[str]]
+    placeholder: Optional[Var[str]]
+    default_value: Optional[Var[int]]
+    disabled: Optional[Var[bool]]
+    formatter: Optional[Var[JsValue]]
+    keyboard: Optional[Var[bool]]
+    max: Optional[Var[int]]
+    min: Optional[Var[int]]
+    parser: Optional[Var[JsValue]]
+    precision: Optional[Var[int]]
+    read_only: Optional[Var[bool]]
+    status: Optional[Var[StatusType]]
+    prefix: Optional[Var[ReactNode]]
+    size: Optional[Var[SizeType]]
+    step: Optional[Var[Union[int, str]]]
+    string_mode: Optional[Var[bool]]
+    value: Optional[Var[int]]
+    variant: Optional[Var[VariantType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value: [value],
+            'on_press_enter': lambda e: [e],
+            "on_step": lambda value, info: [value, info],
+        })
+        return _triggers
 
-config_provider = ConfigProvider.create
-antd_registry_provider = AntdRegistryProvider.create
 
+input_number = InputNumber.create
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/base.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/image.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict
-from functools import lru_cache
-import reflex as rx
-from reflex import Var, Component
-from reflex.utils import imports
-from .. import base
+from typing import Optional, Union, Dict, Any, List
+from reflex import Component, Var
 from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType
 
-class Locale(JsValue):
+class Image(AntdComponent):
 
-    @property
-    def lang(self) -> str:
+    def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
-    def serialize(self) -> str:
-        ...
-
-    def get_imports(self) -> imports.ImportDict:
-        ...
-
-class ConfigProvider(AntdComponent):
-
     @overload
     @classmethod
-    def create(cls, *children, auto_insert_space_in_button: Optional[Union[Var[bool], bool]]=None, component_disabled: Optional[Union[Var[bool], bool]]=None, component_size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, csp: Optional[Union[Var[ContainVar], ContainVar]]=None, direction: Optional[Union[Var[str], str]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, get_target_container: Optional[Union[Var[JsValue], JsValue]]=None, icon_prefix_cls: Optional[Union[Var[str], str]]=None, locale: Optional[Union[Var[Locale], Locale]]=None, popup_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, popup_overflow: Optional[Union[Var[str], str]]=None, prefix_cls: Optional[Union[Var[str], str]]=None, render_empty: Optional[Union[Var[JsValue], JsValue]]=None, theme: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, virtual: Optional[Union[Var[bool], bool]]=None, warning: Optional[Union[Var[Dict], Dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'ConfigProvider':
-        """Create a new ConfigProvider component.
+    def create(cls, *children, alt: Optional[Union[Var[str], str]]=None, fallback: Optional[Union[Var[str], str]]=None, height: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, placeholder: Optional[Union[Var[Component], Component]]=None, description: Optional[Union[Var[Component], Component]]=None, preview: Optional[Union[Var[Union[bool, dict]], Union[bool, dict]]]=None, src: Optional[Union[Var[str], str]]=None, width: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_error: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Image':
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
 
         Returns:
-            A new ConfigProvider component.
+            The component.
+
+        Raises:
+            TypeError: If an invalid child is passed.
         """
         ...
 
-class AntdRegistryProvider(Component):
+class ImagePreviewGroup(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AntdRegistryProvider':
+    def create(cls, *children, preview: Optional[Union[Var[Union[bool, Component]], Union[bool, Component]]]=None, items: Optional[Union[Var[list], list]]=None, fallback: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'ImagePreviewGroup':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
@@ -55,9 +54,9 @@
         Returns:
             The component.
 
         Raises:
             TypeError: If an invalid child is passed.
         """
         ...
-config_provider = ConfigProvider.create
-antd_registry_provider = AntdRegistryProvider.create
+image = Image.create
+image_preview_group = ImagePreviewGroup.create
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/breadcrumb.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/breadcrumb.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/button.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/button.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/button.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/calendar.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/calendar.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/calendar.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/calendar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/card.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/card.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/card.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/carousel.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/carousel.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/carousel.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/carousel.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/cascader.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/cascader.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/cascader.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/cascader.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/checkbox.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/checkbox.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/collapse.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/collapse.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/collapse.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/collapse.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/color_picker.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/color_picker.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/color_picker.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/color_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/date_picker.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/date_picker.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/date_picker.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/descriptions.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/descriptions.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/descriptions.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/descriptions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/divider.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/drawer.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/drawer.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/dropdown.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/dropdown.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/dropdown.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/dropdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/empty.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/empty.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/flex.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/float_button.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/float_button.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/float_button.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/float_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/form.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/form.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/form.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/grid.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/grid.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/grid.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/icon.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/icon.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/icon.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/image.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/image.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/image.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tag.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List
+from typing import Optional, Union, Dict, Any, List, Tuple
 from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import TimelineModeType
 
-class Image(AntdComponent):
+class Tag(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, alt: Optional[Union[Var[str], str]]=None, fallback: Optional[Union[Var[str], str]]=None, height: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, placeholder: Optional[Union[Var[Component], Component]]=None, description: Optional[Union[Var[Component], Component]]=None, preview: Optional[Union[Var[Union[bool, dict]], Union[bool, dict]]]=None, src: Optional[Union[Var[str], str]]=None, width: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_error: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Image':
+    def create(cls, *children, close_icon: Optional[Union[Var[Union[bool, Component]], Union[bool, Component]]]=None, color: Optional[Union[Var[str], str]]=None, icon: Optional[Union[Var[Component], Component]]=None, bordered: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_close: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tag':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
@@ -30,19 +33,22 @@
             The component.
 
         Raises:
             TypeError: If an invalid child is passed.
         """
         ...
 
-class ImagePreviewGroup(AntdComponent):
+class CheckableTag(AntdComponent):
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
 
     @overload
     @classmethod
-    def create(cls, *children, preview: Optional[Union[Var[Union[bool, Component]], Union[bool, Component]]]=None, items: Optional[Union[Var[list], list]]=None, fallback: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'ImagePreviewGroup':
+    def create(cls, *children, checked: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CheckableTag':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
@@ -54,9 +60,9 @@
         Returns:
             The component.
 
         Raises:
             TypeError: If an invalid child is passed.
         """
         ...
-image = Image.create
-image_preview_group = ImagePreviewGroup.create
+tag = Tag.create
+checkable_tag = CheckableTag.create
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/input.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/input.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/input.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/input_number.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Optional, Union, Dict, Any
+from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, VariantType
+from ..base import AntdComponent, ContainVar, JsValue
 
 
-class InputNumber(AntdComponent):
-    tag = "InputNumber"
+class Upload(AntdComponent):
+    tag = 'Upload'
 
-    addon_after: Optional[Var[ReactNode]]
-    addon_before: Optional[Var[ReactNode]]
-    auto_focus: Optional[Var[bool]]
-    change_on_blur: Optional[Var[bool]]
-    change_on_wheel: Optional[Var[bool]]
-    controls: Optional[Var[Union[bool, ContainVar]]]
-    decimal_separator: Optional[Var[str]]
-    placeholder: Optional[Var[str]]
-    default_value: Optional[Var[int]]
+    accept: Optional[Var[str]]
+    action: Optional[Var[Union[str, JsValue]]]
+    before_upload: Optional[Var[JsValue]]
+    custom_request: Optional[Var[JsValue]]
+    data: Optional[Var[Union[ContainVar, JsValue]]]
+    default_file_list: Optional[Var[List[ContainVar]]]
+    directory: Optional[Var[bool]]
     disabled: Optional[Var[bool]]
-    formatter: Optional[Var[JsValue]]
-    keyboard: Optional[Var[bool]]
-    max: Optional[Var[int]]
-    min: Optional[Var[int]]
-    parser: Optional[Var[JsValue]]
-    precision: Optional[Var[int]]
-    read_only: Optional[Var[bool]]
-    status: Optional[Var[StatusType]]
-    prefix: Optional[Var[ReactNode]]
-    size: Optional[Var[SizeType]]
-    step: Optional[Var[Union[int, str]]]
-    string_mode: Optional[Var[bool]]
-    value: Optional[Var[int]]
-    variant: Optional[Var[VariantType]]
+    file_list: Optional[Var[List[ContainVar]]]
+    headers: Optional[Var[Dict]]
+    icon_render: Optional[Var[JsValue]]
+    is_image_url: Optional[Var[JsValue]]
+    list_type: Optional[Var[str]]
+    max_count: Optional[Var[int]]
+    method: Optional[Var[str]]
+    multiple: Optional[Var[bool]]
+    name: Optional[Var[str]]
+    open_file_dialog_on_click: Optional[Var[bool]]
+    preview_file: Optional[Var[JsValue]]
+    progress: Optional[Var[Dict]]
+    show_upload_list: Optional[Var[Union[bool, Dict]]]
+    with_credentials: Optional[Var[Union[bool]]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value: [value],
-            'on_press_enter': lambda e: [e],
-            "on_step": lambda value, info: [value, info],
+            EventTriggers.ON_CHANGE: lambda file, file_list: [file, file_list],
+            "on_drop": lambda event: [event],
+            "on_download": lambda file: [file],
+            "on_preview": lambda file: [file],
+            "on_remove": lambda file: [file]
         })
         return _triggers
 
 
-input_number = InputNumber.create
+upload = Upload.create
+
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/input_number.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/input_number.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/layout.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/layout.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/layout.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/layout.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/list.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/list.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/list.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/mentions.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/mentions.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/mentions.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/mentions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/menu.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/menu.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional, Union, Type, Dict, List, Any, Iterator
-from pydantic import BaseModel
+from reflex.base import pydantic
 from reflex import Component, Var, EventChain, Base
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
 from ..base import AntdComponent, AntdSubComponent, ContainVar, ReactNode
 from ..constant import ThemeType, DirectionType, TriggerType
 
 
-class MenuItem(BaseModel):
+class MenuItem(pydantic.BaseModel):
     key: str
     label: str
     icon: Component
     children: Optional[List["MenuItem"]] = None
 
 
 # class MenuItems(ContainVar):
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/menu.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/message.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/message.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/message.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/message.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/modal.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/modal.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/modal.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/notification.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/notification.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/pagination.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/pagination.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/pagination.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/pagination.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/popconfirm.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/popconfirm.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/popconfirm.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/popconfirm.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/popover.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/progress.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/progress.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/progress.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/qrcode.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/qrcode.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/qrcode.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/qrcode.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/radio.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/radio.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/radio.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/rate.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/rate.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/rate.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/rate.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/result.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/result.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/result.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/result.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/segmented.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/segmented.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/segmented.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/segmented.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/select.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/select.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/select.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/skeleton.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/skeleton.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/slider.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/slider.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/slider.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/space.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/space.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/space.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/space.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/spin.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/spin.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/spin.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/spin.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/statistic.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/statistic.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/statistic.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/statistic.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/steps.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/steps.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/steps.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/steps.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/switch.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/switch.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/switch.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/table.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/table.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/table.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tabs.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tabs.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tag.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tag.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tag.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,31 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List, Tuple
-from reflex import Component, Var
-from reflex.utils import imports
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import TimelineModeType
-
-class Tag(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
-
-    @overload
-    @classmethod
-    def create(cls, *children, close_icon: Optional[Union[Var[Union[bool, Component]], Union[bool, Component]]]=None, color: Optional[Union[Var[str], str]]=None, icon: Optional[Union[Var[Component], Component]]=None, bordered: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_close: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tag':
-        """Create the component.
-
-        Args:
-            *children: The children of the component.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
-
-        Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
-        """
-        ...
+from reflex.utils import imports
+from ..base import AntdComponent, ContainVar, JsNode, ReactNode
+from ..constant import StatusType, SizeType
 
-class CheckableTag(AntdComponent):
+class Tree(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, checked: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CheckableTag':
+    def create(cls, *children, allow_drop: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, auto_expand_parent: Optional[Union[Var[bool], bool]]=None, block_node: Optional[Union[Var[bool], bool]]=None, checkable: Optional[Union[Var[bool], bool]]=None, checked_keys: Optional[Union[Var[Union[List, Dict]], Union[List, Dict]]]=None, check_strictly: Optional[Union[Var[bool], bool]]=None, default_checked_keys: Optional[Union[Var[List[str]], List[str]]]=None, default_expand_all: Optional[Union[Var[bool], bool]]=None, default_expanded_keys: Optional[Union[Var[List[str]], List[str]]]=None, default_expand_parent: Optional[Union[Var[bool], bool]]=None, default_selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, draggable: Optional[Union[Var[Union[bool, JsValue, JsEvent, ContainVar]], Union[bool, JsValue, JsEvent, ContainVar]]]=None, expanded_keys: Optional[Union[Var[List[str]], List[str]]]=None, field_names: Optional[Union[Var[Dict], Dict]]=None, filter_tree_node: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, height: Optional[Union[Var[int], int]]=None, icon: Optional[Union[Var[Union[str, Component, JsValue, JsEvent]], Union[str, Component, JsValue, JsEvent]]]=None, load_data: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, loaded_keys: Optional[Union[Var[List[str]], List[str]]]=None, multiple: Optional[Union[Var[bool], bool]]=None, root_style: Optional[Union[Var[Dict], Dict]]=None, selectable: Optional[Union[Var[bool], bool]]=None, selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, show_icon: Optional[Union[Var[bool], bool]]=None, show_line: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, switcher_icon: Optional[Union[Var[Union[str, Component, JsValue, JsEvent]], Union[str, Component, JsValue, JsEvent]]]=None, title_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, tree_data: Optional[Union[Var[List[Dict]], List[Dict]]]=None, virtual: Optional[Union[Var[bool], bool]]=None, expand_action: Optional[Union[Var[Union[bool, str]], Union[bool, str]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, filter_tree_node: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, load_data: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_check: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_end: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_start: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drop: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_expand: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_load: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_right_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tree':
         """Create the component.
 
         Args:
             *children: The children of the component.
+            expand_action: DirectoryTree
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
@@ -60,9 +33,8 @@
         Returns:
             The component.
 
         Raises:
             TypeError: If an invalid child is passed.
         """
         ...
-tag = Tag.create
-checkable_tag = CheckableTag.create
+tree = Tree.create
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/timeline.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/timeline.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/timeline.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/timeline.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tooltip.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tooltip.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tour.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tour.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tour.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tour.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/transfer.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/transfer.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/transfer.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/transfer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tree.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tree.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree_select.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
-from reflex.utils import imports
-from ..base import AntdComponent, ContainVar, JsNode, ReactNode
-from ..constant import StatusType, SizeType
+from ..base import AntdComponent, ContainVar, JsNode
 
-class Tree(AntdComponent):
+class TreeSelect(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, allow_drop: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, auto_expand_parent: Optional[Union[Var[bool], bool]]=None, block_node: Optional[Union[Var[bool], bool]]=None, checkable: Optional[Union[Var[bool], bool]]=None, checked_keys: Optional[Union[Var[Union[List, Dict]], Union[List, Dict]]]=None, check_strictly: Optional[Union[Var[bool], bool]]=None, default_checked_keys: Optional[Union[Var[List[str]], List[str]]]=None, default_expand_all: Optional[Union[Var[bool], bool]]=None, default_expanded_keys: Optional[Union[Var[List[str]], List[str]]]=None, default_expand_parent: Optional[Union[Var[bool], bool]]=None, default_selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, draggable: Optional[Union[Var[Union[bool, JsValue, JsEvent, ContainVar]], Union[bool, JsValue, JsEvent, ContainVar]]]=None, expanded_keys: Optional[Union[Var[List[str]], List[str]]]=None, field_names: Optional[Union[Var[Dict], Dict]]=None, filter_tree_node: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, height: Optional[Union[Var[int], int]]=None, icon: Optional[Union[Var[Union[str, Component, JsValue, JsEvent]], Union[str, Component, JsValue, JsEvent]]]=None, load_data: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, loaded_keys: Optional[Union[Var[List[str]], List[str]]]=None, multiple: Optional[Union[Var[bool], bool]]=None, root_style: Optional[Union[Var[Dict], Dict]]=None, selectable: Optional[Union[Var[bool], bool]]=None, selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, show_icon: Optional[Union[Var[bool], bool]]=None, show_line: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, switcher_icon: Optional[Union[Var[Union[str, Component, JsValue, JsEvent]], Union[str, Component, JsValue, JsEvent]]]=None, title_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, tree_data: Optional[Union[Var[List[Dict]], List[Dict]]]=None, virtual: Optional[Union[Var[bool], bool]]=None, expand_action: Optional[Union[Var[Union[bool, str]], Union[bool, str]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, filter_tree_node: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, load_data: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_check: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_end: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drag_start: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drop: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_expand: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_load: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_right_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tree':
+    def create(cls, *children, allow_clear: Optional[Union[Var[Union[bool, Component]], Union[bool, Component]]]=None, auto_clear_search_value: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, popup_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, dropdown_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, dropdown_style: Optional[Union[Var[Dict], Dict]]=None, field_names: Optional[Union[Var[Dict], Dict]]=None, filter_tree_node: Optional[Union[Var[Union[bool, JsValue, JsEvent]], Union[bool, JsValue, JsEvent]]]=None, get_popup_container: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, label_in_value: Optional[Union[Var[bool], bool]]=None, list_height: Optional[Union[Var[int], int]]=None, load_data: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, max_tag_count: Optional[Union[Var[int], int]]=None, max_tag_placeholder: Optional[Union[Var[Union[Component, JsValue, JsEvent]], Union[Component, JsValue, JsEvent]]]=None, max_tag_text_length: Optional[Union[Var[int], int]]=None, multiple: Optional[Union[Var[bool], bool]]=None, not_found_content: Optional[Union[Var[Component], Component]]=None, placeholder: Optional[Union[Var[str], str]]=None, placement: Optional[Union[Var[str], str]]=None, search_value: Optional[Union[Var[str], str]]=None, show_checked_strategy: Optional[Union[Var[str], str]]=None, show_search: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[str], str]]=None, status: Optional[Union[Var[str], str]]=None, suffix_icon: Optional[Union[Var[Component], Component]]=None, switcher_icon: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, tag_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, tree_checkable: Optional[Union[Var[bool], bool]]=None, tree_check_strictly: Optional[Union[Var[bool], bool]]=None, tree_data: Optional[Union[Var[List[Dict]], List[Dict]]]=None, tree_data_simple_mode: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, tree_default_expand_all: Optional[Union[Var[bool], bool]]=None, tree_default_expanded_keys: Optional[Union[Var[List], List]]=None, tree_expand_action: Optional[Union[Var[Union[str, bool]], Union[str, bool]]]=None, tree_expanded_keys: Optional[Union[Var[List[str]], List[str]]]=None, tree_icon: Optional[Union[Var[bool], bool]]=None, tree_line: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, tree_loaded_keys: Optional[Union[Var[List[str]], List[str]]]=None, tree_node_filter_prop: Optional[Union[Var[str], str]]=None, tree_node_label_prop: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, variant: Optional[Union[Var[str], str]]=None, virtual: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, filter_tree_node: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, load_data: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tree_expand: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'TreeSelect':
         """Create the component.
 
         Args:
             *children: The children of the component.
-            expand_action: DirectoryTree
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
@@ -33,8 +30,8 @@
         Returns:
             The component.
 
         Raises:
             TypeError: If an invalid child is passed.
         """
         ...
-tree = Tree.create
+tree_select = TreeSelect.create
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tree_select.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree_select.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/tree_select.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/upload.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsNode
+from ..base import AntdComponent, ContainVar, JsValue
 
-class TreeSelect(AntdComponent):
+class Upload(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, allow_clear: Optional[Union[Var[Union[bool, Component]], Union[bool, Component]]]=None, auto_clear_search_value: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, popup_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, dropdown_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, dropdown_style: Optional[Union[Var[Dict], Dict]]=None, field_names: Optional[Union[Var[Dict], Dict]]=None, filter_tree_node: Optional[Union[Var[Union[bool, JsValue, JsEvent]], Union[bool, JsValue, JsEvent]]]=None, get_popup_container: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, label_in_value: Optional[Union[Var[bool], bool]]=None, list_height: Optional[Union[Var[int], int]]=None, load_data: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, max_tag_count: Optional[Union[Var[int], int]]=None, max_tag_placeholder: Optional[Union[Var[Union[Component, JsValue, JsEvent]], Union[Component, JsValue, JsEvent]]]=None, max_tag_text_length: Optional[Union[Var[int], int]]=None, multiple: Optional[Union[Var[bool], bool]]=None, not_found_content: Optional[Union[Var[Component], Component]]=None, placeholder: Optional[Union[Var[str], str]]=None, placement: Optional[Union[Var[str], str]]=None, search_value: Optional[Union[Var[str], str]]=None, show_checked_strategy: Optional[Union[Var[str], str]]=None, show_search: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[str], str]]=None, status: Optional[Union[Var[str], str]]=None, suffix_icon: Optional[Union[Var[Component], Component]]=None, switcher_icon: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, tag_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, tree_checkable: Optional[Union[Var[bool], bool]]=None, tree_check_strictly: Optional[Union[Var[bool], bool]]=None, tree_data: Optional[Union[Var[List[Dict]], List[Dict]]]=None, tree_data_simple_mode: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, tree_default_expand_all: Optional[Union[Var[bool], bool]]=None, tree_default_expanded_keys: Optional[Union[Var[List], List]]=None, tree_expand_action: Optional[Union[Var[Union[str, bool]], Union[str, bool]]]=None, tree_expanded_keys: Optional[Union[Var[List[str]], List[str]]]=None, tree_icon: Optional[Union[Var[bool], bool]]=None, tree_line: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, tree_loaded_keys: Optional[Union[Var[List[str]], List[str]]]=None, tree_node_filter_prop: Optional[Union[Var[str], str]]=None, tree_node_label_prop: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, variant: Optional[Union[Var[str], str]]=None, virtual: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, filter_tree_node: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, load_data: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tree_expand: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'TreeSelect':
+    def create(cls, *children, accept: Optional[Union[Var[str], str]]=None, action: Optional[Union[Var[Union[str, JsValue]], Union[str, JsValue]]]=None, before_upload: Optional[Union[Var[JsValue], JsValue]]=None, custom_request: Optional[Union[Var[JsValue], JsValue]]=None, data: Optional[Union[Var[Union[ContainVar, JsValue]], Union[ContainVar, JsValue]]]=None, default_file_list: Optional[Union[Var[List[ContainVar]], List[ContainVar]]]=None, directory: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, file_list: Optional[Union[Var[List[ContainVar]], List[ContainVar]]]=None, headers: Optional[Union[Var[Dict], Dict]]=None, icon_render: Optional[Union[Var[JsValue], JsValue]]=None, is_image_url: Optional[Union[Var[JsValue], JsValue]]=None, list_type: Optional[Union[Var[str], str]]=None, max_count: Optional[Union[Var[int], int]]=None, method: Optional[Union[Var[str], str]]=None, multiple: Optional[Union[Var[bool], bool]]=None, name: Optional[Union[Var[str], str]]=None, open_file_dialog_on_click: Optional[Union[Var[bool], bool]]=None, preview_file: Optional[Union[Var[JsValue], JsValue]]=None, progress: Optional[Union[Var[Dict], Dict]]=None, show_upload_list: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, with_credentials: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_download: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drop: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_preview: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_remove: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Upload':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
@@ -30,8 +30,8 @@
         Returns:
             The component.
 
         Raises:
             TypeError: If an invalid child is passed.
         """
         ...
-tree_select = TreeSelect.create
+upload = Upload.create
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/typography.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/typography.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/typography.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/upload.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/watermark.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
+from typing import Optional, Union, Dict, Any, List, Tuple
+from reflex import Component, Var
+from reflex.utils import imports
 from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import OrientationType, DirectionType
 
-class Upload(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
+class Watermark(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, accept: Optional[Union[Var[str], str]]=None, action: Optional[Union[Var[Union[str, JsValue]], Union[str, JsValue]]]=None, before_upload: Optional[Union[Var[JsValue], JsValue]]=None, custom_request: Optional[Union[Var[JsValue], JsValue]]=None, data: Optional[Union[Var[Union[ContainVar, JsValue]], Union[ContainVar, JsValue]]]=None, default_file_list: Optional[Union[Var[List[ContainVar]], List[ContainVar]]]=None, directory: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, file_list: Optional[Union[Var[List[ContainVar]], List[ContainVar]]]=None, headers: Optional[Union[Var[Dict], Dict]]=None, icon_render: Optional[Union[Var[JsValue], JsValue]]=None, is_image_url: Optional[Union[Var[JsValue], JsValue]]=None, list_type: Optional[Union[Var[str], str]]=None, max_count: Optional[Union[Var[int], int]]=None, method: Optional[Union[Var[str], str]]=None, multiple: Optional[Union[Var[bool], bool]]=None, name: Optional[Union[Var[str], str]]=None, open_file_dialog_on_click: Optional[Union[Var[bool], bool]]=None, preview_file: Optional[Union[Var[JsValue], JsValue]]=None, progress: Optional[Union[Var[Dict], Dict]]=None, show_upload_list: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, with_credentials: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_download: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drop: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_preview: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_remove: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Upload':
+    def create(cls, *children, width: Optional[Union[Var[int], int]]=None, height: Optional[Union[Var[int], int]]=None, inherit: Optional[Union[Var[bool], bool]]=None, rotate: Optional[Union[Var[int], int]]=None, z_index: Optional[Union[Var[int], int]]=None, image: Optional[Union[Var[str], str]]=None, content: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, font: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, gap: Optional[Union[Var[Tuple[int, int]], Tuple[int, int]]]=None, offset: Optional[Union[Var[Tuple[int, int]], Tuple[int, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Watermark':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
@@ -30,8 +29,8 @@
         Returns:
             The component.
 
         Raises:
             TypeError: If an invalid child is passed.
         """
         ...
-upload = Upload.create
+watermark = Watermark.create
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/antd/watermark.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/antd/watermark.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/base.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -390,16 +390,40 @@
     def get_hooks(self) -> Set[str] | Dict[str, None]:
         return self.item.get_hooks()
 
     def get_custom_components(self) -> set[CustomComponent]:
         return self.item.get_custom_components()
 
 
+class ExVarItem(ExItem):
+    item: Var
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, Var)
+
+    def serialize(self) -> str:
+        return str(self.item).strip('{}')
+
+    def get_imports(self) -> imports.ImportDict:
+        return self.item._var_data.imports if self.item._var_data else {}
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return self.item._var_data.hooks if self.item._var_data else {}
+
+    def get_state(self) -> str:
+        return self.item._var_data.state if self.item._var_data else ""
+
+    def get_interpolations(self) -> List[Tuple[int, int]]:
+        return self.item._var_data.interpolations if self.item._var_data else []
+
+
 class ExFormatter:
     items: List[Type[ExItem]] = [
+        ExVarItem,
         ExStatefulComponentItem,
         ExComponentItem,
         ExStateItem,
         ExJsItem,
         ExEventHandlerItem,
         ExLambdaHandlerItem,
         # ExCallableItem,
@@ -684,15 +708,15 @@
     _custom_components: Set[CustomComponent] = pydantic.PrivateAttr(default_factory=set)
 
     @staticmethod
     @lru_cache(maxsize=None)
     def _get_app_wrap_components() -> dict[tuple[int, str], Component]:
         from .antd.base import config_provider
         return {
-            (160, "AntdProvider"): _config_provider if _config_provider is not None else config_provider(),
+            (40, "AntdProvider"): _config_provider if _config_provider is not None else config_provider(),
         }
 
     def __init__(self, *args, **kwargs):
         contains = {}
         exs = {}
         kw = {}
         for k, v in kwargs.items():
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/base.pyi` & `reflex_antd-0.0.5/custom_components/reflex_antd/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/constant.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/constant.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/display.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/display.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/entry.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/entry.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd/util.py` & `reflex_antd-0.0.5/custom_components/reflex_antd/util.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd.egg-info/PKG-INFO` & `reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-antd
-Version: 0.0.4
+Version: 0.0.5
 Summary: Reflex custom component antd
 Author-email: seewind <seewindcn@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: source, https://github.com/seewindcn/reflex-antd
 Keywords: reflex,reflex-custom-components
```

### Comparing `reflex_antd-0.0.4/custom_components/reflex_antd.egg-info/SOURCES.txt` & `reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 custom_components/reflex_antd/antd/auto_complete.py
 custom_components/reflex_antd/antd/auto_complete.pyi
 custom_components/reflex_antd/antd/avatar.py
 custom_components/reflex_antd/antd/avatar.pyi
 custom_components/reflex_antd/antd/badge.py
 custom_components/reflex_antd/antd/badge.pyi
 custom_components/reflex_antd/antd/base.py
-custom_components/reflex_antd/antd/base.pyi
 custom_components/reflex_antd/antd/breadcrumb.py
 custom_components/reflex_antd/antd/breadcrumb.pyi
 custom_components/reflex_antd/antd/button.py
 custom_components/reflex_antd/antd/button.pyi
 custom_components/reflex_antd/antd/calendar.py
 custom_components/reflex_antd/antd/calendar.pyi
 custom_components/reflex_antd/antd/card.py
```

### Comparing `reflex_antd-0.0.4/pyproject.toml` & `reflex_antd-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-antd"
-version = "0.0.4"
+version = "0.0.5"
 description = "Reflex custom component antd"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "seewind", email = "seewindcn@gmail.com" }]
 keywords = [
     "reflex",
```

