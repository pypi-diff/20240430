# Comparing `tmp/mosaik_heatpump-1.0.0.tar.gz` & `tmp/mosaik_heatpump-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik_heatpump-1.0.0.tar", max compression
+gzip compressed data, was "mosaik_heatpump-1.0.1.tar", max compression
```

## Comparing `mosaik_heatpump-1.0.0.tar` & `mosaik_heatpump-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      193 2024-02-28 13:51:10.632568 mosaik_heatpump-1.0.0/AUTHORS.txt
--rw-r--r--   0        0        0     1071 2024-02-28 13:51:10.632568 mosaik_heatpump-1.0.0/LICENSE
--rw-r--r--   0        0        0     1404 2024-02-28 13:51:10.632568 mosaik_heatpump-1.0.0/README.rst
--rw-r--r--   0        0        0        0 2024-02-28 13:51:10.674568 mosaik_heatpump-1.0.0/mosaik_components/__init__.py
--rw-r--r--   0        0        0    27610 2024-02-28 13:51:10.642568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/Heat_Pump_Design.py
--rw-r--r--   0        0        0     6906 2024-02-28 13:51:10.642568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/Heat_Pump_Model.py
--rw-r--r--   0        0        0     3820 2024-02-28 13:51:10.643568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/Heat_Pump_mosaik.py
--rw-r--r--   0        0        0       82 2024-02-28 13:51:10.643568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 13:51:10.675568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/controller/__init__.py
--rw-r--r--   0        0        0    11680 2024-02-28 13:51:10.643568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/controller/controller.py
--rw-r--r--   0        0        0     4727 2024-02-28 13:51:10.643568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/controller/controller_mosaik.py
--rw-r--r--   0        0        0     2108 2024-02-28 13:51:10.643568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/coolingloadsim/coolingloadsim.py
--rw-r--r--   0        0        0     2530 2024-02-28 13:51:10.643568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/coolingloadsim/coolingloadsim_mosaik.py
--rw-r--r--   0        0        0  3723869 2024-02-28 13:51:10.650568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/cop_m_data.json
--rw-r--r--   0        0        0   145584 2024-02-28 13:51:10.650568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/eta_s_data.json
--rw-r--r--   0        0        0        0 2024-02-28 13:51:10.675568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/hotwatertank/__init__.py
--rw-r--r--   0        0        0    24369 2024-02-28 13:51:10.650568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/hotwatertank/hotwatertank.py
--rw-r--r--   0        0        0     5828 2024-02-28 13:51:10.650568 mosaik_heatpump-1.0.0/mosaik_components/heatpump/hotwatertank/hotwatertank_mosaik.py
--rw-r--r--   0        0        0      778 2024-02-28 13:51:10.650568 mosaik_heatpump-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 mosaik_heatpump-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      193 2024-04-30 09:01:37.565417 mosaik_heatpump-1.0.1/AUTHORS.txt
+-rw-r--r--   0        0        0     1071 2024-04-30 09:01:37.565417 mosaik_heatpump-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1404 2024-04-30 09:01:37.565417 mosaik_heatpump-1.0.1/README.rst
+-rw-r--r--   0        0        0        0 2024-04-30 09:01:37.608417 mosaik_heatpump-1.0.1/mosaik_components/__init__.py
+-rw-r--r--   0        0        0    27610 2024-04-30 09:01:37.575417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/Heat_Pump_Design.py
+-rw-r--r--   0        0        0     6906 2024-04-30 09:01:37.575417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/Heat_Pump_Model.py
+-rw-r--r--   0        0        0     3820 2024-04-30 09:01:37.575417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/Heat_Pump_mosaik.py
+-rw-r--r--   0        0        0       82 2024-04-30 09:01:37.575417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:01:37.609417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/controller/__init__.py
+-rw-r--r--   0        0        0    11680 2024-04-30 09:01:37.575417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/controller/controller.py
+-rw-r--r--   0        0        0     4727 2024-04-30 09:01:37.575417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/controller/controller_mosaik.py
+-rw-r--r--   0        0        0     2108 2024-04-30 09:01:37.575417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/coolingloadsim/coolingloadsim.py
+-rw-r--r--   0        0        0     2530 2024-04-30 09:01:37.576417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/coolingloadsim/coolingloadsim_mosaik.py
+-rw-r--r--   0        0        0  3723869 2024-04-30 09:01:37.582417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/cop_m_data.json
+-rw-r--r--   0        0        0   145584 2024-04-30 09:01:37.583417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/eta_s_data.json
+-rw-r--r--   0        0        0        0 2024-04-30 09:01:37.609417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/hotwatertank/__init__.py
+-rw-r--r--   0        0        0    24369 2024-04-30 09:01:37.583417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/hotwatertank/hotwatertank.py
+-rw-r--r--   0        0        0     5828 2024-04-30 09:01:37.583417 mosaik_heatpump-1.0.1/mosaik_components/heatpump/hotwatertank/hotwatertank_mosaik.py
+-rw-r--r--   0        0        0      793 2024-04-30 09:01:37.583417 mosaik_heatpump-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 mosaik_heatpump-1.0.1/PKG-INFO
```

### Comparing `mosaik_heatpump-1.0.0/LICENSE` & `mosaik_heatpump-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/README.rst` & `mosaik_heatpump-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/Heat_Pump_Design.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/Heat_Pump_Design.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/Heat_Pump_Model.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/Heat_Pump_Model.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/Heat_Pump_mosaik.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/Heat_Pump_mosaik.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/controller/controller.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/controller/controller.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/controller/controller_mosaik.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/controller/controller_mosaik.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/coolingloadsim/coolingloadsim.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/coolingloadsim/coolingloadsim.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/coolingloadsim/coolingloadsim_mosaik.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/coolingloadsim/coolingloadsim_mosaik.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/cop_m_data.json` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/cop_m_data.json`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/eta_s_data.json` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/eta_s_data.json`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/hotwatertank/hotwatertank.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/hotwatertank/hotwatertank.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/mosaik_components/heatpump/hotwatertank/hotwatertank_mosaik.py` & `mosaik_heatpump-1.0.1/mosaik_components/heatpump/hotwatertank/hotwatertank_mosaik.py`

 * *Files identical despite different names*

### Comparing `mosaik_heatpump-1.0.0/pyproject.toml` & `mosaik_heatpump-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "mosaik-heatpump"
-version = "1.0.0"
+version = "1.0.1"
 description = "mosaik-heatpump provides models for the simulation of heating systems"
 authors = ["Pranay Kasturi <mosaik@offis.de>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{ include = "mosaik_components" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 mosaik-api = ">=3.0"
-tespy = ">=0.4.2"
+tespy = ">=0.4.2,<0.7.0"
 jsonpickle = "^3.0.2"
 hplib = "^1.9"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.11.3"
 
 [tool.poetry.group.test.dependencies]
-mosaik = "^3.2.0"
+mosaik = ">=3.2.0,<3.3.0"
 mosaik-csv = "^2.0.0"
 mosaik-hdf5 = "^0.4"
 pytest = "^7.4.3"
 
 [tool.poetry.group.jupyter.dependencies]
 matplotlib = "^3.7.4"
 ipykernel = "^6.27.1"
```

### Comparing `mosaik_heatpump-1.0.0/PKG-INFO` & `mosaik_heatpump-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-heatpump
-Version: 1.0.0
+Version: 1.0.1
 Summary: mosaik-heatpump provides models for the simulation of heating systems
 License: MIT
 Author: Pranay Kasturi
 Author-email: mosaik@offis.de
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: hplib (>=1.9,<2.0)
 Requires-Dist: jsonpickle (>=3.0.2,<4.0.0)
 Requires-Dist: mosaik-api (>=3.0)
-Requires-Dist: tespy (>=0.4.2)
+Requires-Dist: tespy (>=0.4.2,<0.7.0)
 Description-Content-Type: text/x-rst
 
 mosaik-heatpump
 ===============
 
 This package provides models for the simulation of heating systems- consisting of heat pumps, hot water tanks,
 and controllers - and adapters for the co-simulation of these models using *mosaik*.
```

