# Comparing `tmp/pyxxl-0.3.4.tar.gz` & `tmp/pyxxl-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxxl-0.3.4.tar", max compression
+gzip compressed data, was "pyxxl-0.3.5.tar", max compression
```

## Comparing `pyxxl-0.3.4.tar` & `pyxxl-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35149 2023-11-29 08:52:45.880423 pyxxl-0.3.4/LICENSE
--rw-r--r--   0        0        0     4363 2023-11-29 08:52:45.880423 pyxxl-0.3.4/README.md
--rw-r--r--   0        0        0     2147 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      178 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/__init__.py
--rw-r--r--   0        0        0     1041 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/ctx.py
--rw-r--r--   0        0        0      259 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/enum.py
--rw-r--r--   0        0        0      984 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/error.py
--rw-r--r--   0        0        0    12132 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/executor.py
--rw-r--r--   0        0        0       82 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/logger/__init__.py
--rw-r--r--   0        0        0     1420 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/logger/common.py
--rw-r--r--   0        0        0     5026 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/logger/disk.py
--rw-r--r--   0        0        0     4248 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/logger/redis.py
--rw-r--r--   0        0        0     5137 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/main.py
--rw-r--r--   0        0        0     2526 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/prometheus.py
--rw-r--r--   0        0        0      764 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/schema.py
--rw-r--r--   0        0        0     3603 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/server.py
--rw-r--r--   0        0        0     5415 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/setting.py
--rw-r--r--   0        0        0        0 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/api/__init__.py
--rw-r--r--   0        0        0      669 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/api/test_metrics.py
--rw-r--r--   0        0        0     2774 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/api/test_server.py
--rw-r--r--   0        0        0     2122 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/conftest.py
--rw-r--r--   0        0        0     1640 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/test_client.py
--rw-r--r--   0        0        0      905 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/test_context.py
--rw-r--r--   0        0        0     6572 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/test_executor.py
--rw-r--r--   0        0        0     1391 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/test_handler.py
--rw-r--r--   0        0        0     3697 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/test_logger.py
--rw-r--r--   0        0        0      859 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/test_register.py
--rw-r--r--   0        0        0     1896 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/test_setting.py
--rw-r--r--   0        0        0      129 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/test_utils.py
--rw-r--r--   0        0        0      872 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/tests/utils.py
--rw-r--r--   0        0        0      395 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/types.py
--rw-r--r--   0        0        0     2160 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/utils.py
--rw-r--r--   0        0        0     4116 2023-11-29 08:52:45.884423 pyxxl-0.3.4/pyxxl/xxl_client.py
--rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 pyxxl-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 06:58:04.446839 pyxxl-0.3.5/LICENSE
+-rw-r--r--   0        0        0     4407 2024-04-30 06:58:04.450840 pyxxl-0.3.5/README.md
+-rw-r--r--   0        0        0     2120 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      178 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/__init__.py
+-rw-r--r--   0        0        0     1056 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/ctx.py
+-rw-r--r--   0        0        0      259 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/enum.py
+-rw-r--r--   0        0        0      984 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/error.py
+-rw-r--r--   0        0        0    12285 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/executor.py
+-rw-r--r--   0        0        0      452 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/logger/__init__.py
+-rw-r--r--   0        0        0     1502 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/logger/common.py
+-rw-r--r--   0        0        0     4500 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/logger/disk.py
+-rw-r--r--   0        0        0     4268 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/logger/redis.py
+-rw-r--r--   0        0        0     5407 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/main.py
+-rw-r--r--   0        0        0     2526 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/prometheus.py
+-rw-r--r--   0        0        0      764 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/schema.py
+-rw-r--r--   0        0        0     3491 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/server.py
+-rw-r--r--   0        0        0     5511 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/setting.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/api/__init__.py
+-rw-r--r--   0        0        0      669 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/api/test_metrics.py
+-rw-r--r--   0        0        0     2774 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/api/test_server.py
+-rw-r--r--   0        0        0     2122 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/conftest.py
+-rw-r--r--   0        0        0     1640 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/test_client.py
+-rw-r--r--   0        0        0      905 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/test_context.py
+-rw-r--r--   0        0        0     6572 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/test_executor.py
+-rw-r--r--   0        0        0     1391 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/test_handler.py
+-rw-r--r--   0        0        0     3697 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/test_logger.py
+-rw-r--r--   0        0        0      859 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/test_register.py
+-rw-r--r--   0        0        0     1896 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/test_setting.py
+-rw-r--r--   0        0        0      129 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/test_utils.py
+-rw-r--r--   0        0        0      882 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/tests/utils.py
+-rw-r--r--   0        0        0      395 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/types.py
+-rw-r--r--   0        0        0     2160 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/utils.py
+-rw-r--r--   0        0        0     4126 2024-04-30 06:58:04.454840 pyxxl-0.3.5/pyxxl/xxl_client.py
+-rw-r--r--   0        0        0     5541 1970-01-01 00:00:00.000000 pyxxl-0.3.5/PKG-INFO
```

### Comparing `pyxxl-0.3.4/LICENSE` & `pyxxl-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/README.md` & `pyxxl-0.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,26 +25,29 @@
 * 任务的管理（支持在界面上取消，发起等操作，任务完成后会回调admin）
 * 所有阻塞策略的支持
 * 异步支持（推荐）
 * job-admin上查看日志
 
 ## 适配的XXL-JOB版本
 
