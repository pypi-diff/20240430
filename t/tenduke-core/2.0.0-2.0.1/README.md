# Comparing `tmp/tenduke_core-2.0.0.tar.gz` & `tmp/tenduke_core-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenduke_core-2.0.0.tar", max compression
+gzip compressed data, was "tenduke_core-2.0.1.tar", max compression
```

## Comparing `tenduke_core-2.0.0.tar` & `tenduke_core-2.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1108 2024-04-29 01:50:39.175564 tenduke_core-2.0.0/LICENSE
--rw-r--r--   0        0        0     2843 2024-04-29 01:50:39.175564 tenduke_core-2.0.0/README.md
--rw-r--r--   0        0        0     3624 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      191 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/__init__.py
--rw-r--r--   0        0        0      661 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/__init__.py
--rw-r--r--   0        0        0     1665 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/auth_provider.py
--rw-r--r--   0        0        0     1022 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/device_auth_response.py
--rw-r--r--   0        0        0     7364 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/device_flow_client.py
--rw-r--r--   0        0        0     6516 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/oauth_client.py
--rw-r--r--   0        0        0     1115 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/oidc_discovery.py
--rw-r--r--   0        0        0     7029 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/pkce_flow_client.py
--rw-r--r--   0        0        0     1540 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/token_response.py
--rw-r--r--   0        0        0     1789 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/user_info.py
--rw-r--r--   0        0        0     4121 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/base_model.py
--rw-r--r--   0        0        0      135 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/config/__init__.py
--rw-r--r--   0        0        0     4484 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/config/tenduke_config.py
--rw-r--r--   0        0        0      319 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/exceptions/__init__.py
--rw-r--r--   0        0        0     2494 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/exceptions/api.py
--rw-r--r--   0        0        0     5939 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/exceptions/oauth.py
--rw-r--r--   0        0        0     1858 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/exceptions/validation.py
--rw-r--r--   0        0        0      100 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/http/__init__.py
--rw-r--r--   0        0        0     1590 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/http/session_factory.py
--rw-r--r--   0        0        0        0 2024-04-29 01:50:39.204564 tenduke_core-2.0.0/tenduke_core/py.typed
--rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 tenduke_core-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-04-30 03:38:11.345403 tenduke_core-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2843 2024-04-30 03:38:11.345403 tenduke_core-2.0.1/README.md
+-rw-r--r--   0        0        0     3624 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      191 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/__init__.py
+-rw-r--r--   0        0        0      661 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/__init__.py
+-rw-r--r--   0        0        0     1665 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/auth_provider.py
+-rw-r--r--   0        0        0     1022 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/device_auth_response.py
+-rw-r--r--   0        0        0     7547 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/device_flow_client.py
+-rw-r--r--   0        0        0     6699 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/oauth_client.py
+-rw-r--r--   0        0        0     1115 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/oidc_discovery.py
+-rw-r--r--   0        0        0     7592 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/pkce_flow_client.py
+-rw-r--r--   0        0        0     1540 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/token_response.py
+-rw-r--r--   0        0        0     1789 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/auth/user_info.py
+-rw-r--r--   0        0        0     4121 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/base_model.py
+-rw-r--r--   0        0        0      135 2024-04-30 03:38:11.346403 tenduke_core-2.0.1/tenduke_core/config/__init__.py
+-rw-r--r--   0        0        0     4484 2024-04-30 03:38:11.347403 tenduke_core-2.0.1/tenduke_core/config/tenduke_config.py
+-rw-r--r--   0        0        0      319 2024-04-30 03:38:11.347403 tenduke_core-2.0.1/tenduke_core/exceptions/__init__.py
+-rw-r--r--   0        0        0     2494 2024-04-30 03:38:11.347403 tenduke_core-2.0.1/tenduke_core/exceptions/api.py
+-rw-r--r--   0        0        0     5939 2024-04-30 03:38:11.347403 tenduke_core-2.0.1/tenduke_core/exceptions/oauth.py
+-rw-r--r--   0        0        0     1858 2024-04-30 03:38:11.347403 tenduke_core-2.0.1/tenduke_core/exceptions/validation.py
+-rw-r--r--   0        0        0      100 2024-04-30 03:38:11.347403 tenduke_core-2.0.1/tenduke_core/http/__init__.py
+-rw-r--r--   0        0        0     1590 2024-04-30 03:38:11.347403 tenduke_core-2.0.1/tenduke_core/http/session_factory.py
+-rw-r--r--   0        0        0        0 2024-04-30 03:38:11.370403 tenduke_core-2.0.1/tenduke_core/py.typed
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 tenduke_core-2.0.1/PKG-INFO
```

### Comparing `tenduke_core-2.0.0/LICENSE` & `tenduke_core-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/README.md` & `tenduke_core-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/pyproject.toml` & `tenduke_core-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenduke_core"
-version = "2.0.0"
+version = "2.0.1"
 description = "Shared code supporting 10Duke SDKs"
 authors = []
 repository = "https://gitlab.com/10Duke/core/python-core"
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "tenduke_core"},
```

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/__init__.py` & `tenduke_core-2.0.1/tenduke_core/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/auth_provider.py` & `tenduke_core-2.0.1/tenduke_core/auth/auth_provider.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/device_auth_response.py` & `tenduke_core-2.0.1/tenduke_core/auth/device_auth_response.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/device_flow_client.py` & `tenduke_core-2.0.1/tenduke_core/auth/device_flow_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,17 @@
     def __init__(self, config: TendukeConfig, session_factory: SessionFactory):
         """Construct an instance of the DeviceFlowClient.
 
         Args:
             config:
                 Configuration parameters for interacting with the OAuth / Open ID Authorization
                 Server.
+            session_factory:
+                Used to create requests Session configured with the settings from config and with
+                the configured User-Agent header value.
         """
         self._device_code = None
         self._expires_at = None
         self._user_code: str = ""
         self._interval = 5
         self._verification_uri = self.VerificationUri()
         super().__init__(config, session_factory)
```

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/oauth_client.py` & `tenduke_core-2.0.1/tenduke_core/auth/oauth_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,17 @@
         """
         Construct an instance of the OAuth Client.
 
         Args:
             config:
                 Configuration parameters for interacting with the OAuth / Open ID Authorization
                 Server.
+            session_factory:
+                Used to create requests Session configured with the settings from config and with
+                the configured User-Agent header value.
         """
         self.config = config
         self._idp_jwks_client = None
         if config.idp_jwks_uri:
             self._idp_jwks_client = PyJWKClient(
                 config.idp_jwks_uri, cache_keys=True, lifespan=345000
             )
