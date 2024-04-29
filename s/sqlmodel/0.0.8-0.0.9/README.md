# Comparing `tmp/sqlmodel-0.0.8.tar.gz` & `tmp/sqlmodel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel-0.0.8.tar", max compression
+gzip compressed data, was "sqlmodel-0.0.9.tar", max compression
```

## Comparing `sqlmodel-0.0.8.tar` & `sqlmodel-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1086 2022-08-30 17:56:22.990756 sqlmodel-0.0.8/LICENSE
--rw-r--r--   0        0        0     8108 2022-08-30 17:56:22.990756 sqlmodel-0.0.8/README.md
--rw-r--r--   0        0        0     2758 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6505 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/__init__.py
--rw-r--r--   0        0        0      848 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/default.py
--rw-r--r--   0        0        0        0 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/engine/__init__.py
--rw-r--r--   0        0        0     6240 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/engine/create.py
--rw-r--r--   0        0        0     2477 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/engine/result.py
--rw-r--r--   0        0        0        0 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/ext/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/ext/asyncio/__init__.py
--rw-r--r--   0        0        0     2208 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/ext/asyncio/session.py
--rw-r--r--   0        0        0    25969 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/main.py
--rw-r--r--   0        0        0        0 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/orm/__init__.py
--rw-r--r--   0        0        0     4874 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/orm/session.py
--rw-r--r--   0        0        0       67 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/pool/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/py.typed
--rw-r--r--   0        0        0        0 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/sql/__init__.py
--rw-r--r--   0        0        0      170 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/sql/base.py
--rw-r--r--   0        0        0    10018 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/sql/expression.py
--rw-r--r--   0        0        0     2029 2022-08-30 17:56:23.034757 sqlmodel-0.0.8/sqlmodel/sql/sqltypes.py
--rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 sqlmodel-0.0.8/setup.py
--rw-r--r--   0        0        0     9723 1970-01-01 00:00:00.000000 sqlmodel-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-10-23 21:05:12.025669 sqlmodel-0.0.9/LICENSE
+-rw-r--r--   0        0        0     8082 2023-10-23 21:05:12.025669 sqlmodel-0.0.9/README.md
+-rw-r--r--   0        0        0     2592 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6466 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      850 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/default.py
+-rw-r--r--   0        0        0        0 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/engine/__init__.py
+-rw-r--r--   0        0        0     6240 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/engine/create.py
+-rw-r--r--   0        0        0     2477 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/engine/result.py
+-rw-r--r--   0        0        0        0 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/ext/asyncio/__init__.py
+-rw-r--r--   0        0        0     3357 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/ext/asyncio/session.py
+-rw-r--r--   0        0        0    26332 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/main.py
+-rw-r--r--   0        0        0        0 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/orm/__init__.py
+-rw-r--r--   0        0        0     4867 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/orm/session.py
+-rw-r--r--   0        0        0       67 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/pool/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/py.typed
+-rw-r--r--   0        0        0        0 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/sql/__init__.py
+-rw-r--r--   0        0        0      170 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/sql/base.py
+-rw-r--r--   0        0        0     9172 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/sql/expression.py
+-rw-r--r--   0        0        0     2028 2023-10-23 21:05:12.073670 sqlmodel-0.0.9/sqlmodel/sql/sqltypes.py
+-rw-r--r--   0        0        0     9542 1970-01-01 00:00:00.000000 sqlmodel-0.0.9/PKG-INFO
```

### Comparing `sqlmodel-0.0.8/LICENSE` & `sqlmodel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel-0.0.8/README.md` & `sqlmodel-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 <p align="center">
 <a href="https://github.com/tiangolo/sqlmodel/actions?query=workflow%3ATest" target="_blank">
     <img src="https://github.com/tiangolo/sqlmodel/workflows/Test/badge.svg" alt="Test">
 </a>
 <a href="https://github.com/tiangolo/sqlmodel/actions?query=workflow%3APublish" target="_blank">
     <img src="https://github.com/tiangolo/sqlmodel/workflows/Publish/badge.svg" alt="Publish">
 </a>