-* XXL-JOB:2.3.0
+**2.4.0**,**2.3.0**,**2.2.0**
 
-如遇到不兼容的情况请issue告诉我XXL-JOB版本我会尽量适配
+如遇到不兼容的情况请issue告诉我XXL-JOB版本和对应的问题我会尽量适配
 
 ## 如何使用
 
 ```shell
 pip install pyxxl
+
 # 如果日志需要写入redis
 pip install "pyxxl[redis]"
+
 # 如果需要从.env加载配置
 pip install "pyxxl[dotenv]"
+
 # 安装所有功能
 pip install "pyxxl[all]"
 ```
 
 ```python
 import asyncio
 
@@ -135,9 +138,9 @@
 
 
 ```shell
 # if you need. set venv in project.
 # poetry config virtualenvs.in-project true
 poetry install --all-extras
 # 修改app.py中相关的配置信息,然后启动
-poetry run python example/app.py
+poetry run python example/executor_app.py
 ```
```

### Comparing `pyxxl-0.3.4/pyproject.toml` & `pyxxl-0.3.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 [tool.poetry]
 authors = ["fcfangcc <swjfc22@live.com>"]
-classifiers = [
-  "Topic :: Software Development :: Libraries :: Python Modules",
-]
+classifiers = ["Topic :: Software Development :: Libraries :: Python Modules"]
 description = "A Python executor for XXL-jobs"
 keywords = ["XXL"]
 license = "GPL-3.0-only"
 name = "pyxxl"
 readme = "README.md"
 repository = "https://github.com/fcfangcc/pyxxl"
-version = "0.3.4"
+version = "0.3.5"
 
 [tool.poetry.dependencies]
 aiofiles = "^22.1.0"
 aiohttp = "^3.8.1"
-prometheus-client = {version = "*", optional = true}
+prometheus-client = { version = "*", optional = true }
 python = "^3.9"
-python-dotenv = {version = "*", optional = true}
-redis = {version = "^4.4.0", optional = true}
+python-dotenv = { version = "*", optional = true }
+redis = { version = "^4.4.0", optional = true }
 
 [tool.poetry.extras]
 all = ["redis", "python-dotenv", "prometheus-client"]
 dotenv = ["python-dotenv"]
 metrics = ["prometheus-client"]
 redis = ["redis"]
 
 [tool.poetry.group.doc.dependencies]
 mdx-include = "^1.4.2"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.0.9"
-mkdocstrings = {version = "^0.20.0", extras = ["python"]}
+mkdocstrings = { version = "^0.20.0", extras = ["python"] }
 
 [tool.poetry.group.dev.dependencies]
 black = "23.1.0"
-mypy = "0.942"
-pre-commit = "2.19.0"
+mypy = "^1.8.0"
+pre-commit = "^3.6.0"
 pytest = "7.1.2"
 pytest-aiohttp = "1.0.4"
 pytest-asyncio = "0.18.3"
 pytest-cov = "3.0.0"
