# Comparing `tmp/mypy-boto3-signer-1.34.0.tar.gz` & `tmp/mypy_boto3_signer-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-signer-1.34.0.tar", last modified: Wed Dec 13 21:23:52 2023, max compression
+gzip compressed data, was "mypy_boto3_signer-1.34.95.tar", last modified: Tue Apr 30 19:34:55 2024, max compression
```

## Comparing `mypy-boto3-signer-1.34.0.tar` & `mypy_boto3_signer-1.34.95.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:52.943382 mypy-boto3-signer-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13540 2023-12-13 21:23:52.943382 mypy-boto3-signer-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:52.943382 mypy-boto3-signer-1.34.0/mypy_boto3_signer/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17105 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9626 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20006 2023-12-13 21:20:00.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20005 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:52.943382 mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13540 2023-12-13 21:23:52.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-13 21:23:52.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:52.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:52.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:52.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-13 21:23:52.000000 mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:52.943382 mypy-boto3-signer-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-12-13 21:19:57.000000 mypy-boto3-signer-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:55.131069 mypy_boto3_signer-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:34:37.000000 mypy_boto3_signer-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-04-30 19:34:55.131069 mypy_boto3_signer-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-30 19:34:37.000000 mypy_boto3_signer-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:55.131069 mypy_boto3_signer-1.34.95/mypy_boto3_signer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-30 19:34:37.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-30 19:34:37.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-30 19:34:37.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17108 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:37.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20018 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20018 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:34:37.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-30 19:34:38.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:55.131069 mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-04-30 19:34:55.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 19:34:55.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:55.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:55.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:55.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 19:34:55.000000 mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:55.131069 mypy_boto3_signer-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-30 19:34:37.000000 mypy_boto3_signer-1.34.95/setup.py
```

### Comparing `mypy-boto3-signer-1.34.0/LICENSE` & `mypy_boto3_signer-1.34.95/LICENSE`

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

### Comparing `mypy-boto3-signer-1.34.0/PKG-INFO` & `mypy_boto3_signer-1.34.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.34.0
-Summary: Type annotations for boto3.signer 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.95
+Summary: Type annotations for boto3.Signer 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
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
 
 <a id="mypy-boto3-signer"></a>
 
 # mypy-boto3-signer
 
 [![PyPI - mypy-boto3-signer](https://img.shields.io/pypi/v/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.Signer 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -98,21 +98,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `signer`.
+Click `Modify` and select `boto3 common` and `Signer`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `signer` service.
+Install `boto3-stubs` for `Signer` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[signer]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -257,44 +257,44 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`signerClient` provides annotations for `boto3.client("signer")`.
+`SignerClient` provides annotations for `boto3.client("signer")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="paginators-annotations"></a>
 
 ### Paginators annotations
 
 `mypy_boto3_signer.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 from mypy_boto3_signer.paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
 list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator(
     "list_signing_platforms"
 )
@@ -308,18 +308,18 @@
 ### Waiters annotations
 
 `mypy_boto3_signer.waiter` module contains type annotations for all waiters.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 from mypy_boto3_signer.waiter import SuccessfulSigningJobWaiter
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 successful_signing_job_waiter: SuccessfulSigningJobWaiter = client.get_waiter(
     "successful_signing_job"
 )
 ```
@@ -327,15 +327,15 @@
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_signer.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
-Full list of `signer` Literals can be found in
+Full list of `Signer` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/literals/).
 
 ```python
 from mypy_boto3_signer.literals import CategoryType
 
 
 def check_value(value: CategoryType) -> bool: ...
@@ -344,15 +344,15 @@
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
-Full list of `signer` TypeDefs can be found in
+Full list of `Signer` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/type_defs/).
 
 ```python
 from mypy_boto3_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
 
 def get_value() -> AddProfilePermissionRequestRequestTypeDef:
```

### Comparing `mypy-boto3-signer-1.34.0/README.md` & `mypy_boto3_signer-1.34.95/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.Signer 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -65,21 +65,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `signer`.
+Click `Modify` and select `boto3 common` and `Signer`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `signer` service.
+Install `boto3-stubs` for `Signer` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[signer]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -224,44 +224,44 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`signerClient` provides annotations for `boto3.client("signer")`.
+`SignerClient` provides annotations for `boto3.client("signer")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="paginators-annotations"></a>
 
 ### Paginators annotations
 
 `mypy_boto3_signer.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 from mypy_boto3_signer.paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
 list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator(
     "list_signing_platforms"
 )
@@ -275,18 +275,18 @@
 ### Waiters annotations
 
 `mypy_boto3_signer.waiter` module contains type annotations for all waiters.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 from mypy_boto3_signer.waiter import SuccessfulSigningJobWaiter
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 successful_signing_job_waiter: SuccessfulSigningJobWaiter = client.get_waiter(
     "successful_signing_job"
 )
 ```
@@ -294,15 +294,15 @@
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_signer.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
-Full list of `signer` Literals can be found in
+Full list of `Signer` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/literals/).
 
 ```python
 from mypy_boto3_signer.literals import CategoryType
 
 
 def check_value(value: CategoryType) -> bool: ...
@@ -311,15 +311,15 @@
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
-Full list of `signer` TypeDefs can be found in
+Full list of `Signer` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/type_defs/).
 
 ```python
 from mypy_boto3_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
 
 def get_value() -> AddProfilePermissionRequestRequestTypeDef:
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/__init__.py` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,41 +6,40 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_signer import (
         Client,
         ListSigningJobsPaginator,
         ListSigningPlatformsPaginator,
         ListSigningProfilesPaginator,
+        SignerClient,
         SuccessfulSigningJobWaiter,
-        signerClient,
     )
 
     session = Session()
