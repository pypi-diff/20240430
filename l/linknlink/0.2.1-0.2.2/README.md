# Comparing `tmp/linknlink-0.2.1.tar.gz` & `tmp/linknlink-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linknlink-0.2.1.tar", last modified: Tue Mar 12 02:17:01 2024, max compression
+gzip compressed data, was "linknlink-0.2.2.tar", last modified: Tue Apr 30 13:47:18 2024, max compression
```

## Comparing `linknlink-0.2.1.tar` & `linknlink-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-12 02:17:01.073965 linknlink-0.2.1/
--rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-11-08 09:39:11.000000 linknlink-0.2.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      503 2024-03-12 02:17:01.073965 linknlink-0.2.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       77 2023-11-14 06:52:53.000000 linknlink-0.2.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-12 02:17:01.073965 linknlink-0.2.1/linknlink/
--rw-rw-r--   0 user      (1000) user      (1000)     3967 2023-11-14 03:18:06.000000 linknlink-0.2.1/linknlink/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      119 2023-11-10 07:08:46.000000 linknlink-0.2.1/linknlink/const.py
--rw-rw-r--   0 user      (1000) user      (1000)    11979 2024-01-16 10:06:11.000000 linknlink-0.2.1/linknlink/device.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-11-10 07:16:08.000000 linknlink-0.2.1/linknlink/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1847 2023-11-10 07:09:54.000000 linknlink-0.2.1/linknlink/protocol.py
--rw-rw-r--   0 user      (1000) user      (1000)     2350 2024-03-12 02:15:48.000000 linknlink-0.2.1/linknlink/remote.py
--rw-rw-r--   0 user      (1000) user      (1000)     1774 2024-03-08 02:56:11.000000 linknlink-0.2.1/linknlink/sensor.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-12 02:17:01.073965 linknlink-0.2.1/linknlink.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      503 2024-03-12 02:17:01.000000 linknlink-0.2.1/linknlink.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      369 2024-03-12 02:17:01.000000 linknlink-0.2.1/linknlink.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-12 02:17:01.000000 linknlink-0.2.1/linknlink.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-11-10 08:42:09.000000 linknlink-0.2.1/linknlink.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       18 2024-03-12 02:17:01.000000 linknlink-0.2.1/linknlink.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2024-03-12 02:17:01.000000 linknlink-0.2.1/linknlink.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-12 02:17:01.073965 linknlink-0.2.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      743 2024-03-12 02:16:45.000000 linknlink-0.2.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-30 13:47:18.857034 linknlink-0.2.2/
+-rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-11-08 09:39:11.000000 linknlink-0.2.2/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      503 2024-04-30 13:47:18.857034 linknlink-0.2.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       77 2023-11-14 06:52:53.000000 linknlink-0.2.2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-30 13:47:18.857034 linknlink-0.2.2/linknlink/
+-rw-rw-r--   0 user      (1000) user      (1000)     4080 2024-04-10 10:04:04.000000 linknlink-0.2.2/linknlink/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      269 2024-04-02 02:50:19.000000 linknlink-0.2.2/linknlink/const.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12633 2024-04-30 13:41:20.000000 linknlink-0.2.2/linknlink/device.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-11-10 07:16:08.000000 linknlink-0.2.2/linknlink/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1847 2023-11-10 07:09:54.000000 linknlink-0.2.2/linknlink/protocol.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9017 2024-04-30 13:37:50.000000 linknlink-0.2.2/linknlink/remote.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1774 2024-03-25 06:45:21.000000 linknlink-0.2.2/linknlink/sensor.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-30 13:47:18.857034 linknlink-0.2.2/linknlink.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      503 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      369 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-11-10 08:42:09.000000 linknlink-0.2.2/linknlink.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       18 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-30 13:47:18.857034 linknlink-0.2.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      743 2024-04-30 13:45:58.000000 linknlink-0.2.2/setup.py
```

### Comparing `linknlink-0.2.1/LICENSE` & `linknlink-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.1/linknlink/__init__.py` & `linknlink-0.2.2/linknlink/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 """The python-linknlink library."""
 import socket
 import typing as t
 
 from . import exceptions as e
 from .const import DEFAULT_BCAST_ADDR, DEFAULT_PORT, DEFAULT_TIMEOUT
 from .device import Device, scan, ping
