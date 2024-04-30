# Comparing `tmp/ak_requests-0.1.0.tar.gz` & `tmp/ak_requests-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_requests-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ak_requests-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ak_requests-0.1.0.tar` & `ak_requests-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      691 2023-11-11 22:11:08.760659 ak_requests-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     2016 2023-09-22 07:02:49.847345 ak_requests-0.1.0/.gitignore
--rw-r--r--   0        0        0     1100 2023-09-22 07:02:49.847345 ak_requests-0.1.0/LICENSE
--rw-r--r--   0        0        0     5708 2023-11-11 22:11:08.760659 ak_requests-0.1.0/README.md
--rw-r--r--   0        0        0     3397 2023-11-11 22:11:08.761660 ak_requests-0.1.0/development.ipynb
--rw-r--r--   0        0        0      643 2023-11-11 22:11:08.761660 ak_requests-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      193 2023-11-11 22:11:31.698938 ak_requests-0.1.0/src/ak_requests/__init__.py
--rw-r--r--   0        0        0      154 2023-11-09 02:35:08.675654 ak_requests-0.1.0/src/ak_requests/beautifulsoup.py
--rw-r--r--   0        0        0     1496 2023-11-11 22:11:08.761660 ak_requests-0.1.0/src/ak_requests/logger.py
--rw-r--r--   0        0        0    11654 2023-11-11 22:11:08.762660 ak_requests-0.1.0/src/ak_requests/request.py
--rw-r--r--   0        0        0        0 2023-09-22 07:02:49.849345 ak_requests-0.1.0/src/tests/__init__.py
--rw-r--r--   0        0        0     2246 2023-11-11 22:11:08.762660 ak_requests-0.1.0/src/tests/test_request.py
--rw-r--r--   0        0        0     6131 1970-01-01 00:00:00.000000 ak_requests-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      691 2024-03-05 22:48:11.189760 ak_requests-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2016 2024-03-05 22:48:11.191740 ak_requests-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1100 2024-03-05 22:48:11.191740 ak_requests-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5720 2024-04-30 21:14:32.836089 ak_requests-0.1.1/README.md
+-rw-r--r--   0        0        0     3397 2024-03-05 22:48:11.193741 ak_requests-0.1.1/development.ipynb
+-rw-r--r--   0        0        0      643 2024-03-05 22:48:11.194740 ak_requests-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-30 21:15:33.347150 ak_requests-0.1.1/src/ak_requests/__init__.py
+-rw-r--r--   0        0        0      154 2024-03-05 22:48:11.196739 ak_requests-0.1.1/src/ak_requests/beautifulsoup.py
+-rw-r--r--   0        0        0     1496 2024-03-05 22:48:11.197738 ak_requests-0.1.1/src/ak_requests/logger.py
+-rw-r--r--   0        0        0    11760 2024-04-30 21:14:32.844085 ak_requests-0.1.1/src/ak_requests/request.py
+-rw-r--r--   0        0        0        0 2024-03-05 22:48:11.199739 ak_requests-0.1.1/src/tests/__init__.py
+-rw-r--r--   0        0        0     2246 2024-03-05 22:48:11.200755 ak_requests-0.1.1/src/tests/test_request.py
+-rw-r--r--   0        0        0     6143 1970-01-01 00:00:00.000000 ak_requests-0.1.1/PKG-INFO
```

### Comparing `ak_requests-0.1.0/.github/workflows/test.yml` & `ak_requests-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ak_requests-0.1.0/.gitignore` & `ak_requests-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ak_requests-0.1.0/LICENSE` & `ak_requests-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ak_requests-0.1.0/README.md` & `ak_requests-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 <!-- Usage -->
 ## 3. Usage
 
 ```python
 from ak_requests import RequestsSession
 
 # Initialize session
-session = RequestsSession(log=False, retries=5, log_level='error') 
+session = RequestsSession(log=False, retries=5, log_level='error', timeout=10) 
 
 ## Can update session level variables
 session.MIN_REQUEST_GAP = 1.5   # seconds, Change min time bet. requests
 session.RAISE_ERRORS = False    # raises RequestErrors, else returns None; defaults to True
 
 # Update custom header
 session.update_header({'Connection': 'keep-alive'})
```

#### html2text {}

