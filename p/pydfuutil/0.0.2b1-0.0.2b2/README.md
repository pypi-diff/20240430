# Comparing `tmp/pydfuutil-0.0.2b1.tar.gz` & `tmp/pydfuutil-0.0.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydfuutil-0.0.2b1.tar", last modified: Mon Apr 29 19:08:06 2024, max compression
+gzip compressed data, was "pydfuutil-0.0.2b2.tar", last modified: Tue Apr 30 20:56:30 2024, max compression
```

## Comparing `pydfuutil-0.0.2b1.tar` & `pydfuutil-0.0.2b2.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:08:06.334406 pydfuutil-0.0.2b1/pydfuutil/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    19172 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/portable.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/quirks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/usb_dfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/pydfuutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/tests/test_dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/tests/test_dfu_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/pydfuutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37429 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19545 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/portable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/quirks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/usb_dfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/pydfuutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_quirks.py
```

### Comparing `pydfuutil-0.0.2b1/LICENSE` & `pydfuutil-0.0.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b1/PKG-INFO` & `pydfuutil-0.0.2b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.2b1
+Version: 0.0.2b2
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -187,16 +187,19 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyusb
 Requires-Dist: libusb-package
 Requires-Dist: rich
 Requires-Dist: construct
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pylint; extra == "test"
 
 # PyDfuUtil - Pure python fork of **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)** wrappers to **[libusb](https://github.com/libusb/libusb)**
 
 [![PyPI Version](https://img.shields.io/pypi/v/pydfuutil?label=PyPI&logo=pypi)](https://pypi.org/project/pydfuutil/)
 
 ## Table of contents
 * **[Introduction](#introduction)**
@@ -245,41 +248,42 @@
 ### dfu-util
 ```Bash
 pydfuutil -h 
 # or
 python -m pydfuutil -h
 
 ####### usage:
-usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d VID:PID] [-p BUS-PORT] [-c CONFIG_NR] [-i INTF_NR] [-a ALT] [-t SIZE] [-U FILE] [-D FILE] [-R] [-s ADDRESS]
+usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d <deviceID>:<productID>] [-p <bus/port>] [-c <config>] [-i <intf_num>] [-a <alt>] [-t <size>] [-U <file>] [-D <file>] [-R] [-s <address>]
 
 Python implementation of DFU-Util tools
 
 options:
   -h, --help            show this help message and exit
   -V, --version         Print the version number
   -v, --verbose         Print verbose debug statements
   -l, --list            List the currently attached DFU capable USB devices
   -e, --detach          Detach the currently attached DFU capable USB devices
-  -d VID:PID, --device VID:PID
+  -d <deviceID>:<productID>, --device <deviceID>:<productID>
                         Specify Vendor/Product ID of DFU device
-  -p BUS-PORT, --path BUS-PORT
+  -p <bus/port>, --path <bus/port>
                         Specify path to DFU device
-  -c CONFIG_NR, --cfg CONFIG_NR
+  -c <config>, --cfg <config>
                         Specify the Configuration of DFU device
-  -i INTF_NR, --intf INTF_NR
+  -i <interface>, --intf <interface>
                         Specify the DFU Interface number
-  -a ALT, --alt ALT     Specify the Altsetting of the DFU Interface
-  -t SIZE, --transfer-size SIZE
+  -a <alt>, --alt <alt>
+                        Specify the Altsetting of the DFU Interface
+  -t <size>, --transfer-size <size>
                         Specify the number of bytes per USB Transfer
-  -U FILE, --upload FILE
+  -U <file>, --upload <file>
                         Read firmware from device into <file>
-  -D FILE, --download FILE
+  -D <file>, --download <file>
                         Write firmware from <file> into device
   -R, --reset           Issue USB Reset signalling once we`re finished
-  -s ADDRESS, --dfuse-address ADDRESS
+  -s <address>, --dfuse-address <address>
                         ST DfuSe mode, specify target address for raw file download or upload. Not applicable for DfuSe file (.dfu) downloads
 ```
 
 ### dfu-suffix
 ```Bash
 pydfuutil-suffix -h
 # or 
@@ -305,62 +309,26 @@
                         Add device ID into DFU suffix in <file>
   -s <address>, --stellaris-address <address>
                         Specify lmdfu address for LMDFU_ADD
   -T, --stellaris       Set lmdfu mode to LMDFU_CHECK
 
 ```
 
-
-## Todos
-
-#### Modules to implement:
-
-- [ ] main
-  - [x] atoi()
-  - [ ] usb_path2devnum()
-  - [x] find_dfu_if()
-  - [x] _get_first_cb()
-  - [x] _get_first_dfu_if()
-  - [x] _check_match_cb()
-  - [x] get_matching_dfu_if()
-  - [x] _count_match_cb()
-  - [x] count_matching_dfu_if()
-  - [x] get_alt_name()
-  - [x] print_dfu_if()
-  - [x] list_dfu_interfaces()
-  - [x] alt_by_name()
-  - [x] _count_cb()
-  - [x] count_dfu_interfaces()
-  - [x] iterate_dfu_devices()
-  - [x] found_dfu_device()
-  - [x] get_first_dfu_device()
-  - [x] count_one_dfu_device()
-  - [x] count_dfu_devices()
-  - [x] parse_vendprod()
-  - [ ] resolve_device_path()
-  - [x] find_descriptor()
-  - [ ] usb_get_any_descriptor()
-  - [x] get_cached_extra_descriptor()
-  - [x] help_()
-  - [x] print_version()
-  - [ ] main()
-- [ ] dfu_load.PROGRESS_BAR -> rich.Progress
-
-
 #### Done:
 - [x] dfu
 - [x] dfu_file
 - [x] dfu_load
 - [x] portable
 - [x] quirks
-- [x] suffix
+- [x] suffix + cli entry point
 - [x] usb_dfu
 - [x] lmdfu
 - [x] dfuse_mem
-- [x] dfuse
+- [ ] dfuse (not fully supported yet)
+- [ ] dfu-util cli entry point (not fully supported yet)
 
 
 ## Getting help
 * To report a bug or propose a new feature, use our issue tracker. But please search the database before opening a new issue.
 
 ## About
 Dfu-util - Device Firmware Upgrade Utilities
```

### Comparing `pydfuutil-0.0.2b1/README.md` & `pydfuutil-0.0.2b2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -49,41 +49,42 @@
 ### dfu-util
 ```Bash
 pydfuutil -h 
 # or
 python -m pydfuutil -h
 
 ####### usage:
-usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d VID:PID] [-p BUS-PORT] [-c CONFIG_NR] [-i INTF_NR] [-a ALT] [-t SIZE] [-U FILE] [-D FILE] [-R] [-s ADDRESS]
+usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d <deviceID>:<productID>] [-p <bus/port>] [-c <config>] [-i <intf_num>] [-a <alt>] [-t <size>] [-U <file>] [-D <file>] [-R] [-s <address>]
 
 Python implementation of DFU-Util tools
 
 options:
   -h, --help            show this help message and exit
   -V, --version         Print the version number
   -v, --verbose         Print verbose debug statements
   -l, --list            List the currently attached DFU capable USB devices
   -e, --detach          Detach the currently attached DFU capable USB devices
-  -d VID:PID, --device VID:PID
+  -d <deviceID>:<productID>, --device <deviceID>:<productID>
                         Specify Vendor/Product ID of DFU device
-  -p BUS-PORT, --path BUS-PORT
+  -p <bus/port>, --path <bus/port>
                         Specify path to DFU device
-  -c CONFIG_NR, --cfg CONFIG_NR
+  -c <config>, --cfg <config>
                         Specify the Configuration of DFU device
-  -i INTF_NR, --intf INTF_NR
+  -i <interface>, --intf <interface>
                         Specify the DFU Interface number
-  -a ALT, --alt ALT     Specify the Altsetting of the DFU Interface
-  -t SIZE, --transfer-size SIZE
+  -a <alt>, --alt <alt>
+                        Specify the Altsetting of the DFU Interface
+  -t <size>, --transfer-size <size>
                         Specify the number of bytes per USB Transfer
-  -U FILE, --upload FILE
+  -U <file>, --upload <file>
                         Read firmware from device into <file>
-  -D FILE, --download FILE
+  -D <file>, --download <file>
                         Write firmware from <file> into device
   -R, --reset           Issue USB Reset signalling once we`re finished
-  -s ADDRESS, --dfuse-address ADDRESS
+  -s <address>, --dfuse-address <address>
                         ST DfuSe mode, specify target address for raw file download or upload. Not applicable for DfuSe file (.dfu) downloads
 ```
 
 ### dfu-suffix
 ```Bash
 pydfuutil-suffix -h
 # or 
@@ -109,62 +110,26 @@
                         Add device ID into DFU suffix in <file>
   -s <address>, --stellaris-address <address>
                         Specify lmdfu address for LMDFU_ADD
   -T, --stellaris       Set lmdfu mode to LMDFU_CHECK
 
 ```
 
-
-## Todos
-
-#### Modules to implement:
-
-- [ ] main
-  - [x] atoi()
-  - [ ] usb_path2devnum()
-  - [x] find_dfu_if()
-  - [x] _get_first_cb()
-  - [x] _get_first_dfu_if()
-  - [x] _check_match_cb()
-  - [x] get_matching_dfu_if()
-  - [x] _count_match_cb()
-  - [x] count_matching_dfu_if()
-  - [x] get_alt_name()
-  - [x] print_dfu_if()
-  - [x] list_dfu_interfaces()
-  - [x] alt_by_name()
-  - [x] _count_cb()
-  - [x] count_dfu_interfaces()
-  - [x] iterate_dfu_devices()
-  - [x] found_dfu_device()
-  - [x] get_first_dfu_device()
-  - [x] count_one_dfu_device()
-  - [x] count_dfu_devices()
-  - [x] parse_vendprod()
-  - [ ] resolve_device_path()
-  - [x] find_descriptor()
-  - [ ] usb_get_any_descriptor()
-  - [x] get_cached_extra_descriptor()
-  - [x] help_()
-  - [x] print_version()
-  - [ ] main()
-- [ ] dfu_load.PROGRESS_BAR -> rich.Progress
-
-
 #### Done:
 - [x] dfu
 - [x] dfu_file
 - [x] dfu_load
 - [x] portable
 - [x] quirks
-- [x] suffix
+- [x] suffix + cli entry point
 - [x] usb_dfu
 - [x] lmdfu
 - [x] dfuse_mem
-- [x] dfuse
+- [ ] dfuse (not fully supported yet)
+- [ ] dfu-util cli entry point (not fully supported yet)
 
 
 ## Getting help
 * To report a bug or propose a new feature, use our issue tracker. But please search the database before opening a new issue.
 
 ## About
 Dfu-util - Device Firmware Upgrade Utilities
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil/__main__.py` & `pydfuutil-0.0.2b2/pydfuutil/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,40 +6,43 @@
 import argparse
 import errno
 import logging
 import os
 import re
 import sys
 from enum import IntFlag
-from typing import Any, Callable
+from typing import Any, Callable, Literal
 
-import libusb_package
 import usb.core
-from usb.backend import libusb1
 
-from pydfuutil import __version__, __copyright__, dfuse, dfu_load
+from pydfuutil import __version__, __copyright__
 from pydfuutil import dfu
+# from pydfuutil import dfuse
+from pydfuutil import dfu_load
 from pydfuutil.dfu_file import DFUFile, parse_dfu_suffix
 from pydfuutil.logger import get_logger
 from pydfuutil.portable import milli_sleep
 from pydfuutil.quirks import set_quirks, QUIRK_POLLTIMEOUT, QUIRK_FORCE_DFU11
 from pydfuutil.usb_dfu import USB_DT_DFU, bmAttributes, USB_DFU_FUNC_DESCRIPTOR
 
-logging.basicConfig(level=logging.DEBUG)
-logging.propagate = False
-logger = get_logger("dfu_util")
+try:
+    import libusb_package
+    from usb.backend import libusb1
+    libusb1.get_backend(libusb_package.find_library)
+except ImportError:
+    pass
+
+logger = get_logger("pydfuutil")
 logger.setLevel(logging.INFO)
 usb_logger = logging.getLogger('usb')
+
 MAX_DESC_STR_LEN = 253
 HAVE_GETPAGESIZE = not (sys.platform == 'win32')
 VERBOSE = False
 
-# TODO: not implemented yet
-libusb1.get_backend(libusb_package.find_library)
-
 
 def atoi(s: str) -> int:
     """
     Regular expression to match the integer part of the string
     :param s: input
     :return: Return 0 if no integer is found
     """
@@ -90,14 +93,15 @@
                     devnum=dev.address,
                     path=dev.address,
                     flags=0,
                     count=0,
                     dev=dev
                 )
 
+                logger.debug(f"{handler.__name__}, {handler}, {v}")
                 if handler:
                     rc = handler(dfu_if, v)
                     if rc != 0:
                         return rc
 
     return 0
 
@@ -553,41 +557,48 @@
     return value.to_bytes(2, byteorder='little')
 
 
 def le16_to_cpu(data):
     return int.from_bytes(data, byteorder='little')
 
 
-class IntOrBytes:
-    def __init__(self, value):
-        if isinstance(value, int):
-            self._value = value
-        elif isinstance(value, bytes):
-            self._value = int.from_bytes(value, byteorder='big', signed=True)
-        else:
-            raise TypeError("Value must be int or bytes")
-
-    def __lt__(self, other):
-        if isinstance(other, IntOrBytes):
-            return self._value < other._value
-        elif isinstance(other, int):
-            return self._value < other
-        else:
-            raise TypeError("Comparison with unsupported type")
+# class IntOrBytes:
+#     def __init__(self, value):
+#         if isinstance(value, int):
+#             self._value = value
+#         elif isinstance(value, bytes):
+#             self._value = int.from_bytes(value, byteorder='big', signed=True)
+#         else:
+#             raise TypeError("Value must be int or bytes")
+#
+#     def __lt__(self, other):
+#         if isinstance(other, IntOrBytes):
+#             return self._value < other._value
+#         if isinstance(other, int):
+#             return self._value < other
+#         raise TypeError("Comparison with unsupported type")
+#
+#     def __eq__(self, other):
+#         if isinstance(other, IntOrBytes):
+#             return self._value == other._value
+#         elif isinstance(other, int):
+#             return self._value == other
+#         else:
+#             raise TypeError("Comparison with unsupported type")
+#
+#     def __repr__(self):
+#         return f"IntOrBytes({self._value})"
 
-    def __eq__(self, other):
-        if isinstance(other, IntOrBytes):
-            return self._value == other._value
-        elif isinstance(other, int):
-            return self._value == other
-        else:
-            raise TypeError("Comparison with unsupported type")
 
-    def __repr__(self):
-        return f"IntOrBytes({self._value})"
+def int_(value: [int, (bytes, bytearray)], order: Literal["little", "big"] = 'little'):
+    if isinstance(value, int):
+        return value
+    if isinstance(value, (bytes, bytearray)):
+        return int.from_bytes(value, order)
+    raise TypeError("Unsupported type")
 
 
 def main() -> None:
     # Todo: implement
 
     global VERBOSE
 
@@ -602,33 +613,33 @@
                         help="Print the version number")
     parser.add_argument("-v", "--verbose", action="store_true",
                         help="Print verbose debug statements")
     parser.add_argument("-l", "--list", action="store_true",
                         help="List the currently attached DFU capable USB devices")
     parser.add_argument("-e", "--detach", action="store_true",
                         help="Detach the currently attached DFU capable USB devices")
-    parser.add_argument("-d", "--device", metavar="VID:PID",
+    parser.add_argument("-d", "--device", metavar="<deviceID>:<productID>",
                         help="Specify Vendor/Product ID of DFU device")
-    parser.add_argument("-p", "--path", metavar="BUS-PORT",
+    parser.add_argument("-p", "--path", metavar="<bus/port>",
                         help="Specify path to DFU device")
-    parser.add_argument("-c", "--cfg", metavar="CONFIG_NR",
+    parser.add_argument("-c", "--cfg", metavar="<config>",
                         help="Specify the Configuration of DFU device")
-    parser.add_argument("-i", "--intf", metavar="INTF_NR",
+    parser.add_argument("-i", "--intf", metavar="<interface>",
                         help="Specify the DFU Interface number")
-    parser.add_argument("-a", "--alt", metavar="ALT",
+    parser.add_argument("-a", "--alt", metavar="<alt>",
                         help="Specify the Altsetting of the DFU Interface")
-    parser.add_argument("-t", "--transfer-size", metavar="SIZE",
+    parser.add_argument("-t", "--transfer-size", metavar="<size>",
                         help="Specify the number of bytes per USB Transfer")
-    parser.add_argument("-U", "--upload", metavar="FILE",
+    parser.add_argument("-U", "--upload", metavar="<file>",
                         help="Read firmware from device into <file>")
-    parser.add_argument("-D", "--download", metavar="FILE",
+    parser.add_argument("-D", "--download", metavar="<file>",
                         help="Write firmware from <file> into device")
     parser.add_argument("-R", "--reset", action="store_true",
                         help="Issue USB Reset signalling once we're finished")
-    parser.add_argument("-s", "--dfuse-address", metavar="ADDRESS",
+    parser.add_argument("-s", "--dfuse-address", metavar="<address>",
                         help="ST DfuSe mode, specify target address "
                              "for raw file download or upload. "
                              "Not applicable for DfuSe file (.dfu) downloads")
 
     # Parse arguments
     args = parser.parse_args()
 
@@ -643,14 +654,16 @@
     final_reset = 0
 
     func_dfu_rt = USB_DFU_FUNC_DESCRIPTOR.parse(bytes(USB_DFU_FUNC_DESCRIPTOR.sizeof()))
     func_dfu = USB_DFU_FUNC_DESCRIPTOR.parse(bytes(USB_DFU_FUNC_DESCRIPTOR.sizeof()))
 
     if args.verbose:
         VERBOSE = True
+        logger.setLevel(logging.DEBUG)
+        usb_logger.setLevel(logging.DEBUG)
 
     if args.list:
         mode = Mode.LIST
 
     if args.detach:
         mode = Mode.DETACH
 
@@ -711,18 +724,14 @@
         dif.vendor, dif.product = parse_vendprod(device_id_filter)
         logger.info(f"Filter on VID = 0x{dif.vendor:04X} PID = 0x{dif.product:04X}\n")
         if dif.vendor:
             dif.flags |= dfu.Mode.IFF_VENDOR
         if dif.product:
             dif.flags |= dfu.Mode.IFF_PRODUCT
 
-    if VERBOSE:
-        logger.setLevel(logging.DEBUG)
-        usb_logger.setLevel(logging.DEBUG)
-
     # libusb init
     libusb_ctx = list(usb.core.find(find_all=True, **dif.device_ids))
 
     if mode == Mode.LIST:
         list_dfu_interfaces(libusb_ctx)
         sys.exit(0)
 
@@ -771,15 +780,15 @@
     # E.g. Free runner does not like to be requested at this point
 
     ret = get_cached_extra_descriptor(
         _rt_dif.dev, _rt_dif.configuration, _rt_dif.interface,
         # USB_DT_DFU, 0, le16_to_cpu(func_dfu_rt.bcdDFUVersion)
         USB_DT_DFU, 0, USB_DFU_FUNC_DESCRIPTOR.bcdDFUVersion.build(func_dfu_rt.bcdDFUVersion)
     )
-    ret = IntOrBytes(ret)
+    ret = int_(ret)
     if ret == 7:
         logger.info("Deducing device DFU version from functional descriptor "
                     "length")
         func_dfu_rt.bcdDFUVersion = 0x0100
     elif ret < 9:
         logger.warning("Can not find cached DFU functional "
                        "descriptor")
@@ -790,61 +799,64 @@
 
     # Transition from run-Time mode to DFU mode
 
     # status_again
     def check_status():
         logger.debug('Status again')
         _log_msg = "Determining device status: "
-        _, status = dfu.get_status(_rt_dif.dev, _rt_dif.interface)
-        if _ < 0:
+        # ret = int(status_ := dfu.get_status(_rt_dif.dev, _rt_dif.interface))
+        # ret = int(status_ := dif.get_status())
+        # if ret < 0:
+        if int(status_ := dif.get_status()) < 0:
             logger.error(f"{_log_msg}error get_status")
             sys.exit(1)
-        logger.info(f"{_log_msg}state = {dfu.state_to_string(status.bState)}, "
-                    f"status = {status.bStatus}")
+        logger.info(f"{_log_msg}state = {status_.bState.to_string()}, "
+                    f"status = {status_.bStatus}")
 
         if not quirks & QUIRK_POLLTIMEOUT:
-            milli_sleep(status.bwPollTimeout)
-        return status
+            milli_sleep(status_.bwPollTimeout)
+        return status_
 
     while not (_rt_dif.flags & dfu.Mode.IFF_DFU):
         # In the 'first round' during runtime mode, there can only be one
         # DFU Interface descriptor according to the DFU Spec.
 
         # FIXME: check if the selected device really has only one
 
         logger.info("Claiming USB DFU Runtime Interface...")
         try:
             usb.util.claim_interface(_rt_dif.dev, _rt_dif.interface)
-        except usb.core.USBError as exc:
+        except usb.core.USBError:
             logger.error(f"Cannot claim interface {_rt_dif.interface}")
             sys.exit(1)
 
         try:
             _rt_dif.dev.set_interface_altsetting(_rt_dif.interface, 0)
-        except usb.core.USBError as exc:
+        except usb.core.USBError:
             logger.error(f"Cannot set alt interface zero")
             sys.exit(1)
 
         status = check_status()
 
         if status.bState in (dfu.State.APP_IDLE, dfu.State.APP_DETACH):
             logger.info("Device really in Runtime Mode, send DFU "
                         "detach request...")
 
-            if IntOrBytes(dfu.detach(_rt_dif.dev, _rt_dif.interface, 1000)) < 0:
+            # if IntOrBytes(dfu.detach(_rt_dif.dev, _rt_dif.interface, 1000)) < 0:
+            if int_(_rt_dif.detach(1000)) < 0:
                 logger.error("error detaching")
                 sys.exit(1)
 
             if func_dfu_rt.bmAttributes & bmAttributes.USB_DFU_WILL_DETACH:
                 logger.info("Device will detach and reattach...")
             else:
                 logger.info("Resetting USB...\n")
                 try:
                     _rt_dif.dev.reset()
-                except usb.core.USBError as exc:
+                except usb.core.USBError:
                     logger.error("error resetting after detach")
             milli_sleep(2000)
             break
         elif status.bState == dfu.State.DFU_ERROR:
             logger.error("dfuERROR, clearing status")
             if dfu.clear_status(_rt_dif.dev, _rt_dif.interface) < 0:
                 logger.error("error detaching")
@@ -859,15 +871,15 @@
         if mode == Mode.DETACH:
             usb.util.release_interface(_rt_dif.dev, _rt_dif.interface)
             usb.util.dispose_resources(_rt_dif.dev)
             sys.exit(0)
 
         if dif.flags & dfu.Mode.IFF_PATH:
             ret = resolve_device_path(dif)
-            if IntOrBytes(ret) < 0:
+            if int_(ret) < 0:
                 logger.error(f"internal error: cannot re-parse {dif.path}")
                 sys.exit(1)
             if not ret:
                 logger.error("Cannot resolve path after RESET?")
                 sys.exit(1)
 
         dfu_capable = iterate_dfu_devices(libusb_ctx, dif)
@@ -935,22 +947,22 @@
     # except usb.core.USBError as e:
     #     logger.error("Cannot set configuration")
     #     sys.exit(1)
 
     logger.info("Claiming USB DFU Interface...")
     try:
         usb.util.claim_interface(dif.dev, dif.interface)
-    except usb.core.USBError as e:
+    except usb.core.USBError:
         logger.error("Cannot claim interface")
         sys.exit(1)
 
     logger.info(f"Setting Alternate Setting {dif.altsetting} ...\n")
     try:
         dif.dev.set_interface_altsetting(dif.interface, dif.altsetting)
-    except usb.core.USBError as e:
+    except usb.core.USBError:
         logger.error("Cannot set alternate interface")
         sys.exit(1)
 
     status = check_status()
     while status.bState != dfu.State.DFU_IDLE:
 
         if status.bState in (dfu.State.APP_IDLE, dfu.State.APP_DETACH):
@@ -963,53 +975,55 @@
                 logger.error("error clear_status")
                 sys.exit(1)
 
             status = check_status()
 
         elif status.bState == (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_UPLOAD_IDLE):
             logger.warning("aborting previous incomplete transfer")
-            if dfu.abort(dif.dev, dif.interface) < 0:
+            # if dfu.abort(dif.dev, dif.interface) < 0:
+            if dif.abort() < 0:
                 logger.error("can't send DFU_ABORT")
                 sys.exit(1)
 
             status = check_status()
 
         elif status.bState == dfu.State.DFU_IDLE:
             logger.info("dfuIDLE, continuing")
             break
 
     if status.bStatus != dfu.Status.OK:
-        logger.warning(f"DFU Status: {dfu.status_to_string(status.bStatus)}")
+        logger.warning(f"DFU Status: {status.bStatus.to_string()}")
         # Clear our status & try again.
         dfu.clear_status(dif.dev, dif.interface)
-        _, status = dfu.get_status(dif.dev, dif.interface)
+        # _ = int(status := dfu.get_status(dif.dev, dif.interface))
+        _ = int(status := dif.get_status())
         if status.bStatus != dfu.Status.OK:
             logger.error(f"{status.bStatus}")
             sys.exit(1)
         if not quirks & QUIRK_POLLTIMEOUT:
             milli_sleep(status.bwPollTimeout)
 
-    logger.debug(f"State: {dfu.state_to_string(status.bState)}, "
-                 f"Status: {dfu.status_to_string(status.bStatus)} Continue...")
+    logger.debug(f"State: {status.bState.to_string()}, "
+                 f"Status: {status.bStatus.to_string()} Continue...")
 
     # Get the DFU mode DFU functional descriptor
     # If it is not found cached, we will request it from the device
 
     ret = get_cached_extra_descriptor(
         dif.dev, dif.configuration, dif.interface,
         USB_DT_DFU, 0, USB_DFU_FUNC_DESCRIPTOR.bcdDFUVersion.build(func_dfu.bcdDFUVersion)
     )
-    ret = IntOrBytes(ret)
+    ret = int_(ret)
 
     if ret < 7:
         logger.error("obtaining cached DFU functional descriptor")
         ret = usb_get_any_descriptor(
             dif.dev, USB_DT_DFU, 0,
             USB_DFU_FUNC_DESCRIPTOR.bcdDFUVersion.build(func_dfu_rt.bcdDFUVersion))
-        ret = IntOrBytes(ret)
+        ret = int_(ret)
 
     if ret == 7:
         logger.info("Deducing device DFU version from functional descriptor length")
         func_dfu.bcdDFUVersion = 0x0100
     elif ret < 9:
         logger.error("Error obtaining DFU functional descriptor")
         logger.info("Please report this as a bug!")
@@ -1053,15 +1067,18 @@
         # open for "exclusive" writing in a portable way
         try:
             with open(file.name, "ab") as file.filep:
                 if os.path.getsize(file.name) != 0:
                     logger.info(f"{file.name}: File exists")
                     sys.exit(1)
 
+
                 if dfuse_device or dfuse_options:
+                    raise NotImplementedError("DfuSe devices aren't support yet")
+
                     if dfuse.do_upload(dif, transfer_size, file, dfuse_options) < 0:
                         sys.exit(1)
                 else:
                     if dfu_load.do_upload(dif, transfer_size, file) < 0:
                         sys.exit(1)
 
         except OSError as e:
@@ -1078,25 +1095,25 @@
 
                 # Parse DFU suffix
                 ret = parse_dfu_suffix(file)
                 if ret < 0:
                     sys.exit(1)
                 elif ret == 0:
                     logger.warning("File has no DFU suffix")
-                elif file.bcdDFU != 0x0100 and file.bcdDFU != 0x011a:
+                elif file.bcdDFU not in (0x0100, 0x011a):
                     logger.error(f"Unsupported DFU file revision 0x{file.bcdDFU:04x}")
                     sys.exit(1)
 
                 # Check vendor ID
-                if file.idVendor != 0xffff and dif.vendor != file.idVendor:
+                if file.idVendor not in (0xffff, dif.vendor):
                     logger.warning(f"Warning: File vendor ID 0x{file.idVendor:04x} "
                                    f"does not match device 0x{dif.vendor:04x}")
 
                 # Check product ID
-                if file.idProduct != 0xffff and dif.product != file.idProduct:
+                if file.idProduct not in (0xffff, dif.product):
                     logger.warning(f"File product ID 0x{file.idProduct:04x} "
                                    f"does not match device 0x{dif.product:04x}")
 
                 # Perform download based on conditions
                 if dfuse_device or dfuse_options or file.bcdDFU == 0x011a:
                     if dfuse.do_dnload(dif, transfer_size, file, dfuse_options) < 0:
                         sys.exit(1)
@@ -1109,22 +1126,23 @@
             sys.exit(1)
 
     else:
         logger.error(f"Unsupported mode: {mode}")
         sys.exit(1)
 
     if final_reset:
-        if IntOrBytes(dfu.detach(dif.dev, dif.interface, 1000)) < 0:
+        # if IntOrBytes(dfu.detach(dif.dev, dif.interface, 1000)) < 0:
+        if int_(dif.detach(1000)) < 0:
             logger.error("can't detach")
         logger.info("Resetting USB to switch back to runtime mode")
         try:
             dif.dev.reset()
         except usb.core.USBError as e:
             logger.error("error resetting after download")
 
     usb.util.release_interface(dif.dev, dif.interface)
     usb.util.dispose_resources(dif.dev)
-    exit(0)
+    sys.exit(0)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil/dfu.py` & `pydfuutil-0.0.2b2/pydfuutil/dfu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 low-level DFU message sending routines (part of dfu-programmer).
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
 
 import inspect
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from enum import IntEnum, IntFlag
 
 import usb.util
-from construct import Byte, Struct, BytesInteger, Container
 
 from pydfuutil.logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class State(IntEnum):
@@ -25,14 +24,20 @@
     DFU_DOWNLOAD_IDLE = 0x05
     DFU_MANIFEST_SYNC = 0x06
     DFU_MANIFEST = 0x07
     DFU_MANIFEST_WAIT_RESET = 0x08
     DFU_UPLOAD_IDLE = 0x09
     DFU_ERROR = 0x0a
 
+    def to_string(self):
+        """
+        :return: State.self name by State Enum
+        """
+        return state_to_string(self)
+
 
 _STATES_NAMES = {
     State.APP_IDLE: 'appIDLE',
     State.APP_DETACH: 'appDETACH',
     State.DFU_IDLE: 'dfuIDLE',
     State.DFU_DOWNLOAD_SYNC: 'dfuDNLOAD-SYNC',
     State.DFU_DOWNLOAD_BUSY: 'dfuDNBUSY',
@@ -60,29 +65,35 @@
     ERROR_FIRMWARE = 0x0a
     ERROR_VENDOR = 0x0b
     ERROR_USBR = 0x0c
     ERROR_POR = 0x0d
     ERROR_UNKNOWN = 0x0e
     ERROR_STALLEDPKT = 0x0f
 
+    def to_string(self):
+        """
+        :return: Status.self name by Status Enum
+        """
+        return status_to_string(self)
+
 
 _DFU_STATUS_NAMES = {
     Status.OK: "No error condition is present",
     Status.ERROR_TARGET: "File is not targeted for use by this device",
     Status.ERROR_FILE: "File is for this device but fails some vendor-specific test",
     Status.ERROR_WRITE: "Device is unable to write memory",
     Status.ERROR_ERASE: "Memory erase function failed",
     Status.ERROR_CHECK_ERASED: "Memory erase check failed",
     Status.ERROR_PROG: "Program memory function failed",
     Status.ERROR_VERIFY: "Programmed memory failed verification",
     Status.ERROR_ADDRESS: "Cannot program memory due to received address that is out of range",
     Status.ERROR_NOTDONE: "Received DNLOAD with wLength = 0, "
-                             "but device does not think that it has all data yet",
+                          "but device does not think that it has all data yet",
     Status.ERROR_FIRMWARE: "Device's firmware is corrupt. "
-                              "It cannot return to run-time (non-DFU) operations",
+                           "It cannot return to run-time (non-DFU) operations",
     Status.ERROR_VENDOR: "iString indicates a vendor specific error",
     Status.ERROR_USBR: "Device detected unexpected USB reset signalling",
     Status.ERROR_POR: "Device detected unexpected power on reset",
     Status.ERROR_UNKNOWN: "Something went wrong, but the device does not know what it was",
     Status.ERROR_STALLEDPKT: "Device stalled an unexpected request"
 
 }
@@ -108,80 +119,112 @@
     IFF_CONFIG = 0x0400
     IFF_IFACE = 0x0800
     IFF_ALT = 0x1000
     IFF_DEVNUM = 0x2000
     IFF_PATH = 0x4000
 
 
-_STATUS = Struct(
-    bStatus=Byte,
-    bwPollTimeout=BytesInteger(3),
-    bState=Byte,
-    iString=Byte
-)
+@dataclass(frozen=True)
+class StatusData:
+    """
+    Converts dfu_get_status result bytes to applicable dataclass
+    """
+    # pylint: disable=invalid-name
+    bStatus: Status = Status.ERROR_UNKNOWN
+    bwPollTimeout: int = 0
+    bState: State = State.DFU_ERROR
+    iString: int = 0
+
+    @classmethod
+    def from_bytes(cls, data: bytes):
+        """Creates StatusData instance from bytes sequence"""
+        if len(data) >= 6:
+            bStatus = (Status(data[0])
+                       if data[0] in Status.__members__.values()
+                       else Status.ERROR_UNKNOWN)
+            bwPollTimeout = int.from_bytes(data[1:4], 'little')
+            bState = (State(data[4])
+                      if data[0] in State.__members__.values()
+                      else State.DFU_ERROR)
+            iString = data[5]
+            return cls(
+                bStatus,
+                bwPollTimeout,
+                bState,
+                iString
+            )
+        return cls()
+
+    def __bytes__(self) -> bytes:
+        return (
+                bytes([self.bStatus.value])
+                + self.bwPollTimeout.to_bytes(3, 'little')
+                + bytes([self.bState.value, self.iString])
+        )
+
+    def __int__(self):
+        return int.from_bytes(self, 'little')
 
 
 @dataclass
 class DfuIf:  # pylint: disable=too-many-instance-attributes
 
-    """DfuIf structure implementation"""
+    """DFU Interface dataclass"""
+    # pylint: disable=invalid-name
 
-    vendor: int = field(default=None, )
-    product: int = field(default=None, )
-    bcdDevice: int = field(default=0, )
-    configuration: int = field(default=0, )
-    interface: int = field(default=0, )
-    altsetting: int = field(default=0, )
-    alt_name: str = field(default="", )
-    bus: int = field(default=0, )
-    devnum: int = field(default=0, )
-    path: [str, int] = field(default="", )
-    flags: [Mode, int] = field(default=0, )
-    count: int = field(default=0, )
-    dev: usb.core.Device = field(default=None)
+    vendor: int = None
+    product: int = None
+    bcdDevice: int = None
+    configuration: int = None
+    interface: int = None
+    altsetting: int = None
+    alt_name: str = None
+    bus: int = None
+    devnum: int = None
+    path: [str, int] = None
+    flags: [Mode, int] = None
+    count: int = None
+    dev: usb.core.Device = None
 
     @property
     def device_ids(self) -> dict:
+        """Returns filter dict for usb.core.find() by VID:PID"""
         id_filter = {}
         if self.vendor:
             id_filter["idVendor"] = self.vendor
         if self.product:
             id_filter["idProduct"] = self.product
         return id_filter
 
-    # __slots__ = (
-    #     'vendor', 'product', 'bcdDevice',
-    #     'configuration', 'interface',
-    #     'altsetting', 'alt_name',
-    #     'bus', 'devnum',
-    #     'path', 'flags', 'count',
-    #     'dev',
-    # )
-
-    # # pylint: disable=too-many-arguments, invalid-name
-    # def __init__(self, vendor: int, product: int, bcdDevice: int,
-    #              configuration: int, interface: int,
-    #              altsetting: int, alt_name: str,
-    #              bus: int, devnum: int,
-    #              path: [str, int], flags: int, count: int,
-    #              dev: usb.core.Device):
-    #
-    #     self.vendor = vendor
-    #     self.product = product
-    #     self.bcdDevice = bcdDevice
-    #     self.configuration = configuration
-    #     self.interface = interface
-    #     self.altsetting = altsetting
-    #     self.alt_name = alt_name  # or Bytes() pointer
-    #     self.bus = bus
-    #     self.devnum = devnum
-    #     self.path = path  # or Bytes() pointer
-    #     self.flags = flags
-    #     self.count = count
-    #     self.dev = dev
+    # The binds to direct dfu functions to get more pythonic
+    # Use them better instead of direct
+
+    def detach(self, timeout: int) -> bytes:
+        """Binds self to dfu.detach()"""
+        return detach(self.dev, self.interface, timeout)
+
+    def download(self, transaction: int, data_or_length: [bytes, int]) -> int:
+        """Binds self to dfu.download()"""
+        return download(self.dev, self.interface, transaction, data_or_length)
+
+    def upload(self, transaction: int, data_or_length: [bytes, int]) -> bytes:
+        """Binds self to dfu.upload()"""
+        return upload(self.dev, self.interface, transaction, data_or_length)
+
+    def abort(self) -> int:
+        """Binds self to dfu.abort()"""
+        return abort(self.dev, self.interface)
+
+    def get_status(self) -> StatusData:
+        """Binds self to dfu.get_status()"""
+        return get_status(self.dev, self.interface)
+
+    def get_state(self) -> State:
+        """Binds self to dfu.get_state()"""
+        return get_state(self.dev, self.interface)
 
 
 def init(timeout: int) -> None:
     """
     Initiate dfu_util library with specified commands timeout
     :param timeout in milliseconds
     :return: None
@@ -203,22 +246,22 @@
     NOTE: (function: typing.Callable) not needed cause python can get it from stack
     :raise ValueError with caller function name
     :return: 0
     """
     caller = inspect.stack()[0][3]
     if INVALID_DFU_TIMEOUT == TIMEOUT:
         if 0 != DEBUG_LEVEL:
-            raise ValueError(f'"{caller}": dfu system not property initialized.')
+            raise ValueError(f'"{caller}": dfu system not initialized properly.')
     return 0
 
 
 def debug(level: int) -> None:
     """
     NOTE: Maybe not needed cause python can define globals after
-    :param level: logging.level
+    :param level: logging level (DEBUG, INFO, WARNING, ERROR)
     """
 
     # pylint: disable=global-statement
     global DEBUG_LEVEL
     DEBUG_LEVEL = level
     logger.setLevel(level)
 
@@ -317,33 +360,33 @@
     :param device: usb.core.Device
     :param interface: usb.core.Interface.bInterfaceNumber
     :param transaction: start page int(total_data_size/xfer_size)
     :param data_or_length: page size bytes(xfer_size) or xfer_size
     :return: uploaded data or error code in bytes
     """
     verify_init()
-    logger.debug('UPLOAD...')
+    logger.debug('DFU_UPLOAD...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.UPLOAD,
         wValue=transaction,
         wIndex=interface,
         data_or_wLength=data_or_length,
         timeout=TIMEOUT,
     )
 
-    logger.debug(f'UPLOAD {len(result) >= 0}')
+    logger.debug(f'DFU_UPLOAD {len(result) >= 0}')
 
     return result.tobytes()
 
 
-def get_status(device: usb.core.Device, interface: int) -> (int, dict):
+def get_status(device: usb.core.Device, interface: int) -> StatusData:
     """
      *  GETSTATUS Request (DFU Spec 1.0, Section 6.1.2)
      *
      *  device    - the usb_dev_handle to communicate with
      *  interface - the interface to communicate with
      *  status    - the data structure to be populated with the results
      *
@@ -353,40 +396,32 @@
     :param device: usb.core.Device
     :param interface: usb.core.Interface.bInterfaceNumber
     :return: error code and _STATUS [Container, dict] object
     """
     verify_init()
     logger.debug('DFU_GET_STATUS...')
 
-    status = Container(
-        bStatus=Status.ERROR_UNKNOWN,
-        bwPollTimeout=0,
-        bState=State.DFU_ERROR,
-        iString=0
-    )
-
     length = 6
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.GETSTATUS,
         wValue=0,
         wIndex=interface,
         data_or_wLength=length,
         timeout=TIMEOUT,
     )
 
-    if len(result) == 6:
-        con = _STATUS.parse(result.tobytes())
-        con.pop('_io')
-        status.update(con)
-    logger.debug(f'DFU_GET_STATUS {len(result) == 6}')
-    logger.debug(f'CURRENT STATE {state_to_string(status.bState)}')
-    return int.from_bytes(result.tobytes(), byteorder='little'), status
+    if len(result) == length:
+        status = StatusData.from_bytes(result.tobytes())
+        logger.debug(f'DFU_GET_STATUS {len(result) == 6}')
+        logger.debug(f'CURRENT STATE {status.bState.to_string()}')
+        return status
+    return StatusData.from_bytes(result)
 
 
 def clear_status(device: usb.core.Device, interface: int) -> int:
     """
      *  CLRSTATUS Request (DFU Spec 1.0, Section 6.1.3)
      *
      *  device    - the usb_dev_handle to communicate with
@@ -413,15 +448,15 @@
         timeout=TIMEOUT,
     )
     logger.debug(f'DFU_CLEAR_STATUS {result >= 0}')
 
     return result
 
 
-def get_state(device: usb.core.Device, interface: int) -> int:
+def get_state(device: usb.core.Device, interface: int) -> State:
     """
      *  GETSTATE Request (DFU Spec 1.0, Section 6.1.5)
      *
      *  device    - the usb_dev_handle to communicate with
      *  interface - the interface to communicate with
      *  length    - the maximum number of bytes to receive from the USB
      *              device - must be less than wTransferSize
@@ -443,18 +478,20 @@
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.GETSTATE,
         wValue=0,
         wIndex=interface,
         data_or_wLength=length,
         timeout=TIMEOUT,
     )
-
-    if result.tobytes()[0] < 1:
+    value = result.tobytes()[0] < 1
+    if value < 1:
         return -1
-    return result.tobytes()[0]
+    if value in State.__members__.values():
+        value = State(value)
+    return value
 
 
 def abort(device: usb.core.Device, interface: int) -> int:
     """
      *  ABORT Request (DFU Spec 1.0, Section 6.1.4)
      *
      *  device    - the usb_dev_handle to communicate with
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil/dfu_file.py` & `pydfuutil-0.0.2b2/pydfuutil/dfu_file.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b1/pydfuutil/dfu_load.py` & `pydfuutil-0.0.2b2/pydfuutil/dfu_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
+import logging
 
 from rich import progress
 
 from pydfuutil import dfu
 from pydfuutil.dfu_file import DFUFile
 from pydfuutil.logger import get_logger
 from pydfuutil.portable import milli_sleep
 from pydfuutil.quirks import QUIRK_POLLTIMEOUT, DEFAULT_POLLTIMEOUT
 
 logger = get_logger(__name__)
 
-VERBOSE: bool = False  # useless?
+# VERBOSE: bool = False  # useless?
 
 _progress_bar = progress.Progress(
     progress.TextColumn("[progress.description]{task.description}"),
     progress.BarColumn(20),
     progress.TaskProgressColumn(),
     progress.TimeRemainingColumn(),
     progress.DownloadColumn(),
@@ -48,20 +49,22 @@
     )
 
     total_bytes = 0
     transaction = dfu.TRANSACTION  # start page
     buf = bytearray(xfer_size)
 
     while True:
-        rc = dfu.upload(
-            device=dif.dev,
-            interface=dif.interface,
-            transaction=transaction,
-            data_or_length=buf
-        )
+        # rc = dfu.upload(
+        #     device=dif.dev,
+        #     interface=dif.interface,
+        #     transaction=transaction,
+        #     data_or_length=buf
+        # )
+
+        rc = dif.upload(transaction, buf)
 
         if len(rc) < 0:
             ret = rc
             break
 
         if file:
             write_rc = file.filep.write(rc)
@@ -82,111 +85,108 @@
         # _progress_bar.update(upload_task, advance=xfer_size)
         _progress_bar.update(upload_task, advance=xfer_size, description='[magenta1]Uploading...')
 
     _progress_bar.update(upload_task, description='[yellow4]Upload finished!')
     _progress_bar.stop()
     _progress_bar.remove_task(upload_task)
 
-    if VERBOSE:
-        logger.info(f"Received a total of {total_bytes} bytes")
+    logger.debug(f"Received a total of {total_bytes} bytes")
     return ret
 
 
-#     download_task = _progress_bar.add_task(
-#         '[magenta1]Starting upload',
-#         total=total_size if total_size >= 0 else None
-#     )
-
-
+# pylint: disable=too-many-branches
 def do_dnload(dif: dfu.DfuIf, xfer_size: int, file: DFUFile, quirks: int, verbose: bool) -> int:
     """
     :param dif: DfuIf instance
     :param xfer_size: transaction size
     :param file: DFUFile instance
     :param quirks: quirks
     :param verbose: is verbose
     :return:
     """
+
+    logger.setLevel(logging.DEBUG if verbose else logging.INFO)
+
     bytes_sent = 0
     buf = bytearray(xfer_size)
 
     bytes_per_hash = (file.size - file.suffixlen) // PROGRESS_BAR_WIDTH
     if bytes_per_hash == 0:
         bytes_per_hash = 1
     logger.info(f"bytes_per_hash={bytes_per_hash}")
 
     logger.info("Copying data from PC to DFU device")
     logger.info("Starting download: ")
     print("[", end="")
 
     try:
         while bytes_sent < file.size - file.suffixlen:
-            # TODO: no idea what's there
+            # FIXME: no idea what's there
             # bytes_left = file.size - file.suffixlen - bytes_sent
             # chunk_size = min(bytes_left, xfer_size)
 
             if (ret := file.filep.readinto(buf)) < 0:  # Handle read error
                 raise IOError(f"Error reading file: {file.name}")
 
-            ret = dfu.download(dif.dev, dif.interface, ret, buf[:ret] if ret else None)
+            # ret = dfu.download(dif.dev, dif.interface, ret, buf[:ret] if ret else None)
+            ret = dif.download(ret, buf[:ret] if ret else None)
 
             if ret < 0:
                 raise IOError("Error during download")
             bytes_sent += ret
 
             while True:
-                ret, status = dfu.get_status(dif.dev, dif.interface)
-                if ret < 0:
+                # if int(status := dfu.get_status(dif.dev, dif.interface)) < 0:
+                if int(status := dif.get_status()) < 0:
                     raise IOError("Error during download get_status")
                 if status.bState in (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_ERROR):
                     break
                 # Wait while the device executes flashing
                 milli_sleep(
                     DEFAULT_POLLTIMEOUT
                     if quirks & QUIRK_POLLTIMEOUT
                     else status.bwPollTimeout
                 )
 
             if status.bStatus != dfu.Status.OK:
                 print(" failed!")
-                print(f"state({status.bState}) = {dfu.state_to_string(status.bState)}, "
-                      f"status({status.bStatus}) = {dfu.status_to_string(status.bStatus)}")
+                print(f"state({status.bState}) = {status.bState.to_string()}, "
+                      f"status({status.bStatus}) = {status.bStatus.to_string()}")
                 raise IOError("Failed")
 
             print("#" * (bytes_sent // bytes_per_hash), end="")
 
         # Send one zero-sized download request to signalize end
-        ret = dfu.download(dif.dev, dif.interface, dfu.TRANSACTION, bytes())
-        if ret < 0:
+        # if dfu.download(dif.dev, dif.interface, dfu.TRANSACTION, bytes()) < 0:
+        if dif.download(dfu.TRANSACTION, bytes()) < 0:
             raise IOError("Error sending completion packet")
 
         print("]")
         logger.info("finished!")
-        if verbose:
-            logger.info(f"Sent a total of {bytes_sent} bytes")
+        logger.debug(f"Sent a total of {bytes_sent} bytes")
 
         # Transition to MANIFEST_SYNC state
-        ret, status = dfu.get_status(dif.dev, dif.interface)
-        if ret < 0:
+        # if int(status := dfu.get_status(dif.dev, dif.interface)) < 0:
+        if int(status := dif.get_status()) < 0:
             raise IOError("Unable to read DFU status")
-        logger.info(f"state({status.bState}) = {dfu.state_to_string(status.bState)}, "
-                    f"status({status.bStatus}) = {dfu.status_to_string(status.bStatus)}")
+        logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
+                    f"status({status.bStatus}) = {status.bStatus.to_string()}")
 
         if not quirks & QUIRK_POLLTIMEOUT:
             milli_sleep(status.bwPollTimeout)
 
         # Deal correctly with ManifestationTolerant=0 / WillDetach bits
-        while status.bState in {dfu.State.DFU_MANIFEST_SYNC, dfu.State.DFU_MANIFEST}:
+        while status.bState in (dfu.State.DFU_MANIFEST_SYNC, dfu.State.DFU_MANIFEST):
             # Some devices need some time before we can obtain the status
             milli_sleep(1000)
-            ret, status = dfu.get_status(dif.dev, dif.interface)
-            if ret < 0:
+            # if int(status := dfu.get_status(dif.dev, dif.interface)) < 0:
+            if int(status := dif.get_status()) < 0:
                 raise IOError("Unable to read DFU status")
-            print(f"state({status.bState}) = {dfu.state_to_string(status.bState)}, "
-                  f"status({status.bStatus}) = {dfu.status_to_string(status.bStatus)}")
+            print(f"state({status.bState}) = {status.bState.to_string()}, "
+                  f"status({status.bStatus}) = {status.bStatus.to_string()}")
 
         if status.bState == dfu.State.DFU_IDLE:
             logger.info("Done!")
 
     except IOError as err:
         logger.error(err)
         return -1
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil/dfuse.py` & `pydfuutil-0.0.2b2/pydfuutil/dfuse.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from pydfuutil import dfu
 from pydfuutil.dfu_file import DFUFile
 from pydfuutil.dfuse_mem import find_segment, DFUSE, parse_memory_layout, free_segment_list
 from pydfuutil.logger import get_logger
 from pydfuutil.portable import milli_sleep
 
 logger = get_logger(__name__)
+logger.warning("Module pydfuutil.dfuse aren't work as expected, "
+               "will reimplemented in future")
 
 VERBOSE = False
 MEM_LAYOUT: list = []
 
 TIMEOUT = 5000
 
 
@@ -75,15 +77,15 @@
     ret: int
     dst: [dict, None]
 
     try:
 
         if command == Command.ERASE_PAGE:
             segment = find_segment(MEM_LAYOUT, address)
-            if not segment or not segment.memtype & DFUSE.ERASABLE:
+            if not segment or not segment.mem_type & DFUSE.ERASABLE:
                 raise IOError(f"Page at 0x{address:08x} cannot be erased")
 
             page_size = segment.pagesize
             if VERBOSE > 1:
                 logger.info(
                     f"Erasing page size {page_size} at address 0x{address:08x}, "
                     f"page starting at 0x{address & ~(page_size - 1):08x}")
@@ -109,15 +111,16 @@
 
         for i in range(0, 4):
             buf[i + 1] = (address >> (8 * i)) & 0xFF
 
         if download(dif, length, buf, 0) < 0:
             raise IOError("Error during special command download")
 
-        ret, dst = dfu.get_status(dif.dev, dif.interface)
+        # ret = int(dst := dfu.get_status(dif.dev, dif.interface))
+        ret = int(dst := dif.get_status())
         if ret < 0:
             raise IOError("Error during special command get_status")
 
         if dst.bState != dfu.State.DFU_DOWNLOAD_BUSY:
             raise IOError("Wrong state after command download")
 
         # Wait while command is executed
@@ -125,30 +128,33 @@
             logger.info(f"Poll timeout {dst.bwPollTimeout} ms")
 
         milli_sleep(dst.bwPollTimeout)
 
         if command == Command.READ_UNPROTECT:
             return ret
 
-        ret, dst = dfu.get_status(dif.dev, dif.interface)
+        # ret = int(dst := dfu.get_status(dif.dev, dif.interface))
+        ret = int(dst := dif.get_status())
         if ret < 0:
             logger.error(
-                f"state({dst.bState}) = {dfu.state_to_string(dst.bState)}, "
-                f"status({dst.bStatus}) = {dfu.status_to_string(dst.bStatus)}")
+                f"state({dst.bState}) = {dst.bState.to_string()}, "
+                f"status({dst.bStatus}) = {dst.bStatus.to_string()}")
             raise IOError("Error during second get_status")
 
         if dst.bStatus != dfu.Status.OK:
             raise IOError("Command not correctly executed")
 
         milli_sleep(dst.bwPollTimeout)
 
-        if dfu.abort(dif.dev, dif.interface) < 0:
+        # if dfu.abort(dif.dev, dif.interface) < 0:
+        if dif.abort() < 0:
             raise IOError("Error sending dfu abort request")
 
-        ret, dst = dfu.get_status(dif.dev, dif.interface)
+        # ret = int(dst := dfu.get_status(dif.dev, dif.interface))
+        ret = int(dst := dif.get_status())
         if ret < 0:
             raise IOError("Error during abort get_status")
 
         if dst.bState != dfu.State.DFU_IDLE:
             raise IOError("Failed to enter idle state on abort")
 
     except (ValueError, IOError) as err:
@@ -243,15 +249,15 @@
         if parsed_args.address:
             # MEM_LAYOUT = parse_memory_layout(dif.alt_name.decode())
             MEM_LAYOUT = parse_memory_layout(dif.alt_name)  # HOTFIX
             if not MEM_LAYOUT:
                 raise IOError("Failed to parse memory layout")
 
             segment = find_segment(MEM_LAYOUT, parsed_args.address)
-            if not parsed_args.force and (not segment or not segment.memtype & DFUSE.READABLE):
+            if not parsed_args.force and (not segment or not segment.mem_type & DFUSE.READABLE):
                 raise IOError(f"Page at 0x{parsed_args.address:08x} is not readable")
 
             if not upload_limit:
                 upload_limit = segment.end - parsed_args.address + 1
                 logger.info(f"Limiting upload to end of memory segment, {upload_limit} bytes")
             special_command(dif, parsed_args.address, Command.SET_ADDRESS)
         else:
@@ -308,15 +314,16 @@
     if ret < 0:
         logger.error("Error during download")
         return ret
 
     bytes_sent = ret
 
     while True:
-        ret, status = dfu.get_status(dif.dev, dif.interface)
+        # ret = int(status := dfu.get_status(dif.dev, dif.interface))
+        ret = int(status := dif.get_status())
         if ret < 0:
             logger.error("Error during download get_status")
             return ret
 
         # dst = ret # useless?
         milli_sleep(status.bwPollTimeout)
 
@@ -327,16 +334,16 @@
 
     if status.bState == dfu.State.DFU_MANIFEST:
         logger.info("Transitioning to dfuMANIFEST state")
 
     if status.bStatus != dfu.Status.OK:
         logger.error("Download failed!")
         logger.error("state(%u) = %s, status(%u) = %s", status.bState,
-                     dfu.state_to_string(status.bState), status.bStatus,
-                     dfu.status_to_string(status.bStatus))
+                     status.bState.to_string(), status.bStatus,
+                     status.bStatus.to_string())
         return -1
 
     return bytes_sent
 
 
 # Writes an element of any size to the device, taking care of page erases
 # returns 0 on success, otherwise -EINVAL
@@ -356,28 +363,28 @@
     :param xfer_size: Transfer size
     :return: 0 if successful, error code otherwise
     """
 
     ret = 0
     segment = find_segment(MEM_LAYOUT, dwElementAddress + dwElementSize - 1)
 
-    if not segment or not segment.memtype & DFUSE.WRITEABLE:
+    if not segment or not segment.mem_type & DFUSE.WRITEABLE:
         logger.error(
             f"Error: Last page at 0x{dwElementAddress + dwElementSize - 1:08x} is not writeable"
         )
         return -1
 
     p = 0
     while p < dwElementSize:
         # page_size = segment.pagesize  # useless?
         address = dwElementAddress + p
         chunk_size = min(xfer_size, dwElementSize - p)
 
         segment = find_segment(MEM_LAYOUT, address)
-        if not segment or not segment.memtype & DFUSE.WRITEABLE:
+        if not segment or not segment.mem_type & DFUSE.WRITEABLE:
             logger.error(f"Error: Page at 0x{address:08x} is not writeable")
             return -1
 
         if VERBOSE:
             logger.info(f"Download from image offset {p:08x} "
                         f"to memory {address:08x}-{address + chunk_size - 1:08x}"
                         f", size {chunk_size}")
@@ -559,14 +566,15 @@
             return -1
         ret = do_dfuse_dnload(dif, xfer_size, file)
 
     free_segment_list(MEM_LAYOUT)
 
     if opts.leave:
         dnload_chunk(dif, b'', 0, 2)  # Zero-size
-        ret2, dst = dfu.get_status(dif.dev, dif.interface)
+        # ret2 = int(dst := dfu.get_status(dif.dev, dif.interface))
+        ret2 = int(dst := dif.get_status())
         if ret2 < 0:
             logger.error("Error during download get_status")
         if VERBOSE:
             logger.info(f"bState = {dst.bState} and bStatus = {dst.bStatus}")
 
     return ret
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil/dfuse_mem.py` & `pydfuutil-0.0.2b2/pydfuutil/dfuse_mem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,232 @@
 """
 Helper functions for reading the memory map in a device
 following the ST DfuSe 1.1a specification.
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
-
+import logging
 import re
 from dataclasses import dataclass, field
 from enum import IntFlag
-
-from construct import Struct, Int
+from typing import Iterator
 
 from pydfuutil.logger import get_logger
 
 logger = get_logger("dfuse_mem")
 
 
 class DFUSE(IntFlag):
     """DFUSE read/write flags"""
     READABLE = 0x1
     ERASABLE = 0x2
     WRITEABLE = 0x4
 
 
-memsegment = Struct(
-    start=Int,
-    end=Int,
-    pagesize=Int,
-    memtype=Int,
-)
-
-
 @dataclass
 class MemSegment:
     """Memory segment"""
 
-    start: int
-    end: int
-    pagesize: int
-    memtype: int
+    start: int = 0
+    end: int = 0
+    pagesize: int = 0
+    mem_type: int = 0
     next: 'MemSegment' = field(default=None)
 
-    def __bytes__(self):
-        return memsegment.build(self.__dict__)
+    @classmethod
+    def from_bytes(cls, data: bytes) -> 'MemSegment':
+        """
+        Create a MemSegment stack from binary data
+        :param data:
+        :return MemSegment:
+        """
+        return cls(
+            *data[:4],
+            next=MemSegment.from_bytes(data[4:])
+            if len(data) > 4 else None
+        )
+
+    def __iter__(self) -> Iterator['MemSegment']:
+        current = self
+        while current is not None:
+            yield current
+            current = current.next
+
+    def __next__(self):
+        if self.next is not None:
+            return self.next
+        raise StopIteration
+
+    def __len__(self):
+        ret = 1
+        if self.next is not None:
+            ret += self.next.__len__()
+        return ret
+
+    def __bytes__(self) -> bytes:
+        data = bytes((
+            self.start,
+            self.end,
+            self.pagesize,
+            self.mem_type
+        ))
+        if self.next:
+            data += self.next.__bytes__()
+        return data
+
+    def append(self, segment: 'MemSegment') -> None:
+        """
+        Append the other segment to the stack
+        :param segment: MemSegment
+        """
+        new_segment = MemSegment(
+            segment.start,
+            segment.end,
+            segment.pagesize,
+            segment.mem_type
+        )
+        if not self.next:
+            self.next = new_segment
+        else:
+            self.next.append(new_segment)
+
+    def find(self, address: int) -> ['MemSegment', None]:
+        """
+        Find a memory segment in the list containing the given element.
+        :param address: MemSegment address for in the stack.
+        """
+        if self.start <= address <= self.end:
+            return self
+        if self.next is not None:
+            return self.next.find(address)
+        return None
+
+    def free(self) -> None:
+        """Useless cause of garbage collector"""
+        raise NotImplementedError("Useless cause of garbage collector")
 
 
-def add_segment(segment_list: list[MemSegment], segment: MemSegment) -> int:
+def add_segment(seqment_sequence: [MemSegment, None], segment: MemSegment) -> MemSegment:
     """
-    :param segment_list:
+    :param seqment_sequence:
     :param segment:
     :return: 0 if ok
     """
-    # raise NotImplementedError("Feature not yet implemented")
-    new_element = MemSegment(segment.start, segment.end, segment.pagesize, segment.memtype)
+    new_element = MemSegment(segment.start, segment.end, segment.pagesize, segment.mem_type)
 
-    if not segment_list:
+    if not seqment_sequence:
         # list can be empty on the first call
-        segment_list.append(new_element)
-    else:
-        # find the last element in the list
-        next_element = segment_list[0]
-        while next_element.next:
-            next_element = next_element.next
-        next_element.next = new_element
+        return new_element
 
-    return 0
+    # find the last element in the list
+    seqment_sequence.append(new_element)
+    return seqment_sequence
 
 
-def find_segment(elements: list[memsegment], new_element: memsegment) -> memsegment:
+def find_segment(segment_stack: MemSegment, address: int) -> [MemSegment, None]:
     """
     Find a memory segment in the list containing the given element.
 
-    :param elements: List of MemSegment instances.
-    :param new_element: MemSegment instance to search for in the list.
+    :param segment_stack: List of MemSegment instances.
+    :param address: MemSegment address for in the stack.
     :return: MemSegment instance if found, None otherwise.
     """
-    for element in elements:
-        if element.start == new_element.start and element.end == new_element.end:
-            return element
-    return None
+    return segment_stack.find(address)
 
 
-def free_segment_list(elements: list[memsegment]) -> None:
+def free_segment_list(segment_stack: MemSegment) -> None:
     """
     Free the memory allocated for the list of memory segments.
-
-    :param elements: List of MemSegment instances.
+    :param segment_stack: List of MemSegment instances.
     """
-    del elements[:]
+    del segment_stack
 
 
 # Parse memory map from interface descriptor string
 # encoded as per ST document UM0424 section 4.3.2.
 
-def parse_memory_layout(intf_desc: [str, bytes], verbose: bool = False) -> memsegment:
+def parse_memory_layout(intf_desc: [str, bytes], verbose: bool = False) -> [MemSegment, None]:
     """
     Parse memory map from interface descriptor string
     encoded as per ST document UM0424 section 4.3.2.
     :param intf_desc:
     :param verbose:
     :return: MemSegment instance
     """
 
-    segment_list = []
-    count = 0
-
-    while intf_desc:
-        # Read name
-        match = re.match(r"^([^/]+)/", intf_desc)
-        if match is None:
-            logger.error("Error: Could not read name.")
-            return None
+    logger.setLevel(logging.DEBUG if verbose else logging.INFO)
 
-        name = match.group(1)
-        intf_desc = intf_desc[match.end():]
+    if isinstance(intf_desc, bytes):
+        intf_desc = intf_desc.decode('ascii')
 
-        if verbose:
-            logger.info(f"DfuSe interface name: \"{name}\"")
+    count: int = 0
+    segment_list: [MemSegment, None] = None
+    address: [int, None] = None
+
+    match = re.match(r'@([^/]+)', intf_desc)
+    if match is None:
+        logger.error(f"Could not read name, name={match}")
+        return None
+    name = match.group(1)
+    logger.info(f"DfuSe interface name: {name}")
 
-        # Read address
-        match = re.match(r"^0x([\da-fA-F]+)/", intf_desc)
-        if match is None:
-            logger.error("Error: Could not read address.")
-            return None
+    intf_desc = intf_desc[match.end():]
 
+    # while per segment
+    while (match := re.match(r'/0x(\d+)/', intf_desc)) is not None:
         address = int(match.group(1), 16)
+
         intf_desc = intf_desc[match.end():]
 
-        while True:
-            # Initialize variables
-            sectors, size = 0, 0
-
-            # Read segment details
-            match = re.match(r"^(\d+)\*(\d+)([a-zA-Z])?([^/,]+)/", intf_desc)
-            if match is None:
-                break
+        # while per address
+        while (match := re.match(r'(\d+)\*(\d+)(\w)(\w)[,/]?', intf_desc)) is not None:
+            _sectors, _size, multiplier, type_string = match.groups()
+            sectors, size = int(_sectors), int(_size)
+
+            logger.debug(f"{sectors=}, {size=}, {multiplier=}, {type_string=}")
 
             intf_desc = intf_desc[match.end():]
             count += 1
+            mem_type = ord(type_string)
 
-            if match.group(3):
-                memtype = ord(match.group(3))
-            elif match.group(4) and len(match.group(4)) == 1 and match.group(4) != '/':
-                memtype = ord(match.group(4))
-            else:
-                logger.warning(f"Parsing type identifier '{match.group(4)}' "
-                               f"failed for segment {count}")
-                continue
-
-            size_multiplier = match.group(3) if match.group(3) else 'B'
-
-            if size_multiplier == 'K':
+            if multiplier == 'B':
+                pass
+            elif multiplier == 'K':
                 size *= 1024
-            elif size_multiplier == 'M':
+            elif multiplier == 'M':
                 size *= 1024 * 1024
-            elif size_multiplier in {'a', 'b', 'c', 'd', 'e', 'f', 'g'}:
-                if not memtype:
-                    logger.warning(f"Non-valid multiplier '{size_multiplier}', "
-                                   f"interpreted as type identifier instead")
-                    memtype = size_multiplier
+            elif multiplier in ('a', 'b', 'c', 'd', 'e', 'f', 'g'):
+                if not mem_type:
+                    logger.warning(f"Non-valid multiplier {multiplier}, "
+                                   "interpreted as type identifier instead")
+                    mem_type = multiplier
 
-            if not memtype:
+            # fallthrough if memtype was already set
+            else:
+                logger.warning(f"Non-valid multiplier {multiplier} assuming bytes")
+
+            if not mem_type:
                 logger.warning(f"No valid type for segment {count}")
-                continue
 
-            segment_list.append(
+            segment_list = add_segment(
+                segment_list,
                 MemSegment(
-                    start=address,
-                    end=address + sectors * size - 1,
-                    pagesize=size,
-                    memtype=memtype & 7
+                    address,
+                    address + sectors * size - 1,
+                    size,
+                    mem_type & 7
                 )
             )
 
-            if verbose:
-                logger.info(f"Memory segment at "
-                            f"0x{address:08x} {sectors} x {size} = {sectors * size} "
-                            f"({'r' if memtype & DFUSE.READABLE else ''}"
-                            f"{'e' if memtype & DFUSE.ERASABLE else ''}"
-                            f"{'w' if memtype & DFUSE.WRITEABLE else ''})")
+            logger.debug(f"Memory segment at "
+                         f"0x{address:08x} {sectors} x {size} = {sectors * size} "
+                         f"({'r' if mem_type & DFUSE.READABLE else ''}"
+                         f"{'e' if mem_type & DFUSE.ERASABLE else ''}"
+                         f"{'w' if mem_type & DFUSE.WRITEABLE else ''})")
 
             address += sectors * size
 
-            separator = intf_desc[0]
-            if separator == ',':
-                intf_desc = intf_desc[1:]
-            else:
-                break
+        logger.debug(f"Parsed details of {count} segments")
+
+    if address is None:
+        logger.error(f"Could not read address, {address=}")
 
     return segment_list
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil/lmdfu.py` & `pydfuutil-0.0.2b2/pydfuutil/lmdfu.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     :return: 0 if not a valid prefix, 1 if a valid prefix, -1 on error.
     """
 
     try:
         logger.info("Check TI Stellaris prefix")
 
         # Allocate buffer for reading the prefix
-        data = bytearray([0] * 16)
+        data = bytearray(16)
 
         # Read prefix from the file
         ret = file.filep.readinto(data)
         if ret < 16:
             logger.error("Error: Could not read prefix")
             return -1
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil/quirks.py` & `pydfuutil-0.0.2b2/pydfuutil/quirks.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b1/pydfuutil/suffix.py` & `pydfuutil-0.0.2b2/pydfuutil/suffix.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,16 +107,18 @@
             logger.error(e)
             sys.exit(1)
     logger.info("New DFU suffix added.")
 
 
 def _get_argparser():
     """Get custom argument parser"""
+
     class CustomHelpFormatter(argparse.HelpFormatter):
         """Custom argument parser formatter"""
+
         def add_argument(self, action):
             if action.dest == 'help':
                 action.help = 'Print this help message'
             super().add_argument(action)
 
     parser = argparse.ArgumentParser(
         prog='dfu-suffix',
@@ -180,48 +182,38 @@
 
 
 def main() -> None:
     """main executable"""
     parser = _get_argparser()
     args = get_args(parser)
 
-    # file = args.check or args.add or args.delete
-    # file_name = file.name
-
     lmdfu_mode = LmdfuMode.NONE
     lmdfu_flash_address: int = 0
     lmdfu_prefix: int = 0
-    # end: str  # unused
 
-    pid: int = 0xffff
-    vid: int = 0xffff
-    did: int = 0xffff
+    empty = 0xffff
 
     file = DFUFile(args.file.name)
     file.filep, mode = args.file, args.mode
 
-    if args.pid:
-        pid = args.pid
-    if args.vid:
-        vid = args.vid
-    if args.did:
-        did = args.did
+    pid = args.pid if args.pid else empty
+    vid = args.vid if args.vid else empty
+    did = args.did if args.did else empty
+
     if args.lmdfu_flash_address:
-        lmdfu_mode = LmdfuMode.ADD
-        lmdfu_flash_address = args.lmdfu_flash_address
+        lmdfu_mode, lmdfu_flash_address = LmdfuMode.ADD, args.lmdfu_flash_address
+
     if args.lmdfu_mode:
         lmdfu_mode = LmdfuMode.CHECK
 
     if mode == Mode.DEL and lmdfu_mode == LmdfuMode.CHECK:
         lmdfu_mode = LmdfuMode.DEL
 
     if mode != Mode.NONE:
         try:
-            # with open(file.name, "r+b") as file.filep:
-
             if mode == Mode.ADD:
 
                 if check_suffix(file):
                     if lmdfu_prefix:
                         lmdfu.check_prefix(file)
                     logger.warning("Please remove existing DFU suffix before adding a new one.")
                     sys.exit(1)
@@ -236,34 +228,32 @@
             elif mode == Mode.CHECK:
                 # FIXME: could open read-only here
                 check_suffix(file)
                 if lmdfu_mode == LmdfuMode.CHECK:
                     lmdfu.check_prefix(file)
 
             elif mode == Mode.DEL:
-                if not remove_suffix(file):
-                    if lmdfu_mode == LmdfuMode.DEL:
-                        if lmdfu.check_prefix(file):
-                            lmdfu.remove_prefix(file)
-                            sys.exit(1)
+                if (not remove_suffix(file)
+                        and lmdfu_mode == LmdfuMode.DEL
+                        and lmdfu.check_prefix(file)):
+                    lmdfu.remove_prefix(file)
+                    sys.exit(1)
 
             else:
                 parser.print_help()
                 sys.exit(2)
 
-            if lmdfu_mode == LmdfuMode.DEL:
-                if check_suffix(file):
-                    logger.warning(
-                        "DFU suffix exist."
-                        " Remove suffix before using -T or use it with -D to delete suffix"
-                    )
-                    sys.exit(1)
-                else:
-                    if lmdfu.check_prefix(file):
-                        lmdfu.remove_prefix(file)
+            if lmdfu_mode == LmdfuMode.DEL and check_suffix(file):
+                logger.warning(
+                    "DFU suffix exist. "
+                    "Remove suffix before using -T or use it with -D to delete suffix")
+                sys.exit(1)
+
+            if lmdfu_mode == LmdfuMode.DEL and lmdfu.check_prefix(file):
+                lmdfu.remove_prefix(file)
 
         except Exception as error:
             logger.error(error)
             sys.exit(1)
 
     sys.exit(0)
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil/usb_dfu.py` & `pydfuutil-0.0.2b2/pydfuutil/usb_dfu.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,36 +7,29 @@
 https://www.usb.org/developers/devclass_docs/usbdfu10.pdf
 """
 
 from enum import IntEnum
 
 import usb.util
 from construct import Int8ul, Struct, Int16ul
-# from construct import FlagsEnum, Byte
+
 
 USB_DT_DFU = 0x21
 
 class bmAttributes(IntEnum):
+    """Enum of DFU_FUNC_DESCRIPTOR's bmAttributes"""
     USB_DFU_CAN_DOWNLOAD = 0x1
     USB_DFU_CAN_UPLOAD = 0x2
     USB_DFU_MANIFEST_TOL = 0x3
     USB_DFU_WILL_DETACH = 0x4
 
-# bmAttributes = FlagsEnum(
-#     Byte,
-#     USB_DFU_CAN_DOWNLOAD=0x1,  # is support updates
-#     USB_DFU_CAN_UPLOAD=0x2,  # is prog warranty ok
-#     USB_DFU_MANIFEST_TOL=0x4,
-#     USB_DFU_WILL_DETACH=0x8,
-# )
 
 USB_DFU_FUNC_DESCRIPTOR = Struct(
     bLength=Int8ul,
     bDescriptorType=Int8ul,
-    # bmAttributes=bmAttributes,
     bmAttributes=Int8ul,
     wDetachTimeOut=Int16ul,
     wTransferSize=Int16ul,
     bcdDFUVersion=Int16ul,
 )
 
 USB_DT_DFU_SIZE = 9
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil.egg-info/PKG-INFO` & `pydfuutil-0.0.2b2/pydfuutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.2b1
+Version: 0.0.2b2
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -187,16 +187,19 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyusb
 Requires-Dist: libusb-package
 Requires-Dist: rich
 Requires-Dist: construct
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pylint; extra == "test"
 
 # PyDfuUtil - Pure python fork of **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)** wrappers to **[libusb](https://github.com/libusb/libusb)**
 
 [![PyPI Version](https://img.shields.io/pypi/v/pydfuutil?label=PyPI&logo=pypi)](https://pypi.org/project/pydfuutil/)
 
 ## Table of contents
 * **[Introduction](#introduction)**
@@ -245,41 +248,42 @@
 ### dfu-util
 ```Bash
 pydfuutil -h 
 # or
 python -m pydfuutil -h
 
 ####### usage:
-usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d VID:PID] [-p BUS-PORT] [-c CONFIG_NR] [-i INTF_NR] [-a ALT] [-t SIZE] [-U FILE] [-D FILE] [-R] [-s ADDRESS]
+usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d <deviceID>:<productID>] [-p <bus/port>] [-c <config>] [-i <intf_num>] [-a <alt>] [-t <size>] [-U <file>] [-D <file>] [-R] [-s <address>]
 
 Python implementation of DFU-Util tools
 
 options:
   -h, --help            show this help message and exit
   -V, --version         Print the version number
   -v, --verbose         Print verbose debug statements
   -l, --list            List the currently attached DFU capable USB devices
   -e, --detach          Detach the currently attached DFU capable USB devices
-  -d VID:PID, --device VID:PID
+  -d <deviceID>:<productID>, --device <deviceID>:<productID>
                         Specify Vendor/Product ID of DFU device
-  -p BUS-PORT, --path BUS-PORT
+  -p <bus/port>, --path <bus/port>
                         Specify path to DFU device
-  -c CONFIG_NR, --cfg CONFIG_NR
+  -c <config>, --cfg <config>
                         Specify the Configuration of DFU device
-  -i INTF_NR, --intf INTF_NR
+  -i <interface>, --intf <interface>
                         Specify the DFU Interface number
-  -a ALT, --alt ALT     Specify the Altsetting of the DFU Interface
-  -t SIZE, --transfer-size SIZE
+  -a <alt>, --alt <alt>
+                        Specify the Altsetting of the DFU Interface
+  -t <size>, --transfer-size <size>
                         Specify the number of bytes per USB Transfer
-  -U FILE, --upload FILE
+  -U <file>, --upload <file>
                         Read firmware from device into <file>
-  -D FILE, --download FILE
+  -D <file>, --download <file>
                         Write firmware from <file> into device
   -R, --reset           Issue USB Reset signalling once we`re finished
-  -s ADDRESS, --dfuse-address ADDRESS
+  -s <address>, --dfuse-address <address>
                         ST DfuSe mode, specify target address for raw file download or upload. Not applicable for DfuSe file (.dfu) downloads
 ```
 
 ### dfu-suffix
 ```Bash
 pydfuutil-suffix -h
 # or 
@@ -305,62 +309,26 @@
                         Add device ID into DFU suffix in <file>
   -s <address>, --stellaris-address <address>
                         Specify lmdfu address for LMDFU_ADD
   -T, --stellaris       Set lmdfu mode to LMDFU_CHECK
 
 ```
 
-
-## Todos
-
-#### Modules to implement:
-
-- [ ] main
-  - [x] atoi()
-  - [ ] usb_path2devnum()
-  - [x] find_dfu_if()
-  - [x] _get_first_cb()
-  - [x] _get_first_dfu_if()
-  - [x] _check_match_cb()
-  - [x] get_matching_dfu_if()
-  - [x] _count_match_cb()
-  - [x] count_matching_dfu_if()
-  - [x] get_alt_name()
-  - [x] print_dfu_if()
-  - [x] list_dfu_interfaces()
-  - [x] alt_by_name()
-  - [x] _count_cb()
-  - [x] count_dfu_interfaces()
-  - [x] iterate_dfu_devices()
-  - [x] found_dfu_device()
-  - [x] get_first_dfu_device()
-  - [x] count_one_dfu_device()
-  - [x] count_dfu_devices()
-  - [x] parse_vendprod()
-  - [ ] resolve_device_path()
-  - [x] find_descriptor()
-  - [ ] usb_get_any_descriptor()
-  - [x] get_cached_extra_descriptor()
-  - [x] help_()
-  - [x] print_version()
-  - [ ] main()
-- [ ] dfu_load.PROGRESS_BAR -> rich.Progress
-
-
 #### Done:
 - [x] dfu
 - [x] dfu_file
 - [x] dfu_load
 - [x] portable
 - [x] quirks
-- [x] suffix
+- [x] suffix + cli entry point
 - [x] usb_dfu
 - [x] lmdfu
 - [x] dfuse_mem
-- [x] dfuse
+- [ ] dfuse (not fully supported yet)
+- [ ] dfu-util cli entry point (not fully supported yet)
 
 
 ## Getting help
 * To report a bug or propose a new feature, use our issue tracker. But please search the database before opening a new issue.
 
 ## About
 Dfu-util - Device Firmware Upgrade Utilities
```

### Comparing `pydfuutil-0.0.2b1/pydfuutil.egg-info/SOURCES.txt` & `pydfuutil-0.0.2b2/pydfuutil.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,9 +19,13 @@
 pydfuutil/usb_dfu.py
 pydfuutil.egg-info/PKG-INFO
 pydfuutil.egg-info/SOURCES.txt
 pydfuutil.egg-info/dependency_links.txt
 pydfuutil.egg-info/entry_points.txt
 pydfuutil.egg-info/requires.txt
 pydfuutil.egg-info/top_level.txt
+tests/test_dfu.py
 tests/test_dfu_file.py
-tests/test_dfu_load.py
+tests/test_dfu_load.py
+tests/test_dfuse_mem.py
+tests/test_lmdfu.py
+tests/test_quirks.py
```

### Comparing `pydfuutil-0.0.2b1/pyproject.toml` & `pydfuutil-0.0.2b2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = ['pyusb', 'libusb-package', 'rich', 'construct']
+
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/o-murphy/pydfuutil"
 "Bug Reports" = "https://github.com/o-murphy/pydfuutil/issues"
 "Source" = "https://github.com/o-murphy/pydfuutil"
 
@@ -49,12 +50,18 @@
 
 
 [tool.setuptools.dynamic]
 version = {attr = "pydfuutil.__version__"}
 
 
 [project.optional-dependencies]
-dev = ['build']
+build = [
+    "build"
+]
+test = [
+    "pytest",
+    "pylint",
+]
 
 [project.scripts]
 pydfuutil = "pydfuutil.__main__:main"
 pydfuutil-suffix = "pydfuutil.suffix:main"
```

### Comparing `pydfuutil-0.0.2b1/tests/test_dfu_file.py` & `pydfuutil-0.0.2b2/tests/test_dfu_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os.path
 import unittest
 
 from pydfuutil.dfu_file import *
 from pydfuutil.dfu_file import crc32_byte
 
 
 class TestDFUFile(unittest.TestCase):
@@ -25,16 +26,16 @@
          0x00, /* dwCRC --- */
          0x00 /* dwCRC msb */
         };
     """
 
     def setUp(self):
         # You may need to adjust these paths based on your actual implementation
-        self.sample_file_path = "sample_file.bin"
-        self.output_file_path = "output_file.bin"
+        self.sample_file_path = os.path.join(os.path.dirname(__file__), "sample_file.bin")
+        self.output_file_path = os.path.join(os.path.dirname(__file__), "output_file.bin")
 
     def test_crc32_byte(self):
         # You may need to adjust the expected result based on your specific CRC calculation
         result = crc32_byte(0, 0)
         self.assertEqual(result, 0x0)
 
     def test_parse_dfu_suffix(self):
```

