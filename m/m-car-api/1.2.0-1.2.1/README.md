# Comparing `tmp/m_car_api-1.2.0.tar.gz` & `tmp/m_car_api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_car_api-1.2.0.tar", last modified: Sat Apr 13 14:36:53 2024, max compression
+gzip compressed data, was "m_car_api-1.2.1.tar", last modified: Tue Apr 30 21:12:13 2024, max compression
```

## Comparing `m_car_api-1.2.0.tar` & `m_car_api-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 14:36:53.936956 m_car_api-1.2.0/
--rw-r--r--   0 cbrand     (501) staff       (20)     1788 2024-04-13 14:36:53.936617 m_car_api-1.2.0/PKG-INFO
--rw-r--r--   0 cbrand     (501) staff       (20)       38 2024-04-13 14:36:53.937011 m_car_api-1.2.0/setup.cfg
--rw-r--r--   0 cbrand     (501) staff       (20)     2405 2024-04-13 14:36:28.000000 m_car_api-1.2.0/setup.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 14:36:53.930829 m_car_api-1.2.0/src/
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 14:36:53.932780 m_car_api-1.2.0/src/m_car_api/
--rw-r--r--   0 cbrand     (501) staff       (20)      116 2024-04-13 14:15:39.000000 m_car_api-1.2.0/src/m_car_api/__init__.py
--rw-r--r--   0 cbrand     (501) staff       (20)     5413 2024-04-13 14:32:22.000000 m_car_api-1.2.0/src/m_car_api/api.py
--rw-r--r--   0 cbrand     (501) staff       (20)     1169 2024-04-05 14:53:41.000000 m_car_api-1.2.0/src/m_car_api/const.py
--rw-r--r--   0 cbrand     (501) staff       (20)     1123 2024-04-13 14:32:54.000000 m_car_api-1.2.0/src/m_car_api/geo.py
--rw-r--r--   0 cbrand     (501) staff       (20)      467 2024-04-13 12:37:15.000000 m_car_api-1.2.0/src/m_car_api/objects.py
--rw-r--r--   0 cbrand     (501) staff       (20)    11122 2024-04-13 12:34:26.000000 m_car_api-1.2.0/src/m_car_api/objects_pydantic_1.py
--rw-r--r--   0 cbrand     (501) staff       (20)     9884 2024-04-13 12:36:48.000000 m_car_api-1.2.0/src/m_car_api/objects_pydantic_2.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 14:36:53.934572 m_car_api-1.2.0/src/m_car_api/test/
--rw-r--r--   0 cbrand     (501) staff       (20)      901 2024-04-05 15:37:57.000000 m_car_api-1.2.0/src/m_car_api/test/test_miles_api.py
--rw-r--r--   0 cbrand     (501) staff       (20)      693 2024-04-13 14:15:14.000000 m_car_api-1.2.0/src/m_car_api/test/test_objects.py
-drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-13 14:36:53.934890 m_car_api-1.2.0/src/m_car_api.egg-info/
--rw-r--r--   0 cbrand     (501) staff       (20)     1788 2024-04-13 14:36:53.000000 m_car_api-1.2.0/src/m_car_api.egg-info/PKG-INFO
--rw-r--r--   0 cbrand     (501) staff       (20)      534 2024-04-13 14:36:53.000000 m_car_api-1.2.0/src/m_car_api.egg-info/SOURCES.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 14:36:53.000000 m_car_api-1.2.0/src/m_car_api.egg-info/dependency_links.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-13 14:36:53.000000 m_car_api-1.2.0/src/m_car_api.egg-info/namespace_packages.txt
--rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-05 15:37:20.000000 m_car_api-1.2.0/src/m_car_api.egg-info/not-zip-safe
--rw-r--r--   0 cbrand     (501) staff       (20)      354 2024-04-13 14:36:53.000000 m_car_api-1.2.0/src/m_car_api.egg-info/requires.txt
--rw-r--r--   0 cbrand     (501) staff       (20)       10 2024-04-13 14:36:53.000000 m_car_api-1.2.0/src/m_car_api.egg-info/top_level.txt
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-30 21:12:13.361271 m_car_api-1.2.1/
+-rw-r--r--   0 cbrand     (501) staff       (20)     1788 2024-04-30 21:12:13.361036 m_car_api-1.2.1/PKG-INFO
+-rw-r--r--   0 cbrand     (501) staff       (20)       38 2024-04-30 21:12:13.361323 m_car_api-1.2.1/setup.cfg
+-rw-r--r--   0 cbrand     (501) staff       (20)     2405 2024-04-30 21:11:44.000000 m_car_api-1.2.1/setup.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-30 21:12:13.356958 m_car_api-1.2.1/src/
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-30 21:12:13.358181 m_car_api-1.2.1/src/m_car_api/
+-rw-r--r--   0 cbrand     (501) staff       (20)      116 2024-04-13 14:15:39.000000 m_car_api-1.2.1/src/m_car_api/__init__.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     5413 2024-04-13 14:32:22.000000 m_car_api-1.2.1/src/m_car_api/api.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     1169 2024-04-05 14:53:41.000000 m_car_api-1.2.1/src/m_car_api/const.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     1123 2024-04-13 14:32:54.000000 m_car_api-1.2.1/src/m_car_api/geo.py
+-rw-r--r--   0 cbrand     (501) staff       (20)      467 2024-04-13 12:37:15.000000 m_car_api-1.2.1/src/m_car_api/objects.py
+-rw-r--r--   0 cbrand     (501) staff       (20)    11208 2024-04-30 21:10:56.000000 m_car_api-1.2.1/src/m_car_api/objects_pydantic_1.py
+-rw-r--r--   0 cbrand     (501) staff       (20)     9968 2024-04-30 21:11:07.000000 m_car_api-1.2.1/src/m_car_api/objects_pydantic_2.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-30 21:12:13.359447 m_car_api-1.2.1/src/m_car_api/test/
+-rw-r--r--   0 cbrand     (501) staff       (20)      901 2024-04-05 15:37:57.000000 m_car_api-1.2.1/src/m_car_api/test/test_miles_api.py
+-rw-r--r--   0 cbrand     (501) staff       (20)      693 2024-04-13 14:15:14.000000 m_car_api-1.2.1/src/m_car_api/test/test_objects.py
+drwxr-xr-x   0 cbrand     (501) staff       (20)        0 2024-04-30 21:12:13.359625 m_car_api-1.2.1/src/m_car_api.egg-info/
+-rw-r--r--   0 cbrand     (501) staff       (20)     1788 2024-04-30 21:12:13.000000 m_car_api-1.2.1/src/m_car_api.egg-info/PKG-INFO
+-rw-r--r--   0 cbrand     (501) staff       (20)      534 2024-04-30 21:12:13.000000 m_car_api-1.2.1/src/m_car_api.egg-info/SOURCES.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-30 21:12:13.000000 m_car_api-1.2.1/src/m_car_api.egg-info/dependency_links.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-30 21:12:13.000000 m_car_api-1.2.1/src/m_car_api.egg-info/namespace_packages.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)        1 2024-04-05 15:37:20.000000 m_car_api-1.2.1/src/m_car_api.egg-info/not-zip-safe
+-rw-r--r--   0 cbrand     (501) staff       (20)      354 2024-04-30 21:12:13.000000 m_car_api-1.2.1/src/m_car_api.egg-info/requires.txt
+-rw-r--r--   0 cbrand     (501) staff       (20)       10 2024-04-30 21:12:13.000000 m_car_api-1.2.1/src/m_car_api.egg-info/top_level.txt
```

### Comparing `m_car_api-1.2.0/PKG-INFO` & `m_car_api-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_car_api
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/cbrand/m_car_api
 Author: Christoph Brand
 Author-email: christoph@brand.rest
 License: MIT
 Project-URL: GitHub, https://github.com/cbrand/m_car_api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `m_car_api-1.2.0/setup.py` & `m_car_api-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def get_package_dir() -> Dict[str, str]:
     if not os.path.isdir("src"):
         return {}
     return {"": "src"}
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 requirements = ["requests", "mujson", "pydantic"]
 pydantic_1 = ["pydantic>=1,<2", "pydantic_computed"]
 pydantic_2 = ["pydantic>=2,<3"]
 pyproj = ["pyproj"]
 test_requirements = [
     "black>=19.10b0",
     "coverage>=5.1,<7",
```

### Comparing `m_car_api-1.2.0/src/m_car_api/api.py` & `m_car_api-1.2.1/src/m_car_api/api.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.2.0/src/m_car_api/const.py` & `m_car_api-1.2.1/src/m_car_api/const.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.2.0/src/m_car_api/geo.py` & `m_car_api-1.2.1/src/m_car_api/geo.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.2.0/src/m_car_api/objects_pydantic_1.py` & `m_car_api-1.2.1/src/m_car_api/objects_pydantic_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,20 +238,22 @@
     rookie_delay_txt: str = Field(alias="RookieDelayTxt")
     number_days_rookies_delay: int = Field(alias="nDaysRookieDelay")
     premium_restricted_txt: str = Field(alias="PremiumRestrictedTxt")
     city_to_city_options_string: str | None = Field(
         alias="CityToCityOptions", exclude=True
     )
 
-    city_to_city_options: Computed[CityToCityOptions]
+    city_to_city_options: Computed[CityToCityOptions | None]
 
     @computed("city_to_city_options")
     def compute_city_to_city_options(
         city_to_city_options_string: str, **kwargs: Any
-    ) -> CityToCityOptions:
+    ) -> CityToCityOptions | None:
+        if city_to_city_options_string is None:
+            return None
         payload = mujson.loads(city_to_city_options_string)
         return CityToCityOptions.parse_obj(payload)
 
     json_vehicle_damages_input: str | None = Field(
         alias="JSONVehicleDamages", exclude=True
     )
