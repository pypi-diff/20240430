# Comparing `tmp/chat-miner-0.5.2.tar.gz` & `tmp/chat_miner-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-miner-0.5.2.tar", last modified: Sat Mar 16 09:00:29 2024, max compression
+gzip compressed data, was "chat_miner-0.5.3.tar", last modified: Tue Apr 30 20:54:38 2024, max compression
```

## Comparing `chat-miner-0.5.2.tar` & `chat_miner-0.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:00:29.200200 chat-miner-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-16 09:00:24.000000 chat-miner-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-16 09:00:29.200200 chat-miner-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-16 09:00:24.000000 chat-miner-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:00:29.200200 chat-miner-0.5.2/chat_miner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-16 09:00:29.000000 chat-miner-0.5.2/chat_miner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-16 09:00:29.000000 chat-miner-0.5.2/chat_miner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 09:00:29.000000 chat-miner-0.5.2/chat_miner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-16 09:00:29.000000 chat-miner-0.5.2/chat_miner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-16 09:00:29.000000 chat-miner-0.5.2/chat_miner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-16 09:00:29.000000 chat-miner-0.5.2/chat_miner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:00:29.200200 chat-miner-0.5.2/chatminer/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-16 09:00:24.000000 chat-miner-0.5.2/chatminer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12754 2024-03-16 09:00:24.000000 chat-miner-0.5.2/chatminer/chatparsers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-03-16 09:00:24.000000 chat-miner-0.5.2/chatminer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-16 09:00:24.000000 chat-miner-0.5.2/chatminer/nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-03-16 09:00:24.000000 chat-miner-0.5.2/chatminer/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-16 09:00:24.000000 chat-miner-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-16 09:00:29.200200 chat-miner-0.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      483 2024-03-16 09:00:24.000000 chat-miner-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:00:29.200200 chat-miner-0.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 09:00:24.000000 chat-miner-0.5.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-16 09:00:24.000000 chat-miner-0.5.2/test/test_instagram.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-16 09:00:24.000000 chat-miner-0.5.2/test/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-16 09:00:24.000000 chat-miner-0.5.2/test/test_telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-16 09:00:24.000000 chat-miner-0.5.2/test/test_whatsapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:54:38.873614 chat_miner-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 20:54:34.000000 chat_miner-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-30 20:54:38.873614 chat_miner-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-30 20:54:34.000000 chat_miner-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:54:38.873614 chat_miner-0.5.3/chat_miner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-30 20:54:38.000000 chat_miner-0.5.3/chat_miner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-30 20:54:38.000000 chat_miner-0.5.3/chat_miner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:54:38.000000 chat_miner-0.5.3/chat_miner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 20:54:38.000000 chat_miner-0.5.3/chat_miner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 20:54:38.000000 chat_miner-0.5.3/chat_miner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 20:54:38.000000 chat_miner-0.5.3/chat_miner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:54:38.873614 chat_miner-0.5.3/chatminer/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-30 20:54:34.000000 chat_miner-0.5.3/chatminer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-04-30 20:54:34.000000 chat_miner-0.5.3/chatminer/chatparsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-30 20:54:34.000000 chat_miner-0.5.3/chatminer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-30 20:54:34.000000 chat_miner-0.5.3/chatminer/nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-30 20:54:34.000000 chat_miner-0.5.3/chatminer/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 20:54:34.000000 chat_miner-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-30 20:54:38.873614 chat_miner-0.5.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      483 2024-04-30 20:54:34.000000 chat_miner-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:54:38.873614 chat_miner-0.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:54:34.000000 chat_miner-0.5.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-30 20:54:34.000000 chat_miner-0.5.3/test/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-30 20:54:34.000000 chat_miner-0.5.3/test/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 20:54:34.000000 chat_miner-0.5.3/test/test_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-30 20:54:34.000000 chat_miner-0.5.3/test/test_whatsapp.py
```

### Comparing `chat-miner-0.5.2/LICENSE` & `chat_miner-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-miner-0.5.2/PKG-INFO` & `chat_miner-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-miner
-Version: 0.5.2
+Version: 0.5.3
 Summary: chat-miner provides lean parsers for every major platform transforming chats into dataframes.         Artistic visualizations allow you to explore your data and create artwork from your chats.
 Author: Jonas Weich
 Author-email: jns.wch@gmail.com
 Maintainer: Jonas Weich
 Maintainer-email: jns.wch@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/joweich/chat-miner/issues
```

### Comparing `chat-miner-0.5.2/README.md` & `chat_miner-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `chat-miner-0.5.2/chat_miner.egg-info/PKG-INFO` & `chat_miner-0.5.3/chat_miner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-miner
-Version: 0.5.2
+Version: 0.5.3
 Summary: chat-miner provides lean parsers for every major platform transforming chats into dataframes.         Artistic visualizations allow you to explore your data and create artwork from your chats.
 Author: Jonas Weich
 Author-email: jns.wch@gmail.com
 Maintainer: Jonas Weich
 Maintainer-email: jns.wch@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/joweich/chat-miner/issues
```

### Comparing `chat-miner-0.5.2/chatminer/__init__.py` & `chat_miner-0.5.3/chatminer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   X.Y.ZbN   # Beta release
 #   X.Y.ZrcN  # Release Candidate
 #   X.Y.Z     # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.5.2"
+__version__ = "0.5.3"
```

### Comparing `chat-miner-0.5.2/chatminer/chatparsers.py` & `chat_miner-0.5.3/chatminer/chatparsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 class WhatsAppParser(Parser):
     def __init__(self, filepath: str):
         super().__init__(filepath)
         self._datefmt = WhatsAppDateFormat(self._logger)
 
     def _read_raw_messages_from_file(self):
         def _is_new_message(line: str):
-            regex = r"^[\u200e]?\[?(\d{1,4})([./,-])\d{1,2}\2\d{2,4}([, ])"
+            regex = r"^[\u200e]?\[?(\d{1,4})([./,-])\d{1,2}\2\d{2,4}(?:\s|,\s)(0?\d|1\d|2[0-4]):([0-5]?\d)"
             return re.match(regex, line)
 
         with self._file.open(encoding="utf-8") as f:
             lines = reversed(list(f))
 
         self._raw_messages: List[str]
         buffer: List[str] = []
```

### Comparing `chat-miner-0.5.2/chatminer/cli.py` & `chat_miner-0.5.3/chatminer/cli.py`

 * *Files identical despite different names*

### Comparing `chat-miner-0.5.2/chatminer/nlp.py` & `chat_miner-0.5.3/chatminer/nlp.py`

 * *Files identical despite different names*

### Comparing `chat-miner-0.5.2/chatminer/visualizations.py` & `chat_miner-0.5.3/chatminer/visualizations.py`

 * *Files identical despite different names*

### Comparing `chat-miner-0.5.2/setup.cfg` & `chat_miner-0.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `chat-miner-0.5.2/test/test_telegram.py` & `chat_miner-0.5.3/test/test_telegram.py`

 * *Files identical despite different names*

### Comparing `chat-miner-0.5.2/test/test_whatsapp.py` & `chat_miner-0.5.3/test/test_whatsapp.py`

 * *Files identical despite different names*