-    client: signerClient = session.client("signer")
+    client: SignerClient = session.client("signer")
 
     successful_signing_job_waiter: SuccessfulSigningJobWaiter = client.get_waiter("successful_signing_job")
 
     list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
     list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
     list_signing_profiles_paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
     ```
 """
 
-from .client import signerClient
+from .client import SignerClient
 from .paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
-Client = signerClient
-
+Client = SignerClient
 
 __all__ = (
     "Client",
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
+    "SignerClient",
     "SuccessfulSigningJobWaiter",
-    "signerClient",
 )
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/__init__.pyi` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -6,40 +6,40 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_signer import (
         Client,
         ListSigningJobsPaginator,
         ListSigningPlatformsPaginator,
         ListSigningProfilesPaginator,
+        SignerClient,
         SuccessfulSigningJobWaiter,
-        signerClient,
     )
 
     session = Session()
-    client: signerClient = session.client("signer")
+    client: SignerClient = session.client("signer")
 
     successful_signing_job_waiter: SuccessfulSigningJobWaiter = client.get_waiter("successful_signing_job")
 
     list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
     list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
     list_signing_profiles_paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
     ```
 """
 
-from .client import signerClient
+from .client import SignerClient
 from .paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
-Client = signerClient
+Client = SignerClient
 
 __all__ = (
     "Client",
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
+    "SignerClient",
     "SuccessfulSigningJobWaiter",
-    "signerClient",
 )
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/__main__.py` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.signer 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Signer 1.34.95\n"
+        "Version:         1.34.95\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer\n"
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

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/client.py` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/)
 
 Usage::
 
     ```python
     from boto3.session import Session
-    from mypy_boto3_signer.client import signerClient
+    from mypy_boto3_signer.client import SignerClient
 
     session = Session()
