# Comparing `tmp/selenium2-0.0.1.tar.gz` & `tmp/selenium2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium2-0.0.1.tar", last modified: Tue Apr 30 04:03:13 2024, max compression
+gzip compressed data, was "selenium2-0.0.2.tar", last modified: Tue Apr 30 04:40:25 2024, max compression
```

## Comparing `selenium2-0.0.1.tar` & `selenium2-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 04:03:13.946834 selenium2-0.0.1/
--rw-rw-rw-   0        0        0    11556 2024-04-30 03:56:52.000000 selenium2-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    12424 2024-04-30 04:03:13.945834 selenium2-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11740 2024-04-30 03:45:18.000000 selenium2-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-30 04:03:13.930833 selenium2-0.0.1/browser_support/
--rw-rw-rw-   0        0        0        0 2021-04-20 15:35:46.000000 selenium2-0.0.1/browser_support/__init__.py
--rw-rw-rw-   0        0        0    10232 2024-04-30 02:43:13.000000 selenium2-0.0.1/browser_support/_base.py
--rw-rw-rw-   0        0        0      859 2024-04-30 02:43:18.000000 selenium2-0.0.1/browser_support/_driver.py
--rw-rw-rw-   0        0        0     8141 2024-04-30 02:43:52.000000 selenium2-0.0.1/browser_support/_webdrivercreator.py
--rw-rw-rw-   0        0        0     3975 2024-04-30 02:44:04.000000 selenium2-0.0.1/browser_support/alert.py
--rw-rw-rw-   0        0        0     1596 2024-04-30 02:45:02.000000 selenium2-0.0.1/browser_support/browsermanagement.py
--rw-rw-rw-   0        0        0     6365 2024-04-30 02:45:18.000000 selenium2-0.0.1/browser_support/cookies.py
--rw-rw-rw-   0        0        0    18255 2024-04-30 02:45:32.000000 selenium2-0.0.1/browser_support/element.py
--rw-rw-rw-   0        0        0     2500 2024-04-30 02:45:41.000000 selenium2-0.0.1/browser_support/frames.py
--rw-rw-rw-   0        0        0     5395 2024-04-30 03:37:40.000000 selenium2-0.0.1/browser_support/javascript.py
--rw-rw-rw-   0        0        0     4801 2024-04-30 02:42:39.000000 selenium2-0.0.1/browser_support/screenshot.py
--rw-rw-rw-   0        0        0    10519 2024-04-30 03:38:51.000000 selenium2-0.0.1/browser_support/selects.py
--rw-rw-rw-   0        0        0     5933 2024-04-30 03:39:02.000000 selenium2-0.0.1/browser_support/tables.py
--rw-rw-rw-   0        0        0    10727 2024-04-30 03:42:11.000000 selenium2-0.0.1/browser_support/waiting.py
--rw-rw-rw-   0        0        0    14498 2024-04-30 03:42:11.000000 selenium2-0.0.1/browser_support/windowmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-30 04:03:13.934834 selenium2-0.0.1/config/
--rw-rw-rw-   0        0        0      106 2021-12-20 23:07:52.000000 selenium2-0.0.1/config/__init__.py
--rw-rw-rw-   0        0        0      505 2024-04-30 00:42:31.000000 selenium2-0.0.1/config/config.py
--rw-rw-rw-   0        0        0       44 2021-12-20 23:06:56.000000 selenium2-0.0.1/config/config_production.py
-drwxrwxrwx   0        0        0        0 2024-04-30 04:03:13.944834 selenium2-0.0.1/selenium2.egg-info/
--rw-rw-rw-   0        0        0    12424 2024-04-30 04:03:13.000000 selenium2-0.0.1/selenium2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1375 2024-04-30 04:03:13.000000 selenium2-0.0.1/selenium2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 04:03:13.000000 selenium2-0.0.1/selenium2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-30 04:03:13.000000 selenium2-0.0.1/selenium2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-04-30 04:03:13.000000 selenium2-0.0.1/selenium2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 04:03:13.946834 selenium2-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1109 2024-04-30 04:02:41.000000 selenium2-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 04:03:13.942837 selenium2-0.0.1/site_specific/
--rw-rw-rw-   0        0        0       94 2024-04-30 00:27:04.000000 selenium2-0.0.1/site_specific/__init__.py
--rw-rw-rw-   0        0        0     2609 2024-04-30 00:40:12.000000 selenium2-0.0.1/site_specific/default.py
--rw-rw-rw-   0        0        0    35186 2024-04-30 00:30:26.000000 selenium2-0.0.1/site_specific/kijiji.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:40:25.379632 selenium2-0.0.2/
+-rw-rw-rw-   0        0        0    11556 2024-04-30 03:56:52.000000 selenium2-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    15798 2024-04-30 04:40:25.378631 selenium2-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12942 2024-04-30 04:35:17.000000 selenium2-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-30 04:40:25.377631 selenium2-0.0.2/selenium2.egg-info/
+-rw-rw-rw-   0        0        0    15798 2024-04-30 04:40:25.000000 selenium2-0.0.2/selenium2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-04-30 04:40:25.000000 selenium2-0.0.2/selenium2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 04:40:25.000000 selenium2-0.0.2/selenium2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-30 04:40:25.000000 selenium2-0.0.2/selenium2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 04:40:25.000000 selenium2-0.0.2/selenium2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 04:40:25.379632 selenium2-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-04-30 04:39:54.000000 selenium2-0.0.2/setup.py
```

### Comparing `selenium2-0.0.1/LICENSE` & `selenium2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium2-0.0.1/PKG-INFO` & `selenium2-0.0.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: selenium2
-Version: 0.0.1
-Summary: A comprehensive Selenium wrapper designed to simplify browser automation and testing tasks.
-Home-page: https://github.com/loudpumpkins/gsuite-meld
-Author: Alexei Panov
-Author-email: alexei_panov@hotmail.com
-License: MIT
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: selenium==4.2.0
-Provides-Extra: dev
-Requires-Dist: pytest>=7.0; extra == "dev"
-Requires-Dist: twine>=4.0.2; extra == "dev"
-
 Selenium 2
 ============
 
 Extends the python's selenium library by providing easy-to-use methods at the
 cost of customizability. Provides site-specific methods such as login/logout
 for quick browser automation.
 
