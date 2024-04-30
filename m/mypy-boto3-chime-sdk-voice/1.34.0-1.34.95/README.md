# Comparing `tmp/mypy-boto3-chime-sdk-voice-1.34.0.tar.gz` & `tmp/mypy_boto3_chime_sdk_voice-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.34.0.tar", last modified: Wed Dec 13 21:22:07 2023, max compression
+gzip compressed data, was "mypy_boto3_chime_sdk_voice-1.34.95.tar", last modified: Tue Apr 30 19:34:51 2024, max compression
```

## Comparing `mypy-boto3-chime-sdk-voice-1.34.0.tar` & `mypy_boto3_chime_sdk_voice-1.34.95.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:07.395147 mypy-boto3-chime-sdk-voice-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:06:35.000000 mypy-boto3-chime-sdk-voice-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2023-12-13 21:22:07.395147 mypy-boto3-chime-sdk-voice-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2023-12-13 21:06:35.000000 mypy-boto3-chime-sdk-voice-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:07.395147 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-13 21:06:35.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-13 21:06:35.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-12-13 21:06:35.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66978 2023-12-13 21:06:36.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    66974 2023-12-13 21:06:36.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-12-13 21:06:36.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2023-12-13 21:06:36.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2023-12-13 21:06:36.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-12-13 21:06:36.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:06:35.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    63246 2023-12-13 21:06:38.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    63245 2023-12-13 21:06:37.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:06:35.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:07.395147 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2023-12-13 21:22:07.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 21:22:07.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:07.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:07.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:07.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 21:22:07.000000 mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:07.395147 mypy-boto3-chime-sdk-voice-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-12-13 21:06:35.000000 mypy-boto3-chime-sdk-voice-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:51.423027 mypy_boto3_chime_sdk_voice-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-04-30 19:34:51.423027 mypy_boto3_chime_sdk_voice-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:51.423027 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67106 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67103 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-04-30 19:32:03.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    65738 2024-04-30 19:32:03.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65738 2024-04-30 19:32:03.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:51.423027 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-04-30 19:34:51.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-30 19:34:51.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:51.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:51.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:51.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 19:34:51.000000 mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:51.423027 mypy_boto3_chime_sdk_voice-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-30 19:32:02.000000 mypy_boto3_chime_sdk_voice-1.34.95/setup.py
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/LICENSE` & `mypy_boto3_chime_sdk_voice-1.34.95/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/PKG-INFO` & `mypy_boto3_chime_sdk_voice-1.34.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.34.0
-Summary: Type annotations for boto3.ChimeSDKVoice 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.95
+Summary: Type annotations for boto3.ChimeSDKVoice 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-chime-sdk-voice"></a>
 
 # mypy-boto3-chime-sdk-voice
 
 [![PyPI - mypy-boto3-chime-sdk-voice](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/README.md` & `mypy_boto3_chime_sdk_voice-1.34.95/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/__init__.py` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,13 @@
 """
 
 from .client import ChimeSDKVoiceClient
 from .paginator import ListSipMediaApplicationsPaginator, ListSipRulesPaginator
 
 Client = ChimeSDKVoiceClient
 
-
 __all__ = (
     "ChimeSDKVoiceClient",
     "Client",
     "ListSipMediaApplicationsPaginator",
     "ListSipRulesPaginator",
 )
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/__init__.pyi` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/__main__.py` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKVoice 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.ChimeSDKVoice 1.34.95\n"
+        "Version:         1.34.95\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.95")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/client.py` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     CreateVoiceConnectorGroupResponseTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainResponseTypeDef,
     CreateVoiceProfileResponseTypeDef,
     CredentialTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmergencyCallingConfigurationTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetGlobalSettingsResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionResponseTypeDef,
@@ -84,35 +84,35 @@
     ListTagsForResourceResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
     LoggingConfigurationTypeDef,
-    OriginationTypeDef,
+    OriginationUnionTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationUnionTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationUnionTypeDef,
     TagTypeDef,
-    TerminationTypeDef,
+    TerminationUnionTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
@@ -125,15 +125,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ChimeSDKVoiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -185,15 +184,15 @@
         """
 
     def associate_phone_numbers_with_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         E164PhoneNumbers: Sequence[str],
-        ForceAssociate: bool = ...
+        ForceAssociate: bool = ...,
     ) -> AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef:
         """
         Associates phone numbers with the specified Amazon Chime SDK Voice Connector
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.associate_phone_numbers_with_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#associate_phone_numbers_with_voice_connector_group)
@@ -209,15 +208,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#batch_delete_phone_number)
         """
 
     def batch_update_phone_number(
         self, *, UpdatePhoneNumberRequestItems: Sequence[UpdatePhoneNumberRequestItemTypeDef]
     ) -> BatchUpdatePhoneNumberResponseTypeDef:
         """
-        Updates one or more phone numbers.
+        Updates phone number product types, calling names, or phone number names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.batch_update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#batch_update_phone_number)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -236,15 +235,15 @@
         """
 
     def create_phone_number_order(
         self,
         *,
         ProductType: PhoneNumberProductTypeType,
         E164PhoneNumbers: Sequence[str],
-        Name: str = ...
+        Name: str = ...,
     ) -> CreatePhoneNumberOrderResponseTypeDef:
         """
         Creates an order for phone numbers to be provisioned.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_phone_number_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_phone_number_order)
         """
@@ -255,15 +254,15 @@
         VoiceConnectorId: str,
         ParticipantPhoneNumbers: Sequence[str],
         Capabilities: Sequence[CapabilityType],
         Name: str = ...,
         ExpiryMinutes: int = ...,
         NumberSelectionBehavior: NumberSelectionBehaviorType = ...,
         GeoMatchLevel: GeoMatchLevelType = ...,
-        GeoMatchParams: GeoMatchParamsTypeDef = ...
+        GeoMatchParams: GeoMatchParamsTypeDef = ...,
     ) -> CreateProxySessionResponseTypeDef:
         """
         Creates a proxy session for the specified Amazon Chime SDK Voice Connector for
         the specified participant phone
         numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_proxy_session)