-<a href="https://codecov.io/gh/tiangolo/sqlmodel" target="_blank">
-    <img src="https://img.shields.io/codecov/c/github/tiangolo/sqlmodel?color=%2334D058" alt="Coverage">
-</a>
+<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/sqlmodel" target="_blank">
+    <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/sqlmodel.svg" alt="Coverage">
 <a href="https://pypi.org/project/sqlmodel" target="_blank">
     <img src="https://img.shields.io/pypi/v/sqlmodel?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 </p>
 
 ---
 
@@ -47,15 +46,15 @@
 
 It combines SQLAlchemy and Pydantic and tries to simplify the code you write as much as possible, allowing you to reduce the **code duplication to a minimum**, but while getting the **best developer experience** possible.
 
 **SQLModel** is, in fact, a thin layer on top of **Pydantic** and **SQLAlchemy**, carefully designed to be compatible with both.
 
 ## Requirements
 
-A recent and currently supported version of Python (right now, <a href="https://www.python.org/downloads/" class="external-link" target="_blank">Python supports versions 3.6 and above</a>).
+A recent and currently supported <a href="https://www.python.org/downloads/" class="external-link" target="_blank">version of Python</a>.
 
 As **SQLModel** is based on **Pydantic** and **SQLAlchemy**, it requires them. They will be automatically installed when you install SQLModel.
 
 ## Installation
 
 <div class="termy">
```

### Comparing `sqlmodel-0.0.8/sqlmodel/__init__.py` & `sqlmodel-0.0.9/sqlmodel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 # Re-export from SQLAlchemy
 from sqlalchemy.engine import create_mock_engine as create_mock_engine
 from sqlalchemy.engine import engine_from_config as engine_from_config
 from sqlalchemy.inspection import inspect as inspect
 from sqlalchemy.schema import BLANK_SCHEMA as BLANK_SCHEMA
+from sqlalchemy.schema import DDL as DDL
 from sqlalchemy.schema import CheckConstraint as CheckConstraint
 from sqlalchemy.schema import Column as Column
 from sqlalchemy.schema import ColumnDefault as ColumnDefault
 from sqlalchemy.schema import Computed as Computed
 from sqlalchemy.schema import Constraint as Constraint
-from sqlalchemy.schema import DDL as DDL
 from sqlalchemy.schema import DefaultClause as DefaultClause
 from sqlalchemy.schema import FetchedValue as FetchedValue
 from sqlalchemy.schema import ForeignKey as ForeignKey
 from sqlalchemy.schema import ForeignKeyConstraint as ForeignKeyConstraint
 from sqlalchemy.schema import Identity as Identity
 from sqlalchemy.schema import Index as Index
 from sqlalchemy.schema import MetaData as MetaData
 from sqlalchemy.schema import PrimaryKeyConstraint as PrimaryKeyConstraint
 from sqlalchemy.schema import Sequence as Sequence
 from sqlalchemy.schema import Table as Table
 from sqlalchemy.schema import ThreadLocalMetaData as ThreadLocalMetaData
 from sqlalchemy.schema import UniqueConstraint as UniqueConstraint
+from sqlalchemy.sql import LABEL_STYLE_DEFAULT as LABEL_STYLE_DEFAULT
+from sqlalchemy.sql import (
+    LABEL_STYLE_DISAMBIGUATE_ONLY as LABEL_STYLE_DISAMBIGUATE_ONLY,
+)
+from sqlalchemy.sql import LABEL_STYLE_NONE as LABEL_STYLE_NONE
+from sqlalchemy.sql import (
+    LABEL_STYLE_TABLENAME_PLUS_COL as LABEL_STYLE_TABLENAME_PLUS_COL,
+)
 from sqlalchemy.sql import alias as alias
 from sqlalchemy.sql import all_ as all_
 from sqlalchemy.sql import and_ as and_
 from sqlalchemy.sql import any_ as any_
 from sqlalchemy.sql import asc as asc
 from sqlalchemy.sql import between as between
 from sqlalchemy.sql import bindparam as bindparam
