# Comparing `tmp/wdb_utils-2.0.0.tar.gz` & `tmp/wdb_utils-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdb_utils-2.0.0.tar", last modified: Thu Nov 16 21:19:56 2023, max compression
+gzip compressed data, was "wdb_utils-2.1.0.tar", last modified: Tue Apr 30 17:37:28 2024, max compression
```

## Comparing `wdb_utils-2.0.0.tar` & `wdb_utils-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 cwade      (503) staff       (20)        0 2023-11-16 21:19:56.513499 wdb_utils-2.0.0/
--rw-r--r--   0 cwade      (503) staff       (20)      743 2023-11-16 21:19:56.513427 wdb_utils-2.0.0/PKG-INFO
--rw-------   0 cwade      (503) staff       (20)     1386 2023-11-16 21:18:13.000000 wdb_utils-2.0.0/README.md
--rw-------   0 cwade      (503) staff       (20)      582 2023-11-16 21:19:56.513843 wdb_utils-2.0.0/setup.cfg
--rw-------   0 cwade      (503) staff       (20)      645 2023-11-16 21:19:14.000000 wdb_utils-2.0.0/setup.py
-drwxr-xr-x   0 cwade      (503) staff       (20)        0 2023-11-16 21:19:56.511592 wdb_utils-2.0.0/wdb_utils/
--rw-------   0 cwade      (503) staff       (20)     5797 2023-11-16 21:14:27.000000 wdb_utils-2.0.0/wdb_utils/__init__.py
-drwxr-xr-x   0 cwade      (503) staff       (20)        0 2023-11-16 21:19:56.513140 wdb_utils-2.0.0/wdb_utils.egg-info/
--rw-r--r--   0 cwade      (503) staff       (20)      743 2023-11-16 21:19:56.000000 wdb_utils-2.0.0/wdb_utils.egg-info/PKG-INFO
--rw-r--r--   0 cwade      (503) staff       (20)      214 2023-11-16 21:19:56.000000 wdb_utils-2.0.0/wdb_utils.egg-info/SOURCES.txt
--rw-r--r--   0 cwade      (503) staff       (20)        1 2023-11-16 21:19:56.000000 wdb_utils-2.0.0/wdb_utils.egg-info/dependency_links.txt
--rw-r--r--   0 cwade      (503) staff       (20)       38 2023-11-16 21:19:56.000000 wdb_utils-2.0.0/wdb_utils.egg-info/requires.txt
--rw-r--r--   0 cwade      (503) staff       (20)       10 2023-11-16 21:19:56.000000 wdb_utils-2.0.0/wdb_utils.egg-info/top_level.txt
+drwxr-xr-x   0 cwade      (503) staff       (20)        0 2024-04-30 17:37:28.540773 wdb_utils-2.1.0/
+-rw-r--r--   0 cwade      (503) staff       (20)      743 2024-04-30 17:37:28.540706 wdb_utils-2.1.0/PKG-INFO
+-rw-r--r--   0 cwade      (503) staff       (20)     1387 2023-11-16 21:33:53.000000 wdb_utils-2.1.0/README.md
+-rw-r--r--   0 cwade      (503) staff       (20)      582 2024-04-30 17:37:28.541103 wdb_utils-2.1.0/setup.cfg
+-rw-r--r--   0 cwade      (503) staff       (20)      645 2024-04-30 17:36:24.000000 wdb_utils-2.1.0/setup.py
+drwxr-xr-x   0 cwade      (503) staff       (20)        0 2024-04-30 17:37:28.539133 wdb_utils-2.1.0/wdb_utils/
+-rw-r--r--   0 cwade      (503) staff       (20)     6102 2024-04-30 17:02:39.000000 wdb_utils-2.1.0/wdb_utils/__init__.py
+drwxr-xr-x   0 cwade      (503) staff       (20)        0 2024-04-30 17:37:28.540439 wdb_utils-2.1.0/wdb_utils.egg-info/
+-rw-r--r--   0 cwade      (503) staff       (20)      743 2024-04-30 17:37:28.000000 wdb_utils-2.1.0/wdb_utils.egg-info/PKG-INFO
+-rw-------   0 cwade      (503) staff       (20)      214 2024-04-30 17:37:28.000000 wdb_utils-2.1.0/wdb_utils.egg-info/SOURCES.txt
+-rw-------   0 cwade      (503) staff       (20)        1 2024-04-30 17:37:28.000000 wdb_utils-2.1.0/wdb_utils.egg-info/dependency_links.txt
+-rw-------   0 cwade      (503) staff       (20)       38 2024-04-30 17:37:28.000000 wdb_utils-2.1.0/wdb_utils.egg-info/requires.txt
+-rw-------   0 cwade      (503) staff       (20)       10 2024-04-30 17:37:28.000000 wdb_utils-2.1.0/wdb_utils.egg-info/top_level.txt
```

### Comparing `wdb_utils-2.0.0/PKG-INFO` & `wdb_utils-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdb_utils
-Version: 2.0.0
+Version: 2.1.0
 Summary: Utilities for querying and loading data into an Oracle or Snowflake database. Queries return to pandas dataframes. Faster than SQLAlchemy.
 Home-page: https://github.com/cwade/wdb_utils
 Author: Courtney Wade
 Project-URL: repository, https://github.com/cwade/wdb_utils
 Keywords: pandas,oracle,query
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `wdb_utils-2.0.0/README.md` & `wdb_utils-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# db_utils
+# wdb_utils
 Utilities for querying an Oracle and/or Snowflake database. Planning to eventually expand to other database types.
 
 All the methods in this package require a yaml config file. For convenience, we assume this file is located in /Users/username/configs/config-default.yml.
 
 ### Installation
 
 ```
