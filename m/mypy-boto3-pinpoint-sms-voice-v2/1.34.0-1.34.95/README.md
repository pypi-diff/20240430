# Comparing `tmp/mypy-boto3-pinpoint-sms-voice-v2-1.34.0.tar.gz` & `tmp/mypy_boto3_pinpoint_sms_voice_v2-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-sms-voice-v2-1.34.0.tar", last modified: Wed Dec 13 21:23:31 2023, max compression
+gzip compressed data, was "mypy_boto3_pinpoint_sms_voice_v2-1.34.95.tar", last modified: Tue Apr 30 19:34:53 2024, max compression
```

## Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0.tar` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:31.091321 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16886 2023-12-13 21:23:31.091321 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15300 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:31.091321 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64263 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    64259 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18065 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18063 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28119 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    28097 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    73556 2023-12-13 21:15:31.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    73555 2023-12-13 21:15:30.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:31.091321 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16886 2023-12-13 21:23:31.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 21:23:31.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:31.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:31.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:31.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 21:23:31.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:31.091321 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-12-13 21:15:29.000000 mypy-boto3-pinpoint-sms-voice-v2-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.167048 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:32:15.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-30 19:34:53.167048 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-04-30 19:32:15.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.167048 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-30 19:32:15.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-30 19:32:15.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-30 19:32:15.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74463 2024-04-30 19:32:17.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74460 2024-04-30 19:32:16.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-04-30 19:32:17.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-04-30 19:32:17.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29582 2024-04-30 19:32:17.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29560 2024-04-30 19:32:17.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:15.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    83751 2024-04-30 19:32:18.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83751 2024-04-30 19:32:18.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:32:15.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.167048 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-30 19:34:53.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 19:34:53.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:53.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:53.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:53.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 19:34:53.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:53.167048 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-30 19:32:15.000000 mypy_boto3_pinpoint_sms_voice_v2-1.34.95/setup.py
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/LICENSE` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/LICENSE`

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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/PKG-INFO` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-sms-voice-v2
-Version: 1.34.0
-Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.95
+Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
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
 
 <a id="mypy-boto3-pinpoint-sms-voice-v2"></a>
 
 # mypy-boto3-pinpoint-sms-voice-v2
 
 [![PyPI - mypy-boto3-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,14 +290,15 @@
     DescribeAccountLimitsPaginator,
     DescribeConfigurationSetsPaginator,
     DescribeKeywordsPaginator,
     DescribeOptOutListsPaginator,
     DescribeOptedOutNumbersPaginator,
     DescribePhoneNumbersPaginator,
     DescribePoolsPaginator,
+    DescribeProtectConfigurationsPaginator,
     DescribeRegistrationAttachmentsPaginator,
     DescribeRegistrationFieldDefinitionsPaginator,
     DescribeRegistrationFieldValuesPaginator,
     DescribeRegistrationSectionDefinitionsPaginator,
     DescribeRegistrationTypeDefinitionsPaginator,
     DescribeRegistrationVersionsPaginator,
     DescribeRegistrationsPaginator,
@@ -328,14 +329,17 @@
 describe_opted_out_numbers_paginator: DescribeOptedOutNumbersPaginator = client.get_paginator(
     "describe_opted_out_numbers"
 )
 describe_phone_numbers_paginator: DescribePhoneNumbersPaginator = client.get_paginator(
     "describe_phone_numbers"
 )
 describe_pools_paginator: DescribePoolsPaginator = client.get_paginator("describe_pools")
+describe_protect_configurations_paginator: DescribeProtectConfigurationsPaginator = (
+    client.get_paginator("describe_protect_configurations")
+)
 describe_registration_attachments_paginator: DescribeRegistrationAttachmentsPaginator = (
     client.get_paginator("describe_registration_attachments")
 )
 describe_registration_field_definitions_paginator: DescribeRegistrationFieldDefinitionsPaginator = (
     client.get_paginator("describe_registration_field_definitions")
 )
 describe_registration_field_values_paginator: DescribeRegistrationFieldValuesPaginator = (
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/README.md` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,14 +257,15 @@
     DescribeAccountLimitsPaginator,
     DescribeConfigurationSetsPaginator,
     DescribeKeywordsPaginator,
     DescribeOptOutListsPaginator,
     DescribeOptedOutNumbersPaginator,
     DescribePhoneNumbersPaginator,
     DescribePoolsPaginator,
+    DescribeProtectConfigurationsPaginator,
     DescribeRegistrationAttachmentsPaginator,
     DescribeRegistrationFieldDefinitionsPaginator,
     DescribeRegistrationFieldValuesPaginator,
     DescribeRegistrationSectionDefinitionsPaginator,
     DescribeRegistrationTypeDefinitionsPaginator,
     DescribeRegistrationVersionsPaginator,
     DescribeRegistrationsPaginator,
@@ -295,14 +296,17 @@
 describe_opted_out_numbers_paginator: DescribeOptedOutNumbersPaginator = client.get_paginator(
     "describe_opted_out_numbers"
 )
 describe_phone_numbers_paginator: DescribePhoneNumbersPaginator = client.get_paginator(
     "describe_phone_numbers"
 )
 describe_pools_paginator: DescribePoolsPaginator = client.get_paginator("describe_pools")
