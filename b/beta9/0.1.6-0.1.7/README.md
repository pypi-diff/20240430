# Comparing `tmp/beta9-0.1.6.tar.gz` & `tmp/beta9-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beta9-0.1.6.tar", max compression
+gzip compressed data, was "beta9-0.1.7.tar", max compression
```

## Comparing `beta9-0.1.6.tar` & `beta9-0.1.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1127 2024-04-29 20:32:04.904245 beta9-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      586 2024-04-26 16:58:18.488727 beta9-0.1.6/src/beta9/__init__.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.6/src/beta9/abstractions/__init__.py
--rw-r--r--   0        0        0      606 2024-01-27 16:13:22.962265 beta9-0.1.6/src/beta9/abstractions/base/__init__.py
--rw-r--r--   0        0        0     9102 2024-04-29 01:46:22.899381 beta9-0.1.6/src/beta9/abstractions/base/runner.py
--rw-r--r--   0        0        0     3492 2024-04-21 16:36:14.953861 beta9-0.1.6/src/beta9/abstractions/container.py
--rw-r--r--   0        0        0     4698 2024-04-29 20:30:30.521016 beta9-0.1.6/src/beta9/abstractions/endpoint.py
--rw-r--r--   0        0        0     7229 2024-04-29 20:35:39.853896 beta9-0.1.6/src/beta9/abstractions/function.py
--rw-r--r--   0        0        0     4264 2024-04-24 22:31:23.870406 beta9-0.1.6/src/beta9/abstractions/image.py
--rw-r--r--   0        0        0     3237 2024-04-21 16:36:14.954512 beta9-0.1.6/src/beta9/abstractions/map.py
--rw-r--r--   0        0        0     3183 2024-04-21 16:36:14.955563 beta9-0.1.6/src/beta9/abstractions/queue.py
--rw-r--r--   0        0        0     9026 2024-04-29 20:33:22.790110 beta9-0.1.6/src/beta9/abstractions/taskqueue.py
--rw-r--r--   0        0        0     1605 2024-04-21 16:36:14.957214 beta9-0.1.6/src/beta9/abstractions/volume.py
--rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.6/src/beta9/aio.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.6/src/beta9/cli/__init__.py
--rw-r--r--   0        0        0      932 2024-04-21 16:36:14.959066 beta9-0.1.6/src/beta9/cli/config.py
--rw-r--r--   0        0        0      824 2024-04-21 16:36:14.962332 beta9-0.1.6/src/beta9/cli/contexts.py
--rw-r--r--   0        0        0     2422 2024-04-21 16:36:14.964463 beta9-0.1.6/src/beta9/cli/deployment.py
--rw-r--r--   0        0        0     3197 2024-04-21 16:36:14.964958 beta9-0.1.6/src/beta9/cli/extraclick.py
--rw-r--r--   0        0        0     1140 2024-04-21 16:36:14.966489 beta9-0.1.6/src/beta9/cli/main.py
--rw-r--r--   0        0        0     3738 2024-04-21 16:36:14.968025 beta9-0.1.6/src/beta9/cli/task.py
--rw-r--r--   0        0        0     8667 2024-04-21 16:36:14.970907 beta9-0.1.6/src/beta9/cli/volume.py
--rw-r--r--   0        0        0        0 2024-04-27 21:49:44.298869 beta9-0.1.6/src/beta9/clients/__init__.py
--rw-r--r--   0        0        0     2980 2024-04-27 21:49:44.298980 beta9-0.1.6/src/beta9/clients/container/__init__.py
--rw-r--r--   0        0        0     4275 2024-04-27 21:49:44.117994 beta9-0.1.6/src/beta9/clients/endpoint/__init__.py
--rw-r--r--   0        0        0     8023 2024-04-27 21:49:43.256507 beta9-0.1.6/src/beta9/clients/function/__init__.py
--rw-r--r--   0        0        0    22783 2024-04-29 01:46:22.900294 beta9-0.1.6/src/beta9/clients/gateway/__init__.py
--rw-r--r--   0        0        0     4773 2024-04-27 21:49:42.845715 beta9-0.1.6/src/beta9/clients/image/__init__.py
--rw-r--r--   0        0        0     8003 2024-04-27 21:49:43.051036 beta9-0.1.6/src/beta9/clients/map/__init__.py
--rw-r--r--   0        0        0     8687 2024-04-27 21:49:43.458692 beta9-0.1.6/src/beta9/clients/simplequeue/__init__.py
--rw-r--r--   0        0        0    13315 2024-04-27 21:49:43.930351 beta9-0.1.6/src/beta9/clients/taskqueue/__init__.py
--rw-r--r--   0        0        0     9482 2024-04-27 21:49:43.680311 beta9-0.1.6/src/beta9/clients/volume/__init__.py
--rw-r--r--   0        0        0     7301 2024-04-21 16:36:14.980146 beta9-0.1.6/src/beta9/config.py
--rw-r--r--   0        0        0      492 2024-04-26 16:58:18.490032 beta9-0.1.6/src/beta9/env.py
--rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.6/src/beta9/exceptions.py
--rw-r--r--   0        0        0      883 2024-04-26 16:58:18.490335 beta9-0.1.6/src/beta9/logging.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.6/src/beta9/runner/__init__.py
--rw-r--r--   0        0        0     6376 2024-04-29 01:46:22.900678 beta9-0.1.6/src/beta9/runner/common.py
--rw-r--r--   0        0        0     2321 2024-04-21 16:36:14.980604 beta9-0.1.6/src/beta9/runner/container.py
--rw-r--r--   0        0        0     7453 2024-04-29 01:46:22.901219 beta9-0.1.6/src/beta9/runner/endpoint.py
--rw-r--r--   0        0        0     6889 2024-04-29 01:46:22.901734 beta9-0.1.6/src/beta9/runner/function.py
--rw-r--r--   0        0        0     3910 2024-04-21 16:36:14.986354 beta9-0.1.6/src/beta9/runner/serve.py
--rw-r--r--   0        0        0    12265 2024-04-29 01:46:22.902140 beta9-0.1.6/src/beta9/runner/taskqueue.py
--rw-r--r--   0        0        0     5713 2024-04-26 16:58:18.491443 beta9-0.1.6/src/beta9/sync.py
--rw-r--r--   0        0        0     2994 2024-04-21 16:36:14.997902 beta9-0.1.6/src/beta9/terminal.py
--rw-r--r--   0        0        0     1541 2024-04-29 01:46:22.902589 beta9-0.1.6/src/beta9/type.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 beta9-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1149 2024-04-29 21:57:51.839903 beta9-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      586 2024-04-26 18:24:46.913842 beta9-0.1.7/src/beta9/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.669351 beta9-0.1.7/src/beta9/abstractions/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-29 18:52:41.008869 beta9-0.1.7/src/beta9/abstractions/base/__init__.py
+-rw-r--r--   0        0        0     9285 2024-04-29 18:31:09.499178 beta9-0.1.7/src/beta9/abstractions/base/runner.py
+-rw-r--r--   0        0        0     3454 2024-04-29 21:53:15.666398 beta9-0.1.7/src/beta9/abstractions/container.py
+-rw-r--r--   0        0        0     7314 2024-04-29 21:53:15.666604 beta9-0.1.7/src/beta9/abstractions/endpoint.py
+-rw-r--r--   0        0        0     7251 2024-04-29 21:53:15.667152 beta9-0.1.7/src/beta9/abstractions/function.py
+-rw-r--r--   0        0        0     4413 2024-04-29 15:50:05.673117 beta9-0.1.7/src/beta9/abstractions/image.py
+-rw-r--r--   0        0        0     3237 2024-04-17 13:14:18.141834 beta9-0.1.7/src/beta9/abstractions/map.py
+-rw-r--r--   0        0        0     3345 2024-04-29 15:50:05.673407 beta9-0.1.7/src/beta9/abstractions/queue.py
+-rw-r--r--   0        0        0     9054 2024-04-29 21:53:15.667793 beta9-0.1.7/src/beta9/abstractions/taskqueue.py
+-rw-r--r--   0        0        0     1605 2024-04-17 13:14:18.142367 beta9-0.1.7/src/beta9/abstractions/volume.py
+-rw-r--r--   0        0        0      292 2024-04-15 21:13:39.880348 beta9-0.1.7/src/beta9/aio.py
+-rw-r--r--   0        0        0     4839 2024-04-29 19:08:45.672170 beta9-0.1.7/src/beta9/channel.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.670190 beta9-0.1.7/src/beta9/cli/__init__.py
+-rw-r--r--   0        0        0      669 2024-04-29 15:50:05.674161 beta9-0.1.7/src/beta9/cli/config.py
+-rw-r--r--   0        0        0     2418 2024-04-29 19:06:38.918521 beta9-0.1.7/src/beta9/cli/deployment.py
+-rw-r--r--   0        0        0     5582 2024-04-29 19:07:51.112717 beta9-0.1.7/src/beta9/cli/extraclick.py
+-rw-r--r--   0        0        0     1810 2024-04-29 18:32:08.108950 beta9-0.1.7/src/beta9/cli/main.py
+-rw-r--r--   0        0        0     3770 2024-04-29 18:40:09.512566 beta9-0.1.7/src/beta9/cli/task.py
+-rw-r--r--   0        0        0     8591 2024-04-29 18:31:31.881448 beta9-0.1.7/src/beta9/cli/volume.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:32:37.403246 beta9-0.1.7/src/beta9/clients/__init__.py
+-rw-r--r--   0        0        0     2980 2024-04-17 13:14:18.144448 beta9-0.1.7/src/beta9/clients/container/__init__.py
+-rw-r--r--   0        0        0     4275 2024-04-21 18:41:12.433810 beta9-0.1.7/src/beta9/clients/endpoint/__init__.py
+-rw-r--r--   0        0        0     8023 2024-04-17 13:14:18.144848 beta9-0.1.7/src/beta9/clients/function/__init__.py
+-rw-r--r--   0        0        0    22783 2024-04-29 14:36:52.301336 beta9-0.1.7/src/beta9/clients/gateway/__init__.py
+-rw-r--r--   0        0        0     4773 2024-04-17 13:14:18.145074 beta9-0.1.7/src/beta9/clients/image/__init__.py
+-rw-r--r--   0        0        0     8003 2024-04-17 13:14:18.145188 beta9-0.1.7/src/beta9/clients/map/__init__.py
+-rw-r--r--   0        0        0     8687 2024-04-17 13:14:18.145328 beta9-0.1.7/src/beta9/clients/simplequeue/__init__.py
+-rw-r--r--   0        0        0    13315 2024-04-21 18:41:12.433950 beta9-0.1.7/src/beta9/clients/taskqueue/__init__.py
+-rw-r--r--   0        0        0     9482 2024-04-17 13:14:18.145732 beta9-0.1.7/src/beta9/clients/volume/__init__.py
+-rw-r--r--   0        0        0     4843 2024-04-29 21:33:40.077172 beta9-0.1.7/src/beta9/config.py
+-rw-r--r--   0        0        0      492 2024-04-26 18:24:46.916278 beta9-0.1.7/src/beta9/env.py
+-rw-r--r--   0        0        0      207 2024-01-23 23:38:59.671504 beta9-0.1.7/src/beta9/exceptions.py
+-rw-r--r--   0        0        0      883 2024-04-26 18:24:46.916852 beta9-0.1.7/src/beta9/logging.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.671565 beta9-0.1.7/src/beta9/runner/__init__.py
+-rw-r--r--   0        0        0     6364 2024-04-29 19:00:52.006511 beta9-0.1.7/src/beta9/runner/common.py
+-rw-r--r--   0        0        0     2322 2024-04-29 18:32:47.793316 beta9-0.1.7/src/beta9/runner/container.py
+-rw-r--r--   0        0        0     7454 2024-04-29 18:32:58.148052 beta9-0.1.7/src/beta9/runner/endpoint.py
+-rw-r--r--   0        0        0     6890 2024-04-29 18:30:52.002896 beta9-0.1.7/src/beta9/runner/function.py
+-rw-r--r--   0        0        0     3910 2024-04-17 13:14:18.147410 beta9-0.1.7/src/beta9/runner/serve.py
+-rw-r--r--   0        0        0    12307 2024-04-29 21:53:15.668333 beta9-0.1.7/src/beta9/runner/taskqueue.py
+-rw-r--r--   0        0        0     5716 2024-04-29 19:00:25.543057 beta9-0.1.7/src/beta9/sync.py
+-rw-r--r--   0        0        0     3114 2024-04-29 15:50:05.676180 beta9-0.1.7/src/beta9/terminal.py
+-rw-r--r--   0        0        0     1541 2024-04-29 14:36:52.302649 beta9-0.1.7/src/beta9/type.py
+-rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 beta9-0.1.7/PKG-INFO
```

### Comparing `beta9-0.1.6/pyproject.toml` & `beta9-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beta9"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beta9", from = "src" },
     { include = "beta9/**/*.py", from = "src" },
 ]
 