```diff
@@ -24,17 +24,17 @@
 exceptions or skip it completely with `RAISE_EXCEPTIONS` attribute - Can
 support both basic `.basic_auth()` and OAuth `.oauth2_auth()` authentications.
 ## 2. Getting Started ### 2.1. Installation #### 2.1.1. Production Download the
 repo and install with flit ```bash pip install flit flit install --deps
 production ``` Alternatively, you can use pip ```bash pip install ak_requests
 ``` #### 2.1.2. Development Install with flit ```bash flit install --pth-file
 ``` ## 3. Usage ```python from ak_requests import RequestsSession # Initialize
-session session = RequestsSession(log=False, retries=5, log_level='error') ##
-Can update session level variables session.MIN_REQUEST_GAP = 1.5 # seconds,
-Change min time bet. requests session.RAISE_ERRORS = False # raises
+session session = RequestsSession(log=False, retries=5, log_level='error',
+timeout=10) ## Can update session level variables session.MIN_REQUEST_GAP = 1.5
+# seconds, Change min time bet. requests session.RAISE_ERRORS = False # raises
 RequestErrors, else returns None; defaults to True # Update custom header
 session.update_header({'Connection': 'keep-alive'}) # set cookies
 session.update_cookies([{'name':'has_recent_activity', 'value':'1'}]) # Get
 requests res = session.get('https://reqres.in/api/users?page=2', data={},
 proxies = {} ) # Can accept any requests parameters # Make bulk requests urls =
 ['https://reqres.in/api/users?page=2', 'https://reqres.in/api/unknown']
 responses = session.bulk_get(urls) # use beautifulsoup from ak_requests import
```

### Comparing `ak_requests-0.1.0/development.ipynb` & `ak_requests-0.1.1/development.ipynb`

 * *Files identical despite different names*

### Comparing `ak_requests-0.1.0/pyproject.toml` & `ak_requests-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ak_requests-0.1.0/src/ak_requests/logger.py` & `ak_requests-0.1.1/src/ak_requests/logger.py`

 * *Files identical despite different names*

### Comparing `ak_requests-0.1.0/src/ak_requests/request.py` & `ak_requests-0.1.1/src/ak_requests/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 import re
 import time
 from typing import Literal
 import urllib.parse
 
 from ak_requests.logger import Log
 
-DEFAULT_TIMEOUT_s = 5 #seconds
-
 class TimeoutHTTPAdapter(HTTPAdapter):
+    DEFAULT_TIMEOUT_s = 5 #seconds
     #Courtesy of https://findwork.dev/blog/advanced-usage-python-requests-timeouts-retries-hooks/
     def __init__(self, *args, **kwargs):
-        self.timeout = DEFAULT_TIMEOUT_s
+        self.timeout = self.DEFAULT_TIMEOUT_s
         if "timeout" in kwargs:
             self.timeout = kwargs["timeout"]
             del kwargs["timeout"]
         super().__init__(*args, **kwargs)
 
     def send(self, request, **kwargs):
         timeout = kwargs.get("timeout")
@@ -33,23 +32,24 @@
     
 class RequestsSession(Session):
     MIN_REQUEST_GAP: float = 0.9 #seconds
     last_request_time: float = time.time()
     RAISE_ERRORS: bool = True
     
     def __init__(self, log: bool = False, retries: int = 5, 
-                    log_level: Literal['debug', 'info', 'error'] = 'info') -> None:
+                    log_level: Literal['debug', 'info', 'error'] = 'info',
+                    timeout:float=5) -> None:
         self.retries = retries
         self.log: Log | None = Log() if log else None
         self.set_loglevel(log_level)
         
         super().__init__()
         #self.session: Session = requests.Session()
         self._set_default_headers()
-        self._set_default_retry_adapter(retries)
+        self.__set_default_retry_adapter(retries, timeout)
         self.rate_limit_remaining = None
         self.rate_limit_reset = None
         
         self._info(f'Session initialized ({retries=}, {self.MIN_REQUEST_GAP=}, )')
         return None
     
     def check_rate_limit(self) -> None:
@@ -88,21 +88,21 @@
         
     def __repr__(self) -> str:
         return f"RequestsSession(log={self.log is not None})"
     
     def __str__(self) -> str:
         return f"RequestsSession Class. Logging set to {self.log is not None}"
 
