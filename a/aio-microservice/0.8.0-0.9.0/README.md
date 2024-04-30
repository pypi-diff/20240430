# Comparing `tmp/aio_microservice-0.8.0.tar.gz` & `tmp/aio_microservice-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_microservice-0.8.0.tar", last modified: Thu Mar 21 14:28:43 2024, max compression
+gzip compressed data, was "aio_microservice-0.9.0.tar", last modified: Thu Mar 21 17:22:42 2024, max compression
```

## Comparing `aio_microservice-0.8.0.tar` & `aio_microservice-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/LICENSE
--rw-r--r--   0        0        0     1612 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/README.md
--rw-r--r--   0        0        0      423 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/aio_microservice/__init__.py
--rw-r--r--   0        0        0       22 2024-03-21 14:28:43.957785 aio_microservice-0.8.0/aio_microservice/__version__.py
--rw-r--r--   0        0        0      560 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/aio_microservice/amqp/__init__.py
--rw-r--r--   0        0        0     2005 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/aio_microservice/amqp/asyncapi.py
--rw-r--r--   0        0        0     8472 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/aio_microservice/amqp/extension.py
--rw-r--r--   0        0        0     2122 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/aio_microservice/amqp/testing.py
--rw-r--r--   0        0        0        0 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/aio_microservice/core/__init__.py
--rw-r--r--   0        0        0     5009 2024-03-21 14:28:08.925846 aio_microservice-0.8.0/aio_microservice/core/abc.py
--rw-r--r--   0        0        0     1957 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/core/logging.py
--rw-r--r--   0        0        0      531 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/core/openapi.py
--rw-r--r--   0        0        0     8125 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/core/service.py
--rw-r--r--   0        0        0      451 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/core/testing.py
--rw-r--r--   0        0        0      141 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/graphql/__init__.py
--rw-r--r--   0        0        0     3477 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/graphql/extension.py
--rw-r--r--   0        0        0      346 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/http.py
--rw-r--r--   0        0        0        0 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/py.typed
--rw-r--r--   0        0        0      183 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/s3/__init__.py
--rw-r--r--   0        0        0     2044 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/s3/extension.py
--rw-r--r--   0        0        0      198 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/scheduler/__init__.py
--rw-r--r--   0        0        0     6675 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/scheduler/extension.py
--rw-r--r--   0        0        0      118 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/aio_microservice/types.py
--rw-r--r--   0        0        0     5203 2024-03-21 14:28:43.961785 aio_microservice-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0    10785 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/amqp/test_amqp.py
--rw-r--r--   0        0        0     3268 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/amqp/test_amqp_asyncapi.py
--rw-r--r--   0        0        0     7129 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/amqp/test_amqp_test_broker.py
--rw-r--r--   0        0        0      646 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0     2477 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/core/test_cli.py
--rw-r--r--   0        0        0      956 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/core/test_custom_base_service.py
--rw-r--r--   0        0        0     5472 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/core/test_lifecycle_hooks.py
--rw-r--r--   0        0        0     3577 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/core/test_readiness_liveness_probe.py
--rw-r--r--   0        0        0      368 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/core/test_settings.py
--rw-r--r--   0        0        0     1182 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/core/test_startup_message.py
--rw-r--r--   0        0        0      811 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/graphql/test_graphql.py
--rw-r--r--   0        0        0     3884 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/graphql/test_graphql_test_client.py
--rw-r--r--   0        0        0      975 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/http/test_http.py
--rw-r--r--   0        0        0     2364 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/http/test_http_openapi.py
--rw-r--r--   0        0        0      542 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/http/test_http_test_client.py
--rw-r--r--   0        0        0     3590 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/s3/test_s3.py
--rw-r--r--   0        0        0     1924 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/scheduler/test_scheduler.py
--rw-r--r--   0        0        0       77 2024-03-21 14:28:08.929846 aio_microservice-0.8.0/tests/test_import.py
--rw-r--r--   0        0        0     3823 1970-01-01 00:00:00.000000 aio_microservice-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1612 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/README.md
+-rw-r--r--   0        0        0      423 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-21 17:22:42.149193 aio_microservice-0.9.0/aio_microservice/__version__.py
+-rw-r--r--   0        0        0      560 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/amqp/__init__.py
+-rw-r--r--   0        0        0     2005 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/amqp/asyncapi.py
+-rw-r--r--   0        0        0     8628 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/amqp/extension.py
+-rw-r--r--   0        0        0     2122 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/amqp/testing.py
+-rw-r--r--   0        0        0        0 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/core/__init__.py
+-rw-r--r--   0        0        0     5009 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/core/abc.py
+-rw-r--r--   0        0        0     1957 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/core/logging.py
+-rw-r--r--   0        0        0      531 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/core/openapi.py
+-rw-r--r--   0        0        0     8125 2024-03-21 17:22:12.549226 aio_microservice-0.9.0/aio_microservice/core/service.py
+-rw-r--r--   0        0        0      451 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/core/testing.py
+-rw-r--r--   0        0        0      141 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/graphql/__init__.py
+-rw-r--r--   0        0        0     3477 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/graphql/extension.py
+-rw-r--r--   0        0        0      346 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/http.py
+-rw-r--r--   0        0        0        0 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/py.typed
+-rw-r--r--   0        0        0      183 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/s3/__init__.py
+-rw-r--r--   0        0        0     2044 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/s3/extension.py
+-rw-r--r--   0        0        0      198 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/scheduler/__init__.py
+-rw-r--r--   0        0        0     6675 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/scheduler/extension.py
+-rw-r--r--   0        0        0      118 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/aio_microservice/types.py
+-rw-r--r--   0        0        0     5263 2024-03-21 17:22:42.153193 aio_microservice-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    10932 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/amqp/test_amqp.py
+-rw-r--r--   0        0        0     3268 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/amqp/test_amqp_asyncapi.py
+-rw-r--r--   0        0        0     7129 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/amqp/test_amqp_test_broker.py
+-rw-r--r--   0        0        0      646 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     2477 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/core/test_cli.py
+-rw-r--r--   0        0        0      956 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/core/test_custom_base_service.py
+-rw-r--r--   0        0        0     5472 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/core/test_lifecycle_hooks.py
+-rw-r--r--   0        0        0     3577 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/core/test_readiness_liveness_probe.py
+-rw-r--r--   0        0        0      368 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/core/test_settings.py
+-rw-r--r--   0        0        0     1182 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/core/test_startup_message.py
+-rw-r--r--   0        0        0      811 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/graphql/test_graphql.py
+-rw-r--r--   0        0        0     3884 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/graphql/test_graphql_test_client.py
+-rw-r--r--   0        0        0      975 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/http/test_http.py
+-rw-r--r--   0        0        0     2364 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/http/test_http_openapi.py
+-rw-r--r--   0        0        0      542 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/http/test_http_test_client.py
+-rw-r--r--   0        0        0     3590 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/s3/test_s3.py
+-rw-r--r--   0        0        0     1924 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/scheduler/test_scheduler.py
+-rw-r--r--   0        0        0       77 2024-03-21 17:22:12.553226 aio_microservice-0.9.0/tests/test_import.py
+-rw-r--r--   0        0        0     3889 1970-01-01 00:00:00.000000 aio_microservice-0.9.0/PKG-INFO
```

### Comparing `aio_microservice-0.8.0/LICENSE` & `aio_microservice-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/README.md` & `aio_microservice-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/amqp/__init__.py` & `aio_microservice-0.9.0/aio_microservice/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/amqp/asyncapi.py` & `aio_microservice-0.9.0/aio_microservice/amqp/asyncapi.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/amqp/extension.py` & `aio_microservice-0.9.0/aio_microservice/amqp/extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,28 +37,36 @@
         default="guest",
         description="The username for authentication on the broker.",
     )
     password: SecretStr = Field(
         default=SecretStr("guest"),
         description="The password for authentication on the broker.",
     )
