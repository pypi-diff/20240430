# Comparing `tmp/pyspartn-0.3.2.tar.gz` & `tmp/pyspartn-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspartn-0.3.2.tar", last modified: Fri Apr 26 07:21:43 2024, max compression
+gzip compressed data, was "pyspartn-0.3.3.tar", last modified: Tue Apr 30 06:32:39 2024, max compression
```

## Comparing `pyspartn-0.3.2.tar` & `pyspartn-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.611648 pyspartn-0.3.2/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-25 22:03:47.000000 pyspartn-0.3.2/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-25 22:03:47.000000 pyspartn-0.3.2/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    22910 2024-04-26 07:21:43.611349 pyspartn-0.3.2/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    19358 2024-04-26 07:17:19.000000 pyspartn-0.3.2/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2446 2024-04-26 07:17:19.000000 pyspartn-0.3.2/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-04-26 07:21:43.611705 pyspartn-0.3.2/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.606999 pyspartn-0.3.2/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.609070 pyspartn-0.3.2/src/pyspartn/
--rw-r--r--   0 steve      (501) staff       (20)      598 2024-04-25 22:03:47.000000 pyspartn-0.3.2/src/pyspartn/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      671 2024-04-25 22:03:47.000000 pyspartn-0.3.2/src/pyspartn/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     2441 2024-04-25 22:03:47.000000 pyspartn-0.3.2/src/pyspartn/socket_stream.py
--rw-r--r--   0 steve      (501) staff       (20)     8202 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartnhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    18848 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartnmessage.py
--rw-r--r--   0 steve      (501) staff       (20)    11757 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartnreader.py
--rw-r--r--   0 steve      (501) staff       (20)     4010 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartntables.py
--rw-r--r--   0 steve      (501) staff       (20)     9339 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartntypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    25523 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartntypes_get.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.610545 pyspartn-0.3.2/src/pyspartn.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    22910 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      576 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      134 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        9 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.610253 pyspartn-0.3.2/tests/
--rw-r--r--   0 steve      (501) staff       (20)     4043 2024-04-25 22:03:47.000000 pyspartn-0.3.2/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     8457 2024-04-26 07:17:19.000000 pyspartn-0.3.2/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)   137741 2024-04-26 07:17:19.000000 pyspartn-0.3.2/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.909488 pyspartn-0.3.3/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-25 22:03:47.000000 pyspartn-0.3.3/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-25 22:03:47.000000 pyspartn-0.3.3/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    24126 2024-04-30 06:32:39.909196 pyspartn-0.3.3/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    20616 2024-04-30 06:27:38.000000 pyspartn-0.3.3/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2446 2024-04-30 06:27:38.000000 pyspartn-0.3.3/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-04-30 06:32:39.909560 pyspartn-0.3.3/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.904943 pyspartn-0.3.3/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.906992 pyspartn-0.3.3/src/pyspartn/
+-rw-r--r--   0 steve      (501) staff       (20)      598 2024-04-25 22:03:47.000000 pyspartn-0.3.3/src/pyspartn/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2024-04-30 06:27:38.000000 pyspartn-0.3.3/src/pyspartn/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      671 2024-04-25 22:03:47.000000 pyspartn-0.3.3/src/pyspartn/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     2441 2024-04-25 22:03:47.000000 pyspartn-0.3.3/src/pyspartn/socket_stream.py
+-rw-r--r--   0 steve      (501) staff       (20)     8957 2024-04-30 06:31:33.000000 pyspartn-0.3.3/src/pyspartn/spartnhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    18499 2024-04-30 06:27:38.000000 pyspartn-0.3.3/src/pyspartn/spartnmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)    11595 2024-04-30 06:27:38.000000 pyspartn-0.3.3/src/pyspartn/spartnreader.py
+-rw-r--r--   0 steve      (501) staff       (20)     4010 2024-04-26 07:17:19.000000 pyspartn-0.3.3/src/pyspartn/spartntables.py
+-rw-r--r--   0 steve      (501) staff       (20)     9339 2024-04-29 14:57:05.000000 pyspartn-0.3.3/src/pyspartn/spartntypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    25860 2024-04-30 06:27:38.000000 pyspartn-0.3.3/src/pyspartn/spartntypes_get.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.908342 pyspartn-0.3.3/src/pyspartn.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    24126 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      576 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      134 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        9 2024-04-30 06:32:39.000000 pyspartn-0.3.3/src/pyspartn.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-30 06:32:39.908067 pyspartn-0.3.3/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     4043 2024-04-25 22:03:47.000000 pyspartn-0.3.3/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)     8670 2024-04-30 06:27:38.000000 pyspartn-0.3.3/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)   139331 2024-04-30 06:27:38.000000 pyspartn-0.3.3/tests/test_stream.py
```

### Comparing `pyspartn-0.3.2/LICENSE` & `pyspartn-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.2/PKG-INFO` & `pyspartn-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.3.2
+Version: 0.3.3
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -108,17 +108,17 @@
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
-The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
+The `SPARTNReader` class is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements optional decrypt and decode algorithms for OCB, HPAC and GAD message types (*BPAC, EAS & PROP message types are rarely used and not currently implemented*). Test coverage is currently limited by available SPARTN test data sources - additional testing contributions are welcome.
+The `SPARTNMessage` class implements optional decrypt and decode algorithms for individual OCB, HPAC, GAD, BPAC and EAS-DYN message types. Test coverage is currently limited by available SPARTN test data sources.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
@@ -179,117 +179,136 @@
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
->>> from serial import Serial
->>> from pyspartn import SPARTNReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>>spr = SPARTNReader(stream)
->>> (raw_data, parsed_data) = spr.read()
->>> print(parsed_data)
-...
+from serial import Serial
+from pyspartn import SPARTNReader
+stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+spr = SPARTNReader(stream)
+(raw_data, parsed_data) = spr.read()
+print(parsed_data)
 ```
 
 Example - File input (using iterator).
 ```python