@@ -272,15 +271,15 @@
 
     def create_sip_media_application(
         self,
         *,
         AwsRegion: str,
         Name: str,
         Endpoints: Sequence[SipMediaApplicationEndpointTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSipMediaApplicationResponseTypeDef:
         """
         Creates a SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_sip_media_application)
         """
@@ -288,15 +287,15 @@
     def create_sip_media_application_call(
         self,
         *,
         FromPhoneNumber: str,
         ToPhoneNumber: str,
         SipMediaApplicationId: str,
         SipHeaders: Mapping[str, str] = ...,
-        ArgumentsMap: Mapping[str, str] = ...
+        ArgumentsMap: Mapping[str, str] = ...,
     ) -> CreateSipMediaApplicationCallResponseTypeDef:
         """
         Creates an outbound call to a phone number from the phone number specified in
         the request, and it invokes the endpoint of the specified
         `sipMediaApplicationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application_call)
@@ -306,15 +305,15 @@
     def create_sip_rule(
         self,
         *,
         Name: str,
         TriggerType: SipRuleTriggerTypeType,
         TriggerValue: str,
         Disabled: bool = ...,
-        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
+        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...,
     ) -> CreateSipRuleResponseTypeDef:
         """
         Creates a SIP rule, which can be used to run a SIP media application as a
         target for a specific trigger
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_rule)
@@ -323,15 +322,15 @@
 
     def create_voice_connector(
         self,
         *,
         Name: str,
         RequireEncryption: bool,
         AwsRegion: VoiceConnectorAwsRegionType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVoiceConnectorResponseTypeDef:
         """
         Creates an Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_connector)
         """
@@ -362,15 +361,15 @@
     def create_voice_profile_domain(
         self,
         *,
         Name: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVoiceProfileDomainResponseTypeDef:
         """
         Creates a voice profile domain, a collection of voice profiles, their voice
         prints, and encrypted enrollment
         audio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile_domain)
@@ -813,15 +812,15 @@
         self,
         *,
         Status: str = ...,
         ProductType: PhoneNumberProductTypeType = ...,
         FilterName: PhoneNumberAssociationNameType = ...,
         FilterValue: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPhoneNumbersResponseTypeDef:
         """
         Lists the phone numbers for the specified Amazon Chime SDK account, Amazon
         Chime SDK user, Amazon Chime SDK Voice Connector, or Amazon Chime SDK Voice
         Connector
         group.
 
@@ -831,15 +830,15 @@
 
     def list_proxy_sessions(
         self,
         *,
         VoiceConnectorId: str,
         Status: ProxySessionStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProxySessionsResponseTypeDef:
         """
         Lists the proxy sessions for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_proxy_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_proxy_sessions)
         """
@@ -933,41 +932,41 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profiles)
         """
 
     def put_sip_media_application_alexa_skill_configuration(
         self,
         *,
         SipMediaApplicationId: str,
-        SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...
+        SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationUnionTypeDef = ...,
     ) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
         Updates the Alexa Skill configuration for the SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_alexa_skill_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_alexa_skill_configuration)
         """
 
     def put_sip_media_application_logging_configuration(
         self,
         *,
         SipMediaApplicationId: str,
-        SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...
+        SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...,
     ) -> PutSipMediaApplicationLoggingConfigurationResponseTypeDef:
         """
         Updates the logging configuration for the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_logging_configuration)
         """
 
     def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef,
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Updates a Voice Connector's emergency calling configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_emergency_calling_configuration)
         """
@@ -979,15 +978,15 @@
         Updates a Voice Connector's logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_logging_configuration)
         """
 
     def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
+        self, *, VoiceConnectorId: str, Origination: OriginationUnionTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Updates a Voice Connector's origination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_origination)
         """
@@ -995,36 +994,36 @@
     def put_voice_connector_proxy(
         self,
         *,
         VoiceConnectorId: str,
         DefaultSessionExpiryMinutes: int,
         PhoneNumberPoolCountries: Sequence[str],
         FallBackPhoneNumber: str = ...,
-        Disabled: bool = ...
+        Disabled: bool = ...,
     ) -> PutVoiceConnectorProxyResponseTypeDef:
         """
         Puts the specified proxy configuration to the specified Amazon Chime SDK Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_proxy)
         """
 
     def put_voice_connector_streaming_configuration(
-        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
+        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Updates a Voice Connector's streaming configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_streaming_configuration)
         """
 
     def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
+        self, *, VoiceConnectorId: str, Termination: TerminationUnionTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Updates a Voice Connector's termination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_termination)
         """
@@ -1053,15 +1052,15 @@
         AreaCode: str = ...,
         City: str = ...,
         Country: str = ...,
         State: str = ...,
         TollFreePrefix: str = ...,
         PhoneNumberType: PhoneNumberTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
         Searches the provisioned phone numbers in an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#search_available_phone_numbers)
         """
@@ -1069,30 +1068,30 @@
     def start_speaker_search_task(
         self,
         *,
         VoiceConnectorId: str,
         TransactionId: str,
         VoiceProfileDomainId: str,
         ClientRequestToken: str = ...,
-        CallLeg: CallLegTypeType = ...
+        CallLeg: CallLegTypeType = ...,
     ) -> StartSpeakerSearchTaskResponseTypeDef:
         """
         Starts a speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_speaker_search_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_speaker_search_task)
         """
 
     def start_voice_tone_analysis_task(
         self,
         *,
         VoiceConnectorId: str,
         TransactionId: str,
         LanguageCode: Literal["en-US"],
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartVoiceToneAnalysisTaskResponseTypeDef:
         """
         Starts a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_voice_tone_analysis_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_voice_tone_analysis_task)
         """
@@ -1150,19 +1149,19 @@
 
     def update_phone_number(
         self,
         *,
         PhoneNumberId: str,
         ProductType: PhoneNumberProductTypeType = ...,
         CallingName: str = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdatePhoneNumberResponseTypeDef:
         """
-        Updates phone number details, such as product type or calling name, for the
-        specified phone number
+        Updates phone number details, such as product type, calling name, or phone
+        number name for the specified phone number
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_phone_number)
         """
 
     def update_phone_number_settings(self, *, CallingName: str) -> EmptyResponseMetadataTypeDef:
@@ -1177,29 +1176,29 @@
 
     def update_proxy_session(
         self,
         *,
         VoiceConnectorId: str,
         ProxySessionId: str,
         Capabilities: Sequence[CapabilityType],
-        ExpiryMinutes: int = ...
+        ExpiryMinutes: int = ...,
     ) -> UpdateProxySessionResponseTypeDef:
         """
         Updates the specified proxy session details, such as voice or SMS capabilities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_proxy_session)
         """
 
     def update_sip_media_application(
         self,
         *,
         SipMediaApplicationId: str,
         Name: str = ...,
-        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...
+        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...,
     ) -> UpdateSipMediaApplicationResponseTypeDef:
         """
         Updates the details of the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_media_application)
         """
@@ -1218,15 +1217,15 @@
 
     def update_sip_rule(
         self,
         *,
         SipRuleId: str,
         Name: str,
         Disabled: bool = ...,
-        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
+        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...,
     ) -> UpdateSipRuleResponseTypeDef:
         """
         Updates the details of the specified SIP rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_rule)
         """
@@ -1242,28 +1241,28 @@
         """
 
     def update_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         Name: str,
-        VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef]
+        VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef],
     ) -> UpdateVoiceConnectorGroupResponseTypeDef:
         """
         Updates the settings for the specified Amazon Chime SDK Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_connector_group)
         """
 
     def update_voice_profile(
         self, *, VoiceProfileId: str, SpeakerSearchTaskId: str
     ) -> UpdateVoiceProfileResponseTypeDef:
         """
-        Updates the specified voice profile’s voice print and refreshes its expiration
+        Updates the specified voice profile's voice print and refreshes its expiration
         timestamp.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile)
         """
 
     def update_voice_profile_domain(
@@ -1281,15 +1280,15 @@
         *,
         AwsAccountId: str,
         StreetNumber: str,
         StreetInfo: str,
         City: str,
         State: str,
         Country: str,
-        PostalCode: str
+        PostalCode: str,
     ) -> ValidateE911AddressResponseTypeDef:
         """
         Validates an address to be used for 911 calls made with Amazon Chime SDK Voice
         Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.validate_e911_address)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#validate_e911_address)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/client.pyi` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     CreateVoiceConnectorGroupResponseTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     CreateVoiceProfileDomainResponseTypeDef,
     CreateVoiceProfileResponseTypeDef,
     CredentialTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmergencyCallingConfigurationTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetGlobalSettingsResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionResponseTypeDef,
@@ -84,35 +84,35 @@
     ListTagsForResourceResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
     LoggingConfigurationTypeDef,
-    OriginationTypeDef,
+    OriginationUnionTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationUnionTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
     StartSpeakerSearchTaskResponseTypeDef,
     StartVoiceToneAnalysisTaskResponseTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationUnionTypeDef,
     TagTypeDef,
-    TerminationTypeDef,
+    TerminationUnionTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
@@ -181,15 +181,15 @@
         """
 
     def associate_phone_numbers_with_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         E164PhoneNumbers: Sequence[str],
-        ForceAssociate: bool = ...
+        ForceAssociate: bool = ...,
     ) -> AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef:
         """
         Associates phone numbers with the specified Amazon Chime SDK Voice Connector
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.associate_phone_numbers_with_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#associate_phone_numbers_with_voice_connector_group)
@@ -205,15 +205,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#batch_delete_phone_number)
         """
 
     def batch_update_phone_number(
         self, *, UpdatePhoneNumberRequestItems: Sequence[UpdatePhoneNumberRequestItemTypeDef]
     ) -> BatchUpdatePhoneNumberResponseTypeDef:
         """
-        Updates one or more phone numbers.
+        Updates phone number product types, calling names, or phone number names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.batch_update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#batch_update_phone_number)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -232,15 +232,15 @@
         """
 
     def create_phone_number_order(
         self,
         *,
         ProductType: PhoneNumberProductTypeType,
         E164PhoneNumbers: Sequence[str],
-        Name: str = ...
+        Name: str = ...,
     ) -> CreatePhoneNumberOrderResponseTypeDef:
         """
         Creates an order for phone numbers to be provisioned.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_phone_number_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_phone_number_order)
         """
@@ -251,15 +251,15 @@
         VoiceConnectorId: str,
         ParticipantPhoneNumbers: Sequence[str],
         Capabilities: Sequence[CapabilityType],
         Name: str = ...,
         ExpiryMinutes: int = ...,
         NumberSelectionBehavior: NumberSelectionBehaviorType = ...,
         GeoMatchLevel: GeoMatchLevelType = ...,
-        GeoMatchParams: GeoMatchParamsTypeDef = ...
+        GeoMatchParams: GeoMatchParamsTypeDef = ...,
     ) -> CreateProxySessionResponseTypeDef:
         """
         Creates a proxy session for the specified Amazon Chime SDK Voice Connector for
         the specified participant phone
         numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_proxy_session)
