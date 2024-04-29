# Comparing `tmp/pynws-1.6.0.tar.gz` & `tmp/pynws-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynws-1.6.0.tar", last modified: Tue Sep 12 19:51:10 2023, max compression
+gzip compressed data, was "pynws-1.7.0.tar", last modified: Mon Apr 29 23:20:33 2024, max compression
```

## Comparing `pynws-1.6.0.tar` & `pynws-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 19:51:10.180434 pynws-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-12 19:50:57.000000 pynws-1.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-09-12 19:50:57.000000 pynws-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-09-12 19:50:57.000000 pynws-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-09-12 19:51:10.180434 pynws-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-09-12 19:50:57.000000 pynws-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 19:51:10.180434 pynws-1.6.0/pynws/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 19:51:10.180434 pynws-1.6.0/pynws/backports/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/backports/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/nws.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14147 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/simple_nws.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-09-12 19:50:57.000000 pynws-1.6.0/pynws/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 19:51:10.180434 pynws-1.6.0/pynws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-09-12 19:51:10.000000 pynws-1.6.0/pynws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-09-12 19:51:10.000000 pynws-1.6.0/pynws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 19:51:10.000000 pynws-1.6.0/pynws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-12 19:51:10.000000 pynws-1.6.0/pynws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-12 19:51:10.000000 pynws-1.6.0/pynws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-09-12 19:50:57.000000 pynws-1.6.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-12 19:51:10.184434 pynws-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-09-12 19:50:57.000000 pynws-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.446124 pynws-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 23:20:28.000000 pynws-1.7.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.438125 pynws-1.7.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-29 23:20:28.000000 pynws-1.7.0/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-04-29 23:20:28.000000 pynws-1.7.0/.devcontainer/postcreatecommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.438125 pynws-1.7.0/.devcontainer/python3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 23:20:28.000000 pynws-1.7.0/.devcontainer/python3.9/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 23:20:28.000000 pynws-1.7.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.438125 pynws-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-29 23:20:28.000000 pynws-1.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.438125 pynws-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-29 23:20:28.000000 pynws-1.7.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 23:20:28.000000 pynws-1.7.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 23:20:28.000000 pynws-1.7.0/.github/workflows/typing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-29 23:20:28.000000 pynws-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 23:20:28.000000 pynws-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-29 23:20:28.000000 pynws-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-29 23:20:28.000000 pynws-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-29 23:20:33.446124 pynws-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-29 23:20:28.000000 pynws-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-29 23:20:28.000000 pynws-1.7.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-29 23:20:28.000000 pynws-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-29 23:20:28.000000 pynws-1.7.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:20:33.446124 pynws-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.434125 pynws-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.442124 pynws-1.7.0/src/pynws/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.442124 pynws-1.7.0/src/pynws/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/backports/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15711 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/simple_nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.446124 pynws-1.7.0/src/pynws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.442124 pynws-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.446124 pynws-1.7.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/alerts_active_zone.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/alerts_active_zone_second.json
+-rw-r--r--   0 runner    (1001) docker     (127)   132083 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/detailed_forecast.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_forecast.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_forecast_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_forecast_hourly.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_forecast_strings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45128 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_stations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/points.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_alternate_units.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_latest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_metar.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_metar_noparse.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_missing_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_multiple.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_multiple_unsorted.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_noprop.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_other_unitcode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_strings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/test_nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/test_simple_nws.py
```

### Comparing `pynws-1.6.0/LICENSE` & `pynws-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynws-1.6.0/PKG-INFO` & `pynws-1.7.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: pynws
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python library to retrieve observations and forecasts from NWS/NOAA
-Home-page: https://github.com/MatthewFlamm/pynws
-Author: Matthew Flamm
-Author-email: matthewflamm0@gmail.com
+Author-email: Matthew Flamm <matthewhflamm0@gmail.com>
 License: MIT License
+Project-URL: Repository, https://github.com/MatthewFlamm/pynws
+Project-URL: Bug Tracker, https://github.com/MatthewFlamm/pynws/issues
+Keywords: nws,weather
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: metar
+Provides-Extra: retry
+Requires-Dist: tenacity; extra == "retry"
 
 # pynws
 
 A python library to asynchronously retrieve weather observation from NWS/NOAA.
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pynws?style=flat-square)
```

### Comparing `pynws-1.6.0/README.md` & `pynws-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pynws-1.6.0/pynws/backports/enum.py` & `pynws-1.7.0/src/pynws/backports/enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Python 3.11 Enum backports from https://github.com/home-assistant/core/tree/dev/homeassistant/backports"""
+
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, List, TypeVar
 
 _StrEnumT = TypeVar("_StrEnumT", bound="StrEnum")
```

### Comparing `pynws-1.6.0/pynws/const.py` & `pynws-1.7.0/src/pynws/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """
 Constants for pynws
 """
+
+from enum import unique
 import os
 import sys
-from enum import unique
+from typing import Final
 
-from .backports.enum import StrEnum
-from .version import __version__
-
-if sys.version_info >= (3, 8):
-    from typing import Final
+if sys.version_info >= (3, 11):
+    from enum import StrEnum
 else:
-    from typing_extensions import Final
-
+    from .backports.enum import StrEnum
 
 file_dir = os.path.join(os.path.dirname(__file__), "..")
 
