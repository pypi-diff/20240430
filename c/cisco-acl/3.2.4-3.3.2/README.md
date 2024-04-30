# Comparing `tmp/cisco_acl-3.2.4.tar.gz` & `tmp/cisco_acl-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cisco_acl-3.2.4.tar", max compression
+gzip compressed data, was "cisco_acl-3.3.2.tar", max compression
```

## Comparing `cisco_acl-3.2.4.tar` & `cisco_acl-3.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      933 2023-12-04 09:59:54.578612 cisco_acl-3.2.4/cisco_acl/__init__.py
--rw-r--r--   0        0        0    23463 2024-02-01 07:26:36.102829 cisco_acl-3.2.4/cisco_acl/ace.py
--rw-r--r--   0        0        0     4934 2024-02-01 07:26:36.103829 cisco_acl-3.2.4/cisco_acl/ace_base.py
--rw-r--r--   0        0        0    15869 2024-01-31 19:23:54.895813 cisco_acl-3.2.4/cisco_acl/ace_group.py
--rw-r--r--   0        0        0    23734 2024-04-01 13:58:58.121802 cisco_acl-3.2.4/cisco_acl/acl.py
--rw-r--r--   0        0        0    13568 2023-11-22 14:09:38.045056 cisco_acl-3.2.4/cisco_acl/addr_group.py
--rw-r--r--   0        0        0     4799 2023-12-04 10:03:35.657539 cisco_acl-3.2.4/cisco_acl/address.py
--rw-r--r--   0        0        0    11334 2024-02-01 07:26:36.104829 cisco_acl-3.2.4/cisco_acl/address_ag.py
--rw-r--r--   0        0        0    20668 2024-02-01 07:26:36.105830 cisco_acl-3.2.4/cisco_acl/address_base.py
--rw-r--r--   0        0        0     3484 2024-02-01 07:26:36.106829 cisco_acl-3.2.4/cisco_acl/base.py
--rw-r--r--   0        0        0    15308 2023-12-04 10:03:35.659142 cisco_acl-3.2.4/cisco_acl/config_parser.py
--rw-r--r--   0        0        0    14905 2024-02-01 07:26:36.107829 cisco_acl-3.2.4/cisco_acl/functions.py
--rw-r--r--   0        0        0     3703 2023-11-22 14:09:38.048586 cisco_acl-3.2.4/cisco_acl/group.py
--rw-r--r--   0        0        0    16498 2024-02-01 07:26:36.108828 cisco_acl-3.2.4/cisco_acl/helpers.py
--rw-r--r--   0        0        0     3315 2024-02-01 08:51:52.953706 cisco_acl-3.2.4/cisco_acl/option.py
--rw-r--r--   0        0        0     5587 2024-02-01 07:26:36.108828 cisco_acl-3.2.4/cisco_acl/parsers.py
--rw-r--r--   0        0        0    12357 2024-02-01 07:26:36.109829 cisco_acl-3.2.4/cisco_acl/port.py
--rw-r--r--   0        0        0     8446 2023-12-04 10:03:35.655538 cisco_acl-3.2.4/cisco_acl/port_name.py
--rw-r--r--   0        0        0     7454 2024-02-01 07:26:36.110829 cisco_acl-3.2.4/cisco_acl/protocol.py
--rw-r--r--   0        0        0        0 2022-10-06 06:10:23.243000 cisco_acl-3.2.4/cisco_acl/py.typed
--rw-r--r--   0        0        0     3628 2023-11-22 14:09:38.048586 cisco_acl-3.2.4/cisco_acl/remark.py
--rw-r--r--   0        0        0     1111 2023-11-22 14:09:38.048586 cisco_acl-3.2.4/cisco_acl/types_.py
--rw-r--r--   0        0        0    12460 2024-02-01 07:26:36.111827 cisco_acl-3.2.4/cisco_acl/wildcard.py
--rw-r--r--   0        0        0     2553 2024-04-01 13:58:58.123806 cisco_acl-3.2.4/pyproject.toml
--rw-r--r--   0        0        0     8331 2024-04-01 13:58:58.119804 cisco_acl-3.2.4/README.rst
--rw-r--r--   0        0        0     9308 1970-01-01 00:00:00.000000 cisco_acl-3.2.4/PKG-INFO
+-rw-r--r--   0        0        0      933 2023-12-04 09:59:54.578612 cisco_acl-3.3.2/cisco_acl/__init__.py
+-rw-r--r--   0        0        0    24110 2024-04-18 12:01:48.643696 cisco_acl-3.3.2/cisco_acl/ace.py
+-rw-r--r--   0        0        0     5023 2024-04-18 12:01:48.645697 cisco_acl-3.3.2/cisco_acl/ace_base.py
+-rw-r--r--   0        0        0    16343 2024-04-18 14:39:28.977676 cisco_acl-3.3.2/cisco_acl/ace_group.py
+-rw-r--r--   0        0        0    24279 2024-04-18 14:39:28.940298 cisco_acl-3.3.2/cisco_acl/acl.py
+-rw-r--r--   0        0        0    13848 2024-04-18 14:39:28.960547 cisco_acl-3.3.2/cisco_acl/addr_group.py
+-rw-r--r--   0        0        0     4890 2024-04-18 12:01:48.650807 cisco_acl-3.3.2/cisco_acl/address.py
+-rw-r--r--   0        0        0    11425 2024-04-18 12:01:48.652808 cisco_acl-3.3.2/cisco_acl/address_ag.py
+-rw-r--r--   0        0        0    20981 2024-04-18 14:39:28.950380 cisco_acl-3.3.2/cisco_acl/address_base.py
+-rw-r--r--   0        0        0     3816 2024-04-18 12:01:48.654807 cisco_acl-3.3.2/cisco_acl/base.py
+-rw-r--r--   0        0        0    15307 2024-04-18 12:01:48.655807 cisco_acl-3.3.2/cisco_acl/config_parser.py
+-rw-r--r--   0        0        0    19201 2024-04-30 09:35:09.085661 cisco_acl-3.3.2/cisco_acl/functions.py
+-rw-r--r--   0        0        0     3703 2023-11-22 14:09:38.048586 cisco_acl-3.3.2/cisco_acl/group.py
+-rw-r--r--   0        0        0    16940 2024-04-30 09:35:09.086688 cisco_acl-3.3.2/cisco_acl/helpers.py
+-rw-r--r--   0        0        0     3475 2024-04-18 12:01:48.659884 cisco_acl-3.3.2/cisco_acl/option.py
+-rw-r--r--   0        0        0     5651 2024-04-18 12:01:48.661884 cisco_acl-3.3.2/cisco_acl/parsers.py
+-rw-r--r--   0        0        0    12600 2024-04-18 14:39:28.968647 cisco_acl-3.3.2/cisco_acl/port.py
+-rw-r--r--   0        0        0     9019 2024-04-18 12:01:48.663884 cisco_acl-3.3.2/cisco_acl/port_name.py
+-rw-r--r--   0        0        0     7618 2024-04-18 12:01:48.664883 cisco_acl-3.3.2/cisco_acl/protocol.py
+-rw-r--r--   0        0        0        0 2022-10-06 06:10:23.243000 cisco_acl-3.3.2/cisco_acl/py.typed
+-rw-r--r--   0        0        0     3759 2024-04-18 12:01:48.665884 cisco_acl-3.3.2/cisco_acl/remark.py
+-rw-r--r--   0        0        0     1181 2024-04-18 12:01:48.667964 cisco_acl-3.3.2/cisco_acl/types_.py
+-rw-r--r--   0        0        0    12500 2024-04-18 12:01:48.669960 cisco_acl-3.3.2/cisco_acl/wildcard.py
+-rw-r--r--   0        0        0     2637 2024-04-30 09:35:09.087765 cisco_acl-3.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8727 2024-04-18 14:57:21.736071 cisco_acl-3.3.2/README.rst
+-rw-r--r--   0        0        0     9741 1970-01-01 00:00:00.000000 cisco_acl-3.3.2/PKG-INFO
```

### Comparing `cisco_acl-3.2.4/cisco_acl/__init__.py` & `cisco_acl-3.3.2/cisco_acl/__init__.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.4/cisco_acl/ace.py` & `cisco_acl-3.3.2/cisco_acl/ace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ACE - Access Control Entry."""
+
 from __future__ import annotations
 
 from functools import total_ordering
 from typing import List
 
 from cisco_acl import parsers, helpers as h
 from cisco_acl.ace_base import AceBase
@@ -22,14 +23,17 @@
 
         :param line: ACE config, a line that starts with "allow" or "deny".
         :type line: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description.
         :type note: Any
 
         :param max_ncwb: Max count of non-contiguous wildcard bits.
         :type max_ncwb: int
 
@@ -195,35 +199,43 @@
         self._check_parsed_elements(data=ace_d, line=line)
 
         self._sequence = h.init_int(ace_d["sequence"])
         self._action = h.init_ace_action(ace_d["action"])
         self._srcaddr = Address(
             ace_d["srcaddr"],
             platform=self._platform,
+            version=self.version,
             items=self._srcaddr.items,
             max_ncwb=self.max_ncwb,
         )
         self._dstaddr = Address(
             ace_d["dstaddr"],
             platform=self._platform,
+            version=self.version,
             items=self._dstaddr.items,
             max_ncwb=self.max_ncwb,
         )
         protocol_o = Protocol(
             line=ace_d["protocol"],
             platform=self._platform,
+            version=self.version,
             port_nr=self._port_nr,
             protocol_nr=self._protocol_nr,
         )
-        kwargs_port = dict(platform=self._platform, protocol=protocol_o.name, port_nr=self._port_nr)
+        kwargs_port = dict(
+            platform=self._platform,
+            version=self.version,
+            protocol=protocol_o.name,
+            port_nr=self._port_nr,
+        )
         self._srcport = Port(ace_d["srcport"], **kwargs_port)
         self._dstport = Port(ace_d["dstport"], **kwargs_port)
         protocol_o.has_port = bool(self._srcport.line or self._dstport.line)
         self._protocol = protocol_o
-        self._option = Option(ace_d["option"], platform=self._platform)
+        self._option = Option(ace_d["option"], platform=self._platform, version=self.version)
 
     @property
     def option(self) -> Option:
         """ACE option: "syn", "ack", "log", etc.
 
         :return: ACE option.
         :example:
@@ -328,74 +340,82 @@
         :return: ACE data.
 
         :example:
             ace = Ace("10 permit tcp host 10.0.0.1 10.0.0.0 0.0.0.3 eq 80 443 log")
             ace.data() -> {
                 "line": "10 permit tcp host 10.0.0.1 10.0.0.0 0.0.0.3 eq www log",
                 "platform": "ios",
+                "version": "0",
                 "type": "extended",
                 "sequence": 10,
                 "action": "permit",
                 "protocol": {"line": "tcp",
                              "platform": "ios",
+                             "version": "0",
                              "note": "",
                              "protocol_nr": False,
                              "has_port": True,
                              "name": "tcp",
                              "number": 6},
                 "srcaddr": {"line": "host 10.0.0.1",
                             "platform": "ios",
+                            "version": "0",
                             "items": [],
                             "note": "",
                             "addrgroup": "",
                             "ipnet": IPv4Network("10.0.0.1/32"),
                             "prefix": "10.0.0.1/32",
                             "subnet": "10.0.0.1 255.255.255.255",
                             "wildcard": "10.0.0.1 0.0.0.0"},
                 "srcport": {"line": "",
                             "platform": "ios",
+                            "version": "0",
                             "protocol": "",
                             "note": "",
                             "port_nr": False,
                             "items": [],
                             "operator": "",
                             "ports": [],
                             "sport": ""},
                 "dstaddr": {"line": "10.0.0.0 0.0.0.3",
                             "platform": "ios",
+                            "version": "0",
                             "items": [],
                             "note": "",
                             "addrgroup": "",
                             "ipnet": IPv4Network("10.0.0.0/30"),
                             "prefix": "10.0.0.0/30",
                             "subnet": "10.0.0.0 255.255.255.252",
                             "wildcard": "10.0.0.0 0.0.0.3"},
                 "dstport": {"line": "eq www 443",
                             "platform": "ios",
+                            "version": "0",
                             "protocol": "tcp",
                             "note": "",
                             "port_nr": False,
                             "items": [80,
                             443],
                             "operator": "eq",
                             "ports": [80,
                             443],
                             "sport": "80,443"},
                 "option": {"line": "log",
                            "platform": "ios",
+                           "version": "0",
                            "note": "",
                            "flags": [],
                            "logs": ["log"]},
                 "note": "a",
             }
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             type=self._type,
             note=self.note,
             max_ncwb=self.max_ncwb,
             protocol_nr=self._protocol_nr,
             port_nr=self._port_nr,
             # property
             sequence=self._sequence,
```

### Comparing `cisco_acl-3.2.4/cisco_acl/ace_base.py` & `cisco_acl-3.3.2/cisco_acl/ace_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
     def __init__(self, **kwargs):
         """Init AceBase.
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description.
         :type note: Any
 
         :param max_ncwb: Max count of non-contiguous wildcard bits.
         :type max_ncwb: int
 
@@ -62,19 +65,19 @@
         """== equality."""
         if self.__class__ == other.__class__:
             return self.__hash__() == other.__hash__()
         return False
 
     def __repr__(self):
         """__repr__."""
+        name = self.__class__.__name__
         params = self._repr__params()
         params = self._repr__add_param("protocol_nr", params)
         params = self._repr__add_param("port_nr", params)
         kwargs = ", ".join(params)
-        name = self.__class__.__name__
         return f"{name}({kwargs})"
 
     # =========================== property ===========================
 
     @property
     def port_nr(self) -> bool:
         """Well-known TCP/UDP ports as numbers."""
```

### Comparing `cisco_acl-3.2.4/cisco_acl/ace_group.py` & `cisco_acl-3.3.2/cisco_acl/ace_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 These are multiple ACEe items, which must be in a certain order.
 If you are changing Ace items order (sequence numbers) inside Acl,
 the AceGroup behaves like a single item and order of ACE items inside AceGroup is not changed.
 AceGroup is useful for freezing ACEs section, to hold "deny" after certain "permit".
 This class implements most of the Python list methods: append(), extend(), sort(), etc.
 """
+
 from __future__ import annotations
 
 import logging
 from functools import total_ordering
 from ipaddress import NetmaskValueError
 from typing import List, Optional, Union
 
@@ -42,14 +43,17 @@
         This class implements most of the Python list methods: append(), extend(), sort(), etc.
         :param line: String of ACEs, lines that starts with "allow", "deny", "remark".
         :type line: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description.
         :type note: Any
 
         :param max_ncwb: Max count of non-contiguous wildcard bits.
         :type max_ncwb: int
 
@@ -135,17 +139,21 @@
         if not isinstance(items, (list, tuple)):
             raise TypeError(f"{items=} {list} expected")
 
         _items: LUAce = []  # result
         for item in items:
             if isinstance(item, (Ace, Remark)):
                 item._platform = self._platform
+                item.version = self.version
                 item._type = self._type
                 _items.append(item)
             elif isinstance(item, dict):
+                item["platform"] = self._platform
+                item["version"] = str(self.version)
+                item["type"] = self._type
                 ace_o: UAce = self._dict_to_ace(**item)
                 _items.append(ace_o)
             elif isinstance(item, str):
                 line = h.init_line(item)
                 item_ = self._line_to_ace(line)
                 _items.append(item_)
             else:
@@ -235,14 +243,15 @@
 
         :return: The dictionary.
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             type=self._type,
             name=self._name,
             items=[o.data(uuid=uuid) for o in self._items],
             group_by=self._group_by,
             note=self.note,
             protocol_nr=self._protocol_nr,
             port_nr=self._port_nr,
@@ -359,30 +368,32 @@
             data: {line="remark text"}
             return: Remark("text")
         """
         action = kwargs.get("action")
         if action not in ACTIONS:
             raise ValueError(f"invalid action in {kwargs=}, expected {ACTIONS=}")
         kwargs["platform"] = self._platform
+        kwargs["version"] = str(self.version)
         kwargs["type"] = self._type
         kwargs["protocol_nr"] = self._protocol_nr
         kwargs["port_nr"] = self._port_nr
-        if action in ["remark"]:
+        if action == "remark":
             return Remark(**kwargs)
         return Ace(**kwargs)
 
     def _dict_to_aceg(self, **kwargs) -> UAceg:
         """Convert dict data to object: AceGroup, Ace, Remark.
 
         :param kwargs: ACE data.
         :return: ACE object: AceGroup, Ace, Remark.
         """
         items = kwargs.get("items")
         if isinstance(items, (list, tuple)):
             kwargs["platform"] = self._platform
+            kwargs["version"] = str(self.version)
             kwargs["type"] = self._type
             kwargs["protocol_nr"] = self._protocol_nr
             kwargs["port_nr"] = self._port_nr
             return AceGroup(**kwargs)
         return self._dict_to_ace(**kwargs)
 
     def _line_to_ace(self, line: str) -> UAce:
@@ -400,19 +411,20 @@
             return: Remark("text")
 
         :example: not ACE line
             line: "text"
             return: None
         """
         action = parsers.parse_action(line)["action"]
-        if action in ["remark"]:
-            return Remark(line, platform=self._platform, type=self._type)
+        if action == "remark":
+            return Remark(line, platform=self._platform, version=self.version, type=self._type)
         ace_o = Ace(
             line=line,
             platform=self._platform,
+            version=self.version,
             type=self._type,
             protocol_nr=self._protocol_nr,
             port_nr=self._port_nr,
             max_ncwb=self.max_ncwb,
         )
         return ace_o
```

### Comparing `cisco_acl-3.2.4/cisco_acl/acl.py` & `cisco_acl-3.3.2/cisco_acl/acl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ACL - Access Control List.
 
 This class implements most of the Python list methods: append(), extend(), sort(), etc.
 """
+
 from __future__ import annotations
 
 from functools import total_ordering
 from typing import Dict, Generator, List, Union
 
 from cisco_acl import helpers as h
 from cisco_acl.ace import Ace, LAce
@@ -26,14 +27,17 @@
 
         :param line: ACL config, "show running-config" output
         :type line: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         :param input: Interfaces, where Acl is used on input.
         :type input: str
 
         :param output: Interfaces, where Acl is used on output.
         :type output: str
 
         Helpers
@@ -175,18 +179,21 @@
 
         # items
         _items: LUAceg = []
         for item in items:
             # object
             if isinstance(item, (Ace, Remark, AceGroup)):
                 item._platform = self._platform
+                item.version = self.version
                 item._type = self._type
                 _items.append(item)
             # dict
             elif isinstance(item, dict):
+                item["platform"] = self._platform
+                item["version"] = str(self.version)
                 aceg_o: UAceg = self._dict_to_aceg(**item)
                 _items.append(aceg_o)
             # str
             elif isinstance(item, str):
                 line = h.init_line(item)
                 ace_o: UAce = self._line_to_ace(line)
                 _items.append(ace_o)
@@ -270,55 +277,61 @@
             "line": "ip access-list extended NAME\n"
                     "  10 permit tcp host 10.0.0.1 10.0.0.0 0.0.0.3 eq www 443 log",
             "platform": "ios",
             "name": "NAME",
             "items": [
                 {"line": "10 permit tcp host 10.0.0.1 10.0.0.0 0.0.0.3 eq www 443 log",
                  "platform": "ios",
+                 "version": "0",
                  "note": "",
                  "protocol_nr": False,
                  "port_nr": False,
                  "sequence": 10,
                  "action": "permit",
                  "protocol": {"line": "tcp",
                               "platform": "ios",
+                              "version": "0",
                               "note": "",
                               "protocol_nr": False,
                               "has_port": True,
                               "name": "tcp",
                               "number": 6},
                  "srcaddr": {"line": "host 10.0.0.1",
                              "platform": "ios",
+                             "version": "0",
                              "note": "",
                              "items": [],
                              "addrgroup": "",
                              "ipnet": IPv4Network("10.0.0.1/32"),
                              "prefix": "10.0.0.1/32",
                              "subnet": "10.0.0.1 255.255.255.255",
                              "wildcard": "10.0.0.1 0.0.0.0"},
                  "srcport": {"line": "",
                              "platform": "ios",
+                             "version": "0",
                              "note": "",
                              "protocol": "",
                              "port_nr": False,
                              "items": [],
                              "operator": "",
                              "ports": [],
                              "sport": ""},
                  "dstaddr": {"line": "10.0.0.0 0.0.0.3",
                              "platform": "ios",
+                             "version": "0",
                              "note": "",
                              "items": [],
                              "addrgroup": "",
                              "ipnet": IPv4Network("10.0.0.0/30"),
                              "prefix": "10.0.0.0/30",
                              "subnet": "10.0.0.0 255.255.255.252",
                              "wildcard": "10.0.0.0 0.0.0.3"},
                  "dstport": {"line": "eq www 443",
                              "platform": "ios",
+                             "version": "0",
                              "note": "",
                              "protocol": "tcp",
                              "port_nr": False,
                              "items": [80, 443],
                              "operator": "eq",
                              "ports": [80, 443],
                              "sport": "80,443"},
@@ -333,14 +346,15 @@
             "port_nr": False,
         }
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             type=self._type,
             input=self._input.copy(),
             output=self._output.copy(),
             name=self._name,
             items=[o.data(uuid=uuid) for o in self._items],
             group_by=self._group_by,
             note=self.note,
```

### Comparing `cisco_acl-3.2.4/cisco_acl/addr_group.py` & `cisco_acl-3.3.2/cisco_acl/addr_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """AddrGroup.
 
 Group of AddressAg addresses configured in "object-group network" (ios) or
 "object-group ip address" (nxos).
 """
+
 from __future__ import annotations
 
 import logging
 from functools import total_ordering
 from ipaddress import IPv4Network
 from typing import Any, Dict, List, Union
 
@@ -28,14 +29,17 @@
 
         :param line: Address group config line.
         :type line: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description.
         :type note: Any
 
         :param indent: Address lines indentation (default "  ").
         :type indent: str
 
@@ -136,16 +140,19 @@
         if not isinstance(items, (list, tuple)):
             raise TypeError(f"{items=} {list} expected")
 
         _items: LAddressAg = []
         for item in items:
             if isinstance(item, (AddressAg, AddrGroup)):
                 item._platform = self._platform
+                item.version = self.version
                 _items.append(item)
             elif isinstance(item, dict):
+                item["platform"] = self._platform
+                item["version"] = str(self.version)
                 addr_o = AddressAg(**item)
                 _items.append(addr_o)
             elif isinstance(item, str):
                 line = h.init_line(item)
                 # description
                 if item.startswith("description "):  # todo description
                     continue
@@ -251,14 +258,15 @@
 
         :return: Address group data.
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             note=self.note,
             indent=self._indent,
             name=self._name,
             items=[o.data(uuid=uuid) for o in self._items],
         )
         if uuid:
             data["uuid"] = self.uuid
```

### Comparing `cisco_acl-3.2.4/cisco_acl/address.py` & `cisco_acl-3.3.2/cisco_acl/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Address - Source or destination address in ACE."""
+
 from __future__ import annotations
 
 from functools import total_ordering
 from typing import Dict, Iterable, List, Optional, Union
 
 from cisco_acl import address_base
 from cisco_acl.address_base import AddressBase
