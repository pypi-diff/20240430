# Comparing `tmp/sockaddr-0.1.2.tar.gz` & `tmp/sockaddr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockaddr-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sockaddr-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sockaddr-0.1.2.tar` & `sockaddr-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       21 2024-03-14 15:20:57.625383 sockaddr-0.1.2/.gitignore
--rw-r--r--   0        0        0    32422 2024-03-14 14:13:36.111296 sockaddr-0.1.2/LICENSE
--rw-r--r--   0        0        0      600 2024-03-14 15:36:35.216773 sockaddr-0.1.2/README.md
--rw-r--r--   0        0        0      782 2024-03-14 15:37:17.808560 sockaddr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      331 2024-03-14 15:37:30.040499 sockaddr-0.1.2/sockaddr/__init__.py
--rw-r--r--   0        0        0     3111 2024-03-14 15:03:02.022804 sockaddr-0.1.2/sockaddr/addr.py
--rw-r--r--   0        0        0     1643 2024-03-14 15:12:51.063809 sockaddr-0.1.2/sockaddr/util.py
--rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 sockaddr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-03-14 15:20:57.625383 sockaddr-0.1.3/.gitignore
+-rw-r--r--   0        0        0    32422 2024-03-14 14:13:36.111296 sockaddr-0.1.3/LICENSE
+-rw-r--r--   0        0        0      600 2024-03-14 15:36:35.216773 sockaddr-0.1.3/README.md
+-rw-r--r--   0        0        0      782 2024-03-14 15:37:17.808560 sockaddr-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      331 2024-04-30 14:12:59.377784 sockaddr-0.1.3/sockaddr/__init__.py
+-rw-r--r--   0        0        0     3183 2024-04-30 14:12:21.045967 sockaddr-0.1.3/sockaddr/addr.py
+-rw-r--r--   0        0        0     1643 2024-03-14 15:12:51.063809 sockaddr-0.1.3/sockaddr/util.py
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 sockaddr-0.1.3/PKG-INFO
```

### Comparing `sockaddr-0.1.2/LICENSE` & `sockaddr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sockaddr-0.1.2/README.md` & `sockaddr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sockaddr-0.1.2/pyproject.toml` & `sockaddr-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sockaddr-0.1.2/sockaddr/addr.py` & `sockaddr-0.1.3/sockaddr/addr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import ctypes
 
 # Without this, the comments at the end of each field will break
 # fmt:off
 
-class sockaddr_un(ctypes.Structure):
+class sockaddr_un(ctypes.BigEndianStructure):
     """UNIX Socket
 
     man 7 unix
     Defined in <linux/un.h>"""
 
     _fields_ = [
         ("sun_family", ctypes.c_ushort),    # AF_UNIX (POSIX: AF_LOCAL)
         ("sun_path", ctypes.c_char * 108),  # Pathname
     ]
 
 
-class sockaddr_in(ctypes.Structure):
+class sockaddr_in(ctypes.BigEndianStructure):
     """IPv4 Socket
 
     man 7 ip
     sys/socket.h
     <linux/in.h>
     <netinet/in.h>"""
 
@@ -27,68 +27,68 @@
         ("sin_family", ctypes.c_ushort),    # AF_INET
         ("sin_port", ctypes.c_ushort),      # port number
         ("sin_addr", ctypes.c_byte * 4),    # IPv4 address
         ("__pad", ctypes.c_byte * (8)),     # Padding to 16 bytes
     ]
 
 
-class sockaddr_in6(ctypes.Structure):
+class sockaddr_in6(ctypes.BigEndianStructure):
     """IPv6 Socket
 
     man 7 ipv6
     <netinet/in.h>"""
 
     _fields_ = [
         ("sin6_family", ctypes.c_ushort),   # AF_INET6
         ("sin6_port", ctypes.c_ushort),     # port number
         ("sin6_flowinfo", ctypes.c_uint32), # IPv6 flow identifier
         ("sin6_addr", ctypes.c_byte * 16),  # IPv6 address
         ("sin6_scope_id", ctypes.c_uint32), # Scope ID
     ]
 
 
-class sockaddr_nl(ctypes.Structure):
+class sockaddr_nl(ctypes.BigEndianStructure):
     """Netlink Socket
 
     man 7 netlink
     <linux/netlink.h>"""
 
     _fields_ = [
         ("nl_family", ctypes.c_ushort),     # AF_NETLINK
         ("nl_pad", ctypes.c_ushort),        # Zero
         ("nl_pid", ctypes.c_uint32),        # Netlink socket (usually the pid, but check the man page!)
         ("nl_groups", ctypes.c_uint32),     # Bitmask with every bit representing a netlink group number.
     ]
 
 
-class sockaddr_x25(ctypes.Structure):
+class sockaddr_x25(ctypes.BigEndianStructure):
     """ITU-T X.25 Socket
 
     man 7 x25
     <linux/x25.h>"""
 
     _fields_ = [
         ("sx25_family", ctypes.c_ushort),   # AF_X25
         ("sx25_addr", ctypes.c_char * 16),  # Char array that forms the X.121 address
     ]
 
 
-class sockaddr_atalk(ctypes.Structure):
+class sockaddr_atalk(ctypes.BigEndianStructure):
     """AppleTalk Socket
     
     man 7 ddp
     <netatalk/at.h>"""
     _fields_ = [
         ("sat_family", ctypes.c_ushort),    # AF_APPLETALK
         ("sat_port", ctypes.c_ubyte),       # port number (<127 are reserved)
         ("sat_s_net", ctypes.c_ushort),     # Host network
         ("sat_s_node", ctypes.c_ubyte),     # Host node number
     ]
 
-class sockaddr_ll(ctypes.Structure):
+class sockaddr_ll(ctypes.BigEndianStructure):
     """Packet interface on device level
     
     man 7 packet
     <net/ethernet.h>
     <linux/if_packet.h>"""
     _fields_ = [
         ("sll_family", ctypes.c_ushort),    # AF_PACKET
@@ -97,13 +97,13 @@
         ("sll_hatype", ctypes.c_ushort),    # ARP hardware type
         ("sll_pkttype", ctypes.c_ubyte),    # Packet type (PACKET_HOST, PACKET_BROADCAST, etc.)
         ("sll_halen", ctypes.c_ubyte),      # Length of address
         ("sll_addr", ctypes.c_char * 8),    # Physical layer address
     ]
 
 
-class sockaddr_storage(ctypes.Structure):
+class sockaddr_storage(ctypes.BigEndianStructure):
 
     _fields_ = [
         ("ss_family", ctypes.c_ushort),     # address family
         ("__data", ctypes.c_ubyte * 124)    # data
     ]
```

### Comparing `sockaddr-0.1.2/sockaddr/util.py` & `sockaddr-0.1.3/sockaddr/util.py`

 * *Files identical despite different names*

### Comparing `sockaddr-0.1.2/PKG-INFO` & `sockaddr-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockaddr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Prepopulated sockaddr helpers for Python using ctypes
 Keywords: sockaddr,saddr,auditd
 Author-email: tedk <tedk@kpn-cert.nl>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

