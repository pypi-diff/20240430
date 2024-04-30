# Comparing `tmp/hacktegic-0.1.8.tar.gz` & `tmp/hacktegic-0.1.9.tar.gz`

## Comparing `hacktegic-0.1.8.tar` & `hacktegic-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hacktegic-0.1.8/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/__main__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/base_command.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/config.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/credentials.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/parser.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/create.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/delete.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/describe.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/list.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/update.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/auth/login.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/auth/logout.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/auth/register.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/config/get.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/config/set.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/projects/create.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/projects/delete.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/projects/describe.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/projects/list.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/_internal/commands/projects/update.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/cloud/api_clients/assets_cidr.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/cloud/api_clients/projects.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/cloud/resources/assets_cidr.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 hacktegic-0.1.8/hacktegic/cloud/resources/projects.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 hacktegic-0.1.8/.gitignore
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hacktegic-0.1.8/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hacktegic-0.1.8/README.md
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 hacktegic-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hacktegic-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hacktegic-0.1.9/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/__main__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/base_command.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/config.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/credentials.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/parser.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/create.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/delete.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/describe.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/list.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/update.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/auth/login.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/auth/logout.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/auth/register.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/config/get.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/config/set.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/create.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/delete.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/describe.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/list.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/update.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/cloud/api_clients/assets_cidr.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/cloud/api_clients/projects.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/cloud/resources/assets_cidr.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/cloud/resources/projects.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 hacktegic-0.1.9/.gitignore
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hacktegic-0.1.9/LICENSE
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hacktegic-0.1.9/README.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 hacktegic-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hacktegic-0.1.9/PKG-INFO
```

### Comparing `hacktegic-0.1.8/hacktegic/__main__.py` & `hacktegic-0.1.9/hacktegic/__main__.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/config.py` & `hacktegic-0.1.9/hacktegic/_internal/config.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/credentials.py` & `hacktegic-0.1.9/hacktegic/_internal/credentials.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/parser.py` & `hacktegic-0.1.9/hacktegic/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/create.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/create.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/delete.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/delete.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/describe.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/describe.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/list.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/list.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/assets/cidr/update.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/update.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/auth/login.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/auth/login.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/auth/logout.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/auth/logout.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/auth/register.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/auth/register.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,23 +26,15 @@
             if await creds.authenticated():
                 text = Text("You seem to already have an account.")
                 text.stylize("bold green")
                 console.print(text)
                 console.print("If you want to register again, log out first using using 'hacktegic auth logout'.")
 
             else:
-                webbrowser.open("https://cloud.hacktegic.com/register")
+                webbrowser.open(register_url)
                 console.print("Use the web browser to register.")
-                console.print("If it did not open for you, navigate to https://cloud.hacktegic.com/register .")
-                console.print("You seem to already have an account.")
-                console.print(
-                    "If you want to register again, log out first using using 'hacktegic auth logout'."
-                )
+                console.print(f"If it did not open for you navigate to {register_url} .")
                 return
-
-            webbrowser.open(register_url)
-            console.print("Use the web browser to register.")
-            console.print(f"If it did not open for you, navigate to {register_url} .")
         except:
             text = Text("Something went wrong!")
             text.stylize("bold red")
             console.print(text)
```

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/config/get.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/config/get.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/config/set.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/config/set.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/projects/create.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/projects/create.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/projects/delete.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/projects/delete.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/projects/describe.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/projects/describe.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/projects/list.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/projects/list.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/_internal/commands/projects/update.py` & `hacktegic-0.1.9/hacktegic/_internal/commands/projects/update.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/cloud/api_clients/assets_cidr.py` & `hacktegic-0.1.9/hacktegic/cloud/api_clients/assets_cidr.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/hacktegic/cloud/api_clients/projects.py` & `hacktegic-0.1.9/hacktegic/cloud/api_clients/projects.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.8/pyproject.toml` & `hacktegic-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "hacktegic"
 #dynamic = ["version"]
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     { name = "Artiom Mocrenco", email = "artiomm@hacktegic.com" },
 ]
 description = "Hacktegic CLI"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
@@ -16,15 +16,15 @@
     "Topic :: Security",
 ]
 
 dependencies = [
     "aiohttp~=3.9.0b1",
     "rich>=13.6,<13.8",
     "requests~=2.31.0",
-    "platformdirs>=3.11,<4.1",
+    "platformdirs>=3.11,<4.2",
     "aiofiles~=23.2.1",
     "tomlkit~=0.12.2",
     "pydantic~=2.5.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hacktegic/cli"
@@ -43,8 +43,11 @@
 #raw-options = { root = "./hacktegic/" }
 
 [build-system]
 requires = [
     "hatchling",
     #    "hatch-vcs"
 ]
-build-backend = "hatchling.build"
+build-backend = "hatchling.build"
+
+[tool.hatch.build.targets.wheel]
+packages = ["hacktegic"]
```

### Comparing `hacktegic-0.1.8/PKG-INFO` & `hacktegic-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hacktegic
-Version: 0.1.8
+Version: 0.1.9
 Summary: Hacktegic CLI
 Project-URL: Homepage, https://github.com/hacktegic/cli
 Project-URL: Bug Tracker, https://github.com/hacktegic/cli/issues
 Author-email: Artiom Mocrenco <artiomm@hacktegic.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Requires-Python: >=3.12
 Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: aiohttp~=3.9.0b1
-Requires-Dist: platformdirs<4.1,>=3.11
+Requires-Dist: platformdirs<4.2,>=3.11
 Requires-Dist: pydantic~=2.5.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rich<13.8,>=13.6
 Requires-Dist: tomlkit~=0.12.2
 Description-Content-Type: text/markdown
 
 # Hacktegic CLI
```

