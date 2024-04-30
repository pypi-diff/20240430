# Comparing `tmp/grpcio-channelz-1.63.0rc1.tar.gz` & `tmp/grpcio_channelz-1.63.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-channelz-1.63.0rc1.tar", last modified: Fri Apr 12 06:40:43 2024, max compression
+gzip compressed data, was "grpcio_channelz-1.63.0rc2.tar", last modified: Wed Apr 17 21:53:49 2024, max compression
```

## Comparing `grpcio-channelz-1.63.0rc1.tar` & `grpcio_channelz-1.63.0rc2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.754614 grpcio-channelz-1.63.0rc1/
--rw-r--r--   0 root         (0) root         (0)    29687 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1100 2024-04-12 06:40:43.754614 grpcio-channelz-1.63.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      281 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.750614 grpcio-channelz-1.63.0rc1/grpc_channelz/
--rw-r--r--   0 root         (0) root         (0)      580 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/grpc_channelz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.750614 grpcio-channelz-1.63.0rc1/grpc_channelz/v1/
--rw-r--r--   0 root         (0) root         (0)      580 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/grpc_channelz/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2690 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/grpc_channelz/v1/_async.py
--rw-r--r--   0 root         (0) root         (0)     4446 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/grpc_channelz/v1/_servicer.py
--rw-r--r--   0 root         (0) root         (0)     2453 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/grpc_channelz/v1/channelz.py
--rw-r--r--   0 root         (0) root         (0)    16482 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/grpc_channelz/v1/channelz_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24136 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/grpc_channelz/v1/channelz_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    15368 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/grpc_channelz/v1/channelz_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      704 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.754614 grpcio-channelz-1.63.0rc1/grpcio_channelz.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1100 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/grpcio_channelz.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/grpcio_channelz.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/grpcio_channelz.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/grpcio_channelz.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-12 06:40:43.000000 grpcio-channelz-1.63.0rc1/grpcio_channelz.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 06:40:43.754614 grpcio-channelz-1.63.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3123 2024-04-12 06:29:27.000000 grpcio-channelz-1.63.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:49.078890 grpcio_channelz-1.63.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    29687 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1108 2024-04-17 21:53:49.078890 grpcio_channelz-1.63.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      281 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:49.070889 grpcio_channelz-1.63.0rc2/grpc_channelz/
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/grpc_channelz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:49.074890 grpcio_channelz-1.63.0rc2/grpc_channelz/v1/
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/grpc_channelz/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/grpc_channelz/v1/_async.py
+-rw-r--r--   0 root         (0) root         (0)     4446 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/grpc_channelz/v1/_servicer.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/grpc_channelz/v1/channelz.py
+-rw-r--r--   0 root         (0) root         (0)    16484 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/grpc_channelz/v1/channelz_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24136 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/grpc_channelz/v1/channelz_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    15368 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/grpc_channelz/v1/channelz_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      704 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:49.078890 grpcio_channelz-1.63.0rc2/grpcio_channelz.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1108 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/grpcio_channelz.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/grpcio_channelz.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/grpcio_channelz.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/grpcio_channelz.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-17 21:53:49.000000 grpcio_channelz-1.63.0rc2/grpcio_channelz.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:53:49.078890 grpcio_channelz-1.63.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-04-17 21:16:56.000000 grpcio_channelz-1.63.0rc2/setup.py
```

### Comparing `grpcio-channelz-1.63.0rc1/LICENSE` & `grpcio_channelz-1.63.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.63.0rc1/PKG-INFO` & `grpcio_channelz-1.63.0rc2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-channelz
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: Channel Level Live Debug Information Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: protobuf>=4.21.6
-Requires-Dist: grpcio>=1.63.0rc1
+Requires-Dist: protobuf<6.0dev,>=5.26.1
+Requires-Dist: grpcio>=1.63.0rc2
 
 gRPC Python Channelz package
 ==============================
 
 Channelz is a live debug tool in gRPC Python.
 
 Supported Python Versions