-ruff = "^0.0.249"
+ruff = "^0.1.9"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 # if your need
 # https://python-poetry.org/docs/repositories/#install-dependencies-from-a-private-repository
@@ -55,18 +53,15 @@
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.mypy]
 disallow_untyped_defs = true
-exclude = [
-  '^pyxxl/tests/test_.*\.py$',
-  '^pyxxl/tests/api/test_.*\.py$',
-]
+exclude = ['^pyxxl/tests/test_.*\.py$', '^pyxxl/tests/api/test_.*\.py$']
 files = "pyxxl"
 ignore_missing_imports = true
 
 [tool.coverage.run]
 concurrency = ["thread"]
 
 [tool.coverage.report]
@@ -79,27 +74,17 @@
 ]
 
 [tool.black]
 line-length = 119
 target-version = ['py39']
 
 [tool.ruff]
-exclude = [
-  "__init__.py",
-]
+exclude = ["__init__.py"]
 line-length = 119
-select = [
-  "E",
-  "W",
-  "F",
-  "I",
-  "C",
-  "B",
-  "PGH",
-]
+select = ["E", "W", "F", "I", "C", "B", "PGH"]
 
 ignore = [
   "C408", # Unnecessary `dict` call (rewrite as a literal)
 ]
 
 [tool.pytest.ini_options]
 addopts = "--asyncio-mode auto"
```

### Comparing `pyxxl-0.3.4/pyxxl/ctx.py` & `pyxxl-0.3.5/pyxxl/ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import threading
-from contextvars import ContextVar
+from contextvars import ContextVar, Token
 from typing import Any, Optional
 
 from pyxxl.schema import RunData
 
 
 class GlobalVars:
     _DATA: ContextVar = ContextVar("_DATA")
@@ -20,16 +20,16 @@
         return cls._DATA.get(None)
 
     @property
     def xxl_run_data(self) -> RunData:
         return self._DATA.get()
 
     @classmethod
-    def set_task_logger(cls, logger: logging.Logger) -> None:
-        cls._LOGGER.set(logger)
+    def set_task_logger(cls, logger: logging.Logger) -> Token:
+        return cls._LOGGER.set(logger)
 
     @property
     def logger(self) -> logging.Logger:  # pragma: no cover
         return self._LOGGER.get()
 
     @classmethod
     def set_cancel_event(cls, event: threading.Event) -> None:
```

### Comparing `pyxxl-0.3.4/pyxxl/error.py` & `pyxxl-0.3.5/pyxxl/error.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/executor.py` & `pyxxl-0.3.5/pyxxl/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, MutableSet, Optional
 
 from pyxxl import error
 from pyxxl.ctx import g
 from pyxxl.enum import executorBlockStrategy
-from pyxxl.logger import DiskLog, LogBase
+from pyxxl.logger import DiskLog, LogBase, new_logger
 from pyxxl.schema import RunData
 from pyxxl.setting import ExecutorConfig
 from pyxxl.types import DecoratedCallable
 from pyxxl.xxl_client import XXL
 
 logger = logging.getLogger(__name__)
 # https://docs.python.org/3.10/library/asyncio-task.html#asyncio.create_task
@@ -82,15 +82,15 @@
             if handler_name in self._handlers and replace is False:
                 raise error.JobRegisterError("handler %s already registered." % handler_name)
             handler = HandlerInfo(handler=func)
             if not handler.is_async:
                 warnings.warn(
                     "Using the sync method will unknown blocking exception, consider using async method.",
                     SyntaxWarning,
-                    2,
+                    stacklevel=2,
                 )
             self._handlers[handler_name] = handler
             logger.debug("register job %s,is async: %s" % (handler_name, asyncio.iscoroutinefunction(func)))
 
             return func
 
         if len(args) == 1:
@@ -214,43 +214,43 @@
     async def is_running(self, job_id: int) -> bool:
         return job_id in self.tasks
 
     async def _run(self, data: RunData) -> None:
         handler = self.handler.get(data.executorHandler)
         assert handler
         g.set_xxl_run_data(data)
