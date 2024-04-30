# Comparing `tmp/ThermiaOnlineAPI-4.1.1.tar.gz` & `tmp/thermiaonlineapi-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ThermiaOnlineAPI-4.1.1.tar", last modified: Mon Jan  8 16:42:29 2024, max compression
+gzip compressed data, was "thermiaonlineapi-4.2.0.tar", last modified: Tue Apr 30 21:08:31 2024, max compression
```

## Comparing `ThermiaOnlineAPI-4.1.1.tar` & `thermiaonlineapi-4.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:42:29.273846 ThermiaOnlineAPI-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-01-08 16:42:29.273846 ThermiaOnlineAPI-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:42:29.269846 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:42:29.273846 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/api/
--rw-r--r--   0 runner    (1001) docker     (127)    23704 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/api/ThermiaAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:42:29.273846 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/exceptions/AuthenticationException.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/exceptions/NetworkException.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:42:29.273846 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/model/
--rw-r--r--   0 runner    (1001) docker     (127)    33557 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/model/HeatPump.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:42:29.273846 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 16:42:29.273846 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-01-08 16:42:29.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-08 16:42:29.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 16:42:29.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-08 16:42:29.000000 ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-08 16:42:29.273846 ThermiaOnlineAPI-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-01-08 16:42:21.000000 ThermiaOnlineAPI-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:08:31.246516 thermiaonlineapi-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-30 21:08:31.246516 thermiaonlineapi-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:08:31.242516 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:08:31.242516 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/api/ThermiaAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:08:31.242516 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/exceptions/AuthenticationException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/exceptions/NetworkException.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:08:31.242516 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    33557 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/model/HeatPump.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:08:31.242516 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:08:31.246516 thermiaonlineapi-4.2.0/ThermiaOnlineAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-30 21:08:31.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-30 21:08:31.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:08:31.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 21:08:31.000000 thermiaonlineapi-4.2.0/ThermiaOnlineAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 21:08:31.246516 thermiaonlineapi-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-30 21:08:23.000000 thermiaonlineapi-4.2.0/setup.py
```

### Comparing `ThermiaOnlineAPI-4.1.1/LICENSE` & `thermiaonlineapi-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ThermiaOnlineAPI-4.1.1/PKG-INFO` & `thermiaonlineapi-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ThermiaOnlineAPI
-Version: 4.1.1
+Version: 4.2.0
 Summary: A Python API for Thermia heat pumps using https://online.thermia.se
 Home-page: https://github.com/klejejs/python-thermia-online-api
 Download-URL: https://github.com/klejejs/python-thermia-online-api/releases
 Author: Krisjanis Lejejs
 Author-email: krisjanis.lejejs@gmail.com
 License: GPL-3.0
 Keywords: Thermia,Online
```

### Comparing `ThermiaOnlineAPI-4.1.1/README.md` & `thermiaonlineapi-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/__init__.py` & `thermiaonlineapi-4.2.0/ThermiaOnlineAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/api/ThermiaAPI.py` & `thermiaonlineapi-4.2.0/ThermiaOnlineAPI/api/ThermiaAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,22 +577,18 @@
                 AZURE_AUTH_AUTHORIZE_URL, data=request_auth__data
             )
 
             state_code = ""
             csrf_token = ""
 
             if request_auth.status_code == 200:
-                settings_string = [
-                    i
-                    for i in request_auth.text.splitlines()
-                    if i.startswith("var SETTINGS = ")
-                ]
+                settings_string = request_auth.text.split("var SETTINGS = ")
+                settings_string = settings_string[1].split("};")[0] + "}"
                 if len(settings_string) > 0:
-                    settings = json.loads(settings_string[0][15:-1])
-
+                    settings = json.loads(settings_string)
                     state_code = str(settings["transId"]).split("=")[1]
                     csrf_token = settings["csrf"]
             else:
                 _LOGGER.error(
                     "Error fetching authorization API. Status: "
                     + str(request_auth.status_code)
                     + ", Response: "
```

### Comparing `ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/const.py` & `thermiaonlineapi-4.2.0/ThermiaOnlineAPI/const.py`

 * *Files identical despite different names*

### Comparing `ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/model/HeatPump.py` & `thermiaonlineapi-4.2.0/ThermiaOnlineAPI/model/HeatPump.py`

 * *Files identical despite different names*

### Comparing `ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI/utils/utils.py` & `thermiaonlineapi-4.2.0/ThermiaOnlineAPI/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI.egg-info/PKG-INFO` & `thermiaonlineapi-4.2.0/ThermiaOnlineAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ThermiaOnlineAPI
-Version: 4.1.1
+Version: 4.2.0
 Summary: A Python API for Thermia heat pumps using https://online.thermia.se
 Home-page: https://github.com/klejejs/python-thermia-online-api
 Download-URL: https://github.com/klejejs/python-thermia-online-api/releases
 Author: Krisjanis Lejejs
 Author-email: krisjanis.lejejs@gmail.com
 License: GPL-3.0
 Keywords: Thermia,Online
```

### Comparing `ThermiaOnlineAPI-4.1.1/ThermiaOnlineAPI.egg-info/SOURCES.txt` & `thermiaonlineapi-4.2.0/ThermiaOnlineAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ThermiaOnlineAPI-4.1.1/setup.py` & `thermiaonlineapi-4.2.0/setup.py`

 * *Files identical despite different names*

