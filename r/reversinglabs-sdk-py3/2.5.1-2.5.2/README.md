# Comparing `tmp/reversinglabs-sdk-py3-2.5.1.tar.gz` & `tmp/reversinglabs_sdk_py3-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reversinglabs-sdk-py3-2.5.1.tar", last modified: Tue Apr  2 15:20:20 2024, max compression
+gzip compressed data, was "reversinglabs_sdk_py3-2.5.2.tar", last modified: Tue Apr 30 15:51:38 2024, max compression
```

## Comparing `reversinglabs-sdk-py3-2.5.1.tar` & `reversinglabs_sdk_py3-2.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    47425 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    46067 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.620092 reversinglabs-sdk-py3-2.5.1/ReversingLabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95910 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)    19593 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/clouddeepscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)   250836 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/tiscale.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47425 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/tests/test_a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/tests/test_ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/tests/test_tiscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    47537 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    46179 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.634877 reversinglabs_sdk_py3-2.5.2/ReversingLabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.634877 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96422 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19593 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/clouddeepscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250836 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/tiscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47537 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/tests/test_a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/tests/test_ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/tests/test_tiscale.py
```

### Comparing `reversinglabs-sdk-py3-2.5.1/CHANGELOG.md` & `reversinglabs_sdk_py3-2.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -229,8 +229,16 @@
   - `md5` and `sha256` can now be used in `DynamicAnalysis.get_dynamic_analysis_results` for fetching sample analysis results.
 
 
 v2.5.1 (2024-04-02)
 -------------------
 
 #### Improvements
-- Updated the README with an example of error handling.
+- Updated the README with an example of error handling.
+
+
+2.5.2 (2024-04-30)
+-------------------
+
+#### Improvements
+- **a1000** module:
+  - The function for checking file analysis status is now public. It is called `file_analysis_status`.
```

### Comparing `reversinglabs-sdk-py3-2.5.1/LICENSE` & `reversinglabs_sdk_py3-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/PKG-INFO` & `reversinglabs_sdk_py3-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.1
+Version: 2.5.2
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -79,14 +79,16 @@
 - `upload_sample_from_file`
     - Accepts a file open in 'rb' mode and returns a response containing the analysis task ID
 - `upload_sample_from_url`
     - Accepts a url and returns a response containing the analysis task ID
 - `check_submitted_url_status`
     - Accepts a task id returned by upload_sample_from_url and returns a response containing processing status and 
         report if the report is ready
+- `file_analysis_status`
+    - Accepts a list of file hashes and returns their analysis completion information.
 - `get_submitted_url_report`
     - Accepts a task ID returned by upload_sample_from_url and returns a response
     - This method utilizes the set number of retries and wait time in seconds to time
         out if the analysis results are not ready
 - `upload_sample_from_url_and_get_report`
     - Accepts a url and returns a response containing the analysis report
     - The result fetching action of this method utilizes the set number of retries and wait time in seconds to time
```

### Comparing `reversinglabs-sdk-py3-2.5.1/README.md` & `reversinglabs_sdk_py3-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 - `upload_sample_from_file`
     - Accepts a file open in 'rb' mode and returns a response containing the analysis task ID
 - `upload_sample_from_url`
     - Accepts a url and returns a response containing the analysis task ID
 - `check_submitted_url_status`
     - Accepts a task id returned by upload_sample_from_url and returns a response containing processing status and 
         report if the report is ready
+- `file_analysis_status`
+    - Accepts a list of file hashes and returns their analysis completion information.
 - `get_submitted_url_report`
     - Accepts a task ID returned by upload_sample_from_url and returns a response
     - This method utilizes the set number of retries and wait time in seconds to time
         out if the analysis results are not ready
 - `upload_sample_from_url_and_get_report`
     - Accepts a url and returns a response containing the analysis report
     - The result fetching action of this method utilizes the set number of retries and wait time in seconds to time
