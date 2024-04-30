# Comparing `tmp/mypy-boto3-codeartifact-1.34.0.tar.gz` & `tmp/mypy-boto3-codeartifact-1.34.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeartifact-1.34.0.tar", last modified: Wed Dec 13 21:22:13 2023, max compression
+gzip compressed data, was "mypy-boto3-codeartifact-1.34.68.tar", last modified: Thu Mar 21 19:19:26 2024, max compression
```

## Comparing `mypy-boto3-codeartifact-1.34.0.tar` & `mypy-boto3-codeartifact-1.34.68.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:13.407160 mypy-boto3-codeartifact-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:07:06.000000 mypy-boto3-codeartifact-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13674 2023-12-13 21:22:13.407160 mypy-boto3-codeartifact-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2023-12-13 21:07:06.000000 mypy-boto3-codeartifact-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:13.403160 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-12-13 21:07:06.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-13 21:07:06.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-13 21:07:06.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34376 2023-12-13 21:07:07.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34372 2023-12-13 21:07:07.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2023-12-13 21:07:08.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2023-12-13 21:07:07.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8649 2023-12-13 21:07:07.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2023-12-13 21:07:07.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:07:06.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35051 2023-12-13 21:07:08.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35050 2023-12-13 21:07:08.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:07:06.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:13.407160 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13674 2023-12-13 21:22:13.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 21:22:13.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:13.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:13.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:13.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 21:22:13.000000 mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:13.407160 mypy-boto3-codeartifact-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-13 21:07:06.000000 mypy-boto3-codeartifact-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:19:26.911617 mypy-boto3-codeartifact-1.34.68/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-03-21 19:19:26.911617 mypy-boto3-codeartifact-1.34.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:19:26.911617 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43919 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43916 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-03-21 19:19:16.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-03-21 19:19:16.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13748 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    46269 2024-03-21 19:19:16.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46269 2024-03-21 19:19:16.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 19:19:26.911617 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-03-21 19:19:26.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-21 19:19:26.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 19:19:26.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 19:19:26.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-21 19:19:26.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 19:19:26.000000 mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 19:19:26.911617 mypy-boto3-codeartifact-1.34.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-21 19:19:15.000000 mypy-boto3-codeartifact-1.34.68/setup.py
```

### Comparing `mypy-boto3-codeartifact-1.34.0/LICENSE` & `mypy-boto3-codeartifact-1.34.68/LICENSE`

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

### Comparing `mypy-boto3-codeartifact-1.34.0/PKG-INFO` & `mypy-boto3-codeartifact-1.34.68/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.34.0
-Summary: Type annotations for boto3.CodeArtifact 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.68
+Summary: Type annotations for boto3.CodeArtifact 1.34.68 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
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
 
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.34.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,38 +281,54 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_codeartifact import CodeArtifactClient
 from mypy_boto3_codeartifact.paginator import (
+    ListAllowedRepositoriesForGroupPaginator,
+    ListAssociatedPackagesPaginator,
     ListDomainsPaginator,
+    ListPackageGroupsPaginator,
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListPackagesPaginator,
     ListRepositoriesPaginator,
     ListRepositoriesInDomainPaginator,
+    ListSubPackageGroupsPaginator,
 )
 
 client: CodeArtifactClient = Session().client("codeartifact")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_allowed_repositories_for_group_paginator: ListAllowedRepositoriesForGroupPaginator = (
+    client.get_paginator("list_allowed_repositories_for_group")
+)
+list_associated_packages_paginator: ListAssociatedPackagesPaginator = client.get_paginator(
+    "list_associated_packages"
+)
 list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
+list_package_groups_paginator: ListPackageGroupsPaginator = client.get_paginator(
+    "list_package_groups"
+)
 list_package_version_assets_paginator: ListPackageVersionAssetsPaginator = client.get_paginator(
     "list_package_version_assets"
 )
 list_package_versions_paginator: ListPackageVersionsPaginator = client.get_paginator(
     "list_package_versions"
 )
 list_packages_paginator: ListPackagesPaginator = client.get_paginator("list_packages")
 list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
 list_repositories_in_domain_paginator: ListRepositoriesInDomainPaginator = client.get_paginator(
     "list_repositories_in_domain"
 )