+describe_protect_configurations_paginator: DescribeProtectConfigurationsPaginator = (
+    client.get_paginator("describe_protect_configurations")
+)
 describe_registration_attachments_paginator: DescribeRegistrationAttachmentsPaginator = (
     client.get_paginator("describe_registration_attachments")
 )
 describe_registration_field_definitions_paginator: DescribeRegistrationFieldDefinitionsPaginator = (
     client.get_paginator("describe_registration_field_definitions")
 )
 describe_registration_field_values_paginator: DescribeRegistrationFieldValuesPaginator = (
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.py` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         DescribeAccountLimitsPaginator,
         DescribeConfigurationSetsPaginator,
         DescribeKeywordsPaginator,
         DescribeOptOutListsPaginator,
         DescribeOptedOutNumbersPaginator,
         DescribePhoneNumbersPaginator,
         DescribePoolsPaginator,
+        DescribeProtectConfigurationsPaginator,
         DescribeRegistrationAttachmentsPaginator,
         DescribeRegistrationFieldDefinitionsPaginator,
         DescribeRegistrationFieldValuesPaginator,
         DescribeRegistrationSectionDefinitionsPaginator,
         DescribeRegistrationTypeDefinitionsPaginator,
         DescribeRegistrationVersionsPaginator,
         DescribeRegistrationsPaginator,
@@ -37,14 +38,15 @@
     describe_account_limits_paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
     describe_configuration_sets_paginator: DescribeConfigurationSetsPaginator = client.get_paginator("describe_configuration_sets")
     describe_keywords_paginator: DescribeKeywordsPaginator = client.get_paginator("describe_keywords")
     describe_opt_out_lists_paginator: DescribeOptOutListsPaginator = client.get_paginator("describe_opt_out_lists")
     describe_opted_out_numbers_paginator: DescribeOptedOutNumbersPaginator = client.get_paginator("describe_opted_out_numbers")
     describe_phone_numbers_paginator: DescribePhoneNumbersPaginator = client.get_paginator("describe_phone_numbers")
     describe_pools_paginator: DescribePoolsPaginator = client.get_paginator("describe_pools")
+    describe_protect_configurations_paginator: DescribeProtectConfigurationsPaginator = client.get_paginator("describe_protect_configurations")
     describe_registration_attachments_paginator: DescribeRegistrationAttachmentsPaginator = client.get_paginator("describe_registration_attachments")
     describe_registration_field_definitions_paginator: DescribeRegistrationFieldDefinitionsPaginator = client.get_paginator("describe_registration_field_definitions")
     describe_registration_field_values_paginator: DescribeRegistrationFieldValuesPaginator = client.get_paginator("describe_registration_field_values")
     describe_registration_section_definitions_paginator: DescribeRegistrationSectionDefinitionsPaginator = client.get_paginator("describe_registration_section_definitions")
     describe_registration_type_definitions_paginator: DescribeRegistrationTypeDefinitionsPaginator = client.get_paginator("describe_registration_type_definitions")
     describe_registration_versions_paginator: DescribeRegistrationVersionsPaginator = client.get_paginator("describe_registration_versions")
     describe_registrations_paginator: DescribeRegistrationsPaginator = client.get_paginator("describe_registrations")
@@ -62,14 +64,15 @@
     DescribeAccountLimitsPaginator,
     DescribeConfigurationSetsPaginator,
     DescribeKeywordsPaginator,
     DescribeOptedOutNumbersPaginator,
     DescribeOptOutListsPaginator,
     DescribePhoneNumbersPaginator,
     DescribePoolsPaginator,
+    DescribeProtectConfigurationsPaginator,
     DescribeRegistrationAttachmentsPaginator,
     DescribeRegistrationFieldDefinitionsPaginator,
     DescribeRegistrationFieldValuesPaginator,
     DescribeRegistrationSectionDefinitionsPaginator,
     DescribeRegistrationsPaginator,
     DescribeRegistrationTypeDefinitionsPaginator,
     DescribeRegistrationVersionsPaginator,
@@ -78,25 +81,25 @@
     DescribeVerifiedDestinationNumbersPaginator,
     ListPoolOriginationIdentitiesPaginator,
     ListRegistrationAssociationsPaginator,
 )
 
 Client = PinpointSMSVoiceV2Client
 
-
 __all__ = (
     "Client",
     "DescribeAccountAttributesPaginator",
     "DescribeAccountLimitsPaginator",
     "DescribeConfigurationSetsPaginator",
     "DescribeKeywordsPaginator",
     "DescribeOptOutListsPaginator",
     "DescribeOptedOutNumbersPaginator",
     "DescribePhoneNumbersPaginator",
     "DescribePoolsPaginator",
+    "DescribeProtectConfigurationsPaginator",
     "DescribeRegistrationAttachmentsPaginator",
     "DescribeRegistrationFieldDefinitionsPaginator",
     "DescribeRegistrationFieldValuesPaginator",
     "DescribeRegistrationSectionDefinitionsPaginator",
     "DescribeRegistrationTypeDefinitionsPaginator",
     "DescribeRegistrationVersionsPaginator",
     "DescribeRegistrationsPaginator",
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         DescribeAccountLimitsPaginator,
         DescribeConfigurationSetsPaginator,
         DescribeKeywordsPaginator,
         DescribeOptOutListsPaginator,
         DescribeOptedOutNumbersPaginator,
         DescribePhoneNumbersPaginator,
         DescribePoolsPaginator,
+        DescribeProtectConfigurationsPaginator,
         DescribeRegistrationAttachmentsPaginator,
         DescribeRegistrationFieldDefinitionsPaginator,
         DescribeRegistrationFieldValuesPaginator,
         DescribeRegistrationSectionDefinitionsPaginator,
         DescribeRegistrationTypeDefinitionsPaginator,
         DescribeRegistrationVersionsPaginator,
         DescribeRegistrationsPaginator,
@@ -37,14 +38,15 @@
     describe_account_limits_paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
     describe_configuration_sets_paginator: DescribeConfigurationSetsPaginator = client.get_paginator("describe_configuration_sets")
     describe_keywords_paginator: DescribeKeywordsPaginator = client.get_paginator("describe_keywords")
     describe_opt_out_lists_paginator: DescribeOptOutListsPaginator = client.get_paginator("describe_opt_out_lists")
     describe_opted_out_numbers_paginator: DescribeOptedOutNumbersPaginator = client.get_paginator("describe_opted_out_numbers")
     describe_phone_numbers_paginator: DescribePhoneNumbersPaginator = client.get_paginator("describe_phone_numbers")
     describe_pools_paginator: DescribePoolsPaginator = client.get_paginator("describe_pools")
+    describe_protect_configurations_paginator: DescribeProtectConfigurationsPaginator = client.get_paginator("describe_protect_configurations")
     describe_registration_attachments_paginator: DescribeRegistrationAttachmentsPaginator = client.get_paginator("describe_registration_attachments")
     describe_registration_field_definitions_paginator: DescribeRegistrationFieldDefinitionsPaginator = client.get_paginator("describe_registration_field_definitions")
     describe_registration_field_values_paginator: DescribeRegistrationFieldValuesPaginator = client.get_paginator("describe_registration_field_values")
     describe_registration_section_definitions_paginator: DescribeRegistrationSectionDefinitionsPaginator = client.get_paginator("describe_registration_section_definitions")
     describe_registration_type_definitions_paginator: DescribeRegistrationTypeDefinitionsPaginator = client.get_paginator("describe_registration_type_definitions")
     describe_registration_versions_paginator: DescribeRegistrationVersionsPaginator = client.get_paginator("describe_registration_versions")
     describe_registrations_paginator: DescribeRegistrationsPaginator = client.get_paginator("describe_registrations")
@@ -62,14 +64,15 @@
     DescribeAccountLimitsPaginator,
     DescribeConfigurationSetsPaginator,
     DescribeKeywordsPaginator,
     DescribeOptedOutNumbersPaginator,
     DescribeOptOutListsPaginator,
     DescribePhoneNumbersPaginator,
     DescribePoolsPaginator,
+    DescribeProtectConfigurationsPaginator,
     DescribeRegistrationAttachmentsPaginator,
     DescribeRegistrationFieldDefinitionsPaginator,
     DescribeRegistrationFieldValuesPaginator,
     DescribeRegistrationSectionDefinitionsPaginator,
     DescribeRegistrationsPaginator,
     DescribeRegistrationTypeDefinitionsPaginator,
     DescribeRegistrationVersionsPaginator,
@@ -88,14 +91,15 @@
     "DescribeAccountLimitsPaginator",
     "DescribeConfigurationSetsPaginator",
     "DescribeKeywordsPaginator",
     "DescribeOptOutListsPaginator",
     "DescribeOptedOutNumbersPaginator",
     "DescribePhoneNumbersPaginator",
     "DescribePoolsPaginator",
+    "DescribeProtectConfigurationsPaginator",
     "DescribeRegistrationAttachmentsPaginator",
     "DescribeRegistrationFieldDefinitionsPaginator",
     "DescribeRegistrationFieldValuesPaginator",
     "DescribeRegistrationSectionDefinitionsPaginator",
     "DescribeRegistrationTypeDefinitionsPaginator",
     "DescribeRegistrationVersionsPaginator",
     "DescribeRegistrationsPaginator",
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/__main__.py` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointSMSVoiceV2 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2//\nBoto3"
-        " docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.PinpointSMSVoiceV2 1.34.95\n"
+        "Version:         1.34.95\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2\n"
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/client.py` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     DescribeAccountLimitsPaginator,
     DescribeConfigurationSetsPaginator,
     DescribeKeywordsPaginator,
     DescribeOptedOutNumbersPaginator,
     DescribeOptOutListsPaginator,
     DescribePhoneNumbersPaginator,
     DescribePoolsPaginator,
+    DescribeProtectConfigurationsPaginator,
     DescribeRegistrationAttachmentsPaginator,
     DescribeRegistrationFieldDefinitionsPaginator,
     DescribeRegistrationFieldValuesPaginator,
     DescribeRegistrationSectionDefinitionsPaginator,
     DescribeRegistrationsPaginator,
     DescribeRegistrationTypeDefinitionsPaginator,
     DescribeRegistrationVersionsPaginator,
@@ -51,69 +52,79 @@
     DescribeSpendLimitsPaginator,
     DescribeVerifiedDestinationNumbersPaginator,
     ListPoolOriginationIdentitiesPaginator,
     ListRegistrationAssociationsPaginator,
 )
 from .type_defs import (
     AssociateOriginationIdentityResultTypeDef,
+    AssociateProtectConfigurationResultTypeDef,
     BlobTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     CreateConfigurationSetResultTypeDef,
     CreateEventDestinationResultTypeDef,
     CreateOptOutListResultTypeDef,
     CreatePoolResultTypeDef,
+    CreateProtectConfigurationResultTypeDef,
     CreateRegistrationAssociationResultTypeDef,
     CreateRegistrationAttachmentResultTypeDef,
     CreateRegistrationResultTypeDef,
     CreateRegistrationVersionResultTypeDef,
     CreateVerifiedDestinationNumberResultTypeDef,
+    DeleteAccountDefaultProtectConfigurationResultTypeDef,
     DeleteConfigurationSetResultTypeDef,
     DeleteDefaultMessageTypeResultTypeDef,
     DeleteDefaultSenderIdResultTypeDef,
     DeleteEventDestinationResultTypeDef,
     DeleteKeywordResultTypeDef,
+    DeleteMediaMessageSpendLimitOverrideResultTypeDef,
     DeleteOptedOutNumberResultTypeDef,
     DeleteOptOutListResultTypeDef,
     DeletePoolResultTypeDef,
+    DeleteProtectConfigurationResultTypeDef,
     DeleteRegistrationAttachmentResultTypeDef,
     DeleteRegistrationFieldValueResultTypeDef,
     DeleteRegistrationResultTypeDef,
     DeleteTextMessageSpendLimitOverrideResultTypeDef,
     DeleteVerifiedDestinationNumberResultTypeDef,
     DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeAccountLimitsResultTypeDef,
     DescribeConfigurationSetsResultTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribePhoneNumbersResultTypeDef,
     DescribePoolsResultTypeDef,
+    DescribeProtectConfigurationsResultTypeDef,
     DescribeRegistrationAttachmentsResultTypeDef,
     DescribeRegistrationFieldDefinitionsResultTypeDef,
     DescribeRegistrationFieldValuesResultTypeDef,
     DescribeRegistrationSectionDefinitionsResultTypeDef,
     DescribeRegistrationsResultTypeDef,
     DescribeRegistrationTypeDefinitionsResultTypeDef,
     DescribeRegistrationVersionsResultTypeDef,
     DescribeSenderIdsResultTypeDef,
     DescribeSpendLimitsResultTypeDef,
     DescribeVerifiedDestinationNumbersResultTypeDef,
     DisassociateOriginationIdentityResultTypeDef,
+    DisassociateProtectConfigurationResultTypeDef,
     DiscardRegistrationVersionResultTypeDef,
+    GetProtectConfigurationCountryRuleSetResultTypeDef,
     KeywordFilterTypeDef,
     KinesisFirehoseDestinationTypeDef,
     ListPoolOriginationIdentitiesResultTypeDef,
     ListRegistrationAssociationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OptedOutFilterTypeDef,
     PhoneNumberFilterTypeDef,
     PoolFilterTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
+    ProtectConfigurationCountryRuleSetInformationTypeDef,
+    ProtectConfigurationFilterTypeDef,
     PutKeywordResultTypeDef,
     PutOptedOutNumberResultTypeDef,
     PutRegistrationFieldValueResultTypeDef,
     RegistrationAssociationFilterTypeDef,
     RegistrationAttachmentFilterTypeDef,
     RegistrationFilterTypeDef,
     RegistrationTypeFilterTypeDef,
@@ -121,37 +132,41 @@
     ReleasePhoneNumberResultTypeDef,
     ReleaseSenderIdResultTypeDef,
     RequestPhoneNumberResultTypeDef,
     RequestSenderIdResultTypeDef,
     SendDestinationNumberVerificationCodeResultTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
+    SendMediaMessageResultTypeDef,
     SendTextMessageResultTypeDef,
     SendVoiceMessageResultTypeDef,
+    SetAccountDefaultProtectConfigurationResultTypeDef,
     SetDefaultMessageTypeResultTypeDef,
     SetDefaultSenderIdResultTypeDef,
+    SetMediaMessageSpendLimitOverrideResultTypeDef,
     SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideResultTypeDef,
     SnsDestinationTypeDef,
     SubmitRegistrationVersionResultTypeDef,
     TagTypeDef,
     UpdateEventDestinationResultTypeDef,
     UpdatePhoneNumberResultTypeDef,
     UpdatePoolResultTypeDef,
+    UpdateProtectConfigurationCountryRuleSetResultTypeDef,
+    UpdateProtectConfigurationResultTypeDef,
     UpdateSenderIdResultTypeDef,
     VerifiedDestinationNumberFilterTypeDef,
     VerifyDestinationNumberResultTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PinpointSMSVoiceV2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -193,14 +208,24 @@
         """
         Associates the specified origination identity with a pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.associate_origination_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#associate_origination_identity)
         """
 
+    def associate_protect_configuration(
+        self, *, ProtectConfigurationId: str, ConfigurationSetName: str
+    ) -> AssociateProtectConfigurationResultTypeDef:
+        """
+        Associate a protect configuration with a configuration set.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.associate_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#associate_protect_configuration)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#can_paginate)
         """
@@ -228,15 +253,15 @@
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         MatchingEventTypes: Sequence[EventTypeType],
         CloudWatchLogsDestination: CloudWatchLogsDestinationTypeDef = ...,
         KinesisFirehoseDestination: KinesisFirehoseDestinationTypeDef = ...,
         SnsDestination: SnsDestinationTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateEventDestinationResultTypeDef:
         """
         Creates a new event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_event_destination)
         """
@@ -255,24 +280,38 @@
         self,
         *,
         OriginationIdentity: str,
         IsoCountryCode: str,
         MessageType: MessageTypeType,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreatePoolResultTypeDef:
         """
         Creates a new pool and associates the specified origination identity to the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_pool)
         """
 
+    def create_protect_configuration(
+        self,
+        *,
+        ClientToken: str = ...,
+        DeletionProtectionEnabled: bool = ...,
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> CreateProtectConfigurationResultTypeDef:
+        """
+        Create a new protect configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_protect_configuration)
+        """
+
     def create_registration(
         self, *, RegistrationType: str, Tags: Sequence[TagTypeDef] = ..., ClientToken: str = ...
     ) -> CreateRegistrationResultTypeDef:
         """
         Creates a new registration based on the **RegistrationType** field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_registration)
@@ -293,15 +332,15 @@
 
     def create_registration_attachment(
         self,
         *,
         AttachmentBody: BlobTypeDef = ...,
         AttachmentUrl: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateRegistrationAttachmentResultTypeDef:
         """
         Create a new registration attachment to use for uploading a file or a URL to a
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_registration_attachment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_registration_attachment)
@@ -318,25 +357,35 @@
         """
 
     def create_verified_destination_number(
         self,
         *,
         DestinationPhoneNumber: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateVerifiedDestinationNumberResultTypeDef:
         """
         You can only send messages to verified destination numbers when your account is
         in the
         sandbox.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_verified_destination_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_verified_destination_number)
         """
 
+    def delete_account_default_protect_configuration(
+        self,
+    ) -> DeleteAccountDefaultProtectConfigurationResultTypeDef:
+        """
+        Removes the current account default protect configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_account_default_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_account_default_protect_configuration)
+        """
+
     def delete_configuration_set(
         self, *, ConfigurationSetName: str
     ) -> DeleteConfigurationSetResultTypeDef:
         """
         Deletes an existing configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_configuration_set)
@@ -379,14 +428,26 @@
         """
         Deletes an existing keyword from an origination phone number or pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_keyword)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_keyword)
         """
 
+    def delete_media_message_spend_limit_override(
+        self,
+    ) -> DeleteMediaMessageSpendLimitOverrideResultTypeDef:
+        """
+        Deletes an account-level monthly spending limit override for sending multimedia
+        messages
+        (MMS).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_media_message_spend_limit_override)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_media_message_spend_limit_override)
+        """
+
     def delete_opt_out_list(self, *, OptOutListName: str) -> DeleteOptOutListResultTypeDef:
         """
         Deletes an existing opt-out list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_opt_out_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_opt_out_list)
         """
@@ -407,14 +468,24 @@
         """
         Deletes an existing pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_pool)
         """
 
+    def delete_protect_configuration(
+        self, *, ProtectConfigurationId: str
+    ) -> DeleteProtectConfigurationResultTypeDef:
+        """
+        Permanently delete the protect configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_protect_configuration)
+        """
+
     def delete_registration(self, *, RegistrationId: str) -> DeleteRegistrationResultTypeDef:
         """
         Permanently delete an existing registration from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_registration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_registration)
         """
@@ -494,15 +565,15 @@
 
     def describe_configuration_sets(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeConfigurationSetsResultTypeDef:
         """
         Describes the specified configuration sets or all in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_configuration_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_configuration_sets)
         """
@@ -510,15 +581,15 @@
     def describe_keywords(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeKeywordsResultTypeDef:
         """
         Describes the specified keywords or all keywords on your origination phone
         number or
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_keywords)
@@ -538,15 +609,15 @@
     def describe_opted_out_numbers(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeOptedOutNumbersResultTypeDef:
         """
         Describes the specified opted out destination numbers or all opted out
         destination numbers in an opt-out
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_opted_out_numbers)
@@ -555,15 +626,15 @@
 
     def describe_phone_numbers(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribePhoneNumbersResultTypeDef:
         """
         Describes the specified origination phone number, or all the phone numbers in
         your
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_phone_numbers)
@@ -572,32 +643,47 @@
 
     def describe_pools(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribePoolsResultTypeDef:
         """
         Retrieves the specified pools or all pools associated with your Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_pools)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_pools)
         """
 
+    def describe_protect_configurations(
+        self,
+        *,
+        ProtectConfigurationIds: Sequence[str] = ...,
+        Filters: Sequence[ProtectConfigurationFilterTypeDef] = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+    ) -> DescribeProtectConfigurationsResultTypeDef:
+        """
+        Retrieves the protect configurations that match any of filters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_protect_configurations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_protect_configurations)
+        """
+
     def describe_registration_attachments(
         self,
         *,
         RegistrationAttachmentIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationAttachmentsResultTypeDef:
         """
         Retrieves the specified registration attachments or all registration
         attachments associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_attachments)
@@ -607,15 +693,15 @@
     def describe_registration_field_definitions(
         self,
         *,
         RegistrationType: str,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationFieldDefinitionsResultTypeDef:
         """
         Retrieves the specified registration type field definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_field_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_field_definitions)
         """
@@ -624,45 +710,45 @@
         self,
         *,
         RegistrationId: str,
         VersionNumber: int = ...,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationFieldValuesResultTypeDef:
         """
         Retrieves the specified registration field values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_field_values)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_field_values)
         """
 
     def describe_registration_section_definitions(
         self,
         *,
         RegistrationType: str,
         SectionPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationSectionDefinitionsResultTypeDef:
         """
         Retrieves the specified registration section definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_section_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_section_definitions)
         """
 
     def describe_registration_type_definitions(
         self,
         *,
         RegistrationTypes: Sequence[str] = ...,
         Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationTypeDefinitionsResultTypeDef:
         """
         Retrieves the specified registration type definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_type_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_type_definitions)
         """
@@ -670,45 +756,45 @@
     def describe_registration_versions(
         self,
         *,
         RegistrationId: str,
         VersionNumbers: Sequence[int] = ...,
         Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationVersionsResultTypeDef:
         """
         Retrieves the specified registration version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_versions)
         """
 
     def describe_registrations(
         self,
         *,
         RegistrationIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationsResultTypeDef:
         """
         Retrieves the specified registrations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registrations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registrations)
         """
 
     def describe_sender_ids(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeSenderIdsResultTypeDef:
         """
         Describes the specified SenderIds or all SenderIds associated with your Amazon
         Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_sender_ids)
@@ -730,15 +816,15 @@
     def describe_verified_destination_numbers(
         self,
         *,
         VerifiedDestinationNumberIds: Sequence[str] = ...,
         DestinationPhoneNumbers: Sequence[str] = ...,
         Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeVerifiedDestinationNumbersResultTypeDef:
         """
         Retrieves the specified verified destiona numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_verified_destination_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_verified_destination_numbers)
         """
@@ -749,14 +835,24 @@
         """
         Removes the specified origination identity from an existing pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.disassociate_origination_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#disassociate_origination_identity)
         """
 
+    def disassociate_protect_configuration(
+        self, *, ProtectConfigurationId: str, ConfigurationSetName: str
+    ) -> DisassociateProtectConfigurationResultTypeDef:
+        """
+        Disassociate a protect configuration from a configuration set.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.disassociate_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#disassociate_protect_configuration)
+        """
+
     def discard_registration_version(
         self, *, RegistrationId: str
     ) -> DiscardRegistrationVersionResultTypeDef:
         """
         Discard the current version of the registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.discard_registration_version)
@@ -773,36 +869,47 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#generate_presigned_url)
         """
 
+    def get_protect_configuration_country_rule_set(
+        self, *, ProtectConfigurationId: str, NumberCapability: NumberCapabilityType
+    ) -> GetProtectConfigurationCountryRuleSetResultTypeDef:
+        """
+        Retrieve the CountryRuleSet for the specified NumberCapability from a protect
+        configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.get_protect_configuration_country_rule_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#get_protect_configuration_country_rule_set)
+        """
+
     def list_pool_origination_identities(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPoolOriginationIdentitiesResultTypeDef:
         """
         Lists all associated origination identities in your pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.list_pool_origination_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#list_pool_origination_identities)
         """
 
     def list_registration_associations(
         self,
         *,
         RegistrationId: str,
         Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRegistrationAssociationsResultTypeDef:
         """
         Retreive all of the origination identies that are associated with a
         registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.list_registration_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#list_registration_associations)
@@ -818,15 +925,15 @@
 
     def put_keyword(
         self,
         *,
         OriginationIdentity: str,
         Keyword: str,
         KeywordMessage: str,
-        KeywordAction: KeywordActionType = ...
+        KeywordAction: KeywordActionType = ...,
     ) -> PutKeywordResultTypeDef:
         """
         Creates or updates a keyword configuration on an origination phone number or
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.put_keyword)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#put_keyword)
@@ -845,15 +952,15 @@
     def put_registration_field_value(
         self,
         *,
         RegistrationId: str,
         FieldPath: str,
         SelectChoices: Sequence[str] = ...,
         TextValue: str = ...,
-        RegistrationAttachmentId: str = ...
+        RegistrationAttachmentId: str = ...,
     ) -> PutRegistrationFieldValueResultTypeDef:
         """
         Creates or updates a field value for a registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.put_registration_field_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#put_registration_field_value)
         """
@@ -884,15 +991,15 @@
         NumberCapabilities: Sequence[NumberCapabilityType],
         NumberType: RequestableNumberTypeType,
         OptOutListName: str = ...,
         PoolId: str = ...,
         RegistrationId: str = ...,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RequestPhoneNumberResultTypeDef:
         """
         Request an origination phone number for use in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.request_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#request_phone_number)
         """
@@ -901,15 +1008,15 @@
         self,
         *,
         SenderId: str,
         IsoCountryCode: str,
         MessageTypes: Sequence[MessageTypeType] = ...,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RequestSenderIdResultTypeDef:
         """
         Request a new sender ID that doesn't require registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.request_sender_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#request_sender_id)
         """
@@ -919,39 +1026,62 @@
         *,
         VerifiedDestinationNumberId: str,
         VerificationChannel: VerificationChannelType,
         LanguageCode: LanguageCodeType = ...,
         OriginationIdentity: str = ...,
         ConfigurationSetName: str = ...,
         Context: Mapping[str, str] = ...,
-        DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...
+        DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...,
     ) -> SendDestinationNumberVerificationCodeResultTypeDef:
         """
         Before you can send test messages to a verified destination phone number you
         need to opt-in the verified destination phone
         number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_destination_number_verification_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#send_destination_number_verification_code)
         """
 
+    def send_media_message(
+        self,
+        *,
+        DestinationPhoneNumber: str,
+        OriginationIdentity: str,
+        MessageBody: str = ...,
+        MediaUrls: Sequence[str] = ...,
+        ConfigurationSetName: str = ...,
+        MaxPrice: str = ...,
+        TimeToLive: int = ...,
+        Context: Mapping[str, str] = ...,
+        DryRun: bool = ...,
+        ProtectConfigurationId: str = ...,
+    ) -> SendMediaMessageResultTypeDef:
+        """
+        Creates a new multimedia message (MMS) and sends it to a recipient's phone
+        number.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_media_message)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#send_media_message)
+        """
+
     def send_text_message(
         self,
         *,
         DestinationPhoneNumber: str,
         OriginationIdentity: str = ...,
         MessageBody: str = ...,
         MessageType: MessageTypeType = ...,
         Keyword: str = ...,
         ConfigurationSetName: str = ...,
         MaxPrice: str = ...,
         TimeToLive: int = ...,
         Context: Mapping[str, str] = ...,
         DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
+        ProtectConfigurationId: str = ...,
     ) -> SendTextMessageResultTypeDef:
         """
         Creates a new text message and sends it to a recipient's phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_text_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#send_text_message)
         """
@@ -964,23 +1094,34 @@
         MessageBody: str = ...,
         MessageBodyTextType: VoiceMessageBodyTextTypeType = ...,
         VoiceId: VoiceIdType = ...,
         ConfigurationSetName: str = ...,
         MaxPricePerMinute: str = ...,
         TimeToLive: int = ...,
         Context: Mapping[str, str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
+        ProtectConfigurationId: str = ...,
     ) -> SendVoiceMessageResultTypeDef:
         """
         Allows you to send a request that sends a voice message through Amazon Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_voice_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#send_voice_message)
         """
 
+    def set_account_default_protect_configuration(
+        self, *, ProtectConfigurationId: str
+    ) -> SetAccountDefaultProtectConfigurationResultTypeDef:
+        """
+        Set a protect configuration as your account default.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_account_default_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#set_account_default_protect_configuration)
+        """
+
     def set_default_message_type(
         self, *, ConfigurationSetName: str, MessageType: MessageTypeType
     ) -> SetDefaultMessageTypeResultTypeDef:
         """
         Sets the default message type on a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_default_message_type)
@@ -993,14 +1134,24 @@
         """
         Sets default sender ID on a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_default_sender_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#set_default_sender_id)
         """
 
+    def set_media_message_spend_limit_override(
+        self, *, MonthlyLimit: int
+    ) -> SetMediaMessageSpendLimitOverrideResultTypeDef:
+        """
+        Sets an account level monthly spend limit override for sending MMS messages.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_media_message_spend_limit_override)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#set_media_message_spend_limit_override)
+        """
+
     def set_text_message_spend_limit_override(
         self, *, MonthlyLimit: int
     ) -> SetTextMessageSpendLimitOverrideResultTypeDef:
         """
         Sets an account level monthly spend limit override for sending text messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_text_message_spend_limit_override)
@@ -1052,15 +1203,15 @@
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         Enabled: bool = ...,
         MatchingEventTypes: Sequence[EventTypeType] = ...,
         CloudWatchLogsDestination: CloudWatchLogsDestinationTypeDef = ...,
         KinesisFirehoseDestination: KinesisFirehoseDestinationTypeDef = ...,
-        SnsDestination: SnsDestinationTypeDef = ...
+        SnsDestination: SnsDestinationTypeDef = ...,
     ) -> UpdateEventDestinationResultTypeDef:
         """
         Updates an existing event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_event_destination)
         """
@@ -1070,15 +1221,15 @@
         *,
         PhoneNumberId: str,
         TwoWayEnabled: bool = ...,
         TwoWayChannelArn: str = ...,
         TwoWayChannelRole: str = ...,
         SelfManagedOptOutsEnabled: bool = ...,
         OptOutListName: str = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdatePhoneNumberResultTypeDef:
         """
         Updates the configuration of an existing origination phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_phone_number)
         """
@@ -1089,23 +1240,49 @@
         PoolId: str,
         TwoWayEnabled: bool = ...,
         TwoWayChannelArn: str = ...,
         TwoWayChannelRole: str = ...,
         SelfManagedOptOutsEnabled: bool = ...,
         OptOutListName: str = ...,
         SharedRoutesEnabled: bool = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdatePoolResultTypeDef:
         """
         Updates the configuration of an existing pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_pool)
         """
 
+    def update_protect_configuration(
+        self, *, ProtectConfigurationId: str, DeletionProtectionEnabled: bool = ...
+    ) -> UpdateProtectConfigurationResultTypeDef:
+        """
+        Update the setting for an existing protect configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_protect_configuration)
+        """
+
+    def update_protect_configuration_country_rule_set(
+        self,
+        *,
+        ProtectConfigurationId: str,
+        NumberCapability: NumberCapabilityType,
+        CountryRuleSetUpdates: Mapping[str, ProtectConfigurationCountryRuleSetInformationTypeDef],
+    ) -> UpdateProtectConfigurationCountryRuleSetResultTypeDef:
+        """
+        Update a country rule set to `ALLOW` or `BLOCK` messages to be sent to the
+        specified destination
+        counties.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_protect_configuration_country_rule_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_protect_configuration_country_rule_set)
+        """
+
     def update_sender_id(
         self, *, SenderId: str, IsoCountryCode: str, DeletionProtectionEnabled: bool = ...
     ) -> UpdateSenderIdResultTypeDef:
         """
         Updates the configuration of an existing sender ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_sender_id)
@@ -1192,14 +1369,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_protect_configurations"]
+    ) -> DescribeProtectConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_registration_attachments"]
     ) -> DescribeRegistrationAttachmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/client.pyi` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     DescribeAccountLimitsPaginator,
     DescribeConfigurationSetsPaginator,
     DescribeKeywordsPaginator,
     DescribeOptedOutNumbersPaginator,
     DescribeOptOutListsPaginator,
     DescribePhoneNumbersPaginator,
     DescribePoolsPaginator,
+    DescribeProtectConfigurationsPaginator,
     DescribeRegistrationAttachmentsPaginator,
     DescribeRegistrationFieldDefinitionsPaginator,
     DescribeRegistrationFieldValuesPaginator,
     DescribeRegistrationSectionDefinitionsPaginator,
     DescribeRegistrationsPaginator,
     DescribeRegistrationTypeDefinitionsPaginator,
     DescribeRegistrationVersionsPaginator,
@@ -51,69 +52,79 @@
     DescribeSpendLimitsPaginator,
     DescribeVerifiedDestinationNumbersPaginator,
     ListPoolOriginationIdentitiesPaginator,
     ListRegistrationAssociationsPaginator,
 )
 from .type_defs import (
     AssociateOriginationIdentityResultTypeDef,
+    AssociateProtectConfigurationResultTypeDef,
     BlobTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     CreateConfigurationSetResultTypeDef,
     CreateEventDestinationResultTypeDef,
     CreateOptOutListResultTypeDef,
     CreatePoolResultTypeDef,
+    CreateProtectConfigurationResultTypeDef,
     CreateRegistrationAssociationResultTypeDef,
     CreateRegistrationAttachmentResultTypeDef,
     CreateRegistrationResultTypeDef,
     CreateRegistrationVersionResultTypeDef,
     CreateVerifiedDestinationNumberResultTypeDef,
+    DeleteAccountDefaultProtectConfigurationResultTypeDef,
     DeleteConfigurationSetResultTypeDef,
     DeleteDefaultMessageTypeResultTypeDef,
     DeleteDefaultSenderIdResultTypeDef,
     DeleteEventDestinationResultTypeDef,
     DeleteKeywordResultTypeDef,
+    DeleteMediaMessageSpendLimitOverrideResultTypeDef,
     DeleteOptedOutNumberResultTypeDef,
     DeleteOptOutListResultTypeDef,
     DeletePoolResultTypeDef,
+    DeleteProtectConfigurationResultTypeDef,
     DeleteRegistrationAttachmentResultTypeDef,
     DeleteRegistrationFieldValueResultTypeDef,
     DeleteRegistrationResultTypeDef,
     DeleteTextMessageSpendLimitOverrideResultTypeDef,
     DeleteVerifiedDestinationNumberResultTypeDef,
     DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeAccountLimitsResultTypeDef,
     DescribeConfigurationSetsResultTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribePhoneNumbersResultTypeDef,
     DescribePoolsResultTypeDef,
+    DescribeProtectConfigurationsResultTypeDef,
     DescribeRegistrationAttachmentsResultTypeDef,
     DescribeRegistrationFieldDefinitionsResultTypeDef,
     DescribeRegistrationFieldValuesResultTypeDef,
     DescribeRegistrationSectionDefinitionsResultTypeDef,
     DescribeRegistrationsResultTypeDef,
     DescribeRegistrationTypeDefinitionsResultTypeDef,
     DescribeRegistrationVersionsResultTypeDef,
     DescribeSenderIdsResultTypeDef,
     DescribeSpendLimitsResultTypeDef,
     DescribeVerifiedDestinationNumbersResultTypeDef,
     DisassociateOriginationIdentityResultTypeDef,
+    DisassociateProtectConfigurationResultTypeDef,
     DiscardRegistrationVersionResultTypeDef,
+    GetProtectConfigurationCountryRuleSetResultTypeDef,
     KeywordFilterTypeDef,
     KinesisFirehoseDestinationTypeDef,
     ListPoolOriginationIdentitiesResultTypeDef,
     ListRegistrationAssociationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OptedOutFilterTypeDef,
     PhoneNumberFilterTypeDef,
     PoolFilterTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
+    ProtectConfigurationCountryRuleSetInformationTypeDef,
+    ProtectConfigurationFilterTypeDef,
     PutKeywordResultTypeDef,
     PutOptedOutNumberResultTypeDef,
     PutRegistrationFieldValueResultTypeDef,
     RegistrationAssociationFilterTypeDef,
     RegistrationAttachmentFilterTypeDef,
     RegistrationFilterTypeDef,
     RegistrationTypeFilterTypeDef,
@@ -121,26 +132,31 @@
     ReleasePhoneNumberResultTypeDef,
     ReleaseSenderIdResultTypeDef,
     RequestPhoneNumberResultTypeDef,
     RequestSenderIdResultTypeDef,
     SendDestinationNumberVerificationCodeResultTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
+    SendMediaMessageResultTypeDef,
     SendTextMessageResultTypeDef,
     SendVoiceMessageResultTypeDef,
+    SetAccountDefaultProtectConfigurationResultTypeDef,
     SetDefaultMessageTypeResultTypeDef,
     SetDefaultSenderIdResultTypeDef,
+    SetMediaMessageSpendLimitOverrideResultTypeDef,
     SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideResultTypeDef,
     SnsDestinationTypeDef,
     SubmitRegistrationVersionResultTypeDef,
     TagTypeDef,
     UpdateEventDestinationResultTypeDef,
     UpdatePhoneNumberResultTypeDef,
     UpdatePoolResultTypeDef,
+    UpdateProtectConfigurationCountryRuleSetResultTypeDef,
+    UpdateProtectConfigurationResultTypeDef,
     UpdateSenderIdResultTypeDef,
     VerifiedDestinationNumberFilterTypeDef,
     VerifyDestinationNumberResultTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -189,14 +205,24 @@
         """
         Associates the specified origination identity with a pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.associate_origination_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#associate_origination_identity)
         """
 
+    def associate_protect_configuration(
+        self, *, ProtectConfigurationId: str, ConfigurationSetName: str
+    ) -> AssociateProtectConfigurationResultTypeDef:
+        """
+        Associate a protect configuration with a configuration set.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.associate_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#associate_protect_configuration)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#can_paginate)
         """
@@ -224,15 +250,15 @@
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         MatchingEventTypes: Sequence[EventTypeType],
         CloudWatchLogsDestination: CloudWatchLogsDestinationTypeDef = ...,
         KinesisFirehoseDestination: KinesisFirehoseDestinationTypeDef = ...,
         SnsDestination: SnsDestinationTypeDef = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateEventDestinationResultTypeDef:
         """
         Creates a new event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_event_destination)
         """
@@ -251,24 +277,38 @@
         self,
         *,
         OriginationIdentity: str,
         IsoCountryCode: str,
         MessageType: MessageTypeType,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreatePoolResultTypeDef:
         """
         Creates a new pool and associates the specified origination identity to the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_pool)
         """
 
+    def create_protect_configuration(
+        self,
+        *,
+        ClientToken: str = ...,
+        DeletionProtectionEnabled: bool = ...,
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> CreateProtectConfigurationResultTypeDef:
+        """
+        Create a new protect configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_protect_configuration)
+        """
+
     def create_registration(
         self, *, RegistrationType: str, Tags: Sequence[TagTypeDef] = ..., ClientToken: str = ...
     ) -> CreateRegistrationResultTypeDef:
         """
         Creates a new registration based on the **RegistrationType** field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_registration)
@@ -289,15 +329,15 @@
 
     def create_registration_attachment(
         self,
         *,
         AttachmentBody: BlobTypeDef = ...,
         AttachmentUrl: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateRegistrationAttachmentResultTypeDef:
         """
         Create a new registration attachment to use for uploading a file or a URL to a
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_registration_attachment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_registration_attachment)
@@ -314,25 +354,35 @@
         """
 
     def create_verified_destination_number(
         self,
         *,
         DestinationPhoneNumber: str,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateVerifiedDestinationNumberResultTypeDef:
         """
         You can only send messages to verified destination numbers when your account is
         in the
         sandbox.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.create_verified_destination_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#create_verified_destination_number)
         """
 
+    def delete_account_default_protect_configuration(
+        self,
+    ) -> DeleteAccountDefaultProtectConfigurationResultTypeDef:
+        """
+        Removes the current account default protect configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_account_default_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_account_default_protect_configuration)
+        """
+
     def delete_configuration_set(
         self, *, ConfigurationSetName: str
     ) -> DeleteConfigurationSetResultTypeDef:
         """
         Deletes an existing configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_configuration_set)
