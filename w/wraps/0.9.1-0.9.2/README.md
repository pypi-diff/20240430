# Comparing `tmp/wraps-0.9.1.tar.gz` & `tmp/wraps-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraps-0.9.1.tar", max compression
+gzip compressed data, was "wraps-0.9.2.tar", max compression
```

## Comparing `wraps-0.9.1.tar` & `wraps-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1092 2024-02-26 12:21:30.856496 wraps-0.9.1/LICENSE
--rw-r--r--   0        0        0     6515 2024-02-26 12:21:30.856496 wraps-0.9.1/README.md
--rw-r--r--   0        0        0     2777 2024-02-26 12:21:30.860496 wraps-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2679 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/__init__.py
--rw-r--r--   0        0        0     2925 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/early.py
--rw-r--r--   0        0        0    16045 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/either.py
--rw-r--r--   0        0        0      722 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/errors.py
--rw-r--r--   0        0        0      311 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/future/__init__.py
--rw-r--r--   0        0        0     4343 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/future/base.py
--rw-r--r--   0        0        0    13424 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/future/either.py
--rw-r--r--   0        0        0    12047 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/future/option.py
--rw-r--r--   0        0        0    15819 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/future/result.py
--rw-r--r--   0        0        0      194 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/future/typing.py
--rw-r--r--   0        0        0      340 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/markers.py
--rw-r--r--   0        0        0    41122 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/option.py
--rw-r--r--   0        0        0      553 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/panics.py
--rw-r--r--   0        0        0        0 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/py.typed
--rw-r--r--   0        0        0     1828 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/reawaitable.py
--rw-r--r--   0        0        0    53502 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/result.py
--rw-r--r--   0        0        0      540 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/typing.py
--rw-r--r--   0        0        0      634 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/utils.py
--rw-r--r--   0        0        0     9460 2024-02-26 12:21:30.860496 wraps-0.9.1/wraps/wraps.py
--rw-r--r--   0        0        0     7758 1970-01-01 00:00:00.000000 wraps-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-03-17 08:12:26.776952 wraps-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6515 2024-03-17 08:12:26.776952 wraps-0.9.2/README.md
+-rw-r--r--   0        0        0     2777 2024-03-17 08:12:26.780952 wraps-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2680 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/__init__.py
+-rw-r--r--   0        0        0     2925 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/early.py
+-rw-r--r--   0        0        0    15668 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/either.py
+-rw-r--r--   0        0        0      722 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/errors.py
+-rw-r--r--   0        0        0      311 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/future/__init__.py
+-rw-r--r--   0        0        0     4416 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/future/base.py
+-rw-r--r--   0        0        0    13424 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/future/either.py
+-rw-r--r--   0        0        0    12047 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/future/option.py
+-rw-r--r--   0        0        0    15819 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/future/result.py
+-rw-r--r--   0        0        0     1064 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/future/typing.py
+-rw-r--r--   0        0        0      340 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/markers.py
+-rw-r--r--   0        0        0    41051 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/option.py
+-rw-r--r--   0        0        0      553 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/panics.py
+-rw-r--r--   0        0        0        0 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/py.typed
+-rw-r--r--   0        0        0     1828 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/reawaitable.py
+-rw-r--r--   0        0        0    53534 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/result.py
+-rw-r--r--   0        0        0      540 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/typing.py
+-rw-r--r--   0        0        0      634 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/utils.py
+-rw-r--r--   0        0        0     9460 2024-03-17 08:12:26.780952 wraps-0.9.2/wraps/wraps.py
+-rw-r--r--   0        0        0     7758 1970-01-01 00:00:00.000000 wraps-0.9.2/PKG-INFO
```

### Comparing `wraps-0.9.1/LICENSE` & `wraps-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wraps-0.9.1/README.md` & `wraps-0.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.9.1"
+wraps = "^0.9.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
```

### Comparing `wraps-0.9.1/pyproject.toml` & `wraps-0.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wraps"
-version = "0.9.1"
+version = "0.9.2"
 description = "Meaningful and safe wrapping types."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/wraps"