+    prefetch_count: int | None = Field(
+        default=None,
+        description="The prefetch window size.",
+    )
+    timeout_graceful_shutdown: float | None = Field(
+        default=None,
+        description="The timeout for graceful shutdown (in seconds).",
+    )
 
 
 class AmqpExtensionImpl:
     def __init__(self, service: AmqpExtension, settings: AmqpSettings) -> None:
         self._service = service
         self._settings = settings
         self._faststream_rabbit_broker = RabbitBroker(
             host=self._settings.host,
             port=self._settings.port,
             login=self._settings.username,
             password=self._settings.password.get_secret_value(),
             middlewares=service.__amqp_middlewares__,
-            max_consumers=service.__amqp_prefetch_count__,
-            graceful_timeout=service.__amqp_graceful_timeout__,
+            max_consumers=self._settings.prefetch_count,
+            graceful_timeout=self._settings.timeout_graceful_shutdown,
         )
         self._faststream_app = FastStream(
             broker=self._faststream_rabbit_broker,
             title=service.__class__.__name__,
             version=service.__version__,
             description=service.__description__,
         )
@@ -111,16 +119,14 @@
 
 class AmqpExtensionSettings(BaseModel):
     amqp: AmqpSettings = AmqpSettings()
 
 
 class AmqpExtension(ExtensionABC):
     __amqp_middlewares__: ClassVar[list[type[BaseMiddleware]]] = []