```

### Comparing `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/a1000.py` & `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/a1000.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 AVAILABLE_PLATFORMS = ("windows7", "windows10", "macos_11", "windows11", "linux")
 
 
 class A1000(object):
 
     __TOKEN_ENDPOINT = "/api-token-auth/"
     __UPLOAD_ENDPOINT = "/api/uploads/"
-    __CHECK_STATUS_ENDPOINT = "/api/samples/status/"
-    __CHECK_URL_STATUS_ENDPOINT = "/api/uploads/v2/url-samples/{task_id}"
+    __FILE_ANALYSIS_STATUS_ENDPOINT = "/api/samples/status/"
+    __URL_ANALYSIS_STATUS_ENDPOINT = "/api/uploads/v2/url-samples/{task_id}"
     __RESULTS_ENDPOINT = "/api/samples/list/"
     __SUMMARY_REPORT_ENDPOINT_V2 = "/api/samples/v2/list/"
     __DETAILED_REPORT_ENDPOINT_V2 = "/api/samples/v2/list/details/"
     __CLASSIFY_ENDPOINT_V2 = "/api/v2/samples/{hash_value}/classification/?localonly={localonly}"
     __CLASSIFY_ENDPOINT_V3 = "/api/samples/v3/{hash_value}/classification/"
     __REANALYZE_ENDPOINT = "/api/samples/{hash_value}/analyze/"
     __REANALYZE_BULK_ENDPOINT = "/api/samples/analyze_bulk/"
@@ -157,16 +157,17 @@
 
         return configuration
 
     def test_connection(self):
         """Creates a request towards the A1000 Check Status API to test the connection
         with A1000.
         """
