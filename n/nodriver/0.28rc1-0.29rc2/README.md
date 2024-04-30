# Comparing `tmp/nodriver-0.28rc1.tar.gz` & `tmp/nodriver-0.29rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodriver-0.28rc1.tar", last modified: Sat Apr 20 15:14:10 2024, max compression
+gzip compressed data, was "nodriver-0.29rc2.tar", last modified: Tue Apr 30 11:22:35 2024, max compression
```

## Comparing `nodriver-0.28rc1.tar` & `nodriver-0.29rc2.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.209216 nodriver-0.28rc1/
--rw-rw-rw-   0        0        0    32693 2024-01-18 14:05:42.000000 nodriver-0.28rc1/LICENSE.txt
--rw-rw-rw-   0        0        0      121 2024-02-25 19:31:30.000000 nodriver-0.28rc1/MANIFEST.in
--rw-rw-rw-   0        0        0    47611 2024-04-20 15:14:10.209216 nodriver-0.28rc1/PKG-INFO
--rw-rw-rw-   0        0        0     8430 2024-02-25 18:42:37.000000 nodriver-0.28rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.177217 nodriver-0.28rc1/nodriver/
--rw-rw-rw-   0        0        0      616 2024-03-10 03:03:41.000000 nodriver-0.28rc1/nodriver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.204216 nodriver-0.28rc1/nodriver/cdp/
--rw-rw-rw-   0        0        0      172 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/README.md
--rw-rw-rw-   0        0        0     1011 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/__init__.py
--rw-rw-rw-   0        0        0    25019 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/accessibility.py
--rw-rw-rw-   0        0        0    11919 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/animation.py
--rw-rw-rw-   0        0        0    65075 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/audits.py
--rw-rw-rw-   0        0        0     8168 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/autofill.py
--rw-rw-rw-   0        0        0     6359 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/background_service.py
--rw-rw-rw-   0        0        0    22888 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/browser.py
--rw-rw-rw-   0        0        0     9549 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/cache_storage.py
--rw-rw-rw-   0        0        0     4565 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/cast.py
--rw-rw-rw-   0        0        0     3004 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/console.py
--rw-rw-rw-   0        0        0    80456 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/css.py
--rw-rw-rw-   0        0        0     4358 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/database.py
--rw-rw-rw-   0        0        0    54782 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/debugger.py
--rw-rw-rw-   0        0        0     3497 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/device_access.py
--rw-rw-rw-   0        0        0     1187 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/device_orientation.py
--rw-rw-rw-   0        0        0    66246 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/dom.py
--rw-rw-rw-   0        0        0    10211 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/dom_debugger.py
--rw-rw-rw-   0        0        0    43435 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/dom_snapshot.py
--rw-rw-rw-   0        0        0     6124 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/dom_storage.py
--rw-rw-rw-   0        0        0    34831 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/emulation.py
--rw-rw-rw-   0        0        0     1501 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/event_breakpoints.py
--rw-rw-rw-   0        0        0     7347 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/fed_cm.py
--rw-rw-rw-   0        0        0    21611 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/fetch.py
--rw-rw-rw-   0        0        0     5219 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/headless_experimental.py
--rw-rw-rw-   0        0        0    14457 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/heap_profiler.py
--rw-rw-rw-   0        0        0    18362 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/indexed_db.py
--rw-rw-rw-   0        0        0    29314 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/input_.py
--rw-rw-rw-   0        0        0     1743 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/inspector.py
--rw-rw-rw-   0        0        0     3120 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/io.py
--rw-rw-rw-   0        0        0    16878 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/layer_tree.py
--rw-rw-rw-   0        0        0     6092 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/log.py
--rw-rw-rw-   0        0        0     8215 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/media.py
--rw-rw-rw-   0        0        0     7279 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/memory.py
--rw-rw-rw-   0        0        0   147161 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/network.py
--rw-rw-rw-   0        0        0    60483 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/overlay.py
--rw-rw-rw-   0        0        0   117573 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/page.py
--rw-rw-rw-   0        0        0     3203 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/performance.py
--rw-rw-rw-   0        0        0     7587 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/performance_timeline.py
--rw-rw-rw-   0        0        0    22524 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/preload.py
--rw-rw-rw-   0        0        0    14302 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/profiler.py
--rw-rw-rw-   0        0        0        0 2024-01-18 14:08:24.000000 nodriver-0.28rc1/nodriver/cdp/py.typed
--rw-rw-rw-   0        0        0    67631 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/runtime.py
--rw-rw-rw-   0        0        0     1196 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/schema.py
--rw-rw-rw-   0        0        0    18824 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/security.py
--rw-rw-rw-   0        0        0    12358 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/service_worker.py
--rw-rw-rw-   0        0        0    61377 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/storage.py
--rw-rw-rw-   0        0        0    12914 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/system_info.py
--rw-rw-rw-   0        0        0    25505 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/target.py
--rw-rw-rw-   0        0        0     1533 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/tethering.py
--rw-rw-rw-   0        0        0    14682 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/tracing.py
--rw-rw-rw-   0        0        0      470 2024-02-02 09:23:34.000000 nodriver-0.28rc1/nodriver/cdp/util.py
--rw-rw-rw-   0        0        0    18513 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/web_audio.py
--rw-rw-rw-   0        0        0    18390 2024-02-21 01:38:45.000000 nodriver-0.28rc1/nodriver/cdp/web_authn.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.207218 nodriver-0.28rc1/nodriver/core/
--rw-rw-rw-   0        0        0     3828 2024-02-04 19:44:05.000000 nodriver-0.28rc1/nodriver/core/_contradict.py
--rw-rw-rw-   0        0        0    28628 2024-04-20 15:13:01.000000 nodriver-0.28rc1/nodriver/core/browser.py
--rw-rw-rw-   0        0        0    10142 2024-03-10 03:03:41.000000 nodriver-0.28rc1/nodriver/core/config.py
--rw-rw-rw-   0        0        0    21366 2024-04-20 14:29:31.000000 nodriver-0.28rc1/nodriver/core/connection.py
--rw-rw-rw-   0        0        0    35674 2024-04-20 15:13:01.000000 nodriver-0.28rc1/nodriver/core/element.py
--rw-rw-rw-   0        0        0     1282 2024-03-26 18:00:57.000000 nodriver-0.28rc1/nodriver/core/extra.py
--rw-rw-rw-   0        0        0    50251 2024-04-20 15:13:01.000000 nodriver-0.28rc1/nodriver/core/tab.py
--rw-rw-rw-   0        0        0     9399 2024-03-10 03:04:45.000000 nodriver-0.28rc1/nodriver/core/util.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:14:10.208217 nodriver-0.28rc1/nodriver.egg-info/
--rw-rw-rw-   0        0        0    47611 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1828 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 15:14:10.000000 nodriver-0.28rc1/nodriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3560 2024-04-20 15:13:00.000000 nodriver-0.28rc1/pyproject.toml
--rw-rw-rw-   0        0        0       85 2024-04-20 15:14:10.209216 nodriver-0.28rc1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 11:22:35.757540 nodriver-0.29rc2/
+-rw-rw-rw-   0        0        0    32693 2024-01-18 14:05:42.000000 nodriver-0.29rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0      121 2024-02-25 19:31:30.000000 nodriver-0.29rc2/MANIFEST.in
+-rw-rw-rw-   0        0        0    47611 2024-04-30 11:22:35.757030 nodriver-0.29rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     8430 2024-02-25 18:42:37.000000 nodriver-0.29rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 11:22:35.730235 nodriver-0.29rc2/nodriver/
+-rw-rw-rw-   0        0        0      616 2024-03-10 03:03:41.000000 nodriver-0.29rc2/nodriver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:22:35.752834 nodriver-0.29rc2/nodriver/cdp/
+-rw-rw-rw-   0        0        0      172 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/README.md
+-rw-rw-rw-   0        0        0     1011 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/__init__.py
+-rw-rw-rw-   0        0        0    25019 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/accessibility.py
+-rw-rw-rw-   0        0        0    11919 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/animation.py
+-rw-rw-rw-   0        0        0    65075 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/audits.py
+-rw-rw-rw-   0        0        0     8168 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/autofill.py
+-rw-rw-rw-   0        0        0     6359 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/background_service.py
+-rw-rw-rw-   0        0        0    22888 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/browser.py
+-rw-rw-rw-   0        0        0     9549 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/cache_storage.py
+-rw-rw-rw-   0        0        0     4565 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/cast.py
+-rw-rw-rw-   0        0        0     3004 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/console.py
+-rw-rw-rw-   0        0        0    80456 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/css.py
+-rw-rw-rw-   0        0        0     4358 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/database.py
+-rw-rw-rw-   0        0        0    54782 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/debugger.py
+-rw-rw-rw-   0        0        0     3497 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/device_access.py
+-rw-rw-rw-   0        0        0     1187 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/device_orientation.py
+-rw-rw-rw-   0        0        0    66246 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/dom.py
+-rw-rw-rw-   0        0        0    10211 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/dom_debugger.py
+-rw-rw-rw-   0        0        0    43435 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/dom_snapshot.py
+-rw-rw-rw-   0        0        0     6124 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/dom_storage.py
+-rw-rw-rw-   0        0        0    34831 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/emulation.py
+-rw-rw-rw-   0        0        0     1501 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/event_breakpoints.py
+-rw-rw-rw-   0        0        0     7347 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/fed_cm.py
+-rw-rw-rw-   0        0        0    21611 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/fetch.py
+-rw-rw-rw-   0        0        0     5219 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/headless_experimental.py
+-rw-rw-rw-   0        0        0    14457 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/heap_profiler.py
+-rw-rw-rw-   0        0        0    18362 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/indexed_db.py
+-rw-rw-rw-   0        0        0    29314 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/input_.py
+-rw-rw-rw-   0        0        0     1743 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/inspector.py
+-rw-rw-rw-   0        0        0     3120 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/io.py
+-rw-rw-rw-   0        0        0    16878 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/layer_tree.py
+-rw-rw-rw-   0        0        0     6092 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/log.py
+-rw-rw-rw-   0        0        0     8215 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/media.py
+-rw-rw-rw-   0        0        0     7279 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/memory.py
+-rw-rw-rw-   0        0        0   147161 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/network.py
+-rw-rw-rw-   0        0        0    60483 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/overlay.py
+-rw-rw-rw-   0        0        0   117573 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/page.py
+-rw-rw-rw-   0        0        0     3203 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/performance.py
+-rw-rw-rw-   0        0        0     7587 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/performance_timeline.py
+-rw-rw-rw-   0        0        0    22524 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/preload.py
+-rw-rw-rw-   0        0        0    14302 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/profiler.py
+-rw-rw-rw-   0        0        0        0 2024-01-18 14:08:24.000000 nodriver-0.29rc2/nodriver/cdp/py.typed
+-rw-rw-rw-   0        0        0    67631 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/runtime.py
+-rw-rw-rw-   0        0        0     1196 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/schema.py
+-rw-rw-rw-   0        0        0    18824 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/security.py
+-rw-rw-rw-   0        0        0    12358 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/service_worker.py
+-rw-rw-rw-   0        0        0    61377 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/storage.py
+-rw-rw-rw-   0        0        0    12914 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/system_info.py
+-rw-rw-rw-   0        0        0    25505 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/target.py
+-rw-rw-rw-   0        0        0     1533 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/tethering.py
+-rw-rw-rw-   0        0        0    14682 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/tracing.py
+-rw-rw-rw-   0        0        0      470 2024-02-02 09:23:34.000000 nodriver-0.29rc2/nodriver/cdp/util.py
+-rw-rw-rw-   0        0        0    18513 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/web_audio.py
+-rw-rw-rw-   0        0        0    18390 2024-02-21 01:38:45.000000 nodriver-0.29rc2/nodriver/cdp/web_authn.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:22:35.755941 nodriver-0.29rc2/nodriver/core/
+-rw-rw-rw-   0        0        0     3886 2024-04-30 11:16:18.000000 nodriver-0.29rc2/nodriver/core/_contradict.py
+-rw-rw-rw-   0        0        0    28628 2024-04-20 15:13:01.000000 nodriver-0.29rc2/nodriver/core/browser.py
+-rw-rw-rw-   0        0        0    10142 2024-03-10 03:03:41.000000 nodriver-0.29rc2/nodriver/core/config.py
+-rw-rw-rw-   0        0        0    21366 2024-04-20 14:29:31.000000 nodriver-0.29rc2/nodriver/core/connection.py
+-rw-rw-rw-   0        0        0    39162 2024-04-30 11:16:18.000000 nodriver-0.29rc2/nodriver/core/element.py
+-rw-rw-rw-   0        0        0    50646 2024-04-30 11:16:18.000000 nodriver-0.29rc2/nodriver/core/tab.py
+-rw-rw-rw-   0        0        0     9399 2024-03-10 03:04:45.000000 nodriver-0.29rc2/nodriver/core/util.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:22:35.756454 nodriver-0.29rc2/nodriver.egg-info/
+-rw-rw-rw-   0        0        0    47611 2024-04-30 11:22:35.000000 nodriver-0.29rc2/nodriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1805 2024-04-30 11:22:35.000000 nodriver-0.29rc2/nodriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 11:22:35.000000 nodriver-0.29rc2/nodriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-04-30 11:22:35.000000 nodriver-0.29rc2/nodriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 11:22:35.000000 nodriver-0.29rc2/nodriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3560 2024-04-30 11:21:28.000000 nodriver-0.29rc2/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2024-04-30 11:22:35.758052 nodriver-0.29rc2/setup.cfg
```

### Comparing `nodriver-0.28rc1/LICENSE.txt` & `nodriver-0.29rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/PKG-INFO` & `nodriver-0.29rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodriver
-Version: 0.28rc1
+Version: 0.29rc2
 Summary: * Official successor of Undetected Chromedriver
 Author-email: UltrafunkAmsterdam <doesnotexist@ultrafunk.nl>
 Maintainer-email: UltrafunkAmsterdam <doesnotexist@ultrafunk.nl>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nodriver-0.28rc1/README.md` & `nodriver-0.29rc2/README.md`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/__init__.py` & `nodriver-0.29rc2/nodriver/__init__.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/__init__.py` & `nodriver-0.29rc2/nodriver/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/accessibility.py` & `nodriver-0.29rc2/nodriver/cdp/accessibility.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/animation.py` & `nodriver-0.29rc2/nodriver/cdp/animation.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/audits.py` & `nodriver-0.29rc2/nodriver/cdp/audits.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/autofill.py` & `nodriver-0.29rc2/nodriver/cdp/autofill.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/background_service.py` & `nodriver-0.29rc2/nodriver/cdp/background_service.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/browser.py` & `nodriver-0.29rc2/nodriver/cdp/browser.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/cache_storage.py` & `nodriver-0.29rc2/nodriver/cdp/cache_storage.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/cast.py` & `nodriver-0.29rc2/nodriver/cdp/cast.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/console.py` & `nodriver-0.29rc2/nodriver/cdp/console.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/css.py` & `nodriver-0.29rc2/nodriver/cdp/css.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/database.py` & `nodriver-0.29rc2/nodriver/cdp/database.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/debugger.py` & `nodriver-0.29rc2/nodriver/cdp/debugger.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/device_access.py` & `nodriver-0.29rc2/nodriver/cdp/device_access.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/device_orientation.py` & `nodriver-0.29rc2/nodriver/cdp/device_orientation.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/dom.py` & `nodriver-0.29rc2/nodriver/cdp/dom.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/dom_debugger.py` & `nodriver-0.29rc2/nodriver/cdp/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/dom_snapshot.py` & `nodriver-0.29rc2/nodriver/cdp/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/dom_storage.py` & `nodriver-0.29rc2/nodriver/cdp/dom_storage.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/emulation.py` & `nodriver-0.29rc2/nodriver/cdp/emulation.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/event_breakpoints.py` & `nodriver-0.29rc2/nodriver/cdp/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/fed_cm.py` & `nodriver-0.29rc2/nodriver/cdp/fed_cm.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/fetch.py` & `nodriver-0.29rc2/nodriver/cdp/fetch.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/headless_experimental.py` & `nodriver-0.29rc2/nodriver/cdp/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/heap_profiler.py` & `nodriver-0.29rc2/nodriver/cdp/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/indexed_db.py` & `nodriver-0.29rc2/nodriver/cdp/indexed_db.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/input_.py` & `nodriver-0.29rc2/nodriver/cdp/input_.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/inspector.py` & `nodriver-0.29rc2/nodriver/cdp/inspector.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/io.py` & `nodriver-0.29rc2/nodriver/cdp/io.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/layer_tree.py` & `nodriver-0.29rc2/nodriver/cdp/layer_tree.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/log.py` & `nodriver-0.29rc2/nodriver/cdp/log.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/media.py` & `nodriver-0.29rc2/nodriver/cdp/media.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/memory.py` & `nodriver-0.29rc2/nodriver/cdp/memory.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/network.py` & `nodriver-0.29rc2/nodriver/cdp/network.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/overlay.py` & `nodriver-0.29rc2/nodriver/cdp/overlay.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/page.py` & `nodriver-0.29rc2/nodriver/cdp/page.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/performance.py` & `nodriver-0.29rc2/nodriver/cdp/performance.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/performance_timeline.py` & `nodriver-0.29rc2/nodriver/cdp/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/preload.py` & `nodriver-0.29rc2/nodriver/cdp/preload.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/profiler.py` & `nodriver-0.29rc2/nodriver/cdp/profiler.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/runtime.py` & `nodriver-0.29rc2/nodriver/cdp/runtime.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/schema.py` & `nodriver-0.29rc2/nodriver/cdp/schema.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/security.py` & `nodriver-0.29rc2/nodriver/cdp/security.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/service_worker.py` & `nodriver-0.29rc2/nodriver/cdp/service_worker.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/storage.py` & `nodriver-0.29rc2/nodriver/cdp/storage.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/system_info.py` & `nodriver-0.29rc2/nodriver/cdp/system_info.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/target.py` & `nodriver-0.29rc2/nodriver/cdp/target.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/tethering.py` & `nodriver-0.29rc2/nodriver/cdp/tethering.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/tracing.py` & `nodriver-0.29rc2/nodriver/cdp/tracing.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/web_audio.py` & `nodriver-0.29rc2/nodriver/cdp/web_audio.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/cdp/web_authn.py` & `nodriver-0.29rc2/nodriver/cdp/web_authn.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/core/_contradict.py` & `nodriver-0.29rc2/nodriver/core/_contradict.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
     def __dir__(self):
         a = list(self.keys())
         if self.__hide_properties__:
             a += [
                 _ for _ in super().__dir__() if inspect.ismethod(getattr(self, _, None))
             ]
+        a += list(self.__class__.__annotations__.keys())
         return a
 
 
 def _wrap(cls, v):
     if isinstance(v, _Mapping):
         v = cls(v)
```