@@ -44,22 +52,14 @@
 from sqlalchemy.sql import false as false
 from sqlalchemy.sql import func as func
 from sqlalchemy.sql import funcfilter as funcfilter
 from sqlalchemy.sql import insert as insert
 from sqlalchemy.sql import intersect as intersect
 from sqlalchemy.sql import intersect_all as intersect_all
 from sqlalchemy.sql import join as join
-from sqlalchemy.sql import LABEL_STYLE_DEFAULT as LABEL_STYLE_DEFAULT
-from sqlalchemy.sql import (
-    LABEL_STYLE_DISAMBIGUATE_ONLY as LABEL_STYLE_DISAMBIGUATE_ONLY,
-)
-from sqlalchemy.sql import LABEL_STYLE_NONE as LABEL_STYLE_NONE
-from sqlalchemy.sql import (
-    LABEL_STYLE_TABLENAME_PLUS_COL as LABEL_STYLE_TABLENAME_PLUS_COL,
-)
 from sqlalchemy.sql import lambda_stmt as lambda_stmt
 from sqlalchemy.sql import lateral as lateral
 from sqlalchemy.sql import literal as literal
 from sqlalchemy.sql import literal_column as literal_column
 from sqlalchemy.sql import modifier as modifier
 from sqlalchemy.sql import not_ as not_
 from sqlalchemy.sql import null as null
@@ -81,59 +81,57 @@
 from sqlalchemy.sql import union as union
 from sqlalchemy.sql import union_all as union_all
 from sqlalchemy.sql import update as update
 from sqlalchemy.sql import values as values
 from sqlalchemy.sql import within_group as within_group
 from sqlalchemy.types import ARRAY as ARRAY
 from sqlalchemy.types import BIGINT as BIGINT
-from sqlalchemy.types import BigInteger as BigInteger
 from sqlalchemy.types import BINARY as BINARY
 from sqlalchemy.types import BLOB as BLOB
 from sqlalchemy.types import BOOLEAN as BOOLEAN
-from sqlalchemy.types import Boolean as Boolean
 from sqlalchemy.types import CHAR as CHAR
 from sqlalchemy.types import CLOB as CLOB
 from sqlalchemy.types import DATE as DATE
-from sqlalchemy.types import Date as Date
 from sqlalchemy.types import DATETIME as DATETIME
-from sqlalchemy.types import DateTime as DateTime
 from sqlalchemy.types import DECIMAL as DECIMAL
-from sqlalchemy.types import Enum as Enum
 from sqlalchemy.types import FLOAT as FLOAT
-from sqlalchemy.types import Float as Float
 from sqlalchemy.types import INT as INT
 from sqlalchemy.types import INTEGER as INTEGER
-from sqlalchemy.types import Integer as Integer
-from sqlalchemy.types import Interval as Interval
 from sqlalchemy.types import JSON as JSON
-from sqlalchemy.types import LargeBinary as LargeBinary
 from sqlalchemy.types import NCHAR as NCHAR
 from sqlalchemy.types import NUMERIC as NUMERIC
-from sqlalchemy.types import Numeric as Numeric
 from sqlalchemy.types import NVARCHAR as NVARCHAR
-from sqlalchemy.types import PickleType as PickleType
 from sqlalchemy.types import REAL as REAL
 from sqlalchemy.types import SMALLINT as SMALLINT
+from sqlalchemy.types import TEXT as TEXT
+from sqlalchemy.types import TIME as TIME
+from sqlalchemy.types import TIMESTAMP as TIMESTAMP
+from sqlalchemy.types import VARBINARY as VARBINARY
+from sqlalchemy.types import VARCHAR as VARCHAR
+from sqlalchemy.types import BigInteger as BigInteger
+from sqlalchemy.types import Boolean as Boolean
+from sqlalchemy.types import Date as Date
+from sqlalchemy.types import DateTime as DateTime
+from sqlalchemy.types import Enum as Enum
+from sqlalchemy.types import Float as Float
+from sqlalchemy.types import Integer as Integer
+from sqlalchemy.types import Interval as Interval
+from sqlalchemy.types import LargeBinary as LargeBinary
+from sqlalchemy.types import Numeric as Numeric
+from sqlalchemy.types import PickleType as PickleType
 from sqlalchemy.types import SmallInteger as SmallInteger
 from sqlalchemy.types import String as String
