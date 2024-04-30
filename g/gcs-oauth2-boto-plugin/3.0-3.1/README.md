# Comparing `tmp/gcs-oauth2-boto-plugin-3.0.tar.gz` & `tmp/gcs-oauth2-boto-plugin-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcs-oauth2-boto-plugin-3.0.tar", last modified: Tue Sep 21 20:36:56 2021, max compression
+gzip compressed data, was "gcs-oauth2-boto-plugin-3.1.tar", last modified: Tue Apr 30 15:32:50 2024, max compression
```

## Comparing `gcs-oauth2-boto-plugin-3.0.tar` & `gcs-oauth2-boto-plugin-3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 thomasmaclean (630336) primarygroup (89939)        0 2021-09-21 20:36:56.385892 gcs-oauth2-boto-plugin-3.0/
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)    11359 2021-09-08 20:09:39.000000 gcs-oauth2-boto-plugin-3.0/LICENSE
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)       16 2021-09-08 20:09:39.000000 gcs-oauth2-boto-plugin-3.0/MANIFEST.in
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)     1553 2021-09-21 20:36:56.385892 gcs-oauth2-boto-plugin-3.0/PKG-INFO
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)     2222 2021-09-08 20:09:39.000000 gcs-oauth2-boto-plugin-3.0/README.md
-drwxr-x---   0 thomasmaclean (630336) primarygroup (89939)        0 2021-09-21 20:36:56.381892 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)     1542 2021-09-08 20:09:39.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/__init__.py
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)    29061 2021-09-08 20:09:39.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/oauth2_client.py
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)     8540 2021-09-08 20:09:39.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/oauth2_helper.py
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)     2736 2021-09-08 20:09:39.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/oauth2_plugin.py
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)    12943 2021-09-08 20:09:39.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/test_oauth2_client.py
-drwxr-x---   0 thomasmaclean (630336) primarygroup (89939)        0 2021-09-21 20:36:56.385892 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)     1553 2021-09-21 20:36:56.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/PKG-INFO
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)      518 2021-09-21 20:36:56.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/SOURCES.txt
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)        1 2021-09-21 20:36:56.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/dependency_links.txt
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)      183 2021-09-21 20:36:56.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/requires.txt
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)       23 2021-09-21 20:36:56.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/top_level.txt
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)        1 2021-09-21 18:01:09.000000 gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/zip-safe
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)       74 2021-09-21 20:36:56.385892 gcs-oauth2-boto-plugin-3.0/setup.cfg
--rw-r-----   0 thomasmaclean (630336) primarygroup (89939)     2935 2021-09-21 20:34:58.000000 gcs-oauth2-boto-plugin-3.0/setup.py
+drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-04-30 15:32:50.186235 gcs-oauth2-boto-plugin-3.1/
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)    11359 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/LICENSE
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)       16 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/MANIFEST.in
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     1506 2024-04-30 15:32:50.186235 gcs-oauth2-boto-plugin-3.1/PKG-INFO
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     2222 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/README.md
+drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-04-30 15:32:50.182235 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     1542 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/__init__.py
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)    32344 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_client.py
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     8540 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_helper.py
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     2736 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_plugin.py
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)    14135 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/test_oauth2_client.py
+drwxr-xr-x   0 margubur (1016367) primarygroup (89939)        0 2024-04-30 15:32:50.186235 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     1506 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)      518 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)        1 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)      183 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/requires.txt
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)       23 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/top_level.txt
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)        1 2024-04-30 15:32:50.000000 gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/zip-safe
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)       74 2024-04-30 15:32:50.186235 gcs-oauth2-boto-plugin-3.1/setup.cfg
+-rw-r--r--   0 margubur (1016367) primarygroup (89939)     2935 2024-04-30 09:50:35.000000 gcs-oauth2-boto-plugin-3.1/setup.py
```

### Comparing `gcs-oauth2-boto-plugin-3.0/LICENSE` & `gcs-oauth2-boto-plugin-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.0/PKG-INFO` & `gcs-oauth2-boto-plugin-3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: gcs-oauth2-boto-plugin
-Version: 3.0
+Version: 3.1
 Summary: Auth plugin allowing use the use of OAuth 2.0 credentials for Google Cloud Storage in the Boto library.
 Home-page: https://developers.google.com/storage/docs/gspythonlibrary
+Download-URL: https://github.com/GoogleCloudPlatform/gcs-oauth2-boto-plugin
 Author: Google Inc.
 Author-email: gs-team@google.com
 License: Apache 2.0