@@ -30,60 +30,60 @@
 include = "wraps"
 
 [tool.poetry.dependencies]
 python = ">= 3.8"
 
 attrs = ">= 23.2.0"
 
-funcs = ">= 0.9.1"
+funcs = ">= 0.9.2"
 
-typing-aliases = ">= 1.7.1"
+typing-aliases = ">= 1.8.0"
 typing-extensions = ">= 4.10.0"
 
 [tool.poetry.group.format.dependencies]
-ruff = "0.2.2"
+ruff = "0.3.3"
 
 [tool.poetry.group.check.dependencies]
-mypy = "1.8.0"
+mypy = "1.9.0"
 
 [tool.poetry.group.check.dependencies.pre-commit]
 version = "3.6.2"
 python = ">= 3.9"
 
 [tool.poetry.group.test.dependencies]
-coverage = "7.4.3"
-pytest = "8.0.2"
+coverage = "7.4.4"
+pytest = "8.1.1"
 pytest-cov = "4.1.0"
 
 [tool.poetry.group.test.dependencies.anyio]
 version = "4.3.0"
 extras = ["trio"]
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
-mkdocs-material = "9.5.11"
+mkdocs-material = "9.5.13"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
 version = "0.24.0"
 extras = ["python"]
 
 [tool.poetry.group.scripts]
 optional = true
 
 [tool.poetry.group.scripts.dependencies]
-entrypoint = "2.0.1"
+entrypoint = "2.0.3"
 
 [tool.poetry.group.release]
 optional = true
 
 [tool.poetry.group.release.dependencies]
-changelogging = "1.4.1"
+changelogging = "1.4.2"
 
 [tool.ruff]
 line-length = 100
 
 [tool.ruff.lint]
 ignore = [
     "E402",  # module level import not at top of file
@@ -115,15 +115,15 @@
 [tool.mypy]
 strict = true
 
 exclude = ["scripts"]
 
 [tool.changelogging]
 name = "wraps"
-version = "0.9.1"
+version = "0.9.2"
 url = "https://github.com/nekitdev/wraps"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `wraps-0.9.1/wraps/__init__.py` & `wraps-0.9.2/wraps/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 This library implements several types:
 
 - [`Option[T]`][wraps.option.Option] for optional values;
 - [`Result[T, E]`][wraps.result.Result] for error handling;
 - [`Either[L, R]`][wraps.either.Either] for either values;
 - [`Future[T]`][wraps.future.base.Future] for asynchronous abstractions.
 
-The following types are implemented for conveniece:
+The following types are implemented for convenience:
 
 - [`Future[Option[T]] -> FutureOption[T]`][wraps.future.option.FutureOption];
 - [`Future[Result[T, E]] -> FutureResult[T, E]`][wraps.future.result.FutureResult];
 - [`Future[Either[L, R]] -> FutureEither[L, R]`][wraps.future.either.FutureEither].
 
 The library also provides various decorators to wrap functions in order to return the types above.
 """
 
 __description__ = "Meaningful and safe wrapping types."
 __url__ = "https://github.com/nekitdev/wraps"
 
 __title__ = "wraps"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 from wraps.early import early_option, early_option_await, early_result, early_result_await
 from wraps.either import Either, Left, Right, is_left, is_right
 from wraps.future.base import Future
 from wraps.future.either import FutureEither
 from wraps.future.option import FutureOption
 from wraps.future.result import FutureResult
```

### Comparing `wraps-0.9.1/wraps/early.py` & `wraps-0.9.2/wraps/early.py`

 * *Files identical despite different names*

### Comparing `wraps-0.9.1/wraps/either.py` & `wraps-0.9.2/wraps/either.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
     required,
 )
