# Comparing `tmp/pyrate_limiter-3.6.0.tar.gz` & `tmp/pyrate_limiter-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrate_limiter-3.6.0.tar", max compression
+gzip compressed data, was "pyrate_limiter-3.6.1.tar", max compression
```

## Comparing `pyrate_limiter-3.6.0.tar` & `pyrate_limiter-3.6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     4373 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/LICENSE
--rw-r--r--   0        0        0    22404 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/README.md
--rw-r--r--   0        0        0   261075 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/docs/_static/components.jpg
--rw-r--r--   0        0        0    19485 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/docs/_static/logo.png
--rw-r--r--   0        0        0       60 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/docs/changelog.md
--rw-r--r--   0        0        0     1815 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/docs/conf.py
--rw-r--r--   0        0        0       72 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/docs/contributing.md
--rw-r--r--   0        0        0      313 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/docs/index.md
--rw-r--r--   0        0        0      218 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/docs/reference.md
--rw-r--r--   0        0        0     2431 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/pyproject.toml
--rw-r--r--   0        0        0      155 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/pyrate_limiter/__init__.py
--rw-r--r--   0        0        0       87 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/pyrate_limiter/abstracts/__init__.py
--rw-r--r--   0        0        0     9457 2024-03-17 15:06:21.036917 pyrate_limiter-3.6.0/pyrate_limiter/abstracts/bucket.py
--rw-r--r--   0        0        0      300 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/abstracts/clock.py
--rw-r--r--   0        0        0     2455 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/abstracts/rate.py
--rw-r--r--   0        0        0      308 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/buckets/__init__.py
--rw-r--r--   0        0        0     2739 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/buckets/in_memory_bucket.py
--rw-r--r--   0        0        0     5329 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/buckets/postgres.py
--rw-r--r--   0        0        0     5551 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/buckets/redis_bucket.py
--rw-r--r--   0        0        0     5460 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/buckets/sqlite_bucket.py
--rw-r--r--   0        0        0     1816 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/clocks.py
--rw-r--r--   0        0        0     1158 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/exceptions.py
--rw-r--r--   0        0        0    10735 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/limiter.py
--rw-r--r--   0        0        0        0 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/py.typed
--rw-r--r--   0        0        0     2020 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/pyrate_limiter/utils.py
--rw-r--r--   0        0        0        0 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/tests/__init__.py
--rw-r--r--   0        0        0     4250 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/tests/conftest.py
--rw-r--r--   0        0        0     1798 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/tests/demo_bucket_factory.py
--rw-r--r--   0        0        0     2926 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/tests/helpers.py
--rw-r--r--   0        0        0     7618 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/tests/test_bucket_all.py
--rw-r--r--   0        0        0     2291 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/tests/test_bucket_factory.py
--rw-r--r--   0        0        0     8012 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/tests/test_limiter.py
--rw-r--r--   0        0        0     3980 2024-03-17 15:06:21.040917 pyrate_limiter-3.6.0/tests/test_others.py
--rw-r--r--   0        0        0    24114 1970-01-01 00:00:00.000000 pyrate_limiter-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4373 2024-04-30 17:03:20.723619 pyrate_limiter-3.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2024-04-30 17:03:20.723619 pyrate_limiter-3.6.1/LICENSE
+-rw-r--r--   0        0        0    22404 2024-04-30 17:03:20.723619 pyrate_limiter-3.6.1/README.md
+-rw-r--r--   0        0        0   261075 2024-04-30 17:03:20.723619 pyrate_limiter-3.6.1/docs/_static/components.jpg
+-rw-r--r--   0        0        0    19485 2024-04-30 17:03:20.723619 pyrate_limiter-3.6.1/docs/_static/logo.png
+-rw-r--r--   0        0        0       60 2024-04-30 17:03:20.723619 pyrate_limiter-3.6.1/docs/changelog.md
+-rw-r--r--   0        0        0     1815 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/docs/conf.py
+-rw-r--r--   0        0        0       72 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/docs/contributing.md
+-rw-r--r--   0        0        0      313 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/docs/index.md
+-rw-r--r--   0        0        0      218 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/docs/reference.md
+-rw-r--r--   0        0        0     2431 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/abstracts/__init__.py
+-rw-r--r--   0        0        0     9366 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/abstracts/bucket.py
+-rw-r--r--   0        0        0      300 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/abstracts/clock.py
+-rw-r--r--   0        0        0     2455 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/abstracts/rate.py
+-rw-r--r--   0        0        0      308 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/buckets/__init__.py
+-rw-r--r--   0        0        0     2739 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/buckets/in_memory_bucket.py
+-rw-r--r--   0        0        0     5329 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/buckets/postgres.py
+-rw-r--r--   0        0        0     5551 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/buckets/redis_bucket.py
+-rw-r--r--   0        0        0     5460 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/buckets/sqlite_bucket.py
+-rw-r--r--   0        0        0     1816 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/clocks.py
+-rw-r--r--   0        0        0     1158 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/exceptions.py
+-rw-r--r--   0        0        0    11328 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/limiter.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/py.typed
+-rw-r--r--   0        0        0     2020 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/pyrate_limiter/utils.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     4187 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     3861 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/tests/demo_bucket_factory.py
+-rw-r--r--   0        0        0     2926 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/tests/helpers.py
+-rw-r--r--   0        0        0     7618 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/tests/test_bucket_all.py
+-rw-r--r--   0        0        0     2205 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/tests/test_bucket_factory.py
+-rw-r--r--   0        0        0    10717 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/tests/test_limiter.py
+-rw-r--r--   0        0        0     3980 2024-04-30 17:03:20.727619 pyrate_limiter-3.6.1/tests/test_others.py
+-rw-r--r--   0        0        0    24114 1970-01-01 00:00:00.000000 pyrate_limiter-3.6.1/PKG-INFO
```

### Comparing `pyrate_limiter-3.6.0/CHANGELOG.md` & `pyrate_limiter-3.6.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/LICENSE` & `pyrate_limiter-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/README.md` & `pyrate_limiter-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/docs/_static/components.jpg` & `pyrate_limiter-3.6.1/docs/_static/components.jpg`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/docs/_static/logo.png` & `pyrate_limiter-3.6.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/docs/conf.py` & `pyrate_limiter-3.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/pyproject.toml` & `pyrate_limiter-3.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrate-limiter"
-version = "3.6.0"
+version = "3.6.1"
 description = "Python Rate-Limiter using Leaky-Bucket Algorithm"
 authors = ["vutr <me@vutr.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/vutran1710/PyrateLimiter"
 repository = "https://github.com/vutran1710/PyrateLimiter"
 documentation = "https://pyrate-limiter.readthedocs.io"
```

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/abstracts/bucket.py` & `pyrate_limiter-3.6.1/pyrate_limiter/abstracts/bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,14 @@
     is_async_leak_started = False
 
     def __init__(self, leak_interval: int):
         self.sync_buckets = defaultdict()
         self.async_buckets = defaultdict()
         self.clocks = defaultdict()
         self.leak_interval = leak_interval
