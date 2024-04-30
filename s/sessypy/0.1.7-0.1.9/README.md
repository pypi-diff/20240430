# Comparing `tmp/sessypy-0.1.7.tar.gz` & `tmp/sessypy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessypy-0.1.7.tar", last modified: Fri Feb  2 20:10:32 2024, max compression
+gzip compressed data, was "sessypy-0.1.9.tar", last modified: Sun Mar 31 21:44:04 2024, max compression
```

## Comparing `sessypy-0.1.7.tar` & `sessypy-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:10:32.121472 sessypy-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-02-02 20:10:21.000000 sessypy-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41305 2024-02-02 20:10:32.121472 sessypy-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-02 20:10:21.000000 sessypy-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-02 20:10:21.000000 sessypy-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-02 20:10:32.121472 sessypy-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:10:32.117472 sessypy-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:10:32.121472 sessypy-0.1.7/src/sessypy/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-02 20:10:21.000000 sessypy-0.1.7/src/sessypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-02 20:10:21.000000 sessypy-0.1.7/src/sessypy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-02-02 20:10:21.000000 sessypy-0.1.7/src/sessypy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-02-02 20:10:21.000000 sessypy-0.1.7/src/sessypy/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-02 20:10:21.000000 sessypy-0.1.7/src/sessypy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:10:32.121472 sessypy-0.1.7/src/sessypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41305 2024-02-02 20:10:32.000000 sessypy-0.1.7/src/sessypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-02 20:10:32.000000 sessypy-0.1.7/src/sessypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 20:10:32.000000 sessypy-0.1.7/src/sessypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-02 20:10:32.000000 sessypy-0.1.7/src/sessypy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:44:04.860221 sessypy-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-31 21:44:00.000000 sessypy-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41481 2024-03-31 21:44:04.860221 sessypy-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-31 21:44:00.000000 sessypy-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 21:44:00.000000 sessypy-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-31 21:44:04.860221 sessypy-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:44:04.856221 sessypy-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:44:04.860221 sessypy-0.1.9/src/sessypy/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-31 21:44:00.000000 sessypy-0.1.9/src/sessypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-31 21:44:00.000000 sessypy-0.1.9/src/sessypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-31 21:44:00.000000 sessypy-0.1.9/src/sessypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-03-31 21:44:00.000000 sessypy-0.1.9/src/sessypy/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-31 21:44:00.000000 sessypy-0.1.9/src/sessypy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:44:04.860221 sessypy-0.1.9/src/sessypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41481 2024-03-31 21:44:04.000000 sessypy-0.1.9/src/sessypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-31 21:44:04.000000 sessypy-0.1.9/src/sessypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 21:44:04.000000 sessypy-0.1.9/src/sessypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 21:44:04.000000 sessypy-0.1.9/src/sessypy.egg-info/top_level.txt
```

### Comparing `sessypy-0.1.7/LICENSE` & `sessypy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sessypy-0.1.7/PKG-INFO` & `sessypy-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.1.7
+Version: 0.1.9
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,14 +682,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SessyPy
 A python wrapper for Sessy's local REST api.
 
 [![PyPI Build & Publish](https://github.com/PimDoos/sessypy/actions/workflows/python-publish.yml/badge.svg)](https://github.com/PimDoos/sessypy/actions/workflows/python-publish.yml)
+[![Python package](https://github.com/PimDoos/sessypy/actions/workflows/python-package.yml/badge.svg)](https://github.com/PimDoos/sessypy/actions/workflows/python-package.yml)
 
 Installation
 ============
 
 Automatic installation
 ----------------------
 Install the package via PyPI:
```

### Comparing `sessypy-0.1.7/src/sessypy/api.py` & `sessypy-0.1.9/src/sessypy/api.py`

 * *Files identical despite different names*

### Comparing `sessypy-0.1.7/src/sessypy/const.py` & `sessypy-0.1.9/src/sessypy/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from enum import Enum
 
 API_VERSION_1 = "api/v1"
 API_VERSION_2 = "api/v2"
 
 class SessyApiCommand(str, Enum):
     CT_DETAILS = f"{API_VERSION_1}/ct/details"
+    DYNAMIC_SCHEDULE = f"{API_VERSION_1}/dynamic/schedule"
+
     METER_GRID_TARGET = f"{API_VERSION_1}/meter/grid_target"
     
     NETWORK_SCAN = f"{API_VERSION_1}/network/scan"
     NETWORK_STATUS = f"{API_VERSION_1}/network/status"
     OTA_CHECK = f"{API_VERSION_1}/ota/check"
     OTA_START = f"{API_VERSION_1}/ota/start"
     OTA_STATUS = f"{API_VERSION_1}/ota/status"
```

### Comparing `sessypy-0.1.7/src/sessypy/devices.py` & `sessypy-0.1.9/src/sessypy/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     async def set_wifi_credentials(self, ssid: str, password: str):
         return await self.api.post(SessyApiCommand.WIFI_STA_CREDENTIALS, {"ssid":ssid, "pass":password})
 
     async def close(self):
         await self.api.close()
     
 class SessyBattery(SessyDevice):
+    async def get_dynamic_schedule(self):
+        return await self.api.get(SessyApiCommand.DYNAMIC_SCHEDULE)
+    
     async def get_power_status(self):
         return await self.api.get(SessyApiCommand.POWER_STATUS)
     
     async def set_power_setpoint(self, setpoint: int):
         return await self.api.post(SessyApiCommand.POWER_SETPOINT, {"setpoint": setpoint})
     
     async def get_power_strategy(self):
```

### Comparing `sessypy-0.1.7/src/sessypy.egg-info/PKG-INFO` & `sessypy-0.1.9/src/sessypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.1.7
+Version: 0.1.9
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,14 +682,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SessyPy
 A python wrapper for Sessy's local REST api.
 
 [![PyPI Build & Publish](https://github.com/PimDoos/sessypy/actions/workflows/python-publish.yml/badge.svg)](https://github.com/PimDoos/sessypy/actions/workflows/python-publish.yml)
+[![Python package](https://github.com/PimDoos/sessypy/actions/workflows/python-package.yml/badge.svg)](https://github.com/PimDoos/sessypy/actions/workflows/python-package.yml)
 
 Installation
 ============
 
 Automatic installation
 ----------------------
 Install the package via PyPI:
```

