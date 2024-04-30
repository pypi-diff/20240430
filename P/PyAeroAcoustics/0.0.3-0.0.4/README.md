# Comparing `tmp/PyAeroAcoustics-0.0.3.tar.gz` & `tmp/PyAeroAcoustics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAeroAcoustics-0.0.3.tar", last modified: Mon Apr 29 15:45:14 2024, max compression
+gzip compressed data, was "PyAeroAcoustics-0.0.4.tar", last modified: Tue Apr 30 07:08:07 2024, max compression
```

## Comparing `PyAeroAcoustics-0.0.3.tar` & `PyAeroAcoustics-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:45:14.475635 PyAeroAcoustics-0.0.3/
--rw-r--r--   0 brunnerth (76394) p71694   (71694)      549 2024-04-29 15:45:14.474944 PyAeroAcoustics-0.0.3/PKG-INFO
-drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:45:14.470311 PyAeroAcoustics-0.0.3/PyAeroAcoustics/
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       30 2024-04-29 15:44:32.000000 PyAeroAcoustics-0.0.3/PyAeroAcoustics/PyAeroAcoustics.py
-drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:45:14.474305 PyAeroAcoustics-0.0.3/PyAeroAcoustics/Spectrum/
--rw-r--r--   0 brunnerth (76394) p71694   (71694)     2395 2024-04-29 15:31:09.000000 PyAeroAcoustics-0.0.3/PyAeroAcoustics/Spectrum/Spectrum.py
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       22 2024-04-29 15:44:17.000000 PyAeroAcoustics-0.0.3/PyAeroAcoustics/Spectrum/__init__.py
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       22 2024-04-29 15:44:44.000000 PyAeroAcoustics-0.0.3/PyAeroAcoustics/__init__.py
-drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-29 15:45:14.473257 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/
--rw-r--r--   0 brunnerth (76394) p71694   (71694)      549 2024-04-29 15:45:14.471179 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/PKG-INFO
--rw-r--r--   0 brunnerth (76394) p71694   (71694)      301 2024-04-29 15:45:14.472225 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/SOURCES.txt
--rw-r--r--   0 brunnerth (76394) p71694   (71694)        1 2024-04-29 15:45:14.472980 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/dependency_links.txt
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       16 2024-04-29 15:45:14.473342 PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/top_level.txt
--rw-r--r--   0 brunnerth (76394) p71694   (71694)       38 2024-04-29 15:45:14.475744 PyAeroAcoustics-0.0.3/setup.cfg
--rw-r--r--   0 brunnerth (76394) p71694   (71694)      920 2024-04-29 15:45:07.000000 PyAeroAcoustics-0.0.3/setup.py
+drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-30 07:08:07.002401 PyAeroAcoustics-0.0.4/
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)      549 2024-04-30 07:08:07.002032 PyAeroAcoustics-0.0.4/PKG-INFO
+drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-30 07:08:06.989596 PyAeroAcoustics-0.0.4/PyAeroAcoustics/
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       30 2024-04-29 15:44:32.000000 PyAeroAcoustics-0.0.4/PyAeroAcoustics/PyAeroAcoustics.py
+drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-30 07:08:07.000344 PyAeroAcoustics-0.0.4/PyAeroAcoustics/Spectrum/
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)     2836 2024-04-30 07:06:42.000000 PyAeroAcoustics-0.0.4/PyAeroAcoustics/Spectrum/Spectrum.py
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       22 2024-04-29 15:44:17.000000 PyAeroAcoustics-0.0.4/PyAeroAcoustics/Spectrum/__init__.py
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       22 2024-04-29 15:44:44.000000 PyAeroAcoustics-0.0.4/PyAeroAcoustics/__init__.py
+drwxr-xr-x   0 brunnerth (76394) p71694   (71694)        0 2024-04-30 07:08:06.998327 PyAeroAcoustics-0.0.4/PyAeroAcoustics.egg-info/
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)      549 2024-04-30 07:08:06.994525 PyAeroAcoustics-0.0.4/PyAeroAcoustics.egg-info/PKG-INFO
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)      301 2024-04-30 07:08:06.994836 PyAeroAcoustics-0.0.4/PyAeroAcoustics.egg-info/SOURCES.txt
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)        1 2024-04-30 07:08:06.997620 PyAeroAcoustics-0.0.4/PyAeroAcoustics.egg-info/dependency_links.txt
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       16 2024-04-30 07:08:06.998479 PyAeroAcoustics-0.0.4/PyAeroAcoustics.egg-info/top_level.txt
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)       38 2024-04-30 07:08:07.002567 PyAeroAcoustics-0.0.4/setup.cfg
+-rw-r--r--   0 brunnerth (76394) p71694   (71694)      920 2024-04-30 07:08:00.000000 PyAeroAcoustics-0.0.4/setup.py
```

### Comparing `PyAeroAcoustics-0.0.3/PKG-INFO` & `PyAeroAcoustics-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyAeroAcoustics
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyAeroAcoustics
 Home-page: UNKNOWN
 Author: Thomas Brunner
 Author-email: <thomas.brunner@tugraz.at>
 License: UNKNOWN
 Description: PyAeroAcoustics
 Keywords: python,PyAeroAcoustics
```

### Comparing `PyAeroAcoustics-0.0.3/PyAeroAcoustics/Spectrum/Spectrum.py` & `PyAeroAcoustics-0.0.4/PyAeroAcoustics/Spectrum/Spectrum.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,14 +22,22 @@
         self.num_steps = self.num_steps-cutoff_index
 
     def cutoff_indices(self, index_1: int, index_2: int):
         self.time_series_data = self.time_series_data[index_1:index_2]
         self.time = self.time[index_1:index_2]
         self.num_steps = index_2-index_1
 
+    def subtract_mean_dynamics(self, type = "total"):
+        if type == "total":
+            self.time_series_data = self.time_series_data-np.mean(self.time_series_data)
+        elif type == "pointwise":
+            self.time_series_data = self.time_series_data-np.mean(self.time_series_data, axis = 1)
+        elif type == "per_timestep":
+            self.time_series_data = self.time_series_data-np.mean(self.time_series_data, axis = 0)
+
     def use_windows(self, num_windows: int, print_info = True):
         split_ind = int(np.floor(np.shape(self.time)[0]/num_windows))
         self.num_windows = num_windows
         if print_info:
             print(" - using "+str(num_windows)+ " window(s) with "+str(split_ind)+" timesteps")
 
         data_windows = np.zeros((split_ind, num_windows))
```

### Comparing `PyAeroAcoustics-0.0.3/PyAeroAcoustics.egg-info/PKG-INFO` & `PyAeroAcoustics-0.0.4/PyAeroAcoustics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyAeroAcoustics
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyAeroAcoustics
 Home-page: UNKNOWN
 Author: Thomas Brunner
 Author-email: <thomas.brunner@tugraz.at>
 License: UNKNOWN
 Description: PyAeroAcoustics
 Keywords: python,PyAeroAcoustics
```

### Comparing `PyAeroAcoustics-0.0.3/setup.py` & `PyAeroAcoustics-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'PyAeroAcoustics'
 LONG_DESCRIPTION = 'PyAeroAcoustics'
 
 setup(
         name="PyAeroAcoustics", 
         version=VERSION,
         author="Thomas Brunner",
```

