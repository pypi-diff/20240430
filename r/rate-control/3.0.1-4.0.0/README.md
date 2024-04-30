# Comparing `tmp/rate_control-3.0.1.tar.gz` & `tmp/rate_control-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rate_control-3.0.1.tar", max compression
+gzip compressed data, was "rate_control-4.0.0.tar", max compression
```

## Comparing `rate_control-3.0.1.tar` & `rate_control-4.0.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1101 2024-04-27 08:00:53.067565 rate_control-3.0.1/LICENSE
--rw-r--r--   0        0        0     3822 2024-04-27 08:00:53.067565 rate_control-3.0.1/README.rst
--rw-r--r--   0        0        0     2872 2024-04-27 08:00:57.195532 rate_control-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      582 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/__init__.py
--rw-r--r--   0        0        0     3673 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_bucket_group.py
--rw-r--r--   0        0        0      267 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/__init__.py
--rw-r--r--   0        0        0      344 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/__init__.py
--rw-r--r--   0        0        0     2005 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_abc.py
--rw-r--r--   0        0        0     2479 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_base_rate.py
--rw-r--r--   0        0        0      805 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_capacity_updating.py
--rw-r--r--   0        0        0      906 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_token_based.py
--rw-r--r--   0        0        0      977 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_base/_windowed.py
--rw-r--r--   0        0        0     1034 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_fixed_window_counter.py
--rw-r--r--   0        0        0     1372 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_leaky_bucket.py
--rw-r--r--   0        0        0      659 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_buckets/_sliding_window_log.py
--rw-r--r--   0        0        0      179 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_controllers/__init__.py
--rw-r--r--   0        0        0     4987 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_controllers/_abc.py
--rw-r--r--   0        0        0     1121 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_controllers/_rate_limiter.py
--rw-r--r--   0        0        0     8791 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_controllers/_scheduler.py
--rw-r--r--   0        0        0      111 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_enums/__init__.py
--rw-r--r--   0        0        0      262 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_enums/_duration.py
--rw-r--r--   0        0        0      350 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_enums/_priority.py
--rw-r--r--   0        0        0      297 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_errors.py
--rw-r--r--   0        0        0      105 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/__init__.py
--rw-r--r--   0        0        0      781 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/_mk_repr.py
--rw-r--r--   0        0        0      472 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/_protocols.py
--rw-r--r--   0        0        0     1502 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/_request.py
--rw-r--r--   0        0        0     1709 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/_helpers/_validation.py
--rw-r--r--   0        0        0        0 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/py.typed
--rw-r--r--   0        0        0      202 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/__init__.py
--rw-r--r--   0        0        0     1540 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/_abc.py
--rw-r--r--   0        0        0     1336 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/_fifo.py
--rw-r--r--   0        0        0     1311 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/_lifo.py
--rw-r--r--   0        0        0     1658 2024-04-27 08:00:53.071565 rate_control-3.0.1/rate_control/queues/_priority.py
--rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rate_control-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-30 11:59:05.622581 rate_control-4.0.0/LICENSE
+-rw-r--r--   0        0        0     3822 2024-04-30 11:59:05.622581 rate_control-4.0.0/README.rst
+-rw-r--r--   0        0        0     2872 2024-04-30 11:59:09.402567 rate_control-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      582 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/__init__.py
+-rw-r--r--   0        0        0     3865 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_bucket_group.py
+-rw-r--r--   0        0        0      267 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/__init__.py
+-rw-r--r--   0        0        0      344 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/__init__.py
+-rw-r--r--   0        0        0     2025 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_abc.py
+-rw-r--r--   0        0        0     2539 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_base_rate.py
+-rw-r--r--   0        0        0      825 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_capacity_updating.py
+-rw-r--r--   0        0        0      948 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_token_based.py
+-rw-r--r--   0        0        0      997 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_windowed.py
+-rw-r--r--   0        0        0     1074 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_fixed_window_counter.py
+-rw-r--r--   0        0        0     1412 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_leaky_bucket.py
+-rw-r--r--   0        0        0      679 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_sliding_window_log.py
+-rw-r--r--   0        0        0      179 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/__init__.py
+-rw-r--r--   0        0        0     1434 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/_abc.py
+-rw-r--r--   0        0        0     4580 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/_bucket_based.py
+-rw-r--r--   0        0        0     1172 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/_rate_limiter.py
+-rw-r--r--   0        0        0     8930 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/_scheduler.py
+-rw-r--r--   0        0        0      111 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_enums/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_enums/_duration.py
+-rw-r--r--   0        0        0      350 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_enums/_priority.py
+-rw-r--r--   0        0        0      297 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_errors.py
+-rw-r--r--   0        0        0      105 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/_mk_repr.py
+-rw-r--r--   0        0        0      492 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/_protocols.py
+-rw-r--r--   0        0        0     1502 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/_request.py
+-rw-r--r--   0        0        0     1709 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/_validation.py
+-rw-r--r--   0        0        0        0 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/py.typed
+-rw-r--r--   0        0        0      202 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/__init__.py
+-rw-r--r--   0        0        0     1560 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/_abc.py
+-rw-r--r--   0        0        0     1365 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/_fifo.py
+-rw-r--r--   0        0        0     1340 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/_lifo.py
+-rw-r--r--   0        0        0     1687 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/_priority.py
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rate_control-4.0.0/PKG-INFO
```

### Comparing `rate_control-3.0.1/LICENSE` & `rate_control-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.1/README.rst` & `rate_control-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.1/pyproject.toml` & `rate_control-4.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rate-control"
-version = "3.0.1"
+version = "4.0.0"
 description = "Versatile rate controlling in Python"
 authors = ["Corentin Régent <corentin.regent.pro@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/corentin-regent/rate-control"
 repository = "https://github.com/corentin-regent/rate-control"
 documentation = "https://rate-control.readthedocs.io/"
```

### Comparing `rate_control-3.0.1/rate_control/__init__.py` & `rate_control-4.0.0/rate_control/__init__.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.1/rate_control/_bucket_group.py` & `rate_control-4.0.0/rate_control/_bucket_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,24 @@
 else:
     from typing_extensions import override
 
 
 class BucketGroup(Bucket, Iterable[Bucket]):
     """Bucket that aggregates other buckets."""
 
+    __slots__ = (
+        '_buckets',
+        '_recv_stream',
+        '_refill_event',
+        '_send_stream',
+        '_should_enter_context',
+        '_stack',
+        '_task_group',
+    )
+
     def __init__(self, *buckets: Bucket, should_enter_context: bool = True, **kwargs: Any) -> None:
         """
         Args:
             buckets: The buckets to aggregate within this bucket group.
             should_enter_context: Whether entering the context of the bucket group
                 should also enter the context of the underlying buckets.
                 Defaults to `True`.
```

### Comparing `rate_control-3.0.1/rate_control/_buckets/_base/_abc.py` & `rate_control-4.0.0/rate_control/_buckets/_base/_abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 else:
     from typing_extensions import override
 
 
 class Bucket(ABC):
     """Abstract base class for buckets."""
 
+    __slots__ = ()
+
     async def __aenter__(self) -> Self:
         """Enter the bucket context.
 
         It may for example start scheduling replenishments.
         """
         return self
```

### Comparing `rate_control-3.0.1/rate_control/_buckets/_base/_base_rate.py` & `rate_control-4.0.0/rate_control/_buckets/_base/_base_rate.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 else:
     from typing_extensions import override
 
 
 class BaseRateBucket(TokenBasedBucket, ABC):
     """Base class for token buckets that refill at a certain rate."""
 
+    __slots__ = ('_delay', '_refill_event', '_task_group')
+
     def __init__(self, capacity: float, delay: float, **kwargs: Any) -> None:
         """
         Args:
             capacity: The number of tokens that can be acquired within `delay`.
             delay: The refill delay in seconds.
         """
         super().__init__(capacity, **kwargs)
```

### Comparing `rate_control-3.0.1/rate_control/_buckets/_base/_capacity_updating.py` & `rate_control-4.0.0/rate_control/_buckets/_base/_capacity_updating.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from rate_control._buckets._base._token_based import TokenBasedBucket
 from rate_control._helpers._validation import validate_capacity
 
 
 class CapacityUpdatingBucket(TokenBasedBucket):
     """Mixin for buckets which token capacity can be updated."""
 
+    __slots__ = ()
+
     def update_capacity(self, new_capacity: float) -> None:
         """Update the bucket's token capacity.
 
         Changes take effect instantly, and the amount of remaining tokens is updated accordingly.
 
         Args:
             new_capacity: The new token capacity of the bucket.
```

### Comparing `rate_control-3.0.1/rate_control/_buckets/_base/_token_based.py` & `rate_control-4.0.0/rate_control/_buckets/_base/_token_based.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 else:
     from typing_extensions import override
 
 
 class TokenBasedBucket(Bucket, ABC):
     """Base class for buckets that monitor the requests using tokens."""
 
+    __slots__ = ('_capacity', '_tokens')
+
     def __init__(self, capacity: float, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         validate_capacity(capacity)
         self._tokens = self._capacity = capacity
 
     @override
     def can_acquire(self, tokens: float) -> bool:
```

### Comparing `rate_control-3.0.1/rate_control/_buckets/_base/_windowed.py` & `rate_control-4.0.0/rate_control/_buckets/_base/_windowed.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 else:
     from typing_extensions import override
 
 
 class BaseWindowedTokenBucket(BaseRateBucket, ABC):
     """Base class for token buckets that follow strategies based on time windows."""
 
+    __slots__ = ()
+
     def __init__(self, capacity: float, duration: float, **kwargs: Any) -> None:
         """
         Args:
             capacity: The number of tokens that can be acquired within ``duration``.
             duration: The window duration in seconds.
         """
         super().__init__(capacity, duration, **kwargs)
```

### Comparing `rate_control-3.0.1/rate_control/_buckets/_fixed_window_counter.py` & `rate_control-4.0.0/rate_control/_buckets/_fixed_window_counter.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 class FixedWindowCounter(BaseWindowedTokenBucket, CapacityUpdatingBucket):
     """Bucket whose refill strategy follows the fixed window counter algorithm.
 
     The bucket refills once every ``duration`` seconds, to cap its tokens back to ``capacity``.
     """
 
+    __slots__ = ('_scheduled_refill',)
+
     def __init__(self, capacity: float, duration: float, **kwargs: Any) -> None:
         super().__init__(capacity, duration, **kwargs)
         self._scheduled_refill = False
 
     @override
     def _should_schedule_refill(self) -> bool:
         if self._scheduled_refill:
```

### Comparing `rate_control-3.0.1/rate_control/_buckets/_leaky_bucket.py` & `rate_control-4.0.0/rate_control/_buckets/_leaky_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 class LeakyBucket(BaseRateBucket):
     """Bucket whose refill strategy follows the leaky bucket algorithm.
 
     Only one request can get executed every ``delay`` seconds.
     """
 
+    __slots__ = ('_can_pass_through',)
+
     def __init__(self, delay: float, **kwargs: Any) -> None:
         """
         Args:
             delay: The delay before a new request can pass through.
         """
         super().__init__(capacity=math.inf, delay=delay, **kwargs)
         self._can_pass_through = True
```

### Comparing `rate_control-3.0.1/rate_control/_buckets/_sliding_window_log.py` & `rate_control-4.0.0/rate_control/_buckets/_sliding_window_log.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 class SlidingWindowLog(BaseWindowedTokenBucket, CapacityUpdatingBucket):
     """Bucket whose refill strategy follows the sliding window log algorithm.
 
     Every consumed tokens get replenished after ``duration`` seconds.
     """
 
+    __slots__ = ()
+
     @override
     def _should_schedule_refill(self) -> bool:
         return True
 
     @override
     def _refill(self, tokens: float) -> None:
         self._tokens += tokens
```

### Comparing `rate_control-3.0.1/rate_control/_controllers/_abc.py` & `rate_control-4.0.0/rate_control/_controllers/_bucket_based.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 __all__ = [
-    'RateController',
+    'BucketBasedRateController',
 ]
 
 import sys
-from abc import ABC, abstractmethod
-from contextlib import asynccontextmanager, contextmanager
+from abc import ABC
+from contextlib import contextmanager
 from typing import Any, Optional
 
 from rate_control._bucket_group import BucketGroup
 from rate_control._buckets import Bucket
+from rate_control._controllers._abc import RateController
 from rate_control._errors import RateLimit
 from rate_control._helpers import mk_repr
 from rate_control._helpers._validation import validate_max_concurrency
 
 if sys.version_info >= (3, 9):
-    from collections.abc import AsyncIterator, Iterator
+    from collections.abc import Iterator
 else:
-    from typing import AsyncIterator, Iterator
+    from typing import Iterator
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
-class RateController(ABC):
-    """Abstract base class for rate controllers."""
+class BucketBasedRateController(RateController, ABC):
+    """Mixin for rate controllers that use buckets."""
+
+    __slots__ = ('_bucket', '_concurrent_requests', '_max_concurrency', '_should_enter_context')
 
     def __init__(
         self,
         *buckets: Bucket,
         should_enter_context: bool = True,
         max_concurrency: Optional[int] = None,
         **kwargs: Any,
@@ -57,69 +60,54 @@
             if len(buckets) == 1
             else BucketGroup(*buckets, should_enter_context=should_enter_context)
         )
         self._should_enter_context = should_enter_context
         self._max_concurrency = max_concurrency
         self._concurrent_requests = 0
 
+    @override
     async def __aenter__(self) -> Self:
         """Enter the controller's context.
 
         Also enters the context of the underlying buckets,
         if the `should_enter_context` flag was set to `True`.
         """
+        await super().__aenter__()
         if self._should_enter_context and self._bucket is not None:
             await self._bucket.__aenter__()
         return self
 
+    @override
     async def __aexit__(self, *exc_info: Any) -> Optional[bool]:
         """Exit the controller's context.
 
         Also exits the context of the underlying buckets,
         if the `should_enter_context` flag was set to `True`.
         """
         if self._should_enter_context and self._bucket is not None:
             await self._bucket.__aexit__(*exc_info)
-        return False
+        return await super().__aexit__(*exc_info)
 
     @override
     def __repr__(self) -> str:
         return (
             mk_repr(
                 self,
                 self._bucket,
                 should_enter_context=self._should_enter_context,
                 max_concurrency=self._max_concurrency,
             )
             if self._bucket is not None
             else mk_repr(self, max_concurrency=self._max_concurrency)
         )
 
+    @override
     def can_acquire(self, tokens: float = 1) -> bool:
-        """
-        Args:
-            tokens: The amount of tokens to acquire for the request.
-                Defaults to `1`.
-
-        Returns:
-            Whether a request for the given amount of tokens can be processed instantly.
-        """
         return not self._is_concurrency_limited and (self._bucket is None or self._bucket.can_acquire(tokens))
 
-    @asynccontextmanager
-    @abstractmethod
-    async def request(self, tokens: float = 1, **kwargs: Any) -> AsyncIterator[None]:
-        """Asynchronous context manager that requests the given amount of tokens before the execution.
-
-        Args:
-            tokens: The number of tokens required for the request.
-                Defaults to `1`.
-        """
-        yield  # pragma: no cover
-
     @property
     def _is_concurrency_limited(self) -> bool:
         return self._max_concurrency is not None and self._concurrent_requests >= self._max_concurrency
 
     def _assert_can_acquire(self, tokens: float) -> None:
         """Make sure that the request for the given amount of tokens can be processed.
```

### Comparing `rate_control-3.0.1/rate_control/_controllers/_rate_limiter.py` & `rate_control-4.0.0/rate_control/_controllers/_rate_limiter.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,32 @@
     'RateLimiter',
 ]
 
 import sys
 from contextlib import asynccontextmanager
 from typing import Any
 
-from rate_control._controllers._abc import RateController
+from rate_control._controllers._bucket_based import BucketBasedRateController
 
 if sys.version_info >= (3, 9):
     from collections.abc import AsyncIterator
 else:
     from typing import AsyncIterator
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
-class RateLimiter(RateController):
+class RateLimiter(BucketBasedRateController):
     """Rate controller that raises an error if a request cannot be fulfilled instantly."""
 
+    __slots__ = ()
+
     @asynccontextmanager
     @override
     async def request(self, tokens: float = 1, **_: Any) -> AsyncIterator[None]:
         """Context manager that acquires the given amount of tokens while holding concurrency.
 
         Args:
             tokens: The number of tokens to acquire.
```

### Comparing `rate_control-3.0.1/rate_control/_controllers/_scheduler.py` & `rate_control-4.0.0/rate_control/_controllers/_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from contextlib import asynccontextmanager, contextmanager, suppress
 from typing import Any, NoReturn, Optional
 
 from anyio import create_task_group, get_cancelled_exc_class
 from anyio.lowlevel import checkpoint
 
 from rate_control._buckets import Bucket
-from rate_control._controllers._abc import RateController
+from rate_control._controllers._bucket_based import BucketBasedRateController
 from rate_control._enums import Priority
 from rate_control._errors import RateLimit, ReachedMaxPending
 from rate_control._helpers import Request, mk_repr
 from rate_control._helpers._validation import validate_max_pending
 from rate_control.queues import PriorityQueue, Queue
 
 if sys.version_info >= (3, 9):
@@ -29,17 +29,19 @@
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
 
-class Scheduler(RateController):
+class Scheduler(BucketBasedRateController):
     """Rate controller that schedules requests for later processing."""
 
+    __slots__ = ('_is_processing_requests', '_max_pending', '_pending_requests', '_queues', '_task_group')
+
     def __init__(
         self,
         *buckets: Bucket,
         should_enter_context: bool = True,
         max_concurrency: Optional[int] = None,
         max_pending: Optional[int] = None,
         queue_factory: Callable[[], Queue[Request]] = PriorityQueue,
```

### Comparing `rate_control-3.0.1/rate_control/_helpers/_mk_repr.py` & `rate_control-4.0.0/rate_control/_helpers/_mk_repr.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.1/rate_control/_helpers/_request.py` & `rate_control-4.0.0/rate_control/_helpers/_request.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.1/rate_control/_helpers/_validation.py` & `rate_control-4.0.0/rate_control/_helpers/_validation.py`

 * *Files identical despite different names*

### Comparing `rate_control-3.0.1/rate_control/queues/_abc.py` & `rate_control-4.0.0/rate_control/queues/_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 _T = TypeVar('_T')
 
 
 class Queue(ABC, Generic[_T]):
     """Abstract class for representing a queue."""
 
+    __slots__ = ()
+
     @abstractmethod
     def __bool__(self) -> bool:
         """Returns whether the queue contains at least one element"""
 
     @abstractmethod
     @override
     def __repr__(self) -> str:
```

### Comparing `rate_control-3.0.1/rate_control/queues/_fifo.py` & `rate_control-4.0.0/rate_control/queues/_fifo.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 _T = TypeVar('_T')
 
 
 class FifoQueue(Queue[_T]):
     """ "First In, First Out" queue."""
 
+    __slots__ = ('_queue',)
+
     def __init__(self, *elements: _T, **kwargs: Any) -> None:
         """
         Args:
             elements: The elements to initialize the queue with.
         """
         self._queue = deque(elements)
         super().__init__(**kwargs)
```

### Comparing `rate_control-3.0.1/rate_control/queues/_lifo.py` & `rate_control-4.0.0/rate_control/queues/_lifo.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 _T = TypeVar('_T')
 
 
 class LifoQueue(Queue[_T]):
     """ "Last In, First Out" queue."""
 
+    __slots__ = ('_queue',)
+
     def __init__(self, *elements: _T, **kwargs: Any) -> None:
         """
         Args:
             elements: The elements to initialize the queue with.
         """
         self._queue = list(elements)
         super().__init__(**kwargs)
```

### Comparing `rate_control-3.0.1/rate_control/queues/_priority.py` & `rate_control-4.0.0/rate_control/queues/_priority.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     """Queue where the lowest valued elements are retrieved first.
 
     Warning:
         Equally valued elements are not guaranteed to be retrieved
         in the order they arrived.
     """
 
+    __slots__ = ('_queue',)
+
     def __init__(self, *elements: _T, **kwargs: Any) -> None:
         """
         Args:
             elements: The elements to initialize the queue with.
         """
         self._queue = list(elements)
         heapify(self._queue)
```

### Comparing `rate_control-3.0.1/PKG-INFO` & `rate_control-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rate-control
-Version: 3.0.1
+Version: 4.0.0
 Summary: Versatile rate controlling in Python
 Home-page: https://github.com/corentin-regent/rate-control
 License: MIT
 Keywords: async,rate limit,schedule,throttle,token bucket
 Author: Corentin Régent
 Author-email: corentin.regent.pro@gmail.com
 Requires-Python: >=3.8,<4.0
```