-        g.set_task_logger(self.logger_factory.get_logger(data.logId))
-        start_time = int(time.time() * 1000)
-        try:
-            g.logger.info("Start job jobId=%s logId=%s [%s]" % (data.jobId, data.logId, data))
-            timeout = data.executorTimeout or self.config.task_timeout
-            result = await handler.start(timeout)
-            g.logger.info("Job finished jobId=%s logId=%s" % (data.jobId, data.logId))
-            await self.xxl_client.callback(data.logId, start_time, code=200, msg=result)
-            self.successed_callback()
-        except asyncio.CancelledError as e:
-            g.logger.info(e, exc_info=True)
-            await self.xxl_client.callback(data.logId, start_time, code=500, msg="CancelledError")
-            self.failed_callback("cancelled")
-        except asyncio.exceptions.TimeoutError as e:
-            # 同步任务run_in_executor超时会抛出TimeoutError异常
-            # !!! 但是注意线程里面的任务仍然在运行，可能会占满所有的线程池
-            g.logger.warning(e, exc_info=True)
-            await self.xxl_client.callback(data.logId, start_time, code=500, msg="TimeoutError")
-            self.failed_callback("timeout")
-        except Exception as err:  # pylint: disable=broad-except
-            g.logger.exception(err, exc_info=True)
-            await self.xxl_client.callback(data.logId, start_time, code=500, msg=str(err))
-            self.failed_callback("exception")
-        finally:
-            if self.lock.locked():
-                await self._finish(data.jobId)
-            else:
-                async with self.lock:
+        with new_logger(self.logger_factory, data.logId) as task_logger:
+            start_time = int(time.time() * 1000)
+            try:
+                task_logger.info("Start job jobId=%s logId=%s [%s]" % (data.jobId, data.logId, data))
+                timeout = data.executorTimeout or self.config.task_timeout
+                result = await handler.start(timeout)
+                task_logger.info("Job finished jobId=%s logId=%s" % (data.jobId, data.logId))
+                await self.xxl_client.callback(data.logId, start_time, code=200, msg=result)
+                self.successed_callback()
+            except asyncio.CancelledError as e:
+                task_logger.info(e, exc_info=True)
+                await self.xxl_client.callback(data.logId, start_time, code=500, msg="CancelledError")
+                self.failed_callback("cancelled")
+            except asyncio.exceptions.TimeoutError as e:
+                # 同步任务run_in_executor超时会抛出TimeoutError异常
+                # !!! 但是注意线程里面的任务仍然在运行，可能会占满所有的线程池
+                task_logger.warning(e, exc_info=True)
+                await self.xxl_client.callback(data.logId, start_time, code=500, msg="TimeoutError")
+                self.failed_callback("timeout")
+            except Exception as err:  # pylint: disable=broad-except
+                task_logger.exception(err, exc_info=True)
+                await self.xxl_client.callback(data.logId, start_time, code=500, msg=str(err))
+                self.failed_callback("exception")
+            finally:
+                if self.lock.locked():
                     await self._finish(data.jobId)
+                else:
+                    async with self.lock:
+                        await self._finish(data.jobId)
 
     async def _finish(self, job_id: int) -> None:
         # 所有移除tasks的操作全部在这里执行
         finish_task = self.tasks.pop(job_id, None)
         logger.info("Finish task {}".format(finish_task))
         queue = self.get_queue(job_id)
         if not queue.empty():
