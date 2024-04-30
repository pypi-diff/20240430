# Comparing `tmp/streamlit-ldap-authenticator-0.2.5.tar.gz` & `tmp/streamlit-ldap-authenticator-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-ldap-authenticator-0.2.5.tar", last modified: Sat Apr 27 03:20:18 2024, max compression
+gzip compressed data, was "streamlit-ldap-authenticator-0.2.6.tar", last modified: Tue Apr 30 16:51:42 2024, max compression
```

## Comparing `streamlit-ldap-authenticator-0.2.5.tar` & `streamlit-ldap-authenticator-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 03:20:18.297975 streamlit-ldap-authenticator-0.2.5/
--rw-rw-rw-   0        0        0     1089 2024-02-29 23:36:46.000000 streamlit-ldap-authenticator-0.2.5/LICENSE
--rw-rw-rw-   0        0        0    23758 2024-04-27 03:20:18.297086 streamlit-ldap-authenticator-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    22743 2024-04-27 03:20:04.000000 streamlit-ldap-authenticator-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 03:20:18.298976 streamlit-ldap-authenticator-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1505 2024-04-27 03:18:41.000000 streamlit-ldap-authenticator-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:20:18.284974 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/
--rw-rw-rw-   0        0        0      308 2024-03-27 14:06:56.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/__init__.py
--rw-rw-rw-   0        0        0    18526 2024-04-27 03:17:12.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/authenticate.py
--rw-rw-rw-   0        0        0    10671 2024-04-27 03:17:16.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/configs.py
--rw-rw-rw-   0        0        0      971 2024-02-29 23:36:46.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/exceptions.py
--rw-rw-rw-   0        0        0     7428 2024-04-27 03:07:29.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/ldap_authenticate.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:20:18.293974 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/
--rw-rw-rw-   0        0        0    23758 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      231 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-27 03:20:18.000000 streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:51:42.640176 streamlit-ldap-authenticator-0.2.6/
+-rw-rw-rw-   0        0        0     1089 2024-02-29 23:36:46.000000 streamlit-ldap-authenticator-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0    23956 2024-04-30 16:51:42.638160 streamlit-ldap-authenticator-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    22941 2024-04-30 16:38:36.000000 streamlit-ldap-authenticator-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:51:42.640176 streamlit-ldap-authenticator-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1505 2024-04-30 16:21:39.000000 streamlit-ldap-authenticator-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:51:42.627156 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/
+-rw-rw-rw-   0        0        0      308 2024-03-27 14:06:56.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/__init__.py
+-rw-rw-rw-   0        0        0    18526 2024-04-30 16:51:26.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/authenticate.py
+-rw-rw-rw-   0        0        0    11040 2024-04-30 16:37:53.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/configs.py
+-rw-rw-rw-   0        0        0      971 2024-02-29 23:36:46.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/exceptions.py
+-rw-rw-rw-   0        0        0     7428 2024-04-27 03:07:29.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/ldap_authenticate.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:51:42.635151 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator.egg-info/
+-rw-rw-rw-   0        0        0    23956 2024-04-30 16:51:42.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-04-30 16:51:42.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:51:42.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      231 2024-04-30 16:51:42.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-30 16:51:42.000000 streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator.egg-info/top_level.txt
```

### Comparing `streamlit-ldap-authenticator-0.2.5/LICENSE` & `streamlit-ldap-authenticator-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.5/PKG-INFO` & `streamlit-ldap-authenticator-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-ldap-authenticator
-Version: 0.2.5
+Version: 0.2.6
 Summary: Authenticate using ldap
 Home-page: https://github.com/NathanChen198/streamlit-ldap-authenticator
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,14 +87,15 @@
 remember_me = "login_remember_me"
 
 [auth_cookie]
 name = "login_cookie"
 key = "{any password for encryption}"
 expiry_days = 1
 auto_renewal = true
+delay_sec = 0.1
 ```
 
 Create a new file simple_login.py with the following code:
 
 ```python
 import streamlit as st
 from streamlit_ldap_authenticator import Authenticate
