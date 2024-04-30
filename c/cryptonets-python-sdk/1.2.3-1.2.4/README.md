# Comparing `tmp/cryptonets_python_sdk-1.2.3.tar.gz` & `tmp/cryptonets_python_sdk-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptonets_python_sdk-1.2.3.tar", last modified: Wed Apr 24 15:48:49 2024, max compression
+gzip compressed data, was "cryptonets_python_sdk-1.2.4.tar", last modified: Tue Apr 30 12:05:15 2024, max compression
```

## Comparing `cryptonets_python_sdk-1.2.3.tar` & `cryptonets_python_sdk-1.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.3/LICENSE
--rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.3/MANIFEST.in
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/README.md
--rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/setup.cfg
--rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/setup.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.133714 cryptonets_python_sdk-1.2.3/src/
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.133714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.133714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor_modules/
--rw-rw-r--   0 azam      (1000) azam      (1000)    19933 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor_modules/FaceModule.py
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor_modules/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/lib/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/lib/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    44485 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/nativeMethods.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/decorators.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3383 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/messages.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     4476 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/utils.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/cacheType.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    16918 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/configuration.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/loggingLevel.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/supportedPlatforms.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.133714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-24 15:48:48.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-04-24 15:48:49.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-04-24 15:48:48.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-04-24 15:48:48.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/requires.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-04-24 15:48:48.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/tests/
--rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.3/tests/test.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/tests/test_suite.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.4/LICENSE
+-rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.4/MANIFEST.in
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/README.md
+-rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/setup.cfg
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-04-30 12:01:39.000000 cryptonets_python_sdk-1.2.4/setup.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.131822 cryptonets_python_sdk-1.2.4/src/
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/factor.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/factor_modules/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    19933 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/factor_modules/FaceModule.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/factor_modules/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/handler/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/handler/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/handler/lib/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/handler/lib/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    44485 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/handler/nativeMethods.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/decorators.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3383 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/messages.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     4476 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/utils.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/settings/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/settings/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/settings/cacheType.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    17214 2024-04-30 12:01:39.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/settings/configuration.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/settings/loggingLevel.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/settings/supportedPlatforms.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk.egg-info/
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-30 12:05:15.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-04-30 12:05:15.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-04-30 12:05:15.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-04-30 12:05:15.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk.egg-info/requires.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-04-30 12:05:15.000000 cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-30 12:05:15.135822 cryptonets_python_sdk-1.2.4/tests/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.4/tests/test.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.4/tests/test_suite.py
```

### Comparing `cryptonets_python_sdk-1.2.3/PKG-INFO` & `cryptonets_python_sdk-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets_python_sdk
-Version: 1.2.3
+Version: 1.2.4
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.2.3/README.md` & `cryptonets_python_sdk-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/setup.py` & `cryptonets_python_sdk-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 @author: Private Identity
 """
 NAME = "cryptonets_python_sdk"
 DESCRIPTION = "Cryptonets SDK Library for Python"
 AUTHOR = "Private Identity"
 AUTHOR_EMAIL = "support@private.id"
 URL = "https://privateid.com/"
-VERSION = "1.2.3"
+VERSION = "1.2.4"
 REQUIRES = ["numpy >= 1.21.0", "pillow >= 9.1.0","boto3","tqdm","exifread"]
 
 LONG_DESCRIPTION = ""
 if os.path.exists("./README.md"):
     with open("README.md", encoding="utf-8") as fp:
         LONG_DESCRIPTION = fp.read()
 setup(
```

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/factor.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor_modules/FaceModule.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/factor_modules/FaceModule.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/nativeMethods.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/handler/nativeMethods.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/decorators.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/decorators.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/messages.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/messages.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/compareResult.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/compareResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/utils.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/helper/utils.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/configuration.py` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk/settings/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     # PREDICT_RESERVATION_CALLS = "predict"
     DOC_FRONT_RESERVATION_CALLS = "document_model"
     DOC_BACK_RESERVATION_CALLS = "document_model"
     COMPARE_RESERVATION_CALLS = "compare_files"
     FACE_RESERVATION_CALLS = "faces"
     ESTIMATE_AGE_RESERVATION_CALLS = "estimate_age"
     FACE_ISO_RESERVATION_CALLS = "face_iso"
+    THRESHOLD_HIGH_VERTICAL="threshold_high_vertical_enroll"
 
 
 class ParameterValidator:
     def __init__(self):
         self.__parameter = {}
         self.__populate_parameters()
         self.__billing_reservation_parameters = [
@@ -303,14 +304,22 @@
         self.__parameter[PARAMETERS.FACE_ISO_RESERVATION_CALLS] = self.Parameter(
             name=PARAMETERS.FACE_ISO_RESERVATION_CALLS,
             _type="NUMBER",
             min_value=0,
             max_value=100000000,
         )
 
+        self.__parameter[PARAMETERS.THRESHOLD_HIGH_VERTICAL] = self.Parameter(
+            name=PARAMETERS.THRESHOLD_HIGH_VERTICAL,
+            _type="NUMBER",
+            min_value=-100,
+            max_value=100,
+        )
+        
+
         self.__parameter[PARAMETERS.COLLECTION_NAME] = self.Parameter(
             name=PARAMETERS.COLLECTION_NAME, _type="ANY")
 
         self.__parameter[PARAMETERS.K] = self.Parameter(
             name=PARAMETERS.K,_type="NUMBER", min_value=1, max_value=100)
 
     def validate(self, key, value):
```

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/PKG-INFO` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets-python-sdk
-Version: 1.2.3
+Version: 1.2.4
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/SOURCES.txt` & `cryptonets_python_sdk-1.2.4/src/cryptonets_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/tests/test.py` & `cryptonets_python_sdk-1.2.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.3/tests/test_suite.py` & `cryptonets_python_sdk-1.2.4/tests/test_suite.py`

 * *Files identical despite different names*