-    client: signerClient = session.client("signer")
+    client: SignerClient = session.client("signer")
     ```
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
@@ -52,16 +52,15 @@
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
-__all__ = ("signerClient",)
+__all__ = ("SignerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -78,318 +77,318 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
-class signerClient(BaseClient):
+class SignerClient(BaseClient):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/)
     """
 
     meta: ClientMeta
 
     @property
     def exceptions(self) -> Exceptions:
         """
-        signerClient exceptions.
+        SignerClient exceptions.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#exceptions)
         """
 
     def add_profile_permission(
         self,
         *,
         profileName: str,
         action: str,
         principal: str,
         statementId: str,
         profileVersion: str = ...,
-        revisionId: str = ...
+        revisionId: str = ...,
     ) -> AddProfilePermissionResponseTypeDef:
         """
         Adds cross-account permissions to a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.add_profile_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#add_profile_permission)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.can_paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#can_paginate)
         """
 
     def cancel_signing_profile(self, *, profileName: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of an `ACTIVE` signing profile to `CANCELED`.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.cancel_signing_profile)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.cancel_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#cancel_signing_profile)
         """
 
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.close)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#close)
         """
 
     def describe_signing_job(self, *, jobId: str) -> DescribeSigningJobResponseTypeDef:
         """
         Returns information about a specific code signing job.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.describe_signing_job)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.describe_signing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#describe_signing_job)
         """
 
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#generate_presigned_url)
         """
 
     def get_revocation_status(
         self,
         *,
         signatureTimestamp: TimestampTypeDef,
         platformId: str,
         profileVersionArn: str,
         jobArn: str,
-        certificateHashes: Sequence[str]
+        certificateHashes: Sequence[str],
     ) -> GetRevocationStatusResponseTypeDef:
         """
         Retrieves the revocation status of one or more of the signing profile, signing
         job, and signing
         certificate.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_revocation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_revocation_status)
         """
 
     def get_signing_platform(self, *, platformId: str) -> GetSigningPlatformResponseTypeDef:
         """
         Returns information on a specific signing platform.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_signing_platform)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_platform)
         """
 
     def get_signing_profile(
         self, *, profileName: str, profileOwner: str = ...
     ) -> GetSigningProfileResponseTypeDef:
         """
         Returns information on a specific signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_profile)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_profile)
         """
 
     def list_profile_permissions(
         self, *, profileName: str, nextToken: str = ...
     ) -> ListProfilePermissionsResponseTypeDef:
         """
         Lists the cross-account permissions associated with a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_profile_permissions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_profile_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_profile_permissions)
         """
 
     def list_signing_jobs(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: TimestampTypeDef = ...,
         signatureExpiresAfter: TimestampTypeDef = ...,
-        jobInvoker: str = ...
+        jobInvoker: str = ...,
     ) -> ListSigningJobsResponseTypeDef:
         """
         Lists all your signing jobs.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_signing_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_jobs)
         """
 
     def list_signing_platforms(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSigningPlatformsResponseTypeDef:
         """
         Lists all signing platforms available in AWS Signer that match the request
         parameters.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_signing_platforms)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_platforms)
         """
 
     def list_signing_profiles(
         self,
         *,
         includeCanceled: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         platformId: str = ...,
-        statuses: Sequence[SigningProfileStatusType] = ...
+        statuses: Sequence[SigningProfileStatusType] = ...,
     ) -> ListSigningProfilesResponseTypeDef:
         """
         Lists all available signing profiles in your AWS account.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_signing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_profiles)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags associated with a signing profile resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_tags_for_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_tags_for_resource)
         """
 
     def put_signing_profile(
         self,
         *,
         profileName: str,
         platformId: str,
         signingMaterial: SigningMaterialTypeDef = ...,
         signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,
         overrides: SigningPlatformOverridesTypeDef = ...,
         signingParameters: Mapping[str, str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> PutSigningProfileResponseTypeDef:
         """
         Creates a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.put_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#put_signing_profile)
         """
 
     def remove_profile_permission(
         self, *, profileName: str, revisionId: str, statementId: str
     ) -> RemoveProfilePermissionResponseTypeDef:
         """
         Removes cross-account permissions from a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.remove_profile_permission)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.remove_profile_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#remove_profile_permission)
         """
 
     def revoke_signature(
         self, *, jobId: str, reason: str, jobOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing job to REVOKED.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signature)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.revoke_signature)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signature)
         """
 
     def revoke_signing_profile(
         self, *, profileName: str, profileVersion: str, reason: str, effectiveTime: TimestampTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing profile to REVOKED.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.revoke_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signing_profile)
         """
 
     def sign_payload(
         self, *, profileName: str, payload: BlobTypeDef, payloadFormat: str, profileOwner: str = ...
     ) -> SignPayloadResponseTypeDef:
         """
         Signs a binary payload and returns a signature envelope.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.sign_payload)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.sign_payload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#sign_payload)
         """
 
     def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
-        profileOwner: str = ...
+        profileOwner: str = ...,
     ) -> StartSigningJobResponseTypeDef:
         """
         Initiates a signing job to be performed on the code provided.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.start_signing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#start_signing_job)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.tag_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.untag_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#untag_resource)
         """
 
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_jobs"]
     ) -> ListSigningJobsPaginator:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_platforms"]
     ) -> ListSigningPlatformsPaginator:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_profiles"]
     ) -> ListSigningProfilesPaginator:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
 
     def get_waiter(
         self, waiter_name: Literal["successful_signing_job"]
     ) -> SuccessfulSigningJobWaiter:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_waiter)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/client.pyi` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/)
 
 Usage::
 
     ```python
     from boto3.session import Session
-    from mypy_boto3_signer.client import signerClient
+    from mypy_boto3_signer.client import SignerClient
 
     session = Session()
-    client: signerClient = session.client("signer")
+    client: SignerClient = session.client("signer")
     ```
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
@@ -52,15 +52,15 @@
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-__all__ = ("signerClient",)
+__all__ = ("SignerClient",)
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
@@ -74,318 +74,318 @@
     NotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-class signerClient(BaseClient):