-from .remote import ehub
+from .remote import ehub, eremote
 from .sensor import motion, eths
 
 SUPPORTED_TYPES = {
     motion: {
         0xAC7B: ("eMotion", "LinknLink"),
     },
     eths: {
         0xAC7C: ("eTHS", "LinknLink"),
     },
     ehub: {
         0x520B: ("eHub", "LinknLink"),
     },
+    eremote: {
+        0xAC99: ("eRemote", "LinknLink"),
+    },
 }
 
 
 def gendevice(
     dev_type: int,
     host: t.Tuple[str, int],
     mac: t.Union[bytes, str],
@@ -41,15 +44,15 @@
             mac,
             dev_type,
             name=name,
             model=model,
             manufacturer=manufacturer,
             is_locked=is_locked,
         )
-    return Device(host, mac, dev_type, name=name, is_locked=is_locked)
+    return Device(host, mac, dev_type, name=name, model=model, manufacturer=manufacturer, is_locked=is_locked)
 
 
 def hello(
     host: str,
     port: int = DEFAULT_PORT,
     timeout: int = DEFAULT_TIMEOUT,
 ) -> Device:
```

### Comparing `linknlink-0.2.1/linknlink/device.py` & `linknlink-0.2.2/linknlink/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         mac: t.Union[bytes, str],
         devtype: int,
         timeout: int = DEFAULT_TIMEOUT,
         name: str = "",
         model: str = "",
         manufacturer: str = "",
         is_locked: bool = False,
+        cb: callable = None,
     ) -> None:
         """Initialize the controller."""
         self.host = host
         self.mac = bytes.fromhex(mac) if isinstance(mac, str) else mac
         self.devtype = devtype
         self.timeout = timeout
         self.name = name
@@ -120,14 +121,15 @@
         self.manufacturer = manufacturer
         self.is_locked = is_locked
         self.count = random.randint(0x8000, 0xFFFF)
         self.iv = bytes.fromhex(self.__INIT_VECT)
         self.id = 0
         self.type = self.TYPE  # For backwards compatibility.
         self.lock = threading.Lock()