-        self._task = None
         super().__init__()
 
     def register(self, bucket: AbstractBucket, clock: AbstractClock):
         """Register a new bucket with its associated clock"""
         assert self.sync_buckets is not None
         assert self.clocks is not None
         assert self.async_buckets is not None
@@ -168,28 +167,24 @@
                 logger.debug("> Leaking (%s) bucket: %s, %s items", bucket_type, bucket, leak)
 
             await asyncio.sleep(self.leak_interval / 1000)
 
     def leak_async(self):
         if self.async_buckets and not self.is_async_leak_started:
             self.is_async_leak_started = True
-            self._task = asyncio.create_task(self._leak(sync=False))
+            asyncio.create_task(self._leak(sync=False))
 
     def run(self) -> None:
         assert self.sync_buckets
         asyncio.run(self._leak(sync=True))
 
     def start(self) -> None:
         if self.sync_buckets and not self.is_alive():
             super().start()
 
-    def cancel(self) -> None:
-        if self._task:
-            self._task.cancel()
-
 
 class BucketFactory(ABC):
     """Asbtract BucketFactory class.
     It is reserved for user to implement/override this class with
     his own bucket-routing/creating logic
     """
 
@@ -218,15 +213,15 @@
     ) -> Union[RateItem, Awaitable[RateItem]]:
         """Add the current timestamp to the receiving item using any clock backend
         - Turn it into a RateItem
         - Can return either a coroutine or a RateItem instance
         """
 
     @abstractmethod
