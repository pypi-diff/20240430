# Comparing `tmp/qaml-0.0.8.tar.gz` & `tmp/qaml-0.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.8.tar", last modified: Fri Apr 26 14:52:42 2024, max compression
+gzip compressed data, was "qaml-0.0.8.1.tar", last modified: Tue Apr 30 19:51:43 2024, max compression
```

## Comparing `qaml-0.0.8.tar` & `qaml-0.0.8.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-26 14:52:42.457144 qaml-0.0.8/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.8/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1561 2024-04-26 14:52:42.457001 qaml-0.0.8/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.8/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-26 14:52:38.000000 qaml-0.0.8/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-26 14:52:42.456153 qaml-0.0.8/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.8/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.8/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    13893 2024-04-26 03:13:02.000000 qaml-0.0.8/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-26 14:52:42.456866 qaml-0.0.8/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1561 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-26 14:52:42.000000 qaml-0.0.8/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-26 14:52:42.457189 qaml-0.0.8/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-30 19:51:43.733349 qaml-0.0.8.1/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.8.1/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-30 19:51:43.733204 qaml-0.0.8.1/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.8.1/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      770 2024-04-30 19:51:31.000000 qaml-0.0.8.1/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-30 19:51:43.732309 qaml-0.0.8.1/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.8.1/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.8.1/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      981 2024-04-29 18:11:49.000000 qaml-0.0.8.1/qaml/cli_agent.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    16669 2024-04-30 19:46:20.000000 qaml-0.0.8.1/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-30 19:51:43.733063 qaml-0.0.8.1/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      269 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       77 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-30 19:51:43.733378 qaml-0.0.8.1/setup.cfg
```

### Comparing `qaml-0.0.8/LICENSE` & `qaml-0.0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.8/PKG-INFO` & `qaml-0.0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.8/README.md` & `qaml-0.0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.8/pyproject.toml` & `qaml-0.0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.8"
+version = "0.0.8.1"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,11 +23,12 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/qaml-ai/qaml-python"
 
 [project.scripts]
 qaml = "qaml.__main__:main"
+qaml-agent = "qaml.cli_agent:main"
 
 [tool.setuptools.package-data]
 "src" = ["*.txt", "*.dat"]
```

### Comparing `qaml-0.0.8/qaml/__main__.py` & `qaml-0.0.8.1/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.8/qaml/client.py` & `qaml-0.0.8.1/qaml/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 import base64
 import subprocess
 import json
 from PIL import Image
 from io import BytesIO
 import requests
 import os
+import xml.etree.ElementTree as ET
 
 class QAMLExecException(Exception):
     pass
 
 class BaseClient:
     def __init__(self, api_key, api_base_url="https://api.camelqa.com"):
         self.api_key = api_key or os.environ.get("QAML_API_KEY")
         self.api_base_url = os.environ.get("QAML_API_BASE_URL", api_base_url)
         self.driver = None
         self.platform = None
         self.screen_size = None
