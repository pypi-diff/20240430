# Comparing `tmp/typedmongo-1.1.1.tar.gz` & `tmp/typedmongo-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.1.1.tar", last modified: Mon Apr 29 09:26:54 2024, max compression
+gzip compressed data, was "typedmongo-1.1.2.tar", last modified: Mon Apr 29 16:31:30 2024, max compression
```

## Comparing `typedmongo-1.1.1.tar` & `typedmongo-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-29 09:26:40.977586 typedmongo-1.1.1/LICENSE
--rw-r--r--   0        0        0      108 2024-04-29 09:26:40.977586 typedmongo-1.1.1/README.md
--rw-r--r--   0        0        0     1441 2024-04-29 09:26:54.473665 typedmongo-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5789 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     3749 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/sync.py
--rw-r--r--   0        0        0     5549 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/test_marshamallow.py
--rw-r--r--   0        0        0     3741 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/test_table.py
--rw-r--r--   0        0        0      781 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/__init__.py
--rw-r--r--   0        0        0      781 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    11612 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     9494 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     8071 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    11394 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/expressions.py
--rw-r--r--   0        0        0     9494 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/fields.py
--rw-r--r--   0        0        0      538 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/sync.py
--rw-r--r--   0        0        0     8071 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/table.py
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-29 16:31:17.549654 typedmongo-1.1.2/LICENSE
+-rw-r--r--   0        0        0      108 2024-04-29 16:31:17.549654 typedmongo-1.1.2/README.md
+-rw-r--r--   0        0        0     1441 2024-04-29 16:31:30.613791 typedmongo-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5789 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     3745 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/sync.py
+-rw-r--r--   0        0        0     5549 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     3737 2024-04-29 16:31:17.549654 typedmongo-1.1.2/tests/test_table.py
+-rw-r--r--   0        0        0      781 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    11612 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     9494 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     8825 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    11394 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/expressions.py
+-rw-r--r--   0        0        0     9494 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/fields.py
+-rw-r--r--   0        0        0      538 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/sync.py
+-rw-r--r--   0        0        0     8712 2024-04-29 16:31:17.549654 typedmongo-1.1.2/typedmongo/table.py
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.1.2/PKG-INFO
```

### Comparing `typedmongo-1.1.1/LICENSE` & `typedmongo-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/pyproject.toml` & `typedmongo-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.1.1"
+version = "1.1.2"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.1.1/tests/asyncio/test_client.py` & `typedmongo-1.1.2/tests/asyncio/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/tests/asyncio/test_table.py` & `typedmongo-1.1.2/tests/asyncio/test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         partial=True,
     )
     assert isinstance(user._id, str)
 
     user = User(
         name="Aber", age=18, tags=["a", "b"], wallet=Wallet(balance=100), children=[]
     )
-    assert not hasattr(user, "_id")
+    assert hasattr(user, "_id")
     assert isinstance(user.dump(user)["_id"], str)
 
 
 def test_recursion_field():
     user = User.load(
         {
             "name": "Aber",
```

### Comparing `typedmongo-1.1.1/tests/sync.py` & `typedmongo-1.1.2/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/tests/test_client.py` & `typedmongo-1.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/tests/test_expressions.py` & `typedmongo-1.1.2/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/tests/test_marshamallow.py` & `typedmongo-1.1.2/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/tests/test_table.py` & `typedmongo-1.1.2/tests/test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         partial=True,
     )
     assert isinstance(user._id, str)
 
     user = User(
         name="Aber", age=18, tags=["a", "b"], wallet=Wallet(balance=100), children=[]
     )
-    assert not hasattr(user, "_id")
+    assert hasattr(user, "_id")
     assert isinstance(user.dump(user)["_id"], str)
 
 
 def test_recursion_field():
     user = User.load(
         {
             "name": "Aber",
```

### Comparing `typedmongo-1.1.1/typedmongo/__init__.py` & `typedmongo-1.1.2/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/asyncio/__init__.py` & `typedmongo-1.1.2/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/asyncio/client.py` & `typedmongo-1.1.2/typedmongo/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/asyncio/fields.py` & `typedmongo-1.1.2/typedmongo/asyncio/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/asyncio/table.py` & `typedmongo-1.1.2/typedmongo/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,17 +156,35 @@
         if instance.__abstract__:
             raise RuntimeError(
                 "The class {} cannot be instantiated, because it's __abstract__ is True.".format(
                     cls.__name__
                 )
             )
 
-        for name, value in kwargs.items():
+        for name, field in cls.__fields__.items():
+            if name in kwargs:
+                value = kwargs.pop(name)
+            else:
+                if field.default is None:
+                    continue
+                default_value = field.default
+                if callable(default_value):
+                    value = default_value()
+                else:
+                    value = default_value
             setattr(instance, name, value)
 
+        if kwargs:
+            raise TypeError(
+                "{class_name}() got unexpected keyword arguments '{unexpected}'".format(
+                    class_name=cls.__name__,
+                    unexpected="', '".join(kwargs.keys()),
+                )
+            )
+
         return instance
 
     def __setattr__(cls, name, value):
         if name == "__abstract__":
             raise AttributeError(
                 "Can't modify the `__abstract__` attribute dynamically."
             )
```

### Comparing `typedmongo-1.1.1/typedmongo/client.py` & `typedmongo-1.1.2/typedmongo/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/expressions.py` & `typedmongo-1.1.2/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/fields.py` & `typedmongo-1.1.2/typedmongo/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/marshamallow.py` & `typedmongo-1.1.2/typedmongo/marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/sync.py` & `typedmongo-1.1.2/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.1/typedmongo/table.py` & `typedmongo-1.1.2/typedmongo/asyncio/table.py`

 * *Files 4% similar despite different names*

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
@@ -156,17 +160,35 @@
         if instance.__abstract__:
             raise RuntimeError(
                 "The class {} cannot be instantiated, because it's __abstract__ is True.".format(
                     cls.__name__
                 )
             )
 
-        for name, value in kwargs.items():
+        for name, field in cls.__fields__.items():
+            if name in kwargs:
+                value = kwargs.pop(name)
+            else:
+                if field.default is None:
+                    continue
+                default_value = field.default
+                if callable(default_value):
+                    value = default_value()
+                else:
+                    value = default_value
             setattr(instance, name, value)
 
+        if kwargs:
+            raise TypeError(
+                "{class_name}() got unexpected keyword arguments '{unexpected}'".format(
+                    class_name=cls.__name__,
+                    unexpected="', '".join(kwargs.keys()),
+                )
+            )
+
         return instance
 
     def __setattr__(cls, name, value):
         if name == "__abstract__":
             raise AttributeError(
                 "Can't modify the `__abstract__` attribute dynamically."
             )
```

