# Comparing `tmp/pg_alchemy_kit-0.9.17b0.tar.gz` & `tmp/pg_alchemy_kit-0.9.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_alchemy_kit-0.9.17b0.tar", max compression
+gzip compressed data, was "pg_alchemy_kit-0.9.1b0.tar", max compression
```

## Comparing `pg_alchemy_kit-0.9.17b0.tar` & `pg_alchemy_kit-0.9.1b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685000 pg_alchemy_kit-0.9.17b0/README.md
--rw-r--r--   0        0        0     3361 2024-03-15 17:20:52.235395 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/PG.py
--rw-r--r--   0        0        0    12877 2024-04-08 02:01:27.341000 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/PGUtils.py
--rw-r--r--   0        0        0     6323 2024-03-15 17:21:48.231740 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/PGUtilsBase.py
--rw-r--r--   0        0        0     5512 2024-03-15 17:22:12.728679 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/PGUtilsORM.py
--rw-r--r--   0        0        0      353 2023-12-02 13:44:05.554117 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/__init__.py
--rw-r--r--   0        0        0     2780 2024-04-21 00:55:09.212000 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/AsyncPG.py
--rw-r--r--   0        0        0     9670 2024-04-30 15:03:47.140468 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py
--rw-r--r--   0        0        0      402 2024-03-05 23:13:28.466282 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__init__.py
--rw-r--r--   0        0        0     2548 2024-04-20 23:32:34.684000 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc
--rw-r--r--   0        0        0     4706 2024-04-21 00:55:25.414000 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc
--rw-r--r--   0        0        0     8382 2024-03-21 22:25:25.802875 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc
--rw-r--r--   0        0        0    10742 2024-04-20 23:32:34.686000 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc
--rw-r--r--   0        0        0    16328 2024-04-21 00:52:13.046000 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc
--rw-r--r--   0        0        0     4980 2024-02-23 22:12:09.581777 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc
--rw-r--r--   0        0        0     8275 2024-02-23 22:14:07.165516 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc
--rw-r--r--   0        0        0     5417 2024-02-23 22:16:34.786131 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc
--rw-r--r--   0        0        0      460 2024-03-05 23:14:18.543899 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      481 2024-04-20 23:34:09.319000 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5840 2023-11-01 14:19:01.447418 pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/cacheStrategies.py
--rw-r--r--   0        0        0      851 2024-04-30 15:05:45.844442 pg_alchemy_kit-0.9.17b0/pyproject.toml
--rw-r--r--   0        0        0     5927 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.9.17b0/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685000 pg_alchemy_kit-0.9.1b0/README.md
+-rw-r--r--   0        0        0     3361 2024-03-15 17:20:52.235000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PG.py
+-rw-r--r--   0        0        0    12877 2024-04-08 02:01:27.341432 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtils.py
+-rw-r--r--   0        0        0     6323 2024-03-15 17:21:48.231000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsBase.py
+-rw-r--r--   0        0        0     5512 2024-03-15 17:22:12.728000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsORM.py
+-rw-r--r--   0        0        0      353 2023-12-02 13:44:05.554000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/__init__.py
+-rw-r--r--   0        0        0     2780 2024-04-21 00:55:09.212262 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPG.py
+-rw-r--r--   0        0        0     9426 2024-04-21 00:49:46.175891 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py
+-rw-r--r--   0        0        0      402 2024-03-05 23:13:28.466000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__init__.py
+-rw-r--r--   0        0        0     2548 2024-04-20 23:32:34.684154 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc
+-rw-r--r--   0        0        0     4706 2024-04-21 00:55:25.414792 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc
+-rw-r--r--   0        0        0     8382 2024-03-21 22:25:25.802000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc
+-rw-r--r--   0        0        0    10742 2024-04-20 23:32:34.686799 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc
+-rw-r--r--   0        0        0    16328 2024-04-21 00:52:13.046852 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc
+-rw-r--r--   0        0        0     4980 2024-02-23 22:12:09.581000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc
+-rw-r--r--   0        0        0     8275 2024-02-23 22:14:07.165000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc
+-rw-r--r--   0        0        0     5417 2024-02-23 22:16:34.786000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc
+-rw-r--r--   0        0        0      460 2024-03-05 23:14:18.543000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      481 2024-04-20 23:34:09.319347 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5840 2023-11-01 14:19:01.447000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/cacheStrategies.py
+-rw-r--r--   0        0        0      851 2024-04-21 01:01:41.086173 pg_alchemy_kit-0.9.1b0/pyproject.toml
+-rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.9.1b0/PKG-INFO
```

### Comparing `pg_alchemy_kit-0.9.17b0/README.md` & `pg_alchemy_kit-0.9.1b0/README.md`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/PG.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PG.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/PGUtils.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtils.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/PGUtilsBase.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsBase.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/PGUtilsORM.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsORM.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/AsyncPG.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPG.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 from sqlalchemy import select, Select
 
-from typing import Any, TypeVar, Generic, TypedDict
+from typing import Any, TypeVar, Type, Generic, TypedDict
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy import TextClause, text
 import pandas as pd
 from sqlalchemy.orm.query import Query
 from sqlalchemy.dialects import postgresql
 
 
@@ -83,94 +83,94 @@
             return pd.DataFrame([])
 
         if to_camel_case:
             results = cls.__results_to_camel_case(results)
 
         return pd.DataFrame(results)
 
+    def __init__(self, single_transaction: bool = False, **kwargs):
+        self.single_transaction = single_transaction
+        self.snake_case = kwargs.get("snake_case", False)
+
     async def __execute_all(
-        self, session: AsyncSession, stmt: Select[T], **kwargs
+        self, session: AsyncSession, stmt: Select, **kwargs
     ) -> list[T]:
         result = await session.execute(stmt)
         return result.scalars().all()
 
-    async def select(self, session: AsyncSession, stmt: Select[T]) -> list[T]:
+    async def select(self, session: AsyncSession, stmt: Select) -> list[T]:
         try:
             results: list[T] = await self.__execute_all(session, stmt)
 
             if results is None:
                 return []
             return results
 
         except Exception as e:
             raise PGSelectError(str(e))
 
-    async def select_one(self, session: AsyncSession, stmt: Select[T]) -> T:
+    async def select_one(self, session: AsyncSession, stmt: Select) -> T:
         try:
             results: list[T] = await self.__execute_all(session, stmt)
 
             if results is None or len(results) != 1:
                 return {}
 
             result: T = results[0]
             return result
 
         except Exception as e:
             raise PGSelectError(str(e))
 
-    async def select_one_strict(
-        self, session: AsyncSession, stmt: Select[tuple[T]]
-    ) -> T:
+    async def select_one_strict(self, session: AsyncSession, stmt: Select) -> T:
         result = await session.execute(stmt)
-        result_one: T | None = result.scalars().one_or_none()
+        result: T | None = result.scalars().one()
 
-        if result_one is None:
+        if result is None:
             raise PGNotExistsError("No records found")
-        return result_one
+        return result
 
-    async def select_one_or_none(
-        self, session: AsyncSession, stmt: Select[tuple[T]]
-    ) -> T | None:
+    async def select_one_or_none(self, session: AsyncSession, stmt: Select) -> T:
         result = await session.execute(stmt)
-        result_one: T | None = result.scalars().one_or_none()
-        return result_one
+        result: T | None = result.scalars().one_or_none()
+        return result
 
-    async def check_exists(
-        self, session: AsyncSession, stmt: Select[T], **kwargs
-    ) -> bool:
+    async def check_exists(self, session: AsyncSession, stmt: Select, **kwargs) -> bool:
         try:
             results: list[T] = await self.__execute_all(session, stmt)
 
             if results is None:
                 return False
             return len(results) > 0
 
         except Exception as e:
             raise PGNotExistsError(str(e))
 
-    async def execute(self, session: AsyncSession, stmt: Select[T]) -> bool:
+    async def execute(self, session: AsyncSession, stmt: Select) -> bool:
         try:
             tmp = await session.execute(stmt)
             return tmp.fetchall()
         except Exception as e:
             raise PGSelectError(str(e))
 
     async def update(
         self,
         session: AsyncSession,
-        Model: Any,
-        filter_by: dict[str, Any],
-        values: dict[str, Any],
+        Model: T,
+        filter_by: dict,
+        values: dict,
+        **kwargs,
     ) -> T:
         try:
             obj = await self.select_one_strict(
                 session, select(Model).filter_by(**filter_by)
             )
+            to_snake_case = kwargs.get("to_snake_case", self.snake_case)
 
-            if self.snake_case:
+            if to_snake_case:
                 values = self.to_snake_case([values])[0]
 
             for key, value in values.items():
                 setattr(obj, key, value)
 
             if not self.single_transaction:
                 await session.commit()
@@ -180,15 +180,15 @@
             return obj
 
         except Exception as e:
             await session.rollback()
             raise PGUpdateError(str(e))
 
     async def insert(
-        self, session: AsyncSession, model: Any, record: dict[str, Any]
+        self, session: AsyncSession, model: Type[T], record: dict[str, Any]
     ) -> T:
         try:
             if self.snake_case:
                 record = self.to_snake_case([record])[0]
 
             obj = model(**record)
             session.add(obj)
@@ -197,26 +197,14 @@
             else:
                 await session.flush()
             return obj
         except Exception as e:
             await session.rollback()
             raise PGInsertError(str(e))
 
-    async def insert_dto(self, session: AsyncSession, model: T) -> T:
-        try:
-            session.add(model)
-            if not self.single_transaction:
-                await session.commit()
-            else:
-                await session.flush()
-            return model
-        except Exception as e:
-            await session.rollback()
-            raise PGInsertError(str(e))
-
     async def bulk_insert(
         self, session: AsyncSession, model: Any, records: list[dict], **kwargs
     ) -> bool:
         try:
             records_to_insert: list[dict] = [model(**record) for record in records]
 
             session.add_all(records_to_insert)
@@ -239,15 +227,15 @@
                 await session.commit()
             return True
         except Exception as e:
             await session.rollback()
             raise PGDeleteError(str(e))
 
     async def delete_by_id(
-        self, session: AsyncSession, model: Any, record_id: int | uuid.UUID
+        self, session: AsyncSession, model: T, record_id: int | uuid.UUID
     ) -> bool:
         try:
             stmt = select(model).where(model.id == record_id)
             record: T = await self.select_one_strict(session, stmt)
             return await self.delete(session, record)
         except Exception as e:
             raise PGDeleteError(str(e))
```

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pg_alchemy_kit/cacheStrategies.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/cacheStrategies.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.17b0/pyproject.toml` & `pg_alchemy_kit-0.9.1b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pg-alchemy-kit"
-version = "0.9.17-beta"
+version = "0.9.01-beta"
 description = "A simple wrapper around sqlalchemy to make it easier to use with postgresql"
 authors = ["jsaied99 <jsaied99@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jsaied99/pg-alchemy-kit"
 packages = [{ include = "pg_alchemy_kit" }]
 
 [tool.poetry.dependencies]
```

### Comparing `pg_alchemy_kit-0.9.17b0/PKG-INFO` & `pg_alchemy_kit-0.9.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-alchemy-kit
-Version: 0.9.17b0
+Version: 0.9.1b0
 Summary: A simple wrapper around sqlalchemy to make it easier to use with postgresql
 Home-page: https://github.com/jsaied99/pg-alchemy-kit
 Author: jsaied99
 Author-email: jsaied99@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

