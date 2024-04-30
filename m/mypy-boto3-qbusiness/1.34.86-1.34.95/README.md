# Comparing `tmp/mypy_boto3_qbusiness-1.34.86.tar.gz` & `tmp/mypy_boto3_qbusiness-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_qbusiness-1.34.86.tar", last modified: Wed Apr 17 19:47:44 2024, max compression
+gzip compressed data, was "mypy_boto3_qbusiness-1.34.95.tar", last modified: Tue Apr 30 19:34:53 2024, max compression
```

## Comparing `mypy_boto3_qbusiness-1.34.86.tar` & `mypy_boto3_qbusiness-1.34.95.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44581 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    44578 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14275 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-17 19:47:31.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    58504 2024-04-17 19:47:32.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    58504 2024-04-17 19:47:32.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 19:47:44.000000 mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:47:44.461914 mypy_boto3_qbusiness-1.34.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-17 19:47:30.000000 mypy_boto3_qbusiness-1.34.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.519052 mypy_boto3_qbusiness-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:32:19.000000 mypy_boto3_qbusiness-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14229 2024-04-30 19:34:53.519052 mypy_boto3_qbusiness-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-04-30 19:32:19.000000 mypy_boto3_qbusiness-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.519052 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-30 19:32:19.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-30 19:32:19.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 19:32:19.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45095 2024-04-30 19:32:20.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45092 2024-04-30 19:32:20.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-04-30 19:32:20.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-04-30 19:32:20.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-04-30 19:32:20.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-04-30 19:32:20.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:19.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    68232 2024-04-30 19:32:21.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68232 2024-04-30 19:32:21.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:32:19.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.519052 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14229 2024-04-30 19:34:53.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 19:34:53.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:53.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:53.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:53.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 19:34:53.000000 mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:53.519052 mypy_boto3_qbusiness-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-30 19:32:19.000000 mypy_boto3_qbusiness-1.34.95/setup.py
```

### Comparing `mypy_boto3_qbusiness-1.34.86/LICENSE` & `mypy_boto3_qbusiness-1.34.95/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_qbusiness-1.34.86/PKG-INFO` & `mypy_boto3_qbusiness-1.34.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qbusiness
-Version: 1.34.86
-Summary: Type annotations for boto3.QBusiness 1.34.86 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.95
+Summary: Type annotations for boto3.QBusiness 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qbusiness)](https://pepy.tech/project/mypy-boto3-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QBusiness 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[boto3.QBusiness 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,35 +331,35 @@
 `mypy_boto3_qbusiness.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 Full list of `QBusiness` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/literals/).
 
 ```python
-from mypy_boto3_qbusiness.literals import ActionPayloadFieldTypeType
+from mypy_boto3_qbusiness.literals import APISchemaTypeType
 
 
-def check_value(value: ActionPayloadFieldTypeType) -> bool: ...
+def check_value(value: APISchemaTypeType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_qbusiness.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `QBusiness` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/type_defs/).
 
 ```python
-from mypy_boto3_qbusiness.type_defs import ActionExecutionPayloadFieldPaginatorTypeDef
+from mypy_boto3_qbusiness.type_defs import S3TypeDef
 
 
-def get_value() -> ActionExecutionPayloadFieldPaginatorTypeDef:
+def get_value() -> S3TypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy_boto3_qbusiness-1.34.86/README.md` & `mypy_boto3_qbusiness-1.34.95/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qbusiness)](https://pepy.tech/project/mypy-boto3-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QBusiness 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[boto3.QBusiness 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,35 +298,35 @@
 `mypy_boto3_qbusiness.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 Full list of `QBusiness` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/literals/).
 
 ```python
-from mypy_boto3_qbusiness.literals import ActionPayloadFieldTypeType
+from mypy_boto3_qbusiness.literals import APISchemaTypeType
 
 
-def check_value(value: ActionPayloadFieldTypeType) -> bool: ...
+def check_value(value: APISchemaTypeType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_qbusiness.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `QBusiness` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/type_defs/).
 
 ```python
-from mypy_boto3_qbusiness.type_defs import ActionExecutionPayloadFieldPaginatorTypeDef
+from mypy_boto3_qbusiness.type_defs import S3TypeDef
 
 
-def get_value() -> ActionExecutionPayloadFieldPaginatorTypeDef:
+def get_value() -> S3TypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__init__.py` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__init__.pyi` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/__main__.py` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QBusiness 1.34.86\n"
-        "Version:         1.34.86\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.QBusiness 1.34.95\n"
+        "Version:         1.34.95\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.86")
+    print("1.34.95")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/client.py` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ChatModeType,
     DataSourceSyncJobStatusType,
+    IndexTypeType,
     MembershipTypeType,
     PluginStateType,
     PluginTypeType,
     ResponseScopeType,
     RetrieverTypeType,
     WebExperienceSamplePromptsControlModeType,
 )
@@ -40,34 +41,36 @@
     ListIndicesPaginator,
     ListMessagesPaginator,
     ListPluginsPaginator,
     ListRetrieversPaginator,
     ListWebExperiencesPaginator,
 )
 from .type_defs import (
-    ActionExecutionTypeDef,
+    ActionExecutionUnionTypeDef,
     AttachmentInputTypeDef,
     AttachmentsConfigurationTypeDef,
     AttributeFilterTypeDef,
+    AuthChallengeResponseTypeDef,
     BatchDeleteDocumentResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     BlockedPhrasesConfigurationUpdateTypeDef,
     ChatModeConfigurationTypeDef,
     ChatSyncOutputTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreatePluginResponseTypeDef,
     CreateRetrieverResponseTypeDef,
     CreateWebExperienceResponseTypeDef,
     CreatorModeConfigurationTypeDef,
-    DataSourceVpcConfigurationTypeDef,
+    CustomPluginConfigurationTypeDef,
+    DataSourceVpcConfigurationUnionTypeDef,
     DeleteDocumentTypeDef,
     DocumentAttributeConfigurationTypeDef,
-    DocumentEnrichmentConfigurationTypeDef,
+    DocumentEnrichmentConfigurationUnionTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     GetApplicationResponseTypeDef,
     GetChatControlsConfigurationResponseTypeDef,
     GetDataSourceResponseTypeDef,
     GetGroupResponseTypeDef,
@@ -87,20 +90,20 @@
     ListIndicesResponseTypeDef,
     ListMessagesResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListRetrieversResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebExperiencesResponseTypeDef,
     MessageUsefulnessFeedbackTypeDef,
-    PluginAuthConfigurationTypeDef,
-    RetrieverConfigurationTypeDef,
+    PluginAuthConfigurationUnionTypeDef,
+    RetrieverConfigurationUnionTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
-    TopicConfigurationTypeDef,
+    TopicConfigurationUnionTypeDef,
     UpdateUserResponseTypeDef,
     UserAliasTypeDef,
     WebExperienceAuthConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -147,16 +150,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#exceptions)
         """
 
     def batch_delete_document(
         self,
         *,
         applicationId: str,
-        documents: Sequence[DeleteDocumentTypeDef],
         indexId: str,
+        documents: Sequence[DeleteDocumentTypeDef],
         dataSourceSyncId: str = ...,
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Asynchronously deletes one or more documents added using the `BatchPutDocument`
         API from an Amazon Q Business
         index.
 
@@ -164,18 +167,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#batch_delete_document)
         """
 
     def batch_put_document(
         self,
         *,
         applicationId: str,
-        documents: Sequence[DocumentTypeDef],
         indexId: str,
-        dataSourceSyncId: str = ...,
+        documents: Sequence[DocumentTypeDef],
         roleArn: str = ...,
+        dataSourceSyncId: str = ...,
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#batch_put_document)
         """
@@ -188,25 +191,26 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#can_paginate)
         """
 
     def chat_sync(
         self,
         *,
         applicationId: str,
-        actionExecution: ActionExecutionTypeDef = ...,
+        userId: str = ...,
+        userGroups: Sequence[str] = ...,
+        userMessage: str = ...,
         attachments: Sequence[AttachmentInputTypeDef] = ...,
+        actionExecution: ActionExecutionUnionTypeDef = ...,
+        authChallengeResponse: AuthChallengeResponseTypeDef = ...,
+        conversationId: str = ...,
+        parentMessageId: str = ...,
         attributeFilter: "AttributeFilterTypeDef" = ...,
         chatMode: ChatModeType = ...,
         chatModeConfiguration: ChatModeConfigurationTypeDef = ...,
         clientToken: str = ...,
-        conversationId: str = ...,
-        parentMessageId: str = ...,
-        userGroups: Sequence[str] = ...,
-        userId: str = ...,
-        userMessage: str = ...,
     ) -> ChatSyncOutputTypeDef:
         """
         Starts or continues a non-streaming Amazon Q Business conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.chat_sync)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#chat_sync)
         """
@@ -219,132 +223,134 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#close)
         """
 
     def create_application(
         self,
         *,
         displayName: str,
-        roleArn: str,
-        attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
-        clientToken: str = ...,
+        roleArn: str = ...,
+        identityCenterInstanceArn: str = ...,
         description: str = ...,
         encryptionConfiguration: EncryptionConfigurationTypeDef = ...,
-        identityCenterInstanceArn: str = ...,
         tags: Sequence[TagTypeDef] = ...,
+        clientToken: str = ...,
+        attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_application)
         """
 
     def create_data_source(
         self,
         *,
         applicationId: str,
-        configuration: Mapping[str, Any],
-        displayName: str,
         indexId: str,
-        clientToken: str = ...,
+        displayName: str,
+        configuration: Mapping[str, Any],
+        vpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
         description: str = ...,
-        documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
-        roleArn: str = ...,
-        syncSchedule: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
+        syncSchedule: str = ...,
+        roleArn: str = ...,
+        clientToken: str = ...,
+        documentEnrichmentConfiguration: DocumentEnrichmentConfigurationUnionTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector for an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_data_source)
         """
 
     def create_index(
         self,
         *,
         applicationId: str,
         displayName: str,
-        capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
-        clientToken: str = ...,
+        type: IndexTypeType = ...,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
+        capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
+        clientToken: str = ...,
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_index)
         """
 
     def create_plugin(
         self,
         *,
         applicationId: str,
-        authConfiguration: PluginAuthConfigurationTypeDef,
         displayName: str,
-        serverUrl: str,
         type: PluginTypeType,
-        clientToken: str = ...,
+        authConfiguration: PluginAuthConfigurationUnionTypeDef,
+        serverUrl: str = ...,
+        customPluginConfiguration: CustomPluginConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
+        clientToken: str = ...,
     ) -> CreatePluginResponseTypeDef:
         """
         Creates an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_plugin)
         """
 
     def create_retriever(
         self,
         *,
         applicationId: str,
-        configuration: RetrieverConfigurationTypeDef,
-        displayName: str,
         type: RetrieverTypeType,
-        clientToken: str = ...,
+        displayName: str,
+        configuration: RetrieverConfigurationUnionTypeDef,
         roleArn: str = ...,
+        clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRetrieverResponseTypeDef:
         """
         Adds a retriever to your Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_retriever)
         """
 
     def create_user(
         self,
         *,
         applicationId: str,
         userId: str,
-        clientToken: str = ...,
         userAliases: Sequence[UserAliasTypeDef] = ...,
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a universally unique identifier (UUID) mapped to a list of local user
         ids within an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_user)
         """
 
     def create_web_experience(
         self,
         *,
         applicationId: str,
-        clientToken: str = ...,
-        roleArn: str = ...,
-        samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
-        subtitle: str = ...,
-        tags: Sequence[TagTypeDef] = ...,
         title: str = ...,
+        subtitle: str = ...,
         welcomeMessage: str = ...,
+        samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
+        roleArn: str = ...,
+        tags: Sequence[TagTypeDef] = ...,
+        clientToken: str = ...,
     ) -> CreateWebExperienceResponseTypeDef:
         """
         Creates an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_web_experience)
         """
@@ -362,35 +368,35 @@
         Deletes chat controls configured for an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_chat_controls_configuration)
         """
 
     def delete_conversation(
-        self, *, applicationId: str, conversationId: str, userId: str = ...
+        self, *, conversationId: str, applicationId: str, userId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes an Amazon Q Business web experience conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_conversation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_conversation)
         """
 
     def delete_data_source(
-        self, *, applicationId: str, dataSourceId: str, indexId: str
+        self, *, applicationId: str, indexId: str, dataSourceId: str
     ) -> Dict[str, Any]:
         """
         Deletes an Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_data_source)
         """
 
     def delete_group(
-        self, *, applicationId: str, groupName: str, indexId: str, dataSourceId: str = ...
+        self, *, applicationId: str, indexId: str, groupName: str, dataSourceId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a group so that all users and sub groups that belong to the group can
         no longer access documents only available to that
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_group)
@@ -468,25 +474,25 @@
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_chat_controls_configuration)
         """
 
     def get_data_source(
-        self, *, applicationId: str, dataSourceId: str, indexId: str
+        self, *, applicationId: str, indexId: str, dataSourceId: str
     ) -> GetDataSourceResponseTypeDef:
         """
         Gets information about an existing Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_data_source)
         """
 
     def get_group(
-        self, *, applicationId: str, groupName: str, indexId: str, dataSourceId: str = ...
+        self, *, applicationId: str, indexId: str, groupName: str, dataSourceId: str = ...
     ) -> GetGroupResponseTypeDef:
         """
         Describes a group by group name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_group)
         """
@@ -533,71 +539,71 @@
         Gets information about an existing Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_web_experience)
         """
 
     def list_applications(
-        self, *, maxResults: int = ..., nextToken: str = ...
+        self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists Amazon Q Business applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_applications)
         """
 
     def list_conversations(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ..., userId: str = ...
+        self, *, applicationId: str, userId: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListConversationsResponseTypeDef:
         """
         Lists one or more Amazon Q Business conversations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_conversations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_conversations)
         """
 
     def list_data_source_sync_jobs(
         self,
         *,
-        applicationId: str,
         dataSourceId: str,
+        applicationId: str,
         indexId: str,
-        endTime: TimestampTypeDef = ...,
-        maxResults: int = ...,
         nextToken: str = ...,
+        maxResults: int = ...,
         startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         statusFilter: DataSourceSyncJobStatusType = ...,
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Get information about an Amazon Q Business data source connector
         synchronization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_data_source_sync_jobs)
         """
 
     def list_data_sources(
-        self, *, applicationId: str, indexId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, indexId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListDataSourcesResponseTypeDef:
         """
         Lists the Amazon Q Business data source connectors that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_data_sources)
         """
 
     def list_documents(
         self,
         *,
         applicationId: str,
         indexId: str,
         dataSourceIds: Sequence[str] = ...,
-        maxResults: int = ...,
         nextToken: str = ...,
+        maxResults: int = ...,
     ) -> ListDocumentsResponseTypeDef:
         """
         A list of documents attached to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_documents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_documents)
         """
@@ -605,62 +611,62 @@
     def list_groups(
         self,
         *,
         applicationId: str,
         indexId: str,
         updatedEarlierThan: TimestampTypeDef,
         dataSourceId: str = ...,
-        maxResults: int = ...,
         nextToken: str = ...,
+        maxResults: int = ...,
     ) -> ListGroupsResponseTypeDef:
         """
         Provides a list of groups that are mapped to users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_groups)
         """
 
     def list_indices(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListIndicesResponseTypeDef:
         """
         Lists the Amazon Q Business indices you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_indices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_indices)
         """
 
     def list_messages(
         self,
         *,
-        applicationId: str,
         conversationId: str,
-        maxResults: int = ...,
-        nextToken: str = ...,
+        applicationId: str,
         userId: str = ...,
+        nextToken: str = ...,
+        maxResults: int = ...,
     ) -> ListMessagesResponseTypeDef:
         """
         Gets a list of messages associated with an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_messages)
         """
 
     def list_plugins(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListPluginsResponseTypeDef:
         """
         Lists configured Amazon Q Business plugins.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_plugins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_plugins)
         """
 
     def list_retrievers(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListRetrieversResponseTypeDef:
         """
         Lists the retriever used by an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_retrievers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_retrievers)
         """
@@ -670,71 +676,71 @@
         Gets a list of tags associated with a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_tags_for_resource)
         """
 
     def list_web_experiences(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListWebExperiencesResponseTypeDef:
         """
         Lists one or more Amazon Q Business Web Experiences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_web_experiences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_web_experiences)
         """
 
     def put_feedback(
         self,
         *,
         applicationId: str,
         conversationId: str,
         messageId: str,
+        userId: str = ...,
         messageCopiedAt: TimestampTypeDef = ...,
         messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...,
-        userId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables your end user to provide feedback on their Amazon Q Business generated
         chat
         responses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#put_feedback)
         """
 
     def put_group(
         self,
         *,
         applicationId: str,
-        groupMembers: GroupMembersTypeDef,
-        groupName: str,
         indexId: str,
+        groupName: str,
         type: MembershipTypeType,
+        groupMembers: GroupMembersTypeDef,
         dataSourceId: str = ...,
     ) -> Dict[str, Any]:
         """
         Create, or updates, a mapping of users—who have access to a document—to groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#put_group)
         """
 
     def start_data_source_sync_job(
-        self, *, applicationId: str, dataSourceId: str, indexId: str
+        self, *, dataSourceId: str, applicationId: str, indexId: str
     ) -> StartDataSourceSyncJobResponseTypeDef:
         """
         Starts a data source connector synchronization job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.start_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#start_data_source_sync_job)
         """
 
     def stop_data_source_sync_job(
-        self, *, applicationId: str, dataSourceId: str, indexId: str
+        self, *, dataSourceId: str, applicationId: str, indexId: str
     ) -> Dict[str, Any]:
         """
         Stops an Amazon Q Business data source connector synchronization job already in
         progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.stop_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#stop_data_source_sync_job)
@@ -758,106 +764,108 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#untag_resource)
         """
 
     def update_application(
         self,
         *,
         applicationId: str,
-        attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
-        description: str = ...,
+        identityCenterInstanceArn: str = ...,
         displayName: str = ...,
+        description: str = ...,
         roleArn: str = ...,
+        attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_application)
         """
 
     def update_chat_controls_configuration(
         self,
         *,
         applicationId: str,
-        blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,
         clientToken: str = ...,
-        creatorModeConfiguration: CreatorModeConfigurationTypeDef = ...,
         responseScope: ResponseScopeType = ...,
-        topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationTypeDef] = ...,
-        topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...,
+        blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,
+        topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationUnionTypeDef] = ...,
+        topicConfigurationsToDelete: Sequence[TopicConfigurationUnionTypeDef] = ...,
+        creatorModeConfiguration: CreatorModeConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an set of chat controls configured for an existing Amazon Q Business
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_chat_controls_configuration)
         """
 
     def update_data_source(
         self,
         *,
         applicationId: str,
-        dataSourceId: str,
         indexId: str,
+        dataSourceId: str,
+        displayName: str = ...,
         configuration: Mapping[str, Any] = ...,
+        vpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
         description: str = ...,
-        displayName: str = ...,
-        documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
-        roleArn: str = ...,
         syncSchedule: str = ...,
-        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
+        roleArn: str = ...,
+        documentEnrichmentConfiguration: DocumentEnrichmentConfigurationUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_data_source)
         """
 
     def update_index(
         self,
         *,
         applicationId: str,
         indexId: str,
-        capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
-        description: str = ...,
         displayName: str = ...,
+        description: str = ...,
+        capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_index)
         """
 
     def update_plugin(
         self,
         *,
         applicationId: str,
         pluginId: str,
-        authConfiguration: PluginAuthConfigurationTypeDef = ...,
         displayName: str = ...,
-        serverUrl: str = ...,
         state: PluginStateType = ...,
+        serverUrl: str = ...,
+        customPluginConfiguration: CustomPluginConfigurationTypeDef = ...,
+        authConfiguration: PluginAuthConfigurationUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_plugin)
         """
 
     def update_retriever(
         self,
         *,
         applicationId: str,
         retrieverId: str,
-        configuration: RetrieverConfigurationTypeDef = ...,
+        configuration: RetrieverConfigurationUnionTypeDef = ...,
         displayName: str = ...,
         roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the retriever used for your Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_retriever)
@@ -865,34 +873,35 @@
         """
 
     def update_user(
         self,
         *,
         applicationId: str,
         userId: str,
-        userAliasesToDelete: Sequence[UserAliasTypeDef] = ...,
         userAliasesToUpdate: Sequence[UserAliasTypeDef] = ...,
+        userAliasesToDelete: Sequence[UserAliasTypeDef] = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates a information associated with a user id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_user)
         """
 
     def update_web_experience(
         self,
         *,
         applicationId: str,
         webExperienceId: str,
+        roleArn: str = ...,
         authenticationConfiguration: WebExperienceAuthConfigurationTypeDef = ...,
-        samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
-        subtitle: str = ...,
         title: str = ...,
+        subtitle: str = ...,
         welcomeMessage: str = ...,
+        samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_web_experience)
         """
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/client.pyi` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ChatModeType,
     DataSourceSyncJobStatusType,
+    IndexTypeType,
     MembershipTypeType,
     PluginStateType,
     PluginTypeType,
     ResponseScopeType,
     RetrieverTypeType,
     WebExperienceSamplePromptsControlModeType,
 )
@@ -40,34 +41,36 @@
     ListIndicesPaginator,
     ListMessagesPaginator,
     ListPluginsPaginator,
     ListRetrieversPaginator,
     ListWebExperiencesPaginator,
 )
 from .type_defs import (
-    ActionExecutionTypeDef,
+    ActionExecutionUnionTypeDef,
     AttachmentInputTypeDef,
     AttachmentsConfigurationTypeDef,
     AttributeFilterTypeDef,
+    AuthChallengeResponseTypeDef,
     BatchDeleteDocumentResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     BlockedPhrasesConfigurationUpdateTypeDef,
     ChatModeConfigurationTypeDef,
     ChatSyncOutputTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreatePluginResponseTypeDef,
     CreateRetrieverResponseTypeDef,
     CreateWebExperienceResponseTypeDef,
     CreatorModeConfigurationTypeDef,
-    DataSourceVpcConfigurationTypeDef,
+    CustomPluginConfigurationTypeDef,
+    DataSourceVpcConfigurationUnionTypeDef,
     DeleteDocumentTypeDef,
     DocumentAttributeConfigurationTypeDef,
-    DocumentEnrichmentConfigurationTypeDef,
+    DocumentEnrichmentConfigurationUnionTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     GetApplicationResponseTypeDef,
     GetChatControlsConfigurationResponseTypeDef,
     GetDataSourceResponseTypeDef,
     GetGroupResponseTypeDef,
@@ -87,20 +90,20 @@
     ListIndicesResponseTypeDef,
     ListMessagesResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListRetrieversResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebExperiencesResponseTypeDef,
     MessageUsefulnessFeedbackTypeDef,
-    PluginAuthConfigurationTypeDef,
-    RetrieverConfigurationTypeDef,
+    PluginAuthConfigurationUnionTypeDef,
+    RetrieverConfigurationUnionTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
-    TopicConfigurationTypeDef,
+    TopicConfigurationUnionTypeDef,
     UpdateUserResponseTypeDef,
     UserAliasTypeDef,
     WebExperienceAuthConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -144,16 +147,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#exceptions)
         """
 
     def batch_delete_document(
         self,
         *,
         applicationId: str,
-        documents: Sequence[DeleteDocumentTypeDef],
         indexId: str,
+        documents: Sequence[DeleteDocumentTypeDef],
         dataSourceSyncId: str = ...,
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Asynchronously deletes one or more documents added using the `BatchPutDocument`
         API from an Amazon Q Business
         index.
 
@@ -161,18 +164,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#batch_delete_document)
         """
 
     def batch_put_document(
         self,
         *,
         applicationId: str,
-        documents: Sequence[DocumentTypeDef],
         indexId: str,
-        dataSourceSyncId: str = ...,
+        documents: Sequence[DocumentTypeDef],
         roleArn: str = ...,
+        dataSourceSyncId: str = ...,
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#batch_put_document)
         """
@@ -185,25 +188,26 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#can_paginate)
         """
 
     def chat_sync(
         self,
         *,
         applicationId: str,
-        actionExecution: ActionExecutionTypeDef = ...,
+        userId: str = ...,
+        userGroups: Sequence[str] = ...,
+        userMessage: str = ...,
         attachments: Sequence[AttachmentInputTypeDef] = ...,
+        actionExecution: ActionExecutionUnionTypeDef = ...,
+        authChallengeResponse: AuthChallengeResponseTypeDef = ...,
+        conversationId: str = ...,
+        parentMessageId: str = ...,
         attributeFilter: "AttributeFilterTypeDef" = ...,
         chatMode: ChatModeType = ...,
         chatModeConfiguration: ChatModeConfigurationTypeDef = ...,
         clientToken: str = ...,
-        conversationId: str = ...,
-        parentMessageId: str = ...,
-        userGroups: Sequence[str] = ...,
-        userId: str = ...,
-        userMessage: str = ...,
     ) -> ChatSyncOutputTypeDef:
         """
         Starts or continues a non-streaming Amazon Q Business conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.chat_sync)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#chat_sync)
         """
@@ -216,132 +220,134 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#close)
         """
 
     def create_application(
         self,
         *,
         displayName: str,
-        roleArn: str,
-        attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
-        clientToken: str = ...,
+        roleArn: str = ...,
+        identityCenterInstanceArn: str = ...,
         description: str = ...,
         encryptionConfiguration: EncryptionConfigurationTypeDef = ...,
-        identityCenterInstanceArn: str = ...,
         tags: Sequence[TagTypeDef] = ...,
+        clientToken: str = ...,
+        attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_application)
         """
 
     def create_data_source(
         self,
         *,
         applicationId: str,
-        configuration: Mapping[str, Any],
-        displayName: str,
         indexId: str,
-        clientToken: str = ...,
+        displayName: str,
+        configuration: Mapping[str, Any],
+        vpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
         description: str = ...,
-        documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
-        roleArn: str = ...,
-        syncSchedule: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
+        syncSchedule: str = ...,
+        roleArn: str = ...,
+        clientToken: str = ...,
+        documentEnrichmentConfiguration: DocumentEnrichmentConfigurationUnionTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector for an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_data_source)
         """
 
     def create_index(
         self,
         *,
         applicationId: str,
         displayName: str,
-        capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
-        clientToken: str = ...,
+        type: IndexTypeType = ...,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
+        capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
+        clientToken: str = ...,
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_index)
         """
 
     def create_plugin(
         self,
         *,
         applicationId: str,
-        authConfiguration: PluginAuthConfigurationTypeDef,
         displayName: str,
-        serverUrl: str,
         type: PluginTypeType,
-        clientToken: str = ...,
+        authConfiguration: PluginAuthConfigurationUnionTypeDef,
+        serverUrl: str = ...,
+        customPluginConfiguration: CustomPluginConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
+        clientToken: str = ...,
     ) -> CreatePluginResponseTypeDef:
         """
         Creates an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_plugin)
         """
 
     def create_retriever(
         self,
         *,
         applicationId: str,
-        configuration: RetrieverConfigurationTypeDef,
-        displayName: str,
         type: RetrieverTypeType,
-        clientToken: str = ...,
+        displayName: str,
+        configuration: RetrieverConfigurationUnionTypeDef,
         roleArn: str = ...,
+        clientToken: str = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRetrieverResponseTypeDef:
         """
         Adds a retriever to your Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_retriever)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_retriever)
         """
 
     def create_user(
         self,
         *,
         applicationId: str,
         userId: str,
-        clientToken: str = ...,
         userAliases: Sequence[UserAliasTypeDef] = ...,
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates a universally unique identifier (UUID) mapped to a list of local user
         ids within an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_user)
         """
 
     def create_web_experience(
         self,
         *,
         applicationId: str,
-        clientToken: str = ...,
-        roleArn: str = ...,
-        samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
-        subtitle: str = ...,
-        tags: Sequence[TagTypeDef] = ...,
         title: str = ...,
+        subtitle: str = ...,
         welcomeMessage: str = ...,
+        samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
+        roleArn: str = ...,
+        tags: Sequence[TagTypeDef] = ...,
+        clientToken: str = ...,
     ) -> CreateWebExperienceResponseTypeDef:
         """
         Creates an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.create_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#create_web_experience)
         """
