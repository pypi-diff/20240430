# Comparing `tmp/zodchy-0.2.2.tar.gz` & `tmp/zodchy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy-0.2.2.tar", max compression
+gzip compressed data, was "zodchy-0.2.3.tar", max compression
```

## Comparing `zodchy-0.2.2.tar` & `zodchy-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy-0.2.2/README.md
--rw-r--r--   0        0        0      476 2024-04-29 09:46:18.933000 zodchy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-26 14:09:47.283719 zodchy-0.2.2/zodchy/__init__.py
--rw-r--r--   0        0        0       60 2024-04-26 14:04:00.386664 zodchy-0.2.2/zodchy/codex/__init__.py
--rw-r--r--   0        0        0      304 2024-04-26 13:33:12.470259 zodchy-0.2.2/zodchy/codex/cqea/__init__.py
--rw-r--r--   0        0        0      648 2024-04-26 14:04:00.437433 zodchy-0.2.2/zodchy/codex/cqea/actors.py
--rw-r--r--   0        0        0     1083 2024-04-26 13:33:12.496006 zodchy-0.2.2/zodchy/codex/cqea/messages.py
--rw-r--r--   0        0        0     1468 2024-04-11 07:57:07.719538 zodchy-0.2.2/zodchy/codex/di.py
--rw-r--r--   0        0        0      171 2024-04-26 12:52:44.493427 zodchy-0.2.2/zodchy/codex/identity.py
--rw-r--r--   0        0        0      260 2024-04-28 14:31:54.892258 zodchy-0.2.2/zodchy/codex/query/__init__.py
--rw-r--r--   0        0        0     2438 2024-04-26 14:04:00.412260 zodchy-0.2.2/zodchy/codex/query/bits.py
--rw-r--r--   0        0        0      395 2024-04-29 09:46:18.926712 zodchy-0.2.2/zodchy/codex/query/parsing.py
--rw-r--r--   0        0        0       53 2024-04-26 14:05:35.505418 zodchy-0.2.2/zodchy/types.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 zodchy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy-0.2.3/README.md
+-rw-r--r--   0        0        0      476 2024-04-29 10:18:10.969652 zodchy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-26 14:09:47.283719 zodchy-0.2.3/zodchy/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-26 14:04:00.386664 zodchy-0.2.3/zodchy/codex/__init__.py
+-rw-r--r--   0        0        0      304 2024-04-26 13:33:12.470259 zodchy-0.2.3/zodchy/codex/cqea/__init__.py
+-rw-r--r--   0        0        0      648 2024-04-26 14:04:00.437433 zodchy-0.2.3/zodchy/codex/cqea/actors.py
+-rw-r--r--   0        0        0     1083 2024-04-26 13:33:12.496006 zodchy-0.2.3/zodchy/codex/cqea/messages.py
+-rw-r--r--   0        0        0     1468 2024-04-11 07:57:07.719538 zodchy-0.2.3/zodchy/codex/di.py
+-rw-r--r--   0        0        0      171 2024-04-26 12:52:44.493427 zodchy-0.2.3/zodchy/codex/identity.py
+-rw-r--r--   0        0        0      330 2024-04-29 10:18:10.974825 zodchy-0.2.3/zodchy/codex/query/__init__.py
+-rw-r--r--   0        0        0     2438 2024-04-26 14:04:00.412260 zodchy-0.2.3/zodchy/codex/query/bits.py
+-rw-r--r--   0        0        0      395 2024-04-29 10:16:33.980878 zodchy-0.2.3/zodchy/codex/query/parsing.py
+-rw-r--r--   0        0        0       53 2024-04-26 14:05:35.505418 zodchy-0.2.3/zodchy/types.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 zodchy-0.2.3/PKG-INFO
```

### Comparing `zodchy-0.2.2/zodchy/codex/cqea/actors.py` & `zodchy-0.2.3/zodchy/codex/cqea/actors.py`

 * *Files identical despite different names*

### Comparing `zodchy-0.2.2/zodchy/codex/cqea/messages.py` & `zodchy-0.2.3/zodchy/codex/cqea/messages.py`

 * *Files identical despite different names*

### Comparing `zodchy-0.2.2/zodchy/codex/di.py` & `zodchy-0.2.3/zodchy/codex/di.py`

 * *Files identical despite different names*

### Comparing `zodchy-0.2.2/zodchy/codex/query/bits.py` & `zodchy-0.2.3/zodchy/codex/query/bits.py`

 * *Files identical despite different names*

### Comparing `zodchy-0.2.2/PKG-INFO` & `zodchy-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zodchy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Collection of contracts and tools for building CQRS applications
 Home-page: https://github.com/smairon/zodchy
 Author: Smairon
 Author-email: man@smairon.ru
 Maintainer: Smairon
 Maintainer-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
```