+list_sub_package_groups_paginator: ListSubPackageGroupsPaginator = client.get_paginator(
+    "list_sub_package_groups"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_codeartifact.literals` module contains literals extracted from
```

### Comparing `mypy-boto3-codeartifact-1.34.0/README.md` & `mypy-boto3-codeartifact-1.34.68/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.34.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -248,38 +248,54 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_codeartifact import CodeArtifactClient
 from mypy_boto3_codeartifact.paginator import (
+    ListAllowedRepositoriesForGroupPaginator,
+    ListAssociatedPackagesPaginator,
     ListDomainsPaginator,
+    ListPackageGroupsPaginator,
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListPackagesPaginator,
     ListRepositoriesPaginator,
     ListRepositoriesInDomainPaginator,
+    ListSubPackageGroupsPaginator,
 )
 
 client: CodeArtifactClient = Session().client("codeartifact")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_allowed_repositories_for_group_paginator: ListAllowedRepositoriesForGroupPaginator = (
+    client.get_paginator("list_allowed_repositories_for_group")
+)
+list_associated_packages_paginator: ListAssociatedPackagesPaginator = client.get_paginator(
+    "list_associated_packages"
+)
 list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
+list_package_groups_paginator: ListPackageGroupsPaginator = client.get_paginator(
+    "list_package_groups"
+)
 list_package_version_assets_paginator: ListPackageVersionAssetsPaginator = client.get_paginator(
     "list_package_version_assets"
 )
 list_package_versions_paginator: ListPackageVersionsPaginator = client.get_paginator(
     "list_package_versions"
 )
 list_packages_paginator: ListPackagesPaginator = client.get_paginator("list_packages")
 list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
 list_repositories_in_domain_paginator: ListRepositoriesInDomainPaginator = client.get_paginator(
     "list_repositories_in_domain"
 )
+list_sub_package_groups_paginator: ListSubPackageGroupsPaginator = client.get_paginator(
+    "list_sub_package_groups"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_codeartifact.literals` module contains literals extracted from
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/__init__.py` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,50 +4,65 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_codeartifact import (
         Client,
         CodeArtifactClient,
+        ListAllowedRepositoriesForGroupPaginator,
+        ListAssociatedPackagesPaginator,
         ListDomainsPaginator,
+        ListPackageGroupsPaginator,
         ListPackageVersionAssetsPaginator,
         ListPackageVersionsPaginator,
         ListPackagesPaginator,
         ListRepositoriesInDomainPaginator,
         ListRepositoriesPaginator,
+        ListSubPackageGroupsPaginator,
     )
 
     session = Session()
     client: CodeArtifactClient = session.client("codeartifact")
 
+    list_allowed_repositories_for_group_paginator: ListAllowedRepositoriesForGroupPaginator = client.get_paginator("list_allowed_repositories_for_group")
+    list_associated_packages_paginator: ListAssociatedPackagesPaginator = client.get_paginator("list_associated_packages")
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
+    list_package_groups_paginator: ListPackageGroupsPaginator = client.get_paginator("list_package_groups")
     list_package_version_assets_paginator: ListPackageVersionAssetsPaginator = client.get_paginator("list_package_version_assets")
     list_package_versions_paginator: ListPackageVersionsPaginator = client.get_paginator("list_package_versions")
     list_packages_paginator: ListPackagesPaginator = client.get_paginator("list_packages")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
     list_repositories_in_domain_paginator: ListRepositoriesInDomainPaginator = client.get_paginator("list_repositories_in_domain")
+    list_sub_package_groups_paginator: ListSubPackageGroupsPaginator = client.get_paginator("list_sub_package_groups")
     ```
 """
 
 from .client import CodeArtifactClient
 from .paginator import (
+    ListAllowedRepositoriesForGroupPaginator,
+    ListAssociatedPackagesPaginator,
     ListDomainsPaginator,
+    ListPackageGroupsPaginator,
     ListPackagesPaginator,
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
+    ListSubPackageGroupsPaginator,
 )
 
 Client = CodeArtifactClient
 
-
 __all__ = (
     "Client",
     "CodeArtifactClient",
+    "ListAllowedRepositoriesForGroupPaginator",
+    "ListAssociatedPackagesPaginator",
     "ListDomainsPaginator",
+    "ListPackageGroupsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesInDomainPaginator",
     "ListRepositoriesPaginator",
+    "ListSubPackageGroupsPaginator",
 )
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/__init__.pyi` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -4,49 +4,65 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_codeartifact import (
         Client,
         CodeArtifactClient,
+        ListAllowedRepositoriesForGroupPaginator,
+        ListAssociatedPackagesPaginator,
         ListDomainsPaginator,
+        ListPackageGroupsPaginator,
         ListPackageVersionAssetsPaginator,
         ListPackageVersionsPaginator,
         ListPackagesPaginator,
         ListRepositoriesInDomainPaginator,
         ListRepositoriesPaginator,
+        ListSubPackageGroupsPaginator,
     )
 
     session = Session()
     client: CodeArtifactClient = session.client("codeartifact")
 
+    list_allowed_repositories_for_group_paginator: ListAllowedRepositoriesForGroupPaginator = client.get_paginator("list_allowed_repositories_for_group")
+    list_associated_packages_paginator: ListAssociatedPackagesPaginator = client.get_paginator("list_associated_packages")
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
+    list_package_groups_paginator: ListPackageGroupsPaginator = client.get_paginator("list_package_groups")
     list_package_version_assets_paginator: ListPackageVersionAssetsPaginator = client.get_paginator("list_package_version_assets")
     list_package_versions_paginator: ListPackageVersionsPaginator = client.get_paginator("list_package_versions")
     list_packages_paginator: ListPackagesPaginator = client.get_paginator("list_packages")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
     list_repositories_in_domain_paginator: ListRepositoriesInDomainPaginator = client.get_paginator("list_repositories_in_domain")
+    list_sub_package_groups_paginator: ListSubPackageGroupsPaginator = client.get_paginator("list_sub_package_groups")
     ```
 """
 
 from .client import CodeArtifactClient
 from .paginator import (
+    ListAllowedRepositoriesForGroupPaginator,
+    ListAssociatedPackagesPaginator,
     ListDomainsPaginator,
+    ListPackageGroupsPaginator,
     ListPackagesPaginator,
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
+    ListSubPackageGroupsPaginator,
 )
 
 Client = CodeArtifactClient
 
 __all__ = (
     "Client",
     "CodeArtifactClient",
+    "ListAllowedRepositoriesForGroupPaginator",
+    "ListAssociatedPackagesPaginator",
     "ListDomainsPaginator",
+    "ListPackageGroupsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesInDomainPaginator",
     "ListRepositoriesPaginator",
+    "ListSubPackageGroupsPaginator",
 )
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/__main__.py` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeArtifact 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.CodeArtifact 1.34.68\n"
+        "Version:         1.34.68\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.68")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/client.py` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,74 +19,90 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     PackageFormatType,
+    PackageGroupOriginRestrictionModeType,
+    PackageGroupOriginRestrictionTypeType,
     PackageVersionOriginTypeType,
     PackageVersionStatusType,
 )
 from .paginator import (
+    ListAllowedRepositoriesForGroupPaginator,
+    ListAssociatedPackagesPaginator,
     ListDomainsPaginator,
+    ListPackageGroupsPaginator,
     ListPackagesPaginator,
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
+    ListSubPackageGroupsPaginator,
 )
 from .type_defs import (
     AssociateExternalConnectionResultTypeDef,
     BlobTypeDef,
     CopyPackageVersionsResultTypeDef,
     CreateDomainResultTypeDef,
+    CreatePackageGroupResultTypeDef,
     CreateRepositoryResultTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteDomainResultTypeDef,
+    DeletePackageGroupResultTypeDef,
     DeletePackageResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     DeleteRepositoryResultTypeDef,
     DescribeDomainResultTypeDef,
+    DescribePackageGroupResultTypeDef,
     DescribePackageResultTypeDef,
     DescribePackageVersionResultTypeDef,
     DescribeRepositoryResultTypeDef,
     DisassociateExternalConnectionResultTypeDef,
     DisposePackageVersionsResultTypeDef,
+    GetAssociatedPackageGroupResultTypeDef,
     GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
+    ListAllowedRepositoriesForGroupResultTypeDef,
+    ListAssociatedPackagesResultTypeDef,
     ListDomainsResultTypeDef,
+    ListPackageGroupsResultTypeDef,
     ListPackagesResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListPackageVersionsResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListSubPackageGroupsResultTypeDef,
     ListTagsForResourceResultTypeDef,
+    PackageGroupAllowedRepositoryTypeDef,
     PackageOriginRestrictionsTypeDef,
     PublishPackageVersionResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutPackageOriginConfigurationResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     TagTypeDef,
+    UpdatePackageGroupOriginConfigurationResultTypeDef,
+    UpdatePackageGroupResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     UpdateRepositoryResultTypeDef,
     UpstreamRepositoryTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CodeArtifactClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -157,15 +173,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         versions: Sequence[str] = ...,
         versionRevisions: Mapping[str, str] = ...,
         allowOverwrite: bool = ...,
-        includeFromUpstream: bool = ...
+        includeFromUpstream: bool = ...,
     ) -> CopyPackageVersionsResultTypeDef:
         """
         Copies package versions from one repository to another repository in the same
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.copy_package_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#copy_package_versions)
@@ -177,23 +193,40 @@
         """
         Creates a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#create_domain)
         """
 
+    def create_package_group(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        contactInfo: str = ...,
+        description: str = ...,
+        tags: Sequence[TagTypeDef] = ...,
+    ) -> CreatePackageGroupResultTypeDef:
+        """
+        Creates a package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.create_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#create_package_group)
+        """
+
     def create_repository(
         self,
         *,
         domain: str,
         repository: str,
         domainOwner: str = ...,
         description: str = ...,
         upstreams: Sequence[UpstreamRepositoryTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryResultTypeDef:
         """
         Creates a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.create_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#create_repository)
         """
@@ -220,34 +253,44 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DeletePackageResultTypeDef:
         """
         Deletes a package and all associated package versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#delete_package)
         """
 
+    def delete_package_group(
+        self, *, domain: str, packageGroup: str, domainOwner: str = ...
+    ) -> DeletePackageGroupResultTypeDef:
+        """
+        Deletes a package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#delete_package_group)
+        """
+
     def delete_package_versions(
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         domainOwner: str = ...,
         namespace: str = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> DeletePackageVersionsResultTypeDef:
         """
         Deletes one or more versions of a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#delete_package_versions)
         """
@@ -289,36 +332,49 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DescribePackageResultTypeDef:
         """
         Returns a
         [PackageDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageDescription.html)
         object that contains information about the requested
         package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.describe_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#describe_package)
         """
 
+    def describe_package_group(
+        self, *, domain: str, packageGroup: str, domainOwner: str = ...
+    ) -> DescribePackageGroupResultTypeDef:
+        """
+        Returns a
+        [PackageGroupDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageGroupDescription.html)
+        object that contains information about the requested package
+        group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.describe_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#describe_package_group)
+        """
+
     def describe_package_version(
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DescribePackageVersionResultTypeDef:
         """
         Returns a
         [PackageVersionDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionDescription.html)
         object that contains information about the requested package
         version.
 
@@ -355,15 +411,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         domainOwner: str = ...,
         namespace: str = ...,
         versionRevisions: Mapping[str, str] = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> DisposePackageVersionsResultTypeDef:
         """
         Deletes the assets in package versions and sets the package versions' status to
         `Disposed`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.dispose_package_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#dispose_package_versions)
@@ -379,14 +435,30 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#generate_presigned_url)
         """
 
+    def get_associated_package_group(
+        self,
+        *,
+        domain: str,
+        format: PackageFormatType,
+        package: str,
+        domainOwner: str = ...,
+        namespace: str = ...,
+    ) -> GetAssociatedPackageGroupResultTypeDef:
+        """
+        Returns the most closely associated package group to the specified package.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_associated_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_associated_package_group)
+        """
+
     def get_authorization_token(
         self, *, domain: str, domainOwner: str = ..., durationSeconds: int = ...
     ) -> GetAuthorizationTokenResultTypeDef:
         """
         Generates a temporary authorization token for accessing repositories in the
         domain.
 
@@ -411,15 +483,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         asset: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        packageVersionRevision: str = ...
+        packageVersionRevision: str = ...,
     ) -> GetPackageVersionAssetResultTypeDef:
         """
         Returns an asset (or file) that is in a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_package_version_asset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_package_version_asset)
         """
@@ -429,15 +501,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> GetPackageVersionReadmeResultTypeDef:
         """
         Gets the readme file or descriptive text for a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_package_version_readme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_package_version_readme)
         """
@@ -458,40 +530,92 @@
         """
         Returns the resource policy that is set on a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_repository_permissions_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_repository_permissions_policy)
         """
 
+    def list_allowed_repositories_for_group(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        originRestrictionType: PackageGroupOriginRestrictionTypeType,
+        domainOwner: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+    ) -> ListAllowedRepositoriesForGroupResultTypeDef:
+        """
+        Lists the repositories in the added repositories list of the specified
+        restriction type for a package
+        group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_allowed_repositories_for_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_allowed_repositories_for_group)
+        """
+
+    def list_associated_packages(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        preview: bool = ...,
+    ) -> ListAssociatedPackagesResultTypeDef:
+        """
+        Returns a list of packages associated with the requested package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_associated_packages)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_associated_packages)
+        """
+
     def list_domains(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListDomainsResultTypeDef:
         """
         Returns a list of
         [DomainSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionDescription.html)
         objects for all domains owned by the Amazon Web Services account that makes
         this
         call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_domains)
         """
 
+    def list_package_groups(
+        self,
+        *,
+        domain: str,
+        domainOwner: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        prefix: str = ...,
+    ) -> ListPackageGroupsResultTypeDef:
+        """
+        Returns a list of package groups in the requested domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_package_groups)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_package_groups)
+        """
+
     def list_package_version_assets(
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionAssetsResultTypeDef:
         """
         Returns a list of
         [AssetSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_AssetSummary.html)
         objects for assets in a package
         version.
 
@@ -505,15 +629,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionDependenciesResultTypeDef:
         """
         Returns the direct dependencies for a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_package_version_dependencies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_package_version_dependencies)
         """
@@ -527,15 +651,15 @@
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        originType: PackageVersionOriginTypeType = ...
+        originType: PackageVersionOriginTypeType = ...,
     ) -> ListPackageVersionsResultTypeDef:
         """
         Returns a list of
         [PackageVersionSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionSummary.html)
         objects for package versions in a repository that match the request
         parameters.
 
@@ -551,15 +675,15 @@
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         publish: AllowPublishType = ...,
-        upstream: AllowUpstreamType = ...
+        upstream: AllowUpstreamType = ...,
     ) -> ListPackagesResultTypeDef:
         """
         Returns a list of
         [PackageSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageSummary.html)
         objects for packages in a repository that match the request
         parameters.
 
@@ -583,25 +707,41 @@
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRepositoriesInDomainResultTypeDef:
         """
         Returns a list of
         [RepositorySummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_RepositorySummary.html)
         objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_repositories_in_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_repositories_in_domain)
         """
 
+    def list_sub_package_groups(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+    ) -> ListSubPackageGroupsResultTypeDef:
+        """
+        Returns a list of direct children of the specified package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_sub_package_groups)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_sub_package_groups)
+        """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResultTypeDef:
         """
         Gets information about Amazon Web Services tags for a specified Amazon Resource
         Name (ARN) in
         CodeArtifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_tags_for_resource)
@@ -617,15 +757,15 @@
         package: str,
         packageVersion: str,
         assetContent: BlobTypeDef,
         assetName: str,
         assetSHA256: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        unfinished: bool = ...
+        unfinished: bool = ...,
     ) -> PublishPackageVersionResultTypeDef:
         """
         Creates a new package version containing one or more assets (or files).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.publish_package_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#publish_package_version)
         """
@@ -645,15 +785,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         restrictions: PackageOriginRestrictionsTypeDef,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> PutPackageOriginConfigurationResultTypeDef:
         """
         Sets the package origin configuration for a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.put_package_origin_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#put_package_origin_configuration)
         """
@@ -661,15 +801,15 @@
     def put_repository_permissions_policy(
         self,
         *,
         domain: str,
         repository: str,
         policyDocument: str,
         domainOwner: str = ...,
-        policyRevision: str = ...
+        policyRevision: str = ...,
     ) -> PutRepositoryPermissionsPolicyResultTypeDef:
         """
         Sets the resource policy on a repository that specifies permissions to access
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.put_repository_permissions_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#put_repository_permissions_policy)
@@ -687,27 +827,62 @@
         """
         Removes tags from a resource in CodeArtifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#untag_resource)
         """
 
+    def update_package_group(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        contactInfo: str = ...,
+        description: str = ...,
+    ) -> UpdatePackageGroupResultTypeDef:
+        """
+        Updates a package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#update_package_group)
+        """
+
+    def update_package_group_origin_configuration(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        restrictions: Mapping[
+            PackageGroupOriginRestrictionTypeType, PackageGroupOriginRestrictionModeType
+        ] = ...,
+        addAllowedRepositories: Sequence[PackageGroupAllowedRepositoryTypeDef] = ...,
+        removeAllowedRepositories: Sequence[PackageGroupAllowedRepositoryTypeDef] = ...,
+    ) -> UpdatePackageGroupOriginConfigurationResultTypeDef:
+        """
+        Updates the package origin configuration for a package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_package_group_origin_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#update_package_group_origin_configuration)
+        """
+
     def update_package_versions_status(
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         targetStatus: PackageVersionStatusType,
         domainOwner: str = ...,
         namespace: str = ...,
         versionRevisions: Mapping[str, str] = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> UpdatePackageVersionsStatusResultTypeDef:
         """
         Updates the status of one or more versions of a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_package_versions_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#update_package_versions_status)
         """
@@ -715,32 +890,59 @@
     def update_repository(
         self,
         *,
         domain: str,
         repository: str,
         domainOwner: str = ...,
         description: str = ...,
-        upstreams: Sequence[UpstreamRepositoryTypeDef] = ...
+        upstreams: Sequence[UpstreamRepositoryTypeDef] = ...,
     ) -> UpdateRepositoryResultTypeDef:
         """
         Update the properties of a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#update_repository)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_allowed_repositories_for_group"]
+    ) -> ListAllowedRepositoriesForGroupPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_associated_packages"]
+    ) -> ListAssociatedPackagesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_domains"]) -> ListDomainsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_package_groups"]
+    ) -> ListPackageGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_package_version_assets"]
     ) -> ListPackageVersionAssetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
         """
 
@@ -773,7 +975,16 @@
     def get_paginator(
         self, operation_name: Literal["list_repositories_in_domain"]
     ) -> ListRepositoriesInDomainPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_sub_package_groups"]
+    ) -> ListSubPackageGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/client.pyi` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -19,63 +19,80 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     PackageFormatType,
+    PackageGroupOriginRestrictionModeType,
+    PackageGroupOriginRestrictionTypeType,
     PackageVersionOriginTypeType,
     PackageVersionStatusType,
 )
 from .paginator import (
+    ListAllowedRepositoriesForGroupPaginator,
+    ListAssociatedPackagesPaginator,
     ListDomainsPaginator,
+    ListPackageGroupsPaginator,
     ListPackagesPaginator,
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
+    ListSubPackageGroupsPaginator,
 )
 from .type_defs import (
     AssociateExternalConnectionResultTypeDef,
     BlobTypeDef,
     CopyPackageVersionsResultTypeDef,
     CreateDomainResultTypeDef,
+    CreatePackageGroupResultTypeDef,
     CreateRepositoryResultTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteDomainResultTypeDef,
+    DeletePackageGroupResultTypeDef,
     DeletePackageResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     DeleteRepositoryResultTypeDef,
     DescribeDomainResultTypeDef,
+    DescribePackageGroupResultTypeDef,
     DescribePackageResultTypeDef,
     DescribePackageVersionResultTypeDef,
     DescribeRepositoryResultTypeDef,
     DisassociateExternalConnectionResultTypeDef,
     DisposePackageVersionsResultTypeDef,
+    GetAssociatedPackageGroupResultTypeDef,
     GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
+    ListAllowedRepositoriesForGroupResultTypeDef,
+    ListAssociatedPackagesResultTypeDef,
     ListDomainsResultTypeDef,
+    ListPackageGroupsResultTypeDef,
     ListPackagesResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListPackageVersionsResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListSubPackageGroupsResultTypeDef,
     ListTagsForResourceResultTypeDef,
+    PackageGroupAllowedRepositoryTypeDef,
     PackageOriginRestrictionsTypeDef,
     PublishPackageVersionResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutPackageOriginConfigurationResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     TagTypeDef,
+    UpdatePackageGroupOriginConfigurationResultTypeDef,
+    UpdatePackageGroupResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     UpdateRepositoryResultTypeDef,
     UpstreamRepositoryTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -153,15 +170,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         versions: Sequence[str] = ...,
         versionRevisions: Mapping[str, str] = ...,
         allowOverwrite: bool = ...,
-        includeFromUpstream: bool = ...
+        includeFromUpstream: bool = ...,
     ) -> CopyPackageVersionsResultTypeDef:
         """
         Copies package versions from one repository to another repository in the same
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.copy_package_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#copy_package_versions)
@@ -173,23 +190,40 @@
         """
         Creates a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#create_domain)
         """
 
+    def create_package_group(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        contactInfo: str = ...,
+        description: str = ...,
+        tags: Sequence[TagTypeDef] = ...,
+    ) -> CreatePackageGroupResultTypeDef:
+        """
+        Creates a package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.create_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#create_package_group)
+        """
+
     def create_repository(
         self,
         *,
         domain: str,
         repository: str,
         domainOwner: str = ...,
         description: str = ...,
         upstreams: Sequence[UpstreamRepositoryTypeDef] = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRepositoryResultTypeDef:
         """
         Creates a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.create_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#create_repository)
         """
@@ -216,34 +250,44 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DeletePackageResultTypeDef:
         """
         Deletes a package and all associated package versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#delete_package)
         """
 
+    def delete_package_group(
+        self, *, domain: str, packageGroup: str, domainOwner: str = ...
+    ) -> DeletePackageGroupResultTypeDef:
+        """
+        Deletes a package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#delete_package_group)
+        """
+
     def delete_package_versions(
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         domainOwner: str = ...,
         namespace: str = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> DeletePackageVersionsResultTypeDef:
         """
         Deletes one or more versions of a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.delete_package_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#delete_package_versions)
         """
@@ -285,36 +329,49 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DescribePackageResultTypeDef:
         """
         Returns a
         [PackageDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageDescription.html)
         object that contains information about the requested
         package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.describe_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#describe_package)
         """
 
+    def describe_package_group(
+        self, *, domain: str, packageGroup: str, domainOwner: str = ...
+    ) -> DescribePackageGroupResultTypeDef:
+        """
+        Returns a
+        [PackageGroupDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageGroupDescription.html)
+        object that contains information about the requested package
+        group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.describe_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#describe_package_group)
+        """
+
     def describe_package_version(
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> DescribePackageVersionResultTypeDef:
         """
         Returns a
         [PackageVersionDescription](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionDescription.html)
         object that contains information about the requested package
         version.
 