->>> from pyspartn import SPARTNReader
->>> stream = open('spartndata.log', 'rb')
->>> spr = SPARTNReader(stream)
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+from pyspartn import SPARTNReader
+stream = open('spartndata.log', 'rb')
+spr = SPARTNReader(stream)
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
->>> import socket
->>> from pyspartn import SPARTNReader
->>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
->>> stream.connect(("localhost", 50007))
->>> spr = SPARTNReader(stream)
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+import socket
+from pyspartn import SPARTNReader
+stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
+stream.connect(("localhost", 50007))
+spr = SPARTNReader(stream)
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
 Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
 
 The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
->>> from serial import Serial
->>> from pyspartn import SPARTNReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>>spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
->>> (raw_data, parsed_data) = spr.read()
->>> print(parsed_data)
-...
+from serial import Serial
+from pyspartn import SPARTNReader
+stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 Example - Historical file input with decryption.
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader
->>> stream = open('spartndata.log', 'rb')
->>> spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+from datetime import datetime
+from pyspartn import SPARTNReader
+stream = open('spartndata.log', 'rb')
+spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
 Example - without payload decryption or decoding:
 
 ```python
->>> from pyspartn import SPARTNReader
->>> transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
->>> msg = SPARTNReader.parse(transport, decode=0)
->>> print(msg)
+from pyspartn import SPARTNReader
+
+transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+msg = SPARTNReader.parse(transport, decode=0)
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader
->>> transport = b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80'
->>> msg = SPARTNReader.parse(transport, decode=1, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
-                                                                               
->>> print(msg)
+from datetime import datetime
+from pyspartn import SPARTNReader
+
+transport = b"\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80"
+msg = SPARTNReader.parse(
+    transport,
+    decode=1,
+    key="6b30302427df05b4d98911ebff3a4d95",
+    basedate=datetime(2023, 6, 27, 22, 3, 0),
+)
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader, datadesc
->>> msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
->>> print(msg)
-     <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
->>> msg.identity
+from datetime import datetime
+from pyspartn import SPARTNReader, datadesc
+msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
+print(msg)
+print(msg.identity)
+print(msg.gnssTimeTag)
+print(datadesc("SF005"), msg.SF005)
+print(datadesc("SF061a"), msg.SF061a_10_05)
+```
+```
+<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 'SPARTN-1X-HPAC-GPS'
->>> msg.gnssTimeTag
 451165680
->>> datadesc("SF005"), msg.SF005
 ('Solution issue of update (SIOU)', 152)
->>> datadesc("SF061a"), msg.SF061a_10_05
 ('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
+Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
+
+```python
+vals = []
+for i in range(parsed_data.SF030 + 1):  # attribute or formula representing group size
+    vals.append(getattr(parsed_data, f"SF032_{i+1:02d}"))
+print(vals)
+```
+
 Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
 
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
 
@@ -299,38 +318,42 @@
 
 You can create an `SPARTNMessage` object by calling the constructor with the following keyword arguments:
 1. transport as bytes
 
 Example:
 
 ```python
