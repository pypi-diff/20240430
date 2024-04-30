# Comparing `tmp/gemini_ai_app_downloader-1.1.tar.gz` & `tmp/gemini_ai_app_downloader-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_ai_app_downloader-1.1.tar", last modified: Sat Apr 27 05:22:29 2024, max compression
+gzip compressed data, was "gemini_ai_app_downloader-1.2.tar", last modified: Tue Apr 30 11:20:59 2024, max compression
```

## Comparing `gemini_ai_app_downloader-1.1.tar` & `gemini_ai_app_downloader-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-04-27 05:22:29.846235 gemini_ai_app_downloader-1.1/
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     1053 2024-03-24 06:48:54.000000 gemini_ai_app_downloader-1.1/LICENSE
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     3312 2024-04-27 05:22:29.846153 gemini_ai_app_downloader-1.1/PKG-INFO
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     2639 2024-04-27 05:06:59.000000 gemini_ai_app_downloader-1.1/README.md
-drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-04-27 05:22:29.845859 gemini_ai_app_downloader-1.1/gemini_ai_app_downloader.egg-info/
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     3312 2024-04-27 05:22:29.000000 gemini_ai_app_downloader-1.1/gemini_ai_app_downloader.egg-info/PKG-INFO
--rw-r--r--   0 dominictjiptono   (501) staff       (20)      279 2024-04-27 05:22:29.000000 gemini_ai_app_downloader-1.1/gemini_ai_app_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)        1 2024-04-27 05:22:29.000000 gemini_ai_app_downloader-1.1/gemini_ai_app_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       35 2024-04-27 05:22:29.000000 gemini_ai_app_downloader-1.1/gemini_ai_app_downloader.egg-info/entry_points.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       25 2024-04-27 05:22:29.000000 gemini_ai_app_downloader-1.1/gemini_ai_app_downloader.egg-info/top_level.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       79 2024-04-27 05:22:29.846545 gemini_ai_app_downloader-1.1/setup.cfg
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     1104 2024-04-27 05:06:15.000000 gemini_ai_app_downloader-1.1/setup.py
+drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-04-30 11:20:59.310937 gemini_ai_app_downloader-1.2/
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     1053 2024-03-24 06:48:54.000000 gemini_ai_app_downloader-1.2/LICENSE
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     3410 2024-04-30 11:20:59.310849 gemini_ai_app_downloader-1.2/PKG-INFO
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     2737 2024-04-30 11:19:29.000000 gemini_ai_app_downloader-1.2/README.md
+drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-04-30 11:20:59.310541 gemini_ai_app_downloader-1.2/gemini_ai_app_downloader.egg-info/
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     3410 2024-04-30 11:20:59.000000 gemini_ai_app_downloader-1.2/gemini_ai_app_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)      279 2024-04-30 11:20:59.000000 gemini_ai_app_downloader-1.2/gemini_ai_app_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)        1 2024-04-30 11:20:59.000000 gemini_ai_app_downloader-1.2/gemini_ai_app_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       35 2024-04-30 11:20:59.000000 gemini_ai_app_downloader-1.2/gemini_ai_app_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       25 2024-04-30 11:20:59.000000 gemini_ai_app_downloader-1.2/gemini_ai_app_downloader.egg-info/top_level.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       79 2024-04-30 11:20:59.311284 gemini_ai_app_downloader-1.2/setup.cfg
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     1104 2024-04-30 11:20:18.000000 gemini_ai_app_downloader-1.2/setup.py
```

### Comparing `gemini_ai_app_downloader-1.1/LICENSE` & `gemini_ai_app_downloader-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_ai_app_downloader-1.1/PKG-INFO` & `gemini_ai_app_downloader-1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini_ai_app_downloader
-Version: 1.1
+Version: 1.2
 Summary: This package contains implementation of the downloader of applications with Google Gemini AI integrated into them.
 Home-page: https://github.com/SoftwareApkDev/gemini_ai_app_downloader
 Author: SoftwareApkDev
 Author-email: softwareapkdev2022@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,17 +16,18 @@
 
 # gemini_ai_app_downloader
 
 An app which can be used to easily download any apps with Google Gemini AI integrated into them.
 
 # Downloadable Apps
 
-| Name               | Author                                              | Latest Version |
-|--------------------|-----------------------------------------------------|----------------|
-| Gemini Simple Game | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Name                | Author                                              | Latest Version |
+|---------------------|-----------------------------------------------------|----------------|
+| Gemini Simple Game  | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Gemini TXT Analyser | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
 
 # How to Add Your Downloadable App?
 
 1. Enter the name of your app on a new line in the file apps.txt.
 2. Ensure that the name of the app you entered is already available as a PyPi project, with the format containing 
 at least like below, where [your_app_name] is the name of your app and [entry_point_name] is the name
 of the entry point of your app.
```

### Comparing `gemini_ai_app_downloader-1.1/README.md` & `gemini_ai_app_downloader-1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # gemini_ai_app_downloader
 
 An app which can be used to easily download any apps with Google Gemini AI integrated into them.
 
 # Downloadable Apps
 
-| Name               | Author                                              | Latest Version |
-|--------------------|-----------------------------------------------------|----------------|
-| Gemini Simple Game | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Name                | Author                                              | Latest Version |
+|---------------------|-----------------------------------------------------|----------------|
+| Gemini Simple Game  | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Gemini TXT Analyser | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
 
 # How to Add Your Downloadable App?
 
 1. Enter the name of your app on a new line in the file apps.txt.
 2. Ensure that the name of the app you entered is already available as a PyPi project, with the format containing 
 at least like below, where [your_app_name] is the name of your app and [entry_point_name] is the name
 of the entry point of your app.
```

### Comparing `gemini_ai_app_downloader-1.1/gemini_ai_app_downloader.egg-info/PKG-INFO` & `gemini_ai_app_downloader-1.2/gemini_ai_app_downloader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini_ai_app_downloader
-Version: 1.1
+Version: 1.2
 Summary: This package contains implementation of the downloader of applications with Google Gemini AI integrated into them.
 Home-page: https://github.com/SoftwareApkDev/gemini_ai_app_downloader
 Author: SoftwareApkDev
 Author-email: softwareapkdev2022@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,17 +16,18 @@
 
 # gemini_ai_app_downloader
 
 An app which can be used to easily download any apps with Google Gemini AI integrated into them.
 
 # Downloadable Apps
 
-| Name               | Author                                              | Latest Version |
-|--------------------|-----------------------------------------------------|----------------|
-| Gemini Simple Game | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Name                | Author                                              | Latest Version |
+|---------------------|-----------------------------------------------------|----------------|
+| Gemini Simple Game  | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Gemini TXT Analyser | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
 
 # How to Add Your Downloadable App?
 
 1. Enter the name of your app on a new line in the file apps.txt.
 2. Ensure that the name of the app you entered is already available as a PyPi project, with the format containing 
 at least like below, where [your_app_name] is the name of your app and [entry_point_name] is the name
 of the entry point of your app.
```

### Comparing `gemini_ai_app_downloader-1.1/setup.py` & `gemini_ai_app_downloader-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
         return long_description
 
 
 setup(
     name='gemini_ai_app_downloader',
-    version='1.1',
+    version='1.2',
     packages=['gemini_ai_app_downloader'],
     url='https://github.com/SoftwareApkDev/gemini_ai_app_downloader',
     license='MIT',
     author='SoftwareApkDev',
     author_email='softwareapkdev2022@gmail.com',
     description='This package contains implementation of the downloader of applications with '
                 'Google Gemini AI integrated into them.',
```