-    __amqp_prefetch_count__: ClassVar[int | None] = None
-    __amqp_graceful_timeout__: ClassVar[float | None] = None
 
     def __init__(self, settings: AmqpExtensionSettings) -> None:
         self.amqp = AmqpExtensionImpl(service=self, settings=settings.amqp)
         self.register_http_controller(self.amqp._asyncapi_controller)
 
     @startup_message
     async def _amqp_startup_message(self) -> str:
```

### Comparing `aio_microservice-0.8.0/aio_microservice/amqp/testing.py` & `aio_microservice-0.9.0/aio_microservice/amqp/testing.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/core/abc.py` & `aio_microservice-0.9.0/aio_microservice/core/abc.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/core/logging.py` & `aio_microservice-0.9.0/aio_microservice/core/logging.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/core/openapi.py` & `aio_microservice-0.9.0/aio_microservice/core/openapi.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/core/service.py` & `aio_microservice-0.9.0/aio_microservice/core/service.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/graphql/extension.py` & `aio_microservice-0.9.0/aio_microservice/graphql/extension.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/s3/extension.py` & `aio_microservice-0.9.0/aio_microservice/s3/extension.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/aio_microservice/scheduler/extension.py` & `aio_microservice-0.9.0/aio_microservice/scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/pyproject.toml` & `aio_microservice-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,26 @@
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 dynamic = []
 dependencies = [
     "annotated-types>=0.6.0",
     "click>=8.1.3",
+    "eval-type-backport>=0.1.3; python_version < \"3.10\"",
     "litestar>=2.6.3",
     "loguru>=0.7.2",
     "pydantic>=2.6.3",
     "pyhumps>=3.8.0",
     "rich-click>=1.7.3",
     "rich>=13.7.1",
     "typed-settings>=24.1.0",
-    "uvicorn>=0.27.1",
     "typing-extensions>=4.10.0",
+    "uvicorn>=0.27.1",
 ]
-version = "0.8.0"
+version = "0.9.0"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 amqp = [
     "faststream[rabbit]>=0.4.6",
```

### Comparing `aio_microservice-0.8.0/tests/amqp/test_amqp.py` & `aio_microservice-0.9.0/tests/amqp/test_amqp.py`

 * *Files 8% similar despite different names*

```diff
@@ -168,28 +168,32 @@
 ) -> None:
     handler_pre_stub = mocker.stub()
     handler_post_stub = mocker.stub()
 
     class TestSettings(ServiceSettings, AmqpExtensionSettings): ...
 
     class TestService(Service[TestSettings], AmqpExtension):
-        __amqp_prefetch_count__ = 1
-
         def __init__(self, settings: TestSettings | None = None) -> None:
             super().__init__(settings=settings)
             self.keep_running = True
 
         @amqp.subscriber(queue="test-subscriber-queue")
         async def handle_test(self) -> None:
             handler_pre_stub()
             while self.keep_running:
                 await asyncio.sleep(0.1)
             handler_post_stub()
 
-    settings = TestSettings(amqp=AmqpSettings(host=rabbitmq_ip, port=rabbitmq_port))
+    settings = TestSettings(
+        amqp=AmqpSettings(
+            host=rabbitmq_ip,
+            port=rabbitmq_port,
+            prefetch_count=1,
+        ),
+    )
     service = TestService(settings=settings)
 
     async with TestAmqpBroker(service, with_real=True) as amqp_broker:
         task1 = asyncio.create_task(amqp_broker.publish(queue="test-subscriber-queue"))
         task2 = asyncio.create_task(amqp_broker.publish(queue="test-subscriber-queue"))
 
         await asyncio.sleep(0.5)
@@ -258,27 +262,31 @@
     handler_pre_stub = mocker.stub()
     handler_post_stub = mocker.stub()
     handler_cancelled_stub = mocker.stub()
 
     class TestSettings(ServiceSettings, AmqpExtensionSettings): ...
 
     class TestService(Service[TestSettings], AmqpExtension):
-        __amqp_graceful_timeout__ = 0.1
-
         @amqp.subscriber(queue="test-subscriber-queue")
         async def handle_test(self) -> None:
             handler_pre_stub()
             try:
                 await asyncio.sleep(0.5)
             except asyncio.CancelledError:
                 handler_cancelled_stub()
             else:
                 handler_post_stub()
 
-    settings = TestSettings(amqp=AmqpSettings(host=rabbitmq_ip, port=rabbitmq_port))
+    settings = TestSettings(
+        amqp=AmqpSettings(
+            host=rabbitmq_ip,
+            port=rabbitmq_port,
+            timeout_graceful_shutdown=0.1,
+        ),
+    )
     service = TestService(settings=settings)
 
     publish_task = None
 
     async with TestAmqpBroker(service=service, with_real=True) as amqp_broker:
         publish_task = asyncio.create_task(amqp_broker.publish(queue="test-subscriber-queue"))
 
