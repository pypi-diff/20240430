# Comparing `tmp/mypy_boto3_sagemaker-1.34.89.tar.gz` & `tmp/mypy_boto3_sagemaker-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_sagemaker-1.34.89.tar", last modified: Mon Apr 22 19:19:13 2024, max compression
+gzip compressed data, was "mypy_boto3_sagemaker-1.34.95.tar", last modified: Tue Apr 30 19:34:54 2024, max compression
```

## Comparing `mypy_boto3_sagemaker-1.34.89.tar` & `mypy_boto3_sagemaker-1.34.95.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:13.339681 mypy_boto3_sagemaker-1.34.89/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 19:18:43.000000 mypy_boto3_sagemaker-1.34.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25764 2024-04-22 19:19:13.339681 mypy_boto3_sagemaker-1.34.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24201 2024-04-22 19:18:43.000000 mypy_boto3_sagemaker-1.34.89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:13.339681 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-04-22 19:18:43.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-04-22 19:18:43.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-22 19:18:43.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   278115 2024-04-22 19:18:46.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   278112 2024-04-22 19:18:44.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    66823 2024-04-22 19:18:48.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    66823 2024-04-22 19:18:48.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   102894 2024-04-22 19:18:47.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)   102821 2024-04-22 19:18:47.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:18:43.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   503564 2024-04-22 19:18:57.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   503564 2024-04-22 19:18:54.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 19:18:43.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-22 19:18:47.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-04-22 19:18:47.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:13.339681 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25764 2024-04-22 19:19:13.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-22 19:19:13.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:13.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:13.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 19:19:13.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 19:19:13.000000 mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:19:13.339681 mypy_boto3_sagemaker-1.34.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-22 19:18:43.000000 mypy_boto3_sagemaker-1.34.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25764 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24201 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278981 2024-04-30 19:34:24.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278978 2024-04-30 19:34:23.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    66994 2024-04-30 19:34:26.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66994 2024-04-30 19:34:26.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   102768 2024-04-30 19:34:25.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102695 2024-04-30 19:34:24.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   543580 2024-04-30 19:34:37.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   543580 2024-04-30 19:34:33.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-30 19:34:25.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-04-30 19:34:25.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25764 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 19:34:54.000000 mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:54.659064 mypy_boto3_sagemaker-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-30 19:34:20.000000 mypy_boto3_sagemaker-1.34.95/setup.py
```

### Comparing `mypy_boto3_sagemaker-1.34.89/LICENSE` & `mypy_boto3_sagemaker-1.34.95/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.89/PKG-INFO` & `mypy_boto3_sagemaker-1.34.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.34.89
-Summary: Type annotations for boto3.SageMaker 1.34.89 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.95
+Summary: Type annotations for boto3.SageMaker 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker)](https://pepy.tech/project/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_sagemaker-1.34.89/README.md` & `mypy_boto3_sagemaker-1.34.95/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker)](https://pepy.tech/project/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/__init__.py` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/__init__.pyi` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/__main__.py` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMaker 1.34.89\n"
-        "Version:         1.34.89\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.SageMaker 1.34.95\n"
+        "Version:         1.34.95\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.89")
+    print("1.34.95")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/client.py` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -206,39 +206,39 @@
     ListWorkforcesPaginator,
     ListWorkteamsPaginator,
     SearchPaginator,
 )
 from .type_defs import (
     ActionSourceTypeDef,
     AddAssociationResponseTypeDef,
-    AdditionalInferenceSpecificationDefinitionTypeDef,
+    AdditionalInferenceSpecificationDefinitionUnionTypeDef,
     AddTagsOutputTypeDef,
-    AlgorithmSpecificationTypeDef,
-    AlgorithmValidationSpecificationTypeDef,
-    AppSpecificationTypeDef,
-    ArtifactSourceTypeDef,
+    AlgorithmSpecificationUnionTypeDef,
+    AlgorithmValidationSpecificationUnionTypeDef,
+    AppSpecificationUnionTypeDef,
+    ArtifactSourceUnionTypeDef,
     AssociateTrialComponentResponseTypeDef,
-    AsyncInferenceConfigTypeDef,
+    AsyncInferenceConfigUnionTypeDef,
     AutoMLChannelTypeDef,
     AutoMLDataSplitConfigTypeDef,
     AutoMLJobChannelTypeDef,
-    AutoMLJobConfigTypeDef,
+    AutoMLJobConfigUnionTypeDef,
     AutoMLJobObjectiveTypeDef,
     AutoMLOutputDataConfigTypeDef,
-    AutoMLProblemTypeConfigTypeDef,
-    AutoMLSecurityConfigTypeDef,
+    AutoMLProblemTypeConfigUnionTypeDef,
+    AutoMLSecurityConfigUnionTypeDef,
     AutotuneTypeDef,
     BatchDataCaptureConfigTypeDef,
     BatchDescribeModelPackageOutputTypeDef,
-    ChannelTypeDef,
+    ChannelUnionTypeDef,
     CheckpointConfigTypeDef,
     ClusterInstanceGroupSpecificationTypeDef,
-    CodeEditorAppImageConfigTypeDef,
+    CodeEditorAppImageConfigUnionTypeDef,
     CognitoConfigTypeDef,
-    ContainerDefinitionTypeDef,
+    ContainerDefinitionUnionTypeDef,
     ContextSourceTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
@@ -285,34 +285,34 @@
     CreateTrainingJobResponseTypeDef,
     CreateTransformJobResponseTypeDef,
     CreateTrialComponentResponseTypeDef,
     CreateTrialResponseTypeDef,
     CreateUserProfileResponseTypeDef,
     CreateWorkforceResponseTypeDef,
     CreateWorkteamResponseTypeDef,
-    DataCaptureConfigTypeDef,
+    DataCaptureConfigUnionTypeDef,
     DataProcessingTypeDef,
-    DataQualityAppSpecificationTypeDef,
+    DataQualityAppSpecificationUnionTypeDef,
     DataQualityBaselineConfigTypeDef,
-    DataQualityJobInputTypeDef,
-    DebugHookConfigTypeDef,
-    DebugRuleConfigurationTypeDef,
-    DefaultSpaceSettingsTypeDef,
+    DataQualityJobInputUnionTypeDef,
+    DebugHookConfigUnionTypeDef,
+    DebugRuleConfigurationUnionTypeDef,
+    DefaultSpaceSettingsUnionTypeDef,
     DeleteActionResponseTypeDef,
     DeleteArtifactResponseTypeDef,
     DeleteAssociationResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteContextResponseTypeDef,
     DeleteExperimentResponseTypeDef,
     DeleteInferenceExperimentResponseTypeDef,
     DeletePipelineResponseTypeDef,
     DeleteTrialComponentResponseTypeDef,
     DeleteTrialResponseTypeDef,
     DeleteWorkteamResponseTypeDef,
-    DeploymentConfigTypeDef,
+    DeploymentConfigUnionTypeDef,
     DeploymentStageTypeDef,
     DescribeActionResponseTypeDef,
     DescribeAlgorithmOutputTypeDef,
     DescribeAppImageConfigResponseTypeDef,
     DescribeAppResponseTypeDef,
     DescribeArtifactResponseTypeDef,
     DescribeAutoMLJobResponseTypeDef,
@@ -371,54 +371,54 @@
     DescribeUserProfileResponseTypeDef,
     DescribeWorkforceResponseTypeDef,
     DescribeWorkteamResponseTypeDef,
     DesiredWeightAndCapacityTypeDef,
     DeviceTypeDef,
     DisassociateTrialComponentResponseTypeDef,
     DomainSettingsForUpdateTypeDef,
-    DomainSettingsTypeDef,
+    DomainSettingsUnionTypeDef,
     DriftCheckBaselinesTypeDef,
     EdgeDeploymentModelConfigTypeDef,
     EdgeOutputConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     ExperimentConfigTypeDef,
-    ExplainerConfigTypeDef,
+    ExplainerConfigUnionTypeDef,
     FeatureDefinitionTypeDef,
     FeatureParameterTypeDef,
     FlowDefinitionOutputConfigTypeDef,
     GetDeviceFleetReportResponseTypeDef,
     GetLineageGroupPolicyResponseTypeDef,
     GetModelPackageGroupPolicyOutputTypeDef,
     GetSagemakerServicecatalogPortfolioStatusOutputTypeDef,
     GetScalingConfigurationRecommendationResponseTypeDef,
     GetSearchSuggestionsResponseTypeDef,
     GitConfigForUpdateTypeDef,
     GitConfigTypeDef,
     HubS3StorageConfigTypeDef,
     HumanLoopActivationConfigTypeDef,
-    HumanLoopConfigTypeDef,
+    HumanLoopConfigUnionTypeDef,
     HumanLoopRequestSourceTypeDef,
-    HumanTaskConfigTypeDef,
-    HyperParameterTrainingJobDefinitionTypeDef,
-    HyperParameterTuningJobConfigTypeDef,
-    HyperParameterTuningJobWarmStartConfigTypeDef,
+    HumanTaskConfigUnionTypeDef,
+    HyperParameterTrainingJobDefinitionUnionTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
+    HyperParameterTuningJobWarmStartConfigUnionTypeDef,
     ImportHubContentResponseTypeDef,
     InferenceComponentRuntimeConfigTypeDef,
     InferenceComponentSpecificationTypeDef,
     InferenceExecutionConfigTypeDef,
-    InferenceExperimentDataStorageConfigTypeDef,
-    InferenceExperimentScheduleTypeDef,
-    InferenceSpecificationTypeDef,
+    InferenceExperimentDataStorageConfigUnionTypeDef,
+    InferenceExperimentScheduleUnionTypeDef,
+    InferenceSpecificationUnionTypeDef,
     InfraCheckConfigTypeDef,
     InputConfigTypeDef,
     InstanceMetadataServiceConfigurationTypeDef,
-    JupyterLabAppImageConfigTypeDef,
-    KernelGatewayImageConfigTypeDef,
-    LabelingJobAlgorithmsConfigTypeDef,
-    LabelingJobInputConfigTypeDef,
+    JupyterLabAppImageConfigUnionTypeDef,
+    KernelGatewayImageConfigUnionTypeDef,
+    LabelingJobAlgorithmsConfigUnionTypeDef,
+    LabelingJobInputConfigUnionTypeDef,
     LabelingJobOutputConfigTypeDef,
     LabelingJobStoppingConditionsTypeDef,
     ListActionsResponseTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAliasesResponseTypeDef,
     ListAppImageConfigsResponseTypeDef,
     ListAppsResponseTypeDef,
@@ -488,102 +488,103 @@
     ListTrainingJobsResponseTypeDef,
     ListTransformJobsResponseTypeDef,
     ListTrialComponentsResponseTypeDef,
     ListTrialsResponseTypeDef,
     ListUserProfilesResponseTypeDef,
     ListWorkforcesResponseTypeDef,
     ListWorkteamsResponseTypeDef,
-    MemberDefinitionTypeDef,
+    MemberDefinitionUnionTypeDef,
     MetadataPropertiesTypeDef,
-    ModelBiasAppSpecificationTypeDef,
+    ModelBiasAppSpecificationUnionTypeDef,
     ModelBiasBaselineConfigTypeDef,
-    ModelBiasJobInputTypeDef,
+    ModelBiasJobInputUnionTypeDef,
     ModelCardExportOutputConfigTypeDef,
     ModelCardSecurityConfigTypeDef,
     ModelClientConfigTypeDef,
     ModelDeployConfigTypeDef,
-    ModelExplainabilityAppSpecificationTypeDef,
+    ModelExplainabilityAppSpecificationUnionTypeDef,
     ModelExplainabilityBaselineConfigTypeDef,
-    ModelExplainabilityJobInputTypeDef,
+    ModelExplainabilityJobInputUnionTypeDef,
     ModelMetadataSearchExpressionTypeDef,
     ModelMetricsTypeDef,
-    ModelPackageValidationSpecificationTypeDef,
-    ModelQualityAppSpecificationTypeDef,
+    ModelPackageValidationSpecificationUnionTypeDef,
+    ModelQualityAppSpecificationUnionTypeDef,
     ModelQualityBaselineConfigTypeDef,
-    ModelQualityJobInputTypeDef,
+    ModelQualityJobInputUnionTypeDef,
     ModelVariantConfigTypeDef,
-    MonitoringNetworkConfigTypeDef,
-    MonitoringOutputConfigTypeDef,
+    MonitoringNetworkConfigUnionTypeDef,
+    MonitoringOutputConfigUnionTypeDef,
     MonitoringResourcesTypeDef,
-    MonitoringScheduleConfigTypeDef,
+    MonitoringScheduleConfigUnionTypeDef,
     MonitoringStoppingConditionTypeDef,
-    NeoVpcConfigTypeDef,
-    NetworkConfigTypeDef,
+    NeoVpcConfigUnionTypeDef,
+    NetworkConfigUnionTypeDef,
     NotebookInstanceLifecycleHookTypeDef,
     NotificationConfigurationTypeDef,
     OfflineStoreConfigTypeDef,
     OidcConfigTypeDef,
     OnlineStoreConfigTypeDef,
     OnlineStoreConfigUpdateTypeDef,
     OutputConfigTypeDef,
     OutputDataConfigTypeDef,
     OutputParameterTypeDef,
     OwnershipSettingsTypeDef,
     ParallelismConfigurationTypeDef,
     ParameterTypeDef,
     PipelineDefinitionS3LocationTypeDef,
     ProcessingInputTypeDef,
-    ProcessingOutputConfigTypeDef,
+    ProcessingOutputConfigUnionTypeDef,
     ProcessingResourcesTypeDef,
     ProcessingStoppingConditionTypeDef,
     ProductionVariantTypeDef,
     ProfilerConfigForUpdateTypeDef,
-    ProfilerConfigTypeDef,
-    ProfilerRuleConfigurationTypeDef,
+    ProfilerConfigUnionTypeDef,
+    ProfilerRuleConfigurationUnionTypeDef,
     PutModelPackageGroupPolicyOutputTypeDef,
     QueryFiltersTypeDef,
     QueryLineageResponseTypeDef,
-    RecommendationJobInputConfigTypeDef,
+    RecommendationJobInputConfigUnionTypeDef,
     RecommendationJobOutputConfigTypeDef,
-    RecommendationJobStoppingConditionsTypeDef,
+    RecommendationJobStoppingConditionsUnionTypeDef,
     RemoteDebugConfigForUpdateTypeDef,
     RemoteDebugConfigTypeDef,
     RenderableTaskTypeDef,
     RenderUiTemplateResponseTypeDef,
     ResourceConfigForUpdateTypeDef,
-    ResourceConfigTypeDef,
+    ResourceConfigUnionTypeDef,
     ResourceSpecTypeDef,
     RetentionPolicyTypeDef,
     RetryPipelineExecutionResponseTypeDef,
     RetryStrategyTypeDef,
     ScalingPolicyObjectiveTypeDef,
     SearchExpressionTypeDef,
     SearchResponseTypeDef,
-    SelectiveExecutionConfigTypeDef,
+    SelectiveExecutionConfigUnionTypeDef,
     SendPipelineExecutionStepFailureResponseTypeDef,
     SendPipelineExecutionStepSuccessResponseTypeDef,
-    ServiceCatalogProvisioningDetailsTypeDef,
+    ServiceCatalogProvisioningDetailsUnionTypeDef,
     ServiceCatalogProvisioningUpdateDetailsTypeDef,
-    ShadowModeConfigTypeDef,
-    SourceAlgorithmSpecificationTypeDef,
-    SourceIpConfigTypeDef,
-    SpaceSettingsTypeDef,
+    SessionChainingConfigTypeDef,
+    ShadowModeConfigUnionTypeDef,
+    SourceAlgorithmSpecificationUnionTypeDef,
+    SourceIpConfigUnionTypeDef,
+    SpaceSettingsUnionTypeDef,
     SpaceSharingSettingsTypeDef,
     StartInferenceExperimentResponseTypeDef,
     StartPipelineExecutionResponseTypeDef,
     StopInferenceExperimentResponseTypeDef,
     StoppingConditionTypeDef,
     StopPipelineExecutionResponseTypeDef,
     SuggestionQueryTypeDef,
     TagTypeDef,
     TensorBoardOutputConfigTypeDef,
     ThroughputConfigTypeDef,
     ThroughputConfigUpdateTypeDef,
     TimestampTypeDef,
-    TrainingSpecificationTypeDef,
+    TrainingSpecificationUnionTypeDef,
     TransformInputTypeDef,
     TransformOutputTypeDef,
     TransformResourcesTypeDef,
     TrialComponentArtifactTypeDef,
     TrialComponentParameterValueTypeDef,
     TrialComponentStatusTypeDef,
     UiTemplateTypeDef,
@@ -615,18 +616,18 @@
     UpdateSpaceResponseTypeDef,
     UpdateTrainingJobResponseTypeDef,
     UpdateTrialComponentResponseTypeDef,
     UpdateTrialResponseTypeDef,
     UpdateUserProfileResponseTypeDef,
     UpdateWorkforceResponseTypeDef,
     UpdateWorkteamResponseTypeDef,
-    UserSettingsTypeDef,
+    UserSettingsUnionTypeDef,
     VariantPropertyTypeDef,
     VisibilityConditionsTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
     WorkforceVpcConfigRequestTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     EndpointInServiceWaiter,
     ImageCreatedWaiter,
     ImageDeletedWaiter,
@@ -644,31 +645,28 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("SageMakerClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ResourceInUse: Type[BotocoreClientError]
     ResourceLimitExceeded: Type[BotocoreClientError]
     ResourceNotFound: Type[BotocoreClientError]
 
-
 class SageMakerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/)
     """
 
     meta: ClientMeta
@@ -757,18 +755,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_action)
         """
 
     def create_algorithm(
         self,
         *,
         AlgorithmName: str,
-        TrainingSpecification: TrainingSpecificationTypeDef,
+        TrainingSpecification: TrainingSpecificationUnionTypeDef,
         AlgorithmDescription: str = ...,
-        InferenceSpecification: InferenceSpecificationTypeDef = ...,
-        ValidationSpecification: AlgorithmValidationSpecificationTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
+        ValidationSpecification: AlgorithmValidationSpecificationUnionTypeDef = ...,
         CertifyForMarketplace: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAlgorithmOutputTypeDef:
         """
         Create a machine learning algorithm that you can use in SageMaker and list in
         the Amazon Web Services
         Marketplace.
@@ -796,29 +794,29 @@
         """
 
     def create_app_image_config(
         self,
         *,
         AppImageConfigName: str,
         Tags: Sequence[TagTypeDef] = ...,
-        KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...,
-        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...,
-        CodeEditorAppImageConfig: CodeEditorAppImageConfigTypeDef = ...,
+        KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...,
+        JupyterLabAppImageConfig: JupyterLabAppImageConfigUnionTypeDef = ...,
+        CodeEditorAppImageConfig: CodeEditorAppImageConfigUnionTypeDef = ...,
     ) -> CreateAppImageConfigResponseTypeDef:
         """
         Creates a configuration for running a SageMaker image as a KernelGateway app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app_image_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_app_image_config)
         """
 
     def create_artifact(
         self,
         *,
-        Source: ArtifactSourceTypeDef,
+        Source: ArtifactSourceUnionTypeDef,
         ArtifactType: str,
         ArtifactName: str = ...,
         Properties: Mapping[str, str] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateArtifactResponseTypeDef:
         """
@@ -833,15 +831,15 @@
         *,
         AutoMLJobName: str,
         InputDataConfig: Sequence[AutoMLChannelTypeDef],
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
         RoleArn: str,
         ProblemType: ProblemTypeType = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
-        AutoMLJobConfig: AutoMLJobConfigTypeDef = ...,
+        AutoMLJobConfig: AutoMLJobConfigUnionTypeDef = ...,
         GenerateCandidateDefinitionsOnly: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...,
     ) -> CreateAutoMLJobResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job.
 
@@ -851,18 +849,18 @@
 
     def create_auto_ml_job_v2(
         self,
         *,
         AutoMLJobName: str,
         AutoMLJobInputDataConfig: Sequence[AutoMLJobChannelTypeDef],
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
-        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,
+        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigUnionTypeDef,
         RoleArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        SecurityConfig: AutoMLSecurityConfigTypeDef = ...,
+        SecurityConfig: AutoMLSecurityConfigUnionTypeDef = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...,
         DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...,
     ) -> CreateAutoMLJobV2ResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job
         V2.
@@ -872,15 +870,15 @@
         """
 
     def create_cluster(
         self,
         *,
         ClusterName: str,
         InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef],
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a SageMaker HyperPod cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_cluster)
@@ -905,15 +903,15 @@
         *,
         CompilationJobName: str,
         RoleArn: str,
         OutputConfig: OutputConfigTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         ModelPackageVersionArn: str = ...,
         InputConfig: InputConfigTypeDef = ...,
-        VpcConfig: NeoVpcConfigTypeDef = ...,
+        VpcConfig: NeoVpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCompilationJobResponseTypeDef:
         """
         Starts a model compilation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_compilation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_compilation_job)
@@ -936,21 +934,21 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_context)
         """
 
     def create_data_quality_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        DataQualityAppSpecification: DataQualityAppSpecificationTypeDef,
-        DataQualityJobInput: DataQualityJobInputTypeDef,
-        DataQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
+        DataQualityAppSpecification: DataQualityAppSpecificationUnionTypeDef,
+        DataQualityJobInput: DataQualityJobInputUnionTypeDef,
+        DataQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         DataQualityBaselineConfig: DataQualityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors data quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_data_quality_job_definition)
@@ -975,24 +973,24 @@
         """
 
     def create_domain(
         self,
         *,
         DomainName: str,
         AuthMode: AuthModeType,
-        DefaultUserSettings: UserSettingsTypeDef,
+        DefaultUserSettings: UserSettingsUnionTypeDef,
         SubnetIds: Sequence[str],
         VpcId: str,
-        DomainSettings: DomainSettingsTypeDef = ...,
+        DomainSettings: DomainSettingsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AppNetworkAccessType: AppNetworkAccessTypeType = ...,
         HomeEfsFileSystemKmsKeyId: str = ...,
         KmsKeyId: str = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
+        DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a `Domain`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_domain)
         """
@@ -1043,37 +1041,37 @@
         """
 
     def create_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
-        DeploymentConfig: DeploymentConfigTypeDef = ...,
+        DeploymentConfig: DeploymentConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEndpointOutputTypeDef:
         """
         Creates an endpoint using the endpoint configuration specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_endpoint)
         """
 
     def create_endpoint_config(
         self,
         *,
         EndpointConfigName: str,
         ProductionVariants: Sequence[ProductionVariantTypeDef],
-        DataCaptureConfig: DataCaptureConfigTypeDef = ...,
+        DataCaptureConfig: DataCaptureConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
-        AsyncInferenceConfig: AsyncInferenceConfigTypeDef = ...,
-        ExplainerConfig: ExplainerConfigTypeDef = ...,
+        AsyncInferenceConfig: AsyncInferenceConfigUnionTypeDef = ...,
+        ExplainerConfig: ExplainerConfigUnionTypeDef = ...,
         ShadowProductionVariants: Sequence[ProductionVariantTypeDef] = ...,
         ExecutionRoleArn: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         EnableNetworkIsolation: bool = ...,
     ) -> CreateEndpointConfigOutputTypeDef:
         """
         Creates an endpoint configuration that SageMaker hosting services uses to
         deploy
         models.
 
@@ -1121,15 +1119,15 @@
         self,
         *,
         FlowDefinitionName: str,
         OutputConfig: FlowDefinitionOutputConfigTypeDef,
         RoleArn: str,
         HumanLoopRequestSource: HumanLoopRequestSourceTypeDef = ...,
         HumanLoopActivationConfig: HumanLoopActivationConfigTypeDef = ...,
-        HumanLoopConfig: HumanLoopConfigTypeDef = ...,
+        HumanLoopConfig: HumanLoopConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFlowDefinitionResponseTypeDef:
         """
         Creates a flow definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_flow_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_flow_definition)
@@ -1166,18 +1164,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_human_task_ui)
         """
 
     def create_hyper_parameter_tuning_job(
         self,
         *,
         HyperParameterTuningJobName: str,
-        HyperParameterTuningJobConfig: HyperParameterTuningJobConfigTypeDef,
-        TrainingJobDefinition: HyperParameterTrainingJobDefinitionTypeDef = ...,
-        TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionTypeDef] = ...,
-        WarmStartConfig: HyperParameterTuningJobWarmStartConfigTypeDef = ...,
+        HyperParameterTuningJobConfig: HyperParameterTuningJobConfigUnionTypeDef,
+        TrainingJobDefinition: HyperParameterTrainingJobDefinitionUnionTypeDef = ...,
+        TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef] = ...,
+        WarmStartConfig: HyperParameterTuningJobWarmStartConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Autotune: AutotuneTypeDef = ...,
     ) -> CreateHyperParameterTuningJobResponseTypeDef:
         """
         Starts a hyperparameter tuning job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hyper_parameter_tuning_job)
@@ -1245,18 +1243,18 @@
         self,
         *,
         Name: str,
         Type: Literal["ShadowMode"],
         RoleArn: str,
         EndpointName: str,
         ModelVariants: Sequence[ModelVariantConfigTypeDef],
-        ShadowModeConfig: ShadowModeConfigTypeDef,
-        Schedule: InferenceExperimentScheduleTypeDef = ...,
+        ShadowModeConfig: ShadowModeConfigUnionTypeDef,
+        Schedule: InferenceExperimentScheduleUnionTypeDef = ...,
         Description: str = ...,
-        DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
+        DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,
         KmsKey: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceExperimentResponseTypeDef:
         """
         Creates an inference experiment using the configurations specified in the
         request.
 
@@ -1266,17 +1264,17 @@
 
     def create_inference_recommendations_job(
         self,
         *,
         JobName: str,
         JobType: RecommendationJobTypeType,
         RoleArn: str,
-        InputConfig: RecommendationJobInputConfigTypeDef,
+        InputConfig: RecommendationJobInputConfigUnionTypeDef,
         JobDescription: str = ...,
-        StoppingConditions: RecommendationJobStoppingConditionsTypeDef = ...,
+        StoppingConditions: RecommendationJobStoppingConditionsUnionTypeDef = ...,
         OutputConfig: RecommendationJobOutputConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceRecommendationsJobResponseTypeDef:
         """
         Starts a recommendation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_recommendations_job)
@@ -1284,60 +1282,60 @@
         """
 
     def create_labeling_job(
         self,
         *,
         LabelingJobName: str,
         LabelAttributeName: str,
-        InputConfig: LabelingJobInputConfigTypeDef,
+        InputConfig: LabelingJobInputConfigUnionTypeDef,
         OutputConfig: LabelingJobOutputConfigTypeDef,
         RoleArn: str,
-        HumanTaskConfig: HumanTaskConfigTypeDef,
+        HumanTaskConfig: HumanTaskConfigUnionTypeDef,
         LabelCategoryConfigS3Uri: str = ...,
         StoppingConditions: LabelingJobStoppingConditionsTypeDef = ...,
-        LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigTypeDef = ...,
+        LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLabelingJobResponseTypeDef:
         """
         Creates a job that uses workers to label the data objects in your input dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_labeling_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_labeling_job)
         """
 
     def create_model(
         self,
         *,
         ModelName: str,
-        PrimaryContainer: ContainerDefinitionTypeDef = ...,
-        Containers: Sequence[ContainerDefinitionTypeDef] = ...,
+        PrimaryContainer: ContainerDefinitionUnionTypeDef = ...,
+        Containers: Sequence[ContainerDefinitionUnionTypeDef] = ...,
         InferenceExecutionConfig: InferenceExecutionConfigTypeDef = ...,
         ExecutionRoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         EnableNetworkIsolation: bool = ...,
     ) -> CreateModelOutputTypeDef:
         """
         Creates a model in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_model)
         """
 
     def create_model_bias_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelBiasAppSpecification: ModelBiasAppSpecificationTypeDef,
-        ModelBiasJobInput: ModelBiasJobInputTypeDef,
-        ModelBiasJobOutputConfig: MonitoringOutputConfigTypeDef,
+        ModelBiasAppSpecification: ModelBiasAppSpecificationUnionTypeDef,
+        ModelBiasJobInput: ModelBiasJobInputUnionTypeDef,
+        ModelBiasJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelBiasBaselineConfig: ModelBiasBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelBiasJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model bias job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_bias_job_definition)
@@ -1375,21 +1373,21 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_model_card_export_job)
         """
 
     def create_model_explainability_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationTypeDef,
-        ModelExplainabilityJobInput: ModelExplainabilityJobInputTypeDef,
-        ModelExplainabilityJobOutputConfig: MonitoringOutputConfigTypeDef,
+        ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationUnionTypeDef,
+        ModelExplainabilityJobInput: ModelExplainabilityJobInputUnionTypeDef,
+        ModelExplainabilityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelExplainabilityBaselineConfig: ModelExplainabilityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelExplainabilityJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model explainability job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_explainability_job_definition)
@@ -1398,30 +1396,30 @@
 
     def create_model_package(
         self,
         *,
         ModelPackageName: str = ...,
         ModelPackageGroupName: str = ...,
         ModelPackageDescription: str = ...,
-        InferenceSpecification: InferenceSpecificationTypeDef = ...,
-        ValidationSpecification: ModelPackageValidationSpecificationTypeDef = ...,
-        SourceAlgorithmSpecification: SourceAlgorithmSpecificationTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
+        ValidationSpecification: ModelPackageValidationSpecificationUnionTypeDef = ...,
+        SourceAlgorithmSpecification: SourceAlgorithmSpecificationUnionTypeDef = ...,
         CertifyForMarketplace: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         ModelMetrics: ModelMetricsTypeDef = ...,
         ClientToken: str = ...,
         Domain: str = ...,
         Task: str = ...,
         SamplePayloadUrl: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         DriftCheckBaselines: DriftCheckBaselinesTypeDef = ...,
         AdditionalInferenceSpecifications: Sequence[
-            AdditionalInferenceSpecificationDefinitionTypeDef
+            AdditionalInferenceSpecificationDefinitionUnionTypeDef
         ] = ...,
         SkipModelValidation: SkipModelValidationType = ...,
         SourceUri: str = ...,
     ) -> CreateModelPackageOutputTypeDef:
         """
         Creates a model package that you can use to create SageMaker models or list on
         Amazon Web Services Marketplace, or a versioned model that is part of a model
@@ -1445,36 +1443,36 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_model_package_group)
         """
 
     def create_model_quality_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelQualityAppSpecification: ModelQualityAppSpecificationTypeDef,
-        ModelQualityJobInput: ModelQualityJobInputTypeDef,
-        ModelQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
+        ModelQualityAppSpecification: ModelQualityAppSpecificationUnionTypeDef,
+        ModelQualityJobInput: ModelQualityJobInputUnionTypeDef,
+        ModelQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelQualityBaselineConfig: ModelQualityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors model quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_quality_job_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_model_quality_job_definition)
         """
 
     def create_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
+        MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMonitoringScheduleResponseTypeDef:
         """
         Creates a schedule that regularly starts Amazon SageMaker Processing Jobs to
         monitor the data captured for an Amazon SageMaker
         Endpoint.
 
@@ -1573,36 +1571,36 @@
         """
 
     def create_processing_job(
         self,
         *,
         ProcessingJobName: str,
         ProcessingResources: ProcessingResourcesTypeDef,
-        AppSpecification: AppSpecificationTypeDef,
+        AppSpecification: AppSpecificationUnionTypeDef,
         RoleArn: str,
         ProcessingInputs: Sequence[ProcessingInputTypeDef] = ...,
-        ProcessingOutputConfig: ProcessingOutputConfigTypeDef = ...,
+        ProcessingOutputConfig: ProcessingOutputConfigUnionTypeDef = ...,
         StoppingCondition: ProcessingStoppingConditionTypeDef = ...,
         Environment: Mapping[str, str] = ...,
-        NetworkConfig: NetworkConfigTypeDef = ...,
+        NetworkConfig: NetworkConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...,
     ) -> CreateProcessingJobResponseTypeDef:
         """
         Creates a processing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_processing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_processing_job)
         """
 
     def create_project(
         self,
         *,
         ProjectName: str,
-        ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsTypeDef,
+        ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsUnionTypeDef,
         ProjectDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a machine learning (ML) project that can contain one or more templates
         that set up an ML pipeline from training to deploying an approved
         model.
@@ -1613,15 +1611,15 @@
 
     def create_space(
         self,
         *,
         DomainId: str,
         SpaceName: str,
         Tags: Sequence[TagTypeDef] = ...,
-        SpaceSettings: SpaceSettingsTypeDef = ...,
+        SpaceSettings: SpaceSettingsUnionTypeDef = ...,
         OwnershipSettings: OwnershipSettingsTypeDef = ...,
         SpaceSharingSettings: SpaceSharingSettingsTypeDef = ...,
         SpaceDisplayName: str = ...,
     ) -> CreateSpaceResponseTypeDef:
         """
         Creates a space used for real time collaboration in a domain.
 
@@ -1644,37 +1642,38 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_studio_lifecycle_config)
         """
 
     def create_training_job(
         self,
         *,
         TrainingJobName: str,
-        AlgorithmSpecification: AlgorithmSpecificationTypeDef,
+        AlgorithmSpecification: AlgorithmSpecificationUnionTypeDef,
         RoleArn: str,
         OutputDataConfig: OutputDataConfigTypeDef,
-        ResourceConfig: ResourceConfigTypeDef,
+        ResourceConfig: ResourceConfigUnionTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         HyperParameters: Mapping[str, str] = ...,
-        InputDataConfig: Sequence[ChannelTypeDef] = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        InputDataConfig: Sequence[ChannelUnionTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EnableNetworkIsolation: bool = ...,
         EnableInterContainerTrafficEncryption: bool = ...,
         EnableManagedSpotTraining: bool = ...,
         CheckpointConfig: CheckpointConfigTypeDef = ...,
-        DebugHookConfig: DebugHookConfigTypeDef = ...,
-        DebugRuleConfigurations: Sequence[DebugRuleConfigurationTypeDef] = ...,
+        DebugHookConfig: DebugHookConfigUnionTypeDef = ...,
+        DebugRuleConfigurations: Sequence[DebugRuleConfigurationUnionTypeDef] = ...,
         TensorBoardOutputConfig: TensorBoardOutputConfigTypeDef = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...,
-        ProfilerConfig: ProfilerConfigTypeDef = ...,
-        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
+        ProfilerConfig: ProfilerConfigUnionTypeDef = ...,
+        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,
         Environment: Mapping[str, str] = ...,
         RetryStrategy: RetryStrategyTypeDef = ...,
         RemoteDebugConfig: RemoteDebugConfigTypeDef = ...,
         InfraCheckConfig: InfraCheckConfigTypeDef = ...,
+        SessionChainingConfig: SessionChainingConfigTypeDef = ...,
     ) -> CreateTrainingJobResponseTypeDef:
         """
         Starts a model training job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_training_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_training_job)
         """
@@ -1745,45 +1744,45 @@
         self,
         *,
         DomainId: str,
         UserProfileName: str,
         SingleSignOnUserIdentifier: str = ...,
         SingleSignOnUserValue: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        UserSettings: UserSettingsTypeDef = ...,
+        UserSettings: UserSettingsUnionTypeDef = ...,
     ) -> CreateUserProfileResponseTypeDef:
         """
         Creates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_user_profile)
         """
 
     def create_workforce(
         self,
         *,
         WorkforceName: str,
         CognitoConfig: CognitoConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
-        SourceIpConfig: SourceIpConfigTypeDef = ...,
+        SourceIpConfig: SourceIpConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,
     ) -> CreateWorkforceResponseTypeDef:
         """
         Use this operation to create a workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workforce)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_workforce)
         """
 
     def create_workteam(
         self,
         *,
         WorkteamName: str,
-        MemberDefinitions: Sequence[MemberDefinitionTypeDef],
+        MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef],
         Description: str,
         WorkforceName: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkteamResponseTypeDef:
         """
         Creates a new work team for labeling your data.
@@ -1829,15 +1828,15 @@
         Deletes an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_app_image_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#delete_app_image_config)
         """
 
     def delete_artifact(
-        self, *, ArtifactArn: str = ..., Source: ArtifactSourceTypeDef = ...
+        self, *, ArtifactArn: str = ..., Source: ArtifactSourceUnionTypeDef = ...
     ) -> DeleteArtifactResponseTypeDef:
         """
         Deletes an artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_artifact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#delete_artifact)
         """
@@ -4557,15 +4556,15 @@
         *,
         PipelineName: str,
         ClientRequestToken: str,
         PipelineExecutionDisplayName: str = ...,
         PipelineParameters: Sequence[ParameterTypeDef] = ...,
         PipelineExecutionDescription: str = ...,
         ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
-        SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef = ...,
+        SelectiveExecutionConfig: SelectiveExecutionConfigUnionTypeDef = ...,
     ) -> StartPipelineExecutionResponseTypeDef:
         """
         Starts a pipeline execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_pipeline_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#start_pipeline_execution)
         """
@@ -4716,17 +4715,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_action)
         """
 
     def update_app_image_config(
         self,
         *,
         AppImageConfigName: str,
-        KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...,
-        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...,
-        CodeEditorAppImageConfig: CodeEditorAppImageConfigTypeDef = ...,
+        KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...,
+        JupyterLabAppImageConfig: JupyterLabAppImageConfigUnionTypeDef = ...,
+        CodeEditorAppImageConfig: CodeEditorAppImageConfigUnionTypeDef = ...,
     ) -> UpdateAppImageConfigResponseTypeDef:
         """
         Updates the properties of an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_app_image_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_app_image_config)
         """
@@ -4819,18 +4818,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_devices)
         """
 
     def update_domain(
         self,
         *,
         DomainId: str,
-        DefaultUserSettings: UserSettingsTypeDef = ...,
+        DefaultUserSettings: UserSettingsUnionTypeDef = ...,
         DomainSettingsForUpdate: DomainSettingsForUpdateTypeDef = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
+        DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...,
         SubnetIds: Sequence[str] = ...,
         AppNetworkAccessType: AppNetworkAccessTypeType = ...,
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the default settings for new user profiles in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_domain)
@@ -4840,15 +4839,15 @@
     def update_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
         RetainAllVariantProperties: bool = ...,
         ExcludeRetainedVariantProperties: Sequence[VariantPropertyTypeDef] = ...,
-        DeploymentConfig: DeploymentConfigTypeDef = ...,
+        DeploymentConfig: DeploymentConfigUnionTypeDef = ...,
         RetainDeploymentConfig: bool = ...,
     ) -> UpdateEndpointOutputTypeDef:
         """
         Deploys the `EndpointConfig` specified in the request to a new fleet of
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_endpoint)
@@ -4994,19 +4993,19 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_inference_component_runtime_config)
         """
 
     def update_inference_experiment(
         self,
         *,
         Name: str,
-        Schedule: InferenceExperimentScheduleTypeDef = ...,
+        Schedule: InferenceExperimentScheduleUnionTypeDef = ...,
         Description: str = ...,
         ModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,
-        DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
-        ShadowModeConfig: ShadowModeConfigTypeDef = ...,
+        DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,
+        ShadowModeConfig: ShadowModeConfigUnionTypeDef = ...,
     ) -> UpdateInferenceExperimentResponseTypeDef:
         """
         Updates an inference experiment that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_experiment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_inference_experiment)
         """
@@ -5026,17 +5025,17 @@
         *,
         ModelPackageArn: str,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ApprovalDescription: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         CustomerMetadataPropertiesToRemove: Sequence[str] = ...,
         AdditionalInferenceSpecificationsToAdd: Sequence[
-            AdditionalInferenceSpecificationDefinitionTypeDef
+            AdditionalInferenceSpecificationDefinitionUnionTypeDef
         ] = ...,
-        InferenceSpecification: InferenceSpecificationTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
         SourceUri: str = ...,
     ) -> UpdateModelPackageOutputTypeDef:
         """
         Updates a versioned model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_model_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_model_package)
@@ -5057,15 +5056,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_monitoring_alert)
         """
 
     def update_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
+        MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef,
     ) -> UpdateMonitoringScheduleResponseTypeDef:
         """
         Updates a previously created schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_monitoring_schedule)
         """
@@ -5162,30 +5161,30 @@
         """
 
     def update_space(
         self,
         *,
         DomainId: str,
         SpaceName: str,
-        SpaceSettings: SpaceSettingsTypeDef = ...,
+        SpaceSettings: SpaceSettingsUnionTypeDef = ...,
         SpaceDisplayName: str = ...,
     ) -> UpdateSpaceResponseTypeDef:
         """
         Updates the settings of a space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_space)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_space)
         """
 
     def update_training_job(
         self,
         *,
         TrainingJobName: str,
         ProfilerConfig: ProfilerConfigForUpdateTypeDef = ...,
-        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
+        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,
         ResourceConfig: ResourceConfigForUpdateTypeDef = ...,
         RemoteDebugConfig: RemoteDebugConfigForUpdateTypeDef = ...,
     ) -> UpdateTrainingJobResponseTypeDef:
         """
         Update a model training job to request a new Debugger profiling configuration
         or to change warm pool retention
         length.
@@ -5221,43 +5220,43 @@
         Updates one or more properties of a trial component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_trial_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_trial_component)
         """
 
     def update_user_profile(
-        self, *, DomainId: str, UserProfileName: str, UserSettings: UserSettingsTypeDef = ...
+        self, *, DomainId: str, UserProfileName: str, UserSettings: UserSettingsUnionTypeDef = ...
     ) -> UpdateUserProfileResponseTypeDef:
         """
         Updates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_user_profile)
         """
 
     def update_workforce(
         self,
         *,
         WorkforceName: str,
-        SourceIpConfig: SourceIpConfigTypeDef = ...,
+        SourceIpConfig: SourceIpConfigUnionTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
         WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,
     ) -> UpdateWorkforceResponseTypeDef:
         """
         Use this operation to update your workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workforce)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_workforce)
         """
 
     def update_workteam(
         self,
         *,
         WorkteamName: str,
-        MemberDefinitions: Sequence[MemberDefinitionTypeDef] = ...,
+        MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef] = ...,
         Description: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...,
     ) -> UpdateWorkteamResponseTypeDef:
         """
         Updates an existing work team with new member definitions or description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workteam)
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/client.pyi` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,39 +206,39 @@
     ListWorkforcesPaginator,
     ListWorkteamsPaginator,
     SearchPaginator,
 )
 from .type_defs import (
     ActionSourceTypeDef,
     AddAssociationResponseTypeDef,
-    AdditionalInferenceSpecificationDefinitionTypeDef,
+    AdditionalInferenceSpecificationDefinitionUnionTypeDef,
     AddTagsOutputTypeDef,
-    AlgorithmSpecificationTypeDef,
-    AlgorithmValidationSpecificationTypeDef,
-    AppSpecificationTypeDef,
-    ArtifactSourceTypeDef,
+    AlgorithmSpecificationUnionTypeDef,
+    AlgorithmValidationSpecificationUnionTypeDef,
+    AppSpecificationUnionTypeDef,
+    ArtifactSourceUnionTypeDef,
     AssociateTrialComponentResponseTypeDef,
-    AsyncInferenceConfigTypeDef,
+    AsyncInferenceConfigUnionTypeDef,
     AutoMLChannelTypeDef,
     AutoMLDataSplitConfigTypeDef,
     AutoMLJobChannelTypeDef,
-    AutoMLJobConfigTypeDef,
+    AutoMLJobConfigUnionTypeDef,
     AutoMLJobObjectiveTypeDef,
     AutoMLOutputDataConfigTypeDef,
-    AutoMLProblemTypeConfigTypeDef,
-    AutoMLSecurityConfigTypeDef,
+    AutoMLProblemTypeConfigUnionTypeDef,
+    AutoMLSecurityConfigUnionTypeDef,
     AutotuneTypeDef,
     BatchDataCaptureConfigTypeDef,
     BatchDescribeModelPackageOutputTypeDef,
-    ChannelTypeDef,
+    ChannelUnionTypeDef,
     CheckpointConfigTypeDef,
     ClusterInstanceGroupSpecificationTypeDef,
-    CodeEditorAppImageConfigTypeDef,
+    CodeEditorAppImageConfigUnionTypeDef,
     CognitoConfigTypeDef,
-    ContainerDefinitionTypeDef,
+    ContainerDefinitionUnionTypeDef,
     ContextSourceTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
@@ -285,34 +285,34 @@
     CreateTrainingJobResponseTypeDef,
     CreateTransformJobResponseTypeDef,
     CreateTrialComponentResponseTypeDef,
     CreateTrialResponseTypeDef,
     CreateUserProfileResponseTypeDef,
     CreateWorkforceResponseTypeDef,
     CreateWorkteamResponseTypeDef,
-    DataCaptureConfigTypeDef,
+    DataCaptureConfigUnionTypeDef,
     DataProcessingTypeDef,
-    DataQualityAppSpecificationTypeDef,
+    DataQualityAppSpecificationUnionTypeDef,
     DataQualityBaselineConfigTypeDef,
-    DataQualityJobInputTypeDef,
-    DebugHookConfigTypeDef,
-    DebugRuleConfigurationTypeDef,
-    DefaultSpaceSettingsTypeDef,
+    DataQualityJobInputUnionTypeDef,
+    DebugHookConfigUnionTypeDef,
+    DebugRuleConfigurationUnionTypeDef,
+    DefaultSpaceSettingsUnionTypeDef,
     DeleteActionResponseTypeDef,
     DeleteArtifactResponseTypeDef,
     DeleteAssociationResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteContextResponseTypeDef,
     DeleteExperimentResponseTypeDef,
     DeleteInferenceExperimentResponseTypeDef,
     DeletePipelineResponseTypeDef,
     DeleteTrialComponentResponseTypeDef,
     DeleteTrialResponseTypeDef,
     DeleteWorkteamResponseTypeDef,
-    DeploymentConfigTypeDef,
+    DeploymentConfigUnionTypeDef,
     DeploymentStageTypeDef,
     DescribeActionResponseTypeDef,
     DescribeAlgorithmOutputTypeDef,
     DescribeAppImageConfigResponseTypeDef,
     DescribeAppResponseTypeDef,
     DescribeArtifactResponseTypeDef,
     DescribeAutoMLJobResponseTypeDef,
@@ -371,54 +371,54 @@
     DescribeUserProfileResponseTypeDef,
     DescribeWorkforceResponseTypeDef,
     DescribeWorkteamResponseTypeDef,
     DesiredWeightAndCapacityTypeDef,
     DeviceTypeDef,
     DisassociateTrialComponentResponseTypeDef,
     DomainSettingsForUpdateTypeDef,
-    DomainSettingsTypeDef,
+    DomainSettingsUnionTypeDef,
     DriftCheckBaselinesTypeDef,
     EdgeDeploymentModelConfigTypeDef,
     EdgeOutputConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     ExperimentConfigTypeDef,
-    ExplainerConfigTypeDef,
+    ExplainerConfigUnionTypeDef,
     FeatureDefinitionTypeDef,
     FeatureParameterTypeDef,
     FlowDefinitionOutputConfigTypeDef,
     GetDeviceFleetReportResponseTypeDef,
     GetLineageGroupPolicyResponseTypeDef,
     GetModelPackageGroupPolicyOutputTypeDef,
     GetSagemakerServicecatalogPortfolioStatusOutputTypeDef,
     GetScalingConfigurationRecommendationResponseTypeDef,
     GetSearchSuggestionsResponseTypeDef,
     GitConfigForUpdateTypeDef,
     GitConfigTypeDef,
     HubS3StorageConfigTypeDef,
     HumanLoopActivationConfigTypeDef,
-    HumanLoopConfigTypeDef,
+    HumanLoopConfigUnionTypeDef,
     HumanLoopRequestSourceTypeDef,
-    HumanTaskConfigTypeDef,
-    HyperParameterTrainingJobDefinitionTypeDef,
-    HyperParameterTuningJobConfigTypeDef,
-    HyperParameterTuningJobWarmStartConfigTypeDef,
+    HumanTaskConfigUnionTypeDef,
+    HyperParameterTrainingJobDefinitionUnionTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
+    HyperParameterTuningJobWarmStartConfigUnionTypeDef,
     ImportHubContentResponseTypeDef,
     InferenceComponentRuntimeConfigTypeDef,
     InferenceComponentSpecificationTypeDef,
     InferenceExecutionConfigTypeDef,
-    InferenceExperimentDataStorageConfigTypeDef,
-    InferenceExperimentScheduleTypeDef,
-    InferenceSpecificationTypeDef,
+    InferenceExperimentDataStorageConfigUnionTypeDef,
+    InferenceExperimentScheduleUnionTypeDef,
+    InferenceSpecificationUnionTypeDef,
     InfraCheckConfigTypeDef,
     InputConfigTypeDef,
     InstanceMetadataServiceConfigurationTypeDef,
-    JupyterLabAppImageConfigTypeDef,
-    KernelGatewayImageConfigTypeDef,
-    LabelingJobAlgorithmsConfigTypeDef,
-    LabelingJobInputConfigTypeDef,
+    JupyterLabAppImageConfigUnionTypeDef,
+    KernelGatewayImageConfigUnionTypeDef,
+    LabelingJobAlgorithmsConfigUnionTypeDef,
+    LabelingJobInputConfigUnionTypeDef,
     LabelingJobOutputConfigTypeDef,
     LabelingJobStoppingConditionsTypeDef,
     ListActionsResponseTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAliasesResponseTypeDef,
     ListAppImageConfigsResponseTypeDef,
     ListAppsResponseTypeDef,
@@ -488,102 +488,103 @@
     ListTrainingJobsResponseTypeDef,
     ListTransformJobsResponseTypeDef,
     ListTrialComponentsResponseTypeDef,
     ListTrialsResponseTypeDef,
     ListUserProfilesResponseTypeDef,
     ListWorkforcesResponseTypeDef,
     ListWorkteamsResponseTypeDef,
-    MemberDefinitionTypeDef,
+    MemberDefinitionUnionTypeDef,
     MetadataPropertiesTypeDef,
-    ModelBiasAppSpecificationTypeDef,
+    ModelBiasAppSpecificationUnionTypeDef,
     ModelBiasBaselineConfigTypeDef,
-    ModelBiasJobInputTypeDef,
+    ModelBiasJobInputUnionTypeDef,
     ModelCardExportOutputConfigTypeDef,
     ModelCardSecurityConfigTypeDef,
     ModelClientConfigTypeDef,
     ModelDeployConfigTypeDef,
-    ModelExplainabilityAppSpecificationTypeDef,
+    ModelExplainabilityAppSpecificationUnionTypeDef,
     ModelExplainabilityBaselineConfigTypeDef,
-    ModelExplainabilityJobInputTypeDef,
+    ModelExplainabilityJobInputUnionTypeDef,
     ModelMetadataSearchExpressionTypeDef,
     ModelMetricsTypeDef,
-    ModelPackageValidationSpecificationTypeDef,
-    ModelQualityAppSpecificationTypeDef,
+    ModelPackageValidationSpecificationUnionTypeDef,
+    ModelQualityAppSpecificationUnionTypeDef,
     ModelQualityBaselineConfigTypeDef,
-    ModelQualityJobInputTypeDef,
+    ModelQualityJobInputUnionTypeDef,
     ModelVariantConfigTypeDef,
-    MonitoringNetworkConfigTypeDef,
-    MonitoringOutputConfigTypeDef,
+    MonitoringNetworkConfigUnionTypeDef,
+    MonitoringOutputConfigUnionTypeDef,
     MonitoringResourcesTypeDef,
-    MonitoringScheduleConfigTypeDef,
+    MonitoringScheduleConfigUnionTypeDef,
     MonitoringStoppingConditionTypeDef,
-    NeoVpcConfigTypeDef,
-    NetworkConfigTypeDef,
+    NeoVpcConfigUnionTypeDef,
+    NetworkConfigUnionTypeDef,
     NotebookInstanceLifecycleHookTypeDef,
     NotificationConfigurationTypeDef,
     OfflineStoreConfigTypeDef,
     OidcConfigTypeDef,
     OnlineStoreConfigTypeDef,
     OnlineStoreConfigUpdateTypeDef,
     OutputConfigTypeDef,
     OutputDataConfigTypeDef,
     OutputParameterTypeDef,
     OwnershipSettingsTypeDef,
     ParallelismConfigurationTypeDef,
     ParameterTypeDef,
     PipelineDefinitionS3LocationTypeDef,
     ProcessingInputTypeDef,
-    ProcessingOutputConfigTypeDef,
+    ProcessingOutputConfigUnionTypeDef,
     ProcessingResourcesTypeDef,
     ProcessingStoppingConditionTypeDef,
     ProductionVariantTypeDef,
     ProfilerConfigForUpdateTypeDef,
-    ProfilerConfigTypeDef,
-    ProfilerRuleConfigurationTypeDef,
+    ProfilerConfigUnionTypeDef,
+    ProfilerRuleConfigurationUnionTypeDef,
     PutModelPackageGroupPolicyOutputTypeDef,
     QueryFiltersTypeDef,
     QueryLineageResponseTypeDef,
-    RecommendationJobInputConfigTypeDef,
+    RecommendationJobInputConfigUnionTypeDef,
     RecommendationJobOutputConfigTypeDef,
-    RecommendationJobStoppingConditionsTypeDef,
+    RecommendationJobStoppingConditionsUnionTypeDef,
     RemoteDebugConfigForUpdateTypeDef,
     RemoteDebugConfigTypeDef,
     RenderableTaskTypeDef,
     RenderUiTemplateResponseTypeDef,
     ResourceConfigForUpdateTypeDef,
-    ResourceConfigTypeDef,
+    ResourceConfigUnionTypeDef,
     ResourceSpecTypeDef,
     RetentionPolicyTypeDef,
     RetryPipelineExecutionResponseTypeDef,
     RetryStrategyTypeDef,
     ScalingPolicyObjectiveTypeDef,
     SearchExpressionTypeDef,
     SearchResponseTypeDef,
-    SelectiveExecutionConfigTypeDef,
+    SelectiveExecutionConfigUnionTypeDef,
     SendPipelineExecutionStepFailureResponseTypeDef,
     SendPipelineExecutionStepSuccessResponseTypeDef,
-    ServiceCatalogProvisioningDetailsTypeDef,
+    ServiceCatalogProvisioningDetailsUnionTypeDef,
     ServiceCatalogProvisioningUpdateDetailsTypeDef,
-    ShadowModeConfigTypeDef,
-    SourceAlgorithmSpecificationTypeDef,
-    SourceIpConfigTypeDef,
-    SpaceSettingsTypeDef,
+    SessionChainingConfigTypeDef,
+    ShadowModeConfigUnionTypeDef,
+    SourceAlgorithmSpecificationUnionTypeDef,
+    SourceIpConfigUnionTypeDef,
+    SpaceSettingsUnionTypeDef,
     SpaceSharingSettingsTypeDef,
     StartInferenceExperimentResponseTypeDef,
     StartPipelineExecutionResponseTypeDef,
     StopInferenceExperimentResponseTypeDef,
     StoppingConditionTypeDef,
     StopPipelineExecutionResponseTypeDef,
     SuggestionQueryTypeDef,
     TagTypeDef,
     TensorBoardOutputConfigTypeDef,
     ThroughputConfigTypeDef,
     ThroughputConfigUpdateTypeDef,
     TimestampTypeDef,
-    TrainingSpecificationTypeDef,
+    TrainingSpecificationUnionTypeDef,
     TransformInputTypeDef,
     TransformOutputTypeDef,
     TransformResourcesTypeDef,
     TrialComponentArtifactTypeDef,
     TrialComponentParameterValueTypeDef,
     TrialComponentStatusTypeDef,
     UiTemplateTypeDef,
@@ -615,18 +616,18 @@
     UpdateSpaceResponseTypeDef,
     UpdateTrainingJobResponseTypeDef,
     UpdateTrialComponentResponseTypeDef,
     UpdateTrialResponseTypeDef,
     UpdateUserProfileResponseTypeDef,
     UpdateWorkforceResponseTypeDef,
     UpdateWorkteamResponseTypeDef,
-    UserSettingsTypeDef,
+    UserSettingsUnionTypeDef,
     VariantPropertyTypeDef,
     VisibilityConditionsTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
     WorkforceVpcConfigRequestTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     EndpointInServiceWaiter,
     ImageCreatedWaiter,
     ImageDeletedWaiter,
@@ -644,28 +645,31 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("SageMakerClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ResourceInUse: Type[BotocoreClientError]
     ResourceLimitExceeded: Type[BotocoreClientError]
     ResourceNotFound: Type[BotocoreClientError]
 
+
 class SageMakerClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/)
     """
 
     meta: ClientMeta
@@ -754,18 +758,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_action)
         """
 
     def create_algorithm(
         self,
         *,
         AlgorithmName: str,
-        TrainingSpecification: TrainingSpecificationTypeDef,
+        TrainingSpecification: TrainingSpecificationUnionTypeDef,
         AlgorithmDescription: str = ...,
-        InferenceSpecification: InferenceSpecificationTypeDef = ...,
-        ValidationSpecification: AlgorithmValidationSpecificationTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
+        ValidationSpecification: AlgorithmValidationSpecificationUnionTypeDef = ...,
         CertifyForMarketplace: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAlgorithmOutputTypeDef:
         """
         Create a machine learning algorithm that you can use in SageMaker and list in
         the Amazon Web Services
         Marketplace.
@@ -793,29 +797,29 @@
         """
 
     def create_app_image_config(
         self,
         *,
         AppImageConfigName: str,
         Tags: Sequence[TagTypeDef] = ...,
-        KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...,
-        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...,
-        CodeEditorAppImageConfig: CodeEditorAppImageConfigTypeDef = ...,
+        KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...,
+        JupyterLabAppImageConfig: JupyterLabAppImageConfigUnionTypeDef = ...,
+        CodeEditorAppImageConfig: CodeEditorAppImageConfigUnionTypeDef = ...,
     ) -> CreateAppImageConfigResponseTypeDef:
         """
         Creates a configuration for running a SageMaker image as a KernelGateway app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app_image_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_app_image_config)
         """
 
     def create_artifact(
         self,
         *,
-        Source: ArtifactSourceTypeDef,
+        Source: ArtifactSourceUnionTypeDef,
         ArtifactType: str,
         ArtifactName: str = ...,
         Properties: Mapping[str, str] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateArtifactResponseTypeDef:
         """
@@ -830,15 +834,15 @@
         *,
         AutoMLJobName: str,
         InputDataConfig: Sequence[AutoMLChannelTypeDef],
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
         RoleArn: str,
         ProblemType: ProblemTypeType = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
-        AutoMLJobConfig: AutoMLJobConfigTypeDef = ...,
+        AutoMLJobConfig: AutoMLJobConfigUnionTypeDef = ...,
         GenerateCandidateDefinitionsOnly: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...,
     ) -> CreateAutoMLJobResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job.
 
@@ -848,18 +852,18 @@
 
     def create_auto_ml_job_v2(
         self,
         *,
         AutoMLJobName: str,
         AutoMLJobInputDataConfig: Sequence[AutoMLJobChannelTypeDef],
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
-        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,
+        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigUnionTypeDef,
         RoleArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        SecurityConfig: AutoMLSecurityConfigTypeDef = ...,
+        SecurityConfig: AutoMLSecurityConfigUnionTypeDef = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...,
         DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...,
     ) -> CreateAutoMLJobV2ResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job
         V2.
@@ -869,15 +873,15 @@
         """
 
     def create_cluster(
         self,
         *,
         ClusterName: str,
         InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef],
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a SageMaker HyperPod cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_cluster)
@@ -902,15 +906,15 @@
         *,
         CompilationJobName: str,
         RoleArn: str,
         OutputConfig: OutputConfigTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         ModelPackageVersionArn: str = ...,
         InputConfig: InputConfigTypeDef = ...,
-        VpcConfig: NeoVpcConfigTypeDef = ...,
+        VpcConfig: NeoVpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCompilationJobResponseTypeDef:
         """
         Starts a model compilation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_compilation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_compilation_job)
@@ -933,21 +937,21 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_context)
         """
 
     def create_data_quality_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        DataQualityAppSpecification: DataQualityAppSpecificationTypeDef,
-        DataQualityJobInput: DataQualityJobInputTypeDef,
-        DataQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
+        DataQualityAppSpecification: DataQualityAppSpecificationUnionTypeDef,
+        DataQualityJobInput: DataQualityJobInputUnionTypeDef,
+        DataQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         DataQualityBaselineConfig: DataQualityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors data quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_data_quality_job_definition)
@@ -972,24 +976,24 @@
         """
 
     def create_domain(
         self,
         *,
         DomainName: str,
         AuthMode: AuthModeType,
-        DefaultUserSettings: UserSettingsTypeDef,
+        DefaultUserSettings: UserSettingsUnionTypeDef,
         SubnetIds: Sequence[str],
         VpcId: str,
-        DomainSettings: DomainSettingsTypeDef = ...,
+        DomainSettings: DomainSettingsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AppNetworkAccessType: AppNetworkAccessTypeType = ...,
         HomeEfsFileSystemKmsKeyId: str = ...,
         KmsKeyId: str = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
+        DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a `Domain`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_domain)
         """
@@ -1040,37 +1044,37 @@
         """
 
     def create_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
-        DeploymentConfig: DeploymentConfigTypeDef = ...,
+        DeploymentConfig: DeploymentConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEndpointOutputTypeDef:
         """
         Creates an endpoint using the endpoint configuration specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_endpoint)
         """
 
     def create_endpoint_config(
         self,
         *,
         EndpointConfigName: str,
         ProductionVariants: Sequence[ProductionVariantTypeDef],
-        DataCaptureConfig: DataCaptureConfigTypeDef = ...,
+        DataCaptureConfig: DataCaptureConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
-        AsyncInferenceConfig: AsyncInferenceConfigTypeDef = ...,
-        ExplainerConfig: ExplainerConfigTypeDef = ...,
+        AsyncInferenceConfig: AsyncInferenceConfigUnionTypeDef = ...,
+        ExplainerConfig: ExplainerConfigUnionTypeDef = ...,
         ShadowProductionVariants: Sequence[ProductionVariantTypeDef] = ...,
         ExecutionRoleArn: str = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         EnableNetworkIsolation: bool = ...,
     ) -> CreateEndpointConfigOutputTypeDef:
         """
         Creates an endpoint configuration that SageMaker hosting services uses to
         deploy
         models.
 
@@ -1118,15 +1122,15 @@
         self,
         *,
         FlowDefinitionName: str,
         OutputConfig: FlowDefinitionOutputConfigTypeDef,
         RoleArn: str,
         HumanLoopRequestSource: HumanLoopRequestSourceTypeDef = ...,
         HumanLoopActivationConfig: HumanLoopActivationConfigTypeDef = ...,
-        HumanLoopConfig: HumanLoopConfigTypeDef = ...,
+        HumanLoopConfig: HumanLoopConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFlowDefinitionResponseTypeDef:
         """
         Creates a flow definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_flow_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_flow_definition)
@@ -1163,18 +1167,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_human_task_ui)
         """
 
     def create_hyper_parameter_tuning_job(
         self,
         *,
         HyperParameterTuningJobName: str,
-        HyperParameterTuningJobConfig: HyperParameterTuningJobConfigTypeDef,
-        TrainingJobDefinition: HyperParameterTrainingJobDefinitionTypeDef = ...,
-        TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionTypeDef] = ...,
-        WarmStartConfig: HyperParameterTuningJobWarmStartConfigTypeDef = ...,
+        HyperParameterTuningJobConfig: HyperParameterTuningJobConfigUnionTypeDef,
+        TrainingJobDefinition: HyperParameterTrainingJobDefinitionUnionTypeDef = ...,
+        TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef] = ...,
+        WarmStartConfig: HyperParameterTuningJobWarmStartConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Autotune: AutotuneTypeDef = ...,
     ) -> CreateHyperParameterTuningJobResponseTypeDef:
         """
         Starts a hyperparameter tuning job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hyper_parameter_tuning_job)
@@ -1242,18 +1246,18 @@
         self,
         *,
         Name: str,
         Type: Literal["ShadowMode"],
         RoleArn: str,
         EndpointName: str,
         ModelVariants: Sequence[ModelVariantConfigTypeDef],
-        ShadowModeConfig: ShadowModeConfigTypeDef,
-        Schedule: InferenceExperimentScheduleTypeDef = ...,
+        ShadowModeConfig: ShadowModeConfigUnionTypeDef,
+        Schedule: InferenceExperimentScheduleUnionTypeDef = ...,
         Description: str = ...,
-        DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
+        DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,
         KmsKey: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceExperimentResponseTypeDef:
         """
         Creates an inference experiment using the configurations specified in the
         request.
 
@@ -1263,17 +1267,17 @@
 
     def create_inference_recommendations_job(
         self,
         *,
         JobName: str,
         JobType: RecommendationJobTypeType,
         RoleArn: str,
-        InputConfig: RecommendationJobInputConfigTypeDef,
+        InputConfig: RecommendationJobInputConfigUnionTypeDef,
         JobDescription: str = ...,
-        StoppingConditions: RecommendationJobStoppingConditionsTypeDef = ...,
+        StoppingConditions: RecommendationJobStoppingConditionsUnionTypeDef = ...,
         OutputConfig: RecommendationJobOutputConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceRecommendationsJobResponseTypeDef:
         """
         Starts a recommendation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_recommendations_job)
@@ -1281,60 +1285,60 @@
         """
 
     def create_labeling_job(
         self,
         *,
         LabelingJobName: str,
         LabelAttributeName: str,
-        InputConfig: LabelingJobInputConfigTypeDef,
+        InputConfig: LabelingJobInputConfigUnionTypeDef,
         OutputConfig: LabelingJobOutputConfigTypeDef,
         RoleArn: str,
-        HumanTaskConfig: HumanTaskConfigTypeDef,
+        HumanTaskConfig: HumanTaskConfigUnionTypeDef,
         LabelCategoryConfigS3Uri: str = ...,
         StoppingConditions: LabelingJobStoppingConditionsTypeDef = ...,
-        LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigTypeDef = ...,
+        LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLabelingJobResponseTypeDef:
         """
         Creates a job that uses workers to label the data objects in your input dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_labeling_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_labeling_job)
         """
 
     def create_model(
         self,
         *,
         ModelName: str,
-        PrimaryContainer: ContainerDefinitionTypeDef = ...,
-        Containers: Sequence[ContainerDefinitionTypeDef] = ...,
+        PrimaryContainer: ContainerDefinitionUnionTypeDef = ...,
+        Containers: Sequence[ContainerDefinitionUnionTypeDef] = ...,
         InferenceExecutionConfig: InferenceExecutionConfigTypeDef = ...,
         ExecutionRoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         EnableNetworkIsolation: bool = ...,
     ) -> CreateModelOutputTypeDef:
         """
         Creates a model in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_model)
         """
 
     def create_model_bias_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelBiasAppSpecification: ModelBiasAppSpecificationTypeDef,
-        ModelBiasJobInput: ModelBiasJobInputTypeDef,
-        ModelBiasJobOutputConfig: MonitoringOutputConfigTypeDef,
+        ModelBiasAppSpecification: ModelBiasAppSpecificationUnionTypeDef,
+        ModelBiasJobInput: ModelBiasJobInputUnionTypeDef,
+        ModelBiasJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelBiasBaselineConfig: ModelBiasBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelBiasJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model bias job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_bias_job_definition)
@@ -1372,21 +1376,21 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_model_card_export_job)
         """
 
     def create_model_explainability_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationTypeDef,
-        ModelExplainabilityJobInput: ModelExplainabilityJobInputTypeDef,
-        ModelExplainabilityJobOutputConfig: MonitoringOutputConfigTypeDef,
+        ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationUnionTypeDef,
+        ModelExplainabilityJobInput: ModelExplainabilityJobInputUnionTypeDef,
+        ModelExplainabilityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelExplainabilityBaselineConfig: ModelExplainabilityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelExplainabilityJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model explainability job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_explainability_job_definition)
@@ -1395,30 +1399,30 @@
 
     def create_model_package(
         self,
         *,
         ModelPackageName: str = ...,
         ModelPackageGroupName: str = ...,
         ModelPackageDescription: str = ...,
-        InferenceSpecification: InferenceSpecificationTypeDef = ...,
-        ValidationSpecification: ModelPackageValidationSpecificationTypeDef = ...,
-        SourceAlgorithmSpecification: SourceAlgorithmSpecificationTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
+        ValidationSpecification: ModelPackageValidationSpecificationUnionTypeDef = ...,
+        SourceAlgorithmSpecification: SourceAlgorithmSpecificationUnionTypeDef = ...,
         CertifyForMarketplace: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         ModelMetrics: ModelMetricsTypeDef = ...,
         ClientToken: str = ...,
         Domain: str = ...,
         Task: str = ...,
         SamplePayloadUrl: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         DriftCheckBaselines: DriftCheckBaselinesTypeDef = ...,
         AdditionalInferenceSpecifications: Sequence[
-            AdditionalInferenceSpecificationDefinitionTypeDef
+            AdditionalInferenceSpecificationDefinitionUnionTypeDef
         ] = ...,
         SkipModelValidation: SkipModelValidationType = ...,
         SourceUri: str = ...,
     ) -> CreateModelPackageOutputTypeDef:
         """
         Creates a model package that you can use to create SageMaker models or list on
         Amazon Web Services Marketplace, or a versioned model that is part of a model
@@ -1442,36 +1446,36 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_model_package_group)
         """
 
     def create_model_quality_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelQualityAppSpecification: ModelQualityAppSpecificationTypeDef,
-        ModelQualityJobInput: ModelQualityJobInputTypeDef,
-        ModelQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
+        ModelQualityAppSpecification: ModelQualityAppSpecificationUnionTypeDef,
+        ModelQualityJobInput: ModelQualityJobInputUnionTypeDef,
+        ModelQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelQualityBaselineConfig: ModelQualityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors model quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_quality_job_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_model_quality_job_definition)
         """
 
     def create_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
+        MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMonitoringScheduleResponseTypeDef:
         """
         Creates a schedule that regularly starts Amazon SageMaker Processing Jobs to
         monitor the data captured for an Amazon SageMaker
         Endpoint.
 
@@ -1570,36 +1574,36 @@
         """
 
     def create_processing_job(
         self,
         *,
         ProcessingJobName: str,
         ProcessingResources: ProcessingResourcesTypeDef,
-        AppSpecification: AppSpecificationTypeDef,
+        AppSpecification: AppSpecificationUnionTypeDef,
         RoleArn: str,
         ProcessingInputs: Sequence[ProcessingInputTypeDef] = ...,
-        ProcessingOutputConfig: ProcessingOutputConfigTypeDef = ...,
+        ProcessingOutputConfig: ProcessingOutputConfigUnionTypeDef = ...,
         StoppingCondition: ProcessingStoppingConditionTypeDef = ...,
         Environment: Mapping[str, str] = ...,
-        NetworkConfig: NetworkConfigTypeDef = ...,
+        NetworkConfig: NetworkConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...,
     ) -> CreateProcessingJobResponseTypeDef:
         """
         Creates a processing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_processing_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_processing_job)
         """
 
     def create_project(
         self,
         *,
         ProjectName: str,
-        ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsTypeDef,
+        ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsUnionTypeDef,
         ProjectDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a machine learning (ML) project that can contain one or more templates
         that set up an ML pipeline from training to deploying an approved
         model.
@@ -1610,15 +1614,15 @@
 
     def create_space(
         self,
         *,
         DomainId: str,
         SpaceName: str,
         Tags: Sequence[TagTypeDef] = ...,
-        SpaceSettings: SpaceSettingsTypeDef = ...,
+        SpaceSettings: SpaceSettingsUnionTypeDef = ...,
         OwnershipSettings: OwnershipSettingsTypeDef = ...,
         SpaceSharingSettings: SpaceSharingSettingsTypeDef = ...,
         SpaceDisplayName: str = ...,
     ) -> CreateSpaceResponseTypeDef:
         """
         Creates a space used for real time collaboration in a domain.
 
@@ -1641,37 +1645,38 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_studio_lifecycle_config)
         """
 
     def create_training_job(
         self,
         *,
         TrainingJobName: str,
-        AlgorithmSpecification: AlgorithmSpecificationTypeDef,
+        AlgorithmSpecification: AlgorithmSpecificationUnionTypeDef,
         RoleArn: str,
         OutputDataConfig: OutputDataConfigTypeDef,
-        ResourceConfig: ResourceConfigTypeDef,
+        ResourceConfig: ResourceConfigUnionTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         HyperParameters: Mapping[str, str] = ...,
-        InputDataConfig: Sequence[ChannelTypeDef] = ...,
-        VpcConfig: VpcConfigTypeDef = ...,
+        InputDataConfig: Sequence[ChannelUnionTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EnableNetworkIsolation: bool = ...,
         EnableInterContainerTrafficEncryption: bool = ...,
         EnableManagedSpotTraining: bool = ...,
         CheckpointConfig: CheckpointConfigTypeDef = ...,
-        DebugHookConfig: DebugHookConfigTypeDef = ...,
-        DebugRuleConfigurations: Sequence[DebugRuleConfigurationTypeDef] = ...,
+        DebugHookConfig: DebugHookConfigUnionTypeDef = ...,
+        DebugRuleConfigurations: Sequence[DebugRuleConfigurationUnionTypeDef] = ...,
         TensorBoardOutputConfig: TensorBoardOutputConfigTypeDef = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...,
-        ProfilerConfig: ProfilerConfigTypeDef = ...,
-        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
+        ProfilerConfig: ProfilerConfigUnionTypeDef = ...,
+        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,
         Environment: Mapping[str, str] = ...,
         RetryStrategy: RetryStrategyTypeDef = ...,
         RemoteDebugConfig: RemoteDebugConfigTypeDef = ...,
         InfraCheckConfig: InfraCheckConfigTypeDef = ...,
+        SessionChainingConfig: SessionChainingConfigTypeDef = ...,
     ) -> CreateTrainingJobResponseTypeDef:
         """
         Starts a model training job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_training_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_training_job)
         """
@@ -1742,45 +1747,45 @@
         self,
         *,
         DomainId: str,
         UserProfileName: str,
         SingleSignOnUserIdentifier: str = ...,
         SingleSignOnUserValue: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        UserSettings: UserSettingsTypeDef = ...,
+        UserSettings: UserSettingsUnionTypeDef = ...,
     ) -> CreateUserProfileResponseTypeDef:
         """
         Creates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_user_profile)
         """
 
     def create_workforce(
         self,
         *,
         WorkforceName: str,
         CognitoConfig: CognitoConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
-        SourceIpConfig: SourceIpConfigTypeDef = ...,
+        SourceIpConfig: SourceIpConfigUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,
     ) -> CreateWorkforceResponseTypeDef:
         """
         Use this operation to create a workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workforce)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_workforce)
         """
 
     def create_workteam(
         self,
         *,
         WorkteamName: str,
-        MemberDefinitions: Sequence[MemberDefinitionTypeDef],
+        MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef],
         Description: str,
         WorkforceName: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkteamResponseTypeDef:
         """
         Creates a new work team for labeling your data.
@@ -1826,15 +1831,15 @@
         Deletes an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_app_image_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#delete_app_image_config)
         """
 
     def delete_artifact(
-        self, *, ArtifactArn: str = ..., Source: ArtifactSourceTypeDef = ...
+        self, *, ArtifactArn: str = ..., Source: ArtifactSourceUnionTypeDef = ...
     ) -> DeleteArtifactResponseTypeDef:
         """
         Deletes an artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_artifact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#delete_artifact)
         """
@@ -4554,15 +4559,15 @@
         *,
         PipelineName: str,
         ClientRequestToken: str,
         PipelineExecutionDisplayName: str = ...,
         PipelineParameters: Sequence[ParameterTypeDef] = ...,
         PipelineExecutionDescription: str = ...,
         ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
-        SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef = ...,
+        SelectiveExecutionConfig: SelectiveExecutionConfigUnionTypeDef = ...,
     ) -> StartPipelineExecutionResponseTypeDef:
         """
         Starts a pipeline execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_pipeline_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#start_pipeline_execution)
         """
@@ -4713,17 +4718,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_action)
         """
 
     def update_app_image_config(
         self,
         *,
         AppImageConfigName: str,
-        KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...,
-        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...,
-        CodeEditorAppImageConfig: CodeEditorAppImageConfigTypeDef = ...,
+        KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...,
+        JupyterLabAppImageConfig: JupyterLabAppImageConfigUnionTypeDef = ...,
+        CodeEditorAppImageConfig: CodeEditorAppImageConfigUnionTypeDef = ...,
     ) -> UpdateAppImageConfigResponseTypeDef:
         """
         Updates the properties of an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_app_image_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_app_image_config)
         """
@@ -4816,18 +4821,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_devices)
         """
 
     def update_domain(
         self,
         *,
         DomainId: str,
-        DefaultUserSettings: UserSettingsTypeDef = ...,
+        DefaultUserSettings: UserSettingsUnionTypeDef = ...,
         DomainSettingsForUpdate: DomainSettingsForUpdateTypeDef = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
+        DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...,
         SubnetIds: Sequence[str] = ...,
         AppNetworkAccessType: AppNetworkAccessTypeType = ...,
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the default settings for new user profiles in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_domain)
@@ -4837,15 +4842,15 @@
     def update_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
         RetainAllVariantProperties: bool = ...,
         ExcludeRetainedVariantProperties: Sequence[VariantPropertyTypeDef] = ...,
-        DeploymentConfig: DeploymentConfigTypeDef = ...,
+        DeploymentConfig: DeploymentConfigUnionTypeDef = ...,
         RetainDeploymentConfig: bool = ...,
     ) -> UpdateEndpointOutputTypeDef:
         """
         Deploys the `EndpointConfig` specified in the request to a new fleet of
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_endpoint)
@@ -4991,19 +4996,19 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_inference_component_runtime_config)
         """
 
     def update_inference_experiment(
         self,
         *,
         Name: str,
-        Schedule: InferenceExperimentScheduleTypeDef = ...,
+        Schedule: InferenceExperimentScheduleUnionTypeDef = ...,
         Description: str = ...,
         ModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,
-        DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
-        ShadowModeConfig: ShadowModeConfigTypeDef = ...,
+        DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,
+        ShadowModeConfig: ShadowModeConfigUnionTypeDef = ...,
     ) -> UpdateInferenceExperimentResponseTypeDef:
         """
         Updates an inference experiment that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_experiment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_inference_experiment)
         """
@@ -5023,17 +5028,17 @@
         *,
         ModelPackageArn: str,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ApprovalDescription: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         CustomerMetadataPropertiesToRemove: Sequence[str] = ...,
         AdditionalInferenceSpecificationsToAdd: Sequence[
-            AdditionalInferenceSpecificationDefinitionTypeDef
+            AdditionalInferenceSpecificationDefinitionUnionTypeDef
         ] = ...,
-        InferenceSpecification: InferenceSpecificationTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
         SourceUri: str = ...,
     ) -> UpdateModelPackageOutputTypeDef:
         """
         Updates a versioned model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_model_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_model_package)
@@ -5054,15 +5059,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_monitoring_alert)
         """
 
     def update_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
+        MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef,
     ) -> UpdateMonitoringScheduleResponseTypeDef:
         """
         Updates a previously created schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_monitoring_schedule)
         """
@@ -5159,30 +5164,30 @@
         """
 
     def update_space(
         self,
         *,
         DomainId: str,
         SpaceName: str,
-        SpaceSettings: SpaceSettingsTypeDef = ...,
+        SpaceSettings: SpaceSettingsUnionTypeDef = ...,
         SpaceDisplayName: str = ...,
     ) -> UpdateSpaceResponseTypeDef:
         """
         Updates the settings of a space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_space)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_space)
         """
 
     def update_training_job(
         self,
         *,
         TrainingJobName: str,
         ProfilerConfig: ProfilerConfigForUpdateTypeDef = ...,
-        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
+        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,
         ResourceConfig: ResourceConfigForUpdateTypeDef = ...,
         RemoteDebugConfig: RemoteDebugConfigForUpdateTypeDef = ...,
     ) -> UpdateTrainingJobResponseTypeDef:
         """
         Update a model training job to request a new Debugger profiling configuration
         or to change warm pool retention
         length.
@@ -5218,43 +5223,43 @@
         Updates one or more properties of a trial component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_trial_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_trial_component)
         """
 
     def update_user_profile(
-        self, *, DomainId: str, UserProfileName: str, UserSettings: UserSettingsTypeDef = ...
+        self, *, DomainId: str, UserProfileName: str, UserSettings: UserSettingsUnionTypeDef = ...
     ) -> UpdateUserProfileResponseTypeDef:
         """
         Updates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_user_profile)
         """
 
     def update_workforce(
         self,
         *,
         WorkforceName: str,
-        SourceIpConfig: SourceIpConfigTypeDef = ...,
+        SourceIpConfig: SourceIpConfigUnionTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
         WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,
     ) -> UpdateWorkforceResponseTypeDef:
         """
         Use this operation to update your workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workforce)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#update_workforce)
         """
 
     def update_workteam(
         self,
         *,
         WorkteamName: str,
-        MemberDefinitions: Sequence[MemberDefinitionTypeDef] = ...,
+        MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef] = ...,
         Description: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...,
     ) -> UpdateWorkteamResponseTypeDef:
         """
         Updates an existing work team with new member definitions or description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workteam)
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/literals.py` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1359,14 +1359,22 @@
     "ml.g5.16xlarge",
     "ml.g5.24xlarge",
     "ml.g5.2xlarge",
     "ml.g5.48xlarge",
     "ml.g5.4xlarge",
     "ml.g5.8xlarge",
     "ml.g5.xlarge",
+    "ml.g6.12xlarge",
+    "ml.g6.16xlarge",
+    "ml.g6.24xlarge",
+    "ml.g6.2xlarge",
+    "ml.g6.48xlarge",
+    "ml.g6.4xlarge",
+    "ml.g6.8xlarge",
+    "ml.g6.xlarge",
     "ml.inf1.24xlarge",
     "ml.inf1.2xlarge",
     "ml.inf1.6xlarge",
     "ml.inf1.xlarge",
     "ml.inf2.24xlarge",
     "ml.inf2.48xlarge",
     "ml.inf2.8xlarge",
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/literals.pyi` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1359,14 +1359,22 @@
     "ml.g5.16xlarge",
     "ml.g5.24xlarge",
     "ml.g5.2xlarge",
     "ml.g5.48xlarge",
     "ml.g5.4xlarge",
     "ml.g5.8xlarge",
     "ml.g5.xlarge",
+    "ml.g6.12xlarge",
+    "ml.g6.16xlarge",
+    "ml.g6.24xlarge",
+    "ml.g6.2xlarge",
+    "ml.g6.48xlarge",
+    "ml.g6.4xlarge",
+    "ml.g6.8xlarge",
+    "ml.g6.xlarge",
     "ml.inf1.24xlarge",
     "ml.inf1.2xlarge",
     "ml.inf1.6xlarge",
     "ml.inf1.xlarge",
     "ml.inf2.24xlarge",
     "ml.inf2.48xlarge",
     "ml.inf2.8xlarge",
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/paginator.py` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,17 +257,17 @@
     UserProfileSortKeyType,
     WarmPoolResourceStatusType,
 )
 from .type_defs import (
     ListActionsResponseTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAliasesResponseTypeDef,
-    ListAppImageConfigsResponsePaginatorTypeDef,
+    ListAppImageConfigsResponseTypeDef,
     ListAppsResponseTypeDef,
-    ListArtifactsResponsePaginatorTypeDef,
+    ListArtifactsResponseTypeDef,
     ListAssociationsResponseTypeDef,
     ListAutoMLJobsResponseTypeDef,
     ListCandidatesForAutoMLJobResponseTypeDef,
     ListClusterNodesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListCodeRepositoriesOutputTypeDef,
     ListCompilationJobsResponseTypeDef,
@@ -284,19 +284,19 @@
     ListFeatureGroupsResponseTypeDef,
     ListFlowDefinitionsResponseTypeDef,
     ListHumanTaskUisResponseTypeDef,
     ListHyperParameterTuningJobsResponseTypeDef,
     ListImagesResponseTypeDef,
     ListImageVersionsResponseTypeDef,
     ListInferenceComponentsOutputTypeDef,
-    ListInferenceExperimentsResponsePaginatorTypeDef,
+    ListInferenceExperimentsResponseTypeDef,
     ListInferenceRecommendationsJobsResponseTypeDef,
     ListInferenceRecommendationsJobStepsResponseTypeDef,
     ListLabelingJobsForWorkteamResponseTypeDef,
-    ListLabelingJobsResponsePaginatorTypeDef,
+    ListLabelingJobsResponseTypeDef,
     ListLineageGroupsResponseTypeDef,
     ListModelBiasJobDefinitionsResponseTypeDef,
     ListModelCardExportJobsResponseTypeDef,
     ListModelCardsResponseTypeDef,
     ListModelCardVersionsResponseTypeDef,
     ListModelExplainabilityJobDefinitionsResponseTypeDef,
     ListModelMetadataResponseTypeDef,
@@ -323,20 +323,20 @@
     ListTagsOutputTypeDef,
     ListTrainingJobsForHyperParameterTuningJobResponseTypeDef,
     ListTrainingJobsResponseTypeDef,
     ListTransformJobsResponseTypeDef,
     ListTrialComponentsResponseTypeDef,
     ListTrialsResponseTypeDef,
     ListUserProfilesResponseTypeDef,
-    ListWorkforcesResponsePaginatorTypeDef,
-    ListWorkteamsResponsePaginatorTypeDef,
+    ListWorkforcesResponseTypeDef,
+    ListWorkteamsResponseTypeDef,
     ModelMetadataSearchExpressionTypeDef,
     PaginatorConfigTypeDef,
     SearchExpressionTypeDef,
-    SearchResponsePaginatorTypeDef,
+    SearchResponseTypeDef,
     TimestampTypeDef,
     VisibilityConditionsTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -505,15 +505,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: AppImageConfigSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListAppImageConfigsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListAppImageConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAppImageConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listappimageconfigspaginator)
         """
 
 
 class ListAppsPaginator(Paginator):
@@ -550,15 +550,15 @@
         SourceUri: str = ...,
         ArtifactType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: Literal["CreationTime"] = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListArtifactsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListArtifactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listartifactspaginator)
         """
 
 
 class ListAssociationsPaginator(Paginator):
@@ -1131,15 +1131,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         SortBy: SortInferenceExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListInferenceExperimentsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListInferenceExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceExperiments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listinferenceexperimentspaginator)
         """
 
 
 class ListInferenceRecommendationsJobStepsPaginator(Paginator):
@@ -1203,15 +1203,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: LabelingJobStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListLabelingJobsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListLabelingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListLabelingJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listlabelingjobspaginator)
         """
 
 
 class ListLabelingJobsForWorkteamPaginator(Paginator):
@@ -2004,15 +2004,15 @@
     def paginate(
         self,
         *,
         SortBy: ListWorkforcesSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListWorkforcesResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListWorkforcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListWorkforces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listworkforcespaginator)
         """
 
 
 class ListWorkteamsPaginator(Paginator):
@@ -2024,15 +2024,15 @@
     def paginate(
         self,
         *,
         SortBy: ListWorkteamsSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListWorkteamsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListWorkteamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListWorkteams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listworkteamspaginator)
         """
 
 
 class SearchPaginator(Paginator):
@@ -2047,12 +2047,12 @@
         Resource: ResourceTypeType,
         SearchExpression: SearchExpressionTypeDef = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
         CrossAccountFilterOption: CrossAccountFilterOptionType = ...,
         VisibilityConditions: Sequence[VisibilityConditionsTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[SearchResponsePaginatorTypeDef]:
+    ) -> _PageIterator[SearchResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.Search.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#searchpaginator)
         """
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/paginator.pyi` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -257,17 +257,17 @@
     UserProfileSortKeyType,
     WarmPoolResourceStatusType,
 )
 from .type_defs import (
     ListActionsResponseTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAliasesResponseTypeDef,
-    ListAppImageConfigsResponsePaginatorTypeDef,
+    ListAppImageConfigsResponseTypeDef,
     ListAppsResponseTypeDef,
-    ListArtifactsResponsePaginatorTypeDef,
+    ListArtifactsResponseTypeDef,
     ListAssociationsResponseTypeDef,
     ListAutoMLJobsResponseTypeDef,
     ListCandidatesForAutoMLJobResponseTypeDef,
     ListClusterNodesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListCodeRepositoriesOutputTypeDef,
     ListCompilationJobsResponseTypeDef,
@@ -284,19 +284,19 @@
     ListFeatureGroupsResponseTypeDef,
     ListFlowDefinitionsResponseTypeDef,
     ListHumanTaskUisResponseTypeDef,
     ListHyperParameterTuningJobsResponseTypeDef,
     ListImagesResponseTypeDef,
     ListImageVersionsResponseTypeDef,
     ListInferenceComponentsOutputTypeDef,
-    ListInferenceExperimentsResponsePaginatorTypeDef,
+    ListInferenceExperimentsResponseTypeDef,
     ListInferenceRecommendationsJobsResponseTypeDef,
     ListInferenceRecommendationsJobStepsResponseTypeDef,
     ListLabelingJobsForWorkteamResponseTypeDef,
-    ListLabelingJobsResponsePaginatorTypeDef,
+    ListLabelingJobsResponseTypeDef,
     ListLineageGroupsResponseTypeDef,
     ListModelBiasJobDefinitionsResponseTypeDef,
     ListModelCardExportJobsResponseTypeDef,
     ListModelCardsResponseTypeDef,
     ListModelCardVersionsResponseTypeDef,
     ListModelExplainabilityJobDefinitionsResponseTypeDef,
     ListModelMetadataResponseTypeDef,
@@ -323,20 +323,20 @@
     ListTagsOutputTypeDef,
     ListTrainingJobsForHyperParameterTuningJobResponseTypeDef,
     ListTrainingJobsResponseTypeDef,
     ListTransformJobsResponseTypeDef,
     ListTrialComponentsResponseTypeDef,
     ListTrialsResponseTypeDef,
     ListUserProfilesResponseTypeDef,
-    ListWorkforcesResponsePaginatorTypeDef,
-    ListWorkteamsResponsePaginatorTypeDef,
+    ListWorkforcesResponseTypeDef,
+    ListWorkteamsResponseTypeDef,
     ModelMetadataSearchExpressionTypeDef,
     PaginatorConfigTypeDef,
     SearchExpressionTypeDef,
-    SearchResponsePaginatorTypeDef,
+    SearchResponseTypeDef,
     TimestampTypeDef,
     VisibilityConditionsTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -500,15 +500,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: AppImageConfigSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListAppImageConfigsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListAppImageConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAppImageConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listappimageconfigspaginator)
         """
 
 class ListAppsPaginator(Paginator):
     """
@@ -543,15 +543,15 @@
         SourceUri: str = ...,
         ArtifactType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: Literal["CreationTime"] = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListArtifactsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListArtifactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listartifactspaginator)
         """
 
 class ListAssociationsPaginator(Paginator):
     """
@@ -1099,15 +1099,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         SortBy: SortInferenceExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListInferenceExperimentsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListInferenceExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceExperiments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listinferenceexperimentspaginator)
         """
 
 class ListInferenceRecommendationsJobStepsPaginator(Paginator):
     """
@@ -1168,15 +1168,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: LabelingJobStatusType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListLabelingJobsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListLabelingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListLabelingJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listlabelingjobspaginator)
         """
 
 class ListLabelingJobsForWorkteamPaginator(Paginator):
     """
@@ -1933,15 +1933,15 @@
     def paginate(
         self,
         *,
         SortBy: ListWorkforcesSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListWorkforcesResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListWorkforcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListWorkforces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listworkforcespaginator)
         """
 
 class ListWorkteamsPaginator(Paginator):
     """
@@ -1952,15 +1952,15 @@
     def paginate(
         self,
         *,
         SortBy: ListWorkteamsSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListWorkteamsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListWorkteamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListWorkteams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#listworkteamspaginator)
         """
 
 class SearchPaginator(Paginator):
     """
@@ -1974,12 +1974,12 @@
         Resource: ResourceTypeType,
         SearchExpression: SearchExpressionTypeDef = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
         CrossAccountFilterOption: CrossAccountFilterOptionType = ...,
         VisibilityConditions: Sequence[VisibilityConditionsTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[SearchResponsePaginatorTypeDef]:
+    ) -> _PageIterator[SearchResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.Search.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/paginators/#searchpaginator)
         """
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/type_defs.py` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -293,35 +293,39 @@
     "AgentVersionTypeDef",
     "AlarmTypeDef",
     "MetricDefinitionTypeDef",
     "AlgorithmStatusItemTypeDef",
     "AlgorithmSummaryTypeDef",
     "AnnotationConsolidationConfigTypeDef",
     "ResourceSpecTypeDef",
-    "AppSpecificationPaginatorTypeDef",
+    "AppSpecificationExtraOutputTypeDef",
+    "AppSpecificationOutputTypeDef",
     "AppSpecificationTypeDef",
     "ArtifactSourceTypeTypeDef",
     "AssociateTrialComponentRequestRequestTypeDef",
     "AsyncInferenceClientConfigTypeDef",
+    "AsyncInferenceNotificationConfigOutputTypeDef",
     "AsyncInferenceNotificationConfigTypeDef",
     "AthenaDatasetDefinitionTypeDef",
+    "AutoMLAlgorithmConfigOutputTypeDef",
     "AutoMLAlgorithmConfigTypeDef",
     "AutoMLCandidateStepTypeDef",
     "AutoMLContainerDefinitionTypeDef",
     "FinalAutoMLJobObjectiveMetricTypeDef",
     "AutoMLS3DataSourceTypeDef",
     "AutoMLDataSplitConfigTypeDef",
     "AutoMLJobArtifactsTypeDef",
     "AutoMLJobCompletionCriteriaTypeDef",
     "AutoMLJobObjectiveTypeDef",
     "AutoMLJobStepMetadataTypeDef",
     "AutoMLPartialFailureReasonTypeDef",
     "AutoMLOutputDataConfigTypeDef",
     "TabularResolvedAttributesTypeDef",
     "TextGenerationResolvedAttributesTypeDef",
+    "VpcConfigOutputTypeDef",
     "VpcConfigTypeDef",
     "AutoParameterTypeDef",
     "AutotuneTypeDef",
     "BatchDataCaptureConfigTypeDef",
     "BatchDescribeModelPackageErrorTypeDef",
     "BatchDescribeModelPackageInputRequestTypeDef",
     "BestObjectiveNotImprovingTypeDef",
@@ -334,40 +338,48 @@
     "GenerativeAiSettingsTypeDef",
     "IdentityProviderOAuthSettingTypeDef",
     "KendraSettingsTypeDef",
     "ModelRegisterSettingsTypeDef",
     "TimeSeriesForecastingSettingsTypeDef",
     "WorkspaceSettingsTypeDef",
     "CapacitySizeTypeDef",
+    "CaptureContentTypeHeaderOutputTypeDef",
     "CaptureContentTypeHeaderTypeDef",
     "CaptureOptionTypeDef",
-    "CategoricalParameterRangePaginatorTypeDef",
+    "CategoricalParameterOutputTypeDef",
+    "CategoricalParameterRangeExtraOutputTypeDef",
+    "CategoricalParameterRangeOutputTypeDef",
+    "CategoricalParameterRangeSpecificationOutputTypeDef",
     "CategoricalParameterRangeSpecificationTypeDef",
     "CategoricalParameterRangeTypeDef",
     "CategoricalParameterTypeDef",
     "ShuffleConfigTypeDef",
+    "ChannelSpecificationOutputTypeDef",
     "ChannelSpecificationTypeDef",
     "CheckpointConfigTypeDef",
     "ClarifyCheckStepMetadataTypeDef",
+    "ClarifyInferenceConfigOutputTypeDef",
     "ClarifyInferenceConfigTypeDef",
     "ClarifyShapBaselineConfigTypeDef",
     "ClarifyTextConfigTypeDef",
     "ClusterLifeCycleConfigTypeDef",
     "ClusterInstanceStatusDetailsTypeDef",
     "ClusterSummaryTypeDef",
-    "ContainerConfigPaginatorTypeDef",
+    "ContainerConfigExtraOutputTypeDef",
     "FileSystemConfigTypeDef",
+    "ContainerConfigOutputTypeDef",
     "ContainerConfigTypeDef",
     "CustomImageTypeDef",
     "GitConfigTypeDef",
     "CodeRepositoryTypeDef",
     "CognitoConfigTypeDef",
     "CognitoMemberDefinitionTypeDef",
     "VectorConfigTypeDef",
-    "CollectionConfigurationPaginatorTypeDef",
+    "CollectionConfigurationExtraOutputTypeDef",
+    "CollectionConfigurationOutputTypeDef",
     "CollectionConfigurationTypeDef",
     "CompilationJobSummaryTypeDef",
     "ConditionStepMetadataTypeDef",
     "MultiModelConfigTypeDef",
     "ContextSourceTypeDef",
     "ContinuousParameterRangeSpecificationTypeDef",
     "ContinuousParameterRangeTypeDef",
@@ -402,21 +414,20 @@
     "PipelineDefinitionS3LocationTypeDef",
     "CreatePresignedDomainUrlRequestRequestTypeDef",
     "CreatePresignedNotebookInstanceUrlInputRequestTypeDef",
     "ExperimentConfigTypeDef",
     "ProcessingStoppingConditionTypeDef",
     "OwnershipSettingsTypeDef",
     "SpaceSharingSettingsTypeDef",
-    "DebugRuleConfigurationTypeDef",
     "InfraCheckConfigTypeDef",
     "OutputDataConfigTypeDef",
     "ProfilerConfigTypeDef",
-    "ProfilerRuleConfigurationTypeDef",
     "RemoteDebugConfigTypeDef",
     "RetryStrategyTypeDef",
+    "SessionChainingConfigTypeDef",
     "TensorBoardOutputConfigTypeDef",
     "DataProcessingTypeDef",
     "ModelClientConfigTypeDef",
     "TransformOutputTypeDef",
     "TransformResourcesTypeDef",
     "TimestampTypeDef",
     "TrialComponentArtifactTypeDef",
@@ -428,22 +439,26 @@
     "NotificationConfigurationTypeDef",
     "EFSFileSystemConfigTypeDef",
     "EFSFileSystemTypeDef",
     "CustomPosixUserConfigTypeDef",
     "CustomizedMetricSpecificationTypeDef",
     "DataCaptureConfigSummaryTypeDef",
     "DataCatalogConfigTypeDef",
+    "DataQualityAppSpecificationOutputTypeDef",
     "MonitoringConstraintsResourceTypeDef",
     "MonitoringStatisticsResourceTypeDef",
     "EndpointInputTypeDef",
     "FileSystemDataSourceTypeDef",
-    "S3DataSourcePaginatorTypeDef",
+    "S3DataSourceExtraOutputTypeDef",
+    "S3DataSourceOutputTypeDef",
     "S3DataSourceTypeDef",
     "RedshiftDatasetDefinitionTypeDef",
-    "DebugRuleConfigurationPaginatorTypeDef",
+    "DebugRuleConfigurationExtraOutputTypeDef",
+    "DebugRuleConfigurationOutputTypeDef",
+    "DebugRuleConfigurationTypeDef",
     "DebugRuleEvaluationStatusTypeDef",
     "DefaultEbsStorageSettingsTypeDef",
     "DeleteActionRequestRequestTypeDef",
     "DeleteAlgorithmInputRequestTypeDef",
     "DeleteAppImageConfigRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
@@ -488,17 +503,18 @@
     "DeleteTrialComponentRequestRequestTypeDef",
     "DeleteTrialRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
     "DeleteWorkforceRequestRequestTypeDef",
     "DeleteWorkteamRequestRequestTypeDef",
     "DeployedImageTypeDef",
     "RealTimeInferenceRecommendationTypeDef",
-    "DeviceSelectionConfigTypeDef",
+    "DeviceSelectionConfigOutputTypeDef",
     "EdgeDeploymentConfigTypeDef",
     "EdgeDeploymentStatusTypeDef",
+    "DeviceSelectionConfigTypeDef",
     "DeregisterDevicesRequestRequestTypeDef",
     "DerivedInformationTypeDef",
     "DescribeActionRequestRequestTypeDef",
     "DescribeAlgorithmInputRequestTypeDef",
     "DescribeAppImageConfigRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeArtifactRequestRequestTypeDef",
@@ -507,14 +523,15 @@
     "DescribeAutoMLJobV2RequestRequestTypeDef",
     "DescribeClusterNodeRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeCodeRepositoryInputRequestTypeDef",
     "DescribeCompilationJobRequestRequestTypeDef",
     "ModelArtifactsTypeDef",
     "ModelDigestsTypeDef",
+    "NeoVpcConfigOutputTypeDef",
     "DescribeContextRequestRequestTypeDef",
     "DescribeDataQualityJobDefinitionRequestRequestTypeDef",
     "DescribeDeviceFleetRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "EdgeModelTypeDef",
     "DescribeDomainRequestRequestTypeDef",
     "DescribeEdgeDeploymentPlanRequestRequestTypeDef",
@@ -544,28 +561,32 @@
     "TrainingJobStatusCountersTypeDef",
     "DescribeImageRequestRequestTypeDef",
     "DescribeImageVersionRequestRequestTypeDef",
     "DescribeInferenceComponentInputRequestTypeDef",
     "InferenceComponentRuntimeConfigSummaryTypeDef",
     "DescribeInferenceExperimentRequestRequestTypeDef",
     "EndpointMetadataTypeDef",
+    "InferenceExperimentScheduleOutputTypeDef",
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     "DescribeLabelingJobRequestRequestTypeDef",
     "LabelCountersTypeDef",
     "LabelingJobOutputTypeDef",
     "DescribeLineageGroupRequestRequestTypeDef",
     "DescribeModelBiasJobDefinitionRequestRequestTypeDef",
+    "ModelBiasAppSpecificationOutputTypeDef",
     "DescribeModelCardExportJobRequestRequestTypeDef",
     "ModelCardExportArtifactsTypeDef",
     "DescribeModelCardRequestRequestTypeDef",
     "DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef",
+    "ModelExplainabilityAppSpecificationOutputTypeDef",
     "DescribeModelInputRequestTypeDef",
     "DescribeModelPackageGroupInputRequestTypeDef",
     "DescribeModelPackageInputRequestTypeDef",
     "DescribeModelQualityJobDefinitionRequestRequestTypeDef",
+    "ModelQualityAppSpecificationOutputTypeDef",
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     "MonitoringExecutionSummaryTypeDef",
     "DescribeNotebookInstanceInputRequestTypeDef",
     "DescribeNotebookInstanceLifecycleConfigInputRequestTypeDef",
     "DescribePipelineDefinitionForExecutionRequestRequestTypeDef",
     "DescribePipelineExecutionRequestRequestTypeDef",
     "PipelineExperimentConfigTypeDef",
@@ -575,14 +596,16 @@
     "ServiceCatalogProvisionedProductDetailsTypeDef",
     "DescribeSpaceRequestRequestTypeDef",
     "DescribeStudioLifecycleConfigRequestRequestTypeDef",
     "DescribeSubscribedWorkteamRequestRequestTypeDef",
     "SubscribedWorkteamTypeDef",
     "DescribeTrainingJobRequestRequestTypeDef",
     "MetricDataTypeDef",
+    "ProfilerConfigOutputTypeDef",
+    "ProfilerRuleConfigurationOutputTypeDef",
     "ProfilerRuleEvaluationStatusTypeDef",
     "SecondaryStatusTransitionTypeDef",
     "WarmPoolStatusTypeDef",
     "DescribeTransformJobRequestRequestTypeDef",
     "DescribeTrialComponentRequestRequestTypeDef",
     "TrialComponentMetricSummaryTypeDef",
     "TrialComponentSourceTypeDef",
@@ -594,14 +617,15 @@
     "ProductionVariantServerlessUpdateConfigTypeDef",
     "DeviceDeploymentSummaryTypeDef",
     "DeviceFleetSummaryTypeDef",
     "DeviceStatsTypeDef",
     "EdgeModelSummaryTypeDef",
     "DeviceTypeDef",
     "DisassociateTrialComponentRequestRequestTypeDef",
+    "DockerSettingsOutputTypeDef",
     "DockerSettingsTypeDef",
     "DomainDetailsTypeDef",
     "FileSourceTypeDef",
     "EMRStepMetadataTypeDef",
     "EbsStorageSettingsTypeDef",
     "EdgeDeploymentPlanSummaryTypeDef",
     "EdgeModelStatTypeDef",
@@ -627,36 +651,37 @@
     "HolidayConfigAttributesTypeDef",
     "HubContentInfoTypeDef",
     "HubInfoTypeDef",
     "HumanLoopActivationConditionsConfigTypeDef",
     "UiConfigTypeDef",
     "HumanTaskUiSummaryTypeDef",
     "HyperParameterTuningJobObjectiveTypeDef",
-    "VpcConfigPaginatorTypeDef",
+    "VpcConfigExtraOutputTypeDef",
     "HyperParameterTuningInstanceConfigTypeDef",
     "ResourceLimitsTypeDef",
     "HyperbandStrategyConfigTypeDef",
     "ParentHyperParameterTuningJobTypeDef",
     "IamIdentityTypeDef",
     "RepositoryAuthConfigTypeDef",
     "ImageTypeDef",
     "ImageVersionTypeDef",
     "InferenceComponentComputeResourceRequirementsTypeDef",
     "InferenceComponentContainerSpecificationTypeDef",
     "InferenceComponentStartupParametersTypeDef",
     "InferenceComponentSummaryTypeDef",
-    "InferenceExperimentSchedulePaginatorTypeDef",
+    "InferenceExperimentScheduleExtraOutputTypeDef",
     "RecommendationMetricsTypeDef",
     "InferenceRecommendationsJobTypeDef",
     "InstanceGroupTypeDef",
     "IntegerParameterRangeSpecificationTypeDef",
     "IntegerParameterRangeTypeDef",
     "KernelSpecTypeDef",
     "LabelCountersForWorkteamTypeDef",
-    "LabelingJobDataAttributesPaginatorTypeDef",
+    "LabelingJobDataAttributesExtraOutputTypeDef",
+    "LabelingJobDataAttributesOutputTypeDef",
     "LabelingJobDataAttributesTypeDef",
     "LabelingJobS3DataSourceTypeDef",
     "LabelingJobSnsDataSourceTypeDef",
     "LineageGroupSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
@@ -691,28 +716,30 @@
     "ListTagsInputRequestTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef",
     "TransformJobSummaryTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileDetailsTypeDef",
     "ListWorkforcesRequestRequestTypeDef",
     "ListWorkteamsRequestRequestTypeDef",
-    "OidcMemberDefinitionPaginatorTypeDef",
+    "OidcMemberDefinitionExtraOutputTypeDef",
+    "OidcMemberDefinitionOutputTypeDef",
     "OidcMemberDefinitionTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ModelAccessConfigTypeDef",
     "MonitoringGroundTruthS3InputTypeDef",
     "ModelDashboardEndpointTypeDef",
     "ModelDashboardIndicatorActionTypeDef",
     "RealTimeInferenceConfigTypeDef",
     "ModelInputTypeDef",
     "ModelLatencyThresholdTypeDef",
     "ModelMetadataFilterTypeDef",
     "ModelPackageStatusItemTypeDef",
     "ModelStepMetadataTypeDef",
-    "MonitoringAppSpecificationPaginatorTypeDef",
+    "MonitoringAppSpecificationExtraOutputTypeDef",
+    "MonitoringAppSpecificationOutputTypeDef",
     "MonitoringAppSpecificationTypeDef",
     "MonitoringClusterConfigTypeDef",
     "MonitoringCsvDatasetFormatTypeDef",
     "MonitoringJsonDatasetFormatTypeDef",
     "MonitoringS3OutputTypeDef",
     "ScheduleConfigTypeDef",
     "S3StorageConfigTypeDef",
@@ -734,36 +761,40 @@
     "TuningJobStepMetaDataTypeDef",
     "SelectiveExecutionResultTypeDef",
     "ProcessingClusterConfigTypeDef",
     "ProcessingFeatureStoreOutputTypeDef",
     "ProcessingS3InputTypeDef",
     "ProcessingS3OutputTypeDef",
     "ProductionVariantCoreDumpConfigTypeDef",
+    "ProfilerConfigExtraOutputTypeDef",
     "ProfilerConfigForUpdateTypeDef",
-    "ProfilerConfigPaginatorTypeDef",
+    "ProfilerRuleConfigurationTypeDef",
     "PropertyNameQueryTypeDef",
     "ProvisioningParameterTypeDef",
     "USDTypeDef",
     "PutModelPackageGroupPolicyInputRequestTypeDef",
     "VertexTypeDef",
     "RStudioServerProAppSettingsTypeDef",
     "RecommendationJobCompiledOutputConfigTypeDef",
+    "RecommendationJobPayloadConfigOutputTypeDef",
     "RecommendationJobPayloadConfigTypeDef",
     "RecommendationJobResourceLimitTypeDef",
+    "RecommendationJobVpcConfigOutputTypeDef",
     "RecommendationJobVpcConfigTypeDef",
     "RemoteDebugConfigForUpdateTypeDef",
     "RenderableTaskTypeDef",
     "RenderingErrorTypeDef",
     "ResourceConfigForUpdateTypeDef",
     "VisibilityConditionsTypeDef",
     "SelectedStepTypeDef",
     "SendPipelineExecutionStepFailureRequestRequestTypeDef",
     "ShadowModelVariantConfigTypeDef",
     "SharingSettingsTypeDef",
-    "SourceIpConfigPaginatorTypeDef",
+    "SourceIpConfigExtraOutputTypeDef",
+    "SourceIpConfigOutputTypeDef",
     "SpaceSharingSettingsSummaryTypeDef",
     "StairsTypeDef",
     "StartEdgeDeploymentStageRequestRequestTypeDef",
     "StartInferenceExperimentRequestRequestTypeDef",
     "StartMonitoringScheduleRequestRequestTypeDef",
     "StartNotebookInstanceInputRequestTypeDef",
     "StopAutoMLJobRequestRequestTypeDef",
@@ -776,15 +807,17 @@
     "StopMonitoringScheduleRequestRequestTypeDef",
     "StopNotebookInstanceInputRequestTypeDef",
     "StopPipelineExecutionRequestRequestTypeDef",
     "StopProcessingJobRequestRequestTypeDef",
     "StopTrainingJobRequestRequestTypeDef",
     "StopTransformJobRequestRequestTypeDef",
     "ThroughputConfigUpdateTypeDef",
+    "TimeSeriesConfigOutputTypeDef",
     "TimeSeriesConfigTypeDef",
+    "TimeSeriesTransformationsOutputTypeDef",
     "TimeSeriesTransformationsTypeDef",
     "TrainingRepositoryAuthConfigTypeDef",
     "TransformS3DataSourceTypeDef",
     "UpdateActionRequestRequestTypeDef",
     "UpdateArtifactRequestRequestTypeDef",
     "UpdateClusterSoftwareRequestRequestTypeDef",
     "UpdateContextRequestRequestTypeDef",
@@ -917,78 +950,102 @@
     "AddTagsOutputTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
     "CreateModelPackageGroupInputRequestTypeDef",
     "CreateStudioLifecycleConfigRequestRequestTypeDef",
     "ImportHubContentRequestRequestTypeDef",
     "ListTagsOutputTypeDef",
+    "AutoRollbackConfigOutputTypeDef",
     "AutoRollbackConfigTypeDef",
-    "HyperParameterAlgorithmSpecificationPaginatorTypeDef",
+    "HyperParameterAlgorithmSpecificationExtraOutputTypeDef",
+    "HyperParameterAlgorithmSpecificationOutputTypeDef",
     "HyperParameterAlgorithmSpecificationTypeDef",
     "AlgorithmStatusDetailsTypeDef",
     "ListAlgorithmsOutputTypeDef",
     "AppDetailsTypeDef",
     "CreateAppRequestRequestTypeDef",
     "DescribeAppResponseTypeDef",
     "RStudioServerProDomainSettingsForUpdateTypeDef",
     "RStudioServerProDomainSettingsTypeDef",
     "SpaceCodeEditorAppSettingsTypeDef",
     "TensorBoardAppSettingsTypeDef",
-    "ArtifactSourcePaginatorTypeDef",
+    "AppSpecificationUnionTypeDef",
+    "ArtifactSourceExtraOutputTypeDef",
+    "ArtifactSourceOutputTypeDef",
     "ArtifactSourceTypeDef",
+    "AsyncInferenceOutputConfigOutputTypeDef",
     "AsyncInferenceOutputConfigTypeDef",
+    "AutoMLCandidateGenerationConfigOutputTypeDef",
+    "CandidateGenerationConfigOutputTypeDef",
     "AutoMLCandidateGenerationConfigTypeDef",
     "CandidateGenerationConfigTypeDef",
     "AutoMLDataSourceTypeDef",
     "ImageClassificationJobConfigTypeDef",
     "TextClassificationJobConfigTypeDef",
     "ResolvedAttributesTypeDef",
     "AutoMLJobSummaryTypeDef",
     "AutoMLProblemTypeResolvedAttributesTypeDef",
+    "AutoMLSecurityConfigOutputTypeDef",
+    "LabelingJobResourceConfigOutputTypeDef",
+    "MonitoringNetworkConfigOutputTypeDef",
+    "NetworkConfigOutputTypeDef",
     "AutoMLSecurityConfigTypeDef",
     "LabelingJobResourceConfigTypeDef",
     "MonitoringNetworkConfigTypeDef",
     "NetworkConfigTypeDef",
     "BiasTypeDef",
     "DriftCheckModelDataQualityTypeDef",
     "DriftCheckModelQualityTypeDef",
     "ExplainabilityTypeDef",
     "ModelDataQualityTypeDef",
     "ModelQualityTypeDef",
     "CallbackStepMetadataTypeDef",
     "LambdaStepMetadataTypeDef",
     "SendPipelineExecutionStepSuccessRequestRequestTypeDef",
     "CandidatePropertiesTypeDef",
+    "CanvasAppSettingsOutputTypeDef",
     "CanvasAppSettingsTypeDef",
     "RollingUpdatePolicyTypeDef",
     "TrafficRoutingConfigTypeDef",
+    "InferenceExperimentDataStorageConfigOutputTypeDef",
     "InferenceExperimentDataStorageConfigTypeDef",
+    "DataCaptureConfigOutputTypeDef",
     "DataCaptureConfigTypeDef",
+    "EnvironmentParameterRangesOutputTypeDef",
     "EnvironmentParameterRangesTypeDef",
     "ClarifyShapConfigTypeDef",
     "ClusterInstanceGroupDetailsTypeDef",
     "ClusterInstanceGroupSpecificationTypeDef",
     "ClusterNodeDetailsTypeDef",
     "ClusterNodeSummaryTypeDef",
     "ListClustersResponseTypeDef",
-    "CodeEditorAppImageConfigPaginatorTypeDef",
-    "JupyterLabAppImageConfigPaginatorTypeDef",
+    "CodeEditorAppImageConfigExtraOutputTypeDef",
+    "JupyterLabAppImageConfigExtraOutputTypeDef",
+    "CodeEditorAppImageConfigOutputTypeDef",
+    "JupyterLabAppImageConfigOutputTypeDef",
     "CodeEditorAppImageConfigTypeDef",
     "JupyterLabAppImageConfigTypeDef",
+    "CodeEditorAppSettingsOutputTypeDef",
     "CodeEditorAppSettingsTypeDef",
+    "KernelGatewayAppSettingsOutputTypeDef",
     "KernelGatewayAppSettingsTypeDef",
+    "RSessionAppSettingsOutputTypeDef",
     "RSessionAppSettingsTypeDef",
     "CodeRepositorySummaryTypeDef",
     "CreateCodeRepositoryInputRequestTypeDef",
     "DescribeCodeRepositoryOutputTypeDef",
+    "JupyterLabAppSettingsOutputTypeDef",
     "JupyterLabAppSettingsTypeDef",
+    "JupyterServerAppSettingsOutputTypeDef",
     "JupyterServerAppSettingsTypeDef",
+    "SpaceJupyterLabAppSettingsOutputTypeDef",
     "SpaceJupyterLabAppSettingsTypeDef",
     "CollectionConfigTypeDef",
-    "DebugHookConfigPaginatorTypeDef",
+    "DebugHookConfigExtraOutputTypeDef",
+    "DebugHookConfigOutputTypeDef",
     "DebugHookConfigTypeDef",
     "ListCompilationJobsResponseTypeDef",
     "ContextSummaryTypeDef",
     "CreateContextRequestRequestTypeDef",
     "TuningJobCompletionCriteriaTypeDef",
     "CreateActionRequestRequestTypeDef",
     "CreateTrialRequestRequestTypeDef",
@@ -1074,28 +1131,32 @@
     "QueryFiltersTypeDef",
     "CreateTrialComponentRequestRequestTypeDef",
     "UpdateTrialComponentRequestRequestTypeDef",
     "CreateWorkforceRequestRequestTypeDef",
     "UpdateWorkforceRequestRequestTypeDef",
     "CustomFileSystemConfigTypeDef",
     "CustomFileSystemTypeDef",
+    "DataQualityAppSpecificationUnionTypeDef",
     "ModelBiasBaselineConfigTypeDef",
     "ModelExplainabilityBaselineConfigTypeDef",
     "ModelQualityBaselineConfigTypeDef",
     "DataQualityBaselineConfigTypeDef",
     "MonitoringBaselineConfigTypeDef",
-    "DataSourcePaginatorTypeDef",
+    "DataSourceExtraOutputTypeDef",
+    "DataSourceOutputTypeDef",
     "DataSourceTypeDef",
     "DatasetDefinitionTypeDef",
+    "DebugRuleConfigurationUnionTypeDef",
     "DefaultSpaceStorageSettingsTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "InferenceComponentContainerSpecificationSummaryTypeDef",
     "DeploymentRecommendationTypeDef",
-    "DeploymentStageTypeDef",
     "DeploymentStageStatusSummaryTypeDef",
+    "DeploymentStageTypeDef",
+    "NeoVpcConfigUnionTypeDef",
     "DescribeDeviceResponseTypeDef",
     "DescribeEdgePackagingJobResponseTypeDef",
     "DescribeEndpointInputEndpointDeletedWaitTypeDef",
     "DescribeEndpointInputEndpointInServiceWaitTypeDef",
     "DescribeImageRequestImageCreatedWaitTypeDef",
     "DescribeImageRequestImageDeletedWaitTypeDef",
     "DescribeImageRequestImageUpdatedWaitTypeDef",
@@ -1110,15 +1171,19 @@
     "ExperimentSummaryTypeDef",
     "FeatureGroupSummaryTypeDef",
     "DescribeFeatureMetadataResponseTypeDef",
     "FeatureMetadataTypeDef",
     "UpdateFeatureMetadataRequestRequestTypeDef",
     "DescribeHubContentResponseTypeDef",
     "DescribeHumanTaskUiResponseTypeDef",
+    "InferenceExperimentSummaryTypeDef",
+    "ModelBiasAppSpecificationUnionTypeDef",
     "DescribeModelCardExportJobResponseTypeDef",
+    "ModelExplainabilityAppSpecificationUnionTypeDef",
+    "ModelQualityAppSpecificationUnionTypeDef",
     "ListMonitoringExecutionsResponseTypeDef",
     "DescribeSubscribedWorkteamResponseTypeDef",
     "ListSubscribedWorkteamsResponseTypeDef",
     "TrainingJobSummaryTypeDef",
     "TrialSummaryTypeDef",
     "DesiredWeightAndCapacityTypeDef",
     "ListStageDevicesResponseTypeDef",
@@ -1145,35 +1210,41 @@
     "GetSearchSuggestionsResponseTypeDef",
     "UpdateCodeRepositoryInputRequestTypeDef",
     "ListHubContentVersionsResponseTypeDef",
     "ListHubContentsResponseTypeDef",
     "ListHubsResponseTypeDef",
     "HumanLoopActivationConfigTypeDef",
     "ListHumanTaskUisResponseTypeDef",
-    "NetworkConfigPaginatorTypeDef",
-    "HyperParameterTuningResourceConfigPaginatorTypeDef",
+    "NetworkConfigExtraOutputTypeDef",
+    "VpcConfigUnionTypeDef",
+    "HyperParameterTuningResourceConfigExtraOutputTypeDef",
+    "HyperParameterTuningResourceConfigOutputTypeDef",
     "HyperParameterTuningResourceConfigTypeDef",
     "HyperParameterTuningJobSummaryTypeDef",
     "HyperParameterTuningJobStrategyConfigTypeDef",
-    "HyperParameterTuningJobWarmStartConfigPaginatorTypeDef",
+    "HyperParameterTuningJobWarmStartConfigExtraOutputTypeDef",
+    "HyperParameterTuningJobWarmStartConfigOutputTypeDef",
     "HyperParameterTuningJobWarmStartConfigTypeDef",
     "UserContextTypeDef",
     "ImageConfigTypeDef",
     "ListImagesResponseTypeDef",
     "ListImageVersionsResponseTypeDef",
     "InferenceComponentSpecificationTypeDef",
     "ListInferenceComponentsOutputTypeDef",
-    "InferenceExperimentSummaryPaginatorTypeDef",
     "ListInferenceRecommendationsJobsResponseTypeDef",
-    "ResourceConfigPaginatorTypeDef",
+    "ResourceConfigExtraOutputTypeDef",
+    "ResourceConfigOutputTypeDef",
     "ResourceConfigTypeDef",
+    "ParameterRangeOutputTypeDef",
     "ParameterRangeTypeDef",
-    "ParameterRangesPaginatorTypeDef",
+    "ParameterRangesExtraOutputTypeDef",
+    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
-    "KernelGatewayImageConfigPaginatorTypeDef",
+    "KernelGatewayImageConfigExtraOutputTypeDef",
+    "KernelGatewayImageConfigOutputTypeDef",
     "KernelGatewayImageConfigTypeDef",
     "LabelingJobForWorkteamSummaryTypeDef",
     "LabelingJobDataSourceTypeDef",
     "ListLineageGroupsResponseTypeDef",
     "ListActionsRequestListActionsPaginateTypeDef",
     "ListAlgorithmsInputListAlgorithmsPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
@@ -1264,112 +1335,145 @@
     "ListPipelinesResponseTypeDef",
     "ListProcessingJobsResponseTypeDef",
     "ListProjectsOutputTypeDef",
     "ListResourceCatalogsResponseTypeDef",
     "ListStudioLifecycleConfigsResponseTypeDef",
     "ListTransformJobsResponseTypeDef",
     "ListUserProfilesResponseTypeDef",
-    "MemberDefinitionPaginatorTypeDef",
+    "MemberDefinitionExtraOutputTypeDef",
+    "MemberDefinitionOutputTypeDef",
     "MemberDefinitionTypeDef",
     "MetricSpecificationTypeDef",
     "S3ModelDataSourceTypeDef",
+    "TextGenerationJobConfigOutputTypeDef",
     "TextGenerationJobConfigTypeDef",
     "MonitoringAlertActionsTypeDef",
     "ModelInfrastructureConfigTypeDef",
+    "RecommendationJobStoppingConditionsOutputTypeDef",
     "RecommendationJobStoppingConditionsTypeDef",
     "ModelMetadataSearchExpressionTypeDef",
     "ModelPackageStatusDetailsTypeDef",
     "MonitoringResourcesTypeDef",
-    "MonitoringDatasetFormatPaginatorTypeDef",
+    "MonitoringDatasetFormatExtraOutputTypeDef",
+    "MonitoringDatasetFormatOutputTypeDef",
     "MonitoringDatasetFormatTypeDef",
     "MonitoringOutputTypeDef",
     "OfflineStoreConfigTypeDef",
     "OnlineStoreConfigTypeDef",
     "OnlineStoreConfigUpdateTypeDef",
     "OutputConfigTypeDef",
     "PendingProductionVariantSummaryTypeDef",
     "ProductionVariantSummaryTypeDef",
     "ProcessingResourcesTypeDef",
     "ProcessingOutputTypeDef",
     "ProductionVariantTypeDef",
+    "ProfilerConfigUnionTypeDef",
+    "ProfilerRuleConfigurationUnionTypeDef",
     "SuggestionQueryTypeDef",
-    "ServiceCatalogProvisioningDetailsPaginatorTypeDef",
+    "ServiceCatalogProvisioningDetailsExtraOutputTypeDef",
+    "ServiceCatalogProvisioningDetailsOutputTypeDef",
     "ServiceCatalogProvisioningDetailsTypeDef",
     "ServiceCatalogProvisioningUpdateDetailsTypeDef",
     "PublicWorkforceTaskPriceTypeDef",
     "QueryLineageResponseTypeDef",
     "RecommendationJobOutputConfigTypeDef",
+    "RecommendationJobContainerConfigOutputTypeDef",
     "RecommendationJobContainerConfigTypeDef",
     "RenderUiTemplateRequestRequestTypeDef",
     "RenderUiTemplateResponseTypeDef",
-    "UpdateTrainingJobRequestRequestTypeDef",
     "SearchRequestRequestTypeDef",
+    "SelectiveExecutionConfigExtraOutputTypeDef",
+    "SelectiveExecutionConfigOutputTypeDef",
     "SelectiveExecutionConfigTypeDef",
+    "ShadowModeConfigOutputTypeDef",
     "ShadowModeConfigTypeDef",
+    "SourceIpConfigUnionTypeDef",
+    "TrafficPatternOutputTypeDef",
     "TrafficPatternTypeDef",
+    "TimeSeriesForecastingJobConfigOutputTypeDef",
     "TimeSeriesForecastingJobConfigTypeDef",
     "TrainingImageConfigTypeDef",
     "TransformDataSourceTypeDef",
-    "WorkforcePaginatorTypeDef",
     "WorkforceTypeDef",
     "ListActionsResponseTypeDef",
     "ListAppsResponseTypeDef",
     "DomainSettingsForUpdateTypeDef",
+    "DomainSettingsOutputTypeDef",
     "DomainSettingsTypeDef",
-    "ArtifactSummaryPaginatorTypeDef",
     "ArtifactSummaryTypeDef",
+    "ArtifactSourceUnionTypeDef",
     "CreateArtifactRequestRequestTypeDef",
     "DeleteArtifactRequestRequestTypeDef",
+    "AsyncInferenceConfigOutputTypeDef",
     "AsyncInferenceConfigTypeDef",
+    "TabularJobConfigOutputTypeDef",
     "TabularJobConfigTypeDef",
     "AutoMLChannelTypeDef",
     "AutoMLJobChannelTypeDef",
     "ListAutoMLJobsResponseTypeDef",
     "AutoMLResolvedAttributesTypeDef",
+    "AutoMLJobConfigOutputTypeDef",
+    "LabelingJobAlgorithmsConfigOutputTypeDef",
     "AutoMLJobConfigTypeDef",
+    "AutoMLSecurityConfigUnionTypeDef",
     "LabelingJobAlgorithmsConfigTypeDef",
+    "MonitoringNetworkConfigUnionTypeDef",
     "ModelMetricsTypeDef",
     "PipelineExecutionStepMetadataTypeDef",
     "AutoMLCandidateTypeDef",
     "BlueGreenUpdatePolicyTypeDef",
+    "InferenceExperimentDataStorageConfigUnionTypeDef",
+    "DataCaptureConfigUnionTypeDef",
+    "EndpointInputConfigurationOutputTypeDef",
     "EndpointInputConfigurationTypeDef",
+    "ClarifyExplainerConfigOutputTypeDef",
     "ClarifyExplainerConfigTypeDef",
     "DescribeClusterResponseTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "DescribeClusterNodeResponseTypeDef",
     "ListClusterNodesResponseTypeDef",
+    "CodeEditorAppImageConfigUnionTypeDef",
+    "JupyterLabAppImageConfigUnionTypeDef",
     "ListCodeRepositoriesOutputTypeDef",
     "FeatureDefinitionTypeDef",
+    "DebugHookConfigUnionTypeDef",
     "ListContextsResponseTypeDef",
-    "InferenceExperimentSummaryTypeDef",
+    "InferenceExperimentScheduleUnionTypeDef",
     "QueryLineageRequestRequestTypeDef",
-    "ChannelPaginatorTypeDef",
+    "ChannelExtraOutputTypeDef",
+    "ChannelOutputTypeDef",
     "ChannelTypeDef",
     "ProcessingInputTypeDef",
+    "DefaultSpaceSettingsOutputTypeDef",
     "DefaultSpaceSettingsTypeDef",
+    "UserSettingsOutputTypeDef",
     "UserSettingsTypeDef",
     "InferenceComponentSpecificationSummaryTypeDef",
+    "DescribeEdgeDeploymentPlanResponseTypeDef",
     "CreateEdgeDeploymentPlanRequestRequestTypeDef",
     "CreateEdgeDeploymentStageRequestRequestTypeDef",
-    "DescribeEdgeDeploymentPlanResponseTypeDef",
     "ListExperimentsResponseTypeDef",
     "ListFeatureGroupsResponseTypeDef",
+    "ListInferenceExperimentsResponseTypeDef",
     "ListTrainingJobsResponseTypeDef",
     "ListTrialsResponseTypeDef",
     "UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef",
     "ListDevicesResponseTypeDef",
     "DriftCheckBaselinesTypeDef",
+    "SpaceSettingsOutputTypeDef",
     "SpaceSettingsSummaryTypeDef",
     "SpaceSettingsTypeDef",
     "InferenceRecommendationTypeDef",
     "RecommendationJobInferenceBenchmarkTypeDef",
     "SearchExpressionTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobResponseTypeDef",
+    "NetworkConfigUnionTypeDef",
     "ListHyperParameterTuningJobsResponseTypeDef",
+    "HyperParameterTuningJobWarmStartConfigUnionTypeDef",
     "AssociationSummaryTypeDef",
     "DescribeActionResponseTypeDef",
     "DescribeArtifactResponseTypeDef",
     "DescribeContextResponseTypeDef",
     "DescribeExperimentResponseTypeDef",
     "DescribeLineageGroupResponseTypeDef",
     "DescribeModelCardResponseTypeDef",
@@ -1382,214 +1486,265 @@
     "ModelDashboardModelCardTypeDef",
     "ModelPackageGroupTypeDef",
     "PipelineTypeDef",
     "TrialComponentSimpleSummaryTypeDef",
     "TrialComponentSummaryTypeDef",
     "CreateInferenceComponentInputRequestTypeDef",
     "UpdateInferenceComponentInputRequestTypeDef",
-    "ListInferenceExperimentsResponsePaginatorTypeDef",
+    "ResourceConfigUnionTypeDef",
+    "HyperParameterSpecificationOutputTypeDef",
     "HyperParameterSpecificationTypeDef",
-    "HyperParameterTuningJobConfigPaginatorTypeDef",
+    "HyperParameterTuningJobConfigExtraOutputTypeDef",
+    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
-    "AppImageConfigDetailsPaginatorTypeDef",
     "AppImageConfigDetailsTypeDef",
-    "CreateAppImageConfigRequestRequestTypeDef",
     "DescribeAppImageConfigResponseTypeDef",
+    "CreateAppImageConfigRequestRequestTypeDef",
+    "KernelGatewayImageConfigUnionTypeDef",
     "UpdateAppImageConfigRequestRequestTypeDef",
     "ListLabelingJobsForWorkteamResponseTypeDef",
-    "LabelingJobInputConfigPaginatorTypeDef",
+    "LabelingJobInputConfigExtraOutputTypeDef",
+    "LabelingJobInputConfigOutputTypeDef",
     "LabelingJobInputConfigTypeDef",
-    "WorkteamPaginatorTypeDef",
-    "CreateWorkteamRequestRequestTypeDef",
-    "UpdateWorkteamRequestRequestTypeDef",
     "WorkteamTypeDef",
+    "MemberDefinitionUnionTypeDef",
     "TargetTrackingScalingPolicyConfigurationTypeDef",
     "ModelDataSourceTypeDef",
     "MonitoringAlertSummaryTypeDef",
     "ModelVariantConfigSummaryTypeDef",
     "ModelVariantConfigTypeDef",
+    "RecommendationJobStoppingConditionsUnionTypeDef",
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     "ListModelMetadataRequestRequestTypeDef",
-    "BatchTransformInputPaginatorTypeDef",
+    "BatchTransformInputExtraOutputTypeDef",
+    "BatchTransformInputOutputTypeDef",
     "BatchTransformInputTypeDef",
-    "MonitoringOutputConfigPaginatorTypeDef",
+    "MonitoringOutputConfigExtraOutputTypeDef",
+    "MonitoringOutputConfigOutputTypeDef",
     "MonitoringOutputConfigTypeDef",
     "CreateCompilationJobRequestRequestTypeDef",
     "DescribeCompilationJobResponseTypeDef",
     "PendingDeploymentSummaryTypeDef",
-    "ProcessingOutputConfigPaginatorTypeDef",
+    "ProcessingOutputConfigExtraOutputTypeDef",
+    "ProcessingOutputConfigOutputTypeDef",
     "ProcessingOutputConfigTypeDef",
+    "UpdateTrainingJobRequestRequestTypeDef",
     "GetSearchSuggestionsRequestRequestTypeDef",
-    "ProjectPaginatorTypeDef",
-    "CreateProjectInputRequestTypeDef",
     "DescribeProjectOutputTypeDef",
     "ProjectTypeDef",
+    "CreateProjectInputRequestTypeDef",
+    "ServiceCatalogProvisioningDetailsUnionTypeDef",
     "UpdateProjectInputRequestTypeDef",
+    "HumanLoopConfigOutputTypeDef",
     "HumanLoopConfigTypeDef",
+    "HumanTaskConfigOutputTypeDef",
     "HumanTaskConfigTypeDef",
     "DescribePipelineExecutionResponseTypeDef",
     "PipelineExecutionTypeDef",
+    "SelectiveExecutionConfigUnionTypeDef",
     "StartPipelineExecutionRequestRequestTypeDef",
-    "AlgorithmSpecificationPaginatorTypeDef",
+    "ShadowModeConfigUnionTypeDef",
+    "AlgorithmSpecificationExtraOutputTypeDef",
+    "AlgorithmSpecificationOutputTypeDef",
     "AlgorithmSpecificationTypeDef",
     "TransformInputTypeDef",
-    "ListWorkforcesResponsePaginatorTypeDef",
     "DescribeWorkforceResponseTypeDef",
     "ListWorkforcesResponseTypeDef",
     "UpdateWorkforceResponseTypeDef",
-    "ListArtifactsResponsePaginatorTypeDef",
+    "DomainSettingsUnionTypeDef",
     "ListArtifactsResponseTypeDef",
+    "AsyncInferenceConfigUnionTypeDef",
+    "AutoMLProblemTypeConfigOutputTypeDef",
     "AutoMLProblemTypeConfigTypeDef",
+    "AutoMLJobConfigUnionTypeDef",
     "CreateAutoMLJobRequestRequestTypeDef",
+    "LabelingJobAlgorithmsConfigUnionTypeDef",
     "PipelineExecutionStepTypeDef",
     "DescribeAutoMLJobResponseTypeDef",
     "ListCandidatesForAutoMLJobResponseTypeDef",
+    "DeploymentConfigOutputTypeDef",
     "DeploymentConfigTypeDef",
+    "RecommendationJobInputConfigOutputTypeDef",
     "RecommendationJobInputConfigTypeDef",
+    "ExplainerConfigOutputTypeDef",
     "ExplainerConfigTypeDef",
     "CreateFeatureGroupRequestRequestTypeDef",
     "DescribeFeatureGroupResponseTypeDef",
     "FeatureGroupTypeDef",
     "UpdateFeatureGroupRequestRequestTypeDef",
-    "ListInferenceExperimentsResponseTypeDef",
-    "HyperParameterTrainingJobDefinitionPaginatorTypeDef",
+    "HyperParameterTrainingJobDefinitionExtraOutputTypeDef",
+    "HyperParameterTrainingJobDefinitionOutputTypeDef",
+    "TrainingJobDefinitionOutputTypeDef",
+    "ChannelUnionTypeDef",
     "HyperParameterTrainingJobDefinitionTypeDef",
     "TrainingJobDefinitionTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "CreateUserProfileRequestRequestTypeDef",
+    "DefaultSpaceSettingsUnionTypeDef",
     "DescribeDomainResponseTypeDef",
     "DescribeUserProfileResponseTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "CreateUserProfileRequestRequestTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
+    "UserSettingsUnionTypeDef",
     "DescribeInferenceComponentOutputTypeDef",
+    "DescribeSpaceResponseTypeDef",
     "SpaceDetailsTypeDef",
     "CreateSpaceRequestRequestTypeDef",
-    "DescribeSpaceResponseTypeDef",
+    "SpaceSettingsUnionTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
     "InferenceRecommendationsJobStepTypeDef",
     "SearchRequestSearchPaginateTypeDef",
     "ListAssociationsResponseTypeDef",
     "TrialTypeDef",
     "ListTrialComponentsResponseTypeDef",
+    "TrainingSpecificationOutputTypeDef",
     "TrainingSpecificationTypeDef",
-    "ListAppImageConfigsResponsePaginatorTypeDef",
+    "HyperParameterTuningJobConfigUnionTypeDef",
     "ListAppImageConfigsResponseTypeDef",
-    "LabelingJobSummaryPaginatorTypeDef",
     "LabelingJobSummaryTypeDef",
-    "ListWorkteamsResponsePaginatorTypeDef",
+    "LabelingJobInputConfigUnionTypeDef",
     "DescribeWorkteamResponseTypeDef",
     "ListWorkteamsResponseTypeDef",
     "UpdateWorkteamResponseTypeDef",
+    "CreateWorkteamRequestRequestTypeDef",
+    "UpdateWorkteamRequestRequestTypeDef",
     "ScalingPolicyTypeDef",
-    "ContainerDefinitionPaginatorTypeDef",
+    "ContainerDefinitionExtraOutputTypeDef",
+    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
+    "ModelPackageContainerDefinitionExtraOutputTypeDef",
+    "ModelPackageContainerDefinitionOutputTypeDef",
     "ModelPackageContainerDefinitionTypeDef",
     "SourceAlgorithmTypeDef",
     "ListMonitoringAlertsResponseTypeDef",
     "DescribeInferenceExperimentResponseTypeDef",
     "CreateInferenceExperimentRequestRequestTypeDef",
     "StopInferenceExperimentRequestRequestTypeDef",
     "UpdateInferenceExperimentRequestRequestTypeDef",
-    "MonitoringInputPaginatorTypeDef",
+    "MonitoringInputExtraOutputTypeDef",
+    "DataQualityJobInputOutputTypeDef",
+    "ModelBiasJobInputOutputTypeDef",
+    "ModelExplainabilityJobInputOutputTypeDef",
+    "ModelQualityJobInputOutputTypeDef",
+    "MonitoringInputOutputTypeDef",
     "DataQualityJobInputTypeDef",
     "ModelBiasJobInputTypeDef",
     "ModelExplainabilityJobInputTypeDef",
     "ModelQualityJobInputTypeDef",
     "MonitoringInputTypeDef",
-    "ProcessingJobPaginatorTypeDef",
-    "CreateProcessingJobRequestRequestTypeDef",
+    "MonitoringOutputConfigUnionTypeDef",
     "DescribeProcessingJobResponseTypeDef",
     "ProcessingJobTypeDef",
-    "CreateFlowDefinitionRequestRequestTypeDef",
+    "CreateProcessingJobRequestRequestTypeDef",
+    "ProcessingOutputConfigUnionTypeDef",
     "DescribeFlowDefinitionResponseTypeDef",
-    "CreateLabelingJobRequestRequestTypeDef",
+    "CreateFlowDefinitionRequestRequestTypeDef",
+    "HumanLoopConfigUnionTypeDef",
     "DescribeLabelingJobResponseTypeDef",
-    "TrainingJobPaginatorTypeDef",
-    "CreateTrainingJobRequestRequestTypeDef",
+    "CreateLabelingJobRequestRequestTypeDef",
+    "HumanTaskConfigUnionTypeDef",
     "DescribeTrainingJobResponseTypeDef",
     "TrainingJobTypeDef",
+    "AlgorithmSpecificationUnionTypeDef",
     "CreateTransformJobRequestRequestTypeDef",
     "DescribeTransformJobResponseTypeDef",
-    "TransformJobDefinitionPaginatorTypeDef",
+    "TransformJobDefinitionExtraOutputTypeDef",
+    "TransformJobDefinitionOutputTypeDef",
     "TransformJobDefinitionTypeDef",
     "TransformJobTypeDef",
-    "CreateAutoMLJobV2RequestRequestTypeDef",
     "DescribeAutoMLJobV2ResponseTypeDef",
+    "AutoMLProblemTypeConfigUnionTypeDef",
+    "CreateAutoMLJobV2RequestRequestTypeDef",
     "ListPipelineExecutionStepsResponseTypeDef",
     "CreateEndpointInputRequestTypeDef",
+    "DeploymentConfigUnionTypeDef",
     "UpdateEndpointInputRequestTypeDef",
-    "CreateInferenceRecommendationsJobRequestRequestTypeDef",
     "DescribeInferenceRecommendationsJobResponseTypeDef",
-    "CreateEndpointConfigInputRequestTypeDef",
+    "CreateInferenceRecommendationsJobRequestRequestTypeDef",
+    "RecommendationJobInputConfigUnionTypeDef",
     "DescribeEndpointConfigOutputTypeDef",
     "DescribeEndpointOutputTypeDef",
-    "HyperParameterTuningJobSearchEntityPaginatorTypeDef",
-    "CreateHyperParameterTuningJobRequestRequestTypeDef",
+    "CreateEndpointConfigInputRequestTypeDef",
+    "ExplainerConfigUnionTypeDef",
     "DescribeHyperParameterTuningJobResponseTypeDef",
     "HyperParameterTuningJobSearchEntityTypeDef",
+    "CreateTrainingJobRequestRequestTypeDef",
+    "HyperParameterTrainingJobDefinitionUnionTypeDef",
     "ListSpacesResponseTypeDef",
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
-    "ListLabelingJobsResponsePaginatorTypeDef",
+    "TrainingSpecificationUnionTypeDef",
     "ListLabelingJobsResponseTypeDef",
     "DynamicScalingConfigurationTypeDef",
-    "ModelPaginatorTypeDef",
-    "CreateModelInputRequestTypeDef",
     "DescribeModelOutputTypeDef",
     "ModelTypeDef",
-    "AdditionalInferenceSpecificationDefinitionPaginatorTypeDef",
+    "ContainerDefinitionUnionTypeDef",
+    "AdditionalInferenceSpecificationDefinitionExtraOutputTypeDef",
+    "InferenceSpecificationExtraOutputTypeDef",
+    "AdditionalInferenceSpecificationDefinitionOutputTypeDef",
+    "InferenceSpecificationOutputTypeDef",
     "AdditionalInferenceSpecificationDefinitionTypeDef",
     "InferenceSpecificationTypeDef",
-    "SourceAlgorithmSpecificationPaginatorTypeDef",
+    "SourceAlgorithmSpecificationExtraOutputTypeDef",
+    "SourceAlgorithmSpecificationOutputTypeDef",
     "SourceAlgorithmSpecificationTypeDef",
-    "MonitoringJobDefinitionPaginatorTypeDef",
-    "CreateDataQualityJobDefinitionRequestRequestTypeDef",
+    "MonitoringJobDefinitionExtraOutputTypeDef",
     "DescribeDataQualityJobDefinitionResponseTypeDef",
-    "CreateModelBiasJobDefinitionRequestRequestTypeDef",
     "DescribeModelBiasJobDefinitionResponseTypeDef",
-    "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
     "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
-    "CreateModelQualityJobDefinitionRequestRequestTypeDef",
     "DescribeModelQualityJobDefinitionResponseTypeDef",
+    "MonitoringJobDefinitionOutputTypeDef",
+    "CreateDataQualityJobDefinitionRequestRequestTypeDef",
+    "DataQualityJobInputUnionTypeDef",
+    "CreateModelBiasJobDefinitionRequestRequestTypeDef",
+    "ModelBiasJobInputUnionTypeDef",
+    "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
+    "ModelExplainabilityJobInputUnionTypeDef",
+    "CreateModelQualityJobDefinitionRequestRequestTypeDef",
+    "ModelQualityJobInputUnionTypeDef",
     "MonitoringJobDefinitionTypeDef",
-    "ModelPackageValidationProfilePaginatorTypeDef",
+    "ModelPackageValidationProfileExtraOutputTypeDef",
+    "AlgorithmValidationProfileOutputTypeDef",
+    "ModelPackageValidationProfileOutputTypeDef",
     "AlgorithmValidationProfileTypeDef",
     "ModelPackageValidationProfileTypeDef",
-    "TrialComponentSourceDetailPaginatorTypeDef",
     "TrialComponentSourceDetailTypeDef",
+    "CreateHyperParameterTuningJobRequestRequestTypeDef",
     "GetScalingConfigurationRecommendationResponseTypeDef",
+    "CreateModelInputRequestTypeDef",
     "BatchDescribeModelPackageSummaryTypeDef",
-    "UpdateModelPackageInputRequestTypeDef",
-    "MonitoringScheduleConfigPaginatorTypeDef",
+    "AdditionalInferenceSpecificationDefinitionUnionTypeDef",
+    "InferenceSpecificationUnionTypeDef",
+    "SourceAlgorithmSpecificationUnionTypeDef",
+    "MonitoringScheduleConfigExtraOutputTypeDef",
+    "MonitoringScheduleConfigOutputTypeDef",
     "MonitoringScheduleConfigTypeDef",
-    "ModelPackageValidationSpecificationPaginatorTypeDef",
+    "ModelPackageValidationSpecificationExtraOutputTypeDef",
+    "AlgorithmValidationSpecificationOutputTypeDef",
+    "ModelPackageValidationSpecificationOutputTypeDef",
     "AlgorithmValidationSpecificationTypeDef",
     "ModelPackageValidationSpecificationTypeDef",
-    "TrialComponentPaginatorTypeDef",
     "TrialComponentTypeDef",
     "BatchDescribeModelPackageOutputTypeDef",
-    "ModelDashboardMonitoringSchedulePaginatorTypeDef",
-    "MonitoringSchedulePaginatorTypeDef",
-    "CreateMonitoringScheduleRequestRequestTypeDef",
+    "UpdateModelPackageInputRequestTypeDef",
     "DescribeMonitoringScheduleResponseTypeDef",
     "ModelDashboardMonitoringScheduleTypeDef",
     "MonitoringScheduleTypeDef",
+    "CreateMonitoringScheduleRequestRequestTypeDef",
+    "MonitoringScheduleConfigUnionTypeDef",
     "UpdateMonitoringScheduleRequestRequestTypeDef",
-    "ModelPackagePaginatorTypeDef",
-    "CreateAlgorithmInputRequestTypeDef",
     "DescribeAlgorithmOutputTypeDef",
-    "CreateModelPackageInputRequestTypeDef",
     "DescribeModelPackageOutputTypeDef",
     "ModelPackageTypeDef",
-    "ModelDashboardModelPaginatorTypeDef",
-    "EndpointPaginatorTypeDef",
+    "AlgorithmValidationSpecificationUnionTypeDef",
+    "CreateAlgorithmInputRequestTypeDef",
+    "CreateModelPackageInputRequestTypeDef",
+    "ModelPackageValidationSpecificationUnionTypeDef",
     "ModelDashboardModelTypeDef",
     "EndpointTypeDef",
-    "SearchRecordPaginatorTypeDef",
     "SearchRecordTypeDef",
-    "SearchResponsePaginatorTypeDef",
     "SearchResponseTypeDef",
 )
 
 ActionSourceTypeDef = TypedDict(
     "ActionSourceTypeDef",
     {
         "SourceUri": str,
@@ -1680,16 +1835,24 @@
         "SageMakerImageArn": NotRequired[str],
         "SageMakerImageVersionArn": NotRequired[str],
         "SageMakerImageVersionAlias": NotRequired[str],
         "InstanceType": NotRequired[AppInstanceTypeType],
         "LifecycleConfigArn": NotRequired[str],
     },
 )
-AppSpecificationPaginatorTypeDef = TypedDict(
-    "AppSpecificationPaginatorTypeDef",
+AppSpecificationExtraOutputTypeDef = TypedDict(
+    "AppSpecificationExtraOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+    },
+)
+AppSpecificationOutputTypeDef = TypedDict(
+    "AppSpecificationOutputTypeDef",
     {
         "ImageUri": str,
         "ContainerEntrypoint": NotRequired[List[str]],
         "ContainerArguments": NotRequired[List[str]],
     },
 )
 AppSpecificationTypeDef = TypedDict(
@@ -1716,14 +1879,22 @@
 )
 AsyncInferenceClientConfigTypeDef = TypedDict(
     "AsyncInferenceClientConfigTypeDef",
     {
         "MaxConcurrentInvocationsPerInstance": NotRequired[int],
     },
 )
+AsyncInferenceNotificationConfigOutputTypeDef = TypedDict(
+    "AsyncInferenceNotificationConfigOutputTypeDef",
+    {
+        "SuccessTopic": NotRequired[str],
+        "ErrorTopic": NotRequired[str],
+        "IncludeInferenceResponseIn": NotRequired[List[AsyncNotificationTopicTypesType]],
+    },
+)
 AsyncInferenceNotificationConfigTypeDef = TypedDict(
     "AsyncInferenceNotificationConfigTypeDef",
     {
         "SuccessTopic": NotRequired[str],
         "ErrorTopic": NotRequired[str],
         "IncludeInferenceResponseIn": NotRequired[Sequence[AsyncNotificationTopicTypesType]],
     },
@@ -1737,14 +1908,20 @@
         "OutputS3Uri": str,
         "OutputFormat": AthenaResultFormatType,
         "WorkGroup": NotRequired[str],
         "KmsKeyId": NotRequired[str],
         "OutputCompression": NotRequired[AthenaResultCompressionTypeType],
     },
 )
+AutoMLAlgorithmConfigOutputTypeDef = TypedDict(
+    "AutoMLAlgorithmConfigOutputTypeDef",
+    {
+        "AutoMLAlgorithms": List[AutoMLAlgorithmType],
+    },
+)
 AutoMLAlgorithmConfigTypeDef = TypedDict(
     "AutoMLAlgorithmConfigTypeDef",
     {
         "AutoMLAlgorithms": Sequence[AutoMLAlgorithmType],
     },
 )
 AutoMLCandidateStepTypeDef = TypedDict(
@@ -1833,14 +2010,21 @@
 )
 TextGenerationResolvedAttributesTypeDef = TypedDict(
     "TextGenerationResolvedAttributesTypeDef",
     {
         "BaseModelName": NotRequired[str],
     },
 )
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
+    },
+)
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
@@ -1972,34 +2156,61 @@
 CapacitySizeTypeDef = TypedDict(
     "CapacitySizeTypeDef",
     {
         "Type": CapacitySizeTypeType,
         "Value": int,
     },
 )
+CaptureContentTypeHeaderOutputTypeDef = TypedDict(
+    "CaptureContentTypeHeaderOutputTypeDef",
+    {
+        "CsvContentTypes": NotRequired[List[str]],
+        "JsonContentTypes": NotRequired[List[str]],
+    },
+)
 CaptureContentTypeHeaderTypeDef = TypedDict(
     "CaptureContentTypeHeaderTypeDef",
     {
         "CsvContentTypes": NotRequired[Sequence[str]],
         "JsonContentTypes": NotRequired[Sequence[str]],
     },
 )
 CaptureOptionTypeDef = TypedDict(
     "CaptureOptionTypeDef",
     {
         "CaptureMode": CaptureModeType,
     },
 )
-CategoricalParameterRangePaginatorTypeDef = TypedDict(
-    "CategoricalParameterRangePaginatorTypeDef",
+CategoricalParameterOutputTypeDef = TypedDict(
+    "CategoricalParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Value": List[str],
+    },
+)
+CategoricalParameterRangeExtraOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeExtraOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[str],
+    },
+)
+CategoricalParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeOutputTypeDef",
     {
         "Name": str,
         "Values": List[str],
     },
 )
+CategoricalParameterRangeSpecificationOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeSpecificationOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+)
 CategoricalParameterRangeSpecificationTypeDef = TypedDict(
     "CategoricalParameterRangeSpecificationTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 CategoricalParameterRangeTypeDef = TypedDict(
@@ -2018,14 +2229,25 @@
 )
 ShuffleConfigTypeDef = TypedDict(
     "ShuffleConfigTypeDef",
     {
         "Seed": int,
     },
 )
+ChannelSpecificationOutputTypeDef = TypedDict(
+    "ChannelSpecificationOutputTypeDef",
+    {
+        "Name": str,
+        "SupportedContentTypes": List[str],
+        "SupportedInputModes": List[TrainingInputModeType],
+        "Description": NotRequired[str],
+        "IsRequired": NotRequired[bool],
+        "SupportedCompressionTypes": NotRequired[List[CompressionTypeType]],
+    },
+)
 ChannelSpecificationTypeDef = TypedDict(
     "ChannelSpecificationTypeDef",
     {
         "Name": str,
         "SupportedContentTypes": Sequence[str],
         "SupportedInputModes": Sequence[TrainingInputModeType],
         "Description": NotRequired[str],
@@ -2049,14 +2271,30 @@
         "ModelPackageGroupName": NotRequired[str],
         "ViolationReport": NotRequired[str],
         "CheckJobArn": NotRequired[str],
         "SkipCheck": NotRequired[bool],
         "RegisterNewBaseline": NotRequired[bool],
     },
 )
+ClarifyInferenceConfigOutputTypeDef = TypedDict(
+    "ClarifyInferenceConfigOutputTypeDef",
+    {
+        "FeaturesAttribute": NotRequired[str],
+        "ContentTemplate": NotRequired[str],
+        "MaxRecordCount": NotRequired[int],
+        "MaxPayloadInMB": NotRequired[int],
+        "ProbabilityIndex": NotRequired[int],
+        "LabelIndex": NotRequired[int],
+        "ProbabilityAttribute": NotRequired[str],
+        "LabelAttribute": NotRequired[str],
+        "LabelHeaders": NotRequired[List[str]],
+        "FeatureHeaders": NotRequired[List[str]],
+        "FeatureTypes": NotRequired[List[ClarifyFeatureTypeType]],
+    },
+)
 ClarifyInferenceConfigTypeDef = TypedDict(
     "ClarifyInferenceConfigTypeDef",
     {
         "FeaturesAttribute": NotRequired[str],
         "ContentTemplate": NotRequired[str],
         "MaxRecordCount": NotRequired[int],
         "MaxPayloadInMB": NotRequired[int],
@@ -2103,30 +2341,38 @@
     {
         "ClusterArn": str,
         "ClusterName": str,
         "CreationTime": datetime,
         "ClusterStatus": ClusterStatusType,
     },
 )
-ContainerConfigPaginatorTypeDef = TypedDict(
-    "ContainerConfigPaginatorTypeDef",
+ContainerConfigExtraOutputTypeDef = TypedDict(
+    "ContainerConfigExtraOutputTypeDef",
     {
         "ContainerArguments": NotRequired[List[str]],
         "ContainerEntrypoint": NotRequired[List[str]],
         "ContainerEnvironmentVariables": NotRequired[Dict[str, str]],
     },
 )
 FileSystemConfigTypeDef = TypedDict(
     "FileSystemConfigTypeDef",
     {
         "MountPath": NotRequired[str],
         "DefaultUid": NotRequired[int],
         "DefaultGid": NotRequired[int],
     },
 )
+ContainerConfigOutputTypeDef = TypedDict(
+    "ContainerConfigOutputTypeDef",
+    {
+        "ContainerArguments": NotRequired[List[str]],
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerEnvironmentVariables": NotRequired[Dict[str, str]],
+    },
+)
 ContainerConfigTypeDef = TypedDict(
     "ContainerConfigTypeDef",
     {
         "ContainerArguments": NotRequired[Sequence[str]],
         "ContainerEntrypoint": NotRequired[Sequence[str]],
         "ContainerEnvironmentVariables": NotRequired[Mapping[str, str]],
     },
@@ -2170,16 +2416,23 @@
 )
 VectorConfigTypeDef = TypedDict(
     "VectorConfigTypeDef",
     {
         "Dimension": int,
     },
 )
-CollectionConfigurationPaginatorTypeDef = TypedDict(
-    "CollectionConfigurationPaginatorTypeDef",
+CollectionConfigurationExtraOutputTypeDef = TypedDict(
+    "CollectionConfigurationExtraOutputTypeDef",
+    {
+        "CollectionName": NotRequired[str],
+        "CollectionParameters": NotRequired[Dict[str, str]],
+    },
+)
+CollectionConfigurationOutputTypeDef = TypedDict(
+    "CollectionConfigurationOutputTypeDef",
     {
         "CollectionName": NotRequired[str],
         "CollectionParameters": NotRequired[Dict[str, str]],
     },
 )
 CollectionConfigurationTypeDef = TypedDict(
     "CollectionConfigurationTypeDef",
@@ -2502,26 +2755,14 @@
 )
 SpaceSharingSettingsTypeDef = TypedDict(
     "SpaceSharingSettingsTypeDef",
     {
         "SharingType": SharingTypeType,
     },
 )
-DebugRuleConfigurationTypeDef = TypedDict(
-    "DebugRuleConfigurationTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-        "LocalPath": NotRequired[str],
-        "S3OutputPath": NotRequired[str],
-        "InstanceType": NotRequired[ProcessingInstanceTypeType],
-        "VolumeSizeInGB": NotRequired[int],
-        "RuleParameters": NotRequired[Mapping[str, str]],
-    },
-)
 InfraCheckConfigTypeDef = TypedDict(
     "InfraCheckConfigTypeDef",
     {
         "EnableInfraCheck": NotRequired[bool],
     },
 )
 OutputDataConfigTypeDef = TypedDict(
@@ -2537,38 +2778,32 @@
     {
         "S3OutputPath": NotRequired[str],
         "ProfilingIntervalInMilliseconds": NotRequired[int],
         "ProfilingParameters": NotRequired[Mapping[str, str]],
         "DisableProfiler": NotRequired[bool],
     },
 )
-ProfilerRuleConfigurationTypeDef = TypedDict(
-    "ProfilerRuleConfigurationTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-        "LocalPath": NotRequired[str],
-        "S3OutputPath": NotRequired[str],
-        "InstanceType": NotRequired[ProcessingInstanceTypeType],
-        "VolumeSizeInGB": NotRequired[int],
-        "RuleParameters": NotRequired[Mapping[str, str]],
-    },
-)
 RemoteDebugConfigTypeDef = TypedDict(
     "RemoteDebugConfigTypeDef",
     {
         "EnableRemoteDebug": NotRequired[bool],
     },
 )
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "MaximumRetryAttempts": int,
     },
 )
+SessionChainingConfigTypeDef = TypedDict(
+    "SessionChainingConfigTypeDef",
+    {
+        "EnableSessionTagChaining": NotRequired[bool],
+    },
+)
 TensorBoardOutputConfigTypeDef = TypedDict(
     "TensorBoardOutputConfigTypeDef",
     {
         "S3OutputPath": str,
         "LocalPath": NotRequired[str],
     },
 )
@@ -2701,14 +2936,25 @@
     "DataCatalogConfigTypeDef",
     {
         "TableName": str,
         "Catalog": str,
         "Database": str,
     },
 )
+DataQualityAppSpecificationOutputTypeDef = TypedDict(
+    "DataQualityAppSpecificationOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+        "RecordPreprocessorSourceUri": NotRequired[str],
+        "PostAnalyticsProcessorSourceUri": NotRequired[str],
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
 MonitoringConstraintsResourceTypeDef = TypedDict(
     "MonitoringConstraintsResourceTypeDef",
     {
         "S3Uri": NotRequired[str],
     },
 )
 MonitoringStatisticsResourceTypeDef = TypedDict(
@@ -2738,16 +2984,26 @@
     {
         "FileSystemId": str,
         "FileSystemAccessMode": FileSystemAccessModeType,
         "FileSystemType": FileSystemTypeType,
         "DirectoryPath": str,
     },
 )
-S3DataSourcePaginatorTypeDef = TypedDict(
-    "S3DataSourcePaginatorTypeDef",
+S3DataSourceExtraOutputTypeDef = TypedDict(
+    "S3DataSourceExtraOutputTypeDef",
+    {
+        "S3DataType": S3DataTypeType,
+        "S3Uri": str,
+        "S3DataDistributionType": NotRequired[S3DataDistributionType],
+        "AttributeNames": NotRequired[List[str]],
+        "InstanceGroupNames": NotRequired[List[str]],
+    },
+)
+S3DataSourceOutputTypeDef = TypedDict(
+    "S3DataSourceOutputTypeDef",
     {
         "S3DataType": S3DataTypeType,
         "S3Uri": str,
         "S3DataDistributionType": NotRequired[S3DataDistributionType],
         "AttributeNames": NotRequired[List[str]],
         "InstanceGroupNames": NotRequired[List[str]],
     },
@@ -2772,26 +3028,50 @@
         "ClusterRoleArn": str,
         "OutputS3Uri": str,
         "OutputFormat": RedshiftResultFormatType,
         "KmsKeyId": NotRequired[str],
         "OutputCompression": NotRequired[RedshiftResultCompressionTypeType],
     },
 )
-DebugRuleConfigurationPaginatorTypeDef = TypedDict(
-    "DebugRuleConfigurationPaginatorTypeDef",
+DebugRuleConfigurationExtraOutputTypeDef = TypedDict(
+    "DebugRuleConfigurationExtraOutputTypeDef",
     {
         "RuleConfigurationName": str,
         "RuleEvaluatorImage": str,
         "LocalPath": NotRequired[str],
         "S3OutputPath": NotRequired[str],
         "InstanceType": NotRequired[ProcessingInstanceTypeType],
         "VolumeSizeInGB": NotRequired[int],
         "RuleParameters": NotRequired[Dict[str, str]],
     },
 )
+DebugRuleConfigurationOutputTypeDef = TypedDict(
+    "DebugRuleConfigurationOutputTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+        "LocalPath": NotRequired[str],
+        "S3OutputPath": NotRequired[str],
+        "InstanceType": NotRequired[ProcessingInstanceTypeType],
+        "VolumeSizeInGB": NotRequired[int],
+        "RuleParameters": NotRequired[Dict[str, str]],
+    },
+)
+DebugRuleConfigurationTypeDef = TypedDict(
+    "DebugRuleConfigurationTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+        "LocalPath": NotRequired[str],
+        "S3OutputPath": NotRequired[str],
+        "InstanceType": NotRequired[ProcessingInstanceTypeType],
+        "VolumeSizeInGB": NotRequired[int],
+        "RuleParameters": NotRequired[Mapping[str, str]],
+    },
+)
 DebugRuleEvaluationStatusTypeDef = TypedDict(
     "DebugRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": NotRequired[str],
         "RuleEvaluationJobArn": NotRequired[str],
         "RuleEvaluationStatus": NotRequired[RuleEvaluationStatusType],
         "StatusDetails": NotRequired[str],
@@ -3120,20 +3400,20 @@
     "RealTimeInferenceRecommendationTypeDef",
     {
         "RecommendationId": str,
         "InstanceType": ProductionVariantInstanceTypeType,
         "Environment": NotRequired[Dict[str, str]],
     },
 )
-DeviceSelectionConfigTypeDef = TypedDict(
-    "DeviceSelectionConfigTypeDef",
+DeviceSelectionConfigOutputTypeDef = TypedDict(
+    "DeviceSelectionConfigOutputTypeDef",
     {
         "DeviceSubsetType": DeviceSubsetTypeType,
         "Percentage": NotRequired[int],
-        "DeviceNames": NotRequired[Sequence[str]],
+        "DeviceNames": NotRequired[List[str]],
         "DeviceNameContains": NotRequired[str],
     },
 )
 EdgeDeploymentConfigTypeDef = TypedDict(
     "EdgeDeploymentConfigTypeDef",
     {
         "FailureHandlingPolicy": FailureHandlingPolicyType,
@@ -3146,14 +3426,23 @@
         "EdgeDeploymentSuccessInStage": int,
         "EdgeDeploymentPendingInStage": int,
         "EdgeDeploymentFailedInStage": int,
         "EdgeDeploymentStatusMessage": NotRequired[str],
         "EdgeDeploymentStageStartTime": NotRequired[datetime],
     },
 )
+DeviceSelectionConfigTypeDef = TypedDict(
+    "DeviceSelectionConfigTypeDef",
+    {
+        "DeviceSubsetType": DeviceSubsetTypeType,
+        "Percentage": NotRequired[int],
+        "DeviceNames": NotRequired[Sequence[str]],
+        "DeviceNameContains": NotRequired[str],
+    },
+)
 DeregisterDevicesRequestRequestTypeDef = TypedDict(
     "DeregisterDevicesRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
         "DeviceNames": Sequence[str],
     },
 )
@@ -3248,14 +3537,21 @@
 )
 ModelDigestsTypeDef = TypedDict(
     "ModelDigestsTypeDef",
     {
         "ArtifactDigest": NotRequired[str],
     },
 )
+NeoVpcConfigOutputTypeDef = TypedDict(
+    "NeoVpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
+    },
+)
 DescribeContextRequestRequestTypeDef = TypedDict(
     "DescribeContextRequestRequestTypeDef",
     {
         "ContextName": str,
     },
 )
 DescribeDataQualityJobDefinitionRequestRequestTypeDef = TypedDict(
@@ -3507,14 +3803,21 @@
     {
         "EndpointName": str,
         "EndpointConfigName": NotRequired[str],
         "EndpointStatus": NotRequired[EndpointStatusType],
         "FailureReason": NotRequired[str],
     },
 )
+InferenceExperimentScheduleOutputTypeDef = TypedDict(
+    "InferenceExperimentScheduleOutputTypeDef",
+    {
+        "StartTime": NotRequired[datetime],
+        "EndTime": NotRequired[datetime],
+    },
+)
 DescribeInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 DescribeLabelingJobRequestRequestTypeDef = TypedDict(
@@ -3548,14 +3851,22 @@
 )
 DescribeModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelBiasJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
+ModelBiasAppSpecificationOutputTypeDef = TypedDict(
+    "ModelBiasAppSpecificationOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ConfigUri": str,
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
 DescribeModelCardExportJobRequestRequestTypeDef = TypedDict(
     "DescribeModelCardExportJobRequestRequestTypeDef",
     {
         "ModelCardExportJobArn": str,
     },
 )
 ModelCardExportArtifactsTypeDef = TypedDict(
@@ -3573,14 +3884,22 @@
 )
 DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
+ModelExplainabilityAppSpecificationOutputTypeDef = TypedDict(
+    "ModelExplainabilityAppSpecificationOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ConfigUri": str,
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
 DescribeModelInputRequestTypeDef = TypedDict(
     "DescribeModelInputRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 DescribeModelPackageGroupInputRequestTypeDef = TypedDict(
@@ -3597,14 +3916,26 @@
 )
 DescribeModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
+ModelQualityAppSpecificationOutputTypeDef = TypedDict(
+    "ModelQualityAppSpecificationOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+        "RecordPreprocessorSourceUri": NotRequired[str],
+        "PostAnalyticsProcessorSourceUri": NotRequired[str],
+        "ProblemType": NotRequired[MonitoringProblemTypeType],
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
 DescribeMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
     },
 )
 MonitoringExecutionSummaryTypeDef = TypedDict(
@@ -3717,14 +4048,35 @@
     "MetricDataTypeDef",
     {
         "MetricName": NotRequired[str],
         "Value": NotRequired[float],
         "Timestamp": NotRequired[datetime],
     },
 )
+ProfilerConfigOutputTypeDef = TypedDict(
+    "ProfilerConfigOutputTypeDef",
+    {
+        "S3OutputPath": NotRequired[str],
+        "ProfilingIntervalInMilliseconds": NotRequired[int],
+        "ProfilingParameters": NotRequired[Dict[str, str]],
+        "DisableProfiler": NotRequired[bool],
+    },
+)
+ProfilerRuleConfigurationOutputTypeDef = TypedDict(
+    "ProfilerRuleConfigurationOutputTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+        "LocalPath": NotRequired[str],
+        "S3OutputPath": NotRequired[str],
+        "InstanceType": NotRequired[ProcessingInstanceTypeType],
+        "VolumeSizeInGB": NotRequired[int],
+        "RuleParameters": NotRequired[Dict[str, str]],
+    },
+)
 ProfilerRuleEvaluationStatusTypeDef = TypedDict(
     "ProfilerRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": NotRequired[str],
         "RuleEvaluationJobArn": NotRequired[str],
         "RuleEvaluationStatus": NotRequired[RuleEvaluationStatusType],
         "StatusDetails": NotRequired[str],
@@ -3870,14 +4222,21 @@
 DisassociateTrialComponentRequestRequestTypeDef = TypedDict(
     "DisassociateTrialComponentRequestRequestTypeDef",
     {
         "TrialComponentName": str,
         "TrialName": str,
     },
 )
+DockerSettingsOutputTypeDef = TypedDict(
+    "DockerSettingsOutputTypeDef",
+    {
+        "EnableDockerAccess": NotRequired[FeatureStatusType],
+        "VpcOnlyTrustedAccounts": NotRequired[List[str]],
+    },
+)
 DockerSettingsTypeDef = TypedDict(
     "DockerSettingsTypeDef",
     {
         "EnableDockerAccess": NotRequired[FeatureStatusType],
         "VpcOnlyTrustedAccounts": NotRequired[Sequence[str]],
     },
 )
@@ -4142,16 +4501,16 @@
 HyperParameterTuningJobObjectiveTypeDef = TypedDict(
     "HyperParameterTuningJobObjectiveTypeDef",
     {
         "Type": HyperParameterTuningJobObjectiveTypeType,
         "MetricName": str,
     },
 )
-VpcConfigPaginatorTypeDef = TypedDict(
-    "VpcConfigPaginatorTypeDef",
+VpcConfigExtraOutputTypeDef = TypedDict(
+    "VpcConfigExtraOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "Subnets": List[str],
     },
 )
 HyperParameterTuningInstanceConfigTypeDef = TypedDict(
     "HyperParameterTuningInstanceConfigTypeDef",
@@ -4254,16 +4613,16 @@
         "EndpointArn": str,
         "EndpointName": str,
         "VariantName": str,
         "LastModifiedTime": datetime,
         "InferenceComponentStatus": NotRequired[InferenceComponentStatusType],
     },
 )
-InferenceExperimentSchedulePaginatorTypeDef = TypedDict(
-    "InferenceExperimentSchedulePaginatorTypeDef",
+InferenceExperimentScheduleExtraOutputTypeDef = TypedDict(
+    "InferenceExperimentScheduleExtraOutputTypeDef",
     {
         "StartTime": NotRequired[datetime],
         "EndTime": NotRequired[datetime],
     },
 )
 RecommendationMetricsTypeDef = TypedDict(
     "RecommendationMetricsTypeDef",
@@ -4330,16 +4689,22 @@
     "LabelCountersForWorkteamTypeDef",
     {
         "HumanLabeled": NotRequired[int],
         "PendingHuman": NotRequired[int],
         "Total": NotRequired[int],
     },
 )
-LabelingJobDataAttributesPaginatorTypeDef = TypedDict(
-    "LabelingJobDataAttributesPaginatorTypeDef",
+LabelingJobDataAttributesExtraOutputTypeDef = TypedDict(
+    "LabelingJobDataAttributesExtraOutputTypeDef",
+    {
+        "ContentClassifiers": NotRequired[List[ContentClassifierType]],
+    },
+)
+LabelingJobDataAttributesOutputTypeDef = TypedDict(
+    "LabelingJobDataAttributesOutputTypeDef",
     {
         "ContentClassifiers": NotRequired[List[ContentClassifierType]],
     },
 )
 LabelingJobDataAttributesTypeDef = TypedDict(
     "LabelingJobDataAttributesTypeDef",
     {
@@ -4752,16 +5117,22 @@
         "SortBy": NotRequired[ListWorkteamsSortByOptionsType],
         "SortOrder": NotRequired[SortOrderType],
         "NameContains": NotRequired[str],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
 )
-OidcMemberDefinitionPaginatorTypeDef = TypedDict(
-    "OidcMemberDefinitionPaginatorTypeDef",
+OidcMemberDefinitionExtraOutputTypeDef = TypedDict(
+    "OidcMemberDefinitionExtraOutputTypeDef",
+    {
+        "Groups": NotRequired[List[str]],
+    },
+)
+OidcMemberDefinitionOutputTypeDef = TypedDict(
+    "OidcMemberDefinitionOutputTypeDef",
     {
         "Groups": NotRequired[List[str]],
     },
 )
 OidcMemberDefinitionTypeDef = TypedDict(
     "OidcMemberDefinitionTypeDef",
     {
@@ -4839,16 +5210,26 @@
 )
 ModelStepMetadataTypeDef = TypedDict(
     "ModelStepMetadataTypeDef",
     {
         "Arn": NotRequired[str],
     },
 )
-MonitoringAppSpecificationPaginatorTypeDef = TypedDict(
-    "MonitoringAppSpecificationPaginatorTypeDef",
+MonitoringAppSpecificationExtraOutputTypeDef = TypedDict(
+    "MonitoringAppSpecificationExtraOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+        "RecordPreprocessorSourceUri": NotRequired[str],
+        "PostAnalyticsProcessorSourceUri": NotRequired[str],
+    },
+)
+MonitoringAppSpecificationOutputTypeDef = TypedDict(
+    "MonitoringAppSpecificationOutputTypeDef",
     {
         "ImageUri": str,
         "ContainerEntrypoint": NotRequired[List[str]],
         "ContainerArguments": NotRequired[List[str]],
         "RecordPreprocessorSourceUri": NotRequired[str],
         "PostAnalyticsProcessorSourceUri": NotRequired[str],
     },
@@ -5072,30 +5453,42 @@
 ProductionVariantCoreDumpConfigTypeDef = TypedDict(
     "ProductionVariantCoreDumpConfigTypeDef",
     {
         "DestinationS3Uri": str,
         "KmsKeyId": NotRequired[str],
     },
 )
+ProfilerConfigExtraOutputTypeDef = TypedDict(
+    "ProfilerConfigExtraOutputTypeDef",
+    {
+        "S3OutputPath": NotRequired[str],
+        "ProfilingIntervalInMilliseconds": NotRequired[int],
+        "ProfilingParameters": NotRequired[Dict[str, str]],
+        "DisableProfiler": NotRequired[bool],
+    },
+)
 ProfilerConfigForUpdateTypeDef = TypedDict(
     "ProfilerConfigForUpdateTypeDef",
     {
         "S3OutputPath": NotRequired[str],
         "ProfilingIntervalInMilliseconds": NotRequired[int],
         "ProfilingParameters": NotRequired[Mapping[str, str]],
         "DisableProfiler": NotRequired[bool],
     },
 )
-ProfilerConfigPaginatorTypeDef = TypedDict(
-    "ProfilerConfigPaginatorTypeDef",
+ProfilerRuleConfigurationTypeDef = TypedDict(
+    "ProfilerRuleConfigurationTypeDef",
     {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+        "LocalPath": NotRequired[str],
         "S3OutputPath": NotRequired[str],
-        "ProfilingIntervalInMilliseconds": NotRequired[int],
-        "ProfilingParameters": NotRequired[Dict[str, str]],
-        "DisableProfiler": NotRequired[bool],
+        "InstanceType": NotRequired[ProcessingInstanceTypeType],
+        "VolumeSizeInGB": NotRequired[int],
+        "RuleParameters": NotRequired[Mapping[str, str]],
     },
 )
 PropertyNameQueryTypeDef = TypedDict(
     "PropertyNameQueryTypeDef",
     {
         "PropertyNameHint": str,
     },
@@ -5139,28 +5532,42 @@
 )
 RecommendationJobCompiledOutputConfigTypeDef = TypedDict(
     "RecommendationJobCompiledOutputConfigTypeDef",
     {
         "S3OutputUri": NotRequired[str],
     },
 )
+RecommendationJobPayloadConfigOutputTypeDef = TypedDict(
+    "RecommendationJobPayloadConfigOutputTypeDef",
+    {
+        "SamplePayloadUrl": NotRequired[str],
+        "SupportedContentTypes": NotRequired[List[str]],
+    },
+)
 RecommendationJobPayloadConfigTypeDef = TypedDict(
     "RecommendationJobPayloadConfigTypeDef",
     {
         "SamplePayloadUrl": NotRequired[str],
         "SupportedContentTypes": NotRequired[Sequence[str]],
     },
 )
 RecommendationJobResourceLimitTypeDef = TypedDict(
     "RecommendationJobResourceLimitTypeDef",
     {
         "MaxNumberOfTests": NotRequired[int],
         "MaxParallelOfTests": NotRequired[int],
     },
 )
+RecommendationJobVpcConfigOutputTypeDef = TypedDict(
+    "RecommendationJobVpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
+    },
+)
 RecommendationJobVpcConfigTypeDef = TypedDict(
     "RecommendationJobVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
@@ -5221,16 +5628,22 @@
     "SharingSettingsTypeDef",
     {
         "NotebookOutputOption": NotRequired[NotebookOutputOptionType],
         "S3OutputPath": NotRequired[str],
         "S3KmsKeyId": NotRequired[str],
     },
 )
-SourceIpConfigPaginatorTypeDef = TypedDict(
-    "SourceIpConfigPaginatorTypeDef",
+SourceIpConfigExtraOutputTypeDef = TypedDict(
+    "SourceIpConfigExtraOutputTypeDef",
+    {
+        "Cidrs": List[str],
+    },
+)
+SourceIpConfigOutputTypeDef = TypedDict(
+    "SourceIpConfigOutputTypeDef",
     {
         "Cidrs": List[str],
     },
 )
 SpaceSharingSettingsSummaryTypeDef = TypedDict(
     "SpaceSharingSettingsSummaryTypeDef",
     {
@@ -5354,23 +5767,39 @@
     "ThroughputConfigUpdateTypeDef",
     {
         "ThroughputMode": NotRequired[ThroughputModeType],
         "ProvisionedReadCapacityUnits": NotRequired[int],
         "ProvisionedWriteCapacityUnits": NotRequired[int],
     },
 )
+TimeSeriesConfigOutputTypeDef = TypedDict(
+    "TimeSeriesConfigOutputTypeDef",
+    {
+        "TargetAttributeName": str,
+        "TimestampAttributeName": str,
+        "ItemIdentifierAttributeName": str,
+        "GroupingAttributeNames": NotRequired[List[str]],
+    },
+)
 TimeSeriesConfigTypeDef = TypedDict(
     "TimeSeriesConfigTypeDef",
     {
         "TargetAttributeName": str,
         "TimestampAttributeName": str,
         "ItemIdentifierAttributeName": str,
         "GroupingAttributeNames": NotRequired[Sequence[str]],
     },
 )
+TimeSeriesTransformationsOutputTypeDef = TypedDict(
+    "TimeSeriesTransformationsOutputTypeDef",
+    {
+        "Filling": NotRequired[Dict[str, Dict[FillingTypeType, str]]],
+        "Aggregation": NotRequired[Dict[str, AggregationTransformationValueType]],
+    },
+)
 TimeSeriesTransformationsTypeDef = TypedDict(
     "TimeSeriesTransformationsTypeDef",
     {
         "Filling": NotRequired[Mapping[str, Mapping[FillingTypeType, str]]],
         "Aggregation": NotRequired[Mapping[str, AggregationTransformationValueType]],
     },
 )
@@ -6084,16 +6513,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "SageMakerImageVersionAliases": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PutModelPackageGroupPolicyOutputTypeDef = TypedDict(
     "PutModelPackageGroupPolicyOutputTypeDef",
     {
         "ModelPackageGroupArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6425,26 +6854,41 @@
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 ListTagsOutputTypeDef = TypedDict(
     "ListTagsOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+AutoRollbackConfigOutputTypeDef = TypedDict(
+    "AutoRollbackConfigOutputTypeDef",
+    {
+        "Alarms": NotRequired[List[AlarmTypeDef]],
     },
 )
 AutoRollbackConfigTypeDef = TypedDict(
     "AutoRollbackConfigTypeDef",
     {
         "Alarms": NotRequired[Sequence[AlarmTypeDef]],
     },
 )
-HyperParameterAlgorithmSpecificationPaginatorTypeDef = TypedDict(
-    "HyperParameterAlgorithmSpecificationPaginatorTypeDef",
+HyperParameterAlgorithmSpecificationExtraOutputTypeDef = TypedDict(
+    "HyperParameterAlgorithmSpecificationExtraOutputTypeDef",
+    {
+        "TrainingInputMode": TrainingInputModeType,
+        "TrainingImage": NotRequired[str],
+        "AlgorithmName": NotRequired[str],
+        "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
+    },
+)
+HyperParameterAlgorithmSpecificationOutputTypeDef = TypedDict(
+    "HyperParameterAlgorithmSpecificationOutputTypeDef",
     {
         "TrainingInputMode": TrainingInputModeType,
         "TrainingImage": NotRequired[str],
         "AlgorithmName": NotRequired[str],
         "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
     },
 )
@@ -6464,16 +6908,16 @@
         "ImageScanStatuses": NotRequired[List[AlgorithmStatusItemTypeDef]],
     },
 )
 ListAlgorithmsOutputTypeDef = TypedDict(
     "ListAlgorithmsOutputTypeDef",
     {
         "AlgorithmSummaryList": List[AlgorithmSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AppDetailsTypeDef = TypedDict(
     "AppDetailsTypeDef",
     {
         "DomainId": NotRequired[str],
         "UserProfileName": NotRequired[str],
@@ -6541,37 +6985,67 @@
 )
 TensorBoardAppSettingsTypeDef = TypedDict(
     "TensorBoardAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
     },
 )
-ArtifactSourcePaginatorTypeDef = TypedDict(
-    "ArtifactSourcePaginatorTypeDef",
+AppSpecificationUnionTypeDef = Union[AppSpecificationTypeDef, AppSpecificationExtraOutputTypeDef]
+ArtifactSourceExtraOutputTypeDef = TypedDict(
+    "ArtifactSourceExtraOutputTypeDef",
+    {
+        "SourceUri": str,
+        "SourceTypes": NotRequired[List[ArtifactSourceTypeTypeDef]],
+    },
+)
+ArtifactSourceOutputTypeDef = TypedDict(
+    "ArtifactSourceOutputTypeDef",
     {
         "SourceUri": str,
         "SourceTypes": NotRequired[List[ArtifactSourceTypeTypeDef]],
     },
 )
 ArtifactSourceTypeDef = TypedDict(
     "ArtifactSourceTypeDef",
     {
         "SourceUri": str,
         "SourceTypes": NotRequired[Sequence[ArtifactSourceTypeTypeDef]],
     },
 )
+AsyncInferenceOutputConfigOutputTypeDef = TypedDict(
+    "AsyncInferenceOutputConfigOutputTypeDef",
+    {
+        "KmsKeyId": NotRequired[str],
+        "S3OutputPath": NotRequired[str],
+        "NotificationConfig": NotRequired[AsyncInferenceNotificationConfigOutputTypeDef],
+        "S3FailurePath": NotRequired[str],
+    },
+)
 AsyncInferenceOutputConfigTypeDef = TypedDict(
     "AsyncInferenceOutputConfigTypeDef",
     {
         "KmsKeyId": NotRequired[str],
         "S3OutputPath": NotRequired[str],
         "NotificationConfig": NotRequired[AsyncInferenceNotificationConfigTypeDef],
         "S3FailurePath": NotRequired[str],
     },
 )
+AutoMLCandidateGenerationConfigOutputTypeDef = TypedDict(
+    "AutoMLCandidateGenerationConfigOutputTypeDef",
+    {
+        "FeatureSpecificationS3Uri": NotRequired[str],
+        "AlgorithmsConfig": NotRequired[List[AutoMLAlgorithmConfigOutputTypeDef]],
+    },
+)
+CandidateGenerationConfigOutputTypeDef = TypedDict(
+    "CandidateGenerationConfigOutputTypeDef",
+    {
+        "AlgorithmsConfig": NotRequired[List[AutoMLAlgorithmConfigOutputTypeDef]],
+    },
+)
 AutoMLCandidateGenerationConfigTypeDef = TypedDict(
     "AutoMLCandidateGenerationConfigTypeDef",
     {
         "FeatureSpecificationS3Uri": NotRequired[str],
         "AlgorithmsConfig": NotRequired[Sequence[AutoMLAlgorithmConfigTypeDef]],
     },
 )
@@ -6626,14 +7100,45 @@
 AutoMLProblemTypeResolvedAttributesTypeDef = TypedDict(
     "AutoMLProblemTypeResolvedAttributesTypeDef",
     {
         "TabularResolvedAttributes": NotRequired[TabularResolvedAttributesTypeDef],
         "TextGenerationResolvedAttributes": NotRequired[TextGenerationResolvedAttributesTypeDef],
     },
 )
+AutoMLSecurityConfigOutputTypeDef = TypedDict(
+    "AutoMLSecurityConfigOutputTypeDef",
+    {
+        "VolumeKmsKeyId": NotRequired[str],
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+    },
+)
+LabelingJobResourceConfigOutputTypeDef = TypedDict(
+    "LabelingJobResourceConfigOutputTypeDef",
+    {
+        "VolumeKmsKeyId": NotRequired[str],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+    },
+)
+MonitoringNetworkConfigOutputTypeDef = TypedDict(
+    "MonitoringNetworkConfigOutputTypeDef",
+    {
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "EnableNetworkIsolation": NotRequired[bool],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+    },
+)
+NetworkConfigOutputTypeDef = TypedDict(
+    "NetworkConfigOutputTypeDef",
+    {
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "EnableNetworkIsolation": NotRequired[bool],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+    },
+)
 AutoMLSecurityConfigTypeDef = TypedDict(
     "AutoMLSecurityConfigTypeDef",
     {
         "VolumeKmsKeyId": NotRequired[str],
         "EnableInterContainerTrafficEncryption": NotRequired[bool],
         "VpcConfig": NotRequired[VpcConfigTypeDef],
     },
@@ -6729,14 +7234,26 @@
 CandidatePropertiesTypeDef = TypedDict(
     "CandidatePropertiesTypeDef",
     {
         "CandidateArtifactLocations": NotRequired[CandidateArtifactLocationsTypeDef],
         "CandidateMetrics": NotRequired[List[MetricDatumTypeDef]],
     },
 )
+CanvasAppSettingsOutputTypeDef = TypedDict(
+    "CanvasAppSettingsOutputTypeDef",
+    {
+        "TimeSeriesForecastingSettings": NotRequired[TimeSeriesForecastingSettingsTypeDef],
+        "ModelRegisterSettings": NotRequired[ModelRegisterSettingsTypeDef],
+        "WorkspaceSettings": NotRequired[WorkspaceSettingsTypeDef],
+        "IdentityProviderOAuthSettings": NotRequired[List[IdentityProviderOAuthSettingTypeDef]],
+        "DirectDeploySettings": NotRequired[DirectDeploySettingsTypeDef],
+        "KendraSettings": NotRequired[KendraSettingsTypeDef],
+        "GenerativeAiSettings": NotRequired[GenerativeAiSettingsTypeDef],
+    },
+)
 CanvasAppSettingsTypeDef = TypedDict(
     "CanvasAppSettingsTypeDef",
     {
         "TimeSeriesForecastingSettings": NotRequired[TimeSeriesForecastingSettingsTypeDef],
         "ModelRegisterSettings": NotRequired[ModelRegisterSettingsTypeDef],
         "WorkspaceSettings": NotRequired[WorkspaceSettingsTypeDef],
         "IdentityProviderOAuthSettings": NotRequired[Sequence[IdentityProviderOAuthSettingTypeDef]],
@@ -6759,33 +7276,58 @@
     {
         "Type": TrafficRoutingConfigTypeType,
         "WaitIntervalInSeconds": int,
         "CanarySize": NotRequired[CapacitySizeTypeDef],
         "LinearStepSize": NotRequired[CapacitySizeTypeDef],
     },
 )
+InferenceExperimentDataStorageConfigOutputTypeDef = TypedDict(
+    "InferenceExperimentDataStorageConfigOutputTypeDef",
+    {
+        "Destination": str,
+        "KmsKey": NotRequired[str],
+        "ContentType": NotRequired[CaptureContentTypeHeaderOutputTypeDef],
+    },
+)
 InferenceExperimentDataStorageConfigTypeDef = TypedDict(
     "InferenceExperimentDataStorageConfigTypeDef",
     {
         "Destination": str,
         "KmsKey": NotRequired[str],
         "ContentType": NotRequired[CaptureContentTypeHeaderTypeDef],
     },
 )
+DataCaptureConfigOutputTypeDef = TypedDict(
+    "DataCaptureConfigOutputTypeDef",
+    {
+        "InitialSamplingPercentage": int,
+        "DestinationS3Uri": str,
+        "CaptureOptions": List[CaptureOptionTypeDef],
+        "EnableCapture": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "CaptureContentTypeHeader": NotRequired[CaptureContentTypeHeaderOutputTypeDef],
+    },
+)
 DataCaptureConfigTypeDef = TypedDict(
     "DataCaptureConfigTypeDef",
     {
         "InitialSamplingPercentage": int,
         "DestinationS3Uri": str,
         "CaptureOptions": Sequence[CaptureOptionTypeDef],
         "EnableCapture": NotRequired[bool],
         "KmsKeyId": NotRequired[str],
         "CaptureContentTypeHeader": NotRequired[CaptureContentTypeHeaderTypeDef],
     },
 )
+EnvironmentParameterRangesOutputTypeDef = TypedDict(
+    "EnvironmentParameterRangesOutputTypeDef",
+    {
+        "CategoricalParameterRanges": NotRequired[List[CategoricalParameterOutputTypeDef]],
+    },
+)
 EnvironmentParameterRangesTypeDef = TypedDict(
     "EnvironmentParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": NotRequired[Sequence[CategoricalParameterTypeDef]],
     },
 )
 ClarifyShapConfigTypeDef = TypedDict(
@@ -6847,26 +7389,40 @@
     "ListClustersResponseTypeDef",
     {
         "NextToken": str,
         "ClusterSummaries": List[ClusterSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CodeEditorAppImageConfigPaginatorTypeDef = TypedDict(
-    "CodeEditorAppImageConfigPaginatorTypeDef",
+CodeEditorAppImageConfigExtraOutputTypeDef = TypedDict(
+    "CodeEditorAppImageConfigExtraOutputTypeDef",
     {
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
-        "ContainerConfig": NotRequired[ContainerConfigPaginatorTypeDef],
+        "ContainerConfig": NotRequired[ContainerConfigExtraOutputTypeDef],
     },
 )
-JupyterLabAppImageConfigPaginatorTypeDef = TypedDict(
-    "JupyterLabAppImageConfigPaginatorTypeDef",
+JupyterLabAppImageConfigExtraOutputTypeDef = TypedDict(
+    "JupyterLabAppImageConfigExtraOutputTypeDef",
     {
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
-        "ContainerConfig": NotRequired[ContainerConfigPaginatorTypeDef],
+        "ContainerConfig": NotRequired[ContainerConfigExtraOutputTypeDef],
+    },
+)
+CodeEditorAppImageConfigOutputTypeDef = TypedDict(
+    "CodeEditorAppImageConfigOutputTypeDef",
+    {
+        "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
+        "ContainerConfig": NotRequired[ContainerConfigOutputTypeDef],
+    },
+)
+JupyterLabAppImageConfigOutputTypeDef = TypedDict(
+    "JupyterLabAppImageConfigOutputTypeDef",
+    {
+        "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
+        "ContainerConfig": NotRequired[ContainerConfigOutputTypeDef],
     },
 )
 CodeEditorAppImageConfigTypeDef = TypedDict(
     "CodeEditorAppImageConfigTypeDef",
     {
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
         "ContainerConfig": NotRequired[ContainerConfigTypeDef],
@@ -6875,30 +7431,53 @@
 JupyterLabAppImageConfigTypeDef = TypedDict(
     "JupyterLabAppImageConfigTypeDef",
     {
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
         "ContainerConfig": NotRequired[ContainerConfigTypeDef],
     },
 )
+CodeEditorAppSettingsOutputTypeDef = TypedDict(
+    "CodeEditorAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CustomImages": NotRequired[List[CustomImageTypeDef]],
+        "LifecycleConfigArns": NotRequired[List[str]],
+    },
+)
 CodeEditorAppSettingsTypeDef = TypedDict(
     "CodeEditorAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CustomImages": NotRequired[Sequence[CustomImageTypeDef]],
         "LifecycleConfigArns": NotRequired[Sequence[str]],
     },
 )
+KernelGatewayAppSettingsOutputTypeDef = TypedDict(
+    "KernelGatewayAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CustomImages": NotRequired[List[CustomImageTypeDef]],
+        "LifecycleConfigArns": NotRequired[List[str]],
+    },
+)
 KernelGatewayAppSettingsTypeDef = TypedDict(
     "KernelGatewayAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CustomImages": NotRequired[Sequence[CustomImageTypeDef]],
         "LifecycleConfigArns": NotRequired[Sequence[str]],
     },
 )
+RSessionAppSettingsOutputTypeDef = TypedDict(
+    "RSessionAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CustomImages": NotRequired[List[CustomImageTypeDef]],
+    },
+)
 RSessionAppSettingsTypeDef = TypedDict(
     "RSessionAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CustomImages": NotRequired[Sequence[CustomImageTypeDef]],
     },
 )
@@ -6927,51 +7506,84 @@
         "CodeRepositoryArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "GitConfig": GitConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+JupyterLabAppSettingsOutputTypeDef = TypedDict(
+    "JupyterLabAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CustomImages": NotRequired[List[CustomImageTypeDef]],
+        "LifecycleConfigArns": NotRequired[List[str]],
+        "CodeRepositories": NotRequired[List[CodeRepositoryTypeDef]],
+    },
+)
 JupyterLabAppSettingsTypeDef = TypedDict(
     "JupyterLabAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CustomImages": NotRequired[Sequence[CustomImageTypeDef]],
         "LifecycleConfigArns": NotRequired[Sequence[str]],
         "CodeRepositories": NotRequired[Sequence[CodeRepositoryTypeDef]],
     },
 )
+JupyterServerAppSettingsOutputTypeDef = TypedDict(
+    "JupyterServerAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "LifecycleConfigArns": NotRequired[List[str]],
+        "CodeRepositories": NotRequired[List[CodeRepositoryTypeDef]],
+    },
+)
 JupyterServerAppSettingsTypeDef = TypedDict(
     "JupyterServerAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "LifecycleConfigArns": NotRequired[Sequence[str]],
         "CodeRepositories": NotRequired[Sequence[CodeRepositoryTypeDef]],
     },
 )
+SpaceJupyterLabAppSettingsOutputTypeDef = TypedDict(
+    "SpaceJupyterLabAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CodeRepositories": NotRequired[List[CodeRepositoryTypeDef]],
+    },
+)
 SpaceJupyterLabAppSettingsTypeDef = TypedDict(
     "SpaceJupyterLabAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CodeRepositories": NotRequired[Sequence[CodeRepositoryTypeDef]],
     },
 )
 CollectionConfigTypeDef = TypedDict(
     "CollectionConfigTypeDef",
     {
         "VectorConfig": NotRequired[VectorConfigTypeDef],
     },
 )
-DebugHookConfigPaginatorTypeDef = TypedDict(
-    "DebugHookConfigPaginatorTypeDef",
+DebugHookConfigExtraOutputTypeDef = TypedDict(
+    "DebugHookConfigExtraOutputTypeDef",
+    {
+        "S3OutputPath": str,
+        "LocalPath": NotRequired[str],
+        "HookParameters": NotRequired[Dict[str, str]],
+        "CollectionConfigurations": NotRequired[List[CollectionConfigurationExtraOutputTypeDef]],
+    },
+)
+DebugHookConfigOutputTypeDef = TypedDict(
+    "DebugHookConfigOutputTypeDef",
     {
         "S3OutputPath": str,
         "LocalPath": NotRequired[str],
         "HookParameters": NotRequired[Dict[str, str]],
-        "CollectionConfigurations": NotRequired[List[CollectionConfigurationPaginatorTypeDef]],
+        "CollectionConfigurations": NotRequired[List[CollectionConfigurationOutputTypeDef]],
     },
 )
 DebugHookConfigTypeDef = TypedDict(
     "DebugHookConfigTypeDef",
     {
         "S3OutputPath": str,
         "LocalPath": NotRequired[str],
@@ -6979,16 +7591,16 @@
         "CollectionConfigurations": NotRequired[Sequence[CollectionConfigurationTypeDef]],
     },
 )
 ListCompilationJobsResponseTypeDef = TypedDict(
     "ListCompilationJobsResponseTypeDef",
     {
         "CompilationJobSummaries": List[CompilationJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ContextSummaryTypeDef = TypedDict(
     "ContextSummaryTypeDef",
     {
         "ContextArn": NotRequired[str],
         "ContextName": NotRequired[str],
@@ -8176,14 +8788,17 @@
 )
 CustomFileSystemTypeDef = TypedDict(
     "CustomFileSystemTypeDef",
     {
         "EFSFileSystem": NotRequired[EFSFileSystemTypeDef],
     },
 )
+DataQualityAppSpecificationUnionTypeDef = Union[
+    DataQualityAppSpecificationTypeDef, DataQualityAppSpecificationOutputTypeDef
+]
 ModelBiasBaselineConfigTypeDef = TypedDict(
     "ModelBiasBaselineConfigTypeDef",
     {
         "BaseliningJobName": NotRequired[str],
         "ConstraintsResource": NotRequired[MonitoringConstraintsResourceTypeDef],
     },
 )
@@ -8213,18 +8828,25 @@
     "MonitoringBaselineConfigTypeDef",
     {
         "BaseliningJobName": NotRequired[str],
         "ConstraintsResource": NotRequired[MonitoringConstraintsResourceTypeDef],
         "StatisticsResource": NotRequired[MonitoringStatisticsResourceTypeDef],
     },
 )
-DataSourcePaginatorTypeDef = TypedDict(
-    "DataSourcePaginatorTypeDef",
+DataSourceExtraOutputTypeDef = TypedDict(
+    "DataSourceExtraOutputTypeDef",
     {
-        "S3DataSource": NotRequired[S3DataSourcePaginatorTypeDef],
+        "S3DataSource": NotRequired[S3DataSourceExtraOutputTypeDef],
+        "FileSystemDataSource": NotRequired[FileSystemDataSourceTypeDef],
+    },
+)
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "S3DataSource": NotRequired[S3DataSourceOutputTypeDef],
         "FileSystemDataSource": NotRequired[FileSystemDataSourceTypeDef],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "S3DataSource": NotRequired[S3DataSourceTypeDef],
@@ -8237,14 +8859,17 @@
         "AthenaDatasetDefinition": NotRequired[AthenaDatasetDefinitionTypeDef],
         "RedshiftDatasetDefinition": NotRequired[RedshiftDatasetDefinitionTypeDef],
         "LocalPath": NotRequired[str],
         "DataDistributionType": NotRequired[DataDistributionTypeType],
         "InputMode": NotRequired[InputModeType],
     },
 )
+DebugRuleConfigurationUnionTypeDef = Union[
+    DebugRuleConfigurationTypeDef, DebugRuleConfigurationExtraOutputTypeDef
+]
 DefaultSpaceStorageSettingsTypeDef = TypedDict(
     "DefaultSpaceStorageSettingsTypeDef",
     {
         "DefaultEbsStorageSettings": NotRequired[DefaultEbsStorageSettingsTypeDef],
     },
 )
 DeleteDomainRequestRequestTypeDef = TypedDict(
@@ -8267,46 +8892,47 @@
     {
         "RecommendationStatus": RecommendationStatusType,
         "RealTimeInferenceRecommendations": NotRequired[
             List[RealTimeInferenceRecommendationTypeDef]
         ],
     },
 )
-DeploymentStageTypeDef = TypedDict(
-    "DeploymentStageTypeDef",
+DeploymentStageStatusSummaryTypeDef = TypedDict(
+    "DeploymentStageStatusSummaryTypeDef",
     {
         "StageName": str,
-        "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
-        "DeploymentConfig": NotRequired[EdgeDeploymentConfigTypeDef],
+        "DeviceSelectionConfig": DeviceSelectionConfigOutputTypeDef,
+        "DeploymentConfig": EdgeDeploymentConfigTypeDef,
+        "DeploymentStatus": EdgeDeploymentStatusTypeDef,
     },
 )
-DeploymentStageStatusSummaryTypeDef = TypedDict(
-    "DeploymentStageStatusSummaryTypeDef",
+DeploymentStageTypeDef = TypedDict(
+    "DeploymentStageTypeDef",
     {
         "StageName": str,
         "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
-        "DeploymentConfig": EdgeDeploymentConfigTypeDef,
-        "DeploymentStatus": EdgeDeploymentStatusTypeDef,
+        "DeploymentConfig": NotRequired[EdgeDeploymentConfigTypeDef],
     },
 )
+NeoVpcConfigUnionTypeDef = Union[NeoVpcConfigTypeDef, NeoVpcConfigOutputTypeDef]
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceArn": str,
         "DeviceName": str,
         "Description": str,
         "DeviceFleetName": str,
         "IotThingName": str,
         "RegistrationTime": datetime,
         "LatestHeartbeat": datetime,
         "Models": List[EdgeModelTypeDef],
         "MaxModels": int,
-        "NextToken": str,
         "AgentVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeEdgePackagingJobResponseTypeDef = TypedDict(
     "DescribeEdgePackagingJobResponseTypeDef",
     {
         "EdgePackagingJobArn": str,
         "EdgePackagingJobName": str,
@@ -8508,14 +9134,32 @@
         "HumanTaskUiName": str,
         "HumanTaskUiStatus": HumanTaskUiStatusType,
         "CreationTime": datetime,
         "UiTemplate": UiTemplateInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+InferenceExperimentSummaryTypeDef = TypedDict(
+    "InferenceExperimentSummaryTypeDef",
+    {
+        "Name": str,
+        "Type": Literal["ShadowMode"],
+        "Status": InferenceExperimentStatusType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "Schedule": NotRequired[InferenceExperimentScheduleOutputTypeDef],
+        "StatusReason": NotRequired[str],
+        "Description": NotRequired[str],
+        "CompletionTime": NotRequired[datetime],
+        "RoleArn": NotRequired[str],
+    },
+)
+ModelBiasAppSpecificationUnionTypeDef = Union[
+    ModelBiasAppSpecificationTypeDef, ModelBiasAppSpecificationOutputTypeDef
+]
 DescribeModelCardExportJobResponseTypeDef = TypedDict(
     "DescribeModelCardExportJobResponseTypeDef",
     {
         "ModelCardExportJobName": str,
         "ModelCardExportJobArn": str,
         "Status": ModelCardExportJobStatusType,
         "ModelCardName": str,
@@ -8524,35 +9168,41 @@
         "CreatedAt": datetime,
         "LastModifiedAt": datetime,
         "FailureReason": str,
         "ExportArtifacts": ModelCardExportArtifactsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ModelExplainabilityAppSpecificationUnionTypeDef = Union[
+    ModelExplainabilityAppSpecificationTypeDef, ModelExplainabilityAppSpecificationOutputTypeDef
+]
+ModelQualityAppSpecificationUnionTypeDef = Union[
+    ModelQualityAppSpecificationTypeDef, ModelQualityAppSpecificationOutputTypeDef
+]
 ListMonitoringExecutionsResponseTypeDef = TypedDict(
     "ListMonitoringExecutionsResponseTypeDef",
     {
         "MonitoringExecutionSummaries": List[MonitoringExecutionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSubscribedWorkteamResponseTypeDef = TypedDict(
     "DescribeSubscribedWorkteamResponseTypeDef",
     {
         "SubscribedWorkteam": SubscribedWorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSubscribedWorkteamsResponseTypeDef = TypedDict(
     "ListSubscribedWorkteamsResponseTypeDef",
     {
         "SubscribedWorkteams": List[SubscribedWorkteamTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TrainingJobSummaryTypeDef = TypedDict(
     "TrainingJobSummaryTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
@@ -8583,24 +9233,24 @@
         "ServerlessUpdateConfig": NotRequired[ProductionVariantServerlessUpdateConfigTypeDef],
     },
 )
 ListStageDevicesResponseTypeDef = TypedDict(
     "ListStageDevicesResponseTypeDef",
     {
         "DeviceDeploymentSummaries": List[DeviceDeploymentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDeviceFleetsResponseTypeDef = TypedDict(
     "ListDeviceFleetsResponseTypeDef",
     {
         "DeviceFleetSummaries": List[DeviceFleetSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "DeviceName": str,
         "DeviceArn": str,
@@ -8628,16 +9278,16 @@
         "Devices": Sequence[DeviceTypeDef],
     },
 )
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DriftCheckBiasTypeDef = TypedDict(
     "DriftCheckBiasTypeDef",
     {
         "ConfigFile": NotRequired[FileSourceTypeDef],
         "PreTrainingConstraints": NotRequired[MetricsSourceTypeDef],
@@ -8657,16 +9307,16 @@
         "EbsStorageSettings": NotRequired[EbsStorageSettingsTypeDef],
     },
 )
 ListEdgeDeploymentPlansResponseTypeDef = TypedDict(
     "ListEdgeDeploymentPlansResponseTypeDef",
     {
         "EdgeDeploymentPlanSummaries": List[EdgeDeploymentPlanSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetDeviceFleetReportResponseTypeDef = TypedDict(
     "GetDeviceFleetReportResponseTypeDef",
     {
         "DeviceFleetArn": str,
         "DeviceFleetName": str,
@@ -8679,24 +9329,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListEdgePackagingJobsResponseTypeDef = TypedDict(
     "ListEdgePackagingJobsResponseTypeDef",
     {
         "EdgePackagingJobSummaries": List[EdgePackagingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListEndpointConfigsOutputTypeDef = TypedDict(
     "ListEndpointConfigsOutputTypeDef",
     {
         "EndpointConfigs": List[EndpointConfigSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 EndpointOutputConfigurationTypeDef = TypedDict(
     "EndpointOutputConfigurationTypeDef",
     {
         "EndpointName": str,
         "VariantName": str,
@@ -8712,16 +9362,16 @@
         "EndpointInfo": EndpointInfoTypeDef,
     },
 )
 ListEndpointsOutputTypeDef = TypedDict(
     "ListEndpointsOutputTypeDef",
     {
         "Endpoints": List[EndpointSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModelConfigurationTypeDef = TypedDict(
     "ModelConfigurationTypeDef",
     {
         "InferenceSpecificationName": NotRequired[str],
         "EnvironmentParameters": NotRequired[List[EnvironmentParameterTypeDef]],
@@ -8754,16 +9404,16 @@
         "ObjectiveStatus": NotRequired[ObjectiveStatusType],
     },
 )
 ListFlowDefinitionsResponseTypeDef = TypedDict(
     "ListFlowDefinitionsResponseTypeDef",
     {
         "FlowDefinitionSummaries": List[FlowDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
     "GetScalingConfigurationRecommendationRequestRequestTypeDef",
     {
         "InferenceRecommendationsJobName": str,
         "RecommendationId": NotRequired[str],
@@ -8786,58 +9436,70 @@
         "GitConfig": NotRequired[GitConfigForUpdateTypeDef],
     },
 )
 ListHubContentVersionsResponseTypeDef = TypedDict(
     "ListHubContentVersionsResponseTypeDef",
     {
         "HubContentSummaries": List[HubContentInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListHubContentsResponseTypeDef = TypedDict(
     "ListHubContentsResponseTypeDef",
     {
         "HubContentSummaries": List[HubContentInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListHubsResponseTypeDef = TypedDict(
     "ListHubsResponseTypeDef",
     {
         "HubSummaries": List[HubInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 HumanLoopActivationConfigTypeDef = TypedDict(
     "HumanLoopActivationConfigTypeDef",
     {
         "HumanLoopActivationConditionsConfig": HumanLoopActivationConditionsConfigTypeDef,
     },
 )
 ListHumanTaskUisResponseTypeDef = TypedDict(
     "ListHumanTaskUisResponseTypeDef",
     {
         "HumanTaskUiSummaries": List[HumanTaskUiSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-NetworkConfigPaginatorTypeDef = TypedDict(
-    "NetworkConfigPaginatorTypeDef",
+NetworkConfigExtraOutputTypeDef = TypedDict(
+    "NetworkConfigExtraOutputTypeDef",
     {
         "EnableInterContainerTrafficEncryption": NotRequired[bool],
         "EnableNetworkIsolation": NotRequired[bool],
-        "VpcConfig": NotRequired[VpcConfigPaginatorTypeDef],
+        "VpcConfig": NotRequired[VpcConfigExtraOutputTypeDef],
+    },
+)
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigExtraOutputTypeDef]
+HyperParameterTuningResourceConfigExtraOutputTypeDef = TypedDict(
+    "HyperParameterTuningResourceConfigExtraOutputTypeDef",
+    {
+        "InstanceType": NotRequired[TrainingInstanceTypeType],
+        "InstanceCount": NotRequired[int],
+        "VolumeSizeInGB": NotRequired[int],
+        "VolumeKmsKeyId": NotRequired[str],
+        "AllocationStrategy": NotRequired[Literal["Prioritized"]],
+        "InstanceConfigs": NotRequired[List[HyperParameterTuningInstanceConfigTypeDef]],
     },
 )
-HyperParameterTuningResourceConfigPaginatorTypeDef = TypedDict(
-    "HyperParameterTuningResourceConfigPaginatorTypeDef",
+HyperParameterTuningResourceConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningResourceConfigOutputTypeDef",
     {
         "InstanceType": NotRequired[TrainingInstanceTypeType],
         "InstanceCount": NotRequired[int],
         "VolumeSizeInGB": NotRequired[int],
         "VolumeKmsKeyId": NotRequired[str],
         "AllocationStrategy": NotRequired[Literal["Prioritized"]],
         "InstanceConfigs": NotRequired[List[HyperParameterTuningInstanceConfigTypeDef]],
@@ -8871,16 +9533,23 @@
 )
 HyperParameterTuningJobStrategyConfigTypeDef = TypedDict(
     "HyperParameterTuningJobStrategyConfigTypeDef",
     {
         "HyperbandStrategyConfig": NotRequired[HyperbandStrategyConfigTypeDef],
     },
 )
-HyperParameterTuningJobWarmStartConfigPaginatorTypeDef = TypedDict(
-    "HyperParameterTuningJobWarmStartConfigPaginatorTypeDef",
+HyperParameterTuningJobWarmStartConfigExtraOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobWarmStartConfigExtraOutputTypeDef",
+    {
+        "ParentHyperParameterTuningJobs": List[ParentHyperParameterTuningJobTypeDef],
+        "WarmStartType": HyperParameterTuningJobWarmStartTypeType,
+    },
+)
+HyperParameterTuningJobWarmStartConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobWarmStartConfigOutputTypeDef",
     {
         "ParentHyperParameterTuningJobs": List[ParentHyperParameterTuningJobTypeDef],
         "WarmStartType": HyperParameterTuningJobWarmStartTypeType,
     },
 )
 HyperParameterTuningJobWarmStartConfigTypeDef = TypedDict(
     "HyperParameterTuningJobWarmStartConfigTypeDef",
@@ -8905,24 +9574,24 @@
         "RepositoryAuthConfig": NotRequired[RepositoryAuthConfigTypeDef],
     },
 )
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "Images": List[ImageTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListImageVersionsResponseTypeDef = TypedDict(
     "ListImageVersionsResponseTypeDef",
     {
         "ImageVersions": List[ImageVersionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InferenceComponentSpecificationTypeDef = TypedDict(
     "InferenceComponentSpecificationTypeDef",
     {
         "ComputeResourceRequirements": InferenceComponentComputeResourceRequirementsTypeDef,
         "ModelName": NotRequired[str],
@@ -8930,43 +9599,39 @@
         "StartupParameters": NotRequired[InferenceComponentStartupParametersTypeDef],
     },
 )
 ListInferenceComponentsOutputTypeDef = TypedDict(
     "ListInferenceComponentsOutputTypeDef",
     {
         "InferenceComponents": List[InferenceComponentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-InferenceExperimentSummaryPaginatorTypeDef = TypedDict(
-    "InferenceExperimentSummaryPaginatorTypeDef",
-    {
-        "Name": str,
-        "Type": Literal["ShadowMode"],
-        "Status": InferenceExperimentStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "Schedule": NotRequired[InferenceExperimentSchedulePaginatorTypeDef],
-        "StatusReason": NotRequired[str],
-        "Description": NotRequired[str],
-        "CompletionTime": NotRequired[datetime],
-        "RoleArn": NotRequired[str],
+        "NextToken": NotRequired[str],
     },
 )
 ListInferenceRecommendationsJobsResponseTypeDef = TypedDict(
     "ListInferenceRecommendationsJobsResponseTypeDef",
     {
         "InferenceRecommendationsJobs": List[InferenceRecommendationsJobTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-ResourceConfigPaginatorTypeDef = TypedDict(
-    "ResourceConfigPaginatorTypeDef",
+ResourceConfigExtraOutputTypeDef = TypedDict(
+    "ResourceConfigExtraOutputTypeDef",
+    {
+        "VolumeSizeInGB": int,
+        "InstanceType": NotRequired[TrainingInstanceTypeType],
+        "InstanceCount": NotRequired[int],
+        "VolumeKmsKeyId": NotRequired[str],
+        "KeepAlivePeriodInSeconds": NotRequired[int],
+        "InstanceGroups": NotRequired[List[InstanceGroupTypeDef]],
+    },
+)
+ResourceConfigOutputTypeDef = TypedDict(
+    "ResourceConfigOutputTypeDef",
     {
         "VolumeSizeInGB": int,
         "InstanceType": NotRequired[TrainingInstanceTypeType],
         "InstanceCount": NotRequired[int],
         "VolumeKmsKeyId": NotRequired[str],
         "KeepAlivePeriodInSeconds": NotRequired[int],
         "InstanceGroups": NotRequired[List[InstanceGroupTypeDef]],
@@ -8979,48 +9644,80 @@
         "InstanceType": NotRequired[TrainingInstanceTypeType],
         "InstanceCount": NotRequired[int],
         "VolumeKmsKeyId": NotRequired[str],
         "KeepAlivePeriodInSeconds": NotRequired[int],
         "InstanceGroups": NotRequired[Sequence[InstanceGroupTypeDef]],
     },
 )
+ParameterRangeOutputTypeDef = TypedDict(
+    "ParameterRangeOutputTypeDef",
+    {
+        "IntegerParameterRangeSpecification": NotRequired[
+            IntegerParameterRangeSpecificationTypeDef
+        ],
+        "ContinuousParameterRangeSpecification": NotRequired[
+            ContinuousParameterRangeSpecificationTypeDef
+        ],
+        "CategoricalParameterRangeSpecification": NotRequired[
+            CategoricalParameterRangeSpecificationOutputTypeDef
+        ],
+    },
+)
 ParameterRangeTypeDef = TypedDict(
     "ParameterRangeTypeDef",
     {
         "IntegerParameterRangeSpecification": NotRequired[
             IntegerParameterRangeSpecificationTypeDef
         ],
         "ContinuousParameterRangeSpecification": NotRequired[
             ContinuousParameterRangeSpecificationTypeDef
         ],
         "CategoricalParameterRangeSpecification": NotRequired[
             CategoricalParameterRangeSpecificationTypeDef
         ],
     },
 )
-ParameterRangesPaginatorTypeDef = TypedDict(
-    "ParameterRangesPaginatorTypeDef",
+ParameterRangesExtraOutputTypeDef = TypedDict(
+    "ParameterRangesExtraOutputTypeDef",
+    {
+        "IntegerParameterRanges": NotRequired[List[IntegerParameterRangeTypeDef]],
+        "ContinuousParameterRanges": NotRequired[List[ContinuousParameterRangeTypeDef]],
+        "CategoricalParameterRanges": NotRequired[
+            List[CategoricalParameterRangeExtraOutputTypeDef]
+        ],
+        "AutoParameters": NotRequired[List[AutoParameterTypeDef]],
+    },
+)
+ParameterRangesOutputTypeDef = TypedDict(
+    "ParameterRangesOutputTypeDef",
     {
         "IntegerParameterRanges": NotRequired[List[IntegerParameterRangeTypeDef]],
         "ContinuousParameterRanges": NotRequired[List[ContinuousParameterRangeTypeDef]],
-        "CategoricalParameterRanges": NotRequired[List[CategoricalParameterRangePaginatorTypeDef]],
+        "CategoricalParameterRanges": NotRequired[List[CategoricalParameterRangeOutputTypeDef]],
         "AutoParameters": NotRequired[List[AutoParameterTypeDef]],
     },
 )
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "IntegerParameterRanges": NotRequired[Sequence[IntegerParameterRangeTypeDef]],
         "ContinuousParameterRanges": NotRequired[Sequence[ContinuousParameterRangeTypeDef]],
         "CategoricalParameterRanges": NotRequired[Sequence[CategoricalParameterRangeTypeDef]],
         "AutoParameters": NotRequired[Sequence[AutoParameterTypeDef]],
     },
 )
-KernelGatewayImageConfigPaginatorTypeDef = TypedDict(
-    "KernelGatewayImageConfigPaginatorTypeDef",
+KernelGatewayImageConfigExtraOutputTypeDef = TypedDict(
+    "KernelGatewayImageConfigExtraOutputTypeDef",
+    {
+        "KernelSpecs": List[KernelSpecTypeDef],
+        "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
+    },
+)
+KernelGatewayImageConfigOutputTypeDef = TypedDict(
+    "KernelGatewayImageConfigOutputTypeDef",
     {
         "KernelSpecs": List[KernelSpecTypeDef],
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
     },
 )
 KernelGatewayImageConfigTypeDef = TypedDict(
     "KernelGatewayImageConfigTypeDef",
@@ -9047,16 +9744,16 @@
         "SnsDataSource": NotRequired[LabelingJobSnsDataSourceTypeDef],
     },
 )
 ListLineageGroupsResponseTypeDef = TypedDict(
     "ListLineageGroupsResponseTypeDef",
     {
         "LineageGroupSummaries": List[LineageGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListActionsRequestListActionsPaginateTypeDef = TypedDict(
     "ListActionsRequestListActionsPaginateTypeDef",
     {
         "SourceUri": NotRequired[str],
         "ActionType": NotRequired[str],
@@ -9889,207 +10586,214 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDataQualityJobDefinitionsResponseTypeDef = TypedDict(
     "ListDataQualityJobDefinitionsResponseTypeDef",
     {
         "JobDefinitionSummaries": List[MonitoringJobDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelBiasJobDefinitionsResponseTypeDef = TypedDict(
     "ListModelBiasJobDefinitionsResponseTypeDef",
     {
         "JobDefinitionSummaries": List[MonitoringJobDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelExplainabilityJobDefinitionsResponseTypeDef = TypedDict(
     "ListModelExplainabilityJobDefinitionsResponseTypeDef",
     {
         "JobDefinitionSummaries": List[MonitoringJobDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelQualityJobDefinitionsResponseTypeDef = TypedDict(
     "ListModelQualityJobDefinitionsResponseTypeDef",
     {
         "JobDefinitionSummaries": List[MonitoringJobDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelCardExportJobsResponseTypeDef = TypedDict(
     "ListModelCardExportJobsResponseTypeDef",
     {
         "ModelCardExportJobSummaries": List[ModelCardExportJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelCardVersionsResponseTypeDef = TypedDict(
     "ListModelCardVersionsResponseTypeDef",
     {
         "ModelCardVersionSummaryList": List[ModelCardVersionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelCardsResponseTypeDef = TypedDict(
     "ListModelCardsResponseTypeDef",
     {
         "ModelCardSummaries": List[ModelCardSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelMetadataResponseTypeDef = TypedDict(
     "ListModelMetadataResponseTypeDef",
     {
         "ModelMetadataSummaries": List[ModelMetadataSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelPackageGroupsOutputTypeDef = TypedDict(
     "ListModelPackageGroupsOutputTypeDef",
     {
         "ModelPackageGroupSummaryList": List[ModelPackageGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelPackagesOutputTypeDef = TypedDict(
     "ListModelPackagesOutputTypeDef",
     {
         "ModelPackageSummaryList": List[ModelPackageSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelsOutputTypeDef = TypedDict(
     "ListModelsOutputTypeDef",
     {
         "Models": List[ModelSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMonitoringAlertHistoryResponseTypeDef = TypedDict(
     "ListMonitoringAlertHistoryResponseTypeDef",
     {
         "MonitoringAlertHistory": List[MonitoringAlertHistorySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMonitoringSchedulesResponseTypeDef = TypedDict(
     "ListMonitoringSchedulesResponseTypeDef",
     {
         "MonitoringScheduleSummaries": List[MonitoringScheduleSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListNotebookInstanceLifecycleConfigsOutputTypeDef = TypedDict(
     "ListNotebookInstanceLifecycleConfigsOutputTypeDef",
     {
-        "NextToken": str,
         "NotebookInstanceLifecycleConfigs": List[NotebookInstanceLifecycleConfigSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListNotebookInstancesOutputTypeDef = TypedDict(
     "ListNotebookInstancesOutputTypeDef",
     {
-        "NextToken": str,
         "NotebookInstances": List[NotebookInstanceSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPipelineExecutionsResponseTypeDef = TypedDict(
     "ListPipelineExecutionsResponseTypeDef",
     {
         "PipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPipelineParametersForExecutionResponseTypeDef = TypedDict(
     "ListPipelineParametersForExecutionResponseTypeDef",
     {
         "PipelineParameters": List[ParameterTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "PipelineSummaries": List[PipelineSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProcessingJobsResponseTypeDef = TypedDict(
     "ListProcessingJobsResponseTypeDef",
     {
         "ProcessingJobSummaries": List[ProcessingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProjectsOutputTypeDef = TypedDict(
     "ListProjectsOutputTypeDef",
     {
         "ProjectSummaryList": List[ProjectSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListResourceCatalogsResponseTypeDef = TypedDict(
     "ListResourceCatalogsResponseTypeDef",
     {
         "ResourceCatalogs": List[ResourceCatalogTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListStudioLifecycleConfigsResponseTypeDef = TypedDict(
     "ListStudioLifecycleConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "StudioLifecycleConfigs": List[StudioLifecycleConfigDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTransformJobsResponseTypeDef = TypedDict(
     "ListTransformJobsResponseTypeDef",
     {
         "TransformJobSummaries": List[TransformJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUserProfilesResponseTypeDef = TypedDict(
     "ListUserProfilesResponseTypeDef",
     {
         "UserProfiles": List[UserProfileDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+MemberDefinitionExtraOutputTypeDef = TypedDict(
+    "MemberDefinitionExtraOutputTypeDef",
+    {
+        "CognitoMemberDefinition": NotRequired[CognitoMemberDefinitionTypeDef],
+        "OidcMemberDefinition": NotRequired[OidcMemberDefinitionExtraOutputTypeDef],
     },
 )
-MemberDefinitionPaginatorTypeDef = TypedDict(
-    "MemberDefinitionPaginatorTypeDef",
+MemberDefinitionOutputTypeDef = TypedDict(
+    "MemberDefinitionOutputTypeDef",
     {
         "CognitoMemberDefinition": NotRequired[CognitoMemberDefinitionTypeDef],
-        "OidcMemberDefinition": NotRequired[OidcMemberDefinitionPaginatorTypeDef],
+        "OidcMemberDefinition": NotRequired[OidcMemberDefinitionOutputTypeDef],
     },
 )
 MemberDefinitionTypeDef = TypedDict(
     "MemberDefinitionTypeDef",
     {
         "CognitoMemberDefinition": NotRequired[CognitoMemberDefinitionTypeDef],
         "OidcMemberDefinition": NotRequired[OidcMemberDefinitionTypeDef],
@@ -10107,14 +10811,23 @@
     {
         "S3Uri": str,
         "S3DataType": S3ModelDataTypeType,
         "CompressionType": ModelCompressionTypeType,
         "ModelAccessConfig": NotRequired[ModelAccessConfigTypeDef],
     },
 )
+TextGenerationJobConfigOutputTypeDef = TypedDict(
+    "TextGenerationJobConfigOutputTypeDef",
+    {
+        "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
+        "BaseModelName": NotRequired[str],
+        "TextGenerationHyperParameters": NotRequired[Dict[str, str]],
+        "ModelAccessConfig": NotRequired[ModelAccessConfigTypeDef],
+    },
+)
 TextGenerationJobConfigTypeDef = TypedDict(
     "TextGenerationJobConfigTypeDef",
     {
         "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
         "BaseModelName": NotRequired[str],
         "TextGenerationHyperParameters": NotRequired[Mapping[str, str]],
         "ModelAccessConfig": NotRequired[ModelAccessConfigTypeDef],
@@ -10129,14 +10842,22 @@
 ModelInfrastructureConfigTypeDef = TypedDict(
     "ModelInfrastructureConfigTypeDef",
     {
         "InfrastructureType": Literal["RealTimeInference"],
         "RealTimeInferenceConfig": RealTimeInferenceConfigTypeDef,
     },
 )
+RecommendationJobStoppingConditionsOutputTypeDef = TypedDict(
+    "RecommendationJobStoppingConditionsOutputTypeDef",
+    {
+        "MaxInvocations": NotRequired[int],
+        "ModelLatencyThresholds": NotRequired[List[ModelLatencyThresholdTypeDef]],
+        "FlatInvocations": NotRequired[FlatInvocationsType],
+    },
+)
 RecommendationJobStoppingConditionsTypeDef = TypedDict(
     "RecommendationJobStoppingConditionsTypeDef",
     {
         "MaxInvocations": NotRequired[int],
         "ModelLatencyThresholds": NotRequired[Sequence[ModelLatencyThresholdTypeDef]],
         "FlatInvocations": NotRequired[FlatInvocationsType],
     },
@@ -10156,16 +10877,24 @@
 )
 MonitoringResourcesTypeDef = TypedDict(
     "MonitoringResourcesTypeDef",
     {
         "ClusterConfig": MonitoringClusterConfigTypeDef,
     },
 )
-MonitoringDatasetFormatPaginatorTypeDef = TypedDict(
-    "MonitoringDatasetFormatPaginatorTypeDef",
+MonitoringDatasetFormatExtraOutputTypeDef = TypedDict(
+    "MonitoringDatasetFormatExtraOutputTypeDef",
+    {
+        "Csv": NotRequired[MonitoringCsvDatasetFormatTypeDef],
+        "Json": NotRequired[MonitoringJsonDatasetFormatTypeDef],
+        "Parquet": NotRequired[Dict[str, Any]],
+    },
+)
+MonitoringDatasetFormatOutputTypeDef = TypedDict(
+    "MonitoringDatasetFormatOutputTypeDef",
     {
         "Csv": NotRequired[MonitoringCsvDatasetFormatTypeDef],
         "Json": NotRequired[MonitoringJsonDatasetFormatTypeDef],
         "Parquet": NotRequired[Dict[str, Any]],
     },
 )
 MonitoringDatasetFormatTypeDef = TypedDict(
@@ -10280,22 +11009,35 @@
         "ModelDataDownloadTimeoutInSeconds": NotRequired[int],
         "ContainerStartupHealthCheckTimeoutInSeconds": NotRequired[int],
         "EnableSSMAccess": NotRequired[bool],
         "ManagedInstanceScaling": NotRequired[ProductionVariantManagedInstanceScalingTypeDef],
         "RoutingConfig": NotRequired[ProductionVariantRoutingConfigTypeDef],
     },
 )
+ProfilerConfigUnionTypeDef = Union[ProfilerConfigTypeDef, ProfilerConfigExtraOutputTypeDef]
+ProfilerRuleConfigurationUnionTypeDef = Union[
+    ProfilerRuleConfigurationTypeDef, ProfilerRuleConfigurationOutputTypeDef
+]
 SuggestionQueryTypeDef = TypedDict(
     "SuggestionQueryTypeDef",
     {
         "PropertyNameQuery": NotRequired[PropertyNameQueryTypeDef],
     },
 )
-ServiceCatalogProvisioningDetailsPaginatorTypeDef = TypedDict(
-    "ServiceCatalogProvisioningDetailsPaginatorTypeDef",
+ServiceCatalogProvisioningDetailsExtraOutputTypeDef = TypedDict(
+    "ServiceCatalogProvisioningDetailsExtraOutputTypeDef",
+    {
+        "ProductId": str,
+        "ProvisioningArtifactId": NotRequired[str],
+        "PathId": NotRequired[str],
+        "ProvisioningParameters": NotRequired[List[ProvisioningParameterTypeDef]],
+    },
+)
+ServiceCatalogProvisioningDetailsOutputTypeDef = TypedDict(
+    "ServiceCatalogProvisioningDetailsOutputTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": NotRequired[str],
         "PathId": NotRequired[str],
         "ProvisioningParameters": NotRequired[List[ProvisioningParameterTypeDef]],
     },
 )
@@ -10322,25 +11064,40 @@
     },
 )
 QueryLineageResponseTypeDef = TypedDict(
     "QueryLineageResponseTypeDef",
     {
         "Vertices": List[VertexTypeDef],
         "Edges": List[EdgeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RecommendationJobOutputConfigTypeDef = TypedDict(
     "RecommendationJobOutputConfigTypeDef",
     {
         "KmsKeyId": NotRequired[str],
         "CompiledOutputConfig": NotRequired[RecommendationJobCompiledOutputConfigTypeDef],
     },
 )
+RecommendationJobContainerConfigOutputTypeDef = TypedDict(
+    "RecommendationJobContainerConfigOutputTypeDef",
+    {
+        "Domain": NotRequired[str],
+        "Task": NotRequired[str],
+        "Framework": NotRequired[str],
+        "FrameworkVersion": NotRequired[str],
+        "PayloadConfig": NotRequired[RecommendationJobPayloadConfigOutputTypeDef],
+        "NearestModelName": NotRequired[str],
+        "SupportedInstanceTypes": NotRequired[List[str]],
+        "SupportedEndpointType": NotRequired[RecommendationJobSupportedEndpointTypeType],
+        "DataInputConfig": NotRequired[str],
+        "SupportedResponseMIMETypes": NotRequired[List[str]],
+    },
+)
 RecommendationJobContainerConfigTypeDef = TypedDict(
     "RecommendationJobContainerConfigTypeDef",
     {
         "Domain": NotRequired[str],
         "Task": NotRequired[str],
         "Framework": NotRequired[str],
         "FrameworkVersion": NotRequired[str],
@@ -10365,59 +11122,92 @@
     "RenderUiTemplateResponseTypeDef",
     {
         "RenderedContent": str,
         "Errors": List[RenderingErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateTrainingJobRequestRequestTypeDef = TypedDict(
-    "UpdateTrainingJobRequestRequestTypeDef",
-    {
-        "TrainingJobName": str,
-        "ProfilerConfig": NotRequired[ProfilerConfigForUpdateTypeDef],
-        "ProfilerRuleConfigurations": NotRequired[Sequence[ProfilerRuleConfigurationTypeDef]],
-        "ResourceConfig": NotRequired[ResourceConfigForUpdateTypeDef],
-        "RemoteDebugConfig": NotRequired[RemoteDebugConfigForUpdateTypeDef],
-    },
-)
 SearchRequestRequestTypeDef = TypedDict(
     "SearchRequestRequestTypeDef",
     {
         "Resource": ResourceTypeType,
         "SearchExpression": NotRequired["SearchExpressionTypeDef"],
         "SortBy": NotRequired[str],
         "SortOrder": NotRequired[SearchSortOrderType],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
         "CrossAccountFilterOption": NotRequired[CrossAccountFilterOptionType],
         "VisibilityConditions": NotRequired[Sequence[VisibilityConditionsTypeDef]],
     },
 )
+SelectiveExecutionConfigExtraOutputTypeDef = TypedDict(
+    "SelectiveExecutionConfigExtraOutputTypeDef",
+    {
+        "SelectedSteps": List[SelectedStepTypeDef],
+        "SourcePipelineExecutionArn": NotRequired[str],
+    },
+)
+SelectiveExecutionConfigOutputTypeDef = TypedDict(
+    "SelectiveExecutionConfigOutputTypeDef",
+    {
+        "SelectedSteps": List[SelectedStepTypeDef],
+        "SourcePipelineExecutionArn": NotRequired[str],
+    },
+)
 SelectiveExecutionConfigTypeDef = TypedDict(
     "SelectiveExecutionConfigTypeDef",
     {
-        "SelectedSteps": List[SelectedStepTypeDef],
+        "SelectedSteps": Sequence[SelectedStepTypeDef],
         "SourcePipelineExecutionArn": NotRequired[str],
     },
 )
+ShadowModeConfigOutputTypeDef = TypedDict(
+    "ShadowModeConfigOutputTypeDef",
+    {
+        "SourceModelVariantName": str,
+        "ShadowModelVariants": List[ShadowModelVariantConfigTypeDef],
+    },
+)
 ShadowModeConfigTypeDef = TypedDict(
     "ShadowModeConfigTypeDef",
     {
         "SourceModelVariantName": str,
         "ShadowModelVariants": Sequence[ShadowModelVariantConfigTypeDef],
     },
 )
+SourceIpConfigUnionTypeDef = Union[SourceIpConfigTypeDef, SourceIpConfigExtraOutputTypeDef]
+TrafficPatternOutputTypeDef = TypedDict(
+    "TrafficPatternOutputTypeDef",
+    {
+        "TrafficType": NotRequired[TrafficTypeType],
+        "Phases": NotRequired[List[PhaseTypeDef]],
+        "Stairs": NotRequired[StairsTypeDef],
+    },
+)
 TrafficPatternTypeDef = TypedDict(
     "TrafficPatternTypeDef",
     {
         "TrafficType": NotRequired[TrafficTypeType],
         "Phases": NotRequired[Sequence[PhaseTypeDef]],
         "Stairs": NotRequired[StairsTypeDef],
     },
 )
+TimeSeriesForecastingJobConfigOutputTypeDef = TypedDict(
+    "TimeSeriesForecastingJobConfigOutputTypeDef",
+    {
+        "ForecastFrequency": str,
+        "ForecastHorizon": int,
+        "TimeSeriesConfig": TimeSeriesConfigOutputTypeDef,
+        "FeatureSpecificationS3Uri": NotRequired[str],
+        "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
+        "ForecastQuantiles": NotRequired[List[str]],
+        "Transformations": NotRequired[TimeSeriesTransformationsOutputTypeDef],
+        "HolidayConfig": NotRequired[List[HolidayConfigAttributesTypeDef]],
+    },
+)
 TimeSeriesForecastingJobConfigTypeDef = TypedDict(
     "TimeSeriesForecastingJobConfigTypeDef",
     {
         "ForecastFrequency": str,
         "ForecastHorizon": int,
         "TimeSeriesConfig": TimeSeriesConfigTypeDef,
         "FeatureSpecificationS3Uri": NotRequired[str],
@@ -10436,104 +11226,87 @@
 )
 TransformDataSourceTypeDef = TypedDict(
     "TransformDataSourceTypeDef",
     {
         "S3DataSource": TransformS3DataSourceTypeDef,
     },
 )
-WorkforcePaginatorTypeDef = TypedDict(
-    "WorkforcePaginatorTypeDef",
-    {
-        "WorkforceName": str,
-        "WorkforceArn": str,
-        "LastUpdatedDate": NotRequired[datetime],
-        "SourceIpConfig": NotRequired[SourceIpConfigPaginatorTypeDef],
-        "SubDomain": NotRequired[str],
-        "CognitoConfig": NotRequired[CognitoConfigTypeDef],
-        "OidcConfig": NotRequired[OidcConfigForResponseTypeDef],
-        "CreateDate": NotRequired[datetime],
-        "WorkforceVpcConfig": NotRequired[WorkforceVpcConfigResponseTypeDef],
-        "Status": NotRequired[WorkforceStatusType],
-        "FailureReason": NotRequired[str],
-    },
-)
 WorkforceTypeDef = TypedDict(
     "WorkforceTypeDef",
     {
         "WorkforceName": str,
         "WorkforceArn": str,
         "LastUpdatedDate": NotRequired[datetime],
-        "SourceIpConfig": NotRequired[SourceIpConfigTypeDef],
+        "SourceIpConfig": NotRequired[SourceIpConfigOutputTypeDef],
         "SubDomain": NotRequired[str],
         "CognitoConfig": NotRequired[CognitoConfigTypeDef],
         "OidcConfig": NotRequired[OidcConfigForResponseTypeDef],
         "CreateDate": NotRequired[datetime],
         "WorkforceVpcConfig": NotRequired[WorkforceVpcConfigResponseTypeDef],
         "Status": NotRequired[WorkforceStatusType],
         "FailureReason": NotRequired[str],
     },
 )
 ListActionsResponseTypeDef = TypedDict(
     "ListActionsResponseTypeDef",
     {
         "ActionSummaries": List[ActionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "Apps": List[AppDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DomainSettingsForUpdateTypeDef = TypedDict(
     "DomainSettingsForUpdateTypeDef",
     {
         "RStudioServerProDomainSettingsForUpdate": NotRequired[
             RStudioServerProDomainSettingsForUpdateTypeDef
         ],
         "ExecutionRoleIdentityConfig": NotRequired[ExecutionRoleIdentityConfigType],
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "DockerSettings": NotRequired[DockerSettingsTypeDef],
     },
 )
+DomainSettingsOutputTypeDef = TypedDict(
+    "DomainSettingsOutputTypeDef",
+    {
+        "SecurityGroupIds": NotRequired[List[str]],
+        "RStudioServerProDomainSettings": NotRequired[RStudioServerProDomainSettingsTypeDef],
+        "ExecutionRoleIdentityConfig": NotRequired[ExecutionRoleIdentityConfigType],
+        "DockerSettings": NotRequired[DockerSettingsOutputTypeDef],
+    },
+)
 DomainSettingsTypeDef = TypedDict(
     "DomainSettingsTypeDef",
     {
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "RStudioServerProDomainSettings": NotRequired[RStudioServerProDomainSettingsTypeDef],
         "ExecutionRoleIdentityConfig": NotRequired[ExecutionRoleIdentityConfigType],
         "DockerSettings": NotRequired[DockerSettingsTypeDef],
     },
 )
-ArtifactSummaryPaginatorTypeDef = TypedDict(
-    "ArtifactSummaryPaginatorTypeDef",
-    {
-        "ArtifactArn": NotRequired[str],
-        "ArtifactName": NotRequired[str],
-        "Source": NotRequired[ArtifactSourcePaginatorTypeDef],
-        "ArtifactType": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-    },
-)
 ArtifactSummaryTypeDef = TypedDict(
     "ArtifactSummaryTypeDef",
     {
         "ArtifactArn": NotRequired[str],
         "ArtifactName": NotRequired[str],
-        "Source": NotRequired[ArtifactSourceTypeDef],
+        "Source": NotRequired[ArtifactSourceOutputTypeDef],
         "ArtifactType": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
     },
 )
+ArtifactSourceUnionTypeDef = Union[ArtifactSourceTypeDef, ArtifactSourceExtraOutputTypeDef]
 CreateArtifactRequestRequestTypeDef = TypedDict(
     "CreateArtifactRequestRequestTypeDef",
     {
         "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
         "ArtifactName": NotRequired[str],
         "Properties": NotRequired[Mapping[str, str]],
@@ -10544,21 +11317,41 @@
 DeleteArtifactRequestRequestTypeDef = TypedDict(
     "DeleteArtifactRequestRequestTypeDef",
     {
         "ArtifactArn": NotRequired[str],
         "Source": NotRequired[ArtifactSourceTypeDef],
     },
 )
+AsyncInferenceConfigOutputTypeDef = TypedDict(
+    "AsyncInferenceConfigOutputTypeDef",
+    {
+        "OutputConfig": AsyncInferenceOutputConfigOutputTypeDef,
+        "ClientConfig": NotRequired[AsyncInferenceClientConfigTypeDef],
+    },
+)
 AsyncInferenceConfigTypeDef = TypedDict(
     "AsyncInferenceConfigTypeDef",
     {
         "OutputConfig": AsyncInferenceOutputConfigTypeDef,
         "ClientConfig": NotRequired[AsyncInferenceClientConfigTypeDef],
     },
 )
+TabularJobConfigOutputTypeDef = TypedDict(
+    "TabularJobConfigOutputTypeDef",
+    {
+        "TargetAttributeName": str,
+        "CandidateGenerationConfig": NotRequired[CandidateGenerationConfigOutputTypeDef],
+        "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
+        "FeatureSpecificationS3Uri": NotRequired[str],
+        "Mode": NotRequired[AutoMLModeType],
+        "GenerateCandidateDefinitionsOnly": NotRequired[bool],
+        "ProblemType": NotRequired[ProblemTypeType],
+        "SampleWeightAttributeName": NotRequired[str],
+    },
+)
 TabularJobConfigTypeDef = TypedDict(
     "TabularJobConfigTypeDef",
     {
         "TargetAttributeName": str,
         "CandidateGenerationConfig": NotRequired[CandidateGenerationConfigTypeDef],
         "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
         "FeatureSpecificationS3Uri": NotRequired[str],
@@ -10588,46 +11381,70 @@
         "DataSource": NotRequired[AutoMLDataSourceTypeDef],
     },
 )
 ListAutoMLJobsResponseTypeDef = TypedDict(
     "ListAutoMLJobsResponseTypeDef",
     {
         "AutoMLJobSummaries": List[AutoMLJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AutoMLResolvedAttributesTypeDef = TypedDict(
     "AutoMLResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": NotRequired[AutoMLJobObjectiveTypeDef],
         "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
         "AutoMLProblemTypeResolvedAttributes": NotRequired[
             AutoMLProblemTypeResolvedAttributesTypeDef
         ],
     },
 )
+AutoMLJobConfigOutputTypeDef = TypedDict(
+    "AutoMLJobConfigOutputTypeDef",
+    {
+        "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
+        "SecurityConfig": NotRequired[AutoMLSecurityConfigOutputTypeDef],
+        "CandidateGenerationConfig": NotRequired[AutoMLCandidateGenerationConfigOutputTypeDef],
+        "DataSplitConfig": NotRequired[AutoMLDataSplitConfigTypeDef],
+        "Mode": NotRequired[AutoMLModeType],
+    },
+)
+LabelingJobAlgorithmsConfigOutputTypeDef = TypedDict(
+    "LabelingJobAlgorithmsConfigOutputTypeDef",
+    {
+        "LabelingJobAlgorithmSpecificationArn": str,
+        "InitialActiveLearningModelArn": NotRequired[str],
+        "LabelingJobResourceConfig": NotRequired[LabelingJobResourceConfigOutputTypeDef],
+    },
+)
 AutoMLJobConfigTypeDef = TypedDict(
     "AutoMLJobConfigTypeDef",
     {
         "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
         "SecurityConfig": NotRequired[AutoMLSecurityConfigTypeDef],
         "CandidateGenerationConfig": NotRequired[AutoMLCandidateGenerationConfigTypeDef],
         "DataSplitConfig": NotRequired[AutoMLDataSplitConfigTypeDef],
         "Mode": NotRequired[AutoMLModeType],
     },
 )
+AutoMLSecurityConfigUnionTypeDef = Union[
+    AutoMLSecurityConfigTypeDef, AutoMLSecurityConfigOutputTypeDef
+]
 LabelingJobAlgorithmsConfigTypeDef = TypedDict(
     "LabelingJobAlgorithmsConfigTypeDef",
     {
         "LabelingJobAlgorithmSpecificationArn": str,
         "InitialActiveLearningModelArn": NotRequired[str],
         "LabelingJobResourceConfig": NotRequired[LabelingJobResourceConfigTypeDef],
     },
 )
+MonitoringNetworkConfigUnionTypeDef = Union[
+    MonitoringNetworkConfigTypeDef, MonitoringNetworkConfigOutputTypeDef
+]
 ModelMetricsTypeDef = TypedDict(
     "ModelMetricsTypeDef",
     {
         "ModelQuality": NotRequired[ModelQualityTypeDef],
         "ModelDataQuality": NotRequired[ModelDataQualityTypeDef],
         "Bias": NotRequired[BiasTypeDef],
         "Explainability": NotRequired[ExplainabilityTypeDef],
@@ -10675,23 +11492,44 @@
     "BlueGreenUpdatePolicyTypeDef",
     {
         "TrafficRoutingConfiguration": TrafficRoutingConfigTypeDef,
         "TerminationWaitInSeconds": NotRequired[int],
         "MaximumExecutionTimeoutInSeconds": NotRequired[int],
     },
 )
+InferenceExperimentDataStorageConfigUnionTypeDef = Union[
+    InferenceExperimentDataStorageConfigTypeDef, InferenceExperimentDataStorageConfigOutputTypeDef
+]
+DataCaptureConfigUnionTypeDef = Union[DataCaptureConfigTypeDef, DataCaptureConfigOutputTypeDef]
+EndpointInputConfigurationOutputTypeDef = TypedDict(
+    "EndpointInputConfigurationOutputTypeDef",
+    {
+        "InstanceType": NotRequired[ProductionVariantInstanceTypeType],
+        "ServerlessConfig": NotRequired[ProductionVariantServerlessConfigTypeDef],
+        "InferenceSpecificationName": NotRequired[str],
+        "EnvironmentParameterRanges": NotRequired[EnvironmentParameterRangesOutputTypeDef],
+    },
+)
 EndpointInputConfigurationTypeDef = TypedDict(
     "EndpointInputConfigurationTypeDef",
     {
         "InstanceType": NotRequired[ProductionVariantInstanceTypeType],
         "ServerlessConfig": NotRequired[ProductionVariantServerlessConfigTypeDef],
         "InferenceSpecificationName": NotRequired[str],
         "EnvironmentParameterRanges": NotRequired[EnvironmentParameterRangesTypeDef],
     },
 )
+ClarifyExplainerConfigOutputTypeDef = TypedDict(
+    "ClarifyExplainerConfigOutputTypeDef",
+    {
+        "ShapConfig": ClarifyShapConfigTypeDef,
+        "EnableExplanations": NotRequired[str],
+        "InferenceConfig": NotRequired[ClarifyInferenceConfigOutputTypeDef],
+    },
+)
 ClarifyExplainerConfigTypeDef = TypedDict(
     "ClarifyExplainerConfigTypeDef",
     {
         "ShapConfig": ClarifyShapConfigTypeDef,
         "EnableExplanations": NotRequired[str],
         "InferenceConfig": NotRequired[ClarifyInferenceConfigTypeDef],
     },
@@ -10701,15 +11539,15 @@
     {
         "ClusterArn": str,
         "ClusterName": str,
         "ClusterStatus": ClusterStatusType,
         "CreationTime": datetime,
         "FailureMessage": str,
         "InstanceGroups": List[ClusterInstanceGroupDetailsTypeDef],
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateClusterRequestRequestTypeDef = TypedDict(
     "CreateClusterRequestRequestTypeDef",
     {
         "ClusterName": str,
@@ -10736,71 +11574,78 @@
     "ListClusterNodesResponseTypeDef",
     {
         "NextToken": str,
         "ClusterNodeSummaries": List[ClusterNodeSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CodeEditorAppImageConfigUnionTypeDef = Union[
+    CodeEditorAppImageConfigTypeDef, CodeEditorAppImageConfigExtraOutputTypeDef
+]
+JupyterLabAppImageConfigUnionTypeDef = Union[
+    JupyterLabAppImageConfigTypeDef, JupyterLabAppImageConfigExtraOutputTypeDef
+]
 ListCodeRepositoriesOutputTypeDef = TypedDict(
     "ListCodeRepositoriesOutputTypeDef",
     {
         "CodeRepositorySummaryList": List[CodeRepositorySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FeatureDefinitionTypeDef = TypedDict(
     "FeatureDefinitionTypeDef",
     {
         "FeatureName": str,
         "FeatureType": FeatureTypeType,
         "CollectionType": NotRequired[CollectionTypeType],
         "CollectionConfig": NotRequired[CollectionConfigTypeDef],
     },
 )
+DebugHookConfigUnionTypeDef = Union[DebugHookConfigTypeDef, DebugHookConfigExtraOutputTypeDef]
 ListContextsResponseTypeDef = TypedDict(
     "ListContextsResponseTypeDef",
     {
         "ContextSummaries": List[ContextSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-InferenceExperimentSummaryTypeDef = TypedDict(
-    "InferenceExperimentSummaryTypeDef",
-    {
-        "Name": str,
-        "Type": Literal["ShadowMode"],
-        "Status": InferenceExperimentStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "Schedule": NotRequired[InferenceExperimentScheduleTypeDef],
-        "StatusReason": NotRequired[str],
-        "Description": NotRequired[str],
-        "CompletionTime": NotRequired[datetime],
-        "RoleArn": NotRequired[str],
-    },
-)
+InferenceExperimentScheduleUnionTypeDef = Union[
+    InferenceExperimentScheduleTypeDef, InferenceExperimentScheduleExtraOutputTypeDef
+]
 QueryLineageRequestRequestTypeDef = TypedDict(
     "QueryLineageRequestRequestTypeDef",
     {
         "StartArns": NotRequired[Sequence[str]],
         "Direction": NotRequired[DirectionType],
         "IncludeEdges": NotRequired[bool],
         "Filters": NotRequired[QueryFiltersTypeDef],
         "MaxDepth": NotRequired[int],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-ChannelPaginatorTypeDef = TypedDict(
-    "ChannelPaginatorTypeDef",
+ChannelExtraOutputTypeDef = TypedDict(
+    "ChannelExtraOutputTypeDef",
+    {
+        "ChannelName": str,
+        "DataSource": DataSourceExtraOutputTypeDef,
+        "ContentType": NotRequired[str],
+        "CompressionType": NotRequired[CompressionTypeType],
+        "RecordWrapperType": NotRequired[RecordWrapperType],
+        "InputMode": NotRequired[TrainingInputModeType],
+        "ShuffleConfig": NotRequired[ShuffleConfigTypeDef],
+    },
+)
+ChannelOutputTypeDef = TypedDict(
+    "ChannelOutputTypeDef",
     {
         "ChannelName": str,
-        "DataSource": DataSourcePaginatorTypeDef,
+        "DataSource": DataSourceOutputTypeDef,
         "ContentType": NotRequired[str],
         "CompressionType": NotRequired[CompressionTypeType],
         "RecordWrapperType": NotRequired[RecordWrapperType],
         "InputMode": NotRequired[TrainingInputModeType],
         "ShuffleConfig": NotRequired[ShuffleConfigTypeDef],
     },
 )
@@ -10821,27 +11666,61 @@
     {
         "InputName": str,
         "AppManaged": NotRequired[bool],
         "S3Input": NotRequired[ProcessingS3InputTypeDef],
         "DatasetDefinition": NotRequired[DatasetDefinitionTypeDef],
     },
 )
+DefaultSpaceSettingsOutputTypeDef = TypedDict(
+    "DefaultSpaceSettingsOutputTypeDef",
+    {
+        "ExecutionRole": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsOutputTypeDef],
+        "KernelGatewayAppSettings": NotRequired[KernelGatewayAppSettingsOutputTypeDef],
+        "JupyterLabAppSettings": NotRequired[JupyterLabAppSettingsOutputTypeDef],
+        "SpaceStorageSettings": NotRequired[DefaultSpaceStorageSettingsTypeDef],
+        "CustomPosixUserConfig": NotRequired[CustomPosixUserConfigTypeDef],
+        "CustomFileSystemConfigs": NotRequired[List[CustomFileSystemConfigTypeDef]],
+    },
+)
 DefaultSpaceSettingsTypeDef = TypedDict(
     "DefaultSpaceSettingsTypeDef",
     {
         "ExecutionRole": NotRequired[str],
         "SecurityGroups": NotRequired[Sequence[str]],
         "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsTypeDef],
         "KernelGatewayAppSettings": NotRequired[KernelGatewayAppSettingsTypeDef],
         "JupyterLabAppSettings": NotRequired[JupyterLabAppSettingsTypeDef],
         "SpaceStorageSettings": NotRequired[DefaultSpaceStorageSettingsTypeDef],
         "CustomPosixUserConfig": NotRequired[CustomPosixUserConfigTypeDef],
         "CustomFileSystemConfigs": NotRequired[Sequence[CustomFileSystemConfigTypeDef]],
     },
 )
+UserSettingsOutputTypeDef = TypedDict(
+    "UserSettingsOutputTypeDef",
+    {
+        "ExecutionRole": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "SharingSettings": NotRequired[SharingSettingsTypeDef],
+        "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsOutputTypeDef],
+        "KernelGatewayAppSettings": NotRequired[KernelGatewayAppSettingsOutputTypeDef],
+        "TensorBoardAppSettings": NotRequired[TensorBoardAppSettingsTypeDef],
+        "RStudioServerProAppSettings": NotRequired[RStudioServerProAppSettingsTypeDef],
+        "RSessionAppSettings": NotRequired[RSessionAppSettingsOutputTypeDef],
+        "CanvasAppSettings": NotRequired[CanvasAppSettingsOutputTypeDef],
+        "CodeEditorAppSettings": NotRequired[CodeEditorAppSettingsOutputTypeDef],
+        "JupyterLabAppSettings": NotRequired[JupyterLabAppSettingsOutputTypeDef],
+        "SpaceStorageSettings": NotRequired[DefaultSpaceStorageSettingsTypeDef],
+        "DefaultLandingUri": NotRequired[str],
+        "StudioWebPortal": NotRequired[StudioWebPortalType],
+        "CustomPosixUserConfig": NotRequired[CustomPosixUserConfigTypeDef],
+        "CustomFileSystemConfigs": NotRequired[List[CustomFileSystemConfigTypeDef]],
+    },
+)
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "ExecutionRole": NotRequired[str],
         "SecurityGroups": NotRequired[Sequence[str]],
         "SharingSettings": NotRequired[SharingSettingsTypeDef],
         "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsTypeDef],
@@ -10866,14 +11745,31 @@
         "Container": NotRequired[InferenceComponentContainerSpecificationSummaryTypeDef],
         "StartupParameters": NotRequired[InferenceComponentStartupParametersTypeDef],
         "ComputeResourceRequirements": NotRequired[
             InferenceComponentComputeResourceRequirementsTypeDef
         ],
     },
 )
+DescribeEdgeDeploymentPlanResponseTypeDef = TypedDict(
+    "DescribeEdgeDeploymentPlanResponseTypeDef",
+    {
+        "EdgeDeploymentPlanArn": str,
+        "EdgeDeploymentPlanName": str,
+        "ModelConfigs": List[EdgeDeploymentModelConfigTypeDef],
+        "DeviceFleetName": str,
+        "EdgeDeploymentSuccess": int,
+        "EdgeDeploymentPending": int,
+        "EdgeDeploymentFailed": int,
+        "Stages": List[DeploymentStageStatusSummaryTypeDef],
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
 CreateEdgeDeploymentPlanRequestRequestTypeDef = TypedDict(
     "CreateEdgeDeploymentPlanRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "ModelConfigs": Sequence[EdgeDeploymentModelConfigTypeDef],
         "DeviceFleetName": str,
         "Stages": NotRequired[Sequence[DeploymentStageTypeDef]],
@@ -10883,87 +11779,90 @@
 CreateEdgeDeploymentStageRequestRequestTypeDef = TypedDict(
     "CreateEdgeDeploymentStageRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "Stages": Sequence[DeploymentStageTypeDef],
     },
 )
-DescribeEdgeDeploymentPlanResponseTypeDef = TypedDict(
-    "DescribeEdgeDeploymentPlanResponseTypeDef",
-    {
-        "EdgeDeploymentPlanArn": str,
-        "EdgeDeploymentPlanName": str,
-        "ModelConfigs": List[EdgeDeploymentModelConfigTypeDef],
-        "DeviceFleetName": str,
-        "EdgeDeploymentSuccess": int,
-        "EdgeDeploymentPending": int,
-        "EdgeDeploymentFailed": int,
-        "Stages": List[DeploymentStageStatusSummaryTypeDef],
-        "NextToken": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "ExperimentSummaries": List[ExperimentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListFeatureGroupsResponseTypeDef = TypedDict(
     "ListFeatureGroupsResponseTypeDef",
     {
         "FeatureGroupSummaries": List[FeatureGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+ListInferenceExperimentsResponseTypeDef = TypedDict(
+    "ListInferenceExperimentsResponseTypeDef",
+    {
+        "InferenceExperiments": List[InferenceExperimentSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTrainingJobsResponseTypeDef = TypedDict(
     "ListTrainingJobsResponseTypeDef",
     {
         "TrainingJobSummaries": List[TrainingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTrialsResponseTypeDef = TypedDict(
     "ListTrialsResponseTypeDef",
     {
         "TrialSummaries": List[TrialSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef = TypedDict(
     "UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef",
     {
         "EndpointName": str,
         "DesiredWeightsAndCapacities": Sequence[DesiredWeightAndCapacityTypeDef],
     },
 )
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "DeviceSummaries": List[DeviceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DriftCheckBaselinesTypeDef = TypedDict(
     "DriftCheckBaselinesTypeDef",
     {
         "Bias": NotRequired[DriftCheckBiasTypeDef],
         "Explainability": NotRequired[DriftCheckExplainabilityTypeDef],
         "ModelQuality": NotRequired[DriftCheckModelQualityTypeDef],
         "ModelDataQuality": NotRequired[DriftCheckModelDataQualityTypeDef],
     },
 )
+SpaceSettingsOutputTypeDef = TypedDict(
+    "SpaceSettingsOutputTypeDef",
+    {
+        "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsOutputTypeDef],
+        "KernelGatewayAppSettings": NotRequired[KernelGatewayAppSettingsOutputTypeDef],
+        "CodeEditorAppSettings": NotRequired[SpaceCodeEditorAppSettingsTypeDef],
+        "JupyterLabAppSettings": NotRequired[SpaceJupyterLabAppSettingsOutputTypeDef],
+        "AppType": NotRequired[AppTypeType],
+        "SpaceStorageSettings": NotRequired[SpaceStorageSettingsTypeDef],
+        "CustomFileSystems": NotRequired[List[CustomFileSystemTypeDef]],
+    },
+)
 SpaceSettingsSummaryTypeDef = TypedDict(
     "SpaceSettingsSummaryTypeDef",
     {
         "AppType": NotRequired[AppTypeType],
         "SpaceStorageSettings": NotRequired[SpaceStorageSettingsTypeDef],
     },
 )
@@ -11011,26 +11910,31 @@
         "Operator": NotRequired[BooleanOperatorType],
     },
 )
 ListTrainingJobsForHyperParameterTuningJobResponseTypeDef = TypedDict(
     "ListTrainingJobsForHyperParameterTuningJobResponseTypeDef",
     {
         "TrainingJobSummaries": List[HyperParameterTrainingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+NetworkConfigUnionTypeDef = Union[NetworkConfigTypeDef, NetworkConfigExtraOutputTypeDef]
 ListHyperParameterTuningJobsResponseTypeDef = TypedDict(
     "ListHyperParameterTuningJobsResponseTypeDef",
     {
         "HyperParameterTuningJobSummaries": List[HyperParameterTuningJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+HyperParameterTuningJobWarmStartConfigUnionTypeDef = Union[
+    HyperParameterTuningJobWarmStartConfigTypeDef,
+    HyperParameterTuningJobWarmStartConfigExtraOutputTypeDef,
+]
 AssociationSummaryTypeDef = TypedDict(
     "AssociationSummaryTypeDef",
     {
         "SourceArn": NotRequired[str],
         "DestinationArn": NotRequired[str],
         "SourceType": NotRequired[str],
         "DestinationType": NotRequired[str],
@@ -11061,15 +11965,15 @@
     },
 )
 DescribeArtifactResponseTypeDef = TypedDict(
     "DescribeArtifactResponseTypeDef",
     {
         "ArtifactName": str,
         "ArtifactArn": str,
-        "Source": ArtifactSourceTypeDef,
+        "Source": ArtifactSourceOutputTypeDef,
         "ArtifactType": str,
         "Properties": Dict[str, str],
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
@@ -11333,42 +12237,60 @@
     "UpdateInferenceComponentInputRequestTypeDef",
     {
         "InferenceComponentName": str,
         "Specification": NotRequired[InferenceComponentSpecificationTypeDef],
         "RuntimeConfig": NotRequired[InferenceComponentRuntimeConfigTypeDef],
     },
 )
-ListInferenceExperimentsResponsePaginatorTypeDef = TypedDict(
-    "ListInferenceExperimentsResponsePaginatorTypeDef",
+ResourceConfigUnionTypeDef = Union[ResourceConfigTypeDef, ResourceConfigExtraOutputTypeDef]
+HyperParameterSpecificationOutputTypeDef = TypedDict(
+    "HyperParameterSpecificationOutputTypeDef",
     {
-        "InferenceExperiments": List[InferenceExperimentSummaryPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "Type": ParameterTypeType,
+        "Description": NotRequired[str],
+        "Range": NotRequired[ParameterRangeOutputTypeDef],
+        "IsTunable": NotRequired[bool],
+        "IsRequired": NotRequired[bool],
+        "DefaultValue": NotRequired[str],
     },
 )
 HyperParameterSpecificationTypeDef = TypedDict(
     "HyperParameterSpecificationTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Description": NotRequired[str],
         "Range": NotRequired[ParameterRangeTypeDef],
         "IsTunable": NotRequired[bool],
         "IsRequired": NotRequired[bool],
         "DefaultValue": NotRequired[str],
     },
 )
-HyperParameterTuningJobConfigPaginatorTypeDef = TypedDict(
-    "HyperParameterTuningJobConfigPaginatorTypeDef",
+HyperParameterTuningJobConfigExtraOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobConfigExtraOutputTypeDef",
+    {
+        "Strategy": HyperParameterTuningJobStrategyTypeType,
+        "ResourceLimits": ResourceLimitsTypeDef,
+        "StrategyConfig": NotRequired[HyperParameterTuningJobStrategyConfigTypeDef],
+        "HyperParameterTuningJobObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
+        "ParameterRanges": NotRequired[ParameterRangesExtraOutputTypeDef],
+        "TrainingJobEarlyStoppingType": NotRequired[TrainingJobEarlyStoppingTypeType],
+        "TuningJobCompletionCriteria": NotRequired[TuningJobCompletionCriteriaTypeDef],
+        "RandomSeed": NotRequired[int],
+    },
+)
+HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobConfigOutputTypeDef",
     {
         "Strategy": HyperParameterTuningJobStrategyTypeType,
         "ResourceLimits": ResourceLimitsTypeDef,
         "StrategyConfig": NotRequired[HyperParameterTuningJobStrategyConfigTypeDef],
         "HyperParameterTuningJobObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
-        "ParameterRanges": NotRequired[ParameterRangesPaginatorTypeDef],
+        "ParameterRanges": NotRequired[ParameterRangesOutputTypeDef],
         "TrainingJobEarlyStoppingType": NotRequired[TrainingJobEarlyStoppingTypeType],
         "TuningJobCompletionCriteria": NotRequired[TuningJobCompletionCriteriaTypeDef],
         "RandomSeed": NotRequired[int],
     },
 )
 HyperParameterTuningJobConfigTypeDef = TypedDict(
     "HyperParameterTuningJobConfigTypeDef",
@@ -11379,142 +12301,106 @@
         "HyperParameterTuningJobObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
         "ParameterRanges": NotRequired[ParameterRangesTypeDef],
         "TrainingJobEarlyStoppingType": NotRequired[TrainingJobEarlyStoppingTypeType],
         "TuningJobCompletionCriteria": NotRequired[TuningJobCompletionCriteriaTypeDef],
         "RandomSeed": NotRequired[int],
     },
 )
-AppImageConfigDetailsPaginatorTypeDef = TypedDict(
-    "AppImageConfigDetailsPaginatorTypeDef",
+AppImageConfigDetailsTypeDef = TypedDict(
+    "AppImageConfigDetailsTypeDef",
     {
         "AppImageConfigArn": NotRequired[str],
         "AppImageConfigName": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
-        "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigPaginatorTypeDef],
-        "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigPaginatorTypeDef],
-        "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigPaginatorTypeDef],
+        "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigOutputTypeDef],
+        "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigOutputTypeDef],
+        "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigOutputTypeDef],
     },
 )
-AppImageConfigDetailsTypeDef = TypedDict(
-    "AppImageConfigDetailsTypeDef",
+DescribeAppImageConfigResponseTypeDef = TypedDict(
+    "DescribeAppImageConfigResponseTypeDef",
     {
-        "AppImageConfigArn": NotRequired[str],
-        "AppImageConfigName": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigTypeDef],
-        "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigTypeDef],
-        "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigTypeDef],
+        "AppImageConfigArn": str,
+        "AppImageConfigName": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "KernelGatewayImageConfig": KernelGatewayImageConfigOutputTypeDef,
+        "JupyterLabAppImageConfig": JupyterLabAppImageConfigOutputTypeDef,
+        "CodeEditorAppImageConfig": CodeEditorAppImageConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateAppImageConfigRequestRequestTypeDef = TypedDict(
     "CreateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigTypeDef],
         "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigTypeDef],
         "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigTypeDef],
     },
 )
-DescribeAppImageConfigResponseTypeDef = TypedDict(
-    "DescribeAppImageConfigResponseTypeDef",
-    {
-        "AppImageConfigArn": str,
-        "AppImageConfigName": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "KernelGatewayImageConfig": KernelGatewayImageConfigTypeDef,
-        "JupyterLabAppImageConfig": JupyterLabAppImageConfigTypeDef,
-        "CodeEditorAppImageConfig": CodeEditorAppImageConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+KernelGatewayImageConfigUnionTypeDef = Union[
+    KernelGatewayImageConfigTypeDef, KernelGatewayImageConfigExtraOutputTypeDef
+]
 UpdateAppImageConfigRequestRequestTypeDef = TypedDict(
     "UpdateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
         "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigTypeDef],
         "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigTypeDef],
         "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigTypeDef],
     },
 )
 ListLabelingJobsForWorkteamResponseTypeDef = TypedDict(
     "ListLabelingJobsForWorkteamResponseTypeDef",
     {
         "LabelingJobSummaryList": List[LabelingJobForWorkteamSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-LabelingJobInputConfigPaginatorTypeDef = TypedDict(
-    "LabelingJobInputConfigPaginatorTypeDef",
+LabelingJobInputConfigExtraOutputTypeDef = TypedDict(
+    "LabelingJobInputConfigExtraOutputTypeDef",
     {
         "DataSource": LabelingJobDataSourceTypeDef,
-        "DataAttributes": NotRequired[LabelingJobDataAttributesPaginatorTypeDef],
+        "DataAttributes": NotRequired[LabelingJobDataAttributesExtraOutputTypeDef],
     },
 )
-LabelingJobInputConfigTypeDef = TypedDict(
-    "LabelingJobInputConfigTypeDef",
+LabelingJobInputConfigOutputTypeDef = TypedDict(
+    "LabelingJobInputConfigOutputTypeDef",
     {
         "DataSource": LabelingJobDataSourceTypeDef,
-        "DataAttributes": NotRequired[LabelingJobDataAttributesTypeDef],
-    },
-)
-WorkteamPaginatorTypeDef = TypedDict(
-    "WorkteamPaginatorTypeDef",
-    {
-        "WorkteamName": str,
-        "MemberDefinitions": List[MemberDefinitionPaginatorTypeDef],
-        "WorkteamArn": str,
-        "Description": str,
-        "WorkforceArn": NotRequired[str],
-        "ProductListingIds": NotRequired[List[str]],
-        "SubDomain": NotRequired[str],
-        "CreateDate": NotRequired[datetime],
-        "LastUpdatedDate": NotRequired[datetime],
-        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
+        "DataAttributes": NotRequired[LabelingJobDataAttributesOutputTypeDef],
     },
 )
-CreateWorkteamRequestRequestTypeDef = TypedDict(
-    "CreateWorkteamRequestRequestTypeDef",
-    {
-        "WorkteamName": str,
-        "MemberDefinitions": Sequence[MemberDefinitionTypeDef],
-        "Description": str,
-        "WorkforceName": NotRequired[str],
-        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
-UpdateWorkteamRequestRequestTypeDef = TypedDict(
-    "UpdateWorkteamRequestRequestTypeDef",
+LabelingJobInputConfigTypeDef = TypedDict(
+    "LabelingJobInputConfigTypeDef",
     {
-        "WorkteamName": str,
-        "MemberDefinitions": NotRequired[Sequence[MemberDefinitionTypeDef]],
-        "Description": NotRequired[str],
-        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
+        "DataSource": LabelingJobDataSourceTypeDef,
+        "DataAttributes": NotRequired[LabelingJobDataAttributesTypeDef],
     },
 )
 WorkteamTypeDef = TypedDict(
     "WorkteamTypeDef",
     {
         "WorkteamName": str,
-        "MemberDefinitions": List[MemberDefinitionTypeDef],
+        "MemberDefinitions": List[MemberDefinitionOutputTypeDef],
         "WorkteamArn": str,
         "Description": str,
         "WorkforceArn": NotRequired[str],
         "ProductListingIds": NotRequired[List[str]],
         "SubDomain": NotRequired[str],
         "CreateDate": NotRequired[datetime],
         "LastUpdatedDate": NotRequired[datetime],
         "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
     },
 )
+MemberDefinitionUnionTypeDef = Union[MemberDefinitionTypeDef, MemberDefinitionExtraOutputTypeDef]
 TargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
     "TargetTrackingScalingPolicyConfigurationTypeDef",
     {
         "MetricSpecification": NotRequired[MetricSpecificationTypeDef],
         "TargetValue": NotRequired[float],
     },
 )
@@ -11549,14 +12435,17 @@
     "ModelVariantConfigTypeDef",
     {
         "ModelName": str,
         "VariantName": str,
         "InfrastructureConfig": ModelInfrastructureConfigTypeDef,
     },
 )
+RecommendationJobStoppingConditionsUnionTypeDef = Union[
+    RecommendationJobStoppingConditionsTypeDef, RecommendationJobStoppingConditionsOutputTypeDef
+]
 ListModelMetadataRequestListModelMetadataPaginateTypeDef = TypedDict(
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     {
         "SearchExpression": NotRequired[ModelMetadataSearchExpressionTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -11564,19 +12453,36 @@
     "ListModelMetadataRequestRequestTypeDef",
     {
         "SearchExpression": NotRequired[ModelMetadataSearchExpressionTypeDef],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
 )
-BatchTransformInputPaginatorTypeDef = TypedDict(
-    "BatchTransformInputPaginatorTypeDef",
+BatchTransformInputExtraOutputTypeDef = TypedDict(
+    "BatchTransformInputExtraOutputTypeDef",
+    {
+        "DataCapturedDestinationS3Uri": str,
+        "DatasetFormat": MonitoringDatasetFormatExtraOutputTypeDef,
+        "LocalPath": str,
+        "S3InputMode": NotRequired[ProcessingS3InputModeType],
+        "S3DataDistributionType": NotRequired[ProcessingS3DataDistributionTypeType],
+        "FeaturesAttribute": NotRequired[str],
+        "InferenceAttribute": NotRequired[str],
+        "ProbabilityAttribute": NotRequired[str],
+        "ProbabilityThresholdAttribute": NotRequired[float],
+        "StartTimeOffset": NotRequired[str],
+        "EndTimeOffset": NotRequired[str],
+        "ExcludeFeaturesAttribute": NotRequired[str],
+    },
+)
+BatchTransformInputOutputTypeDef = TypedDict(
+    "BatchTransformInputOutputTypeDef",
     {
         "DataCapturedDestinationS3Uri": str,
-        "DatasetFormat": MonitoringDatasetFormatPaginatorTypeDef,
+        "DatasetFormat": MonitoringDatasetFormatOutputTypeDef,
         "LocalPath": str,
         "S3InputMode": NotRequired[ProcessingS3InputModeType],
         "S3DataDistributionType": NotRequired[ProcessingS3DataDistributionTypeType],
         "FeaturesAttribute": NotRequired[str],
         "InferenceAttribute": NotRequired[str],
         "ProbabilityAttribute": NotRequired[str],
         "ProbabilityThresholdAttribute": NotRequired[float],
@@ -11598,16 +12504,23 @@
         "ProbabilityAttribute": NotRequired[str],
         "ProbabilityThresholdAttribute": NotRequired[float],
         "StartTimeOffset": NotRequired[str],
         "EndTimeOffset": NotRequired[str],
         "ExcludeFeaturesAttribute": NotRequired[str],
     },
 )
-MonitoringOutputConfigPaginatorTypeDef = TypedDict(
-    "MonitoringOutputConfigPaginatorTypeDef",
+MonitoringOutputConfigExtraOutputTypeDef = TypedDict(
+    "MonitoringOutputConfigExtraOutputTypeDef",
+    {
+        "MonitoringOutputs": List[MonitoringOutputTypeDef],
+        "KmsKeyId": NotRequired[str],
+    },
+)
+MonitoringOutputConfigOutputTypeDef = TypedDict(
+    "MonitoringOutputConfigOutputTypeDef",
     {
         "MonitoringOutputs": List[MonitoringOutputTypeDef],
         "KmsKeyId": NotRequired[str],
     },
 )
 MonitoringOutputConfigTypeDef = TypedDict(
     "MonitoringOutputConfigTypeDef",
@@ -11644,87 +12557,74 @@
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "ModelDigests": ModelDigestsTypeDef,
         "RoleArn": str,
         "InputConfig": InputConfigTypeDef,
         "OutputConfig": OutputConfigTypeDef,
-        "VpcConfig": NeoVpcConfigTypeDef,
+        "VpcConfig": NeoVpcConfigOutputTypeDef,
         "DerivedInformation": DerivedInformationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PendingDeploymentSummaryTypeDef = TypedDict(
     "PendingDeploymentSummaryTypeDef",
     {
         "EndpointConfigName": str,
         "ProductionVariants": NotRequired[List[PendingProductionVariantSummaryTypeDef]],
         "StartTime": NotRequired[datetime],
         "ShadowProductionVariants": NotRequired[List[PendingProductionVariantSummaryTypeDef]],
     },
 )
-ProcessingOutputConfigPaginatorTypeDef = TypedDict(
-    "ProcessingOutputConfigPaginatorTypeDef",
+ProcessingOutputConfigExtraOutputTypeDef = TypedDict(
+    "ProcessingOutputConfigExtraOutputTypeDef",
+    {
+        "Outputs": List[ProcessingOutputTypeDef],
+        "KmsKeyId": NotRequired[str],
+    },
+)
+ProcessingOutputConfigOutputTypeDef = TypedDict(
+    "ProcessingOutputConfigOutputTypeDef",
     {
         "Outputs": List[ProcessingOutputTypeDef],
         "KmsKeyId": NotRequired[str],
     },
 )
 ProcessingOutputConfigTypeDef = TypedDict(
     "ProcessingOutputConfigTypeDef",
     {
         "Outputs": Sequence[ProcessingOutputTypeDef],
         "KmsKeyId": NotRequired[str],
     },
 )
+UpdateTrainingJobRequestRequestTypeDef = TypedDict(
+    "UpdateTrainingJobRequestRequestTypeDef",
+    {
+        "TrainingJobName": str,
+        "ProfilerConfig": NotRequired[ProfilerConfigForUpdateTypeDef],
+        "ProfilerRuleConfigurations": NotRequired[Sequence[ProfilerRuleConfigurationUnionTypeDef]],
+        "ResourceConfig": NotRequired[ResourceConfigForUpdateTypeDef],
+        "RemoteDebugConfig": NotRequired[RemoteDebugConfigForUpdateTypeDef],
+    },
+)
 GetSearchSuggestionsRequestRequestTypeDef = TypedDict(
     "GetSearchSuggestionsRequestRequestTypeDef",
     {
         "Resource": ResourceTypeType,
         "SuggestionQuery": NotRequired[SuggestionQueryTypeDef],
     },
 )
-ProjectPaginatorTypeDef = TypedDict(
-    "ProjectPaginatorTypeDef",
-    {
-        "ProjectArn": NotRequired[str],
-        "ProjectName": NotRequired[str],
-        "ProjectId": NotRequired[str],
-        "ProjectDescription": NotRequired[str],
-        "ServiceCatalogProvisioningDetails": NotRequired[
-            ServiceCatalogProvisioningDetailsPaginatorTypeDef
-        ],
-        "ServiceCatalogProvisionedProductDetails": NotRequired[
-            ServiceCatalogProvisionedProductDetailsTypeDef
-        ],
-        "ProjectStatus": NotRequired[ProjectStatusType],
-        "CreatedBy": NotRequired[UserContextTypeDef],
-        "CreationTime": NotRequired[datetime],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "LastModifiedTime": NotRequired[datetime],
-        "LastModifiedBy": NotRequired[UserContextTypeDef],
-    },
-)
-CreateProjectInputRequestTypeDef = TypedDict(
-    "CreateProjectInputRequestTypeDef",
-    {
-        "ProjectName": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
-        "ProjectDescription": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 DescribeProjectOutputTypeDef = TypedDict(
     "DescribeProjectOutputTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "ProjectId": str,
         "ProjectDescription": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsOutputTypeDef,
         "ServiceCatalogProvisionedProductDetails": ServiceCatalogProvisionedProductDetailsTypeDef,
         "ProjectStatus": ProjectStatusType,
         "CreatedBy": UserContextTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11733,51 +12633,96 @@
 ProjectTypeDef = TypedDict(
     "ProjectTypeDef",
     {
         "ProjectArn": NotRequired[str],
         "ProjectName": NotRequired[str],
         "ProjectId": NotRequired[str],
         "ProjectDescription": NotRequired[str],
-        "ServiceCatalogProvisioningDetails": NotRequired[ServiceCatalogProvisioningDetailsTypeDef],
+        "ServiceCatalogProvisioningDetails": NotRequired[
+            ServiceCatalogProvisioningDetailsOutputTypeDef
+        ],
         "ServiceCatalogProvisionedProductDetails": NotRequired[
             ServiceCatalogProvisionedProductDetailsTypeDef
         ],
         "ProjectStatus": NotRequired[ProjectStatusType],
         "CreatedBy": NotRequired[UserContextTypeDef],
         "CreationTime": NotRequired[datetime],
         "Tags": NotRequired[List[TagTypeDef]],
         "LastModifiedTime": NotRequired[datetime],
         "LastModifiedBy": NotRequired[UserContextTypeDef],
     },
 )
+CreateProjectInputRequestTypeDef = TypedDict(
+    "CreateProjectInputRequestTypeDef",
+    {
+        "ProjectName": str,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
+        "ProjectDescription": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+ServiceCatalogProvisioningDetailsUnionTypeDef = Union[
+    ServiceCatalogProvisioningDetailsTypeDef, ServiceCatalogProvisioningDetailsExtraOutputTypeDef
+]
 UpdateProjectInputRequestTypeDef = TypedDict(
     "UpdateProjectInputRequestTypeDef",
     {
         "ProjectName": str,
         "ProjectDescription": NotRequired[str],
         "ServiceCatalogProvisioningUpdateDetails": NotRequired[
             ServiceCatalogProvisioningUpdateDetailsTypeDef
         ],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+HumanLoopConfigOutputTypeDef = TypedDict(
+    "HumanLoopConfigOutputTypeDef",
+    {
+        "WorkteamArn": str,
+        "HumanTaskUiArn": str,
+        "TaskTitle": str,
+        "TaskDescription": str,
+        "TaskCount": int,
+        "TaskAvailabilityLifetimeInSeconds": NotRequired[int],
+        "TaskTimeLimitInSeconds": NotRequired[int],
+        "TaskKeywords": NotRequired[List[str]],
+        "PublicWorkforceTaskPrice": NotRequired[PublicWorkforceTaskPriceTypeDef],
+    },
+)
 HumanLoopConfigTypeDef = TypedDict(
     "HumanLoopConfigTypeDef",
     {
         "WorkteamArn": str,
         "HumanTaskUiArn": str,
         "TaskTitle": str,
         "TaskDescription": str,
         "TaskCount": int,
         "TaskAvailabilityLifetimeInSeconds": NotRequired[int],
         "TaskTimeLimitInSeconds": NotRequired[int],
         "TaskKeywords": NotRequired[Sequence[str]],
         "PublicWorkforceTaskPrice": NotRequired[PublicWorkforceTaskPriceTypeDef],
     },
 )
+HumanTaskConfigOutputTypeDef = TypedDict(
+    "HumanTaskConfigOutputTypeDef",
+    {
+        "WorkteamArn": str,
+        "UiConfig": UiConfigTypeDef,
+        "PreHumanTaskLambdaArn": str,
+        "TaskTitle": str,
+        "TaskDescription": str,
+        "NumberOfHumanWorkersPerDataObject": int,
+        "TaskTimeLimitInSeconds": int,
+        "AnnotationConsolidationConfig": AnnotationConsolidationConfigTypeDef,
+        "TaskKeywords": NotRequired[List[str]],
+        "TaskAvailabilityLifetimeInSeconds": NotRequired[int],
+        "MaxConcurrentTaskCount": NotRequired[int],
+        "PublicWorkforceTaskPrice": NotRequired[PublicWorkforceTaskPriceTypeDef],
+    },
+)
 HumanTaskConfigTypeDef = TypedDict(
     "HumanTaskConfigTypeDef",
     {
         "WorkteamArn": str,
         "UiConfig": UiConfigTypeDef,
         "PreHumanTaskLambdaArn": str,
         "TaskTitle": str,
@@ -11802,15 +12747,15 @@
         "PipelineExperimentConfig": PipelineExperimentConfigTypeDef,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
-        "SelectiveExecutionConfig": SelectiveExecutionConfigTypeDef,
+        "SelectiveExecutionConfig": SelectiveExecutionConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PipelineExecutionTypeDef = TypedDict(
     "PipelineExecutionTypeDef",
     {
         "PipelineArn": NotRequired[str],
@@ -11821,32 +12766,49 @@
         "PipelineExperimentConfig": NotRequired[PipelineExperimentConfigTypeDef],
         "FailureReason": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
         "CreatedBy": NotRequired[UserContextTypeDef],
         "LastModifiedBy": NotRequired[UserContextTypeDef],
         "ParallelismConfiguration": NotRequired[ParallelismConfigurationTypeDef],
-        "SelectiveExecutionConfig": NotRequired[SelectiveExecutionConfigTypeDef],
+        "SelectiveExecutionConfig": NotRequired[SelectiveExecutionConfigOutputTypeDef],
         "PipelineParameters": NotRequired[List[ParameterTypeDef]],
     },
 )
+SelectiveExecutionConfigUnionTypeDef = Union[
+    SelectiveExecutionConfigTypeDef, SelectiveExecutionConfigExtraOutputTypeDef
+]
 StartPipelineExecutionRequestRequestTypeDef = TypedDict(
     "StartPipelineExecutionRequestRequestTypeDef",
     {
         "PipelineName": str,
         "ClientRequestToken": str,
         "PipelineExecutionDisplayName": NotRequired[str],
         "PipelineParameters": NotRequired[Sequence[ParameterTypeDef]],
         "PipelineExecutionDescription": NotRequired[str],
         "ParallelismConfiguration": NotRequired[ParallelismConfigurationTypeDef],
         "SelectiveExecutionConfig": NotRequired[SelectiveExecutionConfigTypeDef],
     },
 )
-AlgorithmSpecificationPaginatorTypeDef = TypedDict(
-    "AlgorithmSpecificationPaginatorTypeDef",
+ShadowModeConfigUnionTypeDef = Union[ShadowModeConfigTypeDef, ShadowModeConfigOutputTypeDef]
+AlgorithmSpecificationExtraOutputTypeDef = TypedDict(
+    "AlgorithmSpecificationExtraOutputTypeDef",
+    {
+        "TrainingInputMode": TrainingInputModeType,
+        "TrainingImage": NotRequired[str],
+        "AlgorithmName": NotRequired[str],
+        "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
+        "EnableSageMakerMetricsTimeSeries": NotRequired[bool],
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+        "TrainingImageConfig": NotRequired[TrainingImageConfigTypeDef],
+    },
+)
+AlgorithmSpecificationOutputTypeDef = TypedDict(
+    "AlgorithmSpecificationOutputTypeDef",
     {
         "TrainingInputMode": TrainingInputModeType,
         "TrainingImage": NotRequired[str],
         "AlgorithmName": NotRequired[str],
         "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
         "EnableSageMakerMetricsTimeSeries": NotRequired[bool],
         "ContainerEntrypoint": NotRequired[List[str]],
@@ -11872,70 +12834,69 @@
     {
         "DataSource": TransformDataSourceTypeDef,
         "ContentType": NotRequired[str],
         "CompressionType": NotRequired[CompressionTypeType],
         "SplitType": NotRequired[SplitTypeType],
     },
 )
-ListWorkforcesResponsePaginatorTypeDef = TypedDict(
-    "ListWorkforcesResponsePaginatorTypeDef",
-    {
-        "Workforces": List[WorkforcePaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeWorkforceResponseTypeDef = TypedDict(
     "DescribeWorkforceResponseTypeDef",
     {
         "Workforce": WorkforceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWorkforcesResponseTypeDef = TypedDict(
     "ListWorkforcesResponseTypeDef",
     {
         "Workforces": List[WorkforceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateWorkforceResponseTypeDef = TypedDict(
     "UpdateWorkforceResponseTypeDef",
     {
         "Workforce": WorkforceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListArtifactsResponsePaginatorTypeDef = TypedDict(
-    "ListArtifactsResponsePaginatorTypeDef",
-    {
-        "ArtifactSummaries": List[ArtifactSummaryPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+DomainSettingsUnionTypeDef = Union[DomainSettingsTypeDef, DomainSettingsOutputTypeDef]
 ListArtifactsResponseTypeDef = TypedDict(
     "ListArtifactsResponseTypeDef",
     {
         "ArtifactSummaries": List[ArtifactSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+AsyncInferenceConfigUnionTypeDef = Union[
+    AsyncInferenceConfigTypeDef, AsyncInferenceConfigOutputTypeDef
+]
+AutoMLProblemTypeConfigOutputTypeDef = TypedDict(
+    "AutoMLProblemTypeConfigOutputTypeDef",
+    {
+        "ImageClassificationJobConfig": NotRequired[ImageClassificationJobConfigTypeDef],
+        "TextClassificationJobConfig": NotRequired[TextClassificationJobConfigTypeDef],
+        "TimeSeriesForecastingJobConfig": NotRequired[TimeSeriesForecastingJobConfigOutputTypeDef],
+        "TabularJobConfig": NotRequired[TabularJobConfigOutputTypeDef],
+        "TextGenerationJobConfig": NotRequired[TextGenerationJobConfigOutputTypeDef],
     },
 )
 AutoMLProblemTypeConfigTypeDef = TypedDict(
     "AutoMLProblemTypeConfigTypeDef",
     {
         "ImageClassificationJobConfig": NotRequired[ImageClassificationJobConfigTypeDef],
         "TextClassificationJobConfig": NotRequired[TextClassificationJobConfigTypeDef],
         "TimeSeriesForecastingJobConfig": NotRequired[TimeSeriesForecastingJobConfigTypeDef],
         "TabularJobConfig": NotRequired[TabularJobConfigTypeDef],
         "TextGenerationJobConfig": NotRequired[TextGenerationJobConfigTypeDef],
     },
 )
+AutoMLJobConfigUnionTypeDef = Union[AutoMLJobConfigTypeDef, AutoMLJobConfigOutputTypeDef]
 CreateAutoMLJobRequestRequestTypeDef = TypedDict(
     "CreateAutoMLJobRequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "InputDataConfig": Sequence[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
@@ -11943,14 +12904,17 @@
         "AutoMLJobObjective": NotRequired[AutoMLJobObjectiveTypeDef],
         "AutoMLJobConfig": NotRequired[AutoMLJobConfigTypeDef],
         "GenerateCandidateDefinitionsOnly": NotRequired[bool],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "ModelDeployConfig": NotRequired[ModelDeployConfigTypeDef],
     },
 )
+LabelingJobAlgorithmsConfigUnionTypeDef = Union[
+    LabelingJobAlgorithmsConfigTypeDef, LabelingJobAlgorithmsConfigOutputTypeDef
+]
 PipelineExecutionStepTypeDef = TypedDict(
     "PipelineExecutionStepTypeDef",
     {
         "StepName": NotRequired[str],
         "StepDisplayName": NotRequired[str],
         "StepDescription": NotRequired[str],
         "StartTime": NotRequired[datetime],
@@ -11969,15 +12933,15 @@
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
         "InputDataConfig": List[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
-        "AutoMLJobConfig": AutoMLJobConfigTypeDef,
+        "AutoMLJobConfig": AutoMLJobConfigOutputTypeDef,
         "CreationTime": datetime,
         "EndTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
         "BestCandidate": AutoMLCandidateTypeDef,
         "AutoMLJobStatus": AutoMLJobStatusType,
@@ -11990,26 +12954,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCandidatesForAutoMLJobResponseTypeDef = TypedDict(
     "ListCandidatesForAutoMLJobResponseTypeDef",
     {
         "Candidates": List[AutoMLCandidateTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DeploymentConfigOutputTypeDef = TypedDict(
+    "DeploymentConfigOutputTypeDef",
+    {
+        "BlueGreenUpdatePolicy": NotRequired[BlueGreenUpdatePolicyTypeDef],
+        "RollingUpdatePolicy": NotRequired[RollingUpdatePolicyTypeDef],
+        "AutoRollbackConfiguration": NotRequired[AutoRollbackConfigOutputTypeDef],
     },
 )
 DeploymentConfigTypeDef = TypedDict(
     "DeploymentConfigTypeDef",
     {
         "BlueGreenUpdatePolicy": NotRequired[BlueGreenUpdatePolicyTypeDef],
         "RollingUpdatePolicy": NotRequired[RollingUpdatePolicyTypeDef],
         "AutoRollbackConfiguration": NotRequired[AutoRollbackConfigTypeDef],
     },
 )
+RecommendationJobInputConfigOutputTypeDef = TypedDict(
+    "RecommendationJobInputConfigOutputTypeDef",
+    {
+        "ModelPackageVersionArn": NotRequired[str],
+        "ModelName": NotRequired[str],
+        "JobDurationInSeconds": NotRequired[int],
+        "TrafficPattern": NotRequired[TrafficPatternOutputTypeDef],
+        "ResourceLimit": NotRequired[RecommendationJobResourceLimitTypeDef],
+        "EndpointConfigurations": NotRequired[List[EndpointInputConfigurationOutputTypeDef]],
+        "VolumeKmsKeyId": NotRequired[str],
+        "ContainerConfig": NotRequired[RecommendationJobContainerConfigOutputTypeDef],
+        "Endpoints": NotRequired[List[EndpointInfoTypeDef]],
+        "VpcConfig": NotRequired[RecommendationJobVpcConfigOutputTypeDef],
+    },
+)
 RecommendationJobInputConfigTypeDef = TypedDict(
     "RecommendationJobInputConfigTypeDef",
     {
         "ModelPackageVersionArn": NotRequired[str],
         "ModelName": NotRequired[str],
         "JobDurationInSeconds": NotRequired[int],
         "TrafficPattern": NotRequired[TrafficPatternTypeDef],
@@ -12017,14 +13004,20 @@
         "EndpointConfigurations": NotRequired[Sequence[EndpointInputConfigurationTypeDef]],
         "VolumeKmsKeyId": NotRequired[str],
         "ContainerConfig": NotRequired[RecommendationJobContainerConfigTypeDef],
         "Endpoints": NotRequired[Sequence[EndpointInfoTypeDef]],
         "VpcConfig": NotRequired[RecommendationJobVpcConfigTypeDef],
     },
 )
+ExplainerConfigOutputTypeDef = TypedDict(
+    "ExplainerConfigOutputTypeDef",
+    {
+        "ClarifyExplainerConfig": NotRequired[ClarifyExplainerConfigOutputTypeDef],
+    },
+)
 ExplainerConfigTypeDef = TypedDict(
     "ExplainerConfigTypeDef",
     {
         "ClarifyExplainerConfig": NotRequired[ClarifyExplainerConfigTypeDef],
     },
 )
 CreateFeatureGroupRequestRequestTypeDef = TypedDict(
@@ -12092,47 +13085,76 @@
     {
         "FeatureGroupName": str,
         "FeatureAdditions": NotRequired[Sequence[FeatureDefinitionTypeDef]],
         "OnlineStoreConfig": NotRequired[OnlineStoreConfigUpdateTypeDef],
         "ThroughputConfig": NotRequired[ThroughputConfigUpdateTypeDef],
     },
 )
-ListInferenceExperimentsResponseTypeDef = TypedDict(
-    "ListInferenceExperimentsResponseTypeDef",
+HyperParameterTrainingJobDefinitionExtraOutputTypeDef = TypedDict(
+    "HyperParameterTrainingJobDefinitionExtraOutputTypeDef",
     {
-        "InferenceExperiments": List[InferenceExperimentSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AlgorithmSpecification": HyperParameterAlgorithmSpecificationExtraOutputTypeDef,
+        "RoleArn": str,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "StoppingCondition": StoppingConditionTypeDef,
+        "DefinitionName": NotRequired[str],
+        "TuningObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
+        "HyperParameterRanges": NotRequired[ParameterRangesExtraOutputTypeDef],
+        "StaticHyperParameters": NotRequired[Dict[str, str]],
+        "InputDataConfig": NotRequired[List[ChannelExtraOutputTypeDef]],
+        "VpcConfig": NotRequired[VpcConfigExtraOutputTypeDef],
+        "ResourceConfig": NotRequired[ResourceConfigExtraOutputTypeDef],
+        "HyperParameterTuningResourceConfig": NotRequired[
+            HyperParameterTuningResourceConfigExtraOutputTypeDef
+        ],
+        "EnableNetworkIsolation": NotRequired[bool],
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "EnableManagedSpotTraining": NotRequired[bool],
+        "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
+        "RetryStrategy": NotRequired[RetryStrategyTypeDef],
+        "Environment": NotRequired[Dict[str, str]],
     },
 )
-HyperParameterTrainingJobDefinitionPaginatorTypeDef = TypedDict(
-    "HyperParameterTrainingJobDefinitionPaginatorTypeDef",
+HyperParameterTrainingJobDefinitionOutputTypeDef = TypedDict(
+    "HyperParameterTrainingJobDefinitionOutputTypeDef",
     {
-        "AlgorithmSpecification": HyperParameterAlgorithmSpecificationPaginatorTypeDef,
+        "AlgorithmSpecification": HyperParameterAlgorithmSpecificationOutputTypeDef,
         "RoleArn": str,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "DefinitionName": NotRequired[str],
         "TuningObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
-        "HyperParameterRanges": NotRequired[ParameterRangesPaginatorTypeDef],
+        "HyperParameterRanges": NotRequired[ParameterRangesOutputTypeDef],
         "StaticHyperParameters": NotRequired[Dict[str, str]],
-        "InputDataConfig": NotRequired[List[ChannelPaginatorTypeDef]],
-        "VpcConfig": NotRequired[VpcConfigPaginatorTypeDef],
-        "ResourceConfig": NotRequired[ResourceConfigPaginatorTypeDef],
+        "InputDataConfig": NotRequired[List[ChannelOutputTypeDef]],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+        "ResourceConfig": NotRequired[ResourceConfigOutputTypeDef],
         "HyperParameterTuningResourceConfig": NotRequired[
-            HyperParameterTuningResourceConfigPaginatorTypeDef
+            HyperParameterTuningResourceConfigOutputTypeDef
         ],
         "EnableNetworkIsolation": NotRequired[bool],
         "EnableInterContainerTrafficEncryption": NotRequired[bool],
         "EnableManagedSpotTraining": NotRequired[bool],
         "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
         "RetryStrategy": NotRequired[RetryStrategyTypeDef],
         "Environment": NotRequired[Dict[str, str]],
     },
 )
+TrainingJobDefinitionOutputTypeDef = TypedDict(
+    "TrainingJobDefinitionOutputTypeDef",
+    {
+        "TrainingInputMode": TrainingInputModeType,
+        "InputDataConfig": List[ChannelOutputTypeDef],
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "ResourceConfig": ResourceConfigOutputTypeDef,
+        "StoppingCondition": StoppingConditionTypeDef,
+        "HyperParameters": NotRequired[Dict[str, str]],
+    },
+)
+ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelExtraOutputTypeDef]
 HyperParameterTrainingJobDefinitionTypeDef = TypedDict(
     "HyperParameterTrainingJobDefinitionTypeDef",
     {
         "AlgorithmSpecification": HyperParameterAlgorithmSpecificationTypeDef,
         "RoleArn": str,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
@@ -12161,42 +13183,17 @@
         "InputDataConfig": Sequence[ChannelTypeDef],
         "OutputDataConfig": OutputDataConfigTypeDef,
         "ResourceConfig": ResourceConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "HyperParameters": NotRequired[Mapping[str, str]],
     },
 )
-CreateDomainRequestRequestTypeDef = TypedDict(
-    "CreateDomainRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "AuthMode": AuthModeType,
-        "DefaultUserSettings": UserSettingsTypeDef,
-        "SubnetIds": Sequence[str],
-        "VpcId": str,
-        "DomainSettings": NotRequired[DomainSettingsTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "AppNetworkAccessType": NotRequired[AppNetworkAccessTypeType],
-        "HomeEfsFileSystemKmsKeyId": NotRequired[str],
-        "KmsKeyId": NotRequired[str],
-        "AppSecurityGroupManagement": NotRequired[AppSecurityGroupManagementType],
-        "DefaultSpaceSettings": NotRequired[DefaultSpaceSettingsTypeDef],
-    },
-)
-CreateUserProfileRequestRequestTypeDef = TypedDict(
-    "CreateUserProfileRequestRequestTypeDef",
-    {
-        "DomainId": str,
-        "UserProfileName": str,
-        "SingleSignOnUserIdentifier": NotRequired[str],
-        "SingleSignOnUserValue": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "UserSettings": NotRequired[UserSettingsTypeDef],
-    },
-)
+DefaultSpaceSettingsUnionTypeDef = Union[
+    DefaultSpaceSettingsTypeDef, DefaultSpaceSettingsOutputTypeDef
+]
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "DomainArn": str,
         "DomainId": str,
         "DomainName": str,
         "HomeEfsFileSystemId": str,
@@ -12204,24 +13201,24 @@
         "SingleSignOnApplicationArn": str,
         "Status": DomainStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "SecurityGroupIdForDomainBoundary": str,
         "AuthMode": AuthModeType,
-        "DefaultUserSettings": UserSettingsTypeDef,
-        "DomainSettings": DomainSettingsTypeDef,
+        "DefaultUserSettings": UserSettingsOutputTypeDef,
+        "DomainSettings": DomainSettingsOutputTypeDef,
         "AppNetworkAccessType": AppNetworkAccessTypeType,
         "HomeEfsFileSystemKmsKeyId": str,
         "SubnetIds": List[str],
         "Url": str,
         "VpcId": str,
         "KmsKeyId": str,
         "AppSecurityGroupManagement": AppSecurityGroupManagementType,
-        "DefaultSpaceSettings": DefaultSpaceSettingsTypeDef,
+        "DefaultSpaceSettings": DefaultSpaceSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeUserProfileResponseTypeDef = TypedDict(
     "DescribeUserProfileResponseTypeDef",
     {
         "DomainId": str,
@@ -12230,18 +13227,46 @@
         "HomeEfsFileSystemUid": str,
         "Status": UserProfileStatusType,
         "LastModifiedTime": datetime,
         "CreationTime": datetime,
         "FailureReason": str,
         "SingleSignOnUserIdentifier": str,
         "SingleSignOnUserValue": str,
-        "UserSettings": UserSettingsTypeDef,
+        "UserSettings": UserSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDomainRequestRequestTypeDef = TypedDict(
+    "CreateDomainRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "AuthMode": AuthModeType,
+        "DefaultUserSettings": UserSettingsTypeDef,
+        "SubnetIds": Sequence[str],
+        "VpcId": str,
+        "DomainSettings": NotRequired[DomainSettingsTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "AppNetworkAccessType": NotRequired[AppNetworkAccessTypeType],
+        "HomeEfsFileSystemKmsKeyId": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "AppSecurityGroupManagement": NotRequired[AppSecurityGroupManagementType],
+        "DefaultSpaceSettings": NotRequired[DefaultSpaceSettingsTypeDef],
+    },
+)
+CreateUserProfileRequestRequestTypeDef = TypedDict(
+    "CreateUserProfileRequestRequestTypeDef",
+    {
+        "DomainId": str,
+        "UserProfileName": str,
+        "SingleSignOnUserIdentifier": NotRequired[str],
+        "SingleSignOnUserValue": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "UserSettings": NotRequired[UserSettingsTypeDef],
+    },
+)
 UpdateDomainRequestRequestTypeDef = TypedDict(
     "UpdateDomainRequestRequestTypeDef",
     {
         "DomainId": str,
         "DefaultUserSettings": NotRequired[UserSettingsTypeDef],
         "DomainSettingsForUpdate": NotRequired[DomainSettingsForUpdateTypeDef],
         "AppSecurityGroupManagement": NotRequired[AppSecurityGroupManagementType],
@@ -12254,14 +13279,15 @@
     "UpdateUserProfileRequestRequestTypeDef",
     {
         "DomainId": str,
         "UserProfileName": str,
         "UserSettings": NotRequired[UserSettingsTypeDef],
     },
 )
+UserSettingsUnionTypeDef = Union[UserSettingsTypeDef, UserSettingsOutputTypeDef]
 DescribeInferenceComponentOutputTypeDef = TypedDict(
     "DescribeInferenceComponentOutputTypeDef",
     {
         "InferenceComponentName": str,
         "InferenceComponentArn": str,
         "EndpointName": str,
         "EndpointArn": str,
@@ -12271,14 +13297,33 @@
         "RuntimeConfig": InferenceComponentRuntimeConfigSummaryTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "InferenceComponentStatus": InferenceComponentStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeSpaceResponseTypeDef = TypedDict(
+    "DescribeSpaceResponseTypeDef",
+    {
+        "DomainId": str,
+        "SpaceArn": str,
+        "SpaceName": str,
+        "HomeEfsFileSystemUid": str,
+        "Status": SpaceStatusType,
+        "LastModifiedTime": datetime,
+        "CreationTime": datetime,
+        "FailureReason": str,
+        "SpaceSettings": SpaceSettingsOutputTypeDef,
+        "OwnershipSettings": OwnershipSettingsTypeDef,
+        "SpaceSharingSettings": SpaceSharingSettingsTypeDef,
+        "SpaceDisplayName": str,
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SpaceDetailsTypeDef = TypedDict(
     "SpaceDetailsTypeDef",
     {
         "DomainId": NotRequired[str],
         "SpaceName": NotRequired[str],
         "Status": NotRequired[SpaceStatusType],
         "CreationTime": NotRequired[datetime],
@@ -12297,33 +13342,15 @@
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "SpaceSettings": NotRequired[SpaceSettingsTypeDef],
         "OwnershipSettings": NotRequired[OwnershipSettingsTypeDef],
         "SpaceSharingSettings": NotRequired[SpaceSharingSettingsTypeDef],
         "SpaceDisplayName": NotRequired[str],
     },
 )
-DescribeSpaceResponseTypeDef = TypedDict(
-    "DescribeSpaceResponseTypeDef",
-    {
-        "DomainId": str,
-        "SpaceArn": str,
-        "SpaceName": str,
-        "HomeEfsFileSystemUid": str,
-        "Status": SpaceStatusType,
-        "LastModifiedTime": datetime,
-        "CreationTime": datetime,
-        "FailureReason": str,
-        "SpaceSettings": SpaceSettingsTypeDef,
-        "OwnershipSettings": OwnershipSettingsTypeDef,
-        "SpaceSharingSettings": SpaceSharingSettingsTypeDef,
-        "SpaceDisplayName": str,
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+SpaceSettingsUnionTypeDef = Union[SpaceSettingsTypeDef, SpaceSettingsOutputTypeDef]
 UpdateSpaceRequestRequestTypeDef = TypedDict(
     "UpdateSpaceRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpaceName": str,
         "SpaceSettings": NotRequired[SpaceSettingsTypeDef],
         "SpaceDisplayName": NotRequired[str],
@@ -12350,16 +13377,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListAssociationsResponseTypeDef = TypedDict(
     "ListAssociationsResponseTypeDef",
     {
         "AssociationSummaries": List[AssociationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TrialTypeDef = TypedDict(
     "TrialTypeDef",
     {
         "TrialName": NotRequired[str],
         "TrialArn": NotRequired[str],
@@ -12375,16 +13402,32 @@
         "TrialComponentSummaries": NotRequired[List[TrialComponentSimpleSummaryTypeDef]],
     },
 )
 ListTrialComponentsResponseTypeDef = TypedDict(
     "ListTrialComponentsResponseTypeDef",
     {
         "TrialComponentSummaries": List[TrialComponentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+TrainingSpecificationOutputTypeDef = TypedDict(
+    "TrainingSpecificationOutputTypeDef",
+    {
+        "TrainingImage": str,
+        "SupportedTrainingInstanceTypes": List[TrainingInstanceTypeType],
+        "TrainingChannels": List[ChannelSpecificationOutputTypeDef],
+        "TrainingImageDigest": NotRequired[str],
+        "SupportedHyperParameters": NotRequired[List[HyperParameterSpecificationOutputTypeDef]],
+        "SupportsDistributedTraining": NotRequired[bool],
+        "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
+        "SupportedTuningJobObjectiveMetrics": NotRequired[
+            List[HyperParameterTuningJobObjectiveTypeDef]
+        ],
+        "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
     },
 )
 TrainingSpecificationTypeDef = TypedDict(
     "TrainingSpecificationTypeDef",
     {
         "TrainingImage": str,
         "SupportedTrainingInstanceTypes": Sequence[TrainingInstanceTypeType],
@@ -12395,45 +13438,23 @@
         "MetricDefinitions": NotRequired[Sequence[MetricDefinitionTypeDef]],
         "SupportedTuningJobObjectiveMetrics": NotRequired[
             Sequence[HyperParameterTuningJobObjectiveTypeDef]
         ],
         "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
     },
 )
-ListAppImageConfigsResponsePaginatorTypeDef = TypedDict(
-    "ListAppImageConfigsResponsePaginatorTypeDef",
-    {
-        "NextToken": str,
-        "AppImageConfigs": List[AppImageConfigDetailsPaginatorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+HyperParameterTuningJobConfigUnionTypeDef = Union[
+    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigExtraOutputTypeDef
+]
 ListAppImageConfigsResponseTypeDef = TypedDict(
     "ListAppImageConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "AppImageConfigs": List[AppImageConfigDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-LabelingJobSummaryPaginatorTypeDef = TypedDict(
-    "LabelingJobSummaryPaginatorTypeDef",
-    {
-        "LabelingJobName": str,
-        "LabelingJobArn": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LabelingJobStatus": LabelingJobStatusType,
-        "LabelCounters": LabelCountersTypeDef,
-        "WorkteamArn": str,
-        "PreHumanTaskLambdaArn": str,
-        "AnnotationConsolidationLambdaArn": NotRequired[str],
-        "FailureReason": NotRequired[str],
-        "LabelingJobOutput": NotRequired[LabelingJobOutputTypeDef],
-        "InputConfig": NotRequired[LabelingJobInputConfigPaginatorTypeDef],
+        "NextToken": NotRequired[str],
     },
 )
 LabelingJobSummaryTypeDef = TypedDict(
     "LabelingJobSummaryTypeDef",
     {
         "LabelingJobName": str,
         "LabelingJobArn": str,
@@ -12442,55 +13463,85 @@
         "LabelingJobStatus": LabelingJobStatusType,
         "LabelCounters": LabelCountersTypeDef,
         "WorkteamArn": str,
         "PreHumanTaskLambdaArn": str,
         "AnnotationConsolidationLambdaArn": NotRequired[str],
         "FailureReason": NotRequired[str],
         "LabelingJobOutput": NotRequired[LabelingJobOutputTypeDef],
-        "InputConfig": NotRequired[LabelingJobInputConfigTypeDef],
-    },
-)
-ListWorkteamsResponsePaginatorTypeDef = TypedDict(
-    "ListWorkteamsResponsePaginatorTypeDef",
-    {
-        "Workteams": List[WorkteamPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InputConfig": NotRequired[LabelingJobInputConfigOutputTypeDef],
     },
 )
+LabelingJobInputConfigUnionTypeDef = Union[
+    LabelingJobInputConfigTypeDef, LabelingJobInputConfigExtraOutputTypeDef
+]
 DescribeWorkteamResponseTypeDef = TypedDict(
     "DescribeWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWorkteamsResponseTypeDef = TypedDict(
     "ListWorkteamsResponseTypeDef",
     {
         "Workteams": List[WorkteamTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateWorkteamResponseTypeDef = TypedDict(
     "UpdateWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateWorkteamRequestRequestTypeDef = TypedDict(
+    "CreateWorkteamRequestRequestTypeDef",
+    {
+        "WorkteamName": str,
+        "MemberDefinitions": Sequence[MemberDefinitionUnionTypeDef],
+        "Description": str,
+        "WorkforceName": NotRequired[str],
+        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+UpdateWorkteamRequestRequestTypeDef = TypedDict(
+    "UpdateWorkteamRequestRequestTypeDef",
+    {
+        "WorkteamName": str,
+        "MemberDefinitions": NotRequired[Sequence[MemberDefinitionUnionTypeDef]],
+        "Description": NotRequired[str],
+        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
+    },
+)
 ScalingPolicyTypeDef = TypedDict(
     "ScalingPolicyTypeDef",
     {
         "TargetTracking": NotRequired[TargetTrackingScalingPolicyConfigurationTypeDef],
     },
 )
-ContainerDefinitionPaginatorTypeDef = TypedDict(
-    "ContainerDefinitionPaginatorTypeDef",
+ContainerDefinitionExtraOutputTypeDef = TypedDict(
+    "ContainerDefinitionExtraOutputTypeDef",
+    {
+        "ContainerHostname": NotRequired[str],
+        "Image": NotRequired[str],
+        "ImageConfig": NotRequired[ImageConfigTypeDef],
+        "Mode": NotRequired[ContainerModeType],
+        "ModelDataUrl": NotRequired[str],
+        "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
+        "Environment": NotRequired[Dict[str, str]],
+        "ModelPackageName": NotRequired[str],
+        "InferenceSpecificationName": NotRequired[str],
+        "MultiModelConfig": NotRequired[MultiModelConfigTypeDef],
+    },
+)
+ContainerDefinitionOutputTypeDef = TypedDict(
+    "ContainerDefinitionOutputTypeDef",
     {
         "ContainerHostname": NotRequired[str],
         "Image": NotRequired[str],
         "ImageConfig": NotRequired[ImageConfigTypeDef],
         "Mode": NotRequired[ContainerModeType],
         "ModelDataUrl": NotRequired[str],
         "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
@@ -12511,24 +13562,58 @@
         "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
         "Environment": NotRequired[Mapping[str, str]],
         "ModelPackageName": NotRequired[str],
         "InferenceSpecificationName": NotRequired[str],
         "MultiModelConfig": NotRequired[MultiModelConfigTypeDef],
     },
 )
+ModelPackageContainerDefinitionExtraOutputTypeDef = TypedDict(
+    "ModelPackageContainerDefinitionExtraOutputTypeDef",
+    {
+        "Image": str,
+        "ContainerHostname": NotRequired[str],
+        "ImageDigest": NotRequired[str],
+        "ModelDataUrl": NotRequired[str],
+        "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
+        "ProductId": NotRequired[str],
+        "Environment": NotRequired[Dict[str, str]],
+        "ModelInput": NotRequired[ModelInputTypeDef],
+        "Framework": NotRequired[str],
+        "FrameworkVersion": NotRequired[str],
+        "NearestModelName": NotRequired[str],
+        "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
+    },
+)
+ModelPackageContainerDefinitionOutputTypeDef = TypedDict(
+    "ModelPackageContainerDefinitionOutputTypeDef",
+    {
+        "Image": str,
+        "ContainerHostname": NotRequired[str],
+        "ImageDigest": NotRequired[str],
+        "ModelDataUrl": NotRequired[str],
+        "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
+        "ProductId": NotRequired[str],
+        "Environment": NotRequired[Dict[str, str]],
+        "ModelInput": NotRequired[ModelInputTypeDef],
+        "Framework": NotRequired[str],
+        "FrameworkVersion": NotRequired[str],
+        "NearestModelName": NotRequired[str],
+        "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
+    },
+)
 ModelPackageContainerDefinitionTypeDef = TypedDict(
     "ModelPackageContainerDefinitionTypeDef",
     {
         "Image": str,
         "ContainerHostname": NotRequired[str],
         "ImageDigest": NotRequired[str],
         "ModelDataUrl": NotRequired[str],
         "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
         "ProductId": NotRequired[str],
-        "Environment": NotRequired[Dict[str, str]],
+        "Environment": NotRequired[Mapping[str, str]],
         "ModelInput": NotRequired[ModelInputTypeDef],
         "Framework": NotRequired[str],
         "FrameworkVersion": NotRequired[str],
         "NearestModelName": NotRequired[str],
         "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
     },
 )
@@ -12540,36 +13625,36 @@
         "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
     },
 )
 ListMonitoringAlertsResponseTypeDef = TypedDict(
     "ListMonitoringAlertsResponseTypeDef",
     {
         "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInferenceExperimentResponseTypeDef = TypedDict(
     "DescribeInferenceExperimentResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": Literal["ShadowMode"],
-        "Schedule": InferenceExperimentScheduleTypeDef,
+        "Schedule": InferenceExperimentScheduleOutputTypeDef,
         "Status": InferenceExperimentStatusType,
         "StatusReason": str,
         "Description": str,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "LastModifiedTime": datetime,
         "RoleArn": str,
         "EndpointMetadata": EndpointMetadataTypeDef,
         "ModelVariants": List[ModelVariantConfigSummaryTypeDef],
-        "DataStorageConfig": InferenceExperimentDataStorageConfigTypeDef,
-        "ShadowModeConfig": ShadowModeConfigTypeDef,
+        "DataStorageConfig": InferenceExperimentDataStorageConfigOutputTypeDef,
+        "ShadowModeConfig": ShadowModeConfigOutputTypeDef,
         "KmsKey": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateInferenceExperimentRequestRequestTypeDef = TypedDict(
     "CreateInferenceExperimentRequestRequestTypeDef",
     {
@@ -12603,19 +13688,56 @@
         "Schedule": NotRequired[InferenceExperimentScheduleTypeDef],
         "Description": NotRequired[str],
         "ModelVariants": NotRequired[Sequence[ModelVariantConfigTypeDef]],
         "DataStorageConfig": NotRequired[InferenceExperimentDataStorageConfigTypeDef],
         "ShadowModeConfig": NotRequired[ShadowModeConfigTypeDef],
     },
 )
-MonitoringInputPaginatorTypeDef = TypedDict(
-    "MonitoringInputPaginatorTypeDef",
+MonitoringInputExtraOutputTypeDef = TypedDict(
+    "MonitoringInputExtraOutputTypeDef",
     {
         "EndpointInput": NotRequired[EndpointInputTypeDef],
-        "BatchTransformInput": NotRequired[BatchTransformInputPaginatorTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputExtraOutputTypeDef],
+    },
+)
+DataQualityJobInputOutputTypeDef = TypedDict(
+    "DataQualityJobInputOutputTypeDef",
+    {
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
+    },
+)
+ModelBiasJobInputOutputTypeDef = TypedDict(
+    "ModelBiasJobInputOutputTypeDef",
+    {
+        "GroundTruthS3Input": MonitoringGroundTruthS3InputTypeDef,
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
+    },
+)
+ModelExplainabilityJobInputOutputTypeDef = TypedDict(
+    "ModelExplainabilityJobInputOutputTypeDef",
+    {
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
+    },
+)
+ModelQualityJobInputOutputTypeDef = TypedDict(
+    "ModelQualityJobInputOutputTypeDef",
+    {
+        "GroundTruthS3Input": MonitoringGroundTruthS3InputTypeDef,
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
+    },
+)
+MonitoringInputOutputTypeDef = TypedDict(
+    "MonitoringInputOutputTypeDef",
+    {
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
     },
 )
 DataQualityJobInputTypeDef = TypedDict(
     "DataQualityJobInputTypeDef",
     {
         "EndpointInput": NotRequired[EndpointInputTypeDef],
         "BatchTransformInput": NotRequired[BatchTransformInputTypeDef],
@@ -12647,68 +13769,28 @@
 MonitoringInputTypeDef = TypedDict(
     "MonitoringInputTypeDef",
     {
         "EndpointInput": NotRequired[EndpointInputTypeDef],
         "BatchTransformInput": NotRequired[BatchTransformInputTypeDef],
     },
 )
-ProcessingJobPaginatorTypeDef = TypedDict(
-    "ProcessingJobPaginatorTypeDef",
-    {
-        "ProcessingInputs": NotRequired[List[ProcessingInputTypeDef]],
-        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigPaginatorTypeDef],
-        "ProcessingJobName": NotRequired[str],
-        "ProcessingResources": NotRequired[ProcessingResourcesTypeDef],
-        "StoppingCondition": NotRequired[ProcessingStoppingConditionTypeDef],
-        "AppSpecification": NotRequired[AppSpecificationPaginatorTypeDef],
-        "Environment": NotRequired[Dict[str, str]],
-        "NetworkConfig": NotRequired[NetworkConfigPaginatorTypeDef],
-        "RoleArn": NotRequired[str],
-        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-        "ProcessingJobArn": NotRequired[str],
-        "ProcessingJobStatus": NotRequired[ProcessingJobStatusType],
-        "ExitMessage": NotRequired[str],
-        "FailureReason": NotRequired[str],
-        "ProcessingEndTime": NotRequired[datetime],
-        "ProcessingStartTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "CreationTime": NotRequired[datetime],
-        "MonitoringScheduleArn": NotRequired[str],
-        "AutoMLJobArn": NotRequired[str],
-        "TrainingJobArn": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
-CreateProcessingJobRequestRequestTypeDef = TypedDict(
-    "CreateProcessingJobRequestRequestTypeDef",
-    {
-        "ProcessingJobName": str,
-        "ProcessingResources": ProcessingResourcesTypeDef,
-        "AppSpecification": AppSpecificationTypeDef,
-        "RoleArn": str,
-        "ProcessingInputs": NotRequired[Sequence[ProcessingInputTypeDef]],
-        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigTypeDef],
-        "StoppingCondition": NotRequired[ProcessingStoppingConditionTypeDef],
-        "Environment": NotRequired[Mapping[str, str]],
-        "NetworkConfig": NotRequired[NetworkConfigTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-    },
-)
+MonitoringOutputConfigUnionTypeDef = Union[
+    MonitoringOutputConfigTypeDef, MonitoringOutputConfigExtraOutputTypeDef
+]
 DescribeProcessingJobResponseTypeDef = TypedDict(
     "DescribeProcessingJobResponseTypeDef",
     {
         "ProcessingInputs": List[ProcessingInputTypeDef],
-        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
+        "ProcessingOutputConfig": ProcessingOutputConfigOutputTypeDef,
         "ProcessingJobName": str,
         "ProcessingResources": ProcessingResourcesTypeDef,
         "StoppingCondition": ProcessingStoppingConditionTypeDef,
-        "AppSpecification": AppSpecificationTypeDef,
+        "AppSpecification": AppSpecificationOutputTypeDef,
         "Environment": Dict[str, str],
-        "NetworkConfig": NetworkConfigTypeDef,
+        "NetworkConfig": NetworkConfigOutputTypeDef,
         "RoleArn": str,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ProcessingJobArn": str,
         "ProcessingJobStatus": ProcessingJobStatusType,
         "ExitMessage": str,
         "FailureReason": str,
         "ProcessingEndTime": datetime,
@@ -12721,21 +13803,21 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ProcessingJobTypeDef = TypedDict(
     "ProcessingJobTypeDef",
     {
         "ProcessingInputs": NotRequired[List[ProcessingInputTypeDef]],
-        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigTypeDef],
+        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigOutputTypeDef],
         "ProcessingJobName": NotRequired[str],
         "ProcessingResources": NotRequired[ProcessingResourcesTypeDef],
         "StoppingCondition": NotRequired[ProcessingStoppingConditionTypeDef],
-        "AppSpecification": NotRequired[AppSpecificationTypeDef],
+        "AppSpecification": NotRequired[AppSpecificationOutputTypeDef],
         "Environment": NotRequired[Dict[str, str]],
-        "NetworkConfig": NotRequired[NetworkConfigTypeDef],
+        "NetworkConfig": NotRequired[NetworkConfigOutputTypeDef],
         "RoleArn": NotRequired[str],
         "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
         "ProcessingJobArn": NotRequired[str],
         "ProcessingJobStatus": NotRequired[ProcessingJobStatusType],
         "ExitMessage": NotRequired[str],
         "FailureReason": NotRequired[str],
         "ProcessingEndTime": NotRequired[datetime],
@@ -12744,193 +13826,142 @@
         "CreationTime": NotRequired[datetime],
         "MonitoringScheduleArn": NotRequired[str],
         "AutoMLJobArn": NotRequired[str],
         "TrainingJobArn": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-CreateFlowDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateFlowDefinitionRequestRequestTypeDef",
+CreateProcessingJobRequestRequestTypeDef = TypedDict(
+    "CreateProcessingJobRequestRequestTypeDef",
     {
-        "FlowDefinitionName": str,
-        "OutputConfig": FlowDefinitionOutputConfigTypeDef,
+        "ProcessingJobName": str,
+        "ProcessingResources": ProcessingResourcesTypeDef,
+        "AppSpecification": AppSpecificationTypeDef,
         "RoleArn": str,
-        "HumanLoopRequestSource": NotRequired[HumanLoopRequestSourceTypeDef],
-        "HumanLoopActivationConfig": NotRequired[HumanLoopActivationConfigTypeDef],
-        "HumanLoopConfig": NotRequired[HumanLoopConfigTypeDef],
+        "ProcessingInputs": NotRequired[Sequence[ProcessingInputTypeDef]],
+        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigTypeDef],
+        "StoppingCondition": NotRequired[ProcessingStoppingConditionTypeDef],
+        "Environment": NotRequired[Mapping[str, str]],
+        "NetworkConfig": NotRequired[NetworkConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
+        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
     },
 )
+ProcessingOutputConfigUnionTypeDef = Union[
+    ProcessingOutputConfigTypeDef, ProcessingOutputConfigExtraOutputTypeDef
+]
 DescribeFlowDefinitionResponseTypeDef = TypedDict(
     "DescribeFlowDefinitionResponseTypeDef",
     {
         "FlowDefinitionArn": str,
         "FlowDefinitionName": str,
         "FlowDefinitionStatus": FlowDefinitionStatusType,
         "CreationTime": datetime,
         "HumanLoopRequestSource": HumanLoopRequestSourceTypeDef,
         "HumanLoopActivationConfig": HumanLoopActivationConfigTypeDef,
-        "HumanLoopConfig": HumanLoopConfigTypeDef,
+        "HumanLoopConfig": HumanLoopConfigOutputTypeDef,
         "OutputConfig": FlowDefinitionOutputConfigTypeDef,
         "RoleArn": str,
         "FailureReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateLabelingJobRequestRequestTypeDef = TypedDict(
-    "CreateLabelingJobRequestRequestTypeDef",
+CreateFlowDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateFlowDefinitionRequestRequestTypeDef",
     {
-        "LabelingJobName": str,
-        "LabelAttributeName": str,
-        "InputConfig": LabelingJobInputConfigTypeDef,
-        "OutputConfig": LabelingJobOutputConfigTypeDef,
+        "FlowDefinitionName": str,
+        "OutputConfig": FlowDefinitionOutputConfigTypeDef,
         "RoleArn": str,
-        "HumanTaskConfig": HumanTaskConfigTypeDef,
-        "LabelCategoryConfigS3Uri": NotRequired[str],
-        "StoppingConditions": NotRequired[LabelingJobStoppingConditionsTypeDef],
-        "LabelingJobAlgorithmsConfig": NotRequired[LabelingJobAlgorithmsConfigTypeDef],
+        "HumanLoopRequestSource": NotRequired[HumanLoopRequestSourceTypeDef],
+        "HumanLoopActivationConfig": NotRequired[HumanLoopActivationConfigTypeDef],
+        "HumanLoopConfig": NotRequired[HumanLoopConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+HumanLoopConfigUnionTypeDef = Union[HumanLoopConfigTypeDef, HumanLoopConfigOutputTypeDef]
 DescribeLabelingJobResponseTypeDef = TypedDict(
     "DescribeLabelingJobResponseTypeDef",
     {
         "LabelingJobStatus": LabelingJobStatusType,
         "LabelCounters": LabelCountersTypeDef,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "JobReferenceCode": str,
         "LabelingJobName": str,
         "LabelingJobArn": str,
         "LabelAttributeName": str,
-        "InputConfig": LabelingJobInputConfigTypeDef,
+        "InputConfig": LabelingJobInputConfigOutputTypeDef,
         "OutputConfig": LabelingJobOutputConfigTypeDef,
         "RoleArn": str,
         "LabelCategoryConfigS3Uri": str,
         "StoppingConditions": LabelingJobStoppingConditionsTypeDef,
-        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigTypeDef,
-        "HumanTaskConfig": HumanTaskConfigTypeDef,
+        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigOutputTypeDef,
+        "HumanTaskConfig": HumanTaskConfigOutputTypeDef,
         "Tags": List[TagTypeDef],
         "LabelingJobOutput": LabelingJobOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-TrainingJobPaginatorTypeDef = TypedDict(
-    "TrainingJobPaginatorTypeDef",
-    {
-        "TrainingJobName": NotRequired[str],
-        "TrainingJobArn": NotRequired[str],
-        "TuningJobArn": NotRequired[str],
-        "LabelingJobArn": NotRequired[str],
-        "AutoMLJobArn": NotRequired[str],
-        "ModelArtifacts": NotRequired[ModelArtifactsTypeDef],
-        "TrainingJobStatus": NotRequired[TrainingJobStatusType],
-        "SecondaryStatus": NotRequired[SecondaryStatusType],
-        "FailureReason": NotRequired[str],
-        "HyperParameters": NotRequired[Dict[str, str]],
-        "AlgorithmSpecification": NotRequired[AlgorithmSpecificationPaginatorTypeDef],
-        "RoleArn": NotRequired[str],
-        "InputDataConfig": NotRequired[List[ChannelPaginatorTypeDef]],
-        "OutputDataConfig": NotRequired[OutputDataConfigTypeDef],
-        "ResourceConfig": NotRequired[ResourceConfigPaginatorTypeDef],
-        "VpcConfig": NotRequired[VpcConfigPaginatorTypeDef],
-        "StoppingCondition": NotRequired[StoppingConditionTypeDef],
-        "CreationTime": NotRequired[datetime],
-        "TrainingStartTime": NotRequired[datetime],
-        "TrainingEndTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "SecondaryStatusTransitions": NotRequired[List[SecondaryStatusTransitionTypeDef]],
-        "FinalMetricDataList": NotRequired[List[MetricDataTypeDef]],
-        "EnableNetworkIsolation": NotRequired[bool],
-        "EnableInterContainerTrafficEncryption": NotRequired[bool],
-        "EnableManagedSpotTraining": NotRequired[bool],
-        "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
-        "TrainingTimeInSeconds": NotRequired[int],
-        "BillableTimeInSeconds": NotRequired[int],
-        "DebugHookConfig": NotRequired[DebugHookConfigPaginatorTypeDef],
-        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-        "DebugRuleConfigurations": NotRequired[List[DebugRuleConfigurationPaginatorTypeDef]],
-        "TensorBoardOutputConfig": NotRequired[TensorBoardOutputConfigTypeDef],
-        "DebugRuleEvaluationStatuses": NotRequired[List[DebugRuleEvaluationStatusTypeDef]],
-        "ProfilerConfig": NotRequired[ProfilerConfigPaginatorTypeDef],
-        "Environment": NotRequired[Dict[str, str]],
-        "RetryStrategy": NotRequired[RetryStrategyTypeDef],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
-CreateTrainingJobRequestRequestTypeDef = TypedDict(
-    "CreateTrainingJobRequestRequestTypeDef",
+CreateLabelingJobRequestRequestTypeDef = TypedDict(
+    "CreateLabelingJobRequestRequestTypeDef",
     {
-        "TrainingJobName": str,
-        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
+        "LabelingJobName": str,
+        "LabelAttributeName": str,
+        "InputConfig": LabelingJobInputConfigTypeDef,
+        "OutputConfig": LabelingJobOutputConfigTypeDef,
         "RoleArn": str,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigTypeDef,
-        "StoppingCondition": StoppingConditionTypeDef,
-        "HyperParameters": NotRequired[Mapping[str, str]],
-        "InputDataConfig": NotRequired[Sequence[ChannelTypeDef]],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "HumanTaskConfig": HumanTaskConfigTypeDef,
+        "LabelCategoryConfigS3Uri": NotRequired[str],
+        "StoppingConditions": NotRequired[LabelingJobStoppingConditionsTypeDef],
+        "LabelingJobAlgorithmsConfig": NotRequired[LabelingJobAlgorithmsConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
-        "EnableNetworkIsolation": NotRequired[bool],
-        "EnableInterContainerTrafficEncryption": NotRequired[bool],
-        "EnableManagedSpotTraining": NotRequired[bool],
-        "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
-        "DebugHookConfig": NotRequired[DebugHookConfigTypeDef],
-        "DebugRuleConfigurations": NotRequired[Sequence[DebugRuleConfigurationTypeDef]],
-        "TensorBoardOutputConfig": NotRequired[TensorBoardOutputConfigTypeDef],
-        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-        "ProfilerConfig": NotRequired[ProfilerConfigTypeDef],
-        "ProfilerRuleConfigurations": NotRequired[Sequence[ProfilerRuleConfigurationTypeDef]],
-        "Environment": NotRequired[Mapping[str, str]],
-        "RetryStrategy": NotRequired[RetryStrategyTypeDef],
-        "RemoteDebugConfig": NotRequired[RemoteDebugConfigTypeDef],
-        "InfraCheckConfig": NotRequired[InfraCheckConfigTypeDef],
     },
 )
+HumanTaskConfigUnionTypeDef = Union[HumanTaskConfigTypeDef, HumanTaskConfigOutputTypeDef]
 DescribeTrainingJobResponseTypeDef = TypedDict(
     "DescribeTrainingJobResponseTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
         "TuningJobArn": str,
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "TrainingJobStatus": TrainingJobStatusType,
         "SecondaryStatus": SecondaryStatusType,
         "FailureReason": str,
         "HyperParameters": Dict[str, str],
-        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
+        "AlgorithmSpecification": AlgorithmSpecificationOutputTypeDef,
         "RoleArn": str,
-        "InputDataConfig": List[ChannelTypeDef],
+        "InputDataConfig": List[ChannelOutputTypeDef],
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigTypeDef,
+        "ResourceConfig": ResourceConfigOutputTypeDef,
         "WarmPoolStatus": WarmPoolStatusTypeDef,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "CreationTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
         "LastModifiedTime": datetime,
         "SecondaryStatusTransitions": List[SecondaryStatusTransitionTypeDef],
         "FinalMetricDataList": List[MetricDataTypeDef],
         "EnableNetworkIsolation": bool,
         "EnableInterContainerTrafficEncryption": bool,
         "EnableManagedSpotTraining": bool,
         "CheckpointConfig": CheckpointConfigTypeDef,
         "TrainingTimeInSeconds": int,
         "BillableTimeInSeconds": int,
-        "DebugHookConfig": DebugHookConfigTypeDef,
+        "DebugHookConfig": DebugHookConfigOutputTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
-        "DebugRuleConfigurations": List[DebugRuleConfigurationTypeDef],
+        "DebugRuleConfigurations": List[DebugRuleConfigurationOutputTypeDef],
         "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
         "DebugRuleEvaluationStatuses": List[DebugRuleEvaluationStatusTypeDef],
-        "ProfilerConfig": ProfilerConfigTypeDef,
-        "ProfilerRuleConfigurations": List[ProfilerRuleConfigurationTypeDef],
+        "ProfilerConfig": ProfilerConfigOutputTypeDef,
+        "ProfilerRuleConfigurations": List[ProfilerRuleConfigurationOutputTypeDef],
         "ProfilerRuleEvaluationStatuses": List[ProfilerRuleEvaluationStatusTypeDef],
         "ProfilingStatus": ProfilingStatusType,
         "Environment": Dict[str, str],
         "RetryStrategy": RetryStrategyTypeDef,
         "RemoteDebugConfig": RemoteDebugConfigTypeDef,
         "InfraCheckConfig": InfraCheckConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -12945,44 +13976,47 @@
         "LabelingJobArn": NotRequired[str],
         "AutoMLJobArn": NotRequired[str],
         "ModelArtifacts": NotRequired[ModelArtifactsTypeDef],
         "TrainingJobStatus": NotRequired[TrainingJobStatusType],
         "SecondaryStatus": NotRequired[SecondaryStatusType],
         "FailureReason": NotRequired[str],
         "HyperParameters": NotRequired[Dict[str, str]],
-        "AlgorithmSpecification": NotRequired[AlgorithmSpecificationTypeDef],
+        "AlgorithmSpecification": NotRequired[AlgorithmSpecificationOutputTypeDef],
         "RoleArn": NotRequired[str],
-        "InputDataConfig": NotRequired[List[ChannelTypeDef]],
+        "InputDataConfig": NotRequired[List[ChannelOutputTypeDef]],
         "OutputDataConfig": NotRequired[OutputDataConfigTypeDef],
-        "ResourceConfig": NotRequired[ResourceConfigTypeDef],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "ResourceConfig": NotRequired[ResourceConfigOutputTypeDef],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
         "StoppingCondition": NotRequired[StoppingConditionTypeDef],
         "CreationTime": NotRequired[datetime],
         "TrainingStartTime": NotRequired[datetime],
         "TrainingEndTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
         "SecondaryStatusTransitions": NotRequired[List[SecondaryStatusTransitionTypeDef]],
         "FinalMetricDataList": NotRequired[List[MetricDataTypeDef]],
         "EnableNetworkIsolation": NotRequired[bool],
         "EnableInterContainerTrafficEncryption": NotRequired[bool],
         "EnableManagedSpotTraining": NotRequired[bool],
         "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
         "TrainingTimeInSeconds": NotRequired[int],
         "BillableTimeInSeconds": NotRequired[int],
-        "DebugHookConfig": NotRequired[DebugHookConfigTypeDef],
+        "DebugHookConfig": NotRequired[DebugHookConfigOutputTypeDef],
         "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-        "DebugRuleConfigurations": NotRequired[List[DebugRuleConfigurationTypeDef]],
+        "DebugRuleConfigurations": NotRequired[List[DebugRuleConfigurationOutputTypeDef]],
         "TensorBoardOutputConfig": NotRequired[TensorBoardOutputConfigTypeDef],
         "DebugRuleEvaluationStatuses": NotRequired[List[DebugRuleEvaluationStatusTypeDef]],
-        "ProfilerConfig": NotRequired[ProfilerConfigTypeDef],
+        "ProfilerConfig": NotRequired[ProfilerConfigOutputTypeDef],
         "Environment": NotRequired[Dict[str, str]],
         "RetryStrategy": NotRequired[RetryStrategyTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
+AlgorithmSpecificationUnionTypeDef = Union[
+    AlgorithmSpecificationTypeDef, AlgorithmSpecificationExtraOutputTypeDef
+]
 CreateTransformJobRequestRequestTypeDef = TypedDict(
     "CreateTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
         "ModelName": str,
         "TransformInput": TransformInputTypeDef,
         "TransformOutput": TransformOutputTypeDef,
@@ -13021,16 +14055,28 @@
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "DataProcessing": DataProcessingTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-TransformJobDefinitionPaginatorTypeDef = TypedDict(
-    "TransformJobDefinitionPaginatorTypeDef",
+TransformJobDefinitionExtraOutputTypeDef = TypedDict(
+    "TransformJobDefinitionExtraOutputTypeDef",
+    {
+        "TransformInput": TransformInputTypeDef,
+        "TransformOutput": TransformOutputTypeDef,
+        "TransformResources": TransformResourcesTypeDef,
+        "MaxConcurrentTransforms": NotRequired[int],
+        "MaxPayloadInMB": NotRequired[int],
+        "BatchStrategy": NotRequired[BatchStrategyType],
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
+TransformJobDefinitionOutputTypeDef = TypedDict(
+    "TransformJobDefinitionOutputTypeDef",
     {
         "TransformInput": TransformInputTypeDef,
         "TransformOutput": TransformOutputTypeDef,
         "TransformResources": TransformResourcesTypeDef,
         "MaxConcurrentTransforms": NotRequired[int],
         "MaxPayloadInMB": NotRequired[int],
         "BatchStrategy": NotRequired[BatchStrategyType],
@@ -13072,148 +14118,139 @@
         "LabelingJobArn": NotRequired[str],
         "AutoMLJobArn": NotRequired[str],
         "DataProcessing": NotRequired[DataProcessingTypeDef],
         "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-CreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
-    "CreateAutoMLJobV2RequestRequestTypeDef",
-    {
-        "AutoMLJobName": str,
-        "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
-        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
-        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
-        "RoleArn": str,
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "SecurityConfig": NotRequired[AutoMLSecurityConfigTypeDef],
-        "AutoMLJobObjective": NotRequired[AutoMLJobObjectiveTypeDef],
-        "ModelDeployConfig": NotRequired[ModelDeployConfigTypeDef],
-        "DataSplitConfig": NotRequired[AutoMLDataSplitConfigTypeDef],
-    },
-)
 DescribeAutoMLJobV2ResponseTypeDef = TypedDict(
     "DescribeAutoMLJobV2ResponseTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
         "AutoMLJobInputDataConfig": List[AutoMLJobChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
-        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigOutputTypeDef,
         "AutoMLProblemTypeConfigName": AutoMLProblemTypeConfigNameType,
         "CreationTime": datetime,
         "EndTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
         "BestCandidate": AutoMLCandidateTypeDef,
         "AutoMLJobStatus": AutoMLJobStatusType,
         "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
         "AutoMLJobArtifacts": AutoMLJobArtifactsTypeDef,
         "ResolvedAttributes": AutoMLResolvedAttributesTypeDef,
         "ModelDeployConfig": ModelDeployConfigTypeDef,
         "ModelDeployResult": ModelDeployResultTypeDef,
         "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
-        "SecurityConfig": AutoMLSecurityConfigTypeDef,
+        "SecurityConfig": AutoMLSecurityConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AutoMLProblemTypeConfigUnionTypeDef = Union[
+    AutoMLProblemTypeConfigTypeDef, AutoMLProblemTypeConfigOutputTypeDef
+]
+CreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
+    "CreateAutoMLJobV2RequestRequestTypeDef",
+    {
+        "AutoMLJobName": str,
+        "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
+        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "RoleArn": str,
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "SecurityConfig": NotRequired[AutoMLSecurityConfigTypeDef],
+        "AutoMLJobObjective": NotRequired[AutoMLJobObjectiveTypeDef],
+        "ModelDeployConfig": NotRequired[ModelDeployConfigTypeDef],
+        "DataSplitConfig": NotRequired[AutoMLDataSplitConfigTypeDef],
+    },
+)
 ListPipelineExecutionStepsResponseTypeDef = TypedDict(
     "ListPipelineExecutionStepsResponseTypeDef",
     {
         "PipelineExecutionSteps": List[PipelineExecutionStepTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateEndpointInputRequestTypeDef = TypedDict(
     "CreateEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
         "EndpointConfigName": str,
         "DeploymentConfig": NotRequired[DeploymentConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+DeploymentConfigUnionTypeDef = Union[DeploymentConfigTypeDef, DeploymentConfigOutputTypeDef]
 UpdateEndpointInputRequestTypeDef = TypedDict(
     "UpdateEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
         "EndpointConfigName": str,
         "RetainAllVariantProperties": NotRequired[bool],
         "ExcludeRetainedVariantProperties": NotRequired[Sequence[VariantPropertyTypeDef]],
         "DeploymentConfig": NotRequired[DeploymentConfigTypeDef],
         "RetainDeploymentConfig": NotRequired[bool],
     },
 )
-CreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
-    "CreateInferenceRecommendationsJobRequestRequestTypeDef",
-    {
-        "JobName": str,
-        "JobType": RecommendationJobTypeType,
-        "RoleArn": str,
-        "InputConfig": RecommendationJobInputConfigTypeDef,
-        "JobDescription": NotRequired[str],
-        "StoppingConditions": NotRequired[RecommendationJobStoppingConditionsTypeDef],
-        "OutputConfig": NotRequired[RecommendationJobOutputConfigTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 DescribeInferenceRecommendationsJobResponseTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobResponseTypeDef",
     {
         "JobName": str,
         "JobDescription": str,
         "JobType": RecommendationJobTypeType,
         "JobArn": str,
         "RoleArn": str,
         "Status": RecommendationJobStatusType,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
-        "InputConfig": RecommendationJobInputConfigTypeDef,
-        "StoppingConditions": RecommendationJobStoppingConditionsTypeDef,
+        "InputConfig": RecommendationJobInputConfigOutputTypeDef,
+        "StoppingConditions": RecommendationJobStoppingConditionsOutputTypeDef,
         "InferenceRecommendations": List[InferenceRecommendationTypeDef],
         "EndpointPerformances": List[EndpointPerformanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateEndpointConfigInputRequestTypeDef = TypedDict(
-    "CreateEndpointConfigInputRequestTypeDef",
+CreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
+    "CreateInferenceRecommendationsJobRequestRequestTypeDef",
     {
-        "EndpointConfigName": str,
-        "ProductionVariants": Sequence[ProductionVariantTypeDef],
-        "DataCaptureConfig": NotRequired[DataCaptureConfigTypeDef],
+        "JobName": str,
+        "JobType": RecommendationJobTypeType,
+        "RoleArn": str,
+        "InputConfig": RecommendationJobInputConfigTypeDef,
+        "JobDescription": NotRequired[str],
+        "StoppingConditions": NotRequired[RecommendationJobStoppingConditionsTypeDef],
+        "OutputConfig": NotRequired[RecommendationJobOutputConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
-        "KmsKeyId": NotRequired[str],
-        "AsyncInferenceConfig": NotRequired[AsyncInferenceConfigTypeDef],
-        "ExplainerConfig": NotRequired[ExplainerConfigTypeDef],
-        "ShadowProductionVariants": NotRequired[Sequence[ProductionVariantTypeDef]],
-        "ExecutionRoleArn": NotRequired[str],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
-        "EnableNetworkIsolation": NotRequired[bool],
     },
 )
+RecommendationJobInputConfigUnionTypeDef = Union[
+    RecommendationJobInputConfigTypeDef, RecommendationJobInputConfigOutputTypeDef
+]
 DescribeEndpointConfigOutputTypeDef = TypedDict(
     "DescribeEndpointConfigOutputTypeDef",
     {
         "EndpointConfigName": str,
         "EndpointConfigArn": str,
         "ProductionVariants": List[ProductionVariantTypeDef],
-        "DataCaptureConfig": DataCaptureConfigTypeDef,
+        "DataCaptureConfig": DataCaptureConfigOutputTypeDef,
         "KmsKeyId": str,
         "CreationTime": datetime,
-        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
-        "ExplainerConfig": ExplainerConfigTypeDef,
+        "AsyncInferenceConfig": AsyncInferenceConfigOutputTypeDef,
+        "ExplainerConfig": ExplainerConfigOutputTypeDef,
         "ShadowProductionVariants": List[ProductionVariantTypeDef],
         "ExecutionRoleArn": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "EnableNetworkIsolation": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeEndpointOutputTypeDef = TypedDict(
     "DescribeEndpointOutputTypeDef",
     {
@@ -13222,223 +14259,246 @@
         "EndpointConfigName": str,
         "ProductionVariants": List[ProductionVariantSummaryTypeDef],
         "DataCaptureConfig": DataCaptureConfigSummaryTypeDef,
         "EndpointStatus": EndpointStatusType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "LastDeploymentConfig": DeploymentConfigTypeDef,
-        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
+        "LastDeploymentConfig": DeploymentConfigOutputTypeDef,
+        "AsyncInferenceConfig": AsyncInferenceConfigOutputTypeDef,
         "PendingDeploymentSummary": PendingDeploymentSummaryTypeDef,
-        "ExplainerConfig": ExplainerConfigTypeDef,
+        "ExplainerConfig": ExplainerConfigOutputTypeDef,
         "ShadowProductionVariants": List[ProductionVariantSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-HyperParameterTuningJobSearchEntityPaginatorTypeDef = TypedDict(
-    "HyperParameterTuningJobSearchEntityPaginatorTypeDef",
-    {
-        "HyperParameterTuningJobName": NotRequired[str],
-        "HyperParameterTuningJobArn": NotRequired[str],
-        "HyperParameterTuningJobConfig": NotRequired[HyperParameterTuningJobConfigPaginatorTypeDef],
-        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionPaginatorTypeDef],
-        "TrainingJobDefinitions": NotRequired[
-            List[HyperParameterTrainingJobDefinitionPaginatorTypeDef]
-        ],
-        "HyperParameterTuningJobStatus": NotRequired[HyperParameterTuningJobStatusType],
-        "CreationTime": NotRequired[datetime],
-        "HyperParameterTuningEndTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "TrainingJobStatusCounters": NotRequired[TrainingJobStatusCountersTypeDef],
-        "ObjectiveStatusCounters": NotRequired[ObjectiveStatusCountersTypeDef],
-        "BestTrainingJob": NotRequired[HyperParameterTrainingJobSummaryTypeDef],
-        "OverallBestTrainingJob": NotRequired[HyperParameterTrainingJobSummaryTypeDef],
-        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigPaginatorTypeDef],
-        "FailureReason": NotRequired[str],
-        "TuningJobCompletionDetails": NotRequired[HyperParameterTuningJobCompletionDetailsTypeDef],
-        "ConsumedResources": NotRequired[HyperParameterTuningJobConsumedResourcesTypeDef],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
-CreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
-    "CreateHyperParameterTuningJobRequestRequestTypeDef",
+CreateEndpointConfigInputRequestTypeDef = TypedDict(
+    "CreateEndpointConfigInputRequestTypeDef",
     {
-        "HyperParameterTuningJobName": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
-        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionTypeDef],
-        "TrainingJobDefinitions": NotRequired[Sequence[HyperParameterTrainingJobDefinitionTypeDef]],
-        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigTypeDef],
+        "EndpointConfigName": str,
+        "ProductionVariants": Sequence[ProductionVariantTypeDef],
+        "DataCaptureConfig": NotRequired[DataCaptureConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
-        "Autotune": NotRequired[AutotuneTypeDef],
+        "KmsKeyId": NotRequired[str],
+        "AsyncInferenceConfig": NotRequired[AsyncInferenceConfigTypeDef],
+        "ExplainerConfig": NotRequired[ExplainerConfigTypeDef],
+        "ShadowProductionVariants": NotRequired[Sequence[ProductionVariantTypeDef]],
+        "ExecutionRoleArn": NotRequired[str],
+        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "EnableNetworkIsolation": NotRequired[bool],
     },
 )
+ExplainerConfigUnionTypeDef = Union[ExplainerConfigTypeDef, ExplainerConfigOutputTypeDef]
 DescribeHyperParameterTuningJobResponseTypeDef = TypedDict(
     "DescribeHyperParameterTuningJobResponseTypeDef",
     {
         "HyperParameterTuningJobName": str,
         "HyperParameterTuningJobArn": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
-        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
-        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionTypeDef],
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigOutputTypeDef,
+        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionOutputTypeDef,
+        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionOutputTypeDef],
         "HyperParameterTuningJobStatus": HyperParameterTuningJobStatusType,
         "CreationTime": datetime,
         "HyperParameterTuningEndTime": datetime,
         "LastModifiedTime": datetime,
         "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
         "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
         "BestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
         "OverallBestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
-        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
+        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigOutputTypeDef,
         "Autotune": AutotuneTypeDef,
         "FailureReason": str,
         "TuningJobCompletionDetails": HyperParameterTuningJobCompletionDetailsTypeDef,
         "ConsumedResources": HyperParameterTuningJobConsumedResourcesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 HyperParameterTuningJobSearchEntityTypeDef = TypedDict(
     "HyperParameterTuningJobSearchEntityTypeDef",
     {
         "HyperParameterTuningJobName": NotRequired[str],
         "HyperParameterTuningJobArn": NotRequired[str],
-        "HyperParameterTuningJobConfig": NotRequired[HyperParameterTuningJobConfigTypeDef],
-        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionTypeDef],
-        "TrainingJobDefinitions": NotRequired[List[HyperParameterTrainingJobDefinitionTypeDef]],
+        "HyperParameterTuningJobConfig": NotRequired[HyperParameterTuningJobConfigOutputTypeDef],
+        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionOutputTypeDef],
+        "TrainingJobDefinitions": NotRequired[
+            List[HyperParameterTrainingJobDefinitionOutputTypeDef]
+        ],
         "HyperParameterTuningJobStatus": NotRequired[HyperParameterTuningJobStatusType],
         "CreationTime": NotRequired[datetime],
         "HyperParameterTuningEndTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
         "TrainingJobStatusCounters": NotRequired[TrainingJobStatusCountersTypeDef],
         "ObjectiveStatusCounters": NotRequired[ObjectiveStatusCountersTypeDef],
         "BestTrainingJob": NotRequired[HyperParameterTrainingJobSummaryTypeDef],
         "OverallBestTrainingJob": NotRequired[HyperParameterTrainingJobSummaryTypeDef],
-        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigTypeDef],
+        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigOutputTypeDef],
         "FailureReason": NotRequired[str],
         "TuningJobCompletionDetails": NotRequired[HyperParameterTuningJobCompletionDetailsTypeDef],
         "ConsumedResources": NotRequired[HyperParameterTuningJobConsumedResourcesTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
+CreateTrainingJobRequestRequestTypeDef = TypedDict(
+    "CreateTrainingJobRequestRequestTypeDef",
+    {
+        "TrainingJobName": str,
+        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
+        "RoleArn": str,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "ResourceConfig": ResourceConfigTypeDef,
+        "StoppingCondition": StoppingConditionTypeDef,
+        "HyperParameters": NotRequired[Mapping[str, str]],
+        "InputDataConfig": NotRequired[Sequence[ChannelUnionTypeDef]],
+        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "EnableNetworkIsolation": NotRequired[bool],
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "EnableManagedSpotTraining": NotRequired[bool],
+        "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
+        "DebugHookConfig": NotRequired[DebugHookConfigTypeDef],
+        "DebugRuleConfigurations": NotRequired[Sequence[DebugRuleConfigurationUnionTypeDef]],
+        "TensorBoardOutputConfig": NotRequired[TensorBoardOutputConfigTypeDef],
+        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
+        "ProfilerConfig": NotRequired[ProfilerConfigTypeDef],
+        "ProfilerRuleConfigurations": NotRequired[Sequence[ProfilerRuleConfigurationUnionTypeDef]],
+        "Environment": NotRequired[Mapping[str, str]],
+        "RetryStrategy": NotRequired[RetryStrategyTypeDef],
+        "RemoteDebugConfig": NotRequired[RemoteDebugConfigTypeDef],
+        "InfraCheckConfig": NotRequired[InfraCheckConfigTypeDef],
+        "SessionChainingConfig": NotRequired[SessionChainingConfigTypeDef],
+    },
+)
+HyperParameterTrainingJobDefinitionUnionTypeDef = Union[
+    HyperParameterTrainingJobDefinitionTypeDef,
+    HyperParameterTrainingJobDefinitionExtraOutputTypeDef,
+]
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "Spaces": List[SpaceDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListInferenceRecommendationsJobStepsResponseTypeDef = TypedDict(
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
     {
         "Steps": List[InferenceRecommendationsJobStepTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListLabelingJobsResponsePaginatorTypeDef = TypedDict(
-    "ListLabelingJobsResponsePaginatorTypeDef",
-    {
-        "LabelingJobSummaryList": List[LabelingJobSummaryPaginatorTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+TrainingSpecificationUnionTypeDef = Union[
+    TrainingSpecificationTypeDef, TrainingSpecificationOutputTypeDef
+]
 ListLabelingJobsResponseTypeDef = TypedDict(
     "ListLabelingJobsResponseTypeDef",
     {
         "LabelingJobSummaryList": List[LabelingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DynamicScalingConfigurationTypeDef = TypedDict(
     "DynamicScalingConfigurationTypeDef",
     {
         "MinCapacity": NotRequired[int],
         "MaxCapacity": NotRequired[int],
         "ScaleInCooldown": NotRequired[int],
         "ScaleOutCooldown": NotRequired[int],
         "ScalingPolicies": NotRequired[List[ScalingPolicyTypeDef]],
     },
 )
-ModelPaginatorTypeDef = TypedDict(
-    "ModelPaginatorTypeDef",
-    {
-        "ModelName": NotRequired[str],
-        "PrimaryContainer": NotRequired[ContainerDefinitionPaginatorTypeDef],
-        "Containers": NotRequired[List[ContainerDefinitionPaginatorTypeDef]],
-        "InferenceExecutionConfig": NotRequired[InferenceExecutionConfigTypeDef],
-        "ExecutionRoleArn": NotRequired[str],
-        "VpcConfig": NotRequired[VpcConfigPaginatorTypeDef],
-        "CreationTime": NotRequired[datetime],
-        "ModelArn": NotRequired[str],
-        "EnableNetworkIsolation": NotRequired[bool],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "DeploymentRecommendation": NotRequired[DeploymentRecommendationTypeDef],
-    },
-)
-CreateModelInputRequestTypeDef = TypedDict(
-    "CreateModelInputRequestTypeDef",
-    {
-        "ModelName": str,
-        "PrimaryContainer": NotRequired[ContainerDefinitionTypeDef],
-        "Containers": NotRequired[Sequence[ContainerDefinitionTypeDef]],
-        "InferenceExecutionConfig": NotRequired[InferenceExecutionConfigTypeDef],
-        "ExecutionRoleArn": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
-        "EnableNetworkIsolation": NotRequired[bool],
-    },
-)
 DescribeModelOutputTypeDef = TypedDict(
     "DescribeModelOutputTypeDef",
     {
         "ModelName": str,
-        "PrimaryContainer": ContainerDefinitionTypeDef,
-        "Containers": List[ContainerDefinitionTypeDef],
+        "PrimaryContainer": ContainerDefinitionOutputTypeDef,
+        "Containers": List[ContainerDefinitionOutputTypeDef],
         "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
         "ExecutionRoleArn": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "CreationTime": datetime,
         "ModelArn": str,
         "EnableNetworkIsolation": bool,
         "DeploymentRecommendation": DeploymentRecommendationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ModelTypeDef = TypedDict(
     "ModelTypeDef",
     {
         "ModelName": NotRequired[str],
-        "PrimaryContainer": NotRequired[ContainerDefinitionTypeDef],
-        "Containers": NotRequired[List[ContainerDefinitionTypeDef]],
+        "PrimaryContainer": NotRequired[ContainerDefinitionOutputTypeDef],
+        "Containers": NotRequired[List[ContainerDefinitionOutputTypeDef]],
         "InferenceExecutionConfig": NotRequired[InferenceExecutionConfigTypeDef],
         "ExecutionRoleArn": NotRequired[str],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
         "CreationTime": NotRequired[datetime],
         "ModelArn": NotRequired[str],
         "EnableNetworkIsolation": NotRequired[bool],
         "Tags": NotRequired[List[TagTypeDef]],
         "DeploymentRecommendation": NotRequired[DeploymentRecommendationTypeDef],
     },
 )
-AdditionalInferenceSpecificationDefinitionPaginatorTypeDef = TypedDict(
-    "AdditionalInferenceSpecificationDefinitionPaginatorTypeDef",
+ContainerDefinitionUnionTypeDef = Union[
+    ContainerDefinitionTypeDef, ContainerDefinitionExtraOutputTypeDef
+]
+AdditionalInferenceSpecificationDefinitionExtraOutputTypeDef = TypedDict(
+    "AdditionalInferenceSpecificationDefinitionExtraOutputTypeDef",
     {
         "Name": str,
-        "Containers": List[ModelPackageContainerDefinitionTypeDef],
+        "Containers": List[ModelPackageContainerDefinitionExtraOutputTypeDef],
         "Description": NotRequired[str],
         "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
         "SupportedRealtimeInferenceInstanceTypes": NotRequired[
             List[ProductionVariantInstanceTypeType]
         ],
         "SupportedContentTypes": NotRequired[List[str]],
         "SupportedResponseMIMETypes": NotRequired[List[str]],
     },
 )
+InferenceSpecificationExtraOutputTypeDef = TypedDict(
+    "InferenceSpecificationExtraOutputTypeDef",
+    {
+        "Containers": List[ModelPackageContainerDefinitionExtraOutputTypeDef],
+        "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
+        "SupportedRealtimeInferenceInstanceTypes": NotRequired[
+            List[ProductionVariantInstanceTypeType]
+        ],
+        "SupportedContentTypes": NotRequired[List[str]],
+        "SupportedResponseMIMETypes": NotRequired[List[str]],
+    },
+)
+AdditionalInferenceSpecificationDefinitionOutputTypeDef = TypedDict(
+    "AdditionalInferenceSpecificationDefinitionOutputTypeDef",
+    {
+        "Name": str,
+        "Containers": List[ModelPackageContainerDefinitionOutputTypeDef],
+        "Description": NotRequired[str],
+        "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
+        "SupportedRealtimeInferenceInstanceTypes": NotRequired[
+            List[ProductionVariantInstanceTypeType]
+        ],
+        "SupportedContentTypes": NotRequired[List[str]],
+        "SupportedResponseMIMETypes": NotRequired[List[str]],
+    },
+)
+InferenceSpecificationOutputTypeDef = TypedDict(
+    "InferenceSpecificationOutputTypeDef",
+    {
+        "Containers": List[ModelPackageContainerDefinitionOutputTypeDef],
+        "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
+        "SupportedRealtimeInferenceInstanceTypes": NotRequired[
+            List[ProductionVariantInstanceTypeType]
+        ],
+        "SupportedContentTypes": NotRequired[List[str]],
+        "SupportedResponseMIMETypes": NotRequired[List[str]],
+    },
+)
 AdditionalInferenceSpecificationDefinitionTypeDef = TypedDict(
     "AdditionalInferenceSpecificationDefinitionTypeDef",
     {
         "Name": str,
         "Containers": Sequence[ModelPackageContainerDefinitionTypeDef],
         "Description": NotRequired[str],
         "SupportedTransformInstanceTypes": NotRequired[Sequence[TransformInstanceTypeType]],
@@ -13448,196 +14508,241 @@
         "SupportedContentTypes": NotRequired[Sequence[str]],
         "SupportedResponseMIMETypes": NotRequired[Sequence[str]],
     },
 )
 InferenceSpecificationTypeDef = TypedDict(
     "InferenceSpecificationTypeDef",
     {
-        "Containers": List[ModelPackageContainerDefinitionTypeDef],
-        "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
+        "Containers": Sequence[ModelPackageContainerDefinitionTypeDef],
+        "SupportedTransformInstanceTypes": NotRequired[Sequence[TransformInstanceTypeType]],
         "SupportedRealtimeInferenceInstanceTypes": NotRequired[
-            List[ProductionVariantInstanceTypeType]
+            Sequence[ProductionVariantInstanceTypeType]
         ],
-        "SupportedContentTypes": NotRequired[List[str]],
-        "SupportedResponseMIMETypes": NotRequired[List[str]],
+        "SupportedContentTypes": NotRequired[Sequence[str]],
+        "SupportedResponseMIMETypes": NotRequired[Sequence[str]],
     },
 )
-SourceAlgorithmSpecificationPaginatorTypeDef = TypedDict(
-    "SourceAlgorithmSpecificationPaginatorTypeDef",
+SourceAlgorithmSpecificationExtraOutputTypeDef = TypedDict(
+    "SourceAlgorithmSpecificationExtraOutputTypeDef",
+    {
+        "SourceAlgorithms": List[SourceAlgorithmTypeDef],
+    },
+)
+SourceAlgorithmSpecificationOutputTypeDef = TypedDict(
+    "SourceAlgorithmSpecificationOutputTypeDef",
     {
         "SourceAlgorithms": List[SourceAlgorithmTypeDef],
     },
 )
 SourceAlgorithmSpecificationTypeDef = TypedDict(
     "SourceAlgorithmSpecificationTypeDef",
     {
         "SourceAlgorithms": Sequence[SourceAlgorithmTypeDef],
     },
 )
-MonitoringJobDefinitionPaginatorTypeDef = TypedDict(
-    "MonitoringJobDefinitionPaginatorTypeDef",
+MonitoringJobDefinitionExtraOutputTypeDef = TypedDict(
+    "MonitoringJobDefinitionExtraOutputTypeDef",
     {
-        "MonitoringInputs": List[MonitoringInputPaginatorTypeDef],
-        "MonitoringOutputConfig": MonitoringOutputConfigPaginatorTypeDef,
+        "MonitoringInputs": List[MonitoringInputExtraOutputTypeDef],
+        "MonitoringOutputConfig": MonitoringOutputConfigExtraOutputTypeDef,
         "MonitoringResources": MonitoringResourcesTypeDef,
-        "MonitoringAppSpecification": MonitoringAppSpecificationPaginatorTypeDef,
+        "MonitoringAppSpecification": MonitoringAppSpecificationExtraOutputTypeDef,
         "RoleArn": str,
         "BaselineConfig": NotRequired[MonitoringBaselineConfigTypeDef],
         "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
         "Environment": NotRequired[Dict[str, str]],
-        "NetworkConfig": NotRequired[NetworkConfigPaginatorTypeDef],
+        "NetworkConfig": NotRequired[NetworkConfigExtraOutputTypeDef],
     },
 )
-CreateDataQualityJobDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateDataQualityJobDefinitionRequestRequestTypeDef",
+DescribeDataQualityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeDataQualityJobDefinitionResponseTypeDef",
     {
+        "JobDefinitionArn": str,
         "JobDefinitionName": str,
-        "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
-        "DataQualityJobInput": DataQualityJobInputTypeDef,
-        "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "CreationTime": datetime,
+        "DataQualityBaselineConfig": DataQualityBaselineConfigTypeDef,
+        "DataQualityAppSpecification": DataQualityAppSpecificationOutputTypeDef,
+        "DataQualityJobInput": DataQualityJobInputOutputTypeDef,
+        "DataQualityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
         "RoleArn": str,
-        "DataQualityBaselineConfig": NotRequired[DataQualityBaselineConfigTypeDef],
-        "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
-        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeDataQualityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeDataQualityJobDefinitionResponseTypeDef",
+DescribeModelBiasJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelBiasJobDefinitionResponseTypeDef",
     {
         "JobDefinitionArn": str,
         "JobDefinitionName": str,
         "CreationTime": datetime,
-        "DataQualityBaselineConfig": DataQualityBaselineConfigTypeDef,
-        "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
-        "DataQualityJobInput": DataQualityJobInputTypeDef,
-        "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "ModelBiasBaselineConfig": ModelBiasBaselineConfigTypeDef,
+        "ModelBiasAppSpecification": ModelBiasAppSpecificationOutputTypeDef,
+        "ModelBiasJobInput": ModelBiasJobInputOutputTypeDef,
+        "ModelBiasJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
         "RoleArn": str,
         "StoppingCondition": MonitoringStoppingConditionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateModelBiasJobDefinitionRequestRequestTypeDef",
+DescribeModelExplainabilityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
     {
+        "JobDefinitionArn": str,
         "JobDefinitionName": str,
-        "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
-        "ModelBiasJobInput": ModelBiasJobInputTypeDef,
-        "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "CreationTime": datetime,
+        "ModelExplainabilityBaselineConfig": ModelExplainabilityBaselineConfigTypeDef,
+        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationOutputTypeDef,
+        "ModelExplainabilityJobInput": ModelExplainabilityJobInputOutputTypeDef,
+        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
         "RoleArn": str,
-        "ModelBiasBaselineConfig": NotRequired[ModelBiasBaselineConfigTypeDef],
-        "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
-        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeModelBiasJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelBiasJobDefinitionResponseTypeDef",
+DescribeModelQualityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelQualityJobDefinitionResponseTypeDef",
     {
         "JobDefinitionArn": str,
         "JobDefinitionName": str,
         "CreationTime": datetime,
-        "ModelBiasBaselineConfig": ModelBiasBaselineConfigTypeDef,
-        "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
-        "ModelBiasJobInput": ModelBiasJobInputTypeDef,
-        "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "ModelQualityBaselineConfig": ModelQualityBaselineConfigTypeDef,
+        "ModelQualityAppSpecification": ModelQualityAppSpecificationOutputTypeDef,
+        "ModelQualityJobInput": ModelQualityJobInputOutputTypeDef,
+        "ModelQualityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
         "RoleArn": str,
         "StoppingCondition": MonitoringStoppingConditionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
+MonitoringJobDefinitionOutputTypeDef = TypedDict(
+    "MonitoringJobDefinitionOutputTypeDef",
+    {
+        "MonitoringInputs": List[MonitoringInputOutputTypeDef],
+        "MonitoringOutputConfig": MonitoringOutputConfigOutputTypeDef,
+        "MonitoringResources": MonitoringResourcesTypeDef,
+        "MonitoringAppSpecification": MonitoringAppSpecificationOutputTypeDef,
+        "RoleArn": str,
+        "BaselineConfig": NotRequired[MonitoringBaselineConfigTypeDef],
+        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
+        "Environment": NotRequired[Dict[str, str]],
+        "NetworkConfig": NotRequired[NetworkConfigOutputTypeDef],
+    },
+)
+CreateDataQualityJobDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateDataQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
-        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
-        "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
-        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
+        "DataQualityJobInput": DataQualityJobInputTypeDef,
+        "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
         "RoleArn": str,
-        "ModelExplainabilityBaselineConfig": NotRequired[ModelExplainabilityBaselineConfigTypeDef],
+        "DataQualityBaselineConfig": NotRequired[DataQualityBaselineConfigTypeDef],
         "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
         "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-DescribeModelExplainabilityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
+DataQualityJobInputUnionTypeDef = Union[
+    DataQualityJobInputTypeDef, DataQualityJobInputOutputTypeDef
+]
+CreateModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateModelBiasJobDefinitionRequestRequestTypeDef",
     {
-        "JobDefinitionArn": str,
         "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelExplainabilityBaselineConfig": ModelExplainabilityBaselineConfigTypeDef,
-        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
-        "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
-        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
+        "ModelBiasJobInput": ModelBiasJobInputTypeDef,
+        "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigTypeDef,
         "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ModelBiasBaselineConfig": NotRequired[ModelBiasBaselineConfigTypeDef],
+        "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
+        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-CreateModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateModelQualityJobDefinitionRequestRequestTypeDef",
+ModelBiasJobInputUnionTypeDef = Union[ModelBiasJobInputTypeDef, ModelBiasJobInputOutputTypeDef]
+CreateModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
-        "ModelQualityAppSpecification": ModelQualityAppSpecificationTypeDef,
-        "ModelQualityJobInput": ModelQualityJobInputTypeDef,
-        "ModelQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
+        "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
+        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
         "RoleArn": str,
-        "ModelQualityBaselineConfig": NotRequired[ModelQualityBaselineConfigTypeDef],
+        "ModelExplainabilityBaselineConfig": NotRequired[ModelExplainabilityBaselineConfigTypeDef],
         "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
         "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-DescribeModelQualityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelQualityJobDefinitionResponseTypeDef",
+ModelExplainabilityJobInputUnionTypeDef = Union[
+    ModelExplainabilityJobInputTypeDef, ModelExplainabilityJobInputOutputTypeDef
+]
+CreateModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateModelQualityJobDefinitionRequestRequestTypeDef",
     {
-        "JobDefinitionArn": str,
         "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelQualityBaselineConfig": ModelQualityBaselineConfigTypeDef,
         "ModelQualityAppSpecification": ModelQualityAppSpecificationTypeDef,
         "ModelQualityJobInput": ModelQualityJobInputTypeDef,
         "ModelQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigTypeDef,
         "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ModelQualityBaselineConfig": NotRequired[ModelQualityBaselineConfigTypeDef],
+        "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
+        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+ModelQualityJobInputUnionTypeDef = Union[
+    ModelQualityJobInputTypeDef, ModelQualityJobInputOutputTypeDef
+]
 MonitoringJobDefinitionTypeDef = TypedDict(
     "MonitoringJobDefinitionTypeDef",
     {
         "MonitoringInputs": Sequence[MonitoringInputTypeDef],
         "MonitoringOutputConfig": MonitoringOutputConfigTypeDef,
         "MonitoringResources": MonitoringResourcesTypeDef,
         "MonitoringAppSpecification": MonitoringAppSpecificationTypeDef,
         "RoleArn": str,
         "BaselineConfig": NotRequired[MonitoringBaselineConfigTypeDef],
         "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
         "Environment": NotRequired[Mapping[str, str]],
         "NetworkConfig": NotRequired[NetworkConfigTypeDef],
     },
 )
-ModelPackageValidationProfilePaginatorTypeDef = TypedDict(
-    "ModelPackageValidationProfilePaginatorTypeDef",
+ModelPackageValidationProfileExtraOutputTypeDef = TypedDict(
+    "ModelPackageValidationProfileExtraOutputTypeDef",
+    {
+        "ProfileName": str,
+        "TransformJobDefinition": TransformJobDefinitionExtraOutputTypeDef,
+    },
+)
+AlgorithmValidationProfileOutputTypeDef = TypedDict(
+    "AlgorithmValidationProfileOutputTypeDef",
     {
         "ProfileName": str,
-        "TransformJobDefinition": TransformJobDefinitionPaginatorTypeDef,
+        "TrainingJobDefinition": TrainingJobDefinitionOutputTypeDef,
+        "TransformJobDefinition": NotRequired[TransformJobDefinitionOutputTypeDef],
+    },
+)
+ModelPackageValidationProfileOutputTypeDef = TypedDict(
+    "ModelPackageValidationProfileOutputTypeDef",
+    {
+        "ProfileName": str,
+        "TransformJobDefinition": TransformJobDefinitionOutputTypeDef,
     },
 )
 AlgorithmValidationProfileTypeDef = TypedDict(
     "AlgorithmValidationProfileTypeDef",
     {
         "ProfileName": str,
         "TrainingJobDefinition": TrainingJobDefinitionTypeDef,
@@ -13647,96 +14752,132 @@
 ModelPackageValidationProfileTypeDef = TypedDict(
     "ModelPackageValidationProfileTypeDef",
     {
         "ProfileName": str,
         "TransformJobDefinition": TransformJobDefinitionTypeDef,
     },
 )
-TrialComponentSourceDetailPaginatorTypeDef = TypedDict(
-    "TrialComponentSourceDetailPaginatorTypeDef",
-    {
-        "SourceArn": NotRequired[str],
-        "TrainingJob": NotRequired[TrainingJobPaginatorTypeDef],
-        "ProcessingJob": NotRequired[ProcessingJobPaginatorTypeDef],
-        "TransformJob": NotRequired[TransformJobTypeDef],
-    },
-)
 TrialComponentSourceDetailTypeDef = TypedDict(
     "TrialComponentSourceDetailTypeDef",
     {
         "SourceArn": NotRequired[str],
         "TrainingJob": NotRequired[TrainingJobTypeDef],
         "ProcessingJob": NotRequired[ProcessingJobTypeDef],
         "TransformJob": NotRequired[TransformJobTypeDef],
     },
 )
+CreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
+    "CreateHyperParameterTuningJobRequestRequestTypeDef",
+    {
+        "HyperParameterTuningJobName": str,
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
+        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionTypeDef],
+        "TrainingJobDefinitions": NotRequired[
+            Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef]
+        ],
+        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "Autotune": NotRequired[AutotuneTypeDef],
+    },
+)
 GetScalingConfigurationRecommendationResponseTypeDef = TypedDict(
     "GetScalingConfigurationRecommendationResponseTypeDef",
     {
         "InferenceRecommendationsJobName": str,
         "RecommendationId": str,
         "EndpointName": str,
         "TargetCpuUtilizationPerCore": int,
         "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
         "Metric": ScalingPolicyMetricTypeDef,
         "DynamicScalingConfiguration": DynamicScalingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateModelInputRequestTypeDef = TypedDict(
+    "CreateModelInputRequestTypeDef",
+    {
+        "ModelName": str,
+        "PrimaryContainer": NotRequired[ContainerDefinitionTypeDef],
+        "Containers": NotRequired[Sequence[ContainerDefinitionUnionTypeDef]],
+        "InferenceExecutionConfig": NotRequired[InferenceExecutionConfigTypeDef],
+        "ExecutionRoleArn": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "EnableNetworkIsolation": NotRequired[bool],
+    },
+)
 BatchDescribeModelPackageSummaryTypeDef = TypedDict(
     "BatchDescribeModelPackageSummaryTypeDef",
     {
         "ModelPackageGroupName": str,
         "ModelPackageArn": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
         "ModelPackageVersion": NotRequired[int],
         "ModelPackageDescription": NotRequired[str],
         "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
     },
 )
-UpdateModelPackageInputRequestTypeDef = TypedDict(
-    "UpdateModelPackageInputRequestTypeDef",
+AdditionalInferenceSpecificationDefinitionUnionTypeDef = Union[
+    AdditionalInferenceSpecificationDefinitionTypeDef,
+    AdditionalInferenceSpecificationDefinitionExtraOutputTypeDef,
+]
+InferenceSpecificationUnionTypeDef = Union[
+    InferenceSpecificationTypeDef, InferenceSpecificationExtraOutputTypeDef
+]
+SourceAlgorithmSpecificationUnionTypeDef = Union[
+    SourceAlgorithmSpecificationTypeDef, SourceAlgorithmSpecificationExtraOutputTypeDef
+]
+MonitoringScheduleConfigExtraOutputTypeDef = TypedDict(
+    "MonitoringScheduleConfigExtraOutputTypeDef",
     {
-        "ModelPackageArn": str,
-        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
-        "ApprovalDescription": NotRequired[str],
-        "CustomerMetadataProperties": NotRequired[Mapping[str, str]],
-        "CustomerMetadataPropertiesToRemove": NotRequired[Sequence[str]],
-        "AdditionalInferenceSpecificationsToAdd": NotRequired[
-            Sequence[AdditionalInferenceSpecificationDefinitionTypeDef]
-        ],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "SourceUri": NotRequired[str],
+        "ScheduleConfig": NotRequired[ScheduleConfigTypeDef],
+        "MonitoringJobDefinition": NotRequired[MonitoringJobDefinitionExtraOutputTypeDef],
+        "MonitoringJobDefinitionName": NotRequired[str],
+        "MonitoringType": NotRequired[MonitoringTypeType],
     },
 )
-MonitoringScheduleConfigPaginatorTypeDef = TypedDict(
-    "MonitoringScheduleConfigPaginatorTypeDef",
+MonitoringScheduleConfigOutputTypeDef = TypedDict(
+    "MonitoringScheduleConfigOutputTypeDef",
     {
         "ScheduleConfig": NotRequired[ScheduleConfigTypeDef],
-        "MonitoringJobDefinition": NotRequired[MonitoringJobDefinitionPaginatorTypeDef],
+        "MonitoringJobDefinition": NotRequired[MonitoringJobDefinitionOutputTypeDef],
         "MonitoringJobDefinitionName": NotRequired[str],
         "MonitoringType": NotRequired[MonitoringTypeType],
     },
 )
 MonitoringScheduleConfigTypeDef = TypedDict(
     "MonitoringScheduleConfigTypeDef",
     {
         "ScheduleConfig": NotRequired[ScheduleConfigTypeDef],
         "MonitoringJobDefinition": NotRequired[MonitoringJobDefinitionTypeDef],
         "MonitoringJobDefinitionName": NotRequired[str],
         "MonitoringType": NotRequired[MonitoringTypeType],
     },
 )
-ModelPackageValidationSpecificationPaginatorTypeDef = TypedDict(
-    "ModelPackageValidationSpecificationPaginatorTypeDef",
+ModelPackageValidationSpecificationExtraOutputTypeDef = TypedDict(
+    "ModelPackageValidationSpecificationExtraOutputTypeDef",
+    {
+        "ValidationRole": str,
+        "ValidationProfiles": List[ModelPackageValidationProfileExtraOutputTypeDef],
+    },
+)
+AlgorithmValidationSpecificationOutputTypeDef = TypedDict(
+    "AlgorithmValidationSpecificationOutputTypeDef",
     {
         "ValidationRole": str,
-        "ValidationProfiles": List[ModelPackageValidationProfilePaginatorTypeDef],
+        "ValidationProfiles": List[AlgorithmValidationProfileOutputTypeDef],
+    },
+)
+ModelPackageValidationSpecificationOutputTypeDef = TypedDict(
+    "ModelPackageValidationSpecificationOutputTypeDef",
+    {
+        "ValidationRole": str,
+        "ValidationProfiles": List[ModelPackageValidationProfileOutputTypeDef],
     },
 )
 AlgorithmValidationSpecificationTypeDef = TypedDict(
     "AlgorithmValidationSpecificationTypeDef",
     {
         "ValidationRole": str,
         "ValidationProfiles": Sequence[AlgorithmValidationProfileTypeDef],
@@ -13745,40 +14886,14 @@
 ModelPackageValidationSpecificationTypeDef = TypedDict(
     "ModelPackageValidationSpecificationTypeDef",
     {
         "ValidationRole": str,
         "ValidationProfiles": Sequence[ModelPackageValidationProfileTypeDef],
     },
 )
-TrialComponentPaginatorTypeDef = TypedDict(
-    "TrialComponentPaginatorTypeDef",
-    {
-        "TrialComponentName": NotRequired[str],
-        "DisplayName": NotRequired[str],
-        "TrialComponentArn": NotRequired[str],
-        "Source": NotRequired[TrialComponentSourceTypeDef],
-        "Status": NotRequired[TrialComponentStatusTypeDef],
-        "StartTime": NotRequired[datetime],
-        "EndTime": NotRequired[datetime],
-        "CreationTime": NotRequired[datetime],
-        "CreatedBy": NotRequired[UserContextTypeDef],
-        "LastModifiedTime": NotRequired[datetime],
-        "LastModifiedBy": NotRequired[UserContextTypeDef],
-        "Parameters": NotRequired[Dict[str, TrialComponentParameterValueTypeDef]],
-        "InputArtifacts": NotRequired[Dict[str, TrialComponentArtifactTypeDef]],
-        "OutputArtifacts": NotRequired[Dict[str, TrialComponentArtifactTypeDef]],
-        "Metrics": NotRequired[List[TrialComponentMetricSummaryTypeDef]],
-        "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
-        "SourceDetail": NotRequired[TrialComponentSourceDetailPaginatorTypeDef],
-        "LineageGroupArn": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "Parents": NotRequired[List[ParentTypeDef]],
-        "RunName": NotRequired[str],
-    },
-)
 TrialComponentTypeDef = TypedDict(
     "TrialComponentTypeDef",
     {
         "TrialComponentName": NotRequired[str],
         "DisplayName": NotRequired[str],
         "TrialComponentArn": NotRequired[str],
         "Source": NotRequired[TrialComponentSourceTypeDef],
@@ -13805,66 +14920,40 @@
     "BatchDescribeModelPackageOutputTypeDef",
     {
         "ModelPackageSummaries": Dict[str, BatchDescribeModelPackageSummaryTypeDef],
         "BatchDescribeModelPackageErrorMap": Dict[str, BatchDescribeModelPackageErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ModelDashboardMonitoringSchedulePaginatorTypeDef = TypedDict(
-    "ModelDashboardMonitoringSchedulePaginatorTypeDef",
-    {
-        "MonitoringScheduleArn": NotRequired[str],
-        "MonitoringScheduleName": NotRequired[str],
-        "MonitoringScheduleStatus": NotRequired[ScheduleStatusType],
-        "MonitoringType": NotRequired[MonitoringTypeType],
-        "FailureReason": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigPaginatorTypeDef],
-        "EndpointName": NotRequired[str],
-        "MonitoringAlertSummaries": NotRequired[List[MonitoringAlertSummaryTypeDef]],
-        "LastMonitoringExecutionSummary": NotRequired[MonitoringExecutionSummaryTypeDef],
-        "BatchTransformInput": NotRequired[BatchTransformInputPaginatorTypeDef],
-    },
-)
-MonitoringSchedulePaginatorTypeDef = TypedDict(
-    "MonitoringSchedulePaginatorTypeDef",
-    {
-        "MonitoringScheduleArn": NotRequired[str],
-        "MonitoringScheduleName": NotRequired[str],
-        "MonitoringScheduleStatus": NotRequired[ScheduleStatusType],
-        "MonitoringType": NotRequired[MonitoringTypeType],
-        "FailureReason": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigPaginatorTypeDef],
-        "EndpointName": NotRequired[str],
-        "LastMonitoringExecutionSummary": NotRequired[MonitoringExecutionSummaryTypeDef],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
-CreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "CreateMonitoringScheduleRequestRequestTypeDef",
+UpdateModelPackageInputRequestTypeDef = TypedDict(
+    "UpdateModelPackageInputRequestTypeDef",
     {
-        "MonitoringScheduleName": str,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "ModelPackageArn": str,
+        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
+        "ApprovalDescription": NotRequired[str],
+        "CustomerMetadataProperties": NotRequired[Mapping[str, str]],
+        "CustomerMetadataPropertiesToRemove": NotRequired[Sequence[str]],
+        "AdditionalInferenceSpecificationsToAdd": NotRequired[
+            Sequence[AdditionalInferenceSpecificationDefinitionUnionTypeDef]
+        ],
+        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
+        "SourceUri": NotRequired[str],
     },
 )
 DescribeMonitoringScheduleResponseTypeDef = TypedDict(
     "DescribeMonitoringScheduleResponseTypeDef",
     {
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
         "MonitoringScheduleStatus": ScheduleStatusType,
         "MonitoringType": MonitoringTypeType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigOutputTypeDef,
         "EndpointName": str,
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ModelDashboardMonitoringScheduleTypeDef = TypedDict(
     "ModelDashboardMonitoringScheduleTypeDef",
@@ -13872,147 +14961,84 @@
         "MonitoringScheduleArn": NotRequired[str],
         "MonitoringScheduleName": NotRequired[str],
         "MonitoringScheduleStatus": NotRequired[ScheduleStatusType],
         "MonitoringType": NotRequired[MonitoringTypeType],
         "FailureReason": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
-        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigTypeDef],
+        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigOutputTypeDef],
         "EndpointName": NotRequired[str],
         "MonitoringAlertSummaries": NotRequired[List[MonitoringAlertSummaryTypeDef]],
         "LastMonitoringExecutionSummary": NotRequired[MonitoringExecutionSummaryTypeDef],
-        "BatchTransformInput": NotRequired[BatchTransformInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
     },
 )
 MonitoringScheduleTypeDef = TypedDict(
     "MonitoringScheduleTypeDef",
     {
         "MonitoringScheduleArn": NotRequired[str],
         "MonitoringScheduleName": NotRequired[str],
         "MonitoringScheduleStatus": NotRequired[ScheduleStatusType],
         "MonitoringType": NotRequired[MonitoringTypeType],
         "FailureReason": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
-        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigTypeDef],
+        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigOutputTypeDef],
         "EndpointName": NotRequired[str],
         "LastMonitoringExecutionSummary": NotRequired[MonitoringExecutionSummaryTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "UpdateMonitoringScheduleRequestRequestTypeDef",
+CreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "CreateMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-ModelPackagePaginatorTypeDef = TypedDict(
-    "ModelPackagePaginatorTypeDef",
-    {
-        "ModelPackageName": NotRequired[str],
-        "ModelPackageGroupName": NotRequired[str],
-        "ModelPackageVersion": NotRequired[int],
-        "ModelPackageArn": NotRequired[str],
-        "ModelPackageDescription": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationPaginatorTypeDef],
-        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationPaginatorTypeDef],
-        "ModelPackageStatus": NotRequired[ModelPackageStatusType],
-        "ModelPackageStatusDetails": NotRequired[ModelPackageStatusDetailsTypeDef],
-        "CertifyForMarketplace": NotRequired[bool],
-        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
-        "CreatedBy": NotRequired[UserContextTypeDef],
-        "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
-        "ModelMetrics": NotRequired[ModelMetricsTypeDef],
-        "LastModifiedTime": NotRequired[datetime],
-        "LastModifiedBy": NotRequired[UserContextTypeDef],
-        "ApprovalDescription": NotRequired[str],
-        "Domain": NotRequired[str],
-        "Task": NotRequired[str],
-        "SamplePayloadUrl": NotRequired[str],
-        "AdditionalInferenceSpecifications": NotRequired[
-            List[AdditionalInferenceSpecificationDefinitionPaginatorTypeDef]
-        ],
-        "SourceUri": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "CustomerMetadataProperties": NotRequired[Dict[str, str]],
-        "DriftCheckBaselines": NotRequired[DriftCheckBaselinesTypeDef],
-        "SkipModelValidation": NotRequired[SkipModelValidationType],
-    },
-)
-CreateAlgorithmInputRequestTypeDef = TypedDict(
-    "CreateAlgorithmInputRequestTypeDef",
+MonitoringScheduleConfigUnionTypeDef = Union[
+    MonitoringScheduleConfigTypeDef, MonitoringScheduleConfigExtraOutputTypeDef
+]
+UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "UpdateMonitoringScheduleRequestRequestTypeDef",
     {
-        "AlgorithmName": str,
-        "TrainingSpecification": TrainingSpecificationTypeDef,
-        "AlgorithmDescription": NotRequired[str],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "ValidationSpecification": NotRequired[AlgorithmValidationSpecificationTypeDef],
-        "CertifyForMarketplace": NotRequired[bool],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "MonitoringScheduleName": str,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
     },
 )
 DescribeAlgorithmOutputTypeDef = TypedDict(
     "DescribeAlgorithmOutputTypeDef",
     {
         "AlgorithmName": str,
         "AlgorithmArn": str,
         "AlgorithmDescription": str,
         "CreationTime": datetime,
-        "TrainingSpecification": TrainingSpecificationTypeDef,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
-        "ValidationSpecification": AlgorithmValidationSpecificationTypeDef,
+        "TrainingSpecification": TrainingSpecificationOutputTypeDef,
+        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
+        "ValidationSpecification": AlgorithmValidationSpecificationOutputTypeDef,
         "AlgorithmStatus": AlgorithmStatusType,
         "AlgorithmStatusDetails": AlgorithmStatusDetailsTypeDef,
         "ProductId": str,
         "CertifyForMarketplace": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateModelPackageInputRequestTypeDef = TypedDict(
-    "CreateModelPackageInputRequestTypeDef",
-    {
-        "ModelPackageName": NotRequired[str],
-        "ModelPackageGroupName": NotRequired[str],
-        "ModelPackageDescription": NotRequired[str],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationTypeDef],
-        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationTypeDef],
-        "CertifyForMarketplace": NotRequired[bool],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
-        "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
-        "ModelMetrics": NotRequired[ModelMetricsTypeDef],
-        "ClientToken": NotRequired[str],
-        "Domain": NotRequired[str],
-        "Task": NotRequired[str],
-        "SamplePayloadUrl": NotRequired[str],
-        "CustomerMetadataProperties": NotRequired[Mapping[str, str]],
-        "DriftCheckBaselines": NotRequired[DriftCheckBaselinesTypeDef],
-        "AdditionalInferenceSpecifications": NotRequired[
-            Sequence[AdditionalInferenceSpecificationDefinitionTypeDef]
-        ],
-        "SkipModelValidation": NotRequired[SkipModelValidationType],
-        "SourceUri": NotRequired[str],
-    },
-)
 DescribeModelPackageOutputTypeDef = TypedDict(
     "DescribeModelPackageOutputTypeDef",
     {
         "ModelPackageName": str,
         "ModelPackageGroupName": str,
         "ModelPackageVersion": int,
         "ModelPackageArn": str,
         "ModelPackageDescription": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
-        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
-        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
+        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
+        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationOutputTypeDef,
+        "ValidationSpecification": ModelPackageValidationSpecificationOutputTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
         "ModelPackageStatusDetails": ModelPackageStatusDetailsTypeDef,
         "CertifyForMarketplace": bool,
         "ModelApprovalStatus": ModelApprovalStatusType,
         "CreatedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
         "ModelMetrics": ModelMetricsTypeDef,
@@ -14021,15 +15047,15 @@
         "ApprovalDescription": str,
         "Domain": str,
         "Task": str,
         "SamplePayloadUrl": str,
         "CustomerMetadataProperties": Dict[str, str],
         "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
         "AdditionalInferenceSpecifications": List[
-            AdditionalInferenceSpecificationDefinitionTypeDef
+            AdditionalInferenceSpecificationDefinitionOutputTypeDef
         ],
         "SkipModelValidation": SkipModelValidationType,
         "SourceUri": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ModelPackageTypeDef = TypedDict(
@@ -14037,67 +15063,86 @@
     {
         "ModelPackageName": NotRequired[str],
         "ModelPackageGroupName": NotRequired[str],
         "ModelPackageVersion": NotRequired[int],
         "ModelPackageArn": NotRequired[str],
         "ModelPackageDescription": NotRequired[str],
         "CreationTime": NotRequired[datetime],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationTypeDef],
-        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationTypeDef],
+        "InferenceSpecification": NotRequired[InferenceSpecificationOutputTypeDef],
+        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationOutputTypeDef],
+        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationOutputTypeDef],
         "ModelPackageStatus": NotRequired[ModelPackageStatusType],
         "ModelPackageStatusDetails": NotRequired[ModelPackageStatusDetailsTypeDef],
         "CertifyForMarketplace": NotRequired[bool],
         "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
         "CreatedBy": NotRequired[UserContextTypeDef],
         "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
         "ModelMetrics": NotRequired[ModelMetricsTypeDef],
         "LastModifiedTime": NotRequired[datetime],
         "LastModifiedBy": NotRequired[UserContextTypeDef],
         "ApprovalDescription": NotRequired[str],
         "Domain": NotRequired[str],
         "Task": NotRequired[str],
         "SamplePayloadUrl": NotRequired[str],
         "AdditionalInferenceSpecifications": NotRequired[
-            List[AdditionalInferenceSpecificationDefinitionTypeDef]
+            List[AdditionalInferenceSpecificationDefinitionOutputTypeDef]
         ],
         "SourceUri": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "CustomerMetadataProperties": NotRequired[Dict[str, str]],
         "DriftCheckBaselines": NotRequired[DriftCheckBaselinesTypeDef],
         "SkipModelValidation": NotRequired[SkipModelValidationType],
     },
 )
-ModelDashboardModelPaginatorTypeDef = TypedDict(
-    "ModelDashboardModelPaginatorTypeDef",
+AlgorithmValidationSpecificationUnionTypeDef = Union[
+    AlgorithmValidationSpecificationTypeDef, AlgorithmValidationSpecificationOutputTypeDef
+]
+CreateAlgorithmInputRequestTypeDef = TypedDict(
+    "CreateAlgorithmInputRequestTypeDef",
     {
-        "Model": NotRequired[ModelPaginatorTypeDef],
-        "Endpoints": NotRequired[List[ModelDashboardEndpointTypeDef]],
-        "LastBatchTransformJob": NotRequired[TransformJobTypeDef],
-        "MonitoringSchedules": NotRequired[List[ModelDashboardMonitoringSchedulePaginatorTypeDef]],
-        "ModelCard": NotRequired[ModelDashboardModelCardTypeDef],
+        "AlgorithmName": str,
+        "TrainingSpecification": TrainingSpecificationTypeDef,
+        "AlgorithmDescription": NotRequired[str],
+        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
+        "ValidationSpecification": NotRequired[AlgorithmValidationSpecificationTypeDef],
+        "CertifyForMarketplace": NotRequired[bool],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-EndpointPaginatorTypeDef = TypedDict(
-    "EndpointPaginatorTypeDef",
+CreateModelPackageInputRequestTypeDef = TypedDict(
+    "CreateModelPackageInputRequestTypeDef",
     {
-        "EndpointName": str,
-        "EndpointArn": str,
-        "EndpointConfigName": str,
-        "EndpointStatus": EndpointStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ProductionVariants": NotRequired[List[ProductionVariantSummaryTypeDef]],
-        "DataCaptureConfig": NotRequired[DataCaptureConfigSummaryTypeDef],
-        "FailureReason": NotRequired[str],
-        "MonitoringSchedules": NotRequired[List[MonitoringSchedulePaginatorTypeDef]],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "ShadowProductionVariants": NotRequired[List[ProductionVariantSummaryTypeDef]],
+        "ModelPackageName": NotRequired[str],
+        "ModelPackageGroupName": NotRequired[str],
+        "ModelPackageDescription": NotRequired[str],
+        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
+        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationTypeDef],
+        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationTypeDef],
+        "CertifyForMarketplace": NotRequired[bool],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
+        "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
+        "ModelMetrics": NotRequired[ModelMetricsTypeDef],
+        "ClientToken": NotRequired[str],
+        "Domain": NotRequired[str],
+        "Task": NotRequired[str],
+        "SamplePayloadUrl": NotRequired[str],
+        "CustomerMetadataProperties": NotRequired[Mapping[str, str]],
+        "DriftCheckBaselines": NotRequired[DriftCheckBaselinesTypeDef],
+        "AdditionalInferenceSpecifications": NotRequired[
+            Sequence[AdditionalInferenceSpecificationDefinitionUnionTypeDef]
+        ],
+        "SkipModelValidation": NotRequired[SkipModelValidationType],
+        "SourceUri": NotRequired[str],
     },
 )
+ModelPackageValidationSpecificationUnionTypeDef = Union[
+    ModelPackageValidationSpecificationTypeDef,
+    ModelPackageValidationSpecificationExtraOutputTypeDef,
+]
 ModelDashboardModelTypeDef = TypedDict(
     "ModelDashboardModelTypeDef",
     {
         "Model": NotRequired[ModelTypeDef],
         "Endpoints": NotRequired[List[ModelDashboardEndpointTypeDef]],
         "LastBatchTransformJob": NotRequired[TransformJobTypeDef],
         "MonitoringSchedules": NotRequired[List[ModelDashboardMonitoringScheduleTypeDef]],
@@ -14117,34 +15162,14 @@
         "DataCaptureConfig": NotRequired[DataCaptureConfigSummaryTypeDef],
         "FailureReason": NotRequired[str],
         "MonitoringSchedules": NotRequired[List[MonitoringScheduleTypeDef]],
         "Tags": NotRequired[List[TagTypeDef]],
         "ShadowProductionVariants": NotRequired[List[ProductionVariantSummaryTypeDef]],
     },
 )
-SearchRecordPaginatorTypeDef = TypedDict(
-    "SearchRecordPaginatorTypeDef",
-    {
-        "TrainingJob": NotRequired[TrainingJobPaginatorTypeDef],
-        "Experiment": NotRequired[ExperimentTypeDef],
-        "Trial": NotRequired[TrialTypeDef],
-        "TrialComponent": NotRequired[TrialComponentPaginatorTypeDef],
-        "Endpoint": NotRequired[EndpointPaginatorTypeDef],
-        "ModelPackage": NotRequired[ModelPackagePaginatorTypeDef],
-        "ModelPackageGroup": NotRequired[ModelPackageGroupTypeDef],
-        "Pipeline": NotRequired[PipelineTypeDef],
-        "PipelineExecution": NotRequired[PipelineExecutionTypeDef],
-        "FeatureGroup": NotRequired[FeatureGroupTypeDef],
-        "FeatureMetadata": NotRequired[FeatureMetadataTypeDef],
-        "Project": NotRequired[ProjectPaginatorTypeDef],
-        "HyperParameterTuningJob": NotRequired[HyperParameterTuningJobSearchEntityPaginatorTypeDef],
-        "ModelCard": NotRequired[ModelCardTypeDef],
-        "Model": NotRequired[ModelDashboardModelPaginatorTypeDef],
-    },
-)
 SearchRecordTypeDef = TypedDict(
     "SearchRecordTypeDef",
     {
         "TrainingJob": NotRequired[TrainingJobTypeDef],
         "Experiment": NotRequired[ExperimentTypeDef],
         "Trial": NotRequired[TrialTypeDef],
         "TrialComponent": NotRequired[TrialComponentTypeDef],
@@ -14157,23 +15182,15 @@
         "FeatureMetadata": NotRequired[FeatureMetadataTypeDef],
         "Project": NotRequired[ProjectTypeDef],
         "HyperParameterTuningJob": NotRequired[HyperParameterTuningJobSearchEntityTypeDef],
         "ModelCard": NotRequired[ModelCardTypeDef],
         "Model": NotRequired[ModelDashboardModelTypeDef],
     },
 )
-SearchResponsePaginatorTypeDef = TypedDict(
-    "SearchResponsePaginatorTypeDef",
-    {
-        "Results": List[SearchRecordPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 SearchResponseTypeDef = TypedDict(
     "SearchResponseTypeDef",
     {
         "Results": List[SearchRecordTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/type_defs.pyi` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -293,35 +293,39 @@
     "AgentVersionTypeDef",
     "AlarmTypeDef",
     "MetricDefinitionTypeDef",
     "AlgorithmStatusItemTypeDef",
     "AlgorithmSummaryTypeDef",
     "AnnotationConsolidationConfigTypeDef",
     "ResourceSpecTypeDef",
-    "AppSpecificationPaginatorTypeDef",
+    "AppSpecificationExtraOutputTypeDef",
+    "AppSpecificationOutputTypeDef",
     "AppSpecificationTypeDef",
     "ArtifactSourceTypeTypeDef",
     "AssociateTrialComponentRequestRequestTypeDef",
     "AsyncInferenceClientConfigTypeDef",
+    "AsyncInferenceNotificationConfigOutputTypeDef",
     "AsyncInferenceNotificationConfigTypeDef",
     "AthenaDatasetDefinitionTypeDef",
+    "AutoMLAlgorithmConfigOutputTypeDef",
     "AutoMLAlgorithmConfigTypeDef",
     "AutoMLCandidateStepTypeDef",
     "AutoMLContainerDefinitionTypeDef",
     "FinalAutoMLJobObjectiveMetricTypeDef",
     "AutoMLS3DataSourceTypeDef",
     "AutoMLDataSplitConfigTypeDef",
     "AutoMLJobArtifactsTypeDef",
     "AutoMLJobCompletionCriteriaTypeDef",
     "AutoMLJobObjectiveTypeDef",
     "AutoMLJobStepMetadataTypeDef",
     "AutoMLPartialFailureReasonTypeDef",
     "AutoMLOutputDataConfigTypeDef",
     "TabularResolvedAttributesTypeDef",
     "TextGenerationResolvedAttributesTypeDef",
+    "VpcConfigOutputTypeDef",
     "VpcConfigTypeDef",
     "AutoParameterTypeDef",
     "AutotuneTypeDef",
     "BatchDataCaptureConfigTypeDef",
     "BatchDescribeModelPackageErrorTypeDef",
     "BatchDescribeModelPackageInputRequestTypeDef",
     "BestObjectiveNotImprovingTypeDef",
@@ -334,40 +338,48 @@
     "GenerativeAiSettingsTypeDef",
     "IdentityProviderOAuthSettingTypeDef",
     "KendraSettingsTypeDef",
     "ModelRegisterSettingsTypeDef",
     "TimeSeriesForecastingSettingsTypeDef",
     "WorkspaceSettingsTypeDef",
     "CapacitySizeTypeDef",
+    "CaptureContentTypeHeaderOutputTypeDef",
     "CaptureContentTypeHeaderTypeDef",
     "CaptureOptionTypeDef",
-    "CategoricalParameterRangePaginatorTypeDef",
+    "CategoricalParameterOutputTypeDef",
+    "CategoricalParameterRangeExtraOutputTypeDef",
+    "CategoricalParameterRangeOutputTypeDef",
+    "CategoricalParameterRangeSpecificationOutputTypeDef",
     "CategoricalParameterRangeSpecificationTypeDef",
     "CategoricalParameterRangeTypeDef",
     "CategoricalParameterTypeDef",
     "ShuffleConfigTypeDef",
+    "ChannelSpecificationOutputTypeDef",
     "ChannelSpecificationTypeDef",
     "CheckpointConfigTypeDef",
     "ClarifyCheckStepMetadataTypeDef",
+    "ClarifyInferenceConfigOutputTypeDef",
     "ClarifyInferenceConfigTypeDef",
     "ClarifyShapBaselineConfigTypeDef",
     "ClarifyTextConfigTypeDef",
     "ClusterLifeCycleConfigTypeDef",
     "ClusterInstanceStatusDetailsTypeDef",
     "ClusterSummaryTypeDef",
-    "ContainerConfigPaginatorTypeDef",
+    "ContainerConfigExtraOutputTypeDef",
     "FileSystemConfigTypeDef",
+    "ContainerConfigOutputTypeDef",
     "ContainerConfigTypeDef",
     "CustomImageTypeDef",
     "GitConfigTypeDef",
     "CodeRepositoryTypeDef",
     "CognitoConfigTypeDef",
     "CognitoMemberDefinitionTypeDef",
     "VectorConfigTypeDef",
-    "CollectionConfigurationPaginatorTypeDef",
+    "CollectionConfigurationExtraOutputTypeDef",
+    "CollectionConfigurationOutputTypeDef",
     "CollectionConfigurationTypeDef",
     "CompilationJobSummaryTypeDef",
     "ConditionStepMetadataTypeDef",
     "MultiModelConfigTypeDef",
     "ContextSourceTypeDef",
     "ContinuousParameterRangeSpecificationTypeDef",
     "ContinuousParameterRangeTypeDef",
@@ -402,21 +414,20 @@
     "PipelineDefinitionS3LocationTypeDef",
     "CreatePresignedDomainUrlRequestRequestTypeDef",
     "CreatePresignedNotebookInstanceUrlInputRequestTypeDef",
     "ExperimentConfigTypeDef",
     "ProcessingStoppingConditionTypeDef",
     "OwnershipSettingsTypeDef",
     "SpaceSharingSettingsTypeDef",
-    "DebugRuleConfigurationTypeDef",
     "InfraCheckConfigTypeDef",
     "OutputDataConfigTypeDef",
     "ProfilerConfigTypeDef",
-    "ProfilerRuleConfigurationTypeDef",
     "RemoteDebugConfigTypeDef",
     "RetryStrategyTypeDef",
+    "SessionChainingConfigTypeDef",
     "TensorBoardOutputConfigTypeDef",
     "DataProcessingTypeDef",
     "ModelClientConfigTypeDef",
     "TransformOutputTypeDef",
     "TransformResourcesTypeDef",
     "TimestampTypeDef",
     "TrialComponentArtifactTypeDef",
@@ -428,22 +439,26 @@
     "NotificationConfigurationTypeDef",
     "EFSFileSystemConfigTypeDef",
     "EFSFileSystemTypeDef",
     "CustomPosixUserConfigTypeDef",
     "CustomizedMetricSpecificationTypeDef",
     "DataCaptureConfigSummaryTypeDef",
     "DataCatalogConfigTypeDef",
+    "DataQualityAppSpecificationOutputTypeDef",
     "MonitoringConstraintsResourceTypeDef",
     "MonitoringStatisticsResourceTypeDef",
     "EndpointInputTypeDef",
     "FileSystemDataSourceTypeDef",
-    "S3DataSourcePaginatorTypeDef",
+    "S3DataSourceExtraOutputTypeDef",
+    "S3DataSourceOutputTypeDef",
     "S3DataSourceTypeDef",
     "RedshiftDatasetDefinitionTypeDef",
-    "DebugRuleConfigurationPaginatorTypeDef",
+    "DebugRuleConfigurationExtraOutputTypeDef",
+    "DebugRuleConfigurationOutputTypeDef",
+    "DebugRuleConfigurationTypeDef",
     "DebugRuleEvaluationStatusTypeDef",
     "DefaultEbsStorageSettingsTypeDef",
     "DeleteActionRequestRequestTypeDef",
     "DeleteAlgorithmInputRequestTypeDef",
     "DeleteAppImageConfigRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
@@ -488,17 +503,18 @@
     "DeleteTrialComponentRequestRequestTypeDef",
     "DeleteTrialRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
     "DeleteWorkforceRequestRequestTypeDef",
     "DeleteWorkteamRequestRequestTypeDef",
     "DeployedImageTypeDef",
     "RealTimeInferenceRecommendationTypeDef",
-    "DeviceSelectionConfigTypeDef",
+    "DeviceSelectionConfigOutputTypeDef",
     "EdgeDeploymentConfigTypeDef",
     "EdgeDeploymentStatusTypeDef",
+    "DeviceSelectionConfigTypeDef",
     "DeregisterDevicesRequestRequestTypeDef",
     "DerivedInformationTypeDef",
     "DescribeActionRequestRequestTypeDef",
     "DescribeAlgorithmInputRequestTypeDef",
     "DescribeAppImageConfigRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeArtifactRequestRequestTypeDef",
@@ -507,14 +523,15 @@
     "DescribeAutoMLJobV2RequestRequestTypeDef",
     "DescribeClusterNodeRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeCodeRepositoryInputRequestTypeDef",
     "DescribeCompilationJobRequestRequestTypeDef",
     "ModelArtifactsTypeDef",
     "ModelDigestsTypeDef",
+    "NeoVpcConfigOutputTypeDef",
     "DescribeContextRequestRequestTypeDef",
     "DescribeDataQualityJobDefinitionRequestRequestTypeDef",
     "DescribeDeviceFleetRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "EdgeModelTypeDef",
     "DescribeDomainRequestRequestTypeDef",
     "DescribeEdgeDeploymentPlanRequestRequestTypeDef",
@@ -544,28 +561,32 @@
     "TrainingJobStatusCountersTypeDef",
     "DescribeImageRequestRequestTypeDef",
     "DescribeImageVersionRequestRequestTypeDef",
     "DescribeInferenceComponentInputRequestTypeDef",
     "InferenceComponentRuntimeConfigSummaryTypeDef",
     "DescribeInferenceExperimentRequestRequestTypeDef",
     "EndpointMetadataTypeDef",
+    "InferenceExperimentScheduleOutputTypeDef",
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     "DescribeLabelingJobRequestRequestTypeDef",
     "LabelCountersTypeDef",
     "LabelingJobOutputTypeDef",
     "DescribeLineageGroupRequestRequestTypeDef",
     "DescribeModelBiasJobDefinitionRequestRequestTypeDef",
+    "ModelBiasAppSpecificationOutputTypeDef",
     "DescribeModelCardExportJobRequestRequestTypeDef",
     "ModelCardExportArtifactsTypeDef",
     "DescribeModelCardRequestRequestTypeDef",
     "DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef",
+    "ModelExplainabilityAppSpecificationOutputTypeDef",
     "DescribeModelInputRequestTypeDef",
     "DescribeModelPackageGroupInputRequestTypeDef",
     "DescribeModelPackageInputRequestTypeDef",
     "DescribeModelQualityJobDefinitionRequestRequestTypeDef",
+    "ModelQualityAppSpecificationOutputTypeDef",
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     "MonitoringExecutionSummaryTypeDef",
     "DescribeNotebookInstanceInputRequestTypeDef",
     "DescribeNotebookInstanceLifecycleConfigInputRequestTypeDef",
     "DescribePipelineDefinitionForExecutionRequestRequestTypeDef",
     "DescribePipelineExecutionRequestRequestTypeDef",
     "PipelineExperimentConfigTypeDef",
@@ -575,14 +596,16 @@
     "ServiceCatalogProvisionedProductDetailsTypeDef",
     "DescribeSpaceRequestRequestTypeDef",
     "DescribeStudioLifecycleConfigRequestRequestTypeDef",
     "DescribeSubscribedWorkteamRequestRequestTypeDef",
     "SubscribedWorkteamTypeDef",
     "DescribeTrainingJobRequestRequestTypeDef",
     "MetricDataTypeDef",
+    "ProfilerConfigOutputTypeDef",
+    "ProfilerRuleConfigurationOutputTypeDef",
     "ProfilerRuleEvaluationStatusTypeDef",
     "SecondaryStatusTransitionTypeDef",
     "WarmPoolStatusTypeDef",
     "DescribeTransformJobRequestRequestTypeDef",
     "DescribeTrialComponentRequestRequestTypeDef",
     "TrialComponentMetricSummaryTypeDef",
     "TrialComponentSourceTypeDef",
@@ -594,14 +617,15 @@
     "ProductionVariantServerlessUpdateConfigTypeDef",
     "DeviceDeploymentSummaryTypeDef",
     "DeviceFleetSummaryTypeDef",
     "DeviceStatsTypeDef",
     "EdgeModelSummaryTypeDef",
     "DeviceTypeDef",
     "DisassociateTrialComponentRequestRequestTypeDef",
+    "DockerSettingsOutputTypeDef",
     "DockerSettingsTypeDef",
     "DomainDetailsTypeDef",
     "FileSourceTypeDef",
     "EMRStepMetadataTypeDef",
     "EbsStorageSettingsTypeDef",
     "EdgeDeploymentPlanSummaryTypeDef",
     "EdgeModelStatTypeDef",
@@ -627,36 +651,37 @@
     "HolidayConfigAttributesTypeDef",
     "HubContentInfoTypeDef",
     "HubInfoTypeDef",
     "HumanLoopActivationConditionsConfigTypeDef",
     "UiConfigTypeDef",
     "HumanTaskUiSummaryTypeDef",
     "HyperParameterTuningJobObjectiveTypeDef",
-    "VpcConfigPaginatorTypeDef",
+    "VpcConfigExtraOutputTypeDef",
     "HyperParameterTuningInstanceConfigTypeDef",
     "ResourceLimitsTypeDef",
     "HyperbandStrategyConfigTypeDef",
     "ParentHyperParameterTuningJobTypeDef",
     "IamIdentityTypeDef",
     "RepositoryAuthConfigTypeDef",
     "ImageTypeDef",
     "ImageVersionTypeDef",
     "InferenceComponentComputeResourceRequirementsTypeDef",
     "InferenceComponentContainerSpecificationTypeDef",
     "InferenceComponentStartupParametersTypeDef",
     "InferenceComponentSummaryTypeDef",
-    "InferenceExperimentSchedulePaginatorTypeDef",
+    "InferenceExperimentScheduleExtraOutputTypeDef",
     "RecommendationMetricsTypeDef",
     "InferenceRecommendationsJobTypeDef",
     "InstanceGroupTypeDef",
     "IntegerParameterRangeSpecificationTypeDef",
     "IntegerParameterRangeTypeDef",
     "KernelSpecTypeDef",
     "LabelCountersForWorkteamTypeDef",
-    "LabelingJobDataAttributesPaginatorTypeDef",
+    "LabelingJobDataAttributesExtraOutputTypeDef",
+    "LabelingJobDataAttributesOutputTypeDef",
     "LabelingJobDataAttributesTypeDef",
     "LabelingJobS3DataSourceTypeDef",
     "LabelingJobSnsDataSourceTypeDef",
     "LineageGroupSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
@@ -691,28 +716,30 @@
     "ListTagsInputRequestTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef",
     "TransformJobSummaryTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileDetailsTypeDef",
     "ListWorkforcesRequestRequestTypeDef",
     "ListWorkteamsRequestRequestTypeDef",
-    "OidcMemberDefinitionPaginatorTypeDef",
+    "OidcMemberDefinitionExtraOutputTypeDef",
+    "OidcMemberDefinitionOutputTypeDef",
     "OidcMemberDefinitionTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ModelAccessConfigTypeDef",
     "MonitoringGroundTruthS3InputTypeDef",
     "ModelDashboardEndpointTypeDef",
     "ModelDashboardIndicatorActionTypeDef",
     "RealTimeInferenceConfigTypeDef",
     "ModelInputTypeDef",
     "ModelLatencyThresholdTypeDef",
     "ModelMetadataFilterTypeDef",
     "ModelPackageStatusItemTypeDef",
     "ModelStepMetadataTypeDef",
-    "MonitoringAppSpecificationPaginatorTypeDef",
+    "MonitoringAppSpecificationExtraOutputTypeDef",
+    "MonitoringAppSpecificationOutputTypeDef",
     "MonitoringAppSpecificationTypeDef",
     "MonitoringClusterConfigTypeDef",
     "MonitoringCsvDatasetFormatTypeDef",
     "MonitoringJsonDatasetFormatTypeDef",
     "MonitoringS3OutputTypeDef",
     "ScheduleConfigTypeDef",
     "S3StorageConfigTypeDef",
@@ -734,36 +761,40 @@
     "TuningJobStepMetaDataTypeDef",
     "SelectiveExecutionResultTypeDef",
     "ProcessingClusterConfigTypeDef",
     "ProcessingFeatureStoreOutputTypeDef",
     "ProcessingS3InputTypeDef",
     "ProcessingS3OutputTypeDef",
     "ProductionVariantCoreDumpConfigTypeDef",
+    "ProfilerConfigExtraOutputTypeDef",
     "ProfilerConfigForUpdateTypeDef",
-    "ProfilerConfigPaginatorTypeDef",
+    "ProfilerRuleConfigurationTypeDef",
     "PropertyNameQueryTypeDef",
     "ProvisioningParameterTypeDef",
     "USDTypeDef",
     "PutModelPackageGroupPolicyInputRequestTypeDef",
     "VertexTypeDef",
     "RStudioServerProAppSettingsTypeDef",
     "RecommendationJobCompiledOutputConfigTypeDef",
+    "RecommendationJobPayloadConfigOutputTypeDef",
     "RecommendationJobPayloadConfigTypeDef",
     "RecommendationJobResourceLimitTypeDef",
+    "RecommendationJobVpcConfigOutputTypeDef",
     "RecommendationJobVpcConfigTypeDef",
     "RemoteDebugConfigForUpdateTypeDef",
     "RenderableTaskTypeDef",
     "RenderingErrorTypeDef",
     "ResourceConfigForUpdateTypeDef",
     "VisibilityConditionsTypeDef",
     "SelectedStepTypeDef",
     "SendPipelineExecutionStepFailureRequestRequestTypeDef",
     "ShadowModelVariantConfigTypeDef",
     "SharingSettingsTypeDef",
-    "SourceIpConfigPaginatorTypeDef",
+    "SourceIpConfigExtraOutputTypeDef",
+    "SourceIpConfigOutputTypeDef",
     "SpaceSharingSettingsSummaryTypeDef",
     "StairsTypeDef",
     "StartEdgeDeploymentStageRequestRequestTypeDef",
     "StartInferenceExperimentRequestRequestTypeDef",
     "StartMonitoringScheduleRequestRequestTypeDef",
     "StartNotebookInstanceInputRequestTypeDef",
     "StopAutoMLJobRequestRequestTypeDef",
@@ -776,15 +807,17 @@
     "StopMonitoringScheduleRequestRequestTypeDef",
     "StopNotebookInstanceInputRequestTypeDef",
     "StopPipelineExecutionRequestRequestTypeDef",
     "StopProcessingJobRequestRequestTypeDef",
     "StopTrainingJobRequestRequestTypeDef",
     "StopTransformJobRequestRequestTypeDef",
     "ThroughputConfigUpdateTypeDef",
+    "TimeSeriesConfigOutputTypeDef",
     "TimeSeriesConfigTypeDef",
+    "TimeSeriesTransformationsOutputTypeDef",
     "TimeSeriesTransformationsTypeDef",
     "TrainingRepositoryAuthConfigTypeDef",
     "TransformS3DataSourceTypeDef",
     "UpdateActionRequestRequestTypeDef",
     "UpdateArtifactRequestRequestTypeDef",
     "UpdateClusterSoftwareRequestRequestTypeDef",
     "UpdateContextRequestRequestTypeDef",
@@ -917,78 +950,102 @@
     "AddTagsOutputTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
     "CreateModelPackageGroupInputRequestTypeDef",
     "CreateStudioLifecycleConfigRequestRequestTypeDef",
     "ImportHubContentRequestRequestTypeDef",
     "ListTagsOutputTypeDef",
+    "AutoRollbackConfigOutputTypeDef",
     "AutoRollbackConfigTypeDef",
-    "HyperParameterAlgorithmSpecificationPaginatorTypeDef",
+    "HyperParameterAlgorithmSpecificationExtraOutputTypeDef",
+    "HyperParameterAlgorithmSpecificationOutputTypeDef",
     "HyperParameterAlgorithmSpecificationTypeDef",
     "AlgorithmStatusDetailsTypeDef",
     "ListAlgorithmsOutputTypeDef",
     "AppDetailsTypeDef",
     "CreateAppRequestRequestTypeDef",
     "DescribeAppResponseTypeDef",
     "RStudioServerProDomainSettingsForUpdateTypeDef",
     "RStudioServerProDomainSettingsTypeDef",
     "SpaceCodeEditorAppSettingsTypeDef",
     "TensorBoardAppSettingsTypeDef",
-    "ArtifactSourcePaginatorTypeDef",
+    "AppSpecificationUnionTypeDef",
+    "ArtifactSourceExtraOutputTypeDef",
+    "ArtifactSourceOutputTypeDef",
     "ArtifactSourceTypeDef",
+    "AsyncInferenceOutputConfigOutputTypeDef",
     "AsyncInferenceOutputConfigTypeDef",
+    "AutoMLCandidateGenerationConfigOutputTypeDef",
+    "CandidateGenerationConfigOutputTypeDef",
     "AutoMLCandidateGenerationConfigTypeDef",
     "CandidateGenerationConfigTypeDef",
     "AutoMLDataSourceTypeDef",
     "ImageClassificationJobConfigTypeDef",
     "TextClassificationJobConfigTypeDef",
     "ResolvedAttributesTypeDef",
     "AutoMLJobSummaryTypeDef",
     "AutoMLProblemTypeResolvedAttributesTypeDef",
+    "AutoMLSecurityConfigOutputTypeDef",
+    "LabelingJobResourceConfigOutputTypeDef",
+    "MonitoringNetworkConfigOutputTypeDef",
+    "NetworkConfigOutputTypeDef",
     "AutoMLSecurityConfigTypeDef",
     "LabelingJobResourceConfigTypeDef",
     "MonitoringNetworkConfigTypeDef",
     "NetworkConfigTypeDef",
     "BiasTypeDef",
     "DriftCheckModelDataQualityTypeDef",
     "DriftCheckModelQualityTypeDef",
     "ExplainabilityTypeDef",
     "ModelDataQualityTypeDef",
     "ModelQualityTypeDef",
     "CallbackStepMetadataTypeDef",
     "LambdaStepMetadataTypeDef",
     "SendPipelineExecutionStepSuccessRequestRequestTypeDef",
     "CandidatePropertiesTypeDef",
+    "CanvasAppSettingsOutputTypeDef",
     "CanvasAppSettingsTypeDef",
     "RollingUpdatePolicyTypeDef",
     "TrafficRoutingConfigTypeDef",
+    "InferenceExperimentDataStorageConfigOutputTypeDef",
     "InferenceExperimentDataStorageConfigTypeDef",
+    "DataCaptureConfigOutputTypeDef",
     "DataCaptureConfigTypeDef",
+    "EnvironmentParameterRangesOutputTypeDef",
     "EnvironmentParameterRangesTypeDef",
     "ClarifyShapConfigTypeDef",
     "ClusterInstanceGroupDetailsTypeDef",
     "ClusterInstanceGroupSpecificationTypeDef",
     "ClusterNodeDetailsTypeDef",
     "ClusterNodeSummaryTypeDef",
     "ListClustersResponseTypeDef",
-    "CodeEditorAppImageConfigPaginatorTypeDef",
-    "JupyterLabAppImageConfigPaginatorTypeDef",
+    "CodeEditorAppImageConfigExtraOutputTypeDef",
+    "JupyterLabAppImageConfigExtraOutputTypeDef",
+    "CodeEditorAppImageConfigOutputTypeDef",
+    "JupyterLabAppImageConfigOutputTypeDef",
     "CodeEditorAppImageConfigTypeDef",
     "JupyterLabAppImageConfigTypeDef",
+    "CodeEditorAppSettingsOutputTypeDef",
     "CodeEditorAppSettingsTypeDef",
+    "KernelGatewayAppSettingsOutputTypeDef",
     "KernelGatewayAppSettingsTypeDef",
+    "RSessionAppSettingsOutputTypeDef",
     "RSessionAppSettingsTypeDef",
     "CodeRepositorySummaryTypeDef",
     "CreateCodeRepositoryInputRequestTypeDef",
     "DescribeCodeRepositoryOutputTypeDef",
+    "JupyterLabAppSettingsOutputTypeDef",
     "JupyterLabAppSettingsTypeDef",
+    "JupyterServerAppSettingsOutputTypeDef",
     "JupyterServerAppSettingsTypeDef",
+    "SpaceJupyterLabAppSettingsOutputTypeDef",
     "SpaceJupyterLabAppSettingsTypeDef",
     "CollectionConfigTypeDef",
-    "DebugHookConfigPaginatorTypeDef",
+    "DebugHookConfigExtraOutputTypeDef",
+    "DebugHookConfigOutputTypeDef",
     "DebugHookConfigTypeDef",
     "ListCompilationJobsResponseTypeDef",
     "ContextSummaryTypeDef",
     "CreateContextRequestRequestTypeDef",
     "TuningJobCompletionCriteriaTypeDef",
     "CreateActionRequestRequestTypeDef",
     "CreateTrialRequestRequestTypeDef",
@@ -1074,28 +1131,32 @@
     "QueryFiltersTypeDef",
     "CreateTrialComponentRequestRequestTypeDef",
     "UpdateTrialComponentRequestRequestTypeDef",
     "CreateWorkforceRequestRequestTypeDef",
     "UpdateWorkforceRequestRequestTypeDef",
     "CustomFileSystemConfigTypeDef",
     "CustomFileSystemTypeDef",
+    "DataQualityAppSpecificationUnionTypeDef",
     "ModelBiasBaselineConfigTypeDef",
     "ModelExplainabilityBaselineConfigTypeDef",
     "ModelQualityBaselineConfigTypeDef",
     "DataQualityBaselineConfigTypeDef",
     "MonitoringBaselineConfigTypeDef",
-    "DataSourcePaginatorTypeDef",
+    "DataSourceExtraOutputTypeDef",
+    "DataSourceOutputTypeDef",
     "DataSourceTypeDef",
     "DatasetDefinitionTypeDef",
+    "DebugRuleConfigurationUnionTypeDef",
     "DefaultSpaceStorageSettingsTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "InferenceComponentContainerSpecificationSummaryTypeDef",
     "DeploymentRecommendationTypeDef",
-    "DeploymentStageTypeDef",
     "DeploymentStageStatusSummaryTypeDef",
+    "DeploymentStageTypeDef",
+    "NeoVpcConfigUnionTypeDef",
     "DescribeDeviceResponseTypeDef",
     "DescribeEdgePackagingJobResponseTypeDef",
     "DescribeEndpointInputEndpointDeletedWaitTypeDef",
     "DescribeEndpointInputEndpointInServiceWaitTypeDef",
     "DescribeImageRequestImageCreatedWaitTypeDef",
     "DescribeImageRequestImageDeletedWaitTypeDef",
     "DescribeImageRequestImageUpdatedWaitTypeDef",
@@ -1110,15 +1171,19 @@
     "ExperimentSummaryTypeDef",
     "FeatureGroupSummaryTypeDef",
     "DescribeFeatureMetadataResponseTypeDef",
     "FeatureMetadataTypeDef",
     "UpdateFeatureMetadataRequestRequestTypeDef",
     "DescribeHubContentResponseTypeDef",
     "DescribeHumanTaskUiResponseTypeDef",
+    "InferenceExperimentSummaryTypeDef",
+    "ModelBiasAppSpecificationUnionTypeDef",
     "DescribeModelCardExportJobResponseTypeDef",
+    "ModelExplainabilityAppSpecificationUnionTypeDef",
+    "ModelQualityAppSpecificationUnionTypeDef",
     "ListMonitoringExecutionsResponseTypeDef",
     "DescribeSubscribedWorkteamResponseTypeDef",
     "ListSubscribedWorkteamsResponseTypeDef",
     "TrainingJobSummaryTypeDef",
     "TrialSummaryTypeDef",
     "DesiredWeightAndCapacityTypeDef",
     "ListStageDevicesResponseTypeDef",
@@ -1145,35 +1210,41 @@
     "GetSearchSuggestionsResponseTypeDef",
     "UpdateCodeRepositoryInputRequestTypeDef",
     "ListHubContentVersionsResponseTypeDef",
     "ListHubContentsResponseTypeDef",
     "ListHubsResponseTypeDef",
     "HumanLoopActivationConfigTypeDef",
     "ListHumanTaskUisResponseTypeDef",
-    "NetworkConfigPaginatorTypeDef",
-    "HyperParameterTuningResourceConfigPaginatorTypeDef",
+    "NetworkConfigExtraOutputTypeDef",
+    "VpcConfigUnionTypeDef",
+    "HyperParameterTuningResourceConfigExtraOutputTypeDef",
+    "HyperParameterTuningResourceConfigOutputTypeDef",
     "HyperParameterTuningResourceConfigTypeDef",
     "HyperParameterTuningJobSummaryTypeDef",
     "HyperParameterTuningJobStrategyConfigTypeDef",
-    "HyperParameterTuningJobWarmStartConfigPaginatorTypeDef",
+    "HyperParameterTuningJobWarmStartConfigExtraOutputTypeDef",
+    "HyperParameterTuningJobWarmStartConfigOutputTypeDef",
     "HyperParameterTuningJobWarmStartConfigTypeDef",
     "UserContextTypeDef",
     "ImageConfigTypeDef",
     "ListImagesResponseTypeDef",
     "ListImageVersionsResponseTypeDef",
     "InferenceComponentSpecificationTypeDef",
     "ListInferenceComponentsOutputTypeDef",
-    "InferenceExperimentSummaryPaginatorTypeDef",
     "ListInferenceRecommendationsJobsResponseTypeDef",
-    "ResourceConfigPaginatorTypeDef",
+    "ResourceConfigExtraOutputTypeDef",
+    "ResourceConfigOutputTypeDef",
     "ResourceConfigTypeDef",
+    "ParameterRangeOutputTypeDef",
     "ParameterRangeTypeDef",
-    "ParameterRangesPaginatorTypeDef",
+    "ParameterRangesExtraOutputTypeDef",
+    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
-    "KernelGatewayImageConfigPaginatorTypeDef",
+    "KernelGatewayImageConfigExtraOutputTypeDef",
+    "KernelGatewayImageConfigOutputTypeDef",
     "KernelGatewayImageConfigTypeDef",
     "LabelingJobForWorkteamSummaryTypeDef",
     "LabelingJobDataSourceTypeDef",
     "ListLineageGroupsResponseTypeDef",
     "ListActionsRequestListActionsPaginateTypeDef",
     "ListAlgorithmsInputListAlgorithmsPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
@@ -1264,112 +1335,145 @@
     "ListPipelinesResponseTypeDef",
     "ListProcessingJobsResponseTypeDef",
     "ListProjectsOutputTypeDef",
     "ListResourceCatalogsResponseTypeDef",
     "ListStudioLifecycleConfigsResponseTypeDef",
     "ListTransformJobsResponseTypeDef",
     "ListUserProfilesResponseTypeDef",
-    "MemberDefinitionPaginatorTypeDef",
+    "MemberDefinitionExtraOutputTypeDef",
+    "MemberDefinitionOutputTypeDef",
     "MemberDefinitionTypeDef",
     "MetricSpecificationTypeDef",
     "S3ModelDataSourceTypeDef",
+    "TextGenerationJobConfigOutputTypeDef",
     "TextGenerationJobConfigTypeDef",
     "MonitoringAlertActionsTypeDef",
     "ModelInfrastructureConfigTypeDef",
+    "RecommendationJobStoppingConditionsOutputTypeDef",
     "RecommendationJobStoppingConditionsTypeDef",
     "ModelMetadataSearchExpressionTypeDef",
     "ModelPackageStatusDetailsTypeDef",
     "MonitoringResourcesTypeDef",
-    "MonitoringDatasetFormatPaginatorTypeDef",
+    "MonitoringDatasetFormatExtraOutputTypeDef",
+    "MonitoringDatasetFormatOutputTypeDef",
     "MonitoringDatasetFormatTypeDef",
     "MonitoringOutputTypeDef",
     "OfflineStoreConfigTypeDef",
     "OnlineStoreConfigTypeDef",
     "OnlineStoreConfigUpdateTypeDef",
     "OutputConfigTypeDef",
     "PendingProductionVariantSummaryTypeDef",
     "ProductionVariantSummaryTypeDef",
     "ProcessingResourcesTypeDef",
     "ProcessingOutputTypeDef",
     "ProductionVariantTypeDef",
+    "ProfilerConfigUnionTypeDef",
+    "ProfilerRuleConfigurationUnionTypeDef",
     "SuggestionQueryTypeDef",
-    "ServiceCatalogProvisioningDetailsPaginatorTypeDef",
+    "ServiceCatalogProvisioningDetailsExtraOutputTypeDef",
+    "ServiceCatalogProvisioningDetailsOutputTypeDef",
     "ServiceCatalogProvisioningDetailsTypeDef",
     "ServiceCatalogProvisioningUpdateDetailsTypeDef",
     "PublicWorkforceTaskPriceTypeDef",
     "QueryLineageResponseTypeDef",
     "RecommendationJobOutputConfigTypeDef",
+    "RecommendationJobContainerConfigOutputTypeDef",
     "RecommendationJobContainerConfigTypeDef",
     "RenderUiTemplateRequestRequestTypeDef",
     "RenderUiTemplateResponseTypeDef",
-    "UpdateTrainingJobRequestRequestTypeDef",
     "SearchRequestRequestTypeDef",
+    "SelectiveExecutionConfigExtraOutputTypeDef",
+    "SelectiveExecutionConfigOutputTypeDef",
     "SelectiveExecutionConfigTypeDef",
+    "ShadowModeConfigOutputTypeDef",
     "ShadowModeConfigTypeDef",
+    "SourceIpConfigUnionTypeDef",
+    "TrafficPatternOutputTypeDef",
     "TrafficPatternTypeDef",
+    "TimeSeriesForecastingJobConfigOutputTypeDef",
     "TimeSeriesForecastingJobConfigTypeDef",
     "TrainingImageConfigTypeDef",
     "TransformDataSourceTypeDef",
-    "WorkforcePaginatorTypeDef",
     "WorkforceTypeDef",
     "ListActionsResponseTypeDef",
     "ListAppsResponseTypeDef",
     "DomainSettingsForUpdateTypeDef",
+    "DomainSettingsOutputTypeDef",
     "DomainSettingsTypeDef",
-    "ArtifactSummaryPaginatorTypeDef",
     "ArtifactSummaryTypeDef",
+    "ArtifactSourceUnionTypeDef",
     "CreateArtifactRequestRequestTypeDef",
     "DeleteArtifactRequestRequestTypeDef",
+    "AsyncInferenceConfigOutputTypeDef",
     "AsyncInferenceConfigTypeDef",
+    "TabularJobConfigOutputTypeDef",
     "TabularJobConfigTypeDef",
     "AutoMLChannelTypeDef",
     "AutoMLJobChannelTypeDef",
     "ListAutoMLJobsResponseTypeDef",
     "AutoMLResolvedAttributesTypeDef",
+    "AutoMLJobConfigOutputTypeDef",
+    "LabelingJobAlgorithmsConfigOutputTypeDef",
     "AutoMLJobConfigTypeDef",
+    "AutoMLSecurityConfigUnionTypeDef",
     "LabelingJobAlgorithmsConfigTypeDef",
+    "MonitoringNetworkConfigUnionTypeDef",
     "ModelMetricsTypeDef",
     "PipelineExecutionStepMetadataTypeDef",
     "AutoMLCandidateTypeDef",
     "BlueGreenUpdatePolicyTypeDef",
+    "InferenceExperimentDataStorageConfigUnionTypeDef",
+    "DataCaptureConfigUnionTypeDef",
+    "EndpointInputConfigurationOutputTypeDef",
     "EndpointInputConfigurationTypeDef",
+    "ClarifyExplainerConfigOutputTypeDef",
     "ClarifyExplainerConfigTypeDef",
     "DescribeClusterResponseTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "DescribeClusterNodeResponseTypeDef",
     "ListClusterNodesResponseTypeDef",
+    "CodeEditorAppImageConfigUnionTypeDef",
+    "JupyterLabAppImageConfigUnionTypeDef",
     "ListCodeRepositoriesOutputTypeDef",
     "FeatureDefinitionTypeDef",
+    "DebugHookConfigUnionTypeDef",
     "ListContextsResponseTypeDef",
-    "InferenceExperimentSummaryTypeDef",
+    "InferenceExperimentScheduleUnionTypeDef",
     "QueryLineageRequestRequestTypeDef",
-    "ChannelPaginatorTypeDef",
+    "ChannelExtraOutputTypeDef",
+    "ChannelOutputTypeDef",
     "ChannelTypeDef",
     "ProcessingInputTypeDef",
+    "DefaultSpaceSettingsOutputTypeDef",
     "DefaultSpaceSettingsTypeDef",
+    "UserSettingsOutputTypeDef",
     "UserSettingsTypeDef",
     "InferenceComponentSpecificationSummaryTypeDef",
+    "DescribeEdgeDeploymentPlanResponseTypeDef",
     "CreateEdgeDeploymentPlanRequestRequestTypeDef",
     "CreateEdgeDeploymentStageRequestRequestTypeDef",
-    "DescribeEdgeDeploymentPlanResponseTypeDef",
     "ListExperimentsResponseTypeDef",
     "ListFeatureGroupsResponseTypeDef",
+    "ListInferenceExperimentsResponseTypeDef",
     "ListTrainingJobsResponseTypeDef",
     "ListTrialsResponseTypeDef",
     "UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef",
     "ListDevicesResponseTypeDef",
     "DriftCheckBaselinesTypeDef",
+    "SpaceSettingsOutputTypeDef",
     "SpaceSettingsSummaryTypeDef",
     "SpaceSettingsTypeDef",
     "InferenceRecommendationTypeDef",
     "RecommendationJobInferenceBenchmarkTypeDef",
     "SearchExpressionTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobResponseTypeDef",
+    "NetworkConfigUnionTypeDef",
     "ListHyperParameterTuningJobsResponseTypeDef",
+    "HyperParameterTuningJobWarmStartConfigUnionTypeDef",
     "AssociationSummaryTypeDef",
     "DescribeActionResponseTypeDef",
     "DescribeArtifactResponseTypeDef",
     "DescribeContextResponseTypeDef",
     "DescribeExperimentResponseTypeDef",
     "DescribeLineageGroupResponseTypeDef",
     "DescribeModelCardResponseTypeDef",
@@ -1382,214 +1486,265 @@
     "ModelDashboardModelCardTypeDef",
     "ModelPackageGroupTypeDef",
     "PipelineTypeDef",
     "TrialComponentSimpleSummaryTypeDef",
     "TrialComponentSummaryTypeDef",
     "CreateInferenceComponentInputRequestTypeDef",
     "UpdateInferenceComponentInputRequestTypeDef",
-    "ListInferenceExperimentsResponsePaginatorTypeDef",
+    "ResourceConfigUnionTypeDef",
+    "HyperParameterSpecificationOutputTypeDef",
     "HyperParameterSpecificationTypeDef",
-    "HyperParameterTuningJobConfigPaginatorTypeDef",
+    "HyperParameterTuningJobConfigExtraOutputTypeDef",
+    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
-    "AppImageConfigDetailsPaginatorTypeDef",
     "AppImageConfigDetailsTypeDef",
-    "CreateAppImageConfigRequestRequestTypeDef",
     "DescribeAppImageConfigResponseTypeDef",
+    "CreateAppImageConfigRequestRequestTypeDef",
+    "KernelGatewayImageConfigUnionTypeDef",
     "UpdateAppImageConfigRequestRequestTypeDef",
     "ListLabelingJobsForWorkteamResponseTypeDef",
-    "LabelingJobInputConfigPaginatorTypeDef",
+    "LabelingJobInputConfigExtraOutputTypeDef",
+    "LabelingJobInputConfigOutputTypeDef",
     "LabelingJobInputConfigTypeDef",
-    "WorkteamPaginatorTypeDef",
-    "CreateWorkteamRequestRequestTypeDef",
-    "UpdateWorkteamRequestRequestTypeDef",
     "WorkteamTypeDef",
+    "MemberDefinitionUnionTypeDef",
     "TargetTrackingScalingPolicyConfigurationTypeDef",
     "ModelDataSourceTypeDef",
     "MonitoringAlertSummaryTypeDef",
     "ModelVariantConfigSummaryTypeDef",
     "ModelVariantConfigTypeDef",
+    "RecommendationJobStoppingConditionsUnionTypeDef",
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     "ListModelMetadataRequestRequestTypeDef",
-    "BatchTransformInputPaginatorTypeDef",
+    "BatchTransformInputExtraOutputTypeDef",
+    "BatchTransformInputOutputTypeDef",
     "BatchTransformInputTypeDef",
-    "MonitoringOutputConfigPaginatorTypeDef",
+    "MonitoringOutputConfigExtraOutputTypeDef",
+    "MonitoringOutputConfigOutputTypeDef",
     "MonitoringOutputConfigTypeDef",
     "CreateCompilationJobRequestRequestTypeDef",
     "DescribeCompilationJobResponseTypeDef",
     "PendingDeploymentSummaryTypeDef",
-    "ProcessingOutputConfigPaginatorTypeDef",
+    "ProcessingOutputConfigExtraOutputTypeDef",
+    "ProcessingOutputConfigOutputTypeDef",
     "ProcessingOutputConfigTypeDef",
+    "UpdateTrainingJobRequestRequestTypeDef",
     "GetSearchSuggestionsRequestRequestTypeDef",
-    "ProjectPaginatorTypeDef",
-    "CreateProjectInputRequestTypeDef",
     "DescribeProjectOutputTypeDef",
     "ProjectTypeDef",
+    "CreateProjectInputRequestTypeDef",
+    "ServiceCatalogProvisioningDetailsUnionTypeDef",
     "UpdateProjectInputRequestTypeDef",
+    "HumanLoopConfigOutputTypeDef",
     "HumanLoopConfigTypeDef",
+    "HumanTaskConfigOutputTypeDef",
     "HumanTaskConfigTypeDef",
     "DescribePipelineExecutionResponseTypeDef",
     "PipelineExecutionTypeDef",
+    "SelectiveExecutionConfigUnionTypeDef",
     "StartPipelineExecutionRequestRequestTypeDef",
-    "AlgorithmSpecificationPaginatorTypeDef",
+    "ShadowModeConfigUnionTypeDef",
+    "AlgorithmSpecificationExtraOutputTypeDef",
+    "AlgorithmSpecificationOutputTypeDef",
     "AlgorithmSpecificationTypeDef",
     "TransformInputTypeDef",
-    "ListWorkforcesResponsePaginatorTypeDef",
     "DescribeWorkforceResponseTypeDef",
     "ListWorkforcesResponseTypeDef",
     "UpdateWorkforceResponseTypeDef",
-    "ListArtifactsResponsePaginatorTypeDef",
+    "DomainSettingsUnionTypeDef",
     "ListArtifactsResponseTypeDef",
+    "AsyncInferenceConfigUnionTypeDef",
+    "AutoMLProblemTypeConfigOutputTypeDef",
     "AutoMLProblemTypeConfigTypeDef",
+    "AutoMLJobConfigUnionTypeDef",
     "CreateAutoMLJobRequestRequestTypeDef",
+    "LabelingJobAlgorithmsConfigUnionTypeDef",
     "PipelineExecutionStepTypeDef",
     "DescribeAutoMLJobResponseTypeDef",
     "ListCandidatesForAutoMLJobResponseTypeDef",
+    "DeploymentConfigOutputTypeDef",
     "DeploymentConfigTypeDef",
+    "RecommendationJobInputConfigOutputTypeDef",
     "RecommendationJobInputConfigTypeDef",
+    "ExplainerConfigOutputTypeDef",
     "ExplainerConfigTypeDef",
     "CreateFeatureGroupRequestRequestTypeDef",
     "DescribeFeatureGroupResponseTypeDef",
     "FeatureGroupTypeDef",
     "UpdateFeatureGroupRequestRequestTypeDef",
-    "ListInferenceExperimentsResponseTypeDef",
-    "HyperParameterTrainingJobDefinitionPaginatorTypeDef",
+    "HyperParameterTrainingJobDefinitionExtraOutputTypeDef",
+    "HyperParameterTrainingJobDefinitionOutputTypeDef",
+    "TrainingJobDefinitionOutputTypeDef",
+    "ChannelUnionTypeDef",
     "HyperParameterTrainingJobDefinitionTypeDef",
     "TrainingJobDefinitionTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "CreateUserProfileRequestRequestTypeDef",
+    "DefaultSpaceSettingsUnionTypeDef",
     "DescribeDomainResponseTypeDef",
     "DescribeUserProfileResponseTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "CreateUserProfileRequestRequestTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
+    "UserSettingsUnionTypeDef",
     "DescribeInferenceComponentOutputTypeDef",
+    "DescribeSpaceResponseTypeDef",
     "SpaceDetailsTypeDef",
     "CreateSpaceRequestRequestTypeDef",
-    "DescribeSpaceResponseTypeDef",
+    "SpaceSettingsUnionTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
     "InferenceRecommendationsJobStepTypeDef",
     "SearchRequestSearchPaginateTypeDef",
     "ListAssociationsResponseTypeDef",
     "TrialTypeDef",
     "ListTrialComponentsResponseTypeDef",
+    "TrainingSpecificationOutputTypeDef",
     "TrainingSpecificationTypeDef",
-    "ListAppImageConfigsResponsePaginatorTypeDef",
+    "HyperParameterTuningJobConfigUnionTypeDef",
     "ListAppImageConfigsResponseTypeDef",
-    "LabelingJobSummaryPaginatorTypeDef",
     "LabelingJobSummaryTypeDef",
-    "ListWorkteamsResponsePaginatorTypeDef",
+    "LabelingJobInputConfigUnionTypeDef",
     "DescribeWorkteamResponseTypeDef",
     "ListWorkteamsResponseTypeDef",
     "UpdateWorkteamResponseTypeDef",
+    "CreateWorkteamRequestRequestTypeDef",
+    "UpdateWorkteamRequestRequestTypeDef",
     "ScalingPolicyTypeDef",
-    "ContainerDefinitionPaginatorTypeDef",
+    "ContainerDefinitionExtraOutputTypeDef",
+    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
+    "ModelPackageContainerDefinitionExtraOutputTypeDef",
+    "ModelPackageContainerDefinitionOutputTypeDef",
     "ModelPackageContainerDefinitionTypeDef",
     "SourceAlgorithmTypeDef",
     "ListMonitoringAlertsResponseTypeDef",
     "DescribeInferenceExperimentResponseTypeDef",
     "CreateInferenceExperimentRequestRequestTypeDef",
     "StopInferenceExperimentRequestRequestTypeDef",
     "UpdateInferenceExperimentRequestRequestTypeDef",
-    "MonitoringInputPaginatorTypeDef",
+    "MonitoringInputExtraOutputTypeDef",
+    "DataQualityJobInputOutputTypeDef",
+    "ModelBiasJobInputOutputTypeDef",
+    "ModelExplainabilityJobInputOutputTypeDef",
+    "ModelQualityJobInputOutputTypeDef",
+    "MonitoringInputOutputTypeDef",
     "DataQualityJobInputTypeDef",
     "ModelBiasJobInputTypeDef",
     "ModelExplainabilityJobInputTypeDef",
     "ModelQualityJobInputTypeDef",
     "MonitoringInputTypeDef",
-    "ProcessingJobPaginatorTypeDef",
-    "CreateProcessingJobRequestRequestTypeDef",
+    "MonitoringOutputConfigUnionTypeDef",
     "DescribeProcessingJobResponseTypeDef",
     "ProcessingJobTypeDef",
-    "CreateFlowDefinitionRequestRequestTypeDef",
+    "CreateProcessingJobRequestRequestTypeDef",
+    "ProcessingOutputConfigUnionTypeDef",
     "DescribeFlowDefinitionResponseTypeDef",
-    "CreateLabelingJobRequestRequestTypeDef",
+    "CreateFlowDefinitionRequestRequestTypeDef",
+    "HumanLoopConfigUnionTypeDef",
     "DescribeLabelingJobResponseTypeDef",
-    "TrainingJobPaginatorTypeDef",
-    "CreateTrainingJobRequestRequestTypeDef",
+    "CreateLabelingJobRequestRequestTypeDef",
+    "HumanTaskConfigUnionTypeDef",
     "DescribeTrainingJobResponseTypeDef",
     "TrainingJobTypeDef",
+    "AlgorithmSpecificationUnionTypeDef",
     "CreateTransformJobRequestRequestTypeDef",
     "DescribeTransformJobResponseTypeDef",
-    "TransformJobDefinitionPaginatorTypeDef",
+    "TransformJobDefinitionExtraOutputTypeDef",
+    "TransformJobDefinitionOutputTypeDef",
     "TransformJobDefinitionTypeDef",
     "TransformJobTypeDef",
-    "CreateAutoMLJobV2RequestRequestTypeDef",
     "DescribeAutoMLJobV2ResponseTypeDef",
+    "AutoMLProblemTypeConfigUnionTypeDef",
+    "CreateAutoMLJobV2RequestRequestTypeDef",
     "ListPipelineExecutionStepsResponseTypeDef",
     "CreateEndpointInputRequestTypeDef",
+    "DeploymentConfigUnionTypeDef",
     "UpdateEndpointInputRequestTypeDef",
-    "CreateInferenceRecommendationsJobRequestRequestTypeDef",
     "DescribeInferenceRecommendationsJobResponseTypeDef",
-    "CreateEndpointConfigInputRequestTypeDef",
+    "CreateInferenceRecommendationsJobRequestRequestTypeDef",
+    "RecommendationJobInputConfigUnionTypeDef",
     "DescribeEndpointConfigOutputTypeDef",
     "DescribeEndpointOutputTypeDef",
-    "HyperParameterTuningJobSearchEntityPaginatorTypeDef",
-    "CreateHyperParameterTuningJobRequestRequestTypeDef",
+    "CreateEndpointConfigInputRequestTypeDef",
+    "ExplainerConfigUnionTypeDef",
     "DescribeHyperParameterTuningJobResponseTypeDef",
     "HyperParameterTuningJobSearchEntityTypeDef",
+    "CreateTrainingJobRequestRequestTypeDef",
+    "HyperParameterTrainingJobDefinitionUnionTypeDef",
     "ListSpacesResponseTypeDef",
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
-    "ListLabelingJobsResponsePaginatorTypeDef",
+    "TrainingSpecificationUnionTypeDef",
     "ListLabelingJobsResponseTypeDef",
     "DynamicScalingConfigurationTypeDef",
-    "ModelPaginatorTypeDef",
-    "CreateModelInputRequestTypeDef",
     "DescribeModelOutputTypeDef",
     "ModelTypeDef",
-    "AdditionalInferenceSpecificationDefinitionPaginatorTypeDef",
+    "ContainerDefinitionUnionTypeDef",
+    "AdditionalInferenceSpecificationDefinitionExtraOutputTypeDef",
+    "InferenceSpecificationExtraOutputTypeDef",
+    "AdditionalInferenceSpecificationDefinitionOutputTypeDef",
+    "InferenceSpecificationOutputTypeDef",
     "AdditionalInferenceSpecificationDefinitionTypeDef",
     "InferenceSpecificationTypeDef",
-    "SourceAlgorithmSpecificationPaginatorTypeDef",
+    "SourceAlgorithmSpecificationExtraOutputTypeDef",
+    "SourceAlgorithmSpecificationOutputTypeDef",
     "SourceAlgorithmSpecificationTypeDef",
-    "MonitoringJobDefinitionPaginatorTypeDef",
-    "CreateDataQualityJobDefinitionRequestRequestTypeDef",
+    "MonitoringJobDefinitionExtraOutputTypeDef",
     "DescribeDataQualityJobDefinitionResponseTypeDef",
-    "CreateModelBiasJobDefinitionRequestRequestTypeDef",
     "DescribeModelBiasJobDefinitionResponseTypeDef",
-    "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
     "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
-    "CreateModelQualityJobDefinitionRequestRequestTypeDef",
     "DescribeModelQualityJobDefinitionResponseTypeDef",
+    "MonitoringJobDefinitionOutputTypeDef",
+    "CreateDataQualityJobDefinitionRequestRequestTypeDef",
+    "DataQualityJobInputUnionTypeDef",
+    "CreateModelBiasJobDefinitionRequestRequestTypeDef",
+    "ModelBiasJobInputUnionTypeDef",
+    "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
+    "ModelExplainabilityJobInputUnionTypeDef",
+    "CreateModelQualityJobDefinitionRequestRequestTypeDef",
+    "ModelQualityJobInputUnionTypeDef",
     "MonitoringJobDefinitionTypeDef",
-    "ModelPackageValidationProfilePaginatorTypeDef",
+    "ModelPackageValidationProfileExtraOutputTypeDef",
+    "AlgorithmValidationProfileOutputTypeDef",
+    "ModelPackageValidationProfileOutputTypeDef",
     "AlgorithmValidationProfileTypeDef",
     "ModelPackageValidationProfileTypeDef",
-    "TrialComponentSourceDetailPaginatorTypeDef",
     "TrialComponentSourceDetailTypeDef",
+    "CreateHyperParameterTuningJobRequestRequestTypeDef",
     "GetScalingConfigurationRecommendationResponseTypeDef",
+    "CreateModelInputRequestTypeDef",
     "BatchDescribeModelPackageSummaryTypeDef",
-    "UpdateModelPackageInputRequestTypeDef",
-    "MonitoringScheduleConfigPaginatorTypeDef",
+    "AdditionalInferenceSpecificationDefinitionUnionTypeDef",
+    "InferenceSpecificationUnionTypeDef",
+    "SourceAlgorithmSpecificationUnionTypeDef",
+    "MonitoringScheduleConfigExtraOutputTypeDef",
+    "MonitoringScheduleConfigOutputTypeDef",
     "MonitoringScheduleConfigTypeDef",
-    "ModelPackageValidationSpecificationPaginatorTypeDef",
+    "ModelPackageValidationSpecificationExtraOutputTypeDef",
+    "AlgorithmValidationSpecificationOutputTypeDef",
+    "ModelPackageValidationSpecificationOutputTypeDef",
     "AlgorithmValidationSpecificationTypeDef",
     "ModelPackageValidationSpecificationTypeDef",
-    "TrialComponentPaginatorTypeDef",
     "TrialComponentTypeDef",
     "BatchDescribeModelPackageOutputTypeDef",
-    "ModelDashboardMonitoringSchedulePaginatorTypeDef",
-    "MonitoringSchedulePaginatorTypeDef",
-    "CreateMonitoringScheduleRequestRequestTypeDef",
+    "UpdateModelPackageInputRequestTypeDef",
     "DescribeMonitoringScheduleResponseTypeDef",
     "ModelDashboardMonitoringScheduleTypeDef",
     "MonitoringScheduleTypeDef",
+    "CreateMonitoringScheduleRequestRequestTypeDef",
+    "MonitoringScheduleConfigUnionTypeDef",
     "UpdateMonitoringScheduleRequestRequestTypeDef",
-    "ModelPackagePaginatorTypeDef",
-    "CreateAlgorithmInputRequestTypeDef",
     "DescribeAlgorithmOutputTypeDef",
-    "CreateModelPackageInputRequestTypeDef",
     "DescribeModelPackageOutputTypeDef",
     "ModelPackageTypeDef",
-    "ModelDashboardModelPaginatorTypeDef",
-    "EndpointPaginatorTypeDef",
+    "AlgorithmValidationSpecificationUnionTypeDef",
+    "CreateAlgorithmInputRequestTypeDef",
+    "CreateModelPackageInputRequestTypeDef",
+    "ModelPackageValidationSpecificationUnionTypeDef",
     "ModelDashboardModelTypeDef",
     "EndpointTypeDef",
-    "SearchRecordPaginatorTypeDef",
     "SearchRecordTypeDef",
-    "SearchResponsePaginatorTypeDef",
     "SearchResponseTypeDef",
 )
 
 ActionSourceTypeDef = TypedDict(
     "ActionSourceTypeDef",
     {
         "SourceUri": str,
@@ -1680,16 +1835,24 @@
         "SageMakerImageArn": NotRequired[str],
         "SageMakerImageVersionArn": NotRequired[str],
         "SageMakerImageVersionAlias": NotRequired[str],
         "InstanceType": NotRequired[AppInstanceTypeType],
         "LifecycleConfigArn": NotRequired[str],
     },
 )
-AppSpecificationPaginatorTypeDef = TypedDict(
-    "AppSpecificationPaginatorTypeDef",
+AppSpecificationExtraOutputTypeDef = TypedDict(
+    "AppSpecificationExtraOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+    },
+)
+AppSpecificationOutputTypeDef = TypedDict(
+    "AppSpecificationOutputTypeDef",
     {
         "ImageUri": str,
         "ContainerEntrypoint": NotRequired[List[str]],
         "ContainerArguments": NotRequired[List[str]],
     },
 )
 AppSpecificationTypeDef = TypedDict(
@@ -1716,14 +1879,22 @@
 )
 AsyncInferenceClientConfigTypeDef = TypedDict(
     "AsyncInferenceClientConfigTypeDef",
     {
         "MaxConcurrentInvocationsPerInstance": NotRequired[int],
     },
 )
+AsyncInferenceNotificationConfigOutputTypeDef = TypedDict(
+    "AsyncInferenceNotificationConfigOutputTypeDef",
+    {
+        "SuccessTopic": NotRequired[str],
+        "ErrorTopic": NotRequired[str],
+        "IncludeInferenceResponseIn": NotRequired[List[AsyncNotificationTopicTypesType]],
+    },
+)
 AsyncInferenceNotificationConfigTypeDef = TypedDict(
     "AsyncInferenceNotificationConfigTypeDef",
     {
         "SuccessTopic": NotRequired[str],
         "ErrorTopic": NotRequired[str],
         "IncludeInferenceResponseIn": NotRequired[Sequence[AsyncNotificationTopicTypesType]],
     },
@@ -1737,14 +1908,20 @@
         "OutputS3Uri": str,
         "OutputFormat": AthenaResultFormatType,
         "WorkGroup": NotRequired[str],
         "KmsKeyId": NotRequired[str],
         "OutputCompression": NotRequired[AthenaResultCompressionTypeType],
     },
 )
+AutoMLAlgorithmConfigOutputTypeDef = TypedDict(
+    "AutoMLAlgorithmConfigOutputTypeDef",
+    {
+        "AutoMLAlgorithms": List[AutoMLAlgorithmType],
+    },
+)
 AutoMLAlgorithmConfigTypeDef = TypedDict(
     "AutoMLAlgorithmConfigTypeDef",
     {
         "AutoMLAlgorithms": Sequence[AutoMLAlgorithmType],
     },
 )
 AutoMLCandidateStepTypeDef = TypedDict(
@@ -1833,14 +2010,21 @@
 )
 TextGenerationResolvedAttributesTypeDef = TypedDict(
     "TextGenerationResolvedAttributesTypeDef",
     {
         "BaseModelName": NotRequired[str],
     },
 )
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
+    },
+)
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
@@ -1972,34 +2156,61 @@
 CapacitySizeTypeDef = TypedDict(
     "CapacitySizeTypeDef",
     {
         "Type": CapacitySizeTypeType,
         "Value": int,
     },
 )
+CaptureContentTypeHeaderOutputTypeDef = TypedDict(
+    "CaptureContentTypeHeaderOutputTypeDef",
+    {
+        "CsvContentTypes": NotRequired[List[str]],
+        "JsonContentTypes": NotRequired[List[str]],
+    },
+)
 CaptureContentTypeHeaderTypeDef = TypedDict(
     "CaptureContentTypeHeaderTypeDef",
     {
         "CsvContentTypes": NotRequired[Sequence[str]],
         "JsonContentTypes": NotRequired[Sequence[str]],
     },
 )
 CaptureOptionTypeDef = TypedDict(
     "CaptureOptionTypeDef",
     {
         "CaptureMode": CaptureModeType,
     },
 )
-CategoricalParameterRangePaginatorTypeDef = TypedDict(
-    "CategoricalParameterRangePaginatorTypeDef",
+CategoricalParameterOutputTypeDef = TypedDict(
+    "CategoricalParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Value": List[str],
+    },
+)
+CategoricalParameterRangeExtraOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeExtraOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[str],
+    },
+)
+CategoricalParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeOutputTypeDef",
     {
         "Name": str,
         "Values": List[str],
     },
 )
+CategoricalParameterRangeSpecificationOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeSpecificationOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+)
 CategoricalParameterRangeSpecificationTypeDef = TypedDict(
     "CategoricalParameterRangeSpecificationTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 CategoricalParameterRangeTypeDef = TypedDict(
@@ -2018,14 +2229,25 @@
 )
 ShuffleConfigTypeDef = TypedDict(
     "ShuffleConfigTypeDef",
     {
         "Seed": int,
     },
 )
+ChannelSpecificationOutputTypeDef = TypedDict(
+    "ChannelSpecificationOutputTypeDef",
+    {
+        "Name": str,
+        "SupportedContentTypes": List[str],
+        "SupportedInputModes": List[TrainingInputModeType],
+        "Description": NotRequired[str],
+        "IsRequired": NotRequired[bool],
+        "SupportedCompressionTypes": NotRequired[List[CompressionTypeType]],
+    },
+)
 ChannelSpecificationTypeDef = TypedDict(
     "ChannelSpecificationTypeDef",
     {
         "Name": str,
         "SupportedContentTypes": Sequence[str],
         "SupportedInputModes": Sequence[TrainingInputModeType],
         "Description": NotRequired[str],
@@ -2049,14 +2271,30 @@
         "ModelPackageGroupName": NotRequired[str],
         "ViolationReport": NotRequired[str],
         "CheckJobArn": NotRequired[str],
         "SkipCheck": NotRequired[bool],
         "RegisterNewBaseline": NotRequired[bool],
     },
 )
+ClarifyInferenceConfigOutputTypeDef = TypedDict(
+    "ClarifyInferenceConfigOutputTypeDef",
+    {
+        "FeaturesAttribute": NotRequired[str],
+        "ContentTemplate": NotRequired[str],
+        "MaxRecordCount": NotRequired[int],
+        "MaxPayloadInMB": NotRequired[int],
+        "ProbabilityIndex": NotRequired[int],
+        "LabelIndex": NotRequired[int],
+        "ProbabilityAttribute": NotRequired[str],
+        "LabelAttribute": NotRequired[str],
+        "LabelHeaders": NotRequired[List[str]],
+        "FeatureHeaders": NotRequired[List[str]],
+        "FeatureTypes": NotRequired[List[ClarifyFeatureTypeType]],
+    },
+)
 ClarifyInferenceConfigTypeDef = TypedDict(
     "ClarifyInferenceConfigTypeDef",
     {
         "FeaturesAttribute": NotRequired[str],
         "ContentTemplate": NotRequired[str],
         "MaxRecordCount": NotRequired[int],
         "MaxPayloadInMB": NotRequired[int],
@@ -2103,30 +2341,38 @@
     {
         "ClusterArn": str,
         "ClusterName": str,
         "CreationTime": datetime,
         "ClusterStatus": ClusterStatusType,
     },
 )
-ContainerConfigPaginatorTypeDef = TypedDict(
-    "ContainerConfigPaginatorTypeDef",
+ContainerConfigExtraOutputTypeDef = TypedDict(
+    "ContainerConfigExtraOutputTypeDef",
     {
         "ContainerArguments": NotRequired[List[str]],
         "ContainerEntrypoint": NotRequired[List[str]],
         "ContainerEnvironmentVariables": NotRequired[Dict[str, str]],
     },
 )
 FileSystemConfigTypeDef = TypedDict(
     "FileSystemConfigTypeDef",
     {
         "MountPath": NotRequired[str],
         "DefaultUid": NotRequired[int],
         "DefaultGid": NotRequired[int],
     },
 )
+ContainerConfigOutputTypeDef = TypedDict(
+    "ContainerConfigOutputTypeDef",
+    {
+        "ContainerArguments": NotRequired[List[str]],
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerEnvironmentVariables": NotRequired[Dict[str, str]],
+    },
+)
 ContainerConfigTypeDef = TypedDict(
     "ContainerConfigTypeDef",
     {
         "ContainerArguments": NotRequired[Sequence[str]],
         "ContainerEntrypoint": NotRequired[Sequence[str]],
         "ContainerEnvironmentVariables": NotRequired[Mapping[str, str]],
     },
@@ -2170,16 +2416,23 @@
 )
 VectorConfigTypeDef = TypedDict(
     "VectorConfigTypeDef",
     {
         "Dimension": int,
     },
 )
-CollectionConfigurationPaginatorTypeDef = TypedDict(
-    "CollectionConfigurationPaginatorTypeDef",
+CollectionConfigurationExtraOutputTypeDef = TypedDict(
+    "CollectionConfigurationExtraOutputTypeDef",
+    {
+        "CollectionName": NotRequired[str],
+        "CollectionParameters": NotRequired[Dict[str, str]],
+    },
+)
+CollectionConfigurationOutputTypeDef = TypedDict(
+    "CollectionConfigurationOutputTypeDef",
     {
         "CollectionName": NotRequired[str],
         "CollectionParameters": NotRequired[Dict[str, str]],
     },
 )
 CollectionConfigurationTypeDef = TypedDict(
     "CollectionConfigurationTypeDef",
@@ -2502,26 +2755,14 @@
 )
 SpaceSharingSettingsTypeDef = TypedDict(
     "SpaceSharingSettingsTypeDef",
     {
         "SharingType": SharingTypeType,
     },
 )
-DebugRuleConfigurationTypeDef = TypedDict(
-    "DebugRuleConfigurationTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-        "LocalPath": NotRequired[str],
-        "S3OutputPath": NotRequired[str],
-        "InstanceType": NotRequired[ProcessingInstanceTypeType],
-        "VolumeSizeInGB": NotRequired[int],
-        "RuleParameters": NotRequired[Mapping[str, str]],
-    },
-)
 InfraCheckConfigTypeDef = TypedDict(
     "InfraCheckConfigTypeDef",
     {
         "EnableInfraCheck": NotRequired[bool],
     },
 )
 OutputDataConfigTypeDef = TypedDict(
@@ -2537,38 +2778,32 @@
     {
         "S3OutputPath": NotRequired[str],
         "ProfilingIntervalInMilliseconds": NotRequired[int],
         "ProfilingParameters": NotRequired[Mapping[str, str]],
         "DisableProfiler": NotRequired[bool],
     },
 )
-ProfilerRuleConfigurationTypeDef = TypedDict(
-    "ProfilerRuleConfigurationTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-        "LocalPath": NotRequired[str],
-        "S3OutputPath": NotRequired[str],
-        "InstanceType": NotRequired[ProcessingInstanceTypeType],
-        "VolumeSizeInGB": NotRequired[int],
-        "RuleParameters": NotRequired[Mapping[str, str]],
-    },
-)
 RemoteDebugConfigTypeDef = TypedDict(
     "RemoteDebugConfigTypeDef",
     {
         "EnableRemoteDebug": NotRequired[bool],
     },
 )
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "MaximumRetryAttempts": int,
     },
 )
+SessionChainingConfigTypeDef = TypedDict(
+    "SessionChainingConfigTypeDef",
+    {
+        "EnableSessionTagChaining": NotRequired[bool],
+    },
+)
 TensorBoardOutputConfigTypeDef = TypedDict(
     "TensorBoardOutputConfigTypeDef",
     {
         "S3OutputPath": str,
         "LocalPath": NotRequired[str],
     },
 )
@@ -2701,14 +2936,25 @@
     "DataCatalogConfigTypeDef",
     {
         "TableName": str,
         "Catalog": str,
         "Database": str,
     },
 )
+DataQualityAppSpecificationOutputTypeDef = TypedDict(
+    "DataQualityAppSpecificationOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+        "RecordPreprocessorSourceUri": NotRequired[str],
+        "PostAnalyticsProcessorSourceUri": NotRequired[str],
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
 MonitoringConstraintsResourceTypeDef = TypedDict(
     "MonitoringConstraintsResourceTypeDef",
     {
         "S3Uri": NotRequired[str],
     },
 )
 MonitoringStatisticsResourceTypeDef = TypedDict(
@@ -2738,16 +2984,26 @@
     {
         "FileSystemId": str,
         "FileSystemAccessMode": FileSystemAccessModeType,
         "FileSystemType": FileSystemTypeType,
         "DirectoryPath": str,
     },
 )
-S3DataSourcePaginatorTypeDef = TypedDict(
-    "S3DataSourcePaginatorTypeDef",
+S3DataSourceExtraOutputTypeDef = TypedDict(
+    "S3DataSourceExtraOutputTypeDef",
+    {
+        "S3DataType": S3DataTypeType,
+        "S3Uri": str,
+        "S3DataDistributionType": NotRequired[S3DataDistributionType],
+        "AttributeNames": NotRequired[List[str]],
+        "InstanceGroupNames": NotRequired[List[str]],
+    },
+)
+S3DataSourceOutputTypeDef = TypedDict(
+    "S3DataSourceOutputTypeDef",
     {
         "S3DataType": S3DataTypeType,
         "S3Uri": str,
         "S3DataDistributionType": NotRequired[S3DataDistributionType],
         "AttributeNames": NotRequired[List[str]],
         "InstanceGroupNames": NotRequired[List[str]],
     },
@@ -2772,26 +3028,50 @@
         "ClusterRoleArn": str,
         "OutputS3Uri": str,
         "OutputFormat": RedshiftResultFormatType,
         "KmsKeyId": NotRequired[str],
         "OutputCompression": NotRequired[RedshiftResultCompressionTypeType],
     },
 )
-DebugRuleConfigurationPaginatorTypeDef = TypedDict(
-    "DebugRuleConfigurationPaginatorTypeDef",
+DebugRuleConfigurationExtraOutputTypeDef = TypedDict(
+    "DebugRuleConfigurationExtraOutputTypeDef",
     {
         "RuleConfigurationName": str,
         "RuleEvaluatorImage": str,
         "LocalPath": NotRequired[str],
         "S3OutputPath": NotRequired[str],
         "InstanceType": NotRequired[ProcessingInstanceTypeType],
         "VolumeSizeInGB": NotRequired[int],
         "RuleParameters": NotRequired[Dict[str, str]],
     },
 )
+DebugRuleConfigurationOutputTypeDef = TypedDict(
+    "DebugRuleConfigurationOutputTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+        "LocalPath": NotRequired[str],
+        "S3OutputPath": NotRequired[str],
+        "InstanceType": NotRequired[ProcessingInstanceTypeType],
+        "VolumeSizeInGB": NotRequired[int],
+        "RuleParameters": NotRequired[Dict[str, str]],
+    },
+)
+DebugRuleConfigurationTypeDef = TypedDict(
+    "DebugRuleConfigurationTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+        "LocalPath": NotRequired[str],
+        "S3OutputPath": NotRequired[str],
+        "InstanceType": NotRequired[ProcessingInstanceTypeType],
+        "VolumeSizeInGB": NotRequired[int],
+        "RuleParameters": NotRequired[Mapping[str, str]],
+    },
+)
 DebugRuleEvaluationStatusTypeDef = TypedDict(
     "DebugRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": NotRequired[str],
         "RuleEvaluationJobArn": NotRequired[str],
         "RuleEvaluationStatus": NotRequired[RuleEvaluationStatusType],
         "StatusDetails": NotRequired[str],
@@ -3120,20 +3400,20 @@
     "RealTimeInferenceRecommendationTypeDef",
     {
         "RecommendationId": str,
         "InstanceType": ProductionVariantInstanceTypeType,
         "Environment": NotRequired[Dict[str, str]],
     },
 )
-DeviceSelectionConfigTypeDef = TypedDict(
-    "DeviceSelectionConfigTypeDef",
+DeviceSelectionConfigOutputTypeDef = TypedDict(
+    "DeviceSelectionConfigOutputTypeDef",
     {
         "DeviceSubsetType": DeviceSubsetTypeType,
         "Percentage": NotRequired[int],
-        "DeviceNames": NotRequired[Sequence[str]],
+        "DeviceNames": NotRequired[List[str]],
         "DeviceNameContains": NotRequired[str],
     },
 )
 EdgeDeploymentConfigTypeDef = TypedDict(
     "EdgeDeploymentConfigTypeDef",
     {
         "FailureHandlingPolicy": FailureHandlingPolicyType,
@@ -3146,14 +3426,23 @@
         "EdgeDeploymentSuccessInStage": int,
         "EdgeDeploymentPendingInStage": int,
         "EdgeDeploymentFailedInStage": int,
         "EdgeDeploymentStatusMessage": NotRequired[str],
         "EdgeDeploymentStageStartTime": NotRequired[datetime],
     },
 )
+DeviceSelectionConfigTypeDef = TypedDict(
+    "DeviceSelectionConfigTypeDef",
+    {
+        "DeviceSubsetType": DeviceSubsetTypeType,
+        "Percentage": NotRequired[int],
+        "DeviceNames": NotRequired[Sequence[str]],
+        "DeviceNameContains": NotRequired[str],
+    },
+)
 DeregisterDevicesRequestRequestTypeDef = TypedDict(
     "DeregisterDevicesRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
         "DeviceNames": Sequence[str],
     },
 )
@@ -3248,14 +3537,21 @@
 )
 ModelDigestsTypeDef = TypedDict(
     "ModelDigestsTypeDef",
     {
         "ArtifactDigest": NotRequired[str],
     },
 )
+NeoVpcConfigOutputTypeDef = TypedDict(
+    "NeoVpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
+    },
+)
 DescribeContextRequestRequestTypeDef = TypedDict(
     "DescribeContextRequestRequestTypeDef",
     {
         "ContextName": str,
     },
 )
 DescribeDataQualityJobDefinitionRequestRequestTypeDef = TypedDict(
@@ -3507,14 +3803,21 @@
     {
         "EndpointName": str,
         "EndpointConfigName": NotRequired[str],
         "EndpointStatus": NotRequired[EndpointStatusType],
         "FailureReason": NotRequired[str],
     },
 )
+InferenceExperimentScheduleOutputTypeDef = TypedDict(
+    "InferenceExperimentScheduleOutputTypeDef",
+    {
+        "StartTime": NotRequired[datetime],
+        "EndTime": NotRequired[datetime],
+    },
+)
 DescribeInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 DescribeLabelingJobRequestRequestTypeDef = TypedDict(
@@ -3548,14 +3851,22 @@
 )
 DescribeModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelBiasJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
+ModelBiasAppSpecificationOutputTypeDef = TypedDict(
+    "ModelBiasAppSpecificationOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ConfigUri": str,
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
 DescribeModelCardExportJobRequestRequestTypeDef = TypedDict(
     "DescribeModelCardExportJobRequestRequestTypeDef",
     {
         "ModelCardExportJobArn": str,
     },
 )
 ModelCardExportArtifactsTypeDef = TypedDict(
@@ -3573,14 +3884,22 @@
 )
 DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
+ModelExplainabilityAppSpecificationOutputTypeDef = TypedDict(
+    "ModelExplainabilityAppSpecificationOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ConfigUri": str,
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
 DescribeModelInputRequestTypeDef = TypedDict(
     "DescribeModelInputRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 DescribeModelPackageGroupInputRequestTypeDef = TypedDict(
@@ -3597,14 +3916,26 @@
 )
 DescribeModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
+ModelQualityAppSpecificationOutputTypeDef = TypedDict(
+    "ModelQualityAppSpecificationOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+        "RecordPreprocessorSourceUri": NotRequired[str],
+        "PostAnalyticsProcessorSourceUri": NotRequired[str],
+        "ProblemType": NotRequired[MonitoringProblemTypeType],
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
 DescribeMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
     },
 )
 MonitoringExecutionSummaryTypeDef = TypedDict(
@@ -3717,14 +4048,35 @@
     "MetricDataTypeDef",
     {
         "MetricName": NotRequired[str],
         "Value": NotRequired[float],
         "Timestamp": NotRequired[datetime],
     },
 )
+ProfilerConfigOutputTypeDef = TypedDict(
+    "ProfilerConfigOutputTypeDef",
+    {
+        "S3OutputPath": NotRequired[str],
+        "ProfilingIntervalInMilliseconds": NotRequired[int],
+        "ProfilingParameters": NotRequired[Dict[str, str]],
+        "DisableProfiler": NotRequired[bool],
+    },
+)
+ProfilerRuleConfigurationOutputTypeDef = TypedDict(
+    "ProfilerRuleConfigurationOutputTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+        "LocalPath": NotRequired[str],
+        "S3OutputPath": NotRequired[str],
+        "InstanceType": NotRequired[ProcessingInstanceTypeType],
+        "VolumeSizeInGB": NotRequired[int],
+        "RuleParameters": NotRequired[Dict[str, str]],
+    },
+)
 ProfilerRuleEvaluationStatusTypeDef = TypedDict(
     "ProfilerRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": NotRequired[str],
         "RuleEvaluationJobArn": NotRequired[str],
         "RuleEvaluationStatus": NotRequired[RuleEvaluationStatusType],
         "StatusDetails": NotRequired[str],
@@ -3870,14 +4222,21 @@
 DisassociateTrialComponentRequestRequestTypeDef = TypedDict(
     "DisassociateTrialComponentRequestRequestTypeDef",
     {
         "TrialComponentName": str,
         "TrialName": str,
     },
 )
+DockerSettingsOutputTypeDef = TypedDict(
+    "DockerSettingsOutputTypeDef",
+    {
+        "EnableDockerAccess": NotRequired[FeatureStatusType],
+        "VpcOnlyTrustedAccounts": NotRequired[List[str]],
+    },
+)
 DockerSettingsTypeDef = TypedDict(
     "DockerSettingsTypeDef",
     {
         "EnableDockerAccess": NotRequired[FeatureStatusType],
         "VpcOnlyTrustedAccounts": NotRequired[Sequence[str]],
     },
 )
@@ -4142,16 +4501,16 @@
 HyperParameterTuningJobObjectiveTypeDef = TypedDict(
     "HyperParameterTuningJobObjectiveTypeDef",
     {
         "Type": HyperParameterTuningJobObjectiveTypeType,
         "MetricName": str,
     },
 )
-VpcConfigPaginatorTypeDef = TypedDict(
-    "VpcConfigPaginatorTypeDef",
+VpcConfigExtraOutputTypeDef = TypedDict(
+    "VpcConfigExtraOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "Subnets": List[str],
     },
 )
 HyperParameterTuningInstanceConfigTypeDef = TypedDict(
     "HyperParameterTuningInstanceConfigTypeDef",
@@ -4254,16 +4613,16 @@
         "EndpointArn": str,
         "EndpointName": str,
         "VariantName": str,
         "LastModifiedTime": datetime,
         "InferenceComponentStatus": NotRequired[InferenceComponentStatusType],
     },
 )
-InferenceExperimentSchedulePaginatorTypeDef = TypedDict(
-    "InferenceExperimentSchedulePaginatorTypeDef",
+InferenceExperimentScheduleExtraOutputTypeDef = TypedDict(
+    "InferenceExperimentScheduleExtraOutputTypeDef",
     {
         "StartTime": NotRequired[datetime],
         "EndTime": NotRequired[datetime],
     },
 )
 RecommendationMetricsTypeDef = TypedDict(
     "RecommendationMetricsTypeDef",
@@ -4330,16 +4689,22 @@
     "LabelCountersForWorkteamTypeDef",
     {
         "HumanLabeled": NotRequired[int],
         "PendingHuman": NotRequired[int],
         "Total": NotRequired[int],
     },
 )
-LabelingJobDataAttributesPaginatorTypeDef = TypedDict(
-    "LabelingJobDataAttributesPaginatorTypeDef",
+LabelingJobDataAttributesExtraOutputTypeDef = TypedDict(
+    "LabelingJobDataAttributesExtraOutputTypeDef",
+    {
+        "ContentClassifiers": NotRequired[List[ContentClassifierType]],
+    },
+)
+LabelingJobDataAttributesOutputTypeDef = TypedDict(
+    "LabelingJobDataAttributesOutputTypeDef",
     {
         "ContentClassifiers": NotRequired[List[ContentClassifierType]],
     },
 )
 LabelingJobDataAttributesTypeDef = TypedDict(
     "LabelingJobDataAttributesTypeDef",
     {
@@ -4752,16 +5117,22 @@
         "SortBy": NotRequired[ListWorkteamsSortByOptionsType],
         "SortOrder": NotRequired[SortOrderType],
         "NameContains": NotRequired[str],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
 )
-OidcMemberDefinitionPaginatorTypeDef = TypedDict(
-    "OidcMemberDefinitionPaginatorTypeDef",
+OidcMemberDefinitionExtraOutputTypeDef = TypedDict(
+    "OidcMemberDefinitionExtraOutputTypeDef",
+    {
+        "Groups": NotRequired[List[str]],
+    },
+)
+OidcMemberDefinitionOutputTypeDef = TypedDict(
+    "OidcMemberDefinitionOutputTypeDef",
     {
         "Groups": NotRequired[List[str]],
     },
 )
 OidcMemberDefinitionTypeDef = TypedDict(
     "OidcMemberDefinitionTypeDef",
     {
@@ -4839,16 +5210,26 @@
 )
 ModelStepMetadataTypeDef = TypedDict(
     "ModelStepMetadataTypeDef",
     {
         "Arn": NotRequired[str],
     },
 )
-MonitoringAppSpecificationPaginatorTypeDef = TypedDict(
-    "MonitoringAppSpecificationPaginatorTypeDef",
+MonitoringAppSpecificationExtraOutputTypeDef = TypedDict(
+    "MonitoringAppSpecificationExtraOutputTypeDef",
+    {
+        "ImageUri": str,
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+        "RecordPreprocessorSourceUri": NotRequired[str],
+        "PostAnalyticsProcessorSourceUri": NotRequired[str],
+    },
+)
+MonitoringAppSpecificationOutputTypeDef = TypedDict(
+    "MonitoringAppSpecificationOutputTypeDef",
     {
         "ImageUri": str,
         "ContainerEntrypoint": NotRequired[List[str]],
         "ContainerArguments": NotRequired[List[str]],
         "RecordPreprocessorSourceUri": NotRequired[str],
         "PostAnalyticsProcessorSourceUri": NotRequired[str],
     },
@@ -5072,30 +5453,42 @@
 ProductionVariantCoreDumpConfigTypeDef = TypedDict(
     "ProductionVariantCoreDumpConfigTypeDef",
     {
         "DestinationS3Uri": str,
         "KmsKeyId": NotRequired[str],
     },
 )
+ProfilerConfigExtraOutputTypeDef = TypedDict(
+    "ProfilerConfigExtraOutputTypeDef",
+    {
+        "S3OutputPath": NotRequired[str],
+        "ProfilingIntervalInMilliseconds": NotRequired[int],
+        "ProfilingParameters": NotRequired[Dict[str, str]],
+        "DisableProfiler": NotRequired[bool],
+    },
+)
 ProfilerConfigForUpdateTypeDef = TypedDict(
     "ProfilerConfigForUpdateTypeDef",
     {
         "S3OutputPath": NotRequired[str],
         "ProfilingIntervalInMilliseconds": NotRequired[int],
         "ProfilingParameters": NotRequired[Mapping[str, str]],
         "DisableProfiler": NotRequired[bool],
     },
 )
-ProfilerConfigPaginatorTypeDef = TypedDict(
-    "ProfilerConfigPaginatorTypeDef",
+ProfilerRuleConfigurationTypeDef = TypedDict(
+    "ProfilerRuleConfigurationTypeDef",
     {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+        "LocalPath": NotRequired[str],
         "S3OutputPath": NotRequired[str],
-        "ProfilingIntervalInMilliseconds": NotRequired[int],
-        "ProfilingParameters": NotRequired[Dict[str, str]],
-        "DisableProfiler": NotRequired[bool],
+        "InstanceType": NotRequired[ProcessingInstanceTypeType],
+        "VolumeSizeInGB": NotRequired[int],
+        "RuleParameters": NotRequired[Mapping[str, str]],
     },
 )
 PropertyNameQueryTypeDef = TypedDict(
     "PropertyNameQueryTypeDef",
     {
         "PropertyNameHint": str,
     },
@@ -5139,28 +5532,42 @@
 )
 RecommendationJobCompiledOutputConfigTypeDef = TypedDict(
     "RecommendationJobCompiledOutputConfigTypeDef",
     {
         "S3OutputUri": NotRequired[str],
     },
 )
+RecommendationJobPayloadConfigOutputTypeDef = TypedDict(
+    "RecommendationJobPayloadConfigOutputTypeDef",
+    {
+        "SamplePayloadUrl": NotRequired[str],
+        "SupportedContentTypes": NotRequired[List[str]],
+    },
+)
 RecommendationJobPayloadConfigTypeDef = TypedDict(
     "RecommendationJobPayloadConfigTypeDef",
     {
         "SamplePayloadUrl": NotRequired[str],
         "SupportedContentTypes": NotRequired[Sequence[str]],
     },
 )
 RecommendationJobResourceLimitTypeDef = TypedDict(
     "RecommendationJobResourceLimitTypeDef",
     {
         "MaxNumberOfTests": NotRequired[int],
         "MaxParallelOfTests": NotRequired[int],
     },
 )
+RecommendationJobVpcConfigOutputTypeDef = TypedDict(
+    "RecommendationJobVpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "Subnets": List[str],
+    },
+)
 RecommendationJobVpcConfigTypeDef = TypedDict(
     "RecommendationJobVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
@@ -5221,16 +5628,22 @@
     "SharingSettingsTypeDef",
     {
         "NotebookOutputOption": NotRequired[NotebookOutputOptionType],
         "S3OutputPath": NotRequired[str],
         "S3KmsKeyId": NotRequired[str],
     },
 )
-SourceIpConfigPaginatorTypeDef = TypedDict(
-    "SourceIpConfigPaginatorTypeDef",
+SourceIpConfigExtraOutputTypeDef = TypedDict(
+    "SourceIpConfigExtraOutputTypeDef",
+    {
+        "Cidrs": List[str],
+    },
+)
+SourceIpConfigOutputTypeDef = TypedDict(
+    "SourceIpConfigOutputTypeDef",
     {
         "Cidrs": List[str],
     },
 )
 SpaceSharingSettingsSummaryTypeDef = TypedDict(
     "SpaceSharingSettingsSummaryTypeDef",
     {
@@ -5354,23 +5767,39 @@
     "ThroughputConfigUpdateTypeDef",
     {
         "ThroughputMode": NotRequired[ThroughputModeType],
         "ProvisionedReadCapacityUnits": NotRequired[int],
         "ProvisionedWriteCapacityUnits": NotRequired[int],
     },
 )
+TimeSeriesConfigOutputTypeDef = TypedDict(
+    "TimeSeriesConfigOutputTypeDef",
+    {
+        "TargetAttributeName": str,
+        "TimestampAttributeName": str,
+        "ItemIdentifierAttributeName": str,
+        "GroupingAttributeNames": NotRequired[List[str]],
+    },
+)
 TimeSeriesConfigTypeDef = TypedDict(
     "TimeSeriesConfigTypeDef",
     {
         "TargetAttributeName": str,
         "TimestampAttributeName": str,
         "ItemIdentifierAttributeName": str,
         "GroupingAttributeNames": NotRequired[Sequence[str]],
     },
 )
+TimeSeriesTransformationsOutputTypeDef = TypedDict(
+    "TimeSeriesTransformationsOutputTypeDef",
+    {
+        "Filling": NotRequired[Dict[str, Dict[FillingTypeType, str]]],
+        "Aggregation": NotRequired[Dict[str, AggregationTransformationValueType]],
+    },
+)
 TimeSeriesTransformationsTypeDef = TypedDict(
     "TimeSeriesTransformationsTypeDef",
     {
         "Filling": NotRequired[Mapping[str, Mapping[FillingTypeType, str]]],
         "Aggregation": NotRequired[Mapping[str, AggregationTransformationValueType]],
     },
 )
@@ -6084,16 +6513,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "SageMakerImageVersionAliases": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PutModelPackageGroupPolicyOutputTypeDef = TypedDict(
     "PutModelPackageGroupPolicyOutputTypeDef",
     {
         "ModelPackageGroupArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6425,26 +6854,41 @@
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 ListTagsOutputTypeDef = TypedDict(
     "ListTagsOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+AutoRollbackConfigOutputTypeDef = TypedDict(
+    "AutoRollbackConfigOutputTypeDef",
+    {
+        "Alarms": NotRequired[List[AlarmTypeDef]],
     },
 )
 AutoRollbackConfigTypeDef = TypedDict(
     "AutoRollbackConfigTypeDef",
     {
         "Alarms": NotRequired[Sequence[AlarmTypeDef]],
     },
 )
-HyperParameterAlgorithmSpecificationPaginatorTypeDef = TypedDict(
-    "HyperParameterAlgorithmSpecificationPaginatorTypeDef",
+HyperParameterAlgorithmSpecificationExtraOutputTypeDef = TypedDict(
+    "HyperParameterAlgorithmSpecificationExtraOutputTypeDef",
+    {
+        "TrainingInputMode": TrainingInputModeType,
+        "TrainingImage": NotRequired[str],
+        "AlgorithmName": NotRequired[str],
+        "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
+    },
+)
+HyperParameterAlgorithmSpecificationOutputTypeDef = TypedDict(
+    "HyperParameterAlgorithmSpecificationOutputTypeDef",
     {
         "TrainingInputMode": TrainingInputModeType,
         "TrainingImage": NotRequired[str],
         "AlgorithmName": NotRequired[str],
         "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
     },
 )
@@ -6464,16 +6908,16 @@
         "ImageScanStatuses": NotRequired[List[AlgorithmStatusItemTypeDef]],
     },
 )
 ListAlgorithmsOutputTypeDef = TypedDict(
     "ListAlgorithmsOutputTypeDef",
     {
         "AlgorithmSummaryList": List[AlgorithmSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AppDetailsTypeDef = TypedDict(
     "AppDetailsTypeDef",
     {
         "DomainId": NotRequired[str],
         "UserProfileName": NotRequired[str],
@@ -6541,37 +6985,67 @@
 )
 TensorBoardAppSettingsTypeDef = TypedDict(
     "TensorBoardAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
     },
 )
-ArtifactSourcePaginatorTypeDef = TypedDict(
-    "ArtifactSourcePaginatorTypeDef",
+AppSpecificationUnionTypeDef = Union[AppSpecificationTypeDef, AppSpecificationExtraOutputTypeDef]
+ArtifactSourceExtraOutputTypeDef = TypedDict(
+    "ArtifactSourceExtraOutputTypeDef",
+    {
+        "SourceUri": str,
+        "SourceTypes": NotRequired[List[ArtifactSourceTypeTypeDef]],
+    },
+)
+ArtifactSourceOutputTypeDef = TypedDict(
+    "ArtifactSourceOutputTypeDef",
     {
         "SourceUri": str,
         "SourceTypes": NotRequired[List[ArtifactSourceTypeTypeDef]],
     },
 )
 ArtifactSourceTypeDef = TypedDict(
     "ArtifactSourceTypeDef",
     {
         "SourceUri": str,
         "SourceTypes": NotRequired[Sequence[ArtifactSourceTypeTypeDef]],
     },
 )
+AsyncInferenceOutputConfigOutputTypeDef = TypedDict(
+    "AsyncInferenceOutputConfigOutputTypeDef",
+    {
+        "KmsKeyId": NotRequired[str],
+        "S3OutputPath": NotRequired[str],
+        "NotificationConfig": NotRequired[AsyncInferenceNotificationConfigOutputTypeDef],
+        "S3FailurePath": NotRequired[str],
+    },
+)
 AsyncInferenceOutputConfigTypeDef = TypedDict(
     "AsyncInferenceOutputConfigTypeDef",
     {
         "KmsKeyId": NotRequired[str],
         "S3OutputPath": NotRequired[str],
         "NotificationConfig": NotRequired[AsyncInferenceNotificationConfigTypeDef],
         "S3FailurePath": NotRequired[str],
     },
 )
+AutoMLCandidateGenerationConfigOutputTypeDef = TypedDict(
+    "AutoMLCandidateGenerationConfigOutputTypeDef",
+    {
+        "FeatureSpecificationS3Uri": NotRequired[str],
+        "AlgorithmsConfig": NotRequired[List[AutoMLAlgorithmConfigOutputTypeDef]],
+    },
+)
+CandidateGenerationConfigOutputTypeDef = TypedDict(
+    "CandidateGenerationConfigOutputTypeDef",
+    {
+        "AlgorithmsConfig": NotRequired[List[AutoMLAlgorithmConfigOutputTypeDef]],
+    },
+)
 AutoMLCandidateGenerationConfigTypeDef = TypedDict(
     "AutoMLCandidateGenerationConfigTypeDef",
     {
         "FeatureSpecificationS3Uri": NotRequired[str],
         "AlgorithmsConfig": NotRequired[Sequence[AutoMLAlgorithmConfigTypeDef]],
     },
 )
@@ -6626,14 +7100,45 @@
 AutoMLProblemTypeResolvedAttributesTypeDef = TypedDict(
     "AutoMLProblemTypeResolvedAttributesTypeDef",
     {
         "TabularResolvedAttributes": NotRequired[TabularResolvedAttributesTypeDef],
         "TextGenerationResolvedAttributes": NotRequired[TextGenerationResolvedAttributesTypeDef],
     },
 )
+AutoMLSecurityConfigOutputTypeDef = TypedDict(
+    "AutoMLSecurityConfigOutputTypeDef",
+    {
+        "VolumeKmsKeyId": NotRequired[str],
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+    },
+)
+LabelingJobResourceConfigOutputTypeDef = TypedDict(
+    "LabelingJobResourceConfigOutputTypeDef",
+    {
+        "VolumeKmsKeyId": NotRequired[str],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+    },
+)
+MonitoringNetworkConfigOutputTypeDef = TypedDict(
+    "MonitoringNetworkConfigOutputTypeDef",
+    {
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "EnableNetworkIsolation": NotRequired[bool],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+    },
+)
+NetworkConfigOutputTypeDef = TypedDict(
+    "NetworkConfigOutputTypeDef",
+    {
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "EnableNetworkIsolation": NotRequired[bool],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+    },
+)
 AutoMLSecurityConfigTypeDef = TypedDict(
     "AutoMLSecurityConfigTypeDef",
     {
         "VolumeKmsKeyId": NotRequired[str],
         "EnableInterContainerTrafficEncryption": NotRequired[bool],
         "VpcConfig": NotRequired[VpcConfigTypeDef],
     },
@@ -6729,14 +7234,26 @@
 CandidatePropertiesTypeDef = TypedDict(
     "CandidatePropertiesTypeDef",
     {
         "CandidateArtifactLocations": NotRequired[CandidateArtifactLocationsTypeDef],
         "CandidateMetrics": NotRequired[List[MetricDatumTypeDef]],
     },
 )
+CanvasAppSettingsOutputTypeDef = TypedDict(
+    "CanvasAppSettingsOutputTypeDef",
+    {
+        "TimeSeriesForecastingSettings": NotRequired[TimeSeriesForecastingSettingsTypeDef],
+        "ModelRegisterSettings": NotRequired[ModelRegisterSettingsTypeDef],
+        "WorkspaceSettings": NotRequired[WorkspaceSettingsTypeDef],
+        "IdentityProviderOAuthSettings": NotRequired[List[IdentityProviderOAuthSettingTypeDef]],
+        "DirectDeploySettings": NotRequired[DirectDeploySettingsTypeDef],
+        "KendraSettings": NotRequired[KendraSettingsTypeDef],
+        "GenerativeAiSettings": NotRequired[GenerativeAiSettingsTypeDef],
+    },
+)
 CanvasAppSettingsTypeDef = TypedDict(
     "CanvasAppSettingsTypeDef",
     {
         "TimeSeriesForecastingSettings": NotRequired[TimeSeriesForecastingSettingsTypeDef],
         "ModelRegisterSettings": NotRequired[ModelRegisterSettingsTypeDef],
         "WorkspaceSettings": NotRequired[WorkspaceSettingsTypeDef],
         "IdentityProviderOAuthSettings": NotRequired[Sequence[IdentityProviderOAuthSettingTypeDef]],
@@ -6759,33 +7276,58 @@
     {
         "Type": TrafficRoutingConfigTypeType,
         "WaitIntervalInSeconds": int,
         "CanarySize": NotRequired[CapacitySizeTypeDef],
         "LinearStepSize": NotRequired[CapacitySizeTypeDef],
     },
 )
+InferenceExperimentDataStorageConfigOutputTypeDef = TypedDict(
+    "InferenceExperimentDataStorageConfigOutputTypeDef",
+    {
+        "Destination": str,
+        "KmsKey": NotRequired[str],
+        "ContentType": NotRequired[CaptureContentTypeHeaderOutputTypeDef],
+    },
+)
 InferenceExperimentDataStorageConfigTypeDef = TypedDict(
     "InferenceExperimentDataStorageConfigTypeDef",
     {
         "Destination": str,
         "KmsKey": NotRequired[str],
         "ContentType": NotRequired[CaptureContentTypeHeaderTypeDef],
     },
 )
+DataCaptureConfigOutputTypeDef = TypedDict(
+    "DataCaptureConfigOutputTypeDef",
+    {
+        "InitialSamplingPercentage": int,
+        "DestinationS3Uri": str,
+        "CaptureOptions": List[CaptureOptionTypeDef],
+        "EnableCapture": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "CaptureContentTypeHeader": NotRequired[CaptureContentTypeHeaderOutputTypeDef],
+    },
+)
 DataCaptureConfigTypeDef = TypedDict(
     "DataCaptureConfigTypeDef",
     {
         "InitialSamplingPercentage": int,
         "DestinationS3Uri": str,
         "CaptureOptions": Sequence[CaptureOptionTypeDef],
         "EnableCapture": NotRequired[bool],
         "KmsKeyId": NotRequired[str],
         "CaptureContentTypeHeader": NotRequired[CaptureContentTypeHeaderTypeDef],
     },
 )
+EnvironmentParameterRangesOutputTypeDef = TypedDict(
+    "EnvironmentParameterRangesOutputTypeDef",
+    {
+        "CategoricalParameterRanges": NotRequired[List[CategoricalParameterOutputTypeDef]],
+    },
+)
 EnvironmentParameterRangesTypeDef = TypedDict(
     "EnvironmentParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": NotRequired[Sequence[CategoricalParameterTypeDef]],
     },
 )
 ClarifyShapConfigTypeDef = TypedDict(
@@ -6847,26 +7389,40 @@
     "ListClustersResponseTypeDef",
     {
         "NextToken": str,
         "ClusterSummaries": List[ClusterSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CodeEditorAppImageConfigPaginatorTypeDef = TypedDict(
-    "CodeEditorAppImageConfigPaginatorTypeDef",
+CodeEditorAppImageConfigExtraOutputTypeDef = TypedDict(
+    "CodeEditorAppImageConfigExtraOutputTypeDef",
     {
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
-        "ContainerConfig": NotRequired[ContainerConfigPaginatorTypeDef],
+        "ContainerConfig": NotRequired[ContainerConfigExtraOutputTypeDef],
     },
 )
-JupyterLabAppImageConfigPaginatorTypeDef = TypedDict(
-    "JupyterLabAppImageConfigPaginatorTypeDef",
+JupyterLabAppImageConfigExtraOutputTypeDef = TypedDict(
+    "JupyterLabAppImageConfigExtraOutputTypeDef",
     {
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
-        "ContainerConfig": NotRequired[ContainerConfigPaginatorTypeDef],
+        "ContainerConfig": NotRequired[ContainerConfigExtraOutputTypeDef],
+    },
+)
+CodeEditorAppImageConfigOutputTypeDef = TypedDict(
+    "CodeEditorAppImageConfigOutputTypeDef",
+    {
+        "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
+        "ContainerConfig": NotRequired[ContainerConfigOutputTypeDef],
+    },
+)
+JupyterLabAppImageConfigOutputTypeDef = TypedDict(
+    "JupyterLabAppImageConfigOutputTypeDef",
+    {
+        "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
+        "ContainerConfig": NotRequired[ContainerConfigOutputTypeDef],
     },
 )
 CodeEditorAppImageConfigTypeDef = TypedDict(
     "CodeEditorAppImageConfigTypeDef",
     {
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
         "ContainerConfig": NotRequired[ContainerConfigTypeDef],
@@ -6875,30 +7431,53 @@
 JupyterLabAppImageConfigTypeDef = TypedDict(
     "JupyterLabAppImageConfigTypeDef",
     {
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
         "ContainerConfig": NotRequired[ContainerConfigTypeDef],
     },
 )
+CodeEditorAppSettingsOutputTypeDef = TypedDict(
+    "CodeEditorAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CustomImages": NotRequired[List[CustomImageTypeDef]],
+        "LifecycleConfigArns": NotRequired[List[str]],
+    },
+)
 CodeEditorAppSettingsTypeDef = TypedDict(
     "CodeEditorAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CustomImages": NotRequired[Sequence[CustomImageTypeDef]],
         "LifecycleConfigArns": NotRequired[Sequence[str]],
     },
 )
+KernelGatewayAppSettingsOutputTypeDef = TypedDict(
+    "KernelGatewayAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CustomImages": NotRequired[List[CustomImageTypeDef]],
+        "LifecycleConfigArns": NotRequired[List[str]],
+    },
+)
 KernelGatewayAppSettingsTypeDef = TypedDict(
     "KernelGatewayAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CustomImages": NotRequired[Sequence[CustomImageTypeDef]],
         "LifecycleConfigArns": NotRequired[Sequence[str]],
     },
 )
+RSessionAppSettingsOutputTypeDef = TypedDict(
+    "RSessionAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CustomImages": NotRequired[List[CustomImageTypeDef]],
+    },
+)
 RSessionAppSettingsTypeDef = TypedDict(
     "RSessionAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CustomImages": NotRequired[Sequence[CustomImageTypeDef]],
     },
 )
@@ -6927,51 +7506,84 @@
         "CodeRepositoryArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "GitConfig": GitConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+JupyterLabAppSettingsOutputTypeDef = TypedDict(
+    "JupyterLabAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CustomImages": NotRequired[List[CustomImageTypeDef]],
+        "LifecycleConfigArns": NotRequired[List[str]],
+        "CodeRepositories": NotRequired[List[CodeRepositoryTypeDef]],
+    },
+)
 JupyterLabAppSettingsTypeDef = TypedDict(
     "JupyterLabAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CustomImages": NotRequired[Sequence[CustomImageTypeDef]],
         "LifecycleConfigArns": NotRequired[Sequence[str]],
         "CodeRepositories": NotRequired[Sequence[CodeRepositoryTypeDef]],
     },
 )
+JupyterServerAppSettingsOutputTypeDef = TypedDict(
+    "JupyterServerAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "LifecycleConfigArns": NotRequired[List[str]],
+        "CodeRepositories": NotRequired[List[CodeRepositoryTypeDef]],
+    },
+)
 JupyterServerAppSettingsTypeDef = TypedDict(
     "JupyterServerAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "LifecycleConfigArns": NotRequired[Sequence[str]],
         "CodeRepositories": NotRequired[Sequence[CodeRepositoryTypeDef]],
     },
 )
+SpaceJupyterLabAppSettingsOutputTypeDef = TypedDict(
+    "SpaceJupyterLabAppSettingsOutputTypeDef",
+    {
+        "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
+        "CodeRepositories": NotRequired[List[CodeRepositoryTypeDef]],
+    },
+)
 SpaceJupyterLabAppSettingsTypeDef = TypedDict(
     "SpaceJupyterLabAppSettingsTypeDef",
     {
         "DefaultResourceSpec": NotRequired[ResourceSpecTypeDef],
         "CodeRepositories": NotRequired[Sequence[CodeRepositoryTypeDef]],
     },
 )
 CollectionConfigTypeDef = TypedDict(
     "CollectionConfigTypeDef",
     {
         "VectorConfig": NotRequired[VectorConfigTypeDef],
     },
 )
-DebugHookConfigPaginatorTypeDef = TypedDict(
-    "DebugHookConfigPaginatorTypeDef",
+DebugHookConfigExtraOutputTypeDef = TypedDict(
+    "DebugHookConfigExtraOutputTypeDef",
+    {
+        "S3OutputPath": str,
+        "LocalPath": NotRequired[str],
+        "HookParameters": NotRequired[Dict[str, str]],
+        "CollectionConfigurations": NotRequired[List[CollectionConfigurationExtraOutputTypeDef]],
+    },
+)
+DebugHookConfigOutputTypeDef = TypedDict(
+    "DebugHookConfigOutputTypeDef",
     {
         "S3OutputPath": str,
         "LocalPath": NotRequired[str],
         "HookParameters": NotRequired[Dict[str, str]],
-        "CollectionConfigurations": NotRequired[List[CollectionConfigurationPaginatorTypeDef]],
+        "CollectionConfigurations": NotRequired[List[CollectionConfigurationOutputTypeDef]],
     },
 )
 DebugHookConfigTypeDef = TypedDict(
     "DebugHookConfigTypeDef",
     {
         "S3OutputPath": str,
         "LocalPath": NotRequired[str],
@@ -6979,16 +7591,16 @@
         "CollectionConfigurations": NotRequired[Sequence[CollectionConfigurationTypeDef]],
     },
 )
 ListCompilationJobsResponseTypeDef = TypedDict(
     "ListCompilationJobsResponseTypeDef",
     {
         "CompilationJobSummaries": List[CompilationJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ContextSummaryTypeDef = TypedDict(
     "ContextSummaryTypeDef",
     {
         "ContextArn": NotRequired[str],
         "ContextName": NotRequired[str],
@@ -8176,14 +8788,17 @@
 )
 CustomFileSystemTypeDef = TypedDict(
     "CustomFileSystemTypeDef",
     {
         "EFSFileSystem": NotRequired[EFSFileSystemTypeDef],
     },
 )
+DataQualityAppSpecificationUnionTypeDef = Union[
+    DataQualityAppSpecificationTypeDef, DataQualityAppSpecificationOutputTypeDef
+]
 ModelBiasBaselineConfigTypeDef = TypedDict(
     "ModelBiasBaselineConfigTypeDef",
     {
         "BaseliningJobName": NotRequired[str],
         "ConstraintsResource": NotRequired[MonitoringConstraintsResourceTypeDef],
     },
 )
@@ -8213,18 +8828,25 @@
     "MonitoringBaselineConfigTypeDef",
     {
         "BaseliningJobName": NotRequired[str],
         "ConstraintsResource": NotRequired[MonitoringConstraintsResourceTypeDef],
         "StatisticsResource": NotRequired[MonitoringStatisticsResourceTypeDef],
     },
 )
-DataSourcePaginatorTypeDef = TypedDict(
-    "DataSourcePaginatorTypeDef",
+DataSourceExtraOutputTypeDef = TypedDict(
+    "DataSourceExtraOutputTypeDef",
     {
-        "S3DataSource": NotRequired[S3DataSourcePaginatorTypeDef],
+        "S3DataSource": NotRequired[S3DataSourceExtraOutputTypeDef],
+        "FileSystemDataSource": NotRequired[FileSystemDataSourceTypeDef],
+    },
+)
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "S3DataSource": NotRequired[S3DataSourceOutputTypeDef],
         "FileSystemDataSource": NotRequired[FileSystemDataSourceTypeDef],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "S3DataSource": NotRequired[S3DataSourceTypeDef],
@@ -8237,14 +8859,17 @@
         "AthenaDatasetDefinition": NotRequired[AthenaDatasetDefinitionTypeDef],
         "RedshiftDatasetDefinition": NotRequired[RedshiftDatasetDefinitionTypeDef],
         "LocalPath": NotRequired[str],
         "DataDistributionType": NotRequired[DataDistributionTypeType],
         "InputMode": NotRequired[InputModeType],
     },
 )
+DebugRuleConfigurationUnionTypeDef = Union[
+    DebugRuleConfigurationTypeDef, DebugRuleConfigurationExtraOutputTypeDef
+]
 DefaultSpaceStorageSettingsTypeDef = TypedDict(
     "DefaultSpaceStorageSettingsTypeDef",
     {
         "DefaultEbsStorageSettings": NotRequired[DefaultEbsStorageSettingsTypeDef],
     },
 )
 DeleteDomainRequestRequestTypeDef = TypedDict(
@@ -8267,46 +8892,47 @@
     {
         "RecommendationStatus": RecommendationStatusType,
         "RealTimeInferenceRecommendations": NotRequired[
             List[RealTimeInferenceRecommendationTypeDef]
         ],
     },
 )
-DeploymentStageTypeDef = TypedDict(
-    "DeploymentStageTypeDef",
+DeploymentStageStatusSummaryTypeDef = TypedDict(
+    "DeploymentStageStatusSummaryTypeDef",
     {
         "StageName": str,
-        "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
-        "DeploymentConfig": NotRequired[EdgeDeploymentConfigTypeDef],
+        "DeviceSelectionConfig": DeviceSelectionConfigOutputTypeDef,
+        "DeploymentConfig": EdgeDeploymentConfigTypeDef,
+        "DeploymentStatus": EdgeDeploymentStatusTypeDef,
     },
 )
-DeploymentStageStatusSummaryTypeDef = TypedDict(
-    "DeploymentStageStatusSummaryTypeDef",
+DeploymentStageTypeDef = TypedDict(
+    "DeploymentStageTypeDef",
     {
         "StageName": str,
         "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
-        "DeploymentConfig": EdgeDeploymentConfigTypeDef,
-        "DeploymentStatus": EdgeDeploymentStatusTypeDef,
+        "DeploymentConfig": NotRequired[EdgeDeploymentConfigTypeDef],
     },
 )
+NeoVpcConfigUnionTypeDef = Union[NeoVpcConfigTypeDef, NeoVpcConfigOutputTypeDef]
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceArn": str,
         "DeviceName": str,
         "Description": str,
         "DeviceFleetName": str,
         "IotThingName": str,
         "RegistrationTime": datetime,
         "LatestHeartbeat": datetime,
         "Models": List[EdgeModelTypeDef],
         "MaxModels": int,
-        "NextToken": str,
         "AgentVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeEdgePackagingJobResponseTypeDef = TypedDict(
     "DescribeEdgePackagingJobResponseTypeDef",
     {
         "EdgePackagingJobArn": str,
         "EdgePackagingJobName": str,
@@ -8508,14 +9134,32 @@
         "HumanTaskUiName": str,
         "HumanTaskUiStatus": HumanTaskUiStatusType,
         "CreationTime": datetime,
         "UiTemplate": UiTemplateInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+InferenceExperimentSummaryTypeDef = TypedDict(
+    "InferenceExperimentSummaryTypeDef",
+    {
+        "Name": str,
+        "Type": Literal["ShadowMode"],
+        "Status": InferenceExperimentStatusType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "Schedule": NotRequired[InferenceExperimentScheduleOutputTypeDef],
+        "StatusReason": NotRequired[str],
+        "Description": NotRequired[str],
+        "CompletionTime": NotRequired[datetime],
+        "RoleArn": NotRequired[str],
+    },
+)
+ModelBiasAppSpecificationUnionTypeDef = Union[
+    ModelBiasAppSpecificationTypeDef, ModelBiasAppSpecificationOutputTypeDef
+]
 DescribeModelCardExportJobResponseTypeDef = TypedDict(
     "DescribeModelCardExportJobResponseTypeDef",
     {
         "ModelCardExportJobName": str,
         "ModelCardExportJobArn": str,
         "Status": ModelCardExportJobStatusType,
         "ModelCardName": str,
@@ -8524,35 +9168,41 @@
         "CreatedAt": datetime,
         "LastModifiedAt": datetime,
         "FailureReason": str,
         "ExportArtifacts": ModelCardExportArtifactsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ModelExplainabilityAppSpecificationUnionTypeDef = Union[
+    ModelExplainabilityAppSpecificationTypeDef, ModelExplainabilityAppSpecificationOutputTypeDef
+]
+ModelQualityAppSpecificationUnionTypeDef = Union[
+    ModelQualityAppSpecificationTypeDef, ModelQualityAppSpecificationOutputTypeDef
+]
 ListMonitoringExecutionsResponseTypeDef = TypedDict(
     "ListMonitoringExecutionsResponseTypeDef",
     {
         "MonitoringExecutionSummaries": List[MonitoringExecutionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSubscribedWorkteamResponseTypeDef = TypedDict(
     "DescribeSubscribedWorkteamResponseTypeDef",
     {
         "SubscribedWorkteam": SubscribedWorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSubscribedWorkteamsResponseTypeDef = TypedDict(
     "ListSubscribedWorkteamsResponseTypeDef",
     {
         "SubscribedWorkteams": List[SubscribedWorkteamTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TrainingJobSummaryTypeDef = TypedDict(
     "TrainingJobSummaryTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
@@ -8583,24 +9233,24 @@
         "ServerlessUpdateConfig": NotRequired[ProductionVariantServerlessUpdateConfigTypeDef],
     },
 )
 ListStageDevicesResponseTypeDef = TypedDict(
     "ListStageDevicesResponseTypeDef",
     {
         "DeviceDeploymentSummaries": List[DeviceDeploymentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDeviceFleetsResponseTypeDef = TypedDict(
     "ListDeviceFleetsResponseTypeDef",
     {
         "DeviceFleetSummaries": List[DeviceFleetSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "DeviceName": str,
         "DeviceArn": str,
@@ -8628,16 +9278,16 @@
         "Devices": Sequence[DeviceTypeDef],
     },
 )
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DriftCheckBiasTypeDef = TypedDict(
     "DriftCheckBiasTypeDef",
     {
         "ConfigFile": NotRequired[FileSourceTypeDef],
         "PreTrainingConstraints": NotRequired[MetricsSourceTypeDef],
@@ -8657,16 +9307,16 @@
         "EbsStorageSettings": NotRequired[EbsStorageSettingsTypeDef],
     },
 )
 ListEdgeDeploymentPlansResponseTypeDef = TypedDict(
     "ListEdgeDeploymentPlansResponseTypeDef",
     {
         "EdgeDeploymentPlanSummaries": List[EdgeDeploymentPlanSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetDeviceFleetReportResponseTypeDef = TypedDict(
     "GetDeviceFleetReportResponseTypeDef",
     {
         "DeviceFleetArn": str,
         "DeviceFleetName": str,
@@ -8679,24 +9329,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListEdgePackagingJobsResponseTypeDef = TypedDict(
     "ListEdgePackagingJobsResponseTypeDef",
     {
         "EdgePackagingJobSummaries": List[EdgePackagingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListEndpointConfigsOutputTypeDef = TypedDict(
     "ListEndpointConfigsOutputTypeDef",
     {
         "EndpointConfigs": List[EndpointConfigSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 EndpointOutputConfigurationTypeDef = TypedDict(
     "EndpointOutputConfigurationTypeDef",
     {
         "EndpointName": str,
         "VariantName": str,
@@ -8712,16 +9362,16 @@
         "EndpointInfo": EndpointInfoTypeDef,
     },
 )
 ListEndpointsOutputTypeDef = TypedDict(
     "ListEndpointsOutputTypeDef",
     {
         "Endpoints": List[EndpointSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ModelConfigurationTypeDef = TypedDict(
     "ModelConfigurationTypeDef",
     {
         "InferenceSpecificationName": NotRequired[str],
         "EnvironmentParameters": NotRequired[List[EnvironmentParameterTypeDef]],
@@ -8754,16 +9404,16 @@
         "ObjectiveStatus": NotRequired[ObjectiveStatusType],
     },
 )
 ListFlowDefinitionsResponseTypeDef = TypedDict(
     "ListFlowDefinitionsResponseTypeDef",
     {
         "FlowDefinitionSummaries": List[FlowDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
     "GetScalingConfigurationRecommendationRequestRequestTypeDef",
     {
         "InferenceRecommendationsJobName": str,
         "RecommendationId": NotRequired[str],
@@ -8786,58 +9436,70 @@
         "GitConfig": NotRequired[GitConfigForUpdateTypeDef],
     },
 )
 ListHubContentVersionsResponseTypeDef = TypedDict(
     "ListHubContentVersionsResponseTypeDef",
     {
         "HubContentSummaries": List[HubContentInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListHubContentsResponseTypeDef = TypedDict(
     "ListHubContentsResponseTypeDef",
     {
         "HubContentSummaries": List[HubContentInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListHubsResponseTypeDef = TypedDict(
     "ListHubsResponseTypeDef",
     {
         "HubSummaries": List[HubInfoTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 HumanLoopActivationConfigTypeDef = TypedDict(
     "HumanLoopActivationConfigTypeDef",
     {
         "HumanLoopActivationConditionsConfig": HumanLoopActivationConditionsConfigTypeDef,
     },
 )
 ListHumanTaskUisResponseTypeDef = TypedDict(
     "ListHumanTaskUisResponseTypeDef",
     {
         "HumanTaskUiSummaries": List[HumanTaskUiSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-NetworkConfigPaginatorTypeDef = TypedDict(
-    "NetworkConfigPaginatorTypeDef",
+NetworkConfigExtraOutputTypeDef = TypedDict(
+    "NetworkConfigExtraOutputTypeDef",
     {
         "EnableInterContainerTrafficEncryption": NotRequired[bool],
         "EnableNetworkIsolation": NotRequired[bool],
-        "VpcConfig": NotRequired[VpcConfigPaginatorTypeDef],
+        "VpcConfig": NotRequired[VpcConfigExtraOutputTypeDef],
+    },
+)
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigExtraOutputTypeDef]
+HyperParameterTuningResourceConfigExtraOutputTypeDef = TypedDict(
+    "HyperParameterTuningResourceConfigExtraOutputTypeDef",
+    {
+        "InstanceType": NotRequired[TrainingInstanceTypeType],
+        "InstanceCount": NotRequired[int],
+        "VolumeSizeInGB": NotRequired[int],
+        "VolumeKmsKeyId": NotRequired[str],
+        "AllocationStrategy": NotRequired[Literal["Prioritized"]],
+        "InstanceConfigs": NotRequired[List[HyperParameterTuningInstanceConfigTypeDef]],
     },
 )
-HyperParameterTuningResourceConfigPaginatorTypeDef = TypedDict(
-    "HyperParameterTuningResourceConfigPaginatorTypeDef",
+HyperParameterTuningResourceConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningResourceConfigOutputTypeDef",
     {
         "InstanceType": NotRequired[TrainingInstanceTypeType],
         "InstanceCount": NotRequired[int],
         "VolumeSizeInGB": NotRequired[int],
         "VolumeKmsKeyId": NotRequired[str],
         "AllocationStrategy": NotRequired[Literal["Prioritized"]],
         "InstanceConfigs": NotRequired[List[HyperParameterTuningInstanceConfigTypeDef]],
@@ -8871,16 +9533,23 @@
 )
 HyperParameterTuningJobStrategyConfigTypeDef = TypedDict(
     "HyperParameterTuningJobStrategyConfigTypeDef",
     {
         "HyperbandStrategyConfig": NotRequired[HyperbandStrategyConfigTypeDef],
     },
 )
-HyperParameterTuningJobWarmStartConfigPaginatorTypeDef = TypedDict(
-    "HyperParameterTuningJobWarmStartConfigPaginatorTypeDef",
+HyperParameterTuningJobWarmStartConfigExtraOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobWarmStartConfigExtraOutputTypeDef",
+    {
+        "ParentHyperParameterTuningJobs": List[ParentHyperParameterTuningJobTypeDef],
+        "WarmStartType": HyperParameterTuningJobWarmStartTypeType,
+    },
+)
+HyperParameterTuningJobWarmStartConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobWarmStartConfigOutputTypeDef",
     {
         "ParentHyperParameterTuningJobs": List[ParentHyperParameterTuningJobTypeDef],
         "WarmStartType": HyperParameterTuningJobWarmStartTypeType,
     },
 )
 HyperParameterTuningJobWarmStartConfigTypeDef = TypedDict(
     "HyperParameterTuningJobWarmStartConfigTypeDef",
@@ -8905,24 +9574,24 @@
         "RepositoryAuthConfig": NotRequired[RepositoryAuthConfigTypeDef],
     },
 )
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "Images": List[ImageTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListImageVersionsResponseTypeDef = TypedDict(
     "ListImageVersionsResponseTypeDef",
     {
         "ImageVersions": List[ImageVersionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InferenceComponentSpecificationTypeDef = TypedDict(
     "InferenceComponentSpecificationTypeDef",
     {
         "ComputeResourceRequirements": InferenceComponentComputeResourceRequirementsTypeDef,
         "ModelName": NotRequired[str],
@@ -8930,43 +9599,39 @@
         "StartupParameters": NotRequired[InferenceComponentStartupParametersTypeDef],
     },
 )
 ListInferenceComponentsOutputTypeDef = TypedDict(
     "ListInferenceComponentsOutputTypeDef",
     {
         "InferenceComponents": List[InferenceComponentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-InferenceExperimentSummaryPaginatorTypeDef = TypedDict(
-    "InferenceExperimentSummaryPaginatorTypeDef",
-    {
-        "Name": str,
-        "Type": Literal["ShadowMode"],
-        "Status": InferenceExperimentStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "Schedule": NotRequired[InferenceExperimentSchedulePaginatorTypeDef],
-        "StatusReason": NotRequired[str],
-        "Description": NotRequired[str],
-        "CompletionTime": NotRequired[datetime],
-        "RoleArn": NotRequired[str],
+        "NextToken": NotRequired[str],
     },
 )
 ListInferenceRecommendationsJobsResponseTypeDef = TypedDict(
     "ListInferenceRecommendationsJobsResponseTypeDef",
     {
         "InferenceRecommendationsJobs": List[InferenceRecommendationsJobTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-ResourceConfigPaginatorTypeDef = TypedDict(
-    "ResourceConfigPaginatorTypeDef",
+ResourceConfigExtraOutputTypeDef = TypedDict(
+    "ResourceConfigExtraOutputTypeDef",
+    {
+        "VolumeSizeInGB": int,
+        "InstanceType": NotRequired[TrainingInstanceTypeType],
+        "InstanceCount": NotRequired[int],
+        "VolumeKmsKeyId": NotRequired[str],
+        "KeepAlivePeriodInSeconds": NotRequired[int],
+        "InstanceGroups": NotRequired[List[InstanceGroupTypeDef]],
+    },
+)
+ResourceConfigOutputTypeDef = TypedDict(
+    "ResourceConfigOutputTypeDef",
     {
         "VolumeSizeInGB": int,
         "InstanceType": NotRequired[TrainingInstanceTypeType],
         "InstanceCount": NotRequired[int],
         "VolumeKmsKeyId": NotRequired[str],
         "KeepAlivePeriodInSeconds": NotRequired[int],
         "InstanceGroups": NotRequired[List[InstanceGroupTypeDef]],
@@ -8979,48 +9644,80 @@
         "InstanceType": NotRequired[TrainingInstanceTypeType],
         "InstanceCount": NotRequired[int],
         "VolumeKmsKeyId": NotRequired[str],
         "KeepAlivePeriodInSeconds": NotRequired[int],
         "InstanceGroups": NotRequired[Sequence[InstanceGroupTypeDef]],
     },
 )
+ParameterRangeOutputTypeDef = TypedDict(
+    "ParameterRangeOutputTypeDef",
+    {
+        "IntegerParameterRangeSpecification": NotRequired[
+            IntegerParameterRangeSpecificationTypeDef
+        ],
+        "ContinuousParameterRangeSpecification": NotRequired[
+            ContinuousParameterRangeSpecificationTypeDef
+        ],
+        "CategoricalParameterRangeSpecification": NotRequired[
+            CategoricalParameterRangeSpecificationOutputTypeDef
+        ],
+    },
+)
 ParameterRangeTypeDef = TypedDict(
     "ParameterRangeTypeDef",
     {
         "IntegerParameterRangeSpecification": NotRequired[
             IntegerParameterRangeSpecificationTypeDef
         ],
         "ContinuousParameterRangeSpecification": NotRequired[
             ContinuousParameterRangeSpecificationTypeDef
         ],
         "CategoricalParameterRangeSpecification": NotRequired[
             CategoricalParameterRangeSpecificationTypeDef
         ],
     },
 )
-ParameterRangesPaginatorTypeDef = TypedDict(
-    "ParameterRangesPaginatorTypeDef",
+ParameterRangesExtraOutputTypeDef = TypedDict(
+    "ParameterRangesExtraOutputTypeDef",
+    {
+        "IntegerParameterRanges": NotRequired[List[IntegerParameterRangeTypeDef]],
+        "ContinuousParameterRanges": NotRequired[List[ContinuousParameterRangeTypeDef]],
+        "CategoricalParameterRanges": NotRequired[
+            List[CategoricalParameterRangeExtraOutputTypeDef]
+        ],
+        "AutoParameters": NotRequired[List[AutoParameterTypeDef]],
+    },
+)
+ParameterRangesOutputTypeDef = TypedDict(
+    "ParameterRangesOutputTypeDef",
     {
         "IntegerParameterRanges": NotRequired[List[IntegerParameterRangeTypeDef]],
         "ContinuousParameterRanges": NotRequired[List[ContinuousParameterRangeTypeDef]],
-        "CategoricalParameterRanges": NotRequired[List[CategoricalParameterRangePaginatorTypeDef]],
+        "CategoricalParameterRanges": NotRequired[List[CategoricalParameterRangeOutputTypeDef]],
         "AutoParameters": NotRequired[List[AutoParameterTypeDef]],
     },
 )
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "IntegerParameterRanges": NotRequired[Sequence[IntegerParameterRangeTypeDef]],
         "ContinuousParameterRanges": NotRequired[Sequence[ContinuousParameterRangeTypeDef]],
         "CategoricalParameterRanges": NotRequired[Sequence[CategoricalParameterRangeTypeDef]],
         "AutoParameters": NotRequired[Sequence[AutoParameterTypeDef]],
     },
 )
-KernelGatewayImageConfigPaginatorTypeDef = TypedDict(
-    "KernelGatewayImageConfigPaginatorTypeDef",
+KernelGatewayImageConfigExtraOutputTypeDef = TypedDict(
+    "KernelGatewayImageConfigExtraOutputTypeDef",
+    {
+        "KernelSpecs": List[KernelSpecTypeDef],
+        "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
+    },
+)
+KernelGatewayImageConfigOutputTypeDef = TypedDict(
+    "KernelGatewayImageConfigOutputTypeDef",
     {
         "KernelSpecs": List[KernelSpecTypeDef],
         "FileSystemConfig": NotRequired[FileSystemConfigTypeDef],
     },
 )
 KernelGatewayImageConfigTypeDef = TypedDict(
     "KernelGatewayImageConfigTypeDef",
@@ -9047,16 +9744,16 @@
         "SnsDataSource": NotRequired[LabelingJobSnsDataSourceTypeDef],
     },
 )
 ListLineageGroupsResponseTypeDef = TypedDict(
     "ListLineageGroupsResponseTypeDef",
     {
         "LineageGroupSummaries": List[LineageGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListActionsRequestListActionsPaginateTypeDef = TypedDict(
     "ListActionsRequestListActionsPaginateTypeDef",
     {
         "SourceUri": NotRequired[str],
         "ActionType": NotRequired[str],
@@ -9889,207 +10586,214 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListDataQualityJobDefinitionsResponseTypeDef = TypedDict(
     "ListDataQualityJobDefinitionsResponseTypeDef",
     {
         "JobDefinitionSummaries": List[MonitoringJobDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelBiasJobDefinitionsResponseTypeDef = TypedDict(
     "ListModelBiasJobDefinitionsResponseTypeDef",
     {
         "JobDefinitionSummaries": List[MonitoringJobDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelExplainabilityJobDefinitionsResponseTypeDef = TypedDict(
     "ListModelExplainabilityJobDefinitionsResponseTypeDef",
     {
         "JobDefinitionSummaries": List[MonitoringJobDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelQualityJobDefinitionsResponseTypeDef = TypedDict(
     "ListModelQualityJobDefinitionsResponseTypeDef",
     {
         "JobDefinitionSummaries": List[MonitoringJobDefinitionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelCardExportJobsResponseTypeDef = TypedDict(
     "ListModelCardExportJobsResponseTypeDef",
     {
         "ModelCardExportJobSummaries": List[ModelCardExportJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelCardVersionsResponseTypeDef = TypedDict(
     "ListModelCardVersionsResponseTypeDef",
     {
         "ModelCardVersionSummaryList": List[ModelCardVersionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelCardsResponseTypeDef = TypedDict(
     "ListModelCardsResponseTypeDef",
     {
         "ModelCardSummaries": List[ModelCardSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelMetadataResponseTypeDef = TypedDict(
     "ListModelMetadataResponseTypeDef",
     {
         "ModelMetadataSummaries": List[ModelMetadataSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelPackageGroupsOutputTypeDef = TypedDict(
     "ListModelPackageGroupsOutputTypeDef",
     {
         "ModelPackageGroupSummaryList": List[ModelPackageGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelPackagesOutputTypeDef = TypedDict(
     "ListModelPackagesOutputTypeDef",
     {
         "ModelPackageSummaryList": List[ModelPackageSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListModelsOutputTypeDef = TypedDict(
     "ListModelsOutputTypeDef",
     {
         "Models": List[ModelSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMonitoringAlertHistoryResponseTypeDef = TypedDict(
     "ListMonitoringAlertHistoryResponseTypeDef",
     {
         "MonitoringAlertHistory": List[MonitoringAlertHistorySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMonitoringSchedulesResponseTypeDef = TypedDict(
     "ListMonitoringSchedulesResponseTypeDef",
     {
         "MonitoringScheduleSummaries": List[MonitoringScheduleSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListNotebookInstanceLifecycleConfigsOutputTypeDef = TypedDict(
     "ListNotebookInstanceLifecycleConfigsOutputTypeDef",
     {
-        "NextToken": str,
         "NotebookInstanceLifecycleConfigs": List[NotebookInstanceLifecycleConfigSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListNotebookInstancesOutputTypeDef = TypedDict(
     "ListNotebookInstancesOutputTypeDef",
     {
-        "NextToken": str,
         "NotebookInstances": List[NotebookInstanceSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPipelineExecutionsResponseTypeDef = TypedDict(
     "ListPipelineExecutionsResponseTypeDef",
     {
         "PipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPipelineParametersForExecutionResponseTypeDef = TypedDict(
     "ListPipelineParametersForExecutionResponseTypeDef",
     {
         "PipelineParameters": List[ParameterTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "PipelineSummaries": List[PipelineSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProcessingJobsResponseTypeDef = TypedDict(
     "ListProcessingJobsResponseTypeDef",
     {
         "ProcessingJobSummaries": List[ProcessingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProjectsOutputTypeDef = TypedDict(
     "ListProjectsOutputTypeDef",
     {
         "ProjectSummaryList": List[ProjectSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListResourceCatalogsResponseTypeDef = TypedDict(
     "ListResourceCatalogsResponseTypeDef",
     {
         "ResourceCatalogs": List[ResourceCatalogTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListStudioLifecycleConfigsResponseTypeDef = TypedDict(
     "ListStudioLifecycleConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "StudioLifecycleConfigs": List[StudioLifecycleConfigDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTransformJobsResponseTypeDef = TypedDict(
     "ListTransformJobsResponseTypeDef",
     {
         "TransformJobSummaries": List[TransformJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUserProfilesResponseTypeDef = TypedDict(
     "ListUserProfilesResponseTypeDef",
     {
         "UserProfiles": List[UserProfileDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+MemberDefinitionExtraOutputTypeDef = TypedDict(
+    "MemberDefinitionExtraOutputTypeDef",
+    {
+        "CognitoMemberDefinition": NotRequired[CognitoMemberDefinitionTypeDef],
+        "OidcMemberDefinition": NotRequired[OidcMemberDefinitionExtraOutputTypeDef],
     },
 )
-MemberDefinitionPaginatorTypeDef = TypedDict(
-    "MemberDefinitionPaginatorTypeDef",
+MemberDefinitionOutputTypeDef = TypedDict(
+    "MemberDefinitionOutputTypeDef",
     {
         "CognitoMemberDefinition": NotRequired[CognitoMemberDefinitionTypeDef],
-        "OidcMemberDefinition": NotRequired[OidcMemberDefinitionPaginatorTypeDef],
+        "OidcMemberDefinition": NotRequired[OidcMemberDefinitionOutputTypeDef],
     },
 )
 MemberDefinitionTypeDef = TypedDict(
     "MemberDefinitionTypeDef",
     {
         "CognitoMemberDefinition": NotRequired[CognitoMemberDefinitionTypeDef],
         "OidcMemberDefinition": NotRequired[OidcMemberDefinitionTypeDef],
@@ -10107,14 +10811,23 @@
     {
         "S3Uri": str,
         "S3DataType": S3ModelDataTypeType,
         "CompressionType": ModelCompressionTypeType,
         "ModelAccessConfig": NotRequired[ModelAccessConfigTypeDef],
     },
 )
+TextGenerationJobConfigOutputTypeDef = TypedDict(
+    "TextGenerationJobConfigOutputTypeDef",
+    {
+        "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
+        "BaseModelName": NotRequired[str],
+        "TextGenerationHyperParameters": NotRequired[Dict[str, str]],
+        "ModelAccessConfig": NotRequired[ModelAccessConfigTypeDef],
+    },
+)
 TextGenerationJobConfigTypeDef = TypedDict(
     "TextGenerationJobConfigTypeDef",
     {
         "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
         "BaseModelName": NotRequired[str],
         "TextGenerationHyperParameters": NotRequired[Mapping[str, str]],
         "ModelAccessConfig": NotRequired[ModelAccessConfigTypeDef],
@@ -10129,14 +10842,22 @@
 ModelInfrastructureConfigTypeDef = TypedDict(
     "ModelInfrastructureConfigTypeDef",
     {
         "InfrastructureType": Literal["RealTimeInference"],
         "RealTimeInferenceConfig": RealTimeInferenceConfigTypeDef,
     },
 )
+RecommendationJobStoppingConditionsOutputTypeDef = TypedDict(
+    "RecommendationJobStoppingConditionsOutputTypeDef",
+    {
+        "MaxInvocations": NotRequired[int],
+        "ModelLatencyThresholds": NotRequired[List[ModelLatencyThresholdTypeDef]],
+        "FlatInvocations": NotRequired[FlatInvocationsType],
+    },
+)
 RecommendationJobStoppingConditionsTypeDef = TypedDict(
     "RecommendationJobStoppingConditionsTypeDef",
     {
         "MaxInvocations": NotRequired[int],
         "ModelLatencyThresholds": NotRequired[Sequence[ModelLatencyThresholdTypeDef]],
         "FlatInvocations": NotRequired[FlatInvocationsType],
     },
@@ -10156,16 +10877,24 @@
 )
 MonitoringResourcesTypeDef = TypedDict(
     "MonitoringResourcesTypeDef",
     {
         "ClusterConfig": MonitoringClusterConfigTypeDef,
     },
 )
-MonitoringDatasetFormatPaginatorTypeDef = TypedDict(
-    "MonitoringDatasetFormatPaginatorTypeDef",
+MonitoringDatasetFormatExtraOutputTypeDef = TypedDict(
+    "MonitoringDatasetFormatExtraOutputTypeDef",
+    {
+        "Csv": NotRequired[MonitoringCsvDatasetFormatTypeDef],
+        "Json": NotRequired[MonitoringJsonDatasetFormatTypeDef],
+        "Parquet": NotRequired[Dict[str, Any]],
+    },
+)
+MonitoringDatasetFormatOutputTypeDef = TypedDict(
+    "MonitoringDatasetFormatOutputTypeDef",
     {
         "Csv": NotRequired[MonitoringCsvDatasetFormatTypeDef],
         "Json": NotRequired[MonitoringJsonDatasetFormatTypeDef],
         "Parquet": NotRequired[Dict[str, Any]],
     },
 )
 MonitoringDatasetFormatTypeDef = TypedDict(
@@ -10280,22 +11009,35 @@
         "ModelDataDownloadTimeoutInSeconds": NotRequired[int],
         "ContainerStartupHealthCheckTimeoutInSeconds": NotRequired[int],
         "EnableSSMAccess": NotRequired[bool],
         "ManagedInstanceScaling": NotRequired[ProductionVariantManagedInstanceScalingTypeDef],
         "RoutingConfig": NotRequired[ProductionVariantRoutingConfigTypeDef],
     },
 )
+ProfilerConfigUnionTypeDef = Union[ProfilerConfigTypeDef, ProfilerConfigExtraOutputTypeDef]
+ProfilerRuleConfigurationUnionTypeDef = Union[
+    ProfilerRuleConfigurationTypeDef, ProfilerRuleConfigurationOutputTypeDef
+]
 SuggestionQueryTypeDef = TypedDict(
     "SuggestionQueryTypeDef",
     {
         "PropertyNameQuery": NotRequired[PropertyNameQueryTypeDef],
     },
 )
-ServiceCatalogProvisioningDetailsPaginatorTypeDef = TypedDict(
-    "ServiceCatalogProvisioningDetailsPaginatorTypeDef",
+ServiceCatalogProvisioningDetailsExtraOutputTypeDef = TypedDict(
+    "ServiceCatalogProvisioningDetailsExtraOutputTypeDef",
+    {
+        "ProductId": str,
+        "ProvisioningArtifactId": NotRequired[str],
+        "PathId": NotRequired[str],
+        "ProvisioningParameters": NotRequired[List[ProvisioningParameterTypeDef]],
+    },
+)
+ServiceCatalogProvisioningDetailsOutputTypeDef = TypedDict(
+    "ServiceCatalogProvisioningDetailsOutputTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": NotRequired[str],
         "PathId": NotRequired[str],
         "ProvisioningParameters": NotRequired[List[ProvisioningParameterTypeDef]],
     },
 )
@@ -10322,25 +11064,40 @@
     },
 )
 QueryLineageResponseTypeDef = TypedDict(
     "QueryLineageResponseTypeDef",
     {
         "Vertices": List[VertexTypeDef],
         "Edges": List[EdgeTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RecommendationJobOutputConfigTypeDef = TypedDict(
     "RecommendationJobOutputConfigTypeDef",
     {
         "KmsKeyId": NotRequired[str],
         "CompiledOutputConfig": NotRequired[RecommendationJobCompiledOutputConfigTypeDef],
     },
 )
+RecommendationJobContainerConfigOutputTypeDef = TypedDict(
+    "RecommendationJobContainerConfigOutputTypeDef",
+    {
+        "Domain": NotRequired[str],
+        "Task": NotRequired[str],
+        "Framework": NotRequired[str],
+        "FrameworkVersion": NotRequired[str],
+        "PayloadConfig": NotRequired[RecommendationJobPayloadConfigOutputTypeDef],
+        "NearestModelName": NotRequired[str],
+        "SupportedInstanceTypes": NotRequired[List[str]],
+        "SupportedEndpointType": NotRequired[RecommendationJobSupportedEndpointTypeType],
+        "DataInputConfig": NotRequired[str],
+        "SupportedResponseMIMETypes": NotRequired[List[str]],
+    },
+)
 RecommendationJobContainerConfigTypeDef = TypedDict(
     "RecommendationJobContainerConfigTypeDef",
     {
         "Domain": NotRequired[str],
         "Task": NotRequired[str],
         "Framework": NotRequired[str],
         "FrameworkVersion": NotRequired[str],
@@ -10365,59 +11122,92 @@
     "RenderUiTemplateResponseTypeDef",
     {
         "RenderedContent": str,
         "Errors": List[RenderingErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateTrainingJobRequestRequestTypeDef = TypedDict(
-    "UpdateTrainingJobRequestRequestTypeDef",
-    {
-        "TrainingJobName": str,
-        "ProfilerConfig": NotRequired[ProfilerConfigForUpdateTypeDef],
-        "ProfilerRuleConfigurations": NotRequired[Sequence[ProfilerRuleConfigurationTypeDef]],
-        "ResourceConfig": NotRequired[ResourceConfigForUpdateTypeDef],
-        "RemoteDebugConfig": NotRequired[RemoteDebugConfigForUpdateTypeDef],
-    },
-)
 SearchRequestRequestTypeDef = TypedDict(
     "SearchRequestRequestTypeDef",
     {
         "Resource": ResourceTypeType,
         "SearchExpression": NotRequired["SearchExpressionTypeDef"],
         "SortBy": NotRequired[str],
         "SortOrder": NotRequired[SearchSortOrderType],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
         "CrossAccountFilterOption": NotRequired[CrossAccountFilterOptionType],
         "VisibilityConditions": NotRequired[Sequence[VisibilityConditionsTypeDef]],
     },
 )
+SelectiveExecutionConfigExtraOutputTypeDef = TypedDict(
+    "SelectiveExecutionConfigExtraOutputTypeDef",
+    {
+        "SelectedSteps": List[SelectedStepTypeDef],
+        "SourcePipelineExecutionArn": NotRequired[str],
+    },
+)
+SelectiveExecutionConfigOutputTypeDef = TypedDict(
+    "SelectiveExecutionConfigOutputTypeDef",
+    {
+        "SelectedSteps": List[SelectedStepTypeDef],
+        "SourcePipelineExecutionArn": NotRequired[str],
+    },
+)
 SelectiveExecutionConfigTypeDef = TypedDict(
     "SelectiveExecutionConfigTypeDef",
     {
-        "SelectedSteps": List[SelectedStepTypeDef],
+        "SelectedSteps": Sequence[SelectedStepTypeDef],
         "SourcePipelineExecutionArn": NotRequired[str],
     },
 )
+ShadowModeConfigOutputTypeDef = TypedDict(
+    "ShadowModeConfigOutputTypeDef",
+    {
+        "SourceModelVariantName": str,
+        "ShadowModelVariants": List[ShadowModelVariantConfigTypeDef],
+    },
+)
 ShadowModeConfigTypeDef = TypedDict(
     "ShadowModeConfigTypeDef",
     {
         "SourceModelVariantName": str,
         "ShadowModelVariants": Sequence[ShadowModelVariantConfigTypeDef],
     },
 )
+SourceIpConfigUnionTypeDef = Union[SourceIpConfigTypeDef, SourceIpConfigExtraOutputTypeDef]
+TrafficPatternOutputTypeDef = TypedDict(
+    "TrafficPatternOutputTypeDef",
+    {
+        "TrafficType": NotRequired[TrafficTypeType],
+        "Phases": NotRequired[List[PhaseTypeDef]],
+        "Stairs": NotRequired[StairsTypeDef],
+    },
+)
 TrafficPatternTypeDef = TypedDict(
     "TrafficPatternTypeDef",
     {
         "TrafficType": NotRequired[TrafficTypeType],
         "Phases": NotRequired[Sequence[PhaseTypeDef]],
         "Stairs": NotRequired[StairsTypeDef],
     },
 )
+TimeSeriesForecastingJobConfigOutputTypeDef = TypedDict(
+    "TimeSeriesForecastingJobConfigOutputTypeDef",
+    {
+        "ForecastFrequency": str,
+        "ForecastHorizon": int,
+        "TimeSeriesConfig": TimeSeriesConfigOutputTypeDef,
+        "FeatureSpecificationS3Uri": NotRequired[str],
+        "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
+        "ForecastQuantiles": NotRequired[List[str]],
+        "Transformations": NotRequired[TimeSeriesTransformationsOutputTypeDef],
+        "HolidayConfig": NotRequired[List[HolidayConfigAttributesTypeDef]],
+    },
+)
 TimeSeriesForecastingJobConfigTypeDef = TypedDict(
     "TimeSeriesForecastingJobConfigTypeDef",
     {
         "ForecastFrequency": str,
         "ForecastHorizon": int,
         "TimeSeriesConfig": TimeSeriesConfigTypeDef,
         "FeatureSpecificationS3Uri": NotRequired[str],
@@ -10436,104 +11226,87 @@
 )
 TransformDataSourceTypeDef = TypedDict(
     "TransformDataSourceTypeDef",
     {
         "S3DataSource": TransformS3DataSourceTypeDef,
     },
 )
-WorkforcePaginatorTypeDef = TypedDict(
-    "WorkforcePaginatorTypeDef",
-    {
-        "WorkforceName": str,
-        "WorkforceArn": str,
-        "LastUpdatedDate": NotRequired[datetime],
-        "SourceIpConfig": NotRequired[SourceIpConfigPaginatorTypeDef],
-        "SubDomain": NotRequired[str],
-        "CognitoConfig": NotRequired[CognitoConfigTypeDef],
-        "OidcConfig": NotRequired[OidcConfigForResponseTypeDef],
-        "CreateDate": NotRequired[datetime],
-        "WorkforceVpcConfig": NotRequired[WorkforceVpcConfigResponseTypeDef],
-        "Status": NotRequired[WorkforceStatusType],
-        "FailureReason": NotRequired[str],
-    },
-)
 WorkforceTypeDef = TypedDict(
     "WorkforceTypeDef",
     {
         "WorkforceName": str,
         "WorkforceArn": str,
         "LastUpdatedDate": NotRequired[datetime],
-        "SourceIpConfig": NotRequired[SourceIpConfigTypeDef],
+        "SourceIpConfig": NotRequired[SourceIpConfigOutputTypeDef],
         "SubDomain": NotRequired[str],
         "CognitoConfig": NotRequired[CognitoConfigTypeDef],
         "OidcConfig": NotRequired[OidcConfigForResponseTypeDef],
         "CreateDate": NotRequired[datetime],
         "WorkforceVpcConfig": NotRequired[WorkforceVpcConfigResponseTypeDef],
         "Status": NotRequired[WorkforceStatusType],
         "FailureReason": NotRequired[str],
     },
 )
 ListActionsResponseTypeDef = TypedDict(
     "ListActionsResponseTypeDef",
     {
         "ActionSummaries": List[ActionSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "Apps": List[AppDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DomainSettingsForUpdateTypeDef = TypedDict(
     "DomainSettingsForUpdateTypeDef",
     {
         "RStudioServerProDomainSettingsForUpdate": NotRequired[
             RStudioServerProDomainSettingsForUpdateTypeDef
         ],
         "ExecutionRoleIdentityConfig": NotRequired[ExecutionRoleIdentityConfigType],
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "DockerSettings": NotRequired[DockerSettingsTypeDef],
     },
 )
+DomainSettingsOutputTypeDef = TypedDict(
+    "DomainSettingsOutputTypeDef",
+    {
+        "SecurityGroupIds": NotRequired[List[str]],
+        "RStudioServerProDomainSettings": NotRequired[RStudioServerProDomainSettingsTypeDef],
+        "ExecutionRoleIdentityConfig": NotRequired[ExecutionRoleIdentityConfigType],
+        "DockerSettings": NotRequired[DockerSettingsOutputTypeDef],
+    },
+)
 DomainSettingsTypeDef = TypedDict(
     "DomainSettingsTypeDef",
     {
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "RStudioServerProDomainSettings": NotRequired[RStudioServerProDomainSettingsTypeDef],
         "ExecutionRoleIdentityConfig": NotRequired[ExecutionRoleIdentityConfigType],
         "DockerSettings": NotRequired[DockerSettingsTypeDef],
     },
 )
-ArtifactSummaryPaginatorTypeDef = TypedDict(
-    "ArtifactSummaryPaginatorTypeDef",
-    {
-        "ArtifactArn": NotRequired[str],
-        "ArtifactName": NotRequired[str],
-        "Source": NotRequired[ArtifactSourcePaginatorTypeDef],
-        "ArtifactType": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-    },
-)
 ArtifactSummaryTypeDef = TypedDict(
     "ArtifactSummaryTypeDef",
     {
         "ArtifactArn": NotRequired[str],
         "ArtifactName": NotRequired[str],
-        "Source": NotRequired[ArtifactSourceTypeDef],
+        "Source": NotRequired[ArtifactSourceOutputTypeDef],
         "ArtifactType": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
     },
 )
+ArtifactSourceUnionTypeDef = Union[ArtifactSourceTypeDef, ArtifactSourceExtraOutputTypeDef]
 CreateArtifactRequestRequestTypeDef = TypedDict(
     "CreateArtifactRequestRequestTypeDef",
     {
         "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
         "ArtifactName": NotRequired[str],
         "Properties": NotRequired[Mapping[str, str]],
@@ -10544,21 +11317,41 @@
 DeleteArtifactRequestRequestTypeDef = TypedDict(
     "DeleteArtifactRequestRequestTypeDef",
     {
         "ArtifactArn": NotRequired[str],
         "Source": NotRequired[ArtifactSourceTypeDef],
     },
 )
+AsyncInferenceConfigOutputTypeDef = TypedDict(
+    "AsyncInferenceConfigOutputTypeDef",
+    {
+        "OutputConfig": AsyncInferenceOutputConfigOutputTypeDef,
+        "ClientConfig": NotRequired[AsyncInferenceClientConfigTypeDef],
+    },
+)
 AsyncInferenceConfigTypeDef = TypedDict(
     "AsyncInferenceConfigTypeDef",
     {
         "OutputConfig": AsyncInferenceOutputConfigTypeDef,
         "ClientConfig": NotRequired[AsyncInferenceClientConfigTypeDef],
     },
 )
+TabularJobConfigOutputTypeDef = TypedDict(
+    "TabularJobConfigOutputTypeDef",
+    {
+        "TargetAttributeName": str,
+        "CandidateGenerationConfig": NotRequired[CandidateGenerationConfigOutputTypeDef],
+        "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
+        "FeatureSpecificationS3Uri": NotRequired[str],
+        "Mode": NotRequired[AutoMLModeType],
+        "GenerateCandidateDefinitionsOnly": NotRequired[bool],
+        "ProblemType": NotRequired[ProblemTypeType],
+        "SampleWeightAttributeName": NotRequired[str],
+    },
+)
 TabularJobConfigTypeDef = TypedDict(
     "TabularJobConfigTypeDef",
     {
         "TargetAttributeName": str,
         "CandidateGenerationConfig": NotRequired[CandidateGenerationConfigTypeDef],
         "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
         "FeatureSpecificationS3Uri": NotRequired[str],
@@ -10588,46 +11381,70 @@
         "DataSource": NotRequired[AutoMLDataSourceTypeDef],
     },
 )
 ListAutoMLJobsResponseTypeDef = TypedDict(
     "ListAutoMLJobsResponseTypeDef",
     {
         "AutoMLJobSummaries": List[AutoMLJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AutoMLResolvedAttributesTypeDef = TypedDict(
     "AutoMLResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": NotRequired[AutoMLJobObjectiveTypeDef],
         "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
         "AutoMLProblemTypeResolvedAttributes": NotRequired[
             AutoMLProblemTypeResolvedAttributesTypeDef
         ],
     },
 )
+AutoMLJobConfigOutputTypeDef = TypedDict(
+    "AutoMLJobConfigOutputTypeDef",
+    {
+        "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
+        "SecurityConfig": NotRequired[AutoMLSecurityConfigOutputTypeDef],
+        "CandidateGenerationConfig": NotRequired[AutoMLCandidateGenerationConfigOutputTypeDef],
+        "DataSplitConfig": NotRequired[AutoMLDataSplitConfigTypeDef],
+        "Mode": NotRequired[AutoMLModeType],
+    },
+)
+LabelingJobAlgorithmsConfigOutputTypeDef = TypedDict(
+    "LabelingJobAlgorithmsConfigOutputTypeDef",
+    {
+        "LabelingJobAlgorithmSpecificationArn": str,
+        "InitialActiveLearningModelArn": NotRequired[str],
+        "LabelingJobResourceConfig": NotRequired[LabelingJobResourceConfigOutputTypeDef],
+    },
+)
 AutoMLJobConfigTypeDef = TypedDict(
     "AutoMLJobConfigTypeDef",
     {
         "CompletionCriteria": NotRequired[AutoMLJobCompletionCriteriaTypeDef],
         "SecurityConfig": NotRequired[AutoMLSecurityConfigTypeDef],
         "CandidateGenerationConfig": NotRequired[AutoMLCandidateGenerationConfigTypeDef],
         "DataSplitConfig": NotRequired[AutoMLDataSplitConfigTypeDef],
         "Mode": NotRequired[AutoMLModeType],
     },
 )
+AutoMLSecurityConfigUnionTypeDef = Union[
+    AutoMLSecurityConfigTypeDef, AutoMLSecurityConfigOutputTypeDef
+]
 LabelingJobAlgorithmsConfigTypeDef = TypedDict(
     "LabelingJobAlgorithmsConfigTypeDef",
     {
         "LabelingJobAlgorithmSpecificationArn": str,
         "InitialActiveLearningModelArn": NotRequired[str],
         "LabelingJobResourceConfig": NotRequired[LabelingJobResourceConfigTypeDef],
     },
 )
+MonitoringNetworkConfigUnionTypeDef = Union[
+    MonitoringNetworkConfigTypeDef, MonitoringNetworkConfigOutputTypeDef
+]
 ModelMetricsTypeDef = TypedDict(
     "ModelMetricsTypeDef",
     {
         "ModelQuality": NotRequired[ModelQualityTypeDef],
         "ModelDataQuality": NotRequired[ModelDataQualityTypeDef],
         "Bias": NotRequired[BiasTypeDef],
         "Explainability": NotRequired[ExplainabilityTypeDef],
@@ -10675,23 +11492,44 @@
     "BlueGreenUpdatePolicyTypeDef",
     {
         "TrafficRoutingConfiguration": TrafficRoutingConfigTypeDef,
         "TerminationWaitInSeconds": NotRequired[int],
         "MaximumExecutionTimeoutInSeconds": NotRequired[int],
     },
 )
+InferenceExperimentDataStorageConfigUnionTypeDef = Union[
+    InferenceExperimentDataStorageConfigTypeDef, InferenceExperimentDataStorageConfigOutputTypeDef
+]
+DataCaptureConfigUnionTypeDef = Union[DataCaptureConfigTypeDef, DataCaptureConfigOutputTypeDef]
+EndpointInputConfigurationOutputTypeDef = TypedDict(
+    "EndpointInputConfigurationOutputTypeDef",
+    {
+        "InstanceType": NotRequired[ProductionVariantInstanceTypeType],
+        "ServerlessConfig": NotRequired[ProductionVariantServerlessConfigTypeDef],
+        "InferenceSpecificationName": NotRequired[str],
+        "EnvironmentParameterRanges": NotRequired[EnvironmentParameterRangesOutputTypeDef],
+    },
+)
 EndpointInputConfigurationTypeDef = TypedDict(
     "EndpointInputConfigurationTypeDef",
     {
         "InstanceType": NotRequired[ProductionVariantInstanceTypeType],
         "ServerlessConfig": NotRequired[ProductionVariantServerlessConfigTypeDef],
         "InferenceSpecificationName": NotRequired[str],
         "EnvironmentParameterRanges": NotRequired[EnvironmentParameterRangesTypeDef],
     },
 )
+ClarifyExplainerConfigOutputTypeDef = TypedDict(
+    "ClarifyExplainerConfigOutputTypeDef",
+    {
+        "ShapConfig": ClarifyShapConfigTypeDef,
+        "EnableExplanations": NotRequired[str],
+        "InferenceConfig": NotRequired[ClarifyInferenceConfigOutputTypeDef],
+    },
+)
 ClarifyExplainerConfigTypeDef = TypedDict(
     "ClarifyExplainerConfigTypeDef",
     {
         "ShapConfig": ClarifyShapConfigTypeDef,
         "EnableExplanations": NotRequired[str],
         "InferenceConfig": NotRequired[ClarifyInferenceConfigTypeDef],
     },
@@ -10701,15 +11539,15 @@
     {
         "ClusterArn": str,
         "ClusterName": str,
         "ClusterStatus": ClusterStatusType,
         "CreationTime": datetime,
         "FailureMessage": str,
         "InstanceGroups": List[ClusterInstanceGroupDetailsTypeDef],
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateClusterRequestRequestTypeDef = TypedDict(
     "CreateClusterRequestRequestTypeDef",
     {
         "ClusterName": str,
@@ -10736,71 +11574,78 @@
     "ListClusterNodesResponseTypeDef",
     {
         "NextToken": str,
         "ClusterNodeSummaries": List[ClusterNodeSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CodeEditorAppImageConfigUnionTypeDef = Union[
+    CodeEditorAppImageConfigTypeDef, CodeEditorAppImageConfigExtraOutputTypeDef
+]
+JupyterLabAppImageConfigUnionTypeDef = Union[
+    JupyterLabAppImageConfigTypeDef, JupyterLabAppImageConfigExtraOutputTypeDef
+]
 ListCodeRepositoriesOutputTypeDef = TypedDict(
     "ListCodeRepositoriesOutputTypeDef",
     {
         "CodeRepositorySummaryList": List[CodeRepositorySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FeatureDefinitionTypeDef = TypedDict(
     "FeatureDefinitionTypeDef",
     {
         "FeatureName": str,
         "FeatureType": FeatureTypeType,
         "CollectionType": NotRequired[CollectionTypeType],
         "CollectionConfig": NotRequired[CollectionConfigTypeDef],
     },
 )
+DebugHookConfigUnionTypeDef = Union[DebugHookConfigTypeDef, DebugHookConfigExtraOutputTypeDef]
 ListContextsResponseTypeDef = TypedDict(
     "ListContextsResponseTypeDef",
     {
         "ContextSummaries": List[ContextSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-InferenceExperimentSummaryTypeDef = TypedDict(
-    "InferenceExperimentSummaryTypeDef",
-    {
-        "Name": str,
-        "Type": Literal["ShadowMode"],
-        "Status": InferenceExperimentStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "Schedule": NotRequired[InferenceExperimentScheduleTypeDef],
-        "StatusReason": NotRequired[str],
-        "Description": NotRequired[str],
-        "CompletionTime": NotRequired[datetime],
-        "RoleArn": NotRequired[str],
-    },
-)
+InferenceExperimentScheduleUnionTypeDef = Union[
+    InferenceExperimentScheduleTypeDef, InferenceExperimentScheduleExtraOutputTypeDef
+]
 QueryLineageRequestRequestTypeDef = TypedDict(
     "QueryLineageRequestRequestTypeDef",
     {
         "StartArns": NotRequired[Sequence[str]],
         "Direction": NotRequired[DirectionType],
         "IncludeEdges": NotRequired[bool],
         "Filters": NotRequired[QueryFiltersTypeDef],
         "MaxDepth": NotRequired[int],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-ChannelPaginatorTypeDef = TypedDict(
-    "ChannelPaginatorTypeDef",
+ChannelExtraOutputTypeDef = TypedDict(
+    "ChannelExtraOutputTypeDef",
+    {
+        "ChannelName": str,
+        "DataSource": DataSourceExtraOutputTypeDef,
+        "ContentType": NotRequired[str],
+        "CompressionType": NotRequired[CompressionTypeType],
+        "RecordWrapperType": NotRequired[RecordWrapperType],
+        "InputMode": NotRequired[TrainingInputModeType],
+        "ShuffleConfig": NotRequired[ShuffleConfigTypeDef],
+    },
+)
+ChannelOutputTypeDef = TypedDict(
+    "ChannelOutputTypeDef",
     {
         "ChannelName": str,
-        "DataSource": DataSourcePaginatorTypeDef,
+        "DataSource": DataSourceOutputTypeDef,
         "ContentType": NotRequired[str],
         "CompressionType": NotRequired[CompressionTypeType],
         "RecordWrapperType": NotRequired[RecordWrapperType],
         "InputMode": NotRequired[TrainingInputModeType],
         "ShuffleConfig": NotRequired[ShuffleConfigTypeDef],
     },
 )
@@ -10821,27 +11666,61 @@
     {
         "InputName": str,
         "AppManaged": NotRequired[bool],
         "S3Input": NotRequired[ProcessingS3InputTypeDef],
         "DatasetDefinition": NotRequired[DatasetDefinitionTypeDef],
     },
 )
+DefaultSpaceSettingsOutputTypeDef = TypedDict(
+    "DefaultSpaceSettingsOutputTypeDef",
+    {
+        "ExecutionRole": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsOutputTypeDef],
+        "KernelGatewayAppSettings": NotRequired[KernelGatewayAppSettingsOutputTypeDef],
+        "JupyterLabAppSettings": NotRequired[JupyterLabAppSettingsOutputTypeDef],
+        "SpaceStorageSettings": NotRequired[DefaultSpaceStorageSettingsTypeDef],
+        "CustomPosixUserConfig": NotRequired[CustomPosixUserConfigTypeDef],
+        "CustomFileSystemConfigs": NotRequired[List[CustomFileSystemConfigTypeDef]],
+    },
+)
 DefaultSpaceSettingsTypeDef = TypedDict(
     "DefaultSpaceSettingsTypeDef",
     {
         "ExecutionRole": NotRequired[str],
         "SecurityGroups": NotRequired[Sequence[str]],
         "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsTypeDef],
         "KernelGatewayAppSettings": NotRequired[KernelGatewayAppSettingsTypeDef],
         "JupyterLabAppSettings": NotRequired[JupyterLabAppSettingsTypeDef],
         "SpaceStorageSettings": NotRequired[DefaultSpaceStorageSettingsTypeDef],
         "CustomPosixUserConfig": NotRequired[CustomPosixUserConfigTypeDef],
         "CustomFileSystemConfigs": NotRequired[Sequence[CustomFileSystemConfigTypeDef]],
     },
 )
+UserSettingsOutputTypeDef = TypedDict(
+    "UserSettingsOutputTypeDef",
+    {
+        "ExecutionRole": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "SharingSettings": NotRequired[SharingSettingsTypeDef],
+        "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsOutputTypeDef],
+        "KernelGatewayAppSettings": NotRequired[KernelGatewayAppSettingsOutputTypeDef],
+        "TensorBoardAppSettings": NotRequired[TensorBoardAppSettingsTypeDef],
+        "RStudioServerProAppSettings": NotRequired[RStudioServerProAppSettingsTypeDef],
+        "RSessionAppSettings": NotRequired[RSessionAppSettingsOutputTypeDef],
+        "CanvasAppSettings": NotRequired[CanvasAppSettingsOutputTypeDef],
+        "CodeEditorAppSettings": NotRequired[CodeEditorAppSettingsOutputTypeDef],
+        "JupyterLabAppSettings": NotRequired[JupyterLabAppSettingsOutputTypeDef],
+        "SpaceStorageSettings": NotRequired[DefaultSpaceStorageSettingsTypeDef],
+        "DefaultLandingUri": NotRequired[str],
+        "StudioWebPortal": NotRequired[StudioWebPortalType],
+        "CustomPosixUserConfig": NotRequired[CustomPosixUserConfigTypeDef],
+        "CustomFileSystemConfigs": NotRequired[List[CustomFileSystemConfigTypeDef]],
+    },
+)
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "ExecutionRole": NotRequired[str],
         "SecurityGroups": NotRequired[Sequence[str]],
         "SharingSettings": NotRequired[SharingSettingsTypeDef],
         "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsTypeDef],
@@ -10866,14 +11745,31 @@
         "Container": NotRequired[InferenceComponentContainerSpecificationSummaryTypeDef],
         "StartupParameters": NotRequired[InferenceComponentStartupParametersTypeDef],
         "ComputeResourceRequirements": NotRequired[
             InferenceComponentComputeResourceRequirementsTypeDef
         ],
     },
 )
+DescribeEdgeDeploymentPlanResponseTypeDef = TypedDict(
+    "DescribeEdgeDeploymentPlanResponseTypeDef",
+    {
+        "EdgeDeploymentPlanArn": str,
+        "EdgeDeploymentPlanName": str,
+        "ModelConfigs": List[EdgeDeploymentModelConfigTypeDef],
+        "DeviceFleetName": str,
+        "EdgeDeploymentSuccess": int,
+        "EdgeDeploymentPending": int,
+        "EdgeDeploymentFailed": int,
+        "Stages": List[DeploymentStageStatusSummaryTypeDef],
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
 CreateEdgeDeploymentPlanRequestRequestTypeDef = TypedDict(
     "CreateEdgeDeploymentPlanRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "ModelConfigs": Sequence[EdgeDeploymentModelConfigTypeDef],
         "DeviceFleetName": str,
         "Stages": NotRequired[Sequence[DeploymentStageTypeDef]],
@@ -10883,87 +11779,90 @@
 CreateEdgeDeploymentStageRequestRequestTypeDef = TypedDict(
     "CreateEdgeDeploymentStageRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "Stages": Sequence[DeploymentStageTypeDef],
     },
 )
-DescribeEdgeDeploymentPlanResponseTypeDef = TypedDict(
-    "DescribeEdgeDeploymentPlanResponseTypeDef",
-    {
-        "EdgeDeploymentPlanArn": str,
-        "EdgeDeploymentPlanName": str,
-        "ModelConfigs": List[EdgeDeploymentModelConfigTypeDef],
-        "DeviceFleetName": str,
-        "EdgeDeploymentSuccess": int,
-        "EdgeDeploymentPending": int,
-        "EdgeDeploymentFailed": int,
-        "Stages": List[DeploymentStageStatusSummaryTypeDef],
-        "NextToken": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "ExperimentSummaries": List[ExperimentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListFeatureGroupsResponseTypeDef = TypedDict(
     "ListFeatureGroupsResponseTypeDef",
     {
         "FeatureGroupSummaries": List[FeatureGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+ListInferenceExperimentsResponseTypeDef = TypedDict(
+    "ListInferenceExperimentsResponseTypeDef",
+    {
+        "InferenceExperiments": List[InferenceExperimentSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTrainingJobsResponseTypeDef = TypedDict(
     "ListTrainingJobsResponseTypeDef",
     {
         "TrainingJobSummaries": List[TrainingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTrialsResponseTypeDef = TypedDict(
     "ListTrialsResponseTypeDef",
     {
         "TrialSummaries": List[TrialSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef = TypedDict(
     "UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef",
     {
         "EndpointName": str,
         "DesiredWeightsAndCapacities": Sequence[DesiredWeightAndCapacityTypeDef],
     },
 )
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "DeviceSummaries": List[DeviceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DriftCheckBaselinesTypeDef = TypedDict(
     "DriftCheckBaselinesTypeDef",
     {
         "Bias": NotRequired[DriftCheckBiasTypeDef],
         "Explainability": NotRequired[DriftCheckExplainabilityTypeDef],
         "ModelQuality": NotRequired[DriftCheckModelQualityTypeDef],
         "ModelDataQuality": NotRequired[DriftCheckModelDataQualityTypeDef],
     },
 )
+SpaceSettingsOutputTypeDef = TypedDict(
+    "SpaceSettingsOutputTypeDef",
+    {
+        "JupyterServerAppSettings": NotRequired[JupyterServerAppSettingsOutputTypeDef],
+        "KernelGatewayAppSettings": NotRequired[KernelGatewayAppSettingsOutputTypeDef],
+        "CodeEditorAppSettings": NotRequired[SpaceCodeEditorAppSettingsTypeDef],
+        "JupyterLabAppSettings": NotRequired[SpaceJupyterLabAppSettingsOutputTypeDef],
+        "AppType": NotRequired[AppTypeType],
+        "SpaceStorageSettings": NotRequired[SpaceStorageSettingsTypeDef],
+        "CustomFileSystems": NotRequired[List[CustomFileSystemTypeDef]],
+    },
+)
 SpaceSettingsSummaryTypeDef = TypedDict(
     "SpaceSettingsSummaryTypeDef",
     {
         "AppType": NotRequired[AppTypeType],
         "SpaceStorageSettings": NotRequired[SpaceStorageSettingsTypeDef],
     },
 )
@@ -11011,26 +11910,31 @@
         "Operator": NotRequired[BooleanOperatorType],
     },
 )
 ListTrainingJobsForHyperParameterTuningJobResponseTypeDef = TypedDict(
     "ListTrainingJobsForHyperParameterTuningJobResponseTypeDef",
     {
         "TrainingJobSummaries": List[HyperParameterTrainingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+NetworkConfigUnionTypeDef = Union[NetworkConfigTypeDef, NetworkConfigExtraOutputTypeDef]
 ListHyperParameterTuningJobsResponseTypeDef = TypedDict(
     "ListHyperParameterTuningJobsResponseTypeDef",
     {
         "HyperParameterTuningJobSummaries": List[HyperParameterTuningJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+HyperParameterTuningJobWarmStartConfigUnionTypeDef = Union[
+    HyperParameterTuningJobWarmStartConfigTypeDef,
+    HyperParameterTuningJobWarmStartConfigExtraOutputTypeDef,
+]
 AssociationSummaryTypeDef = TypedDict(
     "AssociationSummaryTypeDef",
     {
         "SourceArn": NotRequired[str],
         "DestinationArn": NotRequired[str],
         "SourceType": NotRequired[str],
         "DestinationType": NotRequired[str],
@@ -11061,15 +11965,15 @@
     },
 )
 DescribeArtifactResponseTypeDef = TypedDict(
     "DescribeArtifactResponseTypeDef",
     {
         "ArtifactName": str,
         "ArtifactArn": str,
-        "Source": ArtifactSourceTypeDef,
+        "Source": ArtifactSourceOutputTypeDef,
         "ArtifactType": str,
         "Properties": Dict[str, str],
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
@@ -11333,42 +12237,60 @@
     "UpdateInferenceComponentInputRequestTypeDef",
     {
         "InferenceComponentName": str,
         "Specification": NotRequired[InferenceComponentSpecificationTypeDef],
         "RuntimeConfig": NotRequired[InferenceComponentRuntimeConfigTypeDef],
     },
 )
-ListInferenceExperimentsResponsePaginatorTypeDef = TypedDict(
-    "ListInferenceExperimentsResponsePaginatorTypeDef",
+ResourceConfigUnionTypeDef = Union[ResourceConfigTypeDef, ResourceConfigExtraOutputTypeDef]
+HyperParameterSpecificationOutputTypeDef = TypedDict(
+    "HyperParameterSpecificationOutputTypeDef",
     {
-        "InferenceExperiments": List[InferenceExperimentSummaryPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "Type": ParameterTypeType,
+        "Description": NotRequired[str],
+        "Range": NotRequired[ParameterRangeOutputTypeDef],
+        "IsTunable": NotRequired[bool],
+        "IsRequired": NotRequired[bool],
+        "DefaultValue": NotRequired[str],
     },
 )
 HyperParameterSpecificationTypeDef = TypedDict(
     "HyperParameterSpecificationTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Description": NotRequired[str],
         "Range": NotRequired[ParameterRangeTypeDef],
         "IsTunable": NotRequired[bool],
         "IsRequired": NotRequired[bool],
         "DefaultValue": NotRequired[str],
     },
 )
-HyperParameterTuningJobConfigPaginatorTypeDef = TypedDict(
-    "HyperParameterTuningJobConfigPaginatorTypeDef",
+HyperParameterTuningJobConfigExtraOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobConfigExtraOutputTypeDef",
+    {
+        "Strategy": HyperParameterTuningJobStrategyTypeType,
+        "ResourceLimits": ResourceLimitsTypeDef,
+        "StrategyConfig": NotRequired[HyperParameterTuningJobStrategyConfigTypeDef],
+        "HyperParameterTuningJobObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
+        "ParameterRanges": NotRequired[ParameterRangesExtraOutputTypeDef],
+        "TrainingJobEarlyStoppingType": NotRequired[TrainingJobEarlyStoppingTypeType],
+        "TuningJobCompletionCriteria": NotRequired[TuningJobCompletionCriteriaTypeDef],
+        "RandomSeed": NotRequired[int],
+    },
+)
+HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobConfigOutputTypeDef",
     {
         "Strategy": HyperParameterTuningJobStrategyTypeType,
         "ResourceLimits": ResourceLimitsTypeDef,
         "StrategyConfig": NotRequired[HyperParameterTuningJobStrategyConfigTypeDef],
         "HyperParameterTuningJobObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
-        "ParameterRanges": NotRequired[ParameterRangesPaginatorTypeDef],
+        "ParameterRanges": NotRequired[ParameterRangesOutputTypeDef],
         "TrainingJobEarlyStoppingType": NotRequired[TrainingJobEarlyStoppingTypeType],
         "TuningJobCompletionCriteria": NotRequired[TuningJobCompletionCriteriaTypeDef],
         "RandomSeed": NotRequired[int],
     },
 )
 HyperParameterTuningJobConfigTypeDef = TypedDict(
     "HyperParameterTuningJobConfigTypeDef",
@@ -11379,142 +12301,106 @@
         "HyperParameterTuningJobObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
         "ParameterRanges": NotRequired[ParameterRangesTypeDef],
         "TrainingJobEarlyStoppingType": NotRequired[TrainingJobEarlyStoppingTypeType],
         "TuningJobCompletionCriteria": NotRequired[TuningJobCompletionCriteriaTypeDef],
         "RandomSeed": NotRequired[int],
     },
 )
-AppImageConfigDetailsPaginatorTypeDef = TypedDict(
-    "AppImageConfigDetailsPaginatorTypeDef",
+AppImageConfigDetailsTypeDef = TypedDict(
+    "AppImageConfigDetailsTypeDef",
     {
         "AppImageConfigArn": NotRequired[str],
         "AppImageConfigName": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
-        "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigPaginatorTypeDef],
-        "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigPaginatorTypeDef],
-        "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigPaginatorTypeDef],
+        "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigOutputTypeDef],
+        "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigOutputTypeDef],
+        "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigOutputTypeDef],
     },
 )
-AppImageConfigDetailsTypeDef = TypedDict(
-    "AppImageConfigDetailsTypeDef",
+DescribeAppImageConfigResponseTypeDef = TypedDict(
+    "DescribeAppImageConfigResponseTypeDef",
     {
-        "AppImageConfigArn": NotRequired[str],
-        "AppImageConfigName": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigTypeDef],
-        "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigTypeDef],
-        "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigTypeDef],
+        "AppImageConfigArn": str,
+        "AppImageConfigName": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "KernelGatewayImageConfig": KernelGatewayImageConfigOutputTypeDef,
+        "JupyterLabAppImageConfig": JupyterLabAppImageConfigOutputTypeDef,
+        "CodeEditorAppImageConfig": CodeEditorAppImageConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateAppImageConfigRequestRequestTypeDef = TypedDict(
     "CreateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigTypeDef],
         "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigTypeDef],
         "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigTypeDef],
     },
 )
-DescribeAppImageConfigResponseTypeDef = TypedDict(
-    "DescribeAppImageConfigResponseTypeDef",
-    {
-        "AppImageConfigArn": str,
-        "AppImageConfigName": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "KernelGatewayImageConfig": KernelGatewayImageConfigTypeDef,
-        "JupyterLabAppImageConfig": JupyterLabAppImageConfigTypeDef,
-        "CodeEditorAppImageConfig": CodeEditorAppImageConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+KernelGatewayImageConfigUnionTypeDef = Union[
+    KernelGatewayImageConfigTypeDef, KernelGatewayImageConfigExtraOutputTypeDef
+]
 UpdateAppImageConfigRequestRequestTypeDef = TypedDict(
     "UpdateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
         "KernelGatewayImageConfig": NotRequired[KernelGatewayImageConfigTypeDef],
         "JupyterLabAppImageConfig": NotRequired[JupyterLabAppImageConfigTypeDef],
         "CodeEditorAppImageConfig": NotRequired[CodeEditorAppImageConfigTypeDef],
     },
 )
 ListLabelingJobsForWorkteamResponseTypeDef = TypedDict(
     "ListLabelingJobsForWorkteamResponseTypeDef",
     {
         "LabelingJobSummaryList": List[LabelingJobForWorkteamSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-LabelingJobInputConfigPaginatorTypeDef = TypedDict(
-    "LabelingJobInputConfigPaginatorTypeDef",
+LabelingJobInputConfigExtraOutputTypeDef = TypedDict(
+    "LabelingJobInputConfigExtraOutputTypeDef",
     {
         "DataSource": LabelingJobDataSourceTypeDef,
-        "DataAttributes": NotRequired[LabelingJobDataAttributesPaginatorTypeDef],
+        "DataAttributes": NotRequired[LabelingJobDataAttributesExtraOutputTypeDef],
     },
 )
-LabelingJobInputConfigTypeDef = TypedDict(
-    "LabelingJobInputConfigTypeDef",
+LabelingJobInputConfigOutputTypeDef = TypedDict(
+    "LabelingJobInputConfigOutputTypeDef",
     {
         "DataSource": LabelingJobDataSourceTypeDef,
-        "DataAttributes": NotRequired[LabelingJobDataAttributesTypeDef],
-    },
-)
-WorkteamPaginatorTypeDef = TypedDict(
-    "WorkteamPaginatorTypeDef",
-    {
-        "WorkteamName": str,
-        "MemberDefinitions": List[MemberDefinitionPaginatorTypeDef],
-        "WorkteamArn": str,
-        "Description": str,
-        "WorkforceArn": NotRequired[str],
-        "ProductListingIds": NotRequired[List[str]],
-        "SubDomain": NotRequired[str],
-        "CreateDate": NotRequired[datetime],
-        "LastUpdatedDate": NotRequired[datetime],
-        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
+        "DataAttributes": NotRequired[LabelingJobDataAttributesOutputTypeDef],
     },
 )
-CreateWorkteamRequestRequestTypeDef = TypedDict(
-    "CreateWorkteamRequestRequestTypeDef",
-    {
-        "WorkteamName": str,
-        "MemberDefinitions": Sequence[MemberDefinitionTypeDef],
-        "Description": str,
-        "WorkforceName": NotRequired[str],
-        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
-UpdateWorkteamRequestRequestTypeDef = TypedDict(
-    "UpdateWorkteamRequestRequestTypeDef",
+LabelingJobInputConfigTypeDef = TypedDict(
+    "LabelingJobInputConfigTypeDef",
     {
-        "WorkteamName": str,
-        "MemberDefinitions": NotRequired[Sequence[MemberDefinitionTypeDef]],
-        "Description": NotRequired[str],
-        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
+        "DataSource": LabelingJobDataSourceTypeDef,
+        "DataAttributes": NotRequired[LabelingJobDataAttributesTypeDef],
     },
 )
 WorkteamTypeDef = TypedDict(
     "WorkteamTypeDef",
     {
         "WorkteamName": str,
-        "MemberDefinitions": List[MemberDefinitionTypeDef],
+        "MemberDefinitions": List[MemberDefinitionOutputTypeDef],
         "WorkteamArn": str,
         "Description": str,
         "WorkforceArn": NotRequired[str],
         "ProductListingIds": NotRequired[List[str]],
         "SubDomain": NotRequired[str],
         "CreateDate": NotRequired[datetime],
         "LastUpdatedDate": NotRequired[datetime],
         "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
     },
 )
+MemberDefinitionUnionTypeDef = Union[MemberDefinitionTypeDef, MemberDefinitionExtraOutputTypeDef]
 TargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
     "TargetTrackingScalingPolicyConfigurationTypeDef",
     {
         "MetricSpecification": NotRequired[MetricSpecificationTypeDef],
         "TargetValue": NotRequired[float],
     },
 )
@@ -11549,14 +12435,17 @@
     "ModelVariantConfigTypeDef",
     {
         "ModelName": str,
         "VariantName": str,
         "InfrastructureConfig": ModelInfrastructureConfigTypeDef,
     },
 )
+RecommendationJobStoppingConditionsUnionTypeDef = Union[
+    RecommendationJobStoppingConditionsTypeDef, RecommendationJobStoppingConditionsOutputTypeDef
+]
 ListModelMetadataRequestListModelMetadataPaginateTypeDef = TypedDict(
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     {
         "SearchExpression": NotRequired[ModelMetadataSearchExpressionTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -11564,19 +12453,36 @@
     "ListModelMetadataRequestRequestTypeDef",
     {
         "SearchExpression": NotRequired[ModelMetadataSearchExpressionTypeDef],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
 )
-BatchTransformInputPaginatorTypeDef = TypedDict(
-    "BatchTransformInputPaginatorTypeDef",
+BatchTransformInputExtraOutputTypeDef = TypedDict(
+    "BatchTransformInputExtraOutputTypeDef",
+    {
+        "DataCapturedDestinationS3Uri": str,
+        "DatasetFormat": MonitoringDatasetFormatExtraOutputTypeDef,
+        "LocalPath": str,
+        "S3InputMode": NotRequired[ProcessingS3InputModeType],
+        "S3DataDistributionType": NotRequired[ProcessingS3DataDistributionTypeType],
+        "FeaturesAttribute": NotRequired[str],
+        "InferenceAttribute": NotRequired[str],
+        "ProbabilityAttribute": NotRequired[str],
+        "ProbabilityThresholdAttribute": NotRequired[float],
+        "StartTimeOffset": NotRequired[str],
+        "EndTimeOffset": NotRequired[str],
+        "ExcludeFeaturesAttribute": NotRequired[str],
+    },
+)
+BatchTransformInputOutputTypeDef = TypedDict(
+    "BatchTransformInputOutputTypeDef",
     {
         "DataCapturedDestinationS3Uri": str,
-        "DatasetFormat": MonitoringDatasetFormatPaginatorTypeDef,
+        "DatasetFormat": MonitoringDatasetFormatOutputTypeDef,
         "LocalPath": str,
         "S3InputMode": NotRequired[ProcessingS3InputModeType],
         "S3DataDistributionType": NotRequired[ProcessingS3DataDistributionTypeType],
         "FeaturesAttribute": NotRequired[str],
         "InferenceAttribute": NotRequired[str],
         "ProbabilityAttribute": NotRequired[str],
         "ProbabilityThresholdAttribute": NotRequired[float],
@@ -11598,16 +12504,23 @@
         "ProbabilityAttribute": NotRequired[str],
         "ProbabilityThresholdAttribute": NotRequired[float],
         "StartTimeOffset": NotRequired[str],
         "EndTimeOffset": NotRequired[str],
         "ExcludeFeaturesAttribute": NotRequired[str],
     },
 )
-MonitoringOutputConfigPaginatorTypeDef = TypedDict(
-    "MonitoringOutputConfigPaginatorTypeDef",
+MonitoringOutputConfigExtraOutputTypeDef = TypedDict(
+    "MonitoringOutputConfigExtraOutputTypeDef",
+    {
+        "MonitoringOutputs": List[MonitoringOutputTypeDef],
+        "KmsKeyId": NotRequired[str],
+    },
+)
+MonitoringOutputConfigOutputTypeDef = TypedDict(
+    "MonitoringOutputConfigOutputTypeDef",
     {
         "MonitoringOutputs": List[MonitoringOutputTypeDef],
         "KmsKeyId": NotRequired[str],
     },
 )
 MonitoringOutputConfigTypeDef = TypedDict(
     "MonitoringOutputConfigTypeDef",
@@ -11644,87 +12557,74 @@
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "ModelDigests": ModelDigestsTypeDef,
         "RoleArn": str,
         "InputConfig": InputConfigTypeDef,
         "OutputConfig": OutputConfigTypeDef,
-        "VpcConfig": NeoVpcConfigTypeDef,
+        "VpcConfig": NeoVpcConfigOutputTypeDef,
         "DerivedInformation": DerivedInformationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PendingDeploymentSummaryTypeDef = TypedDict(
     "PendingDeploymentSummaryTypeDef",
     {
         "EndpointConfigName": str,
         "ProductionVariants": NotRequired[List[PendingProductionVariantSummaryTypeDef]],
         "StartTime": NotRequired[datetime],
         "ShadowProductionVariants": NotRequired[List[PendingProductionVariantSummaryTypeDef]],
     },
 )
-ProcessingOutputConfigPaginatorTypeDef = TypedDict(
-    "ProcessingOutputConfigPaginatorTypeDef",
+ProcessingOutputConfigExtraOutputTypeDef = TypedDict(
+    "ProcessingOutputConfigExtraOutputTypeDef",
+    {
+        "Outputs": List[ProcessingOutputTypeDef],
+        "KmsKeyId": NotRequired[str],
+    },
+)
+ProcessingOutputConfigOutputTypeDef = TypedDict(
+    "ProcessingOutputConfigOutputTypeDef",
     {
         "Outputs": List[ProcessingOutputTypeDef],
         "KmsKeyId": NotRequired[str],
     },
 )
 ProcessingOutputConfigTypeDef = TypedDict(
     "ProcessingOutputConfigTypeDef",
     {
         "Outputs": Sequence[ProcessingOutputTypeDef],
         "KmsKeyId": NotRequired[str],
     },
 )
+UpdateTrainingJobRequestRequestTypeDef = TypedDict(
+    "UpdateTrainingJobRequestRequestTypeDef",
+    {
+        "TrainingJobName": str,
+        "ProfilerConfig": NotRequired[ProfilerConfigForUpdateTypeDef],
+        "ProfilerRuleConfigurations": NotRequired[Sequence[ProfilerRuleConfigurationUnionTypeDef]],
+        "ResourceConfig": NotRequired[ResourceConfigForUpdateTypeDef],
+        "RemoteDebugConfig": NotRequired[RemoteDebugConfigForUpdateTypeDef],
+    },
+)
 GetSearchSuggestionsRequestRequestTypeDef = TypedDict(
     "GetSearchSuggestionsRequestRequestTypeDef",
     {
         "Resource": ResourceTypeType,
         "SuggestionQuery": NotRequired[SuggestionQueryTypeDef],
     },
 )
-ProjectPaginatorTypeDef = TypedDict(
-    "ProjectPaginatorTypeDef",
-    {
-        "ProjectArn": NotRequired[str],
-        "ProjectName": NotRequired[str],
-        "ProjectId": NotRequired[str],
-        "ProjectDescription": NotRequired[str],
-        "ServiceCatalogProvisioningDetails": NotRequired[
-            ServiceCatalogProvisioningDetailsPaginatorTypeDef
-        ],
-        "ServiceCatalogProvisionedProductDetails": NotRequired[
-            ServiceCatalogProvisionedProductDetailsTypeDef
-        ],
-        "ProjectStatus": NotRequired[ProjectStatusType],
-        "CreatedBy": NotRequired[UserContextTypeDef],
-        "CreationTime": NotRequired[datetime],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "LastModifiedTime": NotRequired[datetime],
-        "LastModifiedBy": NotRequired[UserContextTypeDef],
-    },
-)
-CreateProjectInputRequestTypeDef = TypedDict(
-    "CreateProjectInputRequestTypeDef",
-    {
-        "ProjectName": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
-        "ProjectDescription": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 DescribeProjectOutputTypeDef = TypedDict(
     "DescribeProjectOutputTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "ProjectId": str,
         "ProjectDescription": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsOutputTypeDef,
         "ServiceCatalogProvisionedProductDetails": ServiceCatalogProvisionedProductDetailsTypeDef,
         "ProjectStatus": ProjectStatusType,
         "CreatedBy": UserContextTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11733,51 +12633,96 @@
 ProjectTypeDef = TypedDict(
     "ProjectTypeDef",
     {
         "ProjectArn": NotRequired[str],
         "ProjectName": NotRequired[str],
         "ProjectId": NotRequired[str],
         "ProjectDescription": NotRequired[str],
-        "ServiceCatalogProvisioningDetails": NotRequired[ServiceCatalogProvisioningDetailsTypeDef],
+        "ServiceCatalogProvisioningDetails": NotRequired[
+            ServiceCatalogProvisioningDetailsOutputTypeDef
+        ],
         "ServiceCatalogProvisionedProductDetails": NotRequired[
             ServiceCatalogProvisionedProductDetailsTypeDef
         ],
         "ProjectStatus": NotRequired[ProjectStatusType],
         "CreatedBy": NotRequired[UserContextTypeDef],
         "CreationTime": NotRequired[datetime],
         "Tags": NotRequired[List[TagTypeDef]],
         "LastModifiedTime": NotRequired[datetime],
         "LastModifiedBy": NotRequired[UserContextTypeDef],
     },
 )
+CreateProjectInputRequestTypeDef = TypedDict(
+    "CreateProjectInputRequestTypeDef",
+    {
+        "ProjectName": str,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
+        "ProjectDescription": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+ServiceCatalogProvisioningDetailsUnionTypeDef = Union[
+    ServiceCatalogProvisioningDetailsTypeDef, ServiceCatalogProvisioningDetailsExtraOutputTypeDef
+]
 UpdateProjectInputRequestTypeDef = TypedDict(
     "UpdateProjectInputRequestTypeDef",
     {
         "ProjectName": str,
         "ProjectDescription": NotRequired[str],
         "ServiceCatalogProvisioningUpdateDetails": NotRequired[
             ServiceCatalogProvisioningUpdateDetailsTypeDef
         ],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+HumanLoopConfigOutputTypeDef = TypedDict(
+    "HumanLoopConfigOutputTypeDef",
+    {
+        "WorkteamArn": str,
+        "HumanTaskUiArn": str,
+        "TaskTitle": str,
+        "TaskDescription": str,
+        "TaskCount": int,
+        "TaskAvailabilityLifetimeInSeconds": NotRequired[int],
+        "TaskTimeLimitInSeconds": NotRequired[int],
+        "TaskKeywords": NotRequired[List[str]],
+        "PublicWorkforceTaskPrice": NotRequired[PublicWorkforceTaskPriceTypeDef],
+    },
+)
 HumanLoopConfigTypeDef = TypedDict(
     "HumanLoopConfigTypeDef",
     {
         "WorkteamArn": str,
         "HumanTaskUiArn": str,
         "TaskTitle": str,
         "TaskDescription": str,
         "TaskCount": int,
         "TaskAvailabilityLifetimeInSeconds": NotRequired[int],
         "TaskTimeLimitInSeconds": NotRequired[int],
         "TaskKeywords": NotRequired[Sequence[str]],
         "PublicWorkforceTaskPrice": NotRequired[PublicWorkforceTaskPriceTypeDef],
     },
 )
+HumanTaskConfigOutputTypeDef = TypedDict(
+    "HumanTaskConfigOutputTypeDef",
+    {
+        "WorkteamArn": str,
+        "UiConfig": UiConfigTypeDef,
+        "PreHumanTaskLambdaArn": str,
+        "TaskTitle": str,
+        "TaskDescription": str,
+        "NumberOfHumanWorkersPerDataObject": int,
+        "TaskTimeLimitInSeconds": int,
+        "AnnotationConsolidationConfig": AnnotationConsolidationConfigTypeDef,
+        "TaskKeywords": NotRequired[List[str]],
+        "TaskAvailabilityLifetimeInSeconds": NotRequired[int],
+        "MaxConcurrentTaskCount": NotRequired[int],
+        "PublicWorkforceTaskPrice": NotRequired[PublicWorkforceTaskPriceTypeDef],
+    },
+)
 HumanTaskConfigTypeDef = TypedDict(
     "HumanTaskConfigTypeDef",
     {
         "WorkteamArn": str,
         "UiConfig": UiConfigTypeDef,
         "PreHumanTaskLambdaArn": str,
         "TaskTitle": str,
@@ -11802,15 +12747,15 @@
         "PipelineExperimentConfig": PipelineExperimentConfigTypeDef,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
-        "SelectiveExecutionConfig": SelectiveExecutionConfigTypeDef,
+        "SelectiveExecutionConfig": SelectiveExecutionConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PipelineExecutionTypeDef = TypedDict(
     "PipelineExecutionTypeDef",
     {
         "PipelineArn": NotRequired[str],
@@ -11821,32 +12766,49 @@
         "PipelineExperimentConfig": NotRequired[PipelineExperimentConfigTypeDef],
         "FailureReason": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
         "CreatedBy": NotRequired[UserContextTypeDef],
         "LastModifiedBy": NotRequired[UserContextTypeDef],
         "ParallelismConfiguration": NotRequired[ParallelismConfigurationTypeDef],
-        "SelectiveExecutionConfig": NotRequired[SelectiveExecutionConfigTypeDef],
+        "SelectiveExecutionConfig": NotRequired[SelectiveExecutionConfigOutputTypeDef],
         "PipelineParameters": NotRequired[List[ParameterTypeDef]],
     },
 )
+SelectiveExecutionConfigUnionTypeDef = Union[
+    SelectiveExecutionConfigTypeDef, SelectiveExecutionConfigExtraOutputTypeDef
+]
 StartPipelineExecutionRequestRequestTypeDef = TypedDict(
     "StartPipelineExecutionRequestRequestTypeDef",
     {
         "PipelineName": str,
         "ClientRequestToken": str,
         "PipelineExecutionDisplayName": NotRequired[str],
         "PipelineParameters": NotRequired[Sequence[ParameterTypeDef]],
         "PipelineExecutionDescription": NotRequired[str],
         "ParallelismConfiguration": NotRequired[ParallelismConfigurationTypeDef],
         "SelectiveExecutionConfig": NotRequired[SelectiveExecutionConfigTypeDef],
     },
 )
-AlgorithmSpecificationPaginatorTypeDef = TypedDict(
-    "AlgorithmSpecificationPaginatorTypeDef",
+ShadowModeConfigUnionTypeDef = Union[ShadowModeConfigTypeDef, ShadowModeConfigOutputTypeDef]
+AlgorithmSpecificationExtraOutputTypeDef = TypedDict(
+    "AlgorithmSpecificationExtraOutputTypeDef",
+    {
+        "TrainingInputMode": TrainingInputModeType,
+        "TrainingImage": NotRequired[str],
+        "AlgorithmName": NotRequired[str],
+        "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
+        "EnableSageMakerMetricsTimeSeries": NotRequired[bool],
+        "ContainerEntrypoint": NotRequired[List[str]],
+        "ContainerArguments": NotRequired[List[str]],
+        "TrainingImageConfig": NotRequired[TrainingImageConfigTypeDef],
+    },
+)
+AlgorithmSpecificationOutputTypeDef = TypedDict(
+    "AlgorithmSpecificationOutputTypeDef",
     {
         "TrainingInputMode": TrainingInputModeType,
         "TrainingImage": NotRequired[str],
         "AlgorithmName": NotRequired[str],
         "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
         "EnableSageMakerMetricsTimeSeries": NotRequired[bool],
         "ContainerEntrypoint": NotRequired[List[str]],
@@ -11872,70 +12834,69 @@
     {
         "DataSource": TransformDataSourceTypeDef,
         "ContentType": NotRequired[str],
         "CompressionType": NotRequired[CompressionTypeType],
         "SplitType": NotRequired[SplitTypeType],
     },
 )
-ListWorkforcesResponsePaginatorTypeDef = TypedDict(
-    "ListWorkforcesResponsePaginatorTypeDef",
-    {
-        "Workforces": List[WorkforcePaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeWorkforceResponseTypeDef = TypedDict(
     "DescribeWorkforceResponseTypeDef",
     {
         "Workforce": WorkforceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWorkforcesResponseTypeDef = TypedDict(
     "ListWorkforcesResponseTypeDef",
     {
         "Workforces": List[WorkforceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateWorkforceResponseTypeDef = TypedDict(
     "UpdateWorkforceResponseTypeDef",
     {
         "Workforce": WorkforceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListArtifactsResponsePaginatorTypeDef = TypedDict(
-    "ListArtifactsResponsePaginatorTypeDef",
-    {
-        "ArtifactSummaries": List[ArtifactSummaryPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+DomainSettingsUnionTypeDef = Union[DomainSettingsTypeDef, DomainSettingsOutputTypeDef]
 ListArtifactsResponseTypeDef = TypedDict(
     "ListArtifactsResponseTypeDef",
     {
         "ArtifactSummaries": List[ArtifactSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+AsyncInferenceConfigUnionTypeDef = Union[
+    AsyncInferenceConfigTypeDef, AsyncInferenceConfigOutputTypeDef
+]
+AutoMLProblemTypeConfigOutputTypeDef = TypedDict(
+    "AutoMLProblemTypeConfigOutputTypeDef",
+    {
+        "ImageClassificationJobConfig": NotRequired[ImageClassificationJobConfigTypeDef],
+        "TextClassificationJobConfig": NotRequired[TextClassificationJobConfigTypeDef],
+        "TimeSeriesForecastingJobConfig": NotRequired[TimeSeriesForecastingJobConfigOutputTypeDef],
+        "TabularJobConfig": NotRequired[TabularJobConfigOutputTypeDef],
+        "TextGenerationJobConfig": NotRequired[TextGenerationJobConfigOutputTypeDef],
     },
 )
 AutoMLProblemTypeConfigTypeDef = TypedDict(
     "AutoMLProblemTypeConfigTypeDef",
     {
         "ImageClassificationJobConfig": NotRequired[ImageClassificationJobConfigTypeDef],
         "TextClassificationJobConfig": NotRequired[TextClassificationJobConfigTypeDef],
         "TimeSeriesForecastingJobConfig": NotRequired[TimeSeriesForecastingJobConfigTypeDef],
         "TabularJobConfig": NotRequired[TabularJobConfigTypeDef],
         "TextGenerationJobConfig": NotRequired[TextGenerationJobConfigTypeDef],
     },
 )
+AutoMLJobConfigUnionTypeDef = Union[AutoMLJobConfigTypeDef, AutoMLJobConfigOutputTypeDef]
 CreateAutoMLJobRequestRequestTypeDef = TypedDict(
     "CreateAutoMLJobRequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "InputDataConfig": Sequence[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
@@ -11943,14 +12904,17 @@
         "AutoMLJobObjective": NotRequired[AutoMLJobObjectiveTypeDef],
         "AutoMLJobConfig": NotRequired[AutoMLJobConfigTypeDef],
         "GenerateCandidateDefinitionsOnly": NotRequired[bool],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "ModelDeployConfig": NotRequired[ModelDeployConfigTypeDef],
     },
 )
+LabelingJobAlgorithmsConfigUnionTypeDef = Union[
+    LabelingJobAlgorithmsConfigTypeDef, LabelingJobAlgorithmsConfigOutputTypeDef
+]
 PipelineExecutionStepTypeDef = TypedDict(
     "PipelineExecutionStepTypeDef",
     {
         "StepName": NotRequired[str],
         "StepDisplayName": NotRequired[str],
         "StepDescription": NotRequired[str],
         "StartTime": NotRequired[datetime],
@@ -11969,15 +12933,15 @@
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
         "InputDataConfig": List[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
-        "AutoMLJobConfig": AutoMLJobConfigTypeDef,
+        "AutoMLJobConfig": AutoMLJobConfigOutputTypeDef,
         "CreationTime": datetime,
         "EndTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
         "BestCandidate": AutoMLCandidateTypeDef,
         "AutoMLJobStatus": AutoMLJobStatusType,
@@ -11990,26 +12954,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCandidatesForAutoMLJobResponseTypeDef = TypedDict(
     "ListCandidatesForAutoMLJobResponseTypeDef",
     {
         "Candidates": List[AutoMLCandidateTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DeploymentConfigOutputTypeDef = TypedDict(
+    "DeploymentConfigOutputTypeDef",
+    {
+        "BlueGreenUpdatePolicy": NotRequired[BlueGreenUpdatePolicyTypeDef],
+        "RollingUpdatePolicy": NotRequired[RollingUpdatePolicyTypeDef],
+        "AutoRollbackConfiguration": NotRequired[AutoRollbackConfigOutputTypeDef],
     },
 )
 DeploymentConfigTypeDef = TypedDict(
     "DeploymentConfigTypeDef",
     {
         "BlueGreenUpdatePolicy": NotRequired[BlueGreenUpdatePolicyTypeDef],
         "RollingUpdatePolicy": NotRequired[RollingUpdatePolicyTypeDef],
         "AutoRollbackConfiguration": NotRequired[AutoRollbackConfigTypeDef],
     },
 )
+RecommendationJobInputConfigOutputTypeDef = TypedDict(
+    "RecommendationJobInputConfigOutputTypeDef",
+    {
+        "ModelPackageVersionArn": NotRequired[str],
+        "ModelName": NotRequired[str],
+        "JobDurationInSeconds": NotRequired[int],
+        "TrafficPattern": NotRequired[TrafficPatternOutputTypeDef],
+        "ResourceLimit": NotRequired[RecommendationJobResourceLimitTypeDef],
+        "EndpointConfigurations": NotRequired[List[EndpointInputConfigurationOutputTypeDef]],
+        "VolumeKmsKeyId": NotRequired[str],
+        "ContainerConfig": NotRequired[RecommendationJobContainerConfigOutputTypeDef],
+        "Endpoints": NotRequired[List[EndpointInfoTypeDef]],
+        "VpcConfig": NotRequired[RecommendationJobVpcConfigOutputTypeDef],
+    },
+)
 RecommendationJobInputConfigTypeDef = TypedDict(
     "RecommendationJobInputConfigTypeDef",
     {
         "ModelPackageVersionArn": NotRequired[str],
         "ModelName": NotRequired[str],
         "JobDurationInSeconds": NotRequired[int],
         "TrafficPattern": NotRequired[TrafficPatternTypeDef],
@@ -12017,14 +13004,20 @@
         "EndpointConfigurations": NotRequired[Sequence[EndpointInputConfigurationTypeDef]],
         "VolumeKmsKeyId": NotRequired[str],
         "ContainerConfig": NotRequired[RecommendationJobContainerConfigTypeDef],
         "Endpoints": NotRequired[Sequence[EndpointInfoTypeDef]],
         "VpcConfig": NotRequired[RecommendationJobVpcConfigTypeDef],
     },
 )
+ExplainerConfigOutputTypeDef = TypedDict(
+    "ExplainerConfigOutputTypeDef",
+    {
+        "ClarifyExplainerConfig": NotRequired[ClarifyExplainerConfigOutputTypeDef],
+    },
+)
 ExplainerConfigTypeDef = TypedDict(
     "ExplainerConfigTypeDef",
     {
         "ClarifyExplainerConfig": NotRequired[ClarifyExplainerConfigTypeDef],
     },
 )
 CreateFeatureGroupRequestRequestTypeDef = TypedDict(
@@ -12092,47 +13085,76 @@
     {
         "FeatureGroupName": str,
         "FeatureAdditions": NotRequired[Sequence[FeatureDefinitionTypeDef]],
         "OnlineStoreConfig": NotRequired[OnlineStoreConfigUpdateTypeDef],
         "ThroughputConfig": NotRequired[ThroughputConfigUpdateTypeDef],
     },
 )
-ListInferenceExperimentsResponseTypeDef = TypedDict(
-    "ListInferenceExperimentsResponseTypeDef",
+HyperParameterTrainingJobDefinitionExtraOutputTypeDef = TypedDict(
+    "HyperParameterTrainingJobDefinitionExtraOutputTypeDef",
     {
-        "InferenceExperiments": List[InferenceExperimentSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AlgorithmSpecification": HyperParameterAlgorithmSpecificationExtraOutputTypeDef,
+        "RoleArn": str,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "StoppingCondition": StoppingConditionTypeDef,
+        "DefinitionName": NotRequired[str],
+        "TuningObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
+        "HyperParameterRanges": NotRequired[ParameterRangesExtraOutputTypeDef],
+        "StaticHyperParameters": NotRequired[Dict[str, str]],
+        "InputDataConfig": NotRequired[List[ChannelExtraOutputTypeDef]],
+        "VpcConfig": NotRequired[VpcConfigExtraOutputTypeDef],
+        "ResourceConfig": NotRequired[ResourceConfigExtraOutputTypeDef],
+        "HyperParameterTuningResourceConfig": NotRequired[
+            HyperParameterTuningResourceConfigExtraOutputTypeDef
+        ],
+        "EnableNetworkIsolation": NotRequired[bool],
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "EnableManagedSpotTraining": NotRequired[bool],
+        "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
+        "RetryStrategy": NotRequired[RetryStrategyTypeDef],
+        "Environment": NotRequired[Dict[str, str]],
     },
 )
-HyperParameterTrainingJobDefinitionPaginatorTypeDef = TypedDict(
-    "HyperParameterTrainingJobDefinitionPaginatorTypeDef",
+HyperParameterTrainingJobDefinitionOutputTypeDef = TypedDict(
+    "HyperParameterTrainingJobDefinitionOutputTypeDef",
     {
-        "AlgorithmSpecification": HyperParameterAlgorithmSpecificationPaginatorTypeDef,
+        "AlgorithmSpecification": HyperParameterAlgorithmSpecificationOutputTypeDef,
         "RoleArn": str,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "DefinitionName": NotRequired[str],
         "TuningObjective": NotRequired[HyperParameterTuningJobObjectiveTypeDef],
-        "HyperParameterRanges": NotRequired[ParameterRangesPaginatorTypeDef],
+        "HyperParameterRanges": NotRequired[ParameterRangesOutputTypeDef],
         "StaticHyperParameters": NotRequired[Dict[str, str]],
-        "InputDataConfig": NotRequired[List[ChannelPaginatorTypeDef]],
-        "VpcConfig": NotRequired[VpcConfigPaginatorTypeDef],
-        "ResourceConfig": NotRequired[ResourceConfigPaginatorTypeDef],
+        "InputDataConfig": NotRequired[List[ChannelOutputTypeDef]],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
+        "ResourceConfig": NotRequired[ResourceConfigOutputTypeDef],
         "HyperParameterTuningResourceConfig": NotRequired[
-            HyperParameterTuningResourceConfigPaginatorTypeDef
+            HyperParameterTuningResourceConfigOutputTypeDef
         ],
         "EnableNetworkIsolation": NotRequired[bool],
         "EnableInterContainerTrafficEncryption": NotRequired[bool],
         "EnableManagedSpotTraining": NotRequired[bool],
         "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
         "RetryStrategy": NotRequired[RetryStrategyTypeDef],
         "Environment": NotRequired[Dict[str, str]],
     },
 )
+TrainingJobDefinitionOutputTypeDef = TypedDict(
+    "TrainingJobDefinitionOutputTypeDef",
+    {
+        "TrainingInputMode": TrainingInputModeType,
+        "InputDataConfig": List[ChannelOutputTypeDef],
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "ResourceConfig": ResourceConfigOutputTypeDef,
+        "StoppingCondition": StoppingConditionTypeDef,
+        "HyperParameters": NotRequired[Dict[str, str]],
+    },
+)
+ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelExtraOutputTypeDef]
 HyperParameterTrainingJobDefinitionTypeDef = TypedDict(
     "HyperParameterTrainingJobDefinitionTypeDef",
     {
         "AlgorithmSpecification": HyperParameterAlgorithmSpecificationTypeDef,
         "RoleArn": str,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
@@ -12161,42 +13183,17 @@
         "InputDataConfig": Sequence[ChannelTypeDef],
         "OutputDataConfig": OutputDataConfigTypeDef,
         "ResourceConfig": ResourceConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "HyperParameters": NotRequired[Mapping[str, str]],
     },
 )
-CreateDomainRequestRequestTypeDef = TypedDict(
-    "CreateDomainRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "AuthMode": AuthModeType,
-        "DefaultUserSettings": UserSettingsTypeDef,
-        "SubnetIds": Sequence[str],
-        "VpcId": str,
-        "DomainSettings": NotRequired[DomainSettingsTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "AppNetworkAccessType": NotRequired[AppNetworkAccessTypeType],
-        "HomeEfsFileSystemKmsKeyId": NotRequired[str],
-        "KmsKeyId": NotRequired[str],
-        "AppSecurityGroupManagement": NotRequired[AppSecurityGroupManagementType],
-        "DefaultSpaceSettings": NotRequired[DefaultSpaceSettingsTypeDef],
-    },
-)
-CreateUserProfileRequestRequestTypeDef = TypedDict(
-    "CreateUserProfileRequestRequestTypeDef",
-    {
-        "DomainId": str,
-        "UserProfileName": str,
-        "SingleSignOnUserIdentifier": NotRequired[str],
-        "SingleSignOnUserValue": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "UserSettings": NotRequired[UserSettingsTypeDef],
-    },
-)
+DefaultSpaceSettingsUnionTypeDef = Union[
+    DefaultSpaceSettingsTypeDef, DefaultSpaceSettingsOutputTypeDef
+]
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "DomainArn": str,
         "DomainId": str,
         "DomainName": str,
         "HomeEfsFileSystemId": str,
@@ -12204,24 +13201,24 @@
         "SingleSignOnApplicationArn": str,
         "Status": DomainStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "SecurityGroupIdForDomainBoundary": str,
         "AuthMode": AuthModeType,
-        "DefaultUserSettings": UserSettingsTypeDef,
-        "DomainSettings": DomainSettingsTypeDef,
+        "DefaultUserSettings": UserSettingsOutputTypeDef,
+        "DomainSettings": DomainSettingsOutputTypeDef,
         "AppNetworkAccessType": AppNetworkAccessTypeType,
         "HomeEfsFileSystemKmsKeyId": str,
         "SubnetIds": List[str],
         "Url": str,
         "VpcId": str,
         "KmsKeyId": str,
         "AppSecurityGroupManagement": AppSecurityGroupManagementType,
-        "DefaultSpaceSettings": DefaultSpaceSettingsTypeDef,
+        "DefaultSpaceSettings": DefaultSpaceSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeUserProfileResponseTypeDef = TypedDict(
     "DescribeUserProfileResponseTypeDef",
     {
         "DomainId": str,
@@ -12230,18 +13227,46 @@
         "HomeEfsFileSystemUid": str,
         "Status": UserProfileStatusType,
         "LastModifiedTime": datetime,
         "CreationTime": datetime,
         "FailureReason": str,
         "SingleSignOnUserIdentifier": str,
         "SingleSignOnUserValue": str,
-        "UserSettings": UserSettingsTypeDef,
+        "UserSettings": UserSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDomainRequestRequestTypeDef = TypedDict(
+    "CreateDomainRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "AuthMode": AuthModeType,
+        "DefaultUserSettings": UserSettingsTypeDef,
+        "SubnetIds": Sequence[str],
+        "VpcId": str,
+        "DomainSettings": NotRequired[DomainSettingsTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "AppNetworkAccessType": NotRequired[AppNetworkAccessTypeType],
+        "HomeEfsFileSystemKmsKeyId": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "AppSecurityGroupManagement": NotRequired[AppSecurityGroupManagementType],
+        "DefaultSpaceSettings": NotRequired[DefaultSpaceSettingsTypeDef],
+    },
+)
+CreateUserProfileRequestRequestTypeDef = TypedDict(
+    "CreateUserProfileRequestRequestTypeDef",
+    {
+        "DomainId": str,
+        "UserProfileName": str,
+        "SingleSignOnUserIdentifier": NotRequired[str],
+        "SingleSignOnUserValue": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "UserSettings": NotRequired[UserSettingsTypeDef],
+    },
+)
 UpdateDomainRequestRequestTypeDef = TypedDict(
     "UpdateDomainRequestRequestTypeDef",
     {
         "DomainId": str,
         "DefaultUserSettings": NotRequired[UserSettingsTypeDef],
         "DomainSettingsForUpdate": NotRequired[DomainSettingsForUpdateTypeDef],
         "AppSecurityGroupManagement": NotRequired[AppSecurityGroupManagementType],
@@ -12254,14 +13279,15 @@
     "UpdateUserProfileRequestRequestTypeDef",
     {
         "DomainId": str,
         "UserProfileName": str,
         "UserSettings": NotRequired[UserSettingsTypeDef],
     },
 )
+UserSettingsUnionTypeDef = Union[UserSettingsTypeDef, UserSettingsOutputTypeDef]
 DescribeInferenceComponentOutputTypeDef = TypedDict(
     "DescribeInferenceComponentOutputTypeDef",
     {
         "InferenceComponentName": str,
         "InferenceComponentArn": str,
         "EndpointName": str,
         "EndpointArn": str,
@@ -12271,14 +13297,33 @@
         "RuntimeConfig": InferenceComponentRuntimeConfigSummaryTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "InferenceComponentStatus": InferenceComponentStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeSpaceResponseTypeDef = TypedDict(
+    "DescribeSpaceResponseTypeDef",
+    {
+        "DomainId": str,
+        "SpaceArn": str,
+        "SpaceName": str,
+        "HomeEfsFileSystemUid": str,
+        "Status": SpaceStatusType,
+        "LastModifiedTime": datetime,
+        "CreationTime": datetime,
+        "FailureReason": str,
+        "SpaceSettings": SpaceSettingsOutputTypeDef,
+        "OwnershipSettings": OwnershipSettingsTypeDef,
+        "SpaceSharingSettings": SpaceSharingSettingsTypeDef,
+        "SpaceDisplayName": str,
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SpaceDetailsTypeDef = TypedDict(
     "SpaceDetailsTypeDef",
     {
         "DomainId": NotRequired[str],
         "SpaceName": NotRequired[str],
         "Status": NotRequired[SpaceStatusType],
         "CreationTime": NotRequired[datetime],
@@ -12297,33 +13342,15 @@
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "SpaceSettings": NotRequired[SpaceSettingsTypeDef],
         "OwnershipSettings": NotRequired[OwnershipSettingsTypeDef],
         "SpaceSharingSettings": NotRequired[SpaceSharingSettingsTypeDef],
         "SpaceDisplayName": NotRequired[str],
     },
 )
-DescribeSpaceResponseTypeDef = TypedDict(
-    "DescribeSpaceResponseTypeDef",
-    {
-        "DomainId": str,
-        "SpaceArn": str,
-        "SpaceName": str,
-        "HomeEfsFileSystemUid": str,
-        "Status": SpaceStatusType,
-        "LastModifiedTime": datetime,
-        "CreationTime": datetime,
-        "FailureReason": str,
-        "SpaceSettings": SpaceSettingsTypeDef,
-        "OwnershipSettings": OwnershipSettingsTypeDef,
-        "SpaceSharingSettings": SpaceSharingSettingsTypeDef,
-        "SpaceDisplayName": str,
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+SpaceSettingsUnionTypeDef = Union[SpaceSettingsTypeDef, SpaceSettingsOutputTypeDef]
 UpdateSpaceRequestRequestTypeDef = TypedDict(
     "UpdateSpaceRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpaceName": str,
         "SpaceSettings": NotRequired[SpaceSettingsTypeDef],
         "SpaceDisplayName": NotRequired[str],
@@ -12350,16 +13377,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListAssociationsResponseTypeDef = TypedDict(
     "ListAssociationsResponseTypeDef",
     {
         "AssociationSummaries": List[AssociationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TrialTypeDef = TypedDict(
     "TrialTypeDef",
     {
         "TrialName": NotRequired[str],
         "TrialArn": NotRequired[str],
@@ -12375,16 +13402,32 @@
         "TrialComponentSummaries": NotRequired[List[TrialComponentSimpleSummaryTypeDef]],
     },
 )
 ListTrialComponentsResponseTypeDef = TypedDict(
     "ListTrialComponentsResponseTypeDef",
     {
         "TrialComponentSummaries": List[TrialComponentSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+TrainingSpecificationOutputTypeDef = TypedDict(
+    "TrainingSpecificationOutputTypeDef",
+    {
+        "TrainingImage": str,
+        "SupportedTrainingInstanceTypes": List[TrainingInstanceTypeType],
+        "TrainingChannels": List[ChannelSpecificationOutputTypeDef],
+        "TrainingImageDigest": NotRequired[str],
+        "SupportedHyperParameters": NotRequired[List[HyperParameterSpecificationOutputTypeDef]],
+        "SupportsDistributedTraining": NotRequired[bool],
+        "MetricDefinitions": NotRequired[List[MetricDefinitionTypeDef]],
+        "SupportedTuningJobObjectiveMetrics": NotRequired[
+            List[HyperParameterTuningJobObjectiveTypeDef]
+        ],
+        "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
     },
 )
 TrainingSpecificationTypeDef = TypedDict(
     "TrainingSpecificationTypeDef",
     {
         "TrainingImage": str,
         "SupportedTrainingInstanceTypes": Sequence[TrainingInstanceTypeType],
@@ -12395,45 +13438,23 @@
         "MetricDefinitions": NotRequired[Sequence[MetricDefinitionTypeDef]],
         "SupportedTuningJobObjectiveMetrics": NotRequired[
             Sequence[HyperParameterTuningJobObjectiveTypeDef]
         ],
         "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
     },
 )
-ListAppImageConfigsResponsePaginatorTypeDef = TypedDict(
-    "ListAppImageConfigsResponsePaginatorTypeDef",
-    {
-        "NextToken": str,
-        "AppImageConfigs": List[AppImageConfigDetailsPaginatorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+HyperParameterTuningJobConfigUnionTypeDef = Union[
+    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigExtraOutputTypeDef
+]
 ListAppImageConfigsResponseTypeDef = TypedDict(
     "ListAppImageConfigsResponseTypeDef",
     {
-        "NextToken": str,
         "AppImageConfigs": List[AppImageConfigDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-LabelingJobSummaryPaginatorTypeDef = TypedDict(
-    "LabelingJobSummaryPaginatorTypeDef",
-    {
-        "LabelingJobName": str,
-        "LabelingJobArn": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LabelingJobStatus": LabelingJobStatusType,
-        "LabelCounters": LabelCountersTypeDef,
-        "WorkteamArn": str,
-        "PreHumanTaskLambdaArn": str,
-        "AnnotationConsolidationLambdaArn": NotRequired[str],
-        "FailureReason": NotRequired[str],
-        "LabelingJobOutput": NotRequired[LabelingJobOutputTypeDef],
-        "InputConfig": NotRequired[LabelingJobInputConfigPaginatorTypeDef],
+        "NextToken": NotRequired[str],
     },
 )
 LabelingJobSummaryTypeDef = TypedDict(
     "LabelingJobSummaryTypeDef",
     {
         "LabelingJobName": str,
         "LabelingJobArn": str,
@@ -12442,55 +13463,85 @@
         "LabelingJobStatus": LabelingJobStatusType,
         "LabelCounters": LabelCountersTypeDef,
         "WorkteamArn": str,
         "PreHumanTaskLambdaArn": str,
         "AnnotationConsolidationLambdaArn": NotRequired[str],
         "FailureReason": NotRequired[str],
         "LabelingJobOutput": NotRequired[LabelingJobOutputTypeDef],
-        "InputConfig": NotRequired[LabelingJobInputConfigTypeDef],
-    },
-)
-ListWorkteamsResponsePaginatorTypeDef = TypedDict(
-    "ListWorkteamsResponsePaginatorTypeDef",
-    {
-        "Workteams": List[WorkteamPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InputConfig": NotRequired[LabelingJobInputConfigOutputTypeDef],
     },
 )
+LabelingJobInputConfigUnionTypeDef = Union[
+    LabelingJobInputConfigTypeDef, LabelingJobInputConfigExtraOutputTypeDef
+]
 DescribeWorkteamResponseTypeDef = TypedDict(
     "DescribeWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWorkteamsResponseTypeDef = TypedDict(
     "ListWorkteamsResponseTypeDef",
     {
         "Workteams": List[WorkteamTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateWorkteamResponseTypeDef = TypedDict(
     "UpdateWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateWorkteamRequestRequestTypeDef = TypedDict(
+    "CreateWorkteamRequestRequestTypeDef",
+    {
+        "WorkteamName": str,
+        "MemberDefinitions": Sequence[MemberDefinitionUnionTypeDef],
+        "Description": str,
+        "WorkforceName": NotRequired[str],
+        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+UpdateWorkteamRequestRequestTypeDef = TypedDict(
+    "UpdateWorkteamRequestRequestTypeDef",
+    {
+        "WorkteamName": str,
+        "MemberDefinitions": NotRequired[Sequence[MemberDefinitionUnionTypeDef]],
+        "Description": NotRequired[str],
+        "NotificationConfiguration": NotRequired[NotificationConfigurationTypeDef],
+    },
+)
 ScalingPolicyTypeDef = TypedDict(
     "ScalingPolicyTypeDef",
     {
         "TargetTracking": NotRequired[TargetTrackingScalingPolicyConfigurationTypeDef],
     },
 )
-ContainerDefinitionPaginatorTypeDef = TypedDict(
-    "ContainerDefinitionPaginatorTypeDef",
+ContainerDefinitionExtraOutputTypeDef = TypedDict(
+    "ContainerDefinitionExtraOutputTypeDef",
+    {
+        "ContainerHostname": NotRequired[str],
+        "Image": NotRequired[str],
+        "ImageConfig": NotRequired[ImageConfigTypeDef],
+        "Mode": NotRequired[ContainerModeType],
+        "ModelDataUrl": NotRequired[str],
+        "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
+        "Environment": NotRequired[Dict[str, str]],
+        "ModelPackageName": NotRequired[str],
+        "InferenceSpecificationName": NotRequired[str],
+        "MultiModelConfig": NotRequired[MultiModelConfigTypeDef],
+    },
+)
+ContainerDefinitionOutputTypeDef = TypedDict(
+    "ContainerDefinitionOutputTypeDef",
     {
         "ContainerHostname": NotRequired[str],
         "Image": NotRequired[str],
         "ImageConfig": NotRequired[ImageConfigTypeDef],
         "Mode": NotRequired[ContainerModeType],
         "ModelDataUrl": NotRequired[str],
         "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
@@ -12511,24 +13562,58 @@
         "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
         "Environment": NotRequired[Mapping[str, str]],
         "ModelPackageName": NotRequired[str],
         "InferenceSpecificationName": NotRequired[str],
         "MultiModelConfig": NotRequired[MultiModelConfigTypeDef],
     },
 )
+ModelPackageContainerDefinitionExtraOutputTypeDef = TypedDict(
+    "ModelPackageContainerDefinitionExtraOutputTypeDef",
+    {
+        "Image": str,
+        "ContainerHostname": NotRequired[str],
+        "ImageDigest": NotRequired[str],
+        "ModelDataUrl": NotRequired[str],
+        "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
+        "ProductId": NotRequired[str],
+        "Environment": NotRequired[Dict[str, str]],
+        "ModelInput": NotRequired[ModelInputTypeDef],
+        "Framework": NotRequired[str],
+        "FrameworkVersion": NotRequired[str],
+        "NearestModelName": NotRequired[str],
+        "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
+    },
+)
+ModelPackageContainerDefinitionOutputTypeDef = TypedDict(
+    "ModelPackageContainerDefinitionOutputTypeDef",
+    {
+        "Image": str,
+        "ContainerHostname": NotRequired[str],
+        "ImageDigest": NotRequired[str],
+        "ModelDataUrl": NotRequired[str],
+        "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
+        "ProductId": NotRequired[str],
+        "Environment": NotRequired[Dict[str, str]],
+        "ModelInput": NotRequired[ModelInputTypeDef],
+        "Framework": NotRequired[str],
+        "FrameworkVersion": NotRequired[str],
+        "NearestModelName": NotRequired[str],
+        "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
+    },
+)
 ModelPackageContainerDefinitionTypeDef = TypedDict(
     "ModelPackageContainerDefinitionTypeDef",
     {
         "Image": str,
         "ContainerHostname": NotRequired[str],
         "ImageDigest": NotRequired[str],
         "ModelDataUrl": NotRequired[str],
         "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
         "ProductId": NotRequired[str],
-        "Environment": NotRequired[Dict[str, str]],
+        "Environment": NotRequired[Mapping[str, str]],
         "ModelInput": NotRequired[ModelInputTypeDef],
         "Framework": NotRequired[str],
         "FrameworkVersion": NotRequired[str],
         "NearestModelName": NotRequired[str],
         "AdditionalS3DataSource": NotRequired[AdditionalS3DataSourceTypeDef],
     },
 )
@@ -12540,36 +13625,36 @@
         "ModelDataSource": NotRequired[ModelDataSourceTypeDef],
     },
 )
 ListMonitoringAlertsResponseTypeDef = TypedDict(
     "ListMonitoringAlertsResponseTypeDef",
     {
         "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeInferenceExperimentResponseTypeDef = TypedDict(
     "DescribeInferenceExperimentResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": Literal["ShadowMode"],
-        "Schedule": InferenceExperimentScheduleTypeDef,
+        "Schedule": InferenceExperimentScheduleOutputTypeDef,
         "Status": InferenceExperimentStatusType,
         "StatusReason": str,
         "Description": str,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "LastModifiedTime": datetime,
         "RoleArn": str,
         "EndpointMetadata": EndpointMetadataTypeDef,
         "ModelVariants": List[ModelVariantConfigSummaryTypeDef],
-        "DataStorageConfig": InferenceExperimentDataStorageConfigTypeDef,
-        "ShadowModeConfig": ShadowModeConfigTypeDef,
+        "DataStorageConfig": InferenceExperimentDataStorageConfigOutputTypeDef,
+        "ShadowModeConfig": ShadowModeConfigOutputTypeDef,
         "KmsKey": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateInferenceExperimentRequestRequestTypeDef = TypedDict(
     "CreateInferenceExperimentRequestRequestTypeDef",
     {
@@ -12603,19 +13688,56 @@
         "Schedule": NotRequired[InferenceExperimentScheduleTypeDef],
         "Description": NotRequired[str],
         "ModelVariants": NotRequired[Sequence[ModelVariantConfigTypeDef]],
         "DataStorageConfig": NotRequired[InferenceExperimentDataStorageConfigTypeDef],
         "ShadowModeConfig": NotRequired[ShadowModeConfigTypeDef],
     },
 )
-MonitoringInputPaginatorTypeDef = TypedDict(
-    "MonitoringInputPaginatorTypeDef",
+MonitoringInputExtraOutputTypeDef = TypedDict(
+    "MonitoringInputExtraOutputTypeDef",
     {
         "EndpointInput": NotRequired[EndpointInputTypeDef],
-        "BatchTransformInput": NotRequired[BatchTransformInputPaginatorTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputExtraOutputTypeDef],
+    },
+)
+DataQualityJobInputOutputTypeDef = TypedDict(
+    "DataQualityJobInputOutputTypeDef",
+    {
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
+    },
+)
+ModelBiasJobInputOutputTypeDef = TypedDict(
+    "ModelBiasJobInputOutputTypeDef",
+    {
+        "GroundTruthS3Input": MonitoringGroundTruthS3InputTypeDef,
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
+    },
+)
+ModelExplainabilityJobInputOutputTypeDef = TypedDict(
+    "ModelExplainabilityJobInputOutputTypeDef",
+    {
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
+    },
+)
+ModelQualityJobInputOutputTypeDef = TypedDict(
+    "ModelQualityJobInputOutputTypeDef",
+    {
+        "GroundTruthS3Input": MonitoringGroundTruthS3InputTypeDef,
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
+    },
+)
+MonitoringInputOutputTypeDef = TypedDict(
+    "MonitoringInputOutputTypeDef",
+    {
+        "EndpointInput": NotRequired[EndpointInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
     },
 )
 DataQualityJobInputTypeDef = TypedDict(
     "DataQualityJobInputTypeDef",
     {
         "EndpointInput": NotRequired[EndpointInputTypeDef],
         "BatchTransformInput": NotRequired[BatchTransformInputTypeDef],
@@ -12647,68 +13769,28 @@
 MonitoringInputTypeDef = TypedDict(
     "MonitoringInputTypeDef",
     {
         "EndpointInput": NotRequired[EndpointInputTypeDef],
         "BatchTransformInput": NotRequired[BatchTransformInputTypeDef],
     },
 )
-ProcessingJobPaginatorTypeDef = TypedDict(
-    "ProcessingJobPaginatorTypeDef",
-    {
-        "ProcessingInputs": NotRequired[List[ProcessingInputTypeDef]],
-        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigPaginatorTypeDef],
-        "ProcessingJobName": NotRequired[str],
-        "ProcessingResources": NotRequired[ProcessingResourcesTypeDef],
-        "StoppingCondition": NotRequired[ProcessingStoppingConditionTypeDef],
-        "AppSpecification": NotRequired[AppSpecificationPaginatorTypeDef],
-        "Environment": NotRequired[Dict[str, str]],
-        "NetworkConfig": NotRequired[NetworkConfigPaginatorTypeDef],
-        "RoleArn": NotRequired[str],
-        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-        "ProcessingJobArn": NotRequired[str],
-        "ProcessingJobStatus": NotRequired[ProcessingJobStatusType],
-        "ExitMessage": NotRequired[str],
-        "FailureReason": NotRequired[str],
-        "ProcessingEndTime": NotRequired[datetime],
-        "ProcessingStartTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "CreationTime": NotRequired[datetime],
-        "MonitoringScheduleArn": NotRequired[str],
-        "AutoMLJobArn": NotRequired[str],
-        "TrainingJobArn": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
-CreateProcessingJobRequestRequestTypeDef = TypedDict(
-    "CreateProcessingJobRequestRequestTypeDef",
-    {
-        "ProcessingJobName": str,
-        "ProcessingResources": ProcessingResourcesTypeDef,
-        "AppSpecification": AppSpecificationTypeDef,
-        "RoleArn": str,
-        "ProcessingInputs": NotRequired[Sequence[ProcessingInputTypeDef]],
-        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigTypeDef],
-        "StoppingCondition": NotRequired[ProcessingStoppingConditionTypeDef],
-        "Environment": NotRequired[Mapping[str, str]],
-        "NetworkConfig": NotRequired[NetworkConfigTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-    },
-)
+MonitoringOutputConfigUnionTypeDef = Union[
+    MonitoringOutputConfigTypeDef, MonitoringOutputConfigExtraOutputTypeDef
+]
 DescribeProcessingJobResponseTypeDef = TypedDict(
     "DescribeProcessingJobResponseTypeDef",
     {
         "ProcessingInputs": List[ProcessingInputTypeDef],
-        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
+        "ProcessingOutputConfig": ProcessingOutputConfigOutputTypeDef,
         "ProcessingJobName": str,
         "ProcessingResources": ProcessingResourcesTypeDef,
         "StoppingCondition": ProcessingStoppingConditionTypeDef,
-        "AppSpecification": AppSpecificationTypeDef,
+        "AppSpecification": AppSpecificationOutputTypeDef,
         "Environment": Dict[str, str],
-        "NetworkConfig": NetworkConfigTypeDef,
+        "NetworkConfig": NetworkConfigOutputTypeDef,
         "RoleArn": str,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ProcessingJobArn": str,
         "ProcessingJobStatus": ProcessingJobStatusType,
         "ExitMessage": str,
         "FailureReason": str,
         "ProcessingEndTime": datetime,
@@ -12721,21 +13803,21 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ProcessingJobTypeDef = TypedDict(
     "ProcessingJobTypeDef",
     {
         "ProcessingInputs": NotRequired[List[ProcessingInputTypeDef]],
-        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigTypeDef],
+        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigOutputTypeDef],
         "ProcessingJobName": NotRequired[str],
         "ProcessingResources": NotRequired[ProcessingResourcesTypeDef],
         "StoppingCondition": NotRequired[ProcessingStoppingConditionTypeDef],
-        "AppSpecification": NotRequired[AppSpecificationTypeDef],
+        "AppSpecification": NotRequired[AppSpecificationOutputTypeDef],
         "Environment": NotRequired[Dict[str, str]],
-        "NetworkConfig": NotRequired[NetworkConfigTypeDef],
+        "NetworkConfig": NotRequired[NetworkConfigOutputTypeDef],
         "RoleArn": NotRequired[str],
         "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
         "ProcessingJobArn": NotRequired[str],
         "ProcessingJobStatus": NotRequired[ProcessingJobStatusType],
         "ExitMessage": NotRequired[str],
         "FailureReason": NotRequired[str],
         "ProcessingEndTime": NotRequired[datetime],
@@ -12744,193 +13826,142 @@
         "CreationTime": NotRequired[datetime],
         "MonitoringScheduleArn": NotRequired[str],
         "AutoMLJobArn": NotRequired[str],
         "TrainingJobArn": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-CreateFlowDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateFlowDefinitionRequestRequestTypeDef",
+CreateProcessingJobRequestRequestTypeDef = TypedDict(
+    "CreateProcessingJobRequestRequestTypeDef",
     {
-        "FlowDefinitionName": str,
-        "OutputConfig": FlowDefinitionOutputConfigTypeDef,
+        "ProcessingJobName": str,
+        "ProcessingResources": ProcessingResourcesTypeDef,
+        "AppSpecification": AppSpecificationTypeDef,
         "RoleArn": str,
-        "HumanLoopRequestSource": NotRequired[HumanLoopRequestSourceTypeDef],
-        "HumanLoopActivationConfig": NotRequired[HumanLoopActivationConfigTypeDef],
-        "HumanLoopConfig": NotRequired[HumanLoopConfigTypeDef],
+        "ProcessingInputs": NotRequired[Sequence[ProcessingInputTypeDef]],
+        "ProcessingOutputConfig": NotRequired[ProcessingOutputConfigTypeDef],
+        "StoppingCondition": NotRequired[ProcessingStoppingConditionTypeDef],
+        "Environment": NotRequired[Mapping[str, str]],
+        "NetworkConfig": NotRequired[NetworkConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
+        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
     },
 )
+ProcessingOutputConfigUnionTypeDef = Union[
+    ProcessingOutputConfigTypeDef, ProcessingOutputConfigExtraOutputTypeDef
+]
 DescribeFlowDefinitionResponseTypeDef = TypedDict(
     "DescribeFlowDefinitionResponseTypeDef",
     {
         "FlowDefinitionArn": str,
         "FlowDefinitionName": str,
         "FlowDefinitionStatus": FlowDefinitionStatusType,
         "CreationTime": datetime,
         "HumanLoopRequestSource": HumanLoopRequestSourceTypeDef,
         "HumanLoopActivationConfig": HumanLoopActivationConfigTypeDef,
-        "HumanLoopConfig": HumanLoopConfigTypeDef,
+        "HumanLoopConfig": HumanLoopConfigOutputTypeDef,
         "OutputConfig": FlowDefinitionOutputConfigTypeDef,
         "RoleArn": str,
         "FailureReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateLabelingJobRequestRequestTypeDef = TypedDict(
-    "CreateLabelingJobRequestRequestTypeDef",
+CreateFlowDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateFlowDefinitionRequestRequestTypeDef",
     {
-        "LabelingJobName": str,
-        "LabelAttributeName": str,
-        "InputConfig": LabelingJobInputConfigTypeDef,
-        "OutputConfig": LabelingJobOutputConfigTypeDef,
+        "FlowDefinitionName": str,
+        "OutputConfig": FlowDefinitionOutputConfigTypeDef,
         "RoleArn": str,
-        "HumanTaskConfig": HumanTaskConfigTypeDef,
-        "LabelCategoryConfigS3Uri": NotRequired[str],
-        "StoppingConditions": NotRequired[LabelingJobStoppingConditionsTypeDef],
-        "LabelingJobAlgorithmsConfig": NotRequired[LabelingJobAlgorithmsConfigTypeDef],
+        "HumanLoopRequestSource": NotRequired[HumanLoopRequestSourceTypeDef],
+        "HumanLoopActivationConfig": NotRequired[HumanLoopActivationConfigTypeDef],
+        "HumanLoopConfig": NotRequired[HumanLoopConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+HumanLoopConfigUnionTypeDef = Union[HumanLoopConfigTypeDef, HumanLoopConfigOutputTypeDef]
 DescribeLabelingJobResponseTypeDef = TypedDict(
     "DescribeLabelingJobResponseTypeDef",
     {
         "LabelingJobStatus": LabelingJobStatusType,
         "LabelCounters": LabelCountersTypeDef,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "JobReferenceCode": str,
         "LabelingJobName": str,
         "LabelingJobArn": str,
         "LabelAttributeName": str,
-        "InputConfig": LabelingJobInputConfigTypeDef,
+        "InputConfig": LabelingJobInputConfigOutputTypeDef,
         "OutputConfig": LabelingJobOutputConfigTypeDef,
         "RoleArn": str,
         "LabelCategoryConfigS3Uri": str,
         "StoppingConditions": LabelingJobStoppingConditionsTypeDef,
-        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigTypeDef,
-        "HumanTaskConfig": HumanTaskConfigTypeDef,
+        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigOutputTypeDef,
+        "HumanTaskConfig": HumanTaskConfigOutputTypeDef,
         "Tags": List[TagTypeDef],
         "LabelingJobOutput": LabelingJobOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-TrainingJobPaginatorTypeDef = TypedDict(
-    "TrainingJobPaginatorTypeDef",
-    {
-        "TrainingJobName": NotRequired[str],
-        "TrainingJobArn": NotRequired[str],
-        "TuningJobArn": NotRequired[str],
-        "LabelingJobArn": NotRequired[str],
-        "AutoMLJobArn": NotRequired[str],
-        "ModelArtifacts": NotRequired[ModelArtifactsTypeDef],
-        "TrainingJobStatus": NotRequired[TrainingJobStatusType],
-        "SecondaryStatus": NotRequired[SecondaryStatusType],
-        "FailureReason": NotRequired[str],
-        "HyperParameters": NotRequired[Dict[str, str]],
-        "AlgorithmSpecification": NotRequired[AlgorithmSpecificationPaginatorTypeDef],
-        "RoleArn": NotRequired[str],
-        "InputDataConfig": NotRequired[List[ChannelPaginatorTypeDef]],
-        "OutputDataConfig": NotRequired[OutputDataConfigTypeDef],
-        "ResourceConfig": NotRequired[ResourceConfigPaginatorTypeDef],
-        "VpcConfig": NotRequired[VpcConfigPaginatorTypeDef],
-        "StoppingCondition": NotRequired[StoppingConditionTypeDef],
-        "CreationTime": NotRequired[datetime],
-        "TrainingStartTime": NotRequired[datetime],
-        "TrainingEndTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "SecondaryStatusTransitions": NotRequired[List[SecondaryStatusTransitionTypeDef]],
-        "FinalMetricDataList": NotRequired[List[MetricDataTypeDef]],
-        "EnableNetworkIsolation": NotRequired[bool],
-        "EnableInterContainerTrafficEncryption": NotRequired[bool],
-        "EnableManagedSpotTraining": NotRequired[bool],
-        "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
-        "TrainingTimeInSeconds": NotRequired[int],
-        "BillableTimeInSeconds": NotRequired[int],
-        "DebugHookConfig": NotRequired[DebugHookConfigPaginatorTypeDef],
-        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-        "DebugRuleConfigurations": NotRequired[List[DebugRuleConfigurationPaginatorTypeDef]],
-        "TensorBoardOutputConfig": NotRequired[TensorBoardOutputConfigTypeDef],
-        "DebugRuleEvaluationStatuses": NotRequired[List[DebugRuleEvaluationStatusTypeDef]],
-        "ProfilerConfig": NotRequired[ProfilerConfigPaginatorTypeDef],
-        "Environment": NotRequired[Dict[str, str]],
-        "RetryStrategy": NotRequired[RetryStrategyTypeDef],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
-CreateTrainingJobRequestRequestTypeDef = TypedDict(
-    "CreateTrainingJobRequestRequestTypeDef",
+CreateLabelingJobRequestRequestTypeDef = TypedDict(
+    "CreateLabelingJobRequestRequestTypeDef",
     {
-        "TrainingJobName": str,
-        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
+        "LabelingJobName": str,
+        "LabelAttributeName": str,
+        "InputConfig": LabelingJobInputConfigTypeDef,
+        "OutputConfig": LabelingJobOutputConfigTypeDef,
         "RoleArn": str,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigTypeDef,
-        "StoppingCondition": StoppingConditionTypeDef,
-        "HyperParameters": NotRequired[Mapping[str, str]],
-        "InputDataConfig": NotRequired[Sequence[ChannelTypeDef]],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "HumanTaskConfig": HumanTaskConfigTypeDef,
+        "LabelCategoryConfigS3Uri": NotRequired[str],
+        "StoppingConditions": NotRequired[LabelingJobStoppingConditionsTypeDef],
+        "LabelingJobAlgorithmsConfig": NotRequired[LabelingJobAlgorithmsConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
-        "EnableNetworkIsolation": NotRequired[bool],
-        "EnableInterContainerTrafficEncryption": NotRequired[bool],
-        "EnableManagedSpotTraining": NotRequired[bool],
-        "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
-        "DebugHookConfig": NotRequired[DebugHookConfigTypeDef],
-        "DebugRuleConfigurations": NotRequired[Sequence[DebugRuleConfigurationTypeDef]],
-        "TensorBoardOutputConfig": NotRequired[TensorBoardOutputConfigTypeDef],
-        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-        "ProfilerConfig": NotRequired[ProfilerConfigTypeDef],
-        "ProfilerRuleConfigurations": NotRequired[Sequence[ProfilerRuleConfigurationTypeDef]],
-        "Environment": NotRequired[Mapping[str, str]],
-        "RetryStrategy": NotRequired[RetryStrategyTypeDef],
-        "RemoteDebugConfig": NotRequired[RemoteDebugConfigTypeDef],
-        "InfraCheckConfig": NotRequired[InfraCheckConfigTypeDef],
     },
 )
+HumanTaskConfigUnionTypeDef = Union[HumanTaskConfigTypeDef, HumanTaskConfigOutputTypeDef]
 DescribeTrainingJobResponseTypeDef = TypedDict(
     "DescribeTrainingJobResponseTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
         "TuningJobArn": str,
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "TrainingJobStatus": TrainingJobStatusType,
         "SecondaryStatus": SecondaryStatusType,
         "FailureReason": str,
         "HyperParameters": Dict[str, str],
-        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
+        "AlgorithmSpecification": AlgorithmSpecificationOutputTypeDef,
         "RoleArn": str,
-        "InputDataConfig": List[ChannelTypeDef],
+        "InputDataConfig": List[ChannelOutputTypeDef],
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigTypeDef,
+        "ResourceConfig": ResourceConfigOutputTypeDef,
         "WarmPoolStatus": WarmPoolStatusTypeDef,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "CreationTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
         "LastModifiedTime": datetime,
         "SecondaryStatusTransitions": List[SecondaryStatusTransitionTypeDef],
         "FinalMetricDataList": List[MetricDataTypeDef],
         "EnableNetworkIsolation": bool,
         "EnableInterContainerTrafficEncryption": bool,
         "EnableManagedSpotTraining": bool,
         "CheckpointConfig": CheckpointConfigTypeDef,
         "TrainingTimeInSeconds": int,
         "BillableTimeInSeconds": int,
-        "DebugHookConfig": DebugHookConfigTypeDef,
+        "DebugHookConfig": DebugHookConfigOutputTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
-        "DebugRuleConfigurations": List[DebugRuleConfigurationTypeDef],
+        "DebugRuleConfigurations": List[DebugRuleConfigurationOutputTypeDef],
         "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
         "DebugRuleEvaluationStatuses": List[DebugRuleEvaluationStatusTypeDef],
-        "ProfilerConfig": ProfilerConfigTypeDef,
-        "ProfilerRuleConfigurations": List[ProfilerRuleConfigurationTypeDef],
+        "ProfilerConfig": ProfilerConfigOutputTypeDef,
+        "ProfilerRuleConfigurations": List[ProfilerRuleConfigurationOutputTypeDef],
         "ProfilerRuleEvaluationStatuses": List[ProfilerRuleEvaluationStatusTypeDef],
         "ProfilingStatus": ProfilingStatusType,
         "Environment": Dict[str, str],
         "RetryStrategy": RetryStrategyTypeDef,
         "RemoteDebugConfig": RemoteDebugConfigTypeDef,
         "InfraCheckConfig": InfraCheckConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -12945,44 +13976,47 @@
         "LabelingJobArn": NotRequired[str],
         "AutoMLJobArn": NotRequired[str],
         "ModelArtifacts": NotRequired[ModelArtifactsTypeDef],
         "TrainingJobStatus": NotRequired[TrainingJobStatusType],
         "SecondaryStatus": NotRequired[SecondaryStatusType],
         "FailureReason": NotRequired[str],
         "HyperParameters": NotRequired[Dict[str, str]],
-        "AlgorithmSpecification": NotRequired[AlgorithmSpecificationTypeDef],
+        "AlgorithmSpecification": NotRequired[AlgorithmSpecificationOutputTypeDef],
         "RoleArn": NotRequired[str],
-        "InputDataConfig": NotRequired[List[ChannelTypeDef]],
+        "InputDataConfig": NotRequired[List[ChannelOutputTypeDef]],
         "OutputDataConfig": NotRequired[OutputDataConfigTypeDef],
-        "ResourceConfig": NotRequired[ResourceConfigTypeDef],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "ResourceConfig": NotRequired[ResourceConfigOutputTypeDef],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
         "StoppingCondition": NotRequired[StoppingConditionTypeDef],
         "CreationTime": NotRequired[datetime],
         "TrainingStartTime": NotRequired[datetime],
         "TrainingEndTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
         "SecondaryStatusTransitions": NotRequired[List[SecondaryStatusTransitionTypeDef]],
         "FinalMetricDataList": NotRequired[List[MetricDataTypeDef]],
         "EnableNetworkIsolation": NotRequired[bool],
         "EnableInterContainerTrafficEncryption": NotRequired[bool],
         "EnableManagedSpotTraining": NotRequired[bool],
         "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
         "TrainingTimeInSeconds": NotRequired[int],
         "BillableTimeInSeconds": NotRequired[int],
-        "DebugHookConfig": NotRequired[DebugHookConfigTypeDef],
+        "DebugHookConfig": NotRequired[DebugHookConfigOutputTypeDef],
         "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
-        "DebugRuleConfigurations": NotRequired[List[DebugRuleConfigurationTypeDef]],
+        "DebugRuleConfigurations": NotRequired[List[DebugRuleConfigurationOutputTypeDef]],
         "TensorBoardOutputConfig": NotRequired[TensorBoardOutputConfigTypeDef],
         "DebugRuleEvaluationStatuses": NotRequired[List[DebugRuleEvaluationStatusTypeDef]],
-        "ProfilerConfig": NotRequired[ProfilerConfigTypeDef],
+        "ProfilerConfig": NotRequired[ProfilerConfigOutputTypeDef],
         "Environment": NotRequired[Dict[str, str]],
         "RetryStrategy": NotRequired[RetryStrategyTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
+AlgorithmSpecificationUnionTypeDef = Union[
+    AlgorithmSpecificationTypeDef, AlgorithmSpecificationExtraOutputTypeDef
+]
 CreateTransformJobRequestRequestTypeDef = TypedDict(
     "CreateTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
         "ModelName": str,
         "TransformInput": TransformInputTypeDef,
         "TransformOutput": TransformOutputTypeDef,
@@ -13021,16 +14055,28 @@
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "DataProcessing": DataProcessingTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-TransformJobDefinitionPaginatorTypeDef = TypedDict(
-    "TransformJobDefinitionPaginatorTypeDef",
+TransformJobDefinitionExtraOutputTypeDef = TypedDict(
+    "TransformJobDefinitionExtraOutputTypeDef",
+    {
+        "TransformInput": TransformInputTypeDef,
+        "TransformOutput": TransformOutputTypeDef,
+        "TransformResources": TransformResourcesTypeDef,
+        "MaxConcurrentTransforms": NotRequired[int],
+        "MaxPayloadInMB": NotRequired[int],
+        "BatchStrategy": NotRequired[BatchStrategyType],
+        "Environment": NotRequired[Dict[str, str]],
+    },
+)
+TransformJobDefinitionOutputTypeDef = TypedDict(
+    "TransformJobDefinitionOutputTypeDef",
     {
         "TransformInput": TransformInputTypeDef,
         "TransformOutput": TransformOutputTypeDef,
         "TransformResources": TransformResourcesTypeDef,
         "MaxConcurrentTransforms": NotRequired[int],
         "MaxPayloadInMB": NotRequired[int],
         "BatchStrategy": NotRequired[BatchStrategyType],
@@ -13072,148 +14118,139 @@
         "LabelingJobArn": NotRequired[str],
         "AutoMLJobArn": NotRequired[str],
         "DataProcessing": NotRequired[DataProcessingTypeDef],
         "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-CreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
-    "CreateAutoMLJobV2RequestRequestTypeDef",
-    {
-        "AutoMLJobName": str,
-        "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
-        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
-        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
-        "RoleArn": str,
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "SecurityConfig": NotRequired[AutoMLSecurityConfigTypeDef],
-        "AutoMLJobObjective": NotRequired[AutoMLJobObjectiveTypeDef],
-        "ModelDeployConfig": NotRequired[ModelDeployConfigTypeDef],
-        "DataSplitConfig": NotRequired[AutoMLDataSplitConfigTypeDef],
-    },
-)
 DescribeAutoMLJobV2ResponseTypeDef = TypedDict(
     "DescribeAutoMLJobV2ResponseTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
         "AutoMLJobInputDataConfig": List[AutoMLJobChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
-        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigOutputTypeDef,
         "AutoMLProblemTypeConfigName": AutoMLProblemTypeConfigNameType,
         "CreationTime": datetime,
         "EndTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
         "BestCandidate": AutoMLCandidateTypeDef,
         "AutoMLJobStatus": AutoMLJobStatusType,
         "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
         "AutoMLJobArtifacts": AutoMLJobArtifactsTypeDef,
         "ResolvedAttributes": AutoMLResolvedAttributesTypeDef,
         "ModelDeployConfig": ModelDeployConfigTypeDef,
         "ModelDeployResult": ModelDeployResultTypeDef,
         "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
-        "SecurityConfig": AutoMLSecurityConfigTypeDef,
+        "SecurityConfig": AutoMLSecurityConfigOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AutoMLProblemTypeConfigUnionTypeDef = Union[
+    AutoMLProblemTypeConfigTypeDef, AutoMLProblemTypeConfigOutputTypeDef
+]
+CreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
+    "CreateAutoMLJobV2RequestRequestTypeDef",
+    {
+        "AutoMLJobName": str,
+        "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
+        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "RoleArn": str,
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "SecurityConfig": NotRequired[AutoMLSecurityConfigTypeDef],
+        "AutoMLJobObjective": NotRequired[AutoMLJobObjectiveTypeDef],
+        "ModelDeployConfig": NotRequired[ModelDeployConfigTypeDef],
+        "DataSplitConfig": NotRequired[AutoMLDataSplitConfigTypeDef],
+    },
+)
 ListPipelineExecutionStepsResponseTypeDef = TypedDict(
     "ListPipelineExecutionStepsResponseTypeDef",
     {
         "PipelineExecutionSteps": List[PipelineExecutionStepTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateEndpointInputRequestTypeDef = TypedDict(
     "CreateEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
         "EndpointConfigName": str,
         "DeploymentConfig": NotRequired[DeploymentConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+DeploymentConfigUnionTypeDef = Union[DeploymentConfigTypeDef, DeploymentConfigOutputTypeDef]
 UpdateEndpointInputRequestTypeDef = TypedDict(
     "UpdateEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
         "EndpointConfigName": str,
         "RetainAllVariantProperties": NotRequired[bool],
         "ExcludeRetainedVariantProperties": NotRequired[Sequence[VariantPropertyTypeDef]],
         "DeploymentConfig": NotRequired[DeploymentConfigTypeDef],
         "RetainDeploymentConfig": NotRequired[bool],
     },
 )
-CreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
-    "CreateInferenceRecommendationsJobRequestRequestTypeDef",
-    {
-        "JobName": str,
-        "JobType": RecommendationJobTypeType,
-        "RoleArn": str,
-        "InputConfig": RecommendationJobInputConfigTypeDef,
-        "JobDescription": NotRequired[str],
-        "StoppingConditions": NotRequired[RecommendationJobStoppingConditionsTypeDef],
-        "OutputConfig": NotRequired[RecommendationJobOutputConfigTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 DescribeInferenceRecommendationsJobResponseTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobResponseTypeDef",
     {
         "JobName": str,
         "JobDescription": str,
         "JobType": RecommendationJobTypeType,
         "JobArn": str,
         "RoleArn": str,
         "Status": RecommendationJobStatusType,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
-        "InputConfig": RecommendationJobInputConfigTypeDef,
-        "StoppingConditions": RecommendationJobStoppingConditionsTypeDef,
+        "InputConfig": RecommendationJobInputConfigOutputTypeDef,
+        "StoppingConditions": RecommendationJobStoppingConditionsOutputTypeDef,
         "InferenceRecommendations": List[InferenceRecommendationTypeDef],
         "EndpointPerformances": List[EndpointPerformanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateEndpointConfigInputRequestTypeDef = TypedDict(
-    "CreateEndpointConfigInputRequestTypeDef",
+CreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
+    "CreateInferenceRecommendationsJobRequestRequestTypeDef",
     {
-        "EndpointConfigName": str,
-        "ProductionVariants": Sequence[ProductionVariantTypeDef],
-        "DataCaptureConfig": NotRequired[DataCaptureConfigTypeDef],
+        "JobName": str,
+        "JobType": RecommendationJobTypeType,
+        "RoleArn": str,
+        "InputConfig": RecommendationJobInputConfigTypeDef,
+        "JobDescription": NotRequired[str],
+        "StoppingConditions": NotRequired[RecommendationJobStoppingConditionsTypeDef],
+        "OutputConfig": NotRequired[RecommendationJobOutputConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
-        "KmsKeyId": NotRequired[str],
-        "AsyncInferenceConfig": NotRequired[AsyncInferenceConfigTypeDef],
-        "ExplainerConfig": NotRequired[ExplainerConfigTypeDef],
-        "ShadowProductionVariants": NotRequired[Sequence[ProductionVariantTypeDef]],
-        "ExecutionRoleArn": NotRequired[str],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
-        "EnableNetworkIsolation": NotRequired[bool],
     },
 )
+RecommendationJobInputConfigUnionTypeDef = Union[
+    RecommendationJobInputConfigTypeDef, RecommendationJobInputConfigOutputTypeDef
+]
 DescribeEndpointConfigOutputTypeDef = TypedDict(
     "DescribeEndpointConfigOutputTypeDef",
     {
         "EndpointConfigName": str,
         "EndpointConfigArn": str,
         "ProductionVariants": List[ProductionVariantTypeDef],
-        "DataCaptureConfig": DataCaptureConfigTypeDef,
+        "DataCaptureConfig": DataCaptureConfigOutputTypeDef,
         "KmsKeyId": str,
         "CreationTime": datetime,
-        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
-        "ExplainerConfig": ExplainerConfigTypeDef,
+        "AsyncInferenceConfig": AsyncInferenceConfigOutputTypeDef,
+        "ExplainerConfig": ExplainerConfigOutputTypeDef,
         "ShadowProductionVariants": List[ProductionVariantTypeDef],
         "ExecutionRoleArn": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "EnableNetworkIsolation": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeEndpointOutputTypeDef = TypedDict(
     "DescribeEndpointOutputTypeDef",
     {
@@ -13222,223 +14259,246 @@
         "EndpointConfigName": str,
         "ProductionVariants": List[ProductionVariantSummaryTypeDef],
         "DataCaptureConfig": DataCaptureConfigSummaryTypeDef,
         "EndpointStatus": EndpointStatusType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "LastDeploymentConfig": DeploymentConfigTypeDef,
-        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
+        "LastDeploymentConfig": DeploymentConfigOutputTypeDef,
+        "AsyncInferenceConfig": AsyncInferenceConfigOutputTypeDef,
         "PendingDeploymentSummary": PendingDeploymentSummaryTypeDef,
-        "ExplainerConfig": ExplainerConfigTypeDef,
+        "ExplainerConfig": ExplainerConfigOutputTypeDef,
         "ShadowProductionVariants": List[ProductionVariantSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-HyperParameterTuningJobSearchEntityPaginatorTypeDef = TypedDict(
-    "HyperParameterTuningJobSearchEntityPaginatorTypeDef",
-    {
-        "HyperParameterTuningJobName": NotRequired[str],
-        "HyperParameterTuningJobArn": NotRequired[str],
-        "HyperParameterTuningJobConfig": NotRequired[HyperParameterTuningJobConfigPaginatorTypeDef],
-        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionPaginatorTypeDef],
-        "TrainingJobDefinitions": NotRequired[
-            List[HyperParameterTrainingJobDefinitionPaginatorTypeDef]
-        ],
-        "HyperParameterTuningJobStatus": NotRequired[HyperParameterTuningJobStatusType],
-        "CreationTime": NotRequired[datetime],
-        "HyperParameterTuningEndTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "TrainingJobStatusCounters": NotRequired[TrainingJobStatusCountersTypeDef],
-        "ObjectiveStatusCounters": NotRequired[ObjectiveStatusCountersTypeDef],
-        "BestTrainingJob": NotRequired[HyperParameterTrainingJobSummaryTypeDef],
-        "OverallBestTrainingJob": NotRequired[HyperParameterTrainingJobSummaryTypeDef],
-        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigPaginatorTypeDef],
-        "FailureReason": NotRequired[str],
-        "TuningJobCompletionDetails": NotRequired[HyperParameterTuningJobCompletionDetailsTypeDef],
-        "ConsumedResources": NotRequired[HyperParameterTuningJobConsumedResourcesTypeDef],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
-CreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
-    "CreateHyperParameterTuningJobRequestRequestTypeDef",
+CreateEndpointConfigInputRequestTypeDef = TypedDict(
+    "CreateEndpointConfigInputRequestTypeDef",
     {
-        "HyperParameterTuningJobName": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
-        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionTypeDef],
-        "TrainingJobDefinitions": NotRequired[Sequence[HyperParameterTrainingJobDefinitionTypeDef]],
-        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigTypeDef],
+        "EndpointConfigName": str,
+        "ProductionVariants": Sequence[ProductionVariantTypeDef],
+        "DataCaptureConfig": NotRequired[DataCaptureConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
-        "Autotune": NotRequired[AutotuneTypeDef],
+        "KmsKeyId": NotRequired[str],
+        "AsyncInferenceConfig": NotRequired[AsyncInferenceConfigTypeDef],
+        "ExplainerConfig": NotRequired[ExplainerConfigTypeDef],
+        "ShadowProductionVariants": NotRequired[Sequence[ProductionVariantTypeDef]],
+        "ExecutionRoleArn": NotRequired[str],
+        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "EnableNetworkIsolation": NotRequired[bool],
     },
 )
+ExplainerConfigUnionTypeDef = Union[ExplainerConfigTypeDef, ExplainerConfigOutputTypeDef]
 DescribeHyperParameterTuningJobResponseTypeDef = TypedDict(
     "DescribeHyperParameterTuningJobResponseTypeDef",
     {
         "HyperParameterTuningJobName": str,
         "HyperParameterTuningJobArn": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
-        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
-        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionTypeDef],
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigOutputTypeDef,
+        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionOutputTypeDef,
+        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionOutputTypeDef],
         "HyperParameterTuningJobStatus": HyperParameterTuningJobStatusType,
         "CreationTime": datetime,
         "HyperParameterTuningEndTime": datetime,
         "LastModifiedTime": datetime,
         "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
         "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
         "BestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
         "OverallBestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
-        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
+        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigOutputTypeDef,
         "Autotune": AutotuneTypeDef,
         "FailureReason": str,
         "TuningJobCompletionDetails": HyperParameterTuningJobCompletionDetailsTypeDef,
         "ConsumedResources": HyperParameterTuningJobConsumedResourcesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 HyperParameterTuningJobSearchEntityTypeDef = TypedDict(
     "HyperParameterTuningJobSearchEntityTypeDef",
     {
         "HyperParameterTuningJobName": NotRequired[str],
         "HyperParameterTuningJobArn": NotRequired[str],
-        "HyperParameterTuningJobConfig": NotRequired[HyperParameterTuningJobConfigTypeDef],
-        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionTypeDef],
-        "TrainingJobDefinitions": NotRequired[List[HyperParameterTrainingJobDefinitionTypeDef]],
+        "HyperParameterTuningJobConfig": NotRequired[HyperParameterTuningJobConfigOutputTypeDef],
+        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionOutputTypeDef],
+        "TrainingJobDefinitions": NotRequired[
+            List[HyperParameterTrainingJobDefinitionOutputTypeDef]
+        ],
         "HyperParameterTuningJobStatus": NotRequired[HyperParameterTuningJobStatusType],
         "CreationTime": NotRequired[datetime],
         "HyperParameterTuningEndTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
         "TrainingJobStatusCounters": NotRequired[TrainingJobStatusCountersTypeDef],
         "ObjectiveStatusCounters": NotRequired[ObjectiveStatusCountersTypeDef],
         "BestTrainingJob": NotRequired[HyperParameterTrainingJobSummaryTypeDef],
         "OverallBestTrainingJob": NotRequired[HyperParameterTrainingJobSummaryTypeDef],
-        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigTypeDef],
+        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigOutputTypeDef],
         "FailureReason": NotRequired[str],
         "TuningJobCompletionDetails": NotRequired[HyperParameterTuningJobCompletionDetailsTypeDef],
         "ConsumedResources": NotRequired[HyperParameterTuningJobConsumedResourcesTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
+CreateTrainingJobRequestRequestTypeDef = TypedDict(
+    "CreateTrainingJobRequestRequestTypeDef",
+    {
+        "TrainingJobName": str,
+        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
+        "RoleArn": str,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "ResourceConfig": ResourceConfigTypeDef,
+        "StoppingCondition": StoppingConditionTypeDef,
+        "HyperParameters": NotRequired[Mapping[str, str]],
+        "InputDataConfig": NotRequired[Sequence[ChannelUnionTypeDef]],
+        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "EnableNetworkIsolation": NotRequired[bool],
+        "EnableInterContainerTrafficEncryption": NotRequired[bool],
+        "EnableManagedSpotTraining": NotRequired[bool],
+        "CheckpointConfig": NotRequired[CheckpointConfigTypeDef],
+        "DebugHookConfig": NotRequired[DebugHookConfigTypeDef],
+        "DebugRuleConfigurations": NotRequired[Sequence[DebugRuleConfigurationUnionTypeDef]],
+        "TensorBoardOutputConfig": NotRequired[TensorBoardOutputConfigTypeDef],
+        "ExperimentConfig": NotRequired[ExperimentConfigTypeDef],
+        "ProfilerConfig": NotRequired[ProfilerConfigTypeDef],
+        "ProfilerRuleConfigurations": NotRequired[Sequence[ProfilerRuleConfigurationUnionTypeDef]],
+        "Environment": NotRequired[Mapping[str, str]],
+        "RetryStrategy": NotRequired[RetryStrategyTypeDef],
+        "RemoteDebugConfig": NotRequired[RemoteDebugConfigTypeDef],
+        "InfraCheckConfig": NotRequired[InfraCheckConfigTypeDef],
+        "SessionChainingConfig": NotRequired[SessionChainingConfigTypeDef],
+    },
+)
+HyperParameterTrainingJobDefinitionUnionTypeDef = Union[
+    HyperParameterTrainingJobDefinitionTypeDef,
+    HyperParameterTrainingJobDefinitionExtraOutputTypeDef,
+]
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "Spaces": List[SpaceDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListInferenceRecommendationsJobStepsResponseTypeDef = TypedDict(
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
     {
         "Steps": List[InferenceRecommendationsJobStepTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListLabelingJobsResponsePaginatorTypeDef = TypedDict(
-    "ListLabelingJobsResponsePaginatorTypeDef",
-    {
-        "LabelingJobSummaryList": List[LabelingJobSummaryPaginatorTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+TrainingSpecificationUnionTypeDef = Union[
+    TrainingSpecificationTypeDef, TrainingSpecificationOutputTypeDef
+]
 ListLabelingJobsResponseTypeDef = TypedDict(
     "ListLabelingJobsResponseTypeDef",
     {
         "LabelingJobSummaryList": List[LabelingJobSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DynamicScalingConfigurationTypeDef = TypedDict(
     "DynamicScalingConfigurationTypeDef",
     {
         "MinCapacity": NotRequired[int],
         "MaxCapacity": NotRequired[int],
         "ScaleInCooldown": NotRequired[int],
         "ScaleOutCooldown": NotRequired[int],
         "ScalingPolicies": NotRequired[List[ScalingPolicyTypeDef]],
     },
 )
-ModelPaginatorTypeDef = TypedDict(
-    "ModelPaginatorTypeDef",
-    {
-        "ModelName": NotRequired[str],
-        "PrimaryContainer": NotRequired[ContainerDefinitionPaginatorTypeDef],
-        "Containers": NotRequired[List[ContainerDefinitionPaginatorTypeDef]],
-        "InferenceExecutionConfig": NotRequired[InferenceExecutionConfigTypeDef],
-        "ExecutionRoleArn": NotRequired[str],
-        "VpcConfig": NotRequired[VpcConfigPaginatorTypeDef],
-        "CreationTime": NotRequired[datetime],
-        "ModelArn": NotRequired[str],
-        "EnableNetworkIsolation": NotRequired[bool],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "DeploymentRecommendation": NotRequired[DeploymentRecommendationTypeDef],
-    },
-)
-CreateModelInputRequestTypeDef = TypedDict(
-    "CreateModelInputRequestTypeDef",
-    {
-        "ModelName": str,
-        "PrimaryContainer": NotRequired[ContainerDefinitionTypeDef],
-        "Containers": NotRequired[Sequence[ContainerDefinitionTypeDef]],
-        "InferenceExecutionConfig": NotRequired[InferenceExecutionConfigTypeDef],
-        "ExecutionRoleArn": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
-        "EnableNetworkIsolation": NotRequired[bool],
-    },
-)
 DescribeModelOutputTypeDef = TypedDict(
     "DescribeModelOutputTypeDef",
     {
         "ModelName": str,
-        "PrimaryContainer": ContainerDefinitionTypeDef,
-        "Containers": List[ContainerDefinitionTypeDef],
+        "PrimaryContainer": ContainerDefinitionOutputTypeDef,
+        "Containers": List[ContainerDefinitionOutputTypeDef],
         "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
         "ExecutionRoleArn": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "CreationTime": datetime,
         "ModelArn": str,
         "EnableNetworkIsolation": bool,
         "DeploymentRecommendation": DeploymentRecommendationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ModelTypeDef = TypedDict(
     "ModelTypeDef",
     {
         "ModelName": NotRequired[str],
-        "PrimaryContainer": NotRequired[ContainerDefinitionTypeDef],
-        "Containers": NotRequired[List[ContainerDefinitionTypeDef]],
+        "PrimaryContainer": NotRequired[ContainerDefinitionOutputTypeDef],
+        "Containers": NotRequired[List[ContainerDefinitionOutputTypeDef]],
         "InferenceExecutionConfig": NotRequired[InferenceExecutionConfigTypeDef],
         "ExecutionRoleArn": NotRequired[str],
-        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "VpcConfig": NotRequired[VpcConfigOutputTypeDef],
         "CreationTime": NotRequired[datetime],
         "ModelArn": NotRequired[str],
         "EnableNetworkIsolation": NotRequired[bool],
         "Tags": NotRequired[List[TagTypeDef]],
         "DeploymentRecommendation": NotRequired[DeploymentRecommendationTypeDef],
     },
 )
-AdditionalInferenceSpecificationDefinitionPaginatorTypeDef = TypedDict(
-    "AdditionalInferenceSpecificationDefinitionPaginatorTypeDef",
+ContainerDefinitionUnionTypeDef = Union[
+    ContainerDefinitionTypeDef, ContainerDefinitionExtraOutputTypeDef
+]
+AdditionalInferenceSpecificationDefinitionExtraOutputTypeDef = TypedDict(
+    "AdditionalInferenceSpecificationDefinitionExtraOutputTypeDef",
     {
         "Name": str,
-        "Containers": List[ModelPackageContainerDefinitionTypeDef],
+        "Containers": List[ModelPackageContainerDefinitionExtraOutputTypeDef],
         "Description": NotRequired[str],
         "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
         "SupportedRealtimeInferenceInstanceTypes": NotRequired[
             List[ProductionVariantInstanceTypeType]
         ],
         "SupportedContentTypes": NotRequired[List[str]],
         "SupportedResponseMIMETypes": NotRequired[List[str]],
     },
 )
+InferenceSpecificationExtraOutputTypeDef = TypedDict(
+    "InferenceSpecificationExtraOutputTypeDef",
+    {
+        "Containers": List[ModelPackageContainerDefinitionExtraOutputTypeDef],
+        "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
+        "SupportedRealtimeInferenceInstanceTypes": NotRequired[
+            List[ProductionVariantInstanceTypeType]
+        ],
+        "SupportedContentTypes": NotRequired[List[str]],
+        "SupportedResponseMIMETypes": NotRequired[List[str]],
+    },
+)
+AdditionalInferenceSpecificationDefinitionOutputTypeDef = TypedDict(
+    "AdditionalInferenceSpecificationDefinitionOutputTypeDef",
+    {
+        "Name": str,
+        "Containers": List[ModelPackageContainerDefinitionOutputTypeDef],
+        "Description": NotRequired[str],
+        "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
+        "SupportedRealtimeInferenceInstanceTypes": NotRequired[
+            List[ProductionVariantInstanceTypeType]
+        ],
+        "SupportedContentTypes": NotRequired[List[str]],
+        "SupportedResponseMIMETypes": NotRequired[List[str]],
+    },
+)
+InferenceSpecificationOutputTypeDef = TypedDict(
+    "InferenceSpecificationOutputTypeDef",
+    {
+        "Containers": List[ModelPackageContainerDefinitionOutputTypeDef],
+        "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
+        "SupportedRealtimeInferenceInstanceTypes": NotRequired[
+            List[ProductionVariantInstanceTypeType]
+        ],
+        "SupportedContentTypes": NotRequired[List[str]],
+        "SupportedResponseMIMETypes": NotRequired[List[str]],
+    },
+)
 AdditionalInferenceSpecificationDefinitionTypeDef = TypedDict(
     "AdditionalInferenceSpecificationDefinitionTypeDef",
     {
         "Name": str,
         "Containers": Sequence[ModelPackageContainerDefinitionTypeDef],
         "Description": NotRequired[str],
         "SupportedTransformInstanceTypes": NotRequired[Sequence[TransformInstanceTypeType]],
@@ -13448,196 +14508,241 @@
         "SupportedContentTypes": NotRequired[Sequence[str]],
         "SupportedResponseMIMETypes": NotRequired[Sequence[str]],
     },
 )
 InferenceSpecificationTypeDef = TypedDict(
     "InferenceSpecificationTypeDef",
     {
-        "Containers": List[ModelPackageContainerDefinitionTypeDef],
-        "SupportedTransformInstanceTypes": NotRequired[List[TransformInstanceTypeType]],
+        "Containers": Sequence[ModelPackageContainerDefinitionTypeDef],
+        "SupportedTransformInstanceTypes": NotRequired[Sequence[TransformInstanceTypeType]],
         "SupportedRealtimeInferenceInstanceTypes": NotRequired[
-            List[ProductionVariantInstanceTypeType]
+            Sequence[ProductionVariantInstanceTypeType]
         ],
-        "SupportedContentTypes": NotRequired[List[str]],
-        "SupportedResponseMIMETypes": NotRequired[List[str]],
+        "SupportedContentTypes": NotRequired[Sequence[str]],
+        "SupportedResponseMIMETypes": NotRequired[Sequence[str]],
     },
 )
-SourceAlgorithmSpecificationPaginatorTypeDef = TypedDict(
-    "SourceAlgorithmSpecificationPaginatorTypeDef",
+SourceAlgorithmSpecificationExtraOutputTypeDef = TypedDict(
+    "SourceAlgorithmSpecificationExtraOutputTypeDef",
+    {
+        "SourceAlgorithms": List[SourceAlgorithmTypeDef],
+    },
+)
+SourceAlgorithmSpecificationOutputTypeDef = TypedDict(
+    "SourceAlgorithmSpecificationOutputTypeDef",
     {
         "SourceAlgorithms": List[SourceAlgorithmTypeDef],
     },
 )
 SourceAlgorithmSpecificationTypeDef = TypedDict(
     "SourceAlgorithmSpecificationTypeDef",
     {
         "SourceAlgorithms": Sequence[SourceAlgorithmTypeDef],
     },
 )
-MonitoringJobDefinitionPaginatorTypeDef = TypedDict(
-    "MonitoringJobDefinitionPaginatorTypeDef",
+MonitoringJobDefinitionExtraOutputTypeDef = TypedDict(
+    "MonitoringJobDefinitionExtraOutputTypeDef",
     {
-        "MonitoringInputs": List[MonitoringInputPaginatorTypeDef],
-        "MonitoringOutputConfig": MonitoringOutputConfigPaginatorTypeDef,
+        "MonitoringInputs": List[MonitoringInputExtraOutputTypeDef],
+        "MonitoringOutputConfig": MonitoringOutputConfigExtraOutputTypeDef,
         "MonitoringResources": MonitoringResourcesTypeDef,
-        "MonitoringAppSpecification": MonitoringAppSpecificationPaginatorTypeDef,
+        "MonitoringAppSpecification": MonitoringAppSpecificationExtraOutputTypeDef,
         "RoleArn": str,
         "BaselineConfig": NotRequired[MonitoringBaselineConfigTypeDef],
         "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
         "Environment": NotRequired[Dict[str, str]],
-        "NetworkConfig": NotRequired[NetworkConfigPaginatorTypeDef],
+        "NetworkConfig": NotRequired[NetworkConfigExtraOutputTypeDef],
     },
 )
-CreateDataQualityJobDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateDataQualityJobDefinitionRequestRequestTypeDef",
+DescribeDataQualityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeDataQualityJobDefinitionResponseTypeDef",
     {
+        "JobDefinitionArn": str,
         "JobDefinitionName": str,
-        "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
-        "DataQualityJobInput": DataQualityJobInputTypeDef,
-        "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "CreationTime": datetime,
+        "DataQualityBaselineConfig": DataQualityBaselineConfigTypeDef,
+        "DataQualityAppSpecification": DataQualityAppSpecificationOutputTypeDef,
+        "DataQualityJobInput": DataQualityJobInputOutputTypeDef,
+        "DataQualityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
         "RoleArn": str,
-        "DataQualityBaselineConfig": NotRequired[DataQualityBaselineConfigTypeDef],
-        "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
-        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeDataQualityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeDataQualityJobDefinitionResponseTypeDef",
+DescribeModelBiasJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelBiasJobDefinitionResponseTypeDef",
     {
         "JobDefinitionArn": str,
         "JobDefinitionName": str,
         "CreationTime": datetime,
-        "DataQualityBaselineConfig": DataQualityBaselineConfigTypeDef,
-        "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
-        "DataQualityJobInput": DataQualityJobInputTypeDef,
-        "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "ModelBiasBaselineConfig": ModelBiasBaselineConfigTypeDef,
+        "ModelBiasAppSpecification": ModelBiasAppSpecificationOutputTypeDef,
+        "ModelBiasJobInput": ModelBiasJobInputOutputTypeDef,
+        "ModelBiasJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
         "RoleArn": str,
         "StoppingCondition": MonitoringStoppingConditionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateModelBiasJobDefinitionRequestRequestTypeDef",
+DescribeModelExplainabilityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
     {
+        "JobDefinitionArn": str,
         "JobDefinitionName": str,
-        "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
-        "ModelBiasJobInput": ModelBiasJobInputTypeDef,
-        "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "CreationTime": datetime,
+        "ModelExplainabilityBaselineConfig": ModelExplainabilityBaselineConfigTypeDef,
+        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationOutputTypeDef,
+        "ModelExplainabilityJobInput": ModelExplainabilityJobInputOutputTypeDef,
+        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
         "RoleArn": str,
-        "ModelBiasBaselineConfig": NotRequired[ModelBiasBaselineConfigTypeDef],
-        "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
-        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeModelBiasJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelBiasJobDefinitionResponseTypeDef",
+DescribeModelQualityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelQualityJobDefinitionResponseTypeDef",
     {
         "JobDefinitionArn": str,
         "JobDefinitionName": str,
         "CreationTime": datetime,
-        "ModelBiasBaselineConfig": ModelBiasBaselineConfigTypeDef,
-        "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
-        "ModelBiasJobInput": ModelBiasJobInputTypeDef,
-        "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "ModelQualityBaselineConfig": ModelQualityBaselineConfigTypeDef,
+        "ModelQualityAppSpecification": ModelQualityAppSpecificationOutputTypeDef,
+        "ModelQualityJobInput": ModelQualityJobInputOutputTypeDef,
+        "ModelQualityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
         "RoleArn": str,
         "StoppingCondition": MonitoringStoppingConditionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
+MonitoringJobDefinitionOutputTypeDef = TypedDict(
+    "MonitoringJobDefinitionOutputTypeDef",
+    {
+        "MonitoringInputs": List[MonitoringInputOutputTypeDef],
+        "MonitoringOutputConfig": MonitoringOutputConfigOutputTypeDef,
+        "MonitoringResources": MonitoringResourcesTypeDef,
+        "MonitoringAppSpecification": MonitoringAppSpecificationOutputTypeDef,
+        "RoleArn": str,
+        "BaselineConfig": NotRequired[MonitoringBaselineConfigTypeDef],
+        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
+        "Environment": NotRequired[Dict[str, str]],
+        "NetworkConfig": NotRequired[NetworkConfigOutputTypeDef],
+    },
+)
+CreateDataQualityJobDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateDataQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
-        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
-        "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
-        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
+        "DataQualityJobInput": DataQualityJobInputTypeDef,
+        "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
         "RoleArn": str,
-        "ModelExplainabilityBaselineConfig": NotRequired[ModelExplainabilityBaselineConfigTypeDef],
+        "DataQualityBaselineConfig": NotRequired[DataQualityBaselineConfigTypeDef],
         "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
         "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-DescribeModelExplainabilityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
+DataQualityJobInputUnionTypeDef = Union[
+    DataQualityJobInputTypeDef, DataQualityJobInputOutputTypeDef
+]
+CreateModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateModelBiasJobDefinitionRequestRequestTypeDef",
     {
-        "JobDefinitionArn": str,
         "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelExplainabilityBaselineConfig": ModelExplainabilityBaselineConfigTypeDef,
-        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
-        "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
-        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
+        "ModelBiasJobInput": ModelBiasJobInputTypeDef,
+        "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigTypeDef,
         "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ModelBiasBaselineConfig": NotRequired[ModelBiasBaselineConfigTypeDef],
+        "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
+        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-CreateModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateModelQualityJobDefinitionRequestRequestTypeDef",
+ModelBiasJobInputUnionTypeDef = Union[ModelBiasJobInputTypeDef, ModelBiasJobInputOutputTypeDef]
+CreateModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
-        "ModelQualityAppSpecification": ModelQualityAppSpecificationTypeDef,
-        "ModelQualityJobInput": ModelQualityJobInputTypeDef,
-        "ModelQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
+        "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
+        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
         "RoleArn": str,
-        "ModelQualityBaselineConfig": NotRequired[ModelQualityBaselineConfigTypeDef],
+        "ModelExplainabilityBaselineConfig": NotRequired[ModelExplainabilityBaselineConfigTypeDef],
         "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
         "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-DescribeModelQualityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelQualityJobDefinitionResponseTypeDef",
+ModelExplainabilityJobInputUnionTypeDef = Union[
+    ModelExplainabilityJobInputTypeDef, ModelExplainabilityJobInputOutputTypeDef
+]
+CreateModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateModelQualityJobDefinitionRequestRequestTypeDef",
     {
-        "JobDefinitionArn": str,
         "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelQualityBaselineConfig": ModelQualityBaselineConfigTypeDef,
         "ModelQualityAppSpecification": ModelQualityAppSpecificationTypeDef,
         "ModelQualityJobInput": ModelQualityJobInputTypeDef,
         "ModelQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
         "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigTypeDef,
         "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ModelQualityBaselineConfig": NotRequired[ModelQualityBaselineConfigTypeDef],
+        "NetworkConfig": NotRequired[MonitoringNetworkConfigTypeDef],
+        "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+ModelQualityJobInputUnionTypeDef = Union[
+    ModelQualityJobInputTypeDef, ModelQualityJobInputOutputTypeDef
+]
 MonitoringJobDefinitionTypeDef = TypedDict(
     "MonitoringJobDefinitionTypeDef",
     {
         "MonitoringInputs": Sequence[MonitoringInputTypeDef],
         "MonitoringOutputConfig": MonitoringOutputConfigTypeDef,
         "MonitoringResources": MonitoringResourcesTypeDef,
         "MonitoringAppSpecification": MonitoringAppSpecificationTypeDef,
         "RoleArn": str,
         "BaselineConfig": NotRequired[MonitoringBaselineConfigTypeDef],
         "StoppingCondition": NotRequired[MonitoringStoppingConditionTypeDef],
         "Environment": NotRequired[Mapping[str, str]],
         "NetworkConfig": NotRequired[NetworkConfigTypeDef],
     },
 )
-ModelPackageValidationProfilePaginatorTypeDef = TypedDict(
-    "ModelPackageValidationProfilePaginatorTypeDef",
+ModelPackageValidationProfileExtraOutputTypeDef = TypedDict(
+    "ModelPackageValidationProfileExtraOutputTypeDef",
+    {
+        "ProfileName": str,
+        "TransformJobDefinition": TransformJobDefinitionExtraOutputTypeDef,
+    },
+)
+AlgorithmValidationProfileOutputTypeDef = TypedDict(
+    "AlgorithmValidationProfileOutputTypeDef",
     {
         "ProfileName": str,
-        "TransformJobDefinition": TransformJobDefinitionPaginatorTypeDef,
+        "TrainingJobDefinition": TrainingJobDefinitionOutputTypeDef,
+        "TransformJobDefinition": NotRequired[TransformJobDefinitionOutputTypeDef],
+    },
+)
+ModelPackageValidationProfileOutputTypeDef = TypedDict(
+    "ModelPackageValidationProfileOutputTypeDef",
+    {
+        "ProfileName": str,
+        "TransformJobDefinition": TransformJobDefinitionOutputTypeDef,
     },
 )
 AlgorithmValidationProfileTypeDef = TypedDict(
     "AlgorithmValidationProfileTypeDef",
     {
         "ProfileName": str,
         "TrainingJobDefinition": TrainingJobDefinitionTypeDef,
@@ -13647,96 +14752,132 @@
 ModelPackageValidationProfileTypeDef = TypedDict(
     "ModelPackageValidationProfileTypeDef",
     {
         "ProfileName": str,
         "TransformJobDefinition": TransformJobDefinitionTypeDef,
     },
 )
-TrialComponentSourceDetailPaginatorTypeDef = TypedDict(
-    "TrialComponentSourceDetailPaginatorTypeDef",
-    {
-        "SourceArn": NotRequired[str],
-        "TrainingJob": NotRequired[TrainingJobPaginatorTypeDef],
-        "ProcessingJob": NotRequired[ProcessingJobPaginatorTypeDef],
-        "TransformJob": NotRequired[TransformJobTypeDef],
-    },
-)
 TrialComponentSourceDetailTypeDef = TypedDict(
     "TrialComponentSourceDetailTypeDef",
     {
         "SourceArn": NotRequired[str],
         "TrainingJob": NotRequired[TrainingJobTypeDef],
         "ProcessingJob": NotRequired[ProcessingJobTypeDef],
         "TransformJob": NotRequired[TransformJobTypeDef],
     },
 )
+CreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
+    "CreateHyperParameterTuningJobRequestRequestTypeDef",
+    {
+        "HyperParameterTuningJobName": str,
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
+        "TrainingJobDefinition": NotRequired[HyperParameterTrainingJobDefinitionTypeDef],
+        "TrainingJobDefinitions": NotRequired[
+            Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef]
+        ],
+        "WarmStartConfig": NotRequired[HyperParameterTuningJobWarmStartConfigTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "Autotune": NotRequired[AutotuneTypeDef],
+    },
+)
 GetScalingConfigurationRecommendationResponseTypeDef = TypedDict(
     "GetScalingConfigurationRecommendationResponseTypeDef",
     {
         "InferenceRecommendationsJobName": str,
         "RecommendationId": str,
         "EndpointName": str,
         "TargetCpuUtilizationPerCore": int,
         "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
         "Metric": ScalingPolicyMetricTypeDef,
         "DynamicScalingConfiguration": DynamicScalingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateModelInputRequestTypeDef = TypedDict(
+    "CreateModelInputRequestTypeDef",
+    {
+        "ModelName": str,
+        "PrimaryContainer": NotRequired[ContainerDefinitionTypeDef],
+        "Containers": NotRequired[Sequence[ContainerDefinitionUnionTypeDef]],
+        "InferenceExecutionConfig": NotRequired[InferenceExecutionConfigTypeDef],
+        "ExecutionRoleArn": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "VpcConfig": NotRequired[VpcConfigTypeDef],
+        "EnableNetworkIsolation": NotRequired[bool],
+    },
+)
 BatchDescribeModelPackageSummaryTypeDef = TypedDict(
     "BatchDescribeModelPackageSummaryTypeDef",
     {
         "ModelPackageGroupName": str,
         "ModelPackageArn": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
         "ModelPackageVersion": NotRequired[int],
         "ModelPackageDescription": NotRequired[str],
         "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
     },
 )
-UpdateModelPackageInputRequestTypeDef = TypedDict(
-    "UpdateModelPackageInputRequestTypeDef",
+AdditionalInferenceSpecificationDefinitionUnionTypeDef = Union[
+    AdditionalInferenceSpecificationDefinitionTypeDef,
+    AdditionalInferenceSpecificationDefinitionExtraOutputTypeDef,
+]
+InferenceSpecificationUnionTypeDef = Union[
+    InferenceSpecificationTypeDef, InferenceSpecificationExtraOutputTypeDef
+]
+SourceAlgorithmSpecificationUnionTypeDef = Union[
+    SourceAlgorithmSpecificationTypeDef, SourceAlgorithmSpecificationExtraOutputTypeDef
+]
+MonitoringScheduleConfigExtraOutputTypeDef = TypedDict(
+    "MonitoringScheduleConfigExtraOutputTypeDef",
     {
-        "ModelPackageArn": str,
-        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
-        "ApprovalDescription": NotRequired[str],
-        "CustomerMetadataProperties": NotRequired[Mapping[str, str]],
-        "CustomerMetadataPropertiesToRemove": NotRequired[Sequence[str]],
-        "AdditionalInferenceSpecificationsToAdd": NotRequired[
-            Sequence[AdditionalInferenceSpecificationDefinitionTypeDef]
-        ],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "SourceUri": NotRequired[str],
+        "ScheduleConfig": NotRequired[ScheduleConfigTypeDef],
+        "MonitoringJobDefinition": NotRequired[MonitoringJobDefinitionExtraOutputTypeDef],
+        "MonitoringJobDefinitionName": NotRequired[str],
+        "MonitoringType": NotRequired[MonitoringTypeType],
     },
 )
-MonitoringScheduleConfigPaginatorTypeDef = TypedDict(
-    "MonitoringScheduleConfigPaginatorTypeDef",
+MonitoringScheduleConfigOutputTypeDef = TypedDict(
+    "MonitoringScheduleConfigOutputTypeDef",
     {
         "ScheduleConfig": NotRequired[ScheduleConfigTypeDef],
-        "MonitoringJobDefinition": NotRequired[MonitoringJobDefinitionPaginatorTypeDef],
+        "MonitoringJobDefinition": NotRequired[MonitoringJobDefinitionOutputTypeDef],
         "MonitoringJobDefinitionName": NotRequired[str],
         "MonitoringType": NotRequired[MonitoringTypeType],
     },
 )
 MonitoringScheduleConfigTypeDef = TypedDict(
     "MonitoringScheduleConfigTypeDef",
     {
         "ScheduleConfig": NotRequired[ScheduleConfigTypeDef],
         "MonitoringJobDefinition": NotRequired[MonitoringJobDefinitionTypeDef],
         "MonitoringJobDefinitionName": NotRequired[str],
         "MonitoringType": NotRequired[MonitoringTypeType],
     },
 )
-ModelPackageValidationSpecificationPaginatorTypeDef = TypedDict(
-    "ModelPackageValidationSpecificationPaginatorTypeDef",
+ModelPackageValidationSpecificationExtraOutputTypeDef = TypedDict(
+    "ModelPackageValidationSpecificationExtraOutputTypeDef",
+    {
+        "ValidationRole": str,
+        "ValidationProfiles": List[ModelPackageValidationProfileExtraOutputTypeDef],
+    },
+)
+AlgorithmValidationSpecificationOutputTypeDef = TypedDict(
+    "AlgorithmValidationSpecificationOutputTypeDef",
     {
         "ValidationRole": str,
-        "ValidationProfiles": List[ModelPackageValidationProfilePaginatorTypeDef],
+        "ValidationProfiles": List[AlgorithmValidationProfileOutputTypeDef],
+    },
+)
+ModelPackageValidationSpecificationOutputTypeDef = TypedDict(
+    "ModelPackageValidationSpecificationOutputTypeDef",
+    {
+        "ValidationRole": str,
+        "ValidationProfiles": List[ModelPackageValidationProfileOutputTypeDef],
     },
 )
 AlgorithmValidationSpecificationTypeDef = TypedDict(
     "AlgorithmValidationSpecificationTypeDef",
     {
         "ValidationRole": str,
         "ValidationProfiles": Sequence[AlgorithmValidationProfileTypeDef],
@@ -13745,40 +14886,14 @@
 ModelPackageValidationSpecificationTypeDef = TypedDict(
     "ModelPackageValidationSpecificationTypeDef",
     {
         "ValidationRole": str,
         "ValidationProfiles": Sequence[ModelPackageValidationProfileTypeDef],
     },
 )
-TrialComponentPaginatorTypeDef = TypedDict(
-    "TrialComponentPaginatorTypeDef",
-    {
-        "TrialComponentName": NotRequired[str],
-        "DisplayName": NotRequired[str],
-        "TrialComponentArn": NotRequired[str],
-        "Source": NotRequired[TrialComponentSourceTypeDef],
-        "Status": NotRequired[TrialComponentStatusTypeDef],
-        "StartTime": NotRequired[datetime],
-        "EndTime": NotRequired[datetime],
-        "CreationTime": NotRequired[datetime],
-        "CreatedBy": NotRequired[UserContextTypeDef],
-        "LastModifiedTime": NotRequired[datetime],
-        "LastModifiedBy": NotRequired[UserContextTypeDef],
-        "Parameters": NotRequired[Dict[str, TrialComponentParameterValueTypeDef]],
-        "InputArtifacts": NotRequired[Dict[str, TrialComponentArtifactTypeDef]],
-        "OutputArtifacts": NotRequired[Dict[str, TrialComponentArtifactTypeDef]],
-        "Metrics": NotRequired[List[TrialComponentMetricSummaryTypeDef]],
-        "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
-        "SourceDetail": NotRequired[TrialComponentSourceDetailPaginatorTypeDef],
-        "LineageGroupArn": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "Parents": NotRequired[List[ParentTypeDef]],
-        "RunName": NotRequired[str],
-    },
-)
 TrialComponentTypeDef = TypedDict(
     "TrialComponentTypeDef",
     {
         "TrialComponentName": NotRequired[str],
         "DisplayName": NotRequired[str],
         "TrialComponentArn": NotRequired[str],
         "Source": NotRequired[TrialComponentSourceTypeDef],
@@ -13805,66 +14920,40 @@
     "BatchDescribeModelPackageOutputTypeDef",
     {
         "ModelPackageSummaries": Dict[str, BatchDescribeModelPackageSummaryTypeDef],
         "BatchDescribeModelPackageErrorMap": Dict[str, BatchDescribeModelPackageErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ModelDashboardMonitoringSchedulePaginatorTypeDef = TypedDict(
-    "ModelDashboardMonitoringSchedulePaginatorTypeDef",
-    {
-        "MonitoringScheduleArn": NotRequired[str],
-        "MonitoringScheduleName": NotRequired[str],
-        "MonitoringScheduleStatus": NotRequired[ScheduleStatusType],
-        "MonitoringType": NotRequired[MonitoringTypeType],
-        "FailureReason": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigPaginatorTypeDef],
-        "EndpointName": NotRequired[str],
-        "MonitoringAlertSummaries": NotRequired[List[MonitoringAlertSummaryTypeDef]],
-        "LastMonitoringExecutionSummary": NotRequired[MonitoringExecutionSummaryTypeDef],
-        "BatchTransformInput": NotRequired[BatchTransformInputPaginatorTypeDef],
-    },
-)
-MonitoringSchedulePaginatorTypeDef = TypedDict(
-    "MonitoringSchedulePaginatorTypeDef",
-    {
-        "MonitoringScheduleArn": NotRequired[str],
-        "MonitoringScheduleName": NotRequired[str],
-        "MonitoringScheduleStatus": NotRequired[ScheduleStatusType],
-        "MonitoringType": NotRequired[MonitoringTypeType],
-        "FailureReason": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
-        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigPaginatorTypeDef],
-        "EndpointName": NotRequired[str],
-        "LastMonitoringExecutionSummary": NotRequired[MonitoringExecutionSummaryTypeDef],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
-CreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "CreateMonitoringScheduleRequestRequestTypeDef",
+UpdateModelPackageInputRequestTypeDef = TypedDict(
+    "UpdateModelPackageInputRequestTypeDef",
     {
-        "MonitoringScheduleName": str,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "ModelPackageArn": str,
+        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
+        "ApprovalDescription": NotRequired[str],
+        "CustomerMetadataProperties": NotRequired[Mapping[str, str]],
+        "CustomerMetadataPropertiesToRemove": NotRequired[Sequence[str]],
+        "AdditionalInferenceSpecificationsToAdd": NotRequired[
+            Sequence[AdditionalInferenceSpecificationDefinitionUnionTypeDef]
+        ],
+        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
+        "SourceUri": NotRequired[str],
     },
 )
 DescribeMonitoringScheduleResponseTypeDef = TypedDict(
     "DescribeMonitoringScheduleResponseTypeDef",
     {
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
         "MonitoringScheduleStatus": ScheduleStatusType,
         "MonitoringType": MonitoringTypeType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigOutputTypeDef,
         "EndpointName": str,
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ModelDashboardMonitoringScheduleTypeDef = TypedDict(
     "ModelDashboardMonitoringScheduleTypeDef",
@@ -13872,147 +14961,84 @@
         "MonitoringScheduleArn": NotRequired[str],
         "MonitoringScheduleName": NotRequired[str],
         "MonitoringScheduleStatus": NotRequired[ScheduleStatusType],
         "MonitoringType": NotRequired[MonitoringTypeType],
         "FailureReason": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
-        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigTypeDef],
+        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigOutputTypeDef],
         "EndpointName": NotRequired[str],
         "MonitoringAlertSummaries": NotRequired[List[MonitoringAlertSummaryTypeDef]],
         "LastMonitoringExecutionSummary": NotRequired[MonitoringExecutionSummaryTypeDef],
-        "BatchTransformInput": NotRequired[BatchTransformInputTypeDef],
+        "BatchTransformInput": NotRequired[BatchTransformInputOutputTypeDef],
     },
 )
 MonitoringScheduleTypeDef = TypedDict(
     "MonitoringScheduleTypeDef",
     {
         "MonitoringScheduleArn": NotRequired[str],
         "MonitoringScheduleName": NotRequired[str],
         "MonitoringScheduleStatus": NotRequired[ScheduleStatusType],
         "MonitoringType": NotRequired[MonitoringTypeType],
         "FailureReason": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "LastModifiedTime": NotRequired[datetime],
-        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigTypeDef],
+        "MonitoringScheduleConfig": NotRequired[MonitoringScheduleConfigOutputTypeDef],
         "EndpointName": NotRequired[str],
         "LastMonitoringExecutionSummary": NotRequired[MonitoringExecutionSummaryTypeDef],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "UpdateMonitoringScheduleRequestRequestTypeDef",
+CreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "CreateMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-ModelPackagePaginatorTypeDef = TypedDict(
-    "ModelPackagePaginatorTypeDef",
-    {
-        "ModelPackageName": NotRequired[str],
-        "ModelPackageGroupName": NotRequired[str],
-        "ModelPackageVersion": NotRequired[int],
-        "ModelPackageArn": NotRequired[str],
-        "ModelPackageDescription": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationPaginatorTypeDef],
-        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationPaginatorTypeDef],
-        "ModelPackageStatus": NotRequired[ModelPackageStatusType],
-        "ModelPackageStatusDetails": NotRequired[ModelPackageStatusDetailsTypeDef],
-        "CertifyForMarketplace": NotRequired[bool],
-        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
-        "CreatedBy": NotRequired[UserContextTypeDef],
-        "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
-        "ModelMetrics": NotRequired[ModelMetricsTypeDef],
-        "LastModifiedTime": NotRequired[datetime],
-        "LastModifiedBy": NotRequired[UserContextTypeDef],
-        "ApprovalDescription": NotRequired[str],
-        "Domain": NotRequired[str],
-        "Task": NotRequired[str],
-        "SamplePayloadUrl": NotRequired[str],
-        "AdditionalInferenceSpecifications": NotRequired[
-            List[AdditionalInferenceSpecificationDefinitionPaginatorTypeDef]
-        ],
-        "SourceUri": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "CustomerMetadataProperties": NotRequired[Dict[str, str]],
-        "DriftCheckBaselines": NotRequired[DriftCheckBaselinesTypeDef],
-        "SkipModelValidation": NotRequired[SkipModelValidationType],
-    },
-)
-CreateAlgorithmInputRequestTypeDef = TypedDict(
-    "CreateAlgorithmInputRequestTypeDef",
+MonitoringScheduleConfigUnionTypeDef = Union[
+    MonitoringScheduleConfigTypeDef, MonitoringScheduleConfigExtraOutputTypeDef
+]
+UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "UpdateMonitoringScheduleRequestRequestTypeDef",
     {
-        "AlgorithmName": str,
-        "TrainingSpecification": TrainingSpecificationTypeDef,
-        "AlgorithmDescription": NotRequired[str],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "ValidationSpecification": NotRequired[AlgorithmValidationSpecificationTypeDef],
-        "CertifyForMarketplace": NotRequired[bool],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "MonitoringScheduleName": str,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
     },
 )
 DescribeAlgorithmOutputTypeDef = TypedDict(
     "DescribeAlgorithmOutputTypeDef",
     {
         "AlgorithmName": str,
         "AlgorithmArn": str,
         "AlgorithmDescription": str,
         "CreationTime": datetime,
-        "TrainingSpecification": TrainingSpecificationTypeDef,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
-        "ValidationSpecification": AlgorithmValidationSpecificationTypeDef,
+        "TrainingSpecification": TrainingSpecificationOutputTypeDef,
+        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
+        "ValidationSpecification": AlgorithmValidationSpecificationOutputTypeDef,
         "AlgorithmStatus": AlgorithmStatusType,
         "AlgorithmStatusDetails": AlgorithmStatusDetailsTypeDef,
         "ProductId": str,
         "CertifyForMarketplace": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateModelPackageInputRequestTypeDef = TypedDict(
-    "CreateModelPackageInputRequestTypeDef",
-    {
-        "ModelPackageName": NotRequired[str],
-        "ModelPackageGroupName": NotRequired[str],
-        "ModelPackageDescription": NotRequired[str],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationTypeDef],
-        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationTypeDef],
-        "CertifyForMarketplace": NotRequired[bool],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
-        "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
-        "ModelMetrics": NotRequired[ModelMetricsTypeDef],
-        "ClientToken": NotRequired[str],
-        "Domain": NotRequired[str],
-        "Task": NotRequired[str],
-        "SamplePayloadUrl": NotRequired[str],
-        "CustomerMetadataProperties": NotRequired[Mapping[str, str]],
-        "DriftCheckBaselines": NotRequired[DriftCheckBaselinesTypeDef],
-        "AdditionalInferenceSpecifications": NotRequired[
-            Sequence[AdditionalInferenceSpecificationDefinitionTypeDef]
-        ],
-        "SkipModelValidation": NotRequired[SkipModelValidationType],
-        "SourceUri": NotRequired[str],
-    },
-)
 DescribeModelPackageOutputTypeDef = TypedDict(
     "DescribeModelPackageOutputTypeDef",
     {
         "ModelPackageName": str,
         "ModelPackageGroupName": str,
         "ModelPackageVersion": int,
         "ModelPackageArn": str,
         "ModelPackageDescription": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
-        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
-        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
+        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
+        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationOutputTypeDef,
+        "ValidationSpecification": ModelPackageValidationSpecificationOutputTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
         "ModelPackageStatusDetails": ModelPackageStatusDetailsTypeDef,
         "CertifyForMarketplace": bool,
         "ModelApprovalStatus": ModelApprovalStatusType,
         "CreatedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
         "ModelMetrics": ModelMetricsTypeDef,
@@ -14021,15 +15047,15 @@
         "ApprovalDescription": str,
         "Domain": str,
         "Task": str,
         "SamplePayloadUrl": str,
         "CustomerMetadataProperties": Dict[str, str],
         "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
         "AdditionalInferenceSpecifications": List[
-            AdditionalInferenceSpecificationDefinitionTypeDef
+            AdditionalInferenceSpecificationDefinitionOutputTypeDef
         ],
         "SkipModelValidation": SkipModelValidationType,
         "SourceUri": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ModelPackageTypeDef = TypedDict(
@@ -14037,67 +15063,86 @@
     {
         "ModelPackageName": NotRequired[str],
         "ModelPackageGroupName": NotRequired[str],
         "ModelPackageVersion": NotRequired[int],
         "ModelPackageArn": NotRequired[str],
         "ModelPackageDescription": NotRequired[str],
         "CreationTime": NotRequired[datetime],
-        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
-        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationTypeDef],
-        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationTypeDef],
+        "InferenceSpecification": NotRequired[InferenceSpecificationOutputTypeDef],
+        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationOutputTypeDef],
+        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationOutputTypeDef],
         "ModelPackageStatus": NotRequired[ModelPackageStatusType],
         "ModelPackageStatusDetails": NotRequired[ModelPackageStatusDetailsTypeDef],
         "CertifyForMarketplace": NotRequired[bool],
         "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
         "CreatedBy": NotRequired[UserContextTypeDef],
         "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
         "ModelMetrics": NotRequired[ModelMetricsTypeDef],
         "LastModifiedTime": NotRequired[datetime],
         "LastModifiedBy": NotRequired[UserContextTypeDef],
         "ApprovalDescription": NotRequired[str],
         "Domain": NotRequired[str],
         "Task": NotRequired[str],
         "SamplePayloadUrl": NotRequired[str],
         "AdditionalInferenceSpecifications": NotRequired[
-            List[AdditionalInferenceSpecificationDefinitionTypeDef]
+            List[AdditionalInferenceSpecificationDefinitionOutputTypeDef]
         ],
         "SourceUri": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
         "CustomerMetadataProperties": NotRequired[Dict[str, str]],
         "DriftCheckBaselines": NotRequired[DriftCheckBaselinesTypeDef],
         "SkipModelValidation": NotRequired[SkipModelValidationType],
     },
 )
-ModelDashboardModelPaginatorTypeDef = TypedDict(
-    "ModelDashboardModelPaginatorTypeDef",
+AlgorithmValidationSpecificationUnionTypeDef = Union[
+    AlgorithmValidationSpecificationTypeDef, AlgorithmValidationSpecificationOutputTypeDef
+]
+CreateAlgorithmInputRequestTypeDef = TypedDict(
+    "CreateAlgorithmInputRequestTypeDef",
     {
-        "Model": NotRequired[ModelPaginatorTypeDef],
-        "Endpoints": NotRequired[List[ModelDashboardEndpointTypeDef]],
-        "LastBatchTransformJob": NotRequired[TransformJobTypeDef],
-        "MonitoringSchedules": NotRequired[List[ModelDashboardMonitoringSchedulePaginatorTypeDef]],
-        "ModelCard": NotRequired[ModelDashboardModelCardTypeDef],
+        "AlgorithmName": str,
+        "TrainingSpecification": TrainingSpecificationTypeDef,
+        "AlgorithmDescription": NotRequired[str],
+        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
+        "ValidationSpecification": NotRequired[AlgorithmValidationSpecificationTypeDef],
+        "CertifyForMarketplace": NotRequired[bool],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-EndpointPaginatorTypeDef = TypedDict(
-    "EndpointPaginatorTypeDef",
+CreateModelPackageInputRequestTypeDef = TypedDict(
+    "CreateModelPackageInputRequestTypeDef",
     {
-        "EndpointName": str,
-        "EndpointArn": str,
-        "EndpointConfigName": str,
-        "EndpointStatus": EndpointStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ProductionVariants": NotRequired[List[ProductionVariantSummaryTypeDef]],
-        "DataCaptureConfig": NotRequired[DataCaptureConfigSummaryTypeDef],
-        "FailureReason": NotRequired[str],
-        "MonitoringSchedules": NotRequired[List[MonitoringSchedulePaginatorTypeDef]],
-        "Tags": NotRequired[List[TagTypeDef]],
-        "ShadowProductionVariants": NotRequired[List[ProductionVariantSummaryTypeDef]],
+        "ModelPackageName": NotRequired[str],
+        "ModelPackageGroupName": NotRequired[str],
+        "ModelPackageDescription": NotRequired[str],
+        "InferenceSpecification": NotRequired[InferenceSpecificationTypeDef],
+        "ValidationSpecification": NotRequired[ModelPackageValidationSpecificationTypeDef],
+        "SourceAlgorithmSpecification": NotRequired[SourceAlgorithmSpecificationTypeDef],
+        "CertifyForMarketplace": NotRequired[bool],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "ModelApprovalStatus": NotRequired[ModelApprovalStatusType],
+        "MetadataProperties": NotRequired[MetadataPropertiesTypeDef],
+        "ModelMetrics": NotRequired[ModelMetricsTypeDef],
+        "ClientToken": NotRequired[str],
+        "Domain": NotRequired[str],
+        "Task": NotRequired[str],
+        "SamplePayloadUrl": NotRequired[str],
+        "CustomerMetadataProperties": NotRequired[Mapping[str, str]],
+        "DriftCheckBaselines": NotRequired[DriftCheckBaselinesTypeDef],
+        "AdditionalInferenceSpecifications": NotRequired[
+            Sequence[AdditionalInferenceSpecificationDefinitionUnionTypeDef]
+        ],
+        "SkipModelValidation": NotRequired[SkipModelValidationType],
+        "SourceUri": NotRequired[str],
     },
 )
+ModelPackageValidationSpecificationUnionTypeDef = Union[
+    ModelPackageValidationSpecificationTypeDef,
+    ModelPackageValidationSpecificationExtraOutputTypeDef,
+]
 ModelDashboardModelTypeDef = TypedDict(
     "ModelDashboardModelTypeDef",
     {
         "Model": NotRequired[ModelTypeDef],
         "Endpoints": NotRequired[List[ModelDashboardEndpointTypeDef]],
         "LastBatchTransformJob": NotRequired[TransformJobTypeDef],
         "MonitoringSchedules": NotRequired[List[ModelDashboardMonitoringScheduleTypeDef]],
@@ -14117,34 +15162,14 @@
         "DataCaptureConfig": NotRequired[DataCaptureConfigSummaryTypeDef],
         "FailureReason": NotRequired[str],
         "MonitoringSchedules": NotRequired[List[MonitoringScheduleTypeDef]],
         "Tags": NotRequired[List[TagTypeDef]],
         "ShadowProductionVariants": NotRequired[List[ProductionVariantSummaryTypeDef]],
     },
 )
-SearchRecordPaginatorTypeDef = TypedDict(
-    "SearchRecordPaginatorTypeDef",
-    {
-        "TrainingJob": NotRequired[TrainingJobPaginatorTypeDef],
-        "Experiment": NotRequired[ExperimentTypeDef],
-        "Trial": NotRequired[TrialTypeDef],
-        "TrialComponent": NotRequired[TrialComponentPaginatorTypeDef],
-        "Endpoint": NotRequired[EndpointPaginatorTypeDef],
-        "ModelPackage": NotRequired[ModelPackagePaginatorTypeDef],
-        "ModelPackageGroup": NotRequired[ModelPackageGroupTypeDef],
-        "Pipeline": NotRequired[PipelineTypeDef],
-        "PipelineExecution": NotRequired[PipelineExecutionTypeDef],
-        "FeatureGroup": NotRequired[FeatureGroupTypeDef],
-        "FeatureMetadata": NotRequired[FeatureMetadataTypeDef],
-        "Project": NotRequired[ProjectPaginatorTypeDef],
-        "HyperParameterTuningJob": NotRequired[HyperParameterTuningJobSearchEntityPaginatorTypeDef],
-        "ModelCard": NotRequired[ModelCardTypeDef],
-        "Model": NotRequired[ModelDashboardModelPaginatorTypeDef],
-    },
-)
 SearchRecordTypeDef = TypedDict(
     "SearchRecordTypeDef",
     {
         "TrainingJob": NotRequired[TrainingJobTypeDef],
         "Experiment": NotRequired[ExperimentTypeDef],
         "Trial": NotRequired[TrialTypeDef],
         "TrialComponent": NotRequired[TrialComponentTypeDef],
@@ -14157,23 +15182,15 @@
         "FeatureMetadata": NotRequired[FeatureMetadataTypeDef],
         "Project": NotRequired[ProjectTypeDef],
         "HyperParameterTuningJob": NotRequired[HyperParameterTuningJobSearchEntityTypeDef],
         "ModelCard": NotRequired[ModelCardTypeDef],
         "Model": NotRequired[ModelDashboardModelTypeDef],
     },
 )
-SearchResponsePaginatorTypeDef = TypedDict(
-    "SearchResponsePaginatorTypeDef",
-    {
-        "Results": List[SearchRecordPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 SearchResponseTypeDef = TypedDict(
     "SearchResponseTypeDef",
     {
         "Results": List[SearchRecordTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/waiter.py` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker/waiter.pyi` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/PKG-INFO` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.34.89
-Summary: Type annotations for boto3.SageMaker 1.34.89 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.95
+Summary: Type annotations for boto3.SageMaker 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker)](https://pepy.tech/project/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_sagemaker-1.34.89/mypy_boto3_sagemaker.egg-info/SOURCES.txt` & `mypy_boto3_sagemaker-1.34.95/mypy_boto3_sagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_sagemaker-1.34.89/setup.py` & `mypy_boto3_sagemaker-1.34.95/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker",
-    version="1.34.89",
+    version="1.34.95",
     packages=["mypy_boto3_sagemaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.SageMaker 1.34.89 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.SageMaker 1.34.95 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