@@ -202,14 +203,15 @@
 Configuration to store user information to the cookie in client's browser. Thus even when user close the browser and reload the page, Reauthorization is possible with cookie.
 | Name | Type | Description
 | ------------ | ----- | -----------
 | name | str | cookie name to store in client's browser
 | key | str | encryption key to encrypt user information
 | expiry_days | float | expiry date for the cookie
 | auto_renewal | bool | Cookie will expire after defined days from the **last activity** when value is `True`. Cookie will expire after defined days from the **last login** when value is `False`.
+| delay_sec | float | Delay in sec after set or delete cookie
 
 ### EncryptorConfig
 
 Configuration for encryption key location to encrypt user information at the client browser before send back to server.
 | Name | Type | Description
 | ---------- | ---- | -----------
 | folderPath | str | Folder location where the encryption key is stored. (Make sure the key location is private)
@@ -522,14 +524,18 @@
 
 - Fix 'no attribute in signinevent' when cookie option is disabled.
 
 ### Version 0.2.5
 
 - Add Optional delay_sec in cookie config for set and del cookie.
 
+### Version 0.2.6
+
+- Fix `expiry_days` and `delay_sec` is not parse correctly from secrets.toml in CookieConfig.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

### Comparing `streamlit-ldap-authenticator-0.2.5/README.md` & `streamlit-ldap-authenticator-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 remember_me = "login_remember_me"
 
 [auth_cookie]
 name = "login_cookie"
 key = "{any password for encryption}"
 expiry_days = 1
 auto_renewal = true
+delay_sec = 0.1
 ```
 
 Create a new file simple_login.py with the following code:
 
 ```python
 import streamlit as st
 from streamlit_ldap_authenticator import Authenticate
@@ -176,14 +177,15 @@
 Configuration to store user information to the cookie in client's browser. Thus even when user close the browser and reload the page, Reauthorization is possible with cookie.
 | Name | Type | Description
 | ------------ | ----- | -----------
 | name | str | cookie name to store in client's browser
 | key | str | encryption key to encrypt user information
 | expiry_days | float | expiry date for the cookie
 | auto_renewal | bool | Cookie will expire after defined days from the **last activity** when value is `True`. Cookie will expire after defined days from the **last login** when value is `False`.
+| delay_sec | float | Delay in sec after set or delete cookie
 
 ### EncryptorConfig
 
 Configuration for encryption key location to encrypt user information at the client browser before send back to server.
 | Name | Type | Description
 | ---------- | ---- | -----------
 | folderPath | str | Folder location where the encryption key is stored. (Make sure the key location is private)
@@ -496,14 +498,18 @@
 
 - Fix 'no attribute in signinevent' when cookie option is disabled.
 
 ### Version 0.2.5
 
 - Add Optional delay_sec in cookie config for set and del cookie.
 
+### Version 0.2.6
+
+- Fix `expiry_days` and `delay_sec` is not parse correctly from secrets.toml in CookieConfig.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

