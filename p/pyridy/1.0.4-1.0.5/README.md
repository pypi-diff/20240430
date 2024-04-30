# Comparing `tmp/pyridy-1.0.4.tar.gz` & `tmp/pyridy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyridy-1.0.4.tar", max compression
+gzip compressed data, was "pyridy-1.0.5.tar", max compression
```

## Comparing `pyridy-1.0.4.tar` & `pyridy-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11583 2023-02-14 16:19:37.926633 pyridy-1.0.4/LICENSE
--rw-r--r--   0        0        0      988 2024-04-26 13:35:31.503470 pyridy-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       65 2023-02-14 16:19:37.951522 pyridy-1.0.4/pyridy/__init__.py
--rw-r--r--   0        0        0    22145 2023-03-09 12:44:02.621957 pyridy-1.0.4/pyridy/campaign.py
--rw-r--r--   0        0        0     2402 2023-02-14 16:19:37.954033 pyridy-1.0.4/pyridy/config.py
--rw-r--r--   0        0        0    62635 2024-02-20 10:12:28.770803 pyridy-1.0.4/pyridy/file.py
--rw-r--r--   0        0        0       22 2023-02-14 16:19:37.955033 pyridy-1.0.4/pyridy/osm/__init__.py
--rw-r--r--   0        0        0    30598 2023-04-27 12:36:22.469380 pyridy-1.0.4/pyridy/osm/osm.py
--rw-r--r--   0        0        0      121 2023-02-14 16:19:37.956033 pyridy-1.0.4/pyridy/osm/utils/__init__.py
--rw-r--r--   0        0        0    12461 2023-04-27 12:36:22.472382 pyridy-1.0.4/pyridy/osm/utils/elements.py
--rw-r--r--   0        0        0     6329 2023-03-09 12:44:02.642961 pyridy-1.0.4/pyridy/osm/utils/overpass.py
--rw-r--r--   0        0        0     1173 2023-03-09 12:44:02.647963 pyridy-1.0.4/pyridy/osm/utils/query.py
--rw-r--r--   0        0        0       60 2023-02-14 16:19:37.958033 pyridy-1.0.4/pyridy/osm/utils/relation.py
--rw-r--r--   0        0        0    14525 2023-03-09 16:42:58.451384 pyridy-1.0.4/pyridy/osm/utils/tools.py
--rw-r--r--   0        0        0      105 2023-02-14 16:19:37.959032 pyridy-1.0.4/pyridy/processing/__init__.py
--rw-r--r--   0        0        0    16957 2023-03-09 16:42:58.467625 pyridy-1.0.4/pyridy/processing/comfort.py
--rw-r--r--   0        0        0     6510 2023-03-09 12:44:02.659964 pyridy-1.0.4/pyridy/processing/condition.py
--rw-r--r--   0        0        0     8805 2023-03-09 16:42:58.476180 pyridy-1.0.4/pyridy/processing/excitation.py
--rw-r--r--   0        0        0      239 2023-02-14 16:19:37.961198 pyridy-1.0.4/pyridy/processing/processor.py
--rw-r--r--   0        0        0       57 2023-02-14 16:19:37.962255 pyridy-1.0.4/pyridy/utils/__init__.py
--rw-r--r--   0        0        0     3740 2023-02-14 16:19:37.962255 pyridy-1.0.4/pyridy/utils/device.py
--rw-r--r--   0        0        0     2000 2023-02-14 16:19:37.963205 pyridy-1.0.4/pyridy/utils/sensor.py
--rw-r--r--   0        0        0    46523 2023-03-09 16:42:58.434611 pyridy-1.0.4/pyridy/utils/timeseries.py
--rw-r--r--   0        0        0     3890 2023-03-09 16:42:58.443203 pyridy-1.0.4/pyridy/utils/tools.py
--rw-r--r--   0        0        0       18 2023-02-14 16:19:37.965205 pyridy-1.0.4/pyridy/widgets/__init__.py
--rw-r--r--   0        0        0    12800 2023-02-14 16:19:37.965205 pyridy-1.0.4/pyridy/widgets/map.py
--rw-r--r--   0        0        0     2332 2023-02-14 16:19:37.926633 pyridy-1.0.4/README.md
--rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 pyridy-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11583 2023-02-14 16:19:37.926633 pyridy-1.0.5/LICENSE
+-rw-r--r--   0        0        0      988 2024-04-30 13:28:34.750865 pyridy-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-02-14 16:19:37.951522 pyridy-1.0.5/pyridy/__init__.py
+-rw-r--r--   0        0        0    22145 2023-03-09 12:44:02.621957 pyridy-1.0.5/pyridy/campaign.py
+-rw-r--r--   0        0        0     2402 2023-02-14 16:19:37.954033 pyridy-1.0.5/pyridy/config.py
+-rw-r--r--   0        0        0    62635 2024-02-20 10:12:28.770803 pyridy-1.0.5/pyridy/file.py
+-rw-r--r--   0        0        0       22 2023-02-14 16:19:37.955033 pyridy-1.0.5/pyridy/osm/__init__.py
+-rw-r--r--   0        0        0    30598 2023-04-27 12:36:22.469380 pyridy-1.0.5/pyridy/osm/osm.py
+-rw-r--r--   0        0        0      121 2023-02-14 16:19:37.956033 pyridy-1.0.5/pyridy/osm/utils/__init__.py
+-rw-r--r--   0        0        0    12461 2023-04-27 12:36:22.472382 pyridy-1.0.5/pyridy/osm/utils/elements.py
+-rw-r--r--   0        0        0     6329 2023-03-09 12:44:02.642961 pyridy-1.0.5/pyridy/osm/utils/overpass.py
+-rw-r--r--   0        0        0     1173 2023-03-09 12:44:02.647963 pyridy-1.0.5/pyridy/osm/utils/query.py
+-rw-r--r--   0        0        0       60 2023-02-14 16:19:37.958033 pyridy-1.0.5/pyridy/osm/utils/relation.py
+-rw-r--r--   0        0        0    14525 2023-03-09 16:42:58.451384 pyridy-1.0.5/pyridy/osm/utils/tools.py
+-rw-r--r--   0        0        0      105 2023-02-14 16:19:37.959032 pyridy-1.0.5/pyridy/processing/__init__.py
+-rw-r--r--   0        0        0    16995 2024-04-30 13:26:44.454403 pyridy-1.0.5/pyridy/processing/comfort.py
+-rw-r--r--   0        0        0     6510 2023-03-09 12:44:02.659964 pyridy-1.0.5/pyridy/processing/condition.py
+-rw-r--r--   0        0        0     8805 2023-03-09 16:42:58.476180 pyridy-1.0.5/pyridy/processing/excitation.py
+-rw-r--r--   0        0        0      239 2023-02-14 16:19:37.961198 pyridy-1.0.5/pyridy/processing/processor.py
+-rw-r--r--   0        0        0       57 2023-02-14 16:19:37.962255 pyridy-1.0.5/pyridy/utils/__init__.py
+-rw-r--r--   0        0        0     3740 2023-02-14 16:19:37.962255 pyridy-1.0.5/pyridy/utils/device.py
+-rw-r--r--   0        0        0     2000 2023-02-14 16:19:37.963205 pyridy-1.0.5/pyridy/utils/sensor.py
+-rw-r--r--   0        0        0    46523 2023-03-09 16:42:58.434611 pyridy-1.0.5/pyridy/utils/timeseries.py
+-rw-r--r--   0        0        0     3890 2023-03-09 16:42:58.443203 pyridy-1.0.5/pyridy/utils/tools.py
+-rw-r--r--   0        0        0       18 2023-02-14 16:19:37.965205 pyridy-1.0.5/pyridy/widgets/__init__.py
+-rw-r--r--   0        0        0    12800 2023-02-14 16:19:37.965205 pyridy-1.0.5/pyridy/widgets/map.py
+-rw-r--r--   0        0        0     2332 2023-02-14 16:19:37.926633 pyridy-1.0.5/README.md
+-rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 pyridy-1.0.5/PKG-INFO
```

### Comparing `pyridy-1.0.4/LICENSE` & `pyridy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyproject.toml` & `pyridy-1.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyridy"
-version = "1.0.4"
+version = "1.0.5"
 description = "Support library for measurements made with the Ridy Android App"
 authors = ["Philipp Simon Leibner <philipp.leibner@ifs.rwth-aachen.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 classifiers = [
     "Topic :: Scientific/Engineering :: Information Analysis",
```

### Comparing `pyridy-1.0.4/pyridy/campaign.py` & `pyridy-1.0.5/pyridy/campaign.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/config.py` & `pyridy-1.0.5/pyridy/config.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/file.py` & `pyridy-1.0.5/pyridy/file.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/osm/osm.py` & `pyridy-1.0.5/pyridy/osm/osm.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/osm/utils/elements.py` & `pyridy-1.0.5/pyridy/osm/utils/elements.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/osm/utils/overpass.py` & `pyridy-1.0.5/pyridy/osm/utils/overpass.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/osm/utils/query.py` & `pyridy-1.0.5/pyridy/osm/utils/query.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/osm/utils/tools.py` & `pyridy-1.0.5/pyridy/osm/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/processing/comfort.py` & `pyridy-1.0.5/pyridy/processing/comfort.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,20 @@
         cc_y : ndarray
             Continuous comfort index according to y-axis
         cc_z : ndarray
             Continuous comfort index according to z-axis
 
         """
         # The evaluation assumes the phone is laying on the floor pointing in the direction of travel
-        Wb = ComfortProcessor.Wb(f_s) # weighting factor: Vertical Whole-Body Vibration, Z Axis
-        Wd = ComfortProcessor.Wd(f_s) # Horizontal Whole-Body Vibration, X or Y Axis
+        Wb = ComfortProcessor.Wb(f_s)  # weighting factor: Vertical Whole-Body Vibration, Z Axis
+        Wd = ComfortProcessor.Wd(f_s)  # Horizontal Whole-Body Vibration, X or Y Axis
 
-        a_x_wd = signal.lfilter(Wd[0], Wd[1], acc_x)  # Adjusting to vehicle coordinate system
-        a_y_wd = signal.lfilter(Wd[0], Wd[1], acc_y)
-        a_z_wb = signal.lfilter(Wb[0], Wb[1], acc_z)
+        a_x_wd = signal.lfilter(Wd[0], Wd[1], np.squeeze(acc_x))  # Adjusting to vehicle coordinate system
+        a_y_wd = signal.lfilter(Wd[0], Wd[1], np.squeeze(acc_y))
+        a_z_wb = signal.lfilter(Wb[0], Wb[1], np.squeeze(acc_z))
 
         # Moving RMS over 5s window
         f_x, t, Pa_x = signal.spectrogram(a_x_wd, f_s, nperseg=5 * f_s, noverlap=0, mode='psd')
         f_y, _, Pa_y = signal.spectrogram(a_y_wd, f_s, nperseg=5 * f_s, noverlap=0, mode='psd')
         f_z, _, Pa_z = signal.spectrogram(a_z_wb, f_s, nperseg=5 * f_s, noverlap=0, mode='psd')
 
         cc_x = np.sqrt(np.trapz(Pa_x, f_x, axis=0))
```

### Comparing `pyridy-1.0.4/pyridy/processing/condition.py` & `pyridy-1.0.5/pyridy/processing/condition.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/processing/excitation.py` & `pyridy-1.0.5/pyridy/processing/excitation.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/utils/device.py` & `pyridy-1.0.5/pyridy/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/utils/sensor.py` & `pyridy-1.0.5/pyridy/utils/sensor.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/utils/timeseries.py` & `pyridy-1.0.5/pyridy/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/utils/tools.py` & `pyridy-1.0.5/pyridy/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/pyridy/widgets/map.py` & `pyridy-1.0.5/pyridy/widgets/map.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/README.md` & `pyridy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.4/PKG-INFO` & `pyridy-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyridy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Support library for measurements made with the Ridy Android App
 License: Apache-2.0
 Keywords: signal processing,ridy,android
 Author: Philipp Simon Leibner
 Author-email: philipp.leibner@ifs.rwth-aachen.de
 Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyridy Version: 1.0.4 Summary: Support library for
+Metadata-Version: 2.1 Name: pyridy Version: 1.0.5 Summary: Support library for
 measurements made with the Ridy Android App License: Apache-2.0 Keywords:
 signal processing,ridy,android Author: Philipp Simon Leibner Author-email:
 philipp.leibner@ifs.rwth-aachen.de Requires-Python: >=3.9,<3.13 Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

