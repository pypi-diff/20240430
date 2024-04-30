# Comparing `tmp/iqrfpy_app_helpers-0.1.0.dev1.tar.gz` & `tmp/iqrfpy_app_helpers-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqrfpy_app_helpers-0.1.0.dev1.tar", last modified: Mon Apr 22 10:53:23 2024, max compression
+gzip compressed data, was "iqrfpy_app_helpers-0.1.0.dev2.tar", last modified: Tue Apr 23 09:49:03 2024, max compression
```

## Comparing `iqrfpy_app_helpers-0.1.0.dev1.tar` & `iqrfpy_app_helpers-0.1.0.dev2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-22 10:53:23.391307 iqrfpy_app_helpers-0.1.0.dev1/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2024-04-22 05:15:39.000000 iqrfpy_app_helpers-0.1.0.dev1/LICENSE
--rw-r--r--   0 khanak    (1000) khanak    (1000)     1963 2024-04-22 10:53:23.391307 iqrfpy_app_helpers-0.1.0.dev1/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      607 2024-04-22 05:32:13.000000 iqrfpy_app_helpers-0.1.0.dev1/README.md
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-22 10:53:23.391307 iqrfpy_app_helpers-0.1.0.dev1/app_helpers/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      734 2024-04-22 10:38:27.000000 iqrfpy_app_helpers-0.1.0.dev1/app_helpers/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3829 2024-04-22 10:15:40.000000 iqrfpy_app_helpers-0.1.0.dev1/app_helpers/iqmesh_ntw.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    12884 2024-04-22 10:17:40.000000 iqrfpy_app_helpers-0.1.0.dev1/app_helpers/iqrf_application.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6395 2024-04-22 08:05:09.000000 iqrfpy_app_helpers-0.1.0.dev1/app_helpers/ntw_device.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1976 2024-04-22 10:15:25.000000 iqrfpy_app_helpers-0.1.0.dev1/app_helpers/objects.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-22 05:32:54.000000 iqrfpy_app_helpers-0.1.0.dev1/app_helpers/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     7004 2024-04-22 10:43:36.000000 iqrfpy_app_helpers-0.1.0.dev1/app_helpers/utils.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-22 10:53:23.391307 iqrfpy_app_helpers-0.1.0.dev1/iqrfpy_app_helpers.egg-info/
--rw-r--r--   0 khanak    (1000) khanak    (1000)     1963 2024-04-22 10:53:23.000000 iqrfpy_app_helpers-0.1.0.dev1/iqrfpy_app_helpers.egg-info/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      408 2024-04-22 10:53:23.000000 iqrfpy_app_helpers-0.1.0.dev1/iqrfpy_app_helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2024-04-22 10:53:23.000000 iqrfpy_app_helpers-0.1.0.dev1/iqrfpy_app_helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       30 2024-04-22 10:53:23.000000 iqrfpy_app_helpers-0.1.0.dev1/iqrfpy_app_helpers.egg-info/requires.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2024-04-22 10:53:23.000000 iqrfpy_app_helpers-0.1.0.dev1/iqrfpy_app_helpers.egg-info/top_level.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       38 2024-04-22 10:53:23.391307 iqrfpy_app_helpers-0.1.0.dev1/setup.cfg
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1827 2024-04-22 10:50:32.000000 iqrfpy_app_helpers-0.1.0.dev1/setup.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-23 09:49:03.976619 iqrfpy_app_helpers-0.1.0.dev2/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2024-04-22 05:15:39.000000 iqrfpy_app_helpers-0.1.0.dev2/LICENSE
+-rw-r--r--   0 khanak    (1000) khanak    (1000)     2000 2024-04-23 09:49:03.976619 iqrfpy_app_helpers-0.1.0.dev2/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      607 2024-04-22 05:32:13.000000 iqrfpy_app_helpers-0.1.0.dev2/README.md
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-23 09:49:03.976619 iqrfpy_app_helpers-0.1.0.dev2/app_helpers/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      734 2024-04-22 10:38:27.000000 iqrfpy_app_helpers-0.1.0.dev2/app_helpers/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3829 2024-04-22 10:15:40.000000 iqrfpy_app_helpers-0.1.0.dev2/app_helpers/iqmesh_ntw.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    12884 2024-04-22 10:17:40.000000 iqrfpy_app_helpers-0.1.0.dev2/app_helpers/iqrf_application.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7319 2024-04-23 09:37:06.000000 iqrfpy_app_helpers-0.1.0.dev2/app_helpers/ntw_device.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1976 2024-04-22 10:15:25.000000 iqrfpy_app_helpers-0.1.0.dev2/app_helpers/objects.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-22 05:32:54.000000 iqrfpy_app_helpers-0.1.0.dev2/app_helpers/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7004 2024-04-22 10:43:36.000000 iqrfpy_app_helpers-0.1.0.dev2/app_helpers/utils.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-23 09:49:03.976619 iqrfpy_app_helpers-0.1.0.dev2/iqrfpy_app_helpers.egg-info/
+-rw-r--r--   0 khanak    (1000) khanak    (1000)     2000 2024-04-23 09:49:03.000000 iqrfpy_app_helpers-0.1.0.dev2/iqrfpy_app_helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      408 2024-04-23 09:49:03.000000 iqrfpy_app_helpers-0.1.0.dev2/iqrfpy_app_helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2024-04-23 09:49:03.000000 iqrfpy_app_helpers-0.1.0.dev2/iqrfpy_app_helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       52 2024-04-23 09:49:03.000000 iqrfpy_app_helpers-0.1.0.dev2/iqrfpy_app_helpers.egg-info/requires.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2024-04-23 09:49:03.000000 iqrfpy_app_helpers-0.1.0.dev2/iqrfpy_app_helpers.egg-info/top_level.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       38 2024-04-23 09:49:03.976619 iqrfpy_app_helpers-0.1.0.dev2/setup.cfg
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1860 2024-04-23 09:47:46.000000 iqrfpy_app_helpers-0.1.0.dev2/setup.py
```

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/LICENSE` & `iqrfpy_app_helpers-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/PKG-INFO` & `iqrfpy_app_helpers-0.1.0.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy-app-helpers
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Diagnostics for iqrfpy
 Home-page: https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy-app-helpers
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Project-URL: Homepage, https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy-app-helpers
 Project-URL: Changelog, https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy-app-helpers/-/blob/master/changelog.md
@@ -22,14 +22,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: iqrfpy>=0.2.0
+Requires-Dist: iqrfpy-mqtt-transport
 Requires-Dist: tabulate>=0.9.0
 
 ## iqrfpy-app-helpers
 
 An extension for [iqrfpy](https://pypi.org/project/iqrfpy/) offering basic application logic examples.
 
 ## Quick start
```

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/README.md` & `iqrfpy_app_helpers-0.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/app_helpers/__init__.py` & `iqrfpy_app_helpers-0.1.0.dev2/app_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/app_helpers/iqmesh_ntw.py` & `iqrfpy_app_helpers-0.1.0.dev2/app_helpers/iqmesh_ntw.py`

 * *Files identical despite different names*

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/app_helpers/iqrf_application.py` & `iqrfpy_app_helpers-0.1.0.dev2/app_helpers/iqrf_application.py`

 * *Files identical despite different names*

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/app_helpers/ntw_device.py` & `iqrfpy_app_helpers-0.1.0.dev2/app_helpers/ntw_device.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from iqrfpy.objects import ExplorationPerEnumData, OsReadData, OsTrConfData
 from iqrfpy.utils.common import Common
 from iqrfpy.peripherals.exploration import PeripheralEnumerationResponse
 from iqrfpy.peripherals.os import ReadTrConfResponse
