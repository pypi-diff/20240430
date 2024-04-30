# Comparing `tmp/aio_dt_protocol-1.4.2.tar.gz` & `tmp/aio_dt_protocol-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_dt_protocol-1.4.2.tar", last modified: Mon Mar 11 11:50:41 2024, max compression
+gzip compressed data, was "aio_dt_protocol-1.4.4.tar", last modified: Tue Apr 30 11:23:21 2024, max compression
```

## Comparing `aio_dt_protocol-1.4.2.tar` & `aio_dt_protocol-1.4.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.607541 aio_dt_protocol-1.4.2/
--rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     8835 2024-03-11 11:50:41.607541 aio_dt_protocol-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     8056 2023-10-06 08:08:30.000000 aio_dt_protocol-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.532562 aio_dt_protocol-1.4.2/aio_dt_protocol/
--rw-rw-rw-   0        0        0      553 2024-03-11 11:46:43.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/__init__.py
--rw-rw-rw-   0        0        0    11387 2023-10-09 07:25:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/actions.py
--rw-rw-rw-   0        0        0    60831 2024-03-09 06:15:42.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/browser.py
--rw-rw-rw-   0        0        0    17769 2024-03-10 05:32:58.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/connection.py
--rw-rw-rw-   0        0        0    28328 2023-12-24 08:28:14.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/data.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.538560 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/
--rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.542558 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/background_service/
--rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/background_service/__init__.py
--rw-rw-rw-   0        0        0     3328 2023-12-30 06:55:05.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/background_service/background_service.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/background_service/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.545557 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/browser/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/browser/__init__.py
--rw-rw-rw-   0        0        0    14355 2023-11-05 07:36:13.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/browser/browser.py
--rw-rw-rw-   0        0        0     1350 2023-10-09 06:20:22.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/browser/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.548556 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/css/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/css/__init__.py
--rw-rw-rw-   0        0        0     6379 2023-11-05 07:37:03.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/css/css.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/css/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.552555 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/device_orientation/
--rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/device_orientation/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-11-05 07:37:03.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/device_orientation/device_orientation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/device_orientation/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.557553 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/dom/
--rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/dom/__init__.py
--rw-rw-rw-   0        0        0    16534 2023-11-05 07:37:03.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/dom/dom.py
--rw-rw-rw-   0        0        0    35467 2024-03-09 08:56:59.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/dom/dom_element.py
--rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/dom/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.560552 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/emulation/
--rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/emulation/__init__.py
--rw-rw-rw-   0        0        0    25007 2023-11-05 07:39:07.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/emulation/emulation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/emulation/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.564550 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/fetch/
--rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/fetch/__init__.py
--rw-rw-rw-   0        0        0    16985 2023-11-30 12:58:34.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/fetch/fetch.py
--rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/fetch/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.567549 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/input/
--rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/input/__init__.py
--rw-rw-rw-   0        0        0    23671 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/input/input.py
--rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/input/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.570549 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/log/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/log/__init__.py
--rw-rw-rw-   0        0        0     1748 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/log/log.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/log/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.574547 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/network/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/network/__init__.py
--rw-rw-rw-   0        0        0    18967 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/network/network.py
--rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/network/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.577546 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/overlay/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/overlay/__init__.py
--rw-rw-rw-   0        0        0     1778 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/overlay/overlay.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/overlay/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.580545 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/page/
--rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/page/__init__.py
--rw-rw-rw-   0        0        0    32638 2024-03-09 06:36:07.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/page/page.py
--rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/page/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.583543 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/runtime/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/runtime/__init__.py
--rw-rw-rw-   0        0        0    33716 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/runtime/runtime.py
--rw-rw-rw-   0        0        0     8113 2024-03-11 08:25:30.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/runtime/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.587542 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/system_info/
--rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/system_info/__init__.py
--rw-rw-rw-   0        0        0     1368 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/system_info/system_info.py
--rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/system_info/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.605542 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/target/
--rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/target/__init__.py
--rw-rw-rw-   0        0        0    16858 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/target/target.py
--rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/domains/target/types.py
--rw-rw-rw-   0        0        0     4780 2024-03-11 11:43:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/exceptions.py
--rw-rw-rw-   0        0        0     9805 2024-03-11 11:02:28.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/extend_connection.py
--rw-rw-rw-   0        0        0    12324 2023-07-09 14:14:30.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/js.py
--rw-rw-rw-   0        0        0     7576 2024-03-06 14:21:02.000000 aio_dt_protocol-1.4.2/aio_dt_protocol/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:50:41.537560 aio_dt_protocol-1.4.2/aio_dt_protocol.egg-info/
--rw-rw-rw-   0        0        0     8835 2024-03-11 11:50:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2526 2024-03-11 11:50:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 11:50:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-03-11 11:50:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-11 11:50:41.000000 aio_dt_protocol-1.4.2/aio_dt_protocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-11 11:50:41.609541 aio_dt_protocol-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-10-06 07:21:41.000000 aio_dt_protocol-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:21.046549 aio_dt_protocol-1.4.4/
+-rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0     8835 2024-04-30 11:23:21.045549 aio_dt_protocol-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8056 2023-10-06 08:08:30.000000 aio_dt_protocol-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.784154 aio_dt_protocol-1.4.4/aio_dt_protocol/
+-rw-rw-rw-   0        0        0      553 2024-04-30 11:17:02.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/__init__.py
+-rw-rw-rw-   0        0        0    11387 2023-10-09 07:25:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/actions.py
+-rw-rw-rw-   0        0        0    62338 2024-04-28 04:53:51.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/browser.py
+-rw-rw-rw-   0        0        0    17753 2024-03-20 10:36:36.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/connection.py
+-rw-rw-rw-   0        0        0    28828 2024-03-20 10:33:45.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/data.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.806371 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/
+-rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.822049 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/background_service/
+-rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/background_service/__init__.py
+-rw-rw-rw-   0        0        0     3328 2023-12-30 06:55:05.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/background_service/background_service.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/background_service/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.829047 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/browser/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/browser/__init__.py
+-rw-rw-rw-   0        0        0    14336 2024-04-30 05:16:50.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/browser/browser.py
+-rw-rw-rw-   0        0        0     1350 2023-10-09 06:20:22.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/browser/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.844042 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/css/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/css/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-11-05 07:37:03.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/css/css.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/css/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.851039 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/device_orientation/
+-rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/device_orientation/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-11-05 07:37:03.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/device_orientation/device_orientation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/device_orientation/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.886027 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/dom/
+-rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/dom/__init__.py
+-rw-rw-rw-   0        0        0    16534 2023-11-05 07:37:03.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/dom/dom.py
+-rw-rw-rw-   0        0        0    35467 2024-03-09 08:56:59.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/dom/dom_element.py
+-rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/dom/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.893509 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/emulation/
+-rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/emulation/__init__.py
+-rw-rw-rw-   0        0        0    25007 2023-11-05 07:39:07.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/emulation/emulation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/emulation/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.908505 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/fetch/
+-rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/fetch/__init__.py
+-rw-rw-rw-   0        0        0    16985 2023-11-30 12:58:34.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/fetch/fetch.py
+-rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/fetch/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.941051 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/input/
+-rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/input/__init__.py
+-rw-rw-rw-   0        0        0    23671 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/input/input.py
+-rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/input/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.969594 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/log/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/log/__init__.py
+-rw-rw-rw-   0        0        0     1748 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/log/log.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/log/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.976587 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/network/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/network/__init__.py
+-rw-rw-rw-   0        0        0    18967 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/network/network.py
+-rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/network/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.996095 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/overlay/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/overlay/__init__.py
+-rw-rw-rw-   0        0        0     1778 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/overlay/overlay.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/overlay/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:21.003118 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/page/
+-rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/page/__init__.py
+-rw-rw-rw-   0        0        0    32638 2024-03-09 06:36:07.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/page/page.py
+-rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/page/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:21.012622 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/runtime/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/runtime/__init__.py
+-rw-rw-rw-   0        0        0    33716 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/runtime/runtime.py
+-rw-rw-rw-   0        0        0     8113 2024-03-11 08:25:30.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/runtime/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:21.018560 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/system_info/
+-rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/system_info/__init__.py
+-rw-rw-rw-   0        0        0     1368 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/system_info/system_info.py
+-rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/system_info/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:21.044550 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/target/
+-rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/target/__init__.py
+-rw-rw-rw-   0        0        0    16858 2023-11-05 07:43:01.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/target/target.py
+-rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/domains/target/types.py
+-rw-rw-rw-   0        0        0     4780 2024-03-11 11:43:41.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/exceptions.py
+-rw-rw-rw-   0        0        0     9809 2024-04-30 11:09:17.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/extend_connection.py
+-rw-rw-rw-   0        0        0    12324 2023-07-09 14:14:30.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/js.py
+-rw-rw-rw-   0        0        0     7576 2024-03-06 14:21:02.000000 aio_dt_protocol-1.4.4/aio_dt_protocol/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:23:20.804371 aio_dt_protocol-1.4.4/aio_dt_protocol.egg-info/
+-rw-rw-rw-   0        0        0     8835 2024-04-30 11:23:20.000000 aio_dt_protocol-1.4.4/aio_dt_protocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2526 2024-04-30 11:23:20.000000 aio_dt_protocol-1.4.4/aio_dt_protocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 11:23:20.000000 aio_dt_protocol-1.4.4/aio_dt_protocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-30 11:23:20.000000 aio_dt_protocol-1.4.4/aio_dt_protocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-30 11:23:20.000000 aio_dt_protocol-1.4.4/aio_dt_protocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 11:23:21.047549 aio_dt_protocol-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-10-06 07:21:41.000000 aio_dt_protocol-1.4.4/setup.py
```

### Comparing `aio_dt_protocol-1.4.2/LICENSE` & `aio_dt_protocol-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/PKG-INFO` & `aio_dt_protocol-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio_dt_protocol
-Version: 1.4.2
+Version: 1.4.4
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aio_dt_protocol-1.4.2/README.md` & `aio_dt_protocol-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/__init__.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = "1.4.2"
+__version__ = "1.4.4"
 __author__ = "PieceOfGood"
 __email__ = "78sanchezz@gmail.com"
 
 __all__ = [
     "find_instances",
     "CMDFlags",
     "FlagBuilder",
```

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/actions.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/actions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/browser.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
                 debug_port=debug_port,
                 browser_exe=browser_name,
                 **options
             )
 
         return browser, await browser.waitFirstTab(callback=callback)
 
-
     def __init__(
             self, *,
             profile_path: str = "testProfile",
             profile_name: str = "Default",
             dev_tool_profiles:  bool = False,
             url: Optional[Union[str, bytes]] = None,
             flags:  Optional["FlagBuilder"] = None,
@@ -175,21 +174,24 @@
                     # ? НЕ нормальный
                     if exit_type.group(1) != "Normal":
                         result = re.sub(
                             r'"exit_type":"\w+"',
                             '"exit_type":"Normal"',
                             preferences
                         )
-                        with open(preferences_path, "w") as f: f.write(result)
+                        with open(preferences_path, "w") as f:
+                            f.write(result)
                 # ? Только для чтения
                 # os.chmod(preferences_path, READ_ONLY)
-                if verbose: log("Файл настроек — изменён и сохранён")
+                if verbose:
+                    log("Файл настроек — изменён и сохранён")
             else:
                 # os.chmod(preferences_path, READ_WRITE)
-                if verbose: log("Файл настроек — только для чтения")
+                if verbose:
+                    log("Файл настроек — только для чтения")
 
         if "chrome" in browser_exe:
             self.browser_name = "chrome"
             browser_exe = "chrome" if sys.platform == "win32" else "google-chrome"
         elif "brave" in browser_exe:
             self.browser_name = "brave"
             browser_exe = "brave" if sys.platform == "win32" else "brave-browser"
@@ -217,15 +219,15 @@
             self.is_connected = True
             if verbose:
                 log(f"Connected to {self.debug_port} port | Headless mod: {self.is_headless_mode}")
             return
 
         if sys.platform == "win32":
             browser_path = browser_path if browser_path else find_browser_executable_path(browser_exe)
-        else:   #  ! sys.platform == "linux"
+        else:   # ! sys.platform == "linux"
             browser_path = browser_path if browser_path else os.popen("which " + browser_exe).read().strip()
 
         if not os.path.exists(browser_path) or not os.path.isfile(browser_path):
             raise FileNotFoundError(f"Путь до исполняемого файла '{browser_path}' "
                                     "— не существует, или содержит ошибку")
         self.browser_path = browser_path
 
@@ -293,16 +295,16 @@
         # ! Headless mode
         else:
             flag_box.add(CMDFlags.Headless.headless)
 
         if self.proxy_port:
             flag_box.add(CMDFlags.Other.proxy_server, self.proxy_address + ":" + self.proxy_port)
             if self.verbose:
-                log(f"Run browser {self.browser_name!r} on port: {self.debug_port} with proxy " +
-                      f"on http://127.0.0.1:{self.proxy_port}")
+                log(f"Run browser {self.browser_name!r} on port: {self.debug_port} "
+                    f"with proxy on http://127.0.0.1:{self.proxy_port}")
         else:
             if self.verbose:
                 log(f"Run browser {self.browser_name!r} on port: {self.debug_port}")
 
         if flags is not None:
             flag_box += flags
 
@@ -324,15 +326,15 @@
         """
         target_id = target.id if isinstance(target, TargetConnectionInfo) else target
         result = await async_util_call(
             make_request,
             f"http://127.0.0.1:{self.debug_port}/"
             f"json/activate/{target_id}"
         )
-        return result # "Target activated" if success
+        return result   # "Target activated" if success
 
     async def getAllTargetsConnectionInfo(self) -> List[TargetConnectionInfo]:
         """ Возвращает список описаний соединений со всеми
         существующими типами соединений.
         """
         return [TargetConnectionInfo(**i) for i in await self.getConnectionList()]
 
@@ -379,26 +381,27 @@
                     "url": "https://www.yahoo.com/",
                     "webSocketDebuggerUrl": "ws://localhost:9222/devtools/page/DAB7FB6187B554E10B0BD18821265734"
                 }, { ... } ]
         """
         result = await async_util_call(
             make_request, f"http://127.0.0.1:{self.debug_port}/json/list")
 
-        if self.verbose: log("getPageList() => " + result)
+        if self.verbose:
+            log("getPageList() => " + result)
         return Serializer.decode(result)
 
     async def queryNewTab(self, url: str = "about:blank") -> Connection:
         result: str = await async_util_call(
             make_request, f"http://127.0.0.1:{self.debug_port}/json/new?{url}", "PUT")
 
-        if self.verbose: log("queryNewTab() => " + result)
+        if self.verbose:
+            log("queryNewTab() => " + result)
         result: dict = Serializer.decode(result)
         return await self.getConnectionByID(result["id"])
 
-
     async def getConnectionBy(
             self, key: Union[str, int],
             value: Union[str, int],
             match_mode: Literal["exact", "contains", "startswith"] = "exact",
             index: int = 0,
             callback: Optional[CommonCallback] = None) -> Optional[Connection]:
         """
@@ -420,19 +423,19 @@
 
         :return:        <Connection>
         """
 
         if callback is not None and not iscoroutinefunction(callback):
             raise TypeError("Argument 'callback' must be a coroutine")
 
-        counter = 0; v = value.lower()
+        counter, v = 0, value.lower()
         for page_data in await self.getConnectionList():
             data: str = page_data[key].lower()
             if ((match_mode == "exact" and data == v)
-                or (match_mode == "contains" and data.find(v) > -1 )
+                or (match_mode == "contains" and data.find(v) > -1)
                     or (match_mode == "startswith" and data.startswith(v))):
                 if counter == index:
                     conn = Connection(
                         page_data["webSocketDebuggerUrl"],
                         page_data["id"],
                         page_data["devtoolsFrontendUrl"],
                         callback,
@@ -520,14 +523,17 @@
             callback: Optional[CommonCallback] = None) -> Optional[Connection]:
         """
         Создаёт новую вкладку в браузере, используя для этого существующие
         подключения.
         :param url:                     - (optional) Адрес будет открыт при создании.
         :param newWindow:               - (optional) Если 'True' — страница будет открыта в новом окне.
         :param background:              - (optional) Если 'True' — страница будет открыта в фоне.
+        :param wait_for_create:         - (optional) Если 'True' — ожидает окончания создания страницы.
+        :param callback:                - (optional) Корутина, которой будет передаваться контекст абсолютно
+                                            всех событий страницы в виде словаря.
         :return:                    * <Connection>
         """
         while not (tmp := await self.getConnection(callback=callback)):
             await asyncio.sleep(.5)
         page_id = await tmp.Target.createTarget(url, newWindow=newWindow, background=background)
         if wait_for_create:
             while not (page := await self.getConnectionByID(page_id)):
@@ -556,53 +562,61 @@
             self, conn: Connection,
             new_window: bool = True,
             callback: Optional[CommonCallback] = None) -> Optional[Connection]:
         """
         Открывает новую вкладку с дебаггером для инспектируемой страницы.
         :param conn:            - Инспектируемая страница. Может принадлежать любому браузеру.
         :param new_window:      - Создать target в отдельном окне?
+        :param callback:        - Корутина, которой будет передаваться контекст абсолютно
+                                    всех событий страницы в виде словаря.
         :return:        <Connection>
         """
         return await self.createTab(
             "http://127.0.0.1:" + str(self.debug_port) + conn.frontend_url, new_window, callback=callback
         )
 
     async def createPopupWindow(
             self, conn: Connection,
             url: str = "about:blank",
             callback: Optional[CommonCallback] = None) -> Optional[Connection]:
         """ Создаёт всплывающее окно с минимумом интерфейса браузера".
-        :param url:             - Адрес, ресурс которого будет загружен
-        :param conn:            - Родительская страница, инициатор
+        :param url:             - Адрес, ресурс которого будет загружен.
+        :param conn:            - Родительская страница, инициатор.
+        :param callback:        - Корутина, которой будет передаваться контекст абсолютно
+                                    всех событий страницы в виде словаря.
         :return:        Connection or None
         """
         await conn.extend.injectJS(
             f'window.open("{url}", "blank_window_name", "popup,noopener,noreferrer");')
         return await self.getConnectionByOpener(conn, callback=callback)
 
     async def getConnectionByOpener(
             self, conn: Connection,
             callback: Optional[CommonCallback] = None) -> Optional[Connection]:
         """ Возвращает последнее созданное соединение со страницей, открытие которого
         инициировано с конкретной страницы. Например, при использовании JavaScript
         "window.open()".
         :param conn:            - Родительская страница, инициатор
+        :param callback:        - Корутина, которой будет передаваться контекст абсолютно
+                                    всех событий страницы в виде словаря.
         :return:        Connection or None
         """
         for target_info in await conn.Target.getTargets():
             if target_info.openerId == conn.conn_id:
                 return await self.getConnectionByID(target_info.targetId, callback=callback)
         return None
 
     async def getConnectionsByOpener(
             self, conn: Connection,
             callback: Optional[CommonCallback] = None) -> List[Connection]:
         """ Возвращает список всех соединений, открытие которых инициировано с конкретной
         страницы. Например, при использовании JavaScript "window.open()".
         :param conn:            - Родительская страница, инициатор открытых окон
+        :param callback:        - Корутина, которой будет передаваться контекст абсолютно
+                                    всех событий страницы в виде словаря.
         :return:        List[Connection]
         """
         connections = []
         for target_info in await conn.Target.getTargets():
             if target_info.openerId == conn.conn_id:
                 connections.append(await self.getConnectionByID(
                     target_info.targetId, callback=callback))
@@ -621,15 +635,16 @@
         Безусловно дожидается соединения со страницей.
         """
         while True:
             try:
                 while (conn := await self.getConnection(callback=callback)) is None:
                     await asyncio.sleep(.5)
                 return conn
-            except URLError: await asyncio.sleep(1)
+            except URLError:
+                await asyncio.sleep(1)
 
     async def close(self) -> None:
         """ Корректно закрывает браузер если остались ещё его инстансы """
         if conn := await self.getConnection():
             await conn.Browser.close()
 
     async def closeTarget(self, target: Union[TargetConnectionInfo, str]) -> str:
@@ -739,14 +754,15 @@
         result = FlagBuilder()
         setattr(result, "_flags", flags)
         return result
 
 
 class CMDFlag(Enum): pass
 
+
 class CMDFlags:
     """https://github.com/GoogleChrome/chrome-launcher/blob/master/docs/chrome-flags-for-tools.md"""
 
     class Common(CMDFlag):
         # ? Commonly unwanted browser features
         # ! Порт подключения
         remote_debugging_port = "--remote-debugging-port="
@@ -921,16 +937,14 @@
         use_gl = "--use-gl="    # * $
         # + DARK_MODE -- требует двух следующих флагов
         # ! Включает тёмный режим в браузере.
         enable_features_WebUIDarkMode = "--enable-features=WebUIDarkMode"
         # ! Принуждает использовать темный режим в пользовательском интерфейсе для платформ, которые его поддерживают.
         force_dark_mode = "--force-dark-mode"
 
-
-
     class Screen(CMDFlag):
         # ? Window & screen management
         # ! Запускает браузер в режиме KIOSK
         kiosk = "--kiosk"
         # ! Запрещает браузеру resize и убирает некоторые его элементы.
         force_app_mode = "--force-app-mode"
         # ! Все всплывающие окна и вызовы window.open завершатся ошибкой.
@@ -939,15 +953,15 @@
         force_color_profile_SRGB = "--force-color-profile=srgb"
         # ! Переопределяет коэффициент масштабирования устройства для пользовательского интерфейса браузера и содержимого.
         # !     int or float
         force_device_scale_factor = "--force-device-scale-factor="
         # ! Каждая ссылка запускается в новом окне.
         new_window = '--new-window'
         # ! Принимает X и Y позицию верхнего левого угла, окна браузера.
-        window_position="--window-position="            # * $
+        window_position = "--window-position="            # * $
         # ! Принимает ширину и высоту окна браузера.
         window_size = "--window-size="                  # * $
 
     class Process(CMDFlag):
         # ? Process management
         # ! Отключает OOPIF. https://www.chromium.org/Home/chromium-security/site-isolation
         disable_features_site_per_process = "--disable-features=site-per-process"
```

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/connection.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import (
     Callable, Optional, Union, Tuple, Dict, Any, Iterable,
     Awaitable)
 
 from .exceptions import get_cdtp_error
 from .utils import log
 
-from .data import DomainEvent, Sender, Receiver, CommonCallback, Serializer
+from .data import DomainEvent, Sender, Channel, CommonCallback, Serializer
 from .extend_connection import Extend
 
 from .domains.background_service import BackgroundService
 from .domains.browser import Browser
 from .domains.css import CSS
 from .domains.device_orientation import DeviceOrientation
 from .domains.dom import DOM
@@ -26,14 +26,16 @@
 from .domains.page import Page
 from .domains.runtime import Runtime
 from .domains.system_info import SystemInfo
 from .domains.target import Target
 
 Handler = Callable[..., Awaitable[None]]
 
+REQUEST_CHANNEL = Channel[dict]()
+
 
 class Connection:
     """ Если инстанс страницы более не нужен, например, при перезаписи в него нового
     инстанса, перед этим [-!-] ОБЯЗАТЕЛЬНО [-!-] - вызовите у него метод
     Detach(), или закройте вкладку/страницу браузера, с которой он связан,
     тогда это будет выполнено автоматом. Иначе в цикле событий останутся
     задачи связанные с поддержанием соединения, которое более не востребовано.
@@ -155,16 +157,15 @@
         _id = self._id
         data = {
             "id": _id,
             "params": params if params else {},
             "method": domain_and_method
         }
 
-        que = asyncio.Queue()
-        sender, receiver = Sender[dict](que), Receiver[dict](que)
+        sender, receiver = REQUEST_CHANNEL()
         self.responses[_id] = sender
 
         await self._send(Serializer.encode(data))
 
         response = await receiver.recv()
         if "error" in response:
```

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/data.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,33 +105,40 @@
     country: str
     languages: list[str]
     city: str
     state_province: str
     proxy_type: Optional[str] = None
 
 
-class __Base(Generic[T]):
+class BaseQueue(Generic[T]):
     def __init__(self, que: Queue[T]) -> None:
         self.que = que
 
 
-class Sender(__Base[T]):
+class Sender(BaseQueue[T]):
     async def send(self, data: T) -> None:
         await self.que.put(data)
 
 
-class Receiver(__Base[T]):
+class Receiver(BaseQueue[T]):
     async def recv(self) -> T:
         return await self.que.get()
 
 
 class Channel(Generic[T]):
-    @classmethod
-    def one_way(cls) -> Tuple[Sender[T], Receiver[T]]:
-        que: Queue = Queue()
+    """ Channel[T] - создаёт инстанс однонаправленного
+    канала указанного типа, вызов которого всякий раз
+    создаёт новый канал и возвращает его отправителя
+    с получателем, ожидающих сообщения установленного
+    ранее типа. Например:
+        channel = Channel[int]()
+        sender, receiver = channel()
+    """
+    def __call__(self) -> Tuple[Sender[T], Receiver[T]]:
+        que: Queue[T] = Queue()
         return Sender[T](que), Receiver[T](que)
 
 
 class DomainEvent(Enum):
     pass
```

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/background_service/background_service.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/background_service/background_service.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/browser/browser.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/browser/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         """ Устанавливает позицию и/или размер окна.
         !(EXPERIMENTAL)
         https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-setWindowBounds
         :param bounds:          Новые границы окна, а так же состояние.
         :param windowId:        Идентификатор окна.
         """
         if windowId is None:
-            windowId = (await self._connection.Target.getWindowForTarget()).windowId
+            windowId = (await self.getWindowForTarget()).windowId
         await self._connection.call(
             "Browser.setWindowBounds",
             {"windowId": windowId, "bounds": bounds.to_dict()}
         )
 
     async def close(self) -> bool:
         """ Изящно завершает работу браузера.
```

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/browser/types.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/browser/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/css/css.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/css/css.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/device_orientation/device_orientation.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/device_orientation/device_orientation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/dom/dom.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/dom/dom.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/dom/dom_element.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/dom/dom_element.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/dom/types.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/dom/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/emulation/emulation.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/emulation/emulation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/fetch/fetch.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/fetch/types.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/fetch/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/input/input.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/input/input.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/input/types.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/input/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/log/log.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/log/log.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/network/network.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/network/network.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/network/types.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/network/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/overlay/overlay.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/page/page.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/page/page.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/page/types.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/page/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/runtime/runtime.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/runtime/types.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/runtime/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/system_info/system_info.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/system_info/system_info.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/system_info/types.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/system_info/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/domains/target/target.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/domains/target/target.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/exceptions.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/extend_connection.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/extend_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .actions import Actions
 from .data import ViewportRect, WindowRect, GeoInfo, Serializer
 
 import base64
 import re
-from typing import Optional, TYPE_CHECKING
+from typing import Optional, Any, TYPE_CHECKING
 
 from .exceptions import (
     PromiseEvaluateError,
     EvaluateError,
     JavaScriptError,
     JAVASCRIPT_EXCEPTIONS
 )
@@ -122,15 +122,15 @@
         """ Выполняет плавную прокрутку страницы до выбранного селектора. """
         await self.injectJS(
             "document.querySelector(`" +
             selector +
             "`).scrollIntoView({'behavior':'smooth', 'block': 'center'});"
         )
 