### Comparing `nodriver-0.28rc1/nodriver/core/browser.py` & `nodriver-0.29rc2/nodriver/core/browser.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/core/config.py` & `nodriver-0.29rc2/nodriver/core/config.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/core/connection.py` & `nodriver-0.29rc2/nodriver/core/connection.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver/core/element.py` & `nodriver-0.29rc2/nodriver/core/element.py`

 * *Files 6% similar despite different names*

```diff
@@ -224,25 +224,26 @@
     def __getitem__(self, item):
         # we probably deal with an attribute of
         # the html element, so forward it
         return self.attrs.get(item, None)
 
     async def save_to_dom(self):
         """
-        saves a screenshot of this element only
+        saves element to dom
         :return:
         :rtype:
         """
         self._remote_object = await self._tab.send(
             cdp.dom.resolve_node(backend_node_id=self.backend_node_id)
         )
         await self._tab.send(cdp.dom.set_outer_html(self.node_id, outer_html=str(self)))
         await self.update()
 
     async def remove_from_dom(self):
+        """removes the element from dom"""
         await self.update()  # ensure we have latest node_id
         node = util.filter_recurse(
             self._tree, lambda node: node.backend_node_id == self.backend_node_id
         )
         if node:
             await self.tab.send(cdp.dom.remove_node(node.node_id))
         # self._tree = util.remove_from_tree(self.tree, self.node)
@@ -507,14 +508,15 @@
             )
 
     async def mouse_click(
         self,
         button: str = "left",
         buttons: typing.Optional[int] = 1,
         modifiers: typing.Optional[int] = 0,
+        hold: bool = False,
         _until_event: typing.Optional[type] = None,
     ):
         """native click (on element) . note: this likely does not work atm, use click() instead
 
         :param button: str (default = "left")
         :param buttons: which button (default 1 = left)
         :param modifiers: *(Optional)* Bit field representing pressed modifier keys.
@@ -577,14 +579,108 @@
             cdp.input_.dispatch_mouse_event("mouseMoved", x=center[0], y=center[1])
         )
         await self._tab.sleep(0.05)
         await self._tab.send(
             cdp.input_.dispatch_mouse_event("mouseReleased", x=center[0], y=center[1])
         )
 
+    async def mouse_drag(
+        self,
+        destination: typing.Union[Element, typing.Tuple[int, int]],
+        relative: bool = False,
+        steps: int = 1,
+    ):
+        """
+        drag an element to another element or target coordinates. dragging of elements should be supported  by the site of course
+
+
+        :param destination: another element where to drag to, or a tuple (x,y) of ints representing coordinate
+        :type destination: Element or coordinate as x,y tuple
+
+        :param relative: when True, treats coordinate as relative. for example (-100, 200) will move left 100px and down 200px
+        :type relative:
+
+        :param steps: move in <steps> points, this could make it look more "natural" (default 1),
+               but also a lot slower.
+               for very smooth action use 50-100
+        :type steps: int
+        :return:
+        :rtype:
+        """
+        try:
+            start_point = (await self.get_position()).center
+        except AttributeError:
+            return
+        if not start_point:
+            logger.warning("could not calculate box model for %s", self)
+            return
+        end_point = None
+        if isinstance(destination, Element):
+            try:
+                end_point = (await destination.get_position()).center
+            except AttributeError:
+                return
+            if not end_point:
+                logger.warning("could not calculate box model for %s", destination)
+                return
+        elif isinstance(destination, (tuple, list)):
+            if relative:
+                end_point = (
+                    start_point[0] + destination[0],
+                    start_point[1] + destination[1],
+                )
+            else:
+                end_point = destination
+
+        await self._tab.send(
+            cdp.input_.dispatch_mouse_event(
+                "mousePressed",
+                x=start_point[0],
+                y=start_point[1],
+                button=cdp.input_.MouseButton("left"),
+            )
+        )
+
+        steps = 1 if (not steps or steps < 1) else steps
+        if steps == 1:
+            await self._tab.send(
+                cdp.input_.dispatch_mouse_event(
+                    "mouseMoved",
+                    x=end_point[0],
+                    y=end_point[1],
+                )
+            )
+        elif steps > 1:
+            # probably the worst waay of calculating this. but couldn't think of a better solution today.
+            step_size_x = (end_point[0] - start_point[0]) / steps
+            step_size_y = (end_point[1] - start_point[1]) / steps
+            pathway = [
+                (start_point[0] + step_size_x * i, start_point[1] + step_size_y * i)
+                for i in range(steps + 1)
+            ]
+
+            for point in pathway:
+                await self._tab.send(
+                    cdp.input_.dispatch_mouse_event(
+                        "mouseMoved",
+                        x=point[0],
+                        y=point[1],
+                    )
+                )
+                await asyncio.sleep(0)
+
+        await self._tab.send(
+            cdp.input_.dispatch_mouse_event(
+                type_="mouseReleased",
+                x=end_point[0],
+                y=end_point[1],
+                button=cdp.input_.MouseButton("left"),
+            )
+        )
+
     async def scroll_into_view(self):
         """scrolls element into view"""
         try:
             await self.tab.send(
                 cdp.dom.scroll_into_view_if_needed(backend_node_id=self.backend_node_id)
             )
         except Exception as e:
```

