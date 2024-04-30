# Comparing `tmp/fastapi_keycloak_middleware-0.4.0.tar.gz` & `tmp/fastapi_keycloak_middleware-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_keycloak_middleware-0.4.0.tar", max compression
+gzip compressed data, was "fastapi_keycloak_middleware-0.4.1.tar", max compression
```

## Comparing `fastapi_keycloak_middleware-0.4.0.tar` & `fastapi_keycloak_middleware-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/LICENSE
--rw-r--r--   0        0        0     4016 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/README.md
--rw-r--r--   0        0        0     1481 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/__init__.py
--rw-r--r--   0        0        0     5169 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/require_permission.py
--rw-r--r--   0        0        0      856 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/strip_request.py
--rw-r--r--   0        0        0      352 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/dependencies/__init__.py
--rw-r--r--   0        0        0      467 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/dependencies/get_authorization_result.py
--rw-r--r--   0        0        0      420 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/dependencies/get_user.py
--rw-r--r--   0        0        0      703 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/exceptions.py
--rw-r--r--   0        0        0     1042 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/fast_api_user.py
--rw-r--r--   0        0        0     7773 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/keycloak_backend.py
--rw-r--r--   0        0        0     7995 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/middleware.py
--rw-r--r--   0        0        0        0 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/__init__.py
--rw-r--r--   0        0        0      523 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/authorization_methods.py
--rw-r--r--   0        0        0     1257 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/authorization_result.py
--rw-r--r--   0        0        0      232 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/exception_response.py
--rw-r--r--   0        0        0     6452 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/keycloak_configuration.py
--rw-r--r--   0        0        0      581 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/match_strategy.py
--rw-r--r--   0        0        0     5775 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/setup.py
--rw-r--r--   0        0        0      739 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.0/setup.py
--rw-r--r--   0        0        0     4567 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4422 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/README.md
+-rw-r--r--   0        0        0     1481 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/__init__.py
+-rw-r--r--   0        0        0     5058 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/require_permission.py
+-rw-r--r--   0        0        0      856 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/strip_request.py
+-rw-r--r--   0        0        0      352 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/dependencies/__init__.py
+-rw-r--r--   0        0        0      467 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/dependencies/get_authorization_result.py
+-rw-r--r--   0        0        0      420 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/dependencies/get_user.py
+-rw-r--r--   0        0        0      703 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/exceptions.py
+-rw-r--r--   0        0        0     1042 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/fast_api_user.py
+-rw-r--r--   0        0        0     7549 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/keycloak_backend.py
+-rw-r--r--   0        0        0     8039 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/__init__.py
+-rw-r--r--   0        0        0      523 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/authorization_methods.py
+-rw-r--r--   0        0        0     1257 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/authorization_result.py
+-rw-r--r--   0        0        0      232 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/exception_response.py
+-rw-r--r--   0        0        0     6460 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/keycloak_configuration.py
+-rw-r--r--   0        0        0      581 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/match_strategy.py
+-rw-r--r--   0        0        0     5761 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/setup.py
+-rw-r--r--   0        0        0     1637 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.1/setup.py
+-rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.1/PKG-INFO
```

### Comparing `fastapi_keycloak_middleware-0.4.0/LICENSE` & `fastapi_keycloak_middleware-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.0/README.md` & `fastapi_keycloak_middleware-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -68,11 +68,26 @@
 
 ## Acknowledgements
 
 This package is heavily inspired by [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)
 which provides some of the same functionality but without the direct integration
 into Keycloak. Thanks for writing and providing this great piece of software!
 