+        self.cb = cb
 
         self.aes = None
         self.update_aes(bytes.fromhex(self.__INIT_KEY))
 
     def __repr__(self) -> str:
         """Return a formal representation of the device."""
         return (
@@ -340,14 +342,28 @@
         packet[0x08:0x10] = len(payload).to_bytes(2, "little")
 
         p_checksum = sum(packet, 0xBEAF) & 0xFFFF
         p_checksum = sum(payload, p_checksum) & 0xFFFF
         packet[0x04:0x06] = p_checksum.to_bytes(2, "little")
 
         return packet
+    
+    def build_cmdstuV2(self, cmd: int, payload: bytes = b"") -> bytes:
+        """Build a command to send."""
+        packet = bytearray(0x0C)
+        packet[0x00:0x04] = bytes.fromhex("a5a55a5a")
+        packet[0x06:0x08] = cmd.to_bytes(2, "little")
+        packet[0x08:0x10] = len(payload).to_bytes(2, "little")
+        packet[0x10:0x12] = [0, 0]
+        if len(payload):
+            packet.extend(payload)
+        p_checksum = sum(packet, 0xBEAF) & 0xFFFF
+        # p_checksum = sum(payload, p_checksum) & 0xFFFF
+        packet[0x04:0x06] = p_checksum.to_bytes(2, "little")
+        return packet
 
     def analysis_data(self, payload: bytes):
         """Build a command to send."""
         if payload[:4].hex() != "a5a55a5a":
             return False
         
         # TODO checksum
```

### Comparing `linknlink-0.2.1/linknlink/exceptions.py` & `linknlink-0.2.2/linknlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.1/linknlink/protocol.py` & `linknlink-0.2.2/linknlink/protocol.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.1/linknlink/remote.py` & `linknlink-0.2.2/linknlink/sensor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,60 @@
-"""Support for universal remotes."""
-import struct
+"""Support for sensors."""
 
 from . import exceptions as e
 from .device import Device
+import json
 
-class ehub(Device):
-    """Controls a LinknLink ehub."""
+class eths(Device):
+    """Controls a LinknLink eths."""
 
-    TYPE = "EHUB"
+    TYPE = "ETHS"
     
-    # sensor function
     def _send(self, command: int, data: bytes = b"") -> bytes:
         """Send a packet to the device."""
-        packet = struct.pack("<HI", len(data) + 4, command) + data
-        resp = self.send_packet(0x6A, packet)
+        cmdstu = self.build_cmdstu(command)
+        resp = self.send_packet(0x6A, cmdstu)
         e.check_error(resp[0x22:0x24])
         payload = self.decrypt(resp[0x38:])
-        p_len = struct.unpack("<H", payload[:0x2])[0]
-        return payload[0x6 : p_len + 2]
+        res = self.analysis_data(payload)
+        return res[2]
     
     def check_sensors(self) -> dict:
         """Return the state of the sensors."""
-        resp = self._send(0x24)
+        resp = self._send(0x0b01)
+        try:
+            json_string = resp.decode('utf-8')
+            json_object = json.loads(json_string)
+        except Exception:
+            return {}
+        # return json_object
         return {
-            "envtemp": resp[0x0] + resp[0x1] / 100.0,
-            "envhumid": resp[0x2] + resp[0x3] / 100.0,
-            "pir_detected": resp[0x6],
+            "envtemp": float(json_object["envtemp"]) / 100.0,
+            "envhumid": float(json_object["envhumid"]) / 100.0,
         }
 
     def check_temperature(self) -> float:
         """Return the temperature."""
-        return self.check_sensors()["temperature"]
+        return float(self.check_sensors()["envtemp"]) / 100.0
 
     def check_humidity(self) -> float:
         """Return the humidity."""
-        return self.check_sensors()["humidity"]
-    
-    def check_pir(self) -> str:
-        """Return the pirDetected."""
-        return self.check_sensors()["pir_detected"]
+        return float(self.check_sensors()["envhumid"]) / 100.0
+
+class motion(eths):
+    """Controls a LinknLink motion."""
+
+    TYPE = "EMOTION"
 
-    # remote function
-    def sweep_frequency(self) -> None:
-        """Sweep frequency."""
-        self._send(0x19)
-
-    def check_frequency(self) -> bool:
-        """Return True if the frequency was identified successfully."""
-        resp = self._send(0x1A)
-        return resp[0] == 1
-
-    def find_rf_packet(self) -> None:
-        """Enter radiofrequency learning mode."""
-        self._send(0x1B)
-
-    def cancel_sweep_frequency(self) -> None:
-        """Cancel sweep frequency."""
-        self._send(0x1E)
-
-    def update(self) -> None:
-        """Update device name and lock status."""
-        resp = self._send(0x1)
-        self.name = resp[0x48:].split(b"\x00")[0].decode()
-        self.is_locked = bool(resp[0x87])
-
-    def send_data(self, data: bytes) -> None:
-        """Send a code to the device."""
-        self._send(0x2, data)
-
-    def enter_learning(self) -> None:
-        """Enter infrared learning mode."""
-        self._send(0x3)
-
-    def check_data(self) -> bytes:
-        """Return the last captured code."""
-        return self._send(0x4)
+    def check_sensors(self) -> dict:
+        """Return the state of the sensors."""
+        resp = self._send(0x0b01)
+        try:
+            json_string = resp.decode('utf-8')
+            json_object = json.loads(json_string)
+        except Exception:
+            return {}
+        return json_object
+
+    def check_pir(self) -> int:
+        """Return the pirDetected."""
+        return self.check_sensors()["pir_detected"]
```

### Comparing `linknlink-0.2.1/setup.py` & `linknlink-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
 from setuptools import setup, find_packages
 
 
-version = '0.2.1'
+version = '0.2.2'
 
 setup(
     name="linknlink",
     version=version,
     author="Zhao Zehua",
     author_email="huahua.zzh@gmail.com",
     url="https://github.com/xuanxuan000/python-linknlink",
```

