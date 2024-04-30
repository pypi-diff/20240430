# Comparing `tmp/spotflow_device-1.3.0-cp37-abi3-win_amd64.whl.zip` & `tmp/spotflow_device-2.0.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3394960 bytes, number of entries: 7
--rw-r--r--  4.6 unx      264 b- defN 24-Mar-19 09:58 spotflow_device-1.3.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Mar-19 09:58 spotflow_device-1.3.0.dist-info/WHEEL
--rw-r--r--  4.6 unx      143 b- defN 24-Mar-19 09:58 spotflow_device/__init__.py
--rw-r--r--  4.6 unx     3411 b- defN 24-Mar-19 09:58 spotflow_device/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-Mar-19 09:58 spotflow_device/py.typed
--rwxr-xr-x  4.6 unx  8232960 b- defN 24-Mar-19 09:58 spotflow_device/spotflow_device.pyd
--rw-r--r--  4.6 unx      570 b- defN 24-Mar-19 09:58 spotflow_device-1.3.0.dist-info/RECORD
-7 files, 8237442 bytes uncompressed, 3393948 bytes compressed:  58.8%
+Zip file size: 3366172 bytes, number of entries: 7
+-rw-r--r--  4.6 unx      513 b- defN 24-Apr-29 19:23 spotflow_device-2.0.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-Apr-29 19:23 spotflow_device-2.0.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      143 b- defN 24-Apr-29 19:23 spotflow_device/__init__.py
+-rw-r--r--  4.6 unx     2695 b- defN 24-Apr-29 19:23 spotflow_device/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-Apr-29 19:23 spotflow_device/py.typed
+-rwxr-xr-x  4.6 unx  8174592 b- defN 24-Apr-29 19:23 spotflow_device/spotflow_device.pyd
+-rw-r--r--  4.6 unx      570 b- defN 24-Apr-29 19:23 spotflow_device-2.0.0.dist-info/RECORD
+7 files, 8178607 bytes uncompressed, 3365160 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: spotflow_device-1.3.0.dist-info/METADATA
+Filename: spotflow_device-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: spotflow_device-1.3.0.dist-info/WHEEL
+Filename: spotflow_device-2.0.0.dist-info/WHEEL
 Comment: 
 
 Filename: spotflow_device/__init__.py
 Comment: 
 
 Filename: spotflow_device/__init__.pyi
 Comment: 
 
 Filename: spotflow_device/py.typed
 Comment: 
 
 Filename: spotflow_device/spotflow_device.pyd
 Comment: 
 
-Filename: spotflow_device-1.3.0.dist-info/RECORD
+Filename: spotflow_device-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotflow_device/__init__.pyi

