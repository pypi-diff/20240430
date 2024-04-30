# Comparing `tmp/willisapi_client-1.6.tar.gz` & `tmp/willisapi_client-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "willisapi_client-1.6.tar", last modified: Mon Mar 11 14:25:23 2024, max compression
+gzip compressed data, was "willisapi_client-1.7.tar", last modified: Tue Apr 30 19:46:02 2024, max compression
```

## Comparing `willisapi_client-1.6.tar` & `willisapi_client-1.7.tar`

### file list

```diff
@@ -1,49 +1,46 @@
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-11 14:25:23.043755 willisapi_client-1.6/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     8599 2024-03-11 14:24:26.000000 willisapi_client-1.6/LICENSE
--rw-r--r--   0 vijayyadav   (501) staff       (20)       44 2024-03-11 14:24:26.000000 willisapi_client-1.6/MANIFEST.in
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2150 2024-03-11 14:25:23.043823 willisapi_client-1.6/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1840 2024-03-11 14:24:26.000000 willisapi_client-1.6/README.md
--rw-r--r--   0 vijayyadav   (501) staff       (20)      254 2024-03-11 14:24:26.000000 willisapi_client-1.6/RELEASE.md
--rw-r--r--   0 vijayyadav   (501) staff       (20)      372 2024-03-11 14:24:26.000000 willisapi_client-1.6/requirements.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2024-03-11 14:25:23.044008 willisapi_client-1.6/setup.cfg
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1666 2024-03-11 14:24:26.000000 willisapi_client-1.6/setup.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-11 14:25:23.039728 willisapi_client-1.6/tests/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     4793 2024-03-11 14:24:26.000000 willisapi_client-1.6/tests/test_auth.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    21256 2024-03-11 14:24:26.000000 willisapi_client-1.6/tests/test_csv_validation.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2226 2024-03-11 14:24:26.000000 willisapi_client-1.6/tests/test_download.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5162 2024-03-11 14:24:26.000000 willisapi_client-1.6/tests/test_upload.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2648 2024-03-11 14:24:26.000000 willisapi_client-1.6/tests/test_user_permissions.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-11 14:25:23.040516 willisapi_client-1.6/willisapi_client/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      279 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      251 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/__version__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      107 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/logging_setup.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-11 14:25:23.041697 willisapi_client-1.6/willisapi_client/services/
--rw-r--r--   0 vijayyadav   (501) staff       (20)       40 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      264 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/api.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-11 14:25:23.042371 willisapi_client-1.6/willisapi_client/services/auth/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      326 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/auth/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1507 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/auth/account_manager.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     4880 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/auth/auth_utils.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1788 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/auth/login_manager.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1478 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/auth/permissions_manager.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-11 14:25:23.042782 willisapi_client-1.6/willisapi_client/services/download/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      147 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/download/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1952 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/download/download_handler.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     8974 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/download/download_utils.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      367 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/exceptions.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-11 14:25:23.043644 willisapi_client-1.6/willisapi_client/services/upload/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      149 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/upload/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    21962 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/upload/csv_validation.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1635 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/upload/language_choices.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2433 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/upload/multipart_upload_handler.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    14716 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/upload/upload_utils.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)       33 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/services/upload/utils.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      759 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/timer.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1448 2024-03-11 14:24:26.000000 willisapi_client-1.6/willisapi_client/willisapi_client.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-11 14:25:23.041285 willisapi_client-1.6/willisapi_client.egg-info/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2150 2024-03-11 14:25:23.000000 willisapi_client-1.6/willisapi_client.egg-info/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1402 2024-03-11 14:25:23.000000 willisapi_client-1.6/willisapi_client.egg-info/SOURCES.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-03-11 14:25:23.000000 willisapi_client-1.6/willisapi_client.egg-info/dependency_links.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-03-11 14:25:23.000000 willisapi_client-1.6/willisapi_client.egg-info/not-zip-safe
--rw-r--r--   0 vijayyadav   (501) staff       (20)      372 2024-03-11 14:25:23.000000 willisapi_client-1.6/willisapi_client.egg-info/requires.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       17 2024-03-11 14:25:23.000000 willisapi_client-1.6/willisapi_client.egg-info/top_level.txt
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-30 19:46:02.975886 willisapi_client-1.7/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     8599 2024-04-30 19:45:46.000000 willisapi_client-1.7/LICENSE
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       44 2024-04-30 19:45:46.000000 willisapi_client-1.7/MANIFEST.in
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2150 2024-04-30 19:46:02.975958 willisapi_client-1.7/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1840 2024-04-30 19:45:46.000000 willisapi_client-1.7/README.md
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      254 2024-04-30 19:45:46.000000 willisapi_client-1.7/RELEASE.md
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      372 2024-04-30 19:45:46.000000 willisapi_client-1.7/requirements.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2024-04-30 19:46:02.976158 willisapi_client-1.7/setup.cfg
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1666 2024-04-30 19:45:46.000000 willisapi_client-1.7/setup.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-30 19:46:02.971587 willisapi_client-1.7/tests/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2654 2024-04-30 19:45:46.000000 willisapi_client-1.7/tests/test_auth.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    21256 2024-04-30 19:45:46.000000 willisapi_client-1.7/tests/test_csv_validation.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2507 2024-04-30 19:45:46.000000 willisapi_client-1.7/tests/test_download.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5162 2024-04-30 19:45:46.000000 willisapi_client-1.7/tests/test_upload.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-30 19:46:02.972536 willisapi_client-1.7/willisapi_client/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      199 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      251 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/__version__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      107 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/logging_setup.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-30 19:46:02.973794 willisapi_client-1.7/willisapi_client/services/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       40 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      230 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/api.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-30 19:46:02.974322 willisapi_client-1.7/willisapi_client/services/auth/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      134 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/auth/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1670 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/auth/auth_utils.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1788 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/auth/login_manager.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-30 19:46:02.974746 willisapi_client-1.7/willisapi_client/services/download/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      147 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/download/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2036 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/download/download_handler.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     9690 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/download/download_utils.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      367 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/exceptions.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-30 19:46:02.975763 willisapi_client-1.7/willisapi_client/services/upload/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      149 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/upload/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    21962 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/upload/csv_validation.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1635 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/upload/language_choices.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2433 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/upload/multipart_upload_handler.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    14716 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/upload/upload_utils.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       33 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/services/upload/utils.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      759 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/timer.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1101 2024-04-30 19:45:46.000000 willisapi_client-1.7/willisapi_client/willisapi_client.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-30 19:46:02.973294 willisapi_client-1.7/willisapi_client.egg-info/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2150 2024-04-30 19:46:02.000000 willisapi_client-1.7/willisapi_client.egg-info/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1267 2024-04-30 19:46:02.000000 willisapi_client-1.7/willisapi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-30 19:46:02.000000 willisapi_client-1.7/willisapi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-30 19:46:02.000000 willisapi_client-1.7/willisapi_client.egg-info/not-zip-safe
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      372 2024-04-30 19:46:02.000000 willisapi_client-1.7/willisapi_client.egg-info/requires.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       17 2024-04-30 19:46:02.000000 willisapi_client-1.7/willisapi_client.egg-info/top_level.txt
```

### Comparing `willisapi_client-1.6/LICENSE` & `willisapi_client-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/PKG-INFO` & `willisapi_client-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: willisapi_client
-Version: 1.6
+Version: 1.7
 Summary: A Python client for willisapi
 Home-page: https://github.com/bklynhlth/willsiapi_client
 Author: bklynhlth
 Author-email: admin@brooklyn.health
 License: Apache
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `willisapi_client-1.6/README.md` & `willisapi_client-1.7/README.md`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/setup.py` & `willisapi_client-1.7/setup.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/tests/test_csv_validation.py` & `willisapi_client-1.7/tests/test_csv_validation.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/tests/test_download.py` & `willisapi_client-1.7/tests/test_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,29 @@
         data = download(self.key, self.project_name)
         assert data.empty == True
 
     @patch("willisapi_client.services.download.download_utils.DownloadUtils.request")
     def test_download_no_items_from_api(self, mocked_data):
         mocked_data.return_value = {
             "status_code": 200,
-            "items": {},
+            "presigned_url": None,
         }
         data = download(self.key, self.project_name)
         assert data.empty == True
 
     @patch("willisapi_client.services.download.download_utils.DownloadUtils.request")