@@ -375,14 +425,26 @@
         """
         Deletes an existing keyword from an origination phone number or pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_keyword)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_keyword)
         """
 
+    def delete_media_message_spend_limit_override(
+        self,
+    ) -> DeleteMediaMessageSpendLimitOverrideResultTypeDef:
+        """
+        Deletes an account-level monthly spending limit override for sending multimedia
+        messages
+        (MMS).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_media_message_spend_limit_override)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_media_message_spend_limit_override)
+        """
+
     def delete_opt_out_list(self, *, OptOutListName: str) -> DeleteOptOutListResultTypeDef:
         """
         Deletes an existing opt-out list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_opt_out_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_opt_out_list)
         """
@@ -403,14 +465,24 @@
         """
         Deletes an existing pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_pool)
         """
 
+    def delete_protect_configuration(
+        self, *, ProtectConfigurationId: str
+    ) -> DeleteProtectConfigurationResultTypeDef:
+        """
+        Permanently delete the protect configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_protect_configuration)
+        """
+
     def delete_registration(self, *, RegistrationId: str) -> DeleteRegistrationResultTypeDef:
         """
         Permanently delete an existing registration from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.delete_registration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#delete_registration)
         """
@@ -490,15 +562,15 @@
 
     def describe_configuration_sets(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeConfigurationSetsResultTypeDef:
         """
         Describes the specified configuration sets or all in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_configuration_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_configuration_sets)
         """
@@ -506,15 +578,15 @@
     def describe_keywords(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeKeywordsResultTypeDef:
         """
         Describes the specified keywords or all keywords on your origination phone
         number or
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_keywords)
@@ -534,15 +606,15 @@
     def describe_opted_out_numbers(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeOptedOutNumbersResultTypeDef:
         """
         Describes the specified opted out destination numbers or all opted out
         destination numbers in an opt-out
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_opted_out_numbers)
@@ -551,15 +623,15 @@
 
     def describe_phone_numbers(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribePhoneNumbersResultTypeDef:
         """
         Describes the specified origination phone number, or all the phone numbers in
         your
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_phone_numbers)
@@ -568,32 +640,47 @@
 
     def describe_pools(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribePoolsResultTypeDef:
         """
         Retrieves the specified pools or all pools associated with your Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_pools)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_pools)
         """
 
+    def describe_protect_configurations(
+        self,
+        *,
+        ProtectConfigurationIds: Sequence[str] = ...,
+        Filters: Sequence[ProtectConfigurationFilterTypeDef] = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+    ) -> DescribeProtectConfigurationsResultTypeDef:
+        """
+        Retrieves the protect configurations that match any of filters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_protect_configurations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_protect_configurations)
+        """
+
     def describe_registration_attachments(
         self,
         *,
         RegistrationAttachmentIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationAttachmentsResultTypeDef:
         """
         Retrieves the specified registration attachments or all registration
         attachments associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_attachments)
@@ -603,15 +690,15 @@
     def describe_registration_field_definitions(
         self,
         *,
         RegistrationType: str,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationFieldDefinitionsResultTypeDef:
         """
         Retrieves the specified registration type field definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_field_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_field_definitions)
         """
@@ -620,45 +707,45 @@
         self,
         *,
         RegistrationId: str,
         VersionNumber: int = ...,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationFieldValuesResultTypeDef:
         """
         Retrieves the specified registration field values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_field_values)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_field_values)
         """
 
     def describe_registration_section_definitions(
         self,
         *,
         RegistrationType: str,
         SectionPaths: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationSectionDefinitionsResultTypeDef:
         """
         Retrieves the specified registration section definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_section_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_section_definitions)
         """
 
     def describe_registration_type_definitions(
         self,
         *,
         RegistrationTypes: Sequence[str] = ...,
         Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationTypeDefinitionsResultTypeDef:
         """
         Retrieves the specified registration type definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_type_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_type_definitions)
         """
@@ -666,45 +753,45 @@
     def describe_registration_versions(
         self,
         *,
         RegistrationId: str,
         VersionNumbers: Sequence[int] = ...,
         Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationVersionsResultTypeDef:
         """
         Retrieves the specified registration version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registration_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registration_versions)
         """
 
     def describe_registrations(
         self,
         *,
         RegistrationIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeRegistrationsResultTypeDef:
         """
         Retrieves the specified registrations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_registrations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_registrations)
         """
 
     def describe_sender_ids(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeSenderIdsResultTypeDef:
         """
         Describes the specified SenderIds or all SenderIds associated with your Amazon
         Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_sender_ids)
@@ -726,15 +813,15 @@
     def describe_verified_destination_numbers(
         self,
         *,
         VerifiedDestinationNumberIds: Sequence[str] = ...,
         DestinationPhoneNumbers: Sequence[str] = ...,
         Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeVerifiedDestinationNumbersResultTypeDef:
         """
         Retrieves the specified verified destiona numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.describe_verified_destination_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#describe_verified_destination_numbers)
         """
@@ -745,14 +832,24 @@
         """
         Removes the specified origination identity from an existing pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.disassociate_origination_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#disassociate_origination_identity)
         """
 
+    def disassociate_protect_configuration(
+        self, *, ProtectConfigurationId: str, ConfigurationSetName: str
+    ) -> DisassociateProtectConfigurationResultTypeDef:
+        """
+        Disassociate a protect configuration from a configuration set.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.disassociate_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#disassociate_protect_configuration)
+        """
+
     def discard_registration_version(
         self, *, RegistrationId: str
     ) -> DiscardRegistrationVersionResultTypeDef:
         """
         Discard the current version of the registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.discard_registration_version)
@@ -769,36 +866,47 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#generate_presigned_url)
         """
 
+    def get_protect_configuration_country_rule_set(
+        self, *, ProtectConfigurationId: str, NumberCapability: NumberCapabilityType
+    ) -> GetProtectConfigurationCountryRuleSetResultTypeDef:
+        """
+        Retrieve the CountryRuleSet for the specified NumberCapability from a protect
+        configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.get_protect_configuration_country_rule_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#get_protect_configuration_country_rule_set)
+        """
+
     def list_pool_origination_identities(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPoolOriginationIdentitiesResultTypeDef:
         """
         Lists all associated origination identities in your pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.list_pool_origination_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#list_pool_origination_identities)
         """
 
     def list_registration_associations(
         self,
         *,
         RegistrationId: str,
         Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRegistrationAssociationsResultTypeDef:
         """
         Retreive all of the origination identies that are associated with a
         registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.list_registration_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#list_registration_associations)
@@ -814,15 +922,15 @@
 
     def put_keyword(
         self,
         *,
         OriginationIdentity: str,
         Keyword: str,
         KeywordMessage: str,
-        KeywordAction: KeywordActionType = ...
+        KeywordAction: KeywordActionType = ...,
     ) -> PutKeywordResultTypeDef:
         """
         Creates or updates a keyword configuration on an origination phone number or
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.put_keyword)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#put_keyword)
@@ -841,15 +949,15 @@
     def put_registration_field_value(
         self,
         *,
         RegistrationId: str,
         FieldPath: str,
         SelectChoices: Sequence[str] = ...,
         TextValue: str = ...,
-        RegistrationAttachmentId: str = ...
+        RegistrationAttachmentId: str = ...,
     ) -> PutRegistrationFieldValueResultTypeDef:
         """
         Creates or updates a field value for a registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.put_registration_field_value)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#put_registration_field_value)
         """
@@ -880,15 +988,15 @@
         NumberCapabilities: Sequence[NumberCapabilityType],
         NumberType: RequestableNumberTypeType,
         OptOutListName: str = ...,
         PoolId: str = ...,
         RegistrationId: str = ...,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RequestPhoneNumberResultTypeDef:
         """
         Request an origination phone number for use in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.request_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#request_phone_number)
         """
@@ -897,15 +1005,15 @@
         self,
         *,
         SenderId: str,
         IsoCountryCode: str,
         MessageTypes: Sequence[MessageTypeType] = ...,
         DeletionProtectionEnabled: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> RequestSenderIdResultTypeDef:
         """
         Request a new sender ID that doesn't require registration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.request_sender_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#request_sender_id)
         """
@@ -915,39 +1023,62 @@
         *,
         VerifiedDestinationNumberId: str,
         VerificationChannel: VerificationChannelType,
         LanguageCode: LanguageCodeType = ...,
         OriginationIdentity: str = ...,
         ConfigurationSetName: str = ...,
         Context: Mapping[str, str] = ...,
-        DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...
+        DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...,
     ) -> SendDestinationNumberVerificationCodeResultTypeDef:
         """
         Before you can send test messages to a verified destination phone number you
         need to opt-in the verified destination phone
         number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_destination_number_verification_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#send_destination_number_verification_code)
         """
 
+    def send_media_message(
+        self,
+        *,
+        DestinationPhoneNumber: str,
+        OriginationIdentity: str,
+        MessageBody: str = ...,
+        MediaUrls: Sequence[str] = ...,
+        ConfigurationSetName: str = ...,
+        MaxPrice: str = ...,
+        TimeToLive: int = ...,
+        Context: Mapping[str, str] = ...,
+        DryRun: bool = ...,
+        ProtectConfigurationId: str = ...,
+    ) -> SendMediaMessageResultTypeDef:
+        """
+        Creates a new multimedia message (MMS) and sends it to a recipient's phone
+        number.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_media_message)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#send_media_message)
+        """
+
     def send_text_message(
         self,
         *,
         DestinationPhoneNumber: str,
         OriginationIdentity: str = ...,
         MessageBody: str = ...,
         MessageType: MessageTypeType = ...,
         Keyword: str = ...,
         ConfigurationSetName: str = ...,
         MaxPrice: str = ...,
         TimeToLive: int = ...,
         Context: Mapping[str, str] = ...,
         DestinationCountryParameters: Mapping[DestinationCountryParameterKeyType, str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
+        ProtectConfigurationId: str = ...,
     ) -> SendTextMessageResultTypeDef:
         """
         Creates a new text message and sends it to a recipient's phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_text_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#send_text_message)
         """
@@ -960,23 +1091,34 @@
         MessageBody: str = ...,
         MessageBodyTextType: VoiceMessageBodyTextTypeType = ...,
         VoiceId: VoiceIdType = ...,
         ConfigurationSetName: str = ...,
         MaxPricePerMinute: str = ...,
         TimeToLive: int = ...,
         Context: Mapping[str, str] = ...,
-        DryRun: bool = ...
+        DryRun: bool = ...,
+        ProtectConfigurationId: str = ...,
     ) -> SendVoiceMessageResultTypeDef:
         """
         Allows you to send a request that sends a voice message through Amazon Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.send_voice_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#send_voice_message)
         """
 
+    def set_account_default_protect_configuration(
+        self, *, ProtectConfigurationId: str
+    ) -> SetAccountDefaultProtectConfigurationResultTypeDef:
+        """
+        Set a protect configuration as your account default.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_account_default_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#set_account_default_protect_configuration)
+        """
+
     def set_default_message_type(
         self, *, ConfigurationSetName: str, MessageType: MessageTypeType
     ) -> SetDefaultMessageTypeResultTypeDef:
         """
         Sets the default message type on a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_default_message_type)
@@ -989,14 +1131,24 @@
         """
         Sets default sender ID on a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_default_sender_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#set_default_sender_id)
         """
 
+    def set_media_message_spend_limit_override(
+        self, *, MonthlyLimit: int
+    ) -> SetMediaMessageSpendLimitOverrideResultTypeDef:
+        """
+        Sets an account level monthly spend limit override for sending MMS messages.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_media_message_spend_limit_override)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#set_media_message_spend_limit_override)
+        """
+
     def set_text_message_spend_limit_override(
         self, *, MonthlyLimit: int
     ) -> SetTextMessageSpendLimitOverrideResultTypeDef:
         """
         Sets an account level monthly spend limit override for sending text messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.set_text_message_spend_limit_override)
@@ -1048,15 +1200,15 @@
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         Enabled: bool = ...,
         MatchingEventTypes: Sequence[EventTypeType] = ...,
         CloudWatchLogsDestination: CloudWatchLogsDestinationTypeDef = ...,
         KinesisFirehoseDestination: KinesisFirehoseDestinationTypeDef = ...,
-        SnsDestination: SnsDestinationTypeDef = ...
+        SnsDestination: SnsDestinationTypeDef = ...,
     ) -> UpdateEventDestinationResultTypeDef:
         """
         Updates an existing event destination in a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_event_destination)
         """
@@ -1066,15 +1218,15 @@
         *,
         PhoneNumberId: str,
         TwoWayEnabled: bool = ...,
         TwoWayChannelArn: str = ...,
         TwoWayChannelRole: str = ...,
         SelfManagedOptOutsEnabled: bool = ...,
         OptOutListName: str = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdatePhoneNumberResultTypeDef:
         """
         Updates the configuration of an existing origination phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_phone_number)
         """
@@ -1085,23 +1237,49 @@
         PoolId: str,
         TwoWayEnabled: bool = ...,
         TwoWayChannelArn: str = ...,
         TwoWayChannelRole: str = ...,
         SelfManagedOptOutsEnabled: bool = ...,
         OptOutListName: str = ...,
         SharedRoutesEnabled: bool = ...,
-        DeletionProtectionEnabled: bool = ...
+        DeletionProtectionEnabled: bool = ...,
     ) -> UpdatePoolResultTypeDef:
         """
         Updates the configuration of an existing pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_pool)
         """
 
+    def update_protect_configuration(
+        self, *, ProtectConfigurationId: str, DeletionProtectionEnabled: bool = ...
+    ) -> UpdateProtectConfigurationResultTypeDef:
+        """
+        Update the setting for an existing protect configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_protect_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_protect_configuration)
+        """
+
+    def update_protect_configuration_country_rule_set(
+        self,
+        *,
+        ProtectConfigurationId: str,
+        NumberCapability: NumberCapabilityType,
+        CountryRuleSetUpdates: Mapping[str, ProtectConfigurationCountryRuleSetInformationTypeDef],
+    ) -> UpdateProtectConfigurationCountryRuleSetResultTypeDef:
+        """
+        Update a country rule set to `ALLOW` or `BLOCK` messages to be sent to the
+        specified destination
+        counties.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_protect_configuration_country_rule_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#update_protect_configuration_country_rule_set)
+        """
+
     def update_sender_id(
         self, *, SenderId: str, IsoCountryCode: str, DeletionProtectionEnabled: bool = ...
     ) -> UpdateSenderIdResultTypeDef:
         """
         Updates the configuration of an existing sender ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.update_sender_id)