@@ -252,17 +233,55 @@
     def delete_content(self, details: dict) -> bool: ...
     def edit_content(self, details: dict) -> bool: ...
     def is_signed_in(self) -> bool: ...
     def is_signed_out(self) -> bool: ...
     def sign_in(self, details: dict, cookies: str = None) -> NoReturn: ...
     def sign_out(self) -> NoReturn: ...
 
+Environment Variables
+---------------------
+
+The following environment variables can be set to configure various aspects of the Selenium2 behavior:
+
+``DEBUG``
+    Controls the debug output of the Selenium2 wrapper. Set to ``True`` to enable verbose logging.
+    Default is ``False``.
+
+    .. code-block:: bash
+
+        export SELENIUM2_DEBUG=True
+
+``SELENIUM2_DEFAULT_TIMEOUT``
+    Specifies the default timeout in seconds for explicit waits.
+    Default is 15 seconds.
+
+    .. code-block:: bash
+
+        export SELENIUM2_DEFAULT_TIMEOUT=30
+
+``SELENIUM2_SCREENSHOT_PATH``
+    Sets the directory where screenshots will be saved.
+    Default is 'screenshots'.
+
+    .. code-block:: bash
+
+        export SELENIUM2_SCREENSHOT_PATH='/path/to/screenshots'
+
+``SELENIUM2_COOKIES_PATH``
+    Defines the directory for storing browser cookies.
+    Default is 'cookies'.
+
+    .. code-block:: bash
+
+        export SELENIUM2_COOKIES_PATH='/path/to/cookies'
+
+These environment variables allow you to customize the behavior of the Selenium2 wrapper without changing the code. They are particularly useful for adapting the wrapper to different testing environments or requirements.
 
 Contributing
 ------------
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 License
 -------
 
-Apache 2.0
+Apache 2.0
```

### Comparing `selenium2-0.0.1/setup.py` & `selenium2-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import find_packages, setup
 
 # pip install wheel, twine
 # pip install .
 
 # python setup.py bdist_wheel sdist
 # twine check dist/*
-# twine twine upload -r testpypi dist/*
 # twine upload dist/*
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setup(
     name="selenium2",
-    version="0.0.1",
+    version="0.0.2",
     description='A comprehensive Selenium wrapper designed to simplify browser automation and testing tasks.',
     package_dir={"": "."},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    url="https://github.com/loudpumpkins/gsuite-meld",
+    url="https://github.com/loudpumpkins/selenium2",
     author="Alexei Panov",
     author_email="alexei_panov@hotmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
```