-from sqlalchemy.types import TEXT as TEXT
 from sqlalchemy.types import Text as Text
-from sqlalchemy.types import TIME as TIME
 from sqlalchemy.types import Time as Time
-from sqlalchemy.types import TIMESTAMP as TIMESTAMP
 from sqlalchemy.types import TypeDecorator as TypeDecorator
 from sqlalchemy.types import Unicode as Unicode
 from sqlalchemy.types import UnicodeText as UnicodeText
-from sqlalchemy.types import VARBINARY as VARBINARY
-from sqlalchemy.types import VARCHAR as VARCHAR
 
-# Extensions and modifications of SQLAlchemy in SQLModel
+# From SQLModel, modifications of SQLAlchemy or equivalents of Pydantic
 from .engine.create import create_engine as create_engine
+from .main import Field as Field
+from .main import Relationship as Relationship
+from .main import SQLModel as SQLModel
 from .orm.session import Session as Session
-from .sql.expression import select as select
 from .sql.expression import col as col
+from .sql.expression import select as select
 from .sql.sqltypes import AutoString as AutoString
-
-# Export SQLModel specifics (equivalent to Pydantic)
-from .main import SQLModel as SQLModel
-from .main import Field as Field
-from .main import Relationship as Relationship
```

### Comparing `sqlmodel-0.0.8/sqlmodel/default.py` & `sqlmodel-0.0.9/sqlmodel/default.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class _DefaultPlaceholder:
     """
     You shouldn't use this class directly.
 
     It's used internally to recognize when a default value has been overwritten, even
-    if the overriden default value was truthy.
+    if the overridden default value was truthy.
     """
 
     def __init__(self, value: Any):
         self.value = value
 
     def __bool__(self) -> bool:
         return bool(self.value)
@@ -23,10 +23,10 @@
 
 
 def Default(value: _TDefaultType) -> _TDefaultType:
     """
     You shouldn't use this function directly.
 
     It's used internally to recognize when a default value has been overwritten, even
-    if the overriden default value was truthy.
+    if the overridden default value was truthy.
     """
     return _DefaultPlaceholder(value)  # type: ignore
