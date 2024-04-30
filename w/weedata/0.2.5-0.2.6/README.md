# Comparing `tmp/weedata-0.2.5.tar.gz` & `tmp/weedata-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weedata-0.2.5.tar", last modified: Sat Apr 20 12:24:17 2024, max compression
+gzip compressed data, was "weedata-0.2.6.tar", last modified: Tue Apr 30 19:07:03 2024, max compression
```

## Comparing `weedata-0.2.5.tar` & `weedata-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 12:24:17.047013 weedata-0.2.5/
--rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.5/LICENSE
--rw-rw-rw-   0        0        0    19210 2024-04-20 12:24:17.043013 weedata-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    16225 2024-04-20 12:22:52.000000 weedata-0.2.5/README.md
--rw-rw-rw-   0        0        0     1417 2024-04-20 12:23:07.000000 weedata-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-20 12:24:17.048013 weedata-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-20 12:24:16.825013 weedata-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-20 12:24:16.874014 weedata-0.2.5/src/weedata/
--rw-rw-rw-   0        0        0      497 2024-04-20 12:22:59.000000 weedata-0.2.5/src/weedata/__init__.py
--rw-rw-rw-   0        0        0    32289 2024-04-19 13:16:57.000000 weedata-0.2.5/src/weedata/client.py
--rw-rw-rw-   0        0        0    15500 2024-04-13 15:58:34.000000 weedata-0.2.5/src/weedata/fields.py
--rw-rw-rw-   0        0        0     9863 2024-04-20 12:22:08.000000 weedata-0.2.5/src/weedata/model.py
--rw-rw-rw-   0        0        0     8132 2024-04-19 12:41:56.000000 weedata-0.2.5/src/weedata/queries.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:24:17.039013 weedata-0.2.5/src/weedata.egg-info/
--rw-rw-rw-   0        0        0    19210 2024-04-20 12:24:16.000000 weedata-0.2.5/src/weedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-04-20 12:24:16.000000 weedata-0.2.5/src/weedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 12:24:16.000000 weedata-0.2.5/src/weedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-20 12:24:16.000000 weedata-0.2.5/src/weedata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-20 12:24:17.018013 weedata-0.2.5/tests/
--rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.5/tests/test_base.py
--rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.5/tests/test_connection.py
--rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.5/tests/test_delete.py
--rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.5/tests/test_fields.py
--rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.5/tests/test_queries.py
--rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.5/tests/test_save.py
--rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.5/tests/test_update.py
+drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.225186 weedata-0.2.6/
+-rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0    19300 2024-04-30 19:07:03.214186 weedata-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    16310 2024-04-30 18:09:55.000000 weedata-0.2.6/README.md
+-rw-rw-rw-   0        0        0     1417 2024-04-30 18:10:10.000000 weedata-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 19:07:03.226186 weedata-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.065186 weedata-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.104186 weedata-0.2.6/src/weedata/
+-rw-rw-rw-   0        0        0      497 2024-04-20 12:22:59.000000 weedata-0.2.6/src/weedata/__init__.py
+-rw-rw-rw-   0        0        0    32289 2024-04-30 18:36:56.000000 weedata-0.2.6/src/weedata/client.py
+-rw-rw-rw-   0        0        0    15767 2024-04-30 18:36:13.000000 weedata-0.2.6/src/weedata/fields.py
+-rw-rw-rw-   0        0        0     9863 2024-04-20 12:22:08.000000 weedata-0.2.6/src/weedata/model.py
+-rw-rw-rw-   0        0        0     8132 2024-04-19 12:41:56.000000 weedata-0.2.6/src/weedata/queries.py
+drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.211186 weedata-0.2.6/src/weedata.egg-info/
+-rw-rw-rw-   0        0        0    19300 2024-04-30 19:07:02.000000 weedata-0.2.6/src/weedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-04-30 19:07:03.000000 weedata-0.2.6/src/weedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 19:07:03.000000 weedata-0.2.6/src/weedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-30 19:07:03.000000 weedata-0.2.6/src/weedata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.191186 weedata-0.2.6/tests/
+-rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.6/tests/test_base.py
+-rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.6/tests/test_connection.py
+-rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.6/tests/test_delete.py
+-rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.6/tests/test_fields.py
+-rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.6/tests/test_queries.py
+-rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.6/tests/test_save.py
+-rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.6/tests/test_update.py
```

### Comparing `weedata-0.2.5/LICENSE` & `weedata-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/PKG-INFO` & `weedata-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.5
+Version: 0.2.6
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -478,14 +478,19 @@
 
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
+
+* v0.2.6
+1. bugfix: Compatible with peewee, store datetime without timezone info.
+
+
 * v0.2.5
 1. bugfix: The compatibility problem of get_or_none().
 
 
 * v0.2.4
 1. Optimize the modification logic for JSONField, saving to the database at any time.