-Download-URL: https://github.com/GoogleCloudPlatform/gcs-oauth2-boto-plugin
-Description: 
-        gcs-oauth2-boto-plugin is a Python application whose purpose is to behave as an
-        auth plugin for the boto auth plugin framework for use with OAuth 2.0
-        credentials for the Google Cloud Platform. This plugin is compatible with both
-        user accounts and service accounts, and its functionality is essentially a
-        wrapper around oauth2client with the addition of automatically caching tokens
-        for the machine in a thread- and process-safe fashion.
-        
 Platform: any
 Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
+License-File: LICENSE
+
+
+gcs-oauth2-boto-plugin is a Python application whose purpose is to behave as an
+auth plugin for the boto auth plugin framework for use with OAuth 2.0
+credentials for the Google Cloud Platform. This plugin is compatible with both
+user accounts and service accounts, and its functionality is essentially a
+wrapper around oauth2client with the addition of automatically caching tokens
+for the machine in a thread- and process-safe fashion.
```

### Comparing `gcs-oauth2-boto-plugin-3.0/README.md` & `gcs-oauth2-boto-plugin-3.1/README.md`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/__init__.py` & `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/oauth2_client.py` & `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 # pylint: disable=g-bad-import-order
 import boto
 import httplib2
 import oauth2client.client
 import oauth2client.service_account
 from google_reauth import reauth_creds
 import retry_decorator.retry_decorator
+from google.auth import _helpers
+from google.auth.crypt import base as crypt_base
+from google_auth_httplib2 import Request as GoogleAuthRequest
+from google_auth_httplib2 import AuthorizedHttp
+from google.oauth2 import service_account
 
 import six
 from six import BytesIO
 from six.moves import urllib
 
 LOG = logging.getLogger('oauth2_client')
 
@@ -63,14 +68,15 @@
 # operation doesn't attempt concurrent refreshes.
 token_exchange_lock = threading.Lock()
 
 CLOUD_PLATFORM_SCOPE = 'https://www.googleapis.com/auth/cloud-platform'
 FULL_CONTROL_SCOPE = 'https://www.googleapis.com/auth/devstorage.full_control'
 REAUTH_SCOPE = 'https://www.googleapis.com/auth/accounts.reauth'
 DEFAULT_SCOPE = FULL_CONTROL_SCOPE
+GOOGLE_OAUTH2_DEFAULT_FILE_PASSWORD = 'notasecret'
 # Note that these scopes don't necessarily correspond to the refresh token
 # being used. This list is is used for obtaining the RAPT in the reauth
 # flow, to determine which challenges should be used. We define this at module
 # level to allow us to override it for other applications if needed.
 RAPT_SCOPES = [CLOUD_PLATFORM_SCOPE, REAUTH_SCOPE]
 
 METADATA_SERVER = 'http://metadata.google.internal'
@@ -264,14 +270,96 @@
                   cache_file, e)
 
     LOG.debug('FileSystemTokenCache.GetToken: key=%s%s present (cache_file=%s)',
               key, ' not' if value is None else '', cache_file)
     return value
 
 
+class PKCS12Signer(crypt_base.Signer, crypt_base.FromServiceAccountMixin):
+  """Signer for a p12 service account key."""
+
+  def __init__(self, key):
+    self._key = key
+
+  # Defined in crypt_base.Signer interface.
+  # It is not used by p12 service account keys.
+  @property
+  def key_id(self):
+    return None
+
+  def sign(self, message):
+    message = _helpers.to_bytes(message)
+    from google.auth.crypt import _cryptography_rsa  # pylint: disable=g-import-not-at-top
+    return self._key.sign(
+        message,
+        _cryptography_rsa._PADDING,  # pylint: disable=protected-access
+        _cryptography_rsa._SHA256)  # pylint: disable=protected-access
+
+  @classmethod
+  def from_string(cls, key_strings, key_id=None):
+    del key_id #Unused
+    key_string, password = (_helpers.to_bytes(k) for k in key_strings)
+    # Cryptography package is not bundled with gsutil, Keeping it at top would throw error.
+    from cryptography.hazmat.primitives.serialization import pkcs12  # pylint: disable=g-import-not-at-top
+    try:
+      key, _, _ = pkcs12.load_key_and_certificates(key_string, password)
+      return cls(key)
+    except:
+      raise GsInvalidRefreshTokenError('Unable to load the keyfile, Invalid password or PKCS12 data.')
+
+
+class P12Credentials(service_account.Credentials):
+  """google-auth service account credentials  for p12 keys.
+  p12 keys are not supported by the google-auth service account credentials.
+  gsutil uses oauth2client to support p12 key users. Since oauth2client was
+  deprecated and bundling it is security concern, we decided to support p12
+  in gsutil codebase. We prefer not adding it to the google-auth library
+  because p12 is not supported from the beginning by google-auth. GCP strongly
+  suggests users to use the JSON format. gsutil has to support it to not
+  break users.
+  """
+
+  _REQUIRED_FIELDS = ('service_account_email', 'token_uri', 'scopes')
+
+  def authorize(self, http):
+    return AuthorizedHttp(self, http=http)
+
+  @property
+  def access_token(self):
+    return self.token
+
+  @property
+  def token_expiry(self):
+    return self.expiry
+
+  @classmethod
+  def from_service_account_pkcs12_keystring(cls,
+                                            key_string,
+                                            password=None,
+                                            **kwargs):
+    password = password or GOOGLE_OAUTH2_DEFAULT_FILE_PASSWORD
+    signer = PKCS12Signer.from_string((key_string, password))
+
+    missing_fields = [f for f in cls._REQUIRED_FIELDS if f not in kwargs]
+    if missing_fields:
+      raise MissingFieldsError('Missing fields: {}.'.format(
+          ', '.join(missing_fields)))
+    creds = cls(signer, **kwargs)
+    return creds
+
+def CreateP12ServiceAccountCredentials(key_string, password=None, **kwargs):
+  """Creates a service account credentials from a p12 key and handles import errors."""
+  try:
+    return P12Credentials.from_service_account_pkcs12_keystring(
+        key_string, password, **kwargs)
+  except ImportError:
+      raise MissingDependencyError(
+          ('pyca/cryptography is not available. Either install it, or please consider using the .json keyfile'))
+
+
 class OAuth2Client(object):
   """Common logic for OAuth2 clients."""
 
   def __init__(self, cache_key_base, access_token_cache=None,
                datetime_strategy=datetime.datetime, auth_uri=None,
                token_uri=None, disable_ssl_certificate_validation=False,
                proxy_host=None, proxy_port=None, proxy_user=None,
@@ -400,16 +488,18 @@
         disable_ssl_certificate_validation=disable_ssl_certificate_validation,
         proxy_host=proxy_host, proxy_port=proxy_port, proxy_user=proxy_user,
         proxy_pass=proxy_pass, ca_certs_file=ca_certs_file)
     self._client_id = client_id
 
   def FetchAccessToken(self, rapt_token=None):
     credentials = self.GetCredentials()
-    http = self.CreateHttpRequest()
-    credentials.refresh(http)
+    request = self.CreateHttpRequest()
+    if isinstance(credentials, P12Credentials):
+      request = GoogleAuthRequest(request)
+    credentials.refresh(request)
     return AccessToken(credentials.access_token, credentials.token_expiry,
                        datetime_strategy=self.datetime_strategy,
                        rapt_token=rapt_token)
 
 
 class OAuth2ServiceAccountClient(_BaseOAuth2ServiceAccountClient):
   """An OAuth2 service account client using .p12 or .pem keys."""
@@ -444,27 +534,15 @@
         proxy_user=proxy_user,
         proxy_pass=proxy_pass,
         ca_certs_file=ca_certs_file)
     self._private_key = private_key
     self._password = password
 
   def GetCredentials(self):
-    if oauth2client.client.HAS_CRYPTO:
-      # pylint: disable=protected-access
-      return _ServiceAccountCredentials.from_p12_keyfile_buffer(
-          self._client_id,
-          BytesIO(self._private_key),
-          private_key_password=self._password,
-          scopes=DEFAULT_SCOPE,
-          token_uri=self.token_uri)
-      # pylint: enable=protected-access
-    else:
-      raise MissingDependencyError(
-          'Service account authentication requires PyOpenSSL. Please install '
-          'this library and try again.')
+    return CreateP12ServiceAccountCredentials(self._private_key, self._password, scopes=[DEFAULT_SCOPE], service_account_email=self._client_id, token_uri=self.token_uri)
 
 
 class OAuth2JsonServiceAccountClient(_BaseOAuth2ServiceAccountClient):
   """An OAuth2 service account client using .json keys."""
 
   def __init__(self, json_key_dict, access_token_cache=None, auth_uri=None,
                token_uri=None, datetime_strategy=datetime.datetime,
@@ -524,14 +602,20 @@
 
 class MissingDependencyError(Exception):
 
   def __init__(self, e):
     super(MissingDependencyError, self).__init__(e)
 
 
+class MissingFieldsError(Exception):
+
+  def __init__(self, e):
+    super(MissingFieldsError, self).__init__(e)
+
+
 class OAuth2UserAccountClient(OAuth2Client):
   """An OAuth2 client."""
 
   def __init__(self, token_uri, client_id, client_secret, refresh_token,
                auth_uri=None, access_token_cache=None,
                datetime_strategy=datetime.datetime,
                disable_ssl_certificate_validation=False,
```