-    def test_download_success(self, mocked_data):
+    @patch(
+        "willisapi_client.services.download.download_utils.DownloadUtils.get_data_from_presigned_url"
+    )
+    def test_download_success(self, mocked_data, mocked_response):
         with open("tests/test.json") as json_file:
             data = json.load(json_file)
         mocked_data.return_value = data
+        mocked_response.return_value = {
+            "status_code": 200,
+            "presigned_url": "https://google.com",
+        }
         data = download(self.key, self.project_name)
         assert data.empty == False
         assert data.filename.tolist()[0] == "test_video.mp4"
         assert data.pt_id_external.tolist()[0] == "pt_id_external"
         assert len(data.index) == 1
```

### Comparing `willisapi_client-1.6/tests/test_upload.py` & `willisapi_client-1.7/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/willisapi_client/services/auth/account_manager.py` & `willisapi_client-1.7/willisapi_client/services/download/download_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # website:   https://www.brooklyn.health
 from http import HTTPStatus
+import pandas as pd
+from datetime import datetime
 
 from willisapi_client.willisapi_client import WillisapiClient
-from willisapi_client.services.auth.auth_utils import AuthUtils
+from willisapi_client.services.download.download_utils import DownloadUtils
 from willisapi_client.logging_setup import logger as logger