@@ -26,14 +27,17 @@
             object-group NAME   ios         Network object group
             addrgroup NAME      nxos        Network object group
         :type line: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description
         :type note: Any
 
         :param items: List of Address objects for address group
         :type items: str, List[str], dict, List[dict], Address, List[Address]
```

### Comparing `cisco_acl-3.2.4/cisco_acl/address_ag.py` & `cisco_acl-3.3.2/cisco_acl/address_ag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """AddressAg - Address of AddrGroup.
 
 A "group-object" item of "object-group network " command.
 """
+
 from __future__ import annotations
 
 from functools import total_ordering
 from ipaddress import IPv4Network
 from typing import Iterable, List, Optional, Union
 
 from cisco_acl import address_base, parsers, helpers as h
@@ -34,14 +35,17 @@
             A.B.C.D A.B.C.D     nxos        Network subnet and wildcard bits
             A.B.C.D/LEN         nxos        Network prefix and length
         :type line: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description.
         :type note: Any
 
         :param items: List of AddressAg.
         :type items: str, List[str], dict, List[dict], AddressAg, List[AddressAg]
```

### Comparing `cisco_acl-3.2.4/cisco_acl/address_base.py` & `cisco_acl-3.3.2/cisco_acl/address_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """AddressBase, parent of: Address, AddressAg."""
+
 import re
 from abc import abstractmethod
 from functools import total_ordering
 from ipaddress import IPv4Network
 from typing import Optional
 
 from cisco_acl import helpers as h
@@ -17,14 +18,17 @@
 
     def __init__(self, **kwargs):
         """Init AddressBase.
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description.
         :type note: Any
 
         :param max_ncwb: Max count of non-contiguous wildcard bits.
         :type max_ncwb: int
         """
@@ -113,16 +117,19 @@
         if not isinstance(items, (list, tuple)):
             raise TypeError(f"{items=} {list} expected")
 
         items_ = []
         for item in items:
             if isinstance(item, self.__class__):
                 item.platform = self._platform
+                item.version = self.version
                 items_.append(item)
             elif isinstance(item, dict):
+                item["platform"] = self._platform
+                item["version"] = str(self.version)
                 addr_o = self.__class__(**item)
                 items_.append(addr_o)
             elif isinstance(item, str):
                 line = h.init_line(item)
                 addr_o = self.__class__(line=line, platform=self._platform, max_ncwb=self.max_ncwb)
                 items_.append(addr_o)
             else:
@@ -315,14 +322,15 @@
         :return: Address data.
 
         :example:
             address = Address("10.0.0.0/24", platform="nxos")
             address.data() -> {
                 "line": "10.0.0.0/24",
                 "platform": "nxos",
+                "version": "0",
                 "note": "",
                 "items": [],
                 "max_ncwb": 16,
                 "type": "prefix",
                 "addrgroup": "",
                 "ipnet": IPv4Network("10.0.0.0/24"),
                 "prefix": "10.0.0.0/24",
@@ -330,14 +338,15 @@
                 "wildcard": "10.0.0.0 0.0.0.255",
             }
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             note=self.note,
             items=[o.data(uuid=uuid) for o in self._items],
             max_ncwb=self.max_ncwb,
             # property
             type=self._type,
             addrgroup=self._addrgroup,
             ipnet=self.ipnet,
```

### Comparing `cisco_acl-3.2.4/cisco_acl/base.py` & `cisco_acl-3.3.2/cisco_acl/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-"""Base - Parent of: Address, Port, Protocol, AceBase."""
+"""Base - Parent of: Address, Port, Protocol, Ace, AceBase, Acl, AceGroup."""
 
 from abc import ABC, abstractmethod
 from typing import Any
 from uuid import uuid1
 
+from netports import SwVersion
+
 from cisco_acl import helpers as h
 from cisco_acl.helpers import IOS
 from cisco_acl.types_ import LStr, DAny
 
 
 class Base(ABC):
-    """Base - Parent of: Address, Port, Protocol, AceBase."""
+    """Base - Parent of: Address, Port, Protocol, Ace, AceBase, Acl, AceGroup."""
 
     def __init__(self, **kwargs):
         """Init Base.
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param uuid: Unique identifier.
         :type uuid: str
 
         :param note: Object description.
         :type note: Any
         """
         self._platform: str = h.init_platform(**kwargs)
         self._uuid: str = self._init_uuid(**kwargs)
+        self.version: SwVersion = h.init_version(**kwargs)
         self.note: Any = self._init_note(**kwargs)
 
     def __repr__(self):
         """__repr__."""
         params = self._repr__params()
         kwargs = ", ".join(params)
         name = self.__class__.__name__
@@ -116,9 +122,12 @@
         return params
 
     def _repr__params(self) -> LStr:
         """Return parameters for __repr__."""
         params: LStr = [f"{self.line!r}"]
         if self._platform != IOS:
             params.append(f"platform={self._platform!r}")
+        version = str(self.version)
+        if version != "0":
+            params.append(f"{version=!r}")
         params = self._repr__add_param("note", params)
         return params
```

### Comparing `cisco_acl-3.2.4/cisco_acl/config_parser.py` & `cisco_acl-3.3.2/cisco_acl/config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
         :param config: Cisco config, "show running-config" output.
         :type config: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
-        :param version: Software version (not implemented, planned for compatability).
+        :param version: Software version, default is "0".
+        :type version: str
         """
         self.config: str = str(config)  # raw config
         self.platform: str = h.init_platform(**kwargs)
         self.version: str = str(kwargs.get("version") or "")
 
         self.lines: LStr = []  # config in list format
         self.dic: DLStr = {}  # config in dict format, commands as LStr
```

### Comparing `cisco_acl-3.2.4/cisco_acl/functions.py` & `cisco_acl-3.3.2/cisco_acl/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Functions to create Acl objects From the "show running-config" output."""
+
 import logging
 from ipaddress import IPv4Network
 from typing import Union
 
 import netports
+from vhelpers import vlist
 
 from cisco_acl import helpers as h
 from cisco_acl.ace import Ace, LAce
 from cisco_acl.ace_group import LUAceg
 from cisco_acl.acl import Acl, LAcl
 from cisco_acl.addr_group import AddrGroup, LAddrGroup
 from cisco_acl.address import Address, LAddress
 from cisco_acl.address_ag import AddressAg
 from cisco_acl.config_parser import ConfigParser
 from cisco_acl.port import Port
 from cisco_acl.protocol import Protocol
-from cisco_acl.types_ import LDAny, LInt, LStr, DAny
+from cisco_acl.types_ import LDAny, LInt, LStr, DAny, LLStr
 from cisco_acl.wildcard import init_max_ncwb
 
 UAddress = Union[Address, AddressAg]
 
 
 # noinspection PyIncorrectDocstring,DuplicatedCode
 def acls(config: str, **kwargs) -> LAcl:
@@ -31,15 +33,15 @@
 
     :param config: Cisco config, "show running-config" output.
     :type config: str
 
     :param platform: Platform: "asa", "ios", "nxos". Default "ios".
     :type platform: str
 
-    :param version: Software version (not implemented, planned for compatability).
+    :param version: Software version, default is "0".
     :type version: str
 
     :param names: Parses only ACLs with specified names, skips any other.
     :type names: List[str]
 
     :param max_ncwb: Max count of non-contiguous wildcard bits.
     :type max_ncwb: int
