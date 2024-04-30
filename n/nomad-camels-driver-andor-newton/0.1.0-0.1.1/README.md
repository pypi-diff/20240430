# Comparing `tmp/nomad_camels_driver_andor_newton-0.1.0.tar.gz` & `tmp/nomad_camels_driver_andor_newton-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_camels_driver_andor_newton-0.1.0.tar", last modified: Fri Jan 26 08:53:15 2024, max compression
+gzip compressed data, was "nomad_camels_driver_andor_newton-0.1.1.tar", last modified: Tue Apr 30 13:32:13 2024, max compression
```

## Comparing `nomad_camels_driver_andor_newton-0.1.0.tar` & `nomad_camels_driver_andor_newton-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-26 08:53:15.711178 nomad_camels_driver_andor_newton-0.1.0/
--rw-rw-rw-   0        0        0    26525 2023-06-29 08:48:55.000000 nomad_camels_driver_andor_newton-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1154 2024-01-26 08:53:15.708179 nomad_camels_driver_andor_newton-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-01-26 08:48:32.000000 nomad_camels_driver_andor_newton-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-26 08:53:15.661178 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton/
--rw-rw-rw-   0        0        0        0 2023-04-14 09:15:42.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton/__init__.py
--rw-rw-rw-   0        0        0     8580 2023-12-08 13:22:50.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton/andor_newton.py
--rw-rw-rw-   0        0        0    11258 2023-12-08 13:21:04.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton/andor_newton_config.py
--rw-rw-rw-   0        0        0     6223 2023-12-11 10:01:47.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton/andor_newton_ophyd.py
-drwxrwxrwx   0        0        0        0 2024-01-26 08:53:15.706181 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton.egg-info/
--rw-rw-rw-   0        0        0     1154 2024-01-26 08:53:15.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-01-26 08:53:15.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-26 08:53:15.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-01-26 08:53:15.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2024-01-26 08:53:15.000000 nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      737 2024-01-26 08:47:52.000000 nomad_camels_driver_andor_newton-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-26 08:53:15.712179 nomad_camels_driver_andor_newton-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 13:32:13.552937 nomad_camels_driver_andor_newton-0.1.1/
+-rw-rw-rw-   0        0        0    26525 2024-03-19 13:39:32.000000 nomad_camels_driver_andor_newton-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1154 2024-04-30 13:32:13.550938 nomad_camels_driver_andor_newton-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-03-19 13:39:32.000000 nomad_camels_driver_andor_newton-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 13:32:13.513940 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton/
+-rw-rw-rw-   0        0        0        0 2023-04-14 09:15:42.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton/__init__.py
+-rw-rw-rw-   0        0        0     9248 2024-04-30 09:55:35.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton/andor_newton.py
+-rw-rw-rw-   0        0        0    11741 2024-04-30 09:55:12.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton/andor_newton_config.py
+-rw-rw-rw-   0        0        0     6475 2024-04-30 13:30:44.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton/andor_newton_ophyd.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:32:13.548938 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton.egg-info/
+-rw-rw-rw-   0        0        0     1154 2024-04-30 13:32:13.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-04-30 13:32:13.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 13:32:13.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-30 13:32:13.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-04-30 13:32:13.000000 nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      737 2024-04-30 10:04:25.000000 nomad_camels_driver_andor_newton-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 13:32:13.552937 nomad_camels_driver_andor_newton-0.1.1/setup.cfg
```

### Comparing `nomad_camels_driver_andor_newton-0.1.0/LICENSE.txt` & `nomad_camels_driver_andor_newton-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_andor_newton-0.1.0/PKG-INFO` & `nomad_camels_driver_andor_newton-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad_camels_driver_andor_newton
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package provides everything to run an Andor Newton CCD.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
```

### Comparing `nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton/andor_newton.py` & `nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton/andor_newton.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,148 +6,212 @@
 from .andor_newton_ophyd import Andor_Newton
 from PySide6.QtWidgets import QComboBox, QLabel
 from PySide6.QtCore import Qt, Signal
 
 
 class subclass(device_class.Device):
     def __init__(self, **kwargs):
-        super().__init__(name='andor_newton', virtual=False,
-                         tags=['Camera', 'spectrometer', 'CCD', 'spectrum', 'Andor',],
-                         directory='andor_newton', ophyd_device=Andor_Newton,
-                         ophyd_class_name='Andor_Newton', **kwargs)
-        self.config['set_temperature'] = -60
-        self.config['shutter_mode'] = 'auto'
-        self.config['exposure_time'] = 1
-        self.config['readout_mode'] = 'FVB - full vertical binning'
-        self.config['preamp_gain'] = 4
-        self.config['horizontal_binning'] = 1
-        self.config['hs_speed'] = 0.05
-        self.config['vs_speed'] = 25.7
-        self.config['multi_tracks'] = {}
-        self.config['shutter_ttl_open'] = 'low'
+        super().__init__(
+            name="andor_newton",
+            virtual=False,
+            tags=[
+                "Camera",
+                "spectrometer",
+                "CCD",
+                "spectrum",
+                "Andor",
+            ],
+            directory="andor_newton",
+            ophyd_device=Andor_Newton,
+            ophyd_class_name="Andor_Newton",
+            **kwargs,
+        )
+        self.config["set_temperature"] = -60
+        self.config["shutter_mode"] = "auto"
+        self.config["exposure_time"] = 1
+        self.config["readout_mode"] = "FVB - full vertical binning"
+        self.config["preamp_gain"] = 4
+        self.config["horizontal_binning"] = 1
+        self.config["hs_speed"] = 0.05
+        self.config["vs_speed"] = 25.7
+        self.config["multi_tracks"] = {}
+        self.config["shutter_ttl_open"] = "low"
 
 
 class subclass_config(device_class.Device_Config):
-    def __init__(self, parent=None, data='', settings_dict=None, config_dict=None, additional_info=None, **kwargs):
-        super().__init__(parent, 'Andor Newton', data,
-                         settings_dict=settings_dict, config_dict=config_dict,
-                         additional_info=additional_info, **kwargs)
+    def __init__(
+        self,
+        parent=None,
+        data="",
+        settings_dict=None,
+        config_dict=None,
+        additional_info=None,
+        **kwargs,
+    ):
+        super().__init__(
+            parent,
+            "Andor Newton",
+            data,
+            settings_dict=settings_dict,
+            config_dict=config_dict,
+            additional_info=additional_info,
+            **kwargs,
+        )
         self.dll_path = Path_Button_Edit()
-        if 'dll_path' in settings_dict:
-            self.dll_path.line.setText(settings_dict['dll_path'])
+        if "dll_path" in settings_dict:
+            self.dll_path.line.setText(settings_dict["dll_path"])
         self.comboBox_camera = QComboBox()
         self.update_dll()
