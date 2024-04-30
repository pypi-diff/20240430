# Comparing `tmp/pytest_initry-0.3.0.tar.gz` & `tmp/pytest_initry-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_initry-0.3.0.tar", max compression
+gzip compressed data, was "pytest_initry-0.4.0.tar", max compression
```

## Comparing `pytest_initry-0.3.0.tar` & `pytest_initry-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-15 05:59:57.071545 pytest_initry-0.3.0/LICENSE
--rw-r--r--   0        0        0     2536 2024-04-25 20:06:26.000000 pytest_initry-0.3.0/README.md
--rw-r--r--   0        0        0      901 2024-04-25 13:05:19.000000 pytest_initry-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 05:59:57.071545 pytest_initry-0.3.0/pytest_initry/__init__.py
--rw-r--r--   0        0        0    15176 2024-04-27 14:31:52.000000 pytest_initry-0.3.0/pytest_initry/plugin.py
--rw-r--r--   0        0        0       85 2024-04-15 05:59:57.071545 pytest_initry-0.3.0/pytest_initry/protobufs/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-25 09:38:03.860906 pytest_initry-0.3.0/pytest_initry/protobufs/responses_pb2.py
--rw-r--r--   0        0        0      391 2024-04-25 09:38:03.860906 pytest_initry-0.3.0/pytest_initry/protobufs/responses_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-25 09:38:03.860906 pytest_initry-0.3.0/pytest_initry/protobufs/responses_pb2_grpc.py
--rw-r--r--   0        0        0     2936 2024-04-25 09:38:03.936906 pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2.py
--rw-r--r--   0        0        0     2858 2024-04-25 09:38:03.936906 pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2.pyi
--rw-r--r--   0        0        0     6171 2024-04-25 09:38:03.936906 pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2_grpc.py
--rw-r--r--   0        0        0     1885 2024-04-25 09:38:03.900906 pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2.py
--rw-r--r--   0        0        0     1293 2024-04-25 09:38:03.900906 pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2.pyi
--rw-r--r--   0        0        0     3998 2024-04-25 09:38:03.900906 pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2_grpc.py
--rw-r--r--   0        0        0     1635 2024-04-25 09:38:03.976906 pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2.py
--rw-r--r--   0        0        0     1370 2024-04-25 09:38:03.976906 pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2.pyi
--rw-r--r--   0        0        0     2444 2024-04-25 09:38:03.976906 pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2_grpc.py
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 pytest_initry-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-15 05:59:57.071545 pytest_initry-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2536 2024-04-25 20:06:26.000000 pytest_initry-0.4.0/README.md
+-rw-r--r--   0        0        0      901 2024-04-30 17:41:31.000000 pytest_initry-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 05:59:57.071545 pytest_initry-0.4.0/pytest_initry/__init__.py
+-rw-r--r--   0        0        0    16250 2024-04-30 16:13:27.000000 pytest_initry-0.4.0/pytest_initry/plugin.py
+-rw-r--r--   0        0        0       85 2024-04-15 05:59:57.071545 pytest_initry-0.4.0/pytest_initry/protobufs/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-30 09:43:14.175038 pytest_initry-0.4.0/pytest_initry/protobufs/responses_pb2.py
+-rw-r--r--   0        0        0      391 2024-04-30 09:43:14.175038 pytest_initry-0.4.0/pytest_initry/protobufs/responses_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-30 09:43:14.175038 pytest_initry-0.4.0/pytest_initry/protobufs/responses_pb2_grpc.py
+-rw-r--r--   0        0        0     3041 2024-04-30 09:43:14.247038 pytest_initry-0.4.0/pytest_initry/protobufs/test_pb2.py
+-rw-r--r--   0        0        0     3134 2024-04-30 09:43:14.247038 pytest_initry-0.4.0/pytest_initry/protobufs/test_pb2.pyi
+-rw-r--r--   0        0        0     6171 2024-04-30 09:43:14.247038 pytest_initry-0.4.0/pytest_initry/protobufs/test_pb2_grpc.py
+-rw-r--r--   0        0        0     1885 2024-04-30 09:43:14.215038 pytest_initry-0.4.0/pytest_initry/protobufs/test_run_pb2.py
+-rw-r--r--   0        0        0     1293 2024-04-30 09:43:14.215038 pytest_initry-0.4.0/pytest_initry/protobufs/test_run_pb2.pyi
+-rw-r--r--   0        0        0     3998 2024-04-30 09:43:14.215038 pytest_initry-0.4.0/pytest_initry/protobufs/test_run_pb2_grpc.py
+-rw-r--r--   0        0        0     1635 2024-04-30 09:43:14.283038 pytest_initry-0.4.0/pytest_initry/protobufs/tests_pb2.py
+-rw-r--r--   0        0        0     1370 2024-04-30 09:43:14.283038 pytest_initry-0.4.0/pytest_initry/protobufs/tests_pb2.pyi
+-rw-r--r--   0        0        0     2444 2024-04-30 09:43:14.283038 pytest_initry-0.4.0/pytest_initry/protobufs/tests_pb2_grpc.py
+-rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 pytest_initry-0.4.0/PKG-INFO
```

### Comparing `pytest_initry-0.3.0/LICENSE` & `pytest_initry-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/README.md` & `pytest_initry-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/pyproject.toml` & `pytest_initry-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-initry"
-version = "0.3.0"
+version = "0.4.0"
 description = "Plugin for sending automation test data from Pytest to the initry"
 authors = ["Andrejs Smirnovs <and.inbx@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Framework :: Pytest",
 ]
