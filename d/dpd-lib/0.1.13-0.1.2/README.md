# Comparing `tmp/dpd_lib-0.1.13.tar.gz` & `tmp/dpd_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpd_lib-0.1.13.tar", last modified: Mon Apr 29 23:29:22 2024, max compression
+gzip compressed data, was "dpd_lib-0.1.2.tar", last modified: Tue Apr 23 18:44:20 2024, max compression
```

## Comparing `dpd_lib-0.1.13.tar` & `dpd_lib-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 23:29:22.888475 dpd_lib-0.1.13/
--rw-r--r--   0 root         (0) root         (0)     2102 2024-04-29 23:29:22.888475 dpd_lib-0.1.13/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-29 23:27:16.000000 dpd_lib-0.1.13/PYPI.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 23:29:22.884475 dpd_lib-0.1.13/dpd_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 23:29:15.000000 dpd_lib-0.1.13/dpd_lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 23:29:22.884475 dpd_lib-0.1.13/dpd_lib/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 23:29:15.000000 dpd_lib-0.1.13/dpd_lib/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-29 23:27:16.000000 dpd_lib-0.1.13/dpd_lib/client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11658 2024-04-29 23:27:16.000000 dpd_lib-0.1.13/dpd_lib/client/influx.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-29 23:27:16.000000 dpd_lib-0.1.13/dpd_lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-29 23:27:16.000000 dpd_lib-0.1.13/dpd_lib/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 23:29:22.884475 dpd_lib-0.1.13/dpd_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2102 2024-04-29 23:29:22.000000 dpd_lib-0.1.13/dpd_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2024-04-29 23:29:22.000000 dpd_lib-0.1.13/dpd_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 23:29:22.000000 dpd_lib-0.1.13/dpd_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-29 23:29:22.000000 dpd_lib-0.1.13/dpd_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-29 23:29:22.000000 dpd_lib-0.1.13/dpd_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-29 23:27:16.000000 dpd_lib-0.1.13/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 23:29:22.888475 dpd_lib-0.1.13/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:44:20.753496 dpd_lib-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-23 18:44:20.753496 dpd_lib-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/PYPI.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:44:20.749496 dpd_lib-0.1.2/dpd_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:44:11.000000 dpd_lib-0.1.2/dpd_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:44:20.749496 dpd_lib-0.1.2/dpd_lib/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:44:11.000000 dpd_lib-0.1.2/dpd_lib/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/dpd_lib/client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11597 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/dpd_lib/client/influx.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/dpd_lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/dpd_lib/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:44:20.753496 dpd_lib-0.1.2/dpd_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 18:44:20.753496 dpd_lib-0.1.2/setup.cfg
```

### Comparing `dpd_lib-0.1.13/PKG-INFO` & `dpd_lib-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.1.13
+Version: 0.1.2
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.1.13/PYPI.md` & `dpd_lib-0.1.2/PYPI.md`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.1.13/dpd_lib/client/exceptions.py` & `dpd_lib-0.1.2/dpd_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.1.13/dpd_lib/client/influx.py` & `dpd_lib-0.1.2/dpd_lib/client/influx.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,16 @@
 from influxdb_client import InfluxDBClient, Point
 from influxdb_client.client.write_api import SYNCHRONOUS
 from influxdb_client.rest import ApiException
 from loguru import logger
 from pydantic import SecretStr
 from urllib3.exceptions import NewConnectionError
 
-INFRASOUND_TYPES = [
-    "",
-    "mdccm",
-    "velocity",
-    "riam",
-    "pressure",
-    "azimuth",
-    "envelope",
-]
-SEISMIC_TYPES = ["", "rsam", "envelope"]
+INFRASOUND_TYPES = ["", "mccm", "velocity", "rsam", "pressure", "azimuth"]
+SEISMIC_YPES = ["", "rsam"]
 
 
 class InfluxClient:
     """
     A restricted client which implements an interface
     to query data from the influx database.
 
@@ -98,17 +90,17 @@
             InfluxNotAvailableException: An error occurred
                 while contacting the InfluxDB.
             BadQueryException: There is an issue with the
                 influx query.
             BucketNotFoundException: The requested bucket
             is not present in the DB.
         """
-        if type not in SEISMIC_TYPES:
+        if type not in SEISMIC_YPES:
             raise BadQueryException(
-                f"Seismic type not accepted. Accepted types: {SEISMIC_TYPES}."
+                f"Seismic type not accepted. Accepted types: {SEISMIC_YPES}."
             )
         p = (
             Point(type)
             .tag("station", station)
             .field(type, value)
             .time(timestamp)
         )
@@ -138,17 +130,17 @@
             InfluxNotAvailableException: An error occurred
                 while contacting the InfluxDB.
             BadQueryException: There is an issue with the
                 influx query.
             BucketNotFoundException: The requested bucket
             is not present in the DB.
         """
-        if type not in SEISMIC_TYPES:
+        if type not in SEISMIC_YPES:
             raise BadQueryException(
-                f"Seismic type not accepted. Accepted types: {SEISMIC_TYPES}."
+                f"Seismic type not accepted. Accepted types: {SEISMIC_YPES}."
             )
         query = """from(bucket:"{0}")
         |> range(start: {1}, stop: {2})""".format(
             self.bucket,
             t0.strftime("%Y-%m-%dT%H:%M:%SZ"),
             t1.strftime("%Y-%m-%dT%H:%M:%SZ"),
         )
```

### Comparing `dpd_lib-0.1.13/dpd_lib/config.py` & `dpd_lib-0.1.2/dpd_lib/config.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.1.13/dpd_lib/models.py` & `dpd_lib-0.1.2/dpd_lib/models.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.1.13/dpd_lib.egg-info/PKG-INFO` & `dpd_lib-0.1.2/dpd_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.1.13
+Version: 0.1.2
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.1.13/pyproject.toml` & `dpd_lib-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpd_lib"
-version = "0.1.13"
+version = "0.1.2"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "PYPI.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

