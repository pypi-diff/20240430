# Comparing `tmp/remindmail-2024.4.28.2.tar.gz` & `tmp/remindmail-2024.4.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2024.4.28.2.tar", last modified: Sun Apr 28 19:30:13 2024, max compression
+gzip compressed data, was "remindmail-2024.4.29.1.tar", last modified: Tue Apr 30 04:52:53 2024, max compression
```

## Comparing `remindmail-2024.4.28.2.tar` & `remindmail-2024.4.29.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 19:30:13.709124 remindmail-2024.4.28.2/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.28.2/LICENSE.md
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-28 19:30:13.709124 remindmail-2024.4.28.2/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.4.28.2/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.28.2/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-28 19:30:13.709124 remindmail-2024.4.28.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 19:30:13.705124 remindmail-2024.4.28.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 19:30:13.709124 remindmail-2024.4.28.2/src/remind/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.28.2/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2927 2024-04-21 19:03:57.000000 remindmail-2024.4.28.2/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.28.2/src/remind/error_handler.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11616 2024-04-28 19:30:00.000000 remindmail-2024.4.28.2/src/remind/query_manager.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    10846 2024-04-28 18:42:11.000000 remindmail-2024.4.28.2/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    24388 2024-04-28 19:22:42.000000 remindmail-2024.4.28.2/src/remind/reminder_confirmation.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    18650 2024-04-21 19:03:57.000000 remindmail-2024.4.28.2/src/remind/reminder_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-28 19:30:13.709124 remindmail-2024.4.28.2/src/remindmail.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-28 19:30:13.000000 remindmail-2024.4.28.2/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-28 19:30:13.000000 remindmail-2024.4.28.2/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-28 19:30:13.000000 remindmail-2024.4.28.2/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-28 19:30:13.000000 remindmail-2024.4.28.2/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-28 19:30:13.000000 remindmail-2024.4.28.2/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 04:52:53.167540 remindmail-2024.4.29.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.29.1/LICENSE.md
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-30 04:52:53.167540 remindmail-2024.4.29.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.4.29.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.29.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-30 04:52:53.167540 remindmail-2024.4.29.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 04:52:53.167540 remindmail-2024.4.29.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 04:52:53.167540 remindmail-2024.4.29.1/src/remind/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.29.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2927 2024-04-21 19:03:57.000000 remindmail-2024.4.29.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.29.1/src/remind/error_handler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11720 2024-04-30 04:51:52.000000 remindmail-2024.4.29.1/src/remind/query_manager.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    10846 2024-04-28 18:42:11.000000 remindmail-2024.4.29.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    24388 2024-04-28 19:22:42.000000 remindmail-2024.4.29.1/src/remind/reminder_confirmation.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    18650 2024-04-21 19:03:57.000000 remindmail-2024.4.29.1/src/remind/reminder_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 04:52:53.167540 remindmail-2024.4.29.1/src/remindmail.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-30 04:52:53.000000 remindmail-2024.4.29.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-30 04:52:53.000000 remindmail-2024.4.29.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-30 04:52:53.000000 remindmail-2024.4.29.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-30 04:52:53.000000 remindmail-2024.4.29.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-30 04:52:53.000000 remindmail-2024.4.29.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2024.4.28.2/LICENSE.md` & `remindmail-2024.4.29.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.28.2/PKG-INFO` & `remindmail-2024.4.29.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.28.2
+Version: 2024.4.29.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2024.4.28.2/README.md` & `remindmail-2024.4.29.1/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.28.2/setup.cfg` & `remindmail-2024.4.29.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2024.04.28.2
+version = 2024.04.29.1
 author = Tyler Woodfin
 author_email = feedback-remindmail@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2024.4.28.2/src/remind/__main__.py` & `remindmail-2024.4.29.1/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.28.2/src/remind/error_handler.py` & `remindmail-2024.4.29.1/src/remind/error_handler.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.28.2/src/remind/query_manager.py` & `remindmail-2024.4.29.1/src/remind/query_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,18 @@
                 key = ReminderKeyType.DATE
                 value = start_date.strftime('%Y-%m-%d')
 
             # now
             elif input_str == 'now':
                 key = ReminderKeyType.NOW
 
+            # later
+            elif input_str == 'later':
+                key = ReminderKeyType.LATER
+
         else:
             # 'every'
             modifiers = ''
 
             # every n days
             if match := regex_patterns['every_n_days'].match(input_str):
                 key = ReminderKeyType.DAY
```

### Comparing `remindmail-2024.4.28.2/src/remind/reminder.py` & `remindmail-2024.4.29.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.28.2/src/remind/reminder_confirmation.py` & `remindmail-2024.4.29.1/src/remind/reminder_confirmation.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.28.2/src/remind/reminder_manager.py` & `remindmail-2024.4.29.1/src/remind/reminder_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.28.2/src/remindmail.egg-info/PKG-INFO` & `remindmail-2024.4.29.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.28.2
+Version: 2024.4.29.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