### Comparing `gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/oauth2_helper.py` & `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_helper.py`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/oauth2_plugin.py` & `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/oauth2_plugin.py`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin/test_oauth2_client.py` & `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin/test_oauth2_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -170,14 +170,42 @@
     # This should have resulted in a refresh request and a fresh access token.
     self.assertTrue(self.client.fetched_token)
     self.assertEqual(
         self.mock_datetime.mock_now + datetime.timedelta(minutes=60),
         token_3.expiry)
     self.assertEqual(token_3.rapt_token, expected_rapt)
 
+class TestCreateP12ServiceAccountCredentials(unittest.TestCase):
+  
+  @mock.patch.object(oauth2_client.PKCS12Signer, 'from_string')
+  def test_from_service_account_pkcs12_keystring(self, mock_signer):
+    mock_signer.return_value = 'MOCK_SIGNER'
+    with mock.patch.object(oauth2_client.P12Credentials, '__init__') as mock_p12creds:
+      mock_p12creds.return_value = None
+      oauth2_client.P12Credentials.from_service_account_pkcs12_keystring(
+        'MY_KEY',
+        service_account_email='test@google.com',
+        token_uri= 'TOKEN_URI',
+        scopes= ['MYSCOPEEEEE']
+      )
+      mock_p12creds.assert_called_once_with('MOCK_SIGNER', service_account_email='test@google.com',
+        token_uri= 'TOKEN_URI',
+        scopes= ['MYSCOPEEEEE'])
+
+  @mock.patch.object(oauth2_client.PKCS12Signer, 'from_string')
+  def test_from_service_account_pkcs12_keystring_raises_missing_field(self, mock_signer):
+    mock_signer.return_value = 'MOCK_SIGNER'
+    with self.assertRaises(oauth2_client.MissingFieldsError) as exc:
+      oauth2_client.P12Credentials.from_service_account_pkcs12_keystring(
+        'MY_KEY',
+        token_uri= 'TOKEN_URI',
+        scopes= ['MYSCOPEEEEE']
+      )
+      
+
 
 class AccessTokenTest(unittest.TestCase):
   """Unit tests for access token functions."""
 
   def testShouldRefresh(self):
     """Tests that token.ShouldRefresh returns the correct value."""
     mock_datetime = MockDateTime()