-from typing_extensions import Never, TypeGuard
+from typing_extensions import Never, TypeIs
 
 from wraps.option import NULL, Null, Option, Some
 from wraps.panics import panic
 from wraps.utils import async_empty, async_once, empty, identity, once
 
 __all__ = ("Either", "Left", "Right", "is_left", "is_right")
 
@@ -38,190 +38,148 @@
 U = TypeVar("U")
 
 E = TypeVar("E")
 
 
 class EitherProtocol(Protocol[L, R]):  # type: ignore[misc]
     @required
-    def is_left(self) -> bool:
-        ...
+    def is_left(self) -> bool: ...
 
     @required
-    def is_left_and(self, predicate: Predicate[L]) -> bool:
-        ...
+    def is_left_and(self, predicate: Predicate[L]) -> bool: ...
 
     @required
-    async def is_left_and_await(self, predicate: AsyncPredicate[L]) -> bool:
-        ...
+    async def is_left_and_await(self, predicate: AsyncPredicate[L]) -> bool: ...
 
     @required
-    def is_right(self) -> bool:
-        ...
+    def is_right(self) -> bool: ...
 
     @required
-    def is_right_and(self, predicate: Predicate[R]) -> bool:
-        ...
+    def is_right_and(self, predicate: Predicate[R]) -> bool: ...
 
     @required
-    async def is_right_and_await(self, predicate: AsyncPredicate[R]) -> bool:
-        ...
+    async def is_right_and_await(self, predicate: AsyncPredicate[R]) -> bool: ...
 
     @required
-    def expect_left(self, message: str) -> L:
-        ...
+    def expect_left(self, message: str) -> L: ...
 
     @required
-    def expect_right(self, message: str) -> R:
-        ...
+    def expect_right(self, message: str) -> R: ...
 
     @required
-    def unwrap_left(self) -> L:
-        ...
+    def unwrap_left(self) -> L: ...
 
     @required
-    def unwrap_right(self) -> R:
-        ...
+    def unwrap_right(self) -> R: ...
 
     @required
-    def left(self) -> Option[L]:
-        ...
+    def left(self) -> Option[L]: ...
 
     @required
     def left_or(self, default: L) -> L:  # type: ignore
         ...
 
     @required
-    def left_or_else(self, default: Nullary[L]) -> L:
-        ...
+    def left_or_else(self, default: Nullary[L]) -> L: ...
 
     @required
-    async def left_or_else_await(self, default: AsyncNullary[L]) -> L:
-        ...
+    async def left_or_else_await(self, default: AsyncNullary[L]) -> L: ...
 
     @required
-    def right(self) -> Option[R]:
-        ...
+    def right(self) -> Option[R]: ...
 
     @required
     def right_or(self, default: R) -> R:  # type: ignore
         ...
 
     @required
-    def right_or_else(self, default: Nullary[R]) -> R:
-        ...
+    def right_or_else(self, default: Nullary[R]) -> R: ...
 
     @required
-    async def right_or_else_await(self, default: AsyncNullary[R]) -> R:
-        ...
+    async def right_or_else_await(self, default: AsyncNullary[R]) -> R: ...
 
     @required
-    def into_either(self: EitherProtocol[T, T]) -> T:
-        ...
+    def into_either(self: EitherProtocol[T, T]) -> T: ...
 
     @required
-    def inspect_left(self, function: Inspect[L]) -> Either[L, R]:
-        ...
+    def inspect_left(self, function: Inspect[L]) -> Either[L, R]: ...
 
     @required
-    def inspect_right(self, function: Inspect[R]) -> Either[L, R]:
-        ...
+    def inspect_right(self, function: Inspect[R]) -> Either[L, R]: ...
 
     @required
-    async def inspect_left_await(self, function: AsyncInspect[L]) -> Either[L, R]:
-        ...
+    async def inspect_left_await(self, function: AsyncInspect[L]) -> Either[L, R]: ...
 
     @required