@@ -351,15 +408,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         domainOwner: str = ...,
         namespace: str = ...,
         versionRevisions: Mapping[str, str] = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> DisposePackageVersionsResultTypeDef:
         """
         Deletes the assets in package versions and sets the package versions' status to
         `Disposed`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.dispose_package_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#dispose_package_versions)
@@ -375,14 +432,30 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#generate_presigned_url)
         """
 
+    def get_associated_package_group(
+        self,
+        *,
+        domain: str,
+        format: PackageFormatType,
+        package: str,
+        domainOwner: str = ...,
+        namespace: str = ...,
+    ) -> GetAssociatedPackageGroupResultTypeDef:
+        """
+        Returns the most closely associated package group to the specified package.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_associated_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_associated_package_group)
+        """
+
     def get_authorization_token(
         self, *, domain: str, domainOwner: str = ..., durationSeconds: int = ...
     ) -> GetAuthorizationTokenResultTypeDef:
         """
         Generates a temporary authorization token for accessing repositories in the
         domain.
 
@@ -407,15 +480,15 @@
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         asset: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        packageVersionRevision: str = ...
+        packageVersionRevision: str = ...,
     ) -> GetPackageVersionAssetResultTypeDef:
         """
         Returns an asset (or file) that is in a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_package_version_asset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_package_version_asset)
         """
@@ -425,15 +498,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> GetPackageVersionReadmeResultTypeDef:
         """
         Gets the readme file or descriptive text for a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_package_version_readme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_package_version_readme)
         """
@@ -454,40 +527,92 @@
         """
         Returns the resource policy that is set on a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_repository_permissions_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_repository_permissions_policy)
         """
 
+    def list_allowed_repositories_for_group(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        originRestrictionType: PackageGroupOriginRestrictionTypeType,
+        domainOwner: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+    ) -> ListAllowedRepositoriesForGroupResultTypeDef:
+        """
+        Lists the repositories in the added repositories list of the specified
+        restriction type for a package
+        group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_allowed_repositories_for_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_allowed_repositories_for_group)
+        """
+
+    def list_associated_packages(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        preview: bool = ...,
+    ) -> ListAssociatedPackagesResultTypeDef:
+        """
+        Returns a list of packages associated with the requested package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_associated_packages)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_associated_packages)
+        """
+
     def list_domains(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListDomainsResultTypeDef:
         """
         Returns a list of
         [DomainSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionDescription.html)
         objects for all domains owned by the Amazon Web Services account that makes
         this
         call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_domains)
         """
 
+    def list_package_groups(
+        self,
+        *,
+        domain: str,
+        domainOwner: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        prefix: str = ...,
+    ) -> ListPackageGroupsResultTypeDef:
+        """
+        Returns a list of package groups in the requested domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_package_groups)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_package_groups)
+        """
+
     def list_package_version_assets(
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionAssetsResultTypeDef:
         """
         Returns a list of
         [AssetSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_AssetSummary.html)
         objects for assets in a package
         version.
 
@@ -501,15 +626,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListPackageVersionDependenciesResultTypeDef:
         """
         Returns the direct dependencies for a package version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_package_version_dependencies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_package_version_dependencies)
         """
@@ -523,15 +648,15 @@
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        originType: PackageVersionOriginTypeType = ...
+        originType: PackageVersionOriginTypeType = ...,
     ) -> ListPackageVersionsResultTypeDef:
         """
         Returns a list of
         [PackageVersionSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionSummary.html)
         objects for package versions in a repository that match the request
         parameters.
 
@@ -547,15 +672,15 @@
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         publish: AllowPublishType = ...,
-        upstream: AllowUpstreamType = ...
+        upstream: AllowUpstreamType = ...,
     ) -> ListPackagesResultTypeDef:
         """
         Returns a list of
         [PackageSummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageSummary.html)
         objects for packages in a repository that match the request
         parameters.
 