@@ -1188,14 +1366,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_protect_configurations"]
+    ) -> DescribeProtectConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_registration_attachments"]
     ) -> DescribeRegistrationAttachmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/literals.py` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountAttributeNameType",
     "AccountLimitNameType",
     "AttachmentStatusType",
     "AttachmentUploadErrorReasonType",
     "ConfigurationSetFilterNameType",
     "DescribeAccountAttributesPaginatorName",
     "DescribeAccountLimitsPaginatorName",
     "DescribeConfigurationSetsPaginatorName",
     "DescribeKeywordsPaginatorName",
     "DescribeOptOutListsPaginatorName",
     "DescribeOptedOutNumbersPaginatorName",
     "DescribePhoneNumbersPaginatorName",
     "DescribePoolsPaginatorName",
+    "DescribeProtectConfigurationsPaginatorName",
     "DescribeRegistrationAttachmentsPaginatorName",
     "DescribeRegistrationFieldDefinitionsPaginatorName",
     "DescribeRegistrationFieldValuesPaginatorName",
     "DescribeRegistrationSectionDefinitionsPaginatorName",
     "DescribeRegistrationTypeDefinitionsPaginatorName",
     "DescribeRegistrationVersionsPaginatorName",
     "DescribeRegistrationsPaginatorName",
@@ -58,14 +58,16 @@
     "NumberStatusType",
     "NumberTypeType",
     "OptedOutFilterNameType",
     "PhoneNumberFilterNameType",
     "PoolFilterNameType",
     "PoolOriginationIdentitiesFilterNameType",
     "PoolStatusType",
+    "ProtectConfigurationFilterNameType",
+    "ProtectStatusType",
     "RegistrationAssociationBehaviorType",
     "RegistrationAssociationFilterNameType",
     "RegistrationAttachmentFilterNameType",
     "RegistrationDisassociationBehaviorType",
     "RegistrationFilterNameType",
     "RegistrationStatusType",
     "RegistrationTypeFilterNameType",
@@ -82,39 +84,43 @@
     "PinpointSMSVoiceV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
-AccountAttributeNameType = Literal["ACCOUNT_TIER"]
+AccountAttributeNameType = Literal["ACCOUNT_TIER", "DEFAULT_PROTECT_CONFIGURATION_ID"]
 AccountLimitNameType = Literal[
     "CONFIGURATION_SETS",
     "OPT_OUT_LISTS",
     "PHONE_NUMBERS",
     "POOLS",
     "REGISTRATIONS",
     "REGISTRATION_ATTACHMENTS",
     "SENDER_IDS",
     "VERIFIED_DESTINATION_NUMBERS",
 ]
 AttachmentStatusType = Literal["DELETED", "UPLOAD_COMPLETE", "UPLOAD_FAILED", "UPLOAD_IN_PROGRESS"]
 AttachmentUploadErrorReasonType = Literal["INTERNAL_ERROR"]
 ConfigurationSetFilterNameType = Literal[
-    "default-message-type", "default-sender-id", "event-destination-name", "matching-event-types"
+    "default-message-type",
+    "default-sender-id",
+    "event-destination-name",
+    "matching-event-types",
+    "protect-configuration-id",
 ]
 DescribeAccountAttributesPaginatorName = Literal["describe_account_attributes"]
 DescribeAccountLimitsPaginatorName = Literal["describe_account_limits"]
 DescribeConfigurationSetsPaginatorName = Literal["describe_configuration_sets"]
 DescribeKeywordsPaginatorName = Literal["describe_keywords"]
 DescribeOptOutListsPaginatorName = Literal["describe_opt_out_lists"]
 DescribeOptedOutNumbersPaginatorName = Literal["describe_opted_out_numbers"]
 DescribePhoneNumbersPaginatorName = Literal["describe_phone_numbers"]
 DescribePoolsPaginatorName = Literal["describe_pools"]
+DescribeProtectConfigurationsPaginatorName = Literal["describe_protect_configurations"]
 DescribeRegistrationAttachmentsPaginatorName = Literal["describe_registration_attachments"]
 DescribeRegistrationFieldDefinitionsPaginatorName = Literal[
     "describe_registration_field_definitions"
 ]
 DescribeRegistrationFieldValuesPaginatorName = Literal["describe_registration_field_values"]
 DescribeRegistrationSectionDefinitionsPaginatorName = Literal[
     "describe_registration_section_definitions"
@@ -124,14 +130,31 @@
 DescribeRegistrationsPaginatorName = Literal["describe_registrations"]
 DescribeSenderIdsPaginatorName = Literal["describe_sender_ids"]
 DescribeSpendLimitsPaginatorName = Literal["describe_spend_limits"]
 DescribeVerifiedDestinationNumbersPaginatorName = Literal["describe_verified_destination_numbers"]
 DestinationCountryParameterKeyType = Literal["IN_ENTITY_ID", "IN_TEMPLATE_ID"]
 EventTypeType = Literal[
     "ALL",
+    "MEDIA_ALL",
+    "MEDIA_BLOCKED",
+    "MEDIA_CARRIER_BLOCKED",
+    "MEDIA_CARRIER_UNREACHABLE",
+    "MEDIA_DELIVERED",
+    "MEDIA_FILE_INACCESSIBLE",
+    "MEDIA_FILE_SIZE_EXCEEDED",
+    "MEDIA_FILE_TYPE_UNSUPPORTED",
+    "MEDIA_INVALID",
+    "MEDIA_INVALID_MESSAGE",
+    "MEDIA_PENDING",
+    "MEDIA_QUEUED",
+    "MEDIA_SPAM",
+    "MEDIA_SUCCESSFUL",
+    "MEDIA_TTL_EXPIRED",
+    "MEDIA_UNKNOWN",
+    "MEDIA_UNREACHABLE",
     "TEXT_ALL",
     "TEXT_BLOCKED",
     "TEXT_CARRIER_BLOCKED",
     "TEXT_CARRIER_UNREACHABLE",
     "TEXT_DELIVERED",
     "TEXT_INVALID",
     "TEXT_INVALID_MESSAGE",
@@ -171,15 +194,15 @@
     "PT_BR",
     "ZH_CN",
     "ZH_TW",
 ]
 ListPoolOriginationIdentitiesPaginatorName = Literal["list_pool_origination_identities"]
 ListRegistrationAssociationsPaginatorName = Literal["list_registration_associations"]
 MessageTypeType = Literal["PROMOTIONAL", "TRANSACTIONAL"]
-NumberCapabilityType = Literal["SMS", "VOICE"]
+NumberCapabilityType = Literal["MMS", "SMS", "VOICE"]
 NumberStatusType = Literal["ACTIVE", "ASSOCIATING", "DELETED", "DISASSOCIATING", "PENDING"]
 NumberTypeType = Literal["LONG_CODE", "SHORT_CODE", "SIMULATOR", "TEN_DLC", "TOLL_FREE"]
 OptedOutFilterNameType = Literal["end-user-opted-out"]
 PhoneNumberFilterNameType = Literal[
     "deletion-protection-enabled",
     "iso-country-code",
     "message-type",
@@ -199,14 +222,16 @@
     "shared-routes-enabled",
     "status",
     "two-way-channel-arn",
     "two-way-enabled",
 ]
 PoolOriginationIdentitiesFilterNameType = Literal["iso-country-code", "number-capability"]
 PoolStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
+ProtectConfigurationFilterNameType = Literal["account-default", "deletion-protection-enabled"]
+ProtectStatusType = Literal["ALLOW", "BLOCK"]
 RegistrationAssociationBehaviorType = Literal[
     "ASSOCIATE_AFTER_COMPLETE", "ASSOCIATE_BEFORE_SUBMIT", "ASSOCIATE_ON_APPROVAL"
 ]
 RegistrationAssociationFilterNameType = Literal["iso-country-code", "resource-type"]
 RegistrationAttachmentFilterNameType = Literal["attachment-status"]
 RegistrationDisassociationBehaviorType = Literal[
     "DELETE_REGISTRATION_DISASSOCIATES",
@@ -232,15 +257,17 @@
     "APPROVED", "ARCHIVED", "DENIED", "DISCARDED", "DRAFT", "REVIEWING", "REVOKED", "SUBMITTED"
 ]
 RequestableNumberTypeType = Literal["LONG_CODE", "SIMULATOR", "TEN_DLC", "TOLL_FREE"]
 SenderIdFilterNameType = Literal[
     "deletion-protection-enabled", "iso-country-code", "message-type", "registered", "sender-id"
 ]
 SpendLimitNameType = Literal[
-    "TEXT_MESSAGE_MONTHLY_SPEND_LIMIT", "VOICE_MESSAGE_MONTHLY_SPEND_LIMIT"
+    "MEDIA_MESSAGE_MONTHLY_SPEND_LIMIT",
+    "TEXT_MESSAGE_MONTHLY_SPEND_LIMIT",
+    "VOICE_MESSAGE_MONTHLY_SPEND_LIMIT",
 ]
 VerificationChannelType = Literal["TEXT", "VOICE"]
 VerificationStatusType = Literal["PENDING", "VERIFIED"]
 VerifiedDestinationNumberFilterNameType = Literal["status"]
 VoiceIdType = Literal[
     "AMY",
     "ASTRID",
@@ -326,14 +353,15 @@
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
@@ -344,14 +372,15 @@
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
@@ -369,14 +398,15 @@
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
@@ -389,24 +419,26 @@
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
@@ -467,15 +499,14 @@
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
@@ -547,17 +578,19 @@
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
@@ -602,14 +635,15 @@
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
@@ -647,19 +681,21 @@
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
@@ -697,32 +733,50 @@
     "describe_account_limits",
     "describe_configuration_sets",
     "describe_keywords",
     "describe_opt_out_lists",
     "describe_opted_out_numbers",
     "describe_phone_numbers",
     "describe_pools",
+    "describe_protect_configurations",
     "describe_registration_attachments",
     "describe_registration_field_definitions",
     "describe_registration_field_values",
     "describe_registration_section_definitions",
     "describe_registration_type_definitions",
     "describe_registration_versions",
     "describe_registrations",
     "describe_sender_ids",
     "describe_spend_limits",
     "describe_verified_destination_numbers",
     "list_pool_origination_identities",
     "list_registration_associations",
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
+    "eu-west-3",
+    "il-central-1",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
     "us-east-1",
+    "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "DescribeAccountLimitsPaginatorName",
     "DescribeConfigurationSetsPaginatorName",
     "DescribeKeywordsPaginatorName",
     "DescribeOptOutListsPaginatorName",
     "DescribeOptedOutNumbersPaginatorName",
     "DescribePhoneNumbersPaginatorName",
     "DescribePoolsPaginatorName",
+    "DescribeProtectConfigurationsPaginatorName",
     "DescribeRegistrationAttachmentsPaginatorName",
     "DescribeRegistrationFieldDefinitionsPaginatorName",
     "DescribeRegistrationFieldValuesPaginatorName",
     "DescribeRegistrationSectionDefinitionsPaginatorName",
     "DescribeRegistrationTypeDefinitionsPaginatorName",
     "DescribeRegistrationVersionsPaginatorName",
     "DescribeRegistrationsPaginatorName",
@@ -57,14 +58,16 @@
     "NumberStatusType",
     "NumberTypeType",
     "OptedOutFilterNameType",
     "PhoneNumberFilterNameType",
     "PoolFilterNameType",
     "PoolOriginationIdentitiesFilterNameType",
     "PoolStatusType",
+    "ProtectConfigurationFilterNameType",
+    "ProtectStatusType",
     "RegistrationAssociationBehaviorType",
     "RegistrationAssociationFilterNameType",
     "RegistrationAttachmentFilterNameType",
     "RegistrationDisassociationBehaviorType",
     "RegistrationFilterNameType",
     "RegistrationStatusType",
     "RegistrationTypeFilterNameType",
@@ -81,38 +84,43 @@
     "PinpointSMSVoiceV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-AccountAttributeNameType = Literal["ACCOUNT_TIER"]
+AccountAttributeNameType = Literal["ACCOUNT_TIER", "DEFAULT_PROTECT_CONFIGURATION_ID"]
 AccountLimitNameType = Literal[
     "CONFIGURATION_SETS",
     "OPT_OUT_LISTS",
     "PHONE_NUMBERS",
     "POOLS",
     "REGISTRATIONS",
     "REGISTRATION_ATTACHMENTS",
     "SENDER_IDS",
     "VERIFIED_DESTINATION_NUMBERS",
 ]
 AttachmentStatusType = Literal["DELETED", "UPLOAD_COMPLETE", "UPLOAD_FAILED", "UPLOAD_IN_PROGRESS"]
 AttachmentUploadErrorReasonType = Literal["INTERNAL_ERROR"]
 ConfigurationSetFilterNameType = Literal[
-    "default-message-type", "default-sender-id", "event-destination-name", "matching-event-types"
+    "default-message-type",
+    "default-sender-id",
+    "event-destination-name",
+    "matching-event-types",
+    "protect-configuration-id",
 ]
 DescribeAccountAttributesPaginatorName = Literal["describe_account_attributes"]
 DescribeAccountLimitsPaginatorName = Literal["describe_account_limits"]
 DescribeConfigurationSetsPaginatorName = Literal["describe_configuration_sets"]
 DescribeKeywordsPaginatorName = Literal["describe_keywords"]
 DescribeOptOutListsPaginatorName = Literal["describe_opt_out_lists"]
 DescribeOptedOutNumbersPaginatorName = Literal["describe_opted_out_numbers"]
 DescribePhoneNumbersPaginatorName = Literal["describe_phone_numbers"]
 DescribePoolsPaginatorName = Literal["describe_pools"]
+DescribeProtectConfigurationsPaginatorName = Literal["describe_protect_configurations"]
 DescribeRegistrationAttachmentsPaginatorName = Literal["describe_registration_attachments"]
 DescribeRegistrationFieldDefinitionsPaginatorName = Literal[
     "describe_registration_field_definitions"
 ]
 DescribeRegistrationFieldValuesPaginatorName = Literal["describe_registration_field_values"]
 DescribeRegistrationSectionDefinitionsPaginatorName = Literal[
     "describe_registration_section_definitions"
@@ -122,14 +130,31 @@
 DescribeRegistrationsPaginatorName = Literal["describe_registrations"]
 DescribeSenderIdsPaginatorName = Literal["describe_sender_ids"]
 DescribeSpendLimitsPaginatorName = Literal["describe_spend_limits"]
 DescribeVerifiedDestinationNumbersPaginatorName = Literal["describe_verified_destination_numbers"]
 DestinationCountryParameterKeyType = Literal["IN_ENTITY_ID", "IN_TEMPLATE_ID"]
 EventTypeType = Literal[
     "ALL",
+    "MEDIA_ALL",
+    "MEDIA_BLOCKED",
+    "MEDIA_CARRIER_BLOCKED",
+    "MEDIA_CARRIER_UNREACHABLE",
+    "MEDIA_DELIVERED",
+    "MEDIA_FILE_INACCESSIBLE",
+    "MEDIA_FILE_SIZE_EXCEEDED",
+    "MEDIA_FILE_TYPE_UNSUPPORTED",
+    "MEDIA_INVALID",
+    "MEDIA_INVALID_MESSAGE",
+    "MEDIA_PENDING",
+    "MEDIA_QUEUED",
+    "MEDIA_SPAM",
+    "MEDIA_SUCCESSFUL",
+    "MEDIA_TTL_EXPIRED",
+    "MEDIA_UNKNOWN",
+    "MEDIA_UNREACHABLE",
     "TEXT_ALL",
     "TEXT_BLOCKED",
     "TEXT_CARRIER_BLOCKED",
     "TEXT_CARRIER_UNREACHABLE",
     "TEXT_DELIVERED",
     "TEXT_INVALID",
     "TEXT_INVALID_MESSAGE",
@@ -169,15 +194,15 @@
     "PT_BR",
     "ZH_CN",
     "ZH_TW",
 ]
 ListPoolOriginationIdentitiesPaginatorName = Literal["list_pool_origination_identities"]
 ListRegistrationAssociationsPaginatorName = Literal["list_registration_associations"]
 MessageTypeType = Literal["PROMOTIONAL", "TRANSACTIONAL"]
-NumberCapabilityType = Literal["SMS", "VOICE"]
+NumberCapabilityType = Literal["MMS", "SMS", "VOICE"]
 NumberStatusType = Literal["ACTIVE", "ASSOCIATING", "DELETED", "DISASSOCIATING", "PENDING"]
 NumberTypeType = Literal["LONG_CODE", "SHORT_CODE", "SIMULATOR", "TEN_DLC", "TOLL_FREE"]
 OptedOutFilterNameType = Literal["end-user-opted-out"]
 PhoneNumberFilterNameType = Literal[
     "deletion-protection-enabled",
     "iso-country-code",
     "message-type",
@@ -197,14 +222,16 @@
     "shared-routes-enabled",
     "status",
     "two-way-channel-arn",
     "two-way-enabled",
 ]
 PoolOriginationIdentitiesFilterNameType = Literal["iso-country-code", "number-capability"]
 PoolStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
+ProtectConfigurationFilterNameType = Literal["account-default", "deletion-protection-enabled"]
+ProtectStatusType = Literal["ALLOW", "BLOCK"]
 RegistrationAssociationBehaviorType = Literal[
     "ASSOCIATE_AFTER_COMPLETE", "ASSOCIATE_BEFORE_SUBMIT", "ASSOCIATE_ON_APPROVAL"
 ]
 RegistrationAssociationFilterNameType = Literal["iso-country-code", "resource-type"]
 RegistrationAttachmentFilterNameType = Literal["attachment-status"]
 RegistrationDisassociationBehaviorType = Literal[
     "DELETE_REGISTRATION_DISASSOCIATES",
@@ -230,15 +257,17 @@
     "APPROVED", "ARCHIVED", "DENIED", "DISCARDED", "DRAFT", "REVIEWING", "REVOKED", "SUBMITTED"
 ]
 RequestableNumberTypeType = Literal["LONG_CODE", "SIMULATOR", "TEN_DLC", "TOLL_FREE"]
 SenderIdFilterNameType = Literal[
     "deletion-protection-enabled", "iso-country-code", "message-type", "registered", "sender-id"
 ]
 SpendLimitNameType = Literal[
-    "TEXT_MESSAGE_MONTHLY_SPEND_LIMIT", "VOICE_MESSAGE_MONTHLY_SPEND_LIMIT"
+    "MEDIA_MESSAGE_MONTHLY_SPEND_LIMIT",
+    "TEXT_MESSAGE_MONTHLY_SPEND_LIMIT",
+    "VOICE_MESSAGE_MONTHLY_SPEND_LIMIT",
 ]
 VerificationChannelType = Literal["TEXT", "VOICE"]
 VerificationStatusType = Literal["PENDING", "VERIFIED"]
 VerifiedDestinationNumberFilterNameType = Literal["status"]
 VoiceIdType = Literal[
     "AMY",
     "ASTRID",
@@ -324,14 +353,15 @@
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
@@ -342,14 +372,15 @@
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
@@ -367,14 +398,15 @@
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
@@ -387,24 +419,26 @@
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
@@ -465,15 +499,14 @@
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
@@ -545,17 +578,19 @@
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
@@ -600,14 +635,15 @@
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
@@ -645,19 +681,21 @@
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
@@ -695,32 +733,50 @@
     "describe_account_limits",
     "describe_configuration_sets",
     "describe_keywords",
     "describe_opt_out_lists",
     "describe_opted_out_numbers",
     "describe_phone_numbers",
     "describe_pools",
+    "describe_protect_configurations",
     "describe_registration_attachments",
     "describe_registration_field_definitions",
     "describe_registration_field_values",
     "describe_registration_section_definitions",
     "describe_registration_type_definitions",
     "describe_registration_versions",
     "describe_registrations",
     "describe_sender_ids",
     "describe_spend_limits",
     "describe_verified_destination_numbers",
     "list_pool_origination_identities",
     "list_registration_associations",
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
+    "eu-west-3",
+    "il-central-1",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
     "us-east-1",
+    "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.py` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeAccountLimitsPaginator,
         DescribeConfigurationSetsPaginator,
         DescribeKeywordsPaginator,
         DescribeOptOutListsPaginator,
         DescribeOptedOutNumbersPaginator,
         DescribePhoneNumbersPaginator,
         DescribePoolsPaginator,