+class SignerClient(BaseClient):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/)
     """
 
     meta: ClientMeta
 
     @property
     def exceptions(self) -> Exceptions:
         """
-        signerClient exceptions.
+        SignerClient exceptions.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#exceptions)
         """
 
     def add_profile_permission(
         self,
         *,
         profileName: str,
         action: str,
         principal: str,
         statementId: str,
         profileVersion: str = ...,
-        revisionId: str = ...
+        revisionId: str = ...,
     ) -> AddProfilePermissionResponseTypeDef:
         """
         Adds cross-account permissions to a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.add_profile_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#add_profile_permission)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.can_paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#can_paginate)
         """
 
     def cancel_signing_profile(self, *, profileName: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of an `ACTIVE` signing profile to `CANCELED`.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.cancel_signing_profile)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.cancel_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#cancel_signing_profile)
         """
 
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.close)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#close)
         """
 
     def describe_signing_job(self, *, jobId: str) -> DescribeSigningJobResponseTypeDef:
         """
         Returns information about a specific code signing job.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.describe_signing_job)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.describe_signing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#describe_signing_job)
         """
 
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#generate_presigned_url)
         """
 
     def get_revocation_status(
         self,
         *,
         signatureTimestamp: TimestampTypeDef,
         platformId: str,
         profileVersionArn: str,
         jobArn: str,
-        certificateHashes: Sequence[str]
+        certificateHashes: Sequence[str],
     ) -> GetRevocationStatusResponseTypeDef:
         """
         Retrieves the revocation status of one or more of the signing profile, signing
         job, and signing
         certificate.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_revocation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_revocation_status)
         """
 
     def get_signing_platform(self, *, platformId: str) -> GetSigningPlatformResponseTypeDef:
         """
         Returns information on a specific signing platform.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_signing_platform)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_platform)
         """
 
     def get_signing_profile(
         self, *, profileName: str, profileOwner: str = ...
     ) -> GetSigningProfileResponseTypeDef:
         """
         Returns information on a specific signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_profile)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_profile)
         """
 
     def list_profile_permissions(
         self, *, profileName: str, nextToken: str = ...
     ) -> ListProfilePermissionsResponseTypeDef:
         """
         Lists the cross-account permissions associated with a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_profile_permissions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_profile_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_profile_permissions)
         """
 
     def list_signing_jobs(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: TimestampTypeDef = ...,
         signatureExpiresAfter: TimestampTypeDef = ...,
-        jobInvoker: str = ...
+        jobInvoker: str = ...,
     ) -> ListSigningJobsResponseTypeDef:
         """
         Lists all your signing jobs.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_signing_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_jobs)
         """
 
     def list_signing_platforms(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListSigningPlatformsResponseTypeDef:
         """
         Lists all signing platforms available in AWS Signer that match the request
         parameters.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_signing_platforms)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_platforms)
         """
 
     def list_signing_profiles(
         self,
         *,
         includeCanceled: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         platformId: str = ...,
-        statuses: Sequence[SigningProfileStatusType] = ...
+        statuses: Sequence[SigningProfileStatusType] = ...,
     ) -> ListSigningProfilesResponseTypeDef:
         """
         Lists all available signing profiles in your AWS account.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_signing_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_signing_profiles)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags associated with a signing profile resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_tags_for_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#list_tags_for_resource)
         """
 
     def put_signing_profile(
         self,
         *,
         profileName: str,
         platformId: str,
         signingMaterial: SigningMaterialTypeDef = ...,
         signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,
         overrides: SigningPlatformOverridesTypeDef = ...,
         signingParameters: Mapping[str, str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> PutSigningProfileResponseTypeDef:
         """
         Creates a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.put_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#put_signing_profile)
         """
 
     def remove_profile_permission(
         self, *, profileName: str, revisionId: str, statementId: str
     ) -> RemoveProfilePermissionResponseTypeDef:
         """
         Removes cross-account permissions from a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.remove_profile_permission)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.remove_profile_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#remove_profile_permission)
         """
 
     def revoke_signature(
         self, *, jobId: str, reason: str, jobOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing job to REVOKED.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signature)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.revoke_signature)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signature)
         """
 
     def revoke_signing_profile(
         self, *, profileName: str, profileVersion: str, reason: str, effectiveTime: TimestampTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing profile to REVOKED.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.revoke_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signing_profile)
         """
 
     def sign_payload(
         self, *, profileName: str, payload: BlobTypeDef, payloadFormat: str, profileOwner: str = ...
     ) -> SignPayloadResponseTypeDef:
         """
         Signs a binary payload and returns a signature envelope.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.sign_payload)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.sign_payload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#sign_payload)
         """
 
     def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
-        profileOwner: str = ...
+        profileOwner: str = ...,
     ) -> StartSigningJobResponseTypeDef:
         """
         Initiates a signing job to be performed on the code provided.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.start_signing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#start_signing_job)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.tag_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a signing profile.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.untag_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#untag_resource)
         """
 
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_jobs"]
     ) -> ListSigningJobsPaginator:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_platforms"]
     ) -> ListSigningPlatformsPaginator:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_profiles"]
     ) -> ListSigningProfilesPaginator:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_paginator)
         """
 
     def get_waiter(
         self, waiter_name: Literal["successful_signing_job"]
     ) -> SuccessfulSigningJobWaiter:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_waiter)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/literals.py` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,48 +15,46 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CategoryType",
     "EncryptionAlgorithmType",
     "HashAlgorithmType",
     "ImageFormatType",
     "ListSigningJobsPaginatorName",
     "ListSigningPlatformsPaginatorName",
     "ListSigningProfilesPaginatorName",
     "SigningProfileStatusType",
     "SigningStatusType",
     "SuccessfulSigningJobWaiterName",
     "ValidityTypeType",
-    "signerServiceName",
+    "SignerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 CategoryType = Literal["AWSIoT"]
 EncryptionAlgorithmType = Literal["ECDSA", "RSA"]
 HashAlgorithmType = Literal["SHA1", "SHA256"]
 ImageFormatType = Literal["JSON", "JSONDetached", "JSONEmbedded"]
 ListSigningJobsPaginatorName = Literal["list_signing_jobs"]
 ListSigningPlatformsPaginatorName = Literal["list_signing_platforms"]
 ListSigningProfilesPaginatorName = Literal["list_signing_profiles"]
 SigningProfileStatusType = Literal["Active", "Canceled", "Revoked"]
 SigningStatusType = Literal["Failed", "InProgress", "Succeeded"]
 SuccessfulSigningJobWaiterName = Literal["successful_signing_job"]
 ValidityTypeType = Literal["DAYS", "MONTHS", "YEARS"]
-signerServiceName = Literal["signer"]
+SignerServiceName = Literal["signer"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
     "amp",
@@ -75,14 +73,15 @@
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
@@ -93,14 +92,15 @@
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
@@ -118,14 +118,15 @@
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
@@ -138,24 +139,26 @@
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
@@ -216,15 +219,14 @@
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
@@ -296,17 +298,19 @@
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
@@ -351,14 +355,15 @@
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
@@ -396,19 +401,21 @@
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

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/literals.pyi` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "ListSigningJobsPaginatorName",
     "ListSigningPlatformsPaginatorName",
     "ListSigningProfilesPaginatorName",
     "SigningProfileStatusType",
     "SigningStatusType",
     "SuccessfulSigningJobWaiterName",
     "ValidityTypeType",
-    "signerServiceName",
+    "SignerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
@@ -46,15 +46,15 @@
 ListSigningJobsPaginatorName = Literal["list_signing_jobs"]
 ListSigningPlatformsPaginatorName = Literal["list_signing_platforms"]
 ListSigningProfilesPaginatorName = Literal["list_signing_profiles"]
 SigningProfileStatusType = Literal["Active", "Canceled", "Revoked"]
 SigningStatusType = Literal["Failed", "InProgress", "Succeeded"]
 SuccessfulSigningJobWaiterName = Literal["successful_signing_job"]
 ValidityTypeType = Literal["DAYS", "MONTHS", "YEARS"]
-signerServiceName = Literal["signer"]
+SignerServiceName = Literal["signer"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
     "amp",
@@ -73,14 +73,15 @@
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
@@ -91,14 +92,15 @@
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
@@ -116,14 +118,15 @@
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
@@ -136,24 +139,26 @@
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
@@ -214,15 +219,14 @@
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
@@ -294,17 +298,19 @@
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
@@ -349,14 +355,15 @@
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
@@ -394,19 +401,21 @@
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

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/paginator.py` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/)
 
 Usage::
 
     ```python
     from boto3.session import Session
 
-    from mypy_boto3_signer.client import signerClient
+    from mypy_boto3_signer.client import SignerClient
     from mypy_boto3_signer.paginator import (
         ListSigningJobsPaginator,
         ListSigningPlatformsPaginator,
         ListSigningProfilesPaginator,
     )
 
     session = Session()
-    client: signerClient = session.client("signer")
+    client: SignerClient = session.client("signer")
 
     list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
     list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
     list_signing_profiles_paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
     ```
 """
 