-        if 'camera' in self.settings_dict:
-            self.comboBox_camera.setCurrentIndex(self.settings_dict['camera'])
-        self.layout().addWidget(QLabel('Path to dll (atmcd64d_legacy.dll or atmcd64d.dll)'), 17, 0, 1, 5)
+        if "camera" in self.settings_dict:
+            self.comboBox_camera.setCurrentIndex(self.settings_dict["camera"])
+        self.layout().addWidget(
+            QLabel("Path to dll (atmcd64d_legacy.dll or atmcd64d.dll)"), 17, 0, 1, 5
+        )
         self.layout().addWidget(self.dll_path, 18, 0, 1, 5)
-        self.layout().addWidget(QLabel('Camera:'), 19, 0)
+        self.layout().addWidget(QLabel("Camera:"), 19, 0)
         self.layout().addWidget(self.comboBox_camera, 19, 1, 1, 4)
         self.dll_path.path_changed.connect(self.update_dll)
 
-        self.sub_widget = subclass_config_sub(config_dict=config_dict, parent=parent, settings_dict=settings_dict)
+        self.sub_widget = subclass_config_sub(
+            config_dict=config_dict, parent=parent, settings_dict=settings_dict
+        )
         self.layout().addWidget(self.sub_widget, 20, 0, 1, 5)
         self.load_settings()
 
     def update_dll(self):
         self.setCursor(Qt.WaitCursor)
         cam_list = []
         dll_path = self.dll_path.get_path()
         if dll_path:
             import pylablib
-            pylablib.par['devices/dlls/andor_sdk2'] = dll_path
+
+            pylablib.par["devices/dlls/andor_sdk2"] = dll_path
             from pylablib.devices import Andor
+
             try:
                 for i in range(Andor.get_cameras_number_SDK2()):
                     cam = Andor.AndorSDK2Camera(idx=i)
                     info = cam.get_device_info()
-                    cam_list.append(f'{info.controller_model}, {info.head_model}, {info.serial_number}')
+                    cam_list.append(
+                        f"{info.controller_model}, {info.head_model}, {info.serial_number}"
+                    )
                     cam.close()
             except Exception as e:
-                WarnPopup(self, f'Dll could not be loaded\n{e}', 'dll not loaded')
+                WarnPopup(self, f"Dll could not be loaded\n{e}", "dll not loaded")
         self.comboBox_camera.clear()
         if cam_list:
             self.comboBox_camera.addItems(cam_list)
         else:
-            self.comboBox_camera.addItem('No camera detected or wrong dll!')
+            self.comboBox_camera.addItem("No camera detected or wrong dll!")
         self.setCursor(Qt.ArrowCursor)
 
     def get_config(self):
         self.config_dict.update(self.sub_widget.get_config())
         return super().get_config()
 
     def get_settings(self):
-        self.settings_dict['dll_path'] = self.dll_path.get_path()
-        self.settings_dict['camera'] = self.comboBox_camera.currentIndex()
+        self.settings_dict["dll_path"] = self.dll_path.get_path()
+        self.settings_dict["camera"] = self.comboBox_camera.currentIndex()
         return super().get_settings()
 
 
 class subclass_config_sub(device_class.Device_Config_Sub, Ui_andor_newton_config):
     config_changed = Signal(object, str)
 
     def __init__(self, config_dict=None, parent=None, settings_dict=None):
-        super().__init__(parent=parent, config_dict=config_dict,
-                         settings_dict=settings_dict)
+        super().__init__(
+            parent=parent, config_dict=config_dict, settings_dict=settings_dict
+        )
         self.setupUi(self)
         tableData = {}
-        if 'multi_tracks' in config_dict:
-            tableData = config_dict['multi_tracks']
-        self.track_table = AddRemoveTable(headerLabels=['Start', 'End'],
-                                          tableData=tableData, title='Tracks')
+        if "multi_tracks" in config_dict:
+            tableData = config_dict["multi_tracks"]
+        self.track_table = AddRemoveTable(
+            headerLabels=["Start", "End"], tableData=tableData, title="Tracks"
+        )
         self.tracks_frame.layout().addWidget(self.track_table)
         self.load_config()
-        self.set_temperature.lineEdit().returnPressed.connect(lambda x=None, y='set_temperature': self.config_changed.emit(x, y))
-        self.comboBox_shutter_mode.currentTextChanged.connect(lambda x=None, y='shutter_mode': self.config_changed.emit(x, y))
-        self.comboBox_shutter_ttl.currentTextChanged.connect(lambda x=None, y='shutter_ttl_open': self.config_changed.emit(x, y))
-        self.exposure_time.lineEdit().returnPressed.connect(lambda x=None, y='exposure_time': self.config_changed.emit(x, y))
-        self.comboBox_readout_mode.currentTextChanged.connect(lambda x=None, y='readout_mode': self.config_changed.emit(x, y))
-        self.preamp_gain.lineEdit().returnPressed.connect(lambda x=None, y='preamp_gain': self.config_changed.emit(x, y))
-        self.horizontal_binning.lineEdit().returnPressed.connect(lambda x=None, y='horizontal_binning': self.config_changed.emit(x, y))
-        self.hs_speed.lineEdit().returnPressed.connect(lambda x=None, y='hs_speed': self.config_changed.emit(x, y))
-        self.vs_speed.lineEdit().returnPressed.connect(lambda x=None, y='vs_speed': self.config_changed.emit(x, y))
+        self.set_temperature.lineEdit().returnPressed.connect(
+            lambda x=None, y="set_temperature": self.config_changed.emit(x, y)
+        )
+        self.comboBox_shutter_mode.currentTextChanged.connect(
+            lambda x=None, y="shutter_mode": self.config_changed.emit(x, y)
+        )
+        self.comboBox_shutter_ttl.currentTextChanged.connect(
+            lambda x=None, y="shutter_ttl_open": self.config_changed.emit(x, y)
+        )
+        self.exposure_time.lineEdit().returnPressed.connect(
+            lambda x=None, y="exposure_time": self.config_changed.emit(x, y)
+        )
+        self.comboBox_readout_mode.currentTextChanged.connect(
+            lambda x=None, y="readout_mode": self.config_changed.emit(x, y)
+        )
+        self.preamp_gain.lineEdit().returnPressed.connect(
+            lambda x=None, y="preamp_gain": self.config_changed.emit(x, y)
+        )
+        self.horizontal_binning.lineEdit().returnPressed.connect(
+            lambda x=None, y="horizontal_binning": self.config_changed.emit(x, y)
+        )
+        self.hs_speed.lineEdit().returnPressed.connect(
+            lambda x=None, y="hs_speed": self.config_changed.emit(x, y)
+        )
+        self.vs_speed.lineEdit().returnPressed.connect(
+            lambda x=None, y="vs_speed": self.config_changed.emit(x, y)
+        )
         # self.track_table.table.clicked.connect(lambda x=None, y='multi_tracks': self.config_changed.emit(x,y))
 
     def load_config(self):
         tableData = {}
