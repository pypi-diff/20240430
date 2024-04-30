# Comparing `tmp/aveas_openlabel-0.4.8.tar.gz` & `tmp/aveas_openlabel-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aveas_openlabel-0.4.8.tar", max compression
+gzip compressed data, was "aveas_openlabel-0.4.9.tar", max compression
```

## Comparing `aveas_openlabel-0.4.8.tar` & `aveas_openlabel-0.4.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1070 2024-02-27 13:47:22.745969 aveas_openlabel-0.4.8/LICENSE
--rw-r--r--   0        0        0     2921 2024-02-27 13:47:22.745969 aveas_openlabel-0.4.8/README.md
--rw-r--r--   0        0        0    29325 2024-02-27 13:47:22.745969 aveas_openlabel-0.4.8/aveas_openlabel/__init__.py
--rw-r--r--   0        0        0     2583 2024-02-27 13:47:22.745969 aveas_openlabel-0.4.8/aveas_openlabel/attribute_enforcer.py
--rw-r--r--   0        0        0     1137 2024-02-27 13:47:22.745969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/__init__.py
--rw-r--r--   0        0        0     3399 2024-02-27 13:47:22.745969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/dimension.py
--rw-r--r--   0        0        0     7543 2024-02-27 13:47:22.745969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/general.py
--rw-r--r--   0        0        0     3698 2024-02-27 13:47:22.745969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/hmi_feedback.py
--rw-r--r--   0        0        0     3603 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/impact.py
--rw-r--r--   0        0        0     6878 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/interior.py
--rw-r--r--   0        0        0     4020 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/lights.py
--rw-r--r--   0        0        0     2842 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/open_drive.py
--rw-r--r--   0        0        0    13094 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/operator.py
--rw-r--r--   0        0        0     5696 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/road.py
--rw-r--r--   0        0        0    11794 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/summary.py
--rw-r--r--   0        0        0     3710 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/attributes/traffic.py
--rw-r--r--   0        0        0     4781 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/aveas_openlabel.py
--rw-r--r--   0        0        0     1149 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/__init__.py
--rw-r--r--   0        0        0     3028 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/animal.py
--rw-r--r--   0        0        0     2931 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/bicycle.py
--rw-r--r--   0        0        0     2882 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/bus.py
--rw-r--r--   0        0        0     2882 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/car.py
--rw-r--r--   0        0        0     3068 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/human_pedestrian.py
--rw-r--r--   0        0        0     3020 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/mobility_device.py
--rw-r--r--   0        0        0     2967 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/motorcycle.py
--rw-r--r--   0        0        0     2874 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/other_classification.py
--rw-r--r--   0        0        0     3121 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/pushable_pullable.py
--rw-r--r--   0        0        0     3015 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/railvehicle.py
--rw-r--r--   0        0        0     3060 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/trailer.py
--rw-r--r--   0        0        0     2920 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/truck.py
--rw-r--r--   0        0        0     2882 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/classifications/van.py
--rw-r--r--   0        0        0     1157 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/contexts/__init__.py
--rw-r--r--   0        0        0     4622 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/contexts/environment_context.py
--rw-r--r--   0        0        0    12126 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/contexts/environment_context_data.py
--rw-r--r--   0        0        0     5558 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/contexts/scenario_context.py
--rw-r--r--   0        0        0    17051 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/contexts/scenario_context_data.py
--rw-r--r--   0        0        0     6087 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/event.py
--rw-r--r--   0        0        0     2267 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/frame.py
--rw-r--r--   0        0        0     3490 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/metadata.py
--rw-r--r--   0        0        0     1160 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_data/__init__.py
--rw-r--r--   0        0        0     5208 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_data/all.py
--rw-r--r--   0        0        0     5199 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_data/unattached.py
--rw-r--r--   0        0        0     4556 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_data/unsteerable.py
--rw-r--r--   0        0        0     4126 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_data/unsteerable_non_operator.py
--rw-r--r--   0        0        0     4565 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_data/unsteerable_unattached.py
--rw-r--r--   0        0        0     4165 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_data/unsteerable_unattached_non_operator.py
--rw-r--r--   0        0        0     1159 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/__init__.py
--rw-r--r--   0        0        0     6248 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/all.py
--rw-r--r--   0        0        0     6219 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/no_rider.py
--rw-r--r--   0        0        0     4008 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/non_vehicle.py
--rw-r--r--   0        0        0     2957 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/non_vehicle_non_operator.py
--rw-r--r--   0        0        0     4239 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/passive_vehicle_non_operator.py
--rw-r--r--   0        0        0     5944 2024-02-27 13:47:22.749969 aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/unsteerable.py
--rw-r--r--   0        0        0        0 2024-02-27 13:47:22.753969 aveas_openlabel-0.4.8/aveas_openlabel/py.typed
--rw-r--r--   0        0        0     2110 2024-02-27 13:47:22.753969 aveas_openlabel-0.4.8/aveas_openlabel/utils.py
--rw-r--r--   0        0        0     1872 2024-02-27 13:47:22.753969 aveas_openlabel-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 aveas_openlabel-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/LICENSE
+-rw-r--r--   0        0        0     2765 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/README.md
+-rw-r--r--   0        0        0    29294 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/__init__.py
+-rw-r--r--   0        0        0     2583 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attribute_enforcer.py
+-rw-r--r--   0        0        0     1137 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/__init__.py
+-rw-r--r--   0        0        0     3399 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/dimension.py
+-rw-r--r--   0        0        0     7543 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/general.py
+-rw-r--r--   0        0        0     3698 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/hmi_feedback.py
+-rw-r--r--   0        0        0     3603 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/impact.py
+-rw-r--r--   0        0        0     6878 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/interior.py
+-rw-r--r--   0        0        0     4020 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/lights.py
+-rw-r--r--   0        0        0     2842 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/open_drive.py
+-rw-r--r--   0        0        0    13094 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/operator.py
+-rw-r--r--   0        0        0     5696 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/road.py
+-rw-r--r--   0        0        0    11794 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/summary.py
+-rw-r--r--   0        0        0     3710 2024-03-11 10:29:30.342080 aveas_openlabel-0.4.9/aveas_openlabel/attributes/traffic.py
+-rw-r--r--   0        0        0     5217 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/aveas_openlabel.py
+-rw-r--r--   0        0        0     1149 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/__init__.py
+-rw-r--r--   0        0        0     3028 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/animal.py
+-rw-r--r--   0        0        0     2931 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/bicycle.py
+-rw-r--r--   0        0        0     2882 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/bus.py
+-rw-r--r--   0        0        0     2882 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/car.py
+-rw-r--r--   0        0        0     3068 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/human_pedestrian.py
+-rw-r--r--   0        0        0     3020 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/mobility_device.py
+-rw-r--r--   0        0        0     2967 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/motorcycle.py
+-rw-r--r--   0        0        0     2874 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/other_classification.py
+-rw-r--r--   0        0        0     3121 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/pushable_pullable.py
+-rw-r--r--   0        0        0     3015 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/railvehicle.py
+-rw-r--r--   0        0        0     3060 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/trailer.py
+-rw-r--r--   0        0        0     2920 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/truck.py
+-rw-r--r--   0        0        0     2882 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/classifications/van.py
+-rw-r--r--   0        0        0     1157 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/contexts/__init__.py
+-rw-r--r--   0        0        0     4622 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/contexts/environment_context.py
+-rw-r--r--   0        0        0    12126 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/contexts/environment_context_data.py
+-rw-r--r--   0        0        0     5268 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/contexts/scenario_context.py
+-rw-r--r--   0        0        0    15487 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/contexts/scenario_context_data.py
+-rw-r--r--   0        0        0     6008 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/event.py
+-rw-r--r--   0        0        0     2267 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/frame.py
+-rw-r--r--   0        0        0     3490 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/metadata.py
+-rw-r--r--   0        0        0     1160 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_data/__init__.py
+-rw-r--r--   0        0        0     5208 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_data/all.py
+-rw-r--r--   0        0        0     5199 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_data/unattached.py
+-rw-r--r--   0        0        0     4556 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_data/unsteerable.py
+-rw-r--r--   0        0        0     4126 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_data/unsteerable_non_operator.py
+-rw-r--r--   0        0        0     4565 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_data/unsteerable_unattached.py
+-rw-r--r--   0        0        0     4165 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_data/unsteerable_unattached_non_operator.py
+-rw-r--r--   0        0        0     1159 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/__init__.py
+-rw-r--r--   0        0        0     6248 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/all.py
+-rw-r--r--   0        0        0     6219 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/no_rider.py
+-rw-r--r--   0        0        0     4008 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/non_vehicle.py
+-rw-r--r--   0        0        0     2957 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/non_vehicle_non_operator.py
+-rw-r--r--   0        0        0     4239 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/passive_vehicle_non_operator.py
+-rw-r--r--   0        0        0     5944 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/unsteerable.py
+-rw-r--r--   0        0        0        0 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/py.typed
+-rw-r--r--   0        0        0     2110 2024-03-11 10:29:30.346080 aveas_openlabel-0.4.9/aveas_openlabel/utils.py
+-rw-r--r--   0        0        0     1872 2024-03-11 10:29:30.350080 aveas_openlabel-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     3518 1970-01-01 00:00:00.000000 aveas_openlabel-0.4.9/PKG-INFO
```

### Comparing `aveas_openlabel-0.4.8/LICENSE` & `aveas_openlabel-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/README.md` & `aveas_openlabel-0.4.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # AVEAS OpenLABEL
 
 ## Installation and usage
 
 This library can be installed via pip using `pip install aveas_openlabel` or with poetry using `poetry add aveas_openlabel`.