@@ -579,25 +704,41 @@
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRepositoriesInDomainResultTypeDef:
         """
         Returns a list of
         [RepositorySummary](https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_RepositorySummary.html)
         objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_repositories_in_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_repositories_in_domain)
         """
 
+    def list_sub_package_groups(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+    ) -> ListSubPackageGroupsResultTypeDef:
+        """
+        Returns a list of direct children of the specified package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_sub_package_groups)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#list_sub_package_groups)
+        """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResultTypeDef:
         """
         Gets information about Amazon Web Services tags for a specified Amazon Resource
         Name (ARN) in
         CodeArtifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.list_tags_for_resource)
@@ -613,15 +754,15 @@
         package: str,
         packageVersion: str,
         assetContent: BlobTypeDef,
         assetName: str,
         assetSHA256: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        unfinished: bool = ...
+        unfinished: bool = ...,
     ) -> PublishPackageVersionResultTypeDef:
         """
         Creates a new package version containing one or more assets (or files).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.publish_package_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#publish_package_version)
         """
@@ -641,15 +782,15 @@
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         restrictions: PackageOriginRestrictionsTypeDef,
         domainOwner: str = ...,
-        namespace: str = ...
+        namespace: str = ...,
     ) -> PutPackageOriginConfigurationResultTypeDef:
         """
         Sets the package origin configuration for a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.put_package_origin_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#put_package_origin_configuration)
         """
@@ -657,15 +798,15 @@
     def put_repository_permissions_policy(
         self,
         *,
         domain: str,
         repository: str,
         policyDocument: str,
         domainOwner: str = ...,
-        policyRevision: str = ...
+        policyRevision: str = ...,
     ) -> PutRepositoryPermissionsPolicyResultTypeDef:
         """
         Sets the resource policy on a repository that specifies permissions to access
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.put_repository_permissions_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#put_repository_permissions_policy)
@@ -683,27 +824,62 @@
         """
         Removes tags from a resource in CodeArtifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#untag_resource)
         """
 
+    def update_package_group(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        contactInfo: str = ...,
+        description: str = ...,
+    ) -> UpdatePackageGroupResultTypeDef:
+        """
+        Updates a package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_package_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#update_package_group)
+        """
+
+    def update_package_group_origin_configuration(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        restrictions: Mapping[
+            PackageGroupOriginRestrictionTypeType, PackageGroupOriginRestrictionModeType
+        ] = ...,
+        addAllowedRepositories: Sequence[PackageGroupAllowedRepositoryTypeDef] = ...,
+        removeAllowedRepositories: Sequence[PackageGroupAllowedRepositoryTypeDef] = ...,
+    ) -> UpdatePackageGroupOriginConfigurationResultTypeDef:
+        """
+        Updates the package origin configuration for a package group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_package_group_origin_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#update_package_group_origin_configuration)
+        """
+
     def update_package_versions_status(
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         versions: Sequence[str],
         targetStatus: PackageVersionStatusType,
         domainOwner: str = ...,
         namespace: str = ...,
         versionRevisions: Mapping[str, str] = ...,
-        expectedStatus: PackageVersionStatusType = ...
+        expectedStatus: PackageVersionStatusType = ...,
     ) -> UpdatePackageVersionsStatusResultTypeDef:
         """
         Updates the status of one or more versions of a package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_package_versions_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#update_package_versions_status)
         """
@@ -711,32 +887,59 @@
     def update_repository(
         self,
         *,
         domain: str,
         repository: str,
         domainOwner: str = ...,
         description: str = ...,
-        upstreams: Sequence[UpstreamRepositoryTypeDef] = ...
+        upstreams: Sequence[UpstreamRepositoryTypeDef] = ...,
     ) -> UpdateRepositoryResultTypeDef:
         """
         Update the properties of a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.update_repository)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#update_repository)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_allowed_repositories_for_group"]
+    ) -> ListAllowedRepositoriesForGroupPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_associated_packages"]
+    ) -> ListAssociatedPackagesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_domains"]) -> ListDomainsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_package_groups"]
+    ) -> ListPackageGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_package_version_assets"]
     ) -> ListPackageVersionAssetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
         """
 
@@ -769,7 +972,16 @@
     def get_paginator(
         self, operation_name: Literal["list_repositories_in_domain"]
     ) -> ListRepositoriesInDomainPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_sub_package_groups"]
+    ) -> ListSubPackageGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/literals.py` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/literals.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,52 +15,68 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AllowPublishType",
     "AllowUpstreamType",
     "DomainStatusType",
     "ExternalConnectionStatusType",
     "HashAlgorithmType",
+    "ListAllowedRepositoriesForGroupPaginatorName",
+    "ListAssociatedPackagesPaginatorName",
     "ListDomainsPaginatorName",
+    "ListPackageGroupsPaginatorName",
     "ListPackageVersionAssetsPaginatorName",
     "ListPackageVersionsPaginatorName",
     "ListPackagesPaginatorName",
     "ListRepositoriesInDomainPaginatorName",
     "ListRepositoriesPaginatorName",
+    "ListSubPackageGroupsPaginatorName",
     "PackageFormatType",
+    "PackageGroupAllowedRepositoryUpdateTypeType",
+    "PackageGroupAssociationTypeType",
+    "PackageGroupOriginRestrictionModeType",
+    "PackageGroupOriginRestrictionTypeType",
     "PackageVersionErrorCodeType",
     "PackageVersionOriginTypeType",
     "PackageVersionSortTypeType",
     "PackageVersionStatusType",
     "CodeArtifactServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AllowPublishType = Literal["ALLOW", "BLOCK"]
 AllowUpstreamType = Literal["ALLOW", "BLOCK"]
 DomainStatusType = Literal["Active", "Deleted"]
 ExternalConnectionStatusType = Literal["Available"]
 HashAlgorithmType = Literal["MD5", "SHA-1", "SHA-256", "SHA-512"]
+ListAllowedRepositoriesForGroupPaginatorName = Literal["list_allowed_repositories_for_group"]
+ListAssociatedPackagesPaginatorName = Literal["list_associated_packages"]
 ListDomainsPaginatorName = Literal["list_domains"]
+ListPackageGroupsPaginatorName = Literal["list_package_groups"]
 ListPackageVersionAssetsPaginatorName = Literal["list_package_version_assets"]
 ListPackageVersionsPaginatorName = Literal["list_package_versions"]
 ListPackagesPaginatorName = Literal["list_packages"]
 ListRepositoriesInDomainPaginatorName = Literal["list_repositories_in_domain"]
 ListRepositoriesPaginatorName = Literal["list_repositories"]
+ListSubPackageGroupsPaginatorName = Literal["list_sub_package_groups"]
 PackageFormatType = Literal["generic", "maven", "npm", "nuget", "pypi", "swift"]
+PackageGroupAllowedRepositoryUpdateTypeType = Literal["ADDED", "REMOVED"]
+PackageGroupAssociationTypeType = Literal["STRONG", "WEAK"]
+PackageGroupOriginRestrictionModeType = Literal[
+    "ALLOW", "ALLOW_SPECIFIC_REPOSITORIES", "BLOCK", "INHERIT"
+]
+PackageGroupOriginRestrictionTypeType = Literal["EXTERNAL_UPSTREAM", "INTERNAL_UPSTREAM", "PUBLISH"]
 PackageVersionErrorCodeType = Literal[
     "ALREADY_EXISTS",
     "MISMATCHED_REVISION",
     "MISMATCHED_STATUS",
     "NOT_ALLOWED",
     "NOT_FOUND",
     "SKIPPED",
@@ -93,14 +109,15 @@
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
@@ -111,14 +128,15 @@
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
@@ -234,15 +252,14 @@
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
@@ -314,17 +331,19 @@
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
@@ -414,19 +433,21 @@
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
@@ -456,20 +477,24 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
+    "list_allowed_repositories_for_group",
+    "list_associated_packages",
     "list_domains",
+    "list_package_groups",
     "list_package_version_assets",
     "list_package_versions",
     "list_packages",
     "list_repositories",
     "list_repositories_in_domain",
+    "list_sub_package_groups",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/literals.pyi` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/literals.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -21,21 +21,29 @@
 
 __all__ = (
     "AllowPublishType",
     "AllowUpstreamType",
     "DomainStatusType",
     "ExternalConnectionStatusType",
     "HashAlgorithmType",
+    "ListAllowedRepositoriesForGroupPaginatorName",
+    "ListAssociatedPackagesPaginatorName",
     "ListDomainsPaginatorName",
+    "ListPackageGroupsPaginatorName",
     "ListPackageVersionAssetsPaginatorName",
     "ListPackageVersionsPaginatorName",
     "ListPackagesPaginatorName",
     "ListRepositoriesInDomainPaginatorName",
     "ListRepositoriesPaginatorName",
+    "ListSubPackageGroupsPaginatorName",
     "PackageFormatType",
+    "PackageGroupAllowedRepositoryUpdateTypeType",
+    "PackageGroupAssociationTypeType",
+    "PackageGroupOriginRestrictionModeType",
+    "PackageGroupOriginRestrictionTypeType",
     "PackageVersionErrorCodeType",
     "PackageVersionOriginTypeType",
     "PackageVersionSortTypeType",
     "PackageVersionStatusType",
     "CodeArtifactServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -44,21 +52,31 @@
 )
 
 AllowPublishType = Literal["ALLOW", "BLOCK"]
 AllowUpstreamType = Literal["ALLOW", "BLOCK"]
 DomainStatusType = Literal["Active", "Deleted"]
 ExternalConnectionStatusType = Literal["Available"]
 HashAlgorithmType = Literal["MD5", "SHA-1", "SHA-256", "SHA-512"]
+ListAllowedRepositoriesForGroupPaginatorName = Literal["list_allowed_repositories_for_group"]
+ListAssociatedPackagesPaginatorName = Literal["list_associated_packages"]
 ListDomainsPaginatorName = Literal["list_domains"]