@@ -359,35 +365,35 @@
         Deletes chat controls configured for an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_chat_controls_configuration)
         """
 
     def delete_conversation(
-        self, *, applicationId: str, conversationId: str, userId: str = ...
+        self, *, conversationId: str, applicationId: str, userId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes an Amazon Q Business web experience conversation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_conversation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_conversation)
         """
 
     def delete_data_source(
-        self, *, applicationId: str, dataSourceId: str, indexId: str
+        self, *, applicationId: str, indexId: str, dataSourceId: str
     ) -> Dict[str, Any]:
         """
         Deletes an Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#delete_data_source)
         """
 
     def delete_group(
-        self, *, applicationId: str, groupName: str, indexId: str, dataSourceId: str = ...
+        self, *, applicationId: str, indexId: str, groupName: str, dataSourceId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a group so that all users and sub groups that belong to the group can
         no longer access documents only available to that
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.delete_group)
@@ -465,25 +471,25 @@
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_chat_controls_configuration)
         """
 
     def get_data_source(
-        self, *, applicationId: str, dataSourceId: str, indexId: str
+        self, *, applicationId: str, indexId: str, dataSourceId: str
     ) -> GetDataSourceResponseTypeDef:
         """
         Gets information about an existing Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_data_source)
         """
 
     def get_group(
-        self, *, applicationId: str, groupName: str, indexId: str, dataSourceId: str = ...
+        self, *, applicationId: str, indexId: str, groupName: str, dataSourceId: str = ...
     ) -> GetGroupResponseTypeDef:
         """
         Describes a group by group name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_group)
         """
@@ -530,71 +536,71 @@
         Gets information about an existing Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.get_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#get_web_experience)
         """
 
     def list_applications(
-        self, *, maxResults: int = ..., nextToken: str = ...
+        self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists Amazon Q Business applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_applications)
         """
 
     def list_conversations(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ..., userId: str = ...
+        self, *, applicationId: str, userId: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListConversationsResponseTypeDef:
         """
         Lists one or more Amazon Q Business conversations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_conversations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_conversations)
         """
 
     def list_data_source_sync_jobs(
         self,
         *,
-        applicationId: str,
         dataSourceId: str,
+        applicationId: str,
         indexId: str,
-        endTime: TimestampTypeDef = ...,
-        maxResults: int = ...,
         nextToken: str = ...,
+        maxResults: int = ...,
         startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         statusFilter: DataSourceSyncJobStatusType = ...,
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Get information about an Amazon Q Business data source connector
         synchronization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_data_source_sync_jobs)
         """
 
     def list_data_sources(
-        self, *, applicationId: str, indexId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, indexId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListDataSourcesResponseTypeDef:
         """
         Lists the Amazon Q Business data source connectors that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_data_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_data_sources)
         """
 
     def list_documents(
         self,
         *,
         applicationId: str,
         indexId: str,
         dataSourceIds: Sequence[str] = ...,
-        maxResults: int = ...,
         nextToken: str = ...,
+        maxResults: int = ...,
     ) -> ListDocumentsResponseTypeDef:
         """
         A list of documents attached to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_documents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_documents)
         """
@@ -602,62 +608,62 @@
     def list_groups(
         self,
         *,
         applicationId: str,
         indexId: str,
         updatedEarlierThan: TimestampTypeDef,
         dataSourceId: str = ...,
-        maxResults: int = ...,
         nextToken: str = ...,
+        maxResults: int = ...,
     ) -> ListGroupsResponseTypeDef:
         """
         Provides a list of groups that are mapped to users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_groups)
         """
 
     def list_indices(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListIndicesResponseTypeDef:
         """
         Lists the Amazon Q Business indices you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_indices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_indices)
         """
 
     def list_messages(
         self,
         *,
-        applicationId: str,
         conversationId: str,
-        maxResults: int = ...,
-        nextToken: str = ...,
+        applicationId: str,
         userId: str = ...,
+        nextToken: str = ...,
+        maxResults: int = ...,
     ) -> ListMessagesResponseTypeDef:
         """
         Gets a list of messages associated with an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_messages)
         """
 
     def list_plugins(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListPluginsResponseTypeDef:
         """
         Lists configured Amazon Q Business plugins.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_plugins)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_plugins)
         """
 
     def list_retrievers(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListRetrieversResponseTypeDef:
         """
         Lists the retriever used by an Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_retrievers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_retrievers)
         """
@@ -667,71 +673,71 @@
         Gets a list of tags associated with a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_tags_for_resource)
         """
 
     def list_web_experiences(
-        self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
+        self, *, applicationId: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListWebExperiencesResponseTypeDef:
         """
         Lists one or more Amazon Q Business Web Experiences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.list_web_experiences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#list_web_experiences)
         """
 
     def put_feedback(
         self,
         *,
         applicationId: str,
         conversationId: str,
         messageId: str,
+        userId: str = ...,
         messageCopiedAt: TimestampTypeDef = ...,
         messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...,
-        userId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables your end user to provide feedback on their Amazon Q Business generated
         chat
         responses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#put_feedback)
         """
 
     def put_group(
         self,
         *,
         applicationId: str,
-        groupMembers: GroupMembersTypeDef,
-        groupName: str,
         indexId: str,
+        groupName: str,
         type: MembershipTypeType,
+        groupMembers: GroupMembersTypeDef,
         dataSourceId: str = ...,
     ) -> Dict[str, Any]:
         """
         Create, or updates, a mapping of users—who have access to a document—to groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.put_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#put_group)
         """
 
     def start_data_source_sync_job(
-        self, *, applicationId: str, dataSourceId: str, indexId: str
+        self, *, dataSourceId: str, applicationId: str, indexId: str
     ) -> StartDataSourceSyncJobResponseTypeDef:
         """
         Starts a data source connector synchronization job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.start_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#start_data_source_sync_job)
         """
 
     def stop_data_source_sync_job(
-        self, *, applicationId: str, dataSourceId: str, indexId: str
+        self, *, dataSourceId: str, applicationId: str, indexId: str
     ) -> Dict[str, Any]:
         """
         Stops an Amazon Q Business data source connector synchronization job already in
         progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.stop_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#stop_data_source_sync_job)
@@ -755,106 +761,108 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#untag_resource)
         """
 
     def update_application(
         self,
         *,
         applicationId: str,
-        attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
-        description: str = ...,
+        identityCenterInstanceArn: str = ...,
         displayName: str = ...,
+        description: str = ...,
         roleArn: str = ...,
+        attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_application)
         """
 
     def update_chat_controls_configuration(
         self,
         *,
         applicationId: str,
-        blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,
         clientToken: str = ...,
-        creatorModeConfiguration: CreatorModeConfigurationTypeDef = ...,
         responseScope: ResponseScopeType = ...,
-        topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationTypeDef] = ...,
-        topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...,
+        blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,
+        topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationUnionTypeDef] = ...,
+        topicConfigurationsToDelete: Sequence[TopicConfigurationUnionTypeDef] = ...,
+        creatorModeConfiguration: CreatorModeConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an set of chat controls configured for an existing Amazon Q Business
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_chat_controls_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_chat_controls_configuration)
         """
 
     def update_data_source(
         self,
         *,
         applicationId: str,
-        dataSourceId: str,
         indexId: str,
+        dataSourceId: str,
+        displayName: str = ...,
         configuration: Mapping[str, Any] = ...,
+        vpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
         description: str = ...,
-        displayName: str = ...,
-        documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,
-        roleArn: str = ...,
         syncSchedule: str = ...,
-        vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
+        roleArn: str = ...,
+        documentEnrichmentConfiguration: DocumentEnrichmentConfigurationUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing Amazon Q Business data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_data_source)
         """
 
     def update_index(
         self,
         *,
         applicationId: str,
         indexId: str,
-        capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
-        description: str = ...,
         displayName: str = ...,
+        description: str = ...,
+        capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,
         documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q Business index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_index)
         """
 
     def update_plugin(
         self,
         *,
         applicationId: str,
         pluginId: str,
-        authConfiguration: PluginAuthConfigurationTypeDef = ...,
         displayName: str = ...,
-        serverUrl: str = ...,
         state: PluginStateType = ...,
+        serverUrl: str = ...,
+        customPluginConfiguration: CustomPluginConfigurationTypeDef = ...,
+        authConfiguration: PluginAuthConfigurationUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q Business plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_plugin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_plugin)
         """
 
     def update_retriever(
         self,
         *,
         applicationId: str,
         retrieverId: str,
-        configuration: RetrieverConfigurationTypeDef = ...,
+        configuration: RetrieverConfigurationUnionTypeDef = ...,
         displayName: str = ...,
         roleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the retriever used for your Amazon Q Business application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_retriever)
@@ -862,34 +870,35 @@
         """
 
     def update_user(
         self,
         *,
         applicationId: str,
         userId: str,
-        userAliasesToDelete: Sequence[UserAliasTypeDef] = ...,
         userAliasesToUpdate: Sequence[UserAliasTypeDef] = ...,
+        userAliasesToDelete: Sequence[UserAliasTypeDef] = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Updates a information associated with a user id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_user)
         """
 
     def update_web_experience(
         self,
         *,
         applicationId: str,
         webExperienceId: str,
+        roleArn: str = ...,
         authenticationConfiguration: WebExperienceAuthConfigurationTypeDef = ...,
-        samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
-        subtitle: str = ...,
         title: str = ...,
+        subtitle: str = ...,
         welcomeMessage: str = ...,
+        samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,
     ) -> Dict[str, Any]:
         """
         Updates an Amazon Q Business web experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client.update_web_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/client/#update_web_experience)
         """
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/literals.py` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 Type annotations for qbusiness service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_qbusiness.literals import ActionPayloadFieldTypeType
+    from mypy_boto3_qbusiness.literals import APISchemaTypeType
 
-    data: ActionPayloadFieldTypeType = "ARRAY"
+    data: APISchemaTypeType = "OPEN_API_V3"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "APISchemaTypeType",
     "ActionPayloadFieldTypeType",
     "ApplicationStatusType",
     "AttachmentStatusType",
     "AttachmentsControlModeType",
     "AttributeTypeType",
     "AttributeValueOperatorType",
     "ChatModeType",
@@ -35,14 +36,15 @@
     "DocumentContentOperatorType",
     "DocumentEnrichmentConditionOperatorType",
     "DocumentStatusType",
     "ErrorCodeType",
     "GetChatControlsConfigurationPaginatorName",
     "GroupStatusType",
     "IndexStatusType",
+    "IndexTypeType",
     "ListApplicationsPaginatorName",
     "ListConversationsPaginatorName",
     "ListDataSourceSyncJobsPaginatorName",
     "ListDataSourcesPaginatorName",
     "ListDocumentsPaginatorName",
     "ListGroupsPaginatorName",
     "ListIndicesPaginatorName",
@@ -52,14 +54,15 @@
     "ListWebExperiencesPaginatorName",
     "MemberRelationType",
     "MembershipTypeType",
     "MessageTypeType",
     "MessageUsefulnessReasonType",
     "MessageUsefulnessType",
     "NumberAttributeBoostingTypeType",
+    "PluginBuildStatusType",
     "PluginStateType",
     "PluginTypeType",
     "ReadAccessTypeType",
     "ResponseScopeType",
     "RetrieverStatusType",
     "RetrieverTypeType",
     "RuleTypeType",
@@ -70,14 +73,15 @@
     "QBusinessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+APISchemaTypeType = Literal["OPEN_API_V3"]
 ActionPayloadFieldTypeType = Literal["ARRAY", "BOOLEAN", "NUMBER", "STRING"]
 ApplicationStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 AttachmentStatusType = Literal["FAILED", "SUCCEEDED"]
 AttachmentsControlModeType = Literal["DISABLED", "ENABLED"]
 AttributeTypeType = Literal["DATE", "NUMBER", "STRING", "STRING_LIST"]
 AttributeValueOperatorType = Literal["DELETE"]
 ChatModeType = Literal["CREATOR_MODE", "PLUGIN_MODE", "RETRIEVAL_MODE"]
@@ -127,14 +131,15 @@
     "RECEIVED",
     "UPDATED",
 ]
 ErrorCodeType = Literal["InternalError", "InvalidRequest", "ResourceInactive", "ResourceNotFound"]
 GetChatControlsConfigurationPaginatorName = Literal["get_chat_controls_configuration"]
 GroupStatusType = Literal["DELETED", "DELETING", "FAILED", "PROCESSING", "SUCCEEDED"]
 IndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
+IndexTypeType = Literal["ENTERPRISE", "STARTER"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListConversationsPaginatorName = Literal["list_conversations"]
 ListDataSourceSyncJobsPaginatorName = Literal["list_data_source_sync_jobs"]
 ListDataSourcesPaginatorName = Literal["list_data_sources"]
 ListDocumentsPaginatorName = Literal["list_documents"]
 ListGroupsPaginatorName = Literal["list_groups"]
 ListIndicesPaginatorName = Literal["list_indices"]
@@ -157,16 +162,25 @@
     "NOT_FACTUALLY_CORRECT",
     "NOT_HELPFUL",
     "OTHER",
     "RELEVANT_SOURCES",
 ]
 MessageUsefulnessType = Literal["NOT_USEFUL", "USEFUL"]
 NumberAttributeBoostingTypeType = Literal["PRIORITIZE_LARGER_VALUES", "PRIORITIZE_SMALLER_VALUES"]
+PluginBuildStatusType = Literal[
+    "CREATE_FAILED",
+    "CREATE_IN_PROGRESS",
+    "DELETE_FAILED",
+    "DELETE_IN_PROGRESS",
+    "READY",
+    "UPDATE_FAILED",
+    "UPDATE_IN_PROGRESS",
+]
 PluginStateType = Literal["DISABLED", "ENABLED"]
-PluginTypeType = Literal["JIRA", "SALESFORCE", "SERVICE_NOW", "ZENDESK"]
+PluginTypeType = Literal["CUSTOM", "JIRA", "SALESFORCE", "SERVICE_NOW", "ZENDESK"]
 ReadAccessTypeType = Literal["ALLOW", "DENY"]
 ResponseScopeType = Literal["ENTERPRISE_CONTENT_ONLY", "EXTENDED_KNOWLEDGE_ENABLED"]
 RetrieverStatusType = Literal["ACTIVE", "CREATING", "FAILED"]
 RetrieverTypeType = Literal["KENDRA_INDEX", "NATIVE_INDEX"]
 RuleTypeType = Literal["CONTENT_BLOCKER_RULE", "CONTENT_RETRIEVAL_RULE"]
 StatusType = Literal["DISABLED", "ENABLED"]
 StringAttributeValueBoostingLevelType = Literal["HIGH", "LOW", "MEDIUM", "VERY_HIGH"]
@@ -477,14 +491,15 @@
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
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/literals.pyi` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 Type annotations for qbusiness service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_qbusiness.literals import ActionPayloadFieldTypeType
+    from mypy_boto3_qbusiness.literals import APISchemaTypeType
 
-    data: ActionPayloadFieldTypeType = "ARRAY"
+    data: APISchemaTypeType = "OPEN_API_V3"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "APISchemaTypeType",
     "ActionPayloadFieldTypeType",
     "ApplicationStatusType",
     "AttachmentStatusType",
     "AttachmentsControlModeType",
     "AttributeTypeType",
     "AttributeValueOperatorType",
     "ChatModeType",
@@ -35,14 +36,15 @@
     "DocumentContentOperatorType",
     "DocumentEnrichmentConditionOperatorType",
     "DocumentStatusType",
     "ErrorCodeType",
     "GetChatControlsConfigurationPaginatorName",
     "GroupStatusType",
     "IndexStatusType",
+    "IndexTypeType",
     "ListApplicationsPaginatorName",
     "ListConversationsPaginatorName",
     "ListDataSourceSyncJobsPaginatorName",
     "ListDataSourcesPaginatorName",
     "ListDocumentsPaginatorName",
     "ListGroupsPaginatorName",
     "ListIndicesPaginatorName",
@@ -52,14 +54,15 @@
     "ListWebExperiencesPaginatorName",
     "MemberRelationType",
     "MembershipTypeType",
     "MessageTypeType",
     "MessageUsefulnessReasonType",
     "MessageUsefulnessType",
     "NumberAttributeBoostingTypeType",
+    "PluginBuildStatusType",
     "PluginStateType",
     "PluginTypeType",
     "ReadAccessTypeType",
     "ResponseScopeType",
     "RetrieverStatusType",
     "RetrieverTypeType",
     "RuleTypeType",
@@ -70,14 +73,15 @@
     "QBusinessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+APISchemaTypeType = Literal["OPEN_API_V3"]
 ActionPayloadFieldTypeType = Literal["ARRAY", "BOOLEAN", "NUMBER", "STRING"]
 ApplicationStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 AttachmentStatusType = Literal["FAILED", "SUCCEEDED"]
 AttachmentsControlModeType = Literal["DISABLED", "ENABLED"]
 AttributeTypeType = Literal["DATE", "NUMBER", "STRING", "STRING_LIST"]
 AttributeValueOperatorType = Literal["DELETE"]
 ChatModeType = Literal["CREATOR_MODE", "PLUGIN_MODE", "RETRIEVAL_MODE"]
@@ -127,14 +131,15 @@
     "RECEIVED",
     "UPDATED",
 ]
 ErrorCodeType = Literal["InternalError", "InvalidRequest", "ResourceInactive", "ResourceNotFound"]
 GetChatControlsConfigurationPaginatorName = Literal["get_chat_controls_configuration"]
 GroupStatusType = Literal["DELETED", "DELETING", "FAILED", "PROCESSING", "SUCCEEDED"]
 IndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
+IndexTypeType = Literal["ENTERPRISE", "STARTER"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListConversationsPaginatorName = Literal["list_conversations"]
 ListDataSourceSyncJobsPaginatorName = Literal["list_data_source_sync_jobs"]
 ListDataSourcesPaginatorName = Literal["list_data_sources"]
 ListDocumentsPaginatorName = Literal["list_documents"]
 ListGroupsPaginatorName = Literal["list_groups"]
 ListIndicesPaginatorName = Literal["list_indices"]
@@ -157,16 +162,25 @@
     "NOT_FACTUALLY_CORRECT",
     "NOT_HELPFUL",
     "OTHER",
     "RELEVANT_SOURCES",
 ]
 MessageUsefulnessType = Literal["NOT_USEFUL", "USEFUL"]
 NumberAttributeBoostingTypeType = Literal["PRIORITIZE_LARGER_VALUES", "PRIORITIZE_SMALLER_VALUES"]
+PluginBuildStatusType = Literal[
+    "CREATE_FAILED",
+    "CREATE_IN_PROGRESS",
+    "DELETE_FAILED",
+    "DELETE_IN_PROGRESS",
+    "READY",
+    "UPDATE_FAILED",
+    "UPDATE_IN_PROGRESS",
+]
 PluginStateType = Literal["DISABLED", "ENABLED"]
-PluginTypeType = Literal["JIRA", "SALESFORCE", "SERVICE_NOW", "ZENDESK"]
+PluginTypeType = Literal["CUSTOM", "JIRA", "SALESFORCE", "SERVICE_NOW", "ZENDESK"]
 ReadAccessTypeType = Literal["ALLOW", "DENY"]
 ResponseScopeType = Literal["ENTERPRISE_CONTENT_ONLY", "EXTENDED_KNOWLEDGE_ENABLED"]
 RetrieverStatusType = Literal["ACTIVE", "CREATING", "FAILED"]
 RetrieverTypeType = Literal["KENDRA_INDEX", "NATIVE_INDEX"]
 RuleTypeType = Literal["CONTENT_BLOCKER_RULE", "CONTENT_RETRIEVAL_RULE"]
 StatusType = Literal["DISABLED", "ENABLED"]
 StringAttributeValueBoostingLevelType = Literal["HIGH", "LOW", "MEDIUM", "VERY_HIGH"]
@@ -477,14 +491,15 @@
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
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/paginator.py` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ListApplicationsResponseTypeDef,
     ListConversationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListDocumentsResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListIndicesResponseTypeDef,
-    ListMessagesResponsePaginatorTypeDef,
+    ListMessagesResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListRetrieversResponseTypeDef,
     ListWebExperiencesResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
@@ -143,19 +143,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListDataSourceSyncJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listdatasourcesyncjobspaginator)
     """
 
     def paginate(
         self,
         *,
-        applicationId: str,
         dataSourceId: str,
+        applicationId: str,
         indexId: str,
-        endTime: TimestampTypeDef = ...,
         startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         statusFilter: DataSourceSyncJobStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDataSourceSyncJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListDataSourceSyncJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listdatasourcesyncjobspaginator)
         """
@@ -237,19 +237,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListMessages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listmessagespaginator)
     """
 
     def paginate(
         self,
         *,
-        applicationId: str,
         conversationId: str,
+        applicationId: str,
         userId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListMessagesResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listmessagespaginator)
         """
 
 
 class ListPluginsPaginator(Paginator):
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/paginator.pyi` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ListApplicationsResponseTypeDef,
     ListConversationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListDocumentsResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListIndicesResponseTypeDef,
-    ListMessagesResponsePaginatorTypeDef,
+    ListMessagesResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListRetrieversResponseTypeDef,
     ListWebExperiencesResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
@@ -138,19 +138,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListDataSourceSyncJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listdatasourcesyncjobspaginator)
     """
 
     def paginate(
         self,
         *,
-        applicationId: str,
         dataSourceId: str,
+        applicationId: str,
         indexId: str,
-        endTime: TimestampTypeDef = ...,
         startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         statusFilter: DataSourceSyncJobStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListDataSourceSyncJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListDataSourceSyncJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listdatasourcesyncjobspaginator)
         """
@@ -227,19 +227,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListMessages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listmessagespaginator)
     """
 
     def paginate(
         self,
         *,
-        applicationId: str,
         conversationId: str,
+        applicationId: str,
         userId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListMessagesResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Paginator.ListMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/paginators/#listmessagespaginator)
         """
 
 class ListPluginsPaginator(Paginator):
     """
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/type_defs.py` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for qbusiness service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_qbusiness.type_defs import ActionExecutionPayloadFieldPaginatorTypeDef
+    from mypy_boto3_qbusiness.type_defs import S3TypeDef
 
-    data: ActionExecutionPayloadFieldPaginatorTypeDef = ...
+    data: S3TypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
@@ -31,20 +31,22 @@
     DataSourceSyncJobStatusType,
     DocumentAttributeBoostingLevelType,
     DocumentEnrichmentConditionOperatorType,
     DocumentStatusType,
     ErrorCodeType,
     GroupStatusType,
     IndexStatusType,
+    IndexTypeType,
     MemberRelationType,
     MembershipTypeType,
     MessageTypeType,
     MessageUsefulnessReasonType,
     MessageUsefulnessType,
     NumberAttributeBoostingTypeType,
+    PluginBuildStatusType,
     PluginStateType,
     PluginTypeType,
     ReadAccessTypeType,
     ResponseScopeType,
     RetrieverStatusType,
     RetrieverTypeType,
     RuleTypeType,
@@ -64,23 +66,27 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActionExecutionPayloadFieldPaginatorTypeDef",
+    "S3TypeDef",
+    "ActionExecutionPayloadFieldExtraOutputTypeDef",
+    "ActionExecutionPayloadFieldOutputTypeDef",
     "ActionExecutionPayloadFieldTypeDef",
     "ActionReviewPayloadFieldAllowedValueTypeDef",
     "ApplicationTypeDef",
     "AppliedAttachmentsConfigurationTypeDef",
     "AppliedCreatorModeConfigurationTypeDef",
     "BlobTypeDef",
     "ErrorDetailTypeDef",
     "AttachmentsConfigurationTypeDef",
+    "AuthChallengeRequestTypeDef",
+    "AuthChallengeResponseTypeDef",
     "BasicAuthConfigurationTypeDef",
     "DeleteDocumentTypeDef",
     "ResponseMetadataTypeDef",
     "BlockedPhrasesConfigurationTypeDef",
     "BlockedPhrasesConfigurationUpdateTypeDef",
     "PluginConfigurationTypeDef",
     "ContentBlockerRuleTypeDef",
@@ -90,31 +96,33 @@
     "TagTypeDef",
     "DataSourceVpcConfigurationTypeDef",
     "IndexCapacityConfigurationTypeDef",
     "UserAliasTypeDef",
     "CreatorModeConfigurationTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
     "DataSourceTypeDef",
+    "DataSourceVpcConfigurationOutputTypeDef",
     "DateAttributeBoostingConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteChatControlsConfigurationRequestRequestTypeDef",
     "DeleteConversationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteIndexRequestRequestTypeDef",
     "DeletePluginRequestRequestTypeDef",
     "DeleteRetrieverRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteWebExperienceRequestRequestTypeDef",
     "NumberAttributeBoostingConfigurationTypeDef",
-    "StringAttributeBoostingConfigurationTypeDef",
+    "StringAttributeBoostingConfigurationOutputTypeDef",
     "StringListAttributeBoostingConfigurationTypeDef",
+    "StringAttributeBoostingConfigurationTypeDef",
+    "DocumentAttributeValueOutputTypeDef",
     "DocumentAttributeConfigurationTypeDef",
     "TimestampTypeDef",
-    "S3TypeDef",
     "GetApplicationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetChatControlsConfigurationRequestRequestTypeDef",
     "GetDataSourceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIndexRequestRequestTypeDef",
     "GetPluginRequestRequestTypeDef",
@@ -139,24 +147,29 @@
     "RetrieverTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebExperiencesRequestRequestTypeDef",
     "WebExperienceTypeDef",
     "OAuth2ClientCredentialConfigurationTypeDef",
     "PrincipalGroupTypeDef",
     "PrincipalUserTypeDef",
+    "UsersAndGroupsExtraOutputTypeDef",
+    "UsersAndGroupsOutputTypeDef",
     "UsersAndGroupsTypeDef",
     "SamlConfigurationTypeDef",
-    "TextSegmentTypeDef",
+    "SnippetExcerptTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ActionExecutionPaginatorTypeDef",
+    "APISchemaTypeDef",
+    "ActionExecutionExtraOutputTypeDef",
+    "ActionExecutionOutputTypeDef",
     "ActionExecutionTypeDef",
     "ActionReviewPayloadFieldTypeDef",
     "AttachmentInputTypeDef",
+    "DocumentContentTypeDef",
     "AttachmentOutputTypeDef",
     "DocumentDetailsTypeDef",
     "FailedDocumentTypeDef",
     "GroupStatusDetailTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
@@ -165,35 +178,40 @@
     "CreatePluginResponseTypeDef",
     "CreateRetrieverResponseTypeDef",
     "CreateWebExperienceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListApplicationsResponseTypeDef",
     "StartDataSourceSyncJobResponseTypeDef",
     "ChatModeConfigurationTypeDef",
+    "ContentRetrievalRuleExtraOutputTypeDef",
+    "ContentRetrievalRuleOutputTypeDef",
     "ContentRetrievalRuleTypeDef",
     "ListConversationsResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateWebExperienceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "GetUserResponseTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserResponseTypeDef",
     "DataSourceSyncJobTypeDef",
     "ListDataSourcesResponseTypeDef",
+    "DataSourceVpcConfigurationUnionTypeDef",
+    "DocumentAttributeBoostingConfigurationOutputTypeDef",
     "DocumentAttributeBoostingConfigurationTypeDef",
+    "DocumentAttributeConditionOutputTypeDef",
+    "DocumentAttributeTargetOutputTypeDef",
     "UpdateIndexRequestRequestTypeDef",
     "DocumentAttributeValueTypeDef",
     "ListDataSourceSyncJobsRequestRequestTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "MessageUsefulnessFeedbackTypeDef",
-    "DocumentContentTypeDef",
     "GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListConversationsRequestListConversationsPaginateTypeDef",
     "ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef",
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
@@ -205,91 +223,121 @@
     "GroupMembersTypeDef",
     "ListGroupsResponseTypeDef",
     "IndexStatisticsTypeDef",
     "ListIndicesResponseTypeDef",
     "ListPluginsResponseTypeDef",
     "ListRetrieversResponseTypeDef",
     "ListWebExperiencesResponseTypeDef",
+    "PluginAuthConfigurationOutputTypeDef",
     "PluginAuthConfigurationTypeDef",
     "PrincipalTypeDef",
     "WebExperienceAuthConfigurationTypeDef",
-    "SourceAttributionTypeDef",
+    "TextSegmentTypeDef",
+    "CustomPluginConfigurationTypeDef",
+    "ActionExecutionUnionTypeDef",
     "ActionReviewTypeDef",
     "ListDocumentsResponseTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
     "GetGroupResponseTypeDef",
     "ChatSyncInputRequestTypeDef",
+    "RuleConfigurationExtraOutputTypeDef",
+    "RuleConfigurationOutputTypeDef",
     "RuleConfigurationTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
+    "NativeIndexConfigurationOutputTypeDef",
     "NativeIndexConfigurationTypeDef",
+    "HookConfigurationOutputTypeDef",
+    "InlineDocumentEnrichmentConfigurationOutputTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "PutGroupRequestRequestTypeDef",
     "GetIndexResponseTypeDef",
-    "CreatePluginRequestRequestTypeDef",
-    "GetPluginResponseTypeDef",
-    "UpdatePluginRequestRequestTypeDef",
+    "PluginAuthConfigurationUnionTypeDef",
     "AccessControlTypeDef",
     "GetWebExperienceResponseTypeDef",
     "UpdateWebExperienceRequestRequestTypeDef",
-    "ChatSyncOutputTypeDef",
-    "MessagePaginatorTypeDef",
-    "MessageTypeDef",
+    "SourceAttributionTypeDef",
+    "CreatePluginRequestRequestTypeDef",
+    "GetPluginResponseTypeDef",
+    "UpdatePluginRequestRequestTypeDef",
+    "RuleExtraOutputTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
+    "RetrieverConfigurationOutputTypeDef",
     "RetrieverConfigurationTypeDef",
+    "DocumentEnrichmentConfigurationOutputTypeDef",
     "HookConfigurationTypeDef",
     "InlineDocumentEnrichmentConfigurationTypeDef",
     "AttributeFilterTypeDef",
     "AccessConfigurationTypeDef",
-    "ListMessagesResponsePaginatorTypeDef",
-    "ListMessagesResponseTypeDef",
+    "ChatSyncOutputTypeDef",
+    "MessageTypeDef",
+    "TopicConfigurationExtraOutputTypeDef",
+    "TopicConfigurationOutputTypeDef",
     "TopicConfigurationTypeDef",
-    "CreateRetrieverRequestRequestTypeDef",
     "GetRetrieverResponseTypeDef",
+    "CreateRetrieverRequestRequestTypeDef",
+    "RetrieverConfigurationUnionTypeDef",
     "UpdateRetrieverRequestRequestTypeDef",
+    "GetDataSourceResponseTypeDef",
     "DocumentEnrichmentConfigurationTypeDef",
+    "ListMessagesResponseTypeDef",
     "GetChatControlsConfigurationResponseTypeDef",
-    "UpdateChatControlsConfigurationRequestRequestTypeDef",
+    "TopicConfigurationUnionTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
+    "DocumentEnrichmentConfigurationUnionTypeDef",
     "DocumentTypeDef",
-    "GetDataSourceResponseTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
+    "UpdateChatControlsConfigurationRequestRequestTypeDef",
     "BatchPutDocumentRequestRequestTypeDef",
 )
 
-ActionExecutionPayloadFieldPaginatorTypeDef = TypedDict(
-    "ActionExecutionPayloadFieldPaginatorTypeDef",
+S3TypeDef = TypedDict(
+    "S3TypeDef",
+    {
+        "bucket": str,
+        "key": str,
+    },
+)
+ActionExecutionPayloadFieldExtraOutputTypeDef = TypedDict(
+    "ActionExecutionPayloadFieldExtraOutputTypeDef",
+    {
+        "value": Dict[str, Any],
+    },
+)
+ActionExecutionPayloadFieldOutputTypeDef = TypedDict(
+    "ActionExecutionPayloadFieldOutputTypeDef",
     {
         "value": Dict[str, Any],
     },
 )
 ActionExecutionPayloadFieldTypeDef = TypedDict(
     "ActionExecutionPayloadFieldTypeDef",
     {
         "value": Mapping[str, Any],
     },
 )
 ActionReviewPayloadFieldAllowedValueTypeDef = TypedDict(
     "ActionReviewPayloadFieldAllowedValueTypeDef",
     {
-        "displayValue": NotRequired[Dict[str, Any]],
         "value": NotRequired[Dict[str, Any]],
+        "displayValue": NotRequired[Dict[str, Any]],
     },
 )
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
+        "displayName": NotRequired[str],
         "applicationId": NotRequired[str],
         "createdAt": NotRequired[datetime],
-        "displayName": NotRequired[str],
-        "status": NotRequired[ApplicationStatusType],
         "updatedAt": NotRequired[datetime],
+        "status": NotRequired[ApplicationStatusType],
     },
 )
 AppliedAttachmentsConfigurationTypeDef = TypedDict(
     "AppliedAttachmentsConfigurationTypeDef",
     {
         "attachmentsControlMode": NotRequired[AttachmentsControlModeType],
     },
@@ -300,29 +348,41 @@
         "creatorModeControl": CreatorModeControlType,
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
-        "errorCode": NotRequired[ErrorCodeType],
         "errorMessage": NotRequired[str],
+        "errorCode": NotRequired[ErrorCodeType],
     },
 )
 AttachmentsConfigurationTypeDef = TypedDict(
     "AttachmentsConfigurationTypeDef",
     {
         "attachmentsControlMode": AttachmentsControlModeType,
     },
 )
+AuthChallengeRequestTypeDef = TypedDict(
+    "AuthChallengeRequestTypeDef",
+    {
+        "authorizationUrl": str,
+    },
+)
+AuthChallengeResponseTypeDef = TypedDict(
+    "AuthChallengeResponseTypeDef",
+    {
+        "responseMap": Mapping[str, str],
+    },
+)
 BasicAuthConfigurationTypeDef = TypedDict(
     "BasicAuthConfigurationTypeDef",
     {
-        "roleArn": str,
         "secretArn": str,
+        "roleArn": str,
     },
 )
 DeleteDocumentTypeDef = TypedDict(
     "DeleteDocumentTypeDef",
     {
         "documentId": str,
     },
@@ -363,24 +423,24 @@
     {
         "systemMessageOverride": NotRequired[str],
     },
 )
 EligibleDataSourceTypeDef = TypedDict(
     "EligibleDataSourceTypeDef",
     {
-        "dataSourceId": NotRequired[str],
         "indexId": NotRequired[str],
+        "dataSourceId": NotRequired[str],
     },
 )
 ConversationTypeDef = TypedDict(
     "ConversationTypeDef",
     {
         "conversationId": NotRequired[str],
-        "startTime": NotRequired[datetime],
         "title": NotRequired[str],
+        "startTime": NotRequired[datetime],
     },
 )
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "kmsKeyId": NotRequired[str],
     },
@@ -391,57 +451,64 @@
         "key": str,
         "value": str,
     },
 )
 DataSourceVpcConfigurationTypeDef = TypedDict(
     "DataSourceVpcConfigurationTypeDef",
     {
-        "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
+        "securityGroupIds": Sequence[str],
     },
 )
 IndexCapacityConfigurationTypeDef = TypedDict(
     "IndexCapacityConfigurationTypeDef",
     {
         "units": NotRequired[int],
     },
 )
 UserAliasTypeDef = TypedDict(
     "UserAliasTypeDef",
     {
         "userId": str,
-        "dataSourceId": NotRequired[str],
         "indexId": NotRequired[str],
+        "dataSourceId": NotRequired[str],
     },
 )
 CreatorModeConfigurationTypeDef = TypedDict(
     "CreatorModeConfigurationTypeDef",
     {
         "creatorModeControl": CreatorModeControlType,
     },
 )
 DataSourceSyncJobMetricsTypeDef = TypedDict(
     "DataSourceSyncJobMetricsTypeDef",
     {
         "documentsAdded": NotRequired[str],
+        "documentsModified": NotRequired[str],
         "documentsDeleted": NotRequired[str],
         "documentsFailed": NotRequired[str],
-        "documentsModified": NotRequired[str],
         "documentsScanned": NotRequired[str],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
-        "createdAt": NotRequired[datetime],
-        "dataSourceId": NotRequired[str],
         "displayName": NotRequired[str],
-        "status": NotRequired[DataSourceStatusType],
+        "dataSourceId": NotRequired[str],
         "type": NotRequired[str],
+        "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
+        "status": NotRequired[DataSourceStatusType],
+    },
+)
+DataSourceVpcConfigurationOutputTypeDef = TypedDict(
+    "DataSourceVpcConfigurationOutputTypeDef",
+    {
+        "subnetIds": List[str],
+        "securityGroupIds": List[str],
     },
 )
 DateAttributeBoostingConfigurationTypeDef = TypedDict(
     "DateAttributeBoostingConfigurationTypeDef",
     {
         "boostingLevel": DocumentAttributeBoostingLevelType,
         "boostingDurationInSeconds": NotRequired[int],
@@ -458,33 +525,33 @@
     {
         "applicationId": str,
     },
 )
 DeleteConversationRequestRequestTypeDef = TypedDict(
     "DeleteConversationRequestRequestTypeDef",
     {
-        "applicationId": str,
         "conversationId": str,
+        "applicationId": str,
         "userId": NotRequired[str],
     },
 )
 DeleteDataSourceRequestRequestTypeDef = TypedDict(
     "DeleteDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "dataSourceId": str,
         "indexId": str,
+        "dataSourceId": str,
     },
 )
 DeleteGroupRequestRequestTypeDef = TypedDict(
     "DeleteGroupRequestRequestTypeDef",
     {
         "applicationId": str,
-        "groupName": str,
         "indexId": str,
+        "groupName": str,
         "dataSourceId": NotRequired[str],
     },
 )
 DeleteIndexRequestRequestTypeDef = TypedDict(
     "DeleteIndexRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -522,43 +589,52 @@
 NumberAttributeBoostingConfigurationTypeDef = TypedDict(
     "NumberAttributeBoostingConfigurationTypeDef",
     {
         "boostingLevel": DocumentAttributeBoostingLevelType,
         "boostingType": NotRequired[NumberAttributeBoostingTypeType],
     },
 )
-StringAttributeBoostingConfigurationTypeDef = TypedDict(
-    "StringAttributeBoostingConfigurationTypeDef",
+StringAttributeBoostingConfigurationOutputTypeDef = TypedDict(
+    "StringAttributeBoostingConfigurationOutputTypeDef",
     {
         "boostingLevel": DocumentAttributeBoostingLevelType,
-        "attributeValueBoosting": NotRequired[Mapping[str, StringAttributeValueBoostingLevelType]],
+        "attributeValueBoosting": NotRequired[Dict[str, StringAttributeValueBoostingLevelType]],
     },
 )
 StringListAttributeBoostingConfigurationTypeDef = TypedDict(
     "StringListAttributeBoostingConfigurationTypeDef",
     {
         "boostingLevel": DocumentAttributeBoostingLevelType,
     },
 )
+StringAttributeBoostingConfigurationTypeDef = TypedDict(
+    "StringAttributeBoostingConfigurationTypeDef",
+    {
+        "boostingLevel": DocumentAttributeBoostingLevelType,
+        "attributeValueBoosting": NotRequired[Mapping[str, StringAttributeValueBoostingLevelType]],
+    },
+)
+DocumentAttributeValueOutputTypeDef = TypedDict(
+    "DocumentAttributeValueOutputTypeDef",
+    {
+        "stringValue": NotRequired[str],
+        "stringListValue": NotRequired[List[str]],
+        "longValue": NotRequired[int],
+        "dateValue": NotRequired[datetime],
+    },
+)
 DocumentAttributeConfigurationTypeDef = TypedDict(
     "DocumentAttributeConfigurationTypeDef",
     {
         "name": NotRequired[str],
-        "search": NotRequired[StatusType],
         "type": NotRequired[AttributeTypeType],
+        "search": NotRequired[StatusType],
     },
 )
 TimestampTypeDef = Union[datetime, str]
-S3TypeDef = TypedDict(
-    "S3TypeDef",
-    {
-        "bucket": str,
-        "key": str,
-    },
-)
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 PaginatorConfigTypeDef = TypedDict(
@@ -577,24 +653,24 @@
         "nextToken": NotRequired[str],
     },
 )
 GetDataSourceRequestRequestTypeDef = TypedDict(
     "GetDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "dataSourceId": str,
         "indexId": str,
+        "dataSourceId": str,
     },
 )
 GetGroupRequestRequestTypeDef = TypedDict(
     "GetGroupRequestRequestTypeDef",
     {
         "applicationId": str,
-        "groupName": str,
         "indexId": str,
+        "groupName": str,
         "dataSourceId": NotRequired[str],
     },
 )
 GetIndexRequestRequestTypeDef = TypedDict(
     "GetIndexRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -655,357 +731,397 @@
         "indexedTextBytes": NotRequired[int],
         "indexedTextDocumentCount": NotRequired[int],
     },
 )
 IndexTypeDef = TypedDict(
     "IndexTypeDef",
     {
-        "createdAt": NotRequired[datetime],
         "displayName": NotRequired[str],
         "indexId": NotRequired[str],
-        "status": NotRequired[IndexStatusType],
+        "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
+        "status": NotRequired[IndexStatusType],
     },
 )
 KendraIndexConfigurationTypeDef = TypedDict(
     "KendraIndexConfigurationTypeDef",
     {
         "indexId": str,
     },
 )
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListConversationsRequestRequestTypeDef = TypedDict(
     "ListConversationsRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
         "userId": NotRequired[str],
+        "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListDataSourcesRequestRequestTypeDef = TypedDict(
     "ListDataSourcesRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListDocumentsRequestRequestTypeDef = TypedDict(
     "ListDocumentsRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
         "dataSourceIds": NotRequired[Sequence[str]],
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListMessagesRequestRequestTypeDef = TypedDict(
     "ListMessagesRequestRequestTypeDef",
     {
-        "applicationId": str,
         "conversationId": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
+        "applicationId": str,
         "userId": NotRequired[str],
+        "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListPluginsRequestRequestTypeDef = TypedDict(
     "ListPluginsRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 PluginTypeDef = TypedDict(
     "PluginTypeDef",
     {
-        "createdAt": NotRequired[datetime],
-        "displayName": NotRequired[str],
         "pluginId": NotRequired[str],
+        "displayName": NotRequired[str],
+        "type": NotRequired[PluginTypeType],
         "serverUrl": NotRequired[str],
         "state": NotRequired[PluginStateType],
-        "type": NotRequired[PluginTypeType],
+        "buildStatus": NotRequired[PluginBuildStatusType],
+        "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
     },
 )
 ListRetrieversRequestRequestTypeDef = TypedDict(
     "ListRetrieversRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 RetrieverTypeDef = TypedDict(
     "RetrieverTypeDef",
     {
         "applicationId": NotRequired[str],
-        "displayName": NotRequired[str],
         "retrieverId": NotRequired[str],
-        "status": NotRequired[RetrieverStatusType],
         "type": NotRequired[RetrieverTypeType],
+        "status": NotRequired[RetrieverStatusType],
+        "displayName": NotRequired[str],
     },
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
     },
 )
 ListWebExperiencesRequestRequestTypeDef = TypedDict(
     "ListWebExperiencesRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 WebExperienceTypeDef = TypedDict(
     "WebExperienceTypeDef",
     {
+        "webExperienceId": NotRequired[str],
         "createdAt": NotRequired[datetime],
+        "updatedAt": NotRequired[datetime],
         "defaultEndpoint": NotRequired[str],
         "status": NotRequired[WebExperienceStatusType],
-        "updatedAt": NotRequired[datetime],
-        "webExperienceId": NotRequired[str],
     },
 )
 OAuth2ClientCredentialConfigurationTypeDef = TypedDict(
     "OAuth2ClientCredentialConfigurationTypeDef",
     {
-        "roleArn": str,
         "secretArn": str,
+        "roleArn": str,
     },
 )
 PrincipalGroupTypeDef = TypedDict(
     "PrincipalGroupTypeDef",
     {
         "access": ReadAccessTypeType,
-        "membershipType": NotRequired[MembershipTypeType],
         "name": NotRequired[str],
+        "membershipType": NotRequired[MembershipTypeType],
     },
 )
 PrincipalUserTypeDef = TypedDict(
     "PrincipalUserTypeDef",
     {
         "access": ReadAccessTypeType,
         "id": NotRequired[str],
         "membershipType": NotRequired[MembershipTypeType],
     },
 )
-UsersAndGroupsTypeDef = TypedDict(
-    "UsersAndGroupsTypeDef",
+UsersAndGroupsExtraOutputTypeDef = TypedDict(
+    "UsersAndGroupsExtraOutputTypeDef",
     {
+        "userIds": NotRequired[List[str]],
         "userGroups": NotRequired[List[str]],
+    },
+)
+UsersAndGroupsOutputTypeDef = TypedDict(
+    "UsersAndGroupsOutputTypeDef",
+    {
         "userIds": NotRequired[List[str]],
+        "userGroups": NotRequired[List[str]],
+    },
+)
+UsersAndGroupsTypeDef = TypedDict(
+    "UsersAndGroupsTypeDef",
+    {
+        "userIds": NotRequired[Sequence[str]],
+        "userGroups": NotRequired[Sequence[str]],
     },
 )
 SamlConfigurationTypeDef = TypedDict(
     "SamlConfigurationTypeDef",
     {
         "metadataXML": str,
         "roleArn": str,
         "userIdAttribute": str,
         "userGroupAttribute": NotRequired[str],
     },
 )
-TextSegmentTypeDef = TypedDict(
-    "TextSegmentTypeDef",
+SnippetExcerptTypeDef = TypedDict(
+    "SnippetExcerptTypeDef",
     {
-        "beginOffset": NotRequired[int],
-        "endOffset": NotRequired[int],
+        "text": NotRequired[str],
     },
 )
 StartDataSourceSyncJobRequestRequestTypeDef = TypedDict(
     "StartDataSourceSyncJobRequestRequestTypeDef",
     {
-        "applicationId": str,
         "dataSourceId": str,
+        "applicationId": str,
         "indexId": str,
     },
 )
 StopDataSourceSyncJobRequestRequestTypeDef = TypedDict(
     "StopDataSourceSyncJobRequestRequestTypeDef",
     {
-        "applicationId": str,
         "dataSourceId": str,
+        "applicationId": str,
         "indexId": str,
     },
 )
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tagKeys": Sequence[str],
     },
 )
-ActionExecutionPaginatorTypeDef = TypedDict(
-    "ActionExecutionPaginatorTypeDef",
+APISchemaTypeDef = TypedDict(
+    "APISchemaTypeDef",
     {
-        "payload": Dict[str, ActionExecutionPayloadFieldPaginatorTypeDef],
+        "payload": NotRequired[str],
+        "s3": NotRequired[S3TypeDef],
+    },
+)
+ActionExecutionExtraOutputTypeDef = TypedDict(
+    "ActionExecutionExtraOutputTypeDef",
+    {
+        "pluginId": str,
+        "payload": Dict[str, ActionExecutionPayloadFieldExtraOutputTypeDef],
         "payloadFieldNameSeparator": str,
+    },
+)
+ActionExecutionOutputTypeDef = TypedDict(
+    "ActionExecutionOutputTypeDef",
+    {
         "pluginId": str,
+        "payload": Dict[str, ActionExecutionPayloadFieldOutputTypeDef],
+        "payloadFieldNameSeparator": str,
     },
 )
 ActionExecutionTypeDef = TypedDict(
     "ActionExecutionTypeDef",
     {
+        "pluginId": str,
         "payload": Mapping[str, ActionExecutionPayloadFieldTypeDef],
         "payloadFieldNameSeparator": str,
-        "pluginId": str,
     },
 )
 ActionReviewPayloadFieldTypeDef = TypedDict(
     "ActionReviewPayloadFieldTypeDef",
     {
-        "allowedValues": NotRequired[List[ActionReviewPayloadFieldAllowedValueTypeDef]],
         "displayName": NotRequired[str],
         "displayOrder": NotRequired[int],
-        "required": NotRequired[bool],
+        "displayDescription": NotRequired[str],
         "type": NotRequired[ActionPayloadFieldTypeType],
         "value": NotRequired[Dict[str, Any]],
+        "allowedValues": NotRequired[List[ActionReviewPayloadFieldAllowedValueTypeDef]],
+        "allowedFormat": NotRequired[str],
+        "required": NotRequired[bool],
     },
 )
 AttachmentInputTypeDef = TypedDict(
     "AttachmentInputTypeDef",
     {
-        "data": BlobTypeDef,
         "name": str,
+        "data": BlobTypeDef,
+    },
+)
+DocumentContentTypeDef = TypedDict(
+    "DocumentContentTypeDef",
+    {
+        "blob": NotRequired[BlobTypeDef],
+        "s3": NotRequired[S3TypeDef],
     },
 )
 AttachmentOutputTypeDef = TypedDict(
     "AttachmentOutputTypeDef",
     {
-        "error": NotRequired[ErrorDetailTypeDef],
         "name": NotRequired[str],
         "status": NotRequired[AttachmentStatusType],
+        "error": NotRequired[ErrorDetailTypeDef],
     },
 )
 DocumentDetailsTypeDef = TypedDict(
     "DocumentDetailsTypeDef",
     {
-        "createdAt": NotRequired[datetime],
         "documentId": NotRequired[str],
-        "error": NotRequired[ErrorDetailTypeDef],
         "status": NotRequired[DocumentStatusType],
+        "error": NotRequired[ErrorDetailTypeDef],
+        "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
     },
 )
 FailedDocumentTypeDef = TypedDict(
     "FailedDocumentTypeDef",
     {
-        "dataSourceId": NotRequired[str],
-        "error": NotRequired[ErrorDetailTypeDef],
         "id": NotRequired[str],
+        "error": NotRequired[ErrorDetailTypeDef],
+        "dataSourceId": NotRequired[str],
     },
 )
 GroupStatusDetailTypeDef = TypedDict(
     "GroupStatusDetailTypeDef",
     {
-        "errorDetail": NotRequired[ErrorDetailTypeDef],
-        "lastUpdatedAt": NotRequired[datetime],
         "status": NotRequired[GroupStatusType],
+        "lastUpdatedAt": NotRequired[datetime],
+        "errorDetail": NotRequired[ErrorDetailTypeDef],
     },
 )
 UpdateApplicationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
-        "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
-        "description": NotRequired[str],
+        "identityCenterInstanceArn": NotRequired[str],
         "displayName": NotRequired[str],
+        "description": NotRequired[str],
         "roleArn": NotRequired[str],
+        "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
     },
 )
 BatchDeleteDocumentRequestRequestTypeDef = TypedDict(
     "BatchDeleteDocumentRequestRequestTypeDef",
     {
         "applicationId": str,
-        "documents": Sequence[DeleteDocumentTypeDef],
         "indexId": str,
+        "documents": Sequence[DeleteDocumentTypeDef],
         "dataSourceSyncId": NotRequired[str],
     },
 )
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
-        "applicationArn": str,
         "applicationId": str,
+        "applicationArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateDataSourceResponseTypeDef = TypedDict(
     "CreateDataSourceResponseTypeDef",
     {
-        "dataSourceArn": str,
         "dataSourceId": str,
+        "dataSourceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateIndexResponseTypeDef = TypedDict(
     "CreateIndexResponseTypeDef",
     {
-        "indexArn": str,
         "indexId": str,
+        "indexArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreatePluginResponseTypeDef = TypedDict(
     "CreatePluginResponseTypeDef",
     {
-        "pluginArn": str,
         "pluginId": str,
+        "pluginArn": str,
+        "buildStatus": PluginBuildStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateRetrieverResponseTypeDef = TypedDict(
     "CreateRetrieverResponseTypeDef",
     {
-        "retrieverArn": str,
         "retrieverId": str,
+        "retrieverArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateWebExperienceResponseTypeDef = TypedDict(
     "CreateWebExperienceResponseTypeDef",
     {
-        "webExperienceArn": str,
         "webExperienceId": str,
+        "webExperienceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
-        "applications": List[ApplicationTypeDef],
         "nextToken": str,
+        "applications": List[ApplicationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartDataSourceSyncJobResponseTypeDef = TypedDict(
     "StartDataSourceSyncJobResponseTypeDef",
     {
         "executionId": str,
@@ -1014,70 +1130,82 @@
 )
 ChatModeConfigurationTypeDef = TypedDict(
     "ChatModeConfigurationTypeDef",
     {
         "pluginConfiguration": NotRequired[PluginConfigurationTypeDef],
     },
 )
+ContentRetrievalRuleExtraOutputTypeDef = TypedDict(
+    "ContentRetrievalRuleExtraOutputTypeDef",
+    {
+        "eligibleDataSources": NotRequired[List[EligibleDataSourceTypeDef]],
+    },
+)
+ContentRetrievalRuleOutputTypeDef = TypedDict(
+    "ContentRetrievalRuleOutputTypeDef",
+    {
+        "eligibleDataSources": NotRequired[List[EligibleDataSourceTypeDef]],
+    },
+)
 ContentRetrievalRuleTypeDef = TypedDict(
     "ContentRetrievalRuleTypeDef",
     {
-        "eligibleDataSources": NotRequired[List[EligibleDataSourceTypeDef]],
+        "eligibleDataSources": NotRequired[Sequence[EligibleDataSourceTypeDef]],
     },
 )
 ListConversationsResponseTypeDef = TypedDict(
     "ListConversationsResponseTypeDef",
     {
-        "conversations": List[ConversationTypeDef],
         "nextToken": str,
+        "conversations": List[ConversationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
-        "applicationArn": str,
-        "applicationId": str,
-        "attachmentsConfiguration": AppliedAttachmentsConfigurationTypeDef,
-        "createdAt": datetime,
-        "description": str,
         "displayName": str,
-        "encryptionConfiguration": EncryptionConfigurationTypeDef,
-        "error": ErrorDetailTypeDef,
+        "applicationId": str,
+        "applicationArn": str,
         "identityCenterApplicationArn": str,
         "roleArn": str,
         "status": ApplicationStatusType,
+        "description": str,
+        "encryptionConfiguration": EncryptionConfigurationTypeDef,
+        "createdAt": datetime,
         "updatedAt": datetime,
+        "error": ErrorDetailTypeDef,
+        "attachmentsConfiguration": AppliedAttachmentsConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateApplicationRequestRequestTypeDef = TypedDict(
     "CreateApplicationRequestRequestTypeDef",
     {
         "displayName": str,
-        "roleArn": str,
-        "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
-        "clientToken": NotRequired[str],
+        "roleArn": NotRequired[str],
+        "identityCenterInstanceArn": NotRequired[str],
         "description": NotRequired[str],
         "encryptionConfiguration": NotRequired[EncryptionConfigurationTypeDef],
-        "identityCenterInstanceArn": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
+        "clientToken": NotRequired[str],
+        "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
     },
 )
 CreateWebExperienceRequestRequestTypeDef = TypedDict(
     "CreateWebExperienceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "clientToken": NotRequired[str],
-        "roleArn": NotRequired[str],
-        "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
-        "subtitle": NotRequired[str],
-        "tags": NotRequired[Sequence[TagTypeDef]],
         "title": NotRequired[str],
+        "subtitle": NotRequired[str],
         "welcomeMessage": NotRequired[str],
+        "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
+        "roleArn": NotRequired[str],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+        "clientToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1091,143 +1219,165 @@
     },
 )
 CreateIndexRequestRequestTypeDef = TypedDict(
     "CreateIndexRequestRequestTypeDef",
     {
         "applicationId": str,
         "displayName": str,
-        "capacityConfiguration": NotRequired[IndexCapacityConfigurationTypeDef],
-        "clientToken": NotRequired[str],
+        "type": NotRequired[IndexTypeType],
         "description": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
+        "capacityConfiguration": NotRequired[IndexCapacityConfigurationTypeDef],
+        "clientToken": NotRequired[str],
     },
 )
 CreateUserRequestRequestTypeDef = TypedDict(
     "CreateUserRequestRequestTypeDef",
     {
         "applicationId": str,
         "userId": str,
-        "clientToken": NotRequired[str],
         "userAliases": NotRequired[Sequence[UserAliasTypeDef]],
+        "clientToken": NotRequired[str],
     },
 )
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "userAliases": List[UserAliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateUserRequestRequestTypeDef = TypedDict(
     "UpdateUserRequestRequestTypeDef",
     {
         "applicationId": str,
         "userId": str,
-        "userAliasesToDelete": NotRequired[Sequence[UserAliasTypeDef]],
         "userAliasesToUpdate": NotRequired[Sequence[UserAliasTypeDef]],
+        "userAliasesToDelete": NotRequired[Sequence[UserAliasTypeDef]],
     },
 )
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "userAliasesAdded": List[UserAliasTypeDef],
-        "userAliasesDeleted": List[UserAliasTypeDef],
         "userAliasesUpdated": List[UserAliasTypeDef],
+        "userAliasesDeleted": List[UserAliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DataSourceSyncJobTypeDef = TypedDict(
     "DataSourceSyncJobTypeDef",
     {
-        "dataSourceErrorCode": NotRequired[str],
-        "endTime": NotRequired[datetime],
-        "error": NotRequired[ErrorDetailTypeDef],
         "executionId": NotRequired[str],
-        "metrics": NotRequired[DataSourceSyncJobMetricsTypeDef],
         "startTime": NotRequired[datetime],
+        "endTime": NotRequired[datetime],
         "status": NotRequired[DataSourceSyncJobStatusType],
+        "error": NotRequired[ErrorDetailTypeDef],
+        "dataSourceErrorCode": NotRequired[str],
+        "metrics": NotRequired[DataSourceSyncJobMetricsTypeDef],
     },
 )
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "dataSources": List[DataSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DataSourceVpcConfigurationUnionTypeDef = Union[
+    DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
+]
+DocumentAttributeBoostingConfigurationOutputTypeDef = TypedDict(
+    "DocumentAttributeBoostingConfigurationOutputTypeDef",
+    {
+        "numberConfiguration": NotRequired[NumberAttributeBoostingConfigurationTypeDef],
+        "stringConfiguration": NotRequired[StringAttributeBoostingConfigurationOutputTypeDef],
+        "dateConfiguration": NotRequired[DateAttributeBoostingConfigurationTypeDef],
+        "stringListConfiguration": NotRequired[StringListAttributeBoostingConfigurationTypeDef],
+    },
+)
 DocumentAttributeBoostingConfigurationTypeDef = TypedDict(
     "DocumentAttributeBoostingConfigurationTypeDef",
     {
-        "dateConfiguration": NotRequired[DateAttributeBoostingConfigurationTypeDef],
         "numberConfiguration": NotRequired[NumberAttributeBoostingConfigurationTypeDef],
         "stringConfiguration": NotRequired[StringAttributeBoostingConfigurationTypeDef],
+        "dateConfiguration": NotRequired[DateAttributeBoostingConfigurationTypeDef],
         "stringListConfiguration": NotRequired[StringListAttributeBoostingConfigurationTypeDef],
     },
 )
+DocumentAttributeConditionOutputTypeDef = TypedDict(
+    "DocumentAttributeConditionOutputTypeDef",
+    {
+        "key": str,
+        "operator": DocumentEnrichmentConditionOperatorType,
+        "value": NotRequired[DocumentAttributeValueOutputTypeDef],
+    },
+)
+DocumentAttributeTargetOutputTypeDef = TypedDict(
+    "DocumentAttributeTargetOutputTypeDef",
+    {
+        "key": str,
+        "value": NotRequired[DocumentAttributeValueOutputTypeDef],
+        "attributeValueOperator": NotRequired[Literal["DELETE"]],
+    },
+)
 UpdateIndexRequestRequestTypeDef = TypedDict(
     "UpdateIndexRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
-        "capacityConfiguration": NotRequired[IndexCapacityConfigurationTypeDef],
-        "description": NotRequired[str],
         "displayName": NotRequired[str],
+        "description": NotRequired[str],
+        "capacityConfiguration": NotRequired[IndexCapacityConfigurationTypeDef],
         "documentAttributeConfigurations": NotRequired[
             Sequence[DocumentAttributeConfigurationTypeDef]
         ],
     },
 )
 DocumentAttributeValueTypeDef = TypedDict(
     "DocumentAttributeValueTypeDef",
     {
-        "dateValue": NotRequired[TimestampTypeDef],
-        "longValue": NotRequired[int],
-        "stringListValue": NotRequired[Sequence[str]],
         "stringValue": NotRequired[str],
+        "stringListValue": NotRequired[Sequence[str]],
+        "longValue": NotRequired[int],
+        "dateValue": NotRequired[TimestampTypeDef],
     },
 )
 ListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
     "ListDataSourceSyncJobsRequestRequestTypeDef",
     {
-        "applicationId": str,
         "dataSourceId": str,
+        "applicationId": str,
         "indexId": str,
-        "endTime": NotRequired[TimestampTypeDef],
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
         "startTime": NotRequired[TimestampTypeDef],
+        "endTime": NotRequired[TimestampTypeDef],
         "statusFilter": NotRequired[DataSourceSyncJobStatusType],
     },
 )
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
         "updatedEarlierThan": TimestampTypeDef,
         "dataSourceId": NotRequired[str],
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 MessageUsefulnessFeedbackTypeDef = TypedDict(
     "MessageUsefulnessFeedbackTypeDef",
     {
-        "submittedAt": TimestampTypeDef,
         "usefulness": MessageUsefulnessType,
-        "comment": NotRequired[str],
+        "submittedAt": TimestampTypeDef,
         "reason": NotRequired[MessageUsefulnessReasonType],
-    },
-)
-DocumentContentTypeDef = TypedDict(
-    "DocumentContentTypeDef",
-    {
-        "blob": NotRequired[BlobTypeDef],
-        "s3": NotRequired[S3TypeDef],
+        "comment": NotRequired[str],
     },
 )
 GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef = TypedDict(
     "GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef",
     {
         "applicationId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1246,19 +1396,19 @@
         "userId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef = TypedDict(
     "ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef",
     {
-        "applicationId": str,
         "dataSourceId": str,
+        "applicationId": str,
         "indexId": str,
-        "endTime": NotRequired[TimestampTypeDef],
         "startTime": NotRequired[TimestampTypeDef],
+        "endTime": NotRequired[TimestampTypeDef],
         "statusFilter": NotRequired[DataSourceSyncJobStatusType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     {
@@ -1292,16 +1442,16 @@
         "applicationId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListMessagesRequestListMessagesPaginateTypeDef = TypedDict(
     "ListMessagesRequestListMessagesPaginateTypeDef",
     {
-        "applicationId": str,
         "conversationId": str,
+        "applicationId": str,
         "userId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
     "ListPluginsRequestListPluginsPaginateTypeDef",
     {
@@ -1329,97 +1479,114 @@
         "memberGroups": NotRequired[Sequence[MemberGroupTypeDef]],
         "memberUsers": NotRequired[Sequence[MemberUserTypeDef]],
     },
 )
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
-        "items": List[GroupSummaryTypeDef],
         "nextToken": str,
+        "items": List[GroupSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 IndexStatisticsTypeDef = TypedDict(
     "IndexStatisticsTypeDef",
     {
         "textDocumentStatistics": NotRequired[TextDocumentStatisticsTypeDef],
     },
 )
 ListIndicesResponseTypeDef = TypedDict(
     "ListIndicesResponseTypeDef",
     {
-        "indices": List[IndexTypeDef],
         "nextToken": str,
+        "indices": List[IndexTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListPluginsResponseTypeDef = TypedDict(
     "ListPluginsResponseTypeDef",
     {
         "nextToken": str,
         "plugins": List[PluginTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListRetrieversResponseTypeDef = TypedDict(
     "ListRetrieversResponseTypeDef",
     {
-        "nextToken": str,
         "retrievers": List[RetrieverTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWebExperiencesResponseTypeDef = TypedDict(
     "ListWebExperiencesResponseTypeDef",
     {
-        "nextToken": str,
         "webExperiences": List[WebExperienceTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+PluginAuthConfigurationOutputTypeDef = TypedDict(
+    "PluginAuthConfigurationOutputTypeDef",
+    {
+        "basicAuthConfiguration": NotRequired[BasicAuthConfigurationTypeDef],
+        "oAuth2ClientCredentialConfiguration": NotRequired[
+            OAuth2ClientCredentialConfigurationTypeDef
+        ],
+        "noAuthConfiguration": NotRequired[Dict[str, Any]],
+    },
+)
 PluginAuthConfigurationTypeDef = TypedDict(
     "PluginAuthConfigurationTypeDef",
     {
         "basicAuthConfiguration": NotRequired[BasicAuthConfigurationTypeDef],
         "oAuth2ClientCredentialConfiguration": NotRequired[
             OAuth2ClientCredentialConfigurationTypeDef
         ],
+        "noAuthConfiguration": NotRequired[Mapping[str, Any]],
     },
 )
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
-        "group": NotRequired[PrincipalGroupTypeDef],
         "user": NotRequired[PrincipalUserTypeDef],
+        "group": NotRequired[PrincipalGroupTypeDef],
     },
 )
 WebExperienceAuthConfigurationTypeDef = TypedDict(
     "WebExperienceAuthConfigurationTypeDef",
     {
         "samlConfiguration": NotRequired[SamlConfigurationTypeDef],
     },
 )
-SourceAttributionTypeDef = TypedDict(
-    "SourceAttributionTypeDef",
+TextSegmentTypeDef = TypedDict(
+    "TextSegmentTypeDef",
     {
-        "citationNumber": NotRequired[int],
-        "snippet": NotRequired[str],
-        "textMessageSegments": NotRequired[List[TextSegmentTypeDef]],
-        "title": NotRequired[str],
-        "updatedAt": NotRequired[datetime],
-        "url": NotRequired[str],
+        "beginOffset": NotRequired[int],
+        "endOffset": NotRequired[int],
+        "snippetExcerpt": NotRequired[SnippetExcerptTypeDef],
+    },
+)
+CustomPluginConfigurationTypeDef = TypedDict(
+    "CustomPluginConfigurationTypeDef",
+    {
+        "description": str,
+        "apiSchemaType": Literal["OPEN_API_V3"],
+        "apiSchema": APISchemaTypeDef,
     },
 )
+ActionExecutionUnionTypeDef = Union[ActionExecutionTypeDef, ActionExecutionExtraOutputTypeDef]
 ActionReviewTypeDef = TypedDict(
     "ActionReviewTypeDef",
     {
-        "payload": NotRequired[Dict[str, ActionReviewPayloadFieldTypeDef]],
-        "payloadFieldNameSeparator": NotRequired[str],
         "pluginId": NotRequired[str],
         "pluginType": NotRequired[PluginTypeType],
+        "payload": NotRequired[Dict[str, ActionReviewPayloadFieldTypeDef]],
+        "payloadFieldNameSeparator": NotRequired[str],
     },
 )
 ListDocumentsResponseTypeDef = TypedDict(
     "ListDocumentsResponseTypeDef",
     {
         "documentDetailList": List[DocumentDetailsTypeDef],
         "nextToken": str,
@@ -1448,25 +1615,40 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ChatSyncInputRequestTypeDef = TypedDict(
     "ChatSyncInputRequestTypeDef",
     {
         "applicationId": str,
-        "actionExecution": NotRequired[ActionExecutionTypeDef],
+        "userId": NotRequired[str],
+        "userGroups": NotRequired[Sequence[str]],
+        "userMessage": NotRequired[str],
         "attachments": NotRequired[Sequence[AttachmentInputTypeDef]],
+        "actionExecution": NotRequired[ActionExecutionTypeDef],
+        "authChallengeResponse": NotRequired[AuthChallengeResponseTypeDef],
+        "conversationId": NotRequired[str],
+        "parentMessageId": NotRequired[str],
         "attributeFilter": NotRequired["AttributeFilterTypeDef"],
         "chatMode": NotRequired[ChatModeType],
         "chatModeConfiguration": NotRequired[ChatModeConfigurationTypeDef],
         "clientToken": NotRequired[str],
-        "conversationId": NotRequired[str],
-        "parentMessageId": NotRequired[str],
-        "userGroups": NotRequired[Sequence[str]],
-        "userId": NotRequired[str],
-        "userMessage": NotRequired[str],
+    },
+)
+RuleConfigurationExtraOutputTypeDef = TypedDict(
+    "RuleConfigurationExtraOutputTypeDef",
+    {
+        "contentBlockerRule": NotRequired[ContentBlockerRuleTypeDef],
+        "contentRetrievalRule": NotRequired[ContentRetrievalRuleExtraOutputTypeDef],
+    },
+)
+RuleConfigurationOutputTypeDef = TypedDict(
+    "RuleConfigurationOutputTypeDef",
+    {
+        "contentBlockerRule": NotRequired[ContentBlockerRuleTypeDef],
+        "contentRetrievalRule": NotRequired[ContentRetrievalRuleOutputTypeDef],
     },
 )
 RuleConfigurationTypeDef = TypedDict(
     "RuleConfigurationTypeDef",
     {
         "contentBlockerRule": NotRequired[ContentBlockerRuleTypeDef],
         "contentRetrievalRule": NotRequired[ContentRetrievalRuleTypeDef],
@@ -1476,37 +1658,63 @@
     "ListDataSourceSyncJobsResponseTypeDef",
     {
         "history": List[DataSourceSyncJobTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+NativeIndexConfigurationOutputTypeDef = TypedDict(
+    "NativeIndexConfigurationOutputTypeDef",
+    {
+        "indexId": str,
+        "boostingOverride": NotRequired[
+            Dict[str, DocumentAttributeBoostingConfigurationOutputTypeDef]
+        ],
+    },
+)
 NativeIndexConfigurationTypeDef = TypedDict(
     "NativeIndexConfigurationTypeDef",
     {
         "indexId": str,
         "boostingOverride": NotRequired[
             Mapping[str, DocumentAttributeBoostingConfigurationTypeDef]
         ],
     },
 )
+HookConfigurationOutputTypeDef = TypedDict(
+    "HookConfigurationOutputTypeDef",
+    {
+        "invocationCondition": NotRequired[DocumentAttributeConditionOutputTypeDef],
+        "lambdaArn": NotRequired[str],
+        "s3BucketName": NotRequired[str],
+        "roleArn": NotRequired[str],
+    },
+)
+InlineDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
+    "InlineDocumentEnrichmentConfigurationOutputTypeDef",
+    {
+        "condition": NotRequired[DocumentAttributeConditionOutputTypeDef],
+        "target": NotRequired[DocumentAttributeTargetOutputTypeDef],
+        "documentContentOperator": NotRequired[Literal["DELETE"]],
+    },
+)
 DocumentAttributeConditionTypeDef = TypedDict(
     "DocumentAttributeConditionTypeDef",
     {
         "key": str,
         "operator": DocumentEnrichmentConditionOperatorType,
         "value": NotRequired[DocumentAttributeValueTypeDef],
     },
 )
 DocumentAttributeTargetTypeDef = TypedDict(
     "DocumentAttributeTargetTypeDef",
     {
         "key": str,
-        "attributeValueOperator": NotRequired[Literal["DELETE"]],
         "value": NotRequired[DocumentAttributeValueTypeDef],
+        "attributeValueOperator": NotRequired[Literal["DELETE"]],
     },
 )
 DocumentAttributeTypeDef = TypedDict(
     "DocumentAttributeTypeDef",
     {
         "name": str,
         "value": DocumentAttributeValueTypeDef,
@@ -1514,382 +1722,446 @@
 )
 PutFeedbackRequestRequestTypeDef = TypedDict(
     "PutFeedbackRequestRequestTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
         "messageId": str,
+        "userId": NotRequired[str],
         "messageCopiedAt": NotRequired[TimestampTypeDef],
         "messageUsefulness": NotRequired[MessageUsefulnessFeedbackTypeDef],
-        "userId": NotRequired[str],
     },
 )
 PutGroupRequestRequestTypeDef = TypedDict(
     "PutGroupRequestRequestTypeDef",
     {
         "applicationId": str,
-        "groupMembers": GroupMembersTypeDef,
-        "groupName": str,
         "indexId": str,
+        "groupName": str,
         "type": MembershipTypeType,
+        "groupMembers": GroupMembersTypeDef,
         "dataSourceId": NotRequired[str],
     },
 )
 GetIndexResponseTypeDef = TypedDict(
     "GetIndexResponseTypeDef",
     {
         "applicationId": str,
-        "capacityConfiguration": IndexCapacityConfigurationTypeDef,
-        "createdAt": datetime,
-        "description": str,
+        "indexId": str,
         "displayName": str,
-        "documentAttributeConfigurations": List[DocumentAttributeConfigurationTypeDef],
-        "error": ErrorDetailTypeDef,
+        "type": IndexTypeType,
         "indexArn": str,
-        "indexId": str,
-        "indexStatistics": IndexStatisticsTypeDef,
         "status": IndexStatusType,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreatePluginRequestRequestTypeDef = TypedDict(
-    "CreatePluginRequestRequestTypeDef",
-    {
-        "applicationId": str,
-        "authConfiguration": PluginAuthConfigurationTypeDef,
-        "displayName": str,
-        "serverUrl": str,
-        "type": PluginTypeType,
-        "clientToken": NotRequired[str],
-        "tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
-GetPluginResponseTypeDef = TypedDict(
-    "GetPluginResponseTypeDef",
-    {
-        "applicationId": str,
-        "authConfiguration": PluginAuthConfigurationTypeDef,
+        "description": str,
         "createdAt": datetime,
-        "displayName": str,
-        "pluginArn": str,
-        "pluginId": str,
-        "serverUrl": str,
-        "state": PluginStateType,
-        "type": PluginTypeType,
         "updatedAt": datetime,
+        "capacityConfiguration": IndexCapacityConfigurationTypeDef,
+        "documentAttributeConfigurations": List[DocumentAttributeConfigurationTypeDef],
+        "error": ErrorDetailTypeDef,
+        "indexStatistics": IndexStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdatePluginRequestRequestTypeDef = TypedDict(
-    "UpdatePluginRequestRequestTypeDef",
-    {
-        "applicationId": str,
-        "pluginId": str,
-        "authConfiguration": NotRequired[PluginAuthConfigurationTypeDef],
-        "displayName": NotRequired[str],
-        "serverUrl": NotRequired[str],
-        "state": NotRequired[PluginStateType],
-    },
-)
+PluginAuthConfigurationUnionTypeDef = Union[
+    PluginAuthConfigurationTypeDef, PluginAuthConfigurationOutputTypeDef
+]
 AccessControlTypeDef = TypedDict(
     "AccessControlTypeDef",
     {
         "principals": Sequence[PrincipalTypeDef],
         "memberRelation": NotRequired[MemberRelationType],
     },
 )
 GetWebExperienceResponseTypeDef = TypedDict(
     "GetWebExperienceResponseTypeDef",
     {
         "applicationId": str,
-        "authenticationConfiguration": WebExperienceAuthConfigurationTypeDef,
-        "createdAt": datetime,
+        "webExperienceId": str,
+        "webExperienceArn": str,
         "defaultEndpoint": str,
-        "error": ErrorDetailTypeDef,
-        "roleArn": str,
-        "samplePromptsControlMode": WebExperienceSamplePromptsControlModeType,
         "status": WebExperienceStatusType,
-        "subtitle": str,
-        "title": str,
+        "createdAt": datetime,
         "updatedAt": datetime,
-        "webExperienceArn": str,
-        "webExperienceId": str,
+        "title": str,
+        "subtitle": str,
         "welcomeMessage": str,
+        "samplePromptsControlMode": WebExperienceSamplePromptsControlModeType,
+        "roleArn": str,
+        "authenticationConfiguration": WebExperienceAuthConfigurationTypeDef,
+        "error": ErrorDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateWebExperienceRequestRequestTypeDef = TypedDict(
     "UpdateWebExperienceRequestRequestTypeDef",
     {
         "applicationId": str,
         "webExperienceId": str,
+        "roleArn": NotRequired[str],
         "authenticationConfiguration": NotRequired[WebExperienceAuthConfigurationTypeDef],
-        "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
-        "subtitle": NotRequired[str],
         "title": NotRequired[str],
+        "subtitle": NotRequired[str],
         "welcomeMessage": NotRequired[str],
+        "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
     },
 )
-ChatSyncOutputTypeDef = TypedDict(
-    "ChatSyncOutputTypeDef",
+SourceAttributionTypeDef = TypedDict(
+    "SourceAttributionTypeDef",
     {
-        "actionReview": ActionReviewTypeDef,
-        "conversationId": str,
-        "failedAttachments": List[AttachmentOutputTypeDef],
-        "sourceAttributions": List[SourceAttributionTypeDef],
-        "systemMessage": str,
-        "systemMessageId": str,
-        "userMessageId": str,
+        "title": NotRequired[str],
+        "snippet": NotRequired[str],
+        "url": NotRequired[str],
+        "citationNumber": NotRequired[int],
+        "updatedAt": NotRequired[datetime],
+        "textMessageSegments": NotRequired[List[TextSegmentTypeDef]],
+    },
+)
+CreatePluginRequestRequestTypeDef = TypedDict(
+    "CreatePluginRequestRequestTypeDef",
+    {
+        "applicationId": str,
+        "displayName": str,
+        "type": PluginTypeType,
+        "authConfiguration": PluginAuthConfigurationTypeDef,
+        "serverUrl": NotRequired[str],
+        "customPluginConfiguration": NotRequired[CustomPluginConfigurationTypeDef],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+        "clientToken": NotRequired[str],
+    },
+)
+GetPluginResponseTypeDef = TypedDict(
+    "GetPluginResponseTypeDef",
+    {
+        "applicationId": str,
+        "pluginId": str,
+        "displayName": str,
+        "type": PluginTypeType,
+        "serverUrl": str,
+        "authConfiguration": PluginAuthConfigurationOutputTypeDef,
+        "customPluginConfiguration": CustomPluginConfigurationTypeDef,
+        "buildStatus": PluginBuildStatusType,
+        "pluginArn": str,
+        "state": PluginStateType,
+        "createdAt": datetime,
+        "updatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-MessagePaginatorTypeDef = TypedDict(
-    "MessagePaginatorTypeDef",
+UpdatePluginRequestRequestTypeDef = TypedDict(
+    "UpdatePluginRequestRequestTypeDef",
     {
-        "actionExecution": NotRequired[ActionExecutionPaginatorTypeDef],
-        "actionReview": NotRequired[ActionReviewTypeDef],
-        "attachments": NotRequired[List[AttachmentOutputTypeDef]],
-        "body": NotRequired[str],
-        "messageId": NotRequired[str],
-        "sourceAttribution": NotRequired[List[SourceAttributionTypeDef]],
-        "time": NotRequired[datetime],
-        "type": NotRequired[MessageTypeType],
+        "applicationId": str,
+        "pluginId": str,
+        "displayName": NotRequired[str],
+        "state": NotRequired[PluginStateType],
+        "serverUrl": NotRequired[str],
+        "customPluginConfiguration": NotRequired[CustomPluginConfigurationTypeDef],
+        "authConfiguration": NotRequired[PluginAuthConfigurationTypeDef],
     },
 )
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
+RuleExtraOutputTypeDef = TypedDict(
+    "RuleExtraOutputTypeDef",
     {
-        "actionExecution": NotRequired[ActionExecutionTypeDef],
-        "actionReview": NotRequired[ActionReviewTypeDef],
-        "attachments": NotRequired[List[AttachmentOutputTypeDef]],
-        "body": NotRequired[str],
-        "messageId": NotRequired[str],
-        "sourceAttribution": NotRequired[List[SourceAttributionTypeDef]],
-        "time": NotRequired[datetime],
-        "type": NotRequired[MessageTypeType],
+        "ruleType": RuleTypeType,
+        "includedUsersAndGroups": NotRequired[UsersAndGroupsExtraOutputTypeDef],
+        "excludedUsersAndGroups": NotRequired[UsersAndGroupsExtraOutputTypeDef],
+        "ruleConfiguration": NotRequired[RuleConfigurationExtraOutputTypeDef],
+    },
+)
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "ruleType": RuleTypeType,
+        "includedUsersAndGroups": NotRequired[UsersAndGroupsOutputTypeDef],
+        "excludedUsersAndGroups": NotRequired[UsersAndGroupsOutputTypeDef],
+        "ruleConfiguration": NotRequired[RuleConfigurationOutputTypeDef],
     },
 )
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "ruleType": RuleTypeType,
-        "excludedUsersAndGroups": NotRequired[UsersAndGroupsTypeDef],
         "includedUsersAndGroups": NotRequired[UsersAndGroupsTypeDef],
+        "excludedUsersAndGroups": NotRequired[UsersAndGroupsTypeDef],
         "ruleConfiguration": NotRequired[RuleConfigurationTypeDef],
     },
 )
+RetrieverConfigurationOutputTypeDef = TypedDict(
+    "RetrieverConfigurationOutputTypeDef",
+    {
+        "nativeIndexConfiguration": NotRequired[NativeIndexConfigurationOutputTypeDef],
+        "kendraIndexConfiguration": NotRequired[KendraIndexConfigurationTypeDef],
+    },
+)
 RetrieverConfigurationTypeDef = TypedDict(
     "RetrieverConfigurationTypeDef",
     {
-        "kendraIndexConfiguration": NotRequired[KendraIndexConfigurationTypeDef],
         "nativeIndexConfiguration": NotRequired[NativeIndexConfigurationTypeDef],
+        "kendraIndexConfiguration": NotRequired[KendraIndexConfigurationTypeDef],
+    },
+)
+DocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
+    "DocumentEnrichmentConfigurationOutputTypeDef",
+    {
+        "inlineConfigurations": NotRequired[
+            List[InlineDocumentEnrichmentConfigurationOutputTypeDef]
+        ],
+        "preExtractionHookConfiguration": NotRequired[HookConfigurationOutputTypeDef],
+        "postExtractionHookConfiguration": NotRequired[HookConfigurationOutputTypeDef],
     },
 )
 HookConfigurationTypeDef = TypedDict(
     "HookConfigurationTypeDef",
     {
         "invocationCondition": NotRequired[DocumentAttributeConditionTypeDef],
         "lambdaArn": NotRequired[str],
-        "roleArn": NotRequired[str],
         "s3BucketName": NotRequired[str],
+        "roleArn": NotRequired[str],
     },
 )
 InlineDocumentEnrichmentConfigurationTypeDef = TypedDict(
     "InlineDocumentEnrichmentConfigurationTypeDef",
     {
         "condition": NotRequired[DocumentAttributeConditionTypeDef],
-        "documentContentOperator": NotRequired[Literal["DELETE"]],
         "target": NotRequired[DocumentAttributeTargetTypeDef],
+        "documentContentOperator": NotRequired[Literal["DELETE"]],
     },
 )
 AttributeFilterTypeDef = TypedDict(
     "AttributeFilterTypeDef",
     {
         "andAllFilters": NotRequired[Sequence[Dict[str, Any]]],
+        "orAllFilters": NotRequired[Sequence[Dict[str, Any]]],
+        "notFilter": NotRequired[Dict[str, Any]],
+        "equalsTo": NotRequired[DocumentAttributeTypeDef],
         "containsAll": NotRequired[DocumentAttributeTypeDef],
         "containsAny": NotRequired[DocumentAttributeTypeDef],
-        "equalsTo": NotRequired[DocumentAttributeTypeDef],
         "greaterThan": NotRequired[DocumentAttributeTypeDef],
         "greaterThanOrEquals": NotRequired[DocumentAttributeTypeDef],
         "lessThan": NotRequired[DocumentAttributeTypeDef],
         "lessThanOrEquals": NotRequired[DocumentAttributeTypeDef],
-        "notFilter": NotRequired[Dict[str, Any]],
-        "orAllFilters": NotRequired[Sequence[Dict[str, Any]]],
     },
 )
 AccessConfigurationTypeDef = TypedDict(
     "AccessConfigurationTypeDef",
     {
         "accessControls": Sequence[AccessControlTypeDef],
         "memberRelation": NotRequired[MemberRelationType],
     },
 )
-ListMessagesResponsePaginatorTypeDef = TypedDict(
-    "ListMessagesResponsePaginatorTypeDef",
+ChatSyncOutputTypeDef = TypedDict(
+    "ChatSyncOutputTypeDef",
     {
-        "messages": List[MessagePaginatorTypeDef],
-        "nextToken": str,
+        "conversationId": str,
+        "systemMessage": str,
+        "systemMessageId": str,
+        "userMessageId": str,
+        "actionReview": ActionReviewTypeDef,
+        "authChallengeRequest": AuthChallengeRequestTypeDef,
+        "sourceAttributions": List[SourceAttributionTypeDef],
+        "failedAttachments": List[AttachmentOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListMessagesResponseTypeDef = TypedDict(
-    "ListMessagesResponseTypeDef",
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
-        "messages": List[MessageTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "messageId": NotRequired[str],
+        "body": NotRequired[str],
+        "time": NotRequired[datetime],
+        "type": NotRequired[MessageTypeType],
+        "attachments": NotRequired[List[AttachmentOutputTypeDef]],
+        "sourceAttribution": NotRequired[List[SourceAttributionTypeDef]],
+        "actionReview": NotRequired[ActionReviewTypeDef],
+        "actionExecution": NotRequired[ActionExecutionOutputTypeDef],
     },
 )
-TopicConfigurationTypeDef = TypedDict(
-    "TopicConfigurationTypeDef",
+TopicConfigurationExtraOutputTypeDef = TypedDict(
+    "TopicConfigurationExtraOutputTypeDef",
     {
         "name": str,
-        "rules": List[RuleTypeDef],
+        "rules": List[RuleExtraOutputTypeDef],
         "description": NotRequired[str],
         "exampleChatMessages": NotRequired[List[str]],
     },
 )
-CreateRetrieverRequestRequestTypeDef = TypedDict(
-    "CreateRetrieverRequestRequestTypeDef",
+TopicConfigurationOutputTypeDef = TypedDict(
+    "TopicConfigurationOutputTypeDef",
     {
-        "applicationId": str,
-        "configuration": RetrieverConfigurationTypeDef,
-        "displayName": str,
-        "type": RetrieverTypeType,
-        "clientToken": NotRequired[str],
-        "roleArn": NotRequired[str],
-        "tags": NotRequired[Sequence[TagTypeDef]],
+        "name": str,
+        "rules": List[RuleOutputTypeDef],
+        "description": NotRequired[str],
+        "exampleChatMessages": NotRequired[List[str]],
+    },
+)
+TopicConfigurationTypeDef = TypedDict(
+    "TopicConfigurationTypeDef",
+    {
+        "name": str,
+        "rules": Sequence[RuleTypeDef],
+        "description": NotRequired[str],
+        "exampleChatMessages": NotRequired[Sequence[str]],
     },
 )
 GetRetrieverResponseTypeDef = TypedDict(
     "GetRetrieverResponseTypeDef",
     {
         "applicationId": str,
-        "configuration": RetrieverConfigurationTypeDef,
-        "createdAt": datetime,
-        "displayName": str,
-        "retrieverArn": str,
         "retrieverId": str,
-        "roleArn": str,
-        "status": RetrieverStatusType,
+        "retrieverArn": str,
         "type": RetrieverTypeType,
+        "status": RetrieverStatusType,
+        "displayName": str,
+        "configuration": RetrieverConfigurationOutputTypeDef,
+        "roleArn": str,
+        "createdAt": datetime,
         "updatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateRetrieverRequestRequestTypeDef = TypedDict(
+    "CreateRetrieverRequestRequestTypeDef",
+    {
+        "applicationId": str,
+        "type": RetrieverTypeType,
+        "displayName": str,
+        "configuration": RetrieverConfigurationTypeDef,
+        "roleArn": NotRequired[str],
+        "clientToken": NotRequired[str],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+RetrieverConfigurationUnionTypeDef = Union[
+    RetrieverConfigurationTypeDef, RetrieverConfigurationOutputTypeDef
+]
 UpdateRetrieverRequestRequestTypeDef = TypedDict(
     "UpdateRetrieverRequestRequestTypeDef",
     {
         "applicationId": str,
         "retrieverId": str,
         "configuration": NotRequired[RetrieverConfigurationTypeDef],
         "displayName": NotRequired[str],
         "roleArn": NotRequired[str],
     },
 )
+GetDataSourceResponseTypeDef = TypedDict(
+    "GetDataSourceResponseTypeDef",
+    {
+        "applicationId": str,
+        "indexId": str,
+        "dataSourceId": str,
+        "dataSourceArn": str,
+        "displayName": str,
+        "type": str,
+        "configuration": Dict[str, Any],
+        "vpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "description": str,
+        "status": DataSourceStatusType,
+        "syncSchedule": str,
+        "roleArn": str,
+        "error": ErrorDetailTypeDef,
+        "documentEnrichmentConfiguration": DocumentEnrichmentConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DocumentEnrichmentConfigurationTypeDef = TypedDict(
     "DocumentEnrichmentConfigurationTypeDef",
     {
         "inlineConfigurations": NotRequired[Sequence[InlineDocumentEnrichmentConfigurationTypeDef]],
-        "postExtractionHookConfiguration": NotRequired[HookConfigurationTypeDef],
         "preExtractionHookConfiguration": NotRequired[HookConfigurationTypeDef],
+        "postExtractionHookConfiguration": NotRequired[HookConfigurationTypeDef],
+    },
+)
+ListMessagesResponseTypeDef = TypedDict(
+    "ListMessagesResponseTypeDef",
+    {
+        "messages": List[MessageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetChatControlsConfigurationResponseTypeDef = TypedDict(
     "GetChatControlsConfigurationResponseTypeDef",
     {
+        "responseScope": ResponseScopeType,
         "blockedPhrases": BlockedPhrasesConfigurationTypeDef,
+        "topicConfigurations": List[TopicConfigurationExtraOutputTypeDef],
         "creatorModeConfiguration": AppliedCreatorModeConfigurationTypeDef,
         "nextToken": str,
-        "responseScope": ResponseScopeType,
-        "topicConfigurations": List[TopicConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateChatControlsConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateChatControlsConfigurationRequestRequestTypeDef",
-    {
-        "applicationId": str,
-        "blockedPhrasesConfigurationUpdate": NotRequired[BlockedPhrasesConfigurationUpdateTypeDef],
-        "clientToken": NotRequired[str],
-        "creatorModeConfiguration": NotRequired[CreatorModeConfigurationTypeDef],
-        "responseScope": NotRequired[ResponseScopeType],
-        "topicConfigurationsToCreateOrUpdate": NotRequired[Sequence[TopicConfigurationTypeDef]],
-        "topicConfigurationsToDelete": NotRequired[Sequence[TopicConfigurationTypeDef]],
-    },
-)
+TopicConfigurationUnionTypeDef = Union[
+    TopicConfigurationTypeDef, TopicConfigurationExtraOutputTypeDef
+]
 CreateDataSourceRequestRequestTypeDef = TypedDict(
     "CreateDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "configuration": Mapping[str, Any],
-        "displayName": str,
         "indexId": str,
-        "clientToken": NotRequired[str],
+        "displayName": str,
+        "configuration": Mapping[str, Any],
+        "vpcConfiguration": NotRequired[DataSourceVpcConfigurationTypeDef],
         "description": NotRequired[str],
-        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
-        "roleArn": NotRequired[str],
-        "syncSchedule": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
-        "vpcConfiguration": NotRequired[DataSourceVpcConfigurationTypeDef],
+        "syncSchedule": NotRequired[str],
+        "roleArn": NotRequired[str],
+        "clientToken": NotRequired[str],
+        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
     },
 )
+DocumentEnrichmentConfigurationUnionTypeDef = Union[
+    DocumentEnrichmentConfigurationTypeDef, DocumentEnrichmentConfigurationOutputTypeDef
+]
 DocumentTypeDef = TypedDict(
     "DocumentTypeDef",
     {
         "id": str,
-        "accessConfiguration": NotRequired[AccessConfigurationTypeDef],
         "attributes": NotRequired[Sequence[DocumentAttributeTypeDef]],
         "content": NotRequired[DocumentContentTypeDef],
         "contentType": NotRequired[ContentTypeType],
-        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
         "title": NotRequired[str],
-    },
-)
-GetDataSourceResponseTypeDef = TypedDict(
-    "GetDataSourceResponseTypeDef",
-    {
-        "applicationId": str,
-        "configuration": Dict[str, Any],
-        "createdAt": datetime,
-        "dataSourceArn": str,
-        "dataSourceId": str,
-        "description": str,
-        "displayName": str,
-        "documentEnrichmentConfiguration": DocumentEnrichmentConfigurationTypeDef,
-        "error": ErrorDetailTypeDef,
-        "indexId": str,
-        "roleArn": str,
-        "status": DataSourceStatusType,
-        "syncSchedule": str,
-        "type": str,
-        "updatedAt": datetime,
-        "vpcConfiguration": DataSourceVpcConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accessConfiguration": NotRequired[AccessConfigurationTypeDef],
+        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
     },
 )
 UpdateDataSourceRequestRequestTypeDef = TypedDict(
     "UpdateDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "dataSourceId": str,
         "indexId": str,
+        "dataSourceId": str,
+        "displayName": NotRequired[str],
         "configuration": NotRequired[Mapping[str, Any]],
+        "vpcConfiguration": NotRequired[DataSourceVpcConfigurationTypeDef],
         "description": NotRequired[str],
-        "displayName": NotRequired[str],
-        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
-        "roleArn": NotRequired[str],
         "syncSchedule": NotRequired[str],
-        "vpcConfiguration": NotRequired[DataSourceVpcConfigurationTypeDef],
+        "roleArn": NotRequired[str],
+        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
+    },
+)
+UpdateChatControlsConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateChatControlsConfigurationRequestRequestTypeDef",
+    {
+        "applicationId": str,
+        "clientToken": NotRequired[str],
+        "responseScope": NotRequired[ResponseScopeType],
+        "blockedPhrasesConfigurationUpdate": NotRequired[BlockedPhrasesConfigurationUpdateTypeDef],
+        "topicConfigurationsToCreateOrUpdate": NotRequired[
+            Sequence[TopicConfigurationUnionTypeDef]
+        ],
+        "topicConfigurationsToDelete": NotRequired[Sequence[TopicConfigurationUnionTypeDef]],
+        "creatorModeConfiguration": NotRequired[CreatorModeConfigurationTypeDef],
     },
 )
 BatchPutDocumentRequestRequestTypeDef = TypedDict(
     "BatchPutDocumentRequestRequestTypeDef",
     {
         "applicationId": str,
-        "documents": Sequence[DocumentTypeDef],
         "indexId": str,
-        "dataSourceSyncId": NotRequired[str],
+        "documents": Sequence[DocumentTypeDef],
         "roleArn": NotRequired[str],
+        "dataSourceSyncId": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness/type_defs.pyi` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for qbusiness service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_qbusiness.type_defs import ActionExecutionPayloadFieldPaginatorTypeDef
+    from mypy_boto3_qbusiness.type_defs import S3TypeDef
 
-    data: ActionExecutionPayloadFieldPaginatorTypeDef = ...
+    data: S3TypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
@@ -31,20 +31,22 @@
     DataSourceSyncJobStatusType,
     DocumentAttributeBoostingLevelType,
     DocumentEnrichmentConditionOperatorType,
     DocumentStatusType,
     ErrorCodeType,
     GroupStatusType,
     IndexStatusType,
+    IndexTypeType,
     MemberRelationType,
     MembershipTypeType,
     MessageTypeType,
     MessageUsefulnessReasonType,
     MessageUsefulnessType,
     NumberAttributeBoostingTypeType,
+    PluginBuildStatusType,
     PluginStateType,
     PluginTypeType,
     ReadAccessTypeType,
     ResponseScopeType,
     RetrieverStatusType,
     RetrieverTypeType,
     RuleTypeType,
@@ -64,23 +66,27 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActionExecutionPayloadFieldPaginatorTypeDef",
+    "S3TypeDef",
+    "ActionExecutionPayloadFieldExtraOutputTypeDef",
+    "ActionExecutionPayloadFieldOutputTypeDef",
     "ActionExecutionPayloadFieldTypeDef",
     "ActionReviewPayloadFieldAllowedValueTypeDef",
     "ApplicationTypeDef",
     "AppliedAttachmentsConfigurationTypeDef",
     "AppliedCreatorModeConfigurationTypeDef",
     "BlobTypeDef",
     "ErrorDetailTypeDef",
     "AttachmentsConfigurationTypeDef",
+    "AuthChallengeRequestTypeDef",
+    "AuthChallengeResponseTypeDef",
     "BasicAuthConfigurationTypeDef",
     "DeleteDocumentTypeDef",
     "ResponseMetadataTypeDef",
     "BlockedPhrasesConfigurationTypeDef",
     "BlockedPhrasesConfigurationUpdateTypeDef",
     "PluginConfigurationTypeDef",
     "ContentBlockerRuleTypeDef",
@@ -90,31 +96,33 @@
     "TagTypeDef",
     "DataSourceVpcConfigurationTypeDef",
     "IndexCapacityConfigurationTypeDef",
     "UserAliasTypeDef",
     "CreatorModeConfigurationTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
     "DataSourceTypeDef",
+    "DataSourceVpcConfigurationOutputTypeDef",
     "DateAttributeBoostingConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteChatControlsConfigurationRequestRequestTypeDef",
     "DeleteConversationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteIndexRequestRequestTypeDef",
     "DeletePluginRequestRequestTypeDef",
     "DeleteRetrieverRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteWebExperienceRequestRequestTypeDef",
     "NumberAttributeBoostingConfigurationTypeDef",
-    "StringAttributeBoostingConfigurationTypeDef",
+    "StringAttributeBoostingConfigurationOutputTypeDef",
     "StringListAttributeBoostingConfigurationTypeDef",
+    "StringAttributeBoostingConfigurationTypeDef",
+    "DocumentAttributeValueOutputTypeDef",
     "DocumentAttributeConfigurationTypeDef",
     "TimestampTypeDef",
-    "S3TypeDef",
     "GetApplicationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetChatControlsConfigurationRequestRequestTypeDef",
     "GetDataSourceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIndexRequestRequestTypeDef",
     "GetPluginRequestRequestTypeDef",
@@ -139,24 +147,29 @@
     "RetrieverTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebExperiencesRequestRequestTypeDef",
     "WebExperienceTypeDef",
     "OAuth2ClientCredentialConfigurationTypeDef",
     "PrincipalGroupTypeDef",
     "PrincipalUserTypeDef",
+    "UsersAndGroupsExtraOutputTypeDef",
+    "UsersAndGroupsOutputTypeDef",
     "UsersAndGroupsTypeDef",
     "SamlConfigurationTypeDef",
-    "TextSegmentTypeDef",
+    "SnippetExcerptTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ActionExecutionPaginatorTypeDef",
+    "APISchemaTypeDef",
+    "ActionExecutionExtraOutputTypeDef",
+    "ActionExecutionOutputTypeDef",
     "ActionExecutionTypeDef",
     "ActionReviewPayloadFieldTypeDef",
     "AttachmentInputTypeDef",
+    "DocumentContentTypeDef",
     "AttachmentOutputTypeDef",
     "DocumentDetailsTypeDef",
     "FailedDocumentTypeDef",
     "GroupStatusDetailTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
@@ -165,35 +178,40 @@
     "CreatePluginResponseTypeDef",
     "CreateRetrieverResponseTypeDef",
     "CreateWebExperienceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListApplicationsResponseTypeDef",
     "StartDataSourceSyncJobResponseTypeDef",
     "ChatModeConfigurationTypeDef",
+    "ContentRetrievalRuleExtraOutputTypeDef",
+    "ContentRetrievalRuleOutputTypeDef",
     "ContentRetrievalRuleTypeDef",
     "ListConversationsResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateWebExperienceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "GetUserResponseTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserResponseTypeDef",
     "DataSourceSyncJobTypeDef",
     "ListDataSourcesResponseTypeDef",
+    "DataSourceVpcConfigurationUnionTypeDef",
+    "DocumentAttributeBoostingConfigurationOutputTypeDef",
     "DocumentAttributeBoostingConfigurationTypeDef",
+    "DocumentAttributeConditionOutputTypeDef",
+    "DocumentAttributeTargetOutputTypeDef",
     "UpdateIndexRequestRequestTypeDef",
     "DocumentAttributeValueTypeDef",
     "ListDataSourceSyncJobsRequestRequestTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "MessageUsefulnessFeedbackTypeDef",
-    "DocumentContentTypeDef",
     "GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListConversationsRequestListConversationsPaginateTypeDef",
     "ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef",
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
@@ -205,91 +223,121 @@
     "GroupMembersTypeDef",
     "ListGroupsResponseTypeDef",
     "IndexStatisticsTypeDef",
     "ListIndicesResponseTypeDef",
     "ListPluginsResponseTypeDef",
     "ListRetrieversResponseTypeDef",
     "ListWebExperiencesResponseTypeDef",
+    "PluginAuthConfigurationOutputTypeDef",
     "PluginAuthConfigurationTypeDef",
     "PrincipalTypeDef",
     "WebExperienceAuthConfigurationTypeDef",
-    "SourceAttributionTypeDef",
+    "TextSegmentTypeDef",
+    "CustomPluginConfigurationTypeDef",
+    "ActionExecutionUnionTypeDef",
     "ActionReviewTypeDef",
     "ListDocumentsResponseTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
     "GetGroupResponseTypeDef",
     "ChatSyncInputRequestTypeDef",
+    "RuleConfigurationExtraOutputTypeDef",
+    "RuleConfigurationOutputTypeDef",
     "RuleConfigurationTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
+    "NativeIndexConfigurationOutputTypeDef",
     "NativeIndexConfigurationTypeDef",
+    "HookConfigurationOutputTypeDef",
+    "InlineDocumentEnrichmentConfigurationOutputTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "PutGroupRequestRequestTypeDef",
     "GetIndexResponseTypeDef",
-    "CreatePluginRequestRequestTypeDef",
-    "GetPluginResponseTypeDef",
-    "UpdatePluginRequestRequestTypeDef",
+    "PluginAuthConfigurationUnionTypeDef",
     "AccessControlTypeDef",
     "GetWebExperienceResponseTypeDef",
     "UpdateWebExperienceRequestRequestTypeDef",
-    "ChatSyncOutputTypeDef",
-    "MessagePaginatorTypeDef",
-    "MessageTypeDef",
+    "SourceAttributionTypeDef",
+    "CreatePluginRequestRequestTypeDef",
+    "GetPluginResponseTypeDef",
+    "UpdatePluginRequestRequestTypeDef",
+    "RuleExtraOutputTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
+    "RetrieverConfigurationOutputTypeDef",
     "RetrieverConfigurationTypeDef",
+    "DocumentEnrichmentConfigurationOutputTypeDef",
     "HookConfigurationTypeDef",
     "InlineDocumentEnrichmentConfigurationTypeDef",
     "AttributeFilterTypeDef",
     "AccessConfigurationTypeDef",
-    "ListMessagesResponsePaginatorTypeDef",
-    "ListMessagesResponseTypeDef",
+    "ChatSyncOutputTypeDef",
+    "MessageTypeDef",
+    "TopicConfigurationExtraOutputTypeDef",
+    "TopicConfigurationOutputTypeDef",
     "TopicConfigurationTypeDef",
-    "CreateRetrieverRequestRequestTypeDef",
     "GetRetrieverResponseTypeDef",
+    "CreateRetrieverRequestRequestTypeDef",
+    "RetrieverConfigurationUnionTypeDef",
     "UpdateRetrieverRequestRequestTypeDef",
+    "GetDataSourceResponseTypeDef",
     "DocumentEnrichmentConfigurationTypeDef",
+    "ListMessagesResponseTypeDef",
     "GetChatControlsConfigurationResponseTypeDef",
-    "UpdateChatControlsConfigurationRequestRequestTypeDef",
+    "TopicConfigurationUnionTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
+    "DocumentEnrichmentConfigurationUnionTypeDef",
     "DocumentTypeDef",
-    "GetDataSourceResponseTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
+    "UpdateChatControlsConfigurationRequestRequestTypeDef",
     "BatchPutDocumentRequestRequestTypeDef",
 )
 
-ActionExecutionPayloadFieldPaginatorTypeDef = TypedDict(
-    "ActionExecutionPayloadFieldPaginatorTypeDef",
+S3TypeDef = TypedDict(
+    "S3TypeDef",
+    {
+        "bucket": str,
+        "key": str,
+    },
+)
+ActionExecutionPayloadFieldExtraOutputTypeDef = TypedDict(
+    "ActionExecutionPayloadFieldExtraOutputTypeDef",
+    {
+        "value": Dict[str, Any],
+    },
+)
+ActionExecutionPayloadFieldOutputTypeDef = TypedDict(
+    "ActionExecutionPayloadFieldOutputTypeDef",
     {
         "value": Dict[str, Any],
     },
 )
 ActionExecutionPayloadFieldTypeDef = TypedDict(
     "ActionExecutionPayloadFieldTypeDef",
     {
         "value": Mapping[str, Any],
     },
 )
 ActionReviewPayloadFieldAllowedValueTypeDef = TypedDict(
     "ActionReviewPayloadFieldAllowedValueTypeDef",
     {
-        "displayValue": NotRequired[Dict[str, Any]],
         "value": NotRequired[Dict[str, Any]],
+        "displayValue": NotRequired[Dict[str, Any]],
     },
 )
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
+        "displayName": NotRequired[str],
         "applicationId": NotRequired[str],
         "createdAt": NotRequired[datetime],
-        "displayName": NotRequired[str],
-        "status": NotRequired[ApplicationStatusType],
         "updatedAt": NotRequired[datetime],
+        "status": NotRequired[ApplicationStatusType],
     },
 )
 AppliedAttachmentsConfigurationTypeDef = TypedDict(
     "AppliedAttachmentsConfigurationTypeDef",
     {
         "attachmentsControlMode": NotRequired[AttachmentsControlModeType],
     },
@@ -300,29 +348,41 @@
         "creatorModeControl": CreatorModeControlType,
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
-        "errorCode": NotRequired[ErrorCodeType],
         "errorMessage": NotRequired[str],
+        "errorCode": NotRequired[ErrorCodeType],
     },
 )
 AttachmentsConfigurationTypeDef = TypedDict(
     "AttachmentsConfigurationTypeDef",
     {
         "attachmentsControlMode": AttachmentsControlModeType,
     },
 )
+AuthChallengeRequestTypeDef = TypedDict(
+    "AuthChallengeRequestTypeDef",
+    {
+        "authorizationUrl": str,
+    },
+)
+AuthChallengeResponseTypeDef = TypedDict(
+    "AuthChallengeResponseTypeDef",
+    {
+        "responseMap": Mapping[str, str],
+    },
+)
 BasicAuthConfigurationTypeDef = TypedDict(
     "BasicAuthConfigurationTypeDef",
     {
-        "roleArn": str,
         "secretArn": str,
+        "roleArn": str,
     },
 )
 DeleteDocumentTypeDef = TypedDict(
     "DeleteDocumentTypeDef",
     {
         "documentId": str,
     },
@@ -363,24 +423,24 @@
     {
         "systemMessageOverride": NotRequired[str],
     },
 )
 EligibleDataSourceTypeDef = TypedDict(
     "EligibleDataSourceTypeDef",
     {
-        "dataSourceId": NotRequired[str],
         "indexId": NotRequired[str],
+        "dataSourceId": NotRequired[str],
     },
 )
 ConversationTypeDef = TypedDict(
     "ConversationTypeDef",
     {
         "conversationId": NotRequired[str],
-        "startTime": NotRequired[datetime],
         "title": NotRequired[str],
+        "startTime": NotRequired[datetime],
     },
 )
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "kmsKeyId": NotRequired[str],
     },
