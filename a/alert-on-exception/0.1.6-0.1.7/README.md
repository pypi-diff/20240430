# Comparing `tmp/alert_on_exception-0.1.6.tar.gz` & `tmp/alert_on_exception-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alert_on_exception-0.1.6.tar", last modified: Thu Apr 25 05:33:23 2024, max compression
+gzip compressed data, was "alert_on_exception-0.1.7.tar", last modified: Tue Apr 30 11:02:02 2024, max compression
```

## Comparing `alert_on_exception-0.1.6.tar` & `alert_on_exception-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-25 05:33:23.450780 alert_on_exception-0.1.6/
--rw-rw-r--   0 user1     (1001) user1     (1001)     1112 2024-04-24 09:35:45.000000 alert_on_exception-0.1.6/LICENSE
--rw-r--r--   0 user1     (1001) user1     (1001)     1018 2024-04-25 05:33:23.450780 alert_on_exception-0.1.6/PKG-INFO
--rw-rw-r--   0 user1     (1001) user1     (1001)      811 2024-04-25 05:33:17.000000 alert_on_exception-0.1.6/README.md
--rw-rw-r--   0 user1     (1001) user1     (1001)       90 2024-04-24 09:33:49.000000 alert_on_exception-0.1.6/pyproject.toml
--rw-rw-r--   0 user1     (1001) user1     (1001)       38 2024-04-25 05:33:23.450780 alert_on_exception-0.1.6/setup.cfg
--rw-rw-r--   0 user1     (1001) user1     (1001)      684 2024-04-25 05:32:39.000000 alert_on_exception-0.1.6/setup.py
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-25 05:33:23.446803 alert_on_exception-0.1.6/src/
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-25 05:33:23.450780 alert_on_exception-0.1.6/src/alert_on_exception/
--rw-rw-r--   0 user1     (1001) user1     (1001)       36 2024-04-24 11:06:15.000000 alert_on_exception-0.1.6/src/alert_on_exception/__init__.py
--rw-rw-r--   0 user1     (1001) user1     (1001)     1156 2024-04-25 05:31:57.000000 alert_on_exception-0.1.6/src/alert_on_exception/alert.py
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-25 05:33:23.450780 alert_on_exception-0.1.6/src/alert_on_exception.egg-info/
--rw-r--r--   0 user1     (1001) user1     (1001)     1018 2024-04-25 05:33:23.000000 alert_on_exception-0.1.6/src/alert_on_exception.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1001) user1     (1001)      292 2024-04-25 05:33:23.000000 alert_on_exception-0.1.6/src/alert_on_exception.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-25 05:33:23.000000 alert_on_exception-0.1.6/src/alert_on_exception.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)       19 2024-04-25 05:33:23.000000 alert_on_exception-0.1.6/src/alert_on_exception.egg-info/top_level.txt
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-30 11:02:02.090093 alert_on_exception-0.1.7/
+-rw-rw-r--   0 user1     (1001) user1     (1001)     1112 2024-04-24 09:35:45.000000 alert_on_exception-0.1.7/LICENSE
+-rw-r--r--   0 user1     (1001) user1     (1001)     1018 2024-04-30 11:02:02.090093 alert_on_exception-0.1.7/PKG-INFO
+-rw-rw-r--   0 user1     (1001) user1     (1001)      811 2024-04-25 05:33:17.000000 alert_on_exception-0.1.7/README.md
+-rw-rw-r--   0 user1     (1001) user1     (1001)       90 2024-04-24 09:33:49.000000 alert_on_exception-0.1.7/pyproject.toml
+-rw-rw-r--   0 user1     (1001) user1     (1001)       38 2024-04-30 11:02:02.090093 alert_on_exception-0.1.7/setup.cfg
+-rw-rw-r--   0 user1     (1001) user1     (1001)      684 2024-04-30 11:01:54.000000 alert_on_exception-0.1.7/setup.py
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-30 11:02:02.086093 alert_on_exception-0.1.7/src/
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-30 11:02:02.090093 alert_on_exception-0.1.7/src/alert_on_exception/
+-rw-rw-r--   0 user1     (1001) user1     (1001)       36 2024-04-24 11:06:15.000000 alert_on_exception-0.1.7/src/alert_on_exception/__init__.py
+-rw-rw-r--   0 user1     (1001) user1     (1001)     1110 2024-04-30 11:01:42.000000 alert_on_exception-0.1.7/src/alert_on_exception/alert.py
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-30 11:02:02.090093 alert_on_exception-0.1.7/src/alert_on_exception.egg-info/
+-rw-r--r--   0 user1     (1001) user1     (1001)     1018 2024-04-30 11:02:01.000000 alert_on_exception-0.1.7/src/alert_on_exception.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1001) user1     (1001)      292 2024-04-30 11:02:02.000000 alert_on_exception-0.1.7/src/alert_on_exception.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-30 11:02:01.000000 alert_on_exception-0.1.7/src/alert_on_exception.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)       19 2024-04-30 11:02:01.000000 alert_on_exception-0.1.7/src/alert_on_exception.egg-info/top_level.txt
```

### Comparing `alert_on_exception-0.1.6/LICENSE` & `alert_on_exception-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alert_on_exception-0.1.6/PKG-INFO` & `alert_on_exception-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alert_on_exception
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package to alert users about exceptions.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Alert On Exception
```

### Comparing `alert_on_exception-0.1.6/README.md` & `alert_on_exception-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `alert_on_exception-0.1.6/setup.py` & `alert_on_exception-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name="alert_on_exception",
-    version="0.1.6",
+    version="0.1.7",
     package_dir={"": "src"},  # This line is added
     packages=find_packages(where="src"),  # And this line is modified
     install_requires=[],
     python_requires=">=3.6",
     description="A Python package to alert users about exceptions.",  # Short, concise description
     long_description=long_description,  # Detailed description
     long_description_content_type="text/markdown",  # Content type for long description, assuming it's in Markdown
```

### Comparing `alert_on_exception-0.1.6/src/alert_on_exception/alert.py` & `alert_on_exception-0.1.7/src/alert_on_exception/alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import os
 import smtplib
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 
-from dotenv import load_dotenv
-
 # Load environment variables from .env file
-load_dotenv()
 
 
 class AlertOnException:
     """
     receiver_mail: Provide the mail of a receiver to send mail.
     subject: Provide subject to show on the mail
     message: Provide the message body for the mail.
```

### Comparing `alert_on_exception-0.1.6/src/alert_on_exception.egg-info/PKG-INFO` & `alert_on_exception-0.1.7/src/alert_on_exception.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alert_on_exception
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package to alert users about exceptions.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Alert On Exception
```

