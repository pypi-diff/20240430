# Comparing `tmp/kytest-0.0.8.tar.gz` & `tmp/kytest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kytest-0.0.8.tar", last modified: Wed Dec  6 13:00:39 2023, max compression
+gzip compressed data, was "kytest-0.0.9.tar", last modified: Mon Dec 11 12:26:11 2023, max compression
```

## Comparing `kytest-0.0.8.tar` & `kytest-0.0.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.149425 kytest-0.0.8/
--rw-r--r--   0 UI         (502) staff       (20)      310 2023-12-06 13:00:39.148825 kytest-0.0.8/PKG-INFO
--rw-r--r--   0 UI         (502) staff       (20)     5022 2023-12-06 06:47:55.000000 kytest-0.0.8/README.md
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.105953 kytest-0.0.8/demo/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.8/demo/__init__.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.110258 kytest-0.0.8/demo/pages/
--rw-r--r--   0 UI         (502) staff       (20)       49 2023-11-17 09:46:58.000000 kytest-0.0.8/demo/pages/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      376 2023-11-22 00:59:13.000000 kytest-0.0.8/demo/pages/adr_page.py
--rw-r--r--   0 UI         (502) staff       (20)      383 2023-11-22 09:34:21.000000 kytest-0.0.8/demo/pages/image_page.py
--rw-r--r--   0 UI         (502) staff       (20)      273 2023-11-22 00:56:24.000000 kytest-0.0.8/demo/pages/ios_page.py
--rw-r--r--   0 UI         (502) staff       (20)      619 2023-11-22 09:40:23.000000 kytest-0.0.8/demo/pages/web_page.py
--rw-r--r--   0 UI         (502) staff       (20)      222 2023-12-04 13:15:52.000000 kytest-0.0.8/demo/run.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.114521 kytest-0.0.8/demo/tests/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.8/demo/tests/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      634 2023-12-04 13:14:35.000000 kytest-0.0.8/demo/tests/test_adr.py
--rw-r--r--   0 UI         (502) staff       (20)      544 2023-11-22 01:02:26.000000 kytest-0.0.8/demo/tests/test_api.py
--rw-r--r--   0 UI         (502) staff       (20)      664 2023-12-04 13:15:18.000000 kytest-0.0.8/demo/tests/test_image.py
--rw-r--r--   0 UI         (502) staff       (20)      620 2023-12-04 13:14:52.000000 kytest-0.0.8/demo/tests/test_ios.py
--rw-r--r--   0 UI         (502) staff       (20)     1033 2023-12-04 13:15:18.000000 kytest-0.0.8/demo/tests/test_web.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.117372 kytest-0.0.8/kytest/
--rw-r--r--   0 UI         (502) staff       (20)      521 2023-12-06 05:52:36.000000 kytest-0.0.8/kytest/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     3700 2023-11-22 09:29:35.000000 kytest-0.0.8/kytest/case.py
--rw-r--r--   0 UI         (502) staff       (20)      491 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/cli.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.120422 kytest-0.0.8/kytest/core/
--rw-r--r--   0 UI         (502) staff       (20)       51 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/core/__init__.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.122324 kytest-0.0.8/kytest/core/android/
--rw-r--r--   0 UI         (502) staff       (20)      134 2023-11-22 01:37:15.000000 kytest-0.0.8/kytest/core/android/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     7149 2023-12-06 05:50:28.000000 kytest-0.0.8/kytest/core/android/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     9044 2023-12-05 07:23:41.000000 kytest-0.0.8/kytest/core/android/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.123787 kytest-0.0.8/kytest/core/api/
--rw-r--r--   0 UI         (502) staff       (20)        1 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/core/api/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    12299 2023-11-22 01:56:14.000000 kytest-0.0.8/kytest/core/api/request.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.126191 kytest-0.0.8/kytest/core/image/
--rw-r--r--   0 UI         (502) staff       (20)       53 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/core/image/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     1692 2023-11-22 02:05:24.000000 kytest-0.0.8/kytest/core/image/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     3100 2023-11-22 02:08:29.000000 kytest-0.0.8/kytest/core/image/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.128288 kytest-0.0.8/kytest/core/ios/
--rw-r--r--   0 UI         (502) staff       (20)      134 2023-11-22 01:37:52.000000 kytest-0.0.8/kytest/core/ios/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     6582 2023-12-06 05:52:08.000000 kytest-0.0.8/kytest/core/ios/driver.py
--rw-r--r--   0 UI         (502) staff       (20)    11574 2023-12-05 07:23:56.000000 kytest-0.0.8/kytest/core/ios/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.130832 kytest-0.0.8/kytest/core/ocr/
--rw-r--r--   0 UI         (502) staff       (20)       85 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/core/ocr/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      746 2023-11-22 02:07:34.000000 kytest-0.0.8/kytest/core/ocr/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     4222 2023-11-22 02:09:35.000000 kytest-0.0.8/kytest/core/ocr/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.133232 kytest-0.0.8/kytest/core/web/
--rw-r--r--   0 UI         (502) staff       (20)       95 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/core/web/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     2745 2023-11-22 01:58:00.000000 kytest-0.0.8/kytest/core/web/driver.py
--rw-r--r--   0 UI         (502) staff       (20)    10636 2023-11-22 02:04:39.000000 kytest-0.0.8/kytest/core/web/element.py
--rw-r--r--   0 UI         (502) staff       (20)      904 2023-11-22 02:47:18.000000 kytest-0.0.8/kytest/page.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.135431 kytest-0.0.8/kytest/running/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/running/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      182 2023-12-05 07:51:08.000000 kytest-0.0.8/kytest/running/conf.yml
--rw-r--r--   0 UI         (502) staff       (20)     3809 2023-12-04 13:14:48.000000 kytest-0.0.8/kytest/running/runner.py
--rw-r--r--   0 UI         (502) staff       (20)     2667 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/scaffold.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.137051 kytest-0.0.8/kytest/testdata/
--rw-r--r--   0 UI         (502) staff       (20)    10650 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/testdata/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    18623 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/testdata/data.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.147984 kytest-0.0.8/kytest/utils/
--rw-r--r--   0 UI         (502) staff       (20)        1 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/utils/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     6789 2023-11-22 02:40:54.000000 kytest-0.0.8/kytest/utils/allure_util.py
--rw-r--r--   0 UI         (502) staff       (20)     8036 2023-11-22 02:43:09.000000 kytest-0.0.8/kytest/utils/common.py
--rw-r--r--   0 UI         (502) staff       (20)     3445 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/utils/config.py
--rw-r--r--   0 UI         (502) staff       (20)     1396 2023-11-22 02:43:46.000000 kytest-0.0.8/kytest/utils/des_util.py
--rw-r--r--   0 UI         (502) staff       (20)     3277 2023-11-22 02:43:56.000000 kytest-0.0.8/kytest/utils/dingtalk.py
--rw-r--r--   0 UI         (502) staff       (20)     3787 2023-11-22 02:44:11.000000 kytest-0.0.8/kytest/utils/excel.py
--rw-r--r--   0 UI         (502) staff       (20)      159 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/utils/exceptions.py
--rw-r--r--   0 UI         (502) staff       (20)      710 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/utils/log.py
--rw-r--r--   0 UI         (502) staff       (20)     3930 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/utils/mail.py
--rw-r--r--   0 UI         (502) staff       (20)     2179 2023-11-17 09:46:58.000000 kytest-0.0.8/kytest/utils/mysql_util.py
--rw-r--r--   0 UI         (502) staff       (20)     2402 2023-11-22 02:45:31.000000 kytest-0.0.8/kytest/utils/pytest_util.py
--rw-r--r--   0 UI         (502) staff       (20)     4022 2023-11-22 02:45:53.000000 kytest-0.0.8/kytest/utils/swagger_util.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-06 13:00:39.119973 kytest-0.0.8/kytest.egg-info/
--rw-r--r--   0 UI         (502) staff       (20)      310 2023-12-06 13:00:39.000000 kytest-0.0.8/kytest.egg-info/PKG-INFO
--rw-r--r--   0 UI         (502) staff       (20)     1521 2023-12-06 13:00:39.000000 kytest-0.0.8/kytest.egg-info/SOURCES.txt
--rw-r--r--   0 UI         (502) staff       (20)        1 2023-12-06 13:00:39.000000 kytest-0.0.8/kytest.egg-info/dependency_links.txt
--rw-r--r--   0 UI         (502) staff       (20)       43 2023-12-06 13:00:39.000000 kytest-0.0.8/kytest.egg-info/entry_points.txt
--rw-r--r--   0 UI         (502) staff       (20)      301 2023-12-06 13:00:39.000000 kytest-0.0.8/kytest.egg-info/requires.txt
--rw-r--r--   0 UI         (502) staff       (20)       12 2023-12-06 13:00:39.000000 kytest-0.0.8/kytest.egg-info/top_level.txt
--rw-r--r--   0 UI         (502) staff       (20)       38 2023-12-06 13:00:39.149605 kytest-0.0.8/setup.cfg
--rw-r--r--   0 UI         (502) staff       (20)     1363 2023-11-17 09:53:12.000000 kytest-0.0.8/setup.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.312135 kytest-0.0.9/
+-rw-r--r--   0 UI         (502) staff       (20)      310 2023-12-11 12:26:11.311479 kytest-0.0.9/PKG-INFO
+-rw-r--r--   0 UI         (502) staff       (20)     5022 2023-12-06 06:47:55.000000 kytest-0.0.9/README.md
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.265505 kytest-0.0.9/demo/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.9/demo/__init__.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.269543 kytest-0.0.9/demo/pages/
+-rw-r--r--   0 UI         (502) staff       (20)       49 2023-11-17 09:46:58.000000 kytest-0.0.9/demo/pages/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      376 2023-11-22 00:59:13.000000 kytest-0.0.9/demo/pages/adr_page.py
+-rw-r--r--   0 UI         (502) staff       (20)      383 2023-11-22 09:34:21.000000 kytest-0.0.9/demo/pages/image_page.py
+-rw-r--r--   0 UI         (502) staff       (20)      273 2023-11-22 00:56:24.000000 kytest-0.0.9/demo/pages/ios_page.py
+-rw-r--r--   0 UI         (502) staff       (20)      619 2023-11-22 09:40:23.000000 kytest-0.0.9/demo/pages/web_page.py
+-rw-r--r--   0 UI         (502) staff       (20)      222 2023-12-04 13:15:52.000000 kytest-0.0.9/demo/run.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.274508 kytest-0.0.9/demo/tests/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.9/demo/tests/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      634 2023-12-04 13:14:35.000000 kytest-0.0.9/demo/tests/test_adr.py
+-rw-r--r--   0 UI         (502) staff       (20)      544 2023-11-22 01:02:26.000000 kytest-0.0.9/demo/tests/test_api.py
+-rw-r--r--   0 UI         (502) staff       (20)      664 2023-12-04 13:15:18.000000 kytest-0.0.9/demo/tests/test_image.py
+-rw-r--r--   0 UI         (502) staff       (20)      620 2023-12-04 13:14:52.000000 kytest-0.0.9/demo/tests/test_ios.py
+-rw-r--r--   0 UI         (502) staff       (20)     1033 2023-12-04 13:15:18.000000 kytest-0.0.9/demo/tests/test_web.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.277772 kytest-0.0.9/kytest/
+-rw-r--r--   0 UI         (502) staff       (20)      521 2023-12-11 12:26:00.000000 kytest-0.0.9/kytest/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     3700 2023-11-22 09:29:35.000000 kytest-0.0.9/kytest/case.py
+-rw-r--r--   0 UI         (502) staff       (20)      491 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/cli.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.281278 kytest-0.0.9/kytest/core/
+-rw-r--r--   0 UI         (502) staff       (20)       51 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/__init__.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.283654 kytest-0.0.9/kytest/core/android/
+-rw-r--r--   0 UI         (502) staff       (20)      134 2023-11-22 01:37:15.000000 kytest-0.0.9/kytest/core/android/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     7149 2023-12-06 05:50:28.000000 kytest-0.0.9/kytest/core/android/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     9044 2023-12-07 09:29:06.000000 kytest-0.0.9/kytest/core/android/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.285122 kytest-0.0.9/kytest/core/api/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/api/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    12317 2023-12-11 12:25:33.000000 kytest-0.0.9/kytest/core/api/request.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.287518 kytest-0.0.9/kytest/core/image/
+-rw-r--r--   0 UI         (502) staff       (20)       53 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/image/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     1692 2023-11-22 02:05:24.000000 kytest-0.0.9/kytest/core/image/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     3100 2023-11-22 02:08:29.000000 kytest-0.0.9/kytest/core/image/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.290499 kytest-0.0.9/kytest/core/ios/
+-rw-r--r--   0 UI         (502) staff       (20)      134 2023-11-22 01:37:52.000000 kytest-0.0.9/kytest/core/ios/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     6582 2023-12-06 05:52:08.000000 kytest-0.0.9/kytest/core/ios/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)    11574 2023-12-05 07:23:56.000000 kytest-0.0.9/kytest/core/ios/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.293326 kytest-0.0.9/kytest/core/ocr/
+-rw-r--r--   0 UI         (502) staff       (20)       85 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/ocr/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      746 2023-11-22 02:07:34.000000 kytest-0.0.9/kytest/core/ocr/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     4222 2023-11-22 02:09:35.000000 kytest-0.0.9/kytest/core/ocr/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.295760 kytest-0.0.9/kytest/core/web/
+-rw-r--r--   0 UI         (502) staff       (20)       95 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/web/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     2745 2023-11-22 01:58:00.000000 kytest-0.0.9/kytest/core/web/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)    10636 2023-11-22 02:04:39.000000 kytest-0.0.9/kytest/core/web/element.py
+-rw-r--r--   0 UI         (502) staff       (20)      772 2023-12-11 06:53:03.000000 kytest-0.0.9/kytest/page.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.297815 kytest-0.0.9/kytest/running/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/running/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      182 2023-12-05 07:51:08.000000 kytest-0.0.9/kytest/running/conf.yml
+-rw-r--r--   0 UI         (502) staff       (20)     3809 2023-12-04 13:14:48.000000 kytest-0.0.9/kytest/running/runner.py
+-rw-r--r--   0 UI         (502) staff       (20)     2667 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/scaffold.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.299279 kytest-0.0.9/kytest/testdata/
+-rw-r--r--   0 UI         (502) staff       (20)    10650 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/testdata/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    18623 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/testdata/data.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.310844 kytest-0.0.9/kytest/utils/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     6789 2023-11-22 02:40:54.000000 kytest-0.0.9/kytest/utils/allure_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     8036 2023-11-22 02:43:09.000000 kytest-0.0.9/kytest/utils/common.py
+-rw-r--r--   0 UI         (502) staff       (20)     3445 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/config.py
+-rw-r--r--   0 UI         (502) staff       (20)     1396 2023-11-22 02:43:46.000000 kytest-0.0.9/kytest/utils/des_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     3277 2023-11-22 02:43:56.000000 kytest-0.0.9/kytest/utils/dingtalk.py
+-rw-r--r--   0 UI         (502) staff       (20)     3787 2023-11-22 02:44:11.000000 kytest-0.0.9/kytest/utils/excel.py
+-rw-r--r--   0 UI         (502) staff       (20)      159 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/exceptions.py
+-rw-r--r--   0 UI         (502) staff       (20)      710 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/log.py
+-rw-r--r--   0 UI         (502) staff       (20)     3930 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/mail.py
+-rw-r--r--   0 UI         (502) staff       (20)     2179 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/mysql_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     2402 2023-11-22 02:45:31.000000 kytest-0.0.9/kytest/utils/pytest_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     4022 2023-11-22 02:45:53.000000 kytest-0.0.9/kytest/utils/swagger_util.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.280804 kytest-0.0.9/kytest.egg-info/
+-rw-r--r--   0 UI         (502) staff       (20)      310 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/PKG-INFO
+-rw-r--r--   0 UI         (502) staff       (20)     1521 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/SOURCES.txt
+-rw-r--r--   0 UI         (502) staff       (20)        1 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/dependency_links.txt
+-rw-r--r--   0 UI         (502) staff       (20)       43 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/entry_points.txt
+-rw-r--r--   0 UI         (502) staff       (20)      301 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/requires.txt
+-rw-r--r--   0 UI         (502) staff       (20)       12 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/top_level.txt
+-rw-r--r--   0 UI         (502) staff       (20)       38 2023-12-11 12:26:11.312297 kytest-0.0.9/setup.cfg
+-rw-r--r--   0 UI         (502) staff       (20)     1363 2023-11-17 09:53:12.000000 kytest-0.0.9/setup.py
```

### Comparing `kytest-0.0.8/README.md` & `kytest-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/demo/pages/web_page.py` & `kytest-0.0.9/demo/pages/web_page.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/demo/tests/test_adr.py` & `kytest-0.0.9/demo/tests/test_adr.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/demo/tests/test_api.py` & `kytest-0.0.9/demo/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/demo/tests/test_image.py` & `kytest-0.0.9/demo/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/demo/tests/test_ios.py` & `kytest-0.0.9/demo/tests/test_ios.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/demo/tests/test_web.py` & `kytest-0.0.9/demo/tests/test_web.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/__init__.py` & `kytest-0.0.9/kytest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 from .utils.config import config
 from .utils.pytest_util import *
 from .utils.allure_util import *
 from .utils.log import logger
 from .utils.exceptions import KError
 
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __description__ = "API/安卓/IOS/WEB平台自动化测试框架"
```

### Comparing `kytest-0.0.8/kytest/case.py` & `kytest-0.0.9/kytest/case.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/android/driver.py` & `kytest-0.0.9/kytest/core/android/driver.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/android/element.py` & `kytest-0.0.9/kytest/core/android/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         text = []
         for elem in elems:
             text.append(elem.get_text())
         logger.info(text)
         return text
 
     def exists(self, timeout=5):