@@ -302,27 +310,31 @@
     handler_pre_stub = mocker.stub()
     handler_post_stub = mocker.stub()
     handler_cancelled_stub = mocker.stub()
 
     class TestSettings(ServiceSettings, AmqpExtensionSettings): ...
 
     class TestService(Service[TestSettings], AmqpExtension):
-        __amqp_graceful_timeout__ = 1.0
-
         @amqp.subscriber(queue="test-subscriber-queue")
         async def handle_test(self) -> None:
             handler_pre_stub()
             try:
                 await asyncio.sleep(0.5)
             except asyncio.CancelledError:
                 handler_cancelled_stub()
             else:
                 handler_post_stub()
 
-    settings = TestSettings(amqp=AmqpSettings(host=rabbitmq_ip, port=rabbitmq_port))
+    settings = TestSettings(
+        amqp=AmqpSettings(
+            host=rabbitmq_ip,
+            port=rabbitmq_port,
+            timeout_graceful_shutdown=1.0,
+        ),
+    )
     service = TestService(settings=settings)
 
     publish_task = None
 
     async with TestAmqpBroker(service=service, with_real=True) as amqp_broker:
         publish_task = asyncio.create_task(amqp_broker.publish(queue="test-subscriber-queue"))
```

### Comparing `aio_microservice-0.8.0/tests/amqp/test_amqp_asyncapi.py` & `aio_microservice-0.9.0/tests/amqp/test_amqp_asyncapi.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/amqp/test_amqp_test_broker.py` & `aio_microservice-0.9.0/tests/amqp/test_amqp_test_broker.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/conftest.py` & `aio_microservice-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/core/test_cli.py` & `aio_microservice-0.9.0/tests/core/test_cli.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/core/test_custom_base_service.py` & `aio_microservice-0.9.0/tests/core/test_custom_base_service.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/core/test_lifecycle_hooks.py` & `aio_microservice-0.9.0/tests/core/test_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/core/test_readiness_liveness_probe.py` & `aio_microservice-0.9.0/tests/core/test_readiness_liveness_probe.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/core/test_startup_message.py` & `aio_microservice-0.9.0/tests/core/test_startup_message.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/graphql/test_graphql.py` & `aio_microservice-0.9.0/tests/graphql/test_graphql.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/graphql/test_graphql_test_client.py` & `aio_microservice-0.9.0/tests/graphql/test_graphql_test_client.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/http/test_http.py` & `aio_microservice-0.9.0/tests/http/test_http.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/http/test_http_openapi.py` & `aio_microservice-0.9.0/tests/http/test_http_openapi.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/http/test_http_test_client.py` & `aio_microservice-0.9.0/tests/http/test_http_test_client.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/s3/test_s3.py` & `aio_microservice-0.9.0/tests/s3/test_s3.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/tests/scheduler/test_scheduler.py` & `aio_microservice-0.9.0/tests/scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `aio_microservice-0.8.0/PKG-INFO` & `aio_microservice-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-microservice
-Version: 0.8.0
+Version: 0.9.0
 Summary: A library to create microservices.
 Author-Email: betaboon <betaboon@0x80.ninja>
 Maintainer-Email: betaboon <betaboon@0x80.ninja>
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,23 +22,24 @@
 Project-URL: Documentation, https://betaboon.github.io/aio-microservice
 Project-URL: Changelog, https://github.com/betaboon/aio-microservice/releases
 Project-URL: Repository, https://github.com/betaboon/aio-microservice
 Project-URL: Issue tracker, https://github.com/betaboon/aio-microservice/issues
 Requires-Python: <3.13,>=3.9
 Requires-Dist: annotated-types>=0.6.0
 Requires-Dist: click>=8.1.3
+Requires-Dist: eval-type-backport>=0.1.3; python_version < "3.10"
 Requires-Dist: litestar>=2.6.3
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: pydantic>=2.6.3
 Requires-Dist: pyhumps>=3.8.0
 Requires-Dist: rich-click>=1.7.3
 Requires-Dist: rich>=13.7.1
 Requires-Dist: typed-settings>=24.1.0
-Requires-Dist: uvicorn>=0.27.1
 Requires-Dist: typing-extensions>=4.10.0
+Requires-Dist: uvicorn>=0.27.1
 Requires-Dist: faststream[rabbit]>=0.4.6; extra == "amqp"
 Requires-Dist: pyyaml>=6.0.1; extra == "amqp"
 Requires-Dist: aio-microservice[amqp]; extra == "all"
 Requires-Dist: aio-microservice[s3]; extra == "all"
 Requires-Dist: aio-microservice[scheduler]; extra == "all"
 Requires-Dist: boto3>=1.34.54; extra == "s3"
 Requires-Dist: apscheduler>=3.10.4; extra == "scheduler"
```