### Comparing `nodriver-0.28rc1/nodriver/core/tab.py` & `nodriver-0.29rc2/nodriver/core/tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,33 +274,40 @@
                 raise asyncio.TimeoutError(
                     "time ran out while waiting for text: %s" % text
                 )
             await self.sleep(0.5)
         return items
 
     async def select_all(
-        self,
-        selector: str,
-        timeout: Union[int, float] = 10,
+        self, selector: str, timeout: Union[int, float] = 10, include_frames=False
     ) -> List[nodriver.Element]:
         """
         find multiple elements by css selector.
         can also be used to wait for such element to appear.
 
+
         :param selector: css selector, eg a[href], button[class*=close], a > img[src]
         :type selector: str
         :param timeout: raise timeout exception when after this many seconds nothing is found.
         :type timeout: float,int
+        :param include_frames: whether to include results in iframes.
+        :type include_frames: bool
         """
 
         loop = asyncio.get_running_loop()
         now = loop.time()
         selector = selector.strip()
+        items = []
+        if include_frames:
+            frames = await self.query_selector_all("iframe")
+            # unfortunately, asyncio.gather here is not an option
+            for fr in frames:
+                items.extend(await fr.query_selector_all(selector))
 
-        items = await self.query_selector_all(selector)
+        items.extend(await self.query_selector_all(selector))
         while not items:
             await self
             items = await self.query_selector_all(selector)
             if loop.time() - now > timeout:
                 raise asyncio.TimeoutError(
                     "time ran out while waiting for %s" % selector
                 )