-        logger.info(f"检查空间是否存在")
+        logger.info(f"检查控件是否存在")
         if self._image is not None:
             return ImgElem(self._driver,
                            file=self._image,
                            grade=self._grade,
                            _debug=self._debug).exists(timeout=timeout)
         elif self._ocr is not None:
             return OcrElem(self._driver,
```

### Comparing `kytest-0.0.8/kytest/core/api/request.py` & `kytest-0.0.9/kytest/core/api/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,16 @@
                     logger.debug(f"[type]: {content_type}")
                     logger.debug(f"[response]:\n {r.text}")
                     ResponseResult.response = r.text
             else:
                 logger.debug('ContentType为空，响应异常！！！')
                 ResponseResult.response = r.text
 
+        return r
+
     return wrapper
 
 
 class ResponseResult:
     # 并发执行不会串数据，是因为我用的是多进程而不是多线程吧???
     status_code = 200
     response = None
```

### Comparing `kytest-0.0.8/kytest/core/image/driver.py` & `kytest-0.0.9/kytest/core/image/driver.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/image/element.py` & `kytest-0.0.9/kytest/core/image/element.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/ios/driver.py` & `kytest-0.0.9/kytest/core/ios/driver.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/ios/element.py` & `kytest-0.0.9/kytest/core/ios/element.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/ocr/driver.py` & `kytest-0.0.9/kytest/core/ocr/driver.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/ocr/element.py` & `kytest-0.0.9/kytest/core/ocr/element.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/web/driver.py` & `kytest-0.0.9/kytest/core/web/driver.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/core/web/element.py` & `kytest-0.0.9/kytest/core/web/element.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/page.py` & `kytest-0.0.9/kytest/page.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 @Author: kang.yang
 @Date: 2023/9/20 11:21
 """
+from urllib import parse
 from kytest.utils.config import config
 from kytest.utils.exceptions import KError
-from urllib import parse
 
 
 class Page(object):
     """页面基类，用于pom模式封装"""
 
     def __init__(self, driver):
         self.driver = driver
@@ -23,14 +23,11 @@
         if not url.startswith('http'):
             host = config.get_common('base_url')
             if host is not None:
                 url = parse.urljoin(host, url)
             else:
                 raise KError('host不能为空')
 
-        if getattr(self.driver, 'open', None) is not None:
-            self.driver.open(url)
-        else:
-            raise KError('driver没有open_url方法')
+        self.driver.open(url)
```

### Comparing `kytest-0.0.8/kytest/running/runner.py` & `kytest-0.0.9/kytest/running/runner.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/scaffold.py` & `kytest-0.0.9/kytest/scaffold.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/testdata/__init__.py` & `kytest-0.0.9/kytest/testdata/__init__.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/testdata/data.py` & `kytest-0.0.9/kytest/testdata/data.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/allure_util.py` & `kytest-0.0.9/kytest/utils/allure_util.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/common.py` & `kytest-0.0.9/kytest/utils/common.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/config.py` & `kytest-0.0.9/kytest/utils/config.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/des_util.py` & `kytest-0.0.9/kytest/utils/des_util.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/dingtalk.py` & `kytest-0.0.9/kytest/utils/dingtalk.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/excel.py` & `kytest-0.0.9/kytest/utils/excel.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/log.py` & `kytest-0.0.9/kytest/utils/log.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/mail.py` & `kytest-0.0.9/kytest/utils/mail.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/mysql_util.py` & `kytest-0.0.9/kytest/utils/mysql_util.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/pytest_util.py` & `kytest-0.0.9/kytest/utils/pytest_util.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest/utils/swagger_util.py` & `kytest-0.0.9/kytest/utils/swagger_util.py`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/kytest.egg-info/SOURCES.txt` & `kytest-0.0.9/kytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kytest-0.0.8/setup.py` & `kytest-0.0.9/setup.py`

 * *Files identical despite different names*