+## Contributing
+
+The client is written in pure Python.
+Any changes or pull requests are more than welcome, but please adhere to the code style.
+
+Ruff is used both for code formatting and linting. Before committing, please run the following command to ensure
+that your code is properly formatted:
+
+```bash
+ruff check .
+ruff format .
+```
+
+A pre-commit hook configuration is supplied as part of the project.
+
 ## Development
 
 This project is using [Act](https://github.com/nektos/act) to handle local development tasks. It is used
 to work locally and also to test Github actions before deploying them.
```

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/__init__.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Middleware for FastAPI that supports authenticating users against Keycloak
 """
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 import logging
 
 from fastapi_keycloak_middleware.decorators.require_permission import require_permission
 from fastapi_keycloak_middleware.decorators.strip_request import strip_request
 from fastapi_keycloak_middleware.dependencies.get_authorization_result import (
     get_authorization_result,
```

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/require_permission.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/require_permission.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # pylint: disable=logging-not-lazy,consider-using-f-string
 # NOTE: Using % formatting is the safest way as we allow custom loggers.
 #       There could be custom loggers that handle arguments differently
 
 import logging
 import typing
 from collections import OrderedDict
+from collections.abc import Callable
 from functools import wraps
 from inspect import Parameter, signature
-from typing import Callable
 
 import starlette
 from fastapi import HTTPException
 from starlette.requests import Request
 
 from fastapi_keycloak_middleware.decorators.strip_request import strip_request
 from fastapi_keycloak_middleware.schemas.authorization_methods import (
@@ -47,29 +47,25 @@
 
     # Check if permissions is a single string, convert to list if so
     if isinstance(permissions, str):
         permissions = [permissions]
 
     # Check if match_strategy is valid
     if match_strategy not in MatchStrategy:
-        raise ValueError(
-            "Invalid match strategy. Must be 'and' or 'or'. Got %s" % match_strategy
-        )
+        raise ValueError(f"Invalid match strategy. Must be 'and' or 'or'. Got {match_strategy}")
 
     def _check_permission(
         requested_permission: typing.List[str], allowed_scopes: typing.List[str]
     ) -> typing.Tuple[bool, typing.List[str]]:
         """
         Check if the user has permission based on the matching strategy
         """
         # Get matching permissions
         matching_permissions = [
-            permission
-            for permission in requested_permission
-            if permission in allowed_scopes
+            permission for permission in requested_permission if permission in allowed_scopes
         ]
 
         if match_strategy == MatchStrategy.AND:
             return (
                 set(requested_permission) == set(matching_permissions),
                 matching_permissions,
             )
@@ -88,39 +84,37 @@
         async def wrapper(*args, **kwargs):
             request = kwargs.get("request", None)
 
             assert isinstance(request, Request)
 
             user = request.get("user", None)
 
-            log.debug("Checking permission %s for user %s" % (permissions, str(user)))
+            log.debug(f"Checking permission {permissions} for user {str(user)}")
 
             allowed_scopes = request.get("auth", [])
 
             # Check if user has permission
-            allowed, matching_permissions = _check_permission(
-                permissions, allowed_scopes
-            )
+            allowed, matching_permissions = _check_permission(permissions, allowed_scopes)
 
             if allowed:
-                log.info("Permission granted for user %s" % (str(user)))
-                log.debug("Matching permissions: %s" % (matching_permissions))
+                log.info(f"Permission granted for user {str(user)}")
+                log.debug(f"Matching permissions: {matching_permissions}")
 
                 # Check if "matched_scopes" is in function signature.
                 # If so, add it to the function call.
                 if "authorization_result" in signature(func).parameters.keys():
                     kwargs["authorization_result"] = AuthorizationResult(
                         method=AuthorizationMethod.CLAIM,
                         authorized=True,
                         matched_scopes=matching_permissions,
                     )
 
                 return await func(*args, **kwargs)
 
-            log.warning("Permission %s denied for user %s" % (permissions, str(user)))
+            log.warning(f"Permission {permissions} denied for user {str(user)}")
             raise HTTPException(status_code=403, detail="Permission denied")
 
         # Override signature
         # See https://peps.python.org/pep-0362/#signature-object
         # Note that the signature is immutable, so we need to create a new one
         sig = signature(func)
         parameters: OrderedDict = sig.parameters
@@ -132,14 +126,12 @@
                 name="request",
                 kind=Parameter.POSITIONAL_OR_KEYWORD,
                 default=Parameter.empty,
                 annotation=starlette.requests.Request,
             ),
             *parameters.values(),
         ]