+        self.use_accessibility_elements = False
         self.req_session = requests.Session()
         self.req_session.headers.update({"Authorization": f"Bearer {api_key}"})
         self.system_prompt = None
         self.available_functions = {
             "tap": self.tap_coordinates,
             "drag": self.drag,
             "swipe": self.swipe,
@@ -72,57 +74,88 @@
         return screenshot
 
     def _execute_function(self, function_name, **kwargs):
         function = self.available_functions.get(function_name)
         if function:
             function(**kwargs)
 
+    def get_accessibility_elements(self, use_accessibility_elements=False):
+        if (not self.use_accessibility_elements and not use_accessibility_elements):
+            return []
+        appium_page_source = self.driver.page_source
+        root = ET.fromstring(appium_page_source)
+        accessibility_elements = root.findall(".//*[@accessible='true']")
+        accessibility_elements = [element for element in accessibility_elements if element.tag != "XCUIElementTypeStaticText" and element.tag != "android.widget.TextView" and element.tag != "XCUIElementTypeKey"]
+        accessibility_elements = [{"left": int(element.attrib["x"]), "top": int(element.attrib["y"]), "width": int(element.attrib["width"]), "height": int(element.attrib["height"]), "type": element.attrib["type"], "label": element.attrib.get("label", "")} for element in accessibility_elements]
+        # remove elements with no label
+        accessibility_elements = [element for element in accessibility_elements if element["label"] and element["label"].strip()]
+        return accessibility_elements
+
     def execute(self, script):
         screenshot = self.get_screenshot()
-        """
-        now = time.time()
-        appium_page_source = self.driver.page_source
-        print(f"Page source: {appium_page_source}", time.time() - now)
-        """
-        payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.system_prompt}
+        accessibility_elements = self.get_accessibility_elements()
+        payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.system_prompt, "accessibility_elements": accessibility_elements}
         response = self.req_session.post(f"{self.api_base_url}/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
         print(f"Action: {script} - Response: {response.text}")
         try:
             actions = response.json()
             for action in actions:
                 self._execute_function(action["name"], **json.loads(action["arguments"]))
+                time.sleep(0.5)
         except Exception as e:
             print(e)
             pass
 
     def assert_condition(self, script):
         screenshot = self.get_screenshot()
         payload = {"assertion": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.system_prompt}
         response = self.req_session.post(f"{self.api_base_url}/v1/assert", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
         print(f"Action: {script} - Response: {response.text}")
         assertion = response.json()[0]
         args = json.loads(assertion["arguments"])
-        if not args["result"]:
+        if args.get("result") == False:
             raise QAMLExecException(f"Assertion failed: {script}. Reason: {args['reason']}")
         return response.json()
 
-    def agent(self, task):
+    def task(self, task, max_steps=10):
         progress = []
+        iterations = 0
+        yield f"Task: {task}"
         while True:
+            if iterations >= max_steps:
+                raise QAMLExecException(f"Task execution took too many steps. Max steps: {max_steps}")
+            iterations += 1
+            time.sleep(0.5)
             screenshot = self.get_screenshot()
-            payload = {"task": task, "progress": progress, "platform": self.platform, "screenshot": screenshot}
-            response = self.req_session.post(f"{self.api_base_url}/v1/agent", json=payload)
+            accessibility_elements = self.get_accessibility_elements()
+            payload = {"task": task, "progress": progress, "platform": self.platform, "screenshot": screenshot, "extra_context": self.system_prompt, "screen_size": self.screen_size, "accessibility_elements": accessibility_elements}
+            response = self.req_session.post(f"{self.api_base_url}/v1/execute-task", json=payload)
             response_json = response.json()
-            status = response_json["status"]
-            progress += response_json["progress"]
-            actions = response_json["actions"]
-            if status != "in_progress":
-                return status, progress
-            for action in actions:
-                self.execute(action)
+            function_called = False
+            completed = False
+            for function in response_json:
+                args = json.loads(function["arguments"])
+                if function["name"] == "update_progress":
+                    yield f"Progress: {args['progress']}"
+                    progress.append(args["progress"])
+                    continue
+                if function["name"] == "task_completed":
+                    if args["result"] == "success":
+                        completed = True
+                    else:
+                        raise QAMLExecException(f"Task execution failed. Progress: {progress}")
+                function_called = True
+                self._execute_function(function["name"], **args)
+                yield f"{function['name']}({args})"
+                progress.append(f'{function["name"]}({args})')
+            if completed:
+                break
+            if not function_called:
+                pass
+                #raise QAMLExecException("Task execution failed. No function called.")
 
 class AndroidClient(BaseClient):
     def __init__(self, api_key, driver=None):
         super().__init__(api_key)
         self.platform = "Android"
         if driver:
             self.driver = driver
@@ -174,23 +207,22 @@
         self.driver.execute_script("mobile: swipeGesture", {"left": left, "top": top, "width": width, "height": height, "direction": direction, "percent": 1.0})
 
     def scroll(self, direction):
         direction_map = {"up": "down", "down": "up", "left": "right", "right": "left"}
         self.swipe(direction_map[direction])
 
     def type_text(self, text):
-        subprocess.run(["adb", "shell", "input", "text", f"'{text}'"])
+        self.driver.execute_script("mobile: shell", {"command": f"input text '{text}'"})
 
 class IOSClient(BaseClient):
-    def __init__(self, api_key, driver=None, use_mjpeg=True, use_hid_typing=False):
+    def __init__(self, api_key, driver=None, use_mjpeg=True):
         super().__init__(api_key)
         self.available_functions["switch_to_app"] = self.switch_to_app
         self.platform = "iOS"
         self.use_mjpeg = use_mjpeg
-        self.use_hid_typing = use_hid_typing
         if driver:
             self.driver = driver
         else:
             def get_ios_udid():
                 system_profiler_output = subprocess.run(["system_profiler", "SPUSBDataType"], capture_output=True, text=True).stdout
                 serial_numbers = re.findall(r'(iPhone|iPad).*?Serial Number: *([^\n]+)', system_profiler_output, re.DOTALL)
 
@@ -299,38 +331,48 @@
 
             self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": usage, "durationSeconds": 0.005})  # Key down
             self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0x00, "durationSeconds": 0.005})  # Key up
 
     def switch_to_app(self, bundle_id):
         self.driver.activate_app(bundle_id)
 
-def Client(api_key, driver=None, use_mjpeg=True, use_hid_typing=False):
+def Client(api_key, driver=None, use_mjpeg=True, use_hid_typing=False, use_accessibility_elements=False):
 
     def get_connected_android_devices():
         try:
             result = subprocess.run(["adb", "devices"], capture_output=True, text=True)
             devices = result.stdout.splitlines()[1:]  # Skip the first line, which is a header
             connected_devices = [line.split('\t')[0] for line in devices if "device" in line]
             return connected_devices
         except:
             return []
 
     if driver is not None:
         platform_name = driver.capabilities.get("platformName").lower()
         if platform_name == 'android':
             print("Using the provided Appium driver for Android.")
-            return AndroidClient(api_key, driver=driver)
+            client = AndroidClient(api_key, driver=driver)
+            client.use_accessibility_elements = use_accessibility_elements
+            return client
         elif platform_name == 'ios':
             print("Using the provided Appium driver for iOS.")
-            return IOSClient(api_key, driver=driver, use_hid_typing=use_hid_typing)
+            client = IOSClient(api_key, driver=driver)
+            client.use_accessibility_elements = use_accessibility_elements
+            client.use_hid_typing = use_hid_typing
+            return client
         else:
             raise Exception("Unsupported platform specified in the provided driver's capabilities.")
 
     android_devices = get_connected_android_devices()
     if android_devices:
-        return AndroidClient(api_key)
+        client = AndroidClient(api_key)
+        client.use_accessibility_elements = use_accessibility_elements
+        return client
 
     try:
-        return IOSClient(api_key, use_mjpeg=use_mjpeg, use_hid_typing=use_hid_typing)
+        client = IOSClient(api_key, use_mjpeg=use_mjpeg)
+        client.use_accessibility_elements = use_accessibility_elements
+        client.use_hid_typing = use_hid_typing
+        return client
     except:
         raise Exception("No connected devices found or driver provided.")
```

### Comparing `qaml-0.0.8/qaml.egg-info/PKG-INFO` & `qaml-0.0.8.1/qaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