+from tabulate import tabulate, SEPARATING_LINE
 
 __all__ = (
     'NtwDevice'
 )
 
 
 class NtwDevice(object):
@@ -71,22 +72,25 @@
     def device_ident_str(self) -> str:
         """
         Returns a formatted string representing the TR module information.
 
         Returns:
             str: A string containing the TR module type, MID, IQRF OS version, and build number.
         """
-        s = f'{self.tr_type}, MID: {self.mid}, IQRF OS: {self.os_ver} ({self.os_build})'
-        s += f'\nDPA: {Common.dpa_version_to_str(self.dpa_ver)}, HWPID: 0x{self.hwpid:04X} (ver: {int(self.hwpid_ver / 256):02X}.{(self.hwpid_ver & 0x00FF):02X})'
-
-        ntw_type = 'STD+LP' if self.std_lp_ntw_type else 'STD'
-        rf_mode = 'LP' if self.lp_rf_mode else 'STD'
-
-        s += f', Ntw. type: {ntw_type}, Rf mode: {rf_mode}'
-        return s
+        ident_headers = ['Device identification', '']
+        ident_data = [
+            ['TR series', self.tr_type],
+            ['MID', self.mid],
+            ['IQRF OS', f'{self.os_ver} ({self.os_build})'],
+            ['DPA', Common.dpa_version_to_str(self.dpa_ver)],
+            ['HWPID', f'0x{self.hwpid:04X} (ver: {int(self.hwpid_ver / 256):02X}.{(self.hwpid_ver & 0x00FF):02X})'],
+            ['Network type', 'STD+LP' if self.std_lp_ntw_type else 'STD'],
+            ['RF mode', 'LP' if self.lp_rf_mode else 'STD'],
+        ]
+        return tabulate(headers=ident_headers, tabular_data=ident_data, tablefmt='double_outline')
 
     def set_peripheral_enum(self, data: PeripheralEnumerationResponse):
         self._parse_peripheral_enum(data.per_enum_data)
 
     def set_tr_conf(self, data: ReadTrConfResponse) -> bool:
         """
         Saves and parses TR configuration from Read TR configuration response to the object.
@@ -125,33 +129,42 @@
     def tr_conf_str(self):
         """
         Returns a formatted string representing the TR configuration.
 
         Returns:
             str: A string containing TR configuration parameters.
         """
-        s = 'Init PHY:'
-        s += f'\n\tRf band: {self.rf_band}, Thermometer: {self.is_thermometer}, EEEPROM: {self.is_eeeprom}, IL: {self.is_il_type}'
-        s += '\nRF channels:'
-        s += f'\n\tA: {self.tr_config.rf_channel_a}'
-        s += f'\n\tB: {self.tr_config.rf_channel_b}'
-        s += f'\n\tAlternative DSM: {self.tr_config.alternative_dsm_channel}'
-        s += '\nRF:'
-        ntw_type = 'STD+LP' if self.tr_config.std_and_lp_network else 'STD'
-        s += f'\n\tNetwork type: {ntw_type}'
-        s += f'\n\tTX power: {self.tr_config.rf_output_power}'
-        s += f'\n\tRX filter: {self.tr_config.rf_signal_filter}'
-        s += f'\n\tLP RX timeout: {self.tr_config.lp_rf_timeout}'
-        s += '\nEmbedded peripherals (enabled):'
-
-        for x in self.tr_config.embedded_peripherals:
-            s += f'\n\t{x.name}'
-
-        s += '\nOther:'
-        s += f'\n\tCustom DPA Handler: {self.tr_config.custom_dpa_handler}'
-        s += f'\n\tDPA Peer-to-Peer: {self.tr_config.dpa_peer_to_peer}'
-        s += f'\n\tUser peer-to-peer: {self.tr_config.user_peer_to_peer}'
-        s += f'\n\tLocal FRC: {self.tr_config.local_frc}'
-        s += f'\n\tIO Setup: {self.tr_config.io_setup}'
-        s += f'\n\tRouting off: {self.tr_config.routing_off}'
-        s += f'\n\tStay awake when not bonded: {self.tr_config.stay_awake_when_not_bonded}'
-        return s
+        init_phy_headers = ['Init PHY', '']
+        init_phy_data = [
+            ['RF Band', str(self.rf_band)],
+            ['Thermometer', str(self.is_thermometer)],
+            ['EEEPROM', str(self.is_eeeprom)],
+            ['IL', str(self.is_il_type)],
+        ]
+        rf_headers = ['RF', '']
+        rf_data = [
+            ['Network type', 'STD+LP' if self.tr_config.std_and_lp_network else 'STD'],
+            ['TX power', self.tr_config.rf_output_power],
+            ['RX filter', self.tr_config.rf_signal_filter],
+            ['LP RX timeout', self.tr_config.lp_rf_timeout],
+            ['Channel A', self.tr_config.rf_channel_a],
+            ['Channel B', self.tr_config.rf_channel_b],
+            ['Alternative DSM channel', self.tr_config.alternative_dsm_channel],
+        ]
+        embedded_pers_headers = ['Embedded peripherals (enabled)']
+        embedded_pers_data = [[str(x.name)] for x in self.tr_config.embedded_peripherals]
+        other_headers = ['Other', '']
+        other_data = [
+            ['Custom DPA handler', str(self.tr_config.custom_dpa_handler)],
+            ['DPA Peer-to-Peer', str(self.tr_config.dpa_peer_to_peer)],
+            ['User Peer-to-Peer', str(self.tr_config.user_peer_to_peer)],
+            ['Local FRC', str(self.tr_config.local_frc)],
+            ['IO Setup', str(self.tr_config.io_setup)],
+            ['Routing off', str(self.tr_config.routing_off)],
+            ['Stay awake when not bonded', str(self.tr_config.stay_awake_when_not_bonded)],
+        ]
+        init_phy_str = tabulate(headers=init_phy_headers, tabular_data=init_phy_data, tablefmt='double_outline')
+        rf_str = tabulate(headers=rf_headers, tabular_data=rf_data, tablefmt='double_outline')
+        embedded_pers_str = tabulate(headers=embedded_pers_headers, tabular_data=embedded_pers_data,
+                                     tablefmt='double_outline')
+        other_str = tabulate(headers=other_headers, tabular_data=other_data, tablefmt='double_outline')
+        return '\n'.join([init_phy_str, rf_str, embedded_pers_str, other_str])
```

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/app_helpers/objects.py` & `iqrfpy_app_helpers-0.1.0.dev2/app_helpers/objects.py`

 * *Files identical despite different names*

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/app_helpers/utils.py` & `iqrfpy_app_helpers-0.1.0.dev2/app_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/iqrfpy_app_helpers.egg-info/PKG-INFO` & `iqrfpy_app_helpers-0.1.0.dev2/iqrfpy_app_helpers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy-app-helpers
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Diagnostics for iqrfpy
 Home-page: https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy-app-helpers
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Project-URL: Homepage, https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy-app-helpers
 Project-URL: Changelog, https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy-app-helpers/-/blob/master/changelog.md
@@ -22,14 +22,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: iqrfpy>=0.2.0
+Requires-Dist: iqrfpy-mqtt-transport
 Requires-Dist: tabulate>=0.9.0
 
 ## iqrfpy-app-helpers
 
 An extension for [iqrfpy](https://pypi.org/project/iqrfpy/) offering basic application logic examples.
 
 ## Quick start
```

### Comparing `iqrfpy_app_helpers-0.1.0.dev1/setup.py` & `iqrfpy_app_helpers-0.1.0.dev2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = file.read()
 
 setup(
     name='iqrfpy-app-helpers',
     description='Diagnostics for iqrfpy',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.1.0-dev1',
+    version='0.1.0-dev2',
     url='https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy-app-helpers',
     author='Karel Hanák',
     author_email='karel.hanak@iqrf.org',
     license='Apache-2.0',
     keywords=['iqrf'],
     project_urls={
         'Homepage': 'https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy-app-helpers',
@@ -42,10 +42,11 @@
         'iqrfpy.ext.app_helpers': [
             'py.typed'
         ]
     },
     python_requires='>=3.10',
     install_requires=[
         'iqrfpy>=0.2.0',
+        'iqrfpy-mqtt-transport',
         'tabulate>=0.9.0',
     ]
 )
```