@@ -17,25 +17,26 @@
 grpcio = "^1.60.0"
 asgiref = "^3.7.2"
 cloudpickle = "^3.0.0"
 rich = "^13.7.0"
 click = "^8.1.7"
 betterproto = {version = "2.0.0b6", extras = ["compiler"]}
 protobuf = "^4.25.1"
-fastapi = "^0.109.0"
+fastapi = "^0.110.2"
 uvicorn = "^0.29.0"
 watchdog = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pytest-env = "^1.1.3"
 attrs = "^23.2.0"
 docstring-parser = "^0.16"
-ruff = "^0.3.7"
-pydantic = "^2.5.3"
+ruff = "^0.4.2"
+gunicorn = "^22.0.0"
+requests = "^2.31.0"
 
 [tool.poetry.scripts]
 beta9 = "beta9.cli.main:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `beta9-0.1.6/src/beta9/__init__.py` & `beta9-0.1.7/src/beta9/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/abstractions/base/runner.py` & `beta9-0.1.7/src/beta9/abstractions/base/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,23 @@
         self.max_containers = max_containers
         self.retries = retries
         self.timeout = timeout
 
         if on_start is not None:
             self._map_callable_to_attr(attr="on_start", func=on_start)
 
-        self.gateway_stub: GatewayServiceStub = GatewayServiceStub(self.channel)
+        self._gateway_stub: Optional[GatewayServiceStub] = None
         self.syncer: FileSyncer = FileSyncer(self.gateway_stub)
 
