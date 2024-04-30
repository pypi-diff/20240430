# Comparing `tmp/pgqueuer-0.2.2.tar.gz` & `tmp/pgqueuer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.2.2.tar", last modified: Mon Apr 29 20:15:29 2024, max compression
+gzip compressed data, was "pgqueuer-0.2.3.tar", last modified: Tue Apr 30 21:07:23 2024, max compression
```

## Comparing `pgqueuer-0.2.2.tar` & `pgqueuer-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.288138 pgqueuer-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.280138 pgqueuer-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-29 20:15:29.288138 pgqueuer-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:15:29.288138 pgqueuer-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.288138 pgqueuer-0.2.2/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 20:15:29.000000 pgqueuer-0.2.2/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:15:29.284138 pgqueuer-0.2.2/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-29 20:15:19.000000 pgqueuer-0.2.2/tools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.492325 pgqueuer-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.492325 pgqueuer-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.492325 pgqueuer-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/tools/benchmark.py
```

### Comparing `pgqueuer-0.2.2/.github/workflows/ci.yml` & `pgqueuer-0.2.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/.github/workflows/linting.yml` & `pgqueuer-0.2.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/.github/workflows/release.yml` & `pgqueuer-0.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/.gitignore` & `pgqueuer-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/LICENSE` & `pgqueuer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/PKG-INFO` & `pgqueuer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.2.2
+Version: 0.2.3
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
@@ -26,21 +26,23 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anyio>=4.0
 Requires-Dist: asyncpg>=0.27.0
 Requires-Dist: pgcachewatch>=0.4
 Requires-Dist: pydantic>=2.0.0