```

### Comparing `weedata-0.2.5/README.md` & `weedata-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -428,14 +428,19 @@
 
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
+
+* v0.2.6
+1. bugfix: Compatible with peewee, store datetime without timezone info.
+
+
 * v0.2.5
 1. bugfix: The compatibility problem of get_or_none().
 
 
 * v0.2.4
 1. Optimize the modification logic for JSONField, saving to the database at any time.
```

### Comparing `weedata-0.2.5/pyproject.toml` & `weedata-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "weedata"
-version = "0.2.5"
+version = "0.2.6"
 description = "an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 keywords = ["peewee", "ORM", "ODM", "google cloud datastore", "MongoDB", "redis"]
 dependencies = [
 #  "google-cloud-datastore",
```

### Comparing `weedata-0.2.5/src/weedata/client.py` & `weedata-0.2.6/src/weedata/client.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/src/weedata/fields.py` & `weedata-0.2.6/src/weedata/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,34 +359,39 @@
     def check_type(self, value):
         return isinstance(value, bytes)
     def db_value(self, value):
         return value
     def python_value(self, value):
         return value
 
+#compatible with peewee, datetime without timezone
 class DateTimeField(Field):
+    default_tmfmt = "%Y-%m-%d %H:%M:%S"
     def check_type(self, value):
         return isinstance(value, datetime.datetime)
     def db_value(self, value):
         if self.bytes_store:
-            if not value:
-                return b''
-            elif isinstance(value, datetime.datetime):
-                return value.isoformat().encode('utf-8')
+            if isinstance(value, datetime.datetime):
+                value = value.strftime(self.default_tmfmt)
             else:
-                return value
+                value = value or ''
+            return value.encode('utf-8')
+        elif isinstance(value, datetime.datetime):
+            return value.replace(tzinfo=None)
         else:
             return value
+
     def python_value(self, value):
+        if isinstance(value, bytes):
+            value = value.decode('utf-8')
+        
         if self.bytes_store:
-            if not value:
-                return None
-            else:
-                value = value.decode('utf-8') if isinstance(value, bytes)  else value
-                return datetime.datetime.fromisoformat(value)
+            return datetime.datetime.strptime(value, self.default_tmfmt).replace(tzinfo=None) if value else None
+        elif isinstance(value, datetime.datetime):
+            return value.replace(tzinfo=None)
         else:
             return value
 
 class JSONField(Field):
     def __init__(self, **kwargs):
         kwargs.setdefault('index', False)
         super().__init__(**kwargs)
```

### Comparing `weedata-0.2.5/src/weedata/model.py` & `weedata-0.2.6/src/weedata/model.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/src/weedata/queries.py` & `weedata-0.2.6/src/weedata/queries.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/src/weedata.egg-info/PKG-INFO` & `weedata-0.2.6/src/weedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.5
+Version: 0.2.6
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -478,14 +478,19 @@
 
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
+
+* v0.2.6
+1. bugfix: Compatible with peewee, store datetime without timezone info.
+
+
 * v0.2.5
 1. bugfix: The compatibility problem of get_or_none().
 
 
 * v0.2.4
 1. Optimize the modification logic for JSONField, saving to the database at any time.
```

### Comparing `weedata-0.2.5/tests/test_base.py` & `weedata-0.2.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/tests/test_connection.py` & `weedata-0.2.6/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/tests/test_delete.py` & `weedata-0.2.6/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/tests/test_fields.py` & `weedata-0.2.6/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/tests/test_queries.py` & `weedata-0.2.6/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/tests/test_save.py` & `weedata-0.2.6/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.5/tests/test_update.py` & `weedata-0.2.6/tests/test_update.py`

 * *Files identical despite different names*

