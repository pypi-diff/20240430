# Comparing `tmp/mypy_boto3_fms-1.34.92.tar.gz` & `tmp/mypy_boto3_fms-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_fms-1.34.92.tar", last modified: Thu Apr 25 19:32:14 2024, max compression
+gzip compressed data, was "mypy_boto3_fms-1.34.95.tar", last modified: Tue Apr 30 19:34:52 2024, max compression
```

## Comparing `mypy_boto3_fms-1.34.92.tar` & `mypy_boto3_fms-1.34.95.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.679407 mypy_boto3_fms-1.34.92/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-25 19:32:14.679407 mypy_boto3_fms-1.34.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.675407 mypy_boto3_fms-1.34.92/mypy_boto3_fms/
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30934 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30931 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    63196 2024-04-25 19:31:48.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    63196 2024-04-25 19:31:48.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.679407 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:14.679407 mypy_boto3_fms-1.34.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:52.115036 mypy_boto3_fms-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-30 19:34:52.115036 mypy_boto3_fms-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:52.115036 mypy_boto3_fms-1.34.95/mypy_boto3_fms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30934 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30931 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-30 19:32:07.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-30 19:32:07.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-30 19:32:07.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    63300 2024-04-30 19:32:08.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63300 2024-04-30 19:32:08.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:52.115036 mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-30 19:34:52.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-30 19:34:52.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:52.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:52.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:52.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 19:34:52.000000 mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:52.115036 mypy_boto3_fms-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-30 19:32:06.000000 mypy_boto3_fms-1.34.95/setup.py
```

### Comparing `mypy_boto3_fms-1.34.92/LICENSE` & `mypy_boto3_fms-1.34.95/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_fms-1.34.92/PKG-INFO` & `mypy_boto3_fms-1.34.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.34.92
-Summary: Type annotations for boto3.FMS 1.34.92 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.95
+Summary: Type annotations for boto3.FMS 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_fms-1.34.92/README.md` & `mypy_boto3_fms-1.34.95/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/__init__.py` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/__init__.pyi` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/__main__.py` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FMS 1.34.92\n"
-        "Version:         1.34.92\n"
+        "Type annotations for boto3.FMS 1.34.95\n"
+        "Version:         1.34.95\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.92")
+    print("1.34.95")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/client.py` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/client.pyi` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/literals.py` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     "NetworkFirewallOverrideActionType",
     "OrganizationStatusType",
     "PolicyComplianceStatusTypeType",
     "RemediationActionTypeType",
     "ResourceSetStatusType",
     "RuleOrderType",
     "SecurityServiceTypeType",
+    "StreamExceptionPolicyType",
     "TargetTypeType",
     "ThirdPartyFirewallAssociationStatusType",
     "ThirdPartyFirewallType",
     "ViolationReasonType",
     "FMSServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -104,14 +105,15 @@
     "SECURITY_GROUPS_CONTENT_AUDIT",
     "SECURITY_GROUPS_USAGE_AUDIT",
     "SHIELD_ADVANCED",
     "THIRD_PARTY_FIREWALL",
     "WAF",
     "WAFV2",
 ]
+StreamExceptionPolicyType = Literal["CONTINUE", "DROP", "FMS_IGNORE", "REJECT"]
 TargetTypeType = Literal[
     "CARRIER_GATEWAY",
     "EGRESS_ONLY_INTERNET_GATEWAY",
     "GATEWAY",
     "INSTANCE",
     "LOCAL_GATEWAY",
     "NAT_GATEWAY",
```

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/literals.pyi` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     "NetworkFirewallOverrideActionType",
     "OrganizationStatusType",
     "PolicyComplianceStatusTypeType",
     "RemediationActionTypeType",
     "ResourceSetStatusType",
     "RuleOrderType",
     "SecurityServiceTypeType",
+    "StreamExceptionPolicyType",
     "TargetTypeType",
     "ThirdPartyFirewallAssociationStatusType",
     "ThirdPartyFirewallType",
     "ViolationReasonType",
     "FMSServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -104,14 +105,15 @@
     "SECURITY_GROUPS_CONTENT_AUDIT",
     "SECURITY_GROUPS_USAGE_AUDIT",
     "SHIELD_ADVANCED",
     "THIRD_PARTY_FIREWALL",
     "WAF",
     "WAFV2",
 ]
+StreamExceptionPolicyType = Literal["CONTINUE", "DROP", "FMS_IGNORE", "REJECT"]
 TargetTypeType = Literal[
     "CARRIER_GATEWAY",
     "EGRESS_ONLY_INTERNET_GATEWAY",
     "GATEWAY",
     "INSTANCE",
     "LOCAL_GATEWAY",
     "NAT_GATEWAY",
```

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/paginator.py` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/paginator.pyi` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/type_defs.py` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     NetworkAclRuleActionType,
     OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
     ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
+    StreamExceptionPolicyType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
     ThirdPartyFirewallType,
     ViolationReasonType,
 )
 
 if sys.version_info >= (3, 12):
@@ -783,14 +784,15 @@
         "TargetViolationReason": NotRequired[str],
     },
 )
 StatefulEngineOptionsTypeDef = TypedDict(
     "StatefulEngineOptionsTypeDef",
     {
         "RuleOrder": NotRequired[RuleOrderType],
+        "StreamExceptionPolicy": NotRequired[StreamExceptionPolicyType],
     },
 )
 StatelessRuleGroupTypeDef = TypedDict(
     "StatelessRuleGroupTypeDef",
     {
         "RuleGroupName": NotRequired[str],
         "ResourceId": NotRequired[str],
```

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms/type_defs.pyi` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     NetworkAclRuleActionType,
     OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
     ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
+    StreamExceptionPolicyType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
     ThirdPartyFirewallType,
     ViolationReasonType,
 )
 
 if sys.version_info >= (3, 12):
@@ -783,14 +784,15 @@
         "TargetViolationReason": NotRequired[str],
     },
 )
 StatefulEngineOptionsTypeDef = TypedDict(
     "StatefulEngineOptionsTypeDef",
     {
         "RuleOrder": NotRequired[RuleOrderType],
+        "StreamExceptionPolicy": NotRequired[StreamExceptionPolicyType],
     },
 )
 StatelessRuleGroupTypeDef = TypedDict(
     "StatelessRuleGroupTypeDef",
     {
         "RuleGroupName": NotRequired[str],
         "ResourceId": NotRequired[str],
```

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/PKG-INFO` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.34.92
-Summary: Type annotations for boto3.FMS 1.34.92 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.95
+Summary: Type annotations for boto3.FMS 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/SOURCES.txt` & `mypy_boto3_fms-1.34.95/mypy_boto3_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_fms-1.34.92/setup.py` & `mypy_boto3_fms-1.34.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fms",
-    version="1.34.92",
+    version="1.34.95",
     packages=["mypy_boto3_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.FMS 1.34.92 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.FMS 1.34.95 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