+    @property
+    def gateway_stub(self) -> GatewayServiceStub:
+        if not self._gateway_stub:
+            self._gateway_stub = GatewayServiceStub(self.channel)
+        return self._gateway_stub
+
     def _parse_cpu_to_millicores(self, cpu: Union[float, str]) -> int:
         """
         Parse the cpu argument to an integer value in millicores.
 
         Args:
         cpu (Union[int, float, str]): The CPU requirement specified as a float (cores) or string (millicores).
```

### Comparing `beta9-0.1.6/src/beta9/abstractions/container.py` & `beta9-0.1.7/src/beta9/abstractions/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,21 +33,22 @@
         volumes (Optional[List[Volume]]):
             A list of volumes to be mounted to the container. Default is None.
         name (Optional[str]):
             A name for the container. Default is None.
 
     Example usage:
         ```
-        from beta9.abstractions.image import Image
-        from beta9.abstractions.volume import Volume
+        from beta9 import Image, Container
 
-        image = Image(name="python", tag="3.8")
-        container = Container(cpu=2, memory=512, image=image))
-        exit_code = container.run(["python", "-c", "\"print('Hello, World!')\""])
-        print(exit_code)
+
+        def run_container():
+            image = Image()
+            container = Container(cpu=2, memory=512, image=image)
+            exit_code = container.run((["python", "-c", "\"print('Hello, World!')\""]))
+            print(exit_code)
         ```
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
```

### Comparing `beta9-0.1.6/src/beta9/abstractions/function.py` & `beta9-0.1.7/src/beta9/abstractions/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from ..abstractions.volume import Volume
 from ..clients.function import (
     FunctionInvokeRequest,
     FunctionInvokeResponse,
     FunctionServiceStub,
 )
 from ..clients.gateway import DeployStubRequest, DeployStubResponse
-from ..config import GatewayConfig, get_gateway_config
 from ..env import is_local
 from ..sync import FileSyncer
 
 
 class Function(RunnerAbstraction):
     """
     Decorator which allows you to run the decorated function in a remote container.
@@ -58,16 +57,14 @@
         # Call a function in a remote container
         function.remote("some_file.mp4")
 
         # Map the function over several inputs
         # Each of these inputs will be routed to remote containers
         for result in function.map(["file1.mp4", "file2.mp4"]):
             print(result)
-
-
         ```
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
@@ -85,20 +82,26 @@
             image=image,
             timeout=timeout,
             retries=retries,
             callback_url=callback_url,
             volumes=volumes,
         )
 
-        self.function_stub: FunctionServiceStub = FunctionServiceStub(self.channel)
+        self._function_stub: Optional[FunctionServiceStub] = None
         self.syncer: FileSyncer = FileSyncer(self.gateway_stub)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
 
+    @property
+    def function_stub(self) -> FunctionServiceStub:
+        if not self._function_stub:
+            self._function_stub = FunctionServiceStub(self.channel)
+        return self._function_stub
+
 
 class _CallableWrapper:
     def __init__(self, func: Callable, parent: Function) -> None:
         self.func: Callable = func
         self.parent: Function = parent
 
     def __call__(self, *args, **kwargs) -> Any:
@@ -161,20 +164,19 @@
         deploy_response: DeployStubResponse = self.parent.run_sync(
             self.parent.gateway_stub.deploy_stub(
                 DeployStubRequest(stub_id=self.parent.stub_id, name=name)
             )
         )
 
         if deploy_response.ok:
-            gateway_config: GatewayConfig = get_gateway_config()
-            gateway_url = f"{gateway_config.gateway_host}:{gateway_config.gateway_port}"
+            base_url = "https://app.beam.cloud"
 
             terminal.header("Deployed 🎉")
             terminal.detail(
-                f"Call your deployment at: {gateway_url}/api/v1/function/{name}/v{deploy_response.version}"
+                f"Call your deployment at: {base_url}/api/v1/function/{name}/v{deploy_response.version}"
             )
 
         return deploy_response.ok
 
     def _format_args(self, args):
         if isinstance(args, tuple):
             return list(args)
```

### Comparing `beta9-0.1.6/src/beta9/abstractions/image.py` & `beta9-0.1.7/src/beta9/abstractions/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,21 @@
         super().__init__()
 
         self.python_version = python_version
         self.python_packages = python_packages
         self.commands = commands
         self.base_image = base_image
         self.base_image_creds = None