-    def get(self, item: RateItem) -> AbstractBucket:
+    def get(self, item: RateItem) -> Union[AbstractBucket, Awaitable[AbstractBucket]]:
         """Get the corresponding bucket to this item"""
 
     def create(
         self,
         clock: AbstractClock,
         bucket_class: Type[AbstractBucket],
         *args,
```

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/abstracts/rate.py` & `pyrate_limiter-3.6.1/pyrate_limiter/abstracts/rate.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/buckets/in_memory_bucket.py` & `pyrate_limiter-3.6.1/pyrate_limiter/buckets/in_memory_bucket.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/buckets/postgres.py` & `pyrate_limiter-3.6.1/pyrate_limiter/buckets/postgres.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/buckets/redis_bucket.py` & `pyrate_limiter-3.6.1/pyrate_limiter/buckets/redis_bucket.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/buckets/sqlite_bucket.py` & `pyrate_limiter-3.6.1/pyrate_limiter/buckets/sqlite_bucket.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/clocks.py` & `pyrate_limiter-3.6.1/pyrate_limiter/clocks.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/exceptions.py` & `pyrate_limiter-3.6.1/pyrate_limiter/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/limiter.py` & `pyrate_limiter-3.6.1/pyrate_limiter/limiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 
     def wrap_item(self, name: str, weight: int = 1):
         now = self.clock.now()
 
         async def wrap_async():
             return RateItem(name, await now, weight=weight)
 
-        def wrap_sycn():
+        def wrap_sync():
             return RateItem(name, now, weight=weight)
 
-        return wrap_async() if isawaitable(now) else wrap_sycn()
+        return wrap_async() if isawaitable(now) else wrap_sync()
 
     def get(self, _: RateItem) -> AbstractBucket:
         return self.bucket
 
 
 class Limiter:
     """This class responsibility is to sum up all underlying logic
@@ -248,45 +248,62 @@
                 return result
 
             return _put_async()
 
         return _handle_result(acquire)  # type: ignore
 
     def try_acquire(self, name: str, weight: int = 1) -> Union[bool, Awaitable[bool]]:
-        """Try accquiring an item with name & weight
+        """Try acquiring an item with name & weight
         Return true on success, false on failure
         """
         with self.lock:
             assert weight >= 0, "item's weight must be >= 0"
 
             if weight == 0:
                 # NOTE: if item is weightless, just let it go through
-                # NOTE: this might change in the futre
+                # NOTE: this might change in the future
                 return True
 
             item = self.bucket_factory.wrap_item(name, weight)
 
             if isawaitable(item):
 
                 async def _handle_async():
                     nonlocal item
                     item = await item
                     bucket = self.bucket_factory.get(item)
+                    if isawaitable(bucket):
+                        bucket = await bucket
                     assert isinstance(bucket, AbstractBucket), f"Invalid bucket: item: {name}"
                     result = self.handle_bucket_put(bucket, item)
 
                     while isawaitable(result):
                         result = await result
 
                     return result
 
                 return _handle_async()
 
             assert isinstance(item, RateItem)  # NOTE: this is to silence mypy warning
             bucket = self.bucket_factory.get(item)
+            if isawaitable(bucket):
+
+                async def _handle_async_bucket():
+                    nonlocal bucket
+                    bucket = await bucket
+                    assert isinstance(bucket, AbstractBucket), f"Invalid bucket: item: {name}"
+                    result = self.handle_bucket_put(bucket, item)
+
+                    while isawaitable(result):
+                        result = await result
+
+                    return result
+
+                return _handle_async_bucket()
+
             assert isinstance(bucket, AbstractBucket), f"Invalid bucket: item: {name}"
             result = self.handle_bucket_put(bucket, item)
 
             if isawaitable(result):
 
                 async def _handle_async_result():
                     nonlocal result
```

### Comparing `pyrate_limiter-3.6.0/pyrate_limiter/utils.py` & `pyrate_limiter-3.6.1/pyrate_limiter/utils.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/tests/conftest.py` & `pyrate_limiter-3.6.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,39 +15,35 @@
 from pyrate_limiter import id_generator
 from pyrate_limiter import InMemoryBucket
 from pyrate_limiter import MonotonicClock
 from pyrate_limiter import PostgresBucket
 from pyrate_limiter import Rate
 from pyrate_limiter import RedisBucket
 from pyrate_limiter import SQLiteBucket
-from pyrate_limiter import SQLiteClock
 from pyrate_limiter import SQLiteQueries as Queries
 from pyrate_limiter import TimeAsyncClock
 from pyrate_limiter import TimeClock
 
-
 # Make log messages visible on test failure (or with pytest -s)
 basicConfig(level="INFO")
 # Uncomment for more verbose output:
 logger = getLogger("pyrate_limiter")
 logger.setLevel(getenv("LOG_LEVEL", "INFO"))
 
 DEFAULT_RATES = [Rate(3, 1000), Rate(4, 1500)]
 
 clocks = [
     MonotonicClock(),
     TimeClock(),
-    SQLiteClock.default(),
     TimeAsyncClock(),
 ]
 
 ClockSet = Union[
     MonotonicClock,
     TimeClock,
-    SQLiteClock,
     TimeAsyncClock,
 ]
 
 
 @pytest.fixture(params=clocks)
 def clock(request):
     """Parametrization for different clock."""
@@ -71,15 +67,15 @@
     return bucket
 
 
 async def create_async_redis_bucket(rates: List[Rate]):
     from redis.asyncio import ConnectionPool as AsyncConnectionPool
     from redis.asyncio import Redis as AsyncRedis
 
-    pool = AsyncConnectionPool.from_url(getenv("REDIS", "redis://localhost:6379"))
+    pool: AsyncConnectionPool = AsyncConnectionPool.from_url(getenv("REDIS", "redis://localhost:6379"))
     redis_db: AsyncRedis = AsyncRedis(connection_pool=pool)
     bucket_key = f"test-bucket/{id_generator()}"
     await redis_db.delete(bucket_key)
     bucket = await RedisBucket.init(rates, redis_db, bucket_key)
     assert await bucket.count() == 0
     return bucket
```

### Comparing `pyrate_limiter-3.6.0/tests/helpers.py` & `pyrate_limiter-3.6.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/tests/test_bucket_all.py` & `pyrate_limiter-3.6.1/tests/test_bucket_all.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/tests/test_bucket_factory.py` & `pyrate_limiter-3.6.1/tests/test_bucket_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 
     assert isinstance(item, RateItem)
     assert item.weight == 1
 
     bucket = factory.get(item)
 
     assert isinstance(bucket, AbstractBucket)
-    if factory._leaker:
-        factory._leaker.cancel()
 
 
 @pytest.mark.asyncio
 async def test_factory_leak(clock, create_bucket):
     bucket1 = await create_bucket(DEFAULT_RATES)
     bucket2 = await create_bucket(DEFAULT_RATES)
     assert id(bucket1) != id(bucket2)
@@ -80,8 +78,7 @@
             sleep(6)
 
         assert await async_count(bucket1) == 0
         assert await async_count(bucket2) == 0
         assert await async_count(factory.buckets[item_name]) == 0
 
     assert len(factory.buckets) == 3
-    factory._leaker.cancel()
```

### Comparing `pyrate_limiter-3.6.0/tests/test_limiter.py` & `pyrate_limiter-3.6.1/tests/test_limiter.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 from inspect import isawaitable
 
 import pytest
 
 from .conftest import DEFAULT_RATES
 from .conftest import logger
+from .demo_bucket_factory import DemoAsyncGetBucketFactory
 from .demo_bucket_factory import DemoBucketFactory
 from .helpers import async_acquire
 from .helpers import concurrent_acquire
 from .helpers import flushing_bucket
 from .helpers import inspect_bucket_items
 from .helpers import prefilling_bucket
 from pyrate_limiter import AbstractBucket
@@ -37,29 +38,30 @@
     assert isinstance(limiter.bucket_factory.bucket, InMemoryBucket)
     assert limiter.bucket_factory.bucket.rates == DEFAULT_RATES
     assert limiter.bucket_factory.clock == clock
 
 
 @pytest.mark.asyncio
 async def test_limiter_constructor_02(
+    clock,
     create_bucket,
     limiter_should_raise,
     limiter_delay,
 ):
     bucket = await create_bucket(DEFAULT_RATES)
 
     limiter = Limiter(bucket)
     assert isinstance(limiter.bucket_factory, SingleBucketFactory)
     assert isinstance(limiter.bucket_factory.clock, TimeClock)
     assert limiter.max_delay is None
     assert limiter.raise_when_fail is True
 
     limiter = Limiter(
         bucket,
-        clock=TimeClock(),
+        clock=clock,
         raise_when_fail=limiter_should_raise,
         max_delay=limiter_delay,
     )
 
     assert isinstance(limiter.bucket_factory, BucketFactory)
     assert limiter.raise_when_fail == limiter_should_raise
     assert limiter.max_delay == limiter_delay
@@ -67,33 +69,34 @@
     acquire_ok = limiter.try_acquire("example")
 
     if isawaitable(acquire_ok):
         acquire_ok = await acquire_ok
 
     assert acquire_ok
 
-    factory = DemoBucketFactory(TimeClock(), demo=bucket)
+    factory = DemoBucketFactory(clock, demo=bucket)
     limiter = Limiter(
         factory,
         raise_when_fail=limiter_should_raise,
         max_delay=limiter_delay,
     )
     assert limiter.bucket_factory is factory
     assert limiter.raise_when_fail == limiter_should_raise
     assert limiter.max_delay == limiter_delay
 
 
 @pytest.mark.asyncio
 async def test_limiter_01(
+    clock,
     create_bucket,
     limiter_should_raise,
     limiter_delay,
 ):
     bucket = await create_bucket(DEFAULT_RATES)
-    factory = DemoBucketFactory(TimeClock(), demo=bucket)
+    factory = DemoBucketFactory(clock, demo=bucket)
     limiter = Limiter(
         factory,
         raise_when_fail=limiter_should_raise,
         max_delay=limiter_delay,
     )
     bucket = BucketAsyncWrapper(bucket)
     item = "demo"
@@ -162,21 +165,102 @@
     else:
         acquire_ok, cost = await async_acquire(limiter, item, 5)
         assert cost <= 50
         assert not acquire_ok
 
 
 @pytest.mark.asyncio
+async def test_limiter_async_factory_get(
+    clock,
+    limiter_should_raise,
+    limiter_delay,
+):
+    factory = DemoAsyncGetBucketFactory(clock)
+    limiter = Limiter(
+        factory,
+        raise_when_fail=limiter_should_raise,
+        max_delay=limiter_delay,
+    )
+    item = "demo"
+
+    logger.info("If weight = 0, it just passes thru")
+    acquire_ok, cost = await async_acquire(limiter, item, weight=0)
+    assert acquire_ok
+    assert cost <= 10
+
+    logger.info("Limiter Test #1")
+    await prefilling_bucket(limiter, 0.3, item)
+
+    if not limiter_should_raise:
+        acquire_ok, cost = await async_acquire(limiter, item)
+        if limiter_delay is None:
+            assert cost <= 50
+            assert not acquire_ok
+        else:
+            assert acquire_ok
+    else:
+        if limiter_delay is None:
+            with pytest.raises(BucketFullException):
+                acquire_ok, cost = await async_acquire(limiter, item)
+        else:
+            acquire_ok, cost = await async_acquire(limiter, item)
+            assert cost > 400
+            assert acquire_ok
+
+    # # Flush before testing again
+    await factory.flush()
+    logger.info("Limiter Test #2")
+    await prefilling_bucket(limiter, 0, item)
+
+    if limiter_should_raise:
+        if limiter_delay == 500:
+            with pytest.raises(LimiterDelayException) as err:
+                await async_acquire(limiter, item)
+                assert err.meta_info["max_delay"] == 500
+                assert err.meta_info["actual_delay"] > 600
+                assert err.meta_info["name"] == item
+        elif limiter_delay == 2000:
+            acquire_ok, cost = await async_acquire(limiter, item)
+            assert acquire_ok
+        elif limiter_delay == Duration.MINUTE:
+            acquire_ok, cost = await async_acquire(limiter, item)
+            assert acquire_ok
+        else:
+            with pytest.raises(BucketFullException) as err:
+                await async_acquire(limiter, item)
+    else:
+        acquire_ok, cost = await async_acquire(limiter, item)
+        if limiter_delay == 500 or limiter_delay is None:
+            assert not acquire_ok
+        else:
+            assert acquire_ok
+
+    # Flush before testing again
+    await factory.flush()
+    logger.info("Limiter Test #3: exceeding weight")
+    await prefilling_bucket(limiter, 0, item)
+
+    if limiter_should_raise:
+        with pytest.raises(BucketFullException) as err:
+            await async_acquire(limiter, item, 5)
+    else:
+        acquire_ok, cost = await async_acquire(limiter, item, 5)
+        assert cost <= 50
+        assert not acquire_ok
+
+
+@pytest.mark.asyncio
 async def test_limiter_concurrency(
+    clock,
     create_bucket,
     limiter_should_raise,
     limiter_delay,
 ):
     bucket: AbstractBucket = await create_bucket(DEFAULT_RATES)
-    factory = DemoBucketFactory(TimeClock(), demo=bucket)
+    factory = DemoBucketFactory(clock, demo=bucket)
     limiter = Limiter(
         factory,
         raise_when_fail=limiter_should_raise,
         max_delay=limiter_delay,
     )
 
     logger.info("Test Limiter Concurrency: inserting 4 items")
@@ -210,20 +294,21 @@
             result = await concurrent_acquire(limiter, items)
             item_names = await inspect_bucket_items(bucket, 4)
             logger.info("(Raise, delay) Result = %s, Item = %s", result, item_names)
 
 
 @pytest.mark.asyncio
 async def test_limiter_decorator(
+    clock,
     create_bucket,
     limiter_should_raise,
     limiter_delay,
 ):
     bucket = await create_bucket(DEFAULT_RATES)
-    factory = DemoBucketFactory(TimeClock(), demo=bucket)
+    factory = DemoBucketFactory(clock, demo=bucket)
     limiter = Limiter(
         factory,
         raise_when_fail=limiter_should_raise,
         max_delay=limiter_delay,
     )
     limiter_wrapper = limiter.as_decorator()
```

### Comparing `pyrate_limiter-3.6.0/tests/test_others.py` & `pyrate_limiter-3.6.1/tests/test_others.py`

 * *Files identical despite different names*

### Comparing `pyrate_limiter-3.6.0/PKG-INFO` & `pyrate_limiter-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrate-limiter
-Version: 3.6.0
+Version: 3.6.1
 Summary: Python Rate-Limiter using Leaky-Bucket Algorithm
 Home-page: https://github.com/vutran1710/PyrateLimiter
 License: MIT
 Keywords: rate,rate-limiter,rate_limiter,ratelimiter,leaky-bucket,ratelimit,ratelimiting
 Author: vutr
 Author-email: me@vutr.io
 Requires-Python: >=3.8,<4.0
```