->>> from pyspartn import SPARTNMessage
->>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
->>> print(msg)
+from pyspartn import SPARTNMessage
+msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `SPARTNMessage` class implements a `serialize()` method to convert a `SPARTNMMessage` object to a bytes array suitable for writing to an output stream.
 
 e.g. to create and send a SPARTN-1X-OCB-GPS message type:
 
 ```python
->>> from serial import Serial
->>> serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
->>> from pyspartn import SPARTNMessage
->>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
->>> print(msg)
+from serial import Serial
+serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
+from pyspartn import SPARTNMessage
+msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+print(msg)
+output = msg.serialize()
+print(output)
+serialOut.write(output)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
->>> output = msg.serialize()
->>> output
 b's\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad'
->>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
@@ -348,15 +371,34 @@
 
 1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
 
    ```
    pyspartn.exceptions.SPARTNTypeError: Error processing attribute 'group' in message type SPARTN-1X-GAD
    ```
 
-   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the provenence date of your SPARTN datasource.
+   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the original creation date of your SPARTN datasource.
+
+1. `SSL: CERTIFICATE_VERIFY_FAILED` error when attempting to connect to SPARTN MQTT service using `gnssmqttclient` on MacOS:
+
+   ```
+   [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1000)
+   ```
+
+   This is because `gnssmqttclient` is unable to locate the RootCA certificate for the MQTT Broker. This can normally be resolved as follows:
+   - Install the latest version of certifi: ```python3 -m pip install --upgrade certifi```
+   - Run the following command from the terminal (_substituting your Python path and version as required_): ```/Applications/Python\ 3.12/Install\ Certificates.command```
+
+1. Unable to install `crytography` library required by `pyspartn` on 32-bit Linux platforms:
+
+   ```
+   Building wheel for cryptography (PEP 517): started
+   Building wheel for cryptography (PEP 517): finished with status 'error'
+   ```
+
+   Refer to [cryptography installation README.md](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
 
 1. Checking for successful decryption. `SPARTNMessage` objects implement a protected attribute `_padding`, which represents the number of redundant bits added to the payload content in order to byte-align the payload with the number of bytes specified in the transport layer payload length attribute `nData`. If the payload has been successfully decrypted and decoded, the value of `_padding` should always be between 0 and 8. Checking `0 <= msg._padding <= 8` provides an informal (_but not necessarily definitive_) check of successful decryption and decoding (see, for example, [spartn_decrypt.py](https://github.com/semuconsulting/pyspartn/blob/main/examples/spartn_decrypt.py)).
 
 ---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at:
```

### Comparing `pyspartn-0.3.2/README.md` & `pyspartn-0.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
-The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
+The `SPARTNReader` class is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements optional decrypt and decode algorithms for OCB, HPAC and GAD message types (*BPAC, EAS & PROP message types are rarely used and not currently implemented*). Test coverage is currently limited by available SPARTN test data sources - additional testing contributions are welcome.
+The `SPARTNMessage` class implements optional decrypt and decode algorithms for individual OCB, HPAC, GAD, BPAC and EAS-DYN message types. Test coverage is currently limited by available SPARTN test data sources.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
@@ -105,117 +105,136 @@
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
->>> from serial import Serial
->>> from pyspartn import SPARTNReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>>spr = SPARTNReader(stream)
->>> (raw_data, parsed_data) = spr.read()
->>> print(parsed_data)
-...
+from serial import Serial
+from pyspartn import SPARTNReader
+stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+spr = SPARTNReader(stream)
+(raw_data, parsed_data) = spr.read()
+print(parsed_data)
 ```
 
 Example - File input (using iterator).
 ```python
->>> from pyspartn import SPARTNReader
->>> stream = open('spartndata.log', 'rb')
->>> spr = SPARTNReader(stream)
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+from pyspartn import SPARTNReader
+stream = open('spartndata.log', 'rb')
+spr = SPARTNReader(stream)
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
->>> import socket
->>> from pyspartn import SPARTNReader
->>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
->>> stream.connect(("localhost", 50007))
->>> spr = SPARTNReader(stream)
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+import socket
+from pyspartn import SPARTNReader
+stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
+stream.connect(("localhost", 50007))
+spr = SPARTNReader(stream)
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
 Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
 
 The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
