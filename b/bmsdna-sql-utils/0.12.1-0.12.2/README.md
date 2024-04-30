# Comparing `tmp/bmsdna_sql_utils-0.12.1.tar.gz` & `tmp/bmsdna_sql_utils-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_sql_utils-0.12.1.tar", max compression
+gzip compressed data, was "bmsdna_sql_utils-0.12.2.tar", max compression
```

## Comparing `bmsdna_sql_utils-0.12.1.tar` & `bmsdna_sql_utils-0.12.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      255 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/README.md
--rw-r--r--   0        0        0        0 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/__init__.py
--rw-r--r--   0        0        0      382 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/async_db_helper.py
--rw-r--r--   0        0        0     1169 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/case_preserving_set.py
--rw-r--r--   0        0        0     3529 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_helper.py
--rw-r--r--   0        0        0        0 2024-04-29 14:58:42.446423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/__init__.py
--rw-r--r--   0        0        0     2113 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/db_logging.py
--rw-r--r--   0        0        0     5382 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/delta_polars_source.py
--rw-r--r--   0        0        0     6060 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/delta_source.py
--rw-r--r--   0        0        0    26081 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/fill_table.py
--rw-r--r--   0        0        0     2116 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/json_insert.py
--rw-r--r--   0        0        0     5178 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/lake_source.py
--rw-r--r--   0        0        0     1754 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/meta_sql_store.py
--rw-r--r--   0        0        0     1481 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/odbc_insert.py
--rw-r--r--   0        0        0     1736 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/source.py
--rw-r--r--   0        0        0     3651 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/source_spark.py
--rw-r--r--   0        0        0      739 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/sql_utils.py
--rw-r--r--   0        0        0    15908 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/sqlschema.py
--rw-r--r--   0        0        0     1258 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/dbapi.py
--rw-r--r--   0        0        0     1332 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/integrity_check.py
--rw-r--r--   0        0        0      199 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/__init__.py
--rw-r--r--   0        0        0     2423 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/lake_meta.py
--rw-r--r--   0        0        0      822 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/type_fromarrow.py
--rw-r--r--   0        0        0      884 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/types.py
--rw-r--r--   0        0        0     5671 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/metadata/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/query.py
--rw-r--r--   0        0        0     2759 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/query_generation.py
--rw-r--r--   0        0        0     2619 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/result.py
--rw-r--r--   0        0        0     4026 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/server_info.py
--rw-r--r--   0        0        0     1078 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/sql_gen.py
--rw-r--r--   0        0        0     1774 2024-04-29 14:58:42.450423 bmsdna_sql_utils-0.12.1/pyproject.toml
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.1/PKG-INFO
+-rw-r--r--   0        0        0      255 2024-04-30 11:33:09.068932 bmsdna_sql_utils-0.12.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 11:33:09.068932 bmsdna_sql_utils-0.12.2/bmsdna/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/async_db_helper.py
+-rw-r--r--   0        0        0     1169 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/case_preserving_set.py
+-rw-r--r--   0        0        0     3529 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_helper.py
+-rw-r--r--   0        0        0        0 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/db_logging.py
+-rw-r--r--   0        0        0     5388 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/delta_polars_source.py
+-rw-r--r--   0        0        0     6066 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/delta_source.py
+-rw-r--r--   0        0        0    25911 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/fill_table.py
+-rw-r--r--   0        0        0     2116 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/json_insert.py
+-rw-r--r--   0        0        0     5178 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/lake_source.py
+-rw-r--r--   0        0        0     1754 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/meta_sql_store.py
+-rw-r--r--   0        0        0     1481 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/odbc_insert.py
+-rw-r--r--   0        0        0     1856 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/source.py
+-rw-r--r--   0        0        0     3900 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/source_spark.py
+-rw-r--r--   0        0        0      739 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/sql_utils.py
+-rw-r--r--   0        0        0    16306 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/sqlschema.py
+-rw-r--r--   0        0        0     1132 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/dbapi.py
+-rw-r--r--   0        0        0     1332 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/integrity_check.py
+-rw-r--r--   0        0        0      199 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/__init__.py
+-rw-r--r--   0        0        0     2423 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/lake_meta.py
+-rw-r--r--   0        0        0      822 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/type_fromarrow.py
+-rw-r--r--   0        0        0      884 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/types.py
+-rw-r--r--   0        0        0     5671 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/metadata/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/query.py
+-rw-r--r--   0        0        0     2759 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/query_generation.py
+-rw-r--r--   0        0        0     2619 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/result.py
+-rw-r--r--   0        0        0     4026 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/server_info.py
+-rw-r--r--   0        0        0     1078 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/sql_gen.py
+-rw-r--r--   0        0        0     1805 2024-04-30 11:33:09.072932 bmsdna_sql_utils-0.12.2/pyproject.toml
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.2/PKG-INFO
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/async_db_helper.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/async_db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/case_preserving_set.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/case_preserving_set.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_helper.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/db_logging.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/db_logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         ],
         conn,
         overwrite=False,
         primary_keys=[],
     )
 
 