@@ -268,15 +268,15 @@
 
     def create_sip_media_application(
         self,
         *,
         AwsRegion: str,
         Name: str,
         Endpoints: Sequence[SipMediaApplicationEndpointTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSipMediaApplicationResponseTypeDef:
         """
         Creates a SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_sip_media_application)
         """
@@ -284,15 +284,15 @@
     def create_sip_media_application_call(
         self,
         *,
         FromPhoneNumber: str,
         ToPhoneNumber: str,
         SipMediaApplicationId: str,
         SipHeaders: Mapping[str, str] = ...,
-        ArgumentsMap: Mapping[str, str] = ...
+        ArgumentsMap: Mapping[str, str] = ...,
     ) -> CreateSipMediaApplicationCallResponseTypeDef:
         """
         Creates an outbound call to a phone number from the phone number specified in
         the request, and it invokes the endpoint of the specified
         `sipMediaApplicationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application_call)
@@ -302,15 +302,15 @@
     def create_sip_rule(
         self,
         *,
         Name: str,
         TriggerType: SipRuleTriggerTypeType,
         TriggerValue: str,
         Disabled: bool = ...,
-        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
+        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...,
     ) -> CreateSipRuleResponseTypeDef:
         """
         Creates a SIP rule, which can be used to run a SIP media application as a
         target for a specific trigger
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_rule)
@@ -319,15 +319,15 @@
 
     def create_voice_connector(
         self,
         *,
         Name: str,
         RequireEncryption: bool,
         AwsRegion: VoiceConnectorAwsRegionType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVoiceConnectorResponseTypeDef:
         """
         Creates an Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_connector)
         """
@@ -358,15 +358,15 @@
     def create_voice_profile_domain(
         self,
         *,
         Name: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVoiceProfileDomainResponseTypeDef:
         """
         Creates a voice profile domain, a collection of voice profiles, their voice
         prints, and encrypted enrollment
         audio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile_domain)
@@ -809,15 +809,15 @@
         self,
         *,
         Status: str = ...,
         ProductType: PhoneNumberProductTypeType = ...,
         FilterName: PhoneNumberAssociationNameType = ...,
         FilterValue: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListPhoneNumbersResponseTypeDef:
         """
         Lists the phone numbers for the specified Amazon Chime SDK account, Amazon
         Chime SDK user, Amazon Chime SDK Voice Connector, or Amazon Chime SDK Voice
         Connector
         group.
 
@@ -827,15 +827,15 @@
 
     def list_proxy_sessions(
         self,
         *,
         VoiceConnectorId: str,
         Status: ProxySessionStatusType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProxySessionsResponseTypeDef:
         """
         Lists the proxy sessions for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_proxy_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_proxy_sessions)
         """
@@ -929,41 +929,41 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profiles)
         """
 
     def put_sip_media_application_alexa_skill_configuration(
         self,
         *,
         SipMediaApplicationId: str,
-        SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...
+        SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationUnionTypeDef = ...,
     ) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
         Updates the Alexa Skill configuration for the SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_alexa_skill_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_alexa_skill_configuration)
         """
 
     def put_sip_media_application_logging_configuration(
         self,
         *,
         SipMediaApplicationId: str,
-        SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...
+        SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...,
     ) -> PutSipMediaApplicationLoggingConfigurationResponseTypeDef:
         """
         Updates the logging configuration for the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_logging_configuration)
         """
 
     def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef,
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Updates a Voice Connector's emergency calling configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_emergency_calling_configuration)
         """
@@ -975,15 +975,15 @@
         Updates a Voice Connector's logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_logging_configuration)
         """
 
     def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
+        self, *, VoiceConnectorId: str, Origination: OriginationUnionTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Updates a Voice Connector's origination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_origination)
         """
@@ -991,36 +991,36 @@
     def put_voice_connector_proxy(
         self,
         *,
         VoiceConnectorId: str,
         DefaultSessionExpiryMinutes: int,
         PhoneNumberPoolCountries: Sequence[str],
         FallBackPhoneNumber: str = ...,
-        Disabled: bool = ...
+        Disabled: bool = ...,
     ) -> PutVoiceConnectorProxyResponseTypeDef:
         """
         Puts the specified proxy configuration to the specified Amazon Chime SDK Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_proxy)
         """
 
     def put_voice_connector_streaming_configuration(
-        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
+        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Updates a Voice Connector's streaming configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_streaming_configuration)
         """
 
     def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
+        self, *, VoiceConnectorId: str, Termination: TerminationUnionTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Updates a Voice Connector's termination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_termination)
         """
@@ -1049,15 +1049,15 @@
         AreaCode: str = ...,
         City: str = ...,
         Country: str = ...,
         State: str = ...,
         TollFreePrefix: str = ...,
         PhoneNumberType: PhoneNumberTypeType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
         Searches the provisioned phone numbers in an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#search_available_phone_numbers)
         """
@@ -1065,30 +1065,30 @@
     def start_speaker_search_task(
         self,
         *,
         VoiceConnectorId: str,
         TransactionId: str,
         VoiceProfileDomainId: str,
         ClientRequestToken: str = ...,
-        CallLeg: CallLegTypeType = ...
+        CallLeg: CallLegTypeType = ...,
     ) -> StartSpeakerSearchTaskResponseTypeDef:
         """
         Starts a speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_speaker_search_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_speaker_search_task)
         """
 
     def start_voice_tone_analysis_task(
         self,
         *,
         VoiceConnectorId: str,
         TransactionId: str,
         LanguageCode: Literal["en-US"],
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartVoiceToneAnalysisTaskResponseTypeDef:
         """
         Starts a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_voice_tone_analysis_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_voice_tone_analysis_task)
         """
@@ -1146,19 +1146,19 @@
 
     def update_phone_number(
         self,
         *,
         PhoneNumberId: str,
         ProductType: PhoneNumberProductTypeType = ...,
         CallingName: str = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdatePhoneNumberResponseTypeDef:
         """
-        Updates phone number details, such as product type or calling name, for the
-        specified phone number
+        Updates phone number details, such as product type, calling name, or phone
+        number name for the specified phone number
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_phone_number)
         """
 
     def update_phone_number_settings(self, *, CallingName: str) -> EmptyResponseMetadataTypeDef:
@@ -1173,29 +1173,29 @@
 
     def update_proxy_session(
         self,
         *,
         VoiceConnectorId: str,
         ProxySessionId: str,
         Capabilities: Sequence[CapabilityType],
-        ExpiryMinutes: int = ...
+        ExpiryMinutes: int = ...,
     ) -> UpdateProxySessionResponseTypeDef:
         """
         Updates the specified proxy session details, such as voice or SMS capabilities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_proxy_session)
         """
 
     def update_sip_media_application(
         self,
         *,
         SipMediaApplicationId: str,
         Name: str = ...,
-        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...
+        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...,
     ) -> UpdateSipMediaApplicationResponseTypeDef:
         """
         Updates the details of the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_media_application)
         """
@@ -1214,15 +1214,15 @@
 
     def update_sip_rule(
         self,
         *,
         SipRuleId: str,
         Name: str,
         Disabled: bool = ...,
-        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
+        TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...,
     ) -> UpdateSipRuleResponseTypeDef:
         """
         Updates the details of the specified SIP rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_rule)
         """
@@ -1238,28 +1238,28 @@
         """
 
     def update_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         Name: str,
-        VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef]
+        VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef],
     ) -> UpdateVoiceConnectorGroupResponseTypeDef:
         """
         Updates the settings for the specified Amazon Chime SDK Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_connector_group)
         """
 
     def update_voice_profile(
         self, *, VoiceProfileId: str, SpeakerSearchTaskId: str
     ) -> UpdateVoiceProfileResponseTypeDef:
         """
-        Updates the specified voice profile’s voice print and refreshes its expiration
+        Updates the specified voice profile's voice print and refreshes its expiration
         timestamp.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile)
         """
 
     def update_voice_profile_domain(
@@ -1277,15 +1277,15 @@
         *,
         AwsAccountId: str,
         StreetNumber: str,
         StreetInfo: str,
         City: str,
         State: str,
         Country: str,
-        PostalCode: str
+        PostalCode: str,
     ) -> ValidateE911AddressResponseTypeDef:
         """
         Validates an address to be used for 911 calls made with Amazon Chime SDK Voice
         Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.validate_e911_address)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#validate_e911_address)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/literals.py` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlexaSkillStatusType",
     "CallLegTypeType",
     "CallingNameStatusType",
     "CapabilityType",
     "ErrorCodeType",
     "GeoMatchLevelType",
@@ -46,15 +45,14 @@
     "ChimeSDKVoiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AlexaSkillStatusType = Literal["ACTIVE", "INACTIVE"]
 CallLegTypeType = Literal["Callee", "Caller"]
 CallingNameStatusType = Literal["Unassigned", "UpdateFailed", "UpdateInProgress", "UpdateSucceeded"]
 CapabilityType = Literal["SMS", "Voice"]
 ErrorCodeType = Literal[
     "AccessDenied",
     "BadRequest",
@@ -148,14 +146,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -166,14 +165,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -191,14 +191,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -211,24 +212,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -289,15 +292,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -369,17 +371,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -424,14 +428,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -469,19 +474,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/literals.pyi` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -164,14 +165,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -189,14 +191,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -209,24 +212,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -287,15 +292,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -367,17 +371,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -422,14 +428,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -467,19 +474,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/paginator.py` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListSipMediaApplicationsResponseTypeDef,
     ListSipRulesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListSipMediaApplicationsPaginator", "ListSipRulesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/paginator.pyi` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/type_defs.py` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AddressTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AlexaSkillStatusType,
     CallingNameStatusType,
     CallLegTypeType,
     CapabilityType,
     ErrorCodeType,
@@ -47,15 +47,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
@@ -93,15 +92,15 @@
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetSpeakerSearchTaskRequestRequestTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorGroupRequestRequestTypeDef",
@@ -111,15 +110,15 @@
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationTypeDef",
+    "TerminationOutputTypeDef",
     "GetVoiceProfileDomainRequestRequestTypeDef",
     "GetVoiceProfileRequestRequestTypeDef",
     "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -137,15 +136,17 @@
     "VoiceProfileSummaryTypeDef",
     "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "TerminationTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SpeakerSearchResultTypeDef",
     "StartSpeakerSearchTaskRequestRequestTypeDef",
     "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
@@ -194,42 +195,47 @@
     "UpdateVoiceConnectorResponseTypeDef",
     "CreateVoiceProfileDomainRequestRequestTypeDef",
     "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileResponseTypeDef",
     "GetVoiceProfileResponseTypeDef",
     "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
-    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "ListVoiceProfileDomainsResponseTypeDef",
     "ListVoiceProfilesResponseTypeDef",
     "PhoneNumberOrderTypeDef",
+    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationUnionTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "TerminationUnionTypeDef",
     "SpeakerSearchDetailsTypeDef",
+    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     "StartVoiceToneAnalysisTaskResponseTypeDef",
     "CreateSipMediaApplicationResponseTypeDef",
     "GetSipMediaApplicationResponseTypeDef",
     "ListSipMediaApplicationsResponseTypeDef",
     "UpdateSipMediaApplicationResponseTypeDef",
@@ -241,34 +247,37 @@
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
     "CreateVoiceProfileDomainResponseTypeDef",
     "GetVoiceProfileDomainResponseTypeDef",
     "UpdateVoiceProfileDomainResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "EmergencyCallingConfigurationUnionTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "PutVoiceConnectorOriginationResponseTypeDef",
+    "OriginationUnionTypeDef",
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "SpeakerSearchTaskTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    "StreamingConfigurationUnionTypeDef",
     "GetSpeakerSearchTaskResponseTypeDef",
     "StartSpeakerSearchTaskResponseTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
@@ -300,18 +309,18 @@
         "ErrorMessage": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
@@ -590,16 +599,16 @@
 )
 GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
-SipMediaApplicationAlexaSkillConfigurationTypeDef = TypedDict(
-    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+SipMediaApplicationAlexaSkillConfigurationOutputTypeDef = TypedDict(
+    "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     {
         "AlexaSkillStatus": AlexaSkillStatusType,
         "AlexaSkillIds": List[str],
     },
 )
 GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
@@ -705,16 +714,16 @@
 )
 GetVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