->>> from serial import Serial
->>> from pyspartn import SPARTNReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>>spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
->>> (raw_data, parsed_data) = spr.read()
->>> print(parsed_data)
-...
+from serial import Serial
+from pyspartn import SPARTNReader
+stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 Example - Historical file input with decryption.
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader
->>> stream = open('spartndata.log', 'rb')
->>> spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+from datetime import datetime
+from pyspartn import SPARTNReader
+stream = open('spartndata.log', 'rb')
+spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
 Example - without payload decryption or decoding:
 
 ```python
->>> from pyspartn import SPARTNReader
->>> transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
->>> msg = SPARTNReader.parse(transport, decode=0)
->>> print(msg)
+from pyspartn import SPARTNReader
+
+transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+msg = SPARTNReader.parse(transport, decode=0)
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader
->>> transport = b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80'
->>> msg = SPARTNReader.parse(transport, decode=1, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
-                                                                               
->>> print(msg)
+from datetime import datetime
+from pyspartn import SPARTNReader
+
+transport = b"\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80"
+msg = SPARTNReader.parse(
+    transport,
+    decode=1,
+    key="6b30302427df05b4d98911ebff3a4d95",
+    basedate=datetime(2023, 6, 27, 22, 3, 0),
+)
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader, datadesc
->>> msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
->>> print(msg)
-     <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
->>> msg.identity
+from datetime import datetime
+from pyspartn import SPARTNReader, datadesc
+msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
+print(msg)
+print(msg.identity)
+print(msg.gnssTimeTag)
+print(datadesc("SF005"), msg.SF005)
+print(datadesc("SF061a"), msg.SF061a_10_05)
+```
+```
+<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 'SPARTN-1X-HPAC-GPS'
->>> msg.gnssTimeTag
 451165680
->>> datadesc("SF005"), msg.SF005
 ('Solution issue of update (SIOU)', 152)
->>> datadesc("SF061a"), msg.SF061a_10_05
 ('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
+Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
+
+```python
+vals = []
+for i in range(parsed_data.SF030 + 1):  # attribute or formula representing group size
+    vals.append(getattr(parsed_data, f"SF032_{i+1:02d}"))
+print(vals)
+```
+
 Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
 
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
 
@@ -225,38 +244,42 @@
 
 You can create an `SPARTNMessage` object by calling the constructor with the following keyword arguments:
 1. transport as bytes
 
 Example:
 
 ```python
->>> from pyspartn import SPARTNMessage
->>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
->>> print(msg)
+from pyspartn import SPARTNMessage
+msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `SPARTNMessage` class implements a `serialize()` method to convert a `SPARTNMMessage` object to a bytes array suitable for writing to an output stream.
 
 e.g. to create and send a SPARTN-1X-OCB-GPS message type:
 
 ```python
->>> from serial import Serial
->>> serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
->>> from pyspartn import SPARTNMessage
->>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
->>> print(msg)
+from serial import Serial
+serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
+from pyspartn import SPARTNMessage
+msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+print(msg)
+output = msg.serialize()
+print(output)
+serialOut.write(output)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
->>> output = msg.serialize()
->>> output
 b's\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad'
->>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
@@ -274,15 +297,34 @@
 
 1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
 
    ```
    pyspartn.exceptions.SPARTNTypeError: Error processing attribute 'group' in message type SPARTN-1X-GAD
    ```
 
-   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the provenence date of your SPARTN datasource.
+   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the original creation date of your SPARTN datasource.
+
+1. `SSL: CERTIFICATE_VERIFY_FAILED` error when attempting to connect to SPARTN MQTT service using `gnssmqttclient` on MacOS:
+
+   ```
+   [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1000)
+   ```
+
+   This is because `gnssmqttclient` is unable to locate the RootCA certificate for the MQTT Broker. This can normally be resolved as follows:
+   - Install the latest version of certifi: ```python3 -m pip install --upgrade certifi```
+   - Run the following command from the terminal (_substituting your Python path and version as required_): ```/Applications/Python\ 3.12/Install\ Certificates.command```
+
+1. Unable to install `crytography` library required by `pyspartn` on 32-bit Linux platforms:
+
+   ```
+   Building wheel for cryptography (PEP 517): started
+   Building wheel for cryptography (PEP 517): finished with status 'error'
+   ```
+
+   Refer to [cryptography installation README.md](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
 
 1. Checking for successful decryption. `SPARTNMessage` objects implement a protected attribute `_padding`, which represents the number of redundant bits added to the payload content in order to byte-align the payload with the number of bytes specified in the transport layer payload length attribute `nData`. If the payload has been successfully decrypted and decoded, the value of `_padding` should always be between 0 and 8. Checking `0 <= msg._padding <= 8` provides an informal (_but not necessarily definitive_) check of successful decryption and decoding (see, for example, [spartn_decrypt.py](https://github.com/semuconsulting/pyspartn/blob/main/examples/spartn_decrypt.py)).
 
 ---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at:
```

### Comparing `pyspartn-0.3.2/pyproject.toml` & `pyspartn-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pyspartn"
 authors = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 maintainers = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 description = "SPARTN protocol parser"