+ListPackageGroupsPaginatorName = Literal["list_package_groups"]
 ListPackageVersionAssetsPaginatorName = Literal["list_package_version_assets"]
 ListPackageVersionsPaginatorName = Literal["list_package_versions"]
 ListPackagesPaginatorName = Literal["list_packages"]
 ListRepositoriesInDomainPaginatorName = Literal["list_repositories_in_domain"]
 ListRepositoriesPaginatorName = Literal["list_repositories"]
+ListSubPackageGroupsPaginatorName = Literal["list_sub_package_groups"]
 PackageFormatType = Literal["generic", "maven", "npm", "nuget", "pypi", "swift"]
+PackageGroupAllowedRepositoryUpdateTypeType = Literal["ADDED", "REMOVED"]
+PackageGroupAssociationTypeType = Literal["STRONG", "WEAK"]
+PackageGroupOriginRestrictionModeType = Literal[
+    "ALLOW", "ALLOW_SPECIFIC_REPOSITORIES", "BLOCK", "INHERIT"
+]
+PackageGroupOriginRestrictionTypeType = Literal["EXTERNAL_UPSTREAM", "INTERNAL_UPSTREAM", "PUBLISH"]
 PackageVersionErrorCodeType = Literal[
     "ALREADY_EXISTS",
     "MISMATCHED_REVISION",
     "MISMATCHED_STATUS",
     "NOT_ALLOWED",
     "NOT_FOUND",
     "SKIPPED",
@@ -91,14 +109,15 @@
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
@@ -109,14 +128,15 @@
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
@@ -232,15 +252,14 @@
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
@@ -312,17 +331,19 @@
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
@@ -412,19 +433,21 @@
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
@@ -454,20 +477,24 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
+    "list_allowed_repositories_for_group",
+    "list_associated_packages",
     "list_domains",
+    "list_package_groups",
     "list_package_version_assets",
     "list_package_versions",
     "list_packages",
     "list_repositories",
     "list_repositories_in_domain",
+    "list_sub_package_groups",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/paginator.py` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/paginator.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,82 +6,139 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_codeartifact.client import CodeArtifactClient
     from mypy_boto3_codeartifact.paginator import (
+        ListAllowedRepositoriesForGroupPaginator,
+        ListAssociatedPackagesPaginator,
         ListDomainsPaginator,
+        ListPackageGroupsPaginator,
         ListPackageVersionAssetsPaginator,
         ListPackageVersionsPaginator,
         ListPackagesPaginator,
         ListRepositoriesPaginator,
         ListRepositoriesInDomainPaginator,
+        ListSubPackageGroupsPaginator,
     )
 
     session = Session()
     client: CodeArtifactClient = session.client("codeartifact")
 
+    list_allowed_repositories_for_group_paginator: ListAllowedRepositoriesForGroupPaginator = client.get_paginator("list_allowed_repositories_for_group")
+    list_associated_packages_paginator: ListAssociatedPackagesPaginator = client.get_paginator("list_associated_packages")
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
+    list_package_groups_paginator: ListPackageGroupsPaginator = client.get_paginator("list_package_groups")
     list_package_version_assets_paginator: ListPackageVersionAssetsPaginator = client.get_paginator("list_package_version_assets")
     list_package_versions_paginator: ListPackageVersionsPaginator = client.get_paginator("list_package_versions")
     list_packages_paginator: ListPackagesPaginator = client.get_paginator("list_packages")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
     list_repositories_in_domain_paginator: ListRepositoriesInDomainPaginator = client.get_paginator("list_repositories_in_domain")
+    list_sub_package_groups_paginator: ListSubPackageGroupsPaginator = client.get_paginator("list_sub_package_groups")
     ```
 """
 
 import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     PackageFormatType,
+    PackageGroupOriginRestrictionTypeType,
     PackageVersionOriginTypeType,
     PackageVersionStatusType,
 )
 from .type_defs import (
+    ListAllowedRepositoriesForGroupResultTypeDef,
+    ListAssociatedPackagesResultTypeDef,
     ListDomainsResultTypeDef,
+    ListPackageGroupsResultTypeDef,
     ListPackagesResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     ListPackageVersionsResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListSubPackageGroupsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "ListAllowedRepositoriesForGroupPaginator",
+    "ListAssociatedPackagesPaginator",
     "ListDomainsPaginator",
+    "ListPackageGroupsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesPaginator",
     "ListRepositoriesInDomainPaginator",
+    "ListSubPackageGroupsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
 
+class ListAllowedRepositoriesForGroupPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListAllowedRepositoriesForGroup)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listallowedrepositoriesforgrouppaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        originRestrictionType: PackageGroupOriginRestrictionTypeType,
+        domainOwner: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListAllowedRepositoriesForGroupResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListAllowedRepositoriesForGroup.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listallowedrepositoriesforgrouppaginator)
+        """
+
+
+class ListAssociatedPackagesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListAssociatedPackages)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listassociatedpackagespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        preview: bool = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListAssociatedPackagesResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListAssociatedPackages.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listassociatedpackagespaginator)
+        """
+
+
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
     """
 
     def paginate(
@@ -89,14 +146,34 @@
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
         """
 
 
+class ListPackageGroupsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageGroups)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagegroupspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domain: str,
+        domainOwner: str = ...,
+        prefix: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListPackageGroupsResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageGroups.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagegroupspaginator)
+        """
+
+
 class ListPackageVersionAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
     """
 
     def paginate(
@@ -105,15 +182,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
 
@@ -131,15 +208,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionspaginator)
         """
 
 
@@ -156,15 +233,15 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagespaginator)
         """
 
 
@@ -192,13 +269,33 @@
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
+
+
+class ListSubPackageGroupsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListSubPackageGroups)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listsubpackagegroupspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListSubPackageGroupsResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListSubPackageGroups.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listsubpackagegroupspaginator)
+        """
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/paginator.pyi` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/paginator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -6,92 +6,168 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_codeartifact.client import CodeArtifactClient
     from mypy_boto3_codeartifact.paginator import (
+        ListAllowedRepositoriesForGroupPaginator,
+        ListAssociatedPackagesPaginator,
         ListDomainsPaginator,
+        ListPackageGroupsPaginator,
         ListPackageVersionAssetsPaginator,
         ListPackageVersionsPaginator,
         ListPackagesPaginator,
         ListRepositoriesPaginator,
         ListRepositoriesInDomainPaginator,
+        ListSubPackageGroupsPaginator,
     )
 
     session = Session()
     client: CodeArtifactClient = session.client("codeartifact")
 
+    list_allowed_repositories_for_group_paginator: ListAllowedRepositoriesForGroupPaginator = client.get_paginator("list_allowed_repositories_for_group")
+    list_associated_packages_paginator: ListAssociatedPackagesPaginator = client.get_paginator("list_associated_packages")
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
+    list_package_groups_paginator: ListPackageGroupsPaginator = client.get_paginator("list_package_groups")
     list_package_version_assets_paginator: ListPackageVersionAssetsPaginator = client.get_paginator("list_package_version_assets")
     list_package_versions_paginator: ListPackageVersionsPaginator = client.get_paginator("list_package_versions")
     list_packages_paginator: ListPackagesPaginator = client.get_paginator("list_packages")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
     list_repositories_in_domain_paginator: ListRepositoriesInDomainPaginator = client.get_paginator("list_repositories_in_domain")
+    list_sub_package_groups_paginator: ListSubPackageGroupsPaginator = client.get_paginator("list_sub_package_groups")
     ```
 """
 
 import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     PackageFormatType,
+    PackageGroupOriginRestrictionTypeType,
     PackageVersionOriginTypeType,
     PackageVersionStatusType,
 )
 from .type_defs import (
+    ListAllowedRepositoriesForGroupResultTypeDef,
+    ListAssociatedPackagesResultTypeDef,
     ListDomainsResultTypeDef,
+    ListPackageGroupsResultTypeDef,
     ListPackagesResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     ListPackageVersionsResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListSubPackageGroupsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ListAllowedRepositoriesForGroupPaginator",
+    "ListAssociatedPackagesPaginator",
     "ListDomainsPaginator",
+    "ListPackageGroupsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesPaginator",
     "ListRepositoriesInDomainPaginator",
+    "ListSubPackageGroupsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+class ListAllowedRepositoriesForGroupPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListAllowedRepositoriesForGroup)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listallowedrepositoriesforgrouppaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        originRestrictionType: PackageGroupOriginRestrictionTypeType,
+        domainOwner: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListAllowedRepositoriesForGroupResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListAllowedRepositoriesForGroup.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listallowedrepositoriesforgrouppaginator)
+        """
+
+class ListAssociatedPackagesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListAssociatedPackages)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listassociatedpackagespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        preview: bool = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListAssociatedPackagesResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListAssociatedPackages.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listassociatedpackagespaginator)
+        """
+
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
         """
 
+class ListPackageGroupsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageGroups)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagegroupspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domain: str,
+        domainOwner: str = ...,
+        prefix: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListPackageGroupsResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageGroups.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagegroupspaginator)
+        """
+
 class ListPackageVersionAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
     """
 
     def paginate(
@@ -100,15 +176,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
 class ListPackageVersionsPaginator(Paginator):
@@ -125,15 +201,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionspaginator)
         """
 
 class ListPackagesPaginator(Paginator):
@@ -149,15 +225,15 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagespaginator)
         """
 
 class ListRepositoriesPaginator(Paginator):