-        new_sig = sig.replace(
-            parameters=parameters, return_annotation=sig.return_annotation
-        )
+        new_sig = sig.replace(parameters=parameters, return_annotation=sig.return_annotation)
         wrapper.__signature__ = new_sig
         return wrapper
 
     return decorator
```

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/strip_request.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/strip_request.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/exceptions.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/fast_api_user.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/fast_api_user.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/keycloak_backend.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/keycloak_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This module contains the Keycloak backend.
 
 It is used by the middleware to perform the actual authentication.
 """
 
 import logging
 import typing
-from typing import Tuple
 
 import keycloak
 from jose import ExpiredSignatureError, JWTError
 from jose.exceptions import JWTClaimsError
 from keycloak import KeycloakOpenID
 from starlette.authentication import AuthCredentials, AuthenticationBackend, BaseUser
 from starlette.requests import HTTPConnection
@@ -38,33 +37,29 @@
     """
     Backend to perform authentication using Keycloak
     """
 
     def __init__(
         self,
         keycloak_configuration: KeycloakConfiguration,
-        user_mapper: typing.Callable[
-            [typing.Dict[str, typing.Any]], typing.Awaitable[typing.Any]
-        ],
+        user_mapper: typing.Callable[[typing.Dict[str, typing.Any]], typing.Awaitable[typing.Any]],
     ):
         self.keycloak_configuration = keycloak_configuration
         self.keycloak_openid = self._get_keycloak_openid(keycloak_configuration)
         self.get_user = user_mapper if user_mapper else self._get_user
 
         # Fetch KC public key if needed
         if not keycloak_configuration.use_introspection_endpoint:
             self.keycloak_public_key = (
                 "-----BEGIN PUBLIC KEY-----\n"
                 + self.keycloak_openid.public_key()
                 + "\n-----END PUBLIC KEY-----"
             )
 
-    def _get_keycloak_openid(
-        self, keycloak_configuration: KeycloakConfiguration
-    ) -> KeycloakOpenID:
+    def _get_keycloak_openid(self, keycloak_configuration: KeycloakConfiguration) -> KeycloakOpenID:
         """
         Instance-scoped KeycloakOpenID object
         """
         return KeycloakOpenID(
             server_url=self.keycloak_configuration.url,
             client_id=self.keycloak_configuration.client_id,
             realm_name=self.keycloak_configuration.realm,
@@ -78,31 +73,26 @@
         """
         return FastApiUser(
             first_name=userinfo.get("given_name", ""),
             last_name=userinfo.get("family_name", ""),
             user_id=userinfo.get("user_id", ""),
         )
 
-    async def authenticate(
-        self, conn: HTTPConnection
-    ) -> Tuple[AuthCredentials, BaseUser]:
+    async def authenticate(self, conn: HTTPConnection) -> tuple[AuthCredentials, BaseUser | None]:
         """
         The authenticate method is invoked each time a route is called that
         the middleware is applied to.
         """
         if "Authorization" not in conn.headers:
             raise AuthHeaderMissing
 
         # Check if token starts with the authentication scheme
         auth_header = conn.headers["Authorization"]
         token = auth_header.split(" ")
-        if (
-            len(token) != 2
-            or token[0] != self.keycloak_configuration.authentication_scheme
-        ):
+        if len(token) != 2 or token[0] != self.keycloak_configuration.authentication_scheme:
             raise AuthInvalidToken
 
         token_info = None
 
         # Depending on the chosen method by the user, either
         # use the introspection endpoint or decode the token
         if self.keycloak_configuration.use_introspection_endpoint:
@@ -135,41 +125,33 @@
         if (
             self.keycloak_configuration.enable_device_authentication
             and self.keycloak_configuration.device_authentication_claim in token_info
         ):
             # ...only add the device auth claim to the claims to extract
             claims = [self.keycloak_configuration.device_authentication_claim]
             # If claim based authorization is enabled...
-            if (
-                self.keycloak_configuration.authorization_method
-                == AuthorizationMethod.CLAIM
-            ):
+            if self.keycloak_configuration.authorization_method == AuthorizationMethod.CLAIM:
                 # ...add the authorization claim to the claims to extract
                 claims.append(self.keycloak_configuration.authorization_claim)
 
         # Extract claims from token
         user_info = {}
         for claim in claims:
             try:
                 user_info[claim] = token_info[claim]
             except KeyError:
                 log.warning("Claim %s is configured but missing in the token", claim)
                 if self.keycloak_configuration.reject_on_missing_claim:
                     log.warning("Rejecting request because of missing claim")
                     raise AuthClaimMissing from KeyError
-                log.debug(
-                    "Backend is configured to ignore missing claims, continuing..."
-                )
+                log.debug("Backend is configured to ignore missing claims, continuing...")
 
         # Handle Authorization depending on the Claim Method
-        scope_auth = []
-        if (
-            self.keycloak_configuration.authorization_method
-            == AuthorizationMethod.CLAIM
-        ):
+        scope_auth = None
+        if self.keycloak_configuration.authorization_method == AuthorizationMethod.CLAIM:
             if self.keycloak_configuration.authorization_claim not in token_info:
                 raise AuthClaimMissing
             scope_auth = token_info[self.keycloak_configuration.authorization_claim]
 
         # Check if the device authentication claim is present and evaluated to true
         # If so, the rest (mapping claims, user mapper, authorization) is skipped
         if self.keycloak_configuration.enable_device_authentication:
```

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/middleware.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,29 @@
         the user of this library, defaults to None
     :type user_mapper:
         typing.Callable[ [typing.Dict[str, typing.Any]], typing.Awaitable[typing.Any] ]
         optional
     :param scope_mapper: Custom async function that transforms the claim values
         extracted from the token to permissions meaningful for your application,
         defaults to None
