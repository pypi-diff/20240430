# Comparing `tmp/urbanairship-6.2.0.tar.gz` & `tmp/urbanairship-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urbanairship-6.2.0.tar", last modified: Mon Oct 23 16:46:51 2023, max compression
+gzip compressed data, was "urbanairship-6.3.0.tar", last modified: Tue Apr 30 18:40:03 2024, max compression
```

## Comparing `urbanairship-6.2.0.tar` & `urbanairship-6.3.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.486971 urbanairship-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-23 16:46:42.000000 urbanairship-6.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     9472 2023-10-23 16:46:42.000000 urbanairship-6.2.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-10-23 16:46:42.000000 urbanairship-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-23 16:46:42.000000 urbanairship-6.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2023-10-23 16:46:51.486971 urbanairship-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-10-23 16:46:42.000000 urbanairship-6.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-23 16:46:51.486971 urbanairship-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-23 16:46:42.000000 urbanairship-6.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.478971 urbanairship-6.2.0/urbanairship/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.482971 urbanairship-6.2.0/urbanairship/automation/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/automation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/automation/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15478 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/automation/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.482971 urbanairship-6.2.0/urbanairship/custom_events/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/custom_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/custom_events/custom_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.482971 urbanairship-6.2.0/urbanairship/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/channel_uninstall.py
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/devicelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    15856 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/email.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/named_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/open_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13986 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/static_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/subscription_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/devices/tag_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.482971 urbanairship-6.2.0/urbanairship/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/experiments/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/experiments/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/experiments/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.486971 urbanairship-6.2.0/urbanairship/push/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/push/audience.py
--rw-r--r--   0 runner    (1001) docker     (127)    17751 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/push/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    57492 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/push/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/push/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/push/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.486971 urbanairship-6.2.0/urbanairship/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/reports/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2023-10-23 16:46:42.000000 urbanairship-6.2.0/urbanairship/reports/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 16:46:51.482971 urbanairship-6.2.0/urbanairship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2023-10-23 16:46:51.000000 urbanairship-6.2.0/urbanairship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-10-23 16:46:51.000000 urbanairship-6.2.0/urbanairship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 16:46:51.000000 urbanairship-6.2.0/urbanairship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-23 16:46:51.000000 urbanairship-6.2.0/urbanairship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-23 16:46:51.000000 urbanairship-6.2.0/urbanairship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:03.000938 urbanairship-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 18:39:59.000000 urbanairship-6.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-04-30 18:39:59.000000 urbanairship-6.3.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-30 18:39:59.000000 urbanairship-6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 18:39:59.000000 urbanairship-6.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-30 18:40:03.000938 urbanairship-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-30 18:39:59.000000 urbanairship-6.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 18:40:03.000938 urbanairship-6.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-30 18:39:59.000000 urbanairship-6.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:02.992938 urbanairship-6.3.0/urbanairship/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:02.996938 urbanairship-6.3.0/urbanairship/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/automation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/automation/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/automation/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:02.996938 urbanairship-6.3.0/urbanairship/custom_events/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/custom_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/custom_events/custom_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:02.996938 urbanairship-6.3.0/urbanairship/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/channel_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/devicelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/named_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/open_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/static_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/subscription_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/devices/tag_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:02.996938 urbanairship-6.3.0/urbanairship/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/experiments/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/experiments/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/experiments/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:03.000938 urbanairship-6.3.0/urbanairship/push/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/push/audience.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/push/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57462 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/push/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/push/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/push/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:03.000938 urbanairship-6.3.0/urbanairship/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/reports/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/reports/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-30 18:39:59.000000 urbanairship-6.3.0/urbanairship/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:40:03.000938 urbanairship-6.3.0/urbanairship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-30 18:40:02.000000 urbanairship-6.3.0/urbanairship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-30 18:40:02.000000 urbanairship-6.3.0/urbanairship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:40:02.000000 urbanairship-6.3.0/urbanairship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 18:40:02.000000 urbanairship-6.3.0/urbanairship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 18:40:02.000000 urbanairship-6.3.0/urbanairship.egg-info/top_level.txt
```

### Comparing `urbanairship-6.2.0/CHANGELOG` & `urbanairship-6.3.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # urbanairship changelog
 
+## 6.3.0
+
+- Adds Support for OAuth2 Authentication
+- Adds new client classes for BasicAuth, BearerTokenAuth, and OAuth
+- Deprecates the Airship client class in favor of the new client classes
+
 ## 6.2.0
 
 - Adds Support for iOS Live Activity and Android Live Update
 - Adds new class `ConnectionFailure`
 - Adds `bypass_holdout_groups` parameter for push options
 
 ## 6.1.0
```

### Comparing `urbanairship-6.2.0/LICENSE` & `urbanairship-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urbanairship-6.2.0/PKG-INFO` & `urbanairship-6.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urbanairship
-Version: 6.2.0
+Version: 6.3.0
 Summary: Python package for using the Airship API
 Home-page: https://airship.com/
 Author: Airship Tools
 Author-email: tools@airship.com
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -90,14 +90,15 @@
     >>> push.notification = ua.notification(alert='Hello')
     >>> push.device_types = ua.device_types('web')
     >>> push.send()
 
 History
 =======
 
+* 6.3 Support for OAuth2 Authentication. Adds new clients module and class.
 * 6.0 Support for Bearer Token Authentication. Removes support for Python 2.
 * 5.0 Support for SMS and Email messages. See changelog for other updates.
 * 4.0 Support for Automation, removed Feedback
 * 3.0 Support for Open Channels, several other significant changes
 * 2.0 Support for Web Notify and more iOS 10, stopped supporting Python 2.6
 * 1.0 Support for In-App and iOS 10
 * 0.8 Support for Reports APIs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urbanairship Version: 6.2.0 Summary: Python package
+Metadata-Version: 2.1 Name: urbanairship Version: 6.3.0 Summary: Python package
 for using the Airship API Home-page: https://airship.com/ Author: Airship Tools
 Author-email: tools@airship.com License: BSD License Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries License-File: LICENSE
 License-File: AUTHORS Requires-Dist: requests>=1.2 Requires-Dist: six Requires-
@@ -36,15 +36,16 @@
 'Hello, message center user', ... '
 ************ HHeelllloo!! ************
 Goodbye.
 ') >>> push.send() Web Push to a tag ----------------- >>> import urbanairship
 as ua >>> airship = ua.Airship('application_key', 'master_secret') >>> push =
 airship.create_push() >>> push.audience = ua.tag('web_tag') >>>
 push.notification = ua.notification(alert='Hello') >>> push.device_types =
-ua.device_types('web') >>> push.send() History ======= * 6.0 Support for Bearer
+ua.device_types('web') >>> push.send() History ======= * 6.3 Support for OAuth2
+Authentication. Adds new clients module and class. * 6.0 Support for Bearer
 Token Authentication. Removes support for Python 2. * 5.0 Support for SMS and
 Email messages. See changelog for other updates. * 4.0 Support for Automation,
 removed Feedback * 3.0 Support for Open Channels, several other significant
 changes * 2.0 Support for Web Notify and more iOS 10, stopped supporting Python
 2.6 * 1.0 Support for In-App and iOS 10 * 0.8 Support for Reports APIs * 0.7
 Support for Python 3, major refactoring * 0.6 Major refactoring, support for
 push api v3 * 0.5 Added Android, Rich Push, and scheduled notifications * 0.4
```

### Comparing `urbanairship-6.2.0/README.rst` & `urbanairship-6.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     >>> push.notification = ua.notification(alert='Hello')
     >>> push.device_types = ua.device_types('web')
     >>> push.send()
 
 History
 =======
 
+* 6.3 Support for OAuth2 Authentication. Adds new clients module and class.
 * 6.0 Support for Bearer Token Authentication. Removes support for Python 2.
 * 5.0 Support for SMS and Email messages. See changelog for other updates.
 * 4.0 Support for Automation, removed Feedback
 * 3.0 Support for Open Channels, several other significant changes
 * 2.0 Support for Web Notify and more iOS 10, stopped supporting Python 2.6
 * 1.0 Support for In-App and iOS 10
 * 0.8 Support for Reports APIs
```

#### html2text {}

```diff
@@ -27,15 +27,16 @@
 'Hello, message center user', ... '
 ************ HHeelllloo!! ************
 Goodbye.
 ') >>> push.send() Web Push to a tag ----------------- >>> import urbanairship
 as ua >>> airship = ua.Airship('application_key', 'master_secret') >>> push =
 airship.create_push() >>> push.audience = ua.tag('web_tag') >>>
 push.notification = ua.notification(alert='Hello') >>> push.device_types =
-ua.device_types('web') >>> push.send() History ======= * 6.0 Support for Bearer
+ua.device_types('web') >>> push.send() History ======= * 6.3 Support for OAuth2
+Authentication. Adds new clients module and class. * 6.0 Support for Bearer
 Token Authentication. Removes support for Python 2. * 5.0 Support for SMS and
 Email messages. See changelog for other updates. * 4.0 Support for Automation,
 removed Feedback * 3.0 Support for Open Channels, several other significant
 changes * 2.0 Support for Web Notify and more iOS 10, stopped supporting Python
 2.6 * 1.0 Support for In-App and iOS 10 * 0.8 Support for Reports APIs * 0.7
 Support for Python 3, major refactoring * 0.6 Major refactoring, support for
 push api v3 * 0.5 Added Android, Rich Push, and scheduled notifications * 0.4