+        DescribeProtectConfigurationsPaginator,
         DescribeRegistrationAttachmentsPaginator,
         DescribeRegistrationFieldDefinitionsPaginator,
         DescribeRegistrationFieldValuesPaginator,
         DescribeRegistrationSectionDefinitionsPaginator,
         DescribeRegistrationTypeDefinitionsPaginator,
         DescribeRegistrationVersionsPaginator,
         DescribeRegistrationsPaginator,
@@ -39,14 +40,15 @@
     describe_account_limits_paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
     describe_configuration_sets_paginator: DescribeConfigurationSetsPaginator = client.get_paginator("describe_configuration_sets")
     describe_keywords_paginator: DescribeKeywordsPaginator = client.get_paginator("describe_keywords")
     describe_opt_out_lists_paginator: DescribeOptOutListsPaginator = client.get_paginator("describe_opt_out_lists")
     describe_opted_out_numbers_paginator: DescribeOptedOutNumbersPaginator = client.get_paginator("describe_opted_out_numbers")
     describe_phone_numbers_paginator: DescribePhoneNumbersPaginator = client.get_paginator("describe_phone_numbers")
     describe_pools_paginator: DescribePoolsPaginator = client.get_paginator("describe_pools")
+    describe_protect_configurations_paginator: DescribeProtectConfigurationsPaginator = client.get_paginator("describe_protect_configurations")
     describe_registration_attachments_paginator: DescribeRegistrationAttachmentsPaginator = client.get_paginator("describe_registration_attachments")
     describe_registration_field_definitions_paginator: DescribeRegistrationFieldDefinitionsPaginator = client.get_paginator("describe_registration_field_definitions")
     describe_registration_field_values_paginator: DescribeRegistrationFieldValuesPaginator = client.get_paginator("describe_registration_field_values")
     describe_registration_section_definitions_paginator: DescribeRegistrationSectionDefinitionsPaginator = client.get_paginator("describe_registration_section_definitions")
     describe_registration_type_definitions_paginator: DescribeRegistrationTypeDefinitionsPaginator = client.get_paginator("describe_registration_type_definitions")
     describe_registration_versions_paginator: DescribeRegistrationVersionsPaginator = client.get_paginator("describe_registration_versions")
     describe_registrations_paginator: DescribeRegistrationsPaginator = client.get_paginator("describe_registrations")
@@ -68,14 +70,15 @@
     DescribeAccountLimitsResultTypeDef,
     DescribeConfigurationSetsResultTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribePhoneNumbersResultTypeDef,
     DescribePoolsResultTypeDef,
+    DescribeProtectConfigurationsResultTypeDef,
     DescribeRegistrationAttachmentsResultTypeDef,
     DescribeRegistrationFieldDefinitionsResultTypeDef,
     DescribeRegistrationFieldValuesResultTypeDef,
     DescribeRegistrationSectionDefinitionsResultTypeDef,
     DescribeRegistrationsResultTypeDef,
     DescribeRegistrationTypeDefinitionsResultTypeDef,
     DescribeRegistrationVersionsResultTypeDef,
@@ -86,14 +89,15 @@
     ListPoolOriginationIdentitiesResultTypeDef,
     ListRegistrationAssociationsResultTypeDef,
     OptedOutFilterTypeDef,
     PaginatorConfigTypeDef,
     PhoneNumberFilterTypeDef,
     PoolFilterTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
+    ProtectConfigurationFilterTypeDef,
     RegistrationAssociationFilterTypeDef,
     RegistrationAttachmentFilterTypeDef,
     RegistrationFilterTypeDef,
     RegistrationTypeFilterTypeDef,
     RegistrationVersionFilterTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
@@ -105,29 +109,29 @@
     "DescribeAccountLimitsPaginator",
     "DescribeConfigurationSetsPaginator",
     "DescribeKeywordsPaginator",
     "DescribeOptOutListsPaginator",
     "DescribeOptedOutNumbersPaginator",
     "DescribePhoneNumbersPaginator",
     "DescribePoolsPaginator",
+    "DescribeProtectConfigurationsPaginator",
     "DescribeRegistrationAttachmentsPaginator",
     "DescribeRegistrationFieldDefinitionsPaginator",
     "DescribeRegistrationFieldValuesPaginator",
     "DescribeRegistrationSectionDefinitionsPaginator",
     "DescribeRegistrationTypeDefinitionsPaginator",
     "DescribeRegistrationVersionsPaginator",
     "DescribeRegistrationsPaginator",
     "DescribeSenderIdsPaginator",
     "DescribeSpendLimitsPaginator",
     "DescribeVerifiedDestinationNumbersPaginator",
     "ListPoolOriginationIdentitiesPaginator",
     "ListRegistrationAssociationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -171,15 +175,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeConfigurationSetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
         """
 
 
@@ -191,15 +195,15 @@
 
     def paginate(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeKeywordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
         """
 
 
@@ -209,15 +213,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeOptOutListsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
         """
 
 
@@ -229,15 +233,15 @@
 
     def paginate(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeOptedOutNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
         """
 
 
@@ -248,15 +252,15 @@
     """
 
     def paginate(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribePhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
         """
 
 
@@ -267,34 +271,53 @@
     """
 
     def paginate(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
         """
 
 
+class DescribeProtectConfigurationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeProtectConfigurations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeprotectconfigurationspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        ProtectConfigurationIds: Sequence[str] = ...,
+        Filters: Sequence[ProtectConfigurationFilterTypeDef] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[DescribeProtectConfigurationsResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeProtectConfigurations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeprotectconfigurationspaginator)
+        """
+
+
 class DescribeRegistrationAttachmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationattachmentspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationAttachmentIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationattachmentspaginator)
         """
 
 
@@ -306,15 +329,15 @@
 
     def paginate(
         self,
         *,
         RegistrationType: str,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationFieldDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationfielddefinitionspaginator)
         """
 
 
@@ -327,15 +350,15 @@
     def paginate(
         self,
         *,
         RegistrationId: str,
         VersionNumber: int = ...,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationFieldValuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationfieldvaluespaginator)
         """
 
 
@@ -346,15 +369,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistrationType: str,
         SectionPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationSectionDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationSectionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationsectiondefinitionspaginator)
         """
 
 
@@ -365,15 +388,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistrationTypes: Sequence[str] = ...,
         Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationTypeDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationTypeDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationtypedefinitionspaginator)
         """
 
 
@@ -385,15 +408,15 @@
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         VersionNumbers: Sequence[int] = ...,
         Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationversionspaginator)
         """
 
 
@@ -404,15 +427,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistrationIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationspaginator)
         """
 
 
@@ -423,15 +446,15 @@
     """
 
     def paginate(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeSenderIdsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
         """
 
 
@@ -458,15 +481,15 @@
 
     def paginate(
         self,
         *,
         VerifiedDestinationNumberIds: Sequence[str] = ...,
         DestinationPhoneNumbers: Sequence[str] = ...,
         Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeVerifiedDestinationNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeVerifiedDestinationNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeverifieddestinationnumberspaginator)
         """
 
 
@@ -477,15 +500,15 @@
     """
 
     def paginate(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPoolOriginationIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
         """
 
 
@@ -496,13 +519,13 @@
     """
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRegistrationAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListRegistrationAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#listregistrationassociationspaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeAccountLimitsPaginator,
         DescribeConfigurationSetsPaginator,
         DescribeKeywordsPaginator,
         DescribeOptOutListsPaginator,
         DescribeOptedOutNumbersPaginator,
         DescribePhoneNumbersPaginator,
         DescribePoolsPaginator,
+        DescribeProtectConfigurationsPaginator,
         DescribeRegistrationAttachmentsPaginator,
         DescribeRegistrationFieldDefinitionsPaginator,
         DescribeRegistrationFieldValuesPaginator,
         DescribeRegistrationSectionDefinitionsPaginator,
         DescribeRegistrationTypeDefinitionsPaginator,
         DescribeRegistrationVersionsPaginator,
         DescribeRegistrationsPaginator,
@@ -39,14 +40,15 @@
     describe_account_limits_paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")
     describe_configuration_sets_paginator: DescribeConfigurationSetsPaginator = client.get_paginator("describe_configuration_sets")
     describe_keywords_paginator: DescribeKeywordsPaginator = client.get_paginator("describe_keywords")
     describe_opt_out_lists_paginator: DescribeOptOutListsPaginator = client.get_paginator("describe_opt_out_lists")
     describe_opted_out_numbers_paginator: DescribeOptedOutNumbersPaginator = client.get_paginator("describe_opted_out_numbers")
     describe_phone_numbers_paginator: DescribePhoneNumbersPaginator = client.get_paginator("describe_phone_numbers")
     describe_pools_paginator: DescribePoolsPaginator = client.get_paginator("describe_pools")
+    describe_protect_configurations_paginator: DescribeProtectConfigurationsPaginator = client.get_paginator("describe_protect_configurations")
     describe_registration_attachments_paginator: DescribeRegistrationAttachmentsPaginator = client.get_paginator("describe_registration_attachments")
     describe_registration_field_definitions_paginator: DescribeRegistrationFieldDefinitionsPaginator = client.get_paginator("describe_registration_field_definitions")
     describe_registration_field_values_paginator: DescribeRegistrationFieldValuesPaginator = client.get_paginator("describe_registration_field_values")
     describe_registration_section_definitions_paginator: DescribeRegistrationSectionDefinitionsPaginator = client.get_paginator("describe_registration_section_definitions")
     describe_registration_type_definitions_paginator: DescribeRegistrationTypeDefinitionsPaginator = client.get_paginator("describe_registration_type_definitions")
     describe_registration_versions_paginator: DescribeRegistrationVersionsPaginator = client.get_paginator("describe_registration_versions")
     describe_registrations_paginator: DescribeRegistrationsPaginator = client.get_paginator("describe_registrations")
@@ -68,14 +70,15 @@
     DescribeAccountLimitsResultTypeDef,
     DescribeConfigurationSetsResultTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribePhoneNumbersResultTypeDef,
     DescribePoolsResultTypeDef,
+    DescribeProtectConfigurationsResultTypeDef,
     DescribeRegistrationAttachmentsResultTypeDef,
     DescribeRegistrationFieldDefinitionsResultTypeDef,
     DescribeRegistrationFieldValuesResultTypeDef,
     DescribeRegistrationSectionDefinitionsResultTypeDef,
     DescribeRegistrationsResultTypeDef,
     DescribeRegistrationTypeDefinitionsResultTypeDef,
     DescribeRegistrationVersionsResultTypeDef,
@@ -86,14 +89,15 @@
     ListPoolOriginationIdentitiesResultTypeDef,
     ListRegistrationAssociationsResultTypeDef,
     OptedOutFilterTypeDef,
     PaginatorConfigTypeDef,
     PhoneNumberFilterTypeDef,
     PoolFilterTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
+    ProtectConfigurationFilterTypeDef,
     RegistrationAssociationFilterTypeDef,
     RegistrationAttachmentFilterTypeDef,
     RegistrationFilterTypeDef,
     RegistrationTypeFilterTypeDef,
     RegistrationVersionFilterTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
@@ -105,14 +109,15 @@
     "DescribeAccountLimitsPaginator",
     "DescribeConfigurationSetsPaginator",
     "DescribeKeywordsPaginator",
     "DescribeOptOutListsPaginator",
     "DescribeOptedOutNumbersPaginator",
     "DescribePhoneNumbersPaginator",
     "DescribePoolsPaginator",
+    "DescribeProtectConfigurationsPaginator",
     "DescribeRegistrationAttachmentsPaginator",
     "DescribeRegistrationFieldDefinitionsPaginator",
     "DescribeRegistrationFieldValuesPaginator",
     "DescribeRegistrationSectionDefinitionsPaginator",
     "DescribeRegistrationTypeDefinitionsPaginator",
     "DescribeRegistrationVersionsPaginator",
     "DescribeRegistrationsPaginator",
@@ -166,15 +171,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeConfigurationSetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
         """
 
 class DescribeKeywordsPaginator(Paginator):
@@ -185,15 +190,15 @@
 
     def paginate(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeKeywordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
         """
 
 class DescribeOptOutListsPaginator(Paginator):
@@ -202,15 +207,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeOptOutListsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
         """
 
 class DescribeOptedOutNumbersPaginator(Paginator):
@@ -221,15 +226,15 @@
 
     def paginate(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeOptedOutNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
         """
 
 class DescribePhoneNumbersPaginator(Paginator):
@@ -239,15 +244,15 @@
     """
 
     def paginate(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribePhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
         """
 
 class DescribePoolsPaginator(Paginator):
@@ -257,33 +262,51 @@
     """
 
     def paginate(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
         """
 
+class DescribeProtectConfigurationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeProtectConfigurations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeprotectconfigurationspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        ProtectConfigurationIds: Sequence[str] = ...,
+        Filters: Sequence[ProtectConfigurationFilterTypeDef] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[DescribeProtectConfigurationsResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeProtectConfigurations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeprotectconfigurationspaginator)
+        """
+
 class DescribeRegistrationAttachmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationattachmentspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistrationAttachmentIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationattachmentspaginator)
         """
 
 class DescribeRegistrationFieldDefinitionsPaginator(Paginator):
@@ -294,15 +317,15 @@
 
     def paginate(
         self,
         *,
         RegistrationType: str,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationFieldDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationfielddefinitionspaginator)
         """
 
 class DescribeRegistrationFieldValuesPaginator(Paginator):
@@ -314,15 +337,15 @@
     def paginate(
         self,
         *,
         RegistrationId: str,
         VersionNumber: int = ...,
         SectionPath: str = ...,
         FieldPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationFieldValuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationfieldvaluespaginator)
         """
 
 class DescribeRegistrationSectionDefinitionsPaginator(Paginator):
@@ -332,15 +355,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistrationType: str,
         SectionPaths: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationSectionDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationSectionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationsectiondefinitionspaginator)
         """
 
 class DescribeRegistrationTypeDefinitionsPaginator(Paginator):
@@ -350,15 +373,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistrationTypes: Sequence[str] = ...,
         Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationTypeDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationTypeDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationtypedefinitionspaginator)
         """
 
 class DescribeRegistrationVersionsPaginator(Paginator):
@@ -369,15 +392,15 @@
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         VersionNumbers: Sequence[int] = ...,
         Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationversionspaginator)
         """
 
 class DescribeRegistrationsPaginator(Paginator):
@@ -387,15 +410,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistrationIds: Sequence[str] = ...,
         Filters: Sequence[RegistrationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeRegistrationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeregistrationspaginator)
         """
 
 class DescribeSenderIdsPaginator(Paginator):
@@ -405,15 +428,15 @@
     """
 
     def paginate(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeSenderIdsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
         """
 
 class DescribeSpendLimitsPaginator(Paginator):