-
-For examples and instruction on how to use this library, please clone the repository and generate the documentation. 
-To generate the documentation for this project, install the dependencies with Poetry (see below) and run `poetry run pydoctor`. 
-Then, open the html page under `documentation/index.html`. 
+The documentation with minimal examples can be found here: [understand-ai.github.io/aveas_openlabel/](https://understand-ai.github.io/aveas_openlabel/)
 
 
 ## Development
 ### Poetry
 This package uses Poetry, a tool for dependency management and packaging. 
 Please install it via the official installer from [here](https://python-poetry.org/docs/).
 In the root of the repository, you install all dependencies into a virtual environment using `poetry install`.
```

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/__init__.py` & `aveas_openlabel-0.4.9/aveas_openlabel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 Writing AVEAS OpenLABEL files
 -----------------------------
 
 Writing a populated OpenLABEL dataclass structure to a JSON file is similarly simple
 
 >>> import json
 >>> from aveas_openlabel import AveasOpenLabel
->>> aveas_openlabel_example = AveasOpenLabel()
->>> # Code to populate aveas_openlabel_example
+>>> aveas_openlabel_example = AveasOpenLabel.minimum_example()
 >>> content = aveas_openlabel_example.to_dict()
 >>> with open("path/to/file.json", "w") as f:
 ...     json.dump(content, f)
 
 Obtaining a JSON schema file
 ----------------------------
```

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attribute_enforcer.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attribute_enforcer.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/__init__.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/dimension.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/dimension.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/general.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/general.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/hmi_feedback.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/hmi_feedback.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/impact.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/impact.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/interior.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/interior.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/lights.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/lights.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/open_drive.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/open_drive.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/operator.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/operator.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/road.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/road.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/summary.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/summary.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/attributes/traffic.py` & `aveas_openlabel-0.4.9/aveas_openlabel/attributes/traffic.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/aveas_openlabel.py` & `aveas_openlabel-0.4.9/aveas_openlabel/aveas_openlabel.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 )
 from uai_openlabel import (
     OpenLabel as BaseOpenLabel,
 )
 
 from aveas_openlabel.event import Event
 from aveas_openlabel.frame import Frame
-from aveas_openlabel.metadata import Metadata
+from aveas_openlabel.metadata import AcquisitionMethod, Metadata, RightOfUse
 
 __all__: list[str] = []
 
 
 @dataclass
 class AveasOpenLabel(BaseOpenLabel):
     """The AVEAS OpenLABEL class.
@@ -115,7 +115,18 @@
     streams: Optional[dict[StreamUid, Stream]] = field(default=None)
     """
         Streams (cameras, lidars) that were used to record the data. 
         Information about the sensors, such as intrinsic calibration information, is contained in this field. 
     """
 
     # tags: NOT SPECIFIED FOR AVEAS OPENLABEL
+
+    @classmethod
+    def minimum_example(cls: type["AveasOpenLabel"]) -> "AveasOpenLabel":
+        return cls(
+            metadata=Metadata(
+                right_of_use=RightOfUse.RESEARCH_ONLY,
+                acquisition_method=AcquisitionMethod.IN_VEHICLE,
+                acquisition_partner="foo bar institute",
+                acquisition_date="2000-01-01T01:01:01.001Z",
+            )
+        )
```

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/__init__.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/__init__.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/animal.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/animal.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/bicycle.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/bicycle.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/bus.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/bus.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/car.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/car.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/human_pedestrian.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/human_pedestrian.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/mobility_device.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/mobility_device.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/motorcycle.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/motorcycle.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/other_classification.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/other_classification.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/pushable_pullable.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/pushable_pullable.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/railvehicle.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/railvehicle.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/trailer.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/trailer.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/truck.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/truck.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/classifications/van.py` & `aveas_openlabel-0.4.9/aveas_openlabel/classifications/van.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/contexts/__init__.py` & `aveas_openlabel-0.4.9/aveas_openlabel/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/contexts/environment_context.py` & `aveas_openlabel-0.4.9/aveas_openlabel/contexts/environment_context.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/contexts/environment_context_data.py` & `aveas_openlabel-0.4.9/aveas_openlabel/contexts/environment_context_data.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/contexts/scenario_context.py` & `aveas_openlabel-0.4.9/aveas_openlabel/contexts/scenario_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,17 +44,14 @@
     Scenario__IsStaged,
     Scenario__MaximumVehicleSpeed,
     Scenario__MaximumVehicleSpeed__Frame,
     Scenario__MaximumVehicleSpeed__UStdDev,
     Scenario__MinimumVehicleDistanceS,
     Scenario__MinimumVehicleDistanceS__Frame,
     Scenario__MinimumVehicleDistanceS__UStdDev,
-    Scenario__MinimumVehicleDistanceT,
-    Scenario__MinimumVehicleDistanceT__Frame,
-    Scenario__MinimumVehicleDistanceT__UStdDev,
     Scenario__MinimumVehicleSpeed,
     Scenario__MinimumVehicleSpeed__Frame,
     Scenario__MinimumVehicleSpeed__UStdDev,
     Scenario__RatioAverageSpeedToSpeedLimit,
     Scenario__RatioAverageSpeedToSpeedLimit__UStdDev,
     Scenario__Start__Coordinates,
     Scenario__Start__Location,
@@ -86,31 +83,28 @@
         Union[
             Scenario__MinimumVehicleSpeed,
             Scenario__MinimumVehicleSpeed__UStdDev,
             Scenario__MaximumVehicleSpeed,
             Scenario__MaximumVehicleSpeed__UStdDev,
             Scenario__MinimumVehicleDistanceS,
             Scenario__MinimumVehicleDistanceS__UStdDev,
-            Scenario__MinimumVehicleDistanceT,
-            Scenario__MinimumVehicleDistanceT__UStdDev,
             Scenario__WeekdayNumber,
             Scenario__RatioAverageSpeedToSpeedLimit,
             Scenario__RatioAverageSpeedToSpeedLimit__UStdDev,
         ]
     ] = field(default_factory=lambda: no_default(field="ScenarioContextData.num"), metadata=required)
     """The numeric attributes of the `ScenarioContext`"""
 
     text: list[
         Union[
             Scenario__Start__Location,
             Scenario__End__Location,
             Scenario__IsSampled__ReferenceToSourceScenario,
             Scenario__MinimumVehicleSpeed__Frame,
             Scenario__MaximumVehicleSpeed__Frame,
-            Scenario__MinimumVehicleDistanceT__Frame,
             Scenario__MinimumVehicleDistanceS__Frame,
         ]
     ] = field(default_factory=lambda: no_default(field="ScenarioContextData.text"), metadata=required)
     """The textual attributes of the `ScenarioContext`"""
 
     vec: list[Union[Scenario__Start__Coordinates, Scenario__End__Coordinates, Scenario__Course]] = field(
         default_factory=lambda: no_default(field="ScenarioContextData.vec"), metadata=required
```

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/contexts/scenario_context_data.py` & `aveas_openlabel-0.4.9/aveas_openlabel/contexts/scenario_context_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,49 +117,14 @@
     """The frame ID for which Scenario__MinimumVehicleDistanceS occurs."""
 
     name: Literal["scenario/minimum_vehicle_distance_s/frame"] = field(default="scenario/minimum_vehicle_distance_s/frame")
     """Is always 'scenario/minimum_vehicle_distance_s/frame'"""
 
 
 @dataclass
-class Scenario__MinimumVehicleDistanceT(NumberData):
-    """The minimum distance between a moving vehicle and another traffic participant occurring in the scenario in orthogonal direction of the road's reference line."""
-
-    val: float = field(default_factory=lambda: no_default(field="Scenario__MinimumVehicleDistanceT.val"), metadata=required)
-    """The value of the minimum distance in orthogonal direction of the road's reference line."""
-
-    name: Literal["scenario/minimum_vehicle_distance_t"] = field(default="scenario/minimum_vehicle_distance_t")
-    """Is always 'scenario/minimum_vehicle_distance_t'"""
-
-
-@dataclass
-class Scenario__MinimumVehicleDistanceT__UStdDev(NumberData):
-    """Uncertainty for `Scenario__MinimumVehicleDistanceT` as standard deviation around the parent indicated value."""
-
-    val: float = field(default_factory=lambda: no_default(field="FrameMinimumVehicleDistanceT__UStdDev.val"), metadata=required)
-    """Standard deviation around the parent indicated value. """
-
-    name: Literal["scenario/minimum_vehicle_distance_t/ustddev"] = field(default="scenario/minimum_vehicle_distance_t/ustddev")
-    """Is always 'scenario/minimum_vehicle_distance_t/ustddev'."""
-
-
-@dataclass
-class Scenario__MinimumVehicleDistanceT__Frame(TextData):
-    """Specifying the frame ID for which Scenario__MinimumVehicleDistanceT occurs."""
-
-    val: str = field(
-        default_factory=lambda: no_default(field="Scenario__MinimumVehicleDistanceT__Frame.val"), metadata=required
-    )
-    """The frame ID for which Scenario__MinimumVehicleDistanceT occurs."""
-
-    name: Literal["scenario/minimum_vehicle_distance_t/frame"] = field(default="scenario/minimum_vehicle_distance_t/frame")
-    """Is always 'scenario/minimum_vehicle_distance_t/frame'"""
-
-
-@dataclass
 class Scenario__ContainsHighway(BooleanData):
     """Indicating if the scenario is (partially) taking place on highways."""
 
     val: bool = field(default_factory=lambda: no_default(field="Scenario__ContainsHighway.val"), metadata=required)
     """True iff the scenario is (partially) taking place on highways."""
 
     name: Literal["scenario/contains_highway"] = field(default="scenario/contains_highway")
@@ -325,15 +290,19 @@
 
     name: Literal["scenario/end/coordinates"] = field(default="scenario/end/coordinates")
     """Is always 'scenario/end/coordinates'"""
 
 
 @dataclass
 class Scenario__RatioAverageSpeedToSpeedLimit(NumberData):
-    """The average ratio between speed and speed limit over all road-based traffic participants and all frames in the file."""
+    """The average ratio between speed and speed limit over all road-based traffic participants and all frames in the file.
+
+    In case no speed limit is present, the denominator is set to the maximum available speed limit of
+    the country (e.g. 130 km/h for Germany) and 20 km/h is added to it (resulting in 150 km/h for Germany).
+    """
 
     val: float = field(
         default_factory=lambda: no_default(field="Scenario__RatioAverageSpeedToSpeedLimit.val"), metadata=required
     )
     """The average ratio between speed and speed limit over all road-based traffic participants and all frames in the file."""
 
     name: Literal["scenario/ratio_average_speed_to_speed_limit"] = field(default="scenario/ratio_average_speed_to_speed_limit")
```

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/event.py` & `aveas_openlabel-0.4.9/aveas_openlabel/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,15 @@
 )
 
 
 @dataclass
 class RoleAParticipantID(TextData):
     """Participant ID of traffic participant with Role A. Role A is dependent on the event type.
 
-    cut-in      :       vehicle performing the cut-in
-    cut-out     :       vehicle performing the cut-out
+    lane change :       vehicle performing the lane change
     parking     :       vehicle performing the parking maneuver
     turning     :       vehicle that is turning/crossing
     overtaking  :       vehicle that is overtaking
     following   :       vehicle that is following
 
     """
 
@@ -61,16 +60,15 @@
     """Is always 'value'"""
 
 
 @dataclass
 class RoleBParticipantIDs(VectorData):
     """Participant IDs of traffic participants with Role B. Role B is dependent on the event type.
 
-    cut-in      :       vehicle in front of which the cut-in of the Role A vehicle ends
-    cut-out     :       vehicle in front of the Role A vehicle at the start of the cut-out
+    lane change :       empty
     parking     :       vehicles passing the Role A vehicle during the parking event and using the lane closest to the Role A vehicle
     turning     :       vehicles being within the scene during the turning event of the Role A vehicle and whose line of movement crosses the one of the Role A vehicle
     overtaking  :       vehicles that are being overtaken by the Role A vehicle
     following   :       vehicle that is being followed by the Role A vehicle (the vehicle immediately in front)
 
     """
 
@@ -98,21 +96,16 @@
     vec: list[RoleBParticipantIDs] = field(default_factory=lambda: no_default(field="EventData.vec"), metadata=required)
     """A list containing a single attribute, an instance of `RoleBParticipantIDs`."""
 
 
 class EventTypeValue(str, Enum):
     """Possible values of `Event.type`."""
 
-    # TODO: add further events?
-
-    CUT_IN = "cut-in"
-    """Cut-in maneuver."""
-
-    CUT_OUT = "cut-out"
-    """Cut-out maneuver."""
+    LANE_CHANGE = "lane change"
+    """Lane change maneuver."""
 
     PARKING_MANEUVER = "parking"
     """Parking maneuver."""
 
     TURNING = "turning"
     """Turning maneuver."""
 
@@ -136,11 +129,14 @@
 
     name: str = field(default_factory=lambda: no_default(field="Event.name"), metadata=required)
     """Name of the event, equal to type of event concatenated with ID of event. """
 
     frame_intervals: list[FrameInterval] = field(
         default_factory=lambda: no_default(field="Event.frame_intervals"), metadata=required
     )
-    """The frame interval during which the event takes place."""
+    """The frame interval during which the event takes place. 
+    For a lane change, the start and end frame are the same because we annotate the point in time when the center 
+    of a vehicle is over the lane marking crossed during the lane change.
+    """
 
     type: EventTypeValue = field(default_factory=lambda: no_default(field="Event.type"), metadata=required)
     """The type of the event."""
```

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/frame.py` & `aveas_openlabel-0.4.9/aveas_openlabel/frame.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/metadata.py` & `aveas_openlabel-0.4.9/aveas_openlabel/metadata.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_data/__init__.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_data/__init__.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_data/all.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_data/all.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_data/unattached.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_data/unattached.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_data/unsteerable.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_data/unsteerable.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_data/unsteerable_non_operator.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_data/unsteerable_non_operator.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_data/unsteerable_unattached.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_data/unsteerable_unattached.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_data/unsteerable_unattached_non_operator.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_data/unsteerable_unattached_non_operator.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/__init__.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/__init__.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/all.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/all.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/no_rider.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/no_rider.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/non_vehicle.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/non_vehicle.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/non_vehicle_non_operator.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/non_vehicle_non_operator.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/passive_vehicle_non_operator.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/passive_vehicle_non_operator.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/object_in_frame_data/unsteerable.py` & `aveas_openlabel-0.4.9/aveas_openlabel/object_in_frame_data/unsteerable.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/aveas_openlabel/utils.py` & `aveas_openlabel-0.4.9/aveas_openlabel/utils.py`

 * *Files identical despite different names*

### Comparing `aveas_openlabel-0.4.8/pyproject.toml` & `aveas_openlabel-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aveas_openlabel"
-version = "0.4.8"
+version = "0.4.9"
 description = "The AVEAS OpenLABEL specification"
 license = "MIT"
 authors = ["understand.ai <postmaster@understand.ai>"]
 readme = "README.md"
 repository = "https://github.com/understand-ai/aveas_openlabel"
 keywords = ["ASAM OpenLABEL", "AVEAS"]
 packages = [{include = "aveas_openlabel"}]
```

### Comparing `aveas_openlabel-0.4.8/PKG-INFO` & `aveas_openlabel-0.4.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aveas_openlabel
-Version: 0.4.8
+Version: 0.4.9
 Summary: The AVEAS OpenLABEL specification
 Home-page: https://github.com/understand-ai/aveas_openlabel
 License: MIT
 Keywords: ASAM OpenLABEL,AVEAS
 Author: understand.ai
 Author-email: postmaster@understand.ai
 Requires-Python: >=3.9,<3.12
@@ -19,18 +19,15 @@
 Description-Content-Type: text/markdown
 
 # AVEAS OpenLABEL
 
 ## Installation and usage
 
 This library can be installed via pip using `pip install aveas_openlabel` or with poetry using `poetry add aveas_openlabel`.
-
-For examples and instruction on how to use this library, please clone the repository and generate the documentation. 
-To generate the documentation for this project, install the dependencies with Poetry (see below) and run `poetry run pydoctor`. 
-Then, open the html page under `documentation/index.html`. 
+The documentation with minimal examples can be found here: [understand-ai.github.io/aveas_openlabel/](https://understand-ai.github.io/aveas_openlabel/)
 
 
 ## Development
 ### Poetry
 This package uses Poetry, a tool for dependency management and packaging. 
 Please install it via the official installer from [here](https://python-poetry.org/docs/).
 In the root of the repository, you install all dependencies into a virtual environment using `poetry install`.
```