-        if 'multi_tracks' in self.config_dict:
-            tableData = self.config_dict['multi_tracks']
+        if "multi_tracks" in self.config_dict:
+            tableData = self.config_dict["multi_tracks"]
         self.track_table.change_table_data(tableData)
-        if 'set_temperature' in self.config_dict:
-            self.set_temperature.setValue(self.config_dict['set_temperature'])
-        if 'get_temperature' in self.config_dict:
-            self.lineEdit_current_temperature.setText(f'{self.config_dict["get_temperature"]:.2f}')
+        if "set_temperature" in self.config_dict:
+            self.set_temperature.setValue(self.config_dict["set_temperature"])
+        if "get_temperature" in self.config_dict:
+            self.lineEdit_current_temperature.setText(
+                f'{self.config_dict["get_temperature"]:.2f}'
+            )
             self.lineEdit_current_temperature.setHidden(False)
-            if 'temperature_status' in self.config_dict:
+            if "temperature_status" in self.config_dict:
                 from nomad_camels.utility import variables_handling
-                color = 'green' if self.config_dict['temperature_status'] == 'stabilized' else 'red'
-                self.lineEdit_current_temperature.setStyleSheet(f'background-color: rgb{variables_handling.get_color(color, True)}')
+
+                color = (
+                    "green"
+                    if self.config_dict["temperature_status"] == "stabilized"
+                    else "red"
+                )
+                self.lineEdit_current_temperature.setStyleSheet(
+                    f"background-color: rgb{variables_handling.get_color(color, True)}"
+                )
         else:
             self.lineEdit_current_temperature.setHidden(True)
-        if 'shutter_mode' in self.config_dict:
-            self.comboBox_shutter_mode.setCurrentText(self.config_dict['shutter_mode'])
-        if 'shutter_ttl_open' in self.config_dict:
-            self.comboBox_shutter_ttl.setCurrentText(self.config_dict['shutter_ttl_open'])
-        if 'exposure_time' in self.config_dict:
-            self.exposure_time.setValue(self.config_dict['exposure_time'])
-        if 'readout_mode' in self.config_dict:
-            self.comboBox_readout_mode.setCurrentText(self.config_dict['readout_mode'])
-        if 'preamp_gain' in self.config_dict:
-            self.preamp_gain.setValue(self.config_dict['preamp_gain'])
-        if 'horizontal_binning' in self.config_dict:
-            self.horizontal_binning.setValue(self.config_dict['horizontal_binning'])
-        if 'hs_speed' in self.config_dict:
-            self.hs_speed.setValue(self.config_dict['hs_speed'])
-        if 'vs_speed' in self.config_dict:
-            self.vs_speed.setValue(self.config_dict['vs_speed'])
+        if "shutter_mode" in self.config_dict:
+            self.comboBox_shutter_mode.setCurrentText(self.config_dict["shutter_mode"])
+        if "shutter_ttl_open" in self.config_dict:
+            self.comboBox_shutter_ttl.setCurrentText(
+                self.config_dict["shutter_ttl_open"]
+            )
+        if "exposure_time" in self.config_dict:
+            self.exposure_time.setValue(self.config_dict["exposure_time"])
+        if "readout_mode" in self.config_dict:
+            self.comboBox_readout_mode.setCurrentText(self.config_dict["readout_mode"])
+        if "preamp_gain" in self.config_dict:
+            self.preamp_gain.setValue(self.config_dict["preamp_gain"])
+        if "horizontal_binning" in self.config_dict:
+            self.horizontal_binning.setValue(self.config_dict["horizontal_binning"])
+        if "hs_speed" in self.config_dict:
+            self.hs_speed.setValue(self.config_dict["hs_speed"])
+        if "vs_speed" in self.config_dict:
+            self.vs_speed.setValue(self.config_dict["vs_speed"])
 
     def get_config(self):
-        self.config_dict['set_temperature'] = self.set_temperature.value()
-        self.config_dict['shutter_mode'] = self.comboBox_shutter_mode.currentText()
-        self.config_dict['shutter_ttl_open'] = self.comboBox_shutter_ttl.currentText()
-        self.config_dict['exposure_time'] = self.exposure_time.value()
-        self.config_dict['readout_mode'] = self.comboBox_readout_mode.currentText()
-        self.config_dict['preamp_gain'] = self.preamp_gain.value()
-        self.config_dict['horizontal_binning'] = self.horizontal_binning.value()
-        self.config_dict['hs_speed'] = self.hs_speed.value()
-        self.config_dict['vs_speed'] = self.vs_speed.value()
-        self.config_dict['multi_tracks'] = self.track_table.update_table_data()
+        self.config_dict["set_temperature"] = self.set_temperature.value()
+        self.config_dict["shutter_mode"] = self.comboBox_shutter_mode.currentText()
+        self.config_dict["shutter_ttl_open"] = self.comboBox_shutter_ttl.currentText()
+        self.config_dict["exposure_time"] = self.exposure_time.value()
+        self.config_dict["readout_mode"] = self.comboBox_readout_mode.currentText()
+        self.config_dict["preamp_gain"] = self.preamp_gain.value()
+        self.config_dict["horizontal_binning"] = self.horizontal_binning.value()
+        self.config_dict["hs_speed"] = self.hs_speed.value()
+        self.config_dict["vs_speed"] = self.vs_speed.value()
+        self.config_dict["multi_tracks"] = self.track_table.update_table_data()
         return super().get_config()
