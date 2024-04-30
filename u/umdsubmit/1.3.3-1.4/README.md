# Comparing `tmp/umdsubmit-1.3.3.tar.gz` & `tmp/umdsubmit-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umdsubmit-1.3.3.tar", max compression
+gzip compressed data, was "umdsubmit-1.4.tar", max compression
```

## Comparing `umdsubmit-1.3.3.tar` & `umdsubmit-1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2023-12-05 22:24:37.275405 umdsubmit-1.3.3/LICENSE
--rw-r--r--   0        0        0     1800 2023-12-20 21:11:51.853169 umdsubmit-1.3.3/README.md
--rw-r--r--   0        0        0      448 2024-04-07 18:49:47.316111 umdsubmit-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     3885 2024-04-07 18:48:47.172251 umdsubmit-1.3.3/src/umdsubmit/submit.py
--rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 umdsubmit-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-12-05 22:24:37.275405 umdsubmit-1.4/LICENSE
+-rw-r--r--   0        0        0     1800 2023-12-20 21:11:51.853169 umdsubmit-1.4/README.md
+-rw-r--r--   0        0        0      446 2024-04-30 04:11:34.556571 umdsubmit-1.4/pyproject.toml
+-rw-r--r--   0        0        0     3911 2024-04-30 04:11:19.818849 umdsubmit-1.4/src/umdsubmit/submit.py
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 umdsubmit-1.4/PKG-INFO
```

### Comparing `umdsubmit-1.3.3/LICENSE` & `umdsubmit-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `umdsubmit-1.3.3/README.md` & `umdsubmit-1.4/README.md`

 * *Files identical despite different names*

### Comparing `umdsubmit-1.3.3/src/umdsubmit/submit.py` & `umdsubmit-1.4/src/umdsubmit/submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
                     zip_writer.writestr(file_path, f.read())
 
 def auth():
     """
     Authenticates the user by prompting for UMD Directory ID and password,
     and saves the authentication response to the .submitUser file.
     """
+    os.remove(".submitUser") if os.path.exists(".submitUser") else None
     print("Enter UMD Directory ID: ")
     username = input()
     password = getpass.getpass("Enter UMD Password: ")
     data = {"loginName" : username, "password" : password, "courseKey" : get_info("courseKey"), "projectNumber" : get_info("projectNumber")}
     url_part = f"/eclipse/NegotiateOneTimePassword"
     response = requests.post(get_info("baseURL") + url_part, data = data)
     f = open(".submitUser", "x")
@@ -96,18 +97,17 @@
     print(response.text)
 
 def main():
     """
     Main function that creates a zip archive of the current directory,
     submits the archive to a specified URL, and prints the response.
     """
-    if not os.path.isfile('.submitUser'):
-        auth()
+    auth()
     shutil.make_archive('submit', 'zip', os.getcwd())
     submit_zip_object =  open('submit.zip', 'rb')
     files = {"submittedFiles": ("submit.zip", submit_zip_object)}
     data = {"courseName" : get_info("courseName"), "projectNumber" : get_info("projectNumber"), "semester" : get_info("semester"), "courseKey" : get_info("courseKey"), "authentication.type" : get_info("authentication.type"), "baseURL" : get_info("baseURL"), "submitURL" : get_info("submitURL"), "cvsAccount" : get_cvs_account(), "oneTimePassword" : get_one_time_password(), "submitClientTool" : "umdsubmit", "submitClientVersion" : "1.0"}
     response = requests.post(get_info("submitURL"), files = files, data = data)
-    if response.status_code == 401:
+    if response.status_code != 200:
         auth()
         main()
     print(response.text)
```

### Comparing `umdsubmit-1.3.3/PKG-INFO` & `umdsubmit-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umdsubmit
-Version: 1.3.3
+Version: 1.4
 Summary: Allows submitting to the UMD Submit Server from the command line, without the Eclipse Plugin
 Author: Nico Carbone
 Author-email: carbone.nicolas0@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