@@ -39,80 +39,75 @@
 
 __all__ = (
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListSigningJobsPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
     """
 
     def paginate(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: TimestampTypeDef = ...,
         signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSigningJobsResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
         """
 
-
 class ListSigningPlatformsPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningPlatforms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningplatformspaginator)
     """
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSigningPlatformsResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningPlatforms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningplatformspaginator)
         """
 
-
 class ListSigningProfilesPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSigningProfilesResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/paginator.pyi` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/)
 
 Usage::
 
     ```python
     from boto3.session import Session
 
-    from mypy_boto3_signer.client import signerClient
+    from mypy_boto3_signer.client import SignerClient
     from mypy_boto3_signer.paginator import (
         ListSigningJobsPaginator,
         ListSigningPlatformsPaginator,
         ListSigningProfilesPaginator,
     )
 
     session = Session()
-    client: signerClient = session.client("signer")
+    client: SignerClient = session.client("signer")
 
     list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
     list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
     list_signing_profiles_paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
     ```
 """
 
@@ -41,73 +41,77 @@
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListSigningJobsPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
     """
 
     def paginate(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: TimestampTypeDef = ...,
         signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSigningJobsResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
         """
 
+
 class ListSigningPlatformsPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningPlatforms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningplatformspaginator)
     """
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSigningPlatformsResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningPlatforms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningplatformspaginator)
         """
 
+
 class ListSigningProfilesPaginator(Paginator):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningprofilespaginator)
     """
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSigningProfilesResponseTypeDef]:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Paginator.ListSigningProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/type_defs.py` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BlobTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -118,18 +117,18 @@
         "revisionId": NotRequired[str],
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
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/type_defs.pyi` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -117,18 +117,18 @@
         "revisionId": NotRequired[str],
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
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/waiter.py` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/waiter.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/waiters/)
 
 Usage::
 
     ```python
     from boto3.session import Session
 
-    from mypy_boto3_signer.client import signerClient
+    from mypy_boto3_signer.client import SignerClient
     from mypy_boto3_signer.waiter import (
         SuccessfulSigningJobWaiter,
     )
 
     session = Session()
-    client: signerClient = session.client("signer")
+    client: SignerClient = session.client("signer")
 
     successful_signing_job_waiter: SuccessfulSigningJobWaiter = client.get_waiter("successful_signing_job")
     ```
 """
 
 from botocore.waiter import Waiter
 
 from .type_defs import WaiterConfigTypeDef
 
 __all__ = ("SuccessfulSigningJobWaiter",)
 
 
 class SuccessfulSigningJobWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Waiter.SuccessfulSigningJob)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Waiter.SuccessfulSigningJob)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/waiters/#successfulsigningjobwaiter)
     """
 
     def wait(self, *, jobId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Waiter.SuccessfulSigningJob.wait)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Waiter.SuccessfulSigningJob.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/waiters/#successfulsigningjobwaiter)
         """
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer/waiter.pyi` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer/waiter.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/waiters/)
 
 Usage::
 
     ```python
     from boto3.session import Session
 
-    from mypy_boto3_signer.client import signerClient
+    from mypy_boto3_signer.client import SignerClient
     from mypy_boto3_signer.waiter import (
         SuccessfulSigningJobWaiter,
     )
 
     session = Session()
-    client: signerClient = session.client("signer")
+    client: SignerClient = session.client("signer")
 
     successful_signing_job_waiter: SuccessfulSigningJobWaiter = client.get_waiter("successful_signing_job")
     ```
 """
 
 from botocore.waiter import Waiter
 
 from .type_defs import WaiterConfigTypeDef
 
 __all__ = ("SuccessfulSigningJobWaiter",)
 
 class SuccessfulSigningJobWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Waiter.SuccessfulSigningJob)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Waiter.SuccessfulSigningJob)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/waiters/#successfulsigningjobwaiter)
     """
 
     def wait(self, *, jobId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Waiter.SuccessfulSigningJob.wait)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Waiter.SuccessfulSigningJob.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/waiters/#successfulsigningjobwaiter)
         """
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/PKG-INFO` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.34.0
-Summary: Type annotations for boto3.signer 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.95
+Summary: Type annotations for boto3.Signer 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
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
 
 <a id="mypy-boto3-signer"></a>
 
 # mypy-boto3-signer
 
 [![PyPI - mypy-boto3-signer](https://img.shields.io/pypi/v/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.Signer 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -98,21 +98,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `signer`.
+Click `Modify` and select `boto3 common` and `Signer`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `signer` service.
+Install `boto3-stubs` for `Signer` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[signer]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -257,44 +257,44 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`signerClient` provides annotations for `boto3.client("signer")`.
+`SignerClient` provides annotations for `boto3.client("signer")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="paginators-annotations"></a>
 
 ### Paginators annotations
 
 `mypy_boto3_signer.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 from mypy_boto3_signer.paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
 list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator(
     "list_signing_platforms"
 )
@@ -308,18 +308,18 @@
 ### Waiters annotations
 
 `mypy_boto3_signer.waiter` module contains type annotations for all waiters.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_signer import signerClient
+from mypy_boto3_signer import SignerClient
 from mypy_boto3_signer.waiter import SuccessfulSigningJobWaiter
 
-client: signerClient = Session().client("signer")
+client: SignerClient = Session().client("signer")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 successful_signing_job_waiter: SuccessfulSigningJobWaiter = client.get_waiter(
     "successful_signing_job"
 )
 ```
@@ -327,15 +327,15 @@
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_signer.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
-Full list of `signer` Literals can be found in
+Full list of `Signer` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/literals/).
 
 ```python
 from mypy_boto3_signer.literals import CategoryType
 
 
 def check_value(value: CategoryType) -> bool: ...
@@ -344,15 +344,15 @@
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
-Full list of `signer` TypeDefs can be found in
+Full list of `Signer` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/type_defs/).
 
 ```python
 from mypy_boto3_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
 
 def get_value() -> AddProfilePermissionRequestRequestTypeDef:
```

### Comparing `mypy-boto3-signer-1.34.0/mypy_boto3_signer.egg-info/SOURCES.txt` & `mypy_boto3_signer-1.34.95/mypy_boto3_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.34.0/setup.py` & `mypy_boto3_signer-1.34.95/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-signer",
-    version="1.34.0",
+    version="1.34.95",
     packages=["mypy_boto3_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.signer 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.Signer 1.34.95 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 signer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_signer": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