```

### Comparing `nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton/andor_newton_config.py` & `nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton/andor_newton_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,243 +1,332 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'andor_newton_config.ui'
-##
-## Created by: Qt User Interface Compiler version 6.5.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
-    QMetaObject, QObject, QPoint, QRect,
-    QSize, QTime, QUrl, Qt)
-from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
-    QFont, QFontDatabase, QGradient, QIcon,
-    QImage, QKeySequence, QLinearGradient, QPainter,
-    QPalette, QPixmap, QRadialGradient, QTransform)
-from PySide6.QtWidgets import (QAbstractSpinBox, QApplication, QComboBox, QDoubleSpinBox,
-    QFrame, QGridLayout, QLabel, QLineEdit,
-    QSizePolicy, QSpacerItem, QSpinBox, QWidget)
-
-class Ui_andor_newton_config(object):
-    def setupUi(self, andor_newton_config):
-        if not andor_newton_config.objectName():
-            andor_newton_config.setObjectName(u"andor_newton_config")
-        andor_newton_config.resize(339, 285)
-        self.gridLayout = QGridLayout(andor_newton_config)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.tracks_frame = QFrame(andor_newton_config)
-        self.tracks_frame.setObjectName(u"tracks_frame")
-        self.tracks_frame.setFrameShape(QFrame.StyledPanel)
-        self.tracks_frame.setFrameShadow(QFrame.Raised)
-        self.gridLayout_3 = QGridLayout(self.tracks_frame)
-        self.gridLayout_3.setObjectName(u"gridLayout_3")
-
-        self.gridLayout.addWidget(self.tracks_frame, 0, 2, 3, 1)
-
-        self.frame_5 = QFrame(andor_newton_config)
-        self.frame_5.setObjectName(u"frame_5")
-        self.frame_5.setFrameShape(QFrame.StyledPanel)
-        self.frame_5.setFrameShadow(QFrame.Raised)
-        self.gridLayout_5 = QGridLayout(self.frame_5)
-        self.gridLayout_5.setObjectName(u"gridLayout_5")
-        self.label_15 = QLabel(self.frame_5)
-        self.label_15.setObjectName(u"label_15")
-        font = QFont()
-        font.setPointSize(9)
-        font.setBold(True)
-        self.label_15.setFont(font)
-
-        self.gridLayout_5.addWidget(self.label_15, 0, 0, 1, 1)
-
-        self.set_temperature = QSpinBox(self.frame_5)
-        self.set_temperature.setObjectName(u"set_temperature")
-        self.set_temperature.setMinimum(-99)
-        self.set_temperature.setValue(-60)
-
-        self.gridLayout_5.addWidget(self.set_temperature, 1, 0, 1, 1)
-
-        self.lineEdit_current_temperature = QLineEdit(self.frame_5)
-        self.lineEdit_current_temperature.setObjectName(u"lineEdit_current_temperature")
-        self.lineEdit_current_temperature.setEnabled(False)
-
-        self.gridLayout_5.addWidget(self.lineEdit_current_temperature, 2, 0, 1, 1)
-
-
-        self.gridLayout.addWidget(self.frame_5, 0, 0, 1, 1)
-
-        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.gridLayout.addItem(self.verticalSpacer, 2, 0, 1, 1)
-
-        self.frame_3 = QFrame(andor_newton_config)
-        self.frame_3.setObjectName(u"frame_3")
-        self.frame_3.setFrameShape(QFrame.StyledPanel)
-        self.frame_3.setFrameShadow(QFrame.Raised)
-        self.gridLayout_4 = QGridLayout(self.frame_3)
-        self.gridLayout_4.setObjectName(u"gridLayout_4")
-        self.preamp_gain = QSpinBox(self.frame_3)
-        self.preamp_gain.setObjectName(u"preamp_gain")
-        self.preamp_gain.setValue(4)
-
-        self.gridLayout_4.addWidget(self.preamp_gain, 4, 0, 1, 1)
-
-        self.label_8 = QLabel(self.frame_3)
-        self.label_8.setObjectName(u"label_8")
-
-        self.gridLayout_4.addWidget(self.label_8, 1, 0, 1, 1)
-
-        self.comboBox_readout_mode = QComboBox(self.frame_3)
-        self.comboBox_readout_mode.addItem("")
-        self.comboBox_readout_mode.addItem("")
-        self.comboBox_readout_mode.addItem("")
-        self.comboBox_readout_mode.addItem("")
-        self.comboBox_readout_mode.setObjectName(u"comboBox_readout_mode")
-
-        self.gridLayout_4.addWidget(self.comboBox_readout_mode, 2, 0, 1, 1)
-
-        self.label_9 = QLabel(self.frame_3)
-        self.label_9.setObjectName(u"label_9")
-
-        self.gridLayout_4.addWidget(self.label_9, 3, 0, 1, 1)
-
-        self.label_3 = QLabel(self.frame_3)
-        self.label_3.setObjectName(u"label_3")
-        self.label_3.setFont(font)
-
-        self.gridLayout_4.addWidget(self.label_3, 0, 0, 1, 1)
-
-        self.horizontal_binning = QSpinBox(self.frame_3)
-        self.horizontal_binning.setObjectName(u"horizontal_binning")
-        self.horizontal_binning.setSingleStep(2)
-        self.horizontal_binning.setValue(4)
-
-        self.gridLayout_4.addWidget(self.horizontal_binning, 6, 0, 1, 1)
-
-        self.hs_speed = QDoubleSpinBox(self.frame_3)
-        self.hs_speed.setObjectName(u"hs_speed")
-        self.hs_speed.setValue(0.050000000000000)
-
-        self.gridLayout_4.addWidget(self.hs_speed, 8, 0, 1, 1)
-
-        self.label_11 = QLabel(self.frame_3)
-        self.label_11.setObjectName(u"label_11")
-
-        self.gridLayout_4.addWidget(self.label_11, 7, 0, 1, 1)
-
-        self.vs_speed = QDoubleSpinBox(self.frame_3)
-        self.vs_speed.setObjectName(u"vs_speed")
-        self.vs_speed.setValue(25.699999999999999)
-
-        self.gridLayout_4.addWidget(self.vs_speed, 10, 0, 1, 1)
-
-        self.label_12 = QLabel(self.frame_3)
-        self.label_12.setObjectName(u"label_12")
-
-        self.gridLayout_4.addWidget(self.label_12, 9, 0, 1, 1)
-
-        self.label_10 = QLabel(self.frame_3)
-        self.label_10.setObjectName(u"label_10")
-
-        self.gridLayout_4.addWidget(self.label_10, 5, 0, 1, 1)
-
-
-        self.gridLayout.addWidget(self.frame_3, 0, 1, 2, 1)
-
-        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.gridLayout.addItem(self.verticalSpacer_2, 2, 1, 1, 1)
-
-        self.frame = QFrame(andor_newton_config)
-        self.frame.setObjectName(u"frame")
-        self.frame.setFrameShape(QFrame.StyledPanel)
-        self.frame.setFrameShadow(QFrame.Raised)
-        self.gridLayout_2 = QGridLayout(self.frame)
-        self.gridLayout_2.setObjectName(u"gridLayout_2")
-        self.comboBox_shutter_mode = QComboBox(self.frame)
-        self.comboBox_shutter_mode.addItem("")
-        self.comboBox_shutter_mode.addItem("")
-        self.comboBox_shutter_mode.addItem("")
-        self.comboBox_shutter_mode.setObjectName(u"comboBox_shutter_mode")
-
-        self.gridLayout_2.addWidget(self.comboBox_shutter_mode, 2, 0, 1, 1)
-
-        self.exposure_time = QDoubleSpinBox(self.frame)
-        self.exposure_time.setObjectName(u"exposure_time")
-        self.exposure_time.setButtonSymbols(QAbstractSpinBox.NoButtons)
-        self.exposure_time.setDecimals(3)
-        self.exposure_time.setSingleStep(0.100000000000000)
-
-        self.gridLayout_2.addWidget(self.exposure_time, 6, 0, 1, 1)
-
-        self.label = QLabel(self.frame)
-        self.label.setObjectName(u"label")
-        self.label.setFont(font)
-
-        self.gridLayout_2.addWidget(self.label, 0, 0, 1, 1)
-
-        self.label_5 = QLabel(self.frame)
-        self.label_5.setObjectName(u"label_5")
-
-        self.gridLayout_2.addWidget(self.label_5, 5, 0, 1, 1)
-
-        self.label_4 = QLabel(self.frame)
-        self.label_4.setObjectName(u"label_4")
-
-        self.gridLayout_2.addWidget(self.label_4, 1, 0, 1, 1)
-
-        self.label_2 = QLabel(self.frame)
-        self.label_2.setObjectName(u"label_2")
-
-        self.gridLayout_2.addWidget(self.label_2, 3, 0, 1, 1)
-
-        self.comboBox_shutter_ttl = QComboBox(self.frame)
-        self.comboBox_shutter_ttl.addItem("")
-        self.comboBox_shutter_ttl.addItem("")
-        self.comboBox_shutter_ttl.setObjectName(u"comboBox_shutter_ttl")
-
-        self.gridLayout_2.addWidget(self.comboBox_shutter_ttl, 4, 0, 1, 1)
-
-
-        self.gridLayout.addWidget(self.frame, 1, 0, 1, 1)
-
-        QWidget.setTabOrder(self.set_temperature, self.exposure_time)
-        QWidget.setTabOrder(self.exposure_time, self.preamp_gain)
-        QWidget.setTabOrder(self.preamp_gain, self.horizontal_binning)
-        QWidget.setTabOrder(self.horizontal_binning, self.hs_speed)
-        QWidget.setTabOrder(self.hs_speed, self.vs_speed)
-        QWidget.setTabOrder(self.vs_speed, self.comboBox_shutter_mode)
-        QWidget.setTabOrder(self.comboBox_shutter_mode, self.comboBox_readout_mode)
-
-        self.retranslateUi(andor_newton_config)
-
-        QMetaObject.connectSlotsByName(andor_newton_config)
-    # setupUi
-
-    def retranslateUi(self, andor_newton_config):
-        andor_newton_config.setWindowTitle(QCoreApplication.translate("andor_newton_config", u"Form", None))
-        self.label_15.setText(QCoreApplication.translate("andor_newton_config", u"Temperature (\u00b0C)", None))
-        self.label_8.setText(QCoreApplication.translate("andor_newton_config", u"Readout Mode", None))
-        self.comboBox_readout_mode.setItemText(0, QCoreApplication.translate("andor_newton_config", u"FVB - full vertical binning", None))
-        self.comboBox_readout_mode.setItemText(1, QCoreApplication.translate("andor_newton_config", u"multi track", None))
-        self.comboBox_readout_mode.setItemText(2, QCoreApplication.translate("andor_newton_config", u"image", None))
-        self.comboBox_readout_mode.setItemText(3, QCoreApplication.translate("andor_newton_config", u"random track", None))
-
-        self.label_9.setText(QCoreApplication.translate("andor_newton_config", u"Preamp Gain", None))
-        self.label_3.setText(QCoreApplication.translate("andor_newton_config", u"Readout", None))
-        self.label_11.setText(QCoreApplication.translate("andor_newton_config", u"HS Speed (MHz)", None))
-        self.label_12.setText(QCoreApplication.translate("andor_newton_config", u"VS Speed (\u00b5s/shift)", None))
-        self.label_10.setText(QCoreApplication.translate("andor_newton_config", u"Horizontal Binning", None))
-        self.comboBox_shutter_mode.setItemText(0, QCoreApplication.translate("andor_newton_config", u"open", None))
-        self.comboBox_shutter_mode.setItemText(1, QCoreApplication.translate("andor_newton_config", u"closed", None))
-        self.comboBox_shutter_mode.setItemText(2, QCoreApplication.translate("andor_newton_config", u"auto", None))
-
-        self.label.setText(QCoreApplication.translate("andor_newton_config", u"Exposure", None))
-        self.label_5.setText(QCoreApplication.translate("andor_newton_config", u"Exposure Time (s)", None))
-        self.label_4.setText(QCoreApplication.translate("andor_newton_config", u"Shutter Mode", None))
-        self.label_2.setText(QCoreApplication.translate("andor_newton_config", u"Shutter TTL open", None))
-        self.comboBox_shutter_ttl.setItemText(0, QCoreApplication.translate("andor_newton_config", u"low", None))
-        self.comboBox_shutter_ttl.setItemText(1, QCoreApplication.translate("andor_newton_config", u"high", None))
-
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'andor_newton_config.ui'
+##
+## Created by: Qt User Interface Compiler version 6.5.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide6.QtCore import (
+    QCoreApplication,
+    QDate,
+    QDateTime,
+    QLocale,
+    QMetaObject,
+    QObject,
+    QPoint,
+    QRect,
+    QSize,
+    QTime,
+    QUrl,
+    Qt,
+)
+from PySide6.QtGui import (
+    QBrush,
+    QColor,
+    QConicalGradient,
+    QCursor,
+    QFont,
+    QFontDatabase,
+    QGradient,
+    QIcon,
+    QImage,
+    QKeySequence,
+    QLinearGradient,
+    QPainter,
+    QPalette,
+    QPixmap,
+    QRadialGradient,
+    QTransform,
+)
+from PySide6.QtWidgets import (
+    QAbstractSpinBox,
+    QApplication,
+    QComboBox,
+    QDoubleSpinBox,
+    QFrame,
+    QGridLayout,
+    QLabel,
+    QLineEdit,
+    QSizePolicy,
+    QSpacerItem,
+    QSpinBox,
+    QWidget,
+)
+
+
+class Ui_andor_newton_config(object):
+    def setupUi(self, andor_newton_config):
+        if not andor_newton_config.objectName():
+            andor_newton_config.setObjectName("andor_newton_config")
+        andor_newton_config.resize(339, 285)
+        self.gridLayout = QGridLayout(andor_newton_config)
+        self.gridLayout.setObjectName("gridLayout")
+        self.tracks_frame = QFrame(andor_newton_config)
+        self.tracks_frame.setObjectName("tracks_frame")
+        self.tracks_frame.setFrameShape(QFrame.StyledPanel)
+        self.tracks_frame.setFrameShadow(QFrame.Raised)
+        self.gridLayout_3 = QGridLayout(self.tracks_frame)
+        self.gridLayout_3.setObjectName("gridLayout_3")
+
+        self.gridLayout.addWidget(self.tracks_frame, 0, 2, 3, 1)
+
+        self.frame_5 = QFrame(andor_newton_config)
+        self.frame_5.setObjectName("frame_5")
+        self.frame_5.setFrameShape(QFrame.StyledPanel)
+        self.frame_5.setFrameShadow(QFrame.Raised)
+        self.gridLayout_5 = QGridLayout(self.frame_5)
+        self.gridLayout_5.setObjectName("gridLayout_5")
+        self.label_15 = QLabel(self.frame_5)
+        self.label_15.setObjectName("label_15")
+        font = QFont()
+        font.setPointSize(9)
+        font.setBold(True)
+        self.label_15.setFont(font)
+
+        self.gridLayout_5.addWidget(self.label_15, 0, 0, 1, 1)
+
+        self.set_temperature = QSpinBox(self.frame_5)
+        self.set_temperature.setObjectName("set_temperature")
+        self.set_temperature.setMinimum(-99)
+        self.set_temperature.setValue(-60)
+
+        self.gridLayout_5.addWidget(self.set_temperature, 1, 0, 1, 1)
+
+        self.lineEdit_current_temperature = QLineEdit(self.frame_5)
+        self.lineEdit_current_temperature.setObjectName("lineEdit_current_temperature")
+        self.lineEdit_current_temperature.setEnabled(False)
+
+        self.gridLayout_5.addWidget(self.lineEdit_current_temperature, 2, 0, 1, 1)
+
+        self.gridLayout.addWidget(self.frame_5, 0, 0, 1, 1)
+
+        self.verticalSpacer = QSpacerItem(
+            20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding
+        )
+
+        self.gridLayout.addItem(self.verticalSpacer, 2, 0, 1, 1)
+
+        self.frame_3 = QFrame(andor_newton_config)
+        self.frame_3.setObjectName("frame_3")
+        self.frame_3.setFrameShape(QFrame.StyledPanel)
+        self.frame_3.setFrameShadow(QFrame.Raised)
+        self.gridLayout_4 = QGridLayout(self.frame_3)
+        self.gridLayout_4.setObjectName("gridLayout_4")
+        self.preamp_gain = QSpinBox(self.frame_3)
+        self.preamp_gain.setObjectName("preamp_gain")
+        self.preamp_gain.setValue(4)
+
+        self.gridLayout_4.addWidget(self.preamp_gain, 4, 0, 1, 1)
+
+        self.label_8 = QLabel(self.frame_3)
+        self.label_8.setObjectName("label_8")
+
+        self.gridLayout_4.addWidget(self.label_8, 1, 0, 1, 1)
+
+        self.comboBox_readout_mode = QComboBox(self.frame_3)
+        self.comboBox_readout_mode.addItem("")
+        self.comboBox_readout_mode.addItem("")
+        self.comboBox_readout_mode.addItem("")
+        self.comboBox_readout_mode.addItem("")
+        self.comboBox_readout_mode.setObjectName("comboBox_readout_mode")
+
+        self.gridLayout_4.addWidget(self.comboBox_readout_mode, 2, 0, 1, 1)
+
+        self.label_9 = QLabel(self.frame_3)
+        self.label_9.setObjectName("label_9")
+
+        self.gridLayout_4.addWidget(self.label_9, 3, 0, 1, 1)
+
+        self.label_3 = QLabel(self.frame_3)
+        self.label_3.setObjectName("label_3")
+        self.label_3.setFont(font)
+
+        self.gridLayout_4.addWidget(self.label_3, 0, 0, 1, 1)
+
+        self.horizontal_binning = QSpinBox(self.frame_3)
+        self.horizontal_binning.setObjectName("horizontal_binning")
+        self.horizontal_binning.setSingleStep(2)
+        self.horizontal_binning.setValue(4)
+
+        self.gridLayout_4.addWidget(self.horizontal_binning, 6, 0, 1, 1)
+
+        self.hs_speed = QDoubleSpinBox(self.frame_3)
+        self.hs_speed.setObjectName("hs_speed")
+        self.hs_speed.setValue(0.050000000000000)
+
+        self.gridLayout_4.addWidget(self.hs_speed, 8, 0, 1, 1)
+
+        self.label_11 = QLabel(self.frame_3)
+        self.label_11.setObjectName("label_11")
+
+        self.gridLayout_4.addWidget(self.label_11, 7, 0, 1, 1)
+
+        self.vs_speed = QDoubleSpinBox(self.frame_3)
+        self.vs_speed.setObjectName("vs_speed")
+        self.vs_speed.setValue(25.699999999999999)
+
+        self.gridLayout_4.addWidget(self.vs_speed, 10, 0, 1, 1)
+
+        self.label_12 = QLabel(self.frame_3)
+        self.label_12.setObjectName("label_12")
+
+        self.gridLayout_4.addWidget(self.label_12, 9, 0, 1, 1)
+
+        self.label_10 = QLabel(self.frame_3)
+        self.label_10.setObjectName("label_10")
+
+        self.gridLayout_4.addWidget(self.label_10, 5, 0, 1, 1)
+
+        self.gridLayout.addWidget(self.frame_3, 0, 1, 2, 1)
+
+        self.verticalSpacer_2 = QSpacerItem(
+            20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding
+        )
+
+        self.gridLayout.addItem(self.verticalSpacer_2, 2, 1, 1, 1)
+
+        self.frame = QFrame(andor_newton_config)
+        self.frame.setObjectName("frame")
+        self.frame.setFrameShape(QFrame.StyledPanel)
+        self.frame.setFrameShadow(QFrame.Raised)
+        self.gridLayout_2 = QGridLayout(self.frame)
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.comboBox_shutter_mode = QComboBox(self.frame)
+        self.comboBox_shutter_mode.addItem("")
+        self.comboBox_shutter_mode.addItem("")
+        self.comboBox_shutter_mode.addItem("")
+        self.comboBox_shutter_mode.setObjectName("comboBox_shutter_mode")
+
+        self.gridLayout_2.addWidget(self.comboBox_shutter_mode, 2, 0, 1, 1)
+
+        self.exposure_time = QDoubleSpinBox(self.frame)
+        self.exposure_time.setObjectName("exposure_time")
+        self.exposure_time.setButtonSymbols(QAbstractSpinBox.NoButtons)
+        self.exposure_time.setDecimals(3)
+        self.exposure_time.setSingleStep(0.100000000000000)
+
+        self.gridLayout_2.addWidget(self.exposure_time, 6, 0, 1, 1)
+
+        self.label = QLabel(self.frame)
+        self.label.setObjectName("label")
+        self.label.setFont(font)
+
+        self.gridLayout_2.addWidget(self.label, 0, 0, 1, 1)
+
+        self.label_5 = QLabel(self.frame)
+        self.label_5.setObjectName("label_5")
+
+        self.gridLayout_2.addWidget(self.label_5, 5, 0, 1, 1)
+
+        self.label_4 = QLabel(self.frame)
+        self.label_4.setObjectName("label_4")
+
+        self.gridLayout_2.addWidget(self.label_4, 1, 0, 1, 1)
+
+        self.label_2 = QLabel(self.frame)
+        self.label_2.setObjectName("label_2")
+
+        self.gridLayout_2.addWidget(self.label_2, 3, 0, 1, 1)
+
+        self.comboBox_shutter_ttl = QComboBox(self.frame)
+        self.comboBox_shutter_ttl.addItem("")
+        self.comboBox_shutter_ttl.addItem("")
+        self.comboBox_shutter_ttl.setObjectName("comboBox_shutter_ttl")
+
+        self.gridLayout_2.addWidget(self.comboBox_shutter_ttl, 4, 0, 1, 1)
+
+        self.gridLayout.addWidget(self.frame, 1, 0, 1, 1)
+
+        QWidget.setTabOrder(self.set_temperature, self.exposure_time)
+        QWidget.setTabOrder(self.exposure_time, self.preamp_gain)
+        QWidget.setTabOrder(self.preamp_gain, self.horizontal_binning)
+        QWidget.setTabOrder(self.horizontal_binning, self.hs_speed)
+        QWidget.setTabOrder(self.hs_speed, self.vs_speed)
+        QWidget.setTabOrder(self.vs_speed, self.comboBox_shutter_mode)
+        QWidget.setTabOrder(self.comboBox_shutter_mode, self.comboBox_readout_mode)
+
+        self.retranslateUi(andor_newton_config)
+
+        QMetaObject.connectSlotsByName(andor_newton_config)
+
+    # setupUi
+
+    def retranslateUi(self, andor_newton_config):
+        andor_newton_config.setWindowTitle(
+            QCoreApplication.translate("andor_newton_config", "Form", None)
+        )
+        self.label_15.setText(
+            QCoreApplication.translate(
+                "andor_newton_config", "Temperature (\u00b0C)", None
+            )
+        )
+        self.label_8.setText(
+            QCoreApplication.translate("andor_newton_config", "Readout Mode", None)
+        )
+        self.comboBox_readout_mode.setItemText(
+            0,
+            QCoreApplication.translate(
+                "andor_newton_config", "FVB - full vertical binning", None
+            ),
+        )
+        self.comboBox_readout_mode.setItemText(
+            1, QCoreApplication.translate("andor_newton_config", "multi track", None)
+        )
+        self.comboBox_readout_mode.setItemText(
+            2, QCoreApplication.translate("andor_newton_config", "image", None)
+        )
+        self.comboBox_readout_mode.setItemText(
+            3, QCoreApplication.translate("andor_newton_config", "random track", None)
+        )
+
+        self.label_9.setText(
+            QCoreApplication.translate("andor_newton_config", "Preamp Gain", None)
+        )
+        self.label_3.setText(
+            QCoreApplication.translate("andor_newton_config", "Readout", None)
+        )
+        self.label_11.setText(
+            QCoreApplication.translate("andor_newton_config", "HS Speed (MHz)", None)
+        )
+        self.label_12.setText(
+            QCoreApplication.translate(
+                "andor_newton_config", "VS Speed (\u00b5s/shift)", None
+            )
+        )
+        self.label_10.setText(
+            QCoreApplication.translate(
+                "andor_newton_config", "Horizontal Binning", None
+            )
+        )
+        self.comboBox_shutter_mode.setItemText(
+            0, QCoreApplication.translate("andor_newton_config", "open", None)
+        )
+        self.comboBox_shutter_mode.setItemText(
+            1, QCoreApplication.translate("andor_newton_config", "closed", None)
+        )
+        self.comboBox_shutter_mode.setItemText(
+            2, QCoreApplication.translate("andor_newton_config", "auto", None)
+        )
+
+        self.label.setText(
+            QCoreApplication.translate("andor_newton_config", "Exposure", None)
+        )
+        self.label_5.setText(
+            QCoreApplication.translate("andor_newton_config", "Exposure Time (s)", None)
+        )
+        self.label_4.setText(
+            QCoreApplication.translate("andor_newton_config", "Shutter Mode", None)
+        )
+        self.label_2.setText(
+            QCoreApplication.translate("andor_newton_config", "Shutter TTL open", None)
+        )
+        self.comboBox_shutter_ttl.setItemText(
+            0, QCoreApplication.translate("andor_newton_config", "low", None)
+        )
+        self.comboBox_shutter_ttl.setItemText(
+            1, QCoreApplication.translate("andor_newton_config", "high", None)
+        )
+
+    # retranslateUi
```

### Comparing `nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton/andor_newton_ophyd.py` & `nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton/andor_newton_ophyd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,86 @@
 from ophyd import Component as Cpt