```

### Comparing `pytest_initry-0.3.0/pytest_initry/plugin.py` & `pytest_initry-0.4.0/pytest_initry/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 import time
-
+import hashlib
 import pytest
 from _pytest.mark import deselect_by_keyword, deselect_by_mark
 import grpc
 import httpx
 from .protobufs import test_run_pb2_grpc
 from .protobufs import test_pb2_grpc
 from .protobufs import tests_pb2_grpc
@@ -34,104 +34,111 @@
                 response = rpc_method(request)
                 return response
             except grpc.RpcError as e:
                 self._handle_rpc_error(e)
                 return None
 
 
+def is_main_node(config):
+    return not hasattr(config, "workerinput")
+
+
 class PytestInitry:
     def __init__(self, config=None):
         self.config = config
         self.tests = list()
         self.xmlpath = config.option.xmlpath
-        self.test_run_uuid = str(uuid.uuid4())
         self.test_uuid = None
         self.pairs = []
         self.start_records = []
-        self.initry_batching_ini = config.getoption("initry_batching") or config.getini(
-            "initry_batching"
-        )
+        self.initry_batching_ini = config.getoption("initry_batching") or config.getini("initry_batching")
         self.initry_batching = self.initry_batching_ini
-        self.initry_host = config.getoption("initry_host") or config.getini(
-            "initry_host"
-        )
-        self.initry_port = config.getoption("initry_port") or config.getini(
-            "initry_port"
-        )
-        self.initry_grpc_port = config.getoption("initry_grpc_port") or config.getini(
-            "initry_grpc_port"
-        )
-        self.initry_junit_xml_only = config.getoption("initry_junit_xml_only") or config.getini(
-            "initry_junit_xml_only"
-        )
+        self.initry_host = config.getoption("initry_host") or config.getini("initry_host")
+        self.initry_port = config.getoption("initry_port") or config.getini("initry_port")
+        self.initry_grpc_port = config.getoption("initry_grpc_port") or config.getini("initry_grpc_port")
+        self.initry_junit_xml_only = config.getoption("initry_junit_xml_only") or config.getini("initry_junit_xml_only")
         self.test_run_grpc_client = GrpcClient(
             f"{self.initry_host}:{self.initry_grpc_port}",
             test_run_pb2_grpc.TestRunServiceStub,
         )
