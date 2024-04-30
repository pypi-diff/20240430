# Comparing `tmp/imgw_pib-0.0.5.tar.gz` & `tmp/imgw_pib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgw_pib-0.0.5.tar", last modified: Wed Apr 24 15:14:49 2024, max compression
+gzip compressed data, was "imgw_pib-1.0.0.tar", last modified: Tue Apr 30 09:24:59 2024, max compression
```

## Comparing `imgw_pib-0.0.5.tar` & `imgw_pib-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/imgw_pib/
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/imgw_pib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:59.519933 imgw_pib-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-30 09:24:59.519933 imgw_pib-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:59.515933 imgw_pib-1.0.0/imgw_pib/
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:59.519933 imgw_pib-1.0.0/imgw_pib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:24:59.519933 imgw_pib-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:59.515933 imgw_pib-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/tests/test_init.py
```

### Comparing `imgw_pib-0.0.5/LICENSE` & `imgw_pib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imgw_pib-0.0.5/PKG-INFO` & `imgw_pib-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1
-Name: imgw_pib
-Version: 0.0.5
-Summary: Python wrapper for IMGW-PIB API.
-Home-page: https://github.com/bieniu/imgw-pib
-Author: Maciej Bieniek
-License: Apache-2.0 License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Typing :: Typed
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp>=3.8.0
-
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
 [![PayPal_Me][paypal-me-shield]][paypal-me]
 
 # imgw-pib
 
 Python async wrapper for IMGW-PIB API.
 
+## Installation
+
+You can install the library with pip:
+
+```
+pip install imgw-pib
+```
 
 ## How to use package
 
 ```python
 """Example of usage IMGW-PIB."""
 
 import asyncio
@@ -70,14 +58,22 @@
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
 ```
 
+## Error Handling
+
+The library raises `ApiError` when the IMGW-PIB API returns an error, `ClientError` for network-related errors, and `TimeoutError` when a request times out.
+
+## Contributing
+
+Contributions are welcome! Please feel free to submit a Pull Request.
+
 [releases]: https://github.com/bieniu/imgw-pib/releases
 [releases-shield]: https://img.shields.io/github/release/bieniu/imgw-pib.svg?style=popout
 [pypi-releases]: https://pypi.org/project/imgw-pib/
 [pypi-statistics]: https://pepy.tech/project/imgw-pib
 [pypi-releases-shield]: https://img.shields.io/pypi/v/imgw-pib
 [pypi-downloads]: https://pepy.tech/badge/imgw-pib/month
 [paypal-me-shield]: https://img.shields.io/static/v1.svg?label=%20&message=PayPal.Me&logo=paypal
```

### Comparing `imgw_pib-0.0.5/imgw_pib/__init__.py` & `imgw_pib-1.0.0/imgw_pib/__init__.py`

 * *Files identical despite different names*

### Comparing `imgw_pib-0.0.5/imgw_pib/model.py` & `imgw_pib-1.0.0/imgw_pib/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 
 @dataclass
 class ImgwPibData:
     """IMGW-PIB data class."""
 
 
-@dataclass
+@dataclass(kw_only=True, slots=True)
 class SensorData:
     """Data class for sensor."""
 
     name: str
     value: float | None = None
     unit: str | None = None
 
 
-@dataclass
+@dataclass(kw_only=True, slots=True)
 class WeatherData(ImgwPibData):
     """Weather Data class for IMGW-PIB."""
 
     temperature: SensorData
     humidity: SensorData
     pressure: SensorData
     wind_speed: SensorData
@@ -33,15 +33,15 @@
 
     station: str
     station_id: str
 
     measurement_date: datetime | None
 
 
-@dataclass
+@dataclass(kw_only=True, slots=True)
 class HydrologicalData(ImgwPibData):
     """Hudrological Data class for IMGW-PIB."""
 
     water_level: SensorData
     flood_alarm_level: SensorData
     flood_warning_level: SensorData
     water_temperature: SensorData
```

### Comparing `imgw_pib-0.0.5/imgw_pib.egg-info/PKG-INFO` & `imgw_pib-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: imgw_pib
-Version: 0.0.5
+Version: 1.0.0
 Summary: Python wrapper for IMGW-PIB API.
 Home-page: https://github.com/bieniu/imgw-pib
 Author: Maciej Bieniek
 License: Apache-2.0 License
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
@@ -22,14 +23,21 @@
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
 [![PayPal_Me][paypal-me-shield]][paypal-me]
 
 # imgw-pib
 
 Python async wrapper for IMGW-PIB API.
 
+## Installation
+
+You can install the library with pip:
+
+```
+pip install imgw-pib
+```
 
 ## How to use package
 
 ```python
 """Example of usage IMGW-PIB."""
 
 import asyncio
@@ -70,14 +78,22 @@
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
 ```
 
+## Error Handling
+
+The library raises `ApiError` when the IMGW-PIB API returns an error, `ClientError` for network-related errors, and `TimeoutError` when a request times out.
+
+## Contributing
+
+Contributions are welcome! Please feel free to submit a Pull Request.
+
 [releases]: https://github.com/bieniu/imgw-pib/releases
 [releases-shield]: https://img.shields.io/github/release/bieniu/imgw-pib.svg?style=popout
 [pypi-releases]: https://pypi.org/project/imgw-pib/
 [pypi-statistics]: https://pepy.tech/project/imgw-pib
 [pypi-releases-shield]: https://img.shields.io/pypi/v/imgw-pib
 [pypi-downloads]: https://pepy.tech/badge/imgw-pib/month
 [paypal-me-shield]: https://img.shields.io/static/v1.svg?label=%20&message=PayPal.Me&logo=paypal
```

### Comparing `imgw_pib-0.0.5/pyproject.toml` & `imgw_pib-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imgw_pib-0.0.5/setup.py` & `imgw_pib-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.0.5"
+VERSION = "1.0.0"
 
 setup(
     name="imgw_pib",
     version=VERSION,
     author="Maciej Bieniek",
     description="Python wrapper for IMGW-PIB API.",
     long_description=README_FILE.read_text(encoding="utf-8"),
@@ -19,14 +19,15 @@
     url="https://github.com/bieniu/imgw-pib",
     license="Apache-2.0 License",
     packages=["imgw_pib"],
     package_data={"imgw_pib": ["py.typed"]},
     python_requires=">=3.12",
     install_requires=["aiohttp>=3.8.0"],
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Typing :: Typed",
```

### Comparing `imgw_pib-0.0.5/tests/test_init.py` & `imgw_pib-1.0.0/tests/test_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,24 +226,26 @@
             await imgwpib.get_hydrological_data()
 
     await session.close()
 
     assert str(exc.value) == "Invalid water level value"
 
 
+@pytest.mark.parametrize("date_time", [None, "lorem ipsum"])
 @pytest.mark.asyncio()
 async def test_invalid_date(
     hydrological_stations: list[dict[str, Any]],
     hydrological_station: dict[str, Any],
     hydrological_details: dict[str, Any],
+    date_time: str | None,
 ) -> None:
     """Test invalid water level value."""
     session = aiohttp.ClientSession()
 
-    hydrological_station[ApiNames.WATER_LEVEL_MEASUREMENT_DATE] = None
+    hydrological_station[ApiNames.WATER_LEVEL_MEASUREMENT_DATE] = date_time
 
     with aioresponses() as session_mock:
         session_mock.get(API_HYDROLOGICAL_ENDPOINT, payload=hydrological_stations)
         session_mock.get(
             f"{API_HYDROLOGICAL_ENDPOINT}/id/154190050", payload=hydrological_station
         )
         session_mock.get(
```