-        _ = self.__analysis_is_finished(
-            sample_hashes=["0000000000000000000000000000000000000000"]
+        self.file_analysis_status(
+            sample_hashes=["0000000000000000000000000000000000000000"],
+            sample_status="processed"
         )
 
         return
 
     def upload_sample_from_path(self, file_path, custom_filename=None, archive_password=None,
                                 rl_cloud_sandbox_platform=None, tags=None, comment=None, cloud_analysis=True):
         """Accepts a file path string for file upload and returns a response.
@@ -291,25 +292,54 @@
             data=data,
         )
 
         self.__raise_on_error(response)
 
         return response
 
+    def file_analysis_status(self, sample_hashes, sample_status=None):
+        """Accepts a list of file hashes and returns their analysis completion information.
+            :param sample_hashes: list of hash strings
+            :type sample_hashes: list[str]
+            :param sample_status: return only samples with this classification;
+            supported values are 'processed' and 'not_found'
+            :type sample_status: str
+            :return: :class:`Response <Response>` object
+            :rtype: requests.Response
+        """
+        data = {"hash_values": sample_hashes}
+
+        params = {}
+
+        if sample_status:
+            params["status"] = sample_status
+
+        url = self._url.format(endpoint=self.__FILE_ANALYSIS_STATUS_ENDPOINT)
+
+        response = self.__post_request(
+            url=url,
+            data=data,
+            params=params
+        )
+
+        self.__raise_on_error(response)
+
+        return response
+
     def check_submitted_url_status(self, task_id):
         """Accepts a task ID returned by the upload sample from url
             :param task_id: ID of the submitted sample
             :type task_id: str
             :return: response
             :rtype: requests.Response
         """
         if not isinstance(task_id, str):
             raise WrongInputError("task_id parameter must be a string.")
 
-        endpoint = self.__CHECK_URL_STATUS_ENDPOINT.format(task_id=task_id)
+        endpoint = self.__URL_ANALYSIS_STATUS_ENDPOINT.format(task_id=task_id)
 
         url = self._url.format(endpoint=endpoint)
 
         response = self.__get_request(url=url)
 
         self.__raise_on_error(response)
 
@@ -422,16 +452,19 @@
 
         analysis_is_finished = False
 
         for iteration in range(retries + 1):
             if iteration:
                 time.sleep(self._wait_time_seconds)
 
-            analysis_is_finished = self.__analysis_is_finished(sample_hashes)
-            if analysis_is_finished:
+            analysis_status = self.file_analysis_status(sample_hashes=sample_hashes, sample_status="processed")
+
+            if len(analysis_status.json().get("results")) == len(sample_hashes):
+                analysis_is_finished = True
+
                 break
 
         if not analysis_is_finished:
             raise RequestTimeoutError("Report fetching attempts finished - The analysis report is still not ready "
                                       "or the sample does not exist on the appliance.")
 
         url = self._url.format(endpoint=self.__SUMMARY_REPORT_ENDPOINT_V2)
@@ -560,16 +593,19 @@
 
         analysis_is_finished = False
 
         for iteration in range(retries + 1):
             if iteration:
                 time.sleep(self._wait_time_seconds)
 
-            analysis_is_finished = self.__analysis_is_finished(sample_hashes)
-            if analysis_is_finished:
+            analysis_status = self.file_analysis_status(sample_hashes=sample_hashes, sample_status="processed")
+
+            if len(analysis_status.json().get("results")) == len(sample_hashes):
+                analysis_is_finished = True
+
                 break
 
         if not analysis_is_finished:
             raise RequestTimeoutError("Report fetching attempts finished - The analysis report is still not ready "
                                       "or the sample does not exist on the appliance.")
 
         url = self._url.format(endpoint=self.__DETAILED_REPORT_ENDPOINT_V2)
@@ -2214,39 +2250,14 @@
             data['ticloud'] = ticloud
 
         if not data:
             return None
 
         return data
 
-    def __analysis_is_finished(self, sample_hashes):
-        """Accepts a list of hashes and returns boolean.
-            :param sample_hashes: list of hash strings
-            :type sample_hashes: list[str]
-            :return: boolean for processing status.
-            :rtype: bool
-        """
-        data = {"hash_values": sample_hashes}
-        params = {"status": "processed"}
-
-        url = self._url.format(endpoint=self.__CHECK_STATUS_ENDPOINT)
-
-        response = self.__post_request(
-            url=url,
-            data=data,
-            params=params
-        )
-
-        self.__raise_on_error(response)
-
-        if len(response.json().get("results")) == len(sample_hashes):
-            return True
-
-        return False
-
     def __get_request(self, url, params=None):
         """A generic GET request method for all A1000 methods.
             :param url: request URL
             :type url: str
             :return: response
             :rtype: requests.Response
         """
```

### Comparing `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/clouddeepscan.py` & `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/clouddeepscan.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/helper.py` & `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/ticloud.py` & `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/tiscale.py` & `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/tiscale.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/logo.png` & `reversinglabs_sdk_py3-2.5.2/logo.png`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/PKG-INFO` & `reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.1
+Version: 2.5.2
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -79,14 +79,16 @@
 - `upload_sample_from_file`
     - Accepts a file open in 'rb' mode and returns a response containing the analysis task ID
 - `upload_sample_from_url`
     - Accepts a url and returns a response containing the analysis task ID
 - `check_submitted_url_status`
     - Accepts a task id returned by upload_sample_from_url and returns a response containing processing status and 
         report if the report is ready
+- `file_analysis_status`
+    - Accepts a list of file hashes and returns their analysis completion information.
 - `get_submitted_url_report`
     - Accepts a task ID returned by upload_sample_from_url and returns a response
     - This method utilizes the set number of retries and wait time in seconds to time
         out if the analysis results are not ready
 - `upload_sample_from_url_and_get_report`
     - Accepts a url and returns a response containing the analysis report
     - The result fetching action of this method utilizes the set number of retries and wait time in seconds to time
```

### Comparing `reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/SOURCES.txt` & `reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/setup.py` & `reversinglabs_sdk_py3-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/tests/test_a1000.py` & `reversinglabs_sdk_py3-2.5.2/tests/test_a1000.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/tests/test_helper.py` & `reversinglabs_sdk_py3-2.5.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/tests/test_ticloud.py` & `reversinglabs_sdk_py3-2.5.2/tests/test_ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.1/tests/test_tiscale.py` & `reversinglabs_sdk_py3-2.5.2/tests/test_tiscale.py`

 * *Files identical despite different names*