-version = "0.3.2"
+version = "0.3.3"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Environment :: MacOS X",
```

### Comparing `pyspartn-0.3.2/src/pyspartn/__init__.py` & `pyspartn-0.3.3/src/pyspartn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.2/src/pyspartn/exceptions.py` & `pyspartn-0.3.3/src/pyspartn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.2/src/pyspartn/socket_stream.py` & `pyspartn-0.3.3/src/pyspartn/socket_stream.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.2/src/pyspartn/spartnhelpers.py` & `pyspartn-0.3.3/src/pyspartn/spartnhelpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -249,37 +249,53 @@
     """
     Convert 16-bit timetag to 32-bit format.
 
     32-bit timetag represents total seconds since 2010-01-01 00:00:00 (TIMEBASE).
 
     16-bit timetag represents seconds past 'base date' (the datetime the SPARTN
     message was originally sent, to the nearest half-day). It requires knowledge
-    of this base date to convert unambiguously to a 32-bit timetag equlvalent, e.g.
+    of this base date to convert unambiguously to a 32-bit timetag equivalent, e.g.
 
     If base date to nearest half day was "2023-06-27 12:00:00", a timetag16 of
     32580 represents a datetime of:
 
     (2023-06-27 00:00:00 + 12 hours + 32580 seconds) = 2023-06-27 21:03:00
 
     To convert to a 32-bit timetag, calculate number of seconds since TIMEBASE:
 
     (2023-06-27 21:03:00 - 2010-01-01 00:00:00) = 425595780 seconds
 
+    All timetag16 are given in their respective constellation timezone :
+    UTC = GPS + 18s = GAL + 18s = QZSS + 18s = BEI + 4s = GLO - 10800s
+
+    Since all timetags are in GNSS constellation time and basedate is timezone-naive,
+    we calculate three possible 32-bit timetags : basedate, basedate plus half a day,
+    basedate minus half a day, so all constellations and basedate time reference are tried.
+    We then select the unambiguous resolution the closest in time to the original basedate.
+
     :param int timetag16: 16-bit gnssTimeTag
-    :param datetime basedate: original processing datetime to nearest half day
+    :param datetime basedate: original processing datetime accurate to 3 hours
     :return: 32-bit gnssTimeTag
     :rtype: int
     """
 
-    base16 = datetime(basedate.year, basedate.month, basedate.day, 0, 0, 0)
-    secs = timetag16
-    if basedate.hour >= 12:
-        secs += 43200
-    time16 = base16 + timedelta(seconds=secs)
-    return date2timetag(time16)
+    secs_half_day = 43200  # 12 * 60 * 60
+    basedate_seconds = date2timetag(basedate)
+    floor_halfday_timetag = (
+        basedate_seconds - (basedate_seconds % secs_half_day) + timetag16
+    )
+
+    time_options = [
+        floor_halfday_timetag - secs_half_day,
+        floor_halfday_timetag,
+        floor_halfday_timetag + secs_half_day,
+    ]
+
+    closest_time_tag = min(time_options, key=lambda x: abs(x - basedate_seconds))
+    return closest_time_tag
 
 
 def enc2float(value: int, res: float, rngmin: float = 0) -> float:
     """
     Convert encoded floating point value to float.
 
     SPARTN protocol stores floating point numbers in
```

### Comparing `pyspartn-0.3.2/src/pyspartn/spartnmessage.py` & `pyspartn-0.3.3/src/pyspartn/spartnmessage.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,20 +158,14 @@
         if self._validate & VALCRC:
             if not valid_crc(core, self.crc, self.crcType):
                 raise SPARTNMessageError(f"Invalid CRC {self.crc}")
 
         offset = 0  # payload offset in bits
         index = []  # array of (nested) group indices
 
-        # ***********************************************************************************
-        # override of decode flag for message types that cannot yet be decoded
-        if self.msgType not in (0, 1, 2):
-            self._decode = False
-        # ***********************************************************************************
-
         # decrypt payload if encrypted
         if self.eaf and self._decode:
             iv = self._get_iv()
             self._payload = decrypt(payload, self._key, iv)
         else:
             self._payload = payload
 
@@ -444,18 +438,18 @@
             elif key == "SF106":  # BDS code bias mask
                 attl = [8, 15][sflen]
             elif key == "SF107":  # QZSS code bias mask
                 attl = [6, 11][sflen]
         elif key == "SF079":  # Grid node present mask
             attl = (getattr(self, f"SF075{sfx}") + 1) * (
                 getattr(self, f"SF076{sfx}") + 1
-            )  # TODO used by BPAC, not yet tested
-        elif key == "SF088":  # Cryptographic Key,
-            attl = self.SF087
-        elif key == "SF092":  # Computed Authentication Data (CAD),
+            )
+        elif key == "SF088":  # Cryptographic Key length
+            attl = [96, 128, 192, 256, 512][self.SF087]
+        elif key == "SF092":  # Computed Authentication Data (CAD)
             attl = self.SF091
 
         return attl
 
     def _do_unknown(self):
         """
         Handle unknown message type.