-        self.test_grpc_client = GrpcClient(
-            f"{self.initry_host}:{self.initry_grpc_port}", test_pb2_grpc.TestServiceStub
-        )
+        self.test_grpc_client = GrpcClient(f"{self.initry_host}:{self.initry_grpc_port}", test_pb2_grpc.TestServiceStub)
         self.cs_test_grpc_client = GrpcClient(
             f"{self.initry_host}:{self.initry_grpc_port}",
             test_pb2_grpc.ClientStreamTestServiceStub,
         )
         self.tests_grpc_client = GrpcClient(
             f"{self.initry_host}:{self.initry_grpc_port}",
             tests_pb2_grpc.TestsServiceStub,
         )
 
     def nodeid_converter(self, nodeid):
         """
-         Convert a nodeid string into a standardized format.
+        Convert a nodeid string into a standardized format.
 
-         Parameters:
-             nodeid (str): The original nodeid string to be converted.
+        Parameters:
+            nodeid (str): The original nodeid string to be converted.
+
+        Returns:
+            str: The converted nodeid string with '/' replaced by '.' and '::' replaced by '.'.
+                 Additionally, '.py' extension is removed.
+
+        Example:
+            >>> self.nodeid_converter("tests/classes/test_1.py::TestClass::test_one")
+            'tests.classes.test_1.TestClass.test_one'
+        """
+        return nodeid.replace("/", ".").replace("::", ".").replace(".py", "")
 