@@ -69,20 +71,21 @@
     version = str(kwargs.get("version") or "")
     group_by = str(kwargs.get("group_by") or "")
     names = kwargs.get("names")
     indent: str = h.init_indent(**kwargs)
     max_ncwb: int = init_max_ncwb(**kwargs)
     protocol_nr = bool(kwargs.get("protocol_nr"))
     port_nr = bool(kwargs.get("port_nr"))
-    acl_kwargs = dict(indent=indent, max_ncwb=max_ncwb, protocol_nr=protocol_nr, port_nr=port_nr)
 
     parser = ConfigParser(config=config, platform=platform, version=version)
     parser.parse_config()
     parsed_acls: LDAny = parser.acls(names=names)
 
+    acl_kwargs = dict(version=version, indent=indent, max_ncwb=max_ncwb,
+                      protocol_nr=protocol_nr, port_nr=port_nr)
     acls_: LAcl = [Acl(**acl_kwargs, **d) for d in parsed_acls]  # type: ignore
     _add_addgr_to_aces(acls_, parser)
     if group_by:
         for acl_o in acls_:
             acl_o.group(group_by=group_by)
     return acls_
 
@@ -93,15 +96,15 @@
 
     :param config: Cisco config, "show running-config" output.
     :type config: str
 
     :param platform: Platform: "asa", "ios", "nxos". Default "ios".
     :type platform: str
 
-    :param version: Software version (not implemented, planned for compatability).
+    :param version: Software version, default is "0".
     :type version: str
 
     :param max_ncwb: Max count of non-contiguous wildcard bits.
     :type max_ncwb: int
 
     :param protocol_nr: Well-known ip protocols as numbers.
         True  - all ip protocols as numbers,
@@ -123,19 +126,19 @@
     """
     platform = h.init_platform(**kwargs)
     version = str(kwargs.get("version") or "")
     group_by = str(kwargs.get("group_by") or "")
     max_ncwb: int = init_max_ncwb(**kwargs)
     protocol_nr = bool(kwargs.get("protocol_nr"))
     port_nr = bool(kwargs.get("port_nr"))
-    acl_kwargs = dict(max_ncwb=max_ncwb, protocol_nr=protocol_nr, port_nr=port_nr)
 
     parser = ConfigParser(config=config, platform=platform, version=version)
     parser.parse_config()
 
+    acl_kwargs = dict(version=version, max_ncwb=max_ncwb, protocol_nr=protocol_nr, port_nr=port_nr)
     acl_o = Acl(platform=platform, **acl_kwargs)  # type: ignore
     for line in parser.lines:
         # noinspection PyProtectedMember
         if ace_o := acl_o._line_to_oace(line):
             acl_o.items.append(ace_o)
 
     if group_by:
@@ -149,15 +152,15 @@
 
     :param config: Cisco config, "show running-config" output.
     :type config: str
 
     :param platform: Platform: "asa", "ios", "nxos". Default "ios".
     :type platform: str
 
-    :param version: Software version (not implemented, planned for compatability).
+    :param version: Software version, default is "0".
     :type version: str
 
     :param max_ncwb: Max count of non-contiguous wildcard bits.
     :type max_ncwb: int
 
     :param indent: Address lines indentation (default "  ").
     :type indent: str
@@ -165,26 +168,35 @@
     :return: List of AddrGroup objects.
     :rtype: List[AddrGroup]
     """
     platform = h.init_platform(**kwargs)
     version = str(kwargs.get("version") or "")
     max_ncwb: int = init_max_ncwb(**kwargs)
     indent: str = h.init_indent(**kwargs)
-    ag_kwargs = dict(max_ncwb=max_ncwb, indent=indent)
 
     parser = ConfigParser(config=config, platform=platform, version=version)
     parser.parse_config()
 
     parsed_addgrs: LDAny = parser.addgrs()
+    ag_kwargs = dict(version=version, max_ncwb=max_ncwb, indent=indent)
     addgrs: LAddrGroup = [AddrGroup(**ag_kwargs, **d) for d in parsed_addgrs]  # type: ignore
     return addgrs
 
 
 # noinspection PyIncorrectDocstring
-def range_ports(**kwargs) -> LStr:
+def range_ports(
+        srcports: str = "",
+        dstports: str = "",
+        line: str = "permit tcp any any",
+        platform: str = "",
+        port_nr: bool = False,
+        port_count: int = 1,
+        port_range: bool = True,
+        **kwargs,
+) -> LStr:
     """Generate ACEs in required range of TCP/UDP source/destination ports.
 
     :param srcports: Range of TCP/UDP source ports.
     :type srcports: str
 
     :param dstports: Range of TCP/UDP destination ports.
     :type dstports: str
@@ -197,31 +209,48 @@
     :type platform: str
 
     :param port_nr: Well-known TCP/UDP ports as numbers.
         True  - all tcp/udp ports as numbers,
         False - well-known tcp/udp ports as names (default).
     :type port_nr: bool
 
+    :param port_count: Count of ports in ACE lines. Default is 1.
+    :type port_count: int
+
+    :param port_range: Transform ACE lines with match-operator "range" to lines with "eq".
+        True - Split match-operator "range" and "eq" to different ACE lines, default is True,
+        False - Transform all ACEs with "range" to ACEs with "eq" (each port in separate ACE).
+    :type port_range: bool
+
     :return: List of newly generated ACE lines.
     :rtype: List[str]
 
     :example:
         range_ports("21-23,80") -> ["permit tcp any eq ftp any",
                                     "permit tcp any eq 22 any",
                                     "permit tcp any eq telnet any",
                                     "permit tcp any eq www any"]
     """
-    srcports = str(kwargs.get("srcports") or "")
-    dstports = str(kwargs.get("dstports") or "")
+    platform = h.init_platform(platform=platform)
+    port_count = int(h.init_number(port_count or 1))
+    _check_operator_eq_range(line, platform, port_range)
 
     aces_: LAce = []  # result
-    _aces = _range__port(range=srcports, sdst="src", **kwargs)
-    aces_.extend(_aces)
-    _aces = _range__port(range=dstports, sdst="dst", **kwargs)
-    aces_.extend(_aces)
+
+    params = {
+        "line": line,
+        "platform": platform,
+        "port_nr": port_nr,
+        "port_count": port_count,
+        "port_range": port_range,
+    }
+    for sdst, ports_range in [("src", srcports), ("dst", dstports)]:
+        _aces = _range__port(ports_range=ports_range, sdst=sdst, **params)
+        aces_.extend(_aces)
+
     return [o.line for o in aces_]
 
 
 # noinspection PyIncorrectDocstring
 def range_protocols(**kwargs) -> LStr:
     """Generate ACEs in required range of IP protocols.
 
@@ -231,14 +260,17 @@
     :param line: ACE pattern, on whose basis new ACEs will be generated.
         (default "permit ip any any")
     :type line: str
 
     :param platform: Platform: "asa", "ios", "nxos". Default "ios".
     :type platform: str
 
+    :param version: Software version, default is "0".
+    :type version: str
+
     :param protocol_nr: Well-known ip protocols as numbers.
         True  - all ip protocols as numbers,
         False - well-known ip protocols as names (default).
     :type protocol_nr: bool
 
     :return: List of newly generated ACE lines.
     :rtype: List[str]
@@ -287,14 +319,56 @@
             return False
     return True
 
 
 # ============================= helper ===============================
 
 
+def _check_addgr(ace_o, addgrs, address_o, parser) -> bool:
+    """Check addresses in address group.
+
+    :return: True - Single Address group present in config.
+        False - Address group not found in config or detected multiple groups,
+        with the same name.
+    """
+    ace = ace_o.line
+    addrgroup = address_o.addrgroup
+    addgrs_ = [o for o in addgrs if o.name == addrgroup]
+    count = len(addgrs_)
+    if not count:
+        line = f"{parser.pattern__object_group()} {addrgroup}"
+        msg = f"{ace=} has no addresses, {line=} not found in config"
+        logging.warning(msg)
+        return False
+    if count != 1:
+        msg = f"{ace=} has no addresses, found multiple {addrgroup=}, expected 1"
+        logging.warning(msg)
+        return False
+    return True
+
+
+def _check_operator_eq_range(line: str, platform: str, port_range: bool) -> None:
+    """Check if the operator is one of allowed: "eq", "neq", "range".
+
+    :param line: ACE line with interested match-operators to check.
+
+    :param platform: Platform
+
+    :return: None. Raise a ValueError if the operator is invalid.
+    """
+    ace_o = Ace(line, platform=platform)
+    operators = [ace_o.srcport.operator, ace_o.dstport.operator]
+    operators = [s for s in operators if s]
+
+    expected = ["eq", "neq", "range"]
+    for operator in operators:
+        if operator not in expected:
+            raise ValueError(f"invalid {operator=}, {expected=}")
+
+
 def _create_acls_w_acegs(parser: ConfigParser, group_by: str) -> LAcl:
     """Create Acls with AceGroups. Groups ACEs to AceGroup by `group_by` in startswith remarks.
 
     :param parser: Semi-parsed config.
 
     :param group_by: Startswith in remark line. ACEs group, starting from the Remark,
         where line startswith `group_by`, will be applied to the same AceGroup,
@@ -348,72 +422,135 @@
     ipnet = address_ag_d["ipnet"]
     if not isinstance(ipnet, IPv4Network):
         raise TypeError(f"invalid {ipnet=} {IPv4Network} expected")
     wildcard = f"{ipnet.network_address} {ipnet.hostmask}"
     address_ag_d["line"] = wildcard
 
 
-def _check_addgr(ace_o, addgrs, address_o, parser) -> bool:
-    """Check addresses in address group.
+def _range__port(
+        ports_range: str,
+        sdst: str,
+        line: str,
+        platform: str,
+        port_nr: bool,
+        port_count: int,
+        port_range: bool,
+) -> LAce:
+    """Generate range of TCP/UDP ports with match-operator.
 
-    :return: True - Single Address group present in config.
-        False - Address group not found in config or detected multiple groups,
-        with the same name.
-    """
-    ace = ace_o.line
-    addrgroup = address_o.addrgroup
-    addgrs_ = [o for o in addgrs if o.name == addrgroup]
-    count = len(addgrs_)
-    if not count:
-        line = f"{parser.pattern__object_group()} {addrgroup}"
-        msg = f"{ace=} has no addresses, {line=} not found in config"
-        logging.warning(msg)
-        return False
-    if count != 1:
-        msg = f"{ace=} has no addresses, found multiple {addrgroup=}, expected 1"
-        logging.warning(msg)
-        return False
-    return True
-
-
-def _range__port(sdst: str, **kwargs) -> LAce:
-    """Generate range of TCP/UDP source/destination ports.
+    :param ports_range: Range of TCP/UDP source/destination ports.
+    :type ports_range: str
 
     :param sdst: "src", "dst".
     :type sdst: str
 
