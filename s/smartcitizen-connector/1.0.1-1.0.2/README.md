# Comparing `tmp/smartcitizen_connector-1.0.1.tar.gz` & `tmp/smartcitizen_connector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartcitizen_connector-1.0.1.tar", last modified: Wed Apr 24 08:53:22 2024, max compression
+gzip compressed data, was "smartcitizen_connector-1.0.2.tar", last modified: Tue Apr 30 09:13:27 2024, max compression
```

## Comparing `smartcitizen_connector-1.0.1.tar` & `smartcitizen_connector-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.246019 smartcitizen_connector-1.0.1/smartcitizen_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/_config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/_config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/device/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/device/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/measurement/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/measurement/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/models/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/search/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.787064 smartcitizen_connector-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-30 09:13:27.787064 smartcitizen_connector-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 09:13:27.787064 smartcitizen_connector-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.783064 smartcitizen_connector-1.0.2/smartcitizen_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.783064 smartcitizen_connector-1.0.2/smartcitizen_connector/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.783064 smartcitizen_connector-1.0.2/smartcitizen_connector/device/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.783064 smartcitizen_connector-1.0.2/smartcitizen_connector/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/measurement/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.787064 smartcitizen_connector-1.0.2/smartcitizen_connector/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.787064 smartcitizen_connector-1.0.2/smartcitizen_connector/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.787064 smartcitizen_connector-1.0.2/smartcitizen_connector/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.787064 smartcitizen_connector-1.0.2/smartcitizen_connector/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-30 09:13:22.000000 smartcitizen_connector-1.0.2/smartcitizen_connector/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:13:27.787064 smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-30 09:13:27.000000 smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 09:13:27.000000 smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:13:27.000000 smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:13:27.000000 smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 09:13:27.000000 smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 09:13:27.000000 smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/top_level.txt
```

### Comparing `smartcitizen_connector-1.0.1/LICENSE` & `smartcitizen_connector-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.1/PKG-INFO` & `smartcitizen_connector-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen_connector-1.0.1/README.md` & `smartcitizen_connector-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.1/setup.py` & `smartcitizen_connector-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 PROJECT_URLS = {
     "Documentation": "https://docs.smartcitizen.me/",
     "Source Code": "https://github.com/fablabbcn/smartcitizen-connector",
 }
 
 setup(
     name="smartcitizen-connector",
-    version="1.0.1",
+    version="1.0.2",
     description="Python connector to download information collected in SmartCitizen API",
     author="oscgonfer",
     license="GNU General Public License v3",
     keywords=['sensors', 'Smart Citizen'],
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/fablabbcn/smartcitizen-connector",
```

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector/_config/config.py` & `smartcitizen_connector-1.0.2/smartcitizen_connector/_config/config.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector/device/device.py` & `smartcitizen_connector-1.0.2/smartcitizen_connector/device/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,22 @@
     else:
         _hardware_url = ''
 
     return _hardware_url, _hardware_postprocessing, _ok
 
 class SCDevice:
 
-    def __init__(self, id, check_postprocessing=True):
-        self.id = id
+    def __init__(self, id = None, params = None, check_postprocessing=True):
+        if id is not None:
+            self.id = id
+        elif params is not None:
+            self.id = params.id
+        else:
+            raise ValueError("Need at least id or params.id")
+        self.params = params
         self.url = f'{config.DEVICES_URL}{self.id}'
         self.page = f'{config.FRONTEND_URL}{self.id}'
         self.method = 'async'
         self.data = DataFrame()
         self._metrics: List[Metric] = []
         self.__load__()
         self.__get_timezone__()
@@ -569,18 +575,21 @@
     def postprocessing(self):
         if self.json.postprocessing is None:
             return None
         return self.json.postprocessing.model_dump()
 
     @property
     def latest_postprocessing(self):
-        return self.json.postprocessing.latest_postprocessing
+        if self.json.postprocessing is not None:
+            return self.json.postprocessing.latest_postprocessing
+        else:
+            return None
 
     def update_latest_postprocessing(self, date):
-        if self.json.postprocessing.id is not None:
+        if self.json.postprocessing is not None:
             # Add latest postprocessing rounded up with
             # frequency so that we don't end up in
             # and endless loop processing only the latest data line
             # (minute vs. second precission of the data)
             try:
                 self.json.postprocessing.latest_postprocessing = date.to_pydatetime()
             except:
```

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector/measurement/measurement.py` & `smartcitizen_connector-1.0.2/smartcitizen_connector/measurement/measurement.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector/models/models.py` & `smartcitizen_connector-1.0.2/smartcitizen_connector/models/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Optional, List
+from typing import Optional, List, Dict
 from pydantic import BaseModel
 
 class Measurement(BaseModel):
     id: int
     name: str
     description: str
 
@@ -75,22 +75,22 @@
 class HardwarePostprocessing(BaseModel):
     blueprint_url: Optional[str] = None
     description: Optional[str] = None
     versions: Optional[List[HardwareVersion]] = None
     forwarding: Optional[str] = None
 
 class Postprocessing(BaseModel):
-    id: int
+    id: Optional[int] = None
     blueprint_url: Optional[str] = None
     hardware_url: Optional[str] = None
     forwarding_params: Optional[int] = None
     meta: Optional[str] = None
     latest_postprocessing: Optional[datetime] = None
-    created_at: datetime
-    updated_at: datetime
+    created_at: Optional[datetime] = None
+    updated_at: Optional[datetime] = None
 
 class Data(BaseModel):
     sensors: Optional[List[Sensor]] = None
 
 class Notifications(BaseModel):
     low_battery: bool
     stopped_publishing: bool
```

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector/search/search.py` & `smartcitizen_connector-1.0.2/smartcitizen_connector/search/search.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector/sensor/sensor.py` & `smartcitizen_connector-1.0.2/smartcitizen_connector/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector/tools/tools.py` & `smartcitizen_connector-1.0.2/smartcitizen_connector/tools/tools.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/PKG-INFO` & `smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/SOURCES.txt` & `smartcitizen_connector-1.0.2/smartcitizen_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