-    async def inspect_right_await(self, function: AsyncInspect[R]) -> Either[L, R]:
-        ...
+    async def inspect_right_await(self, function: AsyncInspect[R]) -> Either[L, R]: ...
 
     @required
-    def flip(self) -> Either[R, L]:
-        ...
+    def flip(self) -> Either[R, L]: ...
 
     @required
-    def map_left(self, function: Unary[L, M]) -> Either[M, R]:
-        ...
+    def map_left(self, function: Unary[L, M]) -> Either[M, R]: ...
 
     @required
-    async def map_left_await(self, function: AsyncUnary[L, M]) -> Either[M, R]:
-        ...
+    async def map_left_await(self, function: AsyncUnary[L, M]) -> Either[M, R]: ...
 
     @required
-    def map_right(self, function: Unary[R, S]) -> Either[L, S]:
-        ...
+    def map_right(self, function: Unary[R, S]) -> Either[L, S]: ...
 
     @required
-    async def map_right_await(self, function: AsyncUnary[R, S]) -> Either[L, S]:
-        ...
+    async def map_right_await(self, function: AsyncUnary[R, S]) -> Either[L, S]: ...
 
     @required
-    def map(self: EitherProtocol[T, T], function: Unary[T, U]) -> Either[U, U]:
-        ...
+    def map(self: EitherProtocol[T, T], function: Unary[T, U]) -> Either[U, U]: ...
 
     @required
-    async def map_await(self: EitherProtocol[T, T], function: AsyncUnary[T, U]) -> Either[U, U]:
-        ...
+    async def map_await(self: EitherProtocol[T, T], function: AsyncUnary[T, U]) -> Either[U, U]: ...
 
     @required
-    def map_either(self, left: Unary[L, M], right: Unary[R, S]) -> Either[M, S]:
-        ...
+    def map_either(self, left: Unary[L, M], right: Unary[R, S]) -> Either[M, S]: ...
 
     @required
     async def map_either_await(
         self, left: AsyncUnary[L, M], right: AsyncUnary[R, S]
-    ) -> Either[M, S]:
-        ...
+    ) -> Either[M, S]: ...
 
     @required
-    def either(self, left: Unary[L, T], right: Unary[R, T]) -> T:
-        ...
+    def either(self, left: Unary[L, T], right: Unary[R, T]) -> T: ...
 
     @required
-    async def either_await(self, left: AsyncUnary[L, T], right: AsyncUnary[R, T]) -> T:
-        ...
+    async def either_await(self, left: AsyncUnary[L, T], right: AsyncUnary[R, T]) -> T: ...
 
     @required
-    def left_and_then(self, function: Unary[L, Either[M, R]]) -> Either[M, R]:
-        ...
+    def left_and_then(self, function: Unary[L, Either[M, R]]) -> Either[M, R]: ...
 
     @required
-    async def left_and_then_await(self, function: AsyncUnary[L, Either[M, R]]) -> Either[M, R]:
-        ...
+    async def left_and_then_await(self, function: AsyncUnary[L, Either[M, R]]) -> Either[M, R]: ...
 
     @required
-    def right_and_then(self, function: Unary[R, Either[L, S]]) -> Either[L, S]:
-        ...
+    def right_and_then(self, function: Unary[R, Either[L, S]]) -> Either[L, S]: ...
 
     @required
-    async def right_and_then_await(self, function: AsyncUnary[R, Either[L, S]]) -> Either[L, S]:
-        ...
+    async def right_and_then_await(self, function: AsyncUnary[R, Either[L, S]]) -> Either[L, S]: ...
 
     @required
-    def iter_left(self) -> Iterator[L]:
-        ...
+    def iter_left(self) -> Iterator[L]: ...
 
     @required
-    def iter_right(self) -> Iterator[R]:
-        ...
+    def iter_right(self) -> Iterator[R]: ...
 
     @required
