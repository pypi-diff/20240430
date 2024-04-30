# Comparing `tmp/gundi_client_v2-2.1.7.tar.gz` & `tmp/gundi_client_v2-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_client_v2-2.1.7.tar", max compression
+gzip compressed data, was "gundi_client_v2-2.2.0.tar", max compression
```

## Comparing `gundi_client_v2-2.1.7.tar` & `gundi_client_v2-2.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1542 2023-11-16 20:47:17.280064 gundi_client_v2-2.1.7/README.md
--rw-r--r--   0        0        0       53 2023-11-16 20:47:17.280064 gundi_client_v2-2.1.7/gundi_client_v2/__init__.py
--rw-r--r--   0        0        0      684 2023-11-16 20:47:17.280064 gundi_client_v2-2.1.7/gundi_client_v2/auth.py
--rw-r--r--   0        0        0     7662 2023-12-21 12:30:04.704160 gundi_client_v2-2.1.7/gundi_client_v2/client.py
--rw-r--r--   0        0        0        0 2023-12-20 19:28:53.459832 gundi_client_v2-2.1.7/gundi_client_v2/errors.py
--rw-r--r--   0        0        0      719 2023-11-16 20:47:17.280064 gundi_client_v2-2.1.7/gundi_client_v2/settings.py
--rw-r--r--   0        0        0      678 2023-12-21 12:32:17.846390 gundi_client_v2-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 gundi_client_v2-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1542 2024-03-07 13:24:31.154887 gundi_client_v2-2.2.0/README.md
+-rw-r--r--   0        0        0       53 2024-03-07 13:24:31.154887 gundi_client_v2-2.2.0/gundi_client_v2/__init__.py
+-rw-r--r--   0        0        0      684 2024-03-07 13:24:31.154887 gundi_client_v2-2.2.0/gundi_client_v2/auth.py
+-rw-r--r--   0        0        0     8904 2024-03-07 20:07:46.206525 gundi_client_v2-2.2.0/gundi_client_v2/client.py
+-rw-r--r--   0        0        0        0 2024-03-07 13:24:31.158887 gundi_client_v2-2.2.0/gundi_client_v2/errors.py
+-rw-r--r--   0        0        0      719 2024-03-07 13:24:31.158887 gundi_client_v2-2.2.0/gundi_client_v2/settings.py
+-rw-r--r--   0        0        0      678 2024-03-07 13:39:21.519908 gundi_client_v2-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 gundi_client_v2-2.2.0/PKG-INFO
```

### Comparing `gundi_client_v2-2.1.7/README.md` & `gundi_client_v2-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.1.7/gundi_client_v2/auth.py` & `gundi_client_v2-2.2.0/gundi_client_v2/auth.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.1.7/gundi_client_v2/client.py` & `gundi_client_v2-2.2.0/gundi_client_v2/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Timeout,
 )
 from pydantic import parse_obj_as
 from typing import List
 from gundi_core.schemas import (
     OAuthToken,
 )
-from gundi_core.schemas.v2 import Connection, Route, Integration, GundiTrace
+from gundi_core.schemas.v2 import Connection, Route, Integration, GundiTrace, IntegrationType
 from . import settings, errors
 from . import auth
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(settings.LOG_LEVEL)
 
@@ -130,14 +130,36 @@
                 url,
                 params=params,
                 headers=headers,
                 **kwargs,
             )
         return response
 
+    async def _post(self, url, data: dict = None, params=None, headers=None, **kwargs):
+        headers = headers or {}
+        auth_headers = await self.get_auth_header()
+        response = await self._session.post(
+            url,
+            json=data,
+            params=params,
+            headers={**auth_headers, **headers},
+            **kwargs,
+        )
+        # Force refresh the token and retry if we get redirected to the login page
+        if response.status_code == 302 and "auth/realms" in response.headers.get("location", ""):
+            headers = await self.get_auth_header(force_refresh_token=True)
+            await self._session.post(
+                url,
+                json=json,
+                params=params,
+                headers={**auth_headers, **headers},
+                **kwargs,
+            )
+        return response
+
     async def _refresh_token(self):
         token = await auth.get_access_token(
             session=self._session,
             oauth_token_url=self.oauth_token_url,
             client_id=self.client_id,
             client_secret=self.client_secret,
             audience=self.audience
@@ -194,7 +216,18 @@
     async def get_traces(self, params: dict):
         url = f"{self.traces_endpoint}/"
         response = await self._get(url, params=params)
         # ToDo: Add custom exceptions to handle errors
         response.raise_for_status()
         data = response.json()["results"]
         return parse_obj_as(List[GundiTrace], data)
+
+    async def register_integration_type(self, data: dict):
+        url = f"{self.integrations_endpoint}/types/"
+        response = await self._post(
+            url,
+            data=data,
+        )
+        # ToDo: Add custom exceptions to handle errors
+        response.raise_for_status()
+        data = response.json()
+        return IntegrationType.parse_obj(data)
```

### Comparing `gundi_client_v2-2.1.7/gundi_client_v2/settings.py` & `gundi_client_v2-2.2.0/gundi_client_v2/settings.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.1.7/PKG-INFO` & `gundi_client_v2-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gundi-client-v2
-Version: 2.1.7
+Version: 2.2.0
 Summary: An async client for Gundi's API
 License: Apache-2.0
 Author: Chris Doehring
 Author-email: chrisdo@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