-TerminationTypeDef = TypedDict(
-    "TerminationTypeDef",
+TerminationOutputTypeDef = TypedDict(
+    "TerminationOutputTypeDef",
     {
         "CpsLimit": NotRequired[int],
         "DefaultPhoneNumber": NotRequired[str],
         "CallingRegions": NotRequired[List[str]],
         "CidrAllowedList": NotRequired[List[str]],
         "Disabled": NotRequired[bool],
     },
@@ -911,24 +920,41 @@
         "OutboundCall": NotRequired[bool],
         "InboundSMS": NotRequired[bool],
         "OutboundSMS": NotRequired[bool],
         "InboundMMS": NotRequired[bool],
         "OutboundMMS": NotRequired[bool],
     },
 )
+SipMediaApplicationAlexaSkillConfigurationTypeDef = TypedDict(
+    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    {
+        "AlexaSkillStatus": AlexaSkillStatusType,
+        "AlexaSkillIds": Sequence[str],
+    },
+)
 PutVoiceConnectorProxyRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "DefaultSessionExpiryMinutes": int,
         "PhoneNumberPoolCountries": Sequence[str],
         "FallBackPhoneNumber": NotRequired[str],
         "Disabled": NotRequired[bool],
     },
 )
+TerminationTypeDef = TypedDict(
+    "TerminationTypeDef",
+    {
+        "CpsLimit": NotRequired[int],
+        "DefaultPhoneNumber": NotRequired[str],
+        "CallingRegions": NotRequired[Sequence[str]],
+        "CidrAllowedList": NotRequired[Sequence[str]],
+        "Disabled": NotRequired[bool],
+    },
+)
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 SearchAvailablePhoneNumbersRequestRequestTypeDef = TypedDict(
@@ -1134,16 +1160,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
     "SearchAvailablePhoneNumbersResponseTypeDef",
     {
         "E164PhoneNumbers": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
@@ -1321,16 +1347,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListVoiceConnectorsResponseTypeDef = TypedDict(
     "ListVoiceConnectorsResponseTypeDef",
     {
         "VoiceConnectors": List[VoiceConnectorTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateVoiceConnectorResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1382,18 +1408,24 @@
 PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Credentials": NotRequired[Sequence[CredentialTypeDef]],
     },
 )
+EmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "EmergencyCallingConfigurationOutputTypeDef",
+    {
+        "DNIS": NotRequired[List[DNISEmergencyCallingConfigurationTypeDef]],
+    },
+)
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
-        "DNIS": NotRequired[List[DNISEmergencyCallingConfigurationTypeDef]],
+        "DNIS": NotRequired[Sequence[DNISEmergencyCallingConfigurationTypeDef]],
     },
 )
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1404,35 +1436,22 @@
     {
         "VoiceConnector": NotRequired[VoiceConnectorSettingsTypeDef],
     },
 )
 GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