-    :type scope_mapper: typing.Callable[[typing.List[str]], typing.List[str]], optional
+    :type scope_mapper:
+        typing.Callable[[typing.List[str]], typing.Awaitable[typing.List[str]]], optional
     """
 
     def __init__(
         self,
         app: ASGIApp,
         keycloak_configuration: KeycloakConfiguration,
         exclude_patterns: typing.List[str] = None,
         user_mapper: typing.Callable[
             [typing.Dict[str, typing.Any]], typing.Awaitable[typing.Any]
         ] = None,
-        scope_mapper: typing.Callable[[typing.List[str]], typing.List[str]] = None,
+        scope_mapper: typing.Callable[
+            [typing.List[str]], typing.Awaitable[typing.List[str]]
+        ] = None,
     ):
         """Middleware constructor"""
         log.info("Initializing Keycloak Middleware")
         self.app = app
         self.backend: KeycloakBackend = KeycloakBackend(
             keycloak_configuration=keycloak_configuration,
             user_mapper=user_mapper,
@@ -204,10 +207,8 @@
         )
 
     @staticmethod
     def _invalid_token(*args, **kwargs):  # pylint: disable=unused-argument
         """
         Returns a response notifying the user that the acess token is invalid.
         """
-        return JSONResponse(
-            {"detail": "Unable to verify provided access token"}, status_code=401
-        )
+        return JSONResponse({"detail": "Unable to verify provided access token"}, status_code=401)
```

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/authorization_methods.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/authorization_methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/authorization_result.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/authorization_result.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/keycloak_configuration.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/keycloak_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 This module contains the schema to configure Keycloak.
 """
 