```

### Comparing `urbanairship-6.2.0/setup.py` & `urbanairship-6.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `urbanairship-6.2.0/urbanairship/__init__.py` & `urbanairship-6.3.0/urbanairship/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Python package for using the Airship API"""
+
 import logging
 from typing import Any, List
 
-from .core import Airship
-from .automation import Automation, Pipeline
+from .automation.core import Automation
+from .automation.pipeline import Pipeline
+from .client import BasicAuthClient, BearerTokenClient, OAuthClient
 from .common import AirshipFailure, ConnectionFailure, Unauthorized
+from .core import Airship
 from .custom_events import CustomEvent
 from .devices import (
     APIDList,
     Attribute,
-    AttributeResponse,
     AttributeList,
+    AttributeResponse,
     ChannelInfo,
     ChannelList,
     ChannelTags,
     ChannelUninstall,
     DeviceInfo,
     DeviceTokenList,
     Email,
@@ -80,22 +83,22 @@
     open_channel,
     open_platform,
     options,
     or_,
     public_notification,
     recurring_schedule,
     schedule_exclusion,
-    static_list,
-    subscription_list,
     scheduled_time,
     segment,
     sms,
     sms_id,
     sms_sender,
+    static_list,
     style,
+    subscription_list,
     tag,
     tag_group,
     text_attribute,
     wearable,
     web,
     wns,
     wns_payload,
@@ -112,14 +115,17 @@
     ResponseList,
     ResponseReportList,
     TimeInAppList,
     WebResponseReport,
 )
 
 __all__: List[Any] = [
+    BasicAuthClient,
+    BearerTokenClient,
+    OAuthClient,
     Airship,
     AirshipFailure,
     ConnectionFailure,
     Unauthorized,
     all_,
     Push,
     ScheduledPush,
```

### Comparing `urbanairship-6.2.0/urbanairship/automation/core.py` & `urbanairship-6.3.0/urbanairship/automation/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+from __future__ import annotations
+
 import json
-from typing import List, Union, Optional
+from typing import TYPE_CHECKING, List, Optional, Union
 
-from urbanairship import Airship
-from urbanairship.automation.pipeline import Pipeline
 from requests import Response
 
+from urbanairship.automation.pipeline import Pipeline
+
+if TYPE_CHECKING:
+    from urbanairship.client import BaseClient
+
 
 class Automation(object):
     """An object for getting and creating automations.
 
     :keyword airship: An urbanairship.Airship instance,
          instantiated with the key corresponding to the airship project you wish
          to use.
     """
 
-    def __init__(self, airship: Airship) -> None:
+    def __init__(self, airship: BaseClient) -> None:
         self.airship = airship
 
     def create(self, pipelines: Union[Pipeline, List[Pipeline]]) -> Response:
         """Create an automation with one or more Pipeline payloads
 
         :keyword pipelines: A single Pipeline payload or list of Pipeline payloads
         """
```

### Comparing `urbanairship-6.2.0/urbanairship/automation/pipeline.py` & `urbanairship-6.3.0/urbanairship/automation/pipeline.py`

 * *Files identical despite different names*

### Comparing `urbanairship-6.2.0/urbanairship/common.py` & `urbanairship-6.3.0/urbanairship/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import logging
 import datetime
-import six
-from typing import Dict, Optional, Any, TypeVar, Union
+import logging
+from typing import Any, Dict, Optional, Union
 
+import six
 
 logger = logging.getLogger("urbanairship")
 
 
 class Unauthorized(Exception):
     """Raised when we get a 401 from the server"""
```

### Comparing `urbanairship-6.2.0/urbanairship/core.py` & `urbanairship-6.3.0/urbanairship/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,249 +1,168 @@
 import logging
 import re
-import warnings
-from typing import Optional, Dict, Any
+import time
+import uuid
+from typing import Any, Dict, List, Optional
 
-import backoff  # type: ignore
+import backoff
+import jwt
 import requests
+from requests.exceptions import ConnectionError, Timeout
+
+from urbanairship.urls import Urls
 
 from . import __about__, common
-import urbanairship
 
 logger = logging.getLogger("urbanairship")
 
 VALID_KEY = re.compile(r"^[\w-]{22}$")
 VALID_LOCATIONS = ["eu", "us", None]
+DEFAULT_REQ_TIMEOUT_S = 60
+DEFAULT_API_VERSION = 3
+DEFAULT_ASSERTION_EXPIRY = 61
+US_OAUTH_URL = "https://oauth2.asnapius.com"
+EU_OAUTH_URL = "https://oauth2.asnapieu.com"
 
 
-class Urls(object):
-    def __init__(self, location: Optional[str] = None) -> None:
-        if not location or location.lower() == "us":
-            self.base_url = "https://go.urbanairship.com/api/"
-        elif location.lower() == "eu":
-            self.base_url = "https://go.airship.eu/api/"
-
-        self.channel_url = self.base_url + "channels/"
-        self.open_channel_url = self.channel_url + "open/"
-        self.device_token_url = self.base_url + "device_tokens/"
-        self.apid_url = self.base_url + "apids/"
-        self.push_url = self.base_url + "push/"
-        self.validate_url = self.push_url + "validate/"
-        self.schedules_url = self.base_url + "schedules/"
-        self.tags_url = self.base_url + "tags/"
-        self.segments_url = self.base_url + "segments/"
-        self.reports_url = self.base_url + "reports/"
-        self.lists_url = self.base_url + "lists/"
-        self.attributes_url = self.channel_url + "attributes/"
-        self.attributes_list_url = self.base_url + "attribute-lists/"
-        self.message_center_delete_url = self.base_url + "user/messages/"
-        self.subscription_lists_url = self.channel_url + "subscription_lists/"
-        self.templates_url = self.base_url + "templates/"
-        self.schedule_template_url = self.templates_url + "schedules/"
-        self.pipelines_url = self.base_url + "pipelines/"
-        self.named_user_url = self.base_url + "named_users/"
-        self.named_user_tag_url = self.named_user_url + "tags/"
-        self.named_user_disassociate_url = self.named_user_url + "disassociate/"
-        self.named_user_associate_url = self.named_user_url + "associate/"
-        self.named_user_uninstall_url = self.named_user_url + "uninstall/"
-        self.sms_url = self.channel_url + "sms/"
-        self.sms_opt_out_url = self.sms_url + "opt-out/"
-        self.sms_uninstall_url = self.sms_url + "uninstall/"
-        self.sms_custom_response_url = self.base_url + "sms/custom-response/"
-        self.email_url = self.channel_url + "email/"
-        self.email_tags_url = self.email_url + "tags/"
-        self.email_uninstall_url = self.email_url + "uninstall/"
-        self.create_and_send_url = self.base_url + "create-and-send/"
-        self.schedule_create_and_send_url = self.schedules_url + "create-and-send/"
-        self.experiments_url = self.base_url + "experiments/"
-        self.experiments_schedule_url = self.experiments_url + "scheduled/"
-        self.experiments_validate = self.experiments_url + "validate/"
-        self.attachment_url = self.base_url + "attachments/"
-        self.custom_events_url = self.base_url + "custom-events/"
-        self.tag_lists_url = self.base_url + "tag-lists/"
-
-    def get(self, endpoint: str) -> str:
-        url: str = getattr(self, endpoint)
-
-        if not url:
-            raise AttributeError("No url for endpoint %s" % endpoint)
-
-        return url
-
+class BaseClient:
+    """Base client class for interacting with the Airship API
+
+    :param key: [required] An airship app key (project key) which identifies the project
+    :param location: [optional] The Airship cloud site the project is located in.
+        May be 'us' or 'eu'. Defaults to 'us'.
+    :param timeout: [optional]  An integer specifying the number of seconds used
+        for a response timeout threshold
+    :param retries: [optional] An integer specifying the number of times to retry a
+        failed request. Retried requests use exponential backoff between requests.
+        Defaults to 0, no retry.
+    """
 
-class Airship(object):
     def __init__(
         self,
         key: str,
-        secret: Optional[str] = None,
-        token: Optional[str] = None,
         location: str = "us",
-        timeout: Optional[int] = None,
+        timeout: int = DEFAULT_REQ_TIMEOUT_S,
         retries: int = 0,
-    ):
-        """Main client class for interacting with the Airship API.
-
-        :param key: [required] An Airship project key used to authenticate
-        :param secret: [optional] The Airship-generated app or master secret for the
-        provided key
-        :param token: [optional] An Airship-generated bearer token for the provided key
-        :param location: [optional] The Airship cloud site your project is associated
-        with. Possible values: 'us', 'eu'. Defaults to 'us'.
-        :param: timeout: [optional] An integer specifying the number of seconds used
-        for a response timeout threshold
-        :param retries: [optional] An integer specifying the number of times to retry a
-        failed request. Retried requests use exponential backoff between requests.
-        Defaults to 0, no retry.
-        """
-        self.key: str = key
-        self.secret: Optional[str] = secret
-        self.token: Optional[str] = token
-        self.location: str = location
-        self.timeout: Optional[int] = timeout
+    ) -> None:
+        self.key = key
+        self.location = location
+        self.timeout = timeout
         self.retries = retries
         self.urls: Urls = Urls(self.location)
-
-        if all([secret, token]):
-            raise ValueError("One of token or secret must be used, not both")
-
         self.session = requests.Session()
