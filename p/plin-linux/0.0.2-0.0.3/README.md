# Comparing `tmp/plin-linux-0.0.2.tar.gz` & `tmp/plin_linux-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plin-linux-0.0.2.tar", last modified: Fri Aug 11 19:13:54 2023, max compression
+gzip compressed data, was "plin_linux-0.0.3.tar", last modified: Tue Apr 30 00:29:53 2024, max compression
```

## Comparing `plin-linux-0.0.2.tar` & `plin_linux-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxr-x   0 williamzhang  (1000) williamzhang  (1000)        0 2023-08-11 19:13:54.338316 plin-linux-0.0.2/
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)    11353 2023-04-18 20:26:02.000000 plin-linux-0.0.2/LICENSE
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     3659 2023-08-11 19:13:54.338316 plin-linux-0.0.2/PKG-INFO
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     3065 2023-08-08 01:04:10.000000 plin-linux-0.0.2/README.md
-drwxrwxr-x   0 williamzhang  (1000) williamzhang  (1000)        0 2023-08-11 19:13:54.338316 plin-linux-0.0.2/plin/
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)        0 2023-04-18 20:26:02.000000 plin-linux-0.0.2/plin/__init__.py
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)    20499 2023-08-08 00:47:54.000000 plin-linux-0.0.2/plin/device.py
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     2779 2023-08-08 00:47:59.000000 plin-linux-0.0.2/plin/enums.py
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     7852 2023-08-08 00:48:05.000000 plin-linux-0.0.2/plin/structs.py
-drwxrwxr-x   0 williamzhang  (1000) williamzhang  (1000)        0 2023-08-11 19:13:54.338316 plin-linux-0.0.2/plin_linux.egg-info/
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     3659 2023-08-11 19:13:54.000000 plin-linux-0.0.2/plin_linux.egg-info/PKG-INFO
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)      304 2023-08-11 19:13:54.000000 plin-linux-0.0.2/plin_linux.egg-info/SOURCES.txt
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)        1 2023-08-11 19:13:54.000000 plin-linux-0.0.2/plin_linux.egg-info/dependency_links.txt
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)       10 2023-08-11 19:13:54.000000 plin-linux-0.0.2/plin_linux.egg-info/requires.txt
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)        5 2023-08-11 19:13:54.000000 plin-linux-0.0.2/plin_linux.egg-info/top_level.txt
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)      704 2023-08-11 19:13:32.000000 plin-linux-0.0.2/pyproject.toml
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)       38 2023-08-11 19:13:54.338316 plin-linux-0.0.2/setup.cfg
-drwxrwxr-x   0 williamzhang  (1000) williamzhang  (1000)        0 2023-08-11 19:13:54.338316 plin-linux-0.0.2/tests/
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)      268 2023-08-08 00:45:23.000000 plin-linux-0.0.2/tests/test_message.py
--rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     4121 2023-08-08 00:45:47.000000 plin-linux-0.0.2/tests/test_plin.py
+drwxrwxr-x   0 williamzhang  (1000) williamzhang  (1000)        0 2024-04-30 00:29:53.493989 plin_linux-0.0.3/
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)    11353 2023-04-18 20:26:02.000000 plin_linux-0.0.3/LICENSE
+-rw-r--r--   0 williamzhang  (1000) williamzhang  (1000)     3752 2024-04-30 00:29:53.493989 plin_linux-0.0.3/PKG-INFO
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     3133 2024-04-12 01:21:50.000000 plin_linux-0.0.3/README.md
+drwxrwxr-x   0 williamzhang  (1000) williamzhang  (1000)        0 2024-04-30 00:29:53.493989 plin_linux-0.0.3/plin/
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)        0 2023-04-18 20:26:02.000000 plin_linux-0.0.3/plin/__init__.py
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)    20738 2024-04-29 23:47:17.000000 plin_linux-0.0.3/plin/device.py
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     2779 2023-08-08 00:47:59.000000 plin_linux-0.0.3/plin/enums.py
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)     7852 2023-08-08 00:48:05.000000 plin_linux-0.0.3/plin/structs.py
+drwxrwxr-x   0 williamzhang  (1000) williamzhang  (1000)        0 2024-04-30 00:29:53.493989 plin_linux-0.0.3/plin_linux.egg-info/
+-rw-r--r--   0 williamzhang  (1000) williamzhang  (1000)     3752 2024-04-30 00:29:53.000000 plin_linux-0.0.3/plin_linux.egg-info/PKG-INFO
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)      263 2024-04-30 00:29:53.000000 plin_linux-0.0.3/plin_linux.egg-info/SOURCES.txt
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)        1 2024-04-30 00:29:53.000000 plin_linux-0.0.3/plin_linux.egg-info/dependency_links.txt
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)       10 2024-04-30 00:29:53.000000 plin_linux-0.0.3/plin_linux.egg-info/requires.txt
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)        5 2024-04-30 00:29:53.000000 plin_linux-0.0.3/plin_linux.egg-info/top_level.txt
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)      704 2024-04-30 00:28:52.000000 plin_linux-0.0.3/pyproject.toml
+-rw-rw-r--   0 williamzhang  (1000) williamzhang  (1000)       38 2024-04-30 00:29:53.493989 plin_linux-0.0.3/setup.cfg
```

### Comparing `plin-linux-0.0.2/LICENSE` & `plin_linux-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plin-linux-0.0.2/PKG-INFO` & `plin_linux-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: plin-linux
-Version: 0.0.2
+Version: 0.0.3
 Summary: The python-plin package is a Python wrapper for the chardev API provided by the PEAK LIN Linux Beta.
 Author-email: William Zhang <williamzhang@rivian.com>
 Project-URL: Homepage, https://github.com/rivian/python-plin
 Project-URL: Bug Tracker, https://github.com/rivian/python-plin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ioctl_opt
 
 # Python PLIN library
 This library provides a Python interface for interacting with PEAK devices such as the PCAN-USB Pro and PLIN-USB on Linux using the chardev API provided by the PEAK LIN Linux Beta. The PEAK Linux beta driver is required to use this library and is available [here](https://forum.peak-system.com/viewtopic.php?t=5875).
 
 ## Installation
 The `plin-linux` package is available on [PyPI](https://pypi.org/project/plin-linux/) and can be directly installed with `pip install plin-linux`.
 
 ## Examples
 Runnable examples are located in the `examples/` directory.
 
 ### Master Example
 ```python
-from plin.plin import PLIN
+from plin.device import PLIN
 from plin.enums import (PLINFrameChecksumType, PLINFrameDirection,
                         PLINFrameFlag, PLINMode)
 
 # Initializes /dev/plin0 as a LIN master
 master = PLIN(interface="/dev/plin0")
 
 master.start(mode=PLINMode.MASTER, baudrate=19200)
@@ -70,15 +71,15 @@
     result = master.read()
     print(result)
 
 ```
 
 ### Slave Example
 ```python
-from plin.plin import PLIN
+from plin.device import PLIN
 from plin.enums import PLINMode
 
 # Initializes /dev/plin0 as a LIN slave
 slave = PLIN(interface="/dev/plin0")
 
 slave.start(mode=PLINMode.SLAVE, baudrate=19200)
 
@@ -89,19 +90,21 @@
 while True:
     result = slave.read()
     print(result)
 
 ```
 
 ## Unit Tests
-Unit tests are located in the `unit_tests/` directory and require a PEAK LIN device connected to run.
+* Unit tests are located in the `unit_tests/` directory.
+* Tests in `unit_tests/integration/` require a PEAK LIN device connected to run.
+* Can be run with `pytest`.
 
 ## License
 
-    Copyright 2023 Rivian Automotive, Inc.
+    Copyright 2024 Rivian Automotive, Inc.
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `plin-linux-0.0.2/README.md` & `plin_linux-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 The `plin-linux` package is available on [PyPI](https://pypi.org/project/plin-linux/) and can be directly installed with `pip install plin-linux`.
 
 ## Examples
 Runnable examples are located in the `examples/` directory.
 
 ### Master Example
 ```python
-from plin.plin import PLIN
+from plin.device import PLIN
 from plin.enums import (PLINFrameChecksumType, PLINFrameDirection,
                         PLINFrameFlag, PLINMode)
 
 # Initializes /dev/plin0 as a LIN master
 master = PLIN(interface="/dev/plin0")
 
 master.start(mode=PLINMode.MASTER, baudrate=19200)
@@ -56,15 +56,15 @@
     result = master.read()
     print(result)
 
 ```
 
 ### Slave Example
 ```python
-from plin.plin import PLIN
+from plin.device import PLIN
 from plin.enums import PLINMode
 
 # Initializes /dev/plin0 as a LIN slave
 slave = PLIN(interface="/dev/plin0")
 
 slave.start(mode=PLINMode.SLAVE, baudrate=19200)
 
@@ -75,19 +75,21 @@
 while True:
     result = slave.read()
     print(result)
 
 ```
 
 ## Unit Tests
-Unit tests are located in the `unit_tests/` directory and require a PEAK LIN device connected to run.
+* Unit tests are located in the `unit_tests/` directory.
+* Tests in `unit_tests/integration/` require a PEAK LIN device connected to run.
+* Can be run with `pytest`.
 
 ## License
 
-    Copyright 2023 Rivian Automotive, Inc.
+    Copyright 2024 Rivian Automotive, Inc.
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `plin-linux-0.0.2/plin/device.py` & `plin_linux-0.0.3/plin/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,18 @@
 PLIORSTUSBTX = IO(ord('u'), 30)
 PLIOCHGBYTEARRAY = IOW(ord('u'), 31, PLINUSBUpdateData)
 PLIOXMTWAKEUP = IO(ord('u'), 33)
 PLIOSETGETRSPMAP = IOWR(ord('u'), 39, PLINUSBResponseRemap)
 PLIOSETLEDSTATE = IOW(ord('u'), 40, PLINUSBLEDState)
 
 
+class PLINException(Exception):
+    pass
+
+
 class PLIN:
     def __init__(self, interface: str):
         self.interface = interface
         self.response_remap = [-1] * PLIN_USB_RSP_REMAP_ID_LEN
         self.fd = None
 
     def _ioctl(self, *args, **kwargs):
@@ -68,45 +72,50 @@
     def start(self, mode: PLINMode, baudrate: int = 19200):
         '''
         Connects to and configures the PLIN device with the specified mode and baudrate.
         '''
         self.mode = mode
         self.baudrate = baudrate
 
-        if not self.fd:
+        if self.fd:
+            raise PLINException("Already connected to PLIN device!")
+        else:
             self.fd = os.open(self.interface, os.O_RDWR)
-
-        self.reset()
-        buffer = PLINUSBInitHardware(self.baudrate, self.mode, 0)
-        self._ioctl(PLIOHWINIT, buffer)
+            self.reset()
+            buffer = PLINUSBInitHardware(self.baudrate, self.mode, 0)
+            self._ioctl(PLIOHWINIT, buffer)
 
     def stop(self):
         '''
         Disconnects from the PLIN device by closing the file descriptor.
         '''
         if self.fd:
             os.close(self.fd)
+            self.fd = None
+        else:
+            raise PLINException("Not connected to PLIN device!")
 
     def set_frame_entry(self,
                         id: int,
                         direction: PLINFrameDirection,
                         checksum_type: PLINFrameChecksumType,
                         flags: PLINFrameFlag = PLINFrameFlag.NONE,
                         data: bytearray = None,
                         len: int = 0):
         '''
         Adds a frame entry for the specified ID.
 
         IMPORTANT NOTE: For a publisher frame, the flag PLINFrameFlag.RSP_ENABLE must be set in order to allow a slave response.
         This flag is set by default if the frame direction is publisher for convenience.
         '''
-        buffer = PLINUSBFrameEntry(
-            id=id, direction=direction, checksum=checksum_type)
         if direction == PLINFrameDirection.PUBLISHER:
-            buffer.flags = flags & PLINFrameFlag.RSP_ENABLE
+            flags |= PLINFrameFlag.RSP_ENABLE
+
+        buffer = PLINUSBFrameEntry(
+            id=id, direction=direction, checksum=checksum_type, flags=flags)
         if data:
             buffer.d = data
         if len > 0:
             buffer.len = len
         self._ioctl(PLIOSETFRMENTRY, buffer)
 
     def set_frame_entry_data(self, id: int, index: int, data: bytearray, len: int):
```

### Comparing `plin-linux-0.0.2/plin/enums.py` & `plin_linux-0.0.3/plin/enums.py`

 * *Files identical despite different names*

### Comparing `plin-linux-0.0.2/plin/structs.py` & `plin_linux-0.0.3/plin/structs.py`

 * *Files identical despite different names*

### Comparing `plin-linux-0.0.2/plin_linux.egg-info/PKG-INFO` & `plin_linux-0.0.3/plin_linux.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: plin-linux
-Version: 0.0.2
+Version: 0.0.3
 Summary: The python-plin package is a Python wrapper for the chardev API provided by the PEAK LIN Linux Beta.
 Author-email: William Zhang <williamzhang@rivian.com>
 Project-URL: Homepage, https://github.com/rivian/python-plin
 Project-URL: Bug Tracker, https://github.com/rivian/python-plin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ioctl_opt
 
 # Python PLIN library
 This library provides a Python interface for interacting with PEAK devices such as the PCAN-USB Pro and PLIN-USB on Linux using the chardev API provided by the PEAK LIN Linux Beta. The PEAK Linux beta driver is required to use this library and is available [here](https://forum.peak-system.com/viewtopic.php?t=5875).
 
 ## Installation
 The `plin-linux` package is available on [PyPI](https://pypi.org/project/plin-linux/) and can be directly installed with `pip install plin-linux`.
 
 ## Examples
 Runnable examples are located in the `examples/` directory.
 
 ### Master Example
 ```python
-from plin.plin import PLIN
+from plin.device import PLIN
 from plin.enums import (PLINFrameChecksumType, PLINFrameDirection,
                         PLINFrameFlag, PLINMode)
 
 # Initializes /dev/plin0 as a LIN master
 master = PLIN(interface="/dev/plin0")
 
 master.start(mode=PLINMode.MASTER, baudrate=19200)
@@ -70,15 +71,15 @@
     result = master.read()
     print(result)
 
 ```
 
 ### Slave Example
 ```python
-from plin.plin import PLIN
+from plin.device import PLIN
 from plin.enums import PLINMode
 
 # Initializes /dev/plin0 as a LIN slave
 slave = PLIN(interface="/dev/plin0")
 
 slave.start(mode=PLINMode.SLAVE, baudrate=19200)
 
@@ -89,19 +90,21 @@
 while True:
     result = slave.read()
     print(result)
 
 ```
 
 ## Unit Tests
-Unit tests are located in the `unit_tests/` directory and require a PEAK LIN device connected to run.
+* Unit tests are located in the `unit_tests/` directory.
+* Tests in `unit_tests/integration/` require a PEAK LIN device connected to run.
+* Can be run with `pytest`.
 
 ## License
 
-    Copyright 2023 Rivian Automotive, Inc.
+    Copyright 2024 Rivian Automotive, Inc.
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `plin-linux-0.0.2/pyproject.toml` & `plin_linux-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plin-linux"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="William Zhang", email="williamzhang@rivian.com" },
 ]
 description = "The python-plin package is a Python wrapper for the chardev API provided by the PEAK LIN Linux Beta."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