+warned_logging = False
+
+
 def insert_into_log(
     con: "pyodbc.Connection|pytds.Connection",
     table_name: Union[str, tuple[str, str]],
     type: Literal["start_load", "end_load", "error", "schema_drift", "start_merge", "start_full", "skip_load"],
     *,
     partition_filter: Optional[str] = None,
     error: Optional[str] = None,
@@ -40,13 +43,19 @@
     table_name_str = table_name if isinstance(table_name, str) else table_name[0] + "." + table_name[1]
     if sql and len(sql) > 4000:
         sql = sql[0:3999]
     if error:
         logger.error(f"{type} for {table_name}, {partition_filter}:\n {error}")
     else:
         logger.info(f"{type} for {table_name}, {partition_filter}")
-    with con.cursor() as cur:
-        cur.execute(
-            """INSERT INTO lake_import._log(table_name, type, insert_date, partition_filter, error, sql)
-                VALUES(?,?,GETUTCDATE(),?,?,?)""",
-            (table_name_str, type, partition_filter, error, sql),
-        )
+    try:
+        with con.cursor() as cur:
+            cur.execute(
+                """INSERT INTO lake_import._log("table_name", type, insert_date, partition_filter, error, sql)
+                    VALUES(?,?,GETUTCDATE(),?,?,?)""",
+                (table_name_str, type, partition_filter, error, sql),
+            )
+    except Exception as err:
+        global warned_logging
+        if not warned_logging:
+            warned_logging = True
+            logger.warning("Could not log to table", exc_info=err)
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/delta_polars_source.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/delta_polars_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         import polars as pl
 
         schema = self.delta_lake.schema().to_pyarrow()
         sql_lens = []
         length_fields: list[str] = []
         fields: dict[str, SQLField] = dict()
         for fieldname in schema.names:
-            if fieldname.startswith("__"):
+            if fieldname in self.forbidden_cols:
                 continue
             f = schema.field(fieldname)
             t = f.type
             is_complex = (
                 pa.types.is_list(t)
                 or pa.types.is_large_list(t)
                 or pa.types.is_fixed_size_list(t)
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/delta_source.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/delta_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         import duckdb
 
         schema = self.delta_lake.schema().to_pyarrow()
         sql_lens = []
         length_fields: list[str] = []
         fields: dict[str, SQLField] = dict()
         for fieldname in schema.names:
-            if fieldname.startswith("__"):
+            if fieldname in self.forbidden_cols:
                 continue
             f = schema.field(fieldname)
             t = f.type
             is_complex = (
                 pa.types.is_list(t)
                 or pa.types.is_large_list(t)
                 or pa.types.is_fixed_size_list(t)
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/fill_table.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/fill_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,17 +541,15 @@
                     + ", ".join(_get_select(c, constant_values, calculated_columns) for c in all_cols)
                     + " FROM "
                     + sql_quote_name(target_table_part)
                 )
                 select = select or [
                     f.column_name
                     for f in schema
-                    if not f.column_name.startswith("__")
-                    and f.column_name not in constant_values.keys()
-                    and f.column_name not in calculated_columns.keys()
+                    if f.column_name not in constant_values.keys() and f.column_name not in calculated_columns.keys()
                 ]
                 table_sql.append(sql)
             prom = insert_into_table_partition(
                 target_table=target_table_part,
                 source=source,
                 connection=connection_string,
                 skip_create_table=not first and not table_per_partition,
@@ -593,19 +591,15 @@
 
             with pyodbc.connect(connstr_odbc) as conn:
                 conn.execute(view)
 
     else:
         constant_values = source.get_constant_values(None, select=select)
 
-        select = select or [
-            f.column_name
-            for f in schema
-            if not f.column_name.startswith("__") and f.column_name not in constant_values.keys()
-        ]
+        select = select or [f.column_name for f in schema if f.column_name not in constant_values.keys()]
         await insert_into_table_partition(
             target_table=target_table,
             source=source,
             connection=connection_string,
             partition_filter=None,
             schema=schema,
             primary_keys=primary_keys,
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/json_insert.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/json_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/lake_source.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/lake_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/meta_sql_store.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/meta_sql_store.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/odbc_insert.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/odbc_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/source.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 
 @dataclass(frozen=True)
 class WriteInfo:
     column_names: list[str]
     table_name: str | tuple[str, str]
 
 
+forbidden_cols = ["__hash", "__metadata"]
+
+
 class ImportSource(ABC):
+    def __init__(self):
+        self.forbidden_cols = forbidden_cols
+
     @abstractmethod
     async def write_to_sql_server(
         self,
         target_table: str | tuple[str, str],
         connection_string: str | dict,
         partition_filters: dict | None,
         select: list[str] | None = None,
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/source_spark.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/source_spark.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,22 @@
             return [
                 r.asDict(True) for r in self.df.selectExpr("_partition").orderBy("_partition").distinct().collect()
             ]
         return []
 
     def get_schema(self) -> list[SQLField]:
         fields = self.df.schema.fields
-        return [SQLField(f.name, ex.DataType.build(str(f.dataType.simpleString()), dialect="spark")) for f in fields]
+
+        def sqlglot_type(dtype):
+            simple_str = str(dtype.simpleString())
+            if simple_str == "timestamp_ntz":
+                return ex.DataType.build("datetime2", dialect="tsql")  # more or less
+            return ex.DataType.build(simple_str, dialect="spark")
+
+        return [SQLField(f.name, sqlglot_type(f.dataType)) for f in fields]
 
     def get_last_change_date(self):
         if self.change_date:
             return self.change_date
         col_names = [f.column_name for f in self.get_schema()]
         if "__timestamp" in col_names:
             return self.df.selectExpr("max(__timestamp) as max_ts").collect()[0][0]
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/sql_utils.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/sql_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/db_io/sqlschema.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/db_io/sqlschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     import pytds
 logger = logging.getLogger(__name__)
 
 table_name_type = Union[str, tuple[str, str]]
 
 
 def convert_to_sql_field(field: FieldWithType):
-
     sqt = get_sql_type(field["type"]["type_str"], field.get("max_str_length", None))
     return SQLField(field["name"], ex.DataType.build(sqt, dialect="tsql"))
 
 
 def with_max_str_length(t: ex.DataType, max_str_length: int) -> ex.DataType:
     sql_str = t.sql("tsql")
     if "(" in sql_str:
@@ -29,20 +28,24 @@
 
 def get_str_length(field: SQLField | ex.DataType):
     if isinstance(field, SQLField):
         return get_str_length(field.data_type)
     if len(field.expressions) != 1:
         return None
     t_zero = field.expressions[0]
-    if not isinstance(t_zero, int):
+    if not isinstance(t_zero, (float, int, str)):
+        t_zero = t_zero.this
+    if not isinstance(t_zero, (float, int, str)):
         t_zero = t_zero.this
-    if not isinstance(t_zero, int):
+    if not isinstance(t_zero, (float, int, str)):
         t_zero = t_zero.this
-    assert isinstance(t_zero, int)
-    return t_zero
+    assert isinstance(t_zero, (float, int, str)), f"cannot get string length from {str(field)}. AST: {repr(field)}"
+    if isinstance(t_zero, str) and t_zero.upper() == "MAX":
+        return -1
+    return int(t_zero)
 
 
 def get_field_col_definition(
     field: FieldWithType | SQLField, nullable=True, default: str | None = None, formula: str | None = None
 ) -> str:
     if not isinstance(field, SQLField):
         field = convert_to_sql_field(field)
@@ -190,14 +193,15 @@
     if primary_keys and len(primary_keys) > 0:
         pkcols = ", ".join((sql_quote_name(n) for n in primary_keys))
         tbl_name_pk = (
             table_name.removeprefix("##") if isinstance(table_name, str) else table_name[0] + "_" + table_name[1]
         )
         pkdef = f", CONSTRAINT {sql_quote_name('PK_'+tbl_name_pk)}  PRIMARY KEY({pkcols})"
     create_sql = f"CREATE TABLE {sql_quote_name(table_name)}({cols}{pkdef}) "
+
     if with_exist_check:
         return f"""
             IF OBJECT_ID (N'{sql_quote_name(table_name).replace("'", "''")}', N'U') IS NULL 
             BEGIN
                 {create_sql}
                 select 'created' as action
             END
@@ -247,14 +251,16 @@
     conn: "pyodbc.Connection | pytds.Connection",
     primary_keys: list[str] | None,
     overwrite: bool,
     default_values: Mapping[str, tuple[SQLField, Any]] | None = None,
     calculated_values: Mapping[str, str] | None = None,
     callback: list[Callable[[CreateTableCallbackParams], Any]] | None = None,
 ):
+    if not any(schema):
+        raise ValueError("Must provide at least one column")
     created = False
     truncated = False
     adjusted = False
     if overwrite:
         with conn.cursor() as cur:
             sql = f"DROP TABLE IF EXISTS {sql_quote_name(table_name)}"
             logger.info(f"Executing sql: {sql}")
@@ -343,14 +349,15 @@
                             cur.execute(td)
                 else:
                     sql = ";\r\n".join(todos)
                     with conn.cursor() as cur:
                         logger.info(f"Executing alter sql: {sql}")
                         from .db_logging import insert_into_log
 
+                        print(sql)
                         insert_into_log(conn, table_name, "schema_drift", sql=sql)
                         cur.execute(sql)
 
     with conn.cursor() as cur:
         sql = get_sql_for_schema(
             table_name,
             schema,
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/dbapi.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/dbapi.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,53 +6,39 @@
 
 
 class Cursor(Protocol):
     description: Sequence | None
     rowcount: int
     arraysize: int
 
-    def nextset(self) -> bool:
-        ...
+    def nextset(self) -> bool: ...
 
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
-    def execute(self, operation: Any, *args, **kwargs):
-        ...
+    def execute(self, operation: Any, *args, **kwargs): ...
 
-    def executemany(self, operation: Any, seq_of_parameters: Sequence | Mapping, *args, **kwargs):
-        ...
+    def executemany(self, operation: Any, seq_of_parameters: Sequence | Mapping, *args, **kwargs): ...
 
-    def fetchone(self) -> Sequence | None:
-        ...
+    def fetchone(self) -> Sequence | None: ...
 
-    def fetchmany(self, size: int = 0) -> Sequence[Sequence]:
-        ...
+    def fetchmany(self, size: int = 0) -> Sequence[Sequence]: ...
 
-    def fetchall(self, size: int = 0) -> Sequence[Sequence]:
-        ...
+    def fetchall(self, size: int = 0) -> Sequence[Sequence]: ...
 
-    def setinputsizes(self, sizes: Sequence):
-        ...
+    def setinputsizes(self, sizes: Sequence): ...
 
-    def setoutputsize(self, size: Any, column: int | None = None):
-        ...
+    def setoutputsize(self, size: Any, column: int | None = None): ...
 
-    def __enter__(self) -> "Cursor":
-        ...
+    def __enter__(self) -> "Cursor": ...
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        ...
+    def __exit__(self, exc_type, exc_val, exc_tb): ...
 
 
 class ConnectionT(Protocol):
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
-    def commit(self) -> None:
-        ...
+    def commit(self) -> None: ...
 
-    def cursor(self, *args, **kwargs) -> Cursor:
-        ...
+    def cursor(self, *args, **kwargs) -> Cursor: ...
 
 
 Connection: TypeAlias = "ConnectionT | pyodbc.Connection"
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/integrity_check.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/integrity_check.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/lake_meta.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/lake_meta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/type_fromarrow.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/type_fromarrow.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/lake/types.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/lake/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/metadata/__init__.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/query.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,26 +81,23 @@
         return "1" if vl else "0"
     if isinstance(vl, datetime):
         return "'" + vl.isoformat() + "'"
     return "'" + str(vl).replace("'", "''") + "'"
 
 
 @overload
-def get_compatible_name(name: str) -> str:
-    ...
+def get_compatible_name(name: str) -> str: ...
 
 
 @overload
-def get_compatible_name(name: tuple[str, str]) -> tuple[str, str]:
-    ...
+def get_compatible_name(name: tuple[str, str]) -> tuple[str, str]: ...
 
 
 @overload
-def get_compatible_name(name: tuple[str, str, str]) -> tuple[str, str, str]:
-    ...
+def get_compatible_name(name: tuple[str, str, str]) -> tuple[str, str, str]: ...
 
 
 def get_compatible_name(name: SQLObjectNameType) -> SQLObjectNameType:
     if isinstance(name, str):
         first_char = name[0]
         if not (
             (ord(first_char) >= ord("a") and ord(first_char) <= ord("z"))
```

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/query_generation.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/query_generation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/result.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/result.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/server_info.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/server_info.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/bmsdna/sql_utils/sql_gen.py` & `bmsdna_sql_utils-0.12.2/bmsdna/sql_utils/sql_gen.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.12.1/pyproject.toml` & `bmsdna_sql_utils-0.12.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-sql-utils"
-version = "0.12.1"
+version = "0.12.2"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 readme = "README.md"
 packages = [{ include = "bmsdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -20,35 +20,38 @@
 python-dateutil = { version = "^2.8.2", python = "<3.11" }
 arrow-odbc = { version = "^5.0.0", optional = true }
 deltalake2db = ">=0.3.0"
 polars = { version = ">=0.20.21", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.325"
-black = "^23.7.0"
 pyodbc = { version = ">=4.0.0" }
 aioodbc = { version = "^0.5.0" }
 python-tds = { version = "^1.13.0" }
 pydantic = ">=1.10.0"
-isort = "^5.12.0"
-pycln = "^2.4.0"
 sqlglot = ">=20.0.0"
 pyspark = "^3.5.1"
+pandas = "^2.2.2"
+delta-spark = "^3.1.0"
+ruff = "^0.4.2"
 
 
 [tool.poetry.group.test.dependencies]
 pytest-asyncio = "^0.23.5"
 pytest = "^7.4.3"
 pytest-order = "^1.2.0"
 docker = "^7.0.0"
 pytest-cov = "^5.0.0"
 azure-identity = "^1.16.0"
 azure-storage-blob = "^12.19.1"
 python-dotenv = "^1.0.1"
 
+[pytest]
+log_cli = true
+
 [tool.poetry.extras]
 db-io = ["pyodbc", "lakeapi2sql"]
 delta = ["duckdb", "deltalake"]
 db2delta = ["duckdb", "deltalake", "arrow-odbc"]
 polars = ["polars"]
 
 [build-system]
@@ -58,9 +61,9 @@
 
 [tool.pyright]
 venv = ".venv"
 venvPath = "."
 pythonVersion = "3.10"
 typeCheckingMode = "basic"
 
-[tool.black]
+[tool.ruff]
 line-length = 119
```

### Comparing `bmsdna_sql_utils-0.12.1/PKG-INFO` & `bmsdna_sql_utils-0.12.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-sql-utils
-Version: 0.12.1
+Version: 0.12.2
 Summary: 
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