-        if isinstance(token, str):
-            self.session.headers.update(
-                {"X-UA-Appkey": key, "Authorization": f"Bearer {self.token}"}
-            )
-        elif isinstance(secret, str):
-            self.session.auth = (key, secret)
-        else:
-            raise ValueError("Either token or secret must be included")
-
-    @property
-    def retries(self) -> int:
-        return self._retries
-
-    @retries.setter
-    def retries(self, value: int):
-        self._retries = value
-
-    @property
-    def timeout(self) -> Optional[int]:
-        return self._timeout
-
-    @timeout.setter
-    def timeout(self, value: Optional[int]) -> None:
-        if not isinstance(value, int) and value is not None:
-            raise ValueError("Timeout must be an integer")
-        self._timeout = value
 
     @property
     def key(self) -> str:
         return self._key
 
     @key.setter
     def key(self, value: str) -> None:
         if not VALID_KEY.match(value):
             raise ValueError("keys must be 22 characters")
         self._key = value
 
     @property
     def location(self) -> str:
+        """location of the cloud site project belongs to. 'us' or 'eu'"""
         return self._location
 
     @location.setter
     def location(self, value: str):
         if value not in VALID_LOCATIONS:
-            raise ValueError("location must be one of {}".format(VALID_LOCATIONS))
+            raise ValueError(f"location must be one of {format(VALID_LOCATIONS)}")
         self._location = value
 
     @property
-    def secret(self) -> Optional[str]:
-        return self._secret
+    def retries(self) -> int:
+        return self._retries
 
-    @secret.setter
-    def secret(self, value: Optional[str]) -> None:
-        if isinstance(value, str) and not VALID_KEY.match(value):
-            raise ValueError("secrets must be 22 characters")
-        self._secret = value
+    @retries.setter
+    def retries(self, value: int):
+        self._retries = value
 
     @property
-    def token(self) -> Optional[str]:
-        return self._token
+    def timeout(self) -> Optional[int]:
+        return self._timeout
 
-    @token.setter
-    def token(self, value: Optional[str]) -> None:
-        self._token = value
+    @timeout.setter
+    def timeout(self, value: Optional[int]) -> None:
+        if not isinstance(value, int) and value is not None:
+            raise ValueError("Timeout must be an integer")
+        self._timeout = value
 
     def request(
         self,
         method: str,
         body: Any,
         url: str,
         content_type: Optional[str] = None,
-        version: Optional[int] = None,
+        version: int = DEFAULT_API_VERSION,
         params: Optional[Dict[str, Any]] = None,
         encoding: Optional[str] = None,
     ) -> requests.Response:
         return self._request(method, body, url, content_type, version, params, encoding)
 
     def _request(
         self,
         method: str,
         body: Any,
         url: str,
         content_type: Optional[str] = None,
-        version: Optional[int] = None,
+        version: int = DEFAULT_API_VERSION,
         params: Optional[Dict[str, Any]] = None,
         encoding: Optional[str] = None,
     ) -> requests.Response:
         headers: Dict[str, str] = {
             "User-agent": "UAPythonLib/{0} {1}".format(__about__.__version__, self.key)
         }
         if content_type:
             headers["Content-type"] = content_type
         if version:
             headers["Accept"] = (
-                "application/vnd.urbanairship+json; " "version=%d;" % version
+                "application/vnd.urbanairship+json; " f"version={version};"
             )
         if encoding:
             headers["Content-Encoding"] = encoding
+        self.session.headers.update(headers)
 
         @backoff.on_exception(
             backoff.expo,
             (common.AirshipFailure, common.ConnectionFailure),
             max_tries=(self.retries + 1),
         )
         def make_retryable_request(
             method: str,
             url: str,
             body: Any,
             params: Optional[Dict[str, Any]],
             headers: Dict[str, Any],
         ) -> requests.Response:
+            self.session.headers.update(headers)
+            logger.debug(
+                "Making %s request to %s. Headers:\n\t%s\nBody:\n\t%s",
+                method,
+                url,
+                "\n\t".join(
+                    "%s: %s" % (key, value) for (key, value) in headers.items()
+                ),
+                body,
+            )
             try:
                 response: requests.Response = self.session.request(
                     method,
                     url,
                     data=body,
                     params=params,
-                    headers=headers,
                     timeout=self.timeout,
                 )
             except requests.exceptions.ConnectionError as err:
                 raise common.ConnectionFailure(str(err))
 
             logger.debug(
-                "Making %s request to %s. Headers:\n\t%s\nBody:\n\t%s",
-                method,
-                url,
-                "\n\t".join(
-                    "%s: %s" % (key, value) for (key, value) in headers.items()
-                ),
-                body,
-            )
-
-            logger.debug(
                 "Received %s response. Headers:\n\t%s\nBody:\n\t%s",
                 response.status_code,
                 "\n\t".join(
                     "%s: %s" % (key, value) for (key, value) in response.headers.items()
                 ),
                 response.content,
             )
@@ -253,30 +172,210 @@
             elif not (200 <= response.status_code < 300):
                 raise common.AirshipFailure.from_response(response)
 
             return response
 
         return make_retryable_request(method, url, body, params, headers)
 