```

### Comparing `nodriver-0.28rc1/nodriver/core/util.py` & `nodriver-0.29rc2/nodriver/core/util.py`

 * *Files identical despite different names*

### Comparing `nodriver-0.28rc1/nodriver.egg-info/PKG-INFO` & `nodriver-0.29rc2/nodriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodriver
-Version: 0.28rc1
+Version: 0.29rc2
 Summary: * Official successor of Undetected Chromedriver
 Author-email: UltrafunkAmsterdam <doesnotexist@ultrafunk.nl>
 Maintainer-email: UltrafunkAmsterdam <doesnotexist@ultrafunk.nl>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nodriver-0.28rc1/nodriver.egg-info/SOURCES.txt` & `nodriver-0.29rc2/nodriver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,10 +64,9 @@
 nodriver/cdp/web_audio.py
 nodriver/cdp/web_authn.py
 nodriver/core/_contradict.py
 nodriver/core/browser.py
 nodriver/core/config.py
 nodriver/core/connection.py
 nodriver/core/element.py
-nodriver/core/extra.py
 nodriver/core/tab.py
 nodriver/core/util.py
```

### Comparing `nodriver-0.28rc1/pyproject.toml` & `nodriver-0.29rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nodriver" # Required
-version = "0.28rc1"  # Required
+version = "0.29rc2"  # Required
 description = """
     * Official successor of Undetected Chromedriver
     * Can be made to work for for all chromium based browsers.
     * Dropped selenium and chromedriver binary requirements.
     * fully asynchronous == bizarre performance gains, and more granular control
 
     Part of undetected-chromedriver, or merely the successor of it, this library is a full rewrite, providing a
```

