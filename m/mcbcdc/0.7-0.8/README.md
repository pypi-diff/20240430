# Comparing `tmp/mcbcdc-0.7.tar.gz` & `tmp/mcbcdc-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcbcdc-0.7.tar", last modified: Mon Nov 20 20:29:05 2023, max compression
+gzip compressed data, was "mcbcdc-0.8.tar", last modified: Tue Apr 30 07:31:01 2024, max compression
```

## Comparing `mcbcdc-0.7.tar` & `mcbcdc-0.8.tar`

### file list

```diff
@@ -1,29 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 20:29:05.467859 mcbcdc-0.7/
--rw-rw-rw-   0        0        0       42 2023-11-20 18:26:19.000000 mcbcdc-0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      145 2023-11-20 20:29:05.466857 mcbcdc-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-11-20 20:29:05.442618 mcbcdc-0.7/data/
--rw-rw-rw-   0        0        0    13233 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/daa.txt
--rw-rw-rw-   0        0        0     1781 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/daa1a.txt
--rw-rw-rw-   0        0        0     1651 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/daa1b.txt
--rw-rw-rw-   0        0        0     2303 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/daa2.txt
--rw-rw-rw-   0        0        0     2433 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/daa3.txt
--rw-rw-rw-   0        0        0     4808 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/daa4.txt
--rw-rw-rw-   0        0        0      776 2023-11-20 12:45:31.000000 mcbcdc-0.7/data/iot1.txt
--rw-rw-rw-   0        0        0     1907 2023-11-20 12:45:29.000000 mcbcdc-0.7/data/iot2.txt
--rw-rw-rw-   0        0        0     1136 2023-11-20 12:45:33.000000 mcbcdc-0.7/data/iot3.txt
--rw-rw-rw-   0        0        0     1454 2023-11-20 20:14:57.000000 mcbcdc-0.7/data/iot4.txt
--rw-rw-rw-   0        0        0     3914 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/ml.txt
--rw-rw-rw-   0        0        0      696 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/ml1.txt
--rw-rw-rw-   0        0        0      699 2023-11-20 20:19:16.000000 mcbcdc-0.7/data/ml2.txt
--rw-rw-rw-   0        0        0      956 2023-11-20 20:19:17.000000 mcbcdc-0.7/data/ml3.txt
--rw-rw-rw-   0        0        0     1401 2023-11-20 20:19:17.000000 mcbcdc-0.7/data/ml4.txt
-drwxrwxrwx   0        0        0        0 2023-11-20 20:29:05.262577 mcbcdc-0.7/file/
--rw-rw-rw-   0        0        0        0 2023-11-20 17:20:14.000000 mcbcdc-0.7/file/__init__.py
--rw-rw-rw-   0        0        0      324 2023-11-20 18:43:45.000000 mcbcdc-0.7/file/file2.py
-drwxrwxrwx   0        0        0        0 2023-11-20 20:29:05.464866 mcbcdc-0.7/mcbcdc.egg-info/
--rw-rw-rw-   0        0        0      145 2023-11-20 20:29:05.000000 mcbcdc-0.7/mcbcdc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-11-20 20:29:05.000000 mcbcdc-0.7/mcbcdc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 20:29:05.000000 mcbcdc-0.7/mcbcdc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-11-20 20:29:05.000000 mcbcdc-0.7/mcbcdc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-20 20:29:05.467859 mcbcdc-0.7/setup.cfg
--rw-rw-rw-   0        0        0      438 2023-11-20 20:27:34.000000 mcbcdc-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:31:01.671441 mcbcdc-0.8/
+-rw-rw-rw-   0        0        0       42 2023-11-20 18:26:19.000000 mcbcdc-0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      145 2024-04-30 07:31:01.668439 mcbcdc-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 07:31:01.627772 mcbcdc-0.8/data/
+-rw-rw-rw-   0        0        0    13233 2023-11-20 20:19:16.000000 mcbcdc-0.8/data/daa.txt
+-rw-rw-rw-   0        0        0     1405 2024-04-30 07:01:43.000000 mcbcdc-0.8/data/ddos.txt
+-rw-rw-rw-   0        0        0     1882 2024-04-30 07:01:49.000000 mcbcdc-0.8/data/dns.txt
+-rw-rw-rw-   0        0        0      349 2024-04-30 07:01:24.000000 mcbcdc-0.8/data/ip_spoofing.txt
+-rw-rw-rw-   0        0        0      113 2024-04-30 07:01:55.000000 mcbcdc-0.8/data/sniffer_A.txt
+-rw-rw-rw-   0        0        0      645 2024-04-30 07:02:04.000000 mcbcdc-0.8/data/sniffer_B.txt
+-rw-rw-rw-   0        0        0     1952 2024-04-30 07:01:37.000000 mcbcdc-0.8/data/spam_mail.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 07:31:01.363556 mcbcdc-0.8/file/
+-rw-rw-rw-   0        0        0        0 2023-11-20 17:20:14.000000 mcbcdc-0.8/file/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-11-20 18:43:45.000000 mcbcdc-0.8/file/file2.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:31:01.663445 mcbcdc-0.8/mcbcdc.egg-info/
+-rw-rw-rw-   0        0        0      145 2024-04-30 07:31:01.000000 mcbcdc-0.8/mcbcdc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2024-04-30 07:31:01.000000 mcbcdc-0.8/mcbcdc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 07:31:01.000000 mcbcdc-0.8/mcbcdc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-30 07:31:01.000000 mcbcdc-0.8/mcbcdc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 07:31:01.672438 mcbcdc-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      438 2024-04-30 06:59:46.000000 mcbcdc-0.8/setup.py
```

### Comparing `mcbcdc-0.7/data/daa.txt` & `mcbcdc-0.8/data/daa.txt`

 * *Files identical despite different names*