```diff
@@ -1,58 +1,13 @@
 import enum
 from typing import Optional, Callable
 
 class SpotflowError(Exception):
     pass
 
-class DeviceClientOptions:
-    def __init__(self,
-                 database_file: str,
-                 provisioning_token: ProvisioningToken,
-                 device_id: Optional[str] = None) -> None: ...
-
-    @property
-    def database_file(self) -> str: ...
-
-    @database_file.setter
-    def database_file(self, value: str) -> None: ...
-
-    @property
-    def provisioning_token(self) -> ProvisioningToken: ...
-
-    @provisioning_token.setter
-    def provisioning_token(self, value: ProvisioningToken) -> None: ...
-
-    @property
-    def device_id(self) -> Optional[str]: ...
-
-    @device_id.setter
-    def device_id(self, value: Optional[str]) -> None: ...
-
-    @property
-    def instance(self) -> Optional[str]: ...
-
-    @instance.setter
-    def instance(self, value: Optional[str]) -> None: ...
-
-    @property
-    def display_provisioning_operation_callback(self) -> Optional[Callable[[ProvisioningOperation], None]]: ...
-
-    @display_provisioning_operation_callback.setter
-    def display_provisioning_operation_callback(self, value: Optional[Callable[[ProvisioningOperation], None]]) -> None: ...
-
-    @property
-    def desired_properties_updated_callback(self) -> Optional[Callable[[DesiredProperties], None]]: ...
-
-    @desired_properties_updated_callback.setter
-    def desired_properties_updated_callback(self, value: Optional[Callable[[DesiredProperties], None]]) -> None: ...
-
-class ProvisioningToken:
-    def __init__(self, token: str) -> None: ...
-
 class ProvisioningOperation:
     def __init__(self) -> None: ...
 
     @property
     def id(self) -> str: ...
 
     @property
@@ -64,28 +19,39 @@
 class Compression(enum.Enum):
     UNCOMPRESSED = 0
     FASTEST = 1
     SMALLEST_SIZE = 2
 
 class DeviceClient:
     @staticmethod
-    def start(options: DeviceClientOptions) -> DeviceClient: ...
+    def start(device_id: Optional[str],
+              provisioning_token: str,
+              db: str,
+              instance: Optional[str] = None,
+              display_provisioning_operation_callback: Optional[Callable[[ProvisioningOperation], None]] = None,
+              desired_properties_updated_callback: Optional[Callable[[DesiredProperties], None]] = None) -> DeviceClient:
+         ...
+
+    @property
+    def workspace_id(self) -> str: ...
 
     @property
     def device_id(self) -> str: ...
 
     def create_stream_sender(self,
                              stream_group: Optional[str] = None,
                              stream: Optional[str] = None,
                              compression: Optional[Compression] = Compression.UNCOMPRESSED) -> StreamSender:
         ...
 
     @property
     def pending_messages_count(self) -> int: ...
 
+    def wait_enqueued_messages_sent(self) -> None: ...
+
     def get_desired_properties(self) -> DesiredProperties: ...
 
     def get_desired_properties_if_newer(self, version: Optional[int] = None) -> Optional[DesiredProperties]: ...
 
     def update_reported_properties(self, properties: dict) -> None: ...
 
     @property
@@ -96,17 +62,25 @@
                      payload: str | bytes,
                      batch_id: Optional[str] = None,
                      message_id: Optional[str] = None,
                      batch_slice_id: Optional[str] = None,
                      chunk_id: Optional[str] = None) -> None:
         ...
 
-    def complete_batch(self, batch_id: str) -> None: ...
+    def enqueue_message(self, 
+                     payload: str | bytes,
+                     batch_id: Optional[str] = None,
+                     message_id: Optional[str] = None,
+                     batch_slice_id: Optional[str] = None,
+                     chunk_id: Optional[str] = None) -> None:
+        ...
+
+    def enqueue_batch_completion(self, batch_id: str) -> None: ...
 
-    def complete_message(self, batch_id: str, message_id: str) -> None: ...
+    def enqueue_message_completion(self, batch_id: str, message_id: str) -> None: ...
 
 class DesiredProperties:
     @property
     def version(self) -> int: ...
 
     @property
     def values(self) -> dict: ...
```

## Comparing `spotflow_device-1.3.0.dist-info/RECORD` & `spotflow_device-2.0.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-spotflow_device-1.3.0.dist-info/METADATA,sha256=1jMRY8Rm-ugSojhBpR3V6K8_N8mynd_WyjAvfeAXX0E,264
-spotflow_device-1.3.0.dist-info/WHEEL,sha256=d40ZnTlPFCUsdXDb0X9563rVL9wMWbhpBmBuaD2xdkg,94
+spotflow_device-2.0.0.dist-info/METADATA,sha256=d6GQCzKv12RGB0Nk8OyMeUeX90pZZMnJfUVeIlbn3PE,513
+spotflow_device-2.0.0.dist-info/WHEEL,sha256=2KdwICnFEHl2ghwQAXqeXd9gNxeAiTvogEqUIMDbYbo,94
 spotflow_device/__init__.py,sha256=JfDnDKXS9NhCUjE-SCX9orPSkyDRS_iyfQXF4XMWs5o,143
-spotflow_device/__init__.pyi,sha256=vv4fTCbiSUqLul5dABeNRtQjXArtZ4ECc2c7xgXQ0FY,3411
+spotflow_device/__init__.pyi,sha256=yVJmQtUt_FpAOjQ7HgpT6lJtmdEDpUCdxRtQX5brnvQ,2695
 spotflow_device/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-spotflow_device/spotflow_device.pyd,sha256=4JfDfl98LXsZDVQoT0FypaNZIUI9owOi1ADgfcVL0UU,8232960
-spotflow_device-1.3.0.dist-info/RECORD,,
+spotflow_device/spotflow_device.pyd,sha256=jxI5wWtu36Q0nOwcMxihruWL5KSPnzx_qNrzH8uIdPM,8174592
+spotflow_device-2.0.0.dist-info/RECORD,,
```