```

### Comparing `wdb_utils-2.0.0/setup.cfg` & `wdb_utils-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wdb_utils
-version = 2.0.0
+version = 2.1.0
 author = Courtney Wade
 description = Utilities for querying and loading data into an Oracle or Snowflake database. Queries return to pandas dataframes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cwade/wdb_utils
 project_urls = 
 	repository = https://github.com/cwade/wdb_utils
```

### Comparing `wdb_utils-2.0.0/setup.py` & `wdb_utils-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 setup(
     name='wdb_utils',
-    version='2.0.0',
+    version='2.1.0',
     author='Courtney Wade',
     description='Utilities for querying and loading data into an Oracle or Snowflake database. Queries return to pandas dataframes. Faster than SQLAlchemy.',
     long_description='Utilities for querying and loading data into an Oracle or Snowflake database. Eventually planning to add support for other database types',
     url='https://github.com/cwade/wdb_utils',
     keywords='pandas, oracle, query',
     python_requires='>=3.7, <4',
     install_requires=[
```

### Comparing `wdb_utils-2.0.0/wdb_utils/__init__.py` & `wdb_utils-2.1.0/wdb_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,31 @@
         try:
             yield connection
         except Exception as e:
             print('Error creating database connection: {}'.format(e))
 
     def run_query(self, query, arraysize=120000, fetch_ct=1000000):
         results = []
+        cols = None
         with self._connect() as connection:
             cursor = connection.cursor()
             cursor.arraysize = arraysize
             cursor.execute(query)
             while True:
                 rows = cursor.fetchmany(fetch_ct)
                 if not rows:
                     break
                 else:
                     results = results + rows
             cols = [n[0] for n in cursor.description]
-        return pd.DataFrame(results, columns=cols)
+
+        if cols is not None:
+            return pd.DataFrame(results, columns=cols)
+        else:
+            return
 
     def run_command(self, command):
         with self._connect() as connection:
             cursor = connection.cursor()
             try:
                 cursor.execute(command)
             except Exception as e:
@@ -65,15 +70,23 @@
         host = self.config['oracle']['host']
 
         if 'password' in self.config['oracle']:
             pwd = self.config['oracle']['password']
         else:
             pwd = getpass.getpass('Database password: ')
 
+        if 'mode' in self.config['oracle']:
+            mode = self.config['oracle']['mode']
+        else:
+            mode = 'thin'
+
         try:
+            if mode == 'thick':
+                self.oracledb.init_oracle_client()
+
             conn = self.oracledb.connect(user=user, password=pwd, dsn=host)
             return conn
         except Exception as e:
             print('Error creating Oracle connection: {}'.format(e))
             return None
 
     def load_dataframe(self, data, schema, tablename):
```

### Comparing `wdb_utils-2.0.0/wdb_utils.egg-info/PKG-INFO` & `wdb_utils-2.1.0/wdb_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wdb-utils
-Version: 2.0.0
+Name: wdb_utils
+Version: 2.1.0
 Summary: Utilities for querying and loading data into an Oracle or Snowflake database. Queries return to pandas dataframes. Faster than SQLAlchemy.
 Home-page: https://github.com/cwade/wdb_utils
 Author: Courtney Wade
 Project-URL: repository, https://github.com/cwade/wdb_utils
 Keywords: pandas,oracle,query
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

