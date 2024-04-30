# Comparing `tmp/mqttlibpy-1.4.5.tar.gz` & `tmp/mqttlibpy-1.4.6.tar.gz`

## Comparing `mqttlibpy-1.4.5.tar` & `mqttlibpy-1.4.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/requirements.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/upload.sh
--rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/src/MqttLibPy/__init__.py
--rwxr-xr-x   0        0        0    10315 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/src/MqttLibPy/client.py
--rwxr-xr-x   0        0        0     6346 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/src/MqttLibPy/serializer.py
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/test/__init__.py
--rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/test/test_serialize.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/.gitignore
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/LICENSE
--rwxr-xr-x   0        0        0     1695 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/README.md
--rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 mqttlibpy-1.4.5/PKG-INFO
+-rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/main.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/requirements.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/upload.sh
+-rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/src/MqttLibPy/__init__.py
+-rwxr-xr-x   0        0        0    10519 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/src/MqttLibPy/client.py
+-rwxr-xr-x   0        0        0     6346 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/src/MqttLibPy/serializer.py
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/test/__init__.py
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/test/test_serialize.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/.gitignore
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/LICENSE
+-rwxr-xr-x   0        0        0     1695 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/README.md
+-rwxr-xr-x   0        0        0      686 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 mqttlibpy-1.4.6/PKG-INFO
```

### Comparing `mqttlibpy-1.4.5/src/MqttLibPy/client.py` & `mqttlibpy-1.4.6/src/MqttLibPy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,26 +91,30 @@
             metadata = {}
         with open(filepath, "rb") as f:
             file_name = f.name.split("/")[-1]
             file_bytes = f.read()
         print(f"Sending {file_name} of length {len(file_bytes)}")
         self.send_bytes(file_bytes, route, file_name, metadata, secure=secure)
 
-    def register_route(self, route, callback):
-        topic = f'{self.prefix}{route}{self.suffix}'
+    def register_route(self, route, callback, pure_route=False):
+        if not pure_route:
+            topic = f'{self.prefix}{route}{self.suffix}'
+        else:
+            topic = route
+
         self.routes.append(topic)
         print(f"Listening to topic: {topic}")
         self.client.message_callback_add(topic, callback)
 
     def listen(self):
         print(f"Connecting to {self.hostname}:{self.port}")
         self.client.connect(self.hostname, self.port)
         self.client.loop_forever()
 
-    def endpoint(self, route: str, force_json=False, is_file=False, secure=False, endpoint_encryption_callback=None):
+    def endpoint(self, route: str, force_json=False, is_file=False, secure=False, endpoint_encryption_callback=None, pure_route=False):
         """
         :param route: part of the route to listen to, the final route will be of the form {prefix}{route}{suffix}
         :param force_json: The message payload is in json format, and will be passed to the callback as a dict
         :param is_file: Indicates if the type of payload is a bytes object
         :param secure: Whether to decrypt payloads with the provided key or not
         :param endpoint_encryption_callback: Custom encryption callback for this specific endpoint
         :return:
@@ -198,20 +202,20 @@
                         }
                 except Exception as e:
                     self.logger.error(f"Error in metadata endpoint {route} {e}")
                     tb = traceback.format_exc()
                     self.logger.error(tb)
 
             if force_json:
-                self.register_route(route, wrapper_json)
+                self.register_route(route, wrapper_json, pure_route=pure_route)
             elif is_file:
-                self.register_route(route, wrapper_files_metadata)
-                self.register_route(f"{route}/file", wrapper_files)
+                self.register_route(route, wrapper_files_metadata, pure_route=pure_route)
+                self.register_route(f"{route}/file", wrapper_files, pure_route=pure_route)
             else:
-                self.register_route(route, func)
+                self.register_route(route, func, pure_route=pure_route)
 
             def inner(*args, **kwargs):
                 pass
 
             return inner
 
         return decorator
```

### Comparing `mqttlibpy-1.4.5/src/MqttLibPy/serializer.py` & `mqttlibpy-1.4.6/src/MqttLibPy/serializer.py`

 * *Files identical despite different names*

### Comparing `mqttlibpy-1.4.5/test/test_serialize.py` & `mqttlibpy-1.4.6/test/test_serialize.py`

 * *Files identical despite different names*

### Comparing `mqttlibpy-1.4.5/LICENSE` & `mqttlibpy-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttlibpy-1.4.5/README.md` & `mqttlibpy-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `mqttlibpy-1.4.5/pyproject.toml` & `mqttlibpy-1.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MqttLibPy"
-version = "1.4.5"
+version = "1.4.6"
 authors = [
   { name="juan pablo allende - xmarts", email="juan.allende@xmarts.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -20,8 +20,8 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/xmarts/mqtt-common"
-"Bug Tracker" = "https://github.com/xmarts/mqtt-common/issues"
+"Bug Tracker" = "https://github.com/xmarts/mqtt-common/issues"
```

### Comparing `mqttlibpy-1.4.5/PKG-INFO` & `mqttlibpy-1.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: MqttLibPy
-Version: 1.4.5
+Version: 1.4.6
 Summary: A small example package
 Project-URL: Homepage, https://github.com/xmarts/mqtt-common
 Project-URL: Bug Tracker, https://github.com/xmarts/mqtt-common/issues
 Author-email: juan pablo allende - xmarts <juan.allende@xmarts.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