-    :param range: Range of TCP/UDP source/destination ports.
-    :type range: str
+    :param line: ACE line with interested protocol and match operator.
+    :type line: str
+
+    :param platform: Platform: "asa", "ios", "nxos". Default "ios".
+    :type platform: str
 
     :param port_nr: Well-known TCP/UDP ports as numbers.
+        True  - all tcp/udp ports as numbers,
+        False - well-known tcp/udp ports as names (default).
     :type port_nr: bool
 
+    :param port_count: Count of ports in ACE lines. Default is 1.
+    :type port_count: int
+
+    :param port_range: Transform ACE lines with match-operator "range" to lines with "eq".
+        True - Split match-operator "range" and "eq" to different ACE lines, default is True,
+        False - Transform all ACEs with "range" to ACEs with "eq" (each port in separate ACE).
+    :type port_range: bool
+
     :return: List of newly generated Ace objects.
     :rtype: List[Ace]
     """
-    range_ = str(kwargs.get("range") or "")
-    line = str(kwargs.get("line") or "permit tcp any any")
-    platform = h.init_platform(**kwargs)
-    port_nr = bool(kwargs.get("port_nr"))
-
     aces_: LAce = []  # result
-    ports: LInt = netports.itcp(range_)
-    for port in ports:
+
+    ports_for_ace: LLStr = _split_range_for_ace(ports_range, port_count, port_range)
+
+    for ports_ in ports_for_ace:
+        port = " ".join([f"{i}" for i in ports_])
+
         ace_o = Ace(line, platform=platform, port_nr=port_nr)
         ace_o.protocol.has_port = True
 
-        # check operator=="range"
-        port_o: Port = getattr(ace_o, f"{sdst}port")
-        operator = port_o.operator or "eq"
-        expected = ["eq", "gt", "lt", "neq"]
-        if operator not in expected:
-            raise ValueError(f"invalid {operator=}, {expected=}")
+        # operator
+        attr = f"{sdst}port"
+        port_o: Port = getattr(ace_o, attr)
+        operator = port_o.operator
+        if not operator:
+            operator = "eq"
+            if port.find("-") > -1:
+                operator = "range"
+                port = port.replace("-", " ")
 
         port_o = Port(
             line=f"{operator} {port}",
             platform=ace_o.platform,
             protocol=ace_o.protocol.name,
             port_nr=ace_o.port_nr,
         )
-        setattr(ace_o, f"_{sdst}port", port_o)
+        attr = f"_{sdst}port"
+        setattr(ace_o, attr, port_o)
         aces_.append(ace_o)
+
     return aces_
+
+
+def _split_range_for_ace(ports_range: str, port_count: int, port_range: bool) -> LLStr:
+    """Split port_range to strings where each item is for separate ACE.
+
+    :param ports_range: Range of TCP/UDP source/destination ports.
+    :type ports_range: str
+
+    :param port_count: Count of ports in ACE lines. Default is 1.
+    :type port_count: int
+
+    :param port_range: Transform ACE lines with match-operator "range" to lines with "eq".
+        True - Split match-operator "range" and "eq" to different ACE lines, default is True,
+        False - Transform all ACEs with "range" to ACEs with "eq" (each port in separate ACE).
+    :type port_range: bool
+
+    :return: List of newly generated ports.
+    :rtype: List[Ace]
+    """
+    items: LLStr = []
+    ports_i: LStr = []
+    ports = ports_range.split(",")
+    for port in ports:
+        # range
+        if not port.isdigit():
+            if ports_i:
+                items.append(ports_i)
+                ports_i = []
+            if not port:
+                continue
+            if port_range:
+                items.append([port])
+                continue
+            ports_ = [str(i) for i in netports.itcp(port)]
+            items.append(ports_)
+            continue
+
+        # port_count unlimited
+        if not port_count:
+            ports_i.append(port)
+            continue
+
+        # ports
+        if len(ports_i) >= port_count:
+            items.append(ports_i)
+            ports_i = []
+        ports_i.append(port)
+    else:
+        if ports_i:
+            items.append(ports_i)
+
+    if not port_range:
+        items_ = vlist.flatten(items)
+        items = [items_]
+        if port_count:
+            items = vlist.to_multi(items_, count=port_count)
+
+    return items
```

### Comparing `cisco_acl-3.2.4/cisco_acl/group.py` & `cisco_acl-3.3.2/cisco_acl/group.py`

 * *Files identical despite different names*

### Comparing `cisco_acl-3.2.4/cisco_acl/helpers.py` & `cisco_acl-3.3.2/cisco_acl/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import re
 from functools import wraps
 from ipaddress import IPv4Network
 from string import ascii_letters, digits, punctuation
 from time import time
 from typing import Any, List, NamedTuple
 
+from netports import SwVersion
+
 from cisco_acl.types_ import LStr, StrInt, LInt, OInt, SInt, T2Str, T3Str, DInt, SStr, LIpNet
 
 IOS = "ios"
 MAX_LINE_LENGTH = 100
 SEQUENCE_MAX = 4294967295
 PLATFORMS = ("asa", "ios", "nxos")
 ACTIONS = ("remark", "permit", "deny")
@@ -158,26 +160,29 @@
     name = name.strip()
     check_line_length(name)
     return name
 
 
 def init_number(number: StrInt) -> str:
     """Init number, convert int to string."""
-    while True:
-        if isinstance(number, int):
-            if number < 0:
-                raise ValueError(f"{number=} positive expected")
-            break
-        if isinstance(number, str):
-            if number.isdigit():
-                number = int(number)
-                break
-            raise ValueError(f"{number=} digit expected")
-        raise TypeError(f"{number=} {str} {int} expected")
-    return str(number)
+    return str(init_number_int(number))
+
+
+def init_number_int(number: StrInt) -> int:
+    """Init positive integer."""
+    if isinstance(number, int):
+        if number >= 0:
+            return number
+        raise ValueError(f"{number=} positive expected")
+
+    if isinstance(number, str):
+        if number.isdigit():
+            return int(number)
+        raise ValueError(f"{number=} digit expected")
+    raise TypeError(f"{number=} {str} {int} expected")
 
 
 # noinspection PyIncorrectDocstring
 def init_platform(**kwargs) -> str:
     """Init device platform.
 
     :param platform: Not checked platform: "cisco_ios", "cisco_nxos", "cnx", "ios", "nxos".
@@ -249,14 +254,28 @@
             _type = "extended"
     if platform == "nxos" and _type == "standard":
         expected = "extended"
         raise ValueError(f"invalid type={_type!r}, {expected=}")
     return _type
 
 
+# noinspection PyIncorrectDocstring
+def init_version(**kwargs) -> SwVersion:
+    """Init version.
+
+    Convert software version string to SwVersion object.
+    :param version: software version string.
+    :return: SwVersion object.
+    """
+    version = str(kwargs.get("version") or "")
+    if not version:
+        version = "0"
+    return SwVersion(version)
+
+
 def int_to_str(line: StrInt) -> str:
     """Init line, int or string convert to string, replace spaces."""
     if isinstance(line, int):
         if line < 0:
             raise ValueError(f"{line=} positive expected")
         line = str(line)
     if not isinstance(line, str):
```

### Comparing `cisco_acl-3.2.4/cisco_acl/option.py` & `cisco_acl-3.3.2/cisco_acl/option.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ACE. Option."""
+
 from __future__ import annotations
 
 import string
 from functools import total_ordering
 
 from cisco_acl import helpers as h
 from cisco_acl.base import Base
@@ -18,14 +19,17 @@
     def __init__(self, line: str = "", **kwargs):
         """Init Option.
 
         :param line: Option line.
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description.
         :type note: Any
 
         :example:
             option = Option("ack dscp ef log")
             option.line -> "ack log"
@@ -96,23 +100,25 @@
         :return: Option data.
 
         :example:
         option = Option("ack log")
         option.data() -> {
             "line": "ack log",
             "platform": "ios",
+            "version": "0",
             "note": "",
             "flags": ["ack"],
             "logs": ["log"],
         }
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             note=self.note,
             # property
             flags=self._flags,
             logs=self._logs,
         )
         if uuid:
             data["uuid"] = self.uuid
```

### Comparing `cisco_acl-3.2.4/cisco_acl/parsers.py` & `cisco_acl-3.3.2/cisco_acl/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,23 @@
         "dstaddr": "10.0.0.0 255.0.0.0",
         "dstport": "eq web",
         "option": "log",
      }
     """
     space = r"(?: )"
     text = r"\S+"
-    addr = "|".join([
-        "any",  # "any"
-        f"host {h.OCTETS}",  # "host A.B.C.D"
-        f"(?:object-group|addrgroup) {text}",  # ios: "object-group NAME", nxos: "addrgroup NAME"
-        h.OCTETS + r"/\d+",  # "A.B.C.D/LEN"
-        f"{h.OCTETS} {h.OCTETS}",  # "A.B.C.D A.B.C.D"
-    ])
+    addr = "|".join(
+        [
+            "any",  # "any"
+            f"host {h.OCTETS}",  # "host A.B.C.D"
+            f"(?:object-group|addrgroup) {text}",  # ios: "object-group", nxos: "addrgroup"
+            h.OCTETS + r"/\d+",  # "A.B.C.D/LEN"
+            f"{h.OCTETS} {h.OCTETS}",  # "A.B.C.D A.B.C.D"
+        ]
+    )
 
     re_sequence = r"(\d+)?"
     re_action = f"{space}?(permit|deny)"
     re_proto = f"({space}{text})?"
     re_srcaddr = f"{space}({addr})"
     re_srcport = "( .+)?"
     re_dstaddr = f"{space}({addr})"
@@ -77,22 +79,24 @@
                  "srcport": "",
                  "dstaddr": "any",
                  "dstport": "",
                  "option": "log"}
     """
     space = r"(?: )"
     text = r"\S+"