```

### Comparing `m_car_api-1.2.0/src/m_car_api/objects_pydantic_2.py` & `m_car_api-1.2.1/src/m_car_api/objects_pydantic_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,17 @@
     premium_restricted_txt: str = Field(alias="PremiumRestrictedTxt")
     city_to_city_options_string: str | None = Field(
         alias="CityToCityOptions", exclude=True
     )
 
     @computed_field
     @property
-    def city_to_city_options(self) -> CityToCityOptions:
+    def city_to_city_options(self) -> CityToCityOptions | None:
+        if self.city_to_city_options_string is None:
+            return None
         return CityToCityOptions.model_validate_json(self.city_to_city_options_string)
 
     json_vehicle_damages_input: str | None = Field(
         alias="JSONVehicleDamages", exclude=True
     )
 
     @computed_field
```

### Comparing `m_car_api-1.2.0/src/m_car_api/test/test_miles_api.py` & `m_car_api-1.2.1/src/m_car_api/test/test_miles_api.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.2.0/src/m_car_api/test/test_objects.py` & `m_car_api-1.2.1/src/m_car_api/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `m_car_api-1.2.0/src/m_car_api.egg-info/PKG-INFO` & `m_car_api-1.2.1/src/m_car_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_car_api
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/cbrand/m_car_api
 Author: Christoph Brand
 Author-email: christoph@brand.rest
 License: MIT
 Project-URL: GitHub, https://github.com/cbrand/m_car_api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `m_car_api-1.2.0/src/m_car_api.egg-info/SOURCES.txt` & `m_car_api-1.2.1/src/m_car_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