-        self.stub: ImageServiceStub = ImageServiceStub(self.channel)
+        self._stub: Optional[ImageServiceStub] = None
+
+    @property
+    def stub(self) -> ImageServiceStub:
+        if not self._stub:
+            self._stub = ImageServiceStub(self.channel)
+        return self._stub
 
     def exists(self) -> Tuple[bool, ImageBuildResult]:
         r: VerifyImageBuildResponse = self.run_sync(
             self.stub.verify_image_build(
                 VerifyImageBuildRequest(
                     python_packages=self.python_packages,
                     python_version=self.python_version,
```

### Comparing `beta9-0.1.6/src/beta9/abstractions/map.py` & `beta9-0.1.7/src/beta9/abstractions/map.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/abstractions/queue.py` & `beta9-0.1.7/src/beta9/abstractions/queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Optional
 
 import cloudpickle
 
 from ..abstractions.base import BaseAbstraction
 from ..clients.simplequeue import (
     SimpleQueueEmptyResponse,
     SimpleQueuePeekResponse,
@@ -53,23 +53,29 @@
             val = q.pop()
             print(val)
         ```
         """
         super().__init__()
 
         self.name: str = name
-        self.stub: SimpleQueueServiceStub = SimpleQueueServiceStub(self.channel)
+        self._stub: Optional[SimpleQueueServiceStub] = None
         self.max_size: int = max_size
 
+    @property
+    def stub(self) -> SimpleQueueServiceStub:
+        if not self._stub:
+            self._stub = SimpleQueueServiceStub(self.channel)
+        return self._stub
+
     def __len__(self):
         r = self.run_sync(self.stub.simple_queue_size(SimpleQueueRequest(name=self.name)))
         return r.size if r.ok else 0
 
     def __del__(self):
-        self.channel.close()
+        super().__del__()
 
     def put(self, value: Any) -> bool:
         r: SimpleQueuePutResponse = self.run_sync(
             self.stub.simple_queue_put(
                 SimpleQueuePutRequest(name=self.name, value=cloudpickle.dumps(value))
             )
         )
```

### Comparing `beta9-0.1.6/src/beta9/abstractions/taskqueue.py` & `beta9-0.1.7/src/beta9/abstractions/taskqueue.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from ..clients.taskqueue import (
     StartTaskQueueServeRequest,
     StopTaskQueueServeRequest,
     TaskQueuePutRequest,
     TaskQueuePutResponse,
     TaskQueueServiceStub,
 )
-from ..config import GatewayConfig, get_gateway_config
 from ..env import is_local
 
 
 class TaskQueue(RunnerAbstraction):
     """
     Decorator which allows you to create a task queue out of the decorated function. The tasks are executed
     asynchronously, in remote containers. You can interact with the task queue either through an API (when deployed), or directly
@@ -112,16 +111,21 @@
             retries=retries,
             keep_warm_seconds=keep_warm_seconds,
             max_pending_tasks=max_pending_tasks,
             on_start=on_start,
             callback_url=callback_url,
             volumes=volumes,
         )
+        self._taskqueue_stub: Optional[TaskQueueServiceStub] = None
 
-        self.taskqueue_stub: TaskQueueServiceStub = TaskQueueServiceStub(self.channel)
+    @property
+    def taskqueue_stub(self) -> TaskQueueServiceStub:
+        if not self._taskqueue_stub:
+            self._taskqueue_stub = TaskQueueServiceStub(self.channel)
+        return self._taskqueue_stub
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
 
 
 class _CallableWrapper:
     def __init__(self, func: Callable, parent: TaskQueue):
@@ -150,20 +154,19 @@
         deploy_response: DeployStubResponse = self.parent.run_sync(
             self.parent.gateway_stub.deploy_stub(
                 DeployStubRequest(stub_id=self.parent.stub_id, name=name)
             )
         )
 
         if deploy_response.ok:
-            gateway_config: GatewayConfig = get_gateway_config()
-            gateway_url = f"{gateway_config.gateway_host}:{gateway_config.gateway_port}"
+            base_url = "https://app.beam.cloud"
 
             terminal.header("Deployed 🎉")
             terminal.detail(
-                f"Call your deployment at: {gateway_url}/api/v1/taskqueue/{name}/v{deploy_response.version}"
+                f"Call your deployment at: {base_url}/api/v1/taskqueue/{name}/v{deploy_response.version}"
             )
 
         return deploy_response.ok
 
     def serve(self):
         if not self.parent.prepare_runtime(
             func=self.func, stub_type=TASKQUEUE_SERVE_STUB_TYPE, force_create_stub=True
```

### Comparing `beta9-0.1.6/src/beta9/abstractions/volume.py` & `beta9-0.1.7/src/beta9/abstractions/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/cli/deployment.py` & `beta9-0.1.7/src/beta9/cli/deployment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import importlib
 import os
 import sys
 from pathlib import Path
 
 import click
 
-from beta9.cli.extraclick import ClickCommonGroup, ClickManagementGroup
-
 from .. import terminal
-from .contexts import ServiceClient, get_gateway_service
+from ..channel import ServiceClient
+from ..cli import extraclick
+from .extraclick import ClickCommonGroup, ClickManagementGroup
 
 
 @click.group(cls=ClickCommonGroup)
-@click.pass_context
-def common(ctx: click.Context):
-    ctx.obj = ctx.with_resource(ServiceClient())
+def common(**_):
+    pass
 
 
 @common.command(
     name="deploy",
     help="""
     Deploy a new function.
 
     ENTRYPOINT is in the format of "file:function".
     """,
     epilog="""
       Examples:
 
-        beta9 deploy --name my-app app.py:handler
+        {cli_name} deploy --name my-app app.py:handler
 
-        beta9 deploy -n my-app-2 app.py:my_func
+        {cli_name} deploy -n my-app-2 app.py:my_func
         \b
     """,
 )
 @click.option(
     "--name",
     "-n",
     type=click.STRING,
@@ -41,36 +40,36 @@
     required=True,
 )
 @click.argument(
     "entrypoint",
     nargs=1,
     required=True,
 )
+@extraclick.pass_service_client
 @click.pass_context
-def deploy(ctx: click.Context, name: str, entrypoint: str):
+def deploy(ctx: click.Context, service: ServiceClient, name: str, entrypoint: str):
     ctx.invoke(create_deployment, name=name, entrypoint=entrypoint)
 
 
 @click.group(
     name="deployment",
     help="Manage deployments.",
     cls=ClickManagementGroup,
 )
-@click.pass_context
-def management(ctx: click.Context):
-    ctx.obj = ctx.with_resource(get_gateway_service())
+def management():
+    pass
 
 
 @management.command(
     name="create",
     help="Create a new deployment.",
     epilog="""
       Examples:
 
-        beta9 deploy --name my-app --entrypoint app.py:handler
+        {cli_name} deploy --name my-app --entrypoint app.py:handler
         \b
     """,
 )
 @click.option(
     "--name",
     "-n",
     help="The name the deployment.",
@@ -78,28 +77,29 @@
 )
 @click.option(
     "--entrypoint",
     "-e",
     help='The name the entrypoint e.g. "file:function".',
     required=True,
 )
-def create_deployment(name: str, entrypoint: str):
+@extraclick.pass_service_client
+def create_deployment(service: ServiceClient, name: str, entrypoint: str):
     current_dir = os.getcwd()
     if current_dir not in sys.path:
         sys.path.insert(0, current_dir)
 
     module_path, func_name, *_ = entrypoint.split(":") if ":" in entrypoint else (entrypoint, "")
     module_name = module_path.replace(".py", "").replace(os.path.sep, ".")
 
     if not Path(module_path).exists():
         terminal.error(f"Unable to find file '{module_path}'")
     if not func_name:
         terminal.error(f"Unable to parse function '{func_name}'")
 
     module = importlib.import_module(module_name)
 
-    func = getattr(module, func_name, None)
-    if func is None:
+    user_func = getattr(module, func_name, None)
+    if user_func is None:
         terminal.error(f"Unable to find function '{func_name}'")
 
-    if not func.deploy(name=name):
+    if not user_func.deploy(name=name):  # type:ignore
         terminal.error("Deployment failed ☠️")
```

### Comparing `beta9-0.1.6/src/beta9/cli/main.py` & `beta9-0.1.7/src/beta9/cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,65 @@
 import shutil
 from types import ModuleType
-from typing import Any
+from typing import Any, Optional
 
 import click
 
+from .. import terminal
+from ..channel import get_channel
+from ..config import is_config_empty
 from . import config, deployment, task, volume
-from .extraclick import CommandGroupCollection
+from .extraclick import ClickCommonGroup, CommandGroupCollection
 
 click.formatting.FORCED_WIDTH = shutil.get_terminal_size().columns
 
+# Can be overwritten by doing `load_cli(context_settings={})`
+CLICK_CONTEXT_SETTINGS = dict(
+    help_option_names=["-h", "--help"],
+    show_default=True,
+)
+
 
 class CLI:
     """
     The CLI application.
 
     This is used to dynamically register commands. Commands are of type
     click.Group and are named either "common" or "management".
     """
 
-    def __init__(self, **kwargs) -> None:
-        self.group = click.Group()
-        self.collection = CommandGroupCollection(sources=[self.group], **kwargs)
+    def __init__(self, context_settings: Optional[dict] = None) -> None:
+        if context_settings is None:
+            context_settings = CLICK_CONTEXT_SETTINGS
+
+        self.management_group = ClickCommonGroup()
+        self.common_group = CommandGroupCollection(
+            sources=[self.management_group],
+            context_settings=context_settings,
+        )
 
     def __call__(self, *args: Any, **kwargs: Any) -> None:
-        self.collection.main(*args, **kwargs)
+        self.common_group.main(*args, **kwargs)
 
     def register(self, module: ModuleType) -> None:
         if hasattr(module, "common"):
-            self.collection.add_source(module.common)
+            self.common_group.add_command(module.common)
         if hasattr(module, "management"):
-            self.group.add_command(module.management)
+            self.management_group.add_command(module.management)
 
 
-context_settings = dict(
-    help_option_names=["-h", "--help"],
-)
+def load_cli(**kwargs: Any) -> CLI:
+    if is_config_empty():
+        terminal.header("Welcome to Beta9! Let's get started 📡")
+        get_channel().close()
+
+    cli = CLI(**kwargs)
+    cli.register(task)
+    cli.register(deployment)
+    cli.register(volume)
+    cli.register(config)
+
+    return cli
+
 
-cli = CLI(context_settings=context_settings)
-cli.register(task)
-cli.register(deployment)
-cli.register(volume)
-cli.register(config)
+if __name__ == "beta9.cli.main":
+    cli = load_cli()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `beta9-0.1.6/src/beta9/cli/task.py` & `beta9-0.1.7/src/beta9/cli/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from typing import Dict, List
 
 import click
 from betterproto import Casing
 from rich.table import Column, Table, box
 
 from .. import aio, terminal
+from ..channel import ServiceClient
 from ..clients.gateway import (
-    GatewayServiceStub,
     ListTasksRequest,
     ListTasksResponse,
     StopTaskRequest,
     StopTaskResponse,
     StringList,
 )
-from .contexts import ServiceClient
+from . import extraclick
 from .extraclick import ClickManagementGroup
 
 
 @click.group(
     name="task",
     help="Manage tasks.",
     cls=ClickManagementGroup,
 )
-@click.pass_context
-def management(ctx: click.Context):
-    ctx.obj = ctx.with_resource(ServiceClient())
+def management():
+    pass
 
 
 def parse_filter_values(
     ctx: click.Context,
     param: click.Option,
     values: List[str],
 ) -> Dict[str, StringList]:
@@ -49,22 +48,25 @@
     return filters
 
 
 @management.command(
     name="list",
     help="List all tasks.",
     epilog="""
-    # List the first 10 tasks
-    beta9 task list --limit 10
+    Examples:
 
-    # List tasks with status 'running' or 'pending' and stub-id 'function/test:handler'
-    beta9 task list --filter status=running,pending --filter stub-id=function/test:handler
+      # List the first 10 tasks
+      {cli_name} task list --limit 10
 
-    # List tasks and output in JSON format
-    beta9 task list --format json
+      # List tasks with status 'running' or 'pending' and stub-id 'function/test:handler'
+      {cli_name} task list --filter status=running,pending --filter stub-id=function/test:handler
+
+      # List tasks and output in JSON format
+      {cli_name} task list --format json
+      \b
     """,
 )
 @click.option(
     "--limit",
     type=click.IntRange(1, 1000),
     default=100,
     help="The number of tasks to fetch.",
@@ -78,24 +80,24 @@
 )
 @click.option(
     "--filter",
     multiple=True,
     callback=parse_filter_values,
     help="Filters tasks. Add this option for each field you want to filter on.",
 )
-@click.pass_obj
+@extraclick.pass_service_client
 def list_tasks(service: ServiceClient, limit: int, format: str, filter: Dict[str, StringList]):
     res: ListTasksResponse
     res = aio.run_sync(service.gateway.list_tasks(ListTasksRequest(filters=filter, limit=limit)))
 
     if not res.ok:
         terminal.error(res.err_msg)
 
     if format == "json":
-        tasks = [task.to_dict(casing=Casing.SNAKE) for task in res.tasks]
+        tasks = [task.to_dict(casing=Casing.SNAKE) for task in res.tasks]  # type:ignore
         terminal.print_json(tasks)
         return
 
     table = Table(
         Column("Task ID"),
         Column("Status"),
         Column("Started At"),
@@ -130,15 +132,16 @@
     name="stop",
     help="Stop a task.",
 )
 @click.option(
     "--task-id",
     help="The task to stop.",
 )
-@click.pass_obj
-def stop_task(service: GatewayServiceStub, task_id: str):
-    res: StopTaskResponse = aio.run_sync(service.stop_task(StopTaskRequest(task_id=task_id)))
+@extraclick.pass_service_client
+def stop_task(service: ServiceClient, task_id: str):
+    res: StopTaskResponse
+    res = aio.run_sync(service.gateway.stop_task(StopTaskRequest(task_id=task_id)))
 
     if res.ok:
         terminal.detail(f"Stopped task {task_id}", dim=False)
     else:
         terminal.error(f"{res.err_msg}\nFailed to stop task {task_id}")
```

### Comparing `beta9-0.1.6/src/beta9/cli/volume.py` & `beta9-0.1.7/src/beta9/cli/volume.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from pathlib import Path
 from typing import Iterable, Union
 
 import click
 from rich.table import Column, Table, box
 
 from .. import aio, terminal
+from ..channel import ServiceClient
 from ..clients.volume import (
     CopyPathRequest,
     CopyPathResponse,
     DeletePathRequest,
     GetOrCreateVolumeRequest,
     GetOrCreateVolumeResponse,
     ListPathRequest,
     ListPathResponse,
     ListVolumesRequest,
     ListVolumesResponse,
 )
 from ..terminal import pluralize
-from .contexts import ServiceClient
+from . import extraclick
 from .extraclick import ClickCommonGroup, ClickManagementGroup
 
 
 @click.group(cls=ClickCommonGroup)
-@click.pass_context
-def common(ctx: click.Context):
-    ctx.obj = ctx.with_resource(ServiceClient())
+def common(**_):
+    pass
 
 
 @common.command(
     help="List contents in a volume.",
     epilog="""
     Match Syntax:
       This command provides support for Unix shell-style wildcards, which are not the same as regular expressions.
@@ -40,21 +40,21 @@
       [!seq]  matches any character not in `seq`
 
       For a literal match, wrap the meta-characters in brackets. For example, '[?]' matches the character '?'.
 
     Examples:
 
       # List files in the volume named myvol, in the directory named subdir/
-      beta9 ls myvol/subdir
+      {cli_name} ls myvol/subdir
 
       # List files ending in .txt in the directory named subdir
-      beta9 ls myvol/subdir/\\*.txt
+      {cli_name} ls myvol/subdir/\\*.txt
 
       # Same as above, but with single quotes to avoid escaping
-      beta9 ls 'myvol/subdir/*.txt'
+      {cli_name} ls 'myvol/subdir/*.txt'
       \b
     """,
 )
 @click.argument(
     "remote_path",
     required=True,
 )
@@ -62,27 +62,26 @@
     "--long-format",
     "-l",
     is_flag=True,
     default=False,
     show_default=True,
     help="Show mode, modified date, size, and name of file.",
 )
-@click.pass_obj
-def ls(service: ServiceClient, remote_path: str, long_format: bool) -> None:
-    with terminal.progress("Working..."):
-        req = ListPathRequest(path=remote_path, long_format=long_format)
-        res: ListPathResponse = aio.run_sync(service.volume.list_path(req))
+@extraclick.pass_service_client
+def ls(service: ServiceClient, remote_path: str, long_format: bool):
+    req = ListPathRequest(path=remote_path, long_format=long_format)
+    res: ListPathResponse = aio.run_sync(service.volume.list_path(req))
 
-        if not res.ok:
-            terminal.error(f"{remote_path} ({res.err_msg})")
+    if not res.ok:
+        terminal.error(f"{remote_path} ({res.err_msg})")
 
-        num_list, suffix = pluralize(res.paths)
-        terminal.header(f"{remote_path} (found {num_list} object{suffix})")
-        for p in res.paths:
-            terminal.print(p, highlight=False, markup=False)
+    num_list, suffix = pluralize(res.paths)
+    terminal.header(f"{remote_path} (found {num_list} object{suffix})")
+    for p in res.paths:
+        terminal.print(p, highlight=False, markup=False)
 
 
 @common.command(
     help="Copy contents to a volume.",
     epilog="""
     Match Syntax:
       This command provides support for Unix shell-style wildcards, which are not the same as regular expressions.
@@ -93,44 +92,44 @@
       [!seq]  matches any character not in `seq`
 
       For a literal match, wrap the meta-characters in brackets. For example, '[?]' matches the character '?'.
 
     Examples:
 
       # Copy contents to a remote volume
-      beta9 cp mydir myvol/subdir
-      beta9 cp myfile.txt myvol/subdir
+      {cli_name} cp mydir myvol/subdir
+      {cli_name} cp myfile.txt myvol/subdir
 
       # Use a question mark to match a single character in a path
-      beta9 cp 'mydir/?/data?.json' myvol/sub/path
+      {cli_name} cp 'mydir/?/data?.json' myvol/sub/path
 
       # Use an asterisk to match all characters in a path
-      beta9 cp 'mydir/*/*.json' myvol/data
+      {cli_name} cp 'mydir/*/*.json' myvol/data
 
       # Use a sequence to match a specific set of characters in a path
-      beta9 cp 'mydir/[a-c]/data[0-1].json' myvol/data
+      {cli_name} cp 'mydir/[a-c]/data[0-1].json' myvol/data
 
       # Escape special characters if you don't want to single quote your local path
-      beta9 cp mydir/\\[a-c\\]/data[0-1].json' myvol/data
-      beta9 cp mydir/\\?/data\\?.json myvol/sub/path
+      {cli_name} cp mydir/\\[a-c\\]/data[0-1].json' myvol/data
+      {cli_name} cp mydir/\\?/data\\?.json myvol/sub/path
       \b
     """,
 )
 @click.argument(
     "local_path",
     type=click.STRING,
     required=True,
 )
 @click.argument(
     "remote_path",
     type=click.STRING,
     required=True,
 )
-@click.pass_obj
-def cp(service: ServiceClient, local_path: str, remote_path: str) -> None:
+@extraclick.pass_service_client
+def cp(service: ServiceClient, local_path: str, remote_path: str):
     local_path = str(Path(local_path).resolve())
     files_to_upload = []
 
     for match in glob.glob(local_path, recursive=True):
         mpath = Path(match)
         if mpath.is_dir():
             files_to_upload.extend([p for p in mpath.rglob("*") if p.is_file()])
@@ -182,34 +181,34 @@
       [!seq]  matches any character not in `seq`
 
       For a literal match, wrap the meta-characters in brackets. For example, '[?]' matches the character '?'.
 
     Examples:
 
       # Remove the directory
-      beta9 rm myvol/subdir
+      {cli_name} rm myvol/subdir
 
       # Remove files ending in .json
-      beta9 rm myvol/\\*.json
+      {cli_name} rm myvol/\\*.json
 
       # Remove files with letters a - c in their names
-      beta9 rm myvol/\\[a-c\\].json
+      {cli_name} rm myvol/\\[a-c\\].json
 
       # Remove files, use single quotes to avoid escaping
-      beta9 rm 'myvol/?/[i-j][e-g]/*.txt'
+      {cli_name} rm 'myvol/?/[i-j][e-g]/*.txt'
       \b
     """,
 )
 @click.argument(
     "remote_path",
     type=click.STRING,
     required=True,
 )
-@click.pass_obj
-def rm(service: ServiceClient, remote_path: str) -> None:
+@extraclick.pass_service_client
+def rm(service: ServiceClient, remote_path: str):
     req = DeletePathRequest(path=remote_path)
     res = aio.run_sync(service.volume.delete_path(req))
 
     if not res.ok:
         terminal.error(f"{remote_path} ({res.err_msg})")
 
     num_del, suffix = pluralize(res.deleted)
@@ -219,24 +218,23 @@
 
 
 @click.group(
     name="volume",
     help="Manage volumes.",
     cls=ClickManagementGroup,
 )
-@click.pass_context
-def management(ctx: click.Context):
-    ctx.obj = ctx.with_resource(ServiceClient())
+def management():
+    pass
 
 
 @management.command(
     name="list",
     help="List available volumes.",
 )
-@click.pass_obj
+@extraclick.pass_service_client
 def list_volumes(service: ServiceClient):
     res: ListVolumesResponse
     res = aio.run_sync(service.volume.list_volumes(ListVolumesRequest()))
 
     if not res.ok:
         terminal.error(res.err_msg)
 
@@ -271,15 +269,15 @@
 )
 @click.option(
     "--name",
     "-n",
     type=click.STRING,
     required=True,
 )
-@click.pass_obj
+@extraclick.pass_service_client
 def create_volume(service: ServiceClient, name: str):
     res: GetOrCreateVolumeResponse
     res = aio.run_sync(service.volume.get_or_create_volume(GetOrCreateVolumeRequest(name=name)))
 
     if not res.ok:
         terminal.print(res.volume)
         terminal.error(res.err_msg)
```

### Comparing `beta9-0.1.6/src/beta9/clients/container/__init__.py` & `beta9-0.1.7/src/beta9/clients/container/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/clients/endpoint/__init__.py` & `beta9-0.1.7/src/beta9/clients/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/clients/function/__init__.py` & `beta9-0.1.7/src/beta9/clients/function/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/clients/gateway/__init__.py` & `beta9-0.1.7/src/beta9/clients/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/clients/image/__init__.py` & `beta9-0.1.7/src/beta9/clients/image/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/clients/map/__init__.py` & `beta9-0.1.7/src/beta9/clients/map/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/clients/simplequeue/__init__.py` & `beta9-0.1.7/src/beta9/clients/simplequeue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/clients/taskqueue/__init__.py` & `beta9-0.1.7/src/beta9/clients/taskqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/clients/volume/__init__.py` & `beta9-0.1.7/src/beta9/clients/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/logging.py` & `beta9-0.1.7/src/beta9/logging.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/runner/common.py` & `beta9-0.1.7/src/beta9/runner/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     """
 
     def __init__(self) -> None:
         self.pass_context: bool = False
         self.handler: Union[Callable, None] = None
         self._load()
 
-    def _load(self) -> Callable:
+    def _load(self):
         if sys.path[0] != USER_CODE_VOLUME:
             sys.path.insert(0, USER_CODE_VOLUME)
 
         try:
             module, func = config.handler.split(":")
             target_module = importlib.import_module(module)
             self.handler = getattr(target_module, func)
```

### Comparing `beta9-0.1.6/src/beta9/runner/container.py` & `beta9-0.1.7/src/beta9/runner/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import subprocess
 import sys
 from typing import Union
 
 from grpclib.client import Channel
 
 from ..aio import run_sync
+from ..channel import with_runner_context
 from ..clients.gateway import EndTaskRequest, GatewayServiceStub, StartTaskRequest
-from ..config import with_runner_context
 from ..logging import StdoutJsonInterceptor
 from ..runner.common import config
 from ..type import TaskStatus
 
 
 class ContainerManager:
     def __init__(self, cmd: str) -> None:
```

### Comparing `beta9-0.1.6/src/beta9/runner/endpoint.py` & `beta9-0.1.7/src/beta9/runner/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 from starlette.applications import Starlette
 from starlette.types import ASGIApp
 from uvicorn.workers import UvicornWorker
 
 from ..abstractions.base.runner import (
     ENDPOINT_SERVE_STUB_TYPE,
 )
+from ..channel import with_runner_context
 from ..clients.gateway import (
     EndTaskRequest,
     GatewayServiceStub,
     StartTaskRequest,
 )
-from ..config import with_runner_context
 from ..logging import StdoutJsonInterceptor
 from ..runner.common import FunctionContext, FunctionHandler, execute_lifecycle_method
 from ..runner.common import config as cfg
 from ..type import LifeCycleMethod, TaskStatus
 
 
 class EndpointFilter(logging.Filter):
```

### Comparing `beta9-0.1.6/src/beta9/runner/function.py` & `beta9-0.1.7/src/beta9/runner/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import cloudpickle
 import grpc
 import grpclib
 from grpclib.client import Channel
 from grpclib.exceptions import StreamTerminatedError
 
 from ..aio import run_sync
+from ..channel import with_runner_context
 from ..clients.function import (
     FunctionGetArgsRequest,
     FunctionGetArgsResponse,
     FunctionMonitorRequest,
     FunctionMonitorResponse,
     FunctionServiceStub,
     FunctionSetResultRequest,
@@ -22,15 +23,14 @@
 from ..clients.gateway import (
     EndTaskRequest,
     EndTaskResponse,
     GatewayServiceStub,
     StartTaskRequest,
     StartTaskResponse,
 )
-from ..config import with_runner_context
 from ..exceptions import InvalidFunctionArgumentsException, RunnerException
 from ..logging import StdoutJsonInterceptor
 from ..runner.common import FunctionContext, FunctionHandler, config, send_callback
 from ..type import TaskExitCode, TaskStatus
 
 
 def _load_args(args: bytes) -> dict:
```

### Comparing `beta9-0.1.6/src/beta9/runner/serve.py` & `beta9-0.1.7/src/beta9/runner/serve.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/src/beta9/runner/taskqueue.py` & `beta9-0.1.7/src/beta9/runner/taskqueue.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 import grpc
 import grpclib
 from grpclib.client import Channel
 from grpclib.exceptions import StreamTerminatedError
 
 from ..aio import run_sync
+from ..channel import with_runner_context
 from ..clients.gateway import GatewayServiceStub
 from ..clients.taskqueue import (
     TaskQueueCompleteRequest,
     TaskQueueCompleteResponse,
     TaskQueueMonitorRequest,
     TaskQueueMonitorResponse,
     TaskQueuePopRequest,
     TaskQueuePopResponse,
     TaskQueueServiceStub,
 )
-from ..config import with_runner_context
 from ..exceptions import RunnerException
 from ..logging import StdoutJsonInterceptor
 from ..runner.common import (
     FunctionContext,
     FunctionHandler,
     config,
     execute_lifecycle_method,
@@ -304,14 +304,16 @@
                             taskqueue_stub=taskqueue_stub,
                             gateway_stub=gateway_stub,
                         ),
                     )
 
                     start_time = time.time()
                     task_status = TaskStatus.Complete
+                    result = None
+
                     try:
                         args = task.args or []
                         kwargs = task.kwargs or {}
 
                         result = await loop.run_in_executor(
                             executor, lambda: handler(context, *args, **kwargs)
                         )
@@ -338,15 +340,15 @@
 
                         monitor_task.cancel()
                         print(f"Task completed <{task.id}>")
 
                         await send_callback(
                             gateway_stub=gateway_stub,
                             context=context,
-                            payload=result,
+                            payload=result or {},
                             task_status=task_status,
                         )  # Send callback to callback_url, if defined
 
             loop.run_until_complete(_run_task())
 
 
 if __name__ == "__main__":
```

### Comparing `beta9-0.1.6/src/beta9/sync.py` & `beta9-0.1.7/src/beta9/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         terminal.detail(f"Writing {IGNORE_FILE_NAME} file")
         with self.ignore_file_path.open(mode="w") as f:
             f.writelines(IGNORE_FILE_CONTENTS)
 
     def _read_ignore_file(self) -> list:
         if not is_local():
-            return
+            return []
 
         terminal.detail(f"Reading {IGNORE_FILE_NAME} file")
 
         patterns = []
 
         if self.ignore_file_path.is_file():
             with self.ignore_file_path.open() as file:
```

### Comparing `beta9-0.1.6/src/beta9/terminal.py` & `beta9-0.1.7/src/beta9/terminal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import sys
 from contextlib import contextmanager
-from typing import Any, Sequence, Tuple
+from typing import Any, Optional, Sequence, Tuple
 
 from rich.console import Console
 from rich.markup import escape
 from rich.progress import open as _progress_open
 from rich.text import Text
 
 _console = Console()
@@ -20,18 +20,19 @@
     _console.print(*objects, **kwargs)
 
 
 def print_json(data: Any, **kwargs: Any) -> None:
     _console.print_json(data=data, indent=2, default=lambda o: str(o), **kwargs)
 
 
-def prompt(*, text: str, default: Any) -> Any:
-    prompt_text = f"=> {text} [{default}]: "
-    _console.print(Text(prompt_text, style="bold blue"), end="")
-    user_input = input().strip()
+def prompt(
+    *, text: str, default: Optional[Any] = None, markup: bool = False, password: bool = False
+) -> Any:
+    prompt_text = f"{text} [{default}]: " if default is not None else f"{text}: "
+    user_input = _console.input(prompt_text, markup=markup, password=password).strip()
     return user_input if user_input else default
 
 
 def detail(text: str, dim: bool = True, **kwargs) -> None:
     style = "dim" if dim else ""
     _console.print(Text(text, style=style), **kwargs)
 
@@ -66,15 +67,15 @@
         refresh_per_second=60,
         **kwargs,
     )
 
     if "description" in options:
         options["description"] = escape(f"[{options['description']}]")
 
-    return _progress_open(file, mode, **options)
+    return _progress_open(file, mode, **options)  # type:ignore
 
 
 def humanize_date(d: datetime.datetime) -> str:
     # Check if datetime is "zero" time
     if d == datetime.datetime(1, 1, 1, tzinfo=datetime.timezone.utc):
         return ""
```

### Comparing `beta9-0.1.6/src/beta9/type.py` & `beta9-0.1.7/src/beta9/type.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.6/PKG-INFO` & `beta9-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: beta9
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: beam.cloud
 Author-email: support@beam.cloud
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
 Requires-Dist: betterproto[compiler] (==2.0.0b6)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
-Requires-Dist: fastapi (>=0.109.0,<0.110.0)
+Requires-Dist: fastapi (>=0.110.2,<0.111.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: grpclib (>=0.4.7,<0.5.0)
 Requires-Dist: protobuf (>=4.25.1,<5.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
```