-from ophyd import Device
 
 import pylablib as pll
 
-from nomad_camels.bluesky_handling.custom_function_signal import Custom_Function_Signal, Custom_Function_SignalRO
+from nomad_camels.bluesky_handling.custom_function_signal import (
+    Custom_Function_Signal,
+    Custom_Function_SignalRO,
+    Sequential_Device,
+)
 
 
-read_modes = {'FVB - full vertical binning': 'fvb',
-              'multi track': 'multi_track',
-              'random track': 'random_track'}
+read_modes = {
+    "FVB - full vertical binning": "fvb",
+    "multi track": "multi_track",
+    "random track": "random_track",
+}
 
-class Andor_Newton(Device):
+
+class Andor_Newton(Sequential_Device):
     """
     Driver for the Andor Newton CCD camera
     """
-    read_camera = Cpt(Custom_Function_SignalRO, name='read_camera', metadata={'units': 'intensity'})
 
-    get_temperature = Cpt(Custom_Function_SignalRO, name='get_temperature', kind='config')
-    temperature_status = Cpt(Custom_Function_SignalRO, name='temperature_status', kind='config')
+    read_camera = Cpt(
+        Custom_Function_SignalRO, name="read_camera", metadata={"units": "intensity"}
+    )
+
+    get_temperature = Cpt(
+        Custom_Function_SignalRO, name="get_temperature", kind="config"
+    )
+    temperature_status = Cpt(
+        Custom_Function_SignalRO, name="temperature_status", kind="config"
+    )
 
     # Configuration settings
