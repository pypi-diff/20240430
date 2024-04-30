# Comparing `tmp/typedmongo-1.1.2.tar.gz` & `tmp/typedmongo-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.1.2.tar", last modified: Mon Apr 29 16:31:30 2024, max compression
+gzip compressed data, was "typedmongo-1.1.3.tar", last modified: Tue Apr 30 01:52:25 2024, max compression
```

## Comparing `typedmongo-1.1.2.tar` & `typedmongo-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-29 16:31:17.549654 typedmongo-1.1.2/LICENSE
--rw-r--r--   0        0        0      108 2024-04-29 16:31:17.549654 typedmongo-1.1.2/README.md
--rw-r--r--   0        0        0     1441 2024-04-29 16:31:30.613791 typedmongo-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5789 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     3745 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/sync.py
--rw-r--r--   0        0        0     5549 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/test_marshamallow.py
--rw-r--r--   0        0        0     3737 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/test_table.py
--rw-r--r--   0        0        0      781 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/__init__.py
--rw-r--r--   0        0        0      781 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    11612 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     9494 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     8825 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    11394 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/expressions.py
--rw-r--r--   0        0        0     9494 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/fields.py
--rw-r--r--   0        0        0      538 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/sync.py
--rw-r--r--   0        0        0     8712 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/table.py
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 01:52:12.593251 typedmongo-1.1.3/LICENSE
+-rw-r--r--   0        0        0      108 2024-04-30 01:52:12.593251 typedmongo-1.1.3/README.md
+-rw-r--r--   0        0        0     1441 2024-04-30 01:52:25.685305 typedmongo-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5789 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     4233 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/sync.py
+-rw-r--r--   0        0        0     5549 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     4225 2024-04-30 01:52:12.593251 typedmongo-1.1.3/tests/test_table.py
+-rw-r--r--   0        0        0      781 2024-04-30 01:52:12.593251 typedmongo-1.1.3/typedmongo/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-30 01:52:12.593251 typedmongo-1.1.3/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    11612 2024-04-30 01:52:12.593251 typedmongo-1.1.3/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     9521 2024-04-30 01:52:12.593251 typedmongo-1.1.3/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     8825 2024-04-30 01:52:12.597251 typedmongo-1.1.3/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    11394 2024-04-30 01:52:12.597251 typedmongo-1.1.3/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-04-30 01:52:12.597251 typedmongo-1.1.3/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-04-30 01:52:12.597251 typedmongo-1.1.3/typedmongo/expressions.py
+-rw-r--r--   0        0        0     9521 2024-04-30 01:52:12.597251 typedmongo-1.1.3/typedmongo/fields.py
+-rw-r--r--   0        0        0      849 2024-04-30 01:52:12.597251 typedmongo-1.1.3/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-04-30 01:52:12.597251 typedmongo-1.1.3/typedmongo/sync.py
+-rw-r--r--   0        0        0     8825 2024-04-30 01:52:12.597251 typedmongo-1.1.3/typedmongo/table.py
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.1.3/PKG-INFO
```

### Comparing `typedmongo-1.1.2/LICENSE` & `typedmongo-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/pyproject.toml` & `typedmongo-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.1.2"
+version = "1.1.3"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.1.2/tests/asyncio/test_client.py` & `typedmongo-1.1.3/tests/asyncio/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/tests/asyncio/test_table.py` & `typedmongo-1.1.3/tests/asyncio/test_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import datetime
 import uuid
 
 import pytest
 
 import typedmongo.asyncio as mongo
 from typedmongo.expressions import Expression
 
@@ -19,14 +20,17 @@
 
 
 class User(MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
+    created_at: mongo.DateTimeField = mongo.DateTimeField(
+        default=lambda: datetime.datetime.now(datetime.timezone.utc)
+    )
     children: mongo.ListField[User]
     extra: mongo.DictField = mongo.DictField(default=dict)
 
 
 User.__lazy_init_fields__()
 
 
@@ -79,32 +83,35 @@
             "age": 18,
             "tags": ["a", "b"],
             "wallet": {"balance": 100},
             "children": [],
         }
     )
     assert isinstance(user._id, str)