```

### Comparing `gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/PKG-INFO` & `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: gcs-oauth2-boto-plugin
-Version: 3.0
+Version: 3.1
 Summary: Auth plugin allowing use the use of OAuth 2.0 credentials for Google Cloud Storage in the Boto library.
 Home-page: https://developers.google.com/storage/docs/gspythonlibrary
+Download-URL: https://github.com/GoogleCloudPlatform/gcs-oauth2-boto-plugin
 Author: Google Inc.
 Author-email: gs-team@google.com
 License: Apache 2.0
-Download-URL: https://github.com/GoogleCloudPlatform/gcs-oauth2-boto-plugin
-Description: 
-        gcs-oauth2-boto-plugin is a Python application whose purpose is to behave as an
-        auth plugin for the boto auth plugin framework for use with OAuth 2.0
-        credentials for the Google Cloud Platform. This plugin is compatible with both
-        user accounts and service accounts, and its functionality is essentially a
-        wrapper around oauth2client with the addition of automatically caching tokens
-        for the machine in a thread- and process-safe fashion.
-        
 Platform: any
 Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
+License-File: LICENSE
+
+
+gcs-oauth2-boto-plugin is a Python application whose purpose is to behave as an
+auth plugin for the boto auth plugin framework for use with OAuth 2.0
+credentials for the Google Cloud Platform. This plugin is compatible with both
+user accounts and service accounts, and its functionality is essentially a
+wrapper around oauth2client with the addition of automatically caching tokens
+for the machine in a thread- and process-safe fashion.
```

### Comparing `gcs-oauth2-boto-plugin-3.0/gcs_oauth2_boto_plugin.egg-info/SOURCES.txt` & `gcs-oauth2-boto-plugin-3.1/gcs_oauth2_boto_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcs-oauth2-boto-plugin-3.0/setup.py` & `gcs-oauth2-boto-plugin-3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'freezegun',
         'mock;python_version<"3.3"',
     ],
 }
 
 setup(
     name='gcs-oauth2-boto-plugin',
-    version='3.0',
+    version='3.1',
     url='https://developers.google.com/storage/docs/gspythonlibrary',
     download_url=('https://github.com/GoogleCloudPlatform'
                   '/gcs-oauth2-boto-plugin'),
     license='Apache 2.0',
     author='Google Inc.',
     author_email='gs-team@google.com',
     description=('Auth plugin allowing use the use of OAuth 2.0 credentials '
```