-        ),
+        "SipMediaApplicationAlexaSkillConfiguration": SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
-    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "SipMediaApplicationAlexaSkillConfiguration": NotRequired[
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
-        ],
-    },
-)
 PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
-        ),
+        "SipMediaApplicationAlexaSkillConfiguration": SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
@@ -1496,29 +1515,22 @@
         "TerminationHealth": TerminationHealthTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Termination": TerminationTypeDef,
-    },
-)
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
     "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1538,42 +1550,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListVoiceProfileDomainsResponseTypeDef = TypedDict(
     "ListVoiceProfileDomainsResponseTypeDef",
     {
         "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListVoiceProfilesResponseTypeDef = TypedDict(
     "ListVoiceProfilesResponseTypeDef",
     {
         "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": NotRequired[str],
         "ProductType": NotRequired[PhoneNumberProductTypeType],
         "Status": NotRequired[PhoneNumberOrderStatusType],
         "OrderType": NotRequired[PhoneNumberOrderTypeType],
         "OrderedPhoneNumbers": NotRequired[List[OrderedPhoneNumberTypeDef]],
         "CreatedTimestamp": NotRequired[datetime],
         "UpdatedTimestamp": NotRequired[datetime],
     },
 )
+OriginationOutputTypeDef = TypedDict(
+    "OriginationOutputTypeDef",
+    {
+        "Routes": NotRequired[List[OriginationRouteTypeDef]],
+        "Disabled": NotRequired[bool],
+    },
+)
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
     {
-        "Routes": NotRequired[List[OriginationRouteTypeDef]],
+        "Routes": NotRequired[Sequence[OriginationRouteTypeDef]],
         "Disabled": NotRequired[bool],
     },
 )
 ProxySessionTypeDef = TypedDict(
     "ProxySessionTypeDef",
     {
         "VoiceConnectorId": NotRequired[str],
@@ -1607,27 +1626,57 @@
         "CreatedTimestamp": NotRequired[datetime],
         "UpdatedTimestamp": NotRequired[datetime],
         "DeletionTimestamp": NotRequired[datetime],
         "OrderId": NotRequired[str],
         "Name": NotRequired[str],
     },
 )
+PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
+    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "SipMediaApplicationAlexaSkillConfiguration": NotRequired[
+            SipMediaApplicationAlexaSkillConfigurationTypeDef
+        ],
+    },
+)
+SipMediaApplicationAlexaSkillConfigurationUnionTypeDef = Union[
+    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
+]
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
+    },
+)
+TerminationUnionTypeDef = Union[TerminationTypeDef, TerminationOutputTypeDef]
 SpeakerSearchDetailsTypeDef = TypedDict(
     "SpeakerSearchDetailsTypeDef",
     {
         "Results": NotRequired[List[SpeakerSearchResultTypeDef]],
         "VoiceprintGenerationStatus": NotRequired[str],
     },
 )
+StreamingConfigurationOutputTypeDef = TypedDict(
+    "StreamingConfigurationOutputTypeDef",
+    {
+        "DataRetentionInHours": int,
+        "Disabled": bool,
+        "StreamingNotificationTargets": NotRequired[List[StreamingNotificationTargetTypeDef]],
+        "MediaInsightsConfiguration": NotRequired[MediaInsightsConfigurationTypeDef],
+    },
+)
 StreamingConfigurationTypeDef = TypedDict(
     "StreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
         "Disabled": bool,
-        "StreamingNotificationTargets": NotRequired[List[StreamingNotificationTargetTypeDef]],
+        "StreamingNotificationTargets": NotRequired[Sequence[StreamingNotificationTargetTypeDef]],
         "MediaInsightsConfiguration": NotRequired[MediaInsightsConfigurationTypeDef],
     },
 )
 GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     {
         "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
@@ -1655,16 +1704,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSipMediaApplicationsResponseTypeDef = TypedDict(
     "ListSipMediaApplicationsResponseTypeDef",
     {
         "SipMediaApplications": List[SipMediaApplicationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateSipMediaApplicationResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1684,16 +1733,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSipRulesResponseTypeDef = TypedDict(
     "ListSipRulesResponseTypeDef",
     {
         "SipRules": List[SipRuleTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateSipRuleResponseTypeDef = TypedDict(
     "UpdateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1713,16 +1762,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
     "ListVoiceConnectorGroupsResponseTypeDef",
     {
         "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1748,30 +1797,33 @@
         "VoiceProfileDomain": VoiceProfileDomainTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+EmergencyCallingConfigurationUnionTypeDef = Union[
+    EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
+]
+PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1784,39 +1836,40 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListPhoneNumberOrdersResponseTypeDef = TypedDict(
     "ListPhoneNumberOrdersResponseTypeDef",
     {
         "PhoneNumberOrders": List[PhoneNumberOrderTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationResponseTypeDef",
+    {
+        "Origination": OriginationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+OriginationUnionTypeDef = Union[OriginationTypeDef, OriginationOutputTypeDef]
 PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
     },
 )
-PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationResponseTypeDef",
-    {
-        "Origination": OriginationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1827,16 +1880,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListProxySessionsResponseTypeDef = TypedDict(
     "ListProxySessionsResponseTypeDef",
     {
         "ProxySessions": List[ProxySessionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateProxySessionResponseTypeDef = TypedDict(
     "UpdateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1849,16 +1902,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RestorePhoneNumberResponseTypeDef = TypedDict(
     "RestorePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1883,32 +1936,35 @@
         "StartedTimestamp": NotRequired[datetime],
         "StatusMessage": NotRequired[str],
     },
 )
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StreamingConfigurationUnionTypeDef = Union[
+    StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
+]
 GetSpeakerSearchTaskResponseTypeDef = TypedDict(
     "GetSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice/type_defs.pyi` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AddressTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AlexaSkillStatusType,
     CallingNameStatusType,
     CallLegTypeType,
     CapabilityType,
     ErrorCodeType,
@@ -92,15 +92,15 @@
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
     "GetSpeakerSearchTaskRequestRequestTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorGroupRequestRequestTypeDef",
@@ -110,15 +110,15 @@
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationTypeDef",
+    "TerminationOutputTypeDef",
     "GetVoiceProfileDomainRequestRequestTypeDef",
     "GetVoiceProfileRequestRequestTypeDef",
     "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -136,15 +136,17 @@
     "VoiceProfileSummaryTypeDef",
     "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "TerminationTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
     "SpeakerSearchResultTypeDef",
     "StartSpeakerSearchTaskRequestRequestTypeDef",
     "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
@@ -193,42 +195,47 @@
     "UpdateVoiceConnectorResponseTypeDef",
     "CreateVoiceProfileDomainRequestRequestTypeDef",
     "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileResponseTypeDef",
     "GetVoiceProfileResponseTypeDef",
     "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
-    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     "PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "ListVoiceProfileDomainsResponseTypeDef",
     "ListVoiceProfilesResponseTypeDef",
     "PhoneNumberOrderTypeDef",
+    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
+    "SipMediaApplicationAlexaSkillConfigurationUnionTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "TerminationUnionTypeDef",
     "SpeakerSearchDetailsTypeDef",
+    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     "StartVoiceToneAnalysisTaskResponseTypeDef",
     "CreateSipMediaApplicationResponseTypeDef",
     "GetSipMediaApplicationResponseTypeDef",
     "ListSipMediaApplicationsResponseTypeDef",
     "UpdateSipMediaApplicationResponseTypeDef",
@@ -240,34 +247,37 @@
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
     "CreateVoiceProfileDomainResponseTypeDef",
     "GetVoiceProfileDomainResponseTypeDef",
     "UpdateVoiceProfileDomainResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "EmergencyCallingConfigurationUnionTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "PutVoiceConnectorOriginationResponseTypeDef",
+    "OriginationUnionTypeDef",
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "SpeakerSearchTaskTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    "StreamingConfigurationUnionTypeDef",
     "GetSpeakerSearchTaskResponseTypeDef",
     "StartSpeakerSearchTaskResponseTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
@@ -299,18 +309,18 @@
         "ErrorMessage": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
@@ -589,16 +599,16 @@
 )
 GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
     },
 )
-SipMediaApplicationAlexaSkillConfigurationTypeDef = TypedDict(
-    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+SipMediaApplicationAlexaSkillConfigurationOutputTypeDef = TypedDict(
+    "SipMediaApplicationAlexaSkillConfigurationOutputTypeDef",
     {
         "AlexaSkillStatus": AlexaSkillStatusType,
         "AlexaSkillIds": List[str],
     },
 )
 GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
@@ -704,16 +714,16 @@
 )
 GetVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
-TerminationTypeDef = TypedDict(
-    "TerminationTypeDef",
+TerminationOutputTypeDef = TypedDict(
+    "TerminationOutputTypeDef",
     {
         "CpsLimit": NotRequired[int],
         "DefaultPhoneNumber": NotRequired[str],
         "CallingRegions": NotRequired[List[str]],
         "CidrAllowedList": NotRequired[List[str]],
         "Disabled": NotRequired[bool],
     },
@@ -910,24 +920,41 @@
         "OutboundCall": NotRequired[bool],
         "InboundSMS": NotRequired[bool],
         "OutboundSMS": NotRequired[bool],
         "InboundMMS": NotRequired[bool],
         "OutboundMMS": NotRequired[bool],
     },
 )
+SipMediaApplicationAlexaSkillConfigurationTypeDef = TypedDict(
+    "SipMediaApplicationAlexaSkillConfigurationTypeDef",
+    {
+        "AlexaSkillStatus": AlexaSkillStatusType,
+        "AlexaSkillIds": Sequence[str],
+    },
+)
 PutVoiceConnectorProxyRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "DefaultSessionExpiryMinutes": int,
         "PhoneNumberPoolCountries": Sequence[str],
         "FallBackPhoneNumber": NotRequired[str],
         "Disabled": NotRequired[bool],
     },
 )
+TerminationTypeDef = TypedDict(
+    "TerminationTypeDef",
+    {
+        "CpsLimit": NotRequired[int],
+        "DefaultPhoneNumber": NotRequired[str],
+        "CallingRegions": NotRequired[Sequence[str]],
+        "CidrAllowedList": NotRequired[Sequence[str]],
+        "Disabled": NotRequired[bool],
+    },
+)
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 SearchAvailablePhoneNumbersRequestRequestTypeDef = TypedDict(
@@ -1133,16 +1160,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
     "SearchAvailablePhoneNumbersResponseTypeDef",
     {
         "E164PhoneNumbers": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
@@ -1320,16 +1347,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListVoiceConnectorsResponseTypeDef = TypedDict(
     "ListVoiceConnectorsResponseTypeDef",
     {
         "VoiceConnectors": List[VoiceConnectorTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateVoiceConnectorResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1381,18 +1408,24 @@
 PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "Credentials": NotRequired[Sequence[CredentialTypeDef]],
     },
 )
+EmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "EmergencyCallingConfigurationOutputTypeDef",
+    {
+        "DNIS": NotRequired[List[DNISEmergencyCallingConfigurationTypeDef]],
+    },
+)
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
-        "DNIS": NotRequired[List[DNISEmergencyCallingConfigurationTypeDef]],
+        "DNIS": NotRequired[Sequence[DNISEmergencyCallingConfigurationTypeDef]],
     },
 )
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1403,35 +1436,22 @@
     {
         "VoiceConnector": NotRequired[VoiceConnectorSettingsTypeDef],
     },
 )
 GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
-        ),
+        "SipMediaApplicationAlexaSkillConfiguration": SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
-    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "SipMediaApplicationAlexaSkillConfiguration": NotRequired[
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
-        ],
-    },
-)
 PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
-        "SipMediaApplicationAlexaSkillConfiguration": (
-            SipMediaApplicationAlexaSkillConfigurationTypeDef
-        ),
+        "SipMediaApplicationAlexaSkillConfiguration": SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
@@ -1495,29 +1515,22 @@
         "TerminationHealth": TerminationHealthTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Termination": TerminationTypeDef,
-    },
-)
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
     "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1537,42 +1550,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListVoiceProfileDomainsResponseTypeDef = TypedDict(
     "ListVoiceProfileDomainsResponseTypeDef",
     {
         "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListVoiceProfilesResponseTypeDef = TypedDict(
     "ListVoiceProfilesResponseTypeDef",
     {
         "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": NotRequired[str],
         "ProductType": NotRequired[PhoneNumberProductTypeType],
         "Status": NotRequired[PhoneNumberOrderStatusType],
         "OrderType": NotRequired[PhoneNumberOrderTypeType],
         "OrderedPhoneNumbers": NotRequired[List[OrderedPhoneNumberTypeDef]],
         "CreatedTimestamp": NotRequired[datetime],
         "UpdatedTimestamp": NotRequired[datetime],
     },
 )
+OriginationOutputTypeDef = TypedDict(
+    "OriginationOutputTypeDef",
+    {
+        "Routes": NotRequired[List[OriginationRouteTypeDef]],
+        "Disabled": NotRequired[bool],
+    },
+)
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
     {
-        "Routes": NotRequired[List[OriginationRouteTypeDef]],
+        "Routes": NotRequired[Sequence[OriginationRouteTypeDef]],
         "Disabled": NotRequired[bool],
     },
 )
 ProxySessionTypeDef = TypedDict(
     "ProxySessionTypeDef",
     {
         "VoiceConnectorId": NotRequired[str],
@@ -1606,27 +1626,57 @@
         "CreatedTimestamp": NotRequired[datetime],
         "UpdatedTimestamp": NotRequired[datetime],
         "DeletionTimestamp": NotRequired[datetime],
         "OrderId": NotRequired[str],
         "Name": NotRequired[str],
     },
 )
+PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
+    "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "SipMediaApplicationAlexaSkillConfiguration": NotRequired[
+            SipMediaApplicationAlexaSkillConfigurationTypeDef
+        ],
+    },
+)
+SipMediaApplicationAlexaSkillConfigurationUnionTypeDef = Union[
+    SipMediaApplicationAlexaSkillConfigurationTypeDef,
+    SipMediaApplicationAlexaSkillConfigurationOutputTypeDef,
+]
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
+    },
+)
+TerminationUnionTypeDef = Union[TerminationTypeDef, TerminationOutputTypeDef]
 SpeakerSearchDetailsTypeDef = TypedDict(
     "SpeakerSearchDetailsTypeDef",
     {
         "Results": NotRequired[List[SpeakerSearchResultTypeDef]],
         "VoiceprintGenerationStatus": NotRequired[str],
     },
 )