+    assert isinstance(user.created_at, datetime.datetime)
 
     user = User.load(
         {
             "name": "Aber",
             "age": 18,
             "tags": ["a", "b"],
             "wallet": {"balance": 100},
             "children": [],
         },
         partial=True,
     )
     assert isinstance(user._id, str)
+    assert isinstance(user.created_at, datetime.datetime)
 
     user = User(
         name="Aber", age=18, tags=["a", "b"], wallet=Wallet(balance=100), children=[]
     )
     assert hasattr(user, "_id")
     assert isinstance(user.dump(user)["_id"], str)
+    assert isinstance(user.created_at, datetime.datetime)
 
 
 def test_recursion_field():
     user = User.load(
         {
             "name": "Aber",
             "age": 18,
@@ -143,7 +150,12 @@
             "wallet": {"balance": 100},
             "children": [],
             "extra": {"a": "b"},
         }
     )
     assert user.extra == {"a": "b"}
     assert user.dump(user)["extra"] == {"a": "b"}
+
+
+def test_datetime_field():
+    user = User.load(dict(created_at=datetime.datetime.now()), partial=True)
+    assert isinstance(user.created_at, datetime.datetime)
```

### Comparing `typedmongo-1.1.2/tests/sync.py` & `typedmongo-1.1.3/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/tests/test_client.py` & `typedmongo-1.1.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/tests/test_expressions.py` & `typedmongo-1.1.3/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/tests/test_marshamallow.py` & `typedmongo-1.1.3/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/tests/test_table.py` & `typedmongo-1.1.3/tests/test_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import datetime
 import uuid
 
 import pytest
 
 import typedmongo as mongo
 from typedmongo.expressions import Expression
 
@@ -19,14 +20,17 @@
 
 
 class User(MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
+    created_at: mongo.DateTimeField = mongo.DateTimeField(
+        default=lambda: datetime.datetime.now(datetime.timezone.utc)
+    )
     children: mongo.ListField[User]
     extra: mongo.DictField = mongo.DictField(default=dict)
 
 
 User.__lazy_init_fields__()
 
 
@@ -79,32 +83,35 @@
             "age": 18,
             "tags": ["a", "b"],
             "wallet": {"balance": 100},
             "children": [],
         }
     )
     assert isinstance(user._id, str)
+    assert isinstance(user.created_at, datetime.datetime)
 
     user = User.load(
         {
             "name": "Aber",
             "age": 18,
             "tags": ["a", "b"],
             "wallet": {"balance": 100},
             "children": [],
         },
         partial=True,
     )
     assert isinstance(user._id, str)
+    assert isinstance(user.created_at, datetime.datetime)
 
     user = User(
         name="Aber", age=18, tags=["a", "b"], wallet=Wallet(balance=100), children=[]
     )
     assert hasattr(user, "_id")
     assert isinstance(user.dump(user)["_id"], str)
+    assert isinstance(user.created_at, datetime.datetime)
 
 
 def test_recursion_field():
     user = User.load(
         {
             "name": "Aber",
             "age": 18,
@@ -143,7 +150,12 @@
             "wallet": {"balance": 100},
             "children": [],
             "extra": {"a": "b"},
         }
     )
     assert user.extra == {"a": "b"}
     assert user.dump(user)["extra"] == {"a": "b"}
+
+
+def test_datetime_field():
+    user = User.load(dict(created_at=datetime.datetime.now()), partial=True)
+    assert isinstance(user.created_at, datetime.datetime)
```

### Comparing `typedmongo-1.1.2/typedmongo/__init__.py` & `typedmongo-1.1.3/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/typedmongo/asyncio/__init__.py` & `typedmongo-1.1.3/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/typedmongo/asyncio/client.py` & `typedmongo-1.1.3/typedmongo/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/typedmongo/asyncio/fields.py` & `typedmongo-1.1.3/typedmongo/asyncio/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 
 from bson import ObjectId
 from marshmallow import fields
 from typing_extensions import Self
 
 from typedmongo.expressions import CompareMixin, HasFieldName, OrderByMixin
-from typedmongo.marshamallow import MarshamallowObjectId
+from typedmongo.marshamallow import MarshamallowDateTime, MarshamallowObjectId
 
 if TYPE_CHECKING:
     from .table import Table
 
 TypeTable = TypeVar("TypeTable", bound=type["Table"])
 T = TypeVar("T", bound="Table")
 TypeTableOrAny = TypeVar("TypeTableOrAny", bound=type["Table"] | Any)