-
-from datetime import datetime
+from willisapi_client.timer import measure
 
 
-def account_create(
-    key: str,
-    account: str,
-    **kwargs,
-) -> str:
+@measure
+def download(key: str, project_name: str, **kwargs):
     """
     ---------------------------------------------------------------------------------------------------
-    Function: account_create
+    Function: download
 
-    Description: This function to creates account in RDS and AWS Cognito using willis account create API
+    Description: This function to download data using willis download API from secure database
 
     Parameters:
     ----------
-    key: Admin access token
-    account: Client Name
+    key: AWS access id token (str)
+    project_name: name of the project (str)
 
     Returns:
     ----------
-    None
+    measures: A pandas dataframe
     ---------------------------------------------------------------------------------------------------
     """
+
     wc = WillisapiClient(env=kwargs.get("env"))
-    url = wc.get_account_create_url()
+    url = wc.get_download_url() + f"?project_name={project_name}"
     headers = wc.get_headers()
     headers["Authorization"] = key
-    data = dict(
-        account=account.lower(),
-    )
-    logger.info(f'{datetime.now().strftime("%H:%M:%S")}: Creating account')
-    response = AuthUtils.account_create(url, data, headers, try_number=1)
-    if response and "status_code" in response:
+    logger.info(f'{datetime.now().strftime("%H:%M:%S")}: Download started')
+    logger.info(f'{datetime.now().strftime("%H:%M:%S")}: Download is in progress')
+    response = DownloadUtils.request(url, headers, try_number=1)
+    empty_response_df = pd.DataFrame()
+    if "status_code" in response:
+        if response["status_code"] == HTTPStatus.FORBIDDEN:
+            logger.error("Invalid key")
+        if response["status_code"] == HTTPStatus.UNAUTHORIZED:
+            logger.error("No access to project/data for download.")
         if response["status_code"] == HTTPStatus.OK:
-            logger.info(response["message"])
-        else:
-            logger.error(response["message"])
-        return response["message"]
-    else:
-        logger.error(f"Failed")
-        return None
+            logger.info(f'{datetime.now().strftime("%H:%M:%S")}: Download Complete')
+            data = DownloadUtils.get_data_from_presigned_url(response["presigned_url"])
+            response_df, err = DownloadUtils.generate_response_df(data)
+            if not err:
+                return response_df
+    return empty_response_df
```

### Comparing `willisapi_client-1.6/willisapi_client/services/auth/login_manager.py` & `willisapi_client-1.7/willisapi_client/services/auth/login_manager.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/willisapi_client/services/download/download_utils.py` & `willisapi_client-1.7/willisapi_client/services/download/download_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import requests
 import json
 import time
 import random
 import pandas as pd
 from typing import Tuple
+from http import HTTPStatus
+
 
 vocal_acoustic_summary = "vocal_acoustics_summary"
 speech_characteristics_summary = "speech_characteristics_summary"
 rater_qa_summary = "rater_qa_summary"
 
 
 class DownloadUtils:
@@ -60,16 +62,16 @@
 
         Returns:
         ----------
         (project_name, pt_count): Name of the project and number of participants of the project (str, int)
         ------------------------------------------------------------------------------------------------------
         """
         return (
-            response["items"]["project"]["project_name"],
-            len(response["items"]["project"]["participant"]),
+            response["project"]["project_name"],
+            len(response["project"]["participant"]),
         )
 
     def _get_pt_id_ext_and_num_records(response, pt):
         """
         ------------------------------------------------------------------------------------------------------
         Class: DownloadUtils
 
@@ -84,16 +86,16 @@
 
         Returns:
         ----------
         (pt_id, record_count): Id of the participant and number of records of the participant (str, int)
         ------------------------------------------------------------------------------------------------------
         """
         return (
-            response["items"]["project"]["participant"][pt]["participant_Id"],
-            len(response["items"]["project"]["participant"][pt]["results"]),
+            response["project"]["participant"][pt]["participant_Id"],
+            len(response["project"]["participant"][pt]["results"]),
         )
 
     def _get_filename_and_timestamp(response, pt, rec):
         """
         ------------------------------------------------------------------------------------------------------
         Class: DownloadUtils
 
@@ -109,20 +111,16 @@
 
         Returns:
         ----------
         (filename, timestamp): filename and timestamp of the record (str, str)
         ------------------------------------------------------------------------------------------------------
         """
         return (
-            response["items"]["project"]["participant"][pt]["results"][rec][
-                "file_name"
-            ],
-            response["items"]["project"]["participant"][pt]["results"][rec][
-                "timestamp"
-            ],
+            response["project"]["participant"][pt]["results"][rec]["file_name"],
+            response["project"]["participant"][pt]["results"][rec]["timestamp"],
         )
 
     def _get_defined_columns():
         """
         ------------------------------------------------------------------------------------------------------
         Class: DownloadUtils
 
@@ -154,15 +152,15 @@
         workflow_tag: Workflow Tag
 
         Returns:
         ----------
         df: A pandas dataframe of specific workflow tag
         ------------------------------------------------------------------------------------------------------
         """
-        measures_dict = response["items"]["project"]["participant"][pt]["results"][rec][
+        measures_dict = response["project"]["participant"][pt]["results"][rec][
             "measures"
         ]
         if (
             workflow_tag in measures_dict
             and measures_dict[workflow_tag]
             and workflow_tag
             in [
@@ -170,65 +168,93 @@
                 speech_characteristics_summary,
                 rater_qa_summary,
             ]
         ):
             return pd.read_json(json.dumps(measures_dict[workflow_tag][0]))
         return pd.DataFrame()
 
-    def generate_response_df(response) -> Tuple[pd.DataFrame, str]:
+    def get_data_from_presigned_url(url: str):
+        """
+        ------------------------------------------------------------------------------------------------------
+        Class: DownloadUtils
+
+        Function: get_data_from_presigned_url
+
+        Description: This function downloads the json data using S3 preisgned URL
+
+        Parameters:
+        ----------
+        response: S3 Presigned URL
+
+        Returns:
+        ----------
+        (data, error): Generates response data and error message
+        ------------------------------------------------------------------------------------------------------
+        """
+        response = {}
+        try:
+            data = requests.get(url)
+            if data.status_code == HTTPStatus.OK:
+                response = data.json()
+        except Exception:
+            pass
+
+        return response
+
+    def generate_response_df(data) -> Tuple[pd.DataFrame, str]:
         """
         ------------------------------------------------------------------------------------------------------
         Class: DownloadUtils
 
         Function: generate_response_df
 
         Description: This function converts the json data to dataframe
 
         Parameters:
         ----------
