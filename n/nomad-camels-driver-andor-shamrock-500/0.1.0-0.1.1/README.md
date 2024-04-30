# Comparing `tmp/nomad_camels_driver_andor_shamrock_500-0.1.0.tar.gz` & `tmp/nomad_camels_driver_andor_shamrock_500-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_camels_driver_andor_shamrock_500-0.1.0.tar", last modified: Fri Jan 26 09:05:53 2024, max compression
+gzip compressed data, was "nomad_camels_driver_andor_shamrock_500-0.1.1.tar", last modified: Tue Apr 30 13:33:15 2024, max compression
```

## Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0.tar` & `nomad_camels_driver_andor_shamrock_500-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-26 09:05:53.754550 nomad_camels_driver_andor_shamrock_500-0.1.0/
--rw-rw-rw-   0        0        0    26525 2023-06-29 08:48:55.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1181 2024-01-26 09:05:53.752549 nomad_camels_driver_andor_shamrock_500-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      476 2024-01-26 08:45:48.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-26 09:05:53.714549 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/
--rw-rw-rw-   0        0        0        0 2023-04-14 09:15:42.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/__init__.py
--rw-rw-rw-   0        0        0     4038 2023-12-01 14:41:44.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500.py
--rw-rw-rw-   0        0        0    10660 2023-12-12 09:17:46.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_config.py
--rw-rw-rw-   0        0        0     2991 2023-12-12 09:24:07.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_config_sub.py
--rw-rw-rw-   0        0        0    15085 2024-01-10 13:48:51.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_manual_control.py
--rw-rw-rw-   0        0        0     5395 2023-12-12 10:38:41.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_ophyd.py
-drwxrwxrwx   0        0        0        0 2024-01-26 09:05:53.750548 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500.egg-info/
--rw-rw-rw-   0        0        0     1181 2024-01-26 09:05:53.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-01-26 09:05:53.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-26 09:05:53.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-01-26 09:05:53.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500.egg-info/requires.txt
--rw-rw-rw-   0        0        0       39 2024-01-26 09:05:53.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      758 2024-01-26 08:46:44.000000 nomad_camels_driver_andor_shamrock_500-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-26 09:05:53.754550 nomad_camels_driver_andor_shamrock_500-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 13:33:15.020826 nomad_camels_driver_andor_shamrock_500-0.1.1/
+-rw-rw-rw-   0        0        0    26525 2024-03-19 13:39:32.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1181 2024-04-30 13:33:15.018826 nomad_camels_driver_andor_shamrock_500-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2024-03-19 13:39:32.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 13:33:14.985826 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/
+-rw-rw-rw-   0        0        0        0 2023-04-14 09:15:42.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/__init__.py
+-rw-rw-rw-   0        0        0     4206 2024-04-30 09:55:35.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500.py
+-rw-rw-rw-   0        0        0    11209 2024-04-30 09:55:35.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_config.py
+-rw-rw-rw-   0        0        0     3024 2024-04-30 09:55:35.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_config_sub.py
+-rw-rw-rw-   0        0        0    15036 2024-04-30 09:55:35.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_manual_control.py
+-rw-rw-rw-   0        0        0     5767 2024-04-30 13:29:41.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_ophyd.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:33:15.017826 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500.egg-info/
+-rw-rw-rw-   0        0        0     1181 2024-04-30 13:33:14.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-04-30 13:33:14.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 13:33:14.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-30 13:33:14.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2024-04-30 13:33:14.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      758 2024-04-30 10:04:32.000000 nomad_camels_driver_andor_shamrock_500-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 13:33:15.021825 nomad_camels_driver_andor_shamrock_500-0.1.1/setup.cfg
```

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/LICENSE.txt` & `nomad_camels_driver_andor_shamrock_500-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/PKG-INFO` & `nomad_camels_driver_andor_shamrock_500-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad_camels_driver_andor_shamrock_500
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package provides everything to run an Andor Shamrock 500 spectrometer.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
```

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500.py` & `nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,114 @@
 from nomad_camels.main_classes import device_class
 from .andor_shamrock_500_ophyd import Andor_Shamrock_500
 from nomad_camels.ui_widgets.path_button_edit import Path_Button_Edit
 from nomad_camels.ui_widgets.warn_popup import WarnPopup
 from PySide6.QtWidgets import QComboBox, QLabel
 from PySide6.QtCore import Qt
-from .andor_shamrock_500_manual_control import Andor_Manual_Control, Andor_Manual_Control_Config
+from .andor_shamrock_500_manual_control import (
+    Andor_Manual_Control,
+    Andor_Manual_Control_Config,
+)
 from .andor_shamrock_500_config_sub import subclass_config_sub
 
 
 class subclass(device_class.Device):
     def __init__(self, **kwargs):
-        super().__init__(name='andor_shamrock_500', virtual=False,
-                         tags=[ 'spectrometer', 'spectrum', 'Andor'],
-                         directory='andor_shamrock_500',
-                         ophyd_device=Andor_Shamrock_500,
-                         ophyd_class_name='Andor_Shamrock_500', **kwargs)
-        self.config['set_grating_number'] = 1
-        self.config['center_wavelength'] = 800
-        self.config['input_port'] = 'direct'
-        self.config['output_port'] = 'direct'
-        self.config['!non_string!_camera'] = ''
-        self.config['input_slit_size'] = 10
-        self.config['output_slit_size'] = 10
-
-        self.controls = {'Andor_Manual_Control': [Andor_Manual_Control,
-                                                  Andor_Manual_Control_Config]}
+        super().__init__(
+            name="andor_shamrock_500",
+            virtual=False,
+            tags=["spectrometer", "spectrum", "Andor"],
+            directory="andor_shamrock_500",
+            ophyd_device=Andor_Shamrock_500,
+            ophyd_class_name="Andor_Shamrock_500",
+            **kwargs,
+        )
+        self.config["set_grating_number"] = 1
+        self.config["center_wavelength"] = 800
+        self.config["input_port"] = "direct"
+        self.config["output_port"] = "direct"
+        self.config["!non_string!_camera"] = ""
+        self.config["input_slit_size"] = 10
+        self.config["output_slit_size"] = 10
+
+        self.controls = {
+            "Andor_Manual_Control": [Andor_Manual_Control, Andor_Manual_Control_Config]
+        }
 
     def get_necessary_devices(self):
-        return [self.config['!non_string!_camera']]
+        return [self.config["!non_string!_camera"]]
 
 
 class subclass_config(device_class.Device_Config):
-    def __init__(self, parent=None, data='', settings_dict=None, config_dict=None, additional_info=None, **kwargs):
-        super().__init__(parent, 'Andor Shamrock 500', data,
-                         settings_dict=settings_dict, config_dict=config_dict,
-                         additional_info=additional_info, **kwargs)
-        self.sub_widget = subclass_config_sub(config_dict=config_dict, parent=parent, settings_dict=settings_dict)
-        dll_label = QLabel('Path to dll (atspectrograph.dll or ShamrockCIF64.dll or ShamrockCIF.dll)')
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
+            "Andor Shamrock 500",
+            data,
+            settings_dict=settings_dict,
+            config_dict=config_dict,
+            additional_info=additional_info,
+            **kwargs,
+        )
+        self.sub_widget = subclass_config_sub(
+            config_dict=config_dict, parent=parent, settings_dict=settings_dict
+        )
+        dll_label = QLabel(
+            "Path to dll (atspectrograph.dll or ShamrockCIF64.dll or ShamrockCIF.dll)"
+        )
         self.dll_path = Path_Button_Edit()
-        label_spec = QLabel('Spectrometer:')
+        label_spec = QLabel("Spectrometer:")
         self.comboBox_spectrometer = QComboBox()
         self.spectrometer_list = []
-        if 'dll_path' in settings_dict:
-            self.dll_path.line.setText(settings_dict['dll_path'])
+        if "dll_path" in settings_dict:
+            self.dll_path.line.setText(settings_dict["dll_path"])
         self.update_dll()
-        if 'spectrometer' in settings_dict and settings_dict['spectrometer'] in self.spectrometer_list:
-            self.comboBox_spectrometer.setCurrentText(settings_dict['spectrometer'])
+        if (
+            "spectrometer" in settings_dict
+            and settings_dict["spectrometer"] in self.spectrometer_list
+        ):
+            self.comboBox_spectrometer.setCurrentText(settings_dict["spectrometer"])
         self.layout().addWidget(dll_label, 17, 0, 1, 5)
         self.layout().addWidget(self.dll_path, 18, 0, 1, 5)
         self.layout().addWidget(label_spec, 19, 0)
         self.layout().addWidget(self.comboBox_spectrometer, 19, 1, 1, 4)
         self.dll_path.path_changed.connect(self.update_dll)
 
         self.layout().addWidget(self.sub_widget, 20, 0, 1, 5)
         self.load_settings()
 
     def update_dll(self):
         self.setCursor(Qt.WaitCursor)
         dll_path = self.dll_path.get_path()
         if dll_path:
             import pylablib
-            pylablib.par['devices/dlls/andor_shamrock'] = dll_path
+
+            pylablib.par["devices/dlls/andor_shamrock"] = dll_path
             from pylablib.devices import Andor
+
             try:
                 self.spectrometer_list = Andor.list_shamrock_spectrographs()
             except Exception as e:
-                WarnPopup(self, f'Dll could not be loaded\n{e}', 'dll not loaded')
+                WarnPopup(self, f"Dll could not be loaded\n{e}", "dll not loaded")
         self.comboBox_spectrometer.clear()
         if self.spectrometer_list:
             self.comboBox_spectrometer.addItems(self.spectrometer_list)
         else:
-            self.comboBox_spectrometer.addItem('No spectrometer detected or wrong dll!')
+            self.comboBox_spectrometer.addItem("No spectrometer detected or wrong dll!")
         self.setCursor(Qt.ArrowCursor)
 
     def get_config(self):
         self.config_dict.update(self.sub_widget.get_config())
         return super().get_config()
 
     def get_settings(self):
-        self.settings_dict['dll_path'] = self.dll_path.get_path()
-        self.settings_dict['spectrometer'] = self.comboBox_spectrometer.currentText()
+        self.settings_dict["dll_path"] = self.dll_path.get_path()
+        self.settings_dict["spectrometer"] = self.comboBox_spectrometer.currentText()
         return super().get_settings()
-
```

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_config.py` & `nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,240 +1,331 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'andor_shamrock_500_config.ui'
-##
-## Created by: Qt User Interface Compiler version 6.5.1
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
-from PySide6.QtWidgets import (QApplication, QCheckBox, QComboBox, QFrame,
-    QGridLayout, QLabel, QLineEdit, QSizePolicy,
-    QSpacerItem, QSpinBox, QWidget)
-
-class Ui_andor_shamrock500_config(object):
-    def setupUi(self, andor_shamrock500_config):
-        if not andor_shamrock500_config.objectName():
-            andor_shamrock500_config.setObjectName(u"andor_shamrock500_config")
-        andor_shamrock500_config.resize(318, 310)
-        self.gridLayout = QGridLayout(andor_shamrock500_config)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.frame_2 = QFrame(andor_shamrock500_config)
-        self.frame_2.setObjectName(u"frame_2")
-        self.frame_2.setFrameShape(QFrame.StyledPanel)
-        self.frame_2.setFrameShadow(QFrame.Raised)
-        self.gridLayout_3 = QGridLayout(self.frame_2)
-        self.gridLayout_3.setObjectName(u"gridLayout_3")
-        self.lineEdit_wl_start = QLineEdit(self.frame_2)
-        self.lineEdit_wl_start.setObjectName(u"lineEdit_wl_start")
-        self.lineEdit_wl_start.setEnabled(False)
-
-        self.gridLayout_3.addWidget(self.lineEdit_wl_start, 7, 0, 1, 1)
-
-        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.gridLayout_3.addItem(self.verticalSpacer, 8, 0, 1, 1)
-
-        self.label_11 = QLabel(self.frame_2)
-        self.label_11.setObjectName(u"label_11")
-
-        self.gridLayout_3.addWidget(self.label_11, 7, 1, 1, 1)
-
-        self.lineEdit_wl_end = QLineEdit(self.frame_2)
-        self.lineEdit_wl_end.setObjectName(u"lineEdit_wl_end")
-        self.lineEdit_wl_end.setEnabled(False)
-
-        self.gridLayout_3.addWidget(self.lineEdit_wl_end, 7, 2, 1, 1)
-
-        self.initial_wavelength = QSpinBox(self.frame_2)
-        self.initial_wavelength.setObjectName(u"initial_wavelength")
-        self.initial_wavelength.setMaximum(9999)
-        self.initial_wavelength.setValue(800)
-
-        self.gridLayout_3.addWidget(self.initial_wavelength, 6, 0, 1, 3)
-
-        self.label_3 = QLabel(self.frame_2)
-        self.label_3.setObjectName(u"label_3")
-
-        self.gridLayout_3.addWidget(self.label_3, 5, 0, 1, 3)
-
-        self.set_grating_number = QSpinBox(self.frame_2)
-        self.set_grating_number.setObjectName(u"set_grating_number")
-        self.set_grating_number.setValue(1)
-
-        self.gridLayout_3.addWidget(self.set_grating_number, 4, 0, 1, 3)
-
-        self.label_2 = QLabel(self.frame_2)
-        self.label_2.setObjectName(u"label_2")
-
-        self.gridLayout_3.addWidget(self.label_2, 3, 0, 1, 3)
-
-        self.label = QLabel(self.frame_2)
-        self.label.setObjectName(u"label")
-        font = QFont()
-        font.setPointSize(9)
-        font.setBold(True)
-        self.label.setFont(font)
-
-        self.gridLayout_3.addWidget(self.label, 0, 0, 1, 3)
-
-
-        self.gridLayout.addWidget(self.frame_2, 0, 0, 1, 1)
-
-        self.frame_4 = QFrame(andor_shamrock500_config)
-        self.frame_4.setObjectName(u"frame_4")
-        self.frame_4.setFrameShape(QFrame.StyledPanel)
-        self.frame_4.setFrameShadow(QFrame.Raised)
-        self.gridLayout_5 = QGridLayout(self.frame_4)
-        self.gridLayout_5.setObjectName(u"gridLayout_5")
-        self.label_5 = QLabel(self.frame_4)
-        self.label_5.setObjectName(u"label_5")
-        font1 = QFont()
-        font1.setPointSize(10)
-        font1.setBold(True)
-        self.label_5.setFont(font1)
-
-        self.gridLayout_5.addWidget(self.label_5, 0, 0, 1, 1)
-
-        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.gridLayout_5.addItem(self.verticalSpacer_4, 3, 0, 1, 1)
-
-        self.comboBox_camera = QComboBox(self.frame_4)
-        self.comboBox_camera.setObjectName(u"comboBox_camera")
-
-        self.gridLayout_5.addWidget(self.comboBox_camera, 1, 0, 1, 1)
-
-        self.checkBox_horizontal_flip = QCheckBox(self.frame_4)
-        self.checkBox_horizontal_flip.setObjectName(u"checkBox_horizontal_flip")
-
-        self.gridLayout_5.addWidget(self.checkBox_horizontal_flip, 2, 0, 1, 1)
-
-
-        self.gridLayout.addWidget(self.frame_4, 0, 1, 1, 1)
-
-        self.frame = QFrame(andor_shamrock500_config)
-        self.frame.setObjectName(u"frame")
-        self.frame.setFrameShape(QFrame.StyledPanel)
-        self.frame.setFrameShadow(QFrame.Raised)
-        self.gridLayout_2 = QGridLayout(self.frame)
-        self.gridLayout_2.setObjectName(u"gridLayout_2")
-        self.label_4 = QLabel(self.frame)
-        self.label_4.setObjectName(u"label_4")
-
-        self.gridLayout_2.addWidget(self.label_4, 3, 0, 1, 1)
-
-        self.label_7 = QLabel(self.frame)
-        self.label_7.setObjectName(u"label_7")
-
-        self.gridLayout_2.addWidget(self.label_7, 1, 0, 1, 1)
-
-        self.input_port = QComboBox(self.frame)
-        self.input_port.addItem("")
-        self.input_port.addItem("")
-        self.input_port.setObjectName(u"input_port")
-
-        self.gridLayout_2.addWidget(self.input_port, 2, 0, 1, 1)
-
-        self.label_6 = QLabel(self.frame)
-        self.label_6.setObjectName(u"label_6")
-        self.label_6.setFont(font)
-
-        self.gridLayout_2.addWidget(self.label_6, 0, 0, 1, 1)
-
-        self.input_slit_size = QSpinBox(self.frame)
-        self.input_slit_size.setObjectName(u"input_slit_size")
-        self.input_slit_size.setMaximum(2500)
-        self.input_slit_size.setValue(10)
-
-        self.gridLayout_2.addWidget(self.input_slit_size, 4, 0, 1, 1)
-
-        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.gridLayout_2.addItem(self.verticalSpacer_2, 7, 0, 1, 1)
-
-
-        self.gridLayout.addWidget(self.frame, 1, 1, 1, 1)
-
-        self.frame_3 = QFrame(andor_shamrock500_config)
-        self.frame_3.setObjectName(u"frame_3")
-        self.frame_3.setFrameShape(QFrame.StyledPanel)
-        self.frame_3.setFrameShadow(QFrame.Raised)
-        self.gridLayout_4 = QGridLayout(self.frame_3)
-        self.gridLayout_4.setObjectName(u"gridLayout_4")
-        self.output_port = QComboBox(self.frame_3)
-        self.output_port.addItem("")
-        self.output_port.addItem("")
-        self.output_port.setObjectName(u"output_port")
-
-        self.gridLayout_4.addWidget(self.output_port, 2, 0, 1, 1)
-
-        self.label_8 = QLabel(self.frame_3)
-        self.label_8.setObjectName(u"label_8")
-        self.label_8.setFont(font)
-
-        self.gridLayout_4.addWidget(self.label_8, 0, 0, 1, 1)
-
-        self.label_9 = QLabel(self.frame_3)
-        self.label_9.setObjectName(u"label_9")
-
-        self.gridLayout_4.addWidget(self.label_9, 1, 0, 1, 1)
-
-        self.output_slit_size = QSpinBox(self.frame_3)
-        self.output_slit_size.setObjectName(u"output_slit_size")
-        self.output_slit_size.setMaximum(9999)
-
-        self.gridLayout_4.addWidget(self.output_slit_size, 4, 0, 1, 1)
-
-        self.label_10 = QLabel(self.frame_3)
-        self.label_10.setObjectName(u"label_10")
-
-        self.gridLayout_4.addWidget(self.label_10, 3, 0, 1, 1)
-
-        self.verticalSpacer_3 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.gridLayout_4.addItem(self.verticalSpacer_3, 5, 0, 1, 1)
-
-
-        self.gridLayout.addWidget(self.frame_3, 1, 0, 1, 1)
-
-        QWidget.setTabOrder(self.set_grating_number, self.initial_wavelength)
-        QWidget.setTabOrder(self.initial_wavelength, self.input_slit_size)
-        QWidget.setTabOrder(self.input_slit_size, self.output_slit_size)
-        QWidget.setTabOrder(self.output_slit_size, self.input_port)
-        QWidget.setTabOrder(self.input_port, self.output_port)
-
-        self.retranslateUi(andor_shamrock500_config)
-
-        QMetaObject.connectSlotsByName(andor_shamrock500_config)
-    # setupUi
-
-    def retranslateUi(self, andor_shamrock500_config):
-        andor_shamrock500_config.setWindowTitle(QCoreApplication.translate("andor_shamrock500_config", u"Form", None))
-        self.label_11.setText(QCoreApplication.translate("andor_shamrock500_config", u"...", None))
-        self.label_3.setText(QCoreApplication.translate("andor_shamrock500_config", u"center wavelength (nm)", None))
-        self.label_2.setText(QCoreApplication.translate("andor_shamrock500_config", u"grating number", None))
-        self.label.setText(QCoreApplication.translate("andor_shamrock500_config", u"Grating Settings", None))
-        self.label_5.setText(QCoreApplication.translate("andor_shamrock500_config", u"Camera", None))
-        self.checkBox_horizontal_flip.setText(QCoreApplication.translate("andor_shamrock500_config", u"horizontal flip", None))
-        self.label_4.setText(QCoreApplication.translate("andor_shamrock500_config", u"Input Slit Size (\u00b5m)", None))
-        self.label_7.setText(QCoreApplication.translate("andor_shamrock500_config", u"Input Port", None))
-        self.input_port.setItemText(0, QCoreApplication.translate("andor_shamrock500_config", u"side", None))
-        self.input_port.setItemText(1, QCoreApplication.translate("andor_shamrock500_config", u"direct", None))
-
-        self.label_6.setText(QCoreApplication.translate("andor_shamrock500_config", u"Input Port Settings", None))
-        self.output_port.setItemText(0, QCoreApplication.translate("andor_shamrock500_config", u"direct", None))
-        self.output_port.setItemText(1, QCoreApplication.translate("andor_shamrock500_config", u"side", None))
-
-        self.label_8.setText(QCoreApplication.translate("andor_shamrock500_config", u"Output Port Settings", None))
-        self.label_9.setText(QCoreApplication.translate("andor_shamrock500_config", u"Output Port", None))
-        self.label_10.setText(QCoreApplication.translate("andor_shamrock500_config", u"Output Slite Size", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'andor_shamrock_500_config.ui'
+##
+## Created by: Qt User Interface Compiler version 6.5.1
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
+    QApplication,
+    QCheckBox,
+    QComboBox,
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
+class Ui_andor_shamrock500_config(object):
+    def setupUi(self, andor_shamrock500_config):
+        if not andor_shamrock500_config.objectName():
+            andor_shamrock500_config.setObjectName("andor_shamrock500_config")
+        andor_shamrock500_config.resize(318, 310)
+        self.gridLayout = QGridLayout(andor_shamrock500_config)
+        self.gridLayout.setObjectName("gridLayout")
+        self.frame_2 = QFrame(andor_shamrock500_config)
+        self.frame_2.setObjectName("frame_2")
+        self.frame_2.setFrameShape(QFrame.StyledPanel)
+        self.frame_2.setFrameShadow(QFrame.Raised)
+        self.gridLayout_3 = QGridLayout(self.frame_2)
+        self.gridLayout_3.setObjectName("gridLayout_3")
+        self.lineEdit_wl_start = QLineEdit(self.frame_2)
+        self.lineEdit_wl_start.setObjectName("lineEdit_wl_start")
+        self.lineEdit_wl_start.setEnabled(False)
+
+        self.gridLayout_3.addWidget(self.lineEdit_wl_start, 7, 0, 1, 1)
+
+        self.verticalSpacer = QSpacerItem(
+            20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding
+        )
+
+        self.gridLayout_3.addItem(self.verticalSpacer, 8, 0, 1, 1)
+
+        self.label_11 = QLabel(self.frame_2)
+        self.label_11.setObjectName("label_11")
+
+        self.gridLayout_3.addWidget(self.label_11, 7, 1, 1, 1)
+
+        self.lineEdit_wl_end = QLineEdit(self.frame_2)
+        self.lineEdit_wl_end.setObjectName("lineEdit_wl_end")
+        self.lineEdit_wl_end.setEnabled(False)
+
+        self.gridLayout_3.addWidget(self.lineEdit_wl_end, 7, 2, 1, 1)
+
+        self.initial_wavelength = QSpinBox(self.frame_2)
+        self.initial_wavelength.setObjectName("initial_wavelength")
+        self.initial_wavelength.setMaximum(9999)
+        self.initial_wavelength.setValue(800)
+
+        self.gridLayout_3.addWidget(self.initial_wavelength, 6, 0, 1, 3)
+
+        self.label_3 = QLabel(self.frame_2)
+        self.label_3.setObjectName("label_3")
+
+        self.gridLayout_3.addWidget(self.label_3, 5, 0, 1, 3)
+
+        self.set_grating_number = QSpinBox(self.frame_2)
+        self.set_grating_number.setObjectName("set_grating_number")
+        self.set_grating_number.setValue(1)
+
+        self.gridLayout_3.addWidget(self.set_grating_number, 4, 0, 1, 3)
+
+        self.label_2 = QLabel(self.frame_2)
+        self.label_2.setObjectName("label_2")
+
+        self.gridLayout_3.addWidget(self.label_2, 3, 0, 1, 3)
+
+        self.label = QLabel(self.frame_2)
+        self.label.setObjectName("label")
+        font = QFont()
+        font.setPointSize(9)
+        font.setBold(True)
+        self.label.setFont(font)
+
+        self.gridLayout_3.addWidget(self.label, 0, 0, 1, 3)
+
+        self.gridLayout.addWidget(self.frame_2, 0, 0, 1, 1)
+
+        self.frame_4 = QFrame(andor_shamrock500_config)
+        self.frame_4.setObjectName("frame_4")
+        self.frame_4.setFrameShape(QFrame.StyledPanel)
+        self.frame_4.setFrameShadow(QFrame.Raised)
+        self.gridLayout_5 = QGridLayout(self.frame_4)
+        self.gridLayout_5.setObjectName("gridLayout_5")
+        self.label_5 = QLabel(self.frame_4)
+        self.label_5.setObjectName("label_5")
+        font1 = QFont()
+        font1.setPointSize(10)
+        font1.setBold(True)
+        self.label_5.setFont(font1)
+
+        self.gridLayout_5.addWidget(self.label_5, 0, 0, 1, 1)
+
+        self.verticalSpacer_4 = QSpacerItem(
+            20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding
+        )
+
+        self.gridLayout_5.addItem(self.verticalSpacer_4, 3, 0, 1, 1)
+
+        self.comboBox_camera = QComboBox(self.frame_4)
+        self.comboBox_camera.setObjectName("comboBox_camera")
+
+        self.gridLayout_5.addWidget(self.comboBox_camera, 1, 0, 1, 1)
+
+        self.checkBox_horizontal_flip = QCheckBox(self.frame_4)
+        self.checkBox_horizontal_flip.setObjectName("checkBox_horizontal_flip")
+
+        self.gridLayout_5.addWidget(self.checkBox_horizontal_flip, 2, 0, 1, 1)
+
+        self.gridLayout.addWidget(self.frame_4, 0, 1, 1, 1)
+
+        self.frame = QFrame(andor_shamrock500_config)
+        self.frame.setObjectName("frame")
+        self.frame.setFrameShape(QFrame.StyledPanel)
+        self.frame.setFrameShadow(QFrame.Raised)
+        self.gridLayout_2 = QGridLayout(self.frame)
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.label_4 = QLabel(self.frame)
+        self.label_4.setObjectName("label_4")
+
+        self.gridLayout_2.addWidget(self.label_4, 3, 0, 1, 1)
+
+        self.label_7 = QLabel(self.frame)
+        self.label_7.setObjectName("label_7")
+
+        self.gridLayout_2.addWidget(self.label_7, 1, 0, 1, 1)
+
+        self.input_port = QComboBox(self.frame)
+        self.input_port.addItem("")
+        self.input_port.addItem("")
+        self.input_port.setObjectName("input_port")
+
+        self.gridLayout_2.addWidget(self.input_port, 2, 0, 1, 1)
+
+        self.label_6 = QLabel(self.frame)
+        self.label_6.setObjectName("label_6")
+        self.label_6.setFont(font)
+
+        self.gridLayout_2.addWidget(self.label_6, 0, 0, 1, 1)
+
+        self.input_slit_size = QSpinBox(self.frame)
+        self.input_slit_size.setObjectName("input_slit_size")
+        self.input_slit_size.setMaximum(2500)
+        self.input_slit_size.setValue(10)
+
+        self.gridLayout_2.addWidget(self.input_slit_size, 4, 0, 1, 1)
+
+        self.verticalSpacer_2 = QSpacerItem(
+            20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding
+        )
+
+        self.gridLayout_2.addItem(self.verticalSpacer_2, 7, 0, 1, 1)
+
+        self.gridLayout.addWidget(self.frame, 1, 1, 1, 1)
+
+        self.frame_3 = QFrame(andor_shamrock500_config)
+        self.frame_3.setObjectName("frame_3")
+        self.frame_3.setFrameShape(QFrame.StyledPanel)
+        self.frame_3.setFrameShadow(QFrame.Raised)
+        self.gridLayout_4 = QGridLayout(self.frame_3)
+        self.gridLayout_4.setObjectName("gridLayout_4")
+        self.output_port = QComboBox(self.frame_3)
+        self.output_port.addItem("")
+        self.output_port.addItem("")
+        self.output_port.setObjectName("output_port")
+
+        self.gridLayout_4.addWidget(self.output_port, 2, 0, 1, 1)
+
+        self.label_8 = QLabel(self.frame_3)
+        self.label_8.setObjectName("label_8")
+        self.label_8.setFont(font)
+
+        self.gridLayout_4.addWidget(self.label_8, 0, 0, 1, 1)
+
+        self.label_9 = QLabel(self.frame_3)
+        self.label_9.setObjectName("label_9")
+
+        self.gridLayout_4.addWidget(self.label_9, 1, 0, 1, 1)
+
+        self.output_slit_size = QSpinBox(self.frame_3)
+        self.output_slit_size.setObjectName("output_slit_size")
+        self.output_slit_size.setMaximum(9999)
+
+        self.gridLayout_4.addWidget(self.output_slit_size, 4, 0, 1, 1)
+
+        self.label_10 = QLabel(self.frame_3)
+        self.label_10.setObjectName("label_10")
+
+        self.gridLayout_4.addWidget(self.label_10, 3, 0, 1, 1)
+
+        self.verticalSpacer_3 = QSpacerItem(
+            20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding
+        )
+
+        self.gridLayout_4.addItem(self.verticalSpacer_3, 5, 0, 1, 1)
+
+        self.gridLayout.addWidget(self.frame_3, 1, 0, 1, 1)
+
+        QWidget.setTabOrder(self.set_grating_number, self.initial_wavelength)
+        QWidget.setTabOrder(self.initial_wavelength, self.input_slit_size)
+        QWidget.setTabOrder(self.input_slit_size, self.output_slit_size)
+        QWidget.setTabOrder(self.output_slit_size, self.input_port)
+        QWidget.setTabOrder(self.input_port, self.output_port)
+
+        self.retranslateUi(andor_shamrock500_config)
+
+        QMetaObject.connectSlotsByName(andor_shamrock500_config)
+
+    # setupUi
+
+    def retranslateUi(self, andor_shamrock500_config):
+        andor_shamrock500_config.setWindowTitle(
+            QCoreApplication.translate("andor_shamrock500_config", "Form", None)
+        )
+        self.label_11.setText(
+            QCoreApplication.translate("andor_shamrock500_config", "...", None)
+        )
+        self.label_3.setText(
+            QCoreApplication.translate(
+                "andor_shamrock500_config", "center wavelength (nm)", None
+            )
+        )
+        self.label_2.setText(
+            QCoreApplication.translate(
+                "andor_shamrock500_config", "grating number", None
+            )
+        )
+        self.label.setText(
+            QCoreApplication.translate(
+                "andor_shamrock500_config", "Grating Settings", None
+            )
+        )
+        self.label_5.setText(
+            QCoreApplication.translate("andor_shamrock500_config", "Camera", None)
+        )
+        self.checkBox_horizontal_flip.setText(
+            QCoreApplication.translate(
+                "andor_shamrock500_config", "horizontal flip", None
+            )
+        )
+        self.label_4.setText(
+            QCoreApplication.translate(
+                "andor_shamrock500_config", "Input Slit Size (\u00b5m)", None
+            )
+        )
+        self.label_7.setText(
+            QCoreApplication.translate("andor_shamrock500_config", "Input Port", None)
+        )
+        self.input_port.setItemText(
+            0, QCoreApplication.translate("andor_shamrock500_config", "side", None)
+        )
+        self.input_port.setItemText(
+            1, QCoreApplication.translate("andor_shamrock500_config", "direct", None)
+        )
+
+        self.label_6.setText(
+            QCoreApplication.translate(
+                "andor_shamrock500_config", "Input Port Settings", None
+            )
+        )
+        self.output_port.setItemText(
+            0, QCoreApplication.translate("andor_shamrock500_config", "direct", None)
+        )
+        self.output_port.setItemText(
+            1, QCoreApplication.translate("andor_shamrock500_config", "side", None)
+        )
+
+        self.label_8.setText(
+            QCoreApplication.translate(
+                "andor_shamrock500_config", "Output Port Settings", None
+            )
+        )
+        self.label_9.setText(
+            QCoreApplication.translate("andor_shamrock500_config", "Output Port", None)
+        )
+        self.label_10.setText(
+            QCoreApplication.translate(
+                "andor_shamrock500_config", "Output Slite Size", None
+            )
+        )
+
+    # retranslateUi
```

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_config_sub.py` & `nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_config_sub.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,60 @@
-from .andor_shamrock_500_config import Ui_andor_shamrock500_config
-from nomad_camels.utility import variables_handling
-from nomad_camels.main_classes import device_class
-
-
-class subclass_config_sub(device_class.Device_Config_Sub, Ui_andor_shamrock500_config):
-    def __init__(self, config_dict=None, parent=None, settings_dict=None):
-        super().__init__(parent=parent, config_dict=config_dict,
-                         settings_dict=settings_dict)
-        self.setupUi(self)
-        devs = list(variables_handling.devices.keys())
-        self.comboBox_camera.addItems(devs)
-        self.load_config()
-
-    def load_config(self):
-        if 'set_grating_number' in self.config_dict:
-            self.set_grating_number.setValue(self.config_dict['set_grating_number'])
-        if 'center_wavelength' in self.config_dict:
-            self.initial_wavelength.setValue(self.config_dict['center_wavelength'])
-        if 'input_port' in self.config_dict:
-            self.input_port.setCurrentText(self.config_dict['input_port'])
-        if 'output_port' in self.config_dict:
-            self.output_port.setCurrentText(self.config_dict['output_port'])
-        if 'input_slit_size' in self.config_dict:
-            self.input_slit_size.setValue(self.config_dict['input_slit_size'])
-        if 'output_slit_size' in self.config_dict:
-            self.output_slit_size.setValue(self.config_dict['output_slit_size'])
-        devs = list(variables_handling.devices.keys())
-        if '!non_string!_camera' in self.config_dict and self.config_dict['!non_string!_camera'] in devs:
-            self.comboBox_camera.setCurrentText(self.config_dict['!non_string!_camera'])
-        if 'horizontal_cam_flip' in self.config_dict:
-            self.checkBox_horizontal_flip.setChecked(self.config_dict['horizontal_cam_flip'])
-        if 'wavelength' in self.config_dict:
-            wl = self.config_dict['wavelength']
-            self.lineEdit_wl_end.setText(f'{max(wl):.2f}')
-            self.lineEdit_wl_start.setText(f'{min(wl):.2f}')
-            self.lineEdit_wl_end.setHidden(False)
-            self.lineEdit_wl_start.setHidden(False)
-        else:
-            self.lineEdit_wl_end.setHidden(True)
-            self.lineEdit_wl_start.setHidden(True)
-
-
-    def get_config(self):
-        self.config_dict['set_grating_number'] = self.set_grating_number.value()
-        self.config_dict['center_wavelength'] = self.initial_wavelength.value()
-        self.config_dict['input_port'] = self.input_port.currentText()
-        self.config_dict['output_port'] = self.output_port.currentText()
-        self.config_dict['!non_string!_camera'] = self.comboBox_camera.currentText()
-        self.config_dict['input_slit_size'] = self.input_slit_size.value()
-        self.config_dict['output_slit_size'] = self.output_slit_size.value()
-        self.config_dict['horizontal_cam_flip'] = self.checkBox_horizontal_flip.isChecked()
-        return super().get_config()
+from .andor_shamrock_500_config import Ui_andor_shamrock500_config
+from nomad_camels.utility import variables_handling
+from nomad_camels.main_classes import device_class
+
+
+class subclass_config_sub(device_class.Device_Config_Sub, Ui_andor_shamrock500_config):
+    def __init__(self, config_dict=None, parent=None, settings_dict=None):
+        super().__init__(
+            parent=parent, config_dict=config_dict, settings_dict=settings_dict
+        )
+        self.setupUi(self)
+        devs = list(variables_handling.devices.keys())
+        self.comboBox_camera.addItems(devs)
+        self.load_config()
+
+    def load_config(self):
+        if "set_grating_number" in self.config_dict:
+            self.set_grating_number.setValue(self.config_dict["set_grating_number"])
+        if "center_wavelength" in self.config_dict:
+            self.initial_wavelength.setValue(self.config_dict["center_wavelength"])
+        if "input_port" in self.config_dict:
+            self.input_port.setCurrentText(self.config_dict["input_port"])
+        if "output_port" in self.config_dict:
+            self.output_port.setCurrentText(self.config_dict["output_port"])
+        if "input_slit_size" in self.config_dict:
+            self.input_slit_size.setValue(self.config_dict["input_slit_size"])
+        if "output_slit_size" in self.config_dict:
+            self.output_slit_size.setValue(self.config_dict["output_slit_size"])
+        devs = list(variables_handling.devices.keys())
+        if (
+            "!non_string!_camera" in self.config_dict
+            and self.config_dict["!non_string!_camera"] in devs
+        ):
+            self.comboBox_camera.setCurrentText(self.config_dict["!non_string!_camera"])
+        if "horizontal_cam_flip" in self.config_dict:
+            self.checkBox_horizontal_flip.setChecked(
+                self.config_dict["horizontal_cam_flip"]
+            )
+        if "wavelength" in self.config_dict:
+            wl = self.config_dict["wavelength"]
+            self.lineEdit_wl_end.setText(f"{max(wl):.2f}")
+            self.lineEdit_wl_start.setText(f"{min(wl):.2f}")
+            self.lineEdit_wl_end.setHidden(False)
+            self.lineEdit_wl_start.setHidden(False)
+        else:
+            self.lineEdit_wl_end.setHidden(True)
+            self.lineEdit_wl_start.setHidden(True)
+
+    def get_config(self):
+        self.config_dict["set_grating_number"] = self.set_grating_number.value()
+        self.config_dict["center_wavelength"] = self.initial_wavelength.value()
+        self.config_dict["input_port"] = self.input_port.currentText()
+        self.config_dict["output_port"] = self.output_port.currentText()
+        self.config_dict["!non_string!_camera"] = self.comboBox_camera.currentText()
+        self.config_dict["input_slit_size"] = self.input_slit_size.value()
+        self.config_dict["output_slit_size"] = self.output_slit_size.value()
+        self.config_dict["horizontal_cam_flip"] = (
+            self.checkBox_horizontal_flip.isChecked()
+        )
+        return super().get_config()
```

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_manual_control.py` & `nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_manual_control.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,366 +1,409 @@
-import importlib
-import time
-
-import numpy as np
-from nomad_camels.main_classes.manual_control import Manual_Control, Manual_Control_Config
-from .andor_shamrock_500_config_sub import subclass_config_sub
-from nomad_camels.main_classes.plot_widget import PlotWidget_NoBluesky
-from nomad_camels.ui_widgets.warn_popup import WarnPopup
-
-from PySide6.QtWidgets import QCheckBox, QPushButton, QLabel, QComboBox, QGridLayout, QWidget, QFileDialog
-from PySide6.QtCore import Signal, QThread, Qt
-
-from nomad_camels.utility import variables_handling
-
-
-class Andor_Manual_Control(Manual_Control):
-    def __init__(self, parent=None, control_data=None):
-        control_data = control_data or {}
-        if 'name' in control_data:
-            name = control_data['name']
-        else:
-            name = 'Andor Spectrometer - Manual Control'
-        super().__init__(parent=parent, title=name)
-        self.setLayout(QGridLayout())
-        self.device = variables_handling.devices[control_data['spectrometer']]
-
-        self.settings_widge = subclass_config_sub(parent=self, config_dict=self.device.config)
-        self.camera = variables_handling.devices[control_data['camera']]
-        cam_type = self.camera.name
-        py_package = importlib.import_module(f'nomad_camels_driver_{cam_type}.{cam_type}')
-        self.camera_widge = py_package.subclass_config_sub(parent=self, config_dict=self.camera.config)
-
-        self.layout().addWidget(self.settings_widge, 0, 0)
-        self.layout().addWidget(self.camera_widge, 0, 1)
-
-        self.meas_widget = QWidget()
-        lay = QGridLayout()
-        self.meas_widget.setLayout(lay)
-        self.acquire_button = QPushButton('acquire spectrum')
-        self.continuous_button = QPushButton('continuous spectra')
-        self.save_button = QPushButton('save spectrum')
-        self.checkBox_clear_plot = QCheckBox('clear plot every spectrum')
-        self.checkBox_clear_plot.setChecked(True)
-        lay.addWidget(self.save_button, 0, 0)
-        lay.addWidget(self.checkBox_clear_plot, 0, 1)
-        lay.addWidget(self.continuous_button, 0, 2)
-        lay.addWidget(self.acquire_button, 0, 3)
-
-        self.layout().addWidget(self.meas_widget, 1, 0, 1, 2)
-
-        self.spectrum_plot = PlotWidget_NoBluesky('wavelength (nm)',
-                                                  'intensity (counts)',
-                                                  title='Spectrum')
-        self.image_plot = None
-        self.current_data = {}
-
-        self.acquire_button.clicked.connect(self.measure_spectrum)
-        self.continuous_meas = False
-        self.continuous_button.clicked.connect(self.continuous_spectra)
-
-        self.settings_widge.set_grating_number.lineEdit().returnPressed.connect(self.set_grating)
-        self.settings_widge.initial_wavelength.lineEdit().returnPressed.connect(self.set_wavelength)
-        self.settings_widge.input_port.currentTextChanged.connect(self.set_input_port)
-        self.settings_widge.output_port.currentTextChanged.connect(self.set_output_port)
-        self.settings_widge.input_slit_size.lineEdit().returnPressed.connect(self.set_input_slit_size)
-        self.settings_widge.output_slit_size.lineEdit().returnPressed.connect(self.set_output_slit_size)
-        self.settings_widge.checkBox_horizontal_flip.clicked.connect(self.set_horizontal_flip)
-        self.camera_widge.config_changed.connect(self.change_camera_config)
-        self.save_button.clicked.connect(self.save_spectrum)
-
-        self.spectrometer_thread = None
-        self.start_device(control_data['spectrometer'])
-
-
-    def device_ready(self):
-        super().device_ready()
-        self.spectrometer_thread = Spectrometer_Work_Thread(self, self.ophyd_device)
-        self.spectrometer_thread.job_done.connect(self.stop_job)
-        self.spectrometer_thread.spectrum_data_signal.connect(self.show_spectrum)
-        self.spectrometer_thread.new_cam_config.connect(self.update_cam_config)
-        self.spectrometer_thread.new_spec_config.connect(self.update_config)
-        self.spectrometer_thread.start()
-    
-    def save_spectrum(self):
-        if not self.current_data:
-            return
-        file = QFileDialog.getSaveFileName(self, 'Save Spectrum', '*.txt')[0]
-        if not file:
-            return
-        import numpy as np
-        if self.current_data['intensity'].ndim > 1:
-            arr = np.column_stack([self.current_data['wavelength'], self.current_data['intensity'].transpose()])
-        else:
-            arr = np.stack([self.current_data['wavelength'], self.current_data['intensity']]).transpose()
-        np.savetxt(file, arr, delimiter='\t', header='wavelength (nm)\t(intensity)')
-
-
-    def update_config(self, config_dict):
-        self.settings_widge.config_dict = config_dict
-        self.settings_widge.load_config()
-
-    def update_cam_config(self, config_dict):
-        self.camera_widge.config_dict = config_dict
-        self.camera_widge.load_config()
-
-    def start_job(self):
-        self.setCursor(Qt.WaitCursor)
-        self.setEnabled(False)
-
-    def stop_job(self):
-        self.setCursor(Qt.ArrowCursor)
-        self.setEnabled(True)
-
-    def set_grating(self):
-        val = self.settings_widge.set_grating_number.value()
-        self.spectrometer_thread.do_function('set_grating', val)
-        self.start_job()
-
-    def set_wavelength(self):
-        val = self.settings_widge.initial_wavelength.value()
-        self.spectrometer_thread.do_function('set_wavelength', val)
-        self.start_job()
-
-    def set_input_port(self):
-        val = self.settings_widge.input_port.currentText()
-        self.spectrometer_thread.do_function('set_input_port', val)
-        self.start_job()
-
-    def set_output_port(self):
-        val = self.settings_widge.output_port.currentText()
-        self.spectrometer_thread.do_function('set_output_port', val)
-        self.start_job()
-
-    def set_input_slit_size(self):
-        val = self.settings_widge.input_slit_size.value()
-        self.spectrometer_thread.do_function('set_input_slit_size', val)
-        self.start_job()
-
-    def set_output_slit_size(self):
-        val = self.settings_widge.output_slit_size.value()
-        self.spectrometer_thread.do_function('set_output_slit_size', val)
-        self.start_job()
-    
-    def set_horizontal_flip(self):
-        self.ophyd_device.horizontal_cam_flip.put(self.settings_widge.checkBox_horizontal_flip.isChecked())
-
-    def measure_spectrum(self):
-        self.spectrometer_thread.do_function('measure_spectrum', None)
-        self.start_job()
-
-    def show_spectrum(self, wl, intensity):
-        try:
-            self.current_data['intensity'] = intensity
-            self.current_data['wavelength'] = wl
-            if intensity.ndim > 1:
-                if self.image_plot is None:
-                    import matplotlib.pyplot as plt
-                    self.image_plot = plt.subplots()
-                x, y = np.meshgrid(wl, range(len(intensity)))
-                self.image_plot[1].clear()
-                self.image_plot[1].pcolormesh(x, y, intensity)
-                self.image_plot[0].show()
-            else:
-                self.spectrum_plot.plot.add_data(wl, {'intensity': intensity},
-                                                 add=not self.checkBox_clear_plot.isChecked())
-                self.spectrum_plot.show()
-        except Exception as e:
-            WarnPopup(self, str(e), 'error')
-
-    def continuous_spectra(self):
-        if not self.continuous_meas:
-            self.setCursor(Qt.WaitCursor)
-            self.continuous_button.setText('stop acquisition')
-            self.acquire_button.setEnabled(False)
-            self.save_button.setEnabled(False)
-            self.settings_widge.setEnabled(False)
-            self.camera_widge.setEnabled(False)
-            self.continuous_meas = True
-            self.spectrometer_thread.continuous = True
-        else:
-            self.spectrometer_thread.continuous = False
-            self.setCursor(Qt.ArrowCursor)
-            self.continuous_button.setText('continuous spectra')
-            self.acquire_button.setEnabled(True)
-            self.save_button.setEnabled(True)
-            self.settings_widge.setEnabled(True)
-            self.camera_widge.setEnabled(True)
-            self.continuous_meas = False
-
-    def change_camera_config(self, x, conf):
-        configs = self.camera_widge.get_config()
-        value = configs[conf]
-        self.spectrometer_thread.do_function('change_camera_config', [value, conf])
-        self.start_job()
-
-    def close(self) -> bool:
-        self.spectrometer_thread.still_running = False
-        self.spectrometer_thread.continuous = False
-        return super().close()
-
-    def closeEvent(self, a0):
-        self.spectrometer_thread.still_running = False
-        self.spectrometer_thread.continuous = False
-        self.spectrum_plot.close()
-        if self.image_plot is not None:
-            import matplotlib.pyplot as plt
-            plt.close(self.image_plot[0])
-            self.image_plot = None
-        return super().closeEvent(a0)
-
-
-class Spectrometer_Work_Thread(QThread):
-    job_done = Signal()
-    spectrum_data_signal = Signal(object, object)
-    new_spec_config = Signal(dict)
-    new_cam_config = Signal(dict)
-
-    def __init__(self, parent=None, spectrometer=None):
-        super().__init__(parent=parent)
-        self.spectrometer = spectrometer
-        self.still_running = True
-        self.continuous = False
-        self.function_to_do = None
-        self.function_value = None
-        self.last_config = None
-        self.last_cam_config = None
-
-    def run(self):
-        i = 100
-        while self.still_running:
-            time.sleep(0.1)
-            if self.function_to_do:
-                getattr(self, self.function_to_do)(self.function_value)
-                self.function_to_do = None
-                self.function_value = None
-                self.job_done.emit()
-            if self.continuous:
-                self.continuous_function()
-            if i >= 100:
-                self.update_configs()
-                i = 0
-            i += 1
-
-    def update_configs(self):
-        spec_config = self.spectrometer.read_configuration()
-        cam_config = self.spectrometer.get_camera_device().read_configuration()
-        if spec_config != self.last_config:
-            self.last_config = spec_config
-            conf = {}
-            name = self.spectrometer.name
-            for k, v in spec_config.items():
-                conf[k.split(f'{name}_')[1]] = v['value']
-            conf['wavelength'] = self.spectrometer.wavelength.get()
-            self.new_spec_config.emit(conf)
-        if cam_config != self.last_cam_config:
-            name = self.spectrometer.get_camera_device().name
-            conf = {}
-            for k, v in cam_config.items():
-                conf[k.split(f'{name}_')[1]] = v['value']
-            self.last_cam_config = cam_config
-            self.new_cam_config.emit(conf)
-
-    def do_function(self, name, value):
-        self.function_to_do = name
-        self.function_value = value
-
-    def set_grating(self, value):
-        try:
-            self.spectrometer.set_grating_number.put(value)
-        except Exception as e:
-            WarnPopup(None, str(e), 'error')
-
-    def set_wavelength(self, value):
-        try:
-            self.spectrometer.center_wavelength.put(value)
-        except Exception as e:
-            WarnPopup(None, str(e), 'error')
-
-    def set_input_port(self, value):
-        try:
-            self.spectrometer.input_port.put(value)
-        except Exception as e:
-            WarnPopup(None, str(e), 'error')
-
-    def set_output_port(self, value):
-        try:
-            self.spectrometer.output_port.put(value)
-        except Exception as e:
-            WarnPopup(None, str(e), 'error')
-
-    def set_input_slit_size(self, value):
-        try:
-            self.spectrometer.input_slit_size.put(value)
-        except Exception as e:
-            WarnPopup(None, str(e), 'error')
-
-    def set_output_slit_size(self, value):
-        try:
-            self.spectrometer.output_slit_size.put(value)
-        except Exception as e:
-            WarnPopup(None, str(e), 'error')
-
-    def measure_spectrum(self, value):
-        try:
-            intensity = self.spectrometer.spectrum.get()
-            wl = self.spectrometer.wavelength.get()
-            self.spectrum_data_signal.emit(wl, intensity)
-        except Exception as e:
-            WarnPopup(None, str(e), 'error')
-
-    def continuous_function(self):
-        cam = self.spectrometer.get_camera_device().camera
-        cam.start_acquisition()
-        while self.continuous:
-            time.sleep(0.1)
-            im = cam.read_newest_image()
-            if im is not None:
-                wl = self.spectrometer.wavelength.get()
-                if len(im) == 1:
-                    im = im[0]
-                self.spectrum_data_signal.emit(wl, im)
-
-    def change_camera_config(self, value):
-        value, conf = value
-        try:
-            cam = self.spectrometer.get_camera_device()
-            set_signal = getattr(cam, conf)
-            set_signal.put(value)
-        except Exception as e:
-            WarnPopup(None, str(e), 'error')
-
-
-class Andor_Manual_Control_Config(Manual_Control_Config):
-    def __init__(self, parent=None, control_data=None):
-        super().__init__(parent=parent, control_data=control_data,
-                         title='Spectrometer control config',
-                         control_type='Andor_Manual_Control')
-        control_data = control_data or {}
-        select_label = QLabel('Spectrometer:')
-        cam_label = QLabel('Camera:')
-
-        self.spec_box = QComboBox()
-        specs = []
-        for name, device in variables_handling.devices.items():
-            if device.name == 'andor_shamrock_500':
-                specs.append(name)
-        self.spec_box.addItems(specs)
-        if 'spectrometer' in control_data and control_data['spectrometer'] in specs:
-            self.spec_box.setCurrentText(control_data['spectrometer'])
-
-        self.cam_box = QComboBox()
-        cams = []
-        for name, device in variables_handling.devices.items():
-            cams.append(name)
-        self.cam_box.addItems(cams)
-        if 'camera' in control_data and control_data['camera'] in cams:
-            self.cam_box.setCurrentText(control_data['camera'])
-        self.layout().addWidget(select_label, 2, 0)
-        self.layout().addWidget(self.spec_box, 2, 1)
-        self.layout().addWidget(cam_label, 3, 0)
-        self.layout().addWidget(self.cam_box, 3, 1)
-
-    def accept(self):
-        self.control_data['spectrometer'] = self.spec_box.currentText()
-        self.control_data['camera'] = self.cam_box.currentText()
-        super().accept()
+import importlib
+import time
+
+import numpy as np
+from nomad_camels.main_classes.manual_control import (
+    Manual_Control,
+    Manual_Control_Config,
+)
+from .andor_shamrock_500_config_sub import subclass_config_sub
+from nomad_camels.main_classes.plot_widget import PlotWidget_NoBluesky
+from nomad_camels.ui_widgets.warn_popup import WarnPopup
+
+from PySide6.QtWidgets import (
+    QCheckBox,
+    QPushButton,
+    QLabel,
+    QComboBox,
+    QGridLayout,
+    QWidget,
+    QFileDialog,
+)
+from PySide6.QtCore import Signal, QThread, Qt
+
+from nomad_camels.utility import variables_handling
+
+
+class Andor_Manual_Control(Manual_Control):
+    def __init__(self, parent=None, control_data=None):
+        control_data = control_data or {}
+        if "name" in control_data:
+            name = control_data["name"]
+        else:
+            name = "Andor Spectrometer - Manual Control"
+        super().__init__(parent=parent, title=name)
+        self.setLayout(QGridLayout())
+        self.device = variables_handling.devices[control_data["spectrometer"]]
+
+        self.settings_widge = subclass_config_sub(
+            parent=self, config_dict=self.device.config
+        )
+        self.camera = variables_handling.devices[control_data["camera"]]
+        cam_type = self.camera.name
+        py_package = importlib.import_module(
+            f"nomad_camels_driver_{cam_type}.{cam_type}"
+        )
+        self.camera_widge = py_package.subclass_config_sub(
+            parent=self, config_dict=self.camera.config
+        )
+
+        self.layout().addWidget(self.settings_widge, 0, 0)
+        self.layout().addWidget(self.camera_widge, 0, 1)
+
+        self.meas_widget = QWidget()
+        lay = QGridLayout()
+        self.meas_widget.setLayout(lay)
+        self.acquire_button = QPushButton("acquire spectrum")
+        self.continuous_button = QPushButton("continuous spectra")
+        self.save_button = QPushButton("save spectrum")
+        self.checkBox_clear_plot = QCheckBox("clear plot every spectrum")
+        self.checkBox_clear_plot.setChecked(True)
+        lay.addWidget(self.save_button, 0, 0)
+        lay.addWidget(self.checkBox_clear_plot, 0, 1)
+        lay.addWidget(self.continuous_button, 0, 2)
+        lay.addWidget(self.acquire_button, 0, 3)
+
+        self.layout().addWidget(self.meas_widget, 1, 0, 1, 2)
+
+        self.spectrum_plot = PlotWidget_NoBluesky(
+            "wavelength (nm)", "intensity (counts)", title="Spectrum"
+        )
+        self.image_plot = None
+        self.current_data = {}
+
+        self.acquire_button.clicked.connect(self.measure_spectrum)
+        self.continuous_meas = False
+        self.continuous_button.clicked.connect(self.continuous_spectra)
+
+        self.settings_widge.set_grating_number.lineEdit().returnPressed.connect(
+            self.set_grating
+        )
+        self.settings_widge.initial_wavelength.lineEdit().returnPressed.connect(
+            self.set_wavelength
+        )
+        self.settings_widge.input_port.currentTextChanged.connect(self.set_input_port)
+        self.settings_widge.output_port.currentTextChanged.connect(self.set_output_port)
+        self.settings_widge.input_slit_size.lineEdit().returnPressed.connect(
+            self.set_input_slit_size
+        )
+        self.settings_widge.output_slit_size.lineEdit().returnPressed.connect(
+            self.set_output_slit_size
+        )
+        self.settings_widge.checkBox_horizontal_flip.clicked.connect(
+            self.set_horizontal_flip
+        )
+        self.camera_widge.config_changed.connect(self.change_camera_config)
+        self.save_button.clicked.connect(self.save_spectrum)
+
+        self.spectrometer_thread = None
+        self.start_device(control_data["spectrometer"])
+
+    def device_ready(self):
+        super().device_ready()
+        self.spectrometer_thread = Spectrometer_Work_Thread(self, self.ophyd_device)
+        self.spectrometer_thread.job_done.connect(self.stop_job)
+        self.spectrometer_thread.spectrum_data_signal.connect(self.show_spectrum)
+        self.spectrometer_thread.new_cam_config.connect(self.update_cam_config)
+        self.spectrometer_thread.new_spec_config.connect(self.update_config)
+        self.spectrometer_thread.start()
+
+    def save_spectrum(self):
+        if not self.current_data:
+            return
+        file = QFileDialog.getSaveFileName(self, "Save Spectrum", "*.txt")[0]
+        if not file:
+            return
+        import numpy as np
+
+        if self.current_data["intensity"].ndim > 1:
+            arr = np.column_stack(
+                [
+                    self.current_data["wavelength"],
+                    self.current_data["intensity"].transpose(),
+                ]
+            )
+        else:
+            arr = np.stack(
+                [self.current_data["wavelength"], self.current_data["intensity"]]
+            ).transpose()
+        np.savetxt(file, arr, delimiter="\t", header="wavelength (nm)\t(intensity)")
+
+    def update_config(self, config_dict):
+        self.settings_widge.config_dict = config_dict
+        self.settings_widge.load_config()
+
+    def update_cam_config(self, config_dict):
+        self.camera_widge.config_dict = config_dict
+        self.camera_widge.load_config()
+
+    def start_job(self):
+        self.setCursor(Qt.WaitCursor)
+        self.setEnabled(False)
+
+    def stop_job(self):
+        self.setCursor(Qt.ArrowCursor)
+        self.setEnabled(True)
+
+    def set_grating(self):
+        val = self.settings_widge.set_grating_number.value()
+        self.spectrometer_thread.do_function("set_grating", val)
+        self.start_job()
+
+    def set_wavelength(self):
+        val = self.settings_widge.initial_wavelength.value()
+        self.spectrometer_thread.do_function("set_wavelength", val)
+        self.start_job()
+
+    def set_input_port(self):
+        val = self.settings_widge.input_port.currentText()
+        self.spectrometer_thread.do_function("set_input_port", val)
+        self.start_job()
+
+    def set_output_port(self):
+        val = self.settings_widge.output_port.currentText()
+        self.spectrometer_thread.do_function("set_output_port", val)
+        self.start_job()
+
+    def set_input_slit_size(self):
+        val = self.settings_widge.input_slit_size.value()
+        self.spectrometer_thread.do_function("set_input_slit_size", val)
+        self.start_job()
+
+    def set_output_slit_size(self):
+        val = self.settings_widge.output_slit_size.value()
+        self.spectrometer_thread.do_function("set_output_slit_size", val)
+        self.start_job()
+
+    def set_horizontal_flip(self):
+        self.ophyd_device.horizontal_cam_flip.put(
+            self.settings_widge.checkBox_horizontal_flip.isChecked()
+        )
+
+    def measure_spectrum(self):
+        self.spectrometer_thread.do_function("measure_spectrum", None)
+        self.start_job()
+
+    def show_spectrum(self, wl, intensity):
+        try:
+            self.current_data["intensity"] = intensity
+            self.current_data["wavelength"] = wl
+            if intensity.ndim > 1:
+                if self.image_plot is None:
+                    import matplotlib.pyplot as plt
+
+                    self.image_plot = plt.subplots()
+                x, y = np.meshgrid(wl, range(len(intensity)))
+                self.image_plot[1].clear()
+                self.image_plot[1].pcolormesh(x, y, intensity)
+                self.image_plot[0].show()
+            else:
+                self.spectrum_plot.plot.add_data(
+                    wl,
+                    {"intensity": intensity},
+                    add=not self.checkBox_clear_plot.isChecked(),
+                )
+                self.spectrum_plot.show()
+        except Exception as e:
+            WarnPopup(self, str(e), "error")
+
+    def continuous_spectra(self):
+        if not self.continuous_meas:
+            self.setCursor(Qt.WaitCursor)
+            self.continuous_button.setText("stop acquisition")
+            self.acquire_button.setEnabled(False)
+            self.save_button.setEnabled(False)
+            self.settings_widge.setEnabled(False)
+            self.camera_widge.setEnabled(False)
+            self.continuous_meas = True
+            self.spectrometer_thread.continuous = True
+        else:
+            self.spectrometer_thread.continuous = False
+            self.setCursor(Qt.ArrowCursor)
+            self.continuous_button.setText("continuous spectra")
+            self.acquire_button.setEnabled(True)
+            self.save_button.setEnabled(True)
+            self.settings_widge.setEnabled(True)
+            self.camera_widge.setEnabled(True)
+            self.continuous_meas = False
+
+    def change_camera_config(self, x, conf):
+        configs = self.camera_widge.get_config()
+        value = configs[conf]
+        self.spectrometer_thread.do_function("change_camera_config", [value, conf])
+        self.start_job()
+
+    def close(self) -> bool:
+        self.spectrometer_thread.still_running = False
+        self.spectrometer_thread.continuous = False
+        return super().close()
+
+    def closeEvent(self, a0):
+        self.spectrometer_thread.still_running = False
+        self.spectrometer_thread.continuous = False
+        self.spectrum_plot.close()
+        if self.image_plot is not None:
+            import matplotlib.pyplot as plt
+
+            plt.close(self.image_plot[0])
+            self.image_plot = None
+        return super().closeEvent(a0)
+
+
+class Spectrometer_Work_Thread(QThread):
+    job_done = Signal()
+    spectrum_data_signal = Signal(object, object)
+    new_spec_config = Signal(dict)
+    new_cam_config = Signal(dict)
+
+    def __init__(self, parent=None, spectrometer=None):
+        super().__init__(parent=parent)
+        self.spectrometer = spectrometer
+        self.still_running = True
+        self.continuous = False
+        self.function_to_do = None
+        self.function_value = None
+        self.last_config = None
+        self.last_cam_config = None
+
+    def run(self):
+        i = 100
+        while self.still_running:
+            time.sleep(0.1)
+            if self.function_to_do:
+                getattr(self, self.function_to_do)(self.function_value)
+                self.function_to_do = None
+                self.function_value = None
+                self.job_done.emit()
+            if self.continuous:
+                self.continuous_function()
+            if i >= 100:
+                self.update_configs()
+                i = 0
+            i += 1
+
+    def update_configs(self):
+        spec_config = self.spectrometer.read_configuration()
+        cam_config = self.spectrometer.get_camera_device().read_configuration()
+        if spec_config != self.last_config:
+            self.last_config = spec_config
+            conf = {}
+            name = self.spectrometer.name
+            for k, v in spec_config.items():
+                conf[k.split(f"{name}_")[1]] = v["value"]
+            conf["wavelength"] = self.spectrometer.wavelength.get()
+            self.new_spec_config.emit(conf)
+        if cam_config != self.last_cam_config:
+            name = self.spectrometer.get_camera_device().name
+            conf = {}
+            for k, v in cam_config.items():
+                conf[k.split(f"{name}_")[1]] = v["value"]
+            self.last_cam_config = cam_config
+            self.new_cam_config.emit(conf)
+
+    def do_function(self, name, value):
+        self.function_to_do = name
+        self.function_value = value
+
+    def set_grating(self, value):
+        try:
+            self.spectrometer.set_grating_number.put(value)
+        except Exception as e:
+            WarnPopup(None, str(e), "error")
+
+    def set_wavelength(self, value):
+        try:
+            self.spectrometer.center_wavelength.put(value)
+        except Exception as e:
+            WarnPopup(None, str(e), "error")
+
+    def set_input_port(self, value):
+        try:
+            self.spectrometer.input_port.put(value)
+        except Exception as e:
+            WarnPopup(None, str(e), "error")
+
+    def set_output_port(self, value):
+        try:
+            self.spectrometer.output_port.put(value)
+        except Exception as e:
+            WarnPopup(None, str(e), "error")
+
+    def set_input_slit_size(self, value):
+        try:
+            self.spectrometer.input_slit_size.put(value)
+        except Exception as e:
+            WarnPopup(None, str(e), "error")
+
+    def set_output_slit_size(self, value):
+        try:
+            self.spectrometer.output_slit_size.put(value)
+        except Exception as e:
+            WarnPopup(None, str(e), "error")
+
+    def measure_spectrum(self, value):
+        try:
+            intensity = self.spectrometer.spectrum.get()
+            wl = self.spectrometer.wavelength.get()
+            self.spectrum_data_signal.emit(wl, intensity)
+        except Exception as e:
+            WarnPopup(None, str(e), "error")
+
+    def continuous_function(self):
+        cam = self.spectrometer.get_camera_device().camera
+        cam.start_acquisition()
+        while self.continuous:
+            time.sleep(0.1)
+            im = cam.read_newest_image()
+            if im is not None:
+                wl = self.spectrometer.wavelength.get()
+                if len(im) == 1:
+                    im = im[0]
+                self.spectrum_data_signal.emit(wl, im)
+
+    def change_camera_config(self, value):
+        value, conf = value
+        try:
+            cam = self.spectrometer.get_camera_device()
+            set_signal = getattr(cam, conf)
+            set_signal.put(value)
+        except Exception as e:
+            WarnPopup(None, str(e), "error")
+
+
+class Andor_Manual_Control_Config(Manual_Control_Config):
+    def __init__(self, parent=None, control_data=None):
+        super().__init__(
+            parent=parent,
+            control_data=control_data,
+            title="Spectrometer control config",
+            control_type="Andor_Manual_Control",
+        )
+        control_data = control_data or {}
+        select_label = QLabel("Spectrometer:")
+        cam_label = QLabel("Camera:")
+
+        self.spec_box = QComboBox()
+        specs = []
+        for name, device in variables_handling.devices.items():
+            if device.name == "andor_shamrock_500":
+                specs.append(name)
+        self.spec_box.addItems(specs)
+        if "spectrometer" in control_data and control_data["spectrometer"] in specs:
+            self.spec_box.setCurrentText(control_data["spectrometer"])
+
+        self.cam_box = QComboBox()
+        cams = []
+        for name, device in variables_handling.devices.items():
+            cams.append(name)
+        self.cam_box.addItems(cams)
+        if "camera" in control_data and control_data["camera"] in cams:
+            self.cam_box.setCurrentText(control_data["camera"])
+        self.layout().addWidget(select_label, 2, 0)
+        self.layout().addWidget(self.spec_box, 2, 1)
+        self.layout().addWidget(cam_label, 3, 0)
+        self.layout().addWidget(self.cam_box, 3, 1)
+
+    def accept(self):
+        self.control_data["spectrometer"] = self.spec_box.currentText()
+        self.control_data["camera"] = self.cam_box.currentText()
+        super().accept()
```

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_ophyd.py` & `nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500/andor_shamrock_500_ophyd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,80 @@
 from ophyd import Component as Cpt
 import pylablib as pll
 
-from ophyd import Device
-from nomad_camels.bluesky_handling.custom_function_signal import Custom_Function_Signal, Custom_Function_SignalRO
+from nomad_camels.bluesky_handling.custom_function_signal import (
+    Custom_Function_Signal,
+    Custom_Function_SignalRO,
+    Sequential_Device,
+)
 
 
-class Andor_Shamrock_500(Device):
+class Andor_Shamrock_500(Sequential_Device):
     """
     Driver for the Andor Shamrock 500 spectrometer (not the camera!).
     The camera is implemented separately.
     """
-    spectrum = Cpt(Custom_Function_SignalRO, name='spectrum')
-    wavelength = Cpt(Custom_Function_SignalRO, name='wavelength', metadata={'units': 'nm'})
 
-    set_grating_number = Cpt(Custom_Function_Signal, name='set_grating_number', kind='config')
-    center_wavelength = Cpt(Custom_Function_Signal, name='center_wavelength', kind='config')
-    input_port = Cpt(Custom_Function_Signal, name='input_port', kind='config')
-    output_port = Cpt(Custom_Function_Signal, name='output_port', kind='config')
-    camera = Cpt(Custom_Function_Signal, name='camera', kind='config')
-    input_slit_size = Cpt(Custom_Function_Signal, name='input_slit_size', kind='config')
-    output_slit_size = Cpt(Custom_Function_Signal, name='output_slit_size', kind='config')
-    horizontal_cam_flip = Cpt(Custom_Function_Signal, name='horizontal_cam_flip', kind='config')
-
-    def __init__(self, prefix='', *, name, kind=None, read_attrs=None,
-                 configuration_attrs=None, parent=None, spectrometer='',
-                 dll_path='', **kwargs):
-        super().__init__(prefix=prefix, name=name, kind=kind, read_attrs=read_attrs,
-                         configuration_attrs=configuration_attrs, parent=parent, **kwargs)
-        if name == 'test':
+    spectrum = Cpt(Custom_Function_SignalRO, name="spectrum")
+    wavelength = Cpt(
+        Custom_Function_SignalRO, name="wavelength", metadata={"units": "nm"}
+    )
+
+    set_grating_number = Cpt(
+        Custom_Function_Signal, name="set_grating_number", kind="config"
+    )
+    center_wavelength = Cpt(
+        Custom_Function_Signal, name="center_wavelength", kind="config"
+    )
+    input_port = Cpt(Custom_Function_Signal, name="input_port", kind="config")
+    output_port = Cpt(Custom_Function_Signal, name="output_port", kind="config")
+    camera = Cpt(Custom_Function_Signal, name="camera", kind="config")
+    input_slit_size = Cpt(Custom_Function_Signal, name="input_slit_size", kind="config")
+    output_slit_size = Cpt(
+        Custom_Function_Signal, name="output_slit_size", kind="config"
+    )
+    horizontal_cam_flip = Cpt(
+        Custom_Function_Signal, name="horizontal_cam_flip", kind="config"
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
+        spectrometer="",
+        dll_path="",
+        **kwargs,
+    ):
+        super().__init__(
+            prefix=prefix,
+            name=name,
+            kind=kind,
+            read_attrs=read_attrs,
+            configuration_attrs=configuration_attrs,
+            parent=parent,
+            force_sequential=True,
+            **kwargs,
+        )
+        if name == "test":
             return
-        pll.par['devices/dlls/andor_shamrock'] = dll_path
+        pll.par["devices/dlls/andor_shamrock"] = dll_path
         from pylablib.devices import Andor
+
         specs = Andor.list_shamrock_spectrographs()
-        spec = specs.index(spectrometer)
-        self.spectrometer = Andor.ShamrockSpectrograph(idx=spec)
+        try:
+            spec = specs.index(spectrometer)
+            self.spectrometer = Andor.ShamrockSpectrograph(idx=spec)
+        except:
+            self.spectrometer = Andor.ShamrockSpectrograph(idx=0)
+
         self.set_grating_number.put_function = self.set_grating_number_function
         self.center_wavelength.put_function = self.center_wavelength_function
         self.input_port.put_function = self.input_port_function
         self.output_port.put_function = self.output_port_function
         self.camera.put_function = self.camera_function
         self.input_slit_size.put_function = self.input_slit_size_function
         self.output_slit_size.put_function = self.output_slit_size_function
@@ -49,56 +86,57 @@
     def finalize_steps(self):
         self.spectrometer.close()
 
     def set_grating_number_function(self, value):
         self.spectrometer.set_grating(value)
 
     def center_wavelength_function(self, value):
-        self.spectrometer.set_wavelength(value*1e-9)
+        self.spectrometer.set_wavelength(value * 1e-9)
 
     def input_port_function(self, value):
-        if not self.spectrometer.is_flipper_present('input'):
+        if not self.spectrometer.is_flipper_present("input"):
             return
-        self.spectrometer.set_flipper_port('input', value)
+        self.spectrometer.set_flipper_port("input", value)
         self.input_slit_size_function(self.input_slit_size.get())
 
     def output_port_function(self, value):
-        if not self.spectrometer.is_flipper_present('output'):
+        if not self.spectrometer.is_flipper_present("output"):
             return
-        self.spectrometer.set_flipper_port('output', value)
+        self.spectrometer.set_flipper_port("output", value)
         self.output_port._readback = value
         self.output_slit_size_function(self.output_slit_size.get())
 
     def camera_function(self, value):
         if isinstance(value, str):
             from nomad_camels.utility import device_handling
+
             cam = device_handling.running_devices[value].camera
         else:
             cam = value.camera
         self.spectrometer.setup_pixels_from_camera(cam)
 
     def input_slit_size_function(self, value):
-        if not self.spectrometer.is_flipper_present('input'):
-            pos = 'direct'
-            if not self.spectrometer.is_slit_present(f'input_{pos}'):
-                pos = 'side'
+        if not self.spectrometer.is_flipper_present("input"):
+            pos = "direct"
+            if not self.spectrometer.is_slit_present(f"input_{pos}"):
+                pos = "side"
         else:
             pos = self.input_port.get()
-        if not self.spectrometer.is_slit_present(f'input_{pos}'):
+        if not self.spectrometer.is_slit_present(f"input_{pos}"):
             return
-        self.spectrometer.set_slit_width(f'input_{pos}', value*1e-6)
+        self.spectrometer.set_slit_width(f"input_{pos}", value * 1e-6)
 
     def output_slit_size_function(self, value):
-        if not self.spectrometer.is_flipper_present('output'):
-            pos = 'direct'
+        if not self.spectrometer.is_flipper_present("output"):
+            pos = "direct"
         else:
             pos = self.output_port.get()
-        if not self.spectrometer.is_slit_present(f'output_{pos}'):
+        if not self.spectrometer.is_slit_present(f"output_{pos}"):
             return
-        self.spectrometer.set_slit_width(f'output_{pos}', value*1e-6)
+        self.spectrometer.set_slit_width(f"output_{pos}", value * 1e-6)
 
     def get_wavelengths(self):
         self.spectrometer.setup_pixels_from_camera(self.get_camera_device().camera)
         cal = self.spectrometer.get_calibration()
         return cal * 1e9
 
     def read_spectrum(self):
@@ -112,12 +150,13 @@
         else:
             return spec[::-1]
 
     def get_camera_device(self):
         cam = self.camera.get()
         if isinstance(cam, str):
             from nomad_camels.utility import device_handling
+
             cam = device_handling.running_devices[cam]
         return cam
 
     def horizontal_cam_flip_function(self, value):
         self.flip_horizontal = value
```

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500.egg-info/PKG-INFO` & `nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad_camels_driver_andor_shamrock_500
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package provides everything to run an Andor Shamrock 500 spectrometer.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
```

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/nomad_camels_driver_andor_shamrock_500.egg-info/SOURCES.txt` & `nomad_camels_driver_andor_shamrock_500-0.1.1/nomad_camels_driver_andor_shamrock_500.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_andor_shamrock_500-0.1.0/pyproject.toml` & `nomad_camels_driver_andor_shamrock_500-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nomad_camels_driver_andor_shamrock_500"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="FAIRmat - HU Berlin", email="nomad-camels@fau.de" }
 ]
 description = "This package provides everything to run an Andor Shamrock 500 spectrometer."
 readme = "README.md"
 requires-python = ">=3.9.6"
 classifiers = [
```