-    addr = "|".join([
-        "any",  # "any"
-        f"host {h.OCTETS}",  # "host A.B.C.D"
-        f"(?:object-group|addrgroup) {text}",  # ios: "object-group NAME", nxos: "addrgroup NAME"
-        h.OCTETS + r"/\d+",  # "A.B.C.D/LEN"
-        f"{h.OCTETS} {h.OCTETS}",  # "A.B.C.D A.B.C.D"
-        h.OCTETS,  # host
-    ])
+    addr = "|".join(
+        [
+            "any",  # "any"
+            f"host {h.OCTETS}",  # "host A.B.C.D"
+            f"(?:object-group|addrgroup) {text}",  # ios: "object-group", nxos: "addrgroup"
+            h.OCTETS + r"/\d+",  # "A.B.C.D/LEN"
+            f"{h.OCTETS} {h.OCTETS}",  # "A.B.C.D A.B.C.D"
+            h.OCTETS,  # host
+        ]
+    )
 
     re_sequence = r"(\d+)?"
     re_action = f"{space}?(permit|deny)"
     re_srcaddr = f"{space}({addr})"
     re_log = "( .+)?"
 
     regex = f"^{re_sequence}{re_action}{re_srcaddr}{re_log}"
```

### Comparing `cisco_acl-3.2.4/cisco_acl/port.py` & `cisco_acl-3.3.2/cisco_acl/port.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Port - ACE TCP/UDP source or destination port object."""
+
 from __future__ import annotations
 
 from functools import total_ordering
 from typing import List
 
 from cisco_acl import helpers as h
 from cisco_acl.base import Base
@@ -16,17 +17,20 @@
     """Port - ACE TCP/UDP source or destination port object."""
 
     def __init__(self, line: str = "", **kwargs):
         """Init Port.
 
         :param line: TCP/UDP ports line.
 
-        :param platform: Platform: "asa", "ios", "nxos". Default "ios"..
+        :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         :param protocol: ACL protocol: "tcp", "udp", "".
         :type protocol: str
 
         Helpers
         :param note: Object description.
         :type note: Any
 
@@ -118,15 +122,15 @@
     def line(self) -> str:
         """ACE source or destination TCP/UDP ports."""
         if not (self._operator and self._items and self._protocol in ["tcp", "udp"]):
             return ""
         if self._port_nr:
             items_s = " ".join([str(i) for i in self._items])
             return f"{self._operator} {items_s}"
-        port_name = PortName(protocol=self._protocol, platform=self._platform)
+        port_name = PortName(protocol=self._protocol, platform=self._platform, version=self.version)
         data = port_name.ports()
         items_s = " ".join([str(data.get(i) or i) for i in self._items])
         return f"{self._operator} {items_s}"
 
     @line.setter
     def line(self, line: str) -> None:
         line = h.init_line(line)
@@ -226,27 +230,29 @@
         :param uuid: Return self.uuid in data.
         :return: Port data.
         :example:
             address = Address("10.0.0.0/24", platform="nxos")
             address.data() -> {
                 "line": "10.0.0.0/24",
                 "platform": "nxos",
+                "version": "0",
                 "items": [],
                 "note": "",
                 "addrgroup": "",
                 "ipnet": IPv4Network("10.0.0.0/24"),
                 "prefix": "10.0.0.0/24",
                 "subnet": "10.0.0.0 255.255.255.0",
                 "wildcard": "10.0.0.0 0.0.0.255",
             }
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             note=self.note,
             protocol=self._protocol,
             port_nr=self._port_nr,
             # property
             items=self._items,
             operator=self._operator,
             ports=self._ports,
@@ -282,32 +288,34 @@
 
         # convert to int
         ports: LInt = []  # result
         for item in items:
             if item.isdigit():
                 ports.append(int(item))
                 continue
-            port_name = PortName(protocol=self._protocol, platform=self._platform)
+            port_name = PortName(
+                protocol=self._protocol, platform=self._platform, version=self.version
+            )
             data = port_name.names()
             if port_nr := data.get(item):
                 ports.append(port_nr)
                 continue
             msg = f"invalid {item=}"
             if expected := sorted(data):
                 msg = f"{msg}, {expected=}"
             raise ValueError(msg)
 
         # validation
-        platform = self._platform
         operator = self._operator
         if operator in ["lt", "gt"] and len(ports) != 1:
             raise ValueError(f"invalid {operator=} with {ports=}")
         if operator == "range" and len(ports) != 2:
             raise ValueError(f"invalid {operator=} with {ports=} expected 2 ports")
         if self._operator in ["eq", "neq"]:
+            platform = self._platform
             if platform in ["asa", "nxos"] and len(ports) != 1:
                 raise ValueError(f"invalid count of {ports=}, for {platform=} expected 1 port")
 
         return sorted(ports)
 
     def _items_to_ports(self, items: LInt) -> LInt:
         """Transform line items to ports.
```

### Comparing `cisco_acl-3.2.4/cisco_acl/port_name.py` & `cisco_acl-3.3.2/cisco_acl/port_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """TCP/UDP ports and names mapping for Cisco ACL."""
 
+from netports import SwVersion
+
 from cisco_acl import helpers as h
-from cisco_acl.types_ import DInt, DiStr, LStr
+from cisco_acl.types_ import DInt, DiStr, LStr, UVersion
 
 # cisco Nexus 3172T, NXOS: version 9.3(8)
 # cisco ISR4331/K9, Cisco IOS XE Software, Version 16.09.06
 TCP_NAME_PORT__BASE = {
     "echo": 7,
     "discard": 9,
     "daytime": 13,
@@ -96,22 +98,28 @@
 
 # cisco Nexus 3172T, NXOS: version 9.3(8)
 TCP_NAME_PORT__NXOS = {
     "drip": 3949,
 }
 TCP_NAME_PORT__NXOS = {**TCP_NAME_PORT__BASE, **TCP_NAME_PORT__NXOS}
 
+# cisco C6816-X-LE, Cisco IOS Software, Version 15.2(02)SY
+TCP_NAME_PORT__IOS_15 = {
+    "syslog": 514,  # alias of cmd
+}
+TCP_NAME_PORT__IOS_15 = {**TCP_NAME_PORT__BASE, **TCP_NAME_PORT__IOS_15}
+
 # cisco ISR4331/K9, Cisco IOS XE Software, Version 16.09.06
-TCP_NAME_PORT__IOS = {
+TCP_NAME_PORT__IOS_16 = {
     "msrpc": 135,
     "syslog": 514,  # alias of cmd
     "onep-plain": 15001,
     "onep-tls": 15002,
 }
-TCP_NAME_PORT__IOS = {**TCP_NAME_PORT__BASE, **TCP_NAME_PORT__IOS}
+TCP_NAME_PORT__IOS_16 = {**TCP_NAME_PORT__BASE, **TCP_NAME_PORT__IOS_16}
 
 # cisco Nexus 3172T, NXOS: version 9.3(8)
 # cisco ISR4331/K9, Cisco IOS XE Software, Version 16.09.06
 UDP_NAME_PORT__BASE = {
     "echo": 7,
     "discard": 9,
     "time": 37,
@@ -177,135 +185,159 @@
     "sip": 5060,
     "secureid-udp": 5510,
     "pcanywhere-status": 5632,
 }
 # cisco Nexus 3172T, NXOS: version 9.3(8)
 UDP_NAME_PORT__NXOS = UDP_NAME_PORT__BASE
 
+# cisco C6816-X-LE, Cisco IOS Software, Version 15.2(02)SY
+UDP_NAME_PORT__IOS_15 = {**UDP_NAME_PORT__BASE}
+
 # cisco ISR4331/K9, Cisco IOS XE Software, Version 16.09.06
-UDP_NAME_PORT__IOS = {
+UDP_NAME_PORT__IOS_16 = {
     "ripv6": 521,
 }
-UDP_NAME_PORT__IOS = {**UDP_NAME_PORT__BASE, **UDP_NAME_PORT__IOS}
+UDP_NAME_PORT__IOS_16 = {**UDP_NAME_PORT__BASE, **UDP_NAME_PORT__IOS_16}
 
 
 class PortName:
     """TCP/UDP ports and names mapping for Cisco ACL."""
 
-    def __init__(self, protocol: str = "tcp", **kwargs):
+    def __init__(
+        self,
+        protocol: str = "tcp",
+        platform: str = "",
+        version: UVersion = "",
+    ):
         """Init PortName.
 
         :param protocol: Protocol: "tcp", "udp".