```

### Comparing `pyspartn-0.3.2/src/pyspartn/spartnreader.py` & `pyspartn-0.3.3/src/pyspartn/spartnreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,24 +237,21 @@
         raw_data = preamble + core + crcb
         if self._validate & VALCRC:
             if not valid_crc(core, crc, crcType):
                 raise SPARTNParseError(f"Invalid CRC {crc}")
 
         # use 32-bit timetag for this subtype from datastream if available,
         # otherwise use value provided in arguments adjusted for UTC and leap second shift
-        if isinstance(self._basedate, int):  # 32-bit gnssTimetag
-            basedate = self._timetags.get(
-                msgSubtype,
-                self._basedate + TIMETAGSHIFT.get(msgSubtype, 0),
-            )
-        else:  # datetime
-            basedate = self._timetags.get(
-                msgSubtype,
-                self._basedate + timedelta(seconds=TIMETAGSHIFT.get(msgSubtype, 0)),
-            )
+        shift = TIMETAGSHIFT.get(msgSubtype, 0)
+        if isinstance(self._basedate, datetime):
+            shift = timedelta(seconds=shift)
+        basedate = self._timetags.get(
+            msgSubtype,
+            self._basedate + shift,
+        )
         parsed_data = self.parse(
             raw_data,
             validate=self._validate,
             decode=self._decode,
             key=self._key,
             basedate=basedate,
         )
```

### Comparing `pyspartn-0.3.2/src/pyspartn/spartntables.py` & `pyspartn-0.3.3/src/pyspartn/spartntables.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.2/src/pyspartn/spartntypes_core.py` & `pyspartn-0.3.3/src/pyspartn/spartntypes_core.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.2/src/pyspartn/spartntypes_get.py` & `pyspartn-0.3.3/src/pyspartn/spartntypes_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -641,15 +641,22 @@
                         ),
                     },
                 ),
             },
         ),
     },
     # ********************************************************************
-    # EAS-DYN
+    # EAS-DYN TODO not yet tested - no available test data source
     # ********************************************************************
-    "SPARTN-1X-EAS-DYN": {},  # TODO
+    "SPARTN-1X-EAS-DYN": {
+        "SF084": "Customer key ID",  # plain text
+        "SF085": "Dynamic key encryption type",  # plain text
+        "SF086": "Week of applicability",
+        "SF085": "Payload encryption type",
+        "SF087": "Dynamic key length",
+        "SF088": "Dynamic key",  # variable length
+    },
     # ********************************************************************
     # EAS-GRP deprecated
     # ********************************************************************
     "SPARTN-1X-EAS-GRP": {},  # no current plans to implement
 }
```

### Comparing `pyspartn-0.3.2/src/pyspartn.egg-info/PKG-INFO` & `pyspartn-0.3.3/src/pyspartn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.3.2
+Version: 0.3.3
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -108,17 +108,17 @@
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
-The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
+The `SPARTNReader` class is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements optional decrypt and decode algorithms for OCB, HPAC and GAD message types (*BPAC, EAS & PROP message types are rarely used and not currently implemented*). Test coverage is currently limited by available SPARTN test data sources - additional testing contributions are welcome.
+The `SPARTNMessage` class implements optional decrypt and decode algorithms for individual OCB, HPAC, GAD, BPAC and EAS-DYN message types. Test coverage is currently limited by available SPARTN test data sources.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
@@ -179,117 +179,136 @@
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
 Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
->>> from serial import Serial
->>> from pyspartn import SPARTNReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>>spr = SPARTNReader(stream)
->>> (raw_data, parsed_data) = spr.read()
->>> print(parsed_data)
-...
+from serial import Serial
+from pyspartn import SPARTNReader
+stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+spr = SPARTNReader(stream)
+(raw_data, parsed_data) = spr.read()
+print(parsed_data)
 ```
 
 Example - File input (using iterator).
 ```python
->>> from pyspartn import SPARTNReader
->>> stream = open('spartndata.log', 'rb')
->>> spr = SPARTNReader(stream)
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+from pyspartn import SPARTNReader
+stream = open('spartndata.log', 'rb')
+spr = SPARTNReader(stream)
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 Example - Socket input (using iterator):
 ```python
->>> import socket
->>> from pyspartn import SPARTNReader
->>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
->>> stream.connect(("localhost", 50007))
->>> spr = SPARTNReader(stream)
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+import socket
+from pyspartn import SPARTNReader
+stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
+stream.connect(("localhost", 50007))
+spr = SPARTNReader(stream)
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 #### Encrypted Payloads
 
 Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
 
 The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
 
 Example -  Real time serial input with decryption:
 ```python
