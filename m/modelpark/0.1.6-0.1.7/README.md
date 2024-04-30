# Comparing `tmp/modelpark-0.1.6.tar.gz` & `tmp/modelpark-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelpark-0.1.6.tar", last modified: Sun Apr 28 20:19:51 2024, max compression
+gzip compressed data, was "modelpark-0.1.7.tar", last modified: Tue Apr 30 16:04:18 2024, max compression
```

## Comparing `modelpark-0.1.6.tar` & `modelpark-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 20:19:51.724187 modelpark-0.1.6/
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.6/LICENSE
--rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.6/MANIFEST.in
--rw-r--r--   0 vkocaman   (501) staff       (20)     3425 2024-04-28 20:19:51.723959 modelpark-0.1.6/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)     2524 2024-04-28 20:18:29.000000 modelpark-0.1.6/README.md
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 20:19:51.722986 modelpark-0.1.6/modelpark/
--rw-rw-r--   0 vkocaman   (501) staff       (20)      345 2024-04-28 20:19:47.000000 modelpark-0.1.6/modelpark/__init__.py
--rw-rw-r--   0 vkocaman   (501) staff       (20)     3585 2024-04-28 20:09:30.000000 modelpark-0.1.6/modelpark/modelpark.py
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-28 20:19:51.723748 modelpark-0.1.6/modelpark.egg-info/
--rw-r--r--   0 vkocaman   (501) staff       (20)     3425 2024-04-28 20:19:51.000000 modelpark-0.1.6/modelpark.egg-info/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-28 20:19:51.000000 modelpark-0.1.6/modelpark.egg-info/SOURCES.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-28 20:19:51.000000 modelpark-0.1.6/modelpark.egg-info/dependency_links.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-28 20:19:51.000000 modelpark-0.1.6/modelpark.egg-info/requires.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-28 20:19:51.000000 modelpark-0.1.6/modelpark.egg-info/top_level.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-28 20:19:51.724234 modelpark-0.1.6/setup.cfg
--rw-r--r--   0 vkocaman   (501) staff       (20)     2964 2024-04-28 20:19:47.000000 modelpark-0.1.6/setup.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:04:18.628250 modelpark-0.1.7/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.7/LICENSE
+-rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.7/MANIFEST.in
+-rw-r--r--   0 vkocaman   (501) staff       (20)     3425 2024-04-30 16:04:18.628028 modelpark-0.1.7/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2524 2024-04-28 20:18:29.000000 modelpark-0.1.7/README.md
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:04:18.626955 modelpark-0.1.7/modelpark/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)      345 2024-04-30 15:17:46.000000 modelpark-0.1.7/modelpark/__init__.py
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     4836 2024-04-30 16:04:10.000000 modelpark-0.1.7/modelpark/modelpark.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:04:18.627798 modelpark-0.1.7/modelpark.egg-info/
+-rw-r--r--   0 vkocaman   (501) staff       (20)     3425 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/SOURCES.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/dependency_links.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/requires.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/top_level.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-30 16:04:18.628292 modelpark-0.1.7/setup.cfg
+-rw-r--r--   0 vkocaman   (501) staff       (20)     4544 2024-04-30 15:48:13.000000 modelpark-0.1.7/setup.py
```

### Comparing `modelpark-0.1.6/LICENSE` & `modelpark-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.6/PKG-INFO` & `modelpark-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.6
+Version: 0.1.7
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modelpark-0.1.6/README.md` & `modelpark-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.6/modelpark/modelpark.py` & `modelpark-0.1.7/modelpark/modelpark.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import json
 import requests
 import subprocess
 import sys
+import os
+import platform
 
 class CommandRunner:
     """Executes system commands related to ModelPark CLI operations."""
 
     @staticmethod
+    def get_executable_path():
+        """Returns the full path to the executable based on the operating system."""
+        home_dir = os.path.expanduser('~')  # Gets the home directory
+        if platform.system().lower() == 'windows':
+            return os.path.join(home_dir, 'modelpark.exe')  # Windows executable path
+        else:
+            return os.path.join(home_dir, 'modelpark')  # Unix/Mac executable path
+
+    @staticmethod
     def run_command(command):
         try:
+            executable_path = CommandRunner.get_executable_path()
+            command = f"{executable_path} {command}"
             process = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
             print(f"Started process {process.pid}")
             print (f"Command: {command}")
             if 'init' not in command:
                 stdout, stderr = process.communicate()
                 if process.returncode != 0:
                     print("Error:", stderr)
@@ -23,63 +36,79 @@
             sys.exit(1)
 
 class ModelPark:
     def __init__(self):
         pass
 
     def login(self, token=None, username=None, password=None):
-        command = "modelpark login"
+        command = "login"
         if token:
             command += f" -t {token}"
         if username:
             command += f" -u {username}"
         if password:
             command += f" -p {password}"
         CommandRunner.run_command(command)
 
     def init(self, port=None, detach=True):
-        command = "modelpark init"
+        command = "init"
         if port:
             command += f" -p {port}"
-
         if detach !=True:
             command += f" -d {str(detach).lower()}"
         print(f"Running command: {command}")  # Debug print
         output = CommandRunner.run_command(command)
         print("Initialization Output:", output)
 
     def stop(self):
-        CommandRunner.run_command("modelpark stop")
+        CommandRunner.run_command("stop")
 
     def logout(self):
-        CommandRunner.run_command("modelpark logout")
+        CommandRunner.run_command("logout")
 
     def register(self, port, name, file_path=None, access='private', password=None, framework=None):
         if framework:
-            command = f"modelpark register -p {port} -n {name} -a {access} -f {framework}"
+            command = f"register -p {port} -n {name} -a {access} -f {framework}"
         else:
-            command = f"modelpark register -p {port} -n {name} -a {access}"
+            command = f"register -p {port} -n {name} -a {access}"
         if file_path:
             command += f" {file_path}"
         if access == 'public' and password:
             command += f" -password {password}"
         CommandRunner.run_command(command)
+    
+    def register_port(self, name, port, access='private',password=None):
+        command = f"register  -n {name} -a {access} -p {port}"
+        if access == 'public' and password:
+            command += f" -password {password}"
+        CommandRunner.run_command(command)
+
+    def run_with_streamlit_and_register(self, name, file_path, access='private', password=None, port=None):
+        command = f"register {file_path} -n {name} -a {access} -f streamlit"
+        if port:
+            command += f" -p {port}"
+        if access == 'public' and password:
+            command += f" -password {password}"
+        CommandRunner.run_command(command)
 
     def kill(self, name=None, all=False):
-        command = "modelpark kill"
+        command = "kill"
         if all:
             command += " -a"
         elif name:
             command += f" -n {name}"
         CommandRunner.run_command(command)
 
     def ls(self):
-        result = CommandRunner.run_command("modelpark ls")
+        result = CommandRunner.run_command("ls")
         print(result)
 
+    def status(self):
+        result = CommandRunner.run_command("status")
+        print(result)
 
 class APIManager:
     """Manages API interactions for ModelPark."""
 
     @staticmethod
     def get_auth_token(user_credentials):
         url = "https://modelpark.app/api/auth/login"
```

### Comparing `modelpark-0.1.6/modelpark.egg-info/PKG-INFO` & `modelpark-0.1.7/modelpark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.6
+Version: 0.1.7
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
```