-    async def evalPromise(self, expression: str) -> dict:
+    async def evalPromise(self, expression: str) -> Any:
         """ Выполняет асинхронный код на странице и дожидается
         получения результата.
         """
         result = await self._connection.Runtime.evaluate(
             expression=expression,
             objectGroup="console",
             includeCommandLineAPI=True,
@@ -141,18 +141,17 @@
         )
 
         response = await self._connection.Runtime.awaitPromise(
             promiseObjectId=result.objectId,
             returnByValue=False,
             generatePreview=False
         )
+        return response.value
 
-        return Serializer.decode(response.value)
-
-    async def injectJS(self, expression: str) -> any:
+    async def injectJS(self, expression: str) -> Any:
         """ Выполняет JavaScript-выражение во фрейме верхнего уровня.
         Возвращает только простые типы в естественном виде, для сложных
         используйте сериализацию в JSON, или evaluate() домена Runtime.
         """
         try:
             response = await self._connection.Runtime.evaluate(
                 expression=expression,
@@ -183,30 +182,30 @@
             return await resp.text();
         } get_geo_info();
         """
 
         promise = """fetch('https://time.gologin.com/').then(res => res.text())"""
 
         try:
-            result: dict = await self._connection.extend.evalPromise(promise)
+            result: str = await self._connection.extend.evalPromise(promise)
         except PromiseEvaluateError:
             if "://newtab" in await self._connection.extend.getUrl():
                 raise RuntimeError("Doesn't work on the default browser page. Please "
                                    "first go to a blank url, or any other address.")
             raise
-
-        result.update(
+        data: dict = Serializer.decode(result)
+        data.update(
             geo=dict(
-                latitude=float(result["ll"][0]),
-                longitude=float(result["ll"][1]),
-                accuracy=float(result["accuracy"])
+                latitude=float(data["ll"][0]),
+                longitude=float(data["ll"][1]),
+                accuracy=float(data["accuracy"])
             ),
-            languages=result["languages"].split(","),
-            state_province=result.get("stateProv"),
-            proxy_type=(pt := result.get("proxyType"))
+            languages=data["languages"].split(","),
+            state_province=data.get("stateProv"),
+            proxy_type=(pt := data.get("proxyType"))
         )
-        del result["ll"]
-        del result["accuracy"]
-        del result["stateProv"]
+        del data["ll"]
+        del data["accuracy"]
+        del data["stateProv"]
         if pt is not None:
-            del result["proxyType"]
-        return GeoInfo(**result)
+            del data["proxyType"]
+        return GeoInfo(**data)
```

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/js.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/js.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol/utils.py` & `aio_dt_protocol-1.4.4/aio_dt_protocol/utils.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol.egg-info/PKG-INFO` & `aio_dt_protocol-1.4.4/aio_dt_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-dt-protocol
-Version: 1.4.2
+Version: 1.4.4
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aio_dt_protocol-1.4.2/aio_dt_protocol.egg-info/SOURCES.txt` & `aio_dt_protocol-1.4.4/aio_dt_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.4.2/setup.py` & `aio_dt_protocol-1.4.4/setup.py`

 * *Files identical despite different names*