->>> from serial import Serial
->>> from pyspartn import SPARTNReader
->>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
->>>spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
->>> (raw_data, parsed_data) = spr.read()
->>> print(parsed_data)
-...
+from serial import Serial
+from pyspartn import SPARTNReader
+stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 Example - Historical file input with decryption.
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader
->>> stream = open('spartndata.log', 'rb')
->>> spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
->>> for (raw_data, parsed_data) in spr: print(parsed_data)
-...
+from datetime import datetime
+from pyspartn import SPARTNReader
+stream = open('spartndata.log', 'rb')
+spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
+for (raw_data, parsed_data) in spr:
+   print(parsed_data)
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
 You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
 Example - without payload decryption or decoding:
 
 ```python
->>> from pyspartn import SPARTNReader
->>> transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
->>> msg = SPARTNReader.parse(transport, decode=0)
->>> print(msg)
+from pyspartn import SPARTNReader
+
+transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+msg = SPARTNReader.parse(transport, decode=0)
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader
->>> transport = b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80'
->>> msg = SPARTNReader.parse(transport, decode=1, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
-                                                                               
->>> print(msg)
+from datetime import datetime
+from pyspartn import SPARTNReader
+
+transport = b"\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80"
+msg = SPARTNReader.parse(
+    transport,
+    decode=1,
+    key="6b30302427df05b4d98911ebff3a4d95",
+    basedate=datetime(2023, 6, 27, 22, 3, 0),
+)
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
->>> from datetime import datetime
->>> from pyspartn import SPARTNReader, datadesc
->>> msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
->>> print(msg)
-     <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
->>> msg.identity
+from datetime import datetime
+from pyspartn import SPARTNReader, datadesc
+msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
+print(msg)
+print(msg.identity)
+print(msg.gnssTimeTag)
+print(datadesc("SF005"), msg.SF005)
+print(datadesc("SF061a"), msg.SF061a_10_05)
+```
+```
+<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 'SPARTN-1X-HPAC-GPS'
->>> msg.gnssTimeTag
 451165680
->>> datadesc("SF005"), msg.SF005
 ('Solution issue of update (SIOU)', 152)
->>> datadesc("SF061a"), msg.SF061a_10_05
 ('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
+Attributes in nested repeating groups are suffixed with a 2-digit index for each nested level e.g. `SF032_06`, `SF061a_10_05`. To iterate through nested grouped attributes, you can use a construct similar to the following (_this example iterates through SF032 Area reference latitude values in a SPARTN-1X-GAD message_):
+
+```python
+vals = []
+for i in range(parsed_data.SF030 + 1):  # attribute or formula representing group size
+    vals.append(getattr(parsed_data, f"SF032_{i+1:02d}"))
+print(vals)
+```
+
 Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
 
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
 
@@ -299,38 +318,42 @@
 
 You can create an `SPARTNMessage` object by calling the constructor with the following keyword arguments:
 1. transport as bytes
 
 Example:
 
 ```python
->>> from pyspartn import SPARTNMessage
->>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
->>> print(msg)
+from pyspartn import SPARTNMessage
+msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+print(msg)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `SPARTNMessage` class implements a `serialize()` method to convert a `SPARTNMMessage` object to a bytes array suitable for writing to an output stream.
 
 e.g. to create and send a SPARTN-1X-OCB-GPS message type:
 
 ```python
->>> from serial import Serial
->>> serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
->>> from pyspartn import SPARTNMessage
->>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
->>> print(msg)
+from serial import Serial
+serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
+from pyspartn import SPARTNMessage
+msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
+print(msg)
+output = msg.serialize()
+print(output)
+serialOut.write(output)
+```
+```
 <SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
->>> output = msg.serialize()
->>> output
 b's\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad'
->>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
@@ -348,15 +371,34 @@
 
 1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
 
    ```
    pyspartn.exceptions.SPARTNTypeError: Error processing attribute 'group' in message type SPARTN-1X-GAD
    ```
 
-   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the provenence date of your SPARTN datasource.
+   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the original creation date of your SPARTN datasource.
+
+1. `SSL: CERTIFICATE_VERIFY_FAILED` error when attempting to connect to SPARTN MQTT service using `gnssmqttclient` on MacOS:
+
+   ```
+   [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1000)
+   ```
+
+   This is because `gnssmqttclient` is unable to locate the RootCA certificate for the MQTT Broker. This can normally be resolved as follows:
+   - Install the latest version of certifi: ```python3 -m pip install --upgrade certifi```
+   - Run the following command from the terminal (_substituting your Python path and version as required_): ```/Applications/Python\ 3.12/Install\ Certificates.command```
+
+1. Unable to install `crytography` library required by `pyspartn` on 32-bit Linux platforms:
+
+   ```
+   Building wheel for cryptography (PEP 517): started
+   Building wheel for cryptography (PEP 517): finished with status 'error'
+   ```
+
+   Refer to [cryptography installation README.md](https://github.com/semuconsulting/pyspartn/blob/main/cryptography_installation/README.md).
 
 1. Checking for successful decryption. `SPARTNMessage` objects implement a protected attribute `_padding`, which represents the number of redundant bits added to the payload content in order to byte-align the payload with the number of bytes specified in the transport layer payload length attribute `nData`. If the payload has been successfully decrypted and decoded, the value of `_padding` should always be between 0 and 8. Checking `0 <= msg._padding <= 8` provides an informal (_but not necessarily definitive_) check of successful decryption and decoding (see, for example, [spartn_decrypt.py](https://github.com/semuconsulting/pyspartn/blob/main/examples/spartn_decrypt.py)).
 
 ---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at:
```