-    set_temperature = Cpt(Custom_Function_Signal, name='set_temperature', kind='config')
-    shutter_mode = Cpt(Custom_Function_Signal, name='shutter_mode', kind='config')
-    exposure_time = Cpt(Custom_Function_Signal, name='exposure_time', kind='config')
-    readout_mode = Cpt(Custom_Function_Signal, name='readout_mode', kind='config')
-    preamp_gain = Cpt(Custom_Function_Signal, name='preamp_gain', kind='config')
-    horizontal_binning = Cpt(Custom_Function_Signal, name='horizontal_binning', kind='config')
-    hs_speed = Cpt(Custom_Function_Signal, name='hs_speed', kind='config')
-    vs_speed = Cpt(Custom_Function_Signal, name='vs_speed', kind='config')
-    multi_tracks = Cpt(Custom_Function_Signal, name='multi_tracks', kind='config')
+    set_temperature = Cpt(Custom_Function_Signal, name="set_temperature", kind="config")
+    shutter_mode = Cpt(Custom_Function_Signal, name="shutter_mode", kind="config")
+    exposure_time = Cpt(Custom_Function_Signal, name="exposure_time", kind="config")
+    readout_mode = Cpt(Custom_Function_Signal, name="readout_mode", kind="config")
+    preamp_gain = Cpt(Custom_Function_Signal, name="preamp_gain", kind="config")
+    horizontal_binning = Cpt(
+        Custom_Function_Signal, name="horizontal_binning", kind="config"
+    )
+    hs_speed = Cpt(Custom_Function_Signal, name="hs_speed", kind="config")
+    vs_speed = Cpt(Custom_Function_Signal, name="vs_speed", kind="config")
+    multi_tracks = Cpt(Custom_Function_Signal, name="multi_tracks", kind="config")
     # read_settings = Cpt(Custom_Function_SignalRO, name='read_settings', kind='config')