-    def create_push(self):
-        """Create a Push notification."""
-        warnings.warn(
-            category=DeprecationWarning,
-            message="the create_push function is deprecated. please use urbanairship.Push. This will be removed in version 7.0",
+
+class BasicAuthClient(BaseClient):
+    """
+    Client class for interacting with the Airship API using either key and master secret
+        or key and application secret, depending on need.
+
+    :param key: [required] An Airship app key (project key) which identifies the project
+    :param secret: [required] An Airship application secret or master secret used to
+        authenticate.
+    :param location: [optional] The Airship cloud site the project is located in.
+        May be 'us' or 'eu'. Defaults to 'us'.
+    :param timeout: [optional]  An integer specifying the number of seconds used
+        for a response timeout threshold
+    :param retries: [optional] An integer specifying the number of times to retry a
+        failed request. Retried requests use exponential backoff between requests.
+        Defaults to 0, no retry.
+    """
+
+    def __init__(
+        self,
+        key: str,
+        secret: str,
+        location: str = "us",
+        timeout: int = DEFAULT_REQ_TIMEOUT_S,
+        retries: int = 0,
+    ) -> None:
+        super().__init__(key=key, location=location, timeout=timeout, retries=retries)
+        self.secret = secret
+        self.session.auth = (self.key, self.secret)
+
+    @property
+    def secret(self) -> Optional[str]:
+        return self._secret
+
+    @secret.setter
+    def secret(self, value: Optional[str]) -> None:
+        if isinstance(value, str) and not VALID_KEY.match(value):
+            raise ValueError("secrets must be 22 characters")
+        self._secret = value
+
+
+class BearerTokenClient(BaseClient):
+    """
+    Client class for interacting with the Airship API using bearer token authentication
+
+    :param key: [required] An Airship app key (project key) which identifies the project
+    :param token: [required]  An Airship-generated bearer token for the provided key.
+    :param location: [optional] The Airship cloud site the project is located in.
+        May be 'us' or 'eu'. Defaults to 'us'.
+    :param timeout: [optional]  An integer specifying the number of seconds used
+        for a response timeout threshold
+    :param retries: [optional] An integer specifying the number of times to retry a
+        failed request. Retried requests use exponential backoff between requests.
+        Defaults to 0, no retry.
+    """
+
+    def __init__(
+        self,
+        key: str,
+        token: str,
+        location: str = "us",
+        timeout: int = DEFAULT_REQ_TIMEOUT_S,
+        retries: int = 0,
+    ) -> None:
+        super().__init__(key=key, location=location, timeout=timeout, retries=retries)
+        self.token = token
+
+        self.session.headers.update(
+            {"X-UA-Appkey": key, "Authorization": f"Bearer {self.token}"}
         )
-        return urbanairship.Push(self)
 
-    def create_scheduled_push(self):
-        """Create a Scheduled Push notification."""
-        warnings.warn(
-            category=DeprecationWarning,
-            message="the create_scheduled_push function is deprecated. please use urbanairship.ScheduledPush. This will be removed in version 7.0",
+    @property
+    def token(self) -> Optional[str]:
+        return self._token
+
+    @token.setter
+    def token(self, value: Optional[str]) -> None:
+        self._token = value
+
+
+class OAuthClient(BaseClient):
+    """
+    Client class for interacting with the Airship API using OAuth2 authentication with
+    JWT assertion.
+    Note - Not all endpoints support OAuth, and client scope may further restrict
+    the endpoints available to a given client. See Airship API documentation for more.
+
+    :param key: [required] An Airship app key (project key) which identifies the project
+    :param client_id: [required] An Airship provided client id used to generate OAuth
+        authentication tokens.
+    :param public_key:  [required] The public key required to sign JWT assertions,
+        passed as a bytestring.
+    :param scope: [optional] A list of scopes to which the issued token will be entitled.
+    :param ip_addr: [optional] A list of CIDR representations of valid IP addresses to
+        which the issued token is restricted.
+    :param location: [optional] The Airship cloud site the project is located in.
+        May be 'us' or 'eu'. Defaults to 'us'.
+    :param timeout: [optional]  An integer specifying the number of seconds used
+        for a response timeout threshold
+    :param retries: [optional] An integer specifying the number of times to retry a
+        failed request. Retried requests use exponential backoff between requests.
+        Defaults to 0, no retry.
+    """
+
+    def __init__(
+        self,
+        key: str,
+        client_id: str,
+        private_key: str,
+        location: str = "us",
+        scope: Optional[List[str]] = None,
+        ip_addr: Optional[List[str]] = None,
+        timeout: int = DEFAULT_REQ_TIMEOUT_S,
+        retries: int = 0,
+    ) -> None:
+        super().__init__(key, location, timeout, retries)
+        self.key = key
+        self.client_id = client_id
+        self.scope = scope
+        self.ip_addr = ip_addr
+        self.private_key = private_key
+        self.token_url: str = (
+            f"{US_OAUTH_URL if self.location == 'us' else EU_OAUTH_URL}/token"
+        )
+        self.token: Optional[str] = None
+        self.urls = Urls(location=self.location, oauth_base=True)
+        self.access_token_expires_at: int = 0
+
+    def _update_session_oauth_token(self) -> None:
+        @backoff.on_exception(
+            backoff.expo,
+            (Timeout, ConnectionError),
+            max_tries=5,
         )
-        return urbanairship.ScheduledPush(self)
+        def _get_or_refresh_token() -> None:
+            assertion_expires_at = int(time.time()) + DEFAULT_ASSERTION_EXPIRY
+            headers = {
+                "alg": "ES384",
+                "kid": self.client_id,
+            }
+            claims = {
+                "aud": self.token_url,
+                "exp": assertion_expires_at,
+                "iat": int(time.time()),
+                "iss": self.client_id,
+                "nonce": str(uuid.uuid4()),
+                "sub": f"app:{self.key}",
+            }
+            if self.scope:
+                claims["scope"] = self.scope
+            if self.ip_addr:
+                claims["ipaddr"] = self.ip_addr
+
+            encoded_jwt = jwt.encode(
+                payload=claims,
+                key=self.private_key,
+                algorithm="ES384",
+                headers=headers,
+            )
+
+            resp = requests.post(
+                self.token_url,
+                data={
+                    "grant_type": "client_credentials",
+                    "assertion": encoded_jwt,
+                },
+                headers={
+                    "Content-Type": "application/x-www-form-urlencoded",
+                    "Accept": "application/json",
+                },
+                timeout=60,
+            )
+            resp_data = resp.json()
+            self.token = resp_data.get("access_token")
+            self.access_token_expires_at = int(time.time()) + int(
+                resp_data.get("expires_in")
+            )
+            self.session.headers.update(
+                {"X-UA-Appkey": self.key, "Authorization": f"Bearer {self.token}"}
+            )
+
+        if not self.token:
+            logger.debug("No OAuth2 access token found. Getting new token.")
+            return _get_or_refresh_token()
+
+        if self.access_token_expires_at < int(time.time()):
+            logger.debug("OAuth access token expired. Refreshing token.")
+            return _get_or_refresh_token()
 
-    def create_template_push(self):
-        """Create a Scheduled Push notification."""
-        warnings.warn(
-            category=DeprecationWarning,
-            message="the create_template_push function is deprecated. please use urbanairship.TemplatePush. This will be removed in version 7.0",
+    def _request(
+        self,
+        method: str,
+        body: Any,
+        url: str,
+        content_type: Optional[str] = None,
+        version: int = DEFAULT_API_VERSION,
+        params: Optional[Dict[str, Any]] = None,
+        encoding: Optional[str] = None,
+    ) -> requests.Response:
+        self._update_session_oauth_token()
+        return super()._request(
+            method, body, url, content_type, version, params, encoding
         )
-        return urbanairship.TemplatePush(self)
```

### Comparing `urbanairship-6.2.0/urbanairship/custom_events/custom_events.py` & `urbanairship-6.3.0/urbanairship/custom_events/custom_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import datetime
-from typing import Dict, Optional, Union
 import json
+from typing import Dict, Optional, Union
 
-from urbanairship import Airship
+from urbanairship.client import BaseClient
 
 
 class CustomEvent:
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         name: str,
         user: Dict,
         interaction_type: Optional[str] = None,
         interaction_id: Optional[str] = None,
         properties: Optional[Dict] = None,
         session_id: Optional[str] = None,
         transaction: Optional[str] = None,
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/__init__.py` & `urbanairship-6.3.0/urbanairship/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `urbanairship-6.2.0/urbanairship/devices/attributes.py` & `urbanairship-6.3.0/urbanairship/devices/attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 from datetime import datetime
-from typing import Dict, List, Optional, Union, Any
+from typing import Any, Dict, List, Optional, Union
 
 from requests import Response
 
-from urbanairship import Airship
+from urbanairship.client import BaseClient
 
 from .static_lists import GzipCompressReadStream
 
 logger = logging.getLogger("urbanairship")
 
 
 class Attribute(object):
@@ -117,15 +117,15 @@
     :keyword attributes: required. A list of one or more Attributes objects.
     :keyword channel: optional. An existing UUID formatted channel_id
     :keyword named_user: optional. An existing named_user_id
     """
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         attributes: List[Attribute],
         channel: Optional[str] = None,
         named_user: Optional[str] = None,
     ) -> None:
         self.airship = airship
         self.attributes = attributes
         self.channel = channel
@@ -196,15 +196,15 @@
     :param description: Required. A description of your list.
     :param extra: Optional. An optional dict of up to 100 key-value (string-to-string)
         pairs associated with the list.
     """
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         list_name: str,
         description: str,
         extra: Optional[Dict[str, str]] = None,
     ):
         self.airship = airship
         self.list_name = list_name
         self.description = description
@@ -268,15 +268,15 @@
             + self.list_name
             + "/errors/",
         )
 
         return response
 
     @classmethod
-    def list(cls, airship: Airship) -> Response:
+    def list(cls, airship: BaseClient) -> Response:
         """Lists existing attribute lists.
 
         :param airship: An urbanairship.Airship instance.
         """
         response = airship._request(
             method="GET",
             url=airship.urls.get("attributes_list_url"),
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/devicelist.py` & `urbanairship-6.3.0/urbanairship/devices/devicelist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import logging
-from typing import Any, Dict, Optional, List, Generic, TypeVar
+from typing import Any, Dict, List, Optional, TypeVar
 
-from urbanairship import common, Airship
+from urbanairship import common
+from urbanairship.client import BaseClient
 
 logger = logging.getLogger("urbanairship")
 
 ChannelInfoType = TypeVar("ChannelInfoType", bound="ChannelInfo")
 
 
 class ChannelInfo(object):
@@ -72,15 +73,15 @@
     transactional_opted_in: Optional[str] = None
     transactional_opted_out: Optional[str] = None
 
     def __init__(self, airship):
         self.airship = airship
 
     @classmethod
-    def from_payload(cls, payload: Dict, device_key: str, airship: Airship):
+    def from_payload(cls, payload: Dict, device_key: str, airship: BaseClient):
         """Create based on results from a ChannelList iterator."""
         obj = cls(airship)
         obj.channel_id = payload[device_key]
         if airship:
             obj.airship = airship
         for key in payload:
             if key in (
@@ -91,15 +92,15 @@
                 "transactional_opted_in",
                 "transactional_opted_out",
             ):
                 try:
                     payload[key] = datetime.datetime.strptime(
                         payload[key], "%Y-%m-%dT%H:%M:%S"
                     )
-                except:
+                except (KeyError, ValueError):
                     payload[key] = "UNKNOWN"
             setattr(obj, key, payload[key])
         return obj
 
     def lookup(self, channel_id: str):
         """Fetch metadata from a channel ID"""
         start_url = self.airship.urls.get("channel_url")
@@ -132,30 +133,30 @@
 
     id: Optional[str] = None
     device_type: Optional[str] = None
     active: Optional[bool] = None
     tags: Optional[List] = None
     alias: Optional[str] = None
 
-    def __init__(self, airship: Airship):
+    def __init__(self, airship: BaseClient):
         self.airship = airship
 
     @classmethod
-    def from_payload(cls, payload: Dict, device_key: str, airship: Airship):
+    def from_payload(cls, payload: Dict, device_key: str, airship: BaseClient):
         """Create based on results from a DeviceTokenList or APIDList iterator."""
         obj = cls(airship)
         obj.id = payload[device_key]
         obj.device_type = device_key
         for key in payload:
             if key in "created":
                 try:
                     payload[key] = datetime.datetime.strptime(
                         payload[key], "%Y-%m-%d %H:%M:%S"
                     )
-                except:
+                except (KeyError, ValueError):
                     payload[key] = "UNKNOWN"
             setattr(obj, key, payload[key])
         return obj
 
 
 class DeviceTokenList(common.IteratorParent):
     """Iterator for listing all device tokens for this application.
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/email.py` & `urbanairship-6.3.0/urbanairship/devices/email.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import logging
 import re
 from typing import Any, Dict, List, Optional
 
 from requests import Response
 
-from urbanairship import Airship
+from urbanairship.client import BaseClient
 
 logger = logging.getLogger("urbanairship")
 
 VALID_EMAIL = re.compile(r"(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)")
 VALID_ISO_8601 = re.compile(
     "^(-?(?:[1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])"
     "T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\\.[0-9]+)?(Z)?$"
@@ -50,15 +50,15 @@
         timezone setting.
     :param template_fields: For use with CreateAndSend with inline templates.
         A dict of template field names and their substitution values.
     """
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         address: str,
         commercial_opted_in: Optional[str] = None,
         commercial_opted_out: Optional[str] = None,
         transactional_opted_in: Optional[str] = None,
         transactional_opted_out: Optional[str] = None,
         locale_country: Optional[str] = None,
         locale_language: Optional[str] = None,
@@ -152,15 +152,15 @@
     def transactional_opted_out(self, value: Optional[str]) -> None:
         if value is not None and not VALID_ISO_8601.match(value):
             raise ValueError("Must use ISO 8601 timestamp format")
         self._transactional_opted_out = value
 
     @property
     def _full_payload(self) -> Dict[str, Any]:
-        if self.address == None:
+        if self.address is None:
             raise ValueError(
                 "address must be set to register or update an email channel"
             )
 
         payload: Dict[str, Any] = {"type": self._email_type}
 
         reg_payload_keys = [
@@ -290,15 +290,15 @@
         response = self.airship.request(method="POST", body=body, url=url, version=3)
 
         logger.info("Uninstalled email address: %s" % self.address)
 
         return response
 
     @classmethod
-    def lookup(cls, airship: Airship, address: str) -> Response:
+    def lookup(cls, airship: BaseClient, address: str) -> Response:
         if not VALID_EMAIL.match(address) and address is not None:
             raise ValueError("Invalid email address format")
 
         url = airship.urls.get("email_url") + address
 
         response = airship.request(method="GET", url=url, version=3, body=None)
 
@@ -307,15 +307,15 @@
 
 class EmailTags(object):
     """Add, remove or set tags for a list of email addresses
 
     :param address: an email address to mutate tags for
     """
 
-    def __init__(self, airship: Airship, address: str):
+    def __init__(self, airship: BaseClient, address: str):
         self.airship = airship
         self.url = airship.urls.get("email_tags_url")
         self.address = address
         self.add_group: Dict[str, Any] = {}
         self.remove_group: Dict[str, Any] = {}
         self.set_group: Dict[str, Any] = {}
         self._payload: Dict[str, Any] = {}
@@ -409,15 +409,15 @@
         have permissions set to be opened in 'rb' (binary) mode.
 
     :return: the response object from the API including the 'attachment_ids' uuid to
         be used in the email override object.
     """
 
     def __init__(
-        self, airship: Airship, filename: str, content_type: str, filepath: str
+        self, airship: BaseClient, filename: str, content_type: str, filepath: str
     ) -> None:
         self.airship = airship
         self.filename = filename
         self.content_type = content_type
         self.filepath = filepath
 
     def _encode_attachment(self, filepath: str) -> str:
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/named_users.py` & `urbanairship-6.3.0/urbanairship/devices/named_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import json
 import logging
-from typing import Any, Dict, List, Optional, Union, TypeVar
+from typing import Any, Dict, List, Optional, Union
 
 from requests import Response
 
+from urbanairship import common
+from urbanairship.client import BaseClient
 from urbanairship.devices import ChannelTags
-from urbanairship import common, Airship
 
 logger = logging.getLogger("urbanairship")
 
 
 class NamedUser(object):
     """
     Perform various operations on a named user object
 
     :param airship: Required. An instance of urbanairship.Airship.
     """
 
-    def __init__(self, airship: Airship, named_user_id: Optional[str] = None) -> None:
+    def __init__(
+        self, airship: BaseClient, named_user_id: Optional[str] = None
+    ) -> None:
         self._airship = airship
         self.named_user_id = named_user_id
         self.channel_id: Optional[str] = None
         self.email_address: Optional[str] = None
         self.device_type: Optional[str] = None
 
     @property
@@ -268,15 +271,16 @@
         Set or remove attributes on a named user.
         A single request body may contain a set or remove field, or both, or a single
         set field. If both set and remove fields are present and the intersection of
         the attributes in these fields is not empty, then a 400 will be returned.
         If an attribute request is partially valid, i.e. at least one attribute exists,
         Airship returns a 200 with a warning in containing a list of attributes that
         failed to update.
-        Please see https://docs.airship.com/api/ua/#operation-api-named_users-named_user_id-attributes-post
+        Please see
+        https://docs.airship.com/api/ua/#operation-api-named_users-named_user_id-attributes-post
         for more about using Airship attributes.
 
         :params attributes: Required. A list of attribute objects to set or remove on
             the named user.
         """
         if type(attributes) is not list:
             raise ValueError("attributes must be a list of attribute objects")
@@ -288,15 +292,15 @@
             content_type="application/json",
             version=3,
         )
 
         return response
 
     @classmethod
-    def uninstall(cls, airship: Airship, named_users: List[str]) -> Response:
+    def uninstall(cls, airship: BaseClient, named_users: List[str]) -> Response:
         """
         Disassociate and delete all channels associated with the named_user_id(s) and
         also delete the named_user_id(s). This call removes all channels associated
         with a named user from Airship systems in compliance with data privacy laws.
         Uninstalling channels also removes accompanying analytic data (including
         Performance Analytics) from the system.
         Channel uninstallation, like channel creation, is an asynchronous operation,
@@ -335,23 +339,23 @@
 
 class NamedUserList(common.IteratorParent):
     """Retrieves a list of NamedUsers"""
 
     next_url: Optional[str] = None
     data_attribute: str = "named_users"
 
-    def __init__(self, airship: Airship):
+    def __init__(self, airship: BaseClient):
         self.next_url = airship.urls.get("named_user_url")
         super(NamedUserList, self).__init__(airship, None)
 
 
 class NamedUserTags(ChannelTags):
     """Modify the tags for named users"""
 
-    def __init__(self, airship: Airship) -> None:
+    def __init__(self, airship: BaseClient) -> None:
         super(NamedUserTags, self).__init__(airship)
         self.url = airship.urls.get("named_user_tag_url")
 
     def set_audience(
         self,
         user_ids: Optional[List[str]] = None,
         ios: Optional[str] = None,
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/open_channel.py` & `urbanairship-6.3.0/urbanairship/devices/open_channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import json
 import logging
 import re
-from typing import Any, Optional, Dict, List
+from typing import Any, Dict, List, Optional
 
 from requests import Response
 
-from urbanairship import Airship
+from urbanairship.client import BaseClient
 
 VALID_UUID = re.compile(r"[0-9a-f]{12}4[0-9a-f]{3}[89ab][0-9a-f]{15}\Z")
 
 logger = logging.getLogger("urbanairship")
 
 
 class OpenChannel(object):
@@ -29,15 +29,15 @@
     opt_in: Optional[bool] = None
     installed: Optional[bool] = None
     created: Optional[str] = None
     last_registration: Optional[str] = None
     tags: Optional[List] = None
     template_fields: Optional[Dict] = None
 
-    def __init__(self, airship: Airship) -> None:
+    def __init__(self, airship: BaseClient) -> None:
         self.airship = airship
 
     @property
     def create_and_send_audience(self) -> Dict:
         if not self.address:
             raise ValueError("open channel address must be set")
 
@@ -127,15 +127,15 @@
         logger.info(
             "Successful open channel update: %s (%s)", self.channel_id, self.address
         )
 
         return response
 
     @classmethod
-    def from_payload(cls, payload: Dict, airship: Airship):
+    def from_payload(cls, payload: Dict, airship: BaseClient):
         """Instantiate an OpenChannel from a payload."""
         obj = cls(airship)
         for key in payload:
             # Extract the open channel data
             if key == "open":
                 obj.open_platform = payload["open"].get("open_platform_name")
                 obj.identifiers = payload["open"].get("identifiers", [])
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/segment.py` & `urbanairship-6.3.0/urbanairship/devices/segment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import json
 import logging
-from typing import Optional, Dict, TypeVar
+from typing import Dict, Optional
 
 from requests import Response
 
-from urbanairship import common, Airship
+from urbanairship import common
+from urbanairship.client import BaseClient
 
 logger = logging.getLogger("urbanairship")
 
 
 class Segment(object):
     url: Optional[str] = None
     id: Optional[str] = None
     display_name: Optional[str] = None
     creation_date: Optional[str] = None
     modification_date: Optional[str] = None
     criteria: Optional[str] = None
     data: Optional[Dict] = None
 
-    def create(self, airship: Airship) -> Response:
+    def create(self, airship: BaseClient) -> Response:
         """Create a Segment object and return it."""
 
         url = airship.urls.get("segments_url")
 
         body = json.dumps(
             {"display_name": self.display_name, "criteria": self.criteria}
         )
@@ -34,15 +35,15 @@
 
         self.id = seg_id
         self.from_id(airship, seg_id)
 
         return response
 
     @classmethod
-    def from_id(cls, airship: Airship, seg_id: str):
+    def from_id(cls, airship: BaseClient, seg_id: str):
         """Retrieve a segment based on the provided ID."""
 
         url = airship.urls.get("segments_url") + seg_id
         response = airship._request(method="GET", body=None, url=url, version=3)
 
         payload = response.json()
         cls.id = seg_id
@@ -55,29 +56,29 @@
         """Create segment based on results from a SegmentList iterator."""
 
         for key in payload:
             setattr(cls, key, payload[key])
 
         return cls
 
-    def update(self, airship: Airship) -> Response:
+    def update(self, airship: BaseClient) -> Response:
         """Updates the segment associated with data in the current object."""
 
         data = {}
         data["display_name"] = self.display_name
         data["criteria"] = self.criteria
 
         url = f'{airship.urls.get("segments_url")}{self.id}'
         body = json.dumps(data)
         response = airship._request(method="PUT", body=body, url=url, version=3)
         logger.info("Successful segment update: '{0}'".format(self.display_name))
 
         return response
 
-    def delete(self, airship: Airship) -> Response:
+    def delete(self, airship: BaseClient) -> Response:
         url = f'{airship.urls.get("segments_url")}{self.id}'
         res = airship._request(method="DELETE", body=None, url=url, version=3)
         logger.info("Successful segment deletion: '{0}'".format(self.display_name))
         return res
 
 
 class SegmentList(common.IteratorParent):
@@ -86,11 +87,11 @@
     :keyword limit: Number of segments to fetch
 
     """
 
     next_url: Optional[str] = None
     data_attribute: str = "segments"
 
-    def __init__(self, airship: Airship, limit: Optional[int] = None):
+    def __init__(self, airship: BaseClient, limit: Optional[int] = None):
         self.next_url = airship.urls.get("segments_url")
         params = {"limit": limit} if limit else {}
         super(SegmentList, self).__init__(airship, params)
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/sms.py` & `urbanairship-6.3.0/urbanairship/devices/sms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from datetime import datetime
 import json
 import logging
 import re
-from typing import Dict, Optional, List, Union, Any
+from datetime import datetime
+from typing import Any, Dict, List, Optional
 
 from requests import Response
 
-from urbanairship import Airship
+
+from urbanairship.client import BaseClient
 
 logger = logging.getLogger("urbanairship")
 
 VALID_MSISDN = re.compile(r"[0-9]*$")
 VALID_SENDER = re.compile(r"[0-9]*$")
 
 
@@ -35,15 +36,15 @@
         this field becomes a tag in the ua_locale_language tag group.
     :param timezone: The IANA identifier for a timezone, e.g. "America/Los_Angeles".
         The value in this field becomes a tag in the timezone tag group.
     """
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         sender: str,
         msisdn: str,
         opted_in: Optional[datetime] = None,
         template_fields: Optional[Dict] = None,
         locale_country: Optional[str] = None,
         locale_language: Optional[str] = None,
         timezone: Optional[str] = None,
@@ -304,15 +305,15 @@
     :param msisdn: Required. The MSISDN to use for the interacton.
     :param sender_ids: Required. A list of sender id values to use for the interaction.
     :param timestamp: Optional. A datetime.datetime representing the time of the interaction.
     """
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         keyword: str,
         msisdn: str,
         sender_ids: List[str],
         timestamp: Optional[datetime] = None,
     ) -> None:
         self.airship = airship
         self.keyword = keyword
@@ -376,15 +377,15 @@
         `ua.sms()`. This defines the message sent in response.
     :param mms: [optional] An MMS platform override object, created using
         `us.mms()`. The defines the message sent in response.
     """
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         mobile_originated_id: str,
         sms: Optional[Dict] = None,
         mms: Optional[Dict] = None,
     ) -> None:
         self.airship = airship
         self.mobile_originated_id = mobile_originated_id
         self.sms = sms
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/static_lists.py` & `urbanairship-6.3.0/urbanairship/devices/static_lists.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import json
-import gzip
 import collections
 import datetime
-from typing import Dict, Optional
+import gzip
+import json
 from io import TextIOWrapper
+from typing import Dict, Optional
 
 from requests import Response
 
-from urbanairship import common, Airship
+from urbanairship import common
+from urbanairship.client import BaseClient
 
 CHUNK = 16 * 1024
 
 
 class StaticList:
-    def __init__(self, airship: Airship, name: str) -> None:
+    def __init__(self, airship: BaseClient, name: str) -> None:
         self.airship = airship
         self.name = name
         self.description = None
         self.extra = None
 
     def create(self) -> Dict:
         """Create a Static List"""
@@ -80,15 +81,15 @@
         response = self.airship._request(
             "PUT", body, url, "application/json", version=3
         )
 
         return response.json()
 
     @classmethod
-    def download(cls, airship: Airship, list_name: str) -> Response:
+    def download(cls, airship: BaseClient, list_name: str) -> Response:
         """
         Allows you to download the contents of a static list. Alias and named_user
         values are resolved to channels.
 
         :param airship: Required. An urbanairship.Airship instance.
         :param list_name: Required. Name of an existing list to download.
 
@@ -99,15 +100,15 @@
             url=airship.urls.get("lists_url") + list_name + "/csv/",
             body={},
         )
 
         return response
 
     @classmethod
-    def from_payload(cls, payload: Dict, airship: Airship):
+    def from_payload(cls, payload: Dict, airship: BaseClient):
         for key in payload:
             if key in "created" or key in "last_updated":
                 payload[key] = datetime.datetime.strptime(
                     payload[key], "%Y-%m-%dT%H:%M:%S"
                 )
             setattr(cls, key, payload[key])
         return cls
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/subscription_lists.py` & `urbanairship-6.3.0/urbanairship/devices/subscription_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 from typing import Dict
 
 from requests import Response
 
-from urbanairship import Airship
+from urbanairship.client import BaseClient
 
 
 class SubscriptionList(object):
     """
     Subscribe or unsubscribe channels to/from Subscription lists. These lists must
     be created in the Airship web dashboard prior to making these calls. The
     value for list_id can be found after creating these lists.
 
     :param airship: Required. An urbanairship.Airship instance.
     :param list_id: Required. The list_id from the Airship web dashboard.
     """
 
-    def __init__(self, airship: Airship, list_id: str) -> None:
+    def __init__(self, airship: BaseClient, list_id: str) -> None:
         self.airship = airship
         self.list_id = list_id
 
     def unsubscribe(self, audience: Dict) -> Response:
         """
         Unsubscribe an audience from a subscription list.
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/tag.py` & `urbanairship-6.3.0/urbanairship/devices/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 import logging
-from typing import Dict, Optional, List, Any
+from typing import Any, Dict, List, Optional
 
-from urbanairship import Airship
+from urbanairship.client import BaseClient
 
 logger = logging.getLogger("urbanairship")
 
 
 class ChannelTags(object):
     """Modify the tags for a channel
 
     :param airship: An urbanairship.Airship instance.
     """
 
-    def __init__(self, airship: Airship) -> None:
+    def __init__(self, airship: BaseClient) -> None:
         self.url = airship.urls.get("channel_url") + "tags/"
         self._airship = airship
         self.audience: Dict[str, Any] = {}
         self.add_group: Dict[str, Any] = {}
         self.remove_group: Dict[str, Any] = {}
         self.set_group: Dict[str, Any] = {}
 
@@ -58,15 +58,16 @@
         :param group_name: The name of the tag group to remove
         :param tags: The tags to addremove
         """
         self.remove_group[group_name] = tags
 
     def set(self, group_name: str, tags: List[str]) -> None:
         """
-        Sets group and tags to set. Note that a ``set`` operation replaces all tags on the audience upon send.
+        Sets group and tags to set. Note that a ``set`` operation replaces all
+        tags on the audience upon send.
 
         :param group_name: The name of the tag group to set
         :param tags: The tags to set
         """
         self.set_group[group_name] = tags
 
     def send(self) -> Dict:
@@ -106,15 +107,15 @@
         )
         return response.json()
 
 
 class OpenChannelTags(object):
     """Modify the tags for an open channel"""
 
-    def __init__(self, airship: Airship) -> None:
+    def __init__(self, airship: BaseClient) -> None:
         self.url = airship.urls.get("open_channel_url") + "tags/"
         self._airship = airship
         self.audience: Dict = {}
         self.add_group: Dict = {}
         self.remove_group: Dict = {}
         self.set_group: Dict = {}
 
@@ -140,15 +141,16 @@
         :param group_name: The name of the tag group to remove
         :param tags: The tags to addremove
         """
         self.remove_group[group_name] = tags
 
     def set(self, group_name: str, tags: List[str]) -> None:
         """
-        Sets group and tags to set. Note that a ``set`` operation replaces all tags on the audience upon send.
+        Sets group and tags to set. Note that a ``set`` operation replaces all tags on
+        the audience upon send.
 
         :param group_name: The name of the tag group to set
         :param tags: The tags to set
         """
         self.set_group[group_name] = tags
 
     def send(self) -> Dict:
```

### Comparing `urbanairship-6.2.0/urbanairship/devices/tag_lists.py` & `urbanairship-6.3.0/urbanairship/devices/tag_lists.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
-from typing import Dict, Optional, Any, List
+from typing import Any, Dict, List, Optional
 
 from requests import Response
 
-from urbanairship import Airship
+from urbanairship.client import BaseClient
 from urbanairship.devices.static_lists import GzipCompressReadStream
 
 
 class TagList:
     """Create, Upload, Delete, and get information for a tag list.
     Please see the Airship API documentation for more information
     about CSV formatting, limits, and use of this feature.
@@ -23,15 +23,15 @@
     :param set_tags: Optional. A dictionary consisting of a tag group string and list of tag
     strings to set on uploaded channels. Warning: This action is destructive and will
     remove all existing tags associated with channels.
     """
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         list_name: str,
         description: Optional[str] = None,
         extra: Optional[Dict[str, str]] = None,
         add_tags: Optional[Dict[str, List[str]]] = None,
         remove_tags: Optional[Dict[str, List[str]]] = None,
         set_tags: Optional[Dict[str, List[str]]] = None,
     ) -> None:
@@ -105,15 +105,15 @@
             body={},
             url=f"{self.airship.urls.get('tag_lists_url')}/{self.list_name}/errors",
             version=3,
         )
         return response
 
     @classmethod
-    def list(cls, airship: Airship) -> Response:
+    def list(cls, airship: BaseClient) -> Response:
         """Returns a json string with details on all tag lists associated with
         an Airship instance / project.
 
         :return: Response object
         """
         response = airship.request(
             method="GET", body={}, url=airship.urls.get("tag_lists_url"), version=3
```

### Comparing `urbanairship-6.2.0/urbanairship/experiments/core.py` & `urbanairship-6.3.0/urbanairship/experiments/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from typing import Any, Dict, Optional
 import json
+from typing import Any, Dict, Optional
+
+from requests import Response
 
+from urbanairship.client import BaseClient
 from urbanairship.experiments.experiment import Experiment
 
 
 class ABTest(object):
-    def __init__(self, airship):
+    def __init__(self, airship: BaseClient):
         self.airship = airship
 
-    def _get_listing(self, url: str, limit: Optional[int] = None) -> Dict:
+    def _get_listing(self, url: str, limit: Optional[int] = None) -> Response:
         """List experiments
 
         :keyword limit: Optional, maximum number of experiments,
         default is 10, max is 100
         """
 
         params: Dict[str, Any] = {}
@@ -20,56 +23,56 @@
             params["limit"] = limit
 
         response = self.airship.request(
             method="GET", body=None, params=params, url=url, version=3
         )
         return response
 
-    def list_experiments(self) -> Dict:
+    def list_experiments(self) -> Response:
         """List experiments, sorted by created_at date/time from newest to oldest
 
         :keyword limit: Positive maximum number of elements to return per page.
             Default limit is 10. Max: 100 and Min: 1.
         """
         url = self.airship.urls.get("experiments_url")
         return self._get_listing(url)
 
-    def create(self, experiment: Experiment) -> Dict:
+    def create(self, experiment: Experiment) -> Response:
         """Create an experiment"""
 
         url = self.airship.urls.get("experiments_url")
         body = json.dumps(experiment.payload)
         response = self.airship.request(
             method="POST",
             body=body,
             url=url,
             content_type="application/json",
             version=3,
         )
         return response
 
-    def list_scheduled_experiment(self) -> Dict:
+    def list_scheduled_experiment(self) -> Response:
         """List scheduled experiments in order, from closest to the current
         date-time to farthest"""
 
         url = self.airship.urls.get("experiments_schedule_url")
         return self._get_listing(url)
 
-    def delete(self, experiment_id: str) -> Dict:
+    def delete(self, experiment_id: str) -> Response:
         """Delete a scheduled experiment. You can only delete experiments before they start
 
         :keyword experiment_id: The unique identifier of the experiment, type string
         """
 
         url = self.airship.urls.get("experiments_schedule_url") + "/" + experiment_id
         response = self.airship.request(method="DELETE", body=None, url=url, version=3)
 
         return response
 
-    def validate(self, experiment: Experiment) -> Dict:
+    def validate(self, experiment: Experiment) -> Response:
         """Accepts the same range of payloads as /api/experiments,
         but only parses and validates the payload without creating the experiment.
         An experiment may validate and still fail to be delivered. For example,
         you may have a valid experiment with no devices in your audience.
 
         :keyword experiment: Body of the experiment you want to validate
         """
@@ -81,15 +84,15 @@
             url=url,
             content_type="application/json",
             version=3,
         )
 
         return response
 
-    def lookup(self, experiment_id: str) -> Dict:
+    def lookup(self, experiment_id: str) -> Response:
         """Look up an experiment (A/B Test)
 
         :keyword experiment_id: The unique identifier of the experiment, type string
         """
 
         url = self.airship.urls.get("experiments_url") + "/" + experiment_id
         response = self.airship.request(method="GET", body=None, url=url, version=3)
```

### Comparing `urbanairship-6.2.0/urbanairship/experiments/experiment.py` & `urbanairship-6.3.0/urbanairship/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `urbanairship-6.2.0/urbanairship/experiments/variant.py` & `urbanairship-6.3.0/urbanairship/experiments/variant.py`

 * *Files identical despite different names*

### Comparing `urbanairship-6.2.0/urbanairship/push/__init__.py` & `urbanairship-6.3.0/urbanairship/push/__init__.py`

 * *Files identical despite different names*

### Comparing `urbanairship-6.2.0/urbanairship/push/audience.py` & `urbanairship-6.3.0/urbanairship/push/audience.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 DEVICE_TOKEN_FORMAT = re.compile(r"^[0-9a-fA-F]{64}$")
 UUID_FORMAT = re.compile(
     r"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}" r"-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$"
 )
 SMS_SENDER_FORMAT = re.compile(r"^[0-9]*$")
 SMS_MSISDN_FORMAT = re.compile(r"^[0-9]*$")
 
+
 # Value selectors; device IDs, aliases, tags, etc.
 def ios_channel(uuid: str) -> Dict[str, str]:
     """Select a single iOS Channel"""
     if not UUID_FORMAT.match(uuid):
         raise ValueError("Invalid iOS Channel")
     return {"ios_channel": uuid.lower().strip()}
```

### Comparing `urbanairship-6.2.0/urbanairship/push/core.py` & `urbanairship-6.3.0/urbanairship/push/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import json
-from lib2to3.pgen2.token import OP
 import logging
-import warnings
-from typing import Any, Dict, Optional, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 from requests import Response
 
-from urbanairship import Airship, devices
-
+from urbanairship import devices
+from urbanairship.client import BaseClient
 
 logger = logging.getLogger("urbanairship")
 
 
 class PushResponse(object):
     """Response to a successful push notification send or schedule.
 
@@ -40,15 +38,15 @@
     def __str__(self) -> str:
         return "Response Payload: {0}".format(self.payload)
 
 
 class Push(object):
     """A push notification. Set audience, message, etc, and send."""
 
-    def __init__(self, airship: Airship) -> None:
+    def __init__(self, airship: BaseClient) -> None:
         self._airship = airship
         self.audience: Optional[Union[Dict, List[Dict]]] = None
         self.notification: Optional[Dict[str, Any]] = None
         self.options: Optional[Dict[str, Any]] = None
         self.campaigns: Optional[Dict[str, Any]] = None
         self.message: Optional[Dict[str, Any]] = None
         self.in_app: Optional[Dict[str, Any]] = None
@@ -137,15 +135,15 @@
         logger.info(
             "Push successful. push_ids: %s", ", ".join(data.get("push_ids", []))
         )
 
         return PushResponse(response)
 
     @classmethod
-    def message_center_delete(cls, airship: Airship, push_id: str) -> Response:
+    def message_center_delete(cls, airship: BaseClient, push_id: str) -> Response:
         """
         Delete a Message Center message completely, removing it from every user's inbox.
         This is an asynchronous call; a success response means that the deletion has
         been queued for processing.
         This delete call will work with either the message_id or the push_id of the
         accompanying push notification.
         This endpoint will not work with a group_id from an automated message or a
@@ -168,24 +166,24 @@
 
         return response
 
 
 class ScheduledPush(object):
     """A scheduled push notification. Set schedule, push, and send."""
 
-    def __init__(self, airship: Airship):
+    def __init__(self, airship: BaseClient):
         self._airship = airship
         self.schedule: Optional[Dict[str, Any]] = None
         self.recurring: Optional[Dict[str, Any]] = None
         self.name: Optional[str] = None
         self.push: Optional[Push] = None
         self.url: Optional[str] = None
 
     @classmethod
-    def from_url(cls, airship: Airship, url: str):
+    def from_url(cls, airship: BaseClient, url: str):
         """Load an existing scheduled push from its URL."""
 
         sched = cls(airship)
         response = sched._airship._request(method="GET", body=None, url=url, version=3)
         payload = response.json()
         sched.name = payload.get("name")
         sched.schedule = payload["schedule"]
@@ -197,15 +195,15 @@
             sched.push.message = payload["push"]["message"]
         if "options" in payload["push"]:
             sched.push.options = payload["push"]["options"]
         sched.url = url
         return sched
 
     @classmethod
-    def from_payload(cls, payload: Dict, id_key: str, airship: Airship):
+    def from_payload(cls, payload: Dict, id_key: str, airship: BaseClient):
         """Create based on results from a ScheduledList iterator."""
         obj = cls(airship)
         for key in payload:
             setattr(obj, key, payload[key])
         return obj
 
     @property
@@ -342,15 +340,15 @@
         return PushResponse(response)
 
 
 class TemplatePush(object):
     """A personalized push notification. Set details and send."""
 
     def __init__(self, airship):
-        self._airship: Airship = airship
+        self._airship: BaseClient = airship
         self.audience: Optional[Dict] = None
         self.device_types: Optional[List] = None
         self.merge_data: Optional[Dict] = None
 
     @property
     def payload(self) -> Dict:
         data: Dict[str, Any] = {
@@ -405,15 +403,15 @@
     :param airship: Required. An urbanairship.Airship object instantiated with
         master authentication.
     :param channels: Required. A list of Sms, Email or OpenChannel objects.
         channels may only be of one type and must match the single value for
         CreateAndSend.device_types.
     """
 
-    def __init__(self, airship: Airship, channels: List):
+    def __init__(self, airship: BaseClient, channels: List):
         self._airship = airship
         self.channels = channels
         self.notification: Optional[Dict] = None
         self.campaigns: Optional[Dict] = None
 
     @property
     def device_types(self) -> List[str]:
```

### Comparing `urbanairship-6.2.0/urbanairship/push/payload.py` & `urbanairship-6.3.0/urbanairship/push/payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding=utf-8
 import collections
 import re
 import warnings
-from typing import List, Dict, Optional, Any, Union
+from typing import Any, Dict, List, Optional, Union
 
 from urbanairship.enums import LiveActivityEvent, LiveUpdateEvent
 
 # Valid autobadge values: auto, +N, -N
 VALID_AUTOBADGE = re.compile(r"^(auto|[+-][\d]+)$")
 VALID_ICON_COLOR = re.compile(r"^#[0-9a-f]{6}$")
 VALID_ANDROID_CATEGORIES: List[str] = [
@@ -952,29 +952,29 @@
         payload["interactive"] = interactive
     if extra is not None:
         extra["extra"] = extra
 
     return payload
 
 
-def device_types(*types: Any) -> Union[str, List[str]]:
+def device_types(*types: Any) -> List[str]:
     """Create a device type specifier.
 
     >>> device_types('ios', 'wns')
     ['ios', 'wns']
     >>> device_types('ios', 'symbian')
     Traceback (most recent call last):
         ...
     ValueError: Invalid device type 'symbian'
 
     """
     valid_device_types = ("ios", "android", "amazon", "wns", "web", "sms", "email")
-    if types == "all" or (len(types) == 1 and types[0] == "all"):
+    if len(types) == 1 and types[0] == "all":
         warnings.warn("The device type 'all' has been deprecated.", DeprecationWarning)
-        return "all"
+        return ["all"]
 
     for t in types:
         is_open = isinstance(t, str) and t.startswith("open::")
         if t not in valid_device_types and not is_open:
             raise ValueError("Invalid device type '%s'" % t)
     return [t for t in types]
```

### Comparing `urbanairship-6.2.0/urbanairship/push/schedule.py` & `urbanairship-6.3.0/urbanairship/push/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import datetime
+from typing import Any, Dict, List, Optional, Type
 
-from typing import Any, List, Dict, Optional, Type
-
-from urbanairship import common, Airship
+from urbanairship import common
+from urbanairship.client import BaseClient
 from urbanairship.push.core import ScheduledPush
 
-
 VALID_DAYS: List[str] = [
     "monday",
     "tuesday",
     "wednesday",
     "thursday",
     "friday",
     "saturday",
@@ -30,15 +29,15 @@
     """
 
     next_url: Optional[str] = None
     data_attribute: str = "schedules"
     id_key: str = "url"
     instance_class: Type[ScheduledPush] = ScheduledPush
 
-    def __init__(self, airship: Airship, limit: Optional[int] = None) -> None:
+    def __init__(self, airship: BaseClient, limit: Optional[int] = None) -> None:
         self.next_url = airship.urls.get("schedules_url")
         params = {"limit": limit} if limit else {}
         super(ScheduledList, self).__init__(airship, params)
 
 
 def scheduled_time(timestamp: datetime) -> Dict[str, Any]:
     """Specify a time for the delivery of this push.
```

### Comparing `urbanairship-6.2.0/urbanairship/push/template.py` & `urbanairship-6.3.0/urbanairship/push/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import datetime
 import json
 import logging
-from typing import Dict, List, Optional, Any, Type
+from typing import Any, Dict, List, Optional, Type
 
 from requests import Response
 
-from urbanairship import common, Airship
+from urbanairship import common
+from urbanairship.client import BaseClient
 from urbanairship.push.core import Push
 
-
 logger = logging.getLogger("urbanairship")
 
 
 class Template(object):
     """Information object for a template.
 
     :keyword template_id: UUID; the ID of this template, set automatically.
@@ -33,15 +33,15 @@
         messages are sent. Message Center ``message`` is also not supported in
         Templates at this time.
 
     """
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         name: Optional[str] = None,
         description: Optional[str] = None,
         variables: Optional[List[Dict[str, Any]]] = None,
         push: Optional[Type[Push]] = None,
     ) -> None:
         self.airship = airship
         self._template_id: Optional[str] = None
@@ -190,15 +190,15 @@
         obj._template_id = payload[id_key]
         for key in payload:
             if key in ("created_at", "modified_at", "last_used"):
                 try:
                     payload[key] = datetime.datetime.strptime(
                         payload[key], "%Y-%m-%dT%H:%M:%S.%fZ"
                     )
-                except:
+                except (KeyError, ValueError, TypeError):
                     payload[key] = "UNKNOWN"
                 setattr(obj, "_" + key, payload[key])
             elif key == "template_id":
                 obj._template_id = payload[key]
             else:
                 setattr(obj, key, payload[key])
         return obj
```

### Comparing `urbanairship-6.2.0/urbanairship/reports/experiments.py` & `urbanairship-6.3.0/urbanairship/reports/experiments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Dict, Any
+from typing import Any, Dict
 
-from urbanairship import Airship
+from urbanairship.client import BaseClient
 
 
 class ExperimentReport(object):
-    def __init__(self, airship: Airship) -> None:
+    def __init__(self, airship: BaseClient) -> None:
         """Access reporting related to A/B Tests (experiments)
 
         :param airship: An urbanairship.Airship instance.
         """
         self.airship = airship
 
     def get_overview(self, push_id: str) -> Dict[str, Any]:
```

### Comparing `urbanairship-6.2.0/urbanairship/reports/reports.py` & `urbanairship-6.3.0/urbanairship/reports/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import datetime
-from typing import Dict, Any, Optional
+from typing import Optional
 
-from urbanairship import common, Airship
+from urbanairship import common
+from urbanairship.client import BaseClient
 
 DATE_FORMAT_STR: str = "%Y-%m-%d %H:%M:%S"
 
 
 class IndividualResponseStats(object):
     """Returns detailed reports information about a specific push notification."""
 
-    def __init__(self, airship: Airship) -> None:
+    def __init__(self, airship: BaseClient) -> None:
         self.airship = airship
 
     def get(self, push_id: str) -> common.IteratorDataObj:
         url = self.airship.urls.get("reports_url") + "responses/" + push_id
         response = self.airship.request(method="GET", body="", url=url, version=3)
         payload = response.json()
         return common.IteratorDataObj.from_payload(payload)
@@ -25,15 +26,15 @@
     """
 
     next_url: Optional[str] = None
     data_attribute: str = "pushes"
 
     def __init__(
         self,
-        airship: Airship,
+        airship: BaseClient,
         start_date: datetime,
         end_date: datetime,
         limit: Optional[str] = None,
         start_id: Optional[str] = None,
     ):
         if not airship or not start_date or not end_date:
             raise TypeError("airship, start_date, & end_date cannot be empty")
@@ -52,15 +53,15 @@
 
 
 class DevicesReport(object):
     """Returns a project's opted-in and installed device counts broken out by device
     type as a daily snapshot. This endpoint returns the same data that populates the
     Devices Report on the web dashboard."""
 
-    def __init__(self, airship: Airship):
+    def __init__(self, airship: BaseClient):
         self.airship = airship
 
     def get(self, date: datetime):
         if not date:
             raise TypeError("date cannot be empty")
         if not isinstance(date, datetime):
             raise ValueError("date must be a datetime object")
@@ -75,15 +76,19 @@
 class ReportsList(common.IteratorParent):
     """Parent class for reports"""
 
     next_url: Optional[str] = None
     data_attribute: Optional[str] = None
 
     def __init__(
-        self, airship: Airship, start_date: datetime, end_date: datetime, precision: str
+        self,
+        airship: BaseClient,
+        start_date: datetime,
+        end_date: datetime,
+        precision: str,
     ):
         if not airship or not start_date or not end_date or not precision:
             raise TypeError("None of the function parameters can be empty")
 
         if not isinstance(start_date, datetime) or not isinstance(end_date, datetime):
             raise TypeError("start_date and end_date must be datetime objects")
```

### Comparing `urbanairship-6.2.0/urbanairship.egg-info/PKG-INFO` & `urbanairship-6.3.0/urbanairship.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urbanairship
-Version: 6.2.0
+Version: 6.3.0
 Summary: Python package for using the Airship API
 Home-page: https://airship.com/
 Author: Airship Tools
 Author-email: tools@airship.com
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -90,14 +90,15 @@
     >>> push.notification = ua.notification(alert='Hello')
     >>> push.device_types = ua.device_types('web')
     >>> push.send()
 
 History
 =======
 
+* 6.3 Support for OAuth2 Authentication. Adds new clients module and class.
 * 6.0 Support for Bearer Token Authentication. Removes support for Python 2.
 * 5.0 Support for SMS and Email messages. See changelog for other updates.
 * 4.0 Support for Automation, removed Feedback
 * 3.0 Support for Open Channels, several other significant changes
 * 2.0 Support for Web Notify and more iOS 10, stopped supporting Python 2.6
 * 1.0 Support for In-App and iOS 10
 * 0.8 Support for Reports APIs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urbanairship Version: 6.2.0 Summary: Python package
+Metadata-Version: 2.1 Name: urbanairship Version: 6.3.0 Summary: Python package
 for using the Airship API Home-page: https://airship.com/ Author: Airship Tools
 Author-email: tools@airship.com License: BSD License Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries License-File: LICENSE
 License-File: AUTHORS Requires-Dist: requests>=1.2 Requires-Dist: six Requires-
@@ -36,15 +36,16 @@
 'Hello, message center user', ... '
 ************ HHeelllloo!! ************
 Goodbye.
 ') >>> push.send() Web Push to a tag ----------------- >>> import urbanairship
 as ua >>> airship = ua.Airship('application_key', 'master_secret') >>> push =
 airship.create_push() >>> push.audience = ua.tag('web_tag') >>>
 push.notification = ua.notification(alert='Hello') >>> push.device_types =
-ua.device_types('web') >>> push.send() History ======= * 6.0 Support for Bearer
+ua.device_types('web') >>> push.send() History ======= * 6.3 Support for OAuth2
+Authentication. Adds new clients module and class. * 6.0 Support for Bearer
 Token Authentication. Removes support for Python 2. * 5.0 Support for SMS and
 Email messages. See changelog for other updates. * 4.0 Support for Automation,
 removed Feedback * 3.0 Support for Open Channels, several other significant
 changes * 2.0 Support for Web Notify and more iOS 10, stopped supporting Python
 2.6 * 1.0 Support for In-App and iOS 10 * 0.8 Support for Reports APIs * 0.7
 Support for Python 3, major refactoring * 0.6 Major refactoring, support for
 push api v3 * 0.5 Added Android, Rich Push, and scheduled notifications * 0.4
```

### Comparing `urbanairship-6.2.0/urbanairship.egg-info/SOURCES.txt` & `urbanairship-6.3.0/urbanairship.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 urbanairship/__about__.py
 urbanairship/__init__.py
+urbanairship/client.py
 urbanairship/common.py
 urbanairship/core.py
 urbanairship/enums.py
+urbanairship/urls.py
 urbanairship.egg-info/PKG-INFO
 urbanairship.egg-info/SOURCES.txt
 urbanairship.egg-info/dependency_links.txt
 urbanairship.egg-info/requires.txt
 urbanairship.egg-info/top_level.txt
 urbanairship/automation/__init__.py
 urbanairship/automation/core.py
```