-    def iter_either(self: EitherProtocol[T, T]) -> Iterator[T]:
-        ...
+    def iter_either(self: EitherProtocol[T, T]) -> Iterator[T]: ...
 
     @required
-    def async_iter_left(self) -> AsyncIterator[L]:
-        ...
+    def async_iter_left(self) -> AsyncIterator[L]: ...
 
     @required
-    def async_iter_right(self) -> AsyncIterator[R]:
-        ...
+    def async_iter_right(self) -> AsyncIterator[R]: ...
 
     @required
-    def async_iter_either(self: EitherProtocol[T, T]) -> AsyncIterator[T]:
-        ...
+    def async_iter_either(self: EitherProtocol[T, T]) -> AsyncIterator[T]: ...
 
     def flatten_left(self: EitherProtocol[EitherProtocol[L, R], R]) -> Either[L, R]:
         return self.left_and_then(identity)  # type: ignore
 
     def flatten_right(self: EitherProtocol[L, EitherProtocol[L, R]]) -> Either[L, R]:
         return self.right_and_then(identity)  # type: ignore
 
@@ -234,28 +192,24 @@
     #     ...
 
     # @required
     # def factor_ok(self: EitherProtocol[Result[T, L], Result[T, R]]) -> Result[T, Either[L, R]]:
     #     ...
 
     @required
-    def contains_left(self, value: M) -> bool:
-        ...
+    def contains_left(self, value: M) -> bool: ...
 
     @required
-    def contains_right(self, value: S) -> bool:
-        ...
+    def contains_right(self, value: S) -> bool: ...
 
     @required
-    def contains(self: EitherProtocol[T, T], value: U) -> bool:
-        ...
+    def contains(self: EitherProtocol[T, T], value: U) -> bool: ...
 
     @required
-    def into_result(self) -> Result[L, R]:
-        ...
+    def into_result(self) -> Result[L, R]: ...
 
 
 UNWRAP_LEFT_ON_RIGHT = "`unwrap_left` called on right"
 UNWRAP_RIGHT_ON_LEFT = "`unwrap_right` called on left"
 
 
 @final
@@ -580,17 +534,17 @@
 
 Either = Union[Left[L], Right[R]]
 """Either value, expressed as the union of [`Left[L]`][wraps.either.Left]
 and [`Right[R]`][wraps.either.Right].
 """
 
 
-def is_left(either: Either[L, R]) -> TypeGuard[Left[L]]:
+def is_left(either: Either[L, R]) -> TypeIs[Left[L]]:
     return either.is_left()
 
 
-def is_right(either: Either[L, R]) -> TypeGuard[Right[R]]:
+def is_right(either: Either[L, R]) -> TypeIs[Right[R]]:
     return either.is_right()
 
 
 # import cycle solution
 from wraps.result import Error, Ok, Result
```

### Comparing `wraps-0.9.1/wraps/errors.py` & `wraps-0.9.2/wraps/errors.py`

 * *Files identical despite different names*

### Comparing `wraps-0.9.1/wraps/future/base.py` & `wraps-0.9.2/wraps/future/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     async def actual_base_map_future(self, function: Unary[T, U]) -> U:
         return function(await self.awaitable)
 
     async def actual_base_map_future_await(self, function: AsyncUnary[T, U]) -> U:
         return await function(await self.awaitable)
 
-    def then(self, function: Unary[T, Future[U]]) -> Future[U]:
+    def then(self, function: FutureUnary[T, U]) -> Future[U]:
         """Chains computation by applying the `function` to the result, returning the resulting
         [`Future[U]`][wraps.future.base.Future].
 
         Arguments:
             function: The future-returning function to apply.
 
         Returns:
@@ -132,17 +132,22 @@
         future = Future(async_identity(value))
         ```
 
         Example:
             ```python
             value = 42
 
-            assert await Future.from_value(value) is value
+            future = Future.from_value(value)
+
+            assert await future is value
             ```
 
         Arguments:
             value: The value to wrap.
 
         Returns:
             The future wrapping the given value.
         """
         return cls.create(async_identity(value))