+        :type protocol: str
+
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
-        :param version: Software version (not implemented, planned for compatability).
+        :type platform: str
+
+        :param version: Software version.
+        :type version: str
         """
-        self.protocol = self._init_protocol(protocol)
-        self.platform = h.init_platform(**kwargs)
-        self.version = str(kwargs.get("version") or "").lower()
+        self.protocol: str = _init_protocol(protocol)
+        self.platform: str = h.init_platform(platform=platform)
+        self.version: SwVersion = h.init_version(version=version)
 
     def __repr__(self):
         """__repr__."""
         name = self.__class__.__name__
         params = [
             f"protocol={self.protocol!r}",
             f"platform={self.platform!r}",
-            f"version={self.version!r}",
         ]
+        if str(self.version) != "0":
+            params.append(f"version={str(self.version)!r}")
         params_s = ", ".join(params)
         return f"{name}({params_s})"
 
-    @staticmethod
-    def _init_protocol(protocol: str) -> str:
-        """Init protocol.
-
-        Converts TCP/UDP numbers to names.
-        :param protocol: Protocol: "tcp", "udp".
-        :return: Protocol: "tcp", "udp".
-        """
-        protocol = str(protocol).lower()
-        expected = ["tcp", "udp"]
-        if protocol in expected:
-            return protocol
-        if str(protocol) == "6":
-            return "tcp"
-        if str(protocol) == "17":
-            return "udp"
-        raise ValueError(f"invalid {protocol=}, {expected=}")
-
+    # noinspection DuplicatedCode
     def names(self) -> DInt:
         """Return TCP/UDP protocol names and ports based on the platform and software version.
 
         :return: Dictionary with protocol names and ports (platform-specific).
         :example: {"echo": 7, "discard": 9, ...}
         """
-        if self.protocol in ["tcp", "6"]:
+        names_d: DInt = {}
+        if self._is_tcp():
             if self.platform == "asa":
-                return TCP_NAME_PORT__ASA.copy()
-            if self.platform == "ios":
-                return TCP_NAME_PORT__IOS.copy()
-            if self.platform == "nxos":
-                return TCP_NAME_PORT__NXOS.copy()
-            return {}
-        if self.protocol in ["udp", "17"]:
+                names_d = TCP_NAME_PORT__ASA.copy()
+            elif self.platform == "ios":
+                if self.version.major == 15:
+                    names_d = TCP_NAME_PORT__IOS_15.copy()
+                else:
+                    names_d = TCP_NAME_PORT__IOS_16.copy()
+            elif self.platform == "nxos":
+                names_d = TCP_NAME_PORT__NXOS.copy()
+
+        elif self._is_udp():
             if self.platform == "asa":
-                return UDP_NAME_PORT__ASA.copy()
-            if self.platform == "ios":
-                return UDP_NAME_PORT__IOS.copy()
-            if self.platform == "nxos":
-                return UDP_NAME_PORT__NXOS.copy()
-            return {}
-        return {}
+                names_d = UDP_NAME_PORT__ASA.copy()
+            elif self.platform == "ios":
+                if self.version.major == 15:
+                    names_d = UDP_NAME_PORT__IOS_15.copy()
+                else:
+                    names_d = UDP_NAME_PORT__IOS_16.copy()
+            elif self.platform == "nxos":
+                names_d = UDP_NAME_PORT__NXOS.copy()
+
+        return names_d
 
     # noinspection DuplicatedCode
     def ports(self) -> DiStr:
         """Return TCP/UDP protocol ports and names based on the platform and software version.
 
         :return: Dictionary with protocol ports and ports (platform-specific).
         :example: {7: "echo", 9: "discard", ...}
         """
-        if self.protocol in ["tcp", "6"]:
-            if self.platform == "asa":
-                return self._swap(TCP_NAME_PORT__ASA.copy())
-            if self.platform == "ios":
-                return self._swap(TCP_NAME_PORT__IOS.copy())
-            if self.platform == "nxos":
-                return self._swap(TCP_NAME_PORT__NXOS.copy())
-            return {}
+        names_d: DInt = self.names()
+        ports_d: DiStr = _swap(names_d)
+        return ports_d
 
-        if self.protocol in ["udp", "17"]:
-            if self.platform == "asa":
-                return self._swap(UDP_NAME_PORT__ASA.copy())
-            if self.platform == "ios":
-                return self._swap(UDP_NAME_PORT__IOS.copy())
-            if self.platform == "nxos":
-                return self._swap(UDP_NAME_PORT__NXOS.copy())
-            return {}
-        return {}
-
-    @staticmethod
-    def _swap(name_port: DInt) -> DiStr:
-        """Swap names and ports in dict."""
-        data: DiStr = {}
-        for name, port in name_port.items():
-            if port not in data:
-                data[port] = name
-        return data
+    def _is_tcp(self) -> bool:
+        """Check if the protocol is TCP.
+
+        :return: True if the protocol is TCP, False otherwise.
+        """
+        return bool(self.protocol in ["tcp", "6"])
+
+    def _is_udp(self) -> bool:
+        """Check if the protocol is UDP.
+
+        :return: True if the protocol is UDP, False otherwise.
+        """
+        return bool(self.protocol in ["udp", "17"])
 
 
 # ============================ functions =============================
 
 
 def all_known_names() -> LStr:
     """Return all known names, that can be used in Cisco ACL (platform does not matter)."""
     items = set()
     # tcp
     items.update(set(TCP_NAME_PORT__BASE))
     items.update(set(TCP_NAME_PORT__ASA))
-    items.update(set(TCP_NAME_PORT__IOS))
+    items.update(set(TCP_NAME_PORT__IOS_16))
     items.update(set(TCP_NAME_PORT__NXOS))
     items.update(set(UDP_NAME_PORT__BASE))
     # udp
     items.update(set(UDP_NAME_PORT__BASE))
     items.update(set(UDP_NAME_PORT__ASA))
-    items.update(set(UDP_NAME_PORT__IOS))
+    items.update(set(UDP_NAME_PORT__IOS_16))
     items.update(set(UDP_NAME_PORT__NXOS))
     return sorted(items)
+
+
+# ============================= helpers ==============================
+
+
+def _init_protocol(protocol: str) -> str:
+    """Init protocol.
+
+    Convert TCP/UDP numbers to names.
+    :param protocol: Protocol: "tcp", "udp".
+    :return: Protocol: "tcp", "udp".
+    """
+    protocol = str(protocol).lower()
+    expected = ["tcp", "udp"]
+    if protocol in expected:
+        return protocol
+    if str(protocol) == "6":
+        return "tcp"
+    if str(protocol) == "17":
+        return "udp"
+    raise ValueError(f"invalid {protocol=}, {expected=}")
+
+
+def _swap(name_port: DInt) -> DiStr:
+    """Swap names and ports in dict."""
+    data: DiStr = {}
+    for name, port in name_port.items():
+        if port not in data:
+            data[port] = name
+    return data
```

### Comparing `cisco_acl-3.2.4/cisco_acl/protocol.py` & `cisco_acl-3.3.2/cisco_acl/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ACE IP protocol object."""
+
 from __future__ import annotations
 
 from functools import total_ordering
 from typing import List
 
 from cisco_acl import helpers as h
 from cisco_acl.base import Base
@@ -102,14 +103,17 @@
 
         :param line: IP protocol line.
         :type line: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description.
         :type note: Any
 
         :param protocol_nr: Well-known ip protocols as numbers.
             True  - all ip protocols as numbers,
             False - well-known ip protocols as names (default).
@@ -251,25 +255,27 @@
         :return: Protocol data.
 
         :example:
             address = Protocol(line="tcp")
             address.data() -> {
                 "line": "tcp",
                 "platform": "ios",
+                "version": "0",
                 "note": "",
                 "protocol_nr": False,
                 "has_port": False,
                 "name": "tcp",
                 "number": 6,
             }
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             note=self.note,
             protocol_nr=self._protocol_nr,
             has_port=self._has_port,
             # property
             name=self.name,
             number=self._number,
         )
```

### Comparing `cisco_acl-3.2.4/cisco_acl/remark.py` & `cisco_acl-3.3.2/cisco_acl/remark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Remark - comments in ACL."""
+
 from __future__ import annotations
 
 from functools import total_ordering
 from typing import List
 
 from cisco_acl import parsers, helpers as h
 from cisco_acl.ace_base import AceBase
@@ -18,14 +19,17 @@
 
         :param line: string of ACEs.
         :type line: str
 
         :param platform: Platform: "asa", "ios", "nxos". Default "ios".
         :type platform: str
 
+        :param version: Software version, default is "0".
+        :type version: str
+
         Helpers
         :param note: Object description
         :type note: Any
 
         :example:
             remark = Remark("10 remark text")
             remark.line -> "10 remark text"
@@ -113,14 +117,15 @@
 
         :return: Remark data.
         """
         data = dict(
             # init
             line=self.line,
             platform=self._platform,
+            version=str(self.version),
             note=self.note,
             # property
             sequence=self._sequence,
             action=self._action,
             text=self._text,
         )
         if uuid:
```

### Comparing `cisco_acl-3.2.4/cisco_acl/types_.py` & `cisco_acl-3.3.2/cisco_acl/types_.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Typing."""
+
 from ipaddress import IPv4Network, IPv4Address
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, Union
 
+from netports import SwVersion
+
 DAny = Dict[str, Any]
 DInt = Dict[str, int]
 DStr = Dict[str, str]
 DiStr = Dict[int, str]
 IInt = Iterable[int]
 IStr = Iterable[str]
 LAny = List[Any]
@@ -20,14 +23,15 @@
 SStr = Set[str]
 StrInt = Union[str, int]
 T2IStr = Tuple[int, str]
 T2Str = Tuple[str, str]
 T3Str = Tuple[str, str, str]
 TStr = Tuple[str, ...]
 UIInt = Union[bytes, float, int, str, Iterable[Union[bytes, float, int, str]]]
+UVersion = Union[SwVersion, str]
 
 DDAny = Dict[str, DAny]
 DLAny = Dict[str, LAny]
 DLStr = Dict[str, LStr]
 LDAny = List[DAny]
 LDStr = List[DStr]
 LIpNet = List[IPv4Network]
```

### Comparing `cisco_acl-3.2.4/cisco_acl/wildcard.py` & `cisco_acl-3.3.2/cisco_acl/wildcard.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
         :return: The dictionary.
         """
         data = dict(
             # init
             line=self.line,
             max_ncwb=self.max_ncwb,
             platform=self._platform,
+            version=str(self.version),
             note=self.note,
             # property
             ipnet=self.ipnet,
             prefix=self.prefix,
             wildmask=self.wildmask,
         )
         if uuid:
```

### Comparing `cisco_acl-3.2.4/pyproject.toml` & `cisco_acl-3.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cisco_acl"
-version = "3.2.4"
+version = "3.3.2"
 description = "Python package to parse and manage Cisco ACL (Access Control List)"
 authors = ["Vladimirs Prusakovs <vladimir.prusakovs@gmail.com>"]
 readme = "README.rst"
 license = "Apache-2.0"
 homepage = "https://github.com/vladimirs-git/cisco-acl"
 repository = "https://github.com/vladimirs-git/cisco-acl"
 keywords = ["cisco", "acl", "ios", "nexus", "nx-os"]
@@ -16,35 +16,34 @@
     "Programming Language :: Python :: 3.8",
     "Natural Language :: English",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 netports = "^0.12.1"
+vhelpers = "^0.1.18"
 
 [tool.poetry.group.dev.dependencies]
 dictdiffer = "^0.9.0"
-mypy = "^1.8.0"
-pygments = "^2.16.1"
-pylint = "^3.0.3"
-pytest = "^7.4.2"
-pytest-cov = "^4.1.0"
+mypy = "^1.9.0"
+pylint = "^3.1.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
 restructuredtext-lint = "^1.4.0"
-ruff = "^0.1.6"
-twine = "^4.0.2"
+ruff = "^0.3.7"
+twine = "^5.0.0"
 types-tabulate = "^0.9.0.3"