@@ -438,15 +461,15 @@
 
     def paginate(
         self,
         *,
         VerifiedDestinationNumberIds: Sequence[str] = ...,
         DestinationPhoneNumbers: Sequence[str] = ...,
         Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeVerifiedDestinationNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeVerifiedDestinationNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeverifieddestinationnumberspaginator)
         """
 
 class ListPoolOriginationIdentitiesPaginator(Paginator):
@@ -456,15 +479,15 @@
     """
 
     def paginate(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPoolOriginationIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
         """
 
 class ListRegistrationAssociationsPaginator(Paginator):
@@ -474,13 +497,13 @@
     """
 
     def paginate(
         self,
         *,
         RegistrationId: str,
         Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRegistrationAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListRegistrationAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#listregistrationassociationspaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
+    AccountAttributeNameType,
     AccountLimitNameType,
     AttachmentStatusType,
     ConfigurationSetFilterNameType,
     DestinationCountryParameterKeyType,
     EventTypeType,
     FieldRequirementType,
     FieldTypeType,
@@ -32,14 +33,16 @@
     NumberCapabilityType,
     NumberStatusType,
     NumberTypeType,
     PhoneNumberFilterNameType,
     PoolFilterNameType,
     PoolOriginationIdentitiesFilterNameType,
     PoolStatusType,
+    ProtectConfigurationFilterNameType,
+    ProtectStatusType,
     RegistrationAssociationBehaviorType,
     RegistrationAssociationFilterNameType,
     RegistrationDisassociationBehaviorType,
     RegistrationFilterNameType,
     RegistrationStatusType,
     RegistrationTypeFilterNameType,
     RegistrationVersionStatusType,
@@ -61,20 +64,20 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "AssociateProtectConfigurationRequestRequestTypeDef",
     "BlobTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "ConfigurationSetFilterTypeDef",
     "TagTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "CreateRegistrationAssociationRequestRequestTypeDef",
@@ -84,14 +87,15 @@
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
     "DeleteDefaultSenderIdRequestRequestTypeDef",
     "DeleteEventDestinationRequestRequestTypeDef",
     "DeleteKeywordRequestRequestTypeDef",
     "DeleteOptOutListRequestRequestTypeDef",
     "DeleteOptedOutNumberRequestRequestTypeDef",
     "DeletePoolRequestRequestTypeDef",
+    "DeleteProtectConfigurationRequestRequestTypeDef",
     "DeleteRegistrationAttachmentRequestRequestTypeDef",
     "DeleteRegistrationFieldValueRequestRequestTypeDef",
     "DeleteRegistrationRequestRequestTypeDef",
     "DeleteVerifiedDestinationNumberRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAccountAttributesRequestRequestTypeDef",
     "DescribeAccountLimitsRequestRequestTypeDef",
@@ -101,14 +105,16 @@
     "OptOutListInformationTypeDef",
     "OptedOutFilterTypeDef",
     "OptedOutNumberInformationTypeDef",
     "PhoneNumberFilterTypeDef",
     "PhoneNumberInformationTypeDef",
     "PoolFilterTypeDef",
     "PoolInformationTypeDef",
+    "ProtectConfigurationFilterTypeDef",
+    "ProtectConfigurationInformationTypeDef",
     "RegistrationAttachmentFilterTypeDef",
     "RegistrationAttachmentsInformationTypeDef",
     "DescribeRegistrationFieldDefinitionsRequestRequestTypeDef",
     "DescribeRegistrationFieldValuesRequestRequestTypeDef",
     "RegistrationFieldValueInformationTypeDef",
     "DescribeRegistrationSectionDefinitionsRequestRequestTypeDef",
     "RegistrationTypeFilterTypeDef",
@@ -119,15 +125,18 @@
     "SenderIdFilterTypeDef",
     "SenderIdInformationTypeDef",
     "DescribeSpendLimitsRequestRequestTypeDef",
     "SpendLimitTypeDef",
     "VerifiedDestinationNumberFilterTypeDef",
     "VerifiedDestinationNumberInformationTypeDef",
     "DisassociateOriginationIdentityRequestRequestTypeDef",
+    "DisassociateProtectConfigurationRequestRequestTypeDef",
     "DiscardRegistrationVersionRequestRequestTypeDef",
+    "GetProtectConfigurationCountryRuleSetRequestRequestTypeDef",
+    "ProtectConfigurationCountryRuleSetInformationTypeDef",
     "PoolOriginationIdentitiesFilterTypeDef",
     "OriginationIdentityMetadataTypeDef",
     "RegistrationAssociationFilterTypeDef",
     "RegistrationAssociationMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutKeywordRequestRequestTypeDef",
     "PutOptedOutNumberRequestRequestTypeDef",
@@ -138,66 +147,81 @@
     "SelectOptionDescriptionTypeDef",
     "RegistrationSectionDisplayHintsTypeDef",
     "RegistrationTypeDisplayHintsTypeDef",
     "SupportedAssociationTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "ReleaseSenderIdRequestRequestTypeDef",
     "SendDestinationNumberVerificationCodeRequestRequestTypeDef",
+    "SendMediaMessageRequestRequestTypeDef",
     "SendTextMessageRequestRequestTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
+    "SetAccountDefaultProtectConfigurationRequestRequestTypeDef",
     "SetDefaultMessageTypeRequestRequestTypeDef",
     "SetDefaultSenderIdRequestRequestTypeDef",
+    "SetMediaMessageSpendLimitOverrideRequestRequestTypeDef",
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
     "SubmitRegistrationVersionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePoolRequestRequestTypeDef",
+    "UpdateProtectConfigurationRequestRequestTypeDef",
     "UpdateSenderIdRequestRequestTypeDef",
     "VerifyDestinationNumberRequestRequestTypeDef",
     "AssociateOriginationIdentityResultTypeDef",
+    "AssociateProtectConfigurationResultTypeDef",
     "CreateRegistrationAssociationResultTypeDef",
+    "DeleteAccountDefaultProtectConfigurationResultTypeDef",
     "DeleteDefaultMessageTypeResultTypeDef",
     "DeleteDefaultSenderIdResultTypeDef",
     "DeleteKeywordResultTypeDef",
+    "DeleteMediaMessageSpendLimitOverrideResultTypeDef",
     "DeleteOptOutListResultTypeDef",
     "DeleteOptedOutNumberResultTypeDef",
     "DeletePoolResultTypeDef",
+    "DeleteProtectConfigurationResultTypeDef",
     "DeleteRegistrationAttachmentResultTypeDef",
     "DeleteRegistrationFieldValueResultTypeDef",
     "DeleteRegistrationResultTypeDef",
     "DeleteTextMessageSpendLimitOverrideResultTypeDef",
     "DeleteVerifiedDestinationNumberResultTypeDef",
     "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "DescribeAccountLimitsResultTypeDef",
     "DisassociateOriginationIdentityResultTypeDef",
+    "DisassociateProtectConfigurationResultTypeDef",
     "PutKeywordResultTypeDef",
     "PutOptedOutNumberResultTypeDef",
     "PutRegistrationFieldValueResultTypeDef",
     "ReleasePhoneNumberResultTypeDef",
     "ReleaseSenderIdResultTypeDef",
     "SendDestinationNumberVerificationCodeResultTypeDef",
+    "SendMediaMessageResultTypeDef",
     "SendTextMessageResultTypeDef",
     "SendVoiceMessageResultTypeDef",
+    "SetAccountDefaultProtectConfigurationResultTypeDef",
     "SetDefaultMessageTypeResultTypeDef",
     "SetDefaultSenderIdResultTypeDef",
+    "SetMediaMessageSpendLimitOverrideResultTypeDef",
     "SetTextMessageSpendLimitOverrideResultTypeDef",
     "SetVoiceMessageSpendLimitOverrideResultTypeDef",
     "UpdatePhoneNumberResultTypeDef",
     "UpdatePoolResultTypeDef",
+    "UpdateProtectConfigurationResultTypeDef",
     "UpdateSenderIdResultTypeDef",
     "VerifyDestinationNumberResultTypeDef",
     "DescribeConfigurationSetsRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateConfigurationSetResultTypeDef",
     "CreateOptOutListRequestRequestTypeDef",
     "CreateOptOutListResultTypeDef",
     "CreatePoolRequestRequestTypeDef",
     "CreatePoolResultTypeDef",
+    "CreateProtectConfigurationRequestRequestTypeDef",
+    "CreateProtectConfigurationResultTypeDef",
     "CreateRegistrationAttachmentRequestRequestTypeDef",
     "CreateRegistrationAttachmentResultTypeDef",
     "CreateRegistrationRequestRequestTypeDef",
     "CreateRegistrationResultTypeDef",
     "CreateVerifiedDestinationNumberRequestRequestTypeDef",
     "CreateVerifiedDestinationNumberResultTypeDef",
     "ListTagsForResourceResultTypeDef",
@@ -229,14 +253,17 @@
     "DescribeOptedOutNumbersResultTypeDef",
     "DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef",
     "DescribePhoneNumbersRequestRequestTypeDef",
     "DescribePhoneNumbersResultTypeDef",
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     "DescribePoolsRequestRequestTypeDef",
     "DescribePoolsResultTypeDef",
+    "DescribeProtectConfigurationsRequestDescribeProtectConfigurationsPaginateTypeDef",
+    "DescribeProtectConfigurationsRequestRequestTypeDef",
+    "DescribeProtectConfigurationsResultTypeDef",
     "DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef",
     "DescribeRegistrationAttachmentsRequestRequestTypeDef",
     "DescribeRegistrationAttachmentsResultTypeDef",
     "DescribeRegistrationFieldValuesResultTypeDef",
     "DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef",
     "DescribeRegistrationTypeDefinitionsRequestRequestTypeDef",
     "DescribeRegistrationVersionsRequestDescribeRegistrationVersionsPaginateTypeDef",
@@ -247,14 +274,17 @@
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     "DescribeSenderIdsRequestRequestTypeDef",
     "DescribeSenderIdsResultTypeDef",
     "DescribeSpendLimitsResultTypeDef",
     "DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef",
     "DescribeVerifiedDestinationNumbersRequestRequestTypeDef",
     "DescribeVerifiedDestinationNumbersResultTypeDef",
+    "GetProtectConfigurationCountryRuleSetResultTypeDef",
+    "UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef",
+    "UpdateProtectConfigurationCountryRuleSetResultTypeDef",
     "ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
     "ListPoolOriginationIdentitiesRequestRequestTypeDef",
     "ListPoolOriginationIdentitiesResultTypeDef",
     "ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef",
     "ListRegistrationAssociationsRequestRequestTypeDef",
     "ListRegistrationAssociationsResultTypeDef",
     "RegistrationVersionInformationTypeDef",
@@ -273,15 +303,15 @@
     "DescribeConfigurationSetsResultTypeDef",
     "DescribeRegistrationFieldDefinitionsResultTypeDef",
 )
 
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
-        "Name": Literal["ACCOUNT_TIER"],
+        "Name": AccountAttributeNameType,
         "Value": str,
     },
 )
 AccountLimitTypeDef = TypedDict(
     "AccountLimitTypeDef",
     {
         "Name": AccountLimitNameType,
@@ -298,18 +328,25 @@
         "ClientToken": NotRequired[str],
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
+    },
+)
+AssociateProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "AssociateProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "ConfigurationSetName": str,
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
@@ -416,14 +453,20 @@
 )
 DeletePoolRequestRequestTypeDef = TypedDict(
     "DeletePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
+DeleteProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+    },
+)
 DeleteRegistrationAttachmentRequestRequestTypeDef = TypedDict(
     "DeleteRegistrationAttachmentRequestRequestTypeDef",
     {
         "RegistrationAttachmentId": str,
     },
 )
 DeleteRegistrationFieldValueRequestRequestTypeDef = TypedDict(
@@ -563,14 +606,31 @@
         "SharedRoutesEnabled": bool,
         "DeletionProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "TwoWayChannelArn": NotRequired[str],
         "TwoWayChannelRole": NotRequired[str],
     },
 )
+ProtectConfigurationFilterTypeDef = TypedDict(
+    "ProtectConfigurationFilterTypeDef",
+    {
+        "Name": ProtectConfigurationFilterNameType,
+        "Values": Sequence[str],
+    },
+)
+ProtectConfigurationInformationTypeDef = TypedDict(
+    "ProtectConfigurationInformationTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "AccountDefault": bool,
+        "DeletionProtectionEnabled": bool,
+    },
+)
 RegistrationAttachmentFilterTypeDef = TypedDict(
     "RegistrationAttachmentFilterTypeDef",
     {
         "Name": Literal["attachment-status"],
         "Values": Sequence[str],
     },
 )
@@ -724,20 +784,40 @@
     {
         "PoolId": str,
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "ClientToken": NotRequired[str],
     },
 )
+DisassociateProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "DisassociateProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "ConfigurationSetName": str,
+    },
+)
 DiscardRegistrationVersionRequestRequestTypeDef = TypedDict(
     "DiscardRegistrationVersionRequestRequestTypeDef",
     {
         "RegistrationId": str,
     },
 )
+GetProtectConfigurationCountryRuleSetRequestRequestTypeDef = TypedDict(
+    "GetProtectConfigurationCountryRuleSetRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "NumberCapability": NumberCapabilityType,
+    },
+)
+ProtectConfigurationCountryRuleSetInformationTypeDef = TypedDict(
+    "ProtectConfigurationCountryRuleSetInformationTypeDef",
+    {
+        "ProtectStatus": ProtectStatusType,
+    },
+)
 PoolOriginationIdentitiesFilterTypeDef = TypedDict(
     "PoolOriginationIdentitiesFilterTypeDef",
     {
         "Name": PoolOriginationIdentitiesFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -886,14 +966,29 @@
         "ConfigurationSetName": NotRequired[str],
         "Context": NotRequired[Mapping[str, str]],
         "DestinationCountryParameters": NotRequired[
             Mapping[DestinationCountryParameterKeyType, str]
         ],
     },
 )
+SendMediaMessageRequestRequestTypeDef = TypedDict(
+    "SendMediaMessageRequestRequestTypeDef",
+    {
+        "DestinationPhoneNumber": str,
+        "OriginationIdentity": str,
+        "MessageBody": NotRequired[str],
+        "MediaUrls": NotRequired[Sequence[str]],
+        "ConfigurationSetName": NotRequired[str],
+        "MaxPrice": NotRequired[str],
+        "TimeToLive": NotRequired[int],
+        "Context": NotRequired[Mapping[str, str]],
+        "DryRun": NotRequired[bool],
+        "ProtectConfigurationId": NotRequired[str],
+    },
+)
 SendTextMessageRequestRequestTypeDef = TypedDict(
     "SendTextMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
         "OriginationIdentity": NotRequired[str],
         "MessageBody": NotRequired[str],
         "MessageType": NotRequired[MessageTypeType],
@@ -902,14 +997,15 @@
         "MaxPrice": NotRequired[str],
         "TimeToLive": NotRequired[int],
         "Context": NotRequired[Mapping[str, str]],
         "DestinationCountryParameters": NotRequired[
             Mapping[DestinationCountryParameterKeyType, str]
         ],
         "DryRun": NotRequired[bool],
+        "ProtectConfigurationId": NotRequired[str],
     },
 )
 SendVoiceMessageRequestRequestTypeDef = TypedDict(
     "SendVoiceMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
         "OriginationIdentity": str,
@@ -917,14 +1013,21 @@
         "MessageBodyTextType": NotRequired[VoiceMessageBodyTextTypeType],
         "VoiceId": NotRequired[VoiceIdType],
         "ConfigurationSetName": NotRequired[str],
         "MaxPricePerMinute": NotRequired[str],
         "TimeToLive": NotRequired[int],
         "Context": NotRequired[Mapping[str, str]],
         "DryRun": NotRequired[bool],
+        "ProtectConfigurationId": NotRequired[str],
+    },
+)
+SetAccountDefaultProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "SetAccountDefaultProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
     },
 )
 SetDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "SetDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
@@ -933,14 +1036,20 @@
 SetDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "SetDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "SenderId": str,
     },
 )
+SetMediaMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
+    "SetMediaMessageSpendLimitOverrideRequestRequestTypeDef",
+    {
+        "MonthlyLimit": int,
+    },
+)
 SetTextMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
@@ -983,14 +1092,21 @@
         "TwoWayChannelRole": NotRequired[str],
         "SelfManagedOptOutsEnabled": NotRequired[bool],
         "OptOutListName": NotRequired[str],
         "SharedRoutesEnabled": NotRequired[bool],
         "DeletionProtectionEnabled": NotRequired[bool],
     },
 )
+UpdateProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "DeletionProtectionEnabled": NotRequired[bool],
+    },
+)
 UpdateSenderIdRequestRequestTypeDef = TypedDict(
     "UpdateSenderIdRequestRequestTypeDef",
     {
         "SenderId": str,
         "IsoCountryCode": str,
         "DeletionProtectionEnabled": NotRequired[bool],
     },
@@ -1009,28 +1125,46 @@
         "PoolId": str,
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AssociateProtectConfigurationResultTypeDef = TypedDict(
+    "AssociateProtectConfigurationResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateRegistrationAssociationResultTypeDef = TypedDict(
     "CreateRegistrationAssociationResultTypeDef",
     {
         "RegistrationArn": str,
         "RegistrationId": str,
         "RegistrationType": str,
         "ResourceArn": str,
         "ResourceId": str,
         "ResourceType": str,
         "IsoCountryCode": str,
         "PhoneNumber": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeleteAccountDefaultProtectConfigurationResultTypeDef = TypedDict(
+    "DeleteAccountDefaultProtectConfigurationResultTypeDef",
+    {
+        "DefaultProtectConfigurationArn": str,
+        "DefaultProtectConfigurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteDefaultMessageTypeResultTypeDef = TypedDict(
     "DeleteDefaultMessageTypeResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1052,14 +1186,21 @@
         "OriginationIdentity": str,
         "Keyword": str,
         "KeywordMessage": str,
         "KeywordAction": KeywordActionType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeleteMediaMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteMediaMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteOptOutListResultTypeDef = TypedDict(
     "DeleteOptOutListResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1089,14 +1230,25 @@
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeleteProtectConfigurationResultTypeDef = TypedDict(
+    "DeleteProtectConfigurationResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "AccountDefault": bool,
+        "DeletionProtectionEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteRegistrationAttachmentResultTypeDef = TypedDict(
     "DeleteRegistrationAttachmentResultTypeDef",
     {
         "RegistrationAttachmentArn": str,
         "RegistrationAttachmentId": str,
         "AttachmentStatus": AttachmentStatusType,
         "AttachmentUploadErrorReason": Literal["INTERNAL_ERROR"],
@@ -1156,37 +1308,47 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeAccountLimitsResultTypeDef = TypedDict(
     "DescribeAccountLimitsResultTypeDef",
     {
         "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisassociateOriginationIdentityResultTypeDef = TypedDict(
     "DisassociateOriginationIdentityResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DisassociateProtectConfigurationResultTypeDef = TypedDict(
+    "DisassociateProtectConfigurationResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 PutKeywordResultTypeDef = TypedDict(
     "PutKeywordResultTypeDef",
     {
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "Keyword": str,
         "KeywordMessage": str,
@@ -1256,28 +1418,43 @@
 SendDestinationNumberVerificationCodeResultTypeDef = TypedDict(
     "SendDestinationNumberVerificationCodeResultTypeDef",
     {
         "MessageId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SendMediaMessageResultTypeDef = TypedDict(
+    "SendMediaMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SendTextMessageResultTypeDef = TypedDict(
     "SendTextMessageResultTypeDef",
     {
         "MessageId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SendVoiceMessageResultTypeDef = TypedDict(
     "SendVoiceMessageResultTypeDef",
     {
         "MessageId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SetAccountDefaultProtectConfigurationResultTypeDef = TypedDict(
+    "SetAccountDefaultProtectConfigurationResultTypeDef",
+    {
+        "DefaultProtectConfigurationArn": str,
+        "DefaultProtectConfigurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SetDefaultMessageTypeResultTypeDef = TypedDict(
     "SetDefaultMessageTypeResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1288,14 +1465,21 @@
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "SenderId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SetMediaMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetMediaMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
     "SetTextMessageSpendLimitOverrideResultTypeDef",
     {
         "MonthlyLimit": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1343,14 +1527,25 @@
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
         "DeletionProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateProtectConfigurationResultTypeDef = TypedDict(
+    "UpdateProtectConfigurationResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "AccountDefault": bool,
+        "DeletionProtectionEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 UpdateSenderIdResultTypeDef = TypedDict(
     "UpdateSenderIdResultTypeDef",
     {
         "SenderIdArn": str,
         "SenderId": str,
         "IsoCountryCode": str,
         "MessageTypes": List[MessageTypeType],
@@ -1443,14 +1638,34 @@
         "SharedRoutesEnabled": bool,
         "DeletionProtectionEnabled": bool,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateProtectConfigurationRequestRequestTypeDef",
+    {
+        "ClientToken": NotRequired[str],
+        "DeletionProtectionEnabled": NotRequired[bool],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+CreateProtectConfigurationResultTypeDef = TypedDict(
+    "CreateProtectConfigurationResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "AccountDefault": bool,
+        "DeletionProtectionEnabled": bool,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateRegistrationAttachmentRequestRequestTypeDef = TypedDict(
     "CreateRegistrationAttachmentRequestRequestTypeDef",
     {
         "AttachmentBody": NotRequired[BlobTypeDef],
         "AttachmentUrl": NotRequired[str],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "ClientToken": NotRequired[str],
@@ -1738,24 +1953,24 @@
 )
 DescribeKeywordsResultTypeDef = TypedDict(
     "DescribeKeywordsResultTypeDef",
     {
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "Keywords": List[KeywordInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeOptOutListsResultTypeDef = TypedDict(
     "DescribeOptOutListsResultTypeDef",
     {
         "OptOutLists": List[OptOutListInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumbers": NotRequired[Sequence[str]],
@@ -1775,16 +1990,16 @@
 )
 DescribeOptedOutNumbersResultTypeDef = TypedDict(
     "DescribeOptedOutNumbersResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "OptedOutNumbers": List[OptedOutNumberInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef = TypedDict(
     "DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef",
     {
         "PhoneNumberIds": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[PhoneNumberFilterTypeDef]],
@@ -1800,16 +2015,16 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribePhoneNumbersResultTypeDef = TypedDict(
     "DescribePhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribePoolsRequestDescribePoolsPaginateTypeDef = TypedDict(
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     {
         "PoolIds": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[PoolFilterTypeDef]],
@@ -1825,16 +2040,41 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribePoolsResultTypeDef = TypedDict(
     "DescribePoolsResultTypeDef",
     {
         "Pools": List[PoolInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DescribeProtectConfigurationsRequestDescribeProtectConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeProtectConfigurationsRequestDescribeProtectConfigurationsPaginateTypeDef",
+    {
+        "ProtectConfigurationIds": NotRequired[Sequence[str]],
+        "Filters": NotRequired[Sequence[ProtectConfigurationFilterTypeDef]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+DescribeProtectConfigurationsRequestRequestTypeDef = TypedDict(
+    "DescribeProtectConfigurationsRequestRequestTypeDef",
+    {
+        "ProtectConfigurationIds": NotRequired[Sequence[str]],
+        "Filters": NotRequired[Sequence[ProtectConfigurationFilterTypeDef]],
+        "NextToken": NotRequired[str],
+        "MaxResults": NotRequired[int],
+    },
+)
+DescribeProtectConfigurationsResultTypeDef = TypedDict(
+    "DescribeProtectConfigurationsResultTypeDef",
+    {
+        "ProtectConfigurations": List[ProtectConfigurationInformationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef = TypedDict(
     "DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef",
     {
         "RegistrationAttachmentIds": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[RegistrationAttachmentFilterTypeDef]],
@@ -1850,27 +2090,27 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribeRegistrationAttachmentsResultTypeDef = TypedDict(
     "DescribeRegistrationAttachmentsResultTypeDef",
     {
         "RegistrationAttachments": List[RegistrationAttachmentsInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationFieldValuesResultTypeDef = TypedDict(
     "DescribeRegistrationFieldValuesResultTypeDef",
     {
         "RegistrationArn": str,
         "RegistrationId": str,
         "VersionNumber": int,
         "RegistrationFieldValues": List[RegistrationFieldValueInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef = TypedDict(
     "DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef",
     {
         "RegistrationTypes": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[RegistrationTypeFilterTypeDef]],
@@ -1922,16 +2162,16 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribeRegistrationsResultTypeDef = TypedDict(
     "DescribeRegistrationsResultTypeDef",
     {
         "Registrations": List[RegistrationInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef = TypedDict(
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     {
         "SenderIds": NotRequired[Sequence[SenderIdAndCountryTypeDef]],
         "Filters": NotRequired[Sequence[SenderIdFilterTypeDef]],
@@ -1947,24 +2187,24 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribeSenderIdsResultTypeDef = TypedDict(
     "DescribeSenderIdsResultTypeDef",
     {
         "SenderIds": List[SenderIdInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSpendLimitsResultTypeDef = TypedDict(
     "DescribeSpendLimitsResultTypeDef",
     {
         "SpendLimits": List[SpendLimitTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef = TypedDict(
     "DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef",
     {
         "VerifiedDestinationNumberIds": NotRequired[Sequence[str]],
         "DestinationPhoneNumbers": NotRequired[Sequence[str]],
@@ -1982,15 +2222,43 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribeVerifiedDestinationNumbersResultTypeDef = TypedDict(
     "DescribeVerifiedDestinationNumbersResultTypeDef",
     {
         "VerifiedDestinationNumbers": List[VerifiedDestinationNumberInformationTypeDef],
-        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+GetProtectConfigurationCountryRuleSetResultTypeDef = TypedDict(
+    "GetProtectConfigurationCountryRuleSetResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "NumberCapability": NumberCapabilityType,
+        "CountryRuleSet": Dict[str, ProtectConfigurationCountryRuleSetInformationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef = TypedDict(
+    "UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "NumberCapability": NumberCapabilityType,
+        "CountryRuleSetUpdates": Mapping[str, ProtectConfigurationCountryRuleSetInformationTypeDef],
+    },
+)
+UpdateProtectConfigurationCountryRuleSetResultTypeDef = TypedDict(
+    "UpdateProtectConfigurationCountryRuleSetResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "NumberCapability": NumberCapabilityType,
+        "CountryRuleSet": Dict[str, ProtectConfigurationCountryRuleSetInformationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = TypedDict(
     "ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
     {
         "PoolId": str,
@@ -2009,16 +2277,16 @@
 )
 ListPoolOriginationIdentitiesResultTypeDef = TypedDict(
     "ListPoolOriginationIdentitiesResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "OriginationIdentities": List[OriginationIdentityMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef = TypedDict(
     "ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef",
     {
         "RegistrationId": str,
         "Filters": NotRequired[Sequence[RegistrationAssociationFilterTypeDef]],
@@ -2037,16 +2305,16 @@
 ListRegistrationAssociationsResultTypeDef = TypedDict(
     "ListRegistrationAssociationsResultTypeDef",
     {
         "RegistrationArn": str,
         "RegistrationId": str,
         "RegistrationType": str,
         "RegistrationAssociations": List[RegistrationAssociationMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RegistrationVersionInformationTypeDef = TypedDict(
     "RegistrationVersionInformationTypeDef",
     {
         "VersionNumber": int,
         "RegistrationVersionStatus": RegistrationVersionStatusType,
@@ -2087,14 +2355,15 @@
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestinations": List[EventDestinationTypeDef],
         "CreatedTimestamp": datetime,
         "DefaultMessageType": NotRequired[MessageTypeType],
         "DefaultSenderId": NotRequired[str],
+        "ProtectConfigurationId": NotRequired[str],
     },
 )
 CreateEventDestinationResultTypeDef = TypedDict(
     "CreateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
@@ -2134,16 +2403,16 @@
 )
 DescribeRegistrationVersionsResultTypeDef = TypedDict(
     "DescribeRegistrationVersionsResultTypeDef",
     {
         "RegistrationArn": str,
         "RegistrationId": str,
         "RegistrationVersions": List[RegistrationVersionInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RegistrationFieldDefinitionTypeDef = TypedDict(
     "RegistrationFieldDefinitionTypeDef",
     {
         "SectionPath": str,
         "FieldPath": str,
@@ -2155,36 +2424,36 @@
     },
 )
 DescribeRegistrationSectionDefinitionsResultTypeDef = TypedDict(
     "DescribeRegistrationSectionDefinitionsResultTypeDef",
     {
         "RegistrationType": str,
         "RegistrationSectionDefinitions": List[RegistrationSectionDefinitionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationTypeDefinitionsResultTypeDef = TypedDict(
     "DescribeRegistrationTypeDefinitionsResultTypeDef",
     {
         "RegistrationTypeDefinitions": List[RegistrationTypeDefinitionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeConfigurationSetsResultTypeDef = TypedDict(
     "DescribeConfigurationSetsResultTypeDef",
     {
         "ConfigurationSets": List[ConfigurationSetInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationFieldDefinitionsResultTypeDef = TypedDict(
     "DescribeRegistrationFieldDefinitionsResultTypeDef",
     {
         "RegistrationType": str,
         "RegistrationFieldDefinitions": List[RegistrationFieldDefinitionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
+    AccountAttributeNameType,
     AccountLimitNameType,
     AttachmentStatusType,
     ConfigurationSetFilterNameType,
     DestinationCountryParameterKeyType,
     EventTypeType,
     FieldRequirementType,
     FieldTypeType,
@@ -32,14 +33,16 @@
     NumberCapabilityType,
     NumberStatusType,
     NumberTypeType,
     PhoneNumberFilterNameType,
     PoolFilterNameType,
     PoolOriginationIdentitiesFilterNameType,
     PoolStatusType,
+    ProtectConfigurationFilterNameType,
+    ProtectStatusType,
     RegistrationAssociationBehaviorType,
     RegistrationAssociationFilterNameType,
     RegistrationDisassociationBehaviorType,
     RegistrationFilterNameType,
     RegistrationStatusType,
     RegistrationTypeFilterNameType,
     RegistrationVersionStatusType,
@@ -66,14 +69,15 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "AssociateProtectConfigurationRequestRequestTypeDef",
     "BlobTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "ConfigurationSetFilterTypeDef",
     "TagTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "CreateRegistrationAssociationRequestRequestTypeDef",
@@ -83,14 +87,15 @@
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
     "DeleteDefaultSenderIdRequestRequestTypeDef",
     "DeleteEventDestinationRequestRequestTypeDef",
     "DeleteKeywordRequestRequestTypeDef",
     "DeleteOptOutListRequestRequestTypeDef",
     "DeleteOptedOutNumberRequestRequestTypeDef",
     "DeletePoolRequestRequestTypeDef",
+    "DeleteProtectConfigurationRequestRequestTypeDef",
     "DeleteRegistrationAttachmentRequestRequestTypeDef",
     "DeleteRegistrationFieldValueRequestRequestTypeDef",
     "DeleteRegistrationRequestRequestTypeDef",
     "DeleteVerifiedDestinationNumberRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAccountAttributesRequestRequestTypeDef",
     "DescribeAccountLimitsRequestRequestTypeDef",
@@ -100,14 +105,16 @@
     "OptOutListInformationTypeDef",
     "OptedOutFilterTypeDef",
     "OptedOutNumberInformationTypeDef",
     "PhoneNumberFilterTypeDef",
     "PhoneNumberInformationTypeDef",
     "PoolFilterTypeDef",
     "PoolInformationTypeDef",
+    "ProtectConfigurationFilterTypeDef",
+    "ProtectConfigurationInformationTypeDef",
     "RegistrationAttachmentFilterTypeDef",
     "RegistrationAttachmentsInformationTypeDef",
     "DescribeRegistrationFieldDefinitionsRequestRequestTypeDef",
     "DescribeRegistrationFieldValuesRequestRequestTypeDef",
     "RegistrationFieldValueInformationTypeDef",
     "DescribeRegistrationSectionDefinitionsRequestRequestTypeDef",
     "RegistrationTypeFilterTypeDef",
@@ -118,15 +125,18 @@
     "SenderIdFilterTypeDef",
     "SenderIdInformationTypeDef",
     "DescribeSpendLimitsRequestRequestTypeDef",
     "SpendLimitTypeDef",
     "VerifiedDestinationNumberFilterTypeDef",
     "VerifiedDestinationNumberInformationTypeDef",
     "DisassociateOriginationIdentityRequestRequestTypeDef",
+    "DisassociateProtectConfigurationRequestRequestTypeDef",
     "DiscardRegistrationVersionRequestRequestTypeDef",
+    "GetProtectConfigurationCountryRuleSetRequestRequestTypeDef",
+    "ProtectConfigurationCountryRuleSetInformationTypeDef",
     "PoolOriginationIdentitiesFilterTypeDef",
     "OriginationIdentityMetadataTypeDef",
     "RegistrationAssociationFilterTypeDef",
     "RegistrationAssociationMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutKeywordRequestRequestTypeDef",
     "PutOptedOutNumberRequestRequestTypeDef",
@@ -137,66 +147,81 @@
     "SelectOptionDescriptionTypeDef",
     "RegistrationSectionDisplayHintsTypeDef",
     "RegistrationTypeDisplayHintsTypeDef",
     "SupportedAssociationTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
     "ReleaseSenderIdRequestRequestTypeDef",
     "SendDestinationNumberVerificationCodeRequestRequestTypeDef",
+    "SendMediaMessageRequestRequestTypeDef",
     "SendTextMessageRequestRequestTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
+    "SetAccountDefaultProtectConfigurationRequestRequestTypeDef",
     "SetDefaultMessageTypeRequestRequestTypeDef",
     "SetDefaultSenderIdRequestRequestTypeDef",
+    "SetMediaMessageSpendLimitOverrideRequestRequestTypeDef",
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
     "SubmitRegistrationVersionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePoolRequestRequestTypeDef",
+    "UpdateProtectConfigurationRequestRequestTypeDef",
     "UpdateSenderIdRequestRequestTypeDef",
     "VerifyDestinationNumberRequestRequestTypeDef",
     "AssociateOriginationIdentityResultTypeDef",
+    "AssociateProtectConfigurationResultTypeDef",
     "CreateRegistrationAssociationResultTypeDef",
+    "DeleteAccountDefaultProtectConfigurationResultTypeDef",
     "DeleteDefaultMessageTypeResultTypeDef",
     "DeleteDefaultSenderIdResultTypeDef",
     "DeleteKeywordResultTypeDef",
+    "DeleteMediaMessageSpendLimitOverrideResultTypeDef",
     "DeleteOptOutListResultTypeDef",
     "DeleteOptedOutNumberResultTypeDef",
     "DeletePoolResultTypeDef",
+    "DeleteProtectConfigurationResultTypeDef",
     "DeleteRegistrationAttachmentResultTypeDef",
     "DeleteRegistrationFieldValueResultTypeDef",
     "DeleteRegistrationResultTypeDef",
     "DeleteTextMessageSpendLimitOverrideResultTypeDef",
     "DeleteVerifiedDestinationNumberResultTypeDef",
     "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "DescribeAccountLimitsResultTypeDef",
     "DisassociateOriginationIdentityResultTypeDef",
+    "DisassociateProtectConfigurationResultTypeDef",
     "PutKeywordResultTypeDef",
     "PutOptedOutNumberResultTypeDef",
     "PutRegistrationFieldValueResultTypeDef",
     "ReleasePhoneNumberResultTypeDef",
     "ReleaseSenderIdResultTypeDef",
     "SendDestinationNumberVerificationCodeResultTypeDef",
+    "SendMediaMessageResultTypeDef",
     "SendTextMessageResultTypeDef",
     "SendVoiceMessageResultTypeDef",
+    "SetAccountDefaultProtectConfigurationResultTypeDef",
     "SetDefaultMessageTypeResultTypeDef",
     "SetDefaultSenderIdResultTypeDef",
+    "SetMediaMessageSpendLimitOverrideResultTypeDef",
     "SetTextMessageSpendLimitOverrideResultTypeDef",
     "SetVoiceMessageSpendLimitOverrideResultTypeDef",
     "UpdatePhoneNumberResultTypeDef",
     "UpdatePoolResultTypeDef",
+    "UpdateProtectConfigurationResultTypeDef",
     "UpdateSenderIdResultTypeDef",
     "VerifyDestinationNumberResultTypeDef",
     "DescribeConfigurationSetsRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateConfigurationSetResultTypeDef",
     "CreateOptOutListRequestRequestTypeDef",
     "CreateOptOutListResultTypeDef",
     "CreatePoolRequestRequestTypeDef",
     "CreatePoolResultTypeDef",
+    "CreateProtectConfigurationRequestRequestTypeDef",
+    "CreateProtectConfigurationResultTypeDef",
     "CreateRegistrationAttachmentRequestRequestTypeDef",
     "CreateRegistrationAttachmentResultTypeDef",
     "CreateRegistrationRequestRequestTypeDef",
     "CreateRegistrationResultTypeDef",
     "CreateVerifiedDestinationNumberRequestRequestTypeDef",
     "CreateVerifiedDestinationNumberResultTypeDef",
     "ListTagsForResourceResultTypeDef",
@@ -228,14 +253,17 @@
     "DescribeOptedOutNumbersResultTypeDef",
     "DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef",
     "DescribePhoneNumbersRequestRequestTypeDef",
     "DescribePhoneNumbersResultTypeDef",
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     "DescribePoolsRequestRequestTypeDef",
     "DescribePoolsResultTypeDef",
+    "DescribeProtectConfigurationsRequestDescribeProtectConfigurationsPaginateTypeDef",
+    "DescribeProtectConfigurationsRequestRequestTypeDef",
+    "DescribeProtectConfigurationsResultTypeDef",
     "DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef",
     "DescribeRegistrationAttachmentsRequestRequestTypeDef",
     "DescribeRegistrationAttachmentsResultTypeDef",
     "DescribeRegistrationFieldValuesResultTypeDef",
     "DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef",
     "DescribeRegistrationTypeDefinitionsRequestRequestTypeDef",
     "DescribeRegistrationVersionsRequestDescribeRegistrationVersionsPaginateTypeDef",
@@ -246,14 +274,17 @@
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     "DescribeSenderIdsRequestRequestTypeDef",
     "DescribeSenderIdsResultTypeDef",
     "DescribeSpendLimitsResultTypeDef",
     "DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef",
     "DescribeVerifiedDestinationNumbersRequestRequestTypeDef",
     "DescribeVerifiedDestinationNumbersResultTypeDef",
+    "GetProtectConfigurationCountryRuleSetResultTypeDef",
+    "UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef",
+    "UpdateProtectConfigurationCountryRuleSetResultTypeDef",
     "ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
     "ListPoolOriginationIdentitiesRequestRequestTypeDef",
     "ListPoolOriginationIdentitiesResultTypeDef",
     "ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef",
     "ListRegistrationAssociationsRequestRequestTypeDef",
     "ListRegistrationAssociationsResultTypeDef",
     "RegistrationVersionInformationTypeDef",
@@ -272,15 +303,15 @@
     "DescribeConfigurationSetsResultTypeDef",
     "DescribeRegistrationFieldDefinitionsResultTypeDef",
 )
 
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
-        "Name": Literal["ACCOUNT_TIER"],
+        "Name": AccountAttributeNameType,
         "Value": str,
     },
 )
 AccountLimitTypeDef = TypedDict(
     "AccountLimitTypeDef",
     {
         "Name": AccountLimitNameType,
@@ -297,18 +328,25 @@
         "ClientToken": NotRequired[str],
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
+    },
+)
+AssociateProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "AssociateProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "ConfigurationSetName": str,
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
@@ -415,14 +453,20 @@
 )
 DeletePoolRequestRequestTypeDef = TypedDict(
     "DeletePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
+DeleteProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+    },
+)
 DeleteRegistrationAttachmentRequestRequestTypeDef = TypedDict(
     "DeleteRegistrationAttachmentRequestRequestTypeDef",
     {
         "RegistrationAttachmentId": str,
     },
 )
 DeleteRegistrationFieldValueRequestRequestTypeDef = TypedDict(
@@ -562,14 +606,31 @@
         "SharedRoutesEnabled": bool,
         "DeletionProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "TwoWayChannelArn": NotRequired[str],
         "TwoWayChannelRole": NotRequired[str],
     },
 )
+ProtectConfigurationFilterTypeDef = TypedDict(
+    "ProtectConfigurationFilterTypeDef",
+    {
+        "Name": ProtectConfigurationFilterNameType,
+        "Values": Sequence[str],
+    },
+)
+ProtectConfigurationInformationTypeDef = TypedDict(
+    "ProtectConfigurationInformationTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "AccountDefault": bool,
+        "DeletionProtectionEnabled": bool,
+    },
+)
 RegistrationAttachmentFilterTypeDef = TypedDict(
     "RegistrationAttachmentFilterTypeDef",
     {
         "Name": Literal["attachment-status"],
         "Values": Sequence[str],
     },
 )
@@ -723,20 +784,40 @@
     {
         "PoolId": str,
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "ClientToken": NotRequired[str],
     },
 )
+DisassociateProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "DisassociateProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "ConfigurationSetName": str,
+    },
+)
 DiscardRegistrationVersionRequestRequestTypeDef = TypedDict(
     "DiscardRegistrationVersionRequestRequestTypeDef",
     {
         "RegistrationId": str,
     },
 )
+GetProtectConfigurationCountryRuleSetRequestRequestTypeDef = TypedDict(
+    "GetProtectConfigurationCountryRuleSetRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "NumberCapability": NumberCapabilityType,
+    },
+)
+ProtectConfigurationCountryRuleSetInformationTypeDef = TypedDict(
+    "ProtectConfigurationCountryRuleSetInformationTypeDef",
+    {
+        "ProtectStatus": ProtectStatusType,
+    },
+)
 PoolOriginationIdentitiesFilterTypeDef = TypedDict(
     "PoolOriginationIdentitiesFilterTypeDef",
     {
         "Name": PoolOriginationIdentitiesFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -885,14 +966,29 @@
         "ConfigurationSetName": NotRequired[str],
         "Context": NotRequired[Mapping[str, str]],
         "DestinationCountryParameters": NotRequired[
             Mapping[DestinationCountryParameterKeyType, str]
         ],
     },
 )
+SendMediaMessageRequestRequestTypeDef = TypedDict(
+    "SendMediaMessageRequestRequestTypeDef",
+    {
+        "DestinationPhoneNumber": str,
+        "OriginationIdentity": str,
+        "MessageBody": NotRequired[str],
+        "MediaUrls": NotRequired[Sequence[str]],
+        "ConfigurationSetName": NotRequired[str],
+        "MaxPrice": NotRequired[str],
+        "TimeToLive": NotRequired[int],
+        "Context": NotRequired[Mapping[str, str]],
+        "DryRun": NotRequired[bool],
+        "ProtectConfigurationId": NotRequired[str],
+    },
+)
 SendTextMessageRequestRequestTypeDef = TypedDict(
     "SendTextMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
         "OriginationIdentity": NotRequired[str],
         "MessageBody": NotRequired[str],
         "MessageType": NotRequired[MessageTypeType],
@@ -901,14 +997,15 @@
         "MaxPrice": NotRequired[str],
         "TimeToLive": NotRequired[int],
         "Context": NotRequired[Mapping[str, str]],
         "DestinationCountryParameters": NotRequired[
             Mapping[DestinationCountryParameterKeyType, str]
         ],
         "DryRun": NotRequired[bool],
+        "ProtectConfigurationId": NotRequired[str],
     },
 )
 SendVoiceMessageRequestRequestTypeDef = TypedDict(
     "SendVoiceMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
         "OriginationIdentity": str,
@@ -916,14 +1013,21 @@
         "MessageBodyTextType": NotRequired[VoiceMessageBodyTextTypeType],
         "VoiceId": NotRequired[VoiceIdType],
         "ConfigurationSetName": NotRequired[str],
         "MaxPricePerMinute": NotRequired[str],
         "TimeToLive": NotRequired[int],
         "Context": NotRequired[Mapping[str, str]],
         "DryRun": NotRequired[bool],
+        "ProtectConfigurationId": NotRequired[str],
+    },
+)
+SetAccountDefaultProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "SetAccountDefaultProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
     },
 )
 SetDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "SetDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
@@ -932,14 +1036,20 @@
 SetDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "SetDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "SenderId": str,
     },
 )
+SetMediaMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
+    "SetMediaMessageSpendLimitOverrideRequestRequestTypeDef",
+    {
+        "MonthlyLimit": int,
+    },
+)
 SetTextMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
@@ -982,14 +1092,21 @@
         "TwoWayChannelRole": NotRequired[str],
         "SelfManagedOptOutsEnabled": NotRequired[bool],
         "OptOutListName": NotRequired[str],
         "SharedRoutesEnabled": NotRequired[bool],
         "DeletionProtectionEnabled": NotRequired[bool],
     },
 )
+UpdateProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateProtectConfigurationRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "DeletionProtectionEnabled": NotRequired[bool],
+    },
+)
 UpdateSenderIdRequestRequestTypeDef = TypedDict(
     "UpdateSenderIdRequestRequestTypeDef",
     {
         "SenderId": str,
         "IsoCountryCode": str,
         "DeletionProtectionEnabled": NotRequired[bool],
     },
@@ -1008,28 +1125,46 @@
         "PoolId": str,
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AssociateProtectConfigurationResultTypeDef = TypedDict(
+    "AssociateProtectConfigurationResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateRegistrationAssociationResultTypeDef = TypedDict(
     "CreateRegistrationAssociationResultTypeDef",
     {
         "RegistrationArn": str,
         "RegistrationId": str,
         "RegistrationType": str,
         "ResourceArn": str,
         "ResourceId": str,
         "ResourceType": str,
         "IsoCountryCode": str,
         "PhoneNumber": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeleteAccountDefaultProtectConfigurationResultTypeDef = TypedDict(
+    "DeleteAccountDefaultProtectConfigurationResultTypeDef",
+    {
+        "DefaultProtectConfigurationArn": str,
+        "DefaultProtectConfigurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteDefaultMessageTypeResultTypeDef = TypedDict(
     "DeleteDefaultMessageTypeResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1051,14 +1186,21 @@
         "OriginationIdentity": str,
         "Keyword": str,
         "KeywordMessage": str,
         "KeywordAction": KeywordActionType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeleteMediaMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteMediaMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteOptOutListResultTypeDef = TypedDict(
     "DeleteOptOutListResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1088,14 +1230,25 @@
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DeleteProtectConfigurationResultTypeDef = TypedDict(
+    "DeleteProtectConfigurationResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "AccountDefault": bool,
+        "DeletionProtectionEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteRegistrationAttachmentResultTypeDef = TypedDict(
     "DeleteRegistrationAttachmentResultTypeDef",
     {
         "RegistrationAttachmentArn": str,
         "RegistrationAttachmentId": str,
         "AttachmentStatus": AttachmentStatusType,
         "AttachmentUploadErrorReason": Literal["INTERNAL_ERROR"],
@@ -1155,37 +1308,47 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeAccountLimitsResultTypeDef = TypedDict(
     "DescribeAccountLimitsResultTypeDef",
     {
         "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DisassociateOriginationIdentityResultTypeDef = TypedDict(
     "DisassociateOriginationIdentityResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "IsoCountryCode": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DisassociateProtectConfigurationResultTypeDef = TypedDict(
+    "DisassociateProtectConfigurationResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 PutKeywordResultTypeDef = TypedDict(
     "PutKeywordResultTypeDef",
     {
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "Keyword": str,
         "KeywordMessage": str,
@@ -1255,28 +1418,43 @@
 SendDestinationNumberVerificationCodeResultTypeDef = TypedDict(
     "SendDestinationNumberVerificationCodeResultTypeDef",
     {
         "MessageId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SendMediaMessageResultTypeDef = TypedDict(
+    "SendMediaMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SendTextMessageResultTypeDef = TypedDict(
     "SendTextMessageResultTypeDef",
     {
         "MessageId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SendVoiceMessageResultTypeDef = TypedDict(
     "SendVoiceMessageResultTypeDef",
     {
         "MessageId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SetAccountDefaultProtectConfigurationResultTypeDef = TypedDict(
+    "SetAccountDefaultProtectConfigurationResultTypeDef",
+    {
+        "DefaultProtectConfigurationArn": str,
+        "DefaultProtectConfigurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SetDefaultMessageTypeResultTypeDef = TypedDict(
     "SetDefaultMessageTypeResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1287,14 +1465,21 @@
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "SenderId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SetMediaMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetMediaMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
     "SetTextMessageSpendLimitOverrideResultTypeDef",
     {
         "MonthlyLimit": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1342,14 +1527,25 @@
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
         "DeletionProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateProtectConfigurationResultTypeDef = TypedDict(
+    "UpdateProtectConfigurationResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "AccountDefault": bool,
+        "DeletionProtectionEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 UpdateSenderIdResultTypeDef = TypedDict(
     "UpdateSenderIdResultTypeDef",
     {
         "SenderIdArn": str,
         "SenderId": str,
         "IsoCountryCode": str,
         "MessageTypes": List[MessageTypeType],
@@ -1442,14 +1638,34 @@
         "SharedRoutesEnabled": bool,
         "DeletionProtectionEnabled": bool,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateProtectConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateProtectConfigurationRequestRequestTypeDef",
+    {
+        "ClientToken": NotRequired[str],
+        "DeletionProtectionEnabled": NotRequired[bool],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+CreateProtectConfigurationResultTypeDef = TypedDict(
+    "CreateProtectConfigurationResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "AccountDefault": bool,
+        "DeletionProtectionEnabled": bool,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateRegistrationAttachmentRequestRequestTypeDef = TypedDict(
     "CreateRegistrationAttachmentRequestRequestTypeDef",
     {
         "AttachmentBody": NotRequired[BlobTypeDef],
         "AttachmentUrl": NotRequired[str],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "ClientToken": NotRequired[str],
@@ -1737,24 +1953,24 @@
 )
 DescribeKeywordsResultTypeDef = TypedDict(
     "DescribeKeywordsResultTypeDef",
     {
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "Keywords": List[KeywordInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeOptOutListsResultTypeDef = TypedDict(
     "DescribeOptOutListsResultTypeDef",
     {
         "OptOutLists": List[OptOutListInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumbers": NotRequired[Sequence[str]],
@@ -1774,16 +1990,16 @@
 )
 DescribeOptedOutNumbersResultTypeDef = TypedDict(
     "DescribeOptedOutNumbersResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "OptedOutNumbers": List[OptedOutNumberInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef = TypedDict(
     "DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef",
     {
         "PhoneNumberIds": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[PhoneNumberFilterTypeDef]],
@@ -1799,16 +2015,16 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribePhoneNumbersResultTypeDef = TypedDict(
     "DescribePhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribePoolsRequestDescribePoolsPaginateTypeDef = TypedDict(
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     {
         "PoolIds": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[PoolFilterTypeDef]],
@@ -1824,16 +2040,41 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribePoolsResultTypeDef = TypedDict(
     "DescribePoolsResultTypeDef",
     {
         "Pools": List[PoolInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DescribeProtectConfigurationsRequestDescribeProtectConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeProtectConfigurationsRequestDescribeProtectConfigurationsPaginateTypeDef",
+    {
+        "ProtectConfigurationIds": NotRequired[Sequence[str]],
+        "Filters": NotRequired[Sequence[ProtectConfigurationFilterTypeDef]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+DescribeProtectConfigurationsRequestRequestTypeDef = TypedDict(
+    "DescribeProtectConfigurationsRequestRequestTypeDef",
+    {
+        "ProtectConfigurationIds": NotRequired[Sequence[str]],
+        "Filters": NotRequired[Sequence[ProtectConfigurationFilterTypeDef]],
+        "NextToken": NotRequired[str],
+        "MaxResults": NotRequired[int],
+    },
+)
+DescribeProtectConfigurationsResultTypeDef = TypedDict(
+    "DescribeProtectConfigurationsResultTypeDef",
+    {
+        "ProtectConfigurations": List[ProtectConfigurationInformationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef = TypedDict(
     "DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef",
     {
         "RegistrationAttachmentIds": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[RegistrationAttachmentFilterTypeDef]],
@@ -1849,27 +2090,27 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribeRegistrationAttachmentsResultTypeDef = TypedDict(
     "DescribeRegistrationAttachmentsResultTypeDef",
     {
         "RegistrationAttachments": List[RegistrationAttachmentsInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationFieldValuesResultTypeDef = TypedDict(
     "DescribeRegistrationFieldValuesResultTypeDef",
     {
         "RegistrationArn": str,
         "RegistrationId": str,
         "VersionNumber": int,
         "RegistrationFieldValues": List[RegistrationFieldValueInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef = TypedDict(
     "DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef",
     {
         "RegistrationTypes": NotRequired[Sequence[str]],
         "Filters": NotRequired[Sequence[RegistrationTypeFilterTypeDef]],
@@ -1921,16 +2162,16 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribeRegistrationsResultTypeDef = TypedDict(
     "DescribeRegistrationsResultTypeDef",
     {
         "Registrations": List[RegistrationInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef = TypedDict(
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     {
         "SenderIds": NotRequired[Sequence[SenderIdAndCountryTypeDef]],
         "Filters": NotRequired[Sequence[SenderIdFilterTypeDef]],
@@ -1946,24 +2187,24 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribeSenderIdsResultTypeDef = TypedDict(
     "DescribeSenderIdsResultTypeDef",
     {
         "SenderIds": List[SenderIdInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSpendLimitsResultTypeDef = TypedDict(
     "DescribeSpendLimitsResultTypeDef",
     {
         "SpendLimits": List[SpendLimitTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef = TypedDict(
     "DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef",
     {
         "VerifiedDestinationNumberIds": NotRequired[Sequence[str]],
         "DestinationPhoneNumbers": NotRequired[Sequence[str]],
@@ -1981,15 +2222,43 @@
         "MaxResults": NotRequired[int],
     },
 )
 DescribeVerifiedDestinationNumbersResultTypeDef = TypedDict(
     "DescribeVerifiedDestinationNumbersResultTypeDef",
     {
         "VerifiedDestinationNumbers": List[VerifiedDestinationNumberInformationTypeDef],
-        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+GetProtectConfigurationCountryRuleSetResultTypeDef = TypedDict(
+    "GetProtectConfigurationCountryRuleSetResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "NumberCapability": NumberCapabilityType,
+        "CountryRuleSet": Dict[str, ProtectConfigurationCountryRuleSetInformationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef = TypedDict(
+    "UpdateProtectConfigurationCountryRuleSetRequestRequestTypeDef",
+    {
+        "ProtectConfigurationId": str,
+        "NumberCapability": NumberCapabilityType,
+        "CountryRuleSetUpdates": Mapping[str, ProtectConfigurationCountryRuleSetInformationTypeDef],
+    },
+)
+UpdateProtectConfigurationCountryRuleSetResultTypeDef = TypedDict(
+    "UpdateProtectConfigurationCountryRuleSetResultTypeDef",
+    {
+        "ProtectConfigurationArn": str,
+        "ProtectConfigurationId": str,
+        "NumberCapability": NumberCapabilityType,
+        "CountryRuleSet": Dict[str, ProtectConfigurationCountryRuleSetInformationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = TypedDict(
     "ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
     {
         "PoolId": str,
@@ -2008,16 +2277,16 @@
 )
 ListPoolOriginationIdentitiesResultTypeDef = TypedDict(
     "ListPoolOriginationIdentitiesResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "OriginationIdentities": List[OriginationIdentityMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef = TypedDict(
     "ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef",
     {
         "RegistrationId": str,
         "Filters": NotRequired[Sequence[RegistrationAssociationFilterTypeDef]],
@@ -2036,16 +2305,16 @@
 ListRegistrationAssociationsResultTypeDef = TypedDict(
     "ListRegistrationAssociationsResultTypeDef",
     {
         "RegistrationArn": str,
         "RegistrationId": str,
         "RegistrationType": str,
         "RegistrationAssociations": List[RegistrationAssociationMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RegistrationVersionInformationTypeDef = TypedDict(
     "RegistrationVersionInformationTypeDef",
     {
         "VersionNumber": int,
         "RegistrationVersionStatus": RegistrationVersionStatusType,
@@ -2086,14 +2355,15 @@
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestinations": List[EventDestinationTypeDef],
         "CreatedTimestamp": datetime,
         "DefaultMessageType": NotRequired[MessageTypeType],
         "DefaultSenderId": NotRequired[str],
+        "ProtectConfigurationId": NotRequired[str],
     },
 )
 CreateEventDestinationResultTypeDef = TypedDict(
     "CreateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
@@ -2133,16 +2403,16 @@
 )
 DescribeRegistrationVersionsResultTypeDef = TypedDict(
     "DescribeRegistrationVersionsResultTypeDef",
     {
         "RegistrationArn": str,
         "RegistrationId": str,
         "RegistrationVersions": List[RegistrationVersionInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RegistrationFieldDefinitionTypeDef = TypedDict(
     "RegistrationFieldDefinitionTypeDef",
     {
         "SectionPath": str,
         "FieldPath": str,
@@ -2154,36 +2424,36 @@
     },
 )
 DescribeRegistrationSectionDefinitionsResultTypeDef = TypedDict(
     "DescribeRegistrationSectionDefinitionsResultTypeDef",
     {
         "RegistrationType": str,
         "RegistrationSectionDefinitions": List[RegistrationSectionDefinitionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationTypeDefinitionsResultTypeDef = TypedDict(
     "DescribeRegistrationTypeDefinitionsResultTypeDef",
     {
         "RegistrationTypeDefinitions": List[RegistrationTypeDefinitionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeConfigurationSetsResultTypeDef = TypedDict(
     "DescribeConfigurationSetsResultTypeDef",
     {
         "ConfigurationSets": List[ConfigurationSetInformationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeRegistrationFieldDefinitionsResultTypeDef = TypedDict(
     "DescribeRegistrationFieldDefinitionsResultTypeDef",
     {
         "RegistrationType": str,
         "RegistrationFieldDefinitions": List[RegistrationFieldDefinitionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-sms-voice-v2
-Version: 1.34.0
-Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.95
+Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
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
 
 <a id="mypy-boto3-pinpoint-sms-voice-v2"></a>
 
 # mypy-boto3-pinpoint-sms-voice-v2
 
 [![PyPI - mypy-boto3-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-sms-voice-v2)](https://pepy.tech/project/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,14 +290,15 @@
     DescribeAccountLimitsPaginator,
     DescribeConfigurationSetsPaginator,
     DescribeKeywordsPaginator,
     DescribeOptOutListsPaginator,
     DescribeOptedOutNumbersPaginator,
     DescribePhoneNumbersPaginator,
     DescribePoolsPaginator,
+    DescribeProtectConfigurationsPaginator,
     DescribeRegistrationAttachmentsPaginator,
     DescribeRegistrationFieldDefinitionsPaginator,
     DescribeRegistrationFieldValuesPaginator,
     DescribeRegistrationSectionDefinitionsPaginator,
     DescribeRegistrationTypeDefinitionsPaginator,
     DescribeRegistrationVersionsPaginator,
     DescribeRegistrationsPaginator,
@@ -328,14 +329,17 @@
 describe_opted_out_numbers_paginator: DescribeOptedOutNumbersPaginator = client.get_paginator(
     "describe_opted_out_numbers"
 )
 describe_phone_numbers_paginator: DescribePhoneNumbersPaginator = client.get_paginator(
     "describe_phone_numbers"
 )
 describe_pools_paginator: DescribePoolsPaginator = client.get_paginator("describe_pools")
+describe_protect_configurations_paginator: DescribeProtectConfigurationsPaginator = (
+    client.get_paginator("describe_protect_configurations")
+)
 describe_registration_attachments_paginator: DescribeRegistrationAttachmentsPaginator = (
     client.get_paginator("describe_registration_attachments")
 )
 describe_registration_field_definitions_paginator: DescribeRegistrationFieldDefinitionsPaginator = (
     client.get_paginator("describe_registration_field_definitions")
 )
 describe_registration_field_values_paginator: DescribeRegistrationFieldValuesPaginator = (
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.34.0/setup.py` & `mypy_boto3_pinpoint_sms_voice_v2-1.34.95/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,52 +7,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-sms-voice-v2",
-    version="1.34.0",
+    version="1.34.95",
     packages=["mypy_boto3_pinpoint_sms_voice_v2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.PinpointSMSVoiceV2 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.PinpointSMSVoiceV2 1.34.95 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 pinpoint-sms-voice-v2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_pinpoint_sms_voice_v2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
-        "Documentation": (
-            "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/"
-        ),
+        "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
     ],
     zip_safe=False,
```