+
+
+from wraps.future.typing import FutureUnary
```

### Comparing `wraps-0.9.1/wraps/future/either.py` & `wraps-0.9.2/wraps/future/either.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Future either values."""
 
 from __future__ import annotations
 
-from typing import Awaitable, TypeVar
+from typing import Awaitable, TypeVar, final
 
 from attrs import field, frozen
 from typing_aliases import (
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from typing_extensions import Never, final
+from typing_extensions import Never
 
 from wraps.either import Either, Left, Right
 from wraps.future.base import Future
 from wraps.reawaitable import ReAwaitable
 from wraps.result import Result
 from wraps.utils import identity
```

### Comparing `wraps-0.9.1/wraps/future/option.py` & `wraps-0.9.2/wraps/future/option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Future optional values."""
 
 from __future__ import annotations
 
-from typing import Awaitable, Optional, Tuple, TypeVar
+from typing import Awaitable, Optional, Tuple, TypeVar, final
 
 from attrs import field, frozen
 from typing_aliases import (
     AsyncBinary,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Binary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from typing_extensions import Never, final
+from typing_extensions import Never
 
 from wraps.future.base import Future
 from wraps.option import NULL, Option, Some
 from wraps.reawaitable import ReAwaitable
 from wraps.result import Result
 from wraps.utils import identity
```

### Comparing `wraps-0.9.1/wraps/future/result.py` & `wraps-0.9.2/wraps/future/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Future error handling."""
 
 from __future__ import annotations
 
-from typing import Awaitable, TypeVar
+from typing import Awaitable, TypeVar, final
 
 from attrs import field, frozen
 from typing_aliases import (
     AnyError,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from typing_extensions import Never, final
+from typing_extensions import Never
 
 from wraps.either import Either
 from wraps.future.base import Future
 from wraps.option import Option
 from wraps.reawaitable import ReAwaitable
 from wraps.result import Error, Ok, Result
 from wraps.utils import identity
```

### Comparing `wraps-0.9.1/wraps/option.py` & `wraps-0.9.2/wraps/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,21 @@
 from __future__ import annotations
 
 from typing import (
     AsyncIterable,
     AsyncIterator,
     Iterable,
     Iterator,
+    Literal,
     Optional,
+    Protocol,
     Tuple,
     TypeVar,
     Union,
+    final,
     overload,
 )
 
 from attrs import frozen
 from typing_aliases import (
     AsyncBinary,
     AsyncInspect,
@@ -74,15 +77,15 @@
     Binary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
     required,
 )
-from typing_extensions import Literal, Never, Protocol, TypeGuard, final
+from typing_extensions import Never, TypeIs
 
 from wraps.errors import EarlyOption
 from wraps.panics import panic
 from wraps.utils import async_empty, async_once, empty, identity, once
 
 __all__ = ("NULL", "Option", "Some", "Null", "is_some", "is_null")
 
@@ -1389,60 +1392,53 @@
     async def or_else_await(self, default: AsyncNullary[Option[T]]) -> Some[T]:
         return self
 
     def xor(self, option: Option[T]) -> Option[T]:
         return self if is_null(option) else NULL
 
     @overload
-    def zip(self, option: Null) -> Null:
-        ...
+    def zip(self, option: Null) -> Null: ...
 
     @overload
-    def zip(self, option: Some[U]) -> Some[Tuple[T, U]]:
-        ...
+    def zip(self, option: Some[U]) -> Some[Tuple[T, U]]: ...
 
     @overload
-    def zip(self, option: Option[U]) -> Option[Tuple[T, U]]:
-        ...
+    def zip(self, option: Option[U]) -> Option[Tuple[T, U]]: ...
 
     def zip(self, option: Option[U]) -> Option[Tuple[T, U]]:
         if is_some(option):
             return self.create((self.value, option.value))
 
-        return option  # type: ignore
+        return option
 
     @overload
-    def zip_with(self, option: Null, function: Binary[T, U, V]) -> Null:
-        ...
+    def zip_with(self, option: Null, function: Binary[T, U, V]) -> Null: ...
 
     @overload
-    def zip_with(self, option: Some[U], function: Binary[T, U, V]) -> Some[V]:
-        ...
+    def zip_with(self, option: Some[U], function: Binary[T, U, V]) -> Some[V]: ...
 
     @overload
-    def zip_with(self, option: Option[U], function: Binary[T, U, V]) -> Option[V]:
-        ...
+    def zip_with(self, option: Option[U], function: Binary[T, U, V]) -> Option[V]: ...
 
     def zip_with(self, option: Option[U], function: Binary[T, U, V]) -> Option[V]:
         if is_some(option):
             return self.create(function(self.value, option.value))
 
         return NULL
 
     @overload
-    async def zip_with_await(self, option: Null, function: AsyncBinary[T, U, V]) -> Null:
-        ...
+    async def zip_with_await(self, option: Null, function: AsyncBinary[T, U, V]) -> Null: ...
 
     @overload
-    async def zip_with_await(self, option: Some[U], function: AsyncBinary[T, U, V]) -> Some[V]:
-        ...
+    async def zip_with_await(self, option: Some[U], function: AsyncBinary[T, U, V]) -> Some[V]: ...
 
     @overload
-    async def zip_with_await(self, option: Option[U], function: AsyncBinary[T, U, V]) -> Option[V]:
-        ...
+    async def zip_with_await(
+        self, option: Option[U], function: AsyncBinary[T, U, V]
+    ) -> Option[V]: ...
 
     async def zip_with_await(self, option: Option[U], function: AsyncBinary[T, U, V]) -> Option[V]:
         if is_some(option):
             return self.create(await function(self.value, option.value))
 
         return NULL
 
@@ -1463,22 +1459,22 @@
 and [`Null`][wraps.option.Null].
 """
 
 NULL = Null()
 """The instance of [`Null`][wraps.option.Null]."""
 
 
-def is_some(option: Option[T]) -> TypeGuard[Some[T]]:
+def is_some(option: Option[T]) -> TypeIs[Some[T]]:
     """This is the same as [`Option.is_some`][wraps.option.OptionProtocol.is_some],
     except it works as a *type guard*.
     """
     return option.is_some()
 
 
-def is_null(option: Option[T]) -> TypeGuard[Null]:
+def is_null(option: Option[T]) -> TypeIs[Null]:
     """This is the same as [`Option.is_null`][wraps.option.OptionProtocol.is_null],
     except it works as a *type guard*.
     """
     return option.is_null()
 
 
 # import cycle solution
```

### Comparing `wraps-0.9.1/wraps/panics.py` & `wraps-0.9.2/wraps/panics.py`

 * *Files identical despite different names*

### Comparing `wraps-0.9.1/wraps/reawaitable.py` & `wraps-0.9.2/wraps/reawaitable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Awaitable, Callable, Generator, TypeVar
+from typing import Awaitable, Callable, Generator, TypeVar, final
 
 from attrs import define, field
 from funcs.decorators import wraps
 from typing_aliases import AsyncCallable
-from typing_extensions import ParamSpec, final
+from typing_extensions import ParamSpec
 
 from wraps.option import Null, Option, Some
 
 __all__ = ("ReAwaitable", "reawaitable")
 
 P = ParamSpec("P")
 R = TypeVar("R")
```

### Comparing `wraps-0.9.1/wraps/result.py` & `wraps-0.9.2/wraps/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,30 +40,40 @@
     case Error(error):
         print(error)
 ```
 """
 
 from __future__ import annotations
 
-from typing import AsyncIterable, AsyncIterator, Iterable, Iterator, TypeVar, Union
+from typing import (
+    AsyncIterable,
+    AsyncIterator,
+    Iterable,
+    Iterator,
+    Literal,
+    Protocol,
+    TypeVar,
+    Union,
+    final,
+)
 
 from attrs import frozen
 from typing_aliases import (
     AnyError,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
     required,
 )
-from typing_extensions import Literal, Never, ParamSpec, Protocol, TypeGuard, final
+from typing_extensions import Never, ParamSpec, TypeIs
 
 from wraps.errors import EarlyResult
 from wraps.option import NULL, Null, Option, Some
 from wraps.panics import panic
 from wraps.utils import async_empty, async_once, empty, identity, once
 
 __all__ = ("Result", "Ok", "Error", "is_ok", "is_error")
@@ -1856,22 +1866,22 @@
 
 Result = Union[Ok[T], Error[E]]
 """Result value, expressed as the union of [`Ok[T]`][wraps.result.Ok]
 and [`Error[E]`][wraps.result.Error].
 """
 
 
-def is_ok(result: Result[T, E]) -> TypeGuard[Ok[T]]:
+def is_ok(result: Result[T, E]) -> TypeIs[Ok[T]]:
     """This is the same as [`Result.is_ok`][wraps.result.ResultProtocol.is_ok],
     except it works as a *type guard*.
     """
     return result.is_ok()
 
 
-def is_error(result: Result[T, E]) -> TypeGuard[Error[E]]:
+def is_error(result: Result[T, E]) -> TypeIs[Error[E]]:
     """This is the same as [`Result.is_error`][wraps.result.ResultProtocol.is_error],
     except it works as a *type guard*.
     """
     return result.is_error()
 
 
 # import cycle solution
```

### Comparing `wraps-0.9.1/wraps/typing.py` & `wraps-0.9.2/wraps/typing.py`

 * *Files identical despite different names*

### Comparing `wraps-0.9.1/wraps/utils.py` & `wraps-0.9.2/wraps/utils.py`

 * *Files identical despite different names*

### Comparing `wraps-0.9.1/wraps/wraps.py` & `wraps-0.9.2/wraps/wraps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Highly composable wrapping decorators."""
 
 from __future__ import annotations
 
-from typing import Callable, Generic, Optional, Type, TypeVar
+from typing import Callable, Generic, Optional, Type, TypeVar, final
 
 from attrs import frozen
 from funcs.decorators import wraps
 from typing_aliases import AnyError, AsyncCallable, NormalError
-from typing_extensions import ParamSpec, final
+from typing_extensions import ParamSpec
 
 from wraps.either import Either
 from wraps.future.base import Future
 from wraps.future.either import FutureEither
 from wraps.future.option import FutureOption
 from wraps.future.result import FutureResult
 from wraps.option import NULL, Option, Some
```

### Comparing `wraps-0.9.1/PKG-INFO` & `wraps-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wraps
-Version: 0.9.1
+Version: 0.9.2
 Summary: Meaningful and safe wrapping types.
 Home-page: https://github.com/nekitdev/wraps
 License: MIT
 Keywords: python,future,either,option,result
 Author: nekitdev
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: attrs (>=23.2.0)
-Requires-Dist: funcs (>=0.9.1)
-Requires-Dist: typing-aliases (>=1.7.1)
+Requires-Dist: funcs (>=0.9.2)
+Requires-Dist: typing-aliases (>=1.8.0)
 Requires-Dist: typing-extensions (>=4.10.0)
 Project-URL: Chat, https://nekit.dev/chat
 Project-URL: Documentation, https://nekitdev.github.io/wraps
 Project-URL: Funding, https://nekit.dev/funding
 Project-URL: Issues, https://github.com/nekitdev/wraps/issues
 Project-URL: Repository, https://github.com/nekitdev/wraps
 Description-Content-Type: text/markdown
@@ -72,15 +72,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.9.1"
+wraps = "^0.9.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
```