-    def _set_default_retry_adapter(self, max_retries: int) -> requests.Session:
+    def __set_default_retry_adapter(self, max_retries: int, timeout: float) -> requests.Session:
         retries = Retry(total=max_retries,
                         backoff_factor=0.5,
                         status_forcelist=[429, 500, 502, 503, 504]
                         )
-        self.mount('http://', TimeoutHTTPAdapter(max_retries=retries))
-        self.mount('https://', TimeoutHTTPAdapter(max_retries=retries))
+        self.mount('http://', TimeoutHTTPAdapter(max_retries=retries, timeout=timeout))
+        self.mount('https://', TimeoutHTTPAdapter(max_retries=retries, timeout=timeout))
         
         self._debug('Default retry adapters loaded')
         return self
 
     def get(self, *args, **kwargs) -> requests.Response:
         try:
             min_req_gap: float = self.MIN_REQUEST_GAP
```

### Comparing `ak_requests-0.1.0/src/tests/test_request.py` & `ak_requests-0.1.1/src/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `ak_requests-0.1.0/PKG-INFO` & `ak_requests-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ak_requests
-Version: 0.1.0
+Version: 0.1.1
 Summary: Requests package with QOL improvements and anti-bot detection measures
 Author-email: Arun Kishore <pypi@rpakishore.co.in>
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests>=2.31.0
 Requires-Dist: beautifulsoup4>=4.12.2
@@ -103,15 +103,15 @@
 <!-- Usage -->
 ## 3. Usage
 
 ```python
 from ak_requests import RequestsSession
 
 # Initialize session
-session = RequestsSession(log=False, retries=5, log_level='error') 
+session = RequestsSession(log=False, retries=5, log_level='error', timeout=10) 
 
 ## Can update session level variables
 session.MIN_REQUEST_GAP = 1.5   # seconds, Change min time bet. requests
 session.RAISE_ERRORS = False    # raises RequestErrors, else returns None; defaults to True
 
 # Update custom header
 session.update_header({'Connection': 'keep-alive'})
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ak_requests Version: 0.1.0 Summary: Requests
+Metadata-Version: 2.1 Name: ak_requests Version: 0.1.1 Summary: Requests
 package with QOL improvements and anti-bot detection measures Author-email:
 Arun Kishore
 rpakishore.co.in> Requires-Python: >=3.11.0 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Requires-Dist:
 requests>=2.31.0 Requires-Dist: beautifulsoup4>=4.12.2 Requires-Dist: yt-
 dlp>=2023.10.13 Requires-Dist: ipykernel ; extra == "dev" Requires-Dist:
 pytest>=7.4.3 ; extra == "test" Project-URL: Home, https://github.com/
@@ -33,17 +33,17 @@
 exceptions or skip it completely with `RAISE_EXCEPTIONS` attribute - Can
 support both basic `.basic_auth()` and OAuth `.oauth2_auth()` authentications.
 ## 2. Getting Started ### 2.1. Installation #### 2.1.1. Production Download the
 repo and install with flit ```bash pip install flit flit install --deps
 production ``` Alternatively, you can use pip ```bash pip install ak_requests
 ``` #### 2.1.2. Development Install with flit ```bash flit install --pth-file
 ``` ## 3. Usage ```python from ak_requests import RequestsSession # Initialize
-session session = RequestsSession(log=False, retries=5, log_level='error') ##
-Can update session level variables session.MIN_REQUEST_GAP = 1.5 # seconds,
-Change min time bet. requests session.RAISE_ERRORS = False # raises
+session session = RequestsSession(log=False, retries=5, log_level='error',
+timeout=10) ## Can update session level variables session.MIN_REQUEST_GAP = 1.5
+# seconds, Change min time bet. requests session.RAISE_ERRORS = False # raises
 RequestErrors, else returns None; defaults to True # Update custom header
 session.update_header({'Connection': 'keep-alive'}) # set cookies
 session.update_cookies([{'name':'has_recent_activity', 'value':'1'}]) # Get
 requests res = session.get('https://reqres.in/api/users?page=2', data={},
 proxies = {} ) # Can accept any requests parameters # Make bulk requests urls =
 ['https://reqres.in/api/users?page=2', 'https://reqres.in/api/unknown']
 responses = session.bulk_get(urls) # use beautifulsoup from ak_requests import
```

