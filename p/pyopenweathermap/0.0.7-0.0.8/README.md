# Comparing `tmp/pyopenweathermap-0.0.7.tar.gz` & `tmp/pyopenweathermap-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenweathermap-0.0.7.tar", max compression
+gzip compressed data, was "pyopenweathermap-0.0.8.tar", max compression
```

## Comparing `pyopenweathermap-0.0.7.tar` & `pyopenweathermap-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.7/LICENSE
--rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.7/README.md
--rw-r--r--   0        0        0      568 2024-04-29 09:31:05.930254 pyopenweathermap-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.7/src/pyopenweathermap/__init__.py
--rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.7/src/pyopenweathermap/exception.py
--rw-r--r--   0        0        0     3032 2024-04-29 08:55:02.887184 pyopenweathermap-0.0.7/src/pyopenweathermap/owm_client.py
--rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.7/src/pyopenweathermap/weather.py
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 19:46:22.666091 pyopenweathermap-0.0.8/LICENSE
+-rw-r--r--   0        0        0       77 2024-04-24 19:48:45.962832 pyopenweathermap-0.0.8/README.md
+-rw-r--r--   0        0        0      568 2024-04-30 10:38:47.796234 pyopenweathermap-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      232 2024-04-26 09:04:44.323164 pyopenweathermap-0.0.8/src/pyopenweathermap/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-25 14:39:05.904017 pyopenweathermap-0.0.8/src/pyopenweathermap/exception.py
+-rw-r--r--   0        0        0     3228 2024-04-30 10:38:43.544211 pyopenweathermap-0.0.8/src/pyopenweathermap/owm_client.py
+-rw-r--r--   0        0        0     2534 2024-04-26 13:33:43.405295 pyopenweathermap-0.0.8/src/pyopenweathermap/weather.py
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 pyopenweathermap-0.0.8/PKG-INFO
```

### Comparing `pyopenweathermap-0.0.7/LICENSE` & `pyopenweathermap-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.7/pyproject.toml` & `pyopenweathermap-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyopenweathermap"
-version = "0.0.7"
+version = "0.0.8"
 description = "lib for OpenWeatherMap for Home Assistant"
 authors = ["Evgeny <iam@freekode.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["homeassistant", "owm", "openweathermap"]
 packages = [
     { include = "pyopenweathermap", from = "src" },
```

### Comparing `pyopenweathermap-0.0.7/src/pyopenweathermap/owm_client.py` & `pyopenweathermap-0.0.8/src/pyopenweathermap/owm_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,21 @@
                     elif response.status == 401:
                         raise UnauthorizedError(response_json.get('message'))
                     elif response.status == 404:
                         raise RequestError(response_json.get('message'))
                     elif response.status == 429:
                         raise TooManyRequestsError(response_json.get('message'))
                     else:
-                        raise RequestError("Unknown Error")
+                        raise RequestError("Unknown status code: {}".format(response.status))
             except TimeoutError:
                 raise RequestError("Request timeout")
+            except RequestError as error:
+                raise error
+            except Exception as error:
+                raise RequestError(error) from error
 
     def _get_url(self, lat, lon, exclude):
         return (f"{API_URL}?"
                 f"lat={lat}&"
                 f"lon={lon}&"
                 f"exclude={','.join(exclude)}&"
                 f"appid={self.api_key}&"
```

### Comparing `pyopenweathermap-0.0.7/src/pyopenweathermap/weather.py` & `pyopenweathermap-0.0.8/src/pyopenweathermap/weather.py`

 * *Files identical despite different names*

### Comparing `pyopenweathermap-0.0.7/PKG-INFO` & `pyopenweathermap-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenweathermap
-Version: 0.0.7
+Version: 0.0.8
 Summary: lib for OpenWeatherMap for Home Assistant
 License: MIT
 Keywords: homeassistant,owm,openweathermap
 Author: Evgeny
 Author-email: iam@freekode.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