```

### Comparing `sqlmodel-0.0.8/sqlmodel/engine/create.py` & `sqlmodel-0.0.9/sqlmodel/engine/create.py`

 * *Files identical despite different names*

### Comparing `sqlmodel-0.0.8/sqlmodel/engine/result.py` & `sqlmodel-0.0.9/sqlmodel/engine/result.py`

 * *Files identical despite different names*

### Comparing `sqlmodel-0.0.8/sqlmodel/main.py` & `sqlmodel-0.0.9/sqlmodel/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,37 +7,47 @@
 from pathlib import Path
 from typing import (
     AbstractSet,
     Any,
     Callable,
     ClassVar,
     Dict,
+    ForwardRef,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 from pydantic import BaseConfig, BaseModel
 from pydantic.errors import ConfigError, DictError
-from pydantic.fields import SHAPE_SINGLETON
+from pydantic.fields import SHAPE_SINGLETON, ModelField, Undefined, UndefinedType
 from pydantic.fields import FieldInfo as PydanticFieldInfo
-from pydantic.fields import ModelField, Undefined, UndefinedType
 from pydantic.main import ModelMetaclass, validate_model
-from pydantic.typing import ForwardRef, NoArgAnyCallable, resolve_annotations
+from pydantic.typing import NoArgAnyCallable, resolve_annotations
 from pydantic.utils import ROOT_KEY, Representation
-from sqlalchemy import Boolean, Column, Date, DateTime
+from sqlalchemy import (
+    Boolean,
+    Column,
+    Date,
+    DateTime,
+    Float,
+    ForeignKey,
+    Integer,
+    Interval,
+    Numeric,
+    inspect,
+)
 from sqlalchemy import Enum as sa_Enum
-from sqlalchemy import Float, ForeignKey, Integer, Interval, Numeric, inspect
 from sqlalchemy.orm import RelationshipProperty, declared_attr, registry, relationship
 from sqlalchemy.orm.attributes import set_attribute
 from sqlalchemy.orm.decl_api import DeclarativeMeta
 from sqlalchemy.orm.instrumentation import is_instrumented
 from sqlalchemy.sql.schema import MetaData
 from sqlalchemy.sql.sqltypes import LargeBinary, Time
 
@@ -300,42 +310,39 @@
             new_cls.__config__.read_with_orm_mode = True
 
         config_registry = get_config("registry")
         if config_registry is not Undefined:
             config_registry = cast(registry, config_registry)
             # If it was passed by kwargs, ensure it's also set in config
             new_cls.__config__.registry = config_table
-            setattr(new_cls, "_sa_registry", config_registry)
-            setattr(new_cls, "metadata", config_registry.metadata)
-            setattr(new_cls, "__abstract__", True)
+            setattr(new_cls, "_sa_registry", config_registry)  # noqa: B010
+            setattr(new_cls, "metadata", config_registry.metadata)  # noqa: B010
+            setattr(new_cls, "__abstract__", True)  # noqa: B010
         return new_cls
 
     # Override SQLAlchemy, allow both SQLAlchemy and plain Pydantic models
     def __init__(
         cls, classname: str, bases: Tuple[type, ...], dict_: Dict[str, Any], **kw: Any
     ) -> None:
         # Only one of the base classes (or the current one) should be a table model
         # this allows FastAPI cloning a SQLModel for the response_model without
         # trying to create a new SQLAlchemy, for a new table, with the same name, that
         # triggers an error
         base_is_table = False
         for base in bases:
-            config = getattr(base, "__config__")
+            config = getattr(base, "__config__")  # noqa: B009
             if config and getattr(config, "table", False):
                 base_is_table = True
                 break
         if getattr(cls.__config__, "table", False) and not base_is_table:
-            dict_used = dict_.copy()
-            for field_name, field_value in cls.__fields__.items():
-                dict_used[field_name] = get_column_from_field(field_value)
             for rel_name, rel_info in cls.__sqlmodel_relationships__.items():
                 if rel_info.sa_relationship:
                     # There's a SQLAlchemy relationship declared, that takes precedence
                     # over anything else, use that and continue with the next attribute
-                    dict_used[rel_name] = rel_info.sa_relationship
+                    setattr(cls, rel_name, rel_info.sa_relationship)  # Fix #315
                     continue
                 ann = cls.__annotations__[rel_name]
                 temp_field = ModelField.infer(
                     name=rel_name,
                     value=rel_info,
                     annotation=ann,
                     class_validators=None,
@@ -345,93 +352,97 @@
                 if isinstance(temp_field.type_, ForwardRef):
                     relationship_to = temp_field.type_.__forward_arg__
                 rel_kwargs: Dict[str, Any] = {}
                 if rel_info.back_populates:
                     rel_kwargs["back_populates"] = rel_info.back_populates
                 if rel_info.link_model:
                     ins = inspect(rel_info.link_model)
-                    local_table = getattr(ins, "local_table")
+                    local_table = getattr(ins, "local_table")  # noqa: B009
                     if local_table is None:
                         raise RuntimeError(
                             "Couldn't find the secondary table for "
                             f"model {rel_info.link_model}"
                         )
                     rel_kwargs["secondary"] = local_table
                 rel_args: List[Any] = []
                 if rel_info.sa_relationship_args:
                     rel_args.extend(rel_info.sa_relationship_args)
                 if rel_info.sa_relationship_kwargs:
                     rel_kwargs.update(rel_info.sa_relationship_kwargs)
                 rel_value: RelationshipProperty = relationship(  # type: ignore
                     relationship_to, *rel_args, **rel_kwargs
                 )
-                dict_used[rel_name] = rel_value
                 setattr(cls, rel_name, rel_value)  # Fix #315
-            DeclarativeMeta.__init__(cls, classname, bases, dict_used, **kw)
+            # SQLAlchemy no longer uses dict_
+            # Ref: https://github.com/sqlalchemy/sqlalchemy/commit/428ea01f00a9cc7f85e435018565eb6da7af1b77
+            # Tag: 1.4.36
+            DeclarativeMeta.__init__(cls, classname, bases, dict_, **kw)
         else:
             ModelMetaclass.__init__(cls, classname, bases, dict_, **kw)
 
 
-def get_sqlachemy_type(field: ModelField) -> Any:
-    if issubclass(field.type_, str):
-        if field.field_info.max_length:
-            return AutoString(length=field.field_info.max_length)
-        return AutoString
-    if issubclass(field.type_, float):
-        return Float
-    if issubclass(field.type_, bool):
-        return Boolean
-    if issubclass(field.type_, int):
-        return Integer
-    if issubclass(field.type_, datetime):
-        return DateTime
-    if issubclass(field.type_, date):
-        return Date
-    if issubclass(field.type_, timedelta):
-        return Interval
-    if issubclass(field.type_, time):
-        return Time
-    if issubclass(field.type_, Enum):
-        return sa_Enum(field.type_)
-    if issubclass(field.type_, bytes):
-        return LargeBinary
-    if issubclass(field.type_, Decimal):
-        return Numeric(
-            precision=getattr(field.type_, "max_digits", None),
-            scale=getattr(field.type_, "decimal_places", None),
-        )
-    if issubclass(field.type_, ipaddress.IPv4Address):
-        return AutoString
-    if issubclass(field.type_, ipaddress.IPv4Network):
-        return AutoString
-    if issubclass(field.type_, ipaddress.IPv6Address):
-        return AutoString
-    if issubclass(field.type_, ipaddress.IPv6Network):
-        return AutoString
-    if issubclass(field.type_, Path):
-        return AutoString
-    if issubclass(field.type_, uuid.UUID):
-        return GUID
+def get_sqlalchemy_type(field: ModelField) -> Any:
+    if isinstance(field.type_, type) and field.shape == SHAPE_SINGLETON:
+        # Check enums first as an enum can also be a str, needed by Pydantic/FastAPI
+        if issubclass(field.type_, Enum):
+            return sa_Enum(field.type_)
+        if issubclass(field.type_, str):
+            if field.field_info.max_length:
+                return AutoString(length=field.field_info.max_length)
+            return AutoString
+        if issubclass(field.type_, float):
+            return Float
+        if issubclass(field.type_, bool):
+            return Boolean
+        if issubclass(field.type_, int):
+            return Integer
+        if issubclass(field.type_, datetime):
+            return DateTime
+        if issubclass(field.type_, date):
+            return Date
+        if issubclass(field.type_, timedelta):
+            return Interval
+        if issubclass(field.type_, time):
+            return Time
+        if issubclass(field.type_, bytes):
+            return LargeBinary
+        if issubclass(field.type_, Decimal):
+            return Numeric(
+                precision=getattr(field.type_, "max_digits", None),
+                scale=getattr(field.type_, "decimal_places", None),
+            )
+        if issubclass(field.type_, ipaddress.IPv4Address):
+            return AutoString
+        if issubclass(field.type_, ipaddress.IPv4Network):
+            return AutoString
+        if issubclass(field.type_, ipaddress.IPv6Address):
+            return AutoString
+        if issubclass(field.type_, ipaddress.IPv6Network):
+            return AutoString
+        if issubclass(field.type_, Path):
+            return AutoString
+        if issubclass(field.type_, uuid.UUID):
+            return GUID
     raise ValueError(f"The field {field.name} has no matching SQLAlchemy type")
 
 
 def get_column_from_field(field: ModelField) -> Column:  # type: ignore
     sa_column = getattr(field.field_info, "sa_column", Undefined)
     if isinstance(sa_column, Column):
         return sa_column
-    sa_type = get_sqlachemy_type(field)
+    sa_type = get_sqlalchemy_type(field)
     primary_key = getattr(field.field_info, "primary_key", False)
     index = getattr(field.field_info, "index", Undefined)
     if index is Undefined:
         index = False
     nullable = not primary_key and _is_field_noneable(field)
     # Override derived nullability if the nullable property is set explicitly
     # on the field
     if hasattr(field.field_info, "nullable"):
-        field_nullable = getattr(field.field_info, "nullable")
+        field_nullable = getattr(field.field_info, "nullable")  # noqa: B009
         if field_nullable != Undefined:
             nullable = field_nullable
     args = []
     foreign_key = getattr(field.field_info, "foreign_key", None)
     unique = getattr(field.field_info, "unique", False)
     if foreign_key:
         args.append(ForeignKey(foreign_key))
```

### Comparing `sqlmodel-0.0.8/sqlmodel/orm/session.py` & `sqlmodel-0.0.9/sqlmodel/orm/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Mapping, Optional, Sequence, Type, TypeVar, Union, overload
 
 from sqlalchemy import util
 from sqlalchemy.orm import Query as _Query
 from sqlalchemy.orm import Session as _Session
 from sqlalchemy.sql.base import Executable as _Executable
-from sqlmodel.sql.expression import Select, SelectOfScalar
 from typing_extensions import Literal
 
 from ..engine.result import Result, ScalarResult
 from ..sql.base import Executable
+from ..sql.expression import Select, SelectOfScalar
 
 _TSelectParam = TypeVar("_TSelectParam")
 
 
 class Session(_Session):
     @overload
     def exec(
```

### Comparing `sqlmodel-0.0.8/sqlmodel/sql/expression.py` & `sqlmodel-0.0.9/sqlmodel/sql/expression.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,42 @@
 # WARNING: do not modify this code, it is generated by expression.py.jinja2
 
-import sys
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     Generic,
     Mapping,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
-    cast,
     overload,
 )
 from uuid import UUID
 
 from sqlalchemy import Column
 from sqlalchemy.orm import InstrumentedAttribute
 from sqlalchemy.sql.elements import ColumnClause
 from sqlalchemy.sql.expression import Select as _Select
 
 _TSelect = TypeVar("_TSelect")
 
-# Workaround Generics incompatibility in Python 3.6
-# Ref: https://github.com/python/typing/issues/449#issuecomment-316061322
-if sys.version_info.minor >= 7:
-
-    class Select(_Select, Generic[_TSelect]):
-        inherit_cache = True
-
-    # This is not comparable to sqlalchemy.sql.selectable.ScalarSelect, that has a different
-    # purpose. This is the same as a normal SQLAlchemy Select class where there's only one
-    # entity, so the result will be converted to a scalar by default. This way writing
-    # for loops on the results will feel natural.
-    class SelectOfScalar(_Select, Generic[_TSelect]):
-        inherit_cache = True
-
-else:
-    from typing import GenericMeta  # type: ignore
-
-    class GenericSelectMeta(GenericMeta, _Select.__class__):  # type: ignore
-        pass
-
-    class _Py36Select(_Select, Generic[_TSelect], metaclass=GenericSelectMeta):
-        inherit_cache = True
-
-    class _Py36SelectOfScalar(_Select, Generic[_TSelect], metaclass=GenericSelectMeta):
-        inherit_cache = True
-
-    # Cast them for editors to work correctly, from several tricks tried, this works
-    # for both VS Code and PyCharm
-    Select = cast("Select", _Py36Select)  # type: ignore
-    SelectOfScalar = cast("SelectOfScalar", _Py36SelectOfScalar)  # type: ignore
+
+class Select(_Select, Generic[_TSelect]):
+    inherit_cache = True
+
+
+# This is not comparable to sqlalchemy.sql.selectable.ScalarSelect, that has a different
+# purpose. This is the same as a normal SQLAlchemy Select class where there's only one
+# entity, so the result will be converted to a scalar by default. This way writing
+# for loops on the results will feel natural.
+class SelectOfScalar(_Select, Generic[_TSelect]):
+    inherit_cache = True
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from ..main import SQLModel
 
 # Generated TypeVars start
```

### Comparing `sqlmodel-0.0.8/sqlmodel/sql/sqltypes.py` & `sqlmodel-0.0.9/sqlmodel/sql/sqltypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from sqlalchemy import CHAR, types
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.engine.interfaces import Dialect
 from sqlalchemy.sql.type_api import TypeEngine
 
 
 class AutoString(types.TypeDecorator):  # type: ignore
-
     impl = types.String
     cache_ok = True
     mysql_default_length = 255
 
     def load_dialect_impl(self, dialect: Dialect) -> "types.TypeEngine[Any]":
         impl = cast(types.String, self.impl)
         if impl.length is None and dialect.name == "mysql":
```

### Comparing `sqlmodel-0.0.8/PKG-INFO` & `sqlmodel-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: sqlmodel
-Version: 0.0.8
+Version: 0.0.9
 Summary: SQLModel, SQL databases in Python, designed for simplicity, compatibility, and robustness.
 Home-page: https://github.com/tiangolo/sqlmodel
 License: MIT
 Author: Sebastián Ramírez
 Author-email: tiangolo@gmail.com
-Requires-Python: >=3.6.1,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Typing :: Typed
-Requires-Dist: SQLAlchemy (>=1.4.17,<=1.4.41)
+Requires-Dist: SQLAlchemy (>=1.4.36,<2.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: sqlalchemy2-stubs
 Project-URL: Documentation, https://sqlmodel.tiangolo.com
 Project-URL: Repository, https://github.com/tiangolo/sqlmodel
 Description-Content-Type: text/markdown
 
 <p align="center">
@@ -45,17 +42,16 @@
 <p align="center">
 <a href="https://github.com/tiangolo/sqlmodel/actions?query=workflow%3ATest" target="_blank">
     <img src="https://github.com/tiangolo/sqlmodel/workflows/Test/badge.svg" alt="Test">
 </a>
 <a href="https://github.com/tiangolo/sqlmodel/actions?query=workflow%3APublish" target="_blank">
     <img src="https://github.com/tiangolo/sqlmodel/workflows/Publish/badge.svg" alt="Publish">
 </a>
-<a href="https://codecov.io/gh/tiangolo/sqlmodel" target="_blank">
-    <img src="https://img.shields.io/codecov/c/github/tiangolo/sqlmodel?color=%2334D058" alt="Coverage">
-</a>
+<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/sqlmodel" target="_blank">
+    <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/sqlmodel.svg" alt="Coverage">
 <a href="https://pypi.org/project/sqlmodel" target="_blank">
     <img src="https://img.shields.io/pypi/v/sqlmodel?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 </p>
 
 ---
 
@@ -85,15 +81,15 @@
 
 It combines SQLAlchemy and Pydantic and tries to simplify the code you write as much as possible, allowing you to reduce the **code duplication to a minimum**, but while getting the **best developer experience** possible.
 
 **SQLModel** is, in fact, a thin layer on top of **Pydantic** and **SQLAlchemy**, carefully designed to be compatible with both.
 
 ## Requirements
 
-A recent and currently supported version of Python (right now, <a href="https://www.python.org/downloads/" class="external-link" target="_blank">Python supports versions 3.6 and above</a>).
+A recent and currently supported <a href="https://www.python.org/downloads/" class="external-link" target="_blank">version of Python</a>.
 
 As **SQLModel** is based on **Pydantic** and **SQLAlchemy**, it requires them. They will be automatically installed when you install SQLModel.
 
 ## Installation
 
 <div class="termy">
```