### Comparing `streamlit-ldap-authenticator-0.2.5/setup.py` & `streamlit-ldap-authenticator-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='UTF-8')
 
 setup(
     name='streamlit-ldap-authenticator',
-    version='0.2.5',
+    version='0.2.6',
     author='Nathan Chen',
     author_email='nathan.chen.198@gmail.com',
     description='Authenticate using ldap',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NathanChen198/streamlit-ldap-authenticator',
     packages=find_packages(),
```

### Comparing `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/authenticate.py` & `streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/authenticate.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/configs.py` & `streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,22 @@
 UserInfoValue = Union[List[str], str, None]
 UserInfos = Dict[str, Any]
 T = TypeVar('T')
 AttrDict = Union[_AttrDict, dict]
 
 class Config:
     @classmethod
-    def _getAttrWithDefault(cls, dict: AttrDict, key: str, _type: Type, defaultValue: T): # type: ignore
+    def _getAttrWithDefault(cls, dict: AttrDict, key: str, _type: Union[Type, List[Type]], defaultValueIfNone: T): # type: ignore
         if key in dict:
             value = dict[key]
-            value = value if type(value) is _type else defaultValue
-        else: value = defaultValue
+            if type(_type) is list:
+                if not any([type(value) is t for t in _type]): raise ValueError(f"'{value}' is not a valid {key}")
+            else:
+                if not type(value) is _type: raise ValueError(f"'{value}' is not a valid {key}")
+        else: value = defaultValueIfNone
         return value
     
     @classmethod
     def _getAttr(cls, dict: AttrDict, key: str, _type: Type):
         if key not in dict: raise AttributeError(f"'{key}' is not found")
 
         value = dict[key]
@@ -221,17 +224,18 @@
         self.auto_renewal = auto_renewal
         self.delay_sec = delay_sec
 
     @classmethod
     def from_dict(cls, dict: AttrDict) -> 'CookieConfig':
         key = cls._getAttr(dict, 'key', str)
         name = cls._getAttrWithDefault(dict, 'name', str, cls.__default_name__)
-        expiry_days = cls._getAttrWithDefault(dict, 'expiry_days', float, cls.__default_expiry_days__)
+        expiry_days = float(cls._getAttrWithDefault(dict, 'expiry_days', [float, int], cls.__default_expiry_days__))
         auto_renewal = cls._getAttrWithDefault(dict, 'auto_renewal', bool, cls.__default_auto_renewal__)
-        return CookieConfig(key, name, expiry_days, auto_renewal)
+        delay_sec = float(cls._getAttrWithDefault(dict, 'delay_sec', [float, int], cls.__default_delay_sec__))
+        return CookieConfig(key, name, expiry_days, auto_renewal, delay_sec)
 
     @classmethod
     def getInstance(cls, value: Union['CookieConfig', AttrDict, None]) -> Optional['CookieConfig']:
         if type(value) is CookieConfig: return value
         if type(value) is dict or type(value) is _AttrDict: return cls.from_dict(value)
         return None
```

### Comparing `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/exceptions.py` & `streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator/ldap_authenticate.py` & `streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator/ldap_authenticate.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.5/streamlit_ldap_authenticator.egg-info/PKG-INFO` & `streamlit-ldap-authenticator-0.2.6/streamlit_ldap_authenticator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-ldap-authenticator
-Version: 0.2.5
+Version: 0.2.6
 Summary: Authenticate using ldap
 Home-page: https://github.com/NathanChen198/streamlit-ldap-authenticator
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,14 +87,15 @@
 remember_me = "login_remember_me"
 
 [auth_cookie]
 name = "login_cookie"
 key = "{any password for encryption}"
 expiry_days = 1
 auto_renewal = true
+delay_sec = 0.1
 ```
 
 Create a new file simple_login.py with the following code:
 
 ```python
 import streamlit as st
 from streamlit_ldap_authenticator import Authenticate
@@ -202,14 +203,15 @@
 Configuration to store user information to the cookie in client's browser. Thus even when user close the browser and reload the page, Reauthorization is possible with cookie.
 | Name | Type | Description
 | ------------ | ----- | -----------
 | name | str | cookie name to store in client's browser
 | key | str | encryption key to encrypt user information
 | expiry_days | float | expiry date for the cookie
 | auto_renewal | bool | Cookie will expire after defined days from the **last activity** when value is `True`. Cookie will expire after defined days from the **last login** when value is `False`.
+| delay_sec | float | Delay in sec after set or delete cookie
 
 ### EncryptorConfig
 
 Configuration for encryption key location to encrypt user information at the client browser before send back to server.
 | Name | Type | Description
 | ---------- | ---- | -----------
 | folderPath | str | Folder location where the encryption key is stored. (Make sure the key location is private)
@@ -522,14 +524,18 @@
 
 - Fix 'no attribute in signinevent' when cookie option is disabled.
 
 ### Version 0.2.5
 
 - Add Optional delay_sec in cookie config for set and del cookie.
 
+### Version 0.2.6
+
+- Fix `expiry_days` and `delay_sec` is not parse correctly from secrets.toml in CookieConfig.
+
 [pypi_badge]: https://img.shields.io/pypi/v/streamlit-ldap-authenticator.svg
 [pypi_link]: https://pypi.org/project/streamlit-ldap-authenticator
 [pypi_download_badge]: https://static.pepy.tech/badge/streamlit-ldap-authenticator
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-ldap-authenticator/blob/main/LICENSE
```