-        response: The JSON response from the API server.
+        data: The JSON data from the API server.
 
         Returns:
         ----------
         (dataframe, error): Generates response dataframe and error message
         ------------------------------------------------------------------------------------------------------
         """
         response_df = pd.DataFrame()
         try:
-            if not response["items"]:
+            if not data:
                 return response_df, "No Data Found"
             (project_name, num_pts) = DownloadUtils._get_project_name_and_pts_count(
-                response
+                data
             )
             for pt in range(0, num_pts):
                 (pt_id_ext, num_records) = DownloadUtils._get_pt_id_ext_and_num_records(
-                    response, pt
+                    data, pt
                 )
                 for rec in range(0, num_records):
                     (
                         filename,
                         time_collected,
-                    ) = DownloadUtils._get_filename_and_timestamp(response, pt, rec)
+                    ) = DownloadUtils._get_filename_and_timestamp(data, pt, rec)
                     main_df = pd.DataFrame(
                         [[project_name, pt_id_ext, filename, time_collected]],
                         columns=DownloadUtils._get_defined_columns(),
                     )
 
                     vocal_acoustics_summary_df = (
                         DownloadUtils._get_summary_df_from_json(
-                            response, pt, rec, vocal_acoustic_summary
+                            data, pt, rec, vocal_acoustic_summary
                         )
                     )
                     speech_characteristics_summary_df = (
                         DownloadUtils._get_summary_df_from_json(
-                            response, pt, rec, speech_characteristics_summary
+                            data, pt, rec, speech_characteristics_summary
                         )
                     )
                     rater_qa_summary_df = DownloadUtils._get_summary_df_from_json(
-                        response, pt, rec, rater_qa_summary
+                        data, pt, rec, rater_qa_summary
                     )
                     df = pd.concat(
                         [
                             main_df,
                             vocal_acoustics_summary_df,
                             speech_characteristics_summary_df,
                             rater_qa_summary_df,
```

### Comparing `willisapi_client-1.6/willisapi_client/services/upload/csv_validation.py` & `willisapi_client-1.7/willisapi_client/services/upload/csv_validation.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/willisapi_client/services/upload/language_choices.py` & `willisapi_client-1.7/willisapi_client/services/upload/language_choices.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/willisapi_client/services/upload/multipart_upload_handler.py` & `willisapi_client-1.7/willisapi_client/services/upload/multipart_upload_handler.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/willisapi_client/services/upload/upload_utils.py` & `willisapi_client-1.7/willisapi_client/services/upload/upload_utils.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/willisapi_client/timer.py` & `willisapi_client-1.7/willisapi_client/timer.py`

 * *Files identical despite different names*

### Comparing `willisapi_client-1.6/willisapi_client.egg-info/PKG-INFO` & `willisapi_client-1.7/willisapi_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: willisapi-client
-Version: 1.6
+Version: 1.7
 Summary: A Python client for willisapi
 Home-page: https://github.com/bklynhlth/willsiapi_client
 Author: bklynhlth
 Author-email: admin@brooklyn.health
 License: Apache
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `willisapi_client-1.6/willisapi_client.egg-info/SOURCES.txt` & `willisapi_client-1.7/willisapi_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 requirements.txt
 setup.cfg
 setup.py
 tests/test_auth.py
 tests/test_csv_validation.py
 tests/test_download.py
 tests/test_upload.py
-tests/test_user_permissions.py
 willisapi_client/__init__.py
 willisapi_client/__version__.py
 willisapi_client/logging_setup.py
 willisapi_client/timer.py
 willisapi_client/willisapi_client.py
 willisapi_client.egg-info/PKG-INFO
 willisapi_client.egg-info/SOURCES.txt
@@ -21,18 +20,16 @@
 willisapi_client.egg-info/not-zip-safe
 willisapi_client.egg-info/requires.txt
 willisapi_client.egg-info/top_level.txt
 willisapi_client/services/__init__.py
 willisapi_client/services/api.py
 willisapi_client/services/exceptions.py
 willisapi_client/services/auth/__init__.py
-willisapi_client/services/auth/account_manager.py
 willisapi_client/services/auth/auth_utils.py
 willisapi_client/services/auth/login_manager.py
-willisapi_client/services/auth/permissions_manager.py
 willisapi_client/services/download/__init__.py
 willisapi_client/services/download/download_handler.py
 willisapi_client/services/download/download_utils.py
 willisapi_client/services/upload/__init__.py
 willisapi_client/services/upload/csv_validation.py
 willisapi_client/services/upload/language_choices.py
 willisapi_client/services/upload/multipart_upload_handler.py
```