### Comparing `pyspartn-0.3.2/src/pyspartn.egg-info/SOURCES.txt` & `pyspartn-0.3.3/src/pyspartn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.2/tests/test_socket.py` & `pyspartn-0.3.3/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.2/tests/test_static.py` & `pyspartn-0.3.3/tests/test_static.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,18 +126,23 @@
         pt = decrypt(ct, key, iv, "CTR")
         self.assertEqual(msg, pt[0:-pad])
         ct, pad = encrypt(msg, key, iv, "CBC")
         pt = decrypt(ct, key, iv, "CBC")
         self.assertEqual(msg, pt[0:-pad])
 
     def testtimetag(self):
-        basedate = datetime(2023, 6, 27, 23, 13, 0)
-        EXPECTED_RES = 425595780
-        res = convert_timetag(32580, basedate)
-        self.assertEqual(res, EXPECTED_RES)
+        basedate_gps = datetime(2023, 6, 27, 23, 13, 0)
+        EXPECTED_RES_GPS = 425595780
+        res = convert_timetag(32580, basedate_gps)
+        self.assertEqual(res, EXPECTED_RES_GPS)
+
+        basedate_glo = datetime(2024, 4, 25, 11, 37, 0)
+        EXPECTED_RES_GLO = 451751822
+        res = convert_timetag(9422, basedate_glo)
+        self.assertEqual(res, EXPECTED_RES_GLO)
 
     def testiv(self):
         IV32 = "031800c03cb4306c2b40000000000001"
         IV16 = "001400c03cb4586c2580000000000001"
 
         msgType = 0  # 1
         nData = 40  # 560
```

### Comparing `pyspartn-0.3.2/tests/test_stream.py` & `pyspartn-0.3.3/tests/test_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,11 +306,59 @@
         res = str(spr.datastream)
         # print(res[-17:])
         self.assertEqual(
             res[-17:],
             "spartn_mqtt.log'>",
         )
 
+    def testrollover16(
+        self,
+    ):  # test decryption of 16-bit timetag dataset containing half day rollover
+        i = 0
+        with open(
+            os.path.join(self.dirname, "spartn_rollover_only16_20240428235040.log"),
+            "rb",
+        ) as stream:
+            spr = SPARTNReader(
+                stream,
+                quitonerror=ERRRAISE,
+                decode=True,
+                key="930d847b779b126863c8b3b2766ae7cc",
+                basedate=datetime(2024, 4, 28, 23, 50, 40),
+            )
+
+            for raw, parsed in spr:
+                i += 1
+                if raw is not None:
+                    # print(f'"{parsed}",')
+                    self.assertTrue(0 <= parsed._padding <= 8)
+
+        self.assertEqual(i, 75)
+
+    def testrollover32(
+        self,
+    ):  # test decryption of 32-bit & 16-bit timetag dataset containing half day rollover
+        i = 0
+        with open(
+            os.path.join(self.dirname, "spartn_rollover_32and16_20240428235040.log"),
+            "rb",
+        ) as stream:
+            spr = SPARTNReader(
+                stream,
+                quitonerror=ERRRAISE,
+                decode=True,
+                key="930d847b779b126863c8b3b2766ae7cc",
+                basedate=datetime(2024, 4, 28, 23, 50, 40),
+            )
+
+            for raw, parsed in spr:
+                i += 1
+                if raw is not None:
+                    # print(f'"{parsed}",')
+                    self.assertTrue(0 <= parsed._padding <= 8)
+
+        self.assertEqual(i, 99)
+
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