+Requires-Dist: tabulate>=0.9.0
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: types-tabulate; extra == "dev"
 
 ##  🚀 PgQueuer - Building Smoother Workflows One Queue at a Time 🚀
 [![CI](https://github.com/janbjorge/PgQueuer/actions/workflows/ci.yml/badge.svg)](https://github.com/janbjorge/PgQueuer/actions/workflows/ci.yml?query=branch%3Amain)
 [![pypi](https://img.shields.io/pypi/v/PgQueuer.svg)](https://pypi.python.org/pypi/PgQueuer)
 [![downloads](https://static.pepy.tech/badge/PgQueuer/month)](https://pepy.tech/project/PgQueuer)
 [![versions](https://img.shields.io/pypi/pyversions/PgQueuer.svg)](https://github.com/janbjorge/PgQueuer)
```

### Comparing `pgqueuer-0.2.2/README.md` & `pgqueuer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/pyproject.toml` & `pgqueuer-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ]
 
 dependencies = [
     "anyio>=4.0",
     "asyncpg>=0.27.0",
     "pgcachewatch>=0.4",
     "pydantic>=2.0.0",
+    "tabulate>=0.9.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/janbjorge/PgQueuer/"
 Homepage = "https://github.com/janbjorge/PgQueuer/"
 Issues = "https://github.com/janbjorge/PgQueuer/issues"
 Repository = "https://github.com/janbjorge/PgQueuer/"
@@ -46,14 +47,15 @@
 dev = [
     "asyncpg-stubs",
     "mypy-extensions",
     "mypy",
     "pytest-asyncio",
     "pytest",
     "ruff",
+    "types-tabulate",
 ]
 
 [tool.setuptools_scm]
 write_to = "src/_version.py"
 
 [tool.ruff]
 line-length = 88
```

### Comparing `pgqueuer-0.2.2/src/PgQueuer/models.py` & `pgqueuer-0.2.3/src/PgQueuer/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import timedelta
 from typing import Literal
 
 from pydantic import AwareDatetime, BaseModel
 
 STATUS = Literal[
     "queued",
     "picked",
@@ -22,26 +23,28 @@
     priority: int
     created: AwareDatetime
     status: STATUS
     entrypoint: str
     payload: bytes | None
 
 
-class QueueSize(BaseModel):
+class QueueStatistics(BaseModel):
     """
     Represents the number of jobs per entrypoint and priority in the queue.
     """
 
     count: int
     entrypoint: str
     priority: int
 
 
-class LogSize(BaseModel):
+class LogStatistics(BaseModel):
     """
-    Represents log details for jobs based on status, entrypoint, and priority.
+    Represents log statistics for jobs based on status, entrypoint, and priority.
     """
 
     count: int
+    created: AwareDatetime
     entrypoint: str
     priority: int
     status: STATUS_LOG
+    time_in_queue: timedelta
```

### Comparing `pgqueuer-0.2.2/src/PgQueuer/qm.py` & `pgqueuer-0.2.3/src/PgQueuer/qm.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,16 +37,27 @@
 
 
 @overload
 def is_async_callable(obj: SyncEntrypoint) -> TypeGuard[SyncEntrypoint]: ...
 
 
 def is_async_callable(obj: object) -> bool:
-    # Inspired by:
-    # https://github.com/encode/starlette/blob/9f16bf5c25e126200701f6e04330864f4a91a898/starlette/_utils.py#L38
+    """
+    Determines whether an object is an asynchronous callable.
+    This function identifies objects that are either asynchronous coroutine functions
+    or have a callable __call__ method that is an asynchronous coroutine function.
+
+    The function handles functools.partial objects by evaluating the
+    underlying function. It supports overloads to ensure type-specific behavior
+    with AsyncEntrypoint and SyncEntrypoint types.
+
+    Inspired by:
+    https://github.com/encode/starlette/blob/9f16bf5c25e126200701f6e04330864f4a91a898/starlette/_utils.py#L38
+    """
+
     while isinstance(obj, functools.partial):
         obj = obj.func
 
     return asyncio.iscoroutinefunction(obj) or (
         callable(obj) and asyncio.iscoroutinefunction(obj.__call__)
     )
 
@@ -56,40 +67,35 @@
     """
     Manages job queues and dispatches jobs to registered entry points,
     handling database connections and events.
     """
 
     pool: asyncpg.Pool
     queries: Queries = dataclasses.field(init=False)
-    channel: PGChannel = dataclasses.field(
-        default=PGChannel(DBSettings().channel),
-    )
-    alive: bool = dataclasses.field(
-        init=False,
-        default=True,
-    )
+    channel: PGChannel = dataclasses.field(default=PGChannel(DBSettings().channel))
+    alive: bool = dataclasses.field(init=False, default=True)
+
     # Should registry be a weakref?
     registry: dict[str, Entrypoint] = dataclasses.field(
-        init=False,
-        default_factory=dict,
+        init=False, default_factory=dict
     )
 
     def __post_init__(self) -> None:
         """
         Initializes database query handlers and validates pool size upon
         instance creation.
         """
         if self.pool.get_min_size() < 1:
             raise ValueError("... min size must be gt 1.")
         self.queries = Queries(self.pool)
 
     def entrypoint(self, name: str) -> Callable[[T], T]:
         """
-        Decorator to register a function as an entrypoint for
-        handling specific job types.
+        Registers a function as an entrypoint for handling specific
+        job types. Ensures unique naming in the registry.
         """
 
         if name in self.registry:
             raise RuntimeError(f"{name} already in registry, name must be unique.")
 
         def register(func: T) -> T:
             self.registry[name] = func
@@ -98,26 +104,27 @@
         return register
 
     async def run(
         self,
         dequeue_timeout: timedelta = timedelta(seconds=30),
     ) -> None:
         """
-        Starts the event listener and continuously dispatches jobs to
-        registered entry points until stopped.
+        Continuously listens for events and dispatches jobs. Manages connections and
+        tasks, logs timeouts, and resets connections upon termination.
         """
+
         async with (
             self.pool.acquire() as conn,
             TaskManager() as tm,
         ):
             listener = PGEventQueue()
             await listener.connect(conn, self.channel)
 
             while self.alive:
-                while self.alive and (job := await self.queries.dequeue()):
+                while job := await self.queries.dequeue():
                     tm.add(asyncio.create_task(self._dispatch(job)))
 
                 try:
                     await asyncio.wait_for(
                         listener.get(),
                         timeout=dequeue_timeout.total_seconds(),
                     )
@@ -127,16 +134,16 @@
                         dequeue_timeout,
                     )
 
             await conn.reset()
 
     async def _dispatch(self, job: Job) -> None:
         """
-        Internal method to asynchronously handle job dispatch,
-        including exception logging and job status updates.
+        Handles asynchronous job dispatch. Logs exceptions, updates job status,
+        and adapts execution method based on whether the job's function is asynchronous.
         """
 
         logger.debug(
             "Dispatching entrypoint/id: %s/%s",
             job.entrypoint,
             job.id,
         )
```

### Comparing `pgqueuer-0.2.2/src/PgQueuer/tm.py` & `pgqueuer-0.2.3/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/src/PgQueuer.egg-info/PKG-INFO` & `pgqueuer-0.2.3/src/PgQueuer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.2.2
+Version: 0.2.3
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
@@ -26,21 +26,23 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anyio>=4.0
 Requires-Dist: asyncpg>=0.27.0
 Requires-Dist: pgcachewatch>=0.4
 Requires-Dist: pydantic>=2.0.0
+Requires-Dist: tabulate>=0.9.0
 Provides-Extra: dev
 Requires-Dist: asyncpg-stubs; extra == "dev"
 Requires-Dist: mypy-extensions; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: types-tabulate; extra == "dev"
 
 ##  🚀 PgQueuer - Building Smoother Workflows One Queue at a Time 🚀
 [![CI](https://github.com/janbjorge/PgQueuer/actions/workflows/ci.yml/badge.svg)](https://github.com/janbjorge/PgQueuer/actions/workflows/ci.yml?query=branch%3Amain)
 [![pypi](https://img.shields.io/pypi/v/PgQueuer.svg)](https://pypi.python.org/pypi/PgQueuer)
 [![downloads](https://static.pepy.tech/badge/PgQueuer/month)](https://pepy.tech/project/PgQueuer)
 [![versions](https://img.shields.io/pypi/pyversions/PgQueuer.svg)](https://github.com/janbjorge/PgQueuer)
```

### Comparing `pgqueuer-0.2.2/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.2.3/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/test/conftest.py` & `pgqueuer-0.2.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/test/db/Dockerfile` & `pgqueuer-0.2.3/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/test/test_qm.py` & `pgqueuer-0.2.3/test/test_qm.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,19 @@
     async def fetch(context: Job) -> None:
         if context.payload is None:
             c.alive = False
             return
         assert context
         seen.append(int(context.payload))
 
-    for n in range(N):
-        await c.queries.enqueue("fetch", f"{n}".encode())
+    await c.queries.enqueue(
+        ["fetch"] * N,
+        [f"{n}".encode() for n in range(N)],
+        [0] * N,
+    )
 
     # Stop flag
     await c.queries.enqueue("fetch", None)
 
     await asyncio.wait_for(c.run(), timeout=1)
     assert seen == list(range(N))
 
@@ -52,16 +55,19 @@
             if context.payload is None:
                 for qm in qmpool:
                     qm.alive = False
                 return
             assert context
             seen.append(int(context.payload))
 
-    for n in range(N):
-        await q.enqueue("fetch", f"{n}".encode())
+    await q.enqueue(
+        ["fetch"] * N,
+        [f"{n}".encode() for n in range(N)],
+        [0] * N,
+    )
 
     # Stop flag
     await q.enqueue("fetch", None)
 
     await asyncio.wait_for(
         asyncio.gather(*[qm.run() for qm in qmpool]),
         timeout=10,
@@ -88,16 +94,19 @@
             if context.payload is None:
                 for qm in qmpool:
                     qm.alive = False
                 return
             assert context
             seen.append(int(context.payload))
 
-    for n in range(N):
-        await q.enqueue("fetch", f"{n}".encode())
+    await q.enqueue(
+        ["fetch"] * N,
+        [f"{n}".encode() for n in range(N)],
+        [0] * N,
+    )
 
     # Stop flag
     await q.enqueue("fetch", None)
 
     await asyncio.wait_for(
         asyncio.gather(*[qm.run() for qm in qmpool]),
         timeout=10,
```

### Comparing `pgqueuer-0.2.2/test/test_tm.py` & `pgqueuer-0.2.3/test/test_tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.2/tools/benchmark.py` & `pgqueuer-0.2.3/tools/benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 
 async def jobs_per_second(pool: asyncpg.Pool) -> float:
     qm = QueueManager(pool)
     seen = 0
 
     @qm.entrypoint("async")
     async def asyncfetch(job: Job) -> None:
-        nonlocal qm, seen
+        nonlocal seen
         seen += 1
         if job.payload is None:
             qm.alive = False
 
     @qm.entrypoint("sync")
     def syncfetch(job: Job) -> None:
-        nonlocal qm, seen
+        nonlocal seen
         seen += 1
         if job.payload is None:
             qm.alive = False
 
     with timer() as elapsed:
         await qm.run(timedelta(seconds=0))
 
@@ -53,47 +53,49 @@
 async def benchmark(
     entrypoint: str,
     concurrecy: int,
     N: int,
     pool: asyncpg.Pool,
 ) -> None:
     queries = Queries(pool)
-
-    await queries.clear_log()
-    await queries.clear_queue()
-
     await queries.enqueue(
         [entrypoint] * N,
         [f"{n}".encode() for n in range(N)],
         [0] * N,
     )
-    assert sum(x.count for x in await queries.queue_size()) == N
 
     await queries.enqueue(
         [entrypoint] * concurrecy**2,
         [None] * concurrecy**2,
         [0] * concurrecy**2,
     )
 
-    jobs = [jobs_per_second(pool) for _ in range(concurrecy)]
-    results = await asyncio.gather(*jobs)
+    jps = sum(
+        await asyncio.gather(
+            *[jobs_per_second(pool) for _ in range(concurrecy)],
+        )
+    )
 
     print(
         f"Entrypoint: {entrypoint:<5} ",
-        f"Concurrecy: {concurrecy:<2} "
-        f"Jobs: {N:<5} "
-        f"JPS: {sum(results)/1_000:.1f}k",
+        f"Concurrecy: {concurrecy:<2} ",
+        f"Jobs: {N:<5} ",
+        f"JPS: {jps/1_000:.1f}k",
     )
 
 
 async def main() -> None:
     async with asyncpg.create_pool(
         min_size=20,
         max_size=99,
     ) as pool:
+        queries = Queries(pool)
+        await queries.clear_log()
+        await queries.clear_queue()
         for entrypoint in ("sync", "async"):
             for concurrecy in range(1, 6):
-                await benchmark(entrypoint, concurrecy, 1_000 * concurrecy, pool)
+                await benchmark(entrypoint, concurrecy, concurrecy * 1_000, pool)
+                await asyncio.sleep(0)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