-version = __version__
-
 API_URL: Final = "https://api.weather.gov/"
 API_GRIDPOINTS_STATIONS: Final = "gridpoints/{}/{},{}/stations"
 API_STATIONS_OBSERVATIONS: Final = "stations/{}/observations/"
 API_STATIONS_OBSERVATIONS_LATEST: Final = "stations/{}/observations/latest"
 API_ACCEPT: Final = "application/geo+json"
 API_USER: Final = "pynws {}"
 API_DETAILED_FORECAST: Final = "gridpoints/{}/{},{}"
```

### Comparing `pynws-1.6.0/pynws/forecast.py` & `pynws-1.7.0/src/pynws/forecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Forecast classes"""
+
 from __future__ import annotations
 
-import re
 from datetime import datetime, timedelta, timezone
+import re
 from typing import Any, Dict, Iterable, Iterator, List, Tuple, Union
 
 from .const import Detail, Final
 from .units import get_converter
 
 ISO8601_PERIOD_REGEX: Final = re.compile(
     r"^P"
```

### Comparing `pynws-1.6.0/pynws/nws.py` & `pynws-1.7.0/src/pynws/nws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pynws module."""
+
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple, cast
 
 from aiohttp import ClientSession
```

### Comparing `pynws-1.6.0/pynws/raw_data.py` & `pynws-1.7.0/src/pynws/raw_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Functions to retrieve raw data."""
-import logging
+
 from datetime import datetime
+import logging
 from typing import Any, Dict, Optional
 
 from aiohttp import ClientSession
 
 from . import urls
 from .const import API_ACCEPT, API_USER
```

### Comparing `pynws-1.6.0/pynws/simple_nws.py` & `pynws-1.7.0/src/pynws/simple_nws.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 """Support for NWS weather service."""
+
 from __future__ import annotations
 
 from datetime import datetime, timezone
 from statistics import mean
-from typing import Any, Dict, List, NamedTuple, Optional, Set, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    NamedTuple,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+)
+
+if TYPE_CHECKING:
+    from datetime import timedelta
 
-from aiohttp import ClientSession
+from aiohttp import ClientResponseError, ClientSession
 from metar import Metar
 
 from .const import ALERT_ID, API_WEATHER_CODE, Final
 from .forecast import DetailedForecast
 from .nws import Nws, NwsError
 from .units import convert_unit
 
@@ -32,14 +48,61 @@
     "NNW",
 ]
 
 
 WIND: Final = {name: idx * 360 / 16 for idx, name in enumerate(WIND_DIRECTIONS)}
 
 
+def _is_500_error(error: BaseException) -> bool:
+    """Return True if error is ClientResponseError and has a 5xx status."""
+    return isinstance(error, ClientResponseError) and error.status >= 500
+
+
+def _setup_retry_func(
+    func: Callable[[Any, Any], Awaitable[Any]],
+    interval: Union[float, timedelta],
+    stop: Union[float, timedelta],
+) -> Callable[[Any, Any], Awaitable[Any]]:
+    from tenacity import retry, retry_if_exception, stop_after_delay, wait_fixed
+
+    return retry(
+        reraise=True,
+        wait=wait_fixed(interval),
+        stop=stop_after_delay(stop),
+        retry=retry_if_exception(_is_500_error),
+    )(func)
+
+
+async def call_with_retry(
+    func: Callable[[Any, Any], Awaitable[Any]],
+    interval: Union[float, timedelta],
+    stop: Union[float, timedelta],
+    /,
+    *args,
+    **kwargs,
+) -> Callable[[Any, Any], Awaitable[Any]]:
+    """Call an update function with retries.
+
+    Parameters
+    ----------
+    func : Callable
+        An awaitable coroutine to retry.
+    interval : float, datetime.datetime.timedelta
+        Time interval for retry.
+    stop : float, datetime.datetime.timedelta
+        Time interval to stop retrying.
+    args : Any
+        Positional args to pass to func.
+    kwargs : Any
+        Keyword args to pass to func.
+    """
+    retried_func = _setup_retry_func(func, interval, stop)
+    return await retried_func(*args, **kwargs)
+
+
 class MetarParam(NamedTuple):
     """METAR conversion parameter"""
 
     attr: str
     units: Optional[str] = None
     multiplier: Optional[float] = None
```

### Comparing `pynws-1.6.0/pynws/units.py` & `pynws-1.7.0/src/pynws/units.py`

 * *Files identical despite different names*

### Comparing `pynws-1.6.0/pynws/urls.py` & `pynws-1.7.0/src/pynws/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """url formatter."""
+
 from .const import (
     API_ALERTS_ACTIVE_ZONE,
     API_DETAILED_FORECAST,
     API_GRIDPOINTS_FORECAST,
     API_GRIDPOINTS_FORECAST_HOURLY,
     API_GRIDPOINTS_STATIONS,
     API_POINTS,
```

### Comparing `pynws-1.6.0/pynws.egg-info/PKG-INFO` & `pynws-1.7.0/src/pynws.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: pynws
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python library to retrieve observations and forecasts from NWS/NOAA
-Home-page: https://github.com/MatthewFlamm/pynws
-Author: Matthew Flamm
-Author-email: matthewflamm0@gmail.com
+Author-email: Matthew Flamm <matthewhflamm0@gmail.com>
 License: MIT License
+Project-URL: Repository, https://github.com/MatthewFlamm/pynws
+Project-URL: Bug Tracker, https://github.com/MatthewFlamm/pynws/issues
+Keywords: nws,weather
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: metar
+Provides-Extra: retry
+Requires-Dist: tenacity; extra == "retry"
 
 # pynws
 
 A python library to asynchronously retrieve weather observation from NWS/NOAA.
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pynws?style=flat-square)
```

