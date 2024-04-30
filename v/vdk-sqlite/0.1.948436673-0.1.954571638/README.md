# Comparing `tmp/vdk-sqlite-0.1.948436673.tar.gz` & `tmp/vdk-sqlite-0.1.954571638.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-sqlite-0.1.948436673.tar", last modified: Fri Jul 28 09:43:53 2023, max compression
+gzip compressed data, was "vdk-sqlite-0.1.954571638.tar", last modified: Thu Aug  3 11:39:35 2023, max compression
```

## Comparing `vdk-sqlite-0.1.948436673.tar` & `vdk-sqlite-0.1.954571638.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-28 09:43:37.000000 vdk-sqlite-0.1.948436673/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.229933 vdk-sqlite-0.1.948436673/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.229933 vdk-sqlite-0.1.948436673/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.229933 vdk-sqlite-0.1.948436673/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.229933 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/
--rw-rw-rw-   0 root         (0) root         (0)    10113 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/ingest_to_sqlite.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      446 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5223 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/tests/test_sqlite_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 11:39:35.895702 vdk-sqlite-0.1.954571638/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-03 11:39:35.895702 vdk-sqlite-0.1.954571638/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-08-03 11:39:18.000000 vdk-sqlite-0.1.954571638/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 11:39:35.895702 vdk-sqlite-0.1.954571638/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-08-03 11:39:22.000000 vdk-sqlite-0.1.954571638/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 11:39:35.891702 vdk-sqlite-0.1.954571638/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 11:39:35.891702 vdk-sqlite-0.1.954571638/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 11:39:35.891702 vdk-sqlite-0.1.954571638/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 11:39:35.891702 vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/
+-rw-rw-rw-   0 root         (0) root         (0)    10368 2023-08-03 11:39:18.000000 vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/ingest_to_sqlite.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2023-08-03 11:39:18.000000 vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/sqlite_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-08-03 11:39:18.000000 vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/sqlite_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-08-03 11:39:18.000000 vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/sqlite_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 11:39:35.891702 vdk-sqlite-0.1.954571638/src/vdk_sqlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-03 11:39:35.000000 vdk-sqlite-0.1.954571638/src/vdk_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      446 2023-08-03 11:39:35.000000 vdk-sqlite-0.1.954571638/src/vdk_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 11:39:35.000000 vdk-sqlite-0.1.954571638/src/vdk_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-03 11:39:35.000000 vdk-sqlite-0.1.954571638/src/vdk_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-03 11:39:35.000000 vdk-sqlite-0.1.954571638/src/vdk_sqlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-03 11:39:35.000000 vdk-sqlite-0.1.954571638/src/vdk_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 11:39:35.891702 vdk-sqlite-0.1.954571638/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5225 2023-08-03 11:39:18.000000 vdk-sqlite-0.1.954571638/tests/test_sqlite_plugin.py
```

### Comparing `vdk-sqlite-0.1.948436673/README.md` & `vdk-sqlite-0.1.954571638/README.md`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.948436673/setup.py` & `vdk-sqlite-0.1.954571638/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.948436673"
+__version__ = "0.1.954571638"
 
 setuptools.setup(
     name="vdk-sqlite",
     version=__version__,
     install_requires=["vdk-core", "tabulate"],
     package_dir={"": "src"},
     packages=setuptools.find_namespace_packages(where="src"),
```

### Comparing `vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/ingest_to_sqlite.py` & `vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/ingest_to_sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,38 +85,21 @@
                 else:
                     self.__check_destination_table_exists(destination_table, cur)
                 self.__ingest_payload(destination_table, payload, cur)
 
     def __ingest_payload(
         self, destination_table: str, payload: List[dict], cur: Cursor
     ) -> None:
-        fields, query = self.__create_query(destination_table, cur)
-
-        for obj in payload:
+        values, query = self.__create_query(destination_table, payload, cur)
+        for obj in values:
             try:
                 cur.execute(query, obj)
                 log.debug("Payload was ingested.")
             except Exception as e:
-                if collections.Counter(fields) != collections.Counter(obj.keys()):
-                    errors.log_and_rethrow(
-                        errors.ResolvableBy.USER_ERROR,
-                        log,
-                        "Failed to sent payload",
-                        f"""
-                        One or more column names in the input data did NOT
-                        match corresponding column names in the database.
-                           Input Table Columns: {list(obj.keys())}
-                        Database Table Columns: {fields}
-                        """,
-                        "Will not be able to send the payload for ingestion",
-                        "See error message for help ",
-                        e,
-                        wrap_in_vdk_error=True,
-                    )
-                elif isinstance(e, ProgrammingError):
+                if isinstance(e, ProgrammingError):
                     errors.log_and_rethrow(
                         errors.ResolvableBy.USER_ERROR,
                         log,
                         "Failed to sent payload",
                         f"""
                         An issue with the SQL query occured. The error message
                         was: {str(e)}
@@ -165,26 +148,47 @@
         columns = []
         for row in cur.execute(
             f"select name, type from PRAGMA_TABLE_INFO('{destination_table}');"
         ):
             columns.append((row[0], row[1]))
         return columns
 
-    def __create_query(self, destination_table: str, cur: Cursor) -> Tuple[list, str]:
+    def __create_query(
+        self, destination_table: str, payload: List[dict], cur: Cursor
+    ) -> Tuple[list, str]:
         fields = [
             field_tuple[0]
             for field_tuple in cur.execute(
                 f"SELECT name FROM PRAGMA_TABLE_INFO('{destination_table}')"
             ).fetchall()
         ]
-        # the query fstring evaluates to 'INSERT INTO dest_table (val1, val2, val3) VALUES (:val1, :val2, :val3)'
-        # assuming dest_table is the destination_table and val1, val2, val3 are the fields of that table
-        query = f"INSERT INTO {destination_table} ({', '.join(fields)}) VALUES ({', '.join([':' + field for field in fields])})"
 
-        return fields, query
+        # verify that the payload header and table column names match
+        for obj in payload:
+            if collections.Counter(fields) != collections.Counter(obj.keys()):
+                errors.log_and_throw(
+                    errors.ResolvableBy.USER_ERROR,
+                    log,
+                    "Failed to sent payload",
+                    f"""
+                    One or more column names in the input data did NOT
+                    match corresponding column names in the database.
+                       Input Table Columns: {list(obj.keys())}
+                    Database Table Columns: {fields}
+                    """,
+                    "Will not be able to send the payload for ingestion",
+                    "See error message for help ",
+                )
+
+        # the query fstring evaluates to 'INSERT INTO dest_table (val1, val2, val3) VALUES (?, ?, ?)'
+        # assuming dest_table is the destination_table and val1, val2, val3 are the fields of that table
+        values = [[obj.get(field) for field in fields] for obj in payload]
+        fields = [field if " " not in field else f'"{field}"' for field in fields]
+        query = f"INSERT INTO {destination_table} ({', '.join(fields)}) VALUES ({', '.join(['?' for _ in fields])})"
+        return values, query
 
     def __create_table_if_not_exists(
         self, cur: Cursor, destination_table: str, payload: List[dict]
     ):
         columns = self.__table_columns(cur, destination_table)
         if not columns:
             log.info(
@@ -194,20 +198,24 @@
             columns = self.__infer_columns_from_payload(payload)
             self.__create_table(cur, destination_table, columns)
             log.info(f"Table {destination_table} created.")
 
     @staticmethod
     def __create_table(cur: Cursor, destination_table: str, columns: Dict[str, str]):
         """
-        Creates table from give list of columns and table name
+        Creates table from given list of columns and table name
         """
-        columns_as_sql_expression = ",".join(
-            [f"{col_name} {col_type}" for col_name, col_type in columns.items()]
-        )
-        sql = f"CREATE TABLE IF NOT EXISTS {destination_table} ( {columns_as_sql_expression} )"
+        names = [
+            f"{col_name} {col_type}"
+            if " " not in col_name
+            else f'"{col_name}" {col_type}'
+            for col_name, col_type in columns.items()
+        ]
+        columns_as_sql_expression = ",".join(names)
+        sql = f"CREATE TABLE IF NOT EXISTS {destination_table} ( {columns_as_sql_expression} );"
         log.debug(f"Create table using {sql}")
         cur.execute(sql)
 
     def __infer_columns_from_payload(self, payload: List[Dict]):
         """
         Infer the columns from payload. It will infer by getting all the keys from every row.
         So even if row have different number of keys it would find all the columns.
```

### Comparing `vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_configuration.py` & `vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/sqlite_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_connection.py` & `vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_plugin.py` & `vdk-sqlite-0.1.954571638/src/vdk/plugin/sqlite/sqlite_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.948436673/tests/test_sqlite_plugin.py` & `vdk-sqlite-0.1.954571638/tests/test_sqlite_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,36 +50,36 @@
     ):
         # create table first, as the ingestion fails otherwise
         runner = CliEntryBasedTestRunner(sqlite_plugin)
         runner.invoke(
             [
                 "sqlite-query",
                 "--query",
-                "CREATE TABLE test_table (some_data TEXT, more_data TEXT)",
+                r"CREATE TABLE test_table (some\ data TEXT, more_data TEXT)",
             ]
         )
 
         mock_sqlite_conf = mock.MagicMock(SQLiteConfiguration)
         sqlite_ingester = IngestToSQLite(mock_sqlite_conf)
-        payload = [{"some_data": "some_test_data", "more_data": "more_test_data"}]
+        payload = [{"some data": "some test data", "more_data": "more_test_data"}]
 
         sqlite_ingester.ingest_payload(
             payload=payload,
             destination_table="test_table",
             target=db_dir,
         )
 
         check_result = runner.invoke(
             ["sqlite-query", "--query", "SELECT * FROM test_table"]
         )
 
         assert check_result.stdout == (
-            "some_data       more_data\n"
+            "some data       more_data\n"
             "--------------  --------------\n"
-            "some_test_data  more_test_data\n"
+            "some test data  more_test_data\n"
         )
 
 
 def test_sqlite_ingestion_missing_dest_table(tmpdir):
     db_dir = str(tmpdir) + "vdk-sqlite.db"
     with mock.patch.dict(
         os.environ,
```