-         Returns:
-             str: The converted nodeid string with '/' replaced by '.' and '::' replaced by '.'.
-                  Additionally, '.py' extension is removed.
-
-         Example:
-             >>> self.nodeid_converter("tests/classes/test_1.py::TestClass::test_one")
-             'tests.classes.test_1.TestClass.test_one'
-         """
-        return nodeid.replace('/', '.').replace('::', '.').replace('.py', '')
+    def generate_test_id(self, shared_uuid, data):
+        string = (shared_uuid + data).encode("utf-8")
+        number_str = str(int(hashlib.md5(string).hexdigest(), 16))[0:31]
+        number = int(number_str)
+        hex_number = hex(number)[2:]
+        hex_number_padded = hex_number.zfill(32)
+        return str(uuid.UUID(hex=hex_number_padded))
 
-    def append_test(self, item):
+    def append_test(self, item, shared_uuid):
         test = dict()
         test["location"] = item.location[2]
         test["nodeid"] = self.nodeid_converter(item.nodeid)
-        test["uuid"] = str(uuid.uuid4())
-        test["test_run_uuid"] = self.test_run_uuid
+        if shared_uuid:
+            test["uuid"] = self.generate_test_id(shared_uuid, item.nodeid)
+        else:
+            test["uuid"] = str(uuid.uuid4())
+        test["test_run_uuid"] = shared_uuid
         test["description"] = item._obj.__doc__
         self.tests.append(test)
 
     def pytest_collection_modifyitems(self, session, items, config):
+        if not is_main_node(config):
+            shared_uuid = session.config.workerinput["shared_uuid"]
+        else:
+            shared_uuid = session.config.shared_uuid
+
         started_at = Timestamp(seconds=int(time.time()))
 
         deselect_by_keyword(items, config)
         deselect_by_mark(items, config)
 
         for item in session.items:
-            self.append_test(item)
+            self.append_test(item, shared_uuid)
 
         if self.initry_junit_xml_only is False:
             plugin_type = "pytest.initry"
             if self.xmlpath:
                 plugin_type = "pytest.initry.xml"
 
             request_data = test_run_pb2.CreateTestRunRequest(
                 tests_count=len(session.items),
                 started_at=started_at,
-                uuid=self.test_run_uuid,
+                uuid=shared_uuid,
                 plugin_type=plugin_type,
             )
         else:
             request_data = test_run_pb2.CreateTestRunRequest(
-                uuid=self.test_run_uuid,
+                uuid=shared_uuid,
                 started_at=started_at,
                 plugin_type="pytest.xml",
             )
         self.test_run_grpc_client.call_rpc_method("CreateTestRun", request_data)
 
         if self.initry_junit_xml_only:
             request_data = tests_pb2.CreateTestsRequest(tests=self.tests, only_tests_info=True)
@@ -152,63 +159,53 @@
                     status=test_pb2.TestStatus.RUNNING,
                 )
                 if self.initry_batching:
                     self.start_records.append(request_data)
                 else:
                     self.test_grpc_client.call_rpc_method("StartTest", request_data)
 
-    def started_finished_pairs(self):
+    def started_finished_pairs(self, report):
         if self.initry_junit_xml_only is False:
+
             def find_something(uuid: str):
-                _started_at = [
-                    req.started_at
-                    for req in self.pairs
-                    if req.uuid == uuid and hasattr(req, "started_at")
-                ][0]
-                _stopped_at = [
-                    req.stopped_at
-                    for req in self.pairs
-                    if req.uuid == uuid and hasattr(req, "stopped_at")
-                ][0]
-                _status = [
-                    req.status
-                    for req in self.pairs
-                    if req.uuid == uuid and hasattr(req, "stopped_at")
-                ][0]
+                _started_at = [req.started_at for req in self.pairs if req.uuid == uuid and hasattr(req, "started_at")][
+                    0
+                ]
+                _stopped_at = [req.stopped_at for req in self.pairs if req.uuid == uuid and hasattr(req, "stopped_at")][
+                    0
+                ]
+                _status = [req.status for req in self.pairs if req.uuid == uuid and hasattr(req, "stopped_at")][0]
                 return _started_at, _stopped_at, _status
 
             request = None
             for item in self.pairs:
                 started_at, stopped_at, status = find_something(item.uuid)
                 request = test_pb2.ModifyTestRequest(
                     uuid=item.uuid,
                     started_at=started_at,
                     stopped_at=stopped_at,
                     status=status,
+                    log=report.longreprtext,
+                    stdout=report.capstdout,
+                    stderr=report.capstderr,
                 )
             yield request
 
-    def create_pairs_for_batching(self, request):
+    def create_pairs_for_batching(self, request, report):
         if self.initry_junit_xml_only is False:
-            start_record = [
-                record for record in self.start_records if record.uuid == self.test_uuid
-            ][0]
+            start_record = [record for record in self.start_records if record.uuid == self.test_uuid][0]
             if start_record:
                 # send start and stop to self.pairs
                 self.pairs.append(start_record)
                 self.pairs.append(request)
 
                 # clean start_records for previous start_record
-                self.start_records = [
-                    record for record in self.start_records if record.uuid != self.test_uuid
-                ]
+                self.start_records = [record for record in self.start_records if record.uuid != self.test_uuid]
 
-                self.cs_test_grpc_client.call_rpc_method(
-                    "ModifyTest", self.started_finished_pairs()
-                )
+                self.cs_test_grpc_client.call_rpc_method("ModifyTest", self.started_finished_pairs(report))
                 self.pairs = []
 
     def pytest_runtest_logreport(self, report):
         if self.initry_junit_xml_only is False:
             if self.test_uuid is not None:
                 if report.when == "call" and report.outcome == "failed":
                     if report.failed and not hasattr(report, "wasxfail"):
@@ -219,87 +216,95 @@
                             log=report.longreprtext,
                             stdout=report.capstdout,
                             stderr=report.capstderr,
                         )
                         if not self.initry_batching:
                             self.test_grpc_client.call_rpc_method("StopTest", request)
                         else:
-                            self.create_pairs_for_batching(request)
+                            self.create_pairs_for_batching(request, report)
                 elif report.when == "setup" and report.outcome == "failed":
                     if report.failed and not hasattr(report, "wasxfail"):
                         request = test_pb2.StopTestRequest(
                             uuid=self.test_uuid,
                             stopped_at=Timestamp(seconds=int(time.time())),
                             status=test_pb2.TestStatus.FAILED,
                             log=report.longreprtext,
                             stdout=report.capstdout,
                             stderr=report.capstderr,
                         )
                         if not self.initry_batching:
                             self.test_grpc_client.call_rpc_method("StopTest", request)
                         else:
-                            self.create_pairs_for_batching(request)
+                            self.create_pairs_for_batching(request, report)
                 elif report.when == "call" and report.outcome == "passed":
                     request = test_pb2.StopTestRequest(
                         uuid=self.test_uuid,
                         stopped_at=Timestamp(seconds=int(time.time())),
                         status=test_pb2.TestStatus.PASSED,
                     )
                     if not self.initry_batching:
                         self.test_grpc_client.call_rpc_method("StopTest", request)
                     else:
-                        self.create_pairs_for_batching(request)
+                        self.create_pairs_for_batching(request, report)
 
                 elif (report.when == "call" and report.outcome == "skipped") or (
                     report.when == "setup" and report.outcome == "skipped"
                 ):
                     request = test_pb2.StopTestRequest(
                         uuid=self.test_uuid,
                         stopped_at=Timestamp(seconds=int(time.time())),
                         status=test_pb2.TestStatus.SKIPPED,
+                        log=report.longreprtext,
+                        stdout=report.capstdout,
+                        stderr=report.capstderr,
                     )
                     if not self.initry_batching:
                         self.test_grpc_client.call_rpc_method("StopTest", request)
                     else:
-                        self.create_pairs_for_batching(request)
+                        self.create_pairs_for_batching(request, report)
                 elif report.when == "call" and report.outcome == "xfailed":
                     request = test_pb2.StopTestRequest(
                         uuid=self.test_uuid,
                         stopped_at=Timestamp(seconds=int(time.time())),
                         status=test_pb2.TestStatus.EXPECTED_FAILED,
+                        log=report.longreprtext,
+                        stdout=report.capstdout,
+                        stderr=report.capstderr,
                     )
                     if not self.initry_batching:
                         self.test_grpc_client.call_rpc_method("StopTest", request)
                     else:
-                        self.create_pairs_for_batching(request)
+                        self.create_pairs_for_batching(request, report)
                 elif report.when == "call" and report.outcome == "xpassed":
                     request = test_pb2.StopTestRequest(
                         uuid=self.test_uuid,
                         stopped_at=Timestamp(seconds=int(time.time())),
                         status=test_pb2.TestStatus.EXPECTED_PASSED,
                     )
                     if not self.initry_batching:
                         self.test_grpc_client.call_rpc_method("StopTest", request)
                     else:
-                        self.create_pairs_for_batching(request)
+                        self.create_pairs_for_batching(request, report)
 
     def pytest_sessionfinish(self, session):
+        if not is_main_node(session.config):
+            shared_uuid = session.config.workerinput["shared_uuid"]
+        else:
+            shared_uuid = session.config.shared_uuid
+
         if self.xmlpath:
-            timeout = httpx.Timeout(None, read=180.0)
-            files = {'file': open(self.config.option.xmlpath, 'rb')}
-            with httpx.Client(timeout=timeout) as client:
+            files = {"file": open(self.config.option.xmlpath, "rb")}
+            with httpx.Client(timeout=360) as client:
                 if self.initry_junit_xml_only:
-                    data = {"uuid": self.test_run_uuid, "mode": "xml_only"}
+                    data = {"uuid": shared_uuid, "mode": "xml_only"}
                 else:
-                    data = {"uuid": self.test_run_uuid, "mode": "store"}
-                url = f'http://{self.initry_host}:{self.initry_port}/api/test-runs/xml'
+                    data = {"uuid": shared_uuid, "mode": "store"}
+                url = f"http://{self.initry_host}:{self.initry_port}/api/test-runs/xml"
                 client.post(url, files=files, data=data)
-        request_data = test_run_pb2.StopTestRunRequest(
-                uuid=self.test_run_uuid, stopped_at=Timestamp(seconds=int(time.time()))
-            )
+        request_data = test_run_pb2.StopTestRunRequest(uuid=shared_uuid, stopped_at=Timestamp(seconds=int(time.time())))
         self.test_run_grpc_client.call_rpc_method("StopTestRun", request_data)
 
 
 def pytest_addoption(parser):
     group = parser.getgroup("pytest-initry")
     group.addoption(
         "--initry-host",
@@ -336,18 +341,25 @@
         action="store",
         help="No realtime, only use JUnit XML report as source data",
     )
     parser.addini("initry_host", help="initry host", default=None)
     parser.addini("initry_port", help="initry port", default=None)
     parser.addini("initry_grpc_port", help="initry gRPC port", default=None)
     parser.addini("initry_batching", type="bool", help="batch mode", default=None)
-    parser.addini("initry_junit_xml_only", type="bool", help="No realtime, only use JUnit XML report as source data", default=False)
+    parser.addini(
+        "initry_junit_xml_only",
+        type="bool",
+        help="No realtime, only use JUnit XML report as source data",
+        default=False,
+    )
 
 
 def pytest_configure(config):
+    if is_main_node(config):
+        config.shared_uuid = str(uuid.uuid4())
     initry = config.getoption("initry_host") or config.getini("initry_host")
     if initry:
         plugin = PytestInitry(config)
         config._initry = plugin
         config.pluginmanager.register(plugin)
     junitxml = config.option.xmlpath
     junit_xml_only = config.getoption("initry_junit_xml_only") or config.getini("initry_junit_xml_only")
@@ -356,15 +368,20 @@
     if junit_xml_only is True and junitxml is None:
         pytest_unconfigure(config)
         raise pytest.UsageError("'initry_junit_xml_only' config option must be used only with 'junitxml' argument")
 
     if junit_xml_only is True and batching is True:
         raise pytest.UsageError(
             "'initry_batching' config option must not be used together with 'initry_junit_xml_only'. "
-            "There is no point in doing so because the 'initry_junit_xml_only' mode does not utilize real-time reporting.")
+            "There is no point in doing so because the 'initry_junit_xml_only' mode does not utilize real-time reporting."
+        )
+
+
+def pytest_configure_node(node):
+    node.workerinput["shared_uuid"] = node.config.shared_uuid
 
 
 def pytest_unconfigure(config):
     plugin = getattr(config, "_initry", None)
     if plugin is not None:
         del config._initry
         config.pluginmanager.unregister(plugin)
```

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/responses_pb2.py` & `pytest_initry-0.4.0/pytest_initry/protobufs/responses_pb2.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2.py` & `pytest_initry-0.4.0/pytest_initry/protobufs/test_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 import responses_pb2 as responses__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ntest.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0fresponses.proto\"m\n\x10StartTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x03 \x01(\x0e\x32\x0b.TestStatus\"\x99\x01\n\x0fStopTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstopped_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x03 \x01(\x0e\x32\x0b.TestStatus\x12\x0b\n\x03log\x18\x04 \x01(\t\x12\x0e\n\x06stdout\x18\x05 \x01(\t\x12\x0e\n\x06stderr\x18\x06 \x01(\t\"\x9e\x01\n\x11ModifyTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstopped_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x04 \x01(\x0e\x32\x0b.TestStatus*\x80\x01\n\nTestStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\n\n\x06PASSED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x0b\n\x07SKIPPED\x10\x04\x12\x13\n\x0f\x45XPECTED_PASSED\x10\x05\x12\x13\n\x0f\x45XPECTED_FAILED\x10\x06\x12\t\n\x05\x45RROR\x10\x07\x32\x61\n\x0bTestService\x12)\n\tStartTest\x12\x11.StartTestRequest\x1a\t.StatusOk\x12\'\n\x08StopTest\x12\x10.StopTestRequest\x1a\t.StatusOk2H\n\x17\x43lientStreamTestService\x12-\n\nModifyTest\x12\x12.ModifyTestRequest\x1a\t.StatusOk(\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ntest.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0fresponses.proto\"m\n\x10StartTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x03 \x01(\x0e\x32\x0b.TestStatus\"\x99\x01\n\x0fStopTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstopped_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x03 \x01(\x0e\x32\x0b.TestStatus\x12\x0b\n\x03log\x18\x04 \x01(\t\x12\x0e\n\x06stdout\x18\x05 \x01(\t\x12\x0e\n\x06stderr\x18\x06 \x01(\t\"\xcb\x01\n\x11ModifyTestRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstopped_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x06status\x18\x04 \x01(\x0e\x32\x0b.TestStatus\x12\x0b\n\x03log\x18\x05 \x01(\t\x12\x0e\n\x06stdout\x18\x06 \x01(\t\x12\x0e\n\x06stderr\x18\x07 \x01(\t*\x80\x01\n\nTestStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\n\n\x06PASSED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x0b\n\x07SKIPPED\x10\x04\x12\x13\n\x0f\x45XPECTED_PASSED\x10\x05\x12\x13\n\x0f\x45XPECTED_FAILED\x10\x06\x12\t\n\x05\x45RROR\x10\x07\x32\x61\n\x0bTestService\x12)\n\tStartTest\x12\x11.StartTestRequest\x1a\t.StatusOk\x12\'\n\x08StopTest\x12\x10.StopTestRequest\x1a\t.StatusOk2H\n\x17\x43lientStreamTestService\x12-\n\nModifyTest\x12\x12.ModifyTestRequest\x1a\t.StatusOk(\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'test_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_TESTSTATUS']._serialized_start=493
-  _globals['_TESTSTATUS']._serialized_end=621
+  _globals['_TESTSTATUS']._serialized_start=538
+  _globals['_TESTSTATUS']._serialized_end=666
   _globals['_STARTTESTREQUEST']._serialized_start=64
   _globals['_STARTTESTREQUEST']._serialized_end=173
   _globals['_STOPTESTREQUEST']._serialized_start=176
   _globals['_STOPTESTREQUEST']._serialized_end=329
   _globals['_MODIFYTESTREQUEST']._serialized_start=332
-  _globals['_MODIFYTESTREQUEST']._serialized_end=490
-  _globals['_TESTSERVICE']._serialized_start=623
-  _globals['_TESTSERVICE']._serialized_end=720
-  _globals['_CLIENTSTREAMTESTSERVICE']._serialized_start=722
-  _globals['_CLIENTSTREAMTESTSERVICE']._serialized_end=794
+  _globals['_MODIFYTESTREQUEST']._serialized_end=535
+  _globals['_TESTSERVICE']._serialized_start=668
+  _globals['_TESTSERVICE']._serialized_end=765
+  _globals['_CLIENTSTREAMTESTSERVICE']._serialized_start=767
+  _globals['_CLIENTSTREAMTESTSERVICE']._serialized_end=839
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2.pyi` & `pytest_initry-0.4.0/pytest_initry/protobufs/test_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -49,17 +49,23 @@
     status: TestStatus
     log: str
     stdout: str
     stderr: str
     def __init__(self, uuid: _Optional[str] = ..., stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[TestStatus, str]] = ..., log: _Optional[str] = ..., stdout: _Optional[str] = ..., stderr: _Optional[str] = ...) -> None: ...
 
 class ModifyTestRequest(_message.Message):
-    __slots__ = ("uuid", "started_at", "stopped_at", "status")
+    __slots__ = ("uuid", "started_at", "stopped_at", "status", "log", "stdout", "stderr")
     UUID_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     STOPPED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    LOG_FIELD_NUMBER: _ClassVar[int]
+    STDOUT_FIELD_NUMBER: _ClassVar[int]
+    STDERR_FIELD_NUMBER: _ClassVar[int]
     uuid: str
     started_at: _timestamp_pb2.Timestamp
     stopped_at: _timestamp_pb2.Timestamp
     status: TestStatus
-    def __init__(self, uuid: _Optional[str] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[TestStatus, str]] = ...) -> None: ...
+    log: str
+    stdout: str
+    stderr: str
+    def __init__(self, uuid: _Optional[str] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., stopped_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[TestStatus, str]] = ..., log: _Optional[str] = ..., stdout: _Optional[str] = ..., stderr: _Optional[str] = ...) -> None: ...
```

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2_grpc.py` & `pytest_initry-0.4.0/pytest_initry/protobufs/test_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2.py` & `pytest_initry-0.4.0/pytest_initry/protobufs/test_run_pb2.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2.pyi` & `pytest_initry-0.4.0/pytest_initry/protobufs/test_run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2_grpc.py` & `pytest_initry-0.4.0/pytest_initry/protobufs/test_run_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2.py` & `pytest_initry-0.4.0/pytest_initry/protobufs/tests_pb2.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2.pyi` & `pytest_initry-0.4.0/pytest_initry/protobufs/tests_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2_grpc.py` & `pytest_initry-0.4.0/pytest_initry/protobufs/tests_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.3.0/PKG-INFO` & `pytest_initry-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-initry
-Version: 0.3.0
+Version: 0.4.0
 Summary: Plugin for sending automation test data from Pytest to the initry
 Home-page: https://github.com/initry/pytest-initry
 License: MIT
 Keywords: pytest,initry
 Author: Andrejs Smirnovs
 Author-email: and.inbx@gmail.com
 Requires-Python: >=3.11,<4.0
```