-    shutter_ttl_open = Cpt(Custom_Function_Signal, name='shutter_ttl_open', kind='config')
-
-    def __init__(self, prefix='', *, name, kind=None, read_attrs=None,
-                 configuration_attrs=None, parent=None, dll_path='',
-                 camera=0, **kwargs):
-        super().__init__(prefix=prefix, name=name, kind=kind, read_attrs=read_attrs,
-                         configuration_attrs=configuration_attrs, parent=parent, **kwargs)
-        if name == 'test':
+    shutter_ttl_open = Cpt(
+        Custom_Function_Signal, name="shutter_ttl_open", kind="config"
+    )
+
+    def __init__(
+        self,
+        prefix="",
+        *,
+        name,
+        kind=None,
+        read_attrs=None,
+        configuration_attrs=None,
+        parent=None,
+        dll_path="",
+        camera=0,
+        **kwargs
+    ):
+        super().__init__(
+            prefix=prefix,
+            name=name,
+            kind=kind,
+            read_attrs=read_attrs,
+            configuration_attrs=configuration_attrs,
+            parent=parent,
+            force_sequential=True,
+            **kwargs
+        )
+        if name == "test":
             return
-        pll.par['devices/dlls/andor_sdk2'] = dll_path
+        pll.par["devices/dlls/andor_sdk2"] = dll_path
         from pylablib.devices import Andor