-from typing import Dict, Optional, Union
+from typing import Optional, Union
 
 from pydantic import BaseModel, Field
 
 from fastapi_keycloak_middleware.schemas.authorization_methods import (
     AuthorizationMethod,
 )
 
 
 class KeycloakConfiguration(BaseModel):  # pylint: disable=too-few-public-methods
     """
-    This is a Pydantic schema used to pass backend konfiguration
+    This is a Pydantic schema used to pass backend configuration
     for the Keycloak Backend to the middleware.
 
     :param realm: Keycloak realm that should be used for token authentication.
     :type realm: str
     :param url: URL of the Keycloak server. If you use legacy Keycloak versions
         or still have the auth context, you need to add the auth context to the URL.
     :type url: str
@@ -66,15 +66,15 @@
     :type decode_options: Dict[str, Union[bool,int]], optional
     """
 
     realm: str = Field(title="Realm", description="The realm to use.")
     url: str = Field(title="URL", description="The URL of the Keycloak server.")
     client_id: str = Field(title="Client ID", description="The client ID.")
     swagger_client_id: Optional[str] = Field(
-        title="Swagger Client ID", description="The client ID for the swagger UI."
+        default=None, title="Swagger Client ID", description="The client ID for the swagger UI."
     )
     client_secret: Optional[str] = Field(
         default=None, title="Client Secret", description="The client secret."
     )
     claims: list[str] = Field(
         default=[
             "sub",
@@ -127,15 +127,15 @@
         " true, the device authentication will be applied for the request.",
     )
     verify: Union[bool, str] = Field(
         default=True,
         title="Verify",
         description="Whether to verify the SSL connection",
     )
-    decode_options: Dict[str, Union[bool, int]] = Field(
+    decode_options: dict[str, Union[bool, int]] = Field(
         default={
             "verify_signature": True,
             "verify_aud": True,
             "verify_exp": True,
         },
         title="JWT Decode Options",
         description="Decode options that are passed to python-jose decode function.",
```

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/match_strategy.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/match_strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/setup.py` & `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def setup_keycloak_middleware(  # pylint: disable=too-many-arguments
     app: FastAPI,
     keycloak_configuration: KeycloakConfiguration,
     exclude_patterns: typing.List[str] = None,
     user_mapper: typing.Callable[
         [typing.Dict[str, typing.Any]], typing.Awaitable[typing.Any]
     ] = None,
-    scope_mapper: typing.Callable[[typing.List[str]], typing.List[str]] = None,
+    scope_mapper: typing.Callable[[typing.List[str]], typing.Awaitable[typing.List[str]]] = None,
     add_exception_response: bool = True,
     add_swagger_auth: bool = False,
     swagger_auth_scopes: typing.List[str] = None,
     swagger_auth_pkce: bool = True,
     swagger_scheme_name: str = "keycloak-openid",
 ):
     """
@@ -93,28 +93,26 @@
             log.debug("Adding 401 exception response")
             router.responses[401] = {
                 "description": "Unauthorized",
                 "model": ExceptionResponse,
             }
         else:
             log.warning(
-                "Middleware is configured to add 401 exception"
-                " response but it already exists"
+                "Middleware is configured to add 401 exception" " response but it already exists"
             )
 
         if 403 not in router.responses:
             log.debug("Adding 403 exception response")
             router.responses[403] = {
                 "description": "Forbidden",
                 "model": ExceptionResponse,
             }
         else:
             log.warning(
-                "Middleware is configured to add 403 exception"
-                " response but it already exists"
+                "Middleware is configured to add 403 exception" " response but it already exists"
             )
     else:
         log.debug("Skipping adding exception responses")
 
     # Add OpenAPI schema
     if add_swagger_auth:
         suffix = "/.well-known/openid-configuration"
```

### Comparing `fastapi_keycloak_middleware-0.4.0/setup.py` & `fastapi_keycloak_middleware-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,24 @@
  'fastapi_keycloak_middleware.dependencies',
  'fastapi_keycloak_middleware.schemas']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.73.0', 'install>=1.3.5,<2.0.0', 'python-keycloak>2.14.0,<3.9.1']
+['fastapi>=0.73.0',
+ 'install>=1.3.5,<2.0.0',
+ 'python-keycloak>2.14.0,<3.9.1',
+ 'ruff>=0.4.2,<0.5.0']
 
 setup_kwargs = {
     'name': 'fastapi-keycloak-middleware',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Middleware for FastAPI to authenticate a user against keycloak',
-    'long_description': '[![Documentation Status](https://readthedocs.org/projects/fastapi-keycloak-middleware/badge/?version=latest)](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/?badge=latest)\n[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)\n![GitHub issues](https://img.shields.io/github/issues/waza-ari/fastapi-keycloak-middleware)\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/waza-ari/fastapi-keycloak-middleware)\n![GitHub top language](https://img.shields.io/github/languages/top/waza-ari/fastapi-keycloak-middleware)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/waza-ari/fastapi-keycloak-middleware/development.svg)](https://results.pre-commit.ci/latest/github/waza-ari/fastapi-keycloak-middleware/development)\n\n\n# FastAPI Keycloak Middleware\n\n**Full documentation** is [available at Read The Docs](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/)\n\nThis package provides a middleware for [FastAPI](http://fastapi.tiangolo.com)  that\nsimplifies integrating with [Keycloak](http://keycloak.org) for\nauthentication and authorization. It supports OIDC and supports validating access\ntokens, reading roles and basic authentication. In addition it provides several\ndecorators and dependencies to easily integrate into your FastAPI application.\n\nIt relies on the [python-keycloak](http://python-keycloak.readthedocs.io) package,\nwhich is the only dependency outside of the FastAPI ecosystem which would be installed\nanyway. Shoutout to the author of [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich served as inspiration for this package and some of its code.\n\nIn the future, I plan to add support for fine grained authorization using Keycloak\nAuthorization services.\n\n## Motivation\n\nUsing FastAPI and Keycloak quite a lot, and keeping to repeat myself quite a lot when\nit comes to authentiating users, I decided to create this library to help with this.\n\nThere is a clear separation between the authentication and authorization:\n\n- **Authentication** is about verifying the identity of the user\n  (who they are). This is done by an authentication backend\n  that verifies the users access token obtained from the\n  identity provider (Keycloak in this case).\n- **Authorization** is about deciding which resources can be\n  accessed. This package providers convenience decoraters to\n  enforce certain roles or permissions on FastAPI endpoints.\n\n## Installation\n\nInstall the package using poetry:\n\n```bash\npoetry add fastapi-keycloak-middleware\n```\n\nor `pip`:\n\n```bash\npip install fastapi-keycloak-middleware\n```\n\n## Features\n\nThe package helps with:\n\n* An easy to use middleware that validates the request for an access token\n* Validation can done in one of two ways:\n   * Validate locally using the public key obtained from Keycloak\n   * Validate using the Keycloak token introspection endpoint\n* Using Starlette authentication mechanisms to store both the user object as well as the authorization scopes in the Request object\n* Ability to provide custom callback functions to retrieve the user object (e.g. from your database) and to provide an arbitrary mapping to authentication scopes (e.g. roles to permissions)\n* A decorator to use previously stored information to enforce certain roles or permissions on FastAPI endpoints\n* Convenience dependencies to retrieve the user object or the authorization result after evaluation within the FastAPI endpoint\n\n## Acknowledgements\n\nThis package is heavily inspired by [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich provides some of the same functionality but without the direct integration\ninto Keycloak. Thanks for writing and providing this great piece of software!\n\n## Development\n\nThis project is using [Act](https://github.com/nektos/act) to handle local development tasks. It is used\nto work locally and also to test Github actions before deploying them.\n',
+    'long_description': '[![Documentation Status](https://readthedocs.org/projects/fastapi-keycloak-middleware/badge/?version=latest)](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/?badge=latest)\n[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)\n![GitHub issues](https://img.shields.io/github/issues/waza-ari/fastapi-keycloak-middleware)\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/waza-ari/fastapi-keycloak-middleware)\n![GitHub top language](https://img.shields.io/github/languages/top/waza-ari/fastapi-keycloak-middleware)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/waza-ari/fastapi-keycloak-middleware/development.svg)](https://results.pre-commit.ci/latest/github/waza-ari/fastapi-keycloak-middleware/development)\n\n\n# FastAPI Keycloak Middleware\n\n**Full documentation** is [available at Read The Docs](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/)\n\nThis package provides a middleware for [FastAPI](http://fastapi.tiangolo.com)  that\nsimplifies integrating with [Keycloak](http://keycloak.org) for\nauthentication and authorization. It supports OIDC and supports validating access\ntokens, reading roles and basic authentication. In addition it provides several\ndecorators and dependencies to easily integrate into your FastAPI application.\n\nIt relies on the [python-keycloak](http://python-keycloak.readthedocs.io) package,\nwhich is the only dependency outside of the FastAPI ecosystem which would be installed\nanyway. Shoutout to the author of [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich served as inspiration for this package and some of its code.\n\nIn the future, I plan to add support for fine grained authorization using Keycloak\nAuthorization services.\n\n## Motivation\n\nUsing FastAPI and Keycloak quite a lot, and keeping to repeat myself quite a lot when\nit comes to authentiating users, I decided to create this library to help with this.\n\nThere is a clear separation between the authentication and authorization:\n\n- **Authentication** is about verifying the identity of the user\n  (who they are). This is done by an authentication backend\n  that verifies the users access token obtained from the\n  identity provider (Keycloak in this case).\n- **Authorization** is about deciding which resources can be\n  accessed. This package providers convenience decoraters to\n  enforce certain roles or permissions on FastAPI endpoints.\n\n## Installation\n\nInstall the package using poetry:\n\n```bash\npoetry add fastapi-keycloak-middleware\n```\n\nor `pip`:\n\n```bash\npip install fastapi-keycloak-middleware\n```\n\n## Features\n\nThe package helps with:\n\n* An easy to use middleware that validates the request for an access token\n* Validation can done in one of two ways:\n   * Validate locally using the public key obtained from Keycloak\n   * Validate using the Keycloak token introspection endpoint\n* Using Starlette authentication mechanisms to store both the user object as well as the authorization scopes in the Request object\n* Ability to provide custom callback functions to retrieve the user object (e.g. from your database) and to provide an arbitrary mapping to authentication scopes (e.g. roles to permissions)\n* A decorator to use previously stored information to enforce certain roles or permissions on FastAPI endpoints\n* Convenience dependencies to retrieve the user object or the authorization result after evaluation within the FastAPI endpoint\n\n## Acknowledgements\n\nThis package is heavily inspired by [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich provides some of the same functionality but without the direct integration\ninto Keycloak. Thanks for writing and providing this great piece of software!\n\n## Contributing\n\nThe client is written in pure Python.\nAny changes or pull requests are more than welcome, but please adhere to the code style.\n\nRuff is used both for code formatting and linting. Before committing, please run the following command to ensure\nthat your code is properly formatted:\n\n```bash\nruff check .\nruff format .\n```\n\nA pre-commit hook configuration is supplied as part of the project.\n\n## Development\n\nThis project is using [Act](https://github.com/nektos/act) to handle local development tasks. It is used\nto work locally and also to test Github actions before deploying them.\n',
     'author': 'Daniel Herrmann',
     'author_email': 'daniel.herrmann1@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastapi_keycloak_middleware-0.4.0/PKG-INFO` & `fastapi_keycloak_middleware-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: fastapi-keycloak-middleware
-Version: 0.4.0
+Version: 0.4.1
 Summary: Middleware for FastAPI to authenticate a user against keycloak
 Author: Daniel Herrmann
 Author-email: daniel.herrmann1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.73.0)
 Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: python-keycloak (>2.14.0,<3.9.1)
+Requires-Dist: ruff (>=0.4.2,<0.5.0)
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/fastapi-keycloak-middleware/badge/?version=latest)](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 ![GitHub issues](https://img.shields.io/github/issues/waza-ari/fastapi-keycloak-middleware)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/waza-ari/fastapi-keycloak-middleware)
 ![GitHub top language](https://img.shields.io/github/languages/top/waza-ari/fastapi-keycloak-middleware)
@@ -83,12 +84,27 @@
 
 ## Acknowledgements
 
 This package is heavily inspired by [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)
 which provides some of the same functionality but without the direct integration
 into Keycloak. Thanks for writing and providing this great piece of software!
 
+## Contributing
+
+The client is written in pure Python.
+Any changes or pull requests are more than welcome, but please adhere to the code style.
+
+Ruff is used both for code formatting and linting. Before committing, please run the following command to ensure
+that your code is properly formatted:
+
+```bash
+ruff check .
+ruff format .
+```
+
+A pre-commit hook configuration is supplied as part of the project.
+
 ## Development
 
 This project is using [Act](https://github.com/nektos/act) to handle local development tasks. It is used
 to work locally and also to test Github actions before deploying them.
```