```

### Comparing `pyxxl-0.3.4/pyxxl/logger/common.py` & `pyxxl-0.3.5/pyxxl/logger/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,7 +42,10 @@
         Args:
             seconds (int, optional): one loop seconds. Defaults to 3600.
         """
         logger.debug("start expired_loop...")
         while True:
             await self.expired_once()
             await asyncio.sleep(seconds)
+
+    def after_running(self, logger: logging.Logger) -> None:
+        return None
```

### Comparing `pyxxl-0.3.4/pyxxl/logger/disk.py` & `pyxxl-0.3.5/pyxxl/logger/disk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import os
 import time
-import weakref
 from contextlib import asynccontextmanager
 from logging import FileHandler
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, AsyncGenerator, List
+from typing import TYPE_CHECKING, Any, AsyncGenerator, List, Optional
 
 import aiofiles
 
 from pyxxl.types import LogRequest, LogResponse
 from pyxxl.utils import STD_FORMATTER
 
 from .common import LogBase
@@ -20,70 +19,39 @@
 
 LOG_NAME_PREFIX = "pyxxl-{log_id}.log"
 LOG_NAME_REGEX = "pyxxl-*.log"
 MAX_LOG_TAIL_LINES = 1000
 logger = logging.getLogger(__name__)
 
 
-def _close_file_stream(_logger: logging.Logger) -> None:
-    # !!! StreamHandler remove会有问题，需要判断是否是FileHandler
-    for h in _logger.handlers:
-        if isinstance(h, logging.FileHandler):
-            logger.debug("close file log object: {}.".format(h))
-            h.close()
-            _logger.removeHandler(h)
-
-
-class XXLogger:
-    """为了可以关闭文件写入流"""
-
-    def __init__(self, logger: logging.Logger) -> None:
-        self._logger = logger
-
-        self._finalizer = weakref.finalize(self, _close_file_stream, self._logger)
-
-    def remove(self) -> None:
-        self._finalizer()
-
-    @property
-    def removed(self) -> bool:
-        return not self._finalizer.alive
-
-    def __getattr__(self, name: str) -> Any:
-        if name in ["info", "error", "warning", "debug", "exception", "handlers"]:
-            return getattr(self._logger, name)
-
-
 class DiskLog(LogBase):
     def __init__(self, log_path: str, log_tail_lines: int = 0, expired_days: int = 14) -> None:
         self.log_path = Path(log_path)
         if not self.log_path.exists():
             self.log_path.mkdir()  # pragma: no cover
             logger.info("create logdir %s" % self.log_path)  # pragma: no cover
         self.log_tail_lines = log_tail_lines or MAX_LOG_TAIL_LINES
         self.expired_days = expired_days
 
     def key(self, log_id: int) -> str:
         return self.log_path.joinpath(LOG_NAME_PREFIX.format(log_id=log_id)).absolute().as_posix()
 
-    def get_logger(  # type:ignore[override]
-        self, log_id: int, *, stdout: bool = True, level: int = logging.INFO
-    ) -> XXLogger:
+    def get_logger(self, log_id: int, *, stdout: bool = True, level: int = logging.INFO) -> logging.Logger:
         logger = logging.getLogger("pyxxl-task-{%s}" % log_id)
         logger.propagate = False
         logger.setLevel(level)
         handlers: list[Handler] = [logging.StreamHandler()] if stdout else []
         handlers.append(FileHandler(self.key(log_id), delay=True))
         for h in handlers:
             h.setFormatter(STD_FORMATTER)
             h.setLevel(level)
             logger.addHandler(h)
-        return XXLogger(logger)
+        return logger
 
-    async def get_logs(self, request: LogRequest, *, key: str = None) -> LogResponse:
+    async def get_logs(self, request: LogRequest, *, key: Optional[str] = None) -> LogResponse:
         # todo: 优化获取中间行的逻辑，缓存之前每行日志的大小然后直接seek
         logs = ""
         to_line_num = request["fromLineNum"]  # start with 1
         is_end = False
         key = key or self.key(request["logId"])
         try:
             async with aiofiles.open(key, mode="r") as f:
@@ -102,15 +70,15 @@
         return LogResponse(
             fromLineNum=request["fromLineNum"],
             toLineNum=to_line_num,
             logContent=logs,
             isEnd=is_end,
         )
 
-    async def read_task_logs(self, log_id: int, *, key: str = None) -> str:
+    async def read_task_logs(self, log_id: int, *, key: Optional[str] = None) -> str:
         key = key or self.key(log_id)
         async with aiofiles.open(key, mode="r") as f:
             return await f.read()
 
     async def expired_once(self) -> None:
         now = time.time()
         expire_timestamp = now - 3600 * 24 * self.expired_days
@@ -135,7 +103,15 @@
             yield str(f.name)
 
     @asynccontextmanager
     async def mock_logger(self, _log_id: int) -> AsyncGenerator[LogBase, None]:
         async with aiofiles.tempfile.TemporaryDirectory() as d:
             handler = DiskLog(log_path=d)
             yield handler
+
+    def after_running(self, logger: logging.Logger) -> None:
+        # !!! StreamHandler remove会有问题，需要判断是否是FileHandler
+        file_handlers = [h for h in logger.handlers if isinstance(h, logging.FileHandler)]
+        for fh in file_handlers:
+            logger.debug("close file log object: {}.".format(fh))
+            fh.close()
+            logger.removeHandler(fh)
```

### Comparing `pyxxl-0.3.4/pyxxl/logger/redis.py` & `pyxxl-0.3.5/pyxxl/logger/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,20 +81,20 @@
             h.setLevel(level)
             logger.addHandler(h)
         return logger
 
     def key(self, log_id: int) -> str:
         return KEY_PREFIX.format(app=self.app, log_id=log_id)
 
-    async def read_task_logs(self, log_id: int, *, key: str = None) -> str:
+    async def read_task_logs(self, log_id: int, *, key: Optional[str] = None) -> str:
         key = key or self.key(log_id)
         # todo: use async
         return "".join(i.decode() for i in self.rclient.lrange(key, 0, -1))
 
-    async def get_logs(self, request: LogRequest, *, key: str = None) -> LogResponse:
+    async def get_logs(self, request: LogRequest, *, key: Optional[str] = None) -> LogResponse:
         key = key or self.key(request["logId"])
         from_line = request["fromLineNum"] - 1
         to_line = request["fromLineNum"] - 1 + self.log_tail_lines
         llen = self.rclient.llen(key)
         if from_line >= llen:
             logs = "No such logid logs." if llen == 0 else ""
             to_line_num = request["fromLineNum"]
```

### Comparing `pyxxl-0.3.4/pyxxl/main.py` & `pyxxl-0.3.5/pyxxl/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import functools
 import logging
+import os
 from multiprocessing import Process
 from typing import Any, AsyncGenerator, Optional
 
 from aiohttp import web
 
 from pyxxl.executor import Executor, JobHandler
 from pyxxl.logger import DiskLog, LogBase, RedisLog
@@ -21,14 +22,21 @@
     Executor: Executor = functools.partial(  # type: ignore[no-redef]
         Executor,
         successed_callback=prometheus.success,
         failed_callback=prometheus.failed,
     )
 
 
+async def server_info_ctx(app: web.Application) -> AsyncGenerator:
+    pid = os.getpid()
+    logger.info(f"start executor server with pid {pid}.")
+    yield
+    logger.info(f"stop executor server. pid={pid}.")
+
+
 class PyxxlRunner:
     daemon: Optional[Process] = None
 
     def __init__(
         self,
         config: ExecutorConfig,
         handler: Optional[JobHandler] = None,
@@ -112,14 +120,15 @@
         await xxl_client.close()
         logger.info("cleanup executor success.")
 
     def create_server_app(self) -> web.Application:
         """获取执行器的app对象,可以使用自己喜欢的服务器启动这个webapp"""
         app = create_app()
         app.cleanup_ctx.append(self._cleanup_ctx)
+        app.cleanup_ctx.append(server_info_ctx)
         return app
 
     def run_executor(self, handle_signals: bool = True) -> None:
         """用aiohttp的web服务器启动执行器"""
         web.run_app(
             self.create_server_app(),
             port=self.config.executor_listen_port,
```

### Comparing `pyxxl-0.3.4/pyxxl/prometheus.py` & `pyxxl-0.3.5/pyxxl/prometheus.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/schema.py` & `pyxxl-0.3.5/pyxxl/schema.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/server.py` & `pyxxl-0.3.5/pyxxl/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,27 +30,27 @@
         return web.json_response(dict(code=500, msg="job %s is running." % job_id))
     return web.json_response(dict(code=200, msg=None))
 
 
 @routes.post("/run")
 async def run(request: web.Request) -> web.Response:
     """