@@ -183,13 +259,32 @@
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
+
+class ListSubPackageGroupsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListSubPackageGroups)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listsubpackagegroupspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domain: str,
+        packageGroup: str,
+        domainOwner: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListSubPackageGroupsResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListSubPackageGroups.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listsubpackagegroupspaginator)
+        """
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/type_defs.py` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     DomainStatusType,
     HashAlgorithmType,
     PackageFormatType,
+    PackageGroupAllowedRepositoryUpdateTypeType,
+    PackageGroupAssociationTypeType,
+    PackageGroupOriginRestrictionModeType,
+    PackageGroupOriginRestrictionTypeType,
     PackageVersionErrorCodeType,
     PackageVersionOriginTypeType,
     PackageVersionStatusType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -38,78 +42,91 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "AssociatedPackageTypeDef",
     "BlobTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeletePackageGroupRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeletePackageVersionsRequestRequestTypeDef",
     "DeleteRepositoryPermissionsPolicyRequestRequestTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "DescribeDomainRequestRequestTypeDef",
+    "DescribePackageGroupRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
     "DescribeRepositoryRequestRequestTypeDef",
     "DisassociateExternalConnectionRequestRequestTypeDef",
     "DisposePackageVersionsRequestRequestTypeDef",
     "DomainEntryPointTypeDef",
     "DomainSummaryTypeDef",
+    "GetAssociatedPackageGroupRequestRequestTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDomainPermissionsPolicyRequestRequestTypeDef",
     "GetPackageVersionAssetRequestRequestTypeDef",
     "GetPackageVersionReadmeRequestRequestTypeDef",
     "GetRepositoryEndpointRequestRequestTypeDef",
     "GetRepositoryPermissionsPolicyRequestRequestTypeDef",
     "LicenseInfoTypeDef",
     "PaginatorConfigTypeDef",
+    "ListAllowedRepositoriesForGroupRequestRequestTypeDef",
+    "ListAssociatedPackagesRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListPackageGroupsRequestRequestTypeDef",
     "ListPackageVersionAssetsRequestRequestTypeDef",
     "ListPackageVersionDependenciesRequestRequestTypeDef",
     "PackageDependencyTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
+    "ListSubPackageGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PackageGroupAllowedRepositoryTypeDef",
+    "PackageGroupReferenceTypeDef",
     "PackageOriginRestrictionsTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdatePackageGroupRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
     "GetAuthorizationTokenResultTypeDef",
     "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointResultTypeDef",
+    "ListAllowedRepositoriesForGroupResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
+    "ListAssociatedPackagesResultTypeDef",
     "PublishPackageVersionRequestRequestTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
+    "CreatePackageGroupRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainResultTypeDef",
     "DeleteDomainResultTypeDef",
     "DescribeDomainResultTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "UpdateRepositoryRequestRequestTypeDef",
@@ -117,42 +134,59 @@
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     "GetDomainPermissionsPolicyResultTypeDef",
     "GetRepositoryPermissionsPolicyResultTypeDef",
     "PutDomainPermissionsPolicyResultTypeDef",
     "PutRepositoryPermissionsPolicyResultTypeDef",
     "PackageVersionOriginTypeDef",
     "ListDomainsResultTypeDef",
+    "ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef",
+    "ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListPackageGroupsRequestListPackageGroupsPaginateTypeDef",
     "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
+    "ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
+    "UpdatePackageGroupOriginConfigurationRequestRequestTypeDef",
+    "PackageGroupOriginRestrictionTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
     "PackageVersionSummaryTypeDef",
+    "PackageGroupOriginConfigurationTypeDef",
     "PackageDescriptionTypeDef",
     "PackageSummaryTypeDef",
     "PutPackageOriginConfigurationResultTypeDef",
     "AssociateExternalConnectionResultTypeDef",
     "CreateRepositoryResultTypeDef",
     "DeleteRepositoryResultTypeDef",
     "DescribeRepositoryResultTypeDef",
     "DisassociateExternalConnectionResultTypeDef",
     "UpdateRepositoryResultTypeDef",
     "DescribePackageVersionResultTypeDef",
     "ListPackageVersionsResultTypeDef",
+    "PackageGroupDescriptionTypeDef",
+    "PackageGroupSummaryTypeDef",
     "DescribePackageResultTypeDef",
     "DeletePackageResultTypeDef",
     "ListPackagesResultTypeDef",
+    "CreatePackageGroupResultTypeDef",
+    "DeletePackageGroupResultTypeDef",
+    "DescribePackageGroupResultTypeDef",
+    "GetAssociatedPackageGroupResultTypeDef",
+    "UpdatePackageGroupOriginConfigurationResultTypeDef",
+    "UpdatePackageGroupResultTypeDef",
+    "ListPackageGroupsResultTypeDef",
+    "ListSubPackageGroupsResultTypeDef",
 )
 
 AssetSummaryTypeDef = TypedDict(
     "AssetSummaryTypeDef",
     {
         "name": str,
         "size": NotRequired[int],
@@ -168,18 +202,27 @@
         "domainOwner": NotRequired[str],
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
+AssociatedPackageTypeDef = TypedDict(
+    "AssociatedPackageTypeDef",
+    {
+        "format": NotRequired[PackageFormatType],
+        "namespace": NotRequired[str],
+        "package": NotRequired[str],
+        "associationType": NotRequired[PackageGroupAssociationTypeType],
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "CopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
@@ -255,14 +298,22 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domain": str,
         "domainOwner": NotRequired[str],
     },
 )
+DeletePackageGroupRequestRequestTypeDef = TypedDict(
+    "DeletePackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+    },
+)
 DeletePackageRequestRequestTypeDef = TypedDict(
     "DeletePackageRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -303,14 +354,22 @@
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "domain": str,
         "domainOwner": NotRequired[str],
     },
 )
+DescribePackageGroupRequestRequestTypeDef = TypedDict(
+    "DescribePackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+    },
+)
 DescribePackageRequestRequestTypeDef = TypedDict(
     "DescribePackageRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -375,14 +434,24 @@
         "owner": NotRequired[str],
         "arn": NotRequired[str],
         "status": NotRequired[DomainStatusType],
         "createdTime": NotRequired[datetime],
         "encryptionKey": NotRequired[str],
     },
 )
+GetAssociatedPackageGroupRequestRequestTypeDef = TypedDict(
+    "GetAssociatedPackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "format": PackageFormatType,
+        "package": str,
+        "domainOwner": NotRequired[str],
+        "namespace": NotRequired[str],
+    },
+)
 GetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "GetAuthorizationTokenRequestRequestTypeDef",
     {
         "domain": str,
         "domainOwner": NotRequired[str],
         "durationSeconds": NotRequired[int],
     },
@@ -448,21 +517,53 @@
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
 )
+ListAllowedRepositoriesForGroupRequestRequestTypeDef = TypedDict(
+    "ListAllowedRepositoriesForGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "originRestrictionType": PackageGroupOriginRestrictionTypeType,
+        "domainOwner": NotRequired[str],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
+ListAssociatedPackagesRequestRequestTypeDef = TypedDict(
+    "ListAssociatedPackagesRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+        "preview": NotRequired[bool],
+    },
+)
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListPackageGroupsRequestRequestTypeDef = TypedDict(
+    "ListPackageGroupsRequestRequestTypeDef",
+    {
+        "domain": str,
+        "domainOwner": NotRequired[str],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+        "prefix": NotRequired[str],
+    },
+)
 ListPackageVersionAssetsRequestRequestTypeDef = TypedDict(
     "ListPackageVersionAssetsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -553,20 +654,44 @@
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": NotRequired[str],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListSubPackageGroupsRequestRequestTypeDef = TypedDict(
+    "ListSubPackageGroupsRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
+PackageGroupAllowedRepositoryTypeDef = TypedDict(
+    "PackageGroupAllowedRepositoryTypeDef",
+    {
+        "repositoryName": NotRequired[str],
+        "originRestrictionType": NotRequired[PackageGroupOriginRestrictionTypeType],
+    },
+)
+PackageGroupReferenceTypeDef = TypedDict(
+    "PackageGroupReferenceTypeDef",
+    {
+        "arn": NotRequired[str],
+        "pattern": NotRequired[str],
+    },
+)
 PackageOriginRestrictionsTypeDef = TypedDict(
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
 )
@@ -606,14 +731,24 @@
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
+UpdatePackageGroupRequestRequestTypeDef = TypedDict(
+    "UpdatePackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "contactInfo": NotRequired[str],
+        "description": NotRequired[str],
+    },
+)
 UpdatePackageVersionsStatusRequestRequestTypeDef = TypedDict(
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -658,14 +793,22 @@
 GetRepositoryEndpointResultTypeDef = TypedDict(
     "GetRepositoryEndpointResultTypeDef",
     {
         "repositoryEndpoint": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAllowedRepositoriesForGroupResultTypeDef = TypedDict(
+    "ListAllowedRepositoriesForGroupResultTypeDef",
+    {
+        "allowedRepositories": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListPackageVersionAssetsResultTypeDef = TypedDict(
     "ListPackageVersionAssetsResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
@@ -684,14 +827,22 @@
         "version": str,
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAssociatedPackagesResultTypeDef = TypedDict(
+    "ListAssociatedPackagesResultTypeDef",
+    {
+        "packages": List[AssociatedPackageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 PublishPackageVersionRequestRequestTypeDef = TypedDict(
     "PublishPackageVersionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -740,14 +891,25 @@
     "CreateDomainRequestRequestTypeDef",
     {
         "domain": str,
         "encryptionKey": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+CreatePackageGroupRequestRequestTypeDef = TypedDict(
+    "CreatePackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "contactInfo": NotRequired[str],
+        "description": NotRequired[str],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -853,20 +1015,49 @@
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef = TypedDict(
+    "ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "originRestrictionType": PackageGroupOriginRestrictionTypeType,
+        "domainOwner": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef = TypedDict(
+    "ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "preview": NotRequired[bool],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListPackageGroupsRequestListPackageGroupsPaginateTypeDef = TypedDict(
+    "ListPackageGroupsRequestListPackageGroupsPaginateTypeDef",
+    {
+        "domain": str,
+        "domainOwner": NotRequired[str],
+        "prefix": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
     "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -918,14 +1109,23 @@
 ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
     "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     {
         "repositoryPrefix": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef = TypedDict(
+    "ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListPackageVersionDependenciesResultTypeDef = TypedDict(
     "ListPackageVersionDependenciesResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
@@ -947,14 +1147,36 @@
     "ListRepositoriesResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdatePackageGroupOriginConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdatePackageGroupOriginConfigurationRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "restrictions": NotRequired[
+            Mapping[PackageGroupOriginRestrictionTypeType, PackageGroupOriginRestrictionModeType]
+        ],
+        "addAllowedRepositories": NotRequired[Sequence[PackageGroupAllowedRepositoryTypeDef]],
+        "removeAllowedRepositories": NotRequired[Sequence[PackageGroupAllowedRepositoryTypeDef]],
+    },
+)
+PackageGroupOriginRestrictionTypeDef = TypedDict(
+    "PackageGroupOriginRestrictionTypeDef",
+    {
+        "mode": NotRequired[PackageGroupOriginRestrictionModeType],
+        "effectiveMode": NotRequired[PackageGroupOriginRestrictionModeType],
+        "inheritedFrom": NotRequired[PackageGroupReferenceTypeDef],
+        "repositoriesCount": NotRequired[int],
+    },
+)
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
         "restrictions": NotRequired[PackageOriginRestrictionsTypeDef],
     },
 )
 PutPackageOriginConfigurationRequestRequestTypeDef = TypedDict(
@@ -1006,14 +1228,22 @@
     {
         "version": str,
         "status": PackageVersionStatusType,
         "revision": NotRequired[str],
         "origin": NotRequired[PackageVersionOriginTypeDef],
     },
 )
+PackageGroupOriginConfigurationTypeDef = TypedDict(
+    "PackageGroupOriginConfigurationTypeDef",
+    {
+        "restrictions": NotRequired[
+            Dict[PackageGroupOriginRestrictionTypeType, PackageGroupOriginRestrictionTypeDef]
+        ],
+    },
+)
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": NotRequired[PackageFormatType],
         "namespace": NotRequired[str],
         "name": NotRequired[str],
         "originConfiguration": NotRequired[PackageOriginConfigurationTypeDef],
@@ -1092,14 +1322,42 @@
         "namespace": str,
         "package": str,
         "versions": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+PackageGroupDescriptionTypeDef = TypedDict(
+    "PackageGroupDescriptionTypeDef",
+    {
+        "arn": NotRequired[str],
+        "pattern": NotRequired[str],
+        "domainName": NotRequired[str],
+        "domainOwner": NotRequired[str],
+        "createdTime": NotRequired[datetime],
+        "contactInfo": NotRequired[str],
+        "description": NotRequired[str],
+        "originConfiguration": NotRequired[PackageGroupOriginConfigurationTypeDef],
+        "parent": NotRequired[PackageGroupReferenceTypeDef],
+    },
+)
+PackageGroupSummaryTypeDef = TypedDict(
+    "PackageGroupSummaryTypeDef",
+    {
+        "arn": NotRequired[str],
+        "pattern": NotRequired[str],
+        "domainName": NotRequired[str],
+        "domainOwner": NotRequired[str],
+        "createdTime": NotRequired[datetime],
+        "contactInfo": NotRequired[str],
+        "description": NotRequired[str],
+        "originConfiguration": NotRequired[PackageGroupOriginConfigurationTypeDef],
+        "parent": NotRequired[PackageGroupReferenceTypeDef],
+    },
+)
 DescribePackageResultTypeDef = TypedDict(
     "DescribePackageResultTypeDef",
     {
         "package": PackageDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1114,7 +1372,70 @@
     "ListPackagesResultTypeDef",
     {
         "packages": List[PackageSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreatePackageGroupResultTypeDef = TypedDict(
+    "CreatePackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DeletePackageGroupResultTypeDef = TypedDict(
+    "DeletePackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribePackageGroupResultTypeDef = TypedDict(
+    "DescribePackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetAssociatedPackageGroupResultTypeDef = TypedDict(
+    "GetAssociatedPackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "associationType": PackageGroupAssociationTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdatePackageGroupOriginConfigurationResultTypeDef = TypedDict(
+    "UpdatePackageGroupOriginConfigurationResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "allowedRepositoryUpdates": Dict[
+            PackageGroupOriginRestrictionTypeType,
+            Dict[PackageGroupAllowedRepositoryUpdateTypeType, List[str]],
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdatePackageGroupResultTypeDef = TypedDict(
+    "UpdatePackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListPackageGroupsResultTypeDef = TypedDict(
+    "ListPackageGroupsResultTypeDef",
+    {
+        "packageGroups": List[PackageGroupSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListSubPackageGroupsResultTypeDef = TypedDict(
+    "ListSubPackageGroupsResultTypeDef",
+    {
+        "packageGroups": List[PackageGroupSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact/type_defs.pyi` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     DomainStatusType,
     HashAlgorithmType,
     PackageFormatType,
+    PackageGroupAllowedRepositoryUpdateTypeType,
+    PackageGroupAssociationTypeType,
+    PackageGroupOriginRestrictionModeType,
+    PackageGroupOriginRestrictionTypeType,
     PackageVersionErrorCodeType,
     PackageVersionOriginTypeType,
     PackageVersionStatusType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -42,73 +46,87 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "AssociatedPackageTypeDef",
     "BlobTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeletePackageGroupRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeletePackageVersionsRequestRequestTypeDef",
     "DeleteRepositoryPermissionsPolicyRequestRequestTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "DescribeDomainRequestRequestTypeDef",
+    "DescribePackageGroupRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
     "DescribeRepositoryRequestRequestTypeDef",
     "DisassociateExternalConnectionRequestRequestTypeDef",
     "DisposePackageVersionsRequestRequestTypeDef",
     "DomainEntryPointTypeDef",
     "DomainSummaryTypeDef",
+    "GetAssociatedPackageGroupRequestRequestTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDomainPermissionsPolicyRequestRequestTypeDef",
     "GetPackageVersionAssetRequestRequestTypeDef",
     "GetPackageVersionReadmeRequestRequestTypeDef",
     "GetRepositoryEndpointRequestRequestTypeDef",
     "GetRepositoryPermissionsPolicyRequestRequestTypeDef",
     "LicenseInfoTypeDef",
     "PaginatorConfigTypeDef",
+    "ListAllowedRepositoriesForGroupRequestRequestTypeDef",
+    "ListAssociatedPackagesRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListPackageGroupsRequestRequestTypeDef",
     "ListPackageVersionAssetsRequestRequestTypeDef",
     "ListPackageVersionDependenciesRequestRequestTypeDef",
     "PackageDependencyTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
+    "ListSubPackageGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PackageGroupAllowedRepositoryTypeDef",
+    "PackageGroupReferenceTypeDef",
     "PackageOriginRestrictionsTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdatePackageGroupRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
     "GetAuthorizationTokenResultTypeDef",
     "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointResultTypeDef",
+    "ListAllowedRepositoriesForGroupResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
+    "ListAssociatedPackagesResultTypeDef",
     "PublishPackageVersionRequestRequestTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
+    "CreatePackageGroupRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainResultTypeDef",
     "DeleteDomainResultTypeDef",
     "DescribeDomainResultTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "UpdateRepositoryRequestRequestTypeDef",
@@ -116,42 +134,59 @@
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     "GetDomainPermissionsPolicyResultTypeDef",
     "GetRepositoryPermissionsPolicyResultTypeDef",
     "PutDomainPermissionsPolicyResultTypeDef",
     "PutRepositoryPermissionsPolicyResultTypeDef",
     "PackageVersionOriginTypeDef",
     "ListDomainsResultTypeDef",
+    "ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef",
+    "ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListPackageGroupsRequestListPackageGroupsPaginateTypeDef",
     "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
+    "ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
+    "UpdatePackageGroupOriginConfigurationRequestRequestTypeDef",
+    "PackageGroupOriginRestrictionTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
     "PackageVersionSummaryTypeDef",
+    "PackageGroupOriginConfigurationTypeDef",
     "PackageDescriptionTypeDef",
     "PackageSummaryTypeDef",
     "PutPackageOriginConfigurationResultTypeDef",
     "AssociateExternalConnectionResultTypeDef",
     "CreateRepositoryResultTypeDef",
     "DeleteRepositoryResultTypeDef",
     "DescribeRepositoryResultTypeDef",
     "DisassociateExternalConnectionResultTypeDef",
     "UpdateRepositoryResultTypeDef",
     "DescribePackageVersionResultTypeDef",
     "ListPackageVersionsResultTypeDef",
+    "PackageGroupDescriptionTypeDef",
+    "PackageGroupSummaryTypeDef",
     "DescribePackageResultTypeDef",
     "DeletePackageResultTypeDef",
     "ListPackagesResultTypeDef",
+    "CreatePackageGroupResultTypeDef",
+    "DeletePackageGroupResultTypeDef",
+    "DescribePackageGroupResultTypeDef",
+    "GetAssociatedPackageGroupResultTypeDef",
+    "UpdatePackageGroupOriginConfigurationResultTypeDef",
+    "UpdatePackageGroupResultTypeDef",
+    "ListPackageGroupsResultTypeDef",
+    "ListSubPackageGroupsResultTypeDef",
 )
 
 AssetSummaryTypeDef = TypedDict(
     "AssetSummaryTypeDef",
     {
         "name": str,
         "size": NotRequired[int],
@@ -167,18 +202,27 @@
         "domainOwner": NotRequired[str],
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
+AssociatedPackageTypeDef = TypedDict(
+    "AssociatedPackageTypeDef",
+    {
+        "format": NotRequired[PackageFormatType],
+        "namespace": NotRequired[str],
+        "package": NotRequired[str],
+        "associationType": NotRequired[PackageGroupAssociationTypeType],
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "CopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
@@ -254,14 +298,22 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domain": str,
         "domainOwner": NotRequired[str],
     },
 )
+DeletePackageGroupRequestRequestTypeDef = TypedDict(
+    "DeletePackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+    },
+)
 DeletePackageRequestRequestTypeDef = TypedDict(
     "DeletePackageRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -302,14 +354,22 @@
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "domain": str,
         "domainOwner": NotRequired[str],
     },
 )
+DescribePackageGroupRequestRequestTypeDef = TypedDict(
+    "DescribePackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+    },
+)
 DescribePackageRequestRequestTypeDef = TypedDict(
     "DescribePackageRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -374,14 +434,24 @@
         "owner": NotRequired[str],
         "arn": NotRequired[str],
         "status": NotRequired[DomainStatusType],
         "createdTime": NotRequired[datetime],
         "encryptionKey": NotRequired[str],
     },
 )
+GetAssociatedPackageGroupRequestRequestTypeDef = TypedDict(
+    "GetAssociatedPackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "format": PackageFormatType,
+        "package": str,
+        "domainOwner": NotRequired[str],
+        "namespace": NotRequired[str],
+    },
+)
 GetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "GetAuthorizationTokenRequestRequestTypeDef",
     {
         "domain": str,
         "domainOwner": NotRequired[str],
         "durationSeconds": NotRequired[int],
     },
@@ -447,21 +517,53 @@
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
 )
+ListAllowedRepositoriesForGroupRequestRequestTypeDef = TypedDict(
+    "ListAllowedRepositoriesForGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "originRestrictionType": PackageGroupOriginRestrictionTypeType,
+        "domainOwner": NotRequired[str],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
+ListAssociatedPackagesRequestRequestTypeDef = TypedDict(
+    "ListAssociatedPackagesRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+        "preview": NotRequired[bool],
+    },
+)
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListPackageGroupsRequestRequestTypeDef = TypedDict(
+    "ListPackageGroupsRequestRequestTypeDef",
+    {
+        "domain": str,
+        "domainOwner": NotRequired[str],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+        "prefix": NotRequired[str],
+    },
+)
 ListPackageVersionAssetsRequestRequestTypeDef = TypedDict(
     "ListPackageVersionAssetsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -552,20 +654,44 @@
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": NotRequired[str],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListSubPackageGroupsRequestRequestTypeDef = TypedDict(
+    "ListSubPackageGroupsRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
+PackageGroupAllowedRepositoryTypeDef = TypedDict(
+    "PackageGroupAllowedRepositoryTypeDef",
+    {
+        "repositoryName": NotRequired[str],
+        "originRestrictionType": NotRequired[PackageGroupOriginRestrictionTypeType],
+    },
+)
+PackageGroupReferenceTypeDef = TypedDict(
+    "PackageGroupReferenceTypeDef",
+    {
+        "arn": NotRequired[str],
+        "pattern": NotRequired[str],
+    },
+)
 PackageOriginRestrictionsTypeDef = TypedDict(
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
 )
@@ -605,14 +731,24 @@
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
+UpdatePackageGroupRequestRequestTypeDef = TypedDict(
+    "UpdatePackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "contactInfo": NotRequired[str],
+        "description": NotRequired[str],
+    },
+)
 UpdatePackageVersionsStatusRequestRequestTypeDef = TypedDict(
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -657,14 +793,22 @@
 GetRepositoryEndpointResultTypeDef = TypedDict(
     "GetRepositoryEndpointResultTypeDef",
     {
         "repositoryEndpoint": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAllowedRepositoriesForGroupResultTypeDef = TypedDict(
+    "ListAllowedRepositoriesForGroupResultTypeDef",
+    {
+        "allowedRepositories": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListPackageVersionAssetsResultTypeDef = TypedDict(
     "ListPackageVersionAssetsResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
@@ -683,14 +827,22 @@
         "version": str,
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAssociatedPackagesResultTypeDef = TypedDict(
+    "ListAssociatedPackagesResultTypeDef",
+    {
+        "packages": List[AssociatedPackageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 PublishPackageVersionRequestRequestTypeDef = TypedDict(
     "PublishPackageVersionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -739,14 +891,25 @@
     "CreateDomainRequestRequestTypeDef",
     {
         "domain": str,
         "encryptionKey": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+CreatePackageGroupRequestRequestTypeDef = TypedDict(
+    "CreatePackageGroupRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "contactInfo": NotRequired[str],
+        "description": NotRequired[str],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -852,20 +1015,49 @@
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef = TypedDict(
+    "ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "originRestrictionType": PackageGroupOriginRestrictionTypeType,
+        "domainOwner": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef = TypedDict(
+    "ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "preview": NotRequired[bool],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListPackageGroupsRequestListPackageGroupsPaginateTypeDef = TypedDict(
+    "ListPackageGroupsRequestListPackageGroupsPaginateTypeDef",
+    {
+        "domain": str,
+        "domainOwner": NotRequired[str],
+        "prefix": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
     "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -917,14 +1109,23 @@
 ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
     "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     {
         "repositoryPrefix": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef = TypedDict(
+    "ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListPackageVersionDependenciesResultTypeDef = TypedDict(
     "ListPackageVersionDependenciesResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
@@ -946,14 +1147,36 @@
     "ListRepositoriesResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdatePackageGroupOriginConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdatePackageGroupOriginConfigurationRequestRequestTypeDef",
+    {
+        "domain": str,
+        "packageGroup": str,
+        "domainOwner": NotRequired[str],
+        "restrictions": NotRequired[
+            Mapping[PackageGroupOriginRestrictionTypeType, PackageGroupOriginRestrictionModeType]
+        ],
+        "addAllowedRepositories": NotRequired[Sequence[PackageGroupAllowedRepositoryTypeDef]],
+        "removeAllowedRepositories": NotRequired[Sequence[PackageGroupAllowedRepositoryTypeDef]],
+    },
+)
+PackageGroupOriginRestrictionTypeDef = TypedDict(
+    "PackageGroupOriginRestrictionTypeDef",
+    {
+        "mode": NotRequired[PackageGroupOriginRestrictionModeType],
+        "effectiveMode": NotRequired[PackageGroupOriginRestrictionModeType],
+        "inheritedFrom": NotRequired[PackageGroupReferenceTypeDef],
+        "repositoriesCount": NotRequired[int],
+    },
+)
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
         "restrictions": NotRequired[PackageOriginRestrictionsTypeDef],
     },
 )
 PutPackageOriginConfigurationRequestRequestTypeDef = TypedDict(
@@ -1005,14 +1228,22 @@
     {
         "version": str,
         "status": PackageVersionStatusType,
         "revision": NotRequired[str],
         "origin": NotRequired[PackageVersionOriginTypeDef],
     },
 )
+PackageGroupOriginConfigurationTypeDef = TypedDict(
+    "PackageGroupOriginConfigurationTypeDef",
+    {
+        "restrictions": NotRequired[
+            Dict[PackageGroupOriginRestrictionTypeType, PackageGroupOriginRestrictionTypeDef]
+        ],
+    },
+)
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": NotRequired[PackageFormatType],
         "namespace": NotRequired[str],
         "name": NotRequired[str],
         "originConfiguration": NotRequired[PackageOriginConfigurationTypeDef],
@@ -1091,14 +1322,42 @@
         "namespace": str,
         "package": str,
         "versions": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+PackageGroupDescriptionTypeDef = TypedDict(
+    "PackageGroupDescriptionTypeDef",
+    {
+        "arn": NotRequired[str],
+        "pattern": NotRequired[str],
+        "domainName": NotRequired[str],
+        "domainOwner": NotRequired[str],
+        "createdTime": NotRequired[datetime],
+        "contactInfo": NotRequired[str],
+        "description": NotRequired[str],
+        "originConfiguration": NotRequired[PackageGroupOriginConfigurationTypeDef],
+        "parent": NotRequired[PackageGroupReferenceTypeDef],
+    },
+)
+PackageGroupSummaryTypeDef = TypedDict(
+    "PackageGroupSummaryTypeDef",
+    {
+        "arn": NotRequired[str],
+        "pattern": NotRequired[str],
+        "domainName": NotRequired[str],
+        "domainOwner": NotRequired[str],
+        "createdTime": NotRequired[datetime],
+        "contactInfo": NotRequired[str],
+        "description": NotRequired[str],
+        "originConfiguration": NotRequired[PackageGroupOriginConfigurationTypeDef],
+        "parent": NotRequired[PackageGroupReferenceTypeDef],
+    },
+)
 DescribePackageResultTypeDef = TypedDict(
     "DescribePackageResultTypeDef",
     {
         "package": PackageDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1113,7 +1372,70 @@
     "ListPackagesResultTypeDef",
     {
         "packages": List[PackageSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreatePackageGroupResultTypeDef = TypedDict(
+    "CreatePackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DeletePackageGroupResultTypeDef = TypedDict(
+    "DeletePackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribePackageGroupResultTypeDef = TypedDict(
+    "DescribePackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetAssociatedPackageGroupResultTypeDef = TypedDict(
+    "GetAssociatedPackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "associationType": PackageGroupAssociationTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdatePackageGroupOriginConfigurationResultTypeDef = TypedDict(
+    "UpdatePackageGroupOriginConfigurationResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "allowedRepositoryUpdates": Dict[
+            PackageGroupOriginRestrictionTypeType,
+            Dict[PackageGroupAllowedRepositoryUpdateTypeType, List[str]],
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdatePackageGroupResultTypeDef = TypedDict(
+    "UpdatePackageGroupResultTypeDef",
+    {
+        "packageGroup": PackageGroupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListPackageGroupsResultTypeDef = TypedDict(
+    "ListPackageGroupsResultTypeDef",
+    {
+        "packageGroups": List[PackageGroupSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListSubPackageGroupsResultTypeDef = TypedDict(
+    "ListSubPackageGroupsResultTypeDef",
+    {
+        "packageGroups": List[PackageGroupSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/PKG-INFO` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.34.0
-Summary: Type annotations for boto3.CodeArtifact 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.68
+Summary: Type annotations for boto3.CodeArtifact 1.34.68 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
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
 
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.34.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,38 +281,54 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_codeartifact import CodeArtifactClient
 from mypy_boto3_codeartifact.paginator import (
+    ListAllowedRepositoriesForGroupPaginator,
+    ListAssociatedPackagesPaginator,
     ListDomainsPaginator,
+    ListPackageGroupsPaginator,
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListPackagesPaginator,
     ListRepositoriesPaginator,
     ListRepositoriesInDomainPaginator,
+    ListSubPackageGroupsPaginator,
 )
 
 client: CodeArtifactClient = Session().client("codeartifact")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_allowed_repositories_for_group_paginator: ListAllowedRepositoriesForGroupPaginator = (
+    client.get_paginator("list_allowed_repositories_for_group")
+)
+list_associated_packages_paginator: ListAssociatedPackagesPaginator = client.get_paginator(
+    "list_associated_packages"
+)
 list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
+list_package_groups_paginator: ListPackageGroupsPaginator = client.get_paginator(
+    "list_package_groups"
+)
 list_package_version_assets_paginator: ListPackageVersionAssetsPaginator = client.get_paginator(
     "list_package_version_assets"
 )
 list_package_versions_paginator: ListPackageVersionsPaginator = client.get_paginator(
     "list_package_versions"
 )
 list_packages_paginator: ListPackagesPaginator = client.get_paginator("list_packages")
 list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
 list_repositories_in_domain_paginator: ListRepositoriesInDomainPaginator = client.get_paginator(
     "list_repositories_in_domain"
 )
+list_sub_package_groups_paginator: ListSubPackageGroupsPaginator = client.get_paginator(
+    "list_sub_package_groups"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_codeartifact.literals` module contains literals extracted from
```

### Comparing `mypy-boto3-codeartifact-1.34.0/mypy_boto3_codeartifact.egg-info/SOURCES.txt` & `mypy-boto3-codeartifact-1.34.68/mypy_boto3_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.34.0/setup.py` & `mypy-boto3-codeartifact-1.34.68/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeartifact",
-    version="1.34.0",
+    version="1.34.68",
     packages=["mypy_boto3_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.CodeArtifact 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.CodeArtifact 1.34.68 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 codeartifact type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codeartifact": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