-typing-extensions = "^4.8.0"
-vhelpers = "^0.1.14"
+typing-extensions = "^4.11.0"
 
 [tool.poetry.extras]
 test = ["pytest"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/vladimirs-git/cisco-acl/issues"
-"Download URL" = "https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.4.tar.gz"
+"Download URL" = "https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.3.2.tar.gz"
 
 [tool.pylint]
 max-line-length = 100
 
 [tool.pylint.message_control]
 max-args = 10
 max-attributes = 13
@@ -58,27 +57,32 @@
 disable = [
     "invalid-name",
 ]
 
 [tool.pylint."tests.*"]
 disable = [
     "duplicate-code",
+    "line-too-long",
     "protected-access",
     "redefined-outer-name",
     "too-few-public-methods",
     "too-many-locals",
     "too-many-public-methods",
     "unsubscriptable-object",
     "unused-import",
     "use-dict-literal",
 ]
 
 [tool.mypy]
 python_version = "3.8"
 
+[[tool.mypy.overrides]]
+module = "dictdiffer.*"
+ignore_missing_imports = true
+
 [tool.ruff]
 exclude = [
     ".git",
     ".idea",
     ".mypy_cache",
     ".pytype",
     ".ruff_cache",
```

### Comparing `cisco_acl-3.2.4/README.rst` & `cisco_acl-3.3.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 - Cisco IOS (tested on ISR4331/K9, IOS XE version 16.09.06)
 - Cisco Nexus NX-OS (tested on N3K-C3172TQ-XL, NXOS version 7.0(3)I7(8))
 
 Main features:
 
 - Supports wildcards, converts wildcards to prefixes
-- Supports address groups
+- Supports uni-dimensional address groups (address-group inside other address-group is not supported)
 - Represents TCP/UDP ports and IP protocols as numbers or well-known names
 - Converts IOS syntax to NX-OS and vice vera
 - Generates sequence numbers for ACEs
 - Looks for and removes ACEs in the shadow (rules without hits)
 - Groups ACEs to blocks. After sorting, the order of ACEs within a group does not change
 
 .. contents:: **Contents**
@@ -56,15 +56,15 @@
 
     pip install cisco-acl
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.4.tar.gz
+    pip install https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.3.2.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/cisco-acl
 
@@ -78,14 +78,15 @@
 grouped to *AceGroup* by text in remarks (param `group_by`)
 
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 config          *str*        Cisco config, "show running-config" output
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 names           *List[str]*  Parses only ACLs with specified names, skips any other
 max_ncwb        *int*        Max count of non-contiguous wildcard bits
 indent          *str*        ACE lines indentation (default "  ")
 protocol_nr     *bool*       Well-known ip protocols as numbers, True  - all ip protocols as numbers, False - well-known ip protocols as names (default)
 port_nr         *bool*       Well-known TCP/UDP ports as numbers, True  - all tcp/udp ports as numbers, False - well-known tcp/udp ports as names (default)
 group_by        *str*        Startswith in remark line. ACEs group, starting from the Remark, where line startswith `group_by`, will be applied to the same AceGroup, until next Remark that also startswith `group_by`
 =============== ============ =======================================================================
@@ -104,14 +105,15 @@
 Creates *Ace* objects based on the "show running-config" output
 
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 config          *str*        Cisco config, "show running-config" output
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 max_ncwb        *int*        Max count of non-contiguous wildcard bits
 protocol_nr     *bool*       Well-known ip protocols as numbers, True  - all ip protocols as numbers, False - well-known ip protocols as names (default)
 port_nr         *bool*       Well-known TCP/UDP ports as numbers, True  - all tcp/udp ports as numbers, False - well-known tcp/udp ports as names (default)
 group_by        *str*        Startswith in remark line. ACEs group, starting from the Remark, where line startswith `group_by`, will be applied to the same AceGroup, until next Remark that also startswith `group_by`
 =============== ============ =======================================================================
 
 Return
@@ -128,14 +130,15 @@
 Creates *AddrGroup* objects based on the "show running-config" output
 
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 config          *str*        Cisco config, "show running-config" output
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 max_ncwb        *int*        Max count of non-contiguous wildcard bits
 indent          *str*        ACE lines indentation (default "  ")
 =============== ============ =======================================================================
 
 Return
     List of *AddrGroup* objects
 
@@ -148,14 +151,15 @@
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 srcports        *str*        Range of TCP/UDP source ports
 dstports        *str*        Range of TCP/UDP destination ports
 line            *str*        ACE pattern, on whose basis new ACEs will be generated (default "permit tcp any any", operator "eq")
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 port_nr         *bool*       Well-known TCP/UDP ports as numbers, True  - all tcp/udp ports as numbers, False - well-known tcp/udp ports as names (default)
 =============== ============ =======================================================================
 
 Return
     List of newly generated ACE lines
 
 **Examples**
@@ -170,14 +174,15 @@
 
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 protocols       *str*        Range of IP protocols
 line            *str*        ACE pattern, on whose basis new ACEs will be generated (default "permit ip any any")
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 protocol_nr     *bool*       Well-known ip protocols as numbers, True  - all ip protocols as numbers, False - well-known ip protocols as names (default)
 =============== ============ =======================================================================
 
 Return
     List of newly generated ACE lines
 
 **Examples**
```

### Comparing `cisco_acl-3.2.4/PKG-INFO` & `cisco_acl-3.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cisco_acl
-Version: 3.2.4
+Version: 3.3.2
 Summary: Python package to parse and manage Cisco ACL (Access Control List)
 Home-page: https://github.com/vladimirs-git/cisco-acl
 License: Apache-2.0
 Keywords: cisco,acl,ios,nexus,nx-os
 Author: Vladimirs Prusakovs
 Author-email: vladimir.prusakovs@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,16 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Networking
 Provides-Extra: test
 Requires-Dist: netports (>=0.12.1,<0.13.0)
+Requires-Dist: vhelpers (>=0.1.18,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/vladimirs-git/cisco-acl/issues
-Project-URL: Download URL, https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.4.tar.gz
+Project-URL: Download URL, https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.3.2.tar.gz
 Project-URL: Repository, https://github.com/vladimirs-git/cisco-acl
 Description-Content-Type: text/x-rst
 
 
 .. image:: https://img.shields.io/pypi/v/cisco-acl.svg
    :target: https://pypi.python.org/pypi/cisco-acl
 .. image:: https://img.shields.io/pypi/pyversions/cisco-acl.svg
@@ -41,15 +42,15 @@
 
 - Cisco IOS (tested on ISR4331/K9, IOS XE version 16.09.06)
 - Cisco Nexus NX-OS (tested on N3K-C3172TQ-XL, NXOS version 7.0(3)I7(8))
 
 Main features:
 
 - Supports wildcards, converts wildcards to prefixes
-- Supports address groups
+- Supports uni-dimensional address groups (address-group inside other address-group is not supported)
 - Represents TCP/UDP ports and IP protocols as numbers or well-known names
 - Converts IOS syntax to NX-OS and vice vera
 - Generates sequence numbers for ACEs
 - Looks for and removes ACEs in the shadow (rules without hits)
 - Groups ACEs to blocks. After sorting, the order of ACEs within a group does not change
 
 .. contents:: **Contents**
@@ -83,15 +84,15 @@
 
     pip install cisco-acl
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.2.4.tar.gz
+    pip install https://github.com/vladimirs-git/cisco-acl/archive/refs/tags/3.3.2.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/cisco-acl
 
@@ -105,14 +106,15 @@
 grouped to *AceGroup* by text in remarks (param `group_by`)
 
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 config          *str*        Cisco config, "show running-config" output
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 names           *List[str]*  Parses only ACLs with specified names, skips any other
 max_ncwb        *int*        Max count of non-contiguous wildcard bits
 indent          *str*        ACE lines indentation (default "  ")
 protocol_nr     *bool*       Well-known ip protocols as numbers, True  - all ip protocols as numbers, False - well-known ip protocols as names (default)
 port_nr         *bool*       Well-known TCP/UDP ports as numbers, True  - all tcp/udp ports as numbers, False - well-known tcp/udp ports as names (default)
 group_by        *str*        Startswith in remark line. ACEs group, starting from the Remark, where line startswith `group_by`, will be applied to the same AceGroup, until next Remark that also startswith `group_by`
 =============== ============ =======================================================================
@@ -131,14 +133,15 @@
 Creates *Ace* objects based on the "show running-config" output
 
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 config          *str*        Cisco config, "show running-config" output
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 max_ncwb        *int*        Max count of non-contiguous wildcard bits
 protocol_nr     *bool*       Well-known ip protocols as numbers, True  - all ip protocols as numbers, False - well-known ip protocols as names (default)
 port_nr         *bool*       Well-known TCP/UDP ports as numbers, True  - all tcp/udp ports as numbers, False - well-known tcp/udp ports as names (default)
 group_by        *str*        Startswith in remark line. ACEs group, starting from the Remark, where line startswith `group_by`, will be applied to the same AceGroup, until next Remark that also startswith `group_by`
 =============== ============ =======================================================================
 
 Return
@@ -155,14 +158,15 @@
 Creates *AddrGroup* objects based on the "show running-config" output
 
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 config          *str*        Cisco config, "show running-config" output
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 max_ncwb        *int*        Max count of non-contiguous wildcard bits
 indent          *str*        ACE lines indentation (default "  ")
 =============== ============ =======================================================================
 
 Return
     List of *AddrGroup* objects
 
@@ -175,14 +179,15 @@
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 srcports        *str*        Range of TCP/UDP source ports
 dstports        *str*        Range of TCP/UDP destination ports
 line            *str*        ACE pattern, on whose basis new ACEs will be generated (default "permit tcp any any", operator "eq")
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 port_nr         *bool*       Well-known TCP/UDP ports as numbers, True  - all tcp/udp ports as numbers, False - well-known tcp/udp ports as names (default)
 =============== ============ =======================================================================
 
 Return
     List of newly generated ACE lines
 
 **Examples**
@@ -197,14 +202,15 @@
 
 =============== ============ =======================================================================
 Parameter       Type         Description
 =============== ============ =======================================================================
 protocols       *str*        Range of IP protocols
 line            *str*        ACE pattern, on whose basis new ACEs will be generated (default "permit ip any any")
 platform        *str*        Platform: "ios" (default), "nxos"
+version         *str*        Software version, default is "0".
 protocol_nr     *bool*       Well-known ip protocols as numbers, True  - all ip protocols as numbers, False - well-known ip protocols as names (default)
 =============== ============ =======================================================================
 
 Return
     List of newly generated ACE lines
 
 **Examples**
```