```

### Comparing `grpcio-channelz-1.63.0rc1/grpc_channelz/__init__.py` & `grpcio_channelz-1.63.0rc2/grpc_channelz/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.63.0rc1/grpc_channelz/v1/__init__.py` & `grpcio_channelz-1.63.0rc2/grpc_channelz/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.63.0rc1/grpc_channelz/v1/_async.py` & `grpcio_channelz-1.63.0rc2/grpc_channelz/v1/_async.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.63.0rc1/grpc_channelz/v1/_servicer.py` & `grpcio_channelz-1.63.0rc2/grpc_channelz/v1/_servicer.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.63.0rc1/grpc_channelz/v1/channelz.py` & `grpcio_channelz-1.63.0rc2/grpc_channelz/v1/channelz.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.63.0rc1/grpc_channelz/v1/channelz_pb2.py` & `grpcio_channelz-1.63.0rc2/grpc_channelz/v1/channelz_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpc_channelz/v1/channelz.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -19,16 +19,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fgrpc_channelz/v1/channelz.proto\x12\x10grpc.channelz.v1\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xfe\x01\n\x07\x43hannel\x12)\n\x03ref\x18\x01 \x01(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.grpc.channelz.v1.ChannelData\x12\x31\n\x0b\x63hannel_ref\x18\x03 \x03(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12\x37\n\x0esubchannel_ref\x18\x04 \x03(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12/\n\nsocket_ref\x18\x05 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\x84\x02\n\nSubchannel\x12,\n\x03ref\x18\x01 \x01(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.grpc.channelz.v1.ChannelData\x12\x31\n\x0b\x63hannel_ref\x18\x03 \x03(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12\x37\n\x0esubchannel_ref\x18\x04 \x03(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12/\n\nsocket_ref\x18\x05 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\xbb\x01\n\x18\x43hannelConnectivityState\x12?\n\x05state\x18\x01 \x01(\x0e\x32\x30.grpc.channelz.v1.ChannelConnectivityState.State\"^\n\x05State\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04IDLE\x10\x01\x12\x0e\n\nCONNECTING\x10\x02\x12\t\n\x05READY\x10\x03\x12\x15\n\x11TRANSIENT_FAILURE\x10\x04\x12\x0c\n\x08SHUTDOWN\x10\x05\"\x8e\x02\n\x0b\x43hannelData\x12\x39\n\x05state\x18\x01 \x01(\x0b\x32*.grpc.channelz.v1.ChannelConnectivityState\x12\x0e\n\x06target\x18\x02 \x01(\t\x12-\n\x05trace\x18\x03 \x01(\x0b\x32\x1e.grpc.channelz.v1.ChannelTrace\x12\x15\n\rcalls_started\x18\x04 \x01(\x03\x12\x17\n\x0f\x63\x61lls_succeeded\x18\x05 \x01(\x03\x12\x14\n\x0c\x63\x61lls_failed\x18\x06 \x01(\x03\x12?\n\x1blast_call_started_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xdb\x02\n\x11\x43hannelTraceEvent\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12>\n\x08severity\x18\x02 \x01(\x0e\x32,.grpc.channelz.v1.ChannelTraceEvent.Severity\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0b\x63hannel_ref\x18\x04 \x01(\x0b\x32\x1c.grpc.channelz.v1.ChannelRefH\x00\x12\x39\n\x0esubchannel_ref\x18\x05 \x01(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRefH\x00\"E\n\x08Severity\x12\x0e\n\nCT_UNKNOWN\x10\x00\x12\x0b\n\x07\x43T_INFO\x10\x01\x12\x0e\n\nCT_WARNING\x10\x02\x12\x0c\n\x08\x43T_ERROR\x10\x03\x42\x0b\n\tchild_ref\"\x96\x01\n\x0c\x43hannelTrace\x12\x19\n\x11num_events_logged\x18\x01 \x01(\x03\x12\x36\n\x12\x63reation_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x65vents\x18\x03 \x03(\x0b\x32#.grpc.channelz.v1.ChannelTraceEvent\"R\n\nChannelRef\x12\x12\n\nchannel_id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\tJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"X\n\rSubchannelRef\x12\x15\n\rsubchannel_id\x18\x07 \x01(\x03\x12\x0c\n\x04name\x18\x08 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"P\n\tSocketRef\x12\x11\n\tsocket_id\x18\x03 \x01(\x03\x12\x0c\n\x04name\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"P\n\tServerRef\x12\x11\n\tserver_id\x18\x05 \x01(\x03\x12\x0c\n\x04name\x18\x06 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"\x92\x01\n\x06Server\x12(\n\x03ref\x18\x01 \x01(\x0b\x32\x1b.grpc.channelz.v1.ServerRef\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.grpc.channelz.v1.ServerData\x12\x32\n\rlisten_socket\x18\x03 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\xc2\x01\n\nServerData\x12-\n\x05trace\x18\x01 \x01(\x0b\x32\x1e.grpc.channelz.v1.ChannelTrace\x12\x15\n\rcalls_started\x18\x02 \x01(\x03\x12\x17\n\x0f\x63\x61lls_succeeded\x18\x03 \x01(\x03\x12\x14\n\x0c\x63\x61lls_failed\x18\x04 \x01(\x03\x12?\n\x1blast_call_started_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xf6\x01\n\x06Socket\x12(\n\x03ref\x18\x01 \x01(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.grpc.channelz.v1.SocketData\x12(\n\x05local\x18\x03 \x01(\x0b\x32\x19.grpc.channelz.v1.Address\x12)\n\x06remote\x18\x04 \x01(\x0b\x32\x19.grpc.channelz.v1.Address\x12,\n\x08security\x18\x05 \x01(\x0b\x32\x1a.grpc.channelz.v1.Security\x12\x13\n\x0bremote_name\x18\x06 \x01(\t\"\xee\x04\n\nSocketData\x12\x17\n\x0fstreams_started\x18\x01 \x01(\x03\x12\x19\n\x11streams_succeeded\x18\x02 \x01(\x03\x12\x16\n\x0estreams_failed\x18\x03 \x01(\x03\x12\x15\n\rmessages_sent\x18\x04 \x01(\x03\x12\x19\n\x11messages_received\x18\x05 \x01(\x03\x12\x18\n\x10keep_alives_sent\x18\x06 \x01(\x03\x12G\n#last_local_stream_created_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12H\n$last_remote_stream_created_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x1blast_message_sent_timestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x1flast_message_received_timestamp\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x19local_flow_control_window\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12?\n\x1aremote_flow_control_window\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12.\n\x06option\x18\r \x03(\x0b\x32\x1e.grpc.channelz.v1.SocketOption\"\xe8\x02\n\x07\x41\x64\x64ress\x12?\n\rtcpip_address\x18\x01 \x01(\x0b\x32&.grpc.channelz.v1.Address.TcpIpAddressH\x00\x12;\n\x0buds_address\x18\x02 \x01(\x0b\x32$.grpc.channelz.v1.Address.UdsAddressH\x00\x12?\n\rother_address\x18\x03 \x01(\x0b\x32&.grpc.channelz.v1.Address.OtherAddressH\x00\x1a\x30\n\x0cTcpIpAddress\x12\x12\n\nip_address\x18\x01 \x01(\x0c\x12\x0c\n\x04port\x18\x02 \x01(\x05\x1a\x1e\n\nUdsAddress\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x1a\x41\n\x0cOtherAddress\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyB\t\n\x07\x61\x64\x64ress\"\xbe\x02\n\x08Security\x12-\n\x03tls\x18\x01 \x01(\x0b\x32\x1e.grpc.channelz.v1.Security.TlsH\x00\x12\x39\n\x05other\x18\x02 \x01(\x0b\x32(.grpc.channelz.v1.Security.OtherSecurityH\x00\x1a{\n\x03Tls\x12\x17\n\rstandard_name\x18\x01 \x01(\tH\x00\x12\x14\n\nother_name\x18\x02 \x01(\tH\x00\x12\x19\n\x11local_certificate\x18\x03 \x01(\x0c\x12\x1a\n\x12remote_certificate\x18\x04 \x01(\x0c\x42\x0e\n\x0c\x63ipher_suite\x1a\x42\n\rOtherSecurity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyB\x07\n\x05model\"U\n\x0cSocketOption\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12(\n\nadditional\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\"B\n\x13SocketOptionTimeout\x12+\n\x08\x64uration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\"Q\n\x12SocketOptionLinger\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xae\x05\n\x13SocketOptionTcpInfo\x12\x12\n\ntcpi_state\x18\x01 \x01(\r\x12\x15\n\rtcpi_ca_state\x18\x02 \x01(\r\x12\x18\n\x10tcpi_retransmits\x18\x03 \x01(\r\x12\x13\n\x0btcpi_probes\x18\x04 \x01(\r\x12\x14\n\x0ctcpi_backoff\x18\x05 \x01(\r\x12\x14\n\x0ctcpi_options\x18\x06 \x01(\r\x12\x17\n\x0ftcpi_snd_wscale\x18\x07 \x01(\r\x12\x17\n\x0ftcpi_rcv_wscale\x18\x08 \x01(\r\x12\x10\n\x08tcpi_rto\x18\t \x01(\r\x12\x10\n\x08tcpi_ato\x18\n \x01(\r\x12\x14\n\x0ctcpi_snd_mss\x18\x0b \x01(\r\x12\x14\n\x0ctcpi_rcv_mss\x18\x0c \x01(\r\x12\x14\n\x0ctcpi_unacked\x18\r \x01(\r\x12\x13\n\x0btcpi_sacked\x18\x0e \x01(\r\x12\x11\n\ttcpi_lost\x18\x0f \x01(\r\x12\x14\n\x0ctcpi_retrans\x18\x10 \x01(\r\x12\x14\n\x0ctcpi_fackets\x18\x11 \x01(\r\x12\x1b\n\x13tcpi_last_data_sent\x18\x12 \x01(\r\x12\x1a\n\x12tcpi_last_ack_sent\x18\x13 \x01(\r\x12\x1b\n\x13tcpi_last_data_recv\x18\x14 \x01(\r\x12\x1a\n\x12tcpi_last_ack_recv\x18\x15 \x01(\r\x12\x11\n\ttcpi_pmtu\x18\x16 \x01(\r\x12\x19\n\x11tcpi_rcv_ssthresh\x18\x17 \x01(\r\x12\x10\n\x08tcpi_rtt\x18\x18 \x01(\r\x12\x13\n\x0btcpi_rttvar\x18\x19 \x01(\r\x12\x19\n\x11tcpi_snd_ssthresh\x18\x1a \x01(\r\x12\x15\n\rtcpi_snd_cwnd\x18\x1b \x01(\r\x12\x13\n\x0btcpi_advmss\x18\x1c \x01(\r\x12\x17\n\x0ftcpi_reordering\x18\x1d \x01(\r\"F\n\x15GetTopChannelsRequest\x12\x18\n\x10start_channel_id\x18\x01 \x01(\x03\x12\x13\n\x0bmax_results\x18\x02 \x01(\x03\"Q\n\x16GetTopChannelsResponse\x12*\n\x07\x63hannel\x18\x01 \x03(\x0b\x32\x19.grpc.channelz.v1.Channel\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"A\n\x11GetServersRequest\x12\x17\n\x0fstart_server_id\x18\x01 \x01(\x03\x12\x13\n\x0bmax_results\x18\x02 \x01(\x03\"K\n\x12GetServersResponse\x12(\n\x06server\x18\x01 \x03(\x0b\x32\x18.grpc.channelz.v1.Server\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"%\n\x10GetServerRequest\x12\x11\n\tserver_id\x18\x01 \x01(\x03\"=\n\x11GetServerResponse\x12(\n\x06server\x18\x01 \x01(\x0b\x32\x18.grpc.channelz.v1.Server\"Z\n\x17GetServerSocketsRequest\x12\x11\n\tserver_id\x18\x01 \x01(\x03\x12\x17\n\x0fstart_socket_id\x18\x02 \x01(\x03\x12\x13\n\x0bmax_results\x18\x03 \x01(\x03\"X\n\x18GetServerSocketsResponse\x12/\n\nsocket_ref\x18\x01 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"\'\n\x11GetChannelRequest\x12\x12\n\nchannel_id\x18\x01 \x01(\x03\"@\n\x12GetChannelResponse\x12*\n\x07\x63hannel\x18\x01 \x01(\x0b\x32\x19.grpc.channelz.v1.Channel\"-\n\x14GetSubchannelRequest\x12\x15\n\rsubchannel_id\x18\x01 \x01(\x03\"I\n\x15GetSubchannelResponse\x12\x30\n\nsubchannel\x18\x01 \x01(\x0b\x32\x1c.grpc.channelz.v1.Subchannel\"6\n\x10GetSocketRequest\x12\x11\n\tsocket_id\x18\x01 \x01(\x03\x12\x0f\n\x07summary\x18\x02 \x01(\x08\"=\n\x11GetSocketResponse\x12(\n\x06socket\x18\x01 \x01(\x0b\x32\x18.grpc.channelz.v1.Socket2\x9a\x05\n\x08\x43hannelz\x12\x63\n\x0eGetTopChannels\x12\'.grpc.channelz.v1.GetTopChannelsRequest\x1a(.grpc.channelz.v1.GetTopChannelsResponse\x12W\n\nGetServers\x12#.grpc.channelz.v1.GetServersRequest\x1a$.grpc.channelz.v1.GetServersResponse\x12T\n\tGetServer\x12\".grpc.channelz.v1.GetServerRequest\x1a#.grpc.channelz.v1.GetServerResponse\x12i\n\x10GetServerSockets\x12).grpc.channelz.v1.GetServerSocketsRequest\x1a*.grpc.channelz.v1.GetServerSocketsResponse\x12W\n\nGetChannel\x12#.grpc.channelz.v1.GetChannelRequest\x1a$.grpc.channelz.v1.GetChannelResponse\x12`\n\rGetSubchannel\x12&.grpc.channelz.v1.GetSubchannelRequest\x1a\'.grpc.channelz.v1.GetSubchannelResponse\x12T\n\tGetSocket\x12\".grpc.channelz.v1.GetSocketRequest\x1a#.grpc.channelz.v1.GetSocketResponseBX\n\x13io.grpc.channelz.v1B\rChannelzProtoP\x01Z0google.golang.org/grpc/channelz/grpc_channelz_v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpc_channelz.v1.channelz_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\023io.grpc.channelz.v1B\rChannelzProtoP\001Z0google.golang.org/grpc/channelz/grpc_channelz_v1'
   _globals['_CHANNEL']._serialized_start=178
   _globals['_CHANNEL']._serialized_end=432
   _globals['_SUBCHANNEL']._serialized_start=435
   _globals['_SUBCHANNEL']._serialized_end=695
   _globals['_CHANNELCONNECTIVITYSTATE']._serialized_start=698
   _globals['_CHANNELCONNECTIVITYSTATE']._serialized_end=885
```

### Comparing `grpcio-channelz-1.63.0rc1/grpc_channelz/v1/channelz_pb2.pyi` & `grpcio_channelz-1.63.0rc2/grpc_channelz/v1/channelz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.63.0rc1/grpc_channelz/v1/channelz_pb2_grpc.py` & `grpcio_channelz-1.63.0rc2/grpc_channelz/v1/channelz_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from grpc_channelz.v1 import channelz_pb2 as grpc__channelz_dot_v1_dot_channelz__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0rc1'
+GRPC_GENERATED_VERSION = '1.63.0rc2'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
```

### Comparing `grpcio-channelz-1.63.0rc1/grpc_version.py` & `grpcio_channelz-1.63.0rc2/grpc_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_channelz/grpc_version.py.template`!!!
 
-VERSION = '1.63.0rc1'
+VERSION = '1.63.0rc2'
```

### Comparing `grpcio-channelz-1.63.0rc1/grpcio_channelz.egg-info/PKG-INFO` & `grpcio_channelz-1.63.0rc2/grpcio_channelz.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-channelz
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: Channel Level Live Debug Information Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: protobuf>=4.21.6
-Requires-Dist: grpcio>=1.63.0rc1
+Requires-Dist: protobuf<6.0dev,>=5.26.1
+Requires-Dist: grpcio>=1.63.0rc2
 
 gRPC Python Channelz package
 ==============================
 
 Channelz is a live debug tool in gRPC Python.
 
 Supported Python Versions
```

### Comparing `grpcio-channelz-1.63.0rc1/grpcio_channelz.egg-info/SOURCES.txt` & `grpcio_channelz-1.63.0rc2/grpcio_channelz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.63.0rc1/setup.py` & `grpcio_channelz-1.63.0rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ]
 
 PACKAGE_DIRECTORIES = {
     "": ".",
 }
 
 INSTALL_REQUIRES = (
-    "protobuf>=4.21.6",
+    "protobuf>=5.26.1,<6.0dev",
     "grpcio>={version}".format(version=grpc_version.VERSION),
 )
 
 try:
     import channelz_commands as _channelz_commands
 
     # we are in the build environment, otherwise the above import fails
```

