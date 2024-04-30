# Comparing `tmp/excel2db-0.0.1.tar.gz` & `tmp/excel2db-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\excel2db-0.0.1.tar", last modified: Wed Apr 24 14:22:30 2024, max compression
+gzip compressed data, was "dist\excel2db-0.0.2.tar", last modified: Tue Apr 30 02:23:11 2024, max compression
```

## Comparing `excel2db-0.0.1.tar` & `excel2db-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:22:30.000000 excel2db-0.0.1/
--rw-rw-rw-   0        0        0      171 2024-04-24 14:22:30.000000 excel2db-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 14:22:30.000000 excel2db-0.0.1/excel2db/
--rw-rw-rw-   0        0        0        0 2024-04-24 13:59:30.000000 excel2db-0.0.1/excel2db/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-24 13:59:52.000000 excel2db-0.0.1/excel2db/excel2db.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:22:30.000000 excel2db-0.0.1/excel2db.egg-info/
--rw-rw-rw-   0        0        0      171 2024-04-24 14:22:30.000000 excel2db-0.0.1/excel2db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-04-24 14:22:30.000000 excel2db-0.0.1/excel2db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:22:30.000000 excel2db-0.0.1/excel2db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 14:22:30.000000 excel2db-0.0.1/excel2db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 14:22:30.000000 excel2db-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-04-24 14:07:51.000000 excel2db-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/
+-rw-rw-rw-   0        0        0      171 2024-04-30 02:23:11.000000 excel2db-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/
+-rw-rw-rw-   0        0        0        0 2024-04-24 13:59:30.000000 excel2db-0.0.2/excel2db/__init__.py
+-rw-rw-rw-   0        0        0    19636 2024-04-25 02:26:33.000000 excel2db-0.0.2/excel2db/cheakConf.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/com/
+-rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.2/excel2db/com/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/com/util/
+-rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.2/excel2db/com/util/__init__.py
+-rw-rw-rw-   0        0        0     8036 2023-06-28 01:48:10.000000 excel2db-0.0.2/excel2db/com/util/coordinate.py
+-rw-rw-rw-   0        0        0     1637 2024-04-25 02:08:40.000000 excel2db-0.0.2/excel2db/com/util/dbconnect.py
+-rw-rw-rw-   0        0        0     6194 2023-10-17 13:38:33.000000 excel2db-0.0.2/excel2db/com/util/fileTool.py
+-rw-rw-rw-   0        0        0     8842 2024-04-25 02:39:56.000000 excel2db-0.0.2/excel2db/com/util/timeTool.py
+-rw-rw-rw-   0        0        0     5072 2024-04-29 09:11:27.000000 excel2db-0.0.2/excel2db/defaultConf.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/
+-rw-rw-rw-   0        0        0        0 2024-04-25 03:02:41.000000 excel2db-0.0.2/excel2db/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/demo1/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo1/__init__.py
+-rw-rw-rw-   0        0        0      173 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo1/demo1.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/demo2/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo2/__init__.py
+-rw-rw-rw-   0        0        0      190 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo2/demo2.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/demo3/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo3/__init__.py
+-rw-rw-rw-   0        0        0      190 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo3/demo3.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/demo4/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo4/__init__.py
+-rw-rw-rw-   0        0        0      175 2024-04-30 02:21:22.000000 excel2db-0.0.2/excel2db/demo/demo4/demo4.py
+-rw-rw-rw-   0        0        0     3807 2024-04-30 02:21:22.000000 excel2db-0.0.2/excel2db/demo/generalDemoFile.py
+-rw-rw-rw-   0        0        0     2629 2024-04-25 02:28:07.000000 excel2db-0.0.2/excel2db/detailData.py
+-rw-rw-rw-   0        0        0     2636 2024-04-25 02:28:07.000000 excel2db-0.0.2/excel2db/detailTitle.py
+-rw-rw-rw-   0        0        0     2534 2024-04-25 02:37:46.000000 excel2db-0.0.2/excel2db/excel.py
+-rw-rw-rw-   0        0        0      719 2024-04-25 02:26:33.000000 excel2db-0.0.2/excel2db/excel2db.py
+-rw-rw-rw-   0        0        0     2058 2024-04-25 02:37:46.000000 excel2db-0.0.2/excel2db/extraFuction.py
+-rw-rw-rw-   0        0        0     5897 2024-04-30 02:03:04.000000 excel2db-0.0.2/excel2db/insert2sqlite.py
+-rw-rw-rw-   0        0        0     3063 2024-04-25 02:42:06.000000 excel2db-0.0.2/excel2db/mainData.py
+-rw-rw-rw-   0        0        0     3411 2024-04-25 02:42:06.000000 excel2db-0.0.2/excel2db/mainTitle.py
+-rw-rw-rw-   0        0        0     6949 2024-04-25 02:42:06.000000 excel2db-0.0.2/excel2db/scale.py
+-rw-rw-rw-   0        0        0     5200 2024-04-25 02:42:06.000000 excel2db-0.0.2/excel2db/sheet.py
+-rw-rw-rw-   0        0        0     9711 2024-04-25 02:39:56.000000 excel2db-0.0.2/excel2db/value.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/
+-rw-rw-rw-   0        0        0      171 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 02:23:11.000000 excel2db-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-04-30 02:23:10.000000 excel2db-0.0.2/setup.py
```