+StreamingConfigurationOutputTypeDef = TypedDict(
+    "StreamingConfigurationOutputTypeDef",
+    {
+        "DataRetentionInHours": int,
+        "Disabled": bool,
+        "StreamingNotificationTargets": NotRequired[List[StreamingNotificationTargetTypeDef]],
+        "MediaInsightsConfiguration": NotRequired[MediaInsightsConfigurationTypeDef],
+    },
+)
 StreamingConfigurationTypeDef = TypedDict(
     "StreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
         "Disabled": bool,
-        "StreamingNotificationTargets": NotRequired[List[StreamingNotificationTargetTypeDef]],
+        "StreamingNotificationTargets": NotRequired[Sequence[StreamingNotificationTargetTypeDef]],
         "MediaInsightsConfiguration": NotRequired[MediaInsightsConfigurationTypeDef],
     },
 )
 GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     {
         "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
@@ -1654,16 +1704,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSipMediaApplicationsResponseTypeDef = TypedDict(
     "ListSipMediaApplicationsResponseTypeDef",
     {
         "SipMediaApplications": List[SipMediaApplicationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateSipMediaApplicationResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1683,16 +1733,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSipRulesResponseTypeDef = TypedDict(
     "ListSipRulesResponseTypeDef",
     {
         "SipRules": List[SipRuleTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateSipRuleResponseTypeDef = TypedDict(
     "UpdateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1712,16 +1762,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
     "ListVoiceConnectorGroupsResponseTypeDef",
     {
         "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1747,30 +1797,33 @@
         "VoiceProfileDomain": VoiceProfileDomainTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+EmergencyCallingConfigurationUnionTypeDef = Union[
+    EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
+]
+PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1783,37 +1836,38 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListPhoneNumberOrdersResponseTypeDef = TypedDict(
     "ListPhoneNumberOrdersResponseTypeDef",
     {
         "PhoneNumberOrders": List[PhoneNumberOrderTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
+PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationResponseTypeDef",
+OriginationUnionTypeDef = Union[OriginationTypeDef, OriginationOutputTypeDef]
+PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1826,16 +1880,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListProxySessionsResponseTypeDef = TypedDict(
     "ListProxySessionsResponseTypeDef",
     {
         "ProxySessions": List[ProxySessionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateProxySessionResponseTypeDef = TypedDict(
     "UpdateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1848,16 +1902,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RestorePhoneNumberResponseTypeDef = TypedDict(
     "RestorePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1882,32 +1936,35 @@
         "StartedTimestamp": NotRequired[datetime],
         "StatusMessage": NotRequired[str],
     },
 )
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StreamingConfigurationUnionTypeDef = Union[
+    StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
+]
 GetSpeakerSearchTaskResponseTypeDef = TypedDict(
     "GetSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.34.0
-Summary: Type annotations for boto3.ChimeSDKVoice 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.95
+Summary: Type annotations for boto3.ChimeSDKVoice 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-chime-sdk-voice"></a>
 
 # mypy-boto3-chime-sdk-voice
 
 [![PyPI - mypy-boto3-chime-sdk-voice](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-voice)](https://pepy.tech/project/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt` & `mypy_boto3_chime_sdk_voice-1.34.95/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.34.0/setup.py` & `mypy_boto3_chime_sdk_voice-1.34.95/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-voice",
-    version="1.34.0",
+    version="1.34.95",
     packages=["mypy_boto3_chime_sdk_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ChimeSDKVoice 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.ChimeSDKVoice 1.34.95 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 chime-sdk-voice type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_chime_sdk_voice": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