+
         self.camera = Andor.AndorSDK2Camera(idx=camera)
 
         self.read_camera.read_function = self.read_camera_function
         self.get_temperature.read_function = self.get_temperature_function
         self.temperature_status.read_function = self.temperature_status_function
         self.set_temperature.put_function = self.set_temperature_function
         self.shutter_mode.put_function = self.shutter_mode_function
@@ -69,48 +105,48 @@
 
     def finalize_steps(self):
         self.camera.close()
 
     def read_camera_function(self):
         time = self.exposure_time.get()
         self.readout_mode.put(self.readout_mode.get())
-        dat = self.camera.snap(timeout=10*time)
-        if self.readout_mode.get() != 'image':
+        dat = self.camera.snap(timeout=10 * time)
+        if self.readout_mode.get() != "image":
             return dat[0]
         else:
             return dat
 
     def get_temperature_function(self):
         return self.camera.get_temperature()
 
     def temperature_status_function(self):
         return self.camera.get_temperature_status()
 
     def set_temperature_function(self, value):
         self.camera.set_temperature(value, enable_cooler=True)
-        self.camera.set_fan_mode('full')
+        self.camera.set_fan_mode("full")
 
     def shutter_mode_function(self, value):
         self.camera.setup_shutter(value, ttl_mode=self.shutter_ttl_setting)
 
     def shutter_ttl_open_function(self, value):
-        self.shutter_ttl_setting = 1 if value == 'high' else 0
+        self.shutter_ttl_setting = 1 if value == "high" else 0
         self.shutter_mode_function(self.shutter_mode.get())
 
     def exposure_time_function(self, value):
         self.camera.set_exposure(value)
 
     def readout_mode_function(self, value):
         if value in read_modes:
             value = read_modes[value]
-        if value == 'fvb':
-            value = 'multi_track'
+        if value == "fvb":
+            value = "multi_track"
             self.camera.setup_multi_track_mode(1, 255, 0)
-        elif value == 'multi_track':
-            self.multi_tracks.put(self.multi_tracks.get())
+        elif value == "multi_track":
+            self.multi_tracks_function(self.multi_tracks.get())
         self.camera.set_read_mode(value)
 
     def preamp_gain_function(self, value):
         closest = min(self.all_preamps, key=lambda x: abs(x - value))
         self.camera.set_amp_mode(preamp=self.all_preamps[closest])
 
     def horizontal_binning_function(self, value):
@@ -123,20 +159,17 @@
     def vs_speed_function(self, value):
         closest = min(self.all_vs_speeds, key=lambda x: abs(x - value))
         index = self.all_vs_speeds.index(closest)
         self.camera.set_vsspeed(index)
 
     def multi_tracks_function(self, track_data):
         try:
-            width = track_data['End'][0] - track_data['Start'][0]
-            offset = track_data['Start'][0] - 128 + int(width/2)
-            n = len(track_data['Start'])
+            width = track_data["End"][0] - track_data["Start"][0]
+            offset = track_data["Start"][0] - 128 + int(width / 2)
+            n = len(track_data["Start"])
         except Exception as e:
             n = 1
             width = 255
             offset = 0
             print(e)
-            print('Failed to setup multi track, using FVB settings')
+            print("Failed to setup multi track, using FVB settings")
         self.camera.setup_multi_track_mode(n, width, offset)
-
-
-
```

### Comparing `nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton.egg-info/PKG-INFO` & `nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad_camels_driver_andor_newton
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package provides everything to run an Andor Newton CCD.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
```

### Comparing `nomad_camels_driver_andor_newton-0.1.0/nomad_camels_driver_andor_newton.egg-info/SOURCES.txt` & `nomad_camels_driver_andor_newton-0.1.1/nomad_camels_driver_andor_newton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_andor_newton-0.1.0/pyproject.toml` & `nomad_camels_driver_andor_newton-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nomad_camels_driver_andor_newton"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="FAIRmat - HU Berlin", email="nomad-camels@fau.de" }
 ]
 description = "This package provides everything to run an Andor Newton CCD."
 readme = "README.md"
 requires-python = ">=3.9.6"
 classifiers = [
```