-        {
-        "jobId":1,                                  // 任务ID
-        "executorHandler":"demoJobHandler",         // 任务标识
-        "executorParams":"demoJobHandler",          // 任务参数
-        "executorBlockStrategy":"COVER_EARLY",      // 任务阻塞策略，可选值参考 com.xxl.job.core.enums.ExecutorBlockStrategyEnum
-        "executorTimeout":0,                        // 任务超时时间，单位秒，大于零时生效
-        "logId":1,                                  // 本次调度日志ID
-        "logDateTime":1586629003729,                // 本次调度日志时间
-        "glueType":"BEAN",                          // 任务模式，可选值参考 com.xxl.job.core.glue.GlueTypeEnum
-        "glueSource":"xxx",                         // GLUE脚本代码
-        "glueUpdatetime":1586629003727,             // GLUE脚本更新时间，用于判定脚本是否变更以及是否需要刷新
-        "broadcastIndex":0,                         // 分片参数：当前分片
-        "broadcastTotal":0                          // 分片参数：总分片
+    {
+    "jobId":1,                             // 任务ID
+    "executorHandler":"demoJobHandler",    // 任务标识
+    "executorParams":"demoJobHandler",     // 任务参数
+    "executorBlockStrategy":"COVER_EARLY", // 任务阻塞策略，可选值参考 com.xxl.job.core.enums.ExecutorBlockStrategyEnum
+    "executorTimeout":0,                   // 任务超时时间，单位秒，大于零时生效
+    "logId":1,                             // 本次调度日志ID
+    "logDateTime":1586629003729,           // 本次调度日志时间
+    "glueType":"BEAN",                     // 任务模式，可选值参考 com.xxl.job.core.glue.GlueTypeEnum
+    "glueSource":"xxx",                    // GLUE脚本代码
+    "glueUpdatetime":1586629003727,        // GLUE脚本更新时间，用于判定脚本是否变更以及是否需要刷新
+    "broadcastIndex":0,                    // 分片参数：当前分片
+    "broadcastTotal":0                     // 分片参数：总分片
     }
     """
     data = await request.json()
     run_data = RunData(**data)
     logger.info("Get task request. jobId=%s logId=%s [%s]" % (run_data.jobId, run_data.logId, run_data))
     msg = None
     try:
```

### Comparing `pyxxl-0.3.4/pyxxl/setting.py` & `pyxxl-0.3.5/pyxxl/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import logging
 import os
 from dataclasses import asdict, dataclass, field
-from typing import Literal, Optional
+from typing import Any, Literal, Optional, get_origin
 
 from yarl import URL
 
 from pyxxl.utils import get_network_ip, setup_logging
 
 logger = logging.getLogger(__name__)
 
@@ -32,15 +32,18 @@
     """调度器的token. Default: None"""
 
     executor_log_path: str = "pyxxl.log"
     """执行器日志输出的路径(注意路径必须存在). Default: pyxxl.log"""
     executor_port: int = 9999
     """执行器绑定的http服务的端口,作用同host. Default: 9999"""
     executor_host: str = field(default_factory=get_network_ip)
-    """执行器绑定的host,xxl-admin通过这个host来回调pyxxl执行器,如果不填会默认取第一个网卡的地址. Default: 获取到第一个网卡的ip地址"""
+    """
+    执行器绑定的host,xxl-admin通过这个host来回调pyxxl执行器,如果不填会默认取第一个网卡的地址.
+    Default: 获取到第一个网卡的ip地址
+    """
     executor_listen_port: int = 0
     """Default: executor_port"""
     executor_listen_host: str = ""
     """
     执行器HTTP服务绑定的HOST,大部分情况下不需要设置. Default: executor_host
 
     当执行器通过了端口转发暴露给admin的时候,需要把executor_host填写为直连admin的地址.
@@ -106,18 +109,19 @@
             load_dotenv(self.dotenv_path)
         except ImportError:  # pragma: no cover
             pass
 
         for param in inspect.signature(ExecutorConfig).parameters.values():
             env_val = os.getenv(param.name) or os.getenv(param.name.upper())
             if env_val is not None:
-                logger.debug("Get [%s] config from env: [%s]" % (param.name, env_val))
+                logger.debug("Get [%s] config from env." % (param.name))
+                real_value: Any = env_val
                 if param.annotation is bool:
                     real_value = env_val in ["true", "True"]
-                else:
+                elif get_origin(param.annotation) is None:
                     real_value = param.annotation(env_val)
                 setattr(self, param.name, real_value)
 
     def _valid_xxl_admin_baseurl(self) -> None:
         _admin_url: URL = URL(self.xxl_admin_baseurl)
         if not (_admin_url.scheme.startswith("http") and _admin_url.path.endswith("/")):
             raise ValueError("admin_url must like http://localhost:8080/xxl-job-admin/api/")
```

### Comparing `pyxxl-0.3.4/pyxxl/tests/api/test_metrics.py` & `pyxxl-0.3.5/pyxxl/tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/api/test_server.py` & `pyxxl-0.3.5/pyxxl/tests/api/test_server.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/conftest.py` & `pyxxl-0.3.5/pyxxl/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/test_client.py` & `pyxxl-0.3.5/pyxxl/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/test_context.py` & `pyxxl-0.3.5/pyxxl/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/test_executor.py` & `pyxxl-0.3.5/pyxxl/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/test_handler.py` & `pyxxl-0.3.5/pyxxl/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/test_logger.py` & `pyxxl-0.3.5/pyxxl/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/test_register.py` & `pyxxl-0.3.5/pyxxl/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/test_setting.py` & `pyxxl-0.3.5/pyxxl/tests/test_setting.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/tests/utils.py` & `pyxxl-0.3.5/pyxxl/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyxxl.utils import try_import
 from pyxxl.xxl_client import XXL, JsonType, Response
 
 
 class MokeXXL(XXL):
     callback_result: Dict[int, Any] = {}
 
-    async def callback(self, log_id: int, timestamp: int, code: int = 200, msg: str = None) -> None:
+    async def callback(self, log_id: int, timestamp: int, code: int = 200, msg: Optional[str] = None) -> None:
         self.callback_result[log_id] = code
 
     async def _post(self, path: str, payload: JsonType, retry_times: Optional[int] = None) -> Response:
         return Response(code=200)
 
     def clear_result(self) -> None:
         self.callback_result = {}
```

### Comparing `pyxxl-0.3.4/pyxxl/utils.py` & `pyxxl-0.3.5/pyxxl/utils.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.4/pyxxl/xxl_client.py` & `pyxxl-0.3.5/pyxxl/xxl_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         return False
 
     async def registryRemove(self, key: str, value: str) -> None:
         payload = dict(registryGroup="EXECUTOR", registryKey=key, registryValue=value)
         await self._post("registryRemove", payload, retry_times=3)
         logger.info("RegistryRemove successful. %s" % payload)
 
-    async def callback(self, log_id: int, timestamp: int, code: int = 200, msg: str = None) -> None:
+    async def callback(self, log_id: int, timestamp: int, code: int = 200, msg: Optional[str] = None) -> None:
         # executeResult兼容xxl-job2.2版本
         payload = [
             {
                 "logId": log_id,
                 "logDateTim": timestamp,
                 "handleCode": code,
                 "handleMsg": msg,
```

### Comparing `pyxxl-0.3.4/PKG-INFO` & `pyxxl-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxxl
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python executor for XXL-jobs
 Home-page: https://github.com/fcfangcc/pyxxl
 License: GPL-3.0-only
 Keywords: XXL
 Author: fcfangcc
 Author-email: swjfc22@live.com
 Requires-Python: >=3.9,<4.0
@@ -54,26 +54,29 @@
 * 任务的管理（支持在界面上取消，发起等操作，任务完成后会回调admin）
 * 所有阻塞策略的支持
 * 异步支持（推荐）
 * job-admin上查看日志
 
 ## 适配的XXL-JOB版本
 
-* XXL-JOB:2.3.0
+**2.4.0**,**2.3.0**,**2.2.0**
 
-如遇到不兼容的情况请issue告诉我XXL-JOB版本我会尽量适配
+如遇到不兼容的情况请issue告诉我XXL-JOB版本和对应的问题我会尽量适配
 
 ## 如何使用
 
 ```shell
 pip install pyxxl
+
 # 如果日志需要写入redis
 pip install "pyxxl[redis]"
+
 # 如果需要从.env加载配置
 pip install "pyxxl[dotenv]"
+
 # 安装所有功能
 pip install "pyxxl[all]"
 ```
 
 ```python
 import asyncio
 
@@ -164,10 +167,10 @@
 
 
 ```shell
 # if you need. set venv in project.
 # poetry config virtualenvs.in-project true
 poetry install --all-extras
 # 修改app.py中相关的配置信息,然后启动
-poetry run python example/app.py
+poetry run python example/executor_app.py
 ```
```