@@ -158,15 +158,15 @@
 
 @dataclasses.dataclass(eq=False)
 class DateTimeField(Field[datetime]):
     """
     DateTime field
     """
 
-    marshamallow: fields.Field = fields.DateTime(required=True, allow_none=False)
+    marshamallow: fields.Field = MarshamallowDateTime(required=True, allow_none=False)
 
 
 @dataclasses.dataclass(eq=False)
 class DecimalField(Field[decimal.Decimal]):
     """
     Decimal field
     """
```

### Comparing `typedmongo-1.1.2/typedmongo/asyncio/table.py` & `typedmongo-1.1.3/typedmongo/asyncio/table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/typedmongo/client.py` & `typedmongo-1.1.3/typedmongo/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/typedmongo/expressions.py` & `typedmongo-1.1.3/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/typedmongo/fields.py` & `typedmongo-1.1.3/typedmongo/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 
 from bson import ObjectId
 from marshmallow import fields
 from typing_extensions import Self
 
 from typedmongo.expressions import CompareMixin, HasFieldName, OrderByMixin
-from typedmongo.marshamallow import MarshamallowObjectId
+from typedmongo.marshamallow import MarshamallowDateTime, MarshamallowObjectId
 
 if TYPE_CHECKING:
     from .table import Table
 
 TypeTable = TypeVar("TypeTable", bound=type["Table"])
 T = TypeVar("T", bound="Table")
 TypeTableOrAny = TypeVar("TypeTableOrAny", bound=type["Table"] | Any)
@@ -158,15 +158,15 @@
 
 @dataclasses.dataclass(eq=False)
 class DateTimeField(Field[datetime]):
     """
     DateTime field
     """
 
-    marshamallow: fields.Field = fields.DateTime(required=True, allow_none=False)
+    marshamallow: fields.Field = MarshamallowDateTime(required=True, allow_none=False)
 
 
 @dataclasses.dataclass(eq=False)
 class DecimalField(Field[decimal.Decimal]):
     """
     Decimal field
     """
```

### Comparing `typedmongo-1.1.2/typedmongo/marshamallow.py` & `typedmongo-1.1.3/typedmongo/marshamallow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from typing import Any
 
 from bson import ObjectId
 from bson.errors import InvalidId
 from marshmallow import ValidationError, fields
 
 
@@ -12,7 +13,16 @@
     def _deserialize(
         self, value: str | ObjectId | bytes, attr: str | None, data: Any, **kwargs
     ):
         try:
             return ObjectId(value)
         except (InvalidId, TypeError):
             raise ValidationError("Invalid ObjectId.")
+
+
+class MarshamallowDateTime(fields.DateTime):
+    def _deserialize(
+        self, value: str | datetime, attr: str | None, data: Any, **kwargs
+    ):
+        if isinstance(value, datetime):
+            return value
+        return super()._deserialize(value, attr, data, **kwargs)
```

### Comparing `typedmongo-1.1.2/typedmongo/sync.py` & `typedmongo-1.1.3/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.2/typedmongo/table.py` & `typedmongo-1.1.3/typedmongo/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,32 @@
 
 @dataclasses.dataclass
 class Index:
     keys: (
         Field
         | Sequence[tuple[Field, int | str | Mapping[str, Any]]]
         | Mapping[Field, Any]
+        | Mapping[str, Any]
     )
 
     name: Optional[str] = None
     unique: bool = False
     background: bool = False
     sparse: bool = False
     expireAfterSeconds: Optional[int] = None
     partialFilterExpression: Optional[dict[str, Any]] = None
 
     def to_index_model(self) -> IndexModel:
         if isinstance(self.keys, Field):
             keys = self.keys.field_name
         elif isinstance(self.keys, Mapping):
-            keys = {field.field_name: value for field, value in self.keys.items()}
+            keys = {
+                field.field_name if isinstance(field, Field) else field: value
+                for field, value in self.keys.items()
+            }
         else:
             keys = [(field.field_name, value) for field, value in self.keys]
 
         parameters = dataclasses.asdict(self)
         del parameters["keys"]
         if parameters["partialFilterExpression"] is None:
             del parameters["partialFilterExpression"]
```