@@ -391,57 +451,64 @@
         "key": str,
         "value": str,
     },
 )
 DataSourceVpcConfigurationTypeDef = TypedDict(
     "DataSourceVpcConfigurationTypeDef",
     {
-        "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
+        "securityGroupIds": Sequence[str],
     },
 )
 IndexCapacityConfigurationTypeDef = TypedDict(
     "IndexCapacityConfigurationTypeDef",
     {
         "units": NotRequired[int],
     },
 )
 UserAliasTypeDef = TypedDict(
     "UserAliasTypeDef",
     {
         "userId": str,
-        "dataSourceId": NotRequired[str],
         "indexId": NotRequired[str],
+        "dataSourceId": NotRequired[str],
     },
 )
 CreatorModeConfigurationTypeDef = TypedDict(
     "CreatorModeConfigurationTypeDef",
     {
         "creatorModeControl": CreatorModeControlType,
     },
 )
 DataSourceSyncJobMetricsTypeDef = TypedDict(
     "DataSourceSyncJobMetricsTypeDef",
     {
         "documentsAdded": NotRequired[str],
+        "documentsModified": NotRequired[str],
         "documentsDeleted": NotRequired[str],
         "documentsFailed": NotRequired[str],
-        "documentsModified": NotRequired[str],
         "documentsScanned": NotRequired[str],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
-        "createdAt": NotRequired[datetime],
-        "dataSourceId": NotRequired[str],
         "displayName": NotRequired[str],
-        "status": NotRequired[DataSourceStatusType],
+        "dataSourceId": NotRequired[str],
         "type": NotRequired[str],
+        "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
+        "status": NotRequired[DataSourceStatusType],
+    },
+)
+DataSourceVpcConfigurationOutputTypeDef = TypedDict(
+    "DataSourceVpcConfigurationOutputTypeDef",
+    {
+        "subnetIds": List[str],
+        "securityGroupIds": List[str],
     },
 )
 DateAttributeBoostingConfigurationTypeDef = TypedDict(
     "DateAttributeBoostingConfigurationTypeDef",
     {
         "boostingLevel": DocumentAttributeBoostingLevelType,
         "boostingDurationInSeconds": NotRequired[int],
@@ -458,33 +525,33 @@
     {
         "applicationId": str,
     },
 )
 DeleteConversationRequestRequestTypeDef = TypedDict(
     "DeleteConversationRequestRequestTypeDef",
     {
-        "applicationId": str,
         "conversationId": str,
+        "applicationId": str,
         "userId": NotRequired[str],
     },
 )
 DeleteDataSourceRequestRequestTypeDef = TypedDict(
     "DeleteDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "dataSourceId": str,
         "indexId": str,
+        "dataSourceId": str,
     },
 )
 DeleteGroupRequestRequestTypeDef = TypedDict(
     "DeleteGroupRequestRequestTypeDef",
     {
         "applicationId": str,
-        "groupName": str,
         "indexId": str,
+        "groupName": str,
         "dataSourceId": NotRequired[str],
     },
 )
 DeleteIndexRequestRequestTypeDef = TypedDict(
     "DeleteIndexRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -522,43 +589,52 @@
 NumberAttributeBoostingConfigurationTypeDef = TypedDict(
     "NumberAttributeBoostingConfigurationTypeDef",
     {
         "boostingLevel": DocumentAttributeBoostingLevelType,
         "boostingType": NotRequired[NumberAttributeBoostingTypeType],
     },
 )
-StringAttributeBoostingConfigurationTypeDef = TypedDict(
-    "StringAttributeBoostingConfigurationTypeDef",
+StringAttributeBoostingConfigurationOutputTypeDef = TypedDict(
+    "StringAttributeBoostingConfigurationOutputTypeDef",
     {
         "boostingLevel": DocumentAttributeBoostingLevelType,
-        "attributeValueBoosting": NotRequired[Mapping[str, StringAttributeValueBoostingLevelType]],
+        "attributeValueBoosting": NotRequired[Dict[str, StringAttributeValueBoostingLevelType]],
     },
 )
 StringListAttributeBoostingConfigurationTypeDef = TypedDict(
     "StringListAttributeBoostingConfigurationTypeDef",
     {
         "boostingLevel": DocumentAttributeBoostingLevelType,
     },
 )
+StringAttributeBoostingConfigurationTypeDef = TypedDict(
+    "StringAttributeBoostingConfigurationTypeDef",
+    {
+        "boostingLevel": DocumentAttributeBoostingLevelType,
+        "attributeValueBoosting": NotRequired[Mapping[str, StringAttributeValueBoostingLevelType]],
+    },
+)
+DocumentAttributeValueOutputTypeDef = TypedDict(
+    "DocumentAttributeValueOutputTypeDef",
+    {
+        "stringValue": NotRequired[str],
+        "stringListValue": NotRequired[List[str]],
+        "longValue": NotRequired[int],
+        "dateValue": NotRequired[datetime],
+    },
+)
 DocumentAttributeConfigurationTypeDef = TypedDict(
     "DocumentAttributeConfigurationTypeDef",
     {
         "name": NotRequired[str],
-        "search": NotRequired[StatusType],
         "type": NotRequired[AttributeTypeType],
+        "search": NotRequired[StatusType],
     },
 )
 TimestampTypeDef = Union[datetime, str]
-S3TypeDef = TypedDict(
-    "S3TypeDef",
-    {
-        "bucket": str,
-        "key": str,
-    },
-)
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 PaginatorConfigTypeDef = TypedDict(
@@ -577,24 +653,24 @@
         "nextToken": NotRequired[str],
     },
 )
 GetDataSourceRequestRequestTypeDef = TypedDict(
     "GetDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "dataSourceId": str,
         "indexId": str,
+        "dataSourceId": str,
     },
 )
 GetGroupRequestRequestTypeDef = TypedDict(
     "GetGroupRequestRequestTypeDef",
     {
         "applicationId": str,
-        "groupName": str,
         "indexId": str,
+        "groupName": str,
         "dataSourceId": NotRequired[str],
     },
 )
 GetIndexRequestRequestTypeDef = TypedDict(
     "GetIndexRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -655,357 +731,397 @@
         "indexedTextBytes": NotRequired[int],
         "indexedTextDocumentCount": NotRequired[int],
     },
 )
 IndexTypeDef = TypedDict(
     "IndexTypeDef",
     {
-        "createdAt": NotRequired[datetime],
         "displayName": NotRequired[str],
         "indexId": NotRequired[str],
-        "status": NotRequired[IndexStatusType],
+        "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
+        "status": NotRequired[IndexStatusType],
     },
 )
 KendraIndexConfigurationTypeDef = TypedDict(
     "KendraIndexConfigurationTypeDef",
     {
         "indexId": str,
     },
 )
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListConversationsRequestRequestTypeDef = TypedDict(
     "ListConversationsRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
         "userId": NotRequired[str],
+        "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListDataSourcesRequestRequestTypeDef = TypedDict(
     "ListDataSourcesRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListDocumentsRequestRequestTypeDef = TypedDict(
     "ListDocumentsRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
         "dataSourceIds": NotRequired[Sequence[str]],
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListMessagesRequestRequestTypeDef = TypedDict(
     "ListMessagesRequestRequestTypeDef",
     {
-        "applicationId": str,
         "conversationId": str,
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
+        "applicationId": str,
         "userId": NotRequired[str],
+        "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 ListPluginsRequestRequestTypeDef = TypedDict(
     "ListPluginsRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 PluginTypeDef = TypedDict(
     "PluginTypeDef",
     {
-        "createdAt": NotRequired[datetime],
-        "displayName": NotRequired[str],
         "pluginId": NotRequired[str],
+        "displayName": NotRequired[str],
+        "type": NotRequired[PluginTypeType],
         "serverUrl": NotRequired[str],
         "state": NotRequired[PluginStateType],
-        "type": NotRequired[PluginTypeType],
+        "buildStatus": NotRequired[PluginBuildStatusType],
+        "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
     },
 )
 ListRetrieversRequestRequestTypeDef = TypedDict(
     "ListRetrieversRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 RetrieverTypeDef = TypedDict(
     "RetrieverTypeDef",
     {
         "applicationId": NotRequired[str],
-        "displayName": NotRequired[str],
         "retrieverId": NotRequired[str],
-        "status": NotRequired[RetrieverStatusType],
         "type": NotRequired[RetrieverTypeType],
+        "status": NotRequired[RetrieverStatusType],
+        "displayName": NotRequired[str],
     },
 )
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
     },
 )
 ListWebExperiencesRequestRequestTypeDef = TypedDict(
     "ListWebExperiencesRequestRequestTypeDef",
     {
         "applicationId": str,
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 WebExperienceTypeDef = TypedDict(
     "WebExperienceTypeDef",
     {
+        "webExperienceId": NotRequired[str],
         "createdAt": NotRequired[datetime],
+        "updatedAt": NotRequired[datetime],
         "defaultEndpoint": NotRequired[str],
         "status": NotRequired[WebExperienceStatusType],
-        "updatedAt": NotRequired[datetime],
-        "webExperienceId": NotRequired[str],
     },
 )
 OAuth2ClientCredentialConfigurationTypeDef = TypedDict(
     "OAuth2ClientCredentialConfigurationTypeDef",
     {
-        "roleArn": str,
         "secretArn": str,
+        "roleArn": str,
     },
 )
 PrincipalGroupTypeDef = TypedDict(
     "PrincipalGroupTypeDef",
     {
         "access": ReadAccessTypeType,
-        "membershipType": NotRequired[MembershipTypeType],
         "name": NotRequired[str],
+        "membershipType": NotRequired[MembershipTypeType],
     },
 )
 PrincipalUserTypeDef = TypedDict(
     "PrincipalUserTypeDef",
     {
         "access": ReadAccessTypeType,
         "id": NotRequired[str],
         "membershipType": NotRequired[MembershipTypeType],
     },
 )
-UsersAndGroupsTypeDef = TypedDict(
-    "UsersAndGroupsTypeDef",
+UsersAndGroupsExtraOutputTypeDef = TypedDict(
+    "UsersAndGroupsExtraOutputTypeDef",
     {
+        "userIds": NotRequired[List[str]],
         "userGroups": NotRequired[List[str]],
+    },
+)
+UsersAndGroupsOutputTypeDef = TypedDict(
+    "UsersAndGroupsOutputTypeDef",
+    {
         "userIds": NotRequired[List[str]],
+        "userGroups": NotRequired[List[str]],
+    },
+)
+UsersAndGroupsTypeDef = TypedDict(
+    "UsersAndGroupsTypeDef",
+    {
+        "userIds": NotRequired[Sequence[str]],
+        "userGroups": NotRequired[Sequence[str]],
     },
 )
 SamlConfigurationTypeDef = TypedDict(
     "SamlConfigurationTypeDef",
     {
         "metadataXML": str,
         "roleArn": str,
         "userIdAttribute": str,
         "userGroupAttribute": NotRequired[str],
     },
 )
-TextSegmentTypeDef = TypedDict(
-    "TextSegmentTypeDef",
+SnippetExcerptTypeDef = TypedDict(
+    "SnippetExcerptTypeDef",
     {
-        "beginOffset": NotRequired[int],
-        "endOffset": NotRequired[int],
+        "text": NotRequired[str],
     },
 )
 StartDataSourceSyncJobRequestRequestTypeDef = TypedDict(
     "StartDataSourceSyncJobRequestRequestTypeDef",
     {
-        "applicationId": str,
         "dataSourceId": str,
+        "applicationId": str,
         "indexId": str,
     },
 )
 StopDataSourceSyncJobRequestRequestTypeDef = TypedDict(
     "StopDataSourceSyncJobRequestRequestTypeDef",
     {
-        "applicationId": str,
         "dataSourceId": str,
+        "applicationId": str,
         "indexId": str,
     },
 )
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tagKeys": Sequence[str],
     },
 )
-ActionExecutionPaginatorTypeDef = TypedDict(
-    "ActionExecutionPaginatorTypeDef",
+APISchemaTypeDef = TypedDict(
+    "APISchemaTypeDef",
     {
-        "payload": Dict[str, ActionExecutionPayloadFieldPaginatorTypeDef],
+        "payload": NotRequired[str],
+        "s3": NotRequired[S3TypeDef],
+    },
+)
+ActionExecutionExtraOutputTypeDef = TypedDict(
+    "ActionExecutionExtraOutputTypeDef",
+    {
+        "pluginId": str,
+        "payload": Dict[str, ActionExecutionPayloadFieldExtraOutputTypeDef],
         "payloadFieldNameSeparator": str,
+    },
+)
+ActionExecutionOutputTypeDef = TypedDict(
+    "ActionExecutionOutputTypeDef",
+    {
         "pluginId": str,
+        "payload": Dict[str, ActionExecutionPayloadFieldOutputTypeDef],
+        "payloadFieldNameSeparator": str,
     },
 )
 ActionExecutionTypeDef = TypedDict(
     "ActionExecutionTypeDef",
     {
+        "pluginId": str,
         "payload": Mapping[str, ActionExecutionPayloadFieldTypeDef],
         "payloadFieldNameSeparator": str,
-        "pluginId": str,
     },
 )
 ActionReviewPayloadFieldTypeDef = TypedDict(
     "ActionReviewPayloadFieldTypeDef",
     {
-        "allowedValues": NotRequired[List[ActionReviewPayloadFieldAllowedValueTypeDef]],
         "displayName": NotRequired[str],
         "displayOrder": NotRequired[int],
-        "required": NotRequired[bool],
+        "displayDescription": NotRequired[str],
         "type": NotRequired[ActionPayloadFieldTypeType],
         "value": NotRequired[Dict[str, Any]],
+        "allowedValues": NotRequired[List[ActionReviewPayloadFieldAllowedValueTypeDef]],
+        "allowedFormat": NotRequired[str],
+        "required": NotRequired[bool],
     },
 )
 AttachmentInputTypeDef = TypedDict(
     "AttachmentInputTypeDef",
     {
-        "data": BlobTypeDef,
         "name": str,
+        "data": BlobTypeDef,
+    },
+)
+DocumentContentTypeDef = TypedDict(
+    "DocumentContentTypeDef",
+    {
+        "blob": NotRequired[BlobTypeDef],
+        "s3": NotRequired[S3TypeDef],
     },
 )
 AttachmentOutputTypeDef = TypedDict(
     "AttachmentOutputTypeDef",
     {
-        "error": NotRequired[ErrorDetailTypeDef],
         "name": NotRequired[str],
         "status": NotRequired[AttachmentStatusType],
+        "error": NotRequired[ErrorDetailTypeDef],
     },
 )
 DocumentDetailsTypeDef = TypedDict(
     "DocumentDetailsTypeDef",
     {
-        "createdAt": NotRequired[datetime],
         "documentId": NotRequired[str],
-        "error": NotRequired[ErrorDetailTypeDef],
         "status": NotRequired[DocumentStatusType],
+        "error": NotRequired[ErrorDetailTypeDef],
+        "createdAt": NotRequired[datetime],
         "updatedAt": NotRequired[datetime],
     },
 )
 FailedDocumentTypeDef = TypedDict(
     "FailedDocumentTypeDef",
     {
-        "dataSourceId": NotRequired[str],
-        "error": NotRequired[ErrorDetailTypeDef],
         "id": NotRequired[str],
+        "error": NotRequired[ErrorDetailTypeDef],
+        "dataSourceId": NotRequired[str],
     },
 )
 GroupStatusDetailTypeDef = TypedDict(
     "GroupStatusDetailTypeDef",
     {
-        "errorDetail": NotRequired[ErrorDetailTypeDef],
-        "lastUpdatedAt": NotRequired[datetime],
         "status": NotRequired[GroupStatusType],
+        "lastUpdatedAt": NotRequired[datetime],
+        "errorDetail": NotRequired[ErrorDetailTypeDef],
     },
 )
 UpdateApplicationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
-        "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
-        "description": NotRequired[str],
+        "identityCenterInstanceArn": NotRequired[str],
         "displayName": NotRequired[str],
+        "description": NotRequired[str],
         "roleArn": NotRequired[str],
+        "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
     },
 )
 BatchDeleteDocumentRequestRequestTypeDef = TypedDict(
     "BatchDeleteDocumentRequestRequestTypeDef",
     {
         "applicationId": str,
-        "documents": Sequence[DeleteDocumentTypeDef],
         "indexId": str,
+        "documents": Sequence[DeleteDocumentTypeDef],
         "dataSourceSyncId": NotRequired[str],
     },
 )
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
-        "applicationArn": str,
         "applicationId": str,
+        "applicationArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateDataSourceResponseTypeDef = TypedDict(
     "CreateDataSourceResponseTypeDef",
     {
-        "dataSourceArn": str,
         "dataSourceId": str,
+        "dataSourceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateIndexResponseTypeDef = TypedDict(
     "CreateIndexResponseTypeDef",
     {
-        "indexArn": str,
         "indexId": str,
+        "indexArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreatePluginResponseTypeDef = TypedDict(
     "CreatePluginResponseTypeDef",
     {
-        "pluginArn": str,
         "pluginId": str,
+        "pluginArn": str,
+        "buildStatus": PluginBuildStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateRetrieverResponseTypeDef = TypedDict(
     "CreateRetrieverResponseTypeDef",
     {
-        "retrieverArn": str,
         "retrieverId": str,
+        "retrieverArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateWebExperienceResponseTypeDef = TypedDict(
     "CreateWebExperienceResponseTypeDef",
     {
-        "webExperienceArn": str,
         "webExperienceId": str,
+        "webExperienceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
-        "applications": List[ApplicationTypeDef],
         "nextToken": str,
+        "applications": List[ApplicationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartDataSourceSyncJobResponseTypeDef = TypedDict(
     "StartDataSourceSyncJobResponseTypeDef",
     {
         "executionId": str,
@@ -1014,70 +1130,82 @@
 )
 ChatModeConfigurationTypeDef = TypedDict(
     "ChatModeConfigurationTypeDef",
     {
         "pluginConfiguration": NotRequired[PluginConfigurationTypeDef],
     },
 )
+ContentRetrievalRuleExtraOutputTypeDef = TypedDict(
+    "ContentRetrievalRuleExtraOutputTypeDef",
+    {
+        "eligibleDataSources": NotRequired[List[EligibleDataSourceTypeDef]],
+    },
+)
+ContentRetrievalRuleOutputTypeDef = TypedDict(
+    "ContentRetrievalRuleOutputTypeDef",
+    {
+        "eligibleDataSources": NotRequired[List[EligibleDataSourceTypeDef]],
+    },
+)
 ContentRetrievalRuleTypeDef = TypedDict(
     "ContentRetrievalRuleTypeDef",
     {
-        "eligibleDataSources": NotRequired[List[EligibleDataSourceTypeDef]],
+        "eligibleDataSources": NotRequired[Sequence[EligibleDataSourceTypeDef]],
     },
 )
 ListConversationsResponseTypeDef = TypedDict(
     "ListConversationsResponseTypeDef",
     {
-        "conversations": List[ConversationTypeDef],
         "nextToken": str,
+        "conversations": List[ConversationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
-        "applicationArn": str,
-        "applicationId": str,
-        "attachmentsConfiguration": AppliedAttachmentsConfigurationTypeDef,
-        "createdAt": datetime,
-        "description": str,
         "displayName": str,
-        "encryptionConfiguration": EncryptionConfigurationTypeDef,
-        "error": ErrorDetailTypeDef,
+        "applicationId": str,
+        "applicationArn": str,
         "identityCenterApplicationArn": str,
         "roleArn": str,
         "status": ApplicationStatusType,
+        "description": str,
+        "encryptionConfiguration": EncryptionConfigurationTypeDef,
+        "createdAt": datetime,
         "updatedAt": datetime,
+        "error": ErrorDetailTypeDef,
+        "attachmentsConfiguration": AppliedAttachmentsConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateApplicationRequestRequestTypeDef = TypedDict(
     "CreateApplicationRequestRequestTypeDef",
     {
         "displayName": str,
-        "roleArn": str,
-        "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
-        "clientToken": NotRequired[str],
+        "roleArn": NotRequired[str],
+        "identityCenterInstanceArn": NotRequired[str],
         "description": NotRequired[str],
         "encryptionConfiguration": NotRequired[EncryptionConfigurationTypeDef],
-        "identityCenterInstanceArn": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
+        "clientToken": NotRequired[str],
+        "attachmentsConfiguration": NotRequired[AttachmentsConfigurationTypeDef],
     },
 )
 CreateWebExperienceRequestRequestTypeDef = TypedDict(
     "CreateWebExperienceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "clientToken": NotRequired[str],
-        "roleArn": NotRequired[str],
-        "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
-        "subtitle": NotRequired[str],
-        "tags": NotRequired[Sequence[TagTypeDef]],
         "title": NotRequired[str],
+        "subtitle": NotRequired[str],
         "welcomeMessage": NotRequired[str],
+        "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
+        "roleArn": NotRequired[str],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+        "clientToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1091,143 +1219,165 @@
     },
 )
 CreateIndexRequestRequestTypeDef = TypedDict(
     "CreateIndexRequestRequestTypeDef",
     {
         "applicationId": str,
         "displayName": str,
-        "capacityConfiguration": NotRequired[IndexCapacityConfigurationTypeDef],
-        "clientToken": NotRequired[str],
+        "type": NotRequired[IndexTypeType],
         "description": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
+        "capacityConfiguration": NotRequired[IndexCapacityConfigurationTypeDef],
+        "clientToken": NotRequired[str],
     },
 )
 CreateUserRequestRequestTypeDef = TypedDict(
     "CreateUserRequestRequestTypeDef",
     {
         "applicationId": str,
         "userId": str,
-        "clientToken": NotRequired[str],
         "userAliases": NotRequired[Sequence[UserAliasTypeDef]],
+        "clientToken": NotRequired[str],
     },
 )
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "userAliases": List[UserAliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateUserRequestRequestTypeDef = TypedDict(
     "UpdateUserRequestRequestTypeDef",
     {
         "applicationId": str,
         "userId": str,
-        "userAliasesToDelete": NotRequired[Sequence[UserAliasTypeDef]],
         "userAliasesToUpdate": NotRequired[Sequence[UserAliasTypeDef]],
+        "userAliasesToDelete": NotRequired[Sequence[UserAliasTypeDef]],
     },
 )
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "userAliasesAdded": List[UserAliasTypeDef],
-        "userAliasesDeleted": List[UserAliasTypeDef],
         "userAliasesUpdated": List[UserAliasTypeDef],
+        "userAliasesDeleted": List[UserAliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DataSourceSyncJobTypeDef = TypedDict(
     "DataSourceSyncJobTypeDef",
     {
-        "dataSourceErrorCode": NotRequired[str],
-        "endTime": NotRequired[datetime],
-        "error": NotRequired[ErrorDetailTypeDef],
         "executionId": NotRequired[str],
-        "metrics": NotRequired[DataSourceSyncJobMetricsTypeDef],
         "startTime": NotRequired[datetime],
+        "endTime": NotRequired[datetime],
         "status": NotRequired[DataSourceSyncJobStatusType],
+        "error": NotRequired[ErrorDetailTypeDef],
+        "dataSourceErrorCode": NotRequired[str],
+        "metrics": NotRequired[DataSourceSyncJobMetricsTypeDef],
     },
 )
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "dataSources": List[DataSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DataSourceVpcConfigurationUnionTypeDef = Union[
+    DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
+]
+DocumentAttributeBoostingConfigurationOutputTypeDef = TypedDict(
+    "DocumentAttributeBoostingConfigurationOutputTypeDef",
+    {
+        "numberConfiguration": NotRequired[NumberAttributeBoostingConfigurationTypeDef],
+        "stringConfiguration": NotRequired[StringAttributeBoostingConfigurationOutputTypeDef],
+        "dateConfiguration": NotRequired[DateAttributeBoostingConfigurationTypeDef],
+        "stringListConfiguration": NotRequired[StringListAttributeBoostingConfigurationTypeDef],
+    },
+)
 DocumentAttributeBoostingConfigurationTypeDef = TypedDict(
     "DocumentAttributeBoostingConfigurationTypeDef",
     {
-        "dateConfiguration": NotRequired[DateAttributeBoostingConfigurationTypeDef],
         "numberConfiguration": NotRequired[NumberAttributeBoostingConfigurationTypeDef],
         "stringConfiguration": NotRequired[StringAttributeBoostingConfigurationTypeDef],
+        "dateConfiguration": NotRequired[DateAttributeBoostingConfigurationTypeDef],
         "stringListConfiguration": NotRequired[StringListAttributeBoostingConfigurationTypeDef],
     },
 )
+DocumentAttributeConditionOutputTypeDef = TypedDict(
+    "DocumentAttributeConditionOutputTypeDef",
+    {
+        "key": str,
+        "operator": DocumentEnrichmentConditionOperatorType,
+        "value": NotRequired[DocumentAttributeValueOutputTypeDef],
+    },
+)
+DocumentAttributeTargetOutputTypeDef = TypedDict(
+    "DocumentAttributeTargetOutputTypeDef",
+    {
+        "key": str,
+        "value": NotRequired[DocumentAttributeValueOutputTypeDef],
+        "attributeValueOperator": NotRequired[Literal["DELETE"]],
+    },
+)
 UpdateIndexRequestRequestTypeDef = TypedDict(
     "UpdateIndexRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
-        "capacityConfiguration": NotRequired[IndexCapacityConfigurationTypeDef],
-        "description": NotRequired[str],
         "displayName": NotRequired[str],
+        "description": NotRequired[str],
+        "capacityConfiguration": NotRequired[IndexCapacityConfigurationTypeDef],
         "documentAttributeConfigurations": NotRequired[
             Sequence[DocumentAttributeConfigurationTypeDef]
         ],
     },
 )
 DocumentAttributeValueTypeDef = TypedDict(
     "DocumentAttributeValueTypeDef",
     {
-        "dateValue": NotRequired[TimestampTypeDef],
-        "longValue": NotRequired[int],
-        "stringListValue": NotRequired[Sequence[str]],
         "stringValue": NotRequired[str],
+        "stringListValue": NotRequired[Sequence[str]],
+        "longValue": NotRequired[int],
+        "dateValue": NotRequired[TimestampTypeDef],
     },
 )
 ListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
     "ListDataSourceSyncJobsRequestRequestTypeDef",
     {
-        "applicationId": str,
         "dataSourceId": str,
+        "applicationId": str,
         "indexId": str,
-        "endTime": NotRequired[TimestampTypeDef],
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
         "startTime": NotRequired[TimestampTypeDef],
+        "endTime": NotRequired[TimestampTypeDef],
         "statusFilter": NotRequired[DataSourceSyncJobStatusType],
     },
 )
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "applicationId": str,
         "indexId": str,
         "updatedEarlierThan": TimestampTypeDef,
         "dataSourceId": NotRequired[str],
-        "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
     },
 )
 MessageUsefulnessFeedbackTypeDef = TypedDict(
     "MessageUsefulnessFeedbackTypeDef",
     {
-        "submittedAt": TimestampTypeDef,
         "usefulness": MessageUsefulnessType,
-        "comment": NotRequired[str],
+        "submittedAt": TimestampTypeDef,
         "reason": NotRequired[MessageUsefulnessReasonType],
-    },
-)
-DocumentContentTypeDef = TypedDict(
-    "DocumentContentTypeDef",
-    {
-        "blob": NotRequired[BlobTypeDef],
-        "s3": NotRequired[S3TypeDef],
+        "comment": NotRequired[str],
     },
 )
 GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef = TypedDict(
     "GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef",
     {
         "applicationId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1246,19 +1396,19 @@
         "userId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef = TypedDict(
     "ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef",
     {
-        "applicationId": str,
         "dataSourceId": str,
+        "applicationId": str,
         "indexId": str,
-        "endTime": NotRequired[TimestampTypeDef],
         "startTime": NotRequired[TimestampTypeDef],
+        "endTime": NotRequired[TimestampTypeDef],
         "statusFilter": NotRequired[DataSourceSyncJobStatusType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     {
@@ -1292,16 +1442,16 @@
         "applicationId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListMessagesRequestListMessagesPaginateTypeDef = TypedDict(
     "ListMessagesRequestListMessagesPaginateTypeDef",
     {
-        "applicationId": str,
         "conversationId": str,
+        "applicationId": str,
         "userId": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
     "ListPluginsRequestListPluginsPaginateTypeDef",
     {
@@ -1329,97 +1479,114 @@
         "memberGroups": NotRequired[Sequence[MemberGroupTypeDef]],
         "memberUsers": NotRequired[Sequence[MemberUserTypeDef]],
     },
 )
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
-        "items": List[GroupSummaryTypeDef],
         "nextToken": str,
+        "items": List[GroupSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 IndexStatisticsTypeDef = TypedDict(
     "IndexStatisticsTypeDef",
     {
         "textDocumentStatistics": NotRequired[TextDocumentStatisticsTypeDef],
     },
 )
 ListIndicesResponseTypeDef = TypedDict(
     "ListIndicesResponseTypeDef",
     {
-        "indices": List[IndexTypeDef],
         "nextToken": str,
+        "indices": List[IndexTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListPluginsResponseTypeDef = TypedDict(
     "ListPluginsResponseTypeDef",
     {
         "nextToken": str,
         "plugins": List[PluginTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListRetrieversResponseTypeDef = TypedDict(
     "ListRetrieversResponseTypeDef",
     {
-        "nextToken": str,
         "retrievers": List[RetrieverTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWebExperiencesResponseTypeDef = TypedDict(
     "ListWebExperiencesResponseTypeDef",
     {
-        "nextToken": str,
         "webExperiences": List[WebExperienceTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+PluginAuthConfigurationOutputTypeDef = TypedDict(
+    "PluginAuthConfigurationOutputTypeDef",
+    {
+        "basicAuthConfiguration": NotRequired[BasicAuthConfigurationTypeDef],
+        "oAuth2ClientCredentialConfiguration": NotRequired[
+            OAuth2ClientCredentialConfigurationTypeDef
+        ],
+        "noAuthConfiguration": NotRequired[Dict[str, Any]],
+    },
+)
 PluginAuthConfigurationTypeDef = TypedDict(
     "PluginAuthConfigurationTypeDef",
     {
         "basicAuthConfiguration": NotRequired[BasicAuthConfigurationTypeDef],
         "oAuth2ClientCredentialConfiguration": NotRequired[
             OAuth2ClientCredentialConfigurationTypeDef
         ],
+        "noAuthConfiguration": NotRequired[Mapping[str, Any]],
     },
 )
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
-        "group": NotRequired[PrincipalGroupTypeDef],
         "user": NotRequired[PrincipalUserTypeDef],
+        "group": NotRequired[PrincipalGroupTypeDef],
     },
 )
 WebExperienceAuthConfigurationTypeDef = TypedDict(
     "WebExperienceAuthConfigurationTypeDef",
     {
         "samlConfiguration": NotRequired[SamlConfigurationTypeDef],
     },
 )
-SourceAttributionTypeDef = TypedDict(
-    "SourceAttributionTypeDef",
+TextSegmentTypeDef = TypedDict(
+    "TextSegmentTypeDef",
     {
-        "citationNumber": NotRequired[int],
-        "snippet": NotRequired[str],
-        "textMessageSegments": NotRequired[List[TextSegmentTypeDef]],
-        "title": NotRequired[str],
-        "updatedAt": NotRequired[datetime],
-        "url": NotRequired[str],
+        "beginOffset": NotRequired[int],
+        "endOffset": NotRequired[int],
+        "snippetExcerpt": NotRequired[SnippetExcerptTypeDef],
+    },
+)
+CustomPluginConfigurationTypeDef = TypedDict(
+    "CustomPluginConfigurationTypeDef",
+    {
+        "description": str,
+        "apiSchemaType": Literal["OPEN_API_V3"],
+        "apiSchema": APISchemaTypeDef,
     },
 )
+ActionExecutionUnionTypeDef = Union[ActionExecutionTypeDef, ActionExecutionExtraOutputTypeDef]
 ActionReviewTypeDef = TypedDict(
     "ActionReviewTypeDef",
     {
-        "payload": NotRequired[Dict[str, ActionReviewPayloadFieldTypeDef]],
-        "payloadFieldNameSeparator": NotRequired[str],
         "pluginId": NotRequired[str],
         "pluginType": NotRequired[PluginTypeType],
+        "payload": NotRequired[Dict[str, ActionReviewPayloadFieldTypeDef]],
+        "payloadFieldNameSeparator": NotRequired[str],
     },
 )
 ListDocumentsResponseTypeDef = TypedDict(
     "ListDocumentsResponseTypeDef",
     {
         "documentDetailList": List[DocumentDetailsTypeDef],
         "nextToken": str,
@@ -1448,25 +1615,40 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ChatSyncInputRequestTypeDef = TypedDict(
     "ChatSyncInputRequestTypeDef",
     {
         "applicationId": str,
-        "actionExecution": NotRequired[ActionExecutionTypeDef],
+        "userId": NotRequired[str],
+        "userGroups": NotRequired[Sequence[str]],
+        "userMessage": NotRequired[str],
         "attachments": NotRequired[Sequence[AttachmentInputTypeDef]],
+        "actionExecution": NotRequired[ActionExecutionTypeDef],
+        "authChallengeResponse": NotRequired[AuthChallengeResponseTypeDef],
+        "conversationId": NotRequired[str],
+        "parentMessageId": NotRequired[str],
         "attributeFilter": NotRequired["AttributeFilterTypeDef"],
         "chatMode": NotRequired[ChatModeType],
         "chatModeConfiguration": NotRequired[ChatModeConfigurationTypeDef],
         "clientToken": NotRequired[str],
-        "conversationId": NotRequired[str],
-        "parentMessageId": NotRequired[str],
-        "userGroups": NotRequired[Sequence[str]],
-        "userId": NotRequired[str],
-        "userMessage": NotRequired[str],
+    },
+)
+RuleConfigurationExtraOutputTypeDef = TypedDict(
+    "RuleConfigurationExtraOutputTypeDef",
+    {
+        "contentBlockerRule": NotRequired[ContentBlockerRuleTypeDef],
+        "contentRetrievalRule": NotRequired[ContentRetrievalRuleExtraOutputTypeDef],
+    },
+)
+RuleConfigurationOutputTypeDef = TypedDict(
+    "RuleConfigurationOutputTypeDef",
+    {
+        "contentBlockerRule": NotRequired[ContentBlockerRuleTypeDef],
+        "contentRetrievalRule": NotRequired[ContentRetrievalRuleOutputTypeDef],
     },
 )
 RuleConfigurationTypeDef = TypedDict(
     "RuleConfigurationTypeDef",
     {
         "contentBlockerRule": NotRequired[ContentBlockerRuleTypeDef],
         "contentRetrievalRule": NotRequired[ContentRetrievalRuleTypeDef],
@@ -1476,37 +1658,63 @@
     "ListDataSourceSyncJobsResponseTypeDef",
     {
         "history": List[DataSourceSyncJobTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+NativeIndexConfigurationOutputTypeDef = TypedDict(
+    "NativeIndexConfigurationOutputTypeDef",
+    {
+        "indexId": str,
+        "boostingOverride": NotRequired[
+            Dict[str, DocumentAttributeBoostingConfigurationOutputTypeDef]
+        ],
+    },
+)
 NativeIndexConfigurationTypeDef = TypedDict(
     "NativeIndexConfigurationTypeDef",
     {
         "indexId": str,
         "boostingOverride": NotRequired[
             Mapping[str, DocumentAttributeBoostingConfigurationTypeDef]
         ],
     },
 )
+HookConfigurationOutputTypeDef = TypedDict(
+    "HookConfigurationOutputTypeDef",
+    {
+        "invocationCondition": NotRequired[DocumentAttributeConditionOutputTypeDef],
+        "lambdaArn": NotRequired[str],
+        "s3BucketName": NotRequired[str],
+        "roleArn": NotRequired[str],
+    },
+)
+InlineDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
+    "InlineDocumentEnrichmentConfigurationOutputTypeDef",
+    {
+        "condition": NotRequired[DocumentAttributeConditionOutputTypeDef],
+        "target": NotRequired[DocumentAttributeTargetOutputTypeDef],
+        "documentContentOperator": NotRequired[Literal["DELETE"]],
+    },
+)
 DocumentAttributeConditionTypeDef = TypedDict(
     "DocumentAttributeConditionTypeDef",
     {
         "key": str,
         "operator": DocumentEnrichmentConditionOperatorType,
         "value": NotRequired[DocumentAttributeValueTypeDef],
     },
 )
 DocumentAttributeTargetTypeDef = TypedDict(
     "DocumentAttributeTargetTypeDef",
     {
         "key": str,
-        "attributeValueOperator": NotRequired[Literal["DELETE"]],
         "value": NotRequired[DocumentAttributeValueTypeDef],
+        "attributeValueOperator": NotRequired[Literal["DELETE"]],
     },
 )
 DocumentAttributeTypeDef = TypedDict(
     "DocumentAttributeTypeDef",
     {
         "name": str,
         "value": DocumentAttributeValueTypeDef,
@@ -1514,382 +1722,446 @@
 )
 PutFeedbackRequestRequestTypeDef = TypedDict(
     "PutFeedbackRequestRequestTypeDef",
     {
         "applicationId": str,
         "conversationId": str,
         "messageId": str,
+        "userId": NotRequired[str],
         "messageCopiedAt": NotRequired[TimestampTypeDef],
         "messageUsefulness": NotRequired[MessageUsefulnessFeedbackTypeDef],
-        "userId": NotRequired[str],
     },
 )
 PutGroupRequestRequestTypeDef = TypedDict(
     "PutGroupRequestRequestTypeDef",
     {
         "applicationId": str,
-        "groupMembers": GroupMembersTypeDef,
-        "groupName": str,
         "indexId": str,
+        "groupName": str,
         "type": MembershipTypeType,
+        "groupMembers": GroupMembersTypeDef,
         "dataSourceId": NotRequired[str],
     },
 )
 GetIndexResponseTypeDef = TypedDict(
     "GetIndexResponseTypeDef",
     {
         "applicationId": str,
-        "capacityConfiguration": IndexCapacityConfigurationTypeDef,
-        "createdAt": datetime,
-        "description": str,
+        "indexId": str,
         "displayName": str,
-        "documentAttributeConfigurations": List[DocumentAttributeConfigurationTypeDef],
-        "error": ErrorDetailTypeDef,
+        "type": IndexTypeType,
         "indexArn": str,
-        "indexId": str,
-        "indexStatistics": IndexStatisticsTypeDef,
         "status": IndexStatusType,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreatePluginRequestRequestTypeDef = TypedDict(
-    "CreatePluginRequestRequestTypeDef",
-    {
-        "applicationId": str,
-        "authConfiguration": PluginAuthConfigurationTypeDef,
-        "displayName": str,
-        "serverUrl": str,
-        "type": PluginTypeType,
-        "clientToken": NotRequired[str],
-        "tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
-GetPluginResponseTypeDef = TypedDict(
-    "GetPluginResponseTypeDef",
-    {
-        "applicationId": str,
-        "authConfiguration": PluginAuthConfigurationTypeDef,
+        "description": str,
         "createdAt": datetime,
-        "displayName": str,
-        "pluginArn": str,
-        "pluginId": str,
-        "serverUrl": str,
-        "state": PluginStateType,
-        "type": PluginTypeType,
         "updatedAt": datetime,
+        "capacityConfiguration": IndexCapacityConfigurationTypeDef,
+        "documentAttributeConfigurations": List[DocumentAttributeConfigurationTypeDef],
+        "error": ErrorDetailTypeDef,
+        "indexStatistics": IndexStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdatePluginRequestRequestTypeDef = TypedDict(
-    "UpdatePluginRequestRequestTypeDef",
-    {
-        "applicationId": str,
-        "pluginId": str,
-        "authConfiguration": NotRequired[PluginAuthConfigurationTypeDef],
-        "displayName": NotRequired[str],
-        "serverUrl": NotRequired[str],
-        "state": NotRequired[PluginStateType],
-    },
-)
+PluginAuthConfigurationUnionTypeDef = Union[
+    PluginAuthConfigurationTypeDef, PluginAuthConfigurationOutputTypeDef
+]
 AccessControlTypeDef = TypedDict(
     "AccessControlTypeDef",
     {
         "principals": Sequence[PrincipalTypeDef],
         "memberRelation": NotRequired[MemberRelationType],
     },
 )
 GetWebExperienceResponseTypeDef = TypedDict(
     "GetWebExperienceResponseTypeDef",
     {
         "applicationId": str,
-        "authenticationConfiguration": WebExperienceAuthConfigurationTypeDef,
-        "createdAt": datetime,
+        "webExperienceId": str,
+        "webExperienceArn": str,
         "defaultEndpoint": str,
-        "error": ErrorDetailTypeDef,
-        "roleArn": str,
-        "samplePromptsControlMode": WebExperienceSamplePromptsControlModeType,
         "status": WebExperienceStatusType,
-        "subtitle": str,
-        "title": str,
+        "createdAt": datetime,
         "updatedAt": datetime,
-        "webExperienceArn": str,
-        "webExperienceId": str,
+        "title": str,
+        "subtitle": str,
         "welcomeMessage": str,
+        "samplePromptsControlMode": WebExperienceSamplePromptsControlModeType,
+        "roleArn": str,
+        "authenticationConfiguration": WebExperienceAuthConfigurationTypeDef,
+        "error": ErrorDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateWebExperienceRequestRequestTypeDef = TypedDict(
     "UpdateWebExperienceRequestRequestTypeDef",
     {
         "applicationId": str,
         "webExperienceId": str,
+        "roleArn": NotRequired[str],
         "authenticationConfiguration": NotRequired[WebExperienceAuthConfigurationTypeDef],
-        "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
-        "subtitle": NotRequired[str],
         "title": NotRequired[str],
+        "subtitle": NotRequired[str],
         "welcomeMessage": NotRequired[str],
+        "samplePromptsControlMode": NotRequired[WebExperienceSamplePromptsControlModeType],
     },
 )
-ChatSyncOutputTypeDef = TypedDict(
-    "ChatSyncOutputTypeDef",
+SourceAttributionTypeDef = TypedDict(
+    "SourceAttributionTypeDef",
     {
-        "actionReview": ActionReviewTypeDef,
-        "conversationId": str,
-        "failedAttachments": List[AttachmentOutputTypeDef],
-        "sourceAttributions": List[SourceAttributionTypeDef],
-        "systemMessage": str,
-        "systemMessageId": str,
-        "userMessageId": str,
+        "title": NotRequired[str],
+        "snippet": NotRequired[str],
+        "url": NotRequired[str],
+        "citationNumber": NotRequired[int],
+        "updatedAt": NotRequired[datetime],
+        "textMessageSegments": NotRequired[List[TextSegmentTypeDef]],
+    },
+)
+CreatePluginRequestRequestTypeDef = TypedDict(
+    "CreatePluginRequestRequestTypeDef",
+    {
+        "applicationId": str,
+        "displayName": str,
+        "type": PluginTypeType,
+        "authConfiguration": PluginAuthConfigurationTypeDef,
+        "serverUrl": NotRequired[str],
+        "customPluginConfiguration": NotRequired[CustomPluginConfigurationTypeDef],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+        "clientToken": NotRequired[str],
+    },
+)
+GetPluginResponseTypeDef = TypedDict(
+    "GetPluginResponseTypeDef",
+    {
+        "applicationId": str,
+        "pluginId": str,
+        "displayName": str,
+        "type": PluginTypeType,
+        "serverUrl": str,
+        "authConfiguration": PluginAuthConfigurationOutputTypeDef,
+        "customPluginConfiguration": CustomPluginConfigurationTypeDef,
+        "buildStatus": PluginBuildStatusType,
+        "pluginArn": str,
+        "state": PluginStateType,
+        "createdAt": datetime,
+        "updatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-MessagePaginatorTypeDef = TypedDict(
-    "MessagePaginatorTypeDef",
+UpdatePluginRequestRequestTypeDef = TypedDict(
+    "UpdatePluginRequestRequestTypeDef",
     {
-        "actionExecution": NotRequired[ActionExecutionPaginatorTypeDef],
-        "actionReview": NotRequired[ActionReviewTypeDef],
-        "attachments": NotRequired[List[AttachmentOutputTypeDef]],
-        "body": NotRequired[str],
-        "messageId": NotRequired[str],
-        "sourceAttribution": NotRequired[List[SourceAttributionTypeDef]],
-        "time": NotRequired[datetime],
-        "type": NotRequired[MessageTypeType],
+        "applicationId": str,
+        "pluginId": str,
+        "displayName": NotRequired[str],
+        "state": NotRequired[PluginStateType],
+        "serverUrl": NotRequired[str],
+        "customPluginConfiguration": NotRequired[CustomPluginConfigurationTypeDef],
+        "authConfiguration": NotRequired[PluginAuthConfigurationTypeDef],
     },
 )
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
+RuleExtraOutputTypeDef = TypedDict(
+    "RuleExtraOutputTypeDef",
     {
-        "actionExecution": NotRequired[ActionExecutionTypeDef],
-        "actionReview": NotRequired[ActionReviewTypeDef],
-        "attachments": NotRequired[List[AttachmentOutputTypeDef]],
-        "body": NotRequired[str],
-        "messageId": NotRequired[str],
-        "sourceAttribution": NotRequired[List[SourceAttributionTypeDef]],
-        "time": NotRequired[datetime],
-        "type": NotRequired[MessageTypeType],
+        "ruleType": RuleTypeType,
+        "includedUsersAndGroups": NotRequired[UsersAndGroupsExtraOutputTypeDef],
+        "excludedUsersAndGroups": NotRequired[UsersAndGroupsExtraOutputTypeDef],
+        "ruleConfiguration": NotRequired[RuleConfigurationExtraOutputTypeDef],
+    },
+)
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "ruleType": RuleTypeType,
+        "includedUsersAndGroups": NotRequired[UsersAndGroupsOutputTypeDef],
+        "excludedUsersAndGroups": NotRequired[UsersAndGroupsOutputTypeDef],
+        "ruleConfiguration": NotRequired[RuleConfigurationOutputTypeDef],
     },
 )
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "ruleType": RuleTypeType,
-        "excludedUsersAndGroups": NotRequired[UsersAndGroupsTypeDef],
         "includedUsersAndGroups": NotRequired[UsersAndGroupsTypeDef],
+        "excludedUsersAndGroups": NotRequired[UsersAndGroupsTypeDef],
         "ruleConfiguration": NotRequired[RuleConfigurationTypeDef],
     },
 )
+RetrieverConfigurationOutputTypeDef = TypedDict(
+    "RetrieverConfigurationOutputTypeDef",
+    {
+        "nativeIndexConfiguration": NotRequired[NativeIndexConfigurationOutputTypeDef],
+        "kendraIndexConfiguration": NotRequired[KendraIndexConfigurationTypeDef],
+    },
+)
 RetrieverConfigurationTypeDef = TypedDict(
     "RetrieverConfigurationTypeDef",
     {
-        "kendraIndexConfiguration": NotRequired[KendraIndexConfigurationTypeDef],
         "nativeIndexConfiguration": NotRequired[NativeIndexConfigurationTypeDef],
+        "kendraIndexConfiguration": NotRequired[KendraIndexConfigurationTypeDef],
+    },
+)
+DocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
+    "DocumentEnrichmentConfigurationOutputTypeDef",
+    {
+        "inlineConfigurations": NotRequired[
+            List[InlineDocumentEnrichmentConfigurationOutputTypeDef]
+        ],
+        "preExtractionHookConfiguration": NotRequired[HookConfigurationOutputTypeDef],
+        "postExtractionHookConfiguration": NotRequired[HookConfigurationOutputTypeDef],
     },
 )
 HookConfigurationTypeDef = TypedDict(
     "HookConfigurationTypeDef",
     {
         "invocationCondition": NotRequired[DocumentAttributeConditionTypeDef],
         "lambdaArn": NotRequired[str],
-        "roleArn": NotRequired[str],
         "s3BucketName": NotRequired[str],
+        "roleArn": NotRequired[str],
     },
 )
 InlineDocumentEnrichmentConfigurationTypeDef = TypedDict(
     "InlineDocumentEnrichmentConfigurationTypeDef",
     {
         "condition": NotRequired[DocumentAttributeConditionTypeDef],
-        "documentContentOperator": NotRequired[Literal["DELETE"]],
         "target": NotRequired[DocumentAttributeTargetTypeDef],
+        "documentContentOperator": NotRequired[Literal["DELETE"]],
     },
 )
 AttributeFilterTypeDef = TypedDict(
     "AttributeFilterTypeDef",
     {
         "andAllFilters": NotRequired[Sequence[Dict[str, Any]]],
+        "orAllFilters": NotRequired[Sequence[Dict[str, Any]]],
+        "notFilter": NotRequired[Dict[str, Any]],
+        "equalsTo": NotRequired[DocumentAttributeTypeDef],
         "containsAll": NotRequired[DocumentAttributeTypeDef],
         "containsAny": NotRequired[DocumentAttributeTypeDef],
-        "equalsTo": NotRequired[DocumentAttributeTypeDef],
         "greaterThan": NotRequired[DocumentAttributeTypeDef],
         "greaterThanOrEquals": NotRequired[DocumentAttributeTypeDef],
         "lessThan": NotRequired[DocumentAttributeTypeDef],
         "lessThanOrEquals": NotRequired[DocumentAttributeTypeDef],
-        "notFilter": NotRequired[Dict[str, Any]],
-        "orAllFilters": NotRequired[Sequence[Dict[str, Any]]],
     },
 )
 AccessConfigurationTypeDef = TypedDict(
     "AccessConfigurationTypeDef",
     {
         "accessControls": Sequence[AccessControlTypeDef],
         "memberRelation": NotRequired[MemberRelationType],
     },
 )
-ListMessagesResponsePaginatorTypeDef = TypedDict(
-    "ListMessagesResponsePaginatorTypeDef",
+ChatSyncOutputTypeDef = TypedDict(
+    "ChatSyncOutputTypeDef",
     {
-        "messages": List[MessagePaginatorTypeDef],
-        "nextToken": str,
+        "conversationId": str,
+        "systemMessage": str,
+        "systemMessageId": str,
+        "userMessageId": str,
+        "actionReview": ActionReviewTypeDef,
+        "authChallengeRequest": AuthChallengeRequestTypeDef,
+        "sourceAttributions": List[SourceAttributionTypeDef],
+        "failedAttachments": List[AttachmentOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListMessagesResponseTypeDef = TypedDict(
-    "ListMessagesResponseTypeDef",
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
-        "messages": List[MessageTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "messageId": NotRequired[str],
+        "body": NotRequired[str],
+        "time": NotRequired[datetime],
+        "type": NotRequired[MessageTypeType],
+        "attachments": NotRequired[List[AttachmentOutputTypeDef]],
+        "sourceAttribution": NotRequired[List[SourceAttributionTypeDef]],
+        "actionReview": NotRequired[ActionReviewTypeDef],
+        "actionExecution": NotRequired[ActionExecutionOutputTypeDef],
     },
 )
-TopicConfigurationTypeDef = TypedDict(
-    "TopicConfigurationTypeDef",
+TopicConfigurationExtraOutputTypeDef = TypedDict(
+    "TopicConfigurationExtraOutputTypeDef",
     {
         "name": str,
-        "rules": List[RuleTypeDef],
+        "rules": List[RuleExtraOutputTypeDef],
         "description": NotRequired[str],
         "exampleChatMessages": NotRequired[List[str]],
     },
 )
-CreateRetrieverRequestRequestTypeDef = TypedDict(
-    "CreateRetrieverRequestRequestTypeDef",
+TopicConfigurationOutputTypeDef = TypedDict(
+    "TopicConfigurationOutputTypeDef",
     {
-        "applicationId": str,
-        "configuration": RetrieverConfigurationTypeDef,
-        "displayName": str,
-        "type": RetrieverTypeType,
-        "clientToken": NotRequired[str],
-        "roleArn": NotRequired[str],
-        "tags": NotRequired[Sequence[TagTypeDef]],
+        "name": str,
+        "rules": List[RuleOutputTypeDef],
+        "description": NotRequired[str],
+        "exampleChatMessages": NotRequired[List[str]],
+    },
+)
+TopicConfigurationTypeDef = TypedDict(
+    "TopicConfigurationTypeDef",
+    {
+        "name": str,
+        "rules": Sequence[RuleTypeDef],
+        "description": NotRequired[str],
+        "exampleChatMessages": NotRequired[Sequence[str]],
     },
 )
 GetRetrieverResponseTypeDef = TypedDict(
     "GetRetrieverResponseTypeDef",
     {
         "applicationId": str,
-        "configuration": RetrieverConfigurationTypeDef,
-        "createdAt": datetime,
-        "displayName": str,
-        "retrieverArn": str,
         "retrieverId": str,
-        "roleArn": str,
-        "status": RetrieverStatusType,
+        "retrieverArn": str,
         "type": RetrieverTypeType,
+        "status": RetrieverStatusType,
+        "displayName": str,
+        "configuration": RetrieverConfigurationOutputTypeDef,
+        "roleArn": str,
+        "createdAt": datetime,
         "updatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateRetrieverRequestRequestTypeDef = TypedDict(
+    "CreateRetrieverRequestRequestTypeDef",
+    {
+        "applicationId": str,
+        "type": RetrieverTypeType,
+        "displayName": str,
+        "configuration": RetrieverConfigurationTypeDef,
+        "roleArn": NotRequired[str],
+        "clientToken": NotRequired[str],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+RetrieverConfigurationUnionTypeDef = Union[
+    RetrieverConfigurationTypeDef, RetrieverConfigurationOutputTypeDef
+]
 UpdateRetrieverRequestRequestTypeDef = TypedDict(
     "UpdateRetrieverRequestRequestTypeDef",
     {
         "applicationId": str,
         "retrieverId": str,
         "configuration": NotRequired[RetrieverConfigurationTypeDef],
         "displayName": NotRequired[str],
         "roleArn": NotRequired[str],
     },
 )
+GetDataSourceResponseTypeDef = TypedDict(
+    "GetDataSourceResponseTypeDef",
+    {
+        "applicationId": str,
+        "indexId": str,
+        "dataSourceId": str,
+        "dataSourceArn": str,
+        "displayName": str,
+        "type": str,
+        "configuration": Dict[str, Any],
+        "vpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "description": str,
+        "status": DataSourceStatusType,
+        "syncSchedule": str,
+        "roleArn": str,
+        "error": ErrorDetailTypeDef,
+        "documentEnrichmentConfiguration": DocumentEnrichmentConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DocumentEnrichmentConfigurationTypeDef = TypedDict(
     "DocumentEnrichmentConfigurationTypeDef",
     {
         "inlineConfigurations": NotRequired[Sequence[InlineDocumentEnrichmentConfigurationTypeDef]],
-        "postExtractionHookConfiguration": NotRequired[HookConfigurationTypeDef],
         "preExtractionHookConfiguration": NotRequired[HookConfigurationTypeDef],
+        "postExtractionHookConfiguration": NotRequired[HookConfigurationTypeDef],
+    },
+)
+ListMessagesResponseTypeDef = TypedDict(
+    "ListMessagesResponseTypeDef",
+    {
+        "messages": List[MessageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetChatControlsConfigurationResponseTypeDef = TypedDict(
     "GetChatControlsConfigurationResponseTypeDef",
     {
+        "responseScope": ResponseScopeType,
         "blockedPhrases": BlockedPhrasesConfigurationTypeDef,
+        "topicConfigurations": List[TopicConfigurationExtraOutputTypeDef],
         "creatorModeConfiguration": AppliedCreatorModeConfigurationTypeDef,
         "nextToken": str,
-        "responseScope": ResponseScopeType,
-        "topicConfigurations": List[TopicConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateChatControlsConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateChatControlsConfigurationRequestRequestTypeDef",
-    {
-        "applicationId": str,
-        "blockedPhrasesConfigurationUpdate": NotRequired[BlockedPhrasesConfigurationUpdateTypeDef],
-        "clientToken": NotRequired[str],
-        "creatorModeConfiguration": NotRequired[CreatorModeConfigurationTypeDef],
-        "responseScope": NotRequired[ResponseScopeType],
-        "topicConfigurationsToCreateOrUpdate": NotRequired[Sequence[TopicConfigurationTypeDef]],
-        "topicConfigurationsToDelete": NotRequired[Sequence[TopicConfigurationTypeDef]],
-    },
-)
+TopicConfigurationUnionTypeDef = Union[
+    TopicConfigurationTypeDef, TopicConfigurationExtraOutputTypeDef
+]
 CreateDataSourceRequestRequestTypeDef = TypedDict(
     "CreateDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "configuration": Mapping[str, Any],
-        "displayName": str,
         "indexId": str,
-        "clientToken": NotRequired[str],
+        "displayName": str,
+        "configuration": Mapping[str, Any],
+        "vpcConfiguration": NotRequired[DataSourceVpcConfigurationTypeDef],
         "description": NotRequired[str],
-        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
-        "roleArn": NotRequired[str],
-        "syncSchedule": NotRequired[str],
         "tags": NotRequired[Sequence[TagTypeDef]],
-        "vpcConfiguration": NotRequired[DataSourceVpcConfigurationTypeDef],
+        "syncSchedule": NotRequired[str],
+        "roleArn": NotRequired[str],
+        "clientToken": NotRequired[str],
+        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
     },
 )
+DocumentEnrichmentConfigurationUnionTypeDef = Union[
+    DocumentEnrichmentConfigurationTypeDef, DocumentEnrichmentConfigurationOutputTypeDef
+]
 DocumentTypeDef = TypedDict(
     "DocumentTypeDef",
     {
         "id": str,
-        "accessConfiguration": NotRequired[AccessConfigurationTypeDef],
         "attributes": NotRequired[Sequence[DocumentAttributeTypeDef]],
         "content": NotRequired[DocumentContentTypeDef],
         "contentType": NotRequired[ContentTypeType],
-        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
         "title": NotRequired[str],
-    },
-)
-GetDataSourceResponseTypeDef = TypedDict(
-    "GetDataSourceResponseTypeDef",
-    {
-        "applicationId": str,
-        "configuration": Dict[str, Any],
-        "createdAt": datetime,
-        "dataSourceArn": str,
-        "dataSourceId": str,
-        "description": str,
-        "displayName": str,
-        "documentEnrichmentConfiguration": DocumentEnrichmentConfigurationTypeDef,
-        "error": ErrorDetailTypeDef,
-        "indexId": str,
-        "roleArn": str,
-        "status": DataSourceStatusType,
-        "syncSchedule": str,
-        "type": str,
-        "updatedAt": datetime,
-        "vpcConfiguration": DataSourceVpcConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accessConfiguration": NotRequired[AccessConfigurationTypeDef],
+        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
     },
 )
 UpdateDataSourceRequestRequestTypeDef = TypedDict(
     "UpdateDataSourceRequestRequestTypeDef",
     {
         "applicationId": str,
-        "dataSourceId": str,
         "indexId": str,
+        "dataSourceId": str,
+        "displayName": NotRequired[str],
         "configuration": NotRequired[Mapping[str, Any]],
+        "vpcConfiguration": NotRequired[DataSourceVpcConfigurationTypeDef],
         "description": NotRequired[str],
-        "displayName": NotRequired[str],
-        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
-        "roleArn": NotRequired[str],
         "syncSchedule": NotRequired[str],
-        "vpcConfiguration": NotRequired[DataSourceVpcConfigurationTypeDef],
+        "roleArn": NotRequired[str],
+        "documentEnrichmentConfiguration": NotRequired[DocumentEnrichmentConfigurationTypeDef],
+    },
+)
+UpdateChatControlsConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateChatControlsConfigurationRequestRequestTypeDef",
+    {
+        "applicationId": str,
+        "clientToken": NotRequired[str],
+        "responseScope": NotRequired[ResponseScopeType],
+        "blockedPhrasesConfigurationUpdate": NotRequired[BlockedPhrasesConfigurationUpdateTypeDef],
+        "topicConfigurationsToCreateOrUpdate": NotRequired[
+            Sequence[TopicConfigurationUnionTypeDef]
+        ],
+        "topicConfigurationsToDelete": NotRequired[Sequence[TopicConfigurationUnionTypeDef]],
+        "creatorModeConfiguration": NotRequired[CreatorModeConfigurationTypeDef],
     },
 )
 BatchPutDocumentRequestRequestTypeDef = TypedDict(
     "BatchPutDocumentRequestRequestTypeDef",
     {
         "applicationId": str,
-        "documents": Sequence[DocumentTypeDef],
         "indexId": str,
-        "dataSourceSyncId": NotRequired[str],
+        "documents": Sequence[DocumentTypeDef],
         "roleArn": NotRequired[str],
+        "dataSourceSyncId": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/PKG-INFO` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qbusiness
-Version: 1.34.86
-Summary: Type annotations for boto3.QBusiness 1.34.86 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.95
+Summary: Type annotations for boto3.QBusiness 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-qbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qbusiness)](https://pepy.tech/project/mypy-boto3-qbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QBusiness 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
+[boto3.QBusiness 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,35 +331,35 @@
 `mypy_boto3_qbusiness.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 Full list of `QBusiness` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/literals/).
 
 ```python
-from mypy_boto3_qbusiness.literals import ActionPayloadFieldTypeType
+from mypy_boto3_qbusiness.literals import APISchemaTypeType
 
 
-def check_value(value: ActionPayloadFieldTypeType) -> bool: ...
+def check_value(value: APISchemaTypeType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_qbusiness.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
 Full list of `QBusiness` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qbusiness/type_defs/).
 
 ```python
-from mypy_boto3_qbusiness.type_defs import ActionExecutionPayloadFieldPaginatorTypeDef
+from mypy_boto3_qbusiness.type_defs import S3TypeDef
 
 
-def get_value() -> ActionExecutionPayloadFieldPaginatorTypeDef:
+def get_value() -> S3TypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy_boto3_qbusiness-1.34.86/mypy_boto3_qbusiness.egg-info/SOURCES.txt` & `mypy_boto3_qbusiness-1.34.95/mypy_boto3_qbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_qbusiness-1.34.86/setup.py` & `mypy_boto3_qbusiness-1.34.95/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qbusiness",
-    version="1.34.86",
+    version="1.34.95",
     packages=["mypy_boto3_qbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.QBusiness 1.34.86 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.QBusiness 1.34.95 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

