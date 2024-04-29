# Comparing `tmp/space_log-0.1.2-py3-none-any.whl.zip` & `tmp/space_log-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3091 bytes, number of entries: 7
--rw-r--r--  2.0 unx     3641 b- defN 24-Mar-13 18:15 spacelog/SpaceLogClient.py
--rw-r--r--  2.0 unx      860 b- defN 24-Mar-13 18:15 spacelog/SpaceLogHeartbeat.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-13 18:15 spacelog/__init__.py
--rw-r--r--  2.0 unx      300 b- defN 24-Mar-13 18:15 space_log-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-13 18:15 space_log-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-13 18:15 space_log-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      546 b- defN 24-Mar-13 18:15 space_log-0.1.2.dist-info/RECORD
-7 files, 5448 bytes uncompressed, 2115 bytes compressed:  61.2%
+Zip file size: 3117 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     3659 b- defN 24-Apr-29 22:02 spacelog/SpaceLogClient.py
+-rw-r--r--  2.0 unx      860 b- defN 24-Apr-29 22:02 spacelog/SpaceLogHeartbeat.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 22:02 spacelog/__init__.py
+-rw-r--r--  2.0 unx      339 b- defN 24-Apr-29 22:02 space_log-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 22:02 space_log-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-29 22:02 space_log-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      546 b- defN 24-Apr-29 22:02 space_log-0.1.3.dist-info/RECORD
+7 files, 5505 bytes uncompressed, 2141 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: spacelog/SpaceLogHeartbeat.py
 Comment: 
 
 Filename: spacelog/__init__.py
 Comment: 
 
-Filename: space_log-0.1.2.dist-info/METADATA
+Filename: space_log-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: space_log-0.1.2.dist-info/WHEEL
+Filename: space_log-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: space_log-0.1.2.dist-info/top_level.txt
+Filename: space_log-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: space_log-0.1.2.dist-info/RECORD
+Filename: space_log-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spacelog/SpaceLogClient.py

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional
 
 import requests
+from dateutil import parser
 
 from spacelog.SpaceLogHeartbeat import SpaceLogHeartbeat
 
 
 @dataclass
 class SpaceLogPingInfo:
     id: str
@@ -61,15 +62,15 @@
         response_data = response.json()
 
         if "data" in response_data:
             data = response_data["data"]
 
             if len(data) > 0:
                 entry = data[0]
-                last_ping = datetime.fromisoformat(entry["last_ping"])
+                last_ping = parser.parse(entry["last_ping"])
 
                 # Creating an instance of PingInfo with the first entry data
                 ping_info = SpaceLogPingInfo(
                     id=entry["id"],
                     group=entry["group"],
                     application=entry["application"],
                     is_observed=entry["is_observed"],
```