```

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/oidc_discovery.py` & `tenduke_core-2.0.1/tenduke_core/auth/oidc_discovery.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/pkce_flow_client.py` & `tenduke_core-2.0.1/tenduke_core/auth/pkce_flow_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from urllib.parse import urljoin, urlparse, urlunparse
 
 # no type stubs have been published for authlib but they may come in future:
 #  https://github.com/lepture/authlib/issues/460
 from authlib.common.security import generate_token  # type: ignore[import-untyped]
 from authlib.integrations.requests_client import OAuth2Session  # type: ignore[import-untyped]
 
+from tenduke_core.config import TendukeConfig
+from tenduke_core.http import SessionFactory
+
 from ..exceptions.oauth import AuthenticationFailed
 from .oauth_client import OAuthClient
 from .token_response import TokenResponse
 
 AUTH_SUCCESS_MESSAGE = """
 HTTP/1.1 200 OK
 Connection: close
@@ -65,20 +68,29 @@
 
         def do_GET(self):  # pylint: disable=invalid-name
             """Handle OAuth redirect."""
             self.wfile.write(self.server.success_http.encode("UTF-8"))  # pyright:ignore[reportAttributeAccessIssue]
             self.wfile.flush()
             self.server.authorization_response = self.path  # pyright:ignore[reportAttributeAccessIssue]
 
-    def __init__(self, *args, **kwargs):
-        """Construct an instance of the PkceFlowClient."""
+    def __init__(self, config: TendukeConfig, session_factory: SessionFactory, *args, **kwargs):
+        """Construct an instance of the PkceFlowClient.
+
+        Args:
+            config:
+                Configuration parameters for interacting with the OAuth / Open ID Authorization
+                Server.
+            session_factory:
+                Used to create requests Session configured with the settings from config and with
+                the configured User-Agent header value.
+        """
         self.code_verifier = kwargs.pop("code_verifier", None)
         self.state = kwargs.pop("state", None)
         self._client = None
-        super().__init__(*args, **kwargs)
+        super().__init__(config, session_factory)
 
     def _build_redirect_uri(self, port: Optional[int] = None):
         port = port or self.config.auth_redirect_port
         redirect_uri = self.config.auth_redirect_uri
         parsed_result = urlparse(redirect_uri)
         if parsed_result.hostname in (
             "localhost",
@@ -122,15 +134,15 @@
 
         self._client = OAuth2Session(
             client_id=self.config.idp_oauth_client_id,
             scope=self.config.idp_oauth_scope,
             redirect_uri=redirect_uri,
             code_challenge_method="S256",
         )
-        url, state = self._client.create_authorization_url(
+        url, state = self._client.create_authorization_url(  # type: ignore[attr-defined]
             self.config.idp_oauth_authorization_url, code_verifier=self.code_verifier
         )
         self.state = state
         return url
 
     def fetch_token(
         self, authorization_response: Optional[str], port: Optional[int] = None
@@ -149,15 +161,15 @@
         if self._client is None:
             self._client = OAuth2Session(
                 client_id=self.config.idp_oauth_client_id,
                 scope=self.config.idp_oauth_scope,
                 redirect_uri=redirect_uri,
                 code_challenge_method="S256",
             )
-        token = self._client.fetch_token(
+        token = self._client.fetch_token(  # type: ignore[attr-defined]
             self.config.idp_oauth_token_url,
             authorization_response=authorization_response,
             state=self.state,
             code_verifier=self.code_verifier,
         )
         token = TokenResponse.from_api(token)
         self.token = token
```

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/token_response.py` & `tenduke_core-2.0.1/tenduke_core/auth/token_response.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/auth/user_info.py` & `tenduke_core-2.0.1/tenduke_core/auth/user_info.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/base_model.py` & `tenduke_core-2.0.1/tenduke_core/base_model.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/config/tenduke_config.py` & `tenduke_core-2.0.1/tenduke_core/config/tenduke_config.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/exceptions/api.py` & `tenduke_core-2.0.1/tenduke_core/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/exceptions/oauth.py` & `tenduke_core-2.0.1/tenduke_core/exceptions/oauth.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/exceptions/validation.py` & `tenduke_core-2.0.1/tenduke_core/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/tenduke_core/http/session_factory.py` & `tenduke_core-2.0.1/tenduke_core/http/session_factory.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-2.0.0/PKG-INFO` & `tenduke_core-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenduke_core
-Version: 2.0.0
+Version: 2.0.1
 Summary: Shared code supporting 10Duke SDKs
 Home-page: https://gitlab.com/10Duke/core/python-core
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

