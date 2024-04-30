# Comparing `tmp/iam_actions-1.2.20240428.tar.gz` & `tmp/iam_actions-1.2.20240429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240428.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240429.tar", max compression
```

## Comparing `iam_actions-1.2.20240428.tar` & `iam_actions-1.2.20240429.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/README.md
--rw-r--r--   0        0        0      228 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/__init__.py
--rw-r--r--   0        0        0  4812377 2024-04-28 02:24:37.141976 iam_actions-1.2.20240428/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-28 02:22:41.069928 iam_actions-1.2.20240428/iam_actions/generate/services.py
--rw-r--r--   0        0        0   625917 2024-04-28 02:24:37.141976 iam_actions-1.2.20240428/iam_actions/policies.json
--rw-r--r--   0        0        0   209050 2024-04-28 02:24:37.141976 iam_actions-1.2.20240428/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   607313 2024-04-28 02:24:37.141976 iam_actions-1.2.20240428/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-28 02:24:37.805976 iam_actions-1.2.20240428/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240428/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240428/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/README.md
+-rw-r--r--   0        0        0      228 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4812377 2024-04-29 02:20:49.578845 iam_actions-1.2.20240429/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   625917 2024-04-29 02:20:49.578845 iam_actions-1.2.20240429/iam_actions/policies.json
+-rw-r--r--   0        0        0   209050 2024-04-29 02:20:49.578845 iam_actions-1.2.20240429/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   607313 2024-04-29 02:20:49.578845 iam_actions-1.2.20240429/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-29 02:20:50.218846 iam_actions-1.2.20240429/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240429/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240429/PKG-INFO
```

### Comparing `iam_actions-1.2.20240428/LICENSE` & `iam_actions-1.2.20240429/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/README.md` & `iam_actions-1.2.20240429/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/actions.json` & `iam_actions-1.2.20240429/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4442,217 +4442,217 @@
             "resources": [
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appfabric": {
-        "ListAppAuthorizations": {
+        "GetAppBundle": {
             "access_level": "Undocumented",
-            "action": "ListAppAuthorizations",
+            "action": "GetAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartUserAccessTasks": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartUserAccessTasks",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIngestionDestination": {
+        "CreateAppBundle": {
             "access_level": "Undocumented",
-            "action": "UpdateIngestionDestination",
+            "action": "CreateAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionDestination": {
+        "ListAppAuthorizations": {
             "access_level": "Undocumented",
-            "action": "GetIngestionDestination",
+            "action": "ListAppAuthorizations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppBundle": {
+        "CreateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "CreateAppBundle",
+            "action": "CreateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppBundle": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetAppBundle",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAuthorization": {
+        "GetIngestion": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAuthorization",
+            "action": "GetIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ConnectAppAuthorization": {
+        "DeleteAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ConnectAppAuthorization",
+            "action": "DeleteAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppBundle": {
+        "ListAppBundles": {
             "access_level": "Undocumented",
-            "action": "DeleteAppBundle",
+            "action": "ListAppBundles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestionDestination": {
+        "ListIngestionDestinations": {
             "access_level": "Undocumented",
-            "action": "CreateIngestionDestination",
+            "action": "ListIngestionDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionDestinations": {
+        "StartIngestion": {
             "access_level": "Undocumented",
-            "action": "ListIngestionDestinations",
+            "action": "StartIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestions": {
+        "ConnectAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ListIngestions",
+            "action": "ConnectAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestion": {
+        "StopIngestion": {
             "access_level": "Undocumented",
-            "action": "StartIngestion",
+            "action": "StopIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestion": {
+        "BatchGetUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestion",
+            "action": "BatchGetUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppAuthorization": {
+        "CreateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "GetAppAuthorization",
+            "action": "CreateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppAuthorization": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateAppAuthorization",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestion": {
+        "CreateIngestion": {
             "access_level": "Undocumented",
-            "action": "GetIngestion",
+            "action": "CreateIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestionDestination": {
+        "GetAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestionDestination",
+            "action": "GetAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestion": {
+        "ListIngestions": {
             "access_level": "Undocumented",
-            "action": "CreateIngestion",
+            "action": "ListIngestions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopIngestion": {
+        "UpdateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "StopIngestion",
+            "action": "UpdateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppAuthorization": {
+        "DeleteIngestion": {
             "access_level": "Undocumented",
-            "action": "CreateAppAuthorization",
+            "action": "DeleteIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteAppBundle": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppBundles": {
+        "DeleteIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "ListAppBundles",
+            "action": "DeleteIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetUserAccessTasks": {
+        "UpdateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "BatchGetUserAccessTasks",
+            "action": "UpdateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "appflow": {
@@ -5170,121 +5170,121 @@
             "condition_keys": [],
             "description": "Grants permission to update an existing Application Cost Profiler Report configuration",
             "orphan": false,
             "resources": []
         }
     },
     "application-transformation": {
-        "StartDeployment": {
+        "StartRuntimeAssessment": {
             "access_level": "Undocumented",
-            "action": "StartDeployment",
+            "action": "StartRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingCompatibilityAssessment": {
+        "StartPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "GetPortingCompatibilityAssessment",
+            "action": "StartPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartGroupingAssessment": {
             "access_level": "Undocumented",
             "action": "StartGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutLogData": {
+        "GetPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "PutLogData",
+            "action": "GetPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingCompatibilityAssessment": {
+        "GetPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "StartPortingCompatibilityAssessment",
+            "action": "GetPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupingAssessment": {
+        "PutLogData": {
             "access_level": "Undocumented",
-            "action": "GetGroupingAssessment",
+            "action": "PutLogData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingRecommendationAssessment": {
+        "StartPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "GetPortingRecommendationAssessment",
+            "action": "StartPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContainerization": {
+        "GetDeployment": {
             "access_level": "Undocumented",
-            "action": "GetContainerization",
+            "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeployment": {
+        "StartContainerization": {
             "access_level": "Undocumented",
-            "action": "GetDeployment",
+            "action": "StartContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingRecommendationAssessment": {
+        "StartDeployment": {
             "access_level": "Undocumented",
-            "action": "StartPortingRecommendationAssessment",
+            "action": "StartDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMetricData": {
+        "GetGroupingAssessment": {
             "access_level": "Undocumented",
-            "action": "PutMetricData",
+            "action": "GetGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRuntimeAssessment": {
+        "GetRuntimeAssessment": {
             "access_level": "Undocumented",
-            "action": "StartRuntimeAssessment",
+            "action": "GetRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRuntimeAssessment": {
+        "PutMetricData": {
             "access_level": "Undocumented",
-            "action": "GetRuntimeAssessment",
+            "action": "PutMetricData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContainerization": {
+        "GetContainerization": {
             "access_level": "Undocumented",
-            "action": "StartContainerization",
+            "action": "GetContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "applicationinsights": {
@@ -11997,225 +11997,225 @@
             "condition_keys": [],
             "description": "Validates Server Migration Connector Id that was registered with AWS Connector Service.",
             "orphan": false,
             "resources": []
         }
     },
     "b2bi": {
-        "UpdateProfile": {
+        "CreateCapability": {
             "access_level": "Undocumented",
-            "action": "UpdateProfile",
+            "action": "CreateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCapability": {
+        "DeletePartnership": {
             "access_level": "Undocumented",
-            "action": "DeleteCapability",
+            "action": "DeletePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCapability": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateCapability",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCapability": {
+        "UpdateProfile": {
             "access_level": "Undocumented",
-            "action": "CreateCapability",
+            "action": "UpdateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestParsing": {
+        "CreateProfile": {
             "access_level": "Undocumented",
-            "action": "TestParsing",
+            "action": "CreateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTransformer": {
+        "GetProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateTransformer",
+            "action": "GetProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteProfile": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTransformer": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteTransformer",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfile": {
+        "GetTransformer": {
             "access_level": "Undocumented",
-            "action": "GetProfile",
+            "action": "GetTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProfile": {
+        "GetTransformerJob": {
             "access_level": "Undocumented",
-            "action": "DeleteProfile",
+            "action": "GetTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapability": {
+        "GetPartnership": {
             "access_level": "Undocumented",
-            "action": "GetCapability",
+            "action": "GetPartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerships": {
+        "CreateTransformer": {
             "access_level": "Undocumented",
-            "action": "ListPartnerships",
+            "action": "CreateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteCapability": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCapabilities": {
+        "TestMapping": {
             "access_level": "Undocumented",
-            "action": "ListCapabilities",
+            "action": "TestMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTransformerJob": {
+        "UpdateCapability": {
             "access_level": "Undocumented",
-            "action": "StartTransformerJob",
+            "action": "UpdateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePartnership": {
+        "ListPartnerships": {
             "access_level": "Undocumented",
-            "action": "DeletePartnership",
+            "action": "ListPartnerships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransformerJob": {
+        "ListTransformers": {
             "access_level": "Undocumented",
-            "action": "GetTransformerJob",
+            "action": "ListTransformers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestMapping": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TestMapping",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListProfiles": {
             "access_level": "Undocumented",
             "action": "ListProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransformers": {
+        "StartTransformerJob": {
             "access_level": "Undocumented",
-            "action": "ListTransformers",
+            "action": "StartTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTransformer": {
+        "GetCapability": {
             "access_level": "Undocumented",
-            "action": "CreateTransformer",
+            "action": "GetCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnership": {
+        "CreatePartnership": {
             "access_level": "Undocumented",
-            "action": "GetPartnership",
+            "action": "CreatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransformer": {
+        "UpdateTransformer": {
             "access_level": "Undocumented",
-            "action": "GetTransformer",
+            "action": "UpdateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProfile": {
+        "DeleteTransformer": {
             "access_level": "Undocumented",
-            "action": "CreateProfile",
+            "action": "DeleteTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "TestParsing": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TestParsing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnership": {
+        "ListCapabilities": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnership",
+            "action": "ListCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePartnership": {
+        "UpdatePartnership": {
             "access_level": "Undocumented",
-            "action": "CreatePartnership",
+            "action": "UpdatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "backup": {
@@ -13849,819 +13849,819 @@
             "orphan": false,
             "resources": [
                 "scheduling-policy"
             ]
         }
     },
     "bcm-data-exports": {
-        "GetExecution": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetExecution",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExport": {
+        "GetExecution": {
             "access_level": "Undocumented",
-            "action": "CreateExport",
+            "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExport": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetExport",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "GetTable": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "GetTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTables": {
+        "ListExports": {
             "access_level": "Undocumented",
-            "action": "ListTables",
+            "action": "ListExports",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateExport": {
+        "CreateExport": {
             "access_level": "Undocumented",
-            "action": "UpdateExport",
+            "action": "CreateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExports": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListExports",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTables": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExport": {
+        "UpdateExport": {
             "access_level": "Undocumented",
-            "action": "DeleteExport",
+            "action": "UpdateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetExport": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteExport": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTable": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "GetTable",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "bedrock": {
-        "GetEvaluationJob": {
+        "GetUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "GetEvaluationJob",
+            "action": "GetUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ApplyGuardrail": {
             "access_level": "Undocumented",
             "action": "ApplyGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeAgent": {
+        "DeleteCustomModel": {
             "access_level": "Undocumented",
-            "action": "InvokeAgent",
+            "action": "DeleteCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEvaluationJobs": {
+        "GetGuardrail": {
             "access_level": "Undocumented",
-            "action": "ListEvaluationJobs",
+            "action": "GetGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelCustomizationJob": {
+        "ListFoundationModelAgreementOffers": {
             "access_level": "Undocumented",
-            "action": "GetModelCustomizationJob",
+            "action": "ListFoundationModelAgreementOffers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUseCaseForModelAccess": {
+        "GetAgentVersion": {
             "access_level": "Undocumented",
-            "action": "PutUseCaseForModelAccess",
+            "action": "GetAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAgentKnowledgeBase": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "AssociateAgentKnowledgeBase",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentKnowledgeBase": {
+        "ListModelInvocationJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentKnowledgeBase",
+            "action": "ListModelInvocationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProvisionedModelThroughput": {
+        "CreateAgent": {
             "access_level": "Undocumented",
-            "action": "GetProvisionedModelThroughput",
+            "action": "CreateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentAlias": {
+        "ListAgentAliases": {
             "access_level": "Undocumented",
-            "action": "GetAgentAlias",
+            "action": "ListAgentAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "DeleteProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "DeleteProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentVersions": {
+        "GetAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListAgentVersions",
+            "action": "GetAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteModelInvocationLoggingConfiguration": {
+        "GetFoundationModel": {
             "access_level": "Undocumented",
-            "action": "DeleteModelInvocationLoggingConfiguration",
+            "action": "GetFoundationModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFoundationModelAgreement": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteFoundationModelAgreement",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "GetIngestionJob": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "GetIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelCustomizationJob": {
+        "UpdateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "StopModelCustomizationJob",
+            "action": "UpdateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUseCaseForModelAccess": {
+        "DeleteModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetUseCaseForModelAccess",
+            "action": "DeleteModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentActionGroups": {
+        "UpdateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "ListAgentActionGroups",
+            "action": "UpdateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelCustomizationJob": {
+        "CreateGuardrailVersion": {
             "access_level": "Undocumented",
-            "action": "CreateModelCustomizationJob",
+            "action": "CreateGuardrailVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelEvaluationJob": {
+        "CreateGuardrail": {
             "access_level": "Undocumented",
-            "action": "GetModelEvaluationJob",
+            "action": "CreateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModel": {
+        "StopModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "InvokeModel",
+            "action": "StopModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelEvaluationJobs": {
+        "GetModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "ListModelEvaluationJobs",
+            "action": "GetModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionJobs": {
+        "DeleteGuardrail": {
             "access_level": "Undocumented",
-            "action": "ListIngestionJobs",
+            "action": "DeleteGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAgentKnowledgeBase": {
+        "ListAgentActionGroups": {
             "access_level": "Undocumented",
-            "action": "DisassociateAgentKnowledgeBase",
+            "action": "ListAgentActionGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomModel": {
+        "AssociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetCustomModel",
+            "action": "AssociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCustomModels": {
+        "ListAgentKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "ListCustomModels",
+            "action": "ListAgentKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgent": {
+        "UpdateGuardrail": {
             "access_level": "Undocumented",
-            "action": "CreateAgent",
+            "action": "UpdateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateThirdPartyKnowledgeBase": {
+        "StartIngestionJob": {
             "access_level": "Undocumented",
-            "action": "AssociateThirdPartyKnowledgeBase",
+            "action": "StartIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetectGeneratedContent": {
+        "GetModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "DetectGeneratedContent",
+            "action": "GetModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentVersion": {
+        "DetectGeneratedContent": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentVersion",
+            "action": "DetectGeneratedContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModelAvailability": {
+        "CreateModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModelAvailability",
+            "action": "CreateModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "GetAgent": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "GetAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelInvocationJob": {
+        "ListAgentVersions": {
             "access_level": "Undocumented",
-            "action": "CreateModelInvocationJob",
+            "action": "ListAgentVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrail": {
+        "ListCustomModels": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrail",
+            "action": "ListCustomModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProvisionedModelThroughput": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteProvisionedModelThroughput",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCustomModel": {
+        "AssociateThirdPartyKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "DeleteCustomModel",
+            "action": "AssociateThirdPartyKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelInvocationJobs": {
+        "CreateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "ListModelInvocationJobs",
+            "action": "CreateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFoundationModelAgreement": {
+        "InvokeModel": {
             "access_level": "Undocumented",
-            "action": "CreateFoundationModelAgreement",
+            "action": "InvokeModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentAliases": {
+        "CreateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "ListAgentAliases",
+            "action": "CreateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentKnowledgeBases": {
+        "ListGuardrails": {
             "access_level": "Undocumented",
-            "action": "ListAgentKnowledgeBases",
+            "action": "ListGuardrails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelEvaluationJob": {
+        "PrepareAgent": {
             "access_level": "Undocumented",
-            "action": "CreateModelEvaluationJob",
+            "action": "PrepareAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentVersion": {
+        "ListModelEvaluationJobs": {
             "access_level": "Undocumented",
-            "action": "GetAgentVersion",
+            "action": "ListModelEvaluationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModelAgreementOffers": {
+        "InvokeAgent": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModelAgreementOffers",
+            "action": "InvokeAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PrepareAgent": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "PrepareAgent",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Retrieve": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "Retrieve",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgents": {
+        "GetFoundationModelAvailability": {
             "access_level": "Undocumented",
-            "action": "ListAgents",
+            "action": "GetFoundationModelAvailability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListFoundationModels": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListFoundationModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEvaluationJob": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "CreateEvaluationJob",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionJob": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "GetIngestionJob",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestionJob": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "StartIngestionJob",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "DeleteAgent": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "DeleteAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModels": {
+        "CreateFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModels",
+            "action": "CreateFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetAgentAlias": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelCustomizationJobs": {
+        "GetModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "ListModelCustomizationJobs",
+            "action": "GetModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentActionGroup": {
+        "ListEvaluationJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentActionGroup",
+            "action": "ListEvaluationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationJob": {
+        "DisassociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationJob",
+            "action": "DisassociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RetrieveAndGenerate": {
+        "UpdateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "RetrieveAndGenerate",
+            "action": "UpdateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProvisionedModelThroughput": {
+        "StopEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateProvisionedModelThroughput",
+            "action": "StopEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentAlias": {
+        "RetrieveAndGenerate": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentAlias",
+            "action": "RetrieveAndGenerate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "DeleteAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "DeleteAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentKnowledgeBase": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetAgentKnowledgeBase",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentAlias": {
+        "CreateModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "CreateAgentAlias",
+            "action": "CreateModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgent": {
+        "Retrieve": {
             "access_level": "Undocumented",
-            "action": "DeleteAgent",
+            "action": "Retrieve",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentActionGroup": {
+        "PutUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "CreateAgentActionGroup",
+            "action": "PutUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKnowledgeBase": {
+        "UpdateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "UpdateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGuardrails": {
+        "InvokeModelWithResponseStream": {
             "access_level": "Undocumented",
-            "action": "ListGuardrails",
+            "action": "InvokeModelWithResponseStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentActionGroup": {
+        "GetProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "GetAgentActionGroup",
+            "action": "GetProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModelWithResponseStream": {
+        "StopModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "InvokeModelWithResponseStream",
+            "action": "StopModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutModelInvocationLoggingConfiguration": {
+        "UpdateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "PutModelInvocationLoggingConfiguration",
+            "action": "UpdateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFoundationModelEntitlement": {
+        "ListIngestionJobs": {
             "access_level": "Undocumented",
-            "action": "PutFoundationModelEntitlement",
+            "action": "ListIngestionJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentActionGroup": {
+        "UpdateAgent": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentActionGroup",
+            "action": "UpdateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModel": {
+        "GetEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModel",
+            "action": "GetEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "ListModelCustomizationJobs": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "ListModelCustomizationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBase": {
+        "CreateEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBase",
+            "action": "CreateEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelInvocationJob": {
+        "GetModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "StopModelInvocationJob",
+            "action": "GetModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopEvaluationJob": {
+        "PutFoundationModelEntitlement": {
             "access_level": "Undocumented",
-            "action": "StopEvaluationJob",
+            "action": "PutFoundationModelEntitlement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedModelThroughputs": {
+        "PutModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedModelThroughputs",
+            "action": "PutModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgent": {
+        "GetCustomModel": {
             "access_level": "Undocumented",
-            "action": "GetAgent",
+            "action": "GetCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationLoggingConfiguration": {
+        "ListProvisionedModelThroughputs": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationLoggingConfiguration",
+            "action": "ListProvisionedModelThroughputs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGuardrail": {
+        "CreateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "GetGuardrail",
+            "action": "CreateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGuardrail": {
+        "DeleteAgentVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteGuardrail",
+            "action": "DeleteAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProvisionedModelThroughput": {
+        "DeleteFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "CreateProvisionedModelThroughput",
+            "action": "DeleteFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgent": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UpdateAgent",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGuardrail": {
+        "CreateModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateGuardrail",
+            "action": "CreateModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteAgentAlias": {
             "access_level": "Undocumented",
             "action": "DeleteAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrailVersion": {
+        "ListAgents": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrailVersion",
+            "action": "ListAgents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billing": {
@@ -14669,105 +14669,105 @@
             "access_level": "Undocumented",
             "action": "GetIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateBillingPreferences": {
+        "GetContractInformation": {
             "access_level": "Undocumented",
-            "action": "UpdateBillingPreferences",
+            "action": "GetContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBillingViews": {
+        "PutContractInformation": {
             "access_level": "Undocumented",
-            "action": "ListBillingViews",
+            "action": "PutContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RedeemCredits": {
+        "GetBillingDetails": {
             "access_level": "Undocumented",
-            "action": "RedeemCredits",
+            "action": "GetBillingDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingDetails": {
+        "ListBillingViews": {
             "access_level": "Undocumented",
-            "action": "GetBillingDetails",
+            "action": "ListBillingViews",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetBillingNotifications": {
             "access_level": "Undocumented",
             "action": "GetBillingNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredits": {
+        "UpdateBillingPreferences": {
             "access_level": "Undocumented",
-            "action": "GetCredits",
+            "action": "UpdateBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContractInformation": {
+        "UpdateIAMAccessPreference": {
             "access_level": "Undocumented",
-            "action": "GetContractInformation",
+            "action": "UpdateIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingPreferences": {
+        "RedeemCredits": {
             "access_level": "Undocumented",
-            "action": "GetBillingPreferences",
+            "action": "RedeemCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSellerOfRecord": {
+        "GetBillingPreferences": {
             "access_level": "Undocumented",
-            "action": "GetSellerOfRecord",
+            "action": "GetBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIAMAccessPreference": {
+        "GetSellerOfRecord": {
             "access_level": "Undocumented",
-            "action": "UpdateIAMAccessPreference",
+            "action": "GetSellerOfRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingData": {
+        "GetCredits": {
             "access_level": "Undocumented",
-            "action": "GetBillingData",
+            "action": "GetCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutContractInformation": {
+        "GetBillingData": {
             "access_level": "Undocumented",
-            "action": "PutContractInformation",
+            "action": "GetBillingData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billingconductor": {
@@ -19885,715 +19885,715 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "GetCollaboration": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchemaAnalysisRule": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchemaAnalysisRule",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelAssociation": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelAssociation",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgets": {
+        "GetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgets",
+            "action": "GetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "GetConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "GetConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationConfiguredAudienceModelAssociation": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationConfiguredAudienceModelAssociation",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "PreviewPrivacyImpact": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "PreviewPrivacyImpact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListCollaborationAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListCollaborationAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivacyBudgetTemplate": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetPrivacyBudgetTemplate",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "GetCollaborationPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "GetCollaborationPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "GetAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "GetAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePrivacyBudgetTemplate": {
+        "ListPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "UpdatePrivacyBudgetTemplate",
+            "action": "ListPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnalysisTemplates": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListAnalysisTemplates",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "BatchGetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "BatchGetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivacyBudgetTemplate": {
+        "ListCollaborationConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "DeletePrivacyBudgetTemplate",
+            "action": "ListCollaborationConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetCollaborationConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetCollaborationConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgetTemplates": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgetTemplates",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetCollaborationAnalysisTemplate": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "BatchGetCollaborationAnalysisTemplate",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "UpdateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "UpdateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnalysisTemplate": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdateAnalysisTemplate",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModelAssociation": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModelAssociation",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnalysisTemplate": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateAnalysisTemplate",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationAnalysisTemplates": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationAnalysisTemplates",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnalysisTemplate": {
+        "ListCollaborationPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "DeleteAnalysisTemplate",
+            "action": "ListCollaborationPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListConfiguredTables": {
             "access_level": "Undocumented",
             "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PreviewPrivacyImpact": {
+        "UpdateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "PreviewPrivacyImpact",
+            "action": "UpdateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "CreateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "CreateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "ListAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "ListAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgets": {
+        "DeleteConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgets",
+            "action": "DeleteConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivacyBudgetTemplate": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "CreatePrivacyBudgetTemplate",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationAnalysisTemplate": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationAnalysisTemplate",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "ListCollaborationPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "ListCollaborationPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnalysisTemplate": {
+        "DeleteAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "GetAnalysisTemplate",
+            "action": "DeleteAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "GetPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "GetPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "UpdatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "UpdatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationConfiguredAudienceModelAssociations": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationConfiguredAudienceModelAssociations",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelAssociation": {
+        "DeletePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelAssociation",
+            "action": "DeletePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "ListPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "ListPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
             "action": "ListConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModelAssociation": {
+        "BatchGetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModelAssociation",
+            "action": "BatchGetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "CreateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "CreateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationPrivacyBudgetTemplate": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationPrivacyBudgetTemplate",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgetTemplates": {
+        "CreatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgetTemplates",
+            "action": "CreatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms-ml": {
-        "CreateAudienceModel": {
+        "DeleteAudienceModel": {
             "access_level": "Undocumented",
-            "action": "CreateAudienceModel",
+            "action": "DeleteAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTrainingDatasets": {
+        "CreateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListTrainingDatasets",
+            "action": "CreateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceExportJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartAudienceExportJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrainingDataset": {
+        "UpdateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "GetTrainingDataset",
+            "action": "UpdateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrainingDataset": {
+        "ListTrainingDatasets": {
             "access_level": "Undocumented",
-            "action": "DeleteTrainingDataset",
+            "action": "ListTrainingDatasets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListConfiguredAudienceModels": {
             "access_level": "Undocumented",
             "action": "ListConfiguredAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListAudienceExportJobs": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListAudienceExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutConfiguredAudienceModelPolicy": {
+        "CreateTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "PutConfiguredAudienceModelPolicy",
+            "action": "CreateTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceGenerationJob": {
+        "GetTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "StartAudienceGenerationJob",
+            "action": "GetTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceModel": {
+        "DeleteConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceModel",
+            "action": "DeleteConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModel": {
+        "GetConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModel",
+            "action": "GetConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelPolicy": {
+        "DeleteConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelPolicy",
+            "action": "DeleteConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModel": {
+        "ListAudienceGenerationJobs": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModel",
+            "action": "ListAudienceGenerationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceGenerationJob": {
+        "GetAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceGenerationJob",
+            "action": "GetAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceModel": {
+        "DeleteAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "GetAudienceModel",
+            "action": "DeleteAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelPolicy": {
+        "ListAudienceModels": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelPolicy",
+            "action": "ListAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrainingDataset": {
+        "GetConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateTrainingDataset",
+            "action": "GetConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceModels": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListAudienceModels",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModel": {
+        "GetAudienceModel": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModel",
+            "action": "GetAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModel": {
+        "UnTagResource": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModel",
+            "action": "UnTagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceExportJobs": {
+        "StartAudienceExportJob": {
             "access_level": "Undocumented",
-            "action": "ListAudienceExportJobs",
+            "action": "StartAudienceExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UnTagResource": {
+        "CreateAudienceModel": {
             "access_level": "Undocumented",
-            "action": "UnTagResource",
+            "action": "CreateAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceGenerationJob": {
+        "StartAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "GetAudienceGenerationJob",
+            "action": "StartAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "PutConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "PutConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceGenerationJobs": {
+        "DeleteTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "ListAudienceGenerationJobs",
+            "action": "DeleteTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -23580,57 +23580,57 @@
             "orphan": false,
             "resources": [
                 "streaming-distribution"
             ]
         }
     },
     "cloudfront-keyvaluestore": {
-        "UpdateKeys": {
+        "DescribeKeyValueStore": {
             "access_level": "Undocumented",
-            "action": "UpdateKeys",
+            "action": "DescribeKeyValueStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeKeyValueStore": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "DescribeKeyValueStore",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "UpdateKeys": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "UpdateKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutKey": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "PutKey",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "PutKey": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "PutKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloudhsm": {
@@ -27782,305 +27782,305 @@
             "orphan": false,
             "resources": [
                 "repository"
             ]
         }
     },
     "codeconnections": {
-        "GetRepositoryLink": {
+        "GetConnection": {
             "access_level": "Undocumented",
-            "action": "GetRepositoryLink",
+            "action": "GetConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnection": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteConnection",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseConnection": {
+        "CreateConnection": {
             "access_level": "Undocumented",
-            "action": "UseConnection",
+            "action": "CreateConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSyncConfiguration": {
+        "UpdateConnectionInstallation": {
             "access_level": "Undocumented",
-            "action": "DeleteSyncConfiguration",
+            "action": "UpdateConnectionInstallation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetInstallationUrl": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetInstallationUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndividualAccessToken": {
+        "ListSyncConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetIndividualAccessToken",
+            "action": "ListSyncConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConnection": {
+        "UpdateHost": {
             "access_level": "Undocumented",
-            "action": "GetConnection",
+            "action": "UpdateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnection": {
+        "GetRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "CreateConnection",
+            "action": "GetRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListHosts": {
+        "GetHost": {
             "access_level": "Undocumented",
-            "action": "ListHosts",
+            "action": "GetHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSyncConfiguration": {
+        "CreateHost": {
             "access_level": "Undocumented",
-            "action": "CreateSyncConfiguration",
+            "action": "CreateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRepository": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "PassRepository",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartOAuthHandshake": {
+        "UpdateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartOAuthHandshake",
+            "action": "UpdateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConnections": {
+        "ListInstallationTargets": {
             "access_level": "Undocumented",
-            "action": "ListConnections",
+            "action": "ListInstallationTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterAppCode": {
+        "ListRepositoryLinks": {
             "access_level": "Undocumented",
-            "action": "RegisterAppCode",
+            "action": "ListRepositoryLinks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteHost": {
+        "GetSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteHost",
+            "action": "GetSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstallationTargets": {
+        "GetResourceSyncStatus": {
             "access_level": "Undocumented",
-            "action": "ListInstallationTargets",
+            "action": "GetResourceSyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassConnection": {
+        "RegisterAppCode": {
             "access_level": "Undocumented",
-            "action": "PassConnection",
+            "action": "RegisterAppCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRepositoryLink": {
+        "CreateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "DeleteRepositoryLink",
+            "action": "CreateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRepositoryLink": {
+        "UpdateSyncBlocker": {
             "access_level": "Undocumented",
-            "action": "UpdateRepositoryLink",
+            "action": "UpdateSyncBlocker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositorySyncStatus": {
+        "UseConnection": {
             "access_level": "Undocumented",
-            "action": "GetRepositorySyncStatus",
+            "action": "UseConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHost": {
+        "GetRepositorySyncStatus": {
             "access_level": "Undocumented",
-            "action": "GetHost",
+            "action": "GetRepositorySyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConnectionInstallation": {
+        "DeleteSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateConnectionInstallation",
+            "action": "DeleteSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSyncConfiguration": {
+        "ListRepositorySyncDefinitions": {
             "access_level": "Undocumented",
-            "action": "GetSyncConfiguration",
+            "action": "ListRepositorySyncDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSyncConfiguration": {
+        "DeleteHost": {
             "access_level": "Undocumented",
-            "action": "UpdateSyncConfiguration",
+            "action": "DeleteHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceSyncStatus": {
+        "GetSyncBlockerSummary": {
             "access_level": "Undocumented",
-            "action": "GetResourceSyncStatus",
+            "action": "GetSyncBlockerSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSyncBlockerSummary": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetSyncBlockerSummary",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRepositoryLink": {
+        "CreateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateRepositoryLink",
+            "action": "CreateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListConnections": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListConnections",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateHost": {
+        "StartOAuthHandshake": {
             "access_level": "Undocumented",
-            "action": "CreateHost",
+            "action": "StartOAuthHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositoryLinks": {
+        "PassConnection": {
             "access_level": "Undocumented",
-            "action": "ListRepositoryLinks",
+            "action": "PassConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateHost": {
+        "DeleteConnection": {
             "access_level": "Undocumented",
-            "action": "UpdateHost",
+            "action": "DeleteConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSyncConfigurations": {
+        "GetIndividualAccessToken": {
             "access_level": "Undocumented",
-            "action": "ListSyncConfigurations",
+            "action": "GetIndividualAccessToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositorySyncDefinitions": {
+        "DeleteRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "ListRepositorySyncDefinitions",
+            "action": "DeleteRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppRegistrationHandshake": {
+        "PassRepository": {
             "access_level": "Undocumented",
-            "action": "StartAppRegistrationHandshake",
+            "action": "PassRepository",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSyncBlocker": {
+        "StartAppRegistrationHandshake": {
             "access_level": "Undocumented",
-            "action": "UpdateSyncBlocker",
+            "action": "StartAppRegistrationHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstallationUrl": {
+        "UpdateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "GetInstallationUrl",
+            "action": "UpdateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListHosts": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListHosts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codedeploy": {
@@ -29012,129 +29012,129 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "CreateUploadUrl": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteScansByCategory": {
             "access_level": "Undocumented",
             "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountConfiguration": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateScan": {
             "access_level": "Undocumented",
             "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindingsMetrics": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricsSummary": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -37638,25 +37638,25 @@
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         }
     },
     "consoleapp": {
-        "ListDeviceIdentities": {
+        "GetDeviceIdentity": {
             "access_level": "Undocumented",
-            "action": "ListDeviceIdentities",
+            "action": "GetDeviceIdentity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceIdentity": {
+        "ListDeviceIdentities": {
             "access_level": "Undocumented",
-            "action": "GetDeviceIdentity",
+            "action": "ListDeviceIdentities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
@@ -38250,65 +38250,65 @@
             "orphan": false,
             "resources": [
                 "LandingZone"
             ]
         }
     },
     "cost-optimization-hub": {
-        "ListEnrollmentStatuses": {
+        "UpdatePreferences": {
             "access_level": "Undocumented",
-            "action": "ListEnrollmentStatuses",
+            "action": "UpdatePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationSummaries": {
+        "ListRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationSummaries",
+            "action": "ListRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendations": {
+        "ListEnrollmentStatuses": {
             "access_level": "Undocumented",
-            "action": "ListRecommendations",
+            "action": "ListEnrollmentStatuses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePreferences": {
+        "GetPreferences": {
             "access_level": "Undocumented",
-            "action": "UpdatePreferences",
+            "action": "GetPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnrollmentStatus": {
+        "ListRecommendationSummaries": {
             "access_level": "Undocumented",
-            "action": "UpdateEnrollmentStatus",
+            "action": "ListRecommendationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetRecommendation": {
             "access_level": "Undocumented",
             "action": "GetRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPreferences": {
+        "UpdateEnrollmentStatus": {
             "access_level": "Undocumented",
-            "action": "GetPreferences",
+            "action": "UpdateEnrollmentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cur": {
@@ -38427,41 +38427,41 @@
             "condition_keys": [],
             "description": "Grants permission to validates if the s3 bucket exists with appropriate permissions for CUR delivery",
             "orphan": false,
             "resources": []
         }
     },
     "customer-verification": {
-        "UpdateCustomerVerificationDetails": {
+        "GetCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "UpdateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetCustomerVerificationEligibility": {
             "access_level": "Undocumented",
             "action": "GetCustomerVerificationEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCustomerVerificationDetails": {
+        "UpdateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "CreateCustomerVerificationDetails",
+            "action": "UpdateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationDetails": {
+        "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationDetails",
+            "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "databrew": {
@@ -40145,1065 +40145,1065 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "GetSubscriptionRequestDetails": {
+        "DeleteSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionRequestDetails",
+            "action": "DeleteSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscription": {
+        "StopMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "GetSubscription",
+            "action": "StopMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "DeleteEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "DeleteEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchUserProfiles": {
+        "GetEnvironmentCredentials": {
             "access_level": "Undocumented",
-            "action": "SearchUserProfiles",
+            "action": "GetEnvironmentCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutEnvironmentBlueprintConfiguration": {
+        "GetGlossary": {
             "access_level": "Undocumented",
-            "action": "PutEnvironmentBlueprintConfiguration",
+            "action": "GetGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetListing": {
+        "UpdateSubscriptionGrantStatus": {
             "access_level": "Undocumented",
-            "action": "GetListing",
+            "action": "UpdateSubscriptionGrantStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionEligibility": {
+        "Search": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionEligibility",
+            "action": "Search",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "ListSubscriptionRequests": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "ListSubscriptionRequests",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionRequest": {
+        "CreateUserProfile": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionRequest",
+            "action": "CreateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossaryTerm": {
+        "UpdateDomain": {
             "access_level": "Undocumented",
-            "action": "GetGlossaryTerm",
+            "action": "UpdateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RevokeSubscription": {
+        "CreateProject": {
             "access_level": "Undocumented",
-            "action": "RevokeSubscription",
+            "action": "CreateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotifications": {
+        "GetGroupProfile": {
             "access_level": "Undocumented",
-            "action": "ListNotifications",
+            "action": "GetGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossaryTerm": {
+        "UpdateGlossary": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossaryTerm",
+            "action": "UpdateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogout": {
+        "CreateListingChangeSet": {
             "access_level": "Undocumented",
-            "action": "SsoLogout",
+            "action": "CreateListingChangeSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprintConfiguration": {
+        "AddPolicyGrant": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprintConfiguration",
+            "action": "AddPolicyGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemovePolicyGrant": {
+        "AcceptSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "RemovePolicyGrant",
+            "action": "AcceptSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Search": {
+        "PostTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "Search",
+            "action": "PostTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetType": {
+        "CreateFormType": {
             "access_level": "Undocumented",
-            "action": "CreateAssetType",
+            "action": "CreateFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDomain": {
+        "ListWarehouseMetadata": {
             "access_level": "Undocumented",
-            "action": "UpdateDomain",
+            "action": "ListWarehouseMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomainSharingPolicy": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "GetDomainSharingPolicy",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossary": {
+        "AcceptPredictions": {
             "access_level": "Undocumented",
-            "action": "CreateGlossary",
+            "action": "AcceptPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataGenerationRun": {
+        "StartDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "GetMetadataGenerationRun",
+            "action": "StartDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSourceRunActivities": {
+        "SearchGroupProfiles": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSourceRunActivities",
+            "action": "SearchGroupProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProjectMembership": {
+        "ListSubscriptionTargets": {
             "access_level": "Undocumented",
-            "action": "CreateProjectMembership",
+            "action": "ListSubscriptionTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomain": {
+        "PutEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteDomain",
+            "action": "PutEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionRequest": {
+        "GetUserProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionRequest",
+            "action": "GetUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserProfile": {
+        "ListMetadataGenerationRuns": {
             "access_level": "Undocumented",
-            "action": "GetUserProfile",
+            "action": "ListMetadataGenerationRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopMetadataGenerationRun": {
+        "DeleteTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "StopMetadataGenerationRun",
+            "action": "DeleteTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionGrant": {
+        "RejectSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionGrant",
+            "action": "RejectSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProject": {
+        "PutDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateProject",
+            "action": "PutDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentProfile": {
+        "GetAssetType": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentProfile",
+            "action": "GetAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyGrants": {
+        "CreateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "ListPolicyGrants",
+            "action": "CreateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "DeleteSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "DeleteSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectSubscriptionRequest": {
+        "RevokeSubscription": {
             "access_level": "Undocumented",
-            "action": "RejectSubscriptionRequest",
+            "action": "RevokeSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProject": {
+        "DeleteAssetType": {
             "access_level": "Undocumented",
-            "action": "CreateProject",
+            "action": "DeleteAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFormType": {
+        "RefreshToken": {
             "access_level": "Undocumented",
-            "action": "DeleteFormType",
+            "action": "RefreshToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossaryTerm": {
+        "CancelSubscription": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossaryTerm",
+            "action": "CancelSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionGrant": {
+        "DeleteProject": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionGrant",
+            "action": "DeleteProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprintConfiguration": {
+        "GetIamPortalLoginUrl": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprintConfiguration",
+            "action": "GetIamPortalLoginUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSubscription": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "CancelSubscription",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceRun": {
+        "DeleteProjectMembership": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceRun",
+            "action": "DeleteProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWarehouseMetadata": {
+        "CreateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "ListWarehouseMetadata",
+            "action": "CreateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMetadataGenerationRun": {
+        "GetFormType": {
             "access_level": "Undocumented",
-            "action": "CancelMetadataGenerationRun",
+            "action": "GetFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "CreateAssetType": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "CreateAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "UpdateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "UpdateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroupProfile": {
+        "SearchTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateGroupProfile",
+            "action": "SearchTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTimeSeriesDataPoint": {
+        "UpdateProject": {
             "access_level": "Undocumented",
-            "action": "GetTimeSeriesDataPoint",
+            "action": "UpdateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "GetDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "GetDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchListings": {
+        "GetSubscriptionEligibility": {
             "access_level": "Undocumented",
-            "action": "SearchListings",
+            "action": "GetSubscriptionEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionTarget": {
+        "CreateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionTarget",
+            "action": "CreateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAsset": {
+        "GetEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateAsset",
+            "action": "GetEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "GetSubscriptionRequestDetails": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "GetSubscriptionRequestDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUserProfile": {
+        "CreateSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "CreateUserProfile",
+            "action": "CreateSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectPredictions": {
+        "ListSubscriptionGrants": {
             "access_level": "Undocumented",
-            "action": "RejectPredictions",
+            "action": "ListSubscriptionGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "ListDataSourceRunActivities": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "ListDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProjectMembership": {
+        "GetEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "DeleteProjectMembership",
+            "action": "GetEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMetadataGenerationRun": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "StartMetadataGenerationRun",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogin": {
+        "GetGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "SsoLogin",
+            "action": "GetGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroupProfile": {
+        "DeleteEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreateGroupProfile",
+            "action": "DeleteEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListing": {
+        "GetListing": {
             "access_level": "Undocumented",
-            "action": "DeleteListing",
+            "action": "GetListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PostTimeSeriesDataPoints": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "PostTimeSeriesDataPoints",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurationSummaries": {
+        "DeleteFormType": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurationSummaries",
+            "action": "DeleteFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossary": {
+        "ListDataSourceRuns": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossary",
+            "action": "ListDataSourceRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ProvisionDomain": {
+        "UpdateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "ProvisionDomain",
+            "action": "UpdateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "UpdateEnvironmentConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "UpdateEnvironmentConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomainSharingPolicy": {
+        "GetSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "DeleteDomainSharingPolicy",
+            "action": "GetSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprints": {
+        "CreateAssetRevision": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprints",
+            "action": "CreateAssetRevision",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFormType": {
+        "GetMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "CreateFormType",
+            "action": "GetMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTimeSeriesDataPoints": {
+        "UpdateUserProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteTimeSeriesDataPoints",
+            "action": "UpdateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAsset": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "DeleteAsset",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssetType": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteAssetType",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "ListAssetRevisions": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "ListAssetRevisions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountEnvironments": {
+        "GetSubscription": {
             "access_level": "Undocumented",
-            "action": "ListAccountEnvironments",
+            "action": "GetSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentBlueprint": {
+        "DeleteDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentBlueprint",
+            "action": "DeleteDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptSubscriptionRequest": {
+        "GetEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "AcceptSubscriptionRequest",
+            "action": "GetEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentCredentials": {
+        "ListEnvironmentBlueprintConfigurationSummaries": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentCredentials",
+            "action": "ListEnvironmentBlueprintConfigurationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIamPortalLoginUrl": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "GetIamPortalLoginUrl",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProject": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteProject",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionRequests": {
+        "GetEnvironmentActionLink": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionRequests",
+            "action": "GetEnvironmentActionLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionTarget": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionTarget",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptions": {
+        "CreateAsset": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptions",
+            "action": "CreateAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentProfile": {
+        "DeleteSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentProfile",
+            "action": "DeleteSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTypes": {
+        "ValidatePassRole": {
             "access_level": "Undocumented",
-            "action": "SearchTypes",
+            "action": "ValidatePassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionRequest": {
+        "DeleteGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionRequest",
+            "action": "DeleteGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "ListPolicyGrants": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "ListPolicyGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionGrantStatus": {
+        "SearchUserProfiles": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionGrantStatus",
+            "action": "SearchUserProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionTarget": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionTarget",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurations": {
+        "CreateDomain": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurations",
+            "action": "CreateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentProfiles": {
+        "ListAccountEnvironments": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentProfiles",
+            "action": "ListAccountEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossary": {
+        "UpdateDataSourceRunActivities": {
             "access_level": "Undocumented",
-            "action": "GetGlossary",
+            "action": "UpdateDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssetRevisions": {
+        "UpdateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "ListAssetRevisions",
+            "action": "UpdateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePassRole": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ValidatePassRole",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RefreshToken": {
+        "CreateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "RefreshToken",
+            "action": "CreateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceRun": {
+        "ListNotifications": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceRun",
+            "action": "ListNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDomain": {
+        "GetDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "CreateDomain",
+            "action": "GetDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataGenerationRuns": {
+        "DeleteAsset": {
             "access_level": "Undocumented",
-            "action": "ListMetadataGenerationRuns",
+            "action": "DeleteAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteGlossary": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentProfile": {
+        "UpdateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentProfile",
+            "action": "UpdateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionTarget": {
+        "UpdateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionTarget",
+            "action": "UpdateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetRevision": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateAssetRevision",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupProfile": {
+        "DeleteEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "GetGroupProfile",
+            "action": "DeleteEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossary": {
+        "CreateGlossary": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossary",
+            "action": "CreateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "RejectPredictions": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "RejectPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionGrants": {
+        "ListEnvironmentProfiles": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionGrants",
+            "action": "ListEnvironmentProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "UpdateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "UpdateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyGrant": {
+        "DeleteListing": {
             "access_level": "Undocumented",
-            "action": "AddPolicyGrant",
+            "action": "DeleteListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentBlueprint": {
+        "ProvisionDomain": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentBlueprint",
+            "action": "ProvisionDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListingChangeSet": {
+        "UpdateEnvironmentDeploymentStatus": {
             "access_level": "Undocumented",
-            "action": "CreateListingChangeSet",
+            "action": "UpdateEnvironmentDeploymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetType": {
+        "CreateProjectMembership": {
             "access_level": "Undocumented",
-            "action": "GetAssetType",
+            "action": "CreateProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchGroupProfiles": {
+        "StartMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "SearchGroupProfiles",
+            "action": "StartMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentDeploymentStatus": {
+        "CancelMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentDeploymentStatus",
+            "action": "CancelMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentConfiguration": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentConfiguration",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAsset": {
+        "GetTimeSeriesDataPoint": {
             "access_level": "Undocumented",
-            "action": "GetAsset",
+            "action": "GetTimeSeriesDataPoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossaryTerm": {
+        "CreateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "CreateGlossaryTerm",
+            "action": "CreateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionGrant": {
+        "ListSubscriptions": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionGrant",
+            "action": "ListSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentProfile": {
+        "SsoLogout": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentProfile",
+            "action": "SsoLogout",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFormType": {
+        "ListProjectMemberships": {
             "access_level": "Undocumented",
-            "action": "GetFormType",
+            "action": "ListProjectMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionTargets": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionTargets",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRunActivities": {
+        "RemovePolicyGrant": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRunActivities",
+            "action": "RemovePolicyGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUserProfile": {
+        "SsoLogin": {
             "access_level": "Undocumented",
-            "action": "UpdateUserProfile",
+            "action": "SsoLogin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprint": {
+        "ListEnvironmentBlueprints": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprint",
+            "action": "ListEnvironmentBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptPredictions": {
+        "SearchListings": {
             "access_level": "Undocumented",
-            "action": "AcceptPredictions",
+            "action": "SearchListings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentActionLink": {
+        "ListTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentActionLink",
+            "action": "ListTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRuns": {
+        "GetAsset": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRuns",
+            "action": "GetAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjectMemberships": {
+        "ListEnvironmentBlueprintConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListProjectMemberships",
+            "action": "ListEnvironmentBlueprintConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTimeSeriesDataPoints": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListTimeSeriesDataPoints",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprint": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprint",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDomainSharingPolicy": {
+        "DeleteDomain": {
             "access_level": "Undocumented",
-            "action": "PutDomainSharingPolicy",
+            "action": "DeleteDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -41597,833 +41597,833 @@
             "condition_keys": [],
             "description": "Grants permission to update query tab",
             "orphan": false,
             "resources": []
         }
     },
     "deadline": {
-        "CreateFarm": {
+        "CreateJob": {
             "access_level": "Undocumented",
-            "action": "CreateFarm",
+            "action": "CreateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfile": {
+        "ListJobs": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfile",
+            "action": "ListJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBudget": {
+        "SearchWorkers": {
             "access_level": "Undocumented",
-            "action": "GetBudget",
+            "action": "SearchWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToJob": {
+        "AssumeFleetRoleForRead": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToJob",
+            "action": "AssumeFleetRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
             "action": "GetSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForRead": {
+        "GetFarm": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForRead",
+            "action": "GetFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFleet": {
+        "DisassociateMemberFromJob": {
             "access_level": "Undocumented",
-            "action": "CreateFleet",
+            "action": "DisassociateMemberFromJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueue": {
+        "ListStepConsumers": {
             "access_level": "Undocumented",
-            "action": "CreateQueue",
+            "action": "ListStepConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStep": {
+        "ListSessions": {
             "access_level": "Undocumented",
-            "action": "GetStep",
+            "action": "ListSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "CreateQueue": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "CreateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTask": {
+        "ListFarms": {
             "access_level": "Undocumented",
-            "action": "GetTask",
+            "action": "ListFarms",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkers": {
+        "CreateFarm": {
             "access_level": "Undocumented",
-            "action": "ListWorkers",
+            "action": "CreateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetJobEntity": {
+        "ListSessionActions": {
             "access_level": "Undocumented",
-            "action": "BatchGetJobEntity",
+            "action": "ListSessionActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetJob": {
+        "ListSessionsForWorker": {
             "access_level": "Undocumented",
-            "action": "GetJob",
+            "action": "ListSessionsForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSessionsStatisticsAggregation": {
+        "GetStep": {
             "access_level": "Undocumented",
-            "action": "StartSessionsStatisticsAggregation",
+            "action": "GetStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTasks": {
+        "CreateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListTasks",
+            "action": "CreateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorker": {
+        "ListBudgets": {
             "access_level": "Undocumented",
-            "action": "CreateWorker",
+            "action": "ListBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "StartSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "StartSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "CreateFleet": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "CreateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFarm": {
+        "DeleteFleet": {
             "access_level": "Undocumented",
-            "action": "UpdateFarm",
+            "action": "DeleteFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueue": {
+        "DeleteLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "UpdateQueue",
+            "action": "DeleteLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToQueue": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToQueue",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromQueue": {
+        "UpdateTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromQueue",
+            "action": "UpdateTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFleet": {
+        "DeleteQueue": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFleet",
+            "action": "DeleteQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionAction": {
+        "CreateBudget": {
             "access_level": "Undocumented",
-            "action": "GetSessionAction",
+            "action": "CreateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueFleetAssociation": {
+        "ListFleets": {
             "access_level": "Undocumented",
-            "action": "CreateQueueFleetAssociation",
+            "action": "ListFleets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBudget": {
+        "UpdateQueue": {
             "access_level": "Undocumented",
-            "action": "CreateBudget",
+            "action": "UpdateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBudgets": {
+        "ListTasks": {
             "access_level": "Undocumented",
-            "action": "ListBudgets",
+            "action": "ListTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFleet": {
+        "SearchTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateFleet",
+            "action": "SearchTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStorageProfile": {
+        "DisassociateMemberFromFleet": {
             "access_level": "Undocumented",
-            "action": "UpdateStorageProfile",
+            "action": "DisassociateMemberFromFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueues": {
+        "UpdateBudget": {
             "access_level": "Undocumented",
-            "action": "ListQueues",
+            "action": "UpdateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForWorker": {
+        "UpdateJob": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForWorker",
+            "action": "UpdateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobs": {
+        "GetJob": {
             "access_level": "Undocumented",
-            "action": "ListJobs",
+            "action": "GetJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicenseEndpoint": {
+        "UpdateStep": {
             "access_level": "Undocumented",
-            "action": "CreateLicenseEndpoint",
+            "action": "UpdateStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSteps": {
+        "GetWorker": {
             "access_level": "Undocumented",
-            "action": "ListSteps",
+            "action": "GetWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchJobs": {
+        "UpdateFarm": {
             "access_level": "Undocumented",
-            "action": "SearchJobs",
+            "action": "UpdateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFleet": {
+        "GetQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteFleet",
+            "action": "GetQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "ListQueueFleetAssociations": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "ListQueueFleetAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleetMembers": {
+        "ListAvailableMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "ListFleetMembers",
+            "action": "ListAvailableMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStorageProfile": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateStorageProfile",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFarm": {
+        "GetFleet": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFarm",
+            "action": "GetFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorker": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "GetWorker",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueFleetAssociation": {
+        "AssociateMemberToFleet": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueFleetAssociation",
+            "action": "AssociateMemberToFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTask": {
+        "DisassociateMemberFromQueue": {
             "access_level": "Undocumented",
-            "action": "UpdateTask",
+            "action": "DisassociateMemberFromQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueEnvironment": {
+        "GetQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueEnvironment",
+            "action": "GetQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFarm": {
+        "ListStepDependencies": {
             "access_level": "Undocumented",
-            "action": "DeleteFarm",
+            "action": "ListStepDependencies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLicenseEndpoints": {
+        "DeleteBudget": {
             "access_level": "Undocumented",
-            "action": "ListLicenseEndpoints",
+            "action": "DeleteBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfiles": {
+        "SearchJobs": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfiles",
+            "action": "SearchJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfilesForQueue": {
+        "UpdateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfilesForQueue",
+            "action": "UpdateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "AssociateMemberToQueue": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "AssociateMemberToQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueMembers": {
+        "CreateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "ListQueueMembers",
+            "action": "CreateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStorageProfile": {
+        "PutMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "DeleteStorageProfile",
+            "action": "PutMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfileForQueue": {
+        "ListQueues": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfileForQueue",
+            "action": "ListQueues",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "AssumeFleetRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "AssumeFleetRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkerSchedule": {
+        "GetMonitor": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkerSchedule",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWorkers": {
+        "ListFleetMembers": {
             "access_level": "Undocumented",
-            "action": "SearchWorkers",
+            "action": "ListFleetMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueFleetAssociations": {
+        "ListFarmMembers": {
             "access_level": "Undocumented",
-            "action": "ListQueueFleetAssociations",
+            "action": "ListFarmMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueFleetAssociation": {
+        "GetSessionAction": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueFleetAssociation",
+            "action": "GetSessionAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMeteredProducts": {
+        "UpdateWorkerSchedule": {
             "access_level": "Undocumented",
-            "action": "ListMeteredProducts",
+            "action": "UpdateWorkerSchedule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStep": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateStep",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobMembers": {
+        "ListQueueEnvironments": {
             "access_level": "Undocumented",
-            "action": "ListJobMembers",
+            "action": "ListQueueEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyJobTemplate": {
+        "AssumeQueueRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "CopyJobTemplate",
+            "action": "AssumeQueueRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionsForWorker": {
+        "ListJobMembers": {
             "access_level": "Undocumented",
-            "action": "ListSessionsForWorker",
+            "action": "ListJobMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListSteps": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFarm": {
+        "AssumeQueueRoleForUser": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFarm",
+            "action": "AssumeQueueRoleForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorker": {
+        "UpdateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateWorker",
+            "action": "UpdateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarmMembers": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "ListFarmMembers",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueEnvironment": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "CreateQueueEnvironment",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueFleetAssociation": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "GetQueueFleetAssociation",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSteps": {
+        "ListWorkers": {
             "access_level": "Undocumented",
-            "action": "SearchSteps",
+            "action": "ListWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForUser": {
+        "ListStorageProfilesForQueue": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForUser",
+            "action": "ListStorageProfilesForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplicationVersion": {
+        "GetStorageProfile": {
             "access_level": "Undocumented",
-            "action": "GetApplicationVersion",
+            "action": "GetStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromJob": {
+        "AssociateMemberToFarm": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromJob",
+            "action": "AssociateMemberToFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateJob": {
+        "BatchGetJobEntity": {
             "access_level": "Undocumented",
-            "action": "CreateJob",
+            "action": "BatchGetJobEntity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForWorker": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForWorker",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleets": {
+        "DeleteWorker": {
             "access_level": "Undocumented",
-            "action": "ListFleets",
+            "action": "DeleteWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTasks": {
+        "GetLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "SearchTasks",
+            "action": "GetLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarms": {
+        "AssociateMemberToJob": {
             "access_level": "Undocumented",
-            "action": "ListFarms",
+            "action": "AssociateMemberToJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionActions": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "ListSessionActions",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBudget": {
+        "SearchSteps": {
             "access_level": "Undocumented",
-            "action": "DeleteBudget",
+            "action": "SearchSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueue": {
+        "UpdateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "GetQueue",
+            "action": "UpdateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueue": {
+        "DeleteQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "DeleteQueue",
+            "action": "DeleteQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLicenseEndpoint": {
+        "GetApplicationVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteLicenseEndpoint",
+            "action": "GetApplicationVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueEnvironments": {
+        "CreateLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListQueueEnvironments",
+            "action": "CreateLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForRead": {
+        "ListLicenseEndpoints": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForRead",
+            "action": "ListLicenseEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorker": {
+        "DisassociateMemberFromFarm": {
             "access_level": "Undocumented",
-            "action": "DeleteWorker",
+            "action": "DisassociateMemberFromFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepDependencies": {
+        "DeleteFarm": {
             "access_level": "Undocumented",
-            "action": "ListStepDependencies",
+            "action": "DeleteFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessions": {
+        "GetQueue": {
             "access_level": "Undocumented",
-            "action": "ListSessions",
+            "action": "GetQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMeteredProduct": {
+        "CreateWorker": {
             "access_level": "Undocumented",
-            "action": "DeleteMeteredProduct",
+            "action": "CreateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetTask": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateBudget": {
+        "DeleteQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateBudget",
+            "action": "DeleteQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicenseEndpoint": {
+        "ListQueueMembers": {
             "access_level": "Undocumented",
-            "action": "GetLicenseEndpoint",
+            "action": "ListQueueMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFarm": {
+        "AssumeQueueRoleForRead": {
             "access_level": "Undocumented",
-            "action": "GetFarm",
+            "action": "AssumeQueueRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueEnvironment": {
+        "DeleteStorageProfile": {
             "access_level": "Undocumented",
-            "action": "GetQueueEnvironment",
+            "action": "DeleteStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFleet": {
+        "UpdateFleet": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFleet",
+            "action": "UpdateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueEnvironment": {
+        "CreateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueEnvironment",
+            "action": "CreateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFleet": {
+        "ListStorageProfiles": {
             "access_level": "Undocumented",
-            "action": "GetFleet",
+            "action": "ListStorageProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "GetStorageProfileForQueue": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "GetStorageProfileForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMonitor": {
+        "UpdateWorker": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "UpdateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAvailableMeteredProducts": {
+        "DeleteMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "ListAvailableMeteredProducts",
+            "action": "DeleteMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMeteredProduct": {
+        "ListMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "PutMeteredProduct",
+            "action": "ListMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepConsumers": {
+        "GetBudget": {
             "access_level": "Undocumented",
-            "action": "ListStepConsumers",
+            "action": "GetBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateJob": {
+        "CopyJobTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateJob",
+            "action": "CopyJobTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "deepcomposer": {
@@ -64916,305 +64916,305 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "SetSubnets": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "SetSubnets",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "DescribeTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "DescribeTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreCaCertificatesBundle": {
+        "GetTrustStoreRevocationContent": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreCaCertificatesBundle",
+            "action": "GetTrustStoreRevocationContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTrustStoreRevocations": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "AddTrustStoreRevocations",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroup": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroup",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTrustStoreRevocations": {
+        "ModifyTargetGroup": {
             "access_level": "Undocumented",
-            "action": "RemoveTrustStoreRevocations",
+            "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrustStore": {
+        "RemoveTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "DeleteTrustStore",
+            "action": "RemoveTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterTargets": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "RegisterTargets",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreRevocationContent": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreRevocationContent",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "CreateTargetGroup": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreRevocations": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreRevocations",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroupAttributes": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetGroup": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetGroup",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRule": {
+        "AddTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "AddTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrustStore": {
+        "ModifyTrustStore": {
             "access_level": "Undocumented",
-            "action": "CreateTrustStore",
+            "action": "ModifyTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreAssociations": {
+        "ModifyListener": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreAssociations",
+            "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTrustStore": {
+        "SetSubnets": {
             "access_level": "Undocumented",
-            "action": "ModifyTrustStore",
+            "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "DeleteTargetGroup": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStores": {
+        "DeleteTrustStore": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStores",
+            "action": "DeleteTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RemoveListenerCertificates": {
             "access_level": "Undocumented",
             "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetGroup": {
+        "DescribeTrustStores": {
             "access_level": "Undocumented",
-            "action": "CreateTargetGroup",
+            "action": "DescribeTrustStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "RegisterTargets": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "DescribeTrustStoreAssociations": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "DescribeTrustStoreAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyListener": {
+        "CreateTrustStore": {
             "access_level": "Undocumented",
-            "action": "ModifyListener",
+            "action": "CreateTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "GetTrustStoreCaCertificatesBundle": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "GetTrustStoreCaCertificatesBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroupAttributes": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroupAttributes",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -66915,305 +66915,305 @@
             "orphan": false,
             "resources": [
                 "application"
             ]
         }
     },
     "entityresolution": {
-        "PutPolicy": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "PutPolicy",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaMapping": {
+        "DeletePolicyStatement": {
             "access_level": "Undocumented",
-            "action": "GetSchemaMapping",
+            "action": "DeletePolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingWorkflow": {
+        "DeleteSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "GetMatchingWorkflow",
+            "action": "DeleteSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListIdMappingJobs": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListIdMappingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdNamespace": {
+        "CreateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "UpdateIdNamespace",
+            "action": "CreateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingWorkflow": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingWorkflow",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSchemaMapping": {
+        "ListIdNamespaces": {
             "access_level": "Undocumented",
-            "action": "UpdateSchemaMapping",
+            "action": "ListIdNamespaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdMappingWorkflow": {
+        "ListMatchingJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateIdMappingWorkflow",
+            "action": "ListMatchingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdMappingWorkflow": {
+        "UpdateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteIdMappingWorkflow",
+            "action": "UpdateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStatement": {
+        "GetMatchingJob": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStatement",
+            "action": "GetMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchId": {
+        "GetIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetMatchId",
+            "action": "GetIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingWorkflows": {
+        "CreateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingWorkflows",
+            "action": "CreateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "GetIdNamespace": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "GetIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIdMappingJob": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartIdMappingJob",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingJobs": {
+        "DeleteMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListMatchingJobs",
+            "action": "DeleteMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProviderServices": {
+        "UseIdNamespace": {
             "access_level": "Undocumented",
-            "action": "ListProviderServices",
+            "action": "UseIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMatchingWorkflow": {
+        "CreateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "UpdateMatchingWorkflow",
+            "action": "CreateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProviderService": {
+        "CreateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetProviderService",
+            "action": "CreateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMatchingJob": {
+        "GetSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "StartMatchingJob",
+            "action": "GetSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMatchingWorkflow": {
+        "ListMatchingWorkflows": {
             "access_level": "Undocumented",
-            "action": "CreateMatchingWorkflow",
+            "action": "ListMatchingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyStatement": {
+        "ListProviderServices": {
             "access_level": "Undocumented",
-            "action": "AddPolicyStatement",
+            "action": "ListProviderServices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingJob": {
+        "GetMatchId": {
             "access_level": "Undocumented",
-            "action": "GetMatchingJob",
+            "action": "GetMatchId",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingWorkflows": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListMatchingWorkflows",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMatchingWorkflow": {
+        "DeleteIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteMatchingWorkflow",
+            "action": "DeleteIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdNamespaces": {
+        "GetProviderService": {
             "access_level": "Undocumented",
-            "action": "ListIdNamespaces",
+            "action": "GetProviderService",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseIdNamespace": {
+        "PutPolicy": {
             "access_level": "Undocumented",
-            "action": "UseIdNamespace",
+            "action": "PutPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdMappingWorkflow": {
+        "UpdateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "CreateIdMappingWorkflow",
+            "action": "UpdateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdNamespace": {
+        "DeleteIdNamespace": {
             "access_level": "Undocumented",
-            "action": "GetIdNamespace",
+            "action": "DeleteIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdNamespace": {
+        "UpdateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "CreateIdNamespace",
+            "action": "UpdateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingJobs": {
+        "GetMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingJobs",
+            "action": "GetMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdNamespace": {
+        "ListIdMappingWorkflows": {
             "access_level": "Undocumented",
-            "action": "DeleteIdNamespace",
+            "action": "ListIdMappingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingJob": {
+        "AddPolicyStatement": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingJob",
+            "action": "AddPolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSchemaMappings": {
             "access_level": "Undocumented",
             "action": "ListSchemaMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSchemaMapping": {
+        "StartIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "CreateSchemaMapping",
+            "action": "StartIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSchemaMapping": {
+        "StartMatchingJob": {
             "access_level": "Undocumented",
-            "action": "DeleteSchemaMapping",
+            "action": "StartMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "es": {
@@ -69931,225 +69931,225 @@
             "orphan": false,
             "resources": [
                 "deliverystream"
             ]
         }
     },
     "fis": {
-        "InjectApiUnavailableError": {
+        "StartExperiment": {
             "access_level": "Undocumented",
-            "action": "InjectApiUnavailableError",
+            "action": "StartExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTemplates": {
+        "UpdateExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTemplates",
+            "action": "UpdateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExperimentTemplate": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateExperimentTemplate",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExperimentTemplate": {
+        "UpdateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteExperimentTemplate",
+            "action": "UpdateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExperiment": {
+        "GetExperimentTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartExperiment",
+            "action": "GetExperimentTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopExperiment": {
+        "GetAction": {
             "access_level": "Undocumented",
-            "action": "StopExperiment",
+            "action": "GetAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetResourceType": {
+        "GetExperiment": {
             "access_level": "Undocumented",
-            "action": "GetTargetResourceType",
+            "action": "GetExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateExperimentTemplate": {
+        "StopExperiment": {
             "access_level": "Undocumented",
-            "action": "UpdateExperimentTemplate",
+            "action": "StopExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetAccountConfiguration": {
+        "ListExperimentTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetAccountConfiguration",
+            "action": "ListExperimentTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListExperiments": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListExperiments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperiments": {
+        "GetTargetResourceType": {
             "access_level": "Undocumented",
-            "action": "ListExperiments",
+            "action": "GetTargetResourceType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiInternalError": {
+        "ListExperimentTemplates": {
             "access_level": "Undocumented",
-            "action": "InjectApiInternalError",
+            "action": "ListExperimentTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetResourceTypes": {
+        "InjectApiUnavailableError": {
             "access_level": "Undocumented",
-            "action": "ListTargetResourceTypes",
+            "action": "InjectApiUnavailableError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetAccountConfiguration": {
+        "InjectApiInternalError": {
             "access_level": "Undocumented",
-            "action": "CreateTargetAccountConfiguration",
+            "action": "InjectApiInternalError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetAccountConfigurations": {
+        "CreateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListTargetAccountConfigurations",
+            "action": "CreateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperimentTargetAccountConfiguration": {
+        "GetTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTargetAccountConfiguration",
+            "action": "GetTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiThrottleError": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "InjectApiThrottleError",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentResolvedTargets": {
+        "ListTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListExperimentResolvedTargets",
+            "action": "ListTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperiment": {
+        "DeleteTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetExperiment",
+            "action": "DeleteTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetAccountConfiguration": {
+        "ListTargetResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetTargetAccountConfiguration",
+            "action": "ListTargetResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetExperimentTemplate": {
             "access_level": "Undocumented",
             "action": "GetExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAction": {
+        "DeleteExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "GetAction",
+            "action": "DeleteExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListExperimentResolvedTargets": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListExperimentResolvedTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTargetAccountConfigurations": {
+        "CreateExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTargetAccountConfigurations",
+            "action": "CreateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListActions": {
+        "InjectApiThrottleError": {
             "access_level": "Undocumented",
-            "action": "ListActions",
+            "action": "InjectApiThrottleError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTargetAccountConfiguration": {
+        "ListActions": {
             "access_level": "Undocumented",
-            "action": "UpdateTargetAccountConfiguration",
+            "action": "ListActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fms": {
@@ -72396,25 +72396,25 @@
             "access_level": "Undocumented",
             "action": "GetFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFreeTierAlertPreference": {
+        "GetFreeTierUsage": {
             "access_level": "Undocumented",
-            "action": "PutFreeTierAlertPreference",
+            "action": "GetFreeTierUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierUsage": {
+        "PutFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierUsage",
+            "action": "PutFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fsx": {
@@ -80606,169 +80606,169 @@
             "condition_keys": [],
             "description": "Grants permission to enable the Organizational View feature",
             "orphan": false,
             "resources": []
         }
     },
     "healthlake": {
-        "UpdateResource": {
+        "ListFHIRImportJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateResource",
+            "action": "ListFHIRImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRDatastores": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListFHIRDatastores",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFHIRDatastore": {
+        "DescribeFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "CreateFHIRDatastore",
+            "action": "DescribeFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadResource": {
+        "CreateFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "ReadResource",
+            "action": "CreateFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListFHIRDatastores": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListFHIRDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRExportJob": {
+        "ReadResource": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRExportJob",
+            "action": "ReadResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRExportJob": {
+        "ListFHIRExportJobs": {
             "access_level": "Undocumented",
-            "action": "StartFHIRExportJob",
+            "action": "ListFHIRExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRExportJobs": {
+        "SearchWithPost": {
             "access_level": "Undocumented",
-            "action": "ListFHIRExportJobs",
+            "action": "SearchWithPost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRImportJob": {
+        "SearchEverything": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRImportJob",
+            "action": "SearchEverything",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapabilities": {
+        "CreateResource": {
             "access_level": "Undocumented",
-            "action": "GetCapabilities",
+            "action": "CreateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithPost": {
+        "DescribeFHIRImportJob": {
             "access_level": "Undocumented",
-            "action": "SearchWithPost",
+            "action": "DescribeFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFHIRDatastore": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteFHIRDatastore",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRDatastore": {
+        "SearchWithGet": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRDatastore",
+            "action": "SearchWithGet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithGet": {
+        "GetCapabilities": {
             "access_level": "Undocumented",
-            "action": "SearchWithGet",
+            "action": "GetCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchEverything": {
+        "DeleteResource": {
             "access_level": "Undocumented",
-            "action": "SearchEverything",
+            "action": "DeleteResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRImportJobs": {
+        "DeleteFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "ListFHIRImportJobs",
+            "action": "DeleteFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResource": {
+        "DescribeFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "DeleteResource",
+            "action": "DescribeFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "StartFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "StartFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartFHIRImportJob": {
             "access_level": "Undocumented",
@@ -81042,1377 +81042,1377 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "UpdateAccessKey": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "GetMFADevice": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "GetMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMFADevice": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GetMFADevice",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -84653,41 +84653,41 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "PutInvoiceEmailDeliveryPreferences": {
+        "GetInvoicePDF": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoicePDF",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoiceEmailDeliveryPreferences": {
+        "ListInvoiceSummaries": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "ListInvoiceSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoicePDF": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoicePDF",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInvoiceSummaries": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "ListInvoiceSummaries",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iot": {
@@ -90852,913 +90852,913 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "ListMulticastGroups": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "GetMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "GetMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetDestination": {
             "access_level": "Undocumented",
             "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricConfiguration": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetMetricConfiguration",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "GetMetrics": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "GetMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetrics": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "GetMetrics",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
             "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMetricConfiguration": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "UpdateMetricConfiguration",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "UpdateMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "UpdateMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -94925,339 +94925,339 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "CreateRescoreExecutionPlan": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRescoreExecutionPlans": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListRescoreExecutionPlans",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRescoreExecutionPlan": {
+        "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRescoreExecutionPlan": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DeleteRescoreExecutionPlan",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRescoreExecutionPlan": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "ListTagsForStream": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourcePolicy": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "PutResourcePolicy",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "GetResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "GetResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetRecords": {
             "access_level": "Undocumented",
             "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicy": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicy",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "DeleteResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "DeleteResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStream": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "CreateStream",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SplitShard": {
             "access_level": "Undocumented",
             "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "PutResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "PutResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourcePolicy": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "DeleteResourcePolicy",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -97927,273 +97927,273 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "GetIpAddress": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceRecommendation": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "GetResourceRecommendation",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "GetResourceRecommendation": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "GetResourceRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "ListResourceCostEstimates": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "ListResourceCostEstimates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetResourceCostEstimate": {
             "access_level": "Undocumented",
             "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSettingsSet": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "GetSettingsSet",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentPatterns": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentPatterns",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "ListWorkloadDeploymentPatterns": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "ListWorkloadDeploymentPatterns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "GetDeployment": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "DeleteDeployment": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "DeleteDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSettingsSet": {
+        "ListDeployments": {
             "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
+            "action": "ListDeployments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeployment": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "DeleteDeployment",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAsset": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAsset",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "PutSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "PutSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllowedResources": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListAllowedResources",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeployment": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "GetDeployment",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeploymentEvents": {
+        "CreateDeployment": {
             "access_level": "Undocumented",
-            "action": "ListDeploymentEvents",
+            "action": "CreateDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeployment": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "CreateDeployment",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceCostEstimates": {
+        "GetSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListResourceCostEstimates",
+            "action": "GetSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkload": {
+        "ListDeploymentEvents": {
             "access_level": "Undocumented",
-            "action": "GetWorkload",
+            "action": "ListDeploymentEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "GetWorkload": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "GetWorkload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeployments": {
+        "GetWorkloadAsset": {
             "access_level": "Undocumented",
-            "action": "ListDeployments",
+            "action": "GetWorkloadAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSettingsSet": {
+        "ListAllowedResources": {
             "access_level": "Undocumented",
-            "action": "PutSettingsSet",
+            "action": "ListAllowedResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -105408,107 +105408,107 @@
             "orphan": false,
             "resources": [
                 "proposal"
             ]
         }
     },
     "managedblockchain-query": {
-        "GetAssetContract": {
+        "BatchGetTokenBalance": {
             "access_level": "Undocumented",
-            "action": "GetAssetContract",
+            "action": "BatchGetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFilteredTransactionEvents": {
+        "ListTransactions": {
             "access_level": "Undocumented",
-            "action": "ListFilteredTransactionEvents",
+            "action": "ListTransactions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAssetContracts": {
             "access_level": "Undocumented",
             "action": "ListAssetContracts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransactionEvents": {
+        "GetTransaction": {
             "access_level": "Undocumented",
-            "action": "ListTransactionEvents",
+            "action": "GetTransaction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransaction": {
+        "ListTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "GetTransaction",
+            "action": "ListTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTokenBalances": {
+        "ListFilteredTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "ListTokenBalances",
+            "action": "ListFilteredTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetTokenBalance": {
+        "GetTokenBalance": {
             "access_level": "Undocumented",
-            "action": "BatchGetTokenBalance",
+            "action": "GetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransactions": {
+        "ListTokenBalances": {
             "access_level": "Undocumented",
-            "action": "ListTransactions",
+            "action": "ListTokenBalances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTokenBalance": {
+        "GetAssetContract": {
             "access_level": "Undocumented",
-            "action": "GetTokenBalance",
+            "action": "GetAssetContract",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mapcredits": {
-        "ListAssociatedPrograms": {
+        "ListQuarterCredits": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedPrograms",
+            "action": "ListQuarterCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuarterCredits": {
+        "ListQuarterSpend": {
             "access_level": "Undocumented",
-            "action": "ListQuarterCredits",
+            "action": "ListQuarterSpend",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuarterSpend": {
+        "ListAssociatedPrograms": {
             "access_level": "Undocumented",
-            "action": "ListQuarterSpend",
+            "action": "ListAssociatedPrograms",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "marketplacecommerceanalytics": {
@@ -107952,225 +107952,225 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "CreateChannelGroup": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateChannelGroup",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelPolicy": {
+        "CreateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutOriginEndpointPolicy": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "PutOriginEndpointPolicy",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannelGroups": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "GetChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "GetChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpointPolicy": {
+        "PutChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpointPolicy",
+            "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "CreateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "ListOriginEndpoints": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannel": {
+        "CreateChannel": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHeadObject": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "GetHeadObject",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOriginEndpoint": {
+        "UpdateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "CreateOriginEndpoint",
+            "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannel": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutObject": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "PutObject",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelGroup": {
+        "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannelGroup": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "UpdateChannelGroup",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOriginEndpoint": {
+        "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateOriginEndpoint",
+            "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOriginEndpoints": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "ListOriginEndpoints",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutChannelPolicy": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "PutChannelPolicy",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "PutObject": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannel": {
+        "GetHeadObject": {
             "access_level": "Undocumented",
-            "action": "CreateChannel",
+            "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mediastore": {
@@ -108888,153 +108888,153 @@
             "orphan": false,
             "resources": [
                 "vodSource"
             ]
         }
     },
     "medical-imaging": {
-        "ListDICOMImportJobs": {
+        "ListImageSetVersions": {
             "access_level": "Undocumented",
-            "action": "ListDICOMImportJobs",
+            "action": "ListImageSetVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDatastore": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDatastore",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDatastore": {
+        "GetImageSet": {
             "access_level": "Undocumented",
-            "action": "CreateDatastore",
+            "action": "GetImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteImageSet": {
             "access_level": "Undocumented",
             "action": "DeleteImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDatastores": {
+        "GetDatastore": {
             "access_level": "Undocumented",
-            "action": "ListDatastores",
+            "action": "GetDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSet": {
+        "StartDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "GetImageSet",
+            "action": "StartDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateImageSetMetadata": {
+        "GetImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "UpdateImageSetMetadata",
+            "action": "GetImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListDICOMImportJobs": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListDICOMImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDatastore": {
+        "DeleteDatastore": {
             "access_level": "Undocumented",
-            "action": "GetDatastore",
+            "action": "DeleteDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDICOMImportJob": {
+        "ListDatastores": {
             "access_level": "Undocumented",
-            "action": "GetDICOMImportJob",
+            "action": "ListDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDICOMImportJob": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartDICOMImportJob",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyImageSet": {
+        "SearchImageSets": {
             "access_level": "Undocumented",
-            "action": "CopyImageSet",
+            "action": "SearchImageSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchImageSets": {
+        "CreateDatastore": {
             "access_level": "Undocumented",
-            "action": "SearchImageSets",
+            "action": "CreateDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImageSetVersions": {
+        "CopyImageSet": {
             "access_level": "Undocumented",
-            "action": "ListImageSetVersions",
+            "action": "CopyImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSetMetadata": {
+        "GetImageFrame": {
             "access_level": "Undocumented",
-            "action": "GetImageSetMetadata",
+            "action": "GetImageFrame",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageFrame": {
+        "GetDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "GetImageFrame",
+            "action": "GetDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "memorydb": {
@@ -113450,265 +113450,265 @@
             "orphan": false,
             "resources": [
                 "database"
             ]
         }
     },
     "neptune-graph": {
-        "ListGraphSnapshots": {
+        "CreatePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListGraphSnapshots",
+            "action": "CreatePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraph": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteGraph",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadDataViaQuery": {
+        "CancelImportTask": {
             "access_level": "Undocumented",
-            "action": "ReadDataViaQuery",
+            "action": "CancelImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphUsingImportTask": {
+        "GetStatisticsStatus": {
             "access_level": "Undocumented",
-            "action": "CreateGraphUsingImportTask",
+            "action": "GetStatisticsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImportTask": {
+        "DeleteGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "GetImportTask",
+            "action": "DeleteGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraph": {
+        "GetGraphSummary": {
             "access_level": "Undocumented",
-            "action": "GetGraph",
+            "action": "GetGraphSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetEngineStatus": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetEngineStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreGraphFromSnapshot": {
+        "ResetGraph": {
             "access_level": "Undocumented",
-            "action": "RestoreGraphFromSnapshot",
+            "action": "ResetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportTasks": {
+        "GetGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "ListImportTasks",
+            "action": "GetGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStatisticsStatus": {
+        "GetPrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetStatisticsStatus",
+            "action": "GetPrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivateGraphEndpoint": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreatePrivateGraphEndpoint",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEngineStatus": {
+        "WriteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "GetEngineStatus",
+            "action": "WriteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivateGraphEndpoint": {
+        "GetQueryStatus": {
             "access_level": "Undocumented",
-            "action": "DeletePrivateGraphEndpoint",
+            "action": "GetQueryStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraph": {
+        "StartImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateGraph",
+            "action": "StartImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSnapshot": {
+        "ListGraphSnapshots": {
             "access_level": "Undocumented",
-            "action": "GetGraphSnapshot",
+            "action": "ListGraphSnapshots",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelQuery": {
+        "ListGraphs": {
             "access_level": "Undocumented",
-            "action": "CancelQuery",
+            "action": "ListGraphs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetGraph": {
+        "DeleteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "ResetGraph",
+            "action": "DeleteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphSnapshot": {
+        "CreateGraphUsingImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateGraphSnapshot",
+            "action": "CreateGraphUsingImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivateGraphEndpoint": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetPrivateGraphEndpoint",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivateGraphEndpoints": {
+        "ReadDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "ListPrivateGraphEndpoints",
+            "action": "ReadDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueries": {
+        "CancelQuery": {
             "access_level": "Undocumented",
-            "action": "ListQueries",
+            "action": "CancelQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraphSnapshot": {
+        "UpdateGraph": {
             "access_level": "Undocumented",
-            "action": "DeleteGraphSnapshot",
+            "action": "UpdateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "WriteDataViaQuery": {
+        "ListPrivateGraphEndpoints": {
             "access_level": "Undocumented",
-            "action": "WriteDataViaQuery",
+            "action": "ListPrivateGraphEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataViaQuery": {
+        "CreateGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "DeleteDataViaQuery",
+            "action": "CreateGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelImportTask": {
+        "RestoreGraphFromSnapshot": {
             "access_level": "Undocumented",
-            "action": "CancelImportTask",
+            "action": "RestoreGraphFromSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteGraph": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGraph": {
+        "GetGraph": {
             "access_level": "Undocumented",
-            "action": "UpdateGraph",
+            "action": "GetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphs": {
+        "GetImportTask": {
             "access_level": "Undocumented",
-            "action": "ListGraphs",
+            "action": "GetImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueryStatus": {
+        "CreateGraph": {
             "access_level": "Undocumented",
-            "action": "GetQueryStatus",
+            "action": "CreateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportTask": {
+        "ListQueries": {
             "access_level": "Undocumented",
-            "action": "StartImportTask",
+            "action": "ListQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeletePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeletePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSummary": {
+        "ListImportTasks": {
             "access_level": "Undocumented",
-            "action": "GetGraphSummary",
+            "action": "ListImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "network-firewall": {
@@ -115075,163 +115075,163 @@
             "orphan": false,
             "resources": [
                 "attachment"
             ]
         }
     },
     "networkmanager-chat": {
-        "DeleteConversation": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "DeleteConversation",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendConversationMessage": {
+        "ListConversationMessages": {
             "access_level": "Undocumented",
-            "action": "SendConversationMessage",
+            "action": "ListConversationMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversationMessages": {
+        "CancelMessageResponse": {
             "access_level": "Undocumented",
-            "action": "ListConversationMessages",
+            "action": "CancelMessageResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "NotifyConversationIsActive": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "NotifyConversationIsActive",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMessageResponse": {
+        "CreateConversation": {
             "access_level": "Undocumented",
-            "action": "CancelMessageResponse",
+            "action": "CreateConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConversation": {
+        "DeleteConversation": {
             "access_level": "Undocumented",
-            "action": "CreateConversation",
+            "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyConversationIsActive": {
+        "SendConversationMessage": {
             "access_level": "Undocumented",
-            "action": "NotifyConversationIsActive",
+            "action": "SendConversationMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "networkmonitor": {
-        "ListMonitors": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProbe": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateProbe",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "DeleteProbe": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "DeleteProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProbe": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteProbe",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProbe": {
+        "UpdateProbe": {
             "access_level": "Undocumented",
-            "action": "CreateProbe",
+            "action": "UpdateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProbe": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetProbe",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "GetProbe": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "GetProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetMonitor": {
             "access_level": "Undocumented",
             "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateProbe": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "nimble": {
@@ -115799,251 +115799,251 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "GetEventRule": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationEvent": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventRule": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventRules": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "GetEmailContact": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateEmailContact": {
             "access_level": "Undocumented",
             "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendActivationCode": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "SendActivationCode",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEmailContacts": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "SendActivationCode": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -116221,883 +116221,883 @@
             "orphan": false,
             "resources": [
                 "Link"
             ]
         }
     },
     "omics": {
-        "DeleteRun": {
+        "DeleteShare": {
             "access_level": "Undocumented",
-            "action": "DeleteRun",
+            "action": "DeleteShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantStore": {
+        "ListMultipartReadSetUploads": {
             "access_level": "Undocumented",
-            "action": "GetVariantStore",
+            "action": "ListMultipartReadSetUploads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVariantStore": {
+        "ListVariantStores": {
             "access_level": "Undocumented",
-            "action": "DeleteVariantStore",
+            "action": "ListVariantStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantImportJob": {
+        "ListVariantImportJobs": {
             "access_level": "Undocumented",
-            "action": "GetVariantImportJob",
+            "action": "ListVariantImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelVariantImportJob": {
+        "CreateShare": {
             "access_level": "Undocumented",
-            "action": "CancelVariantImportJob",
+            "action": "CreateShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkflow": {
+        "CompleteMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkflow",
+            "action": "CompleteMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReference": {
+        "ListAnnotationStores": {
             "access_level": "Undocumented",
-            "action": "GetReference",
+            "action": "ListAnnotationStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRun": {
+        "CreateMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "GetRun",
+            "action": "CreateMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetImportJob": {
+        "StartAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReadSetImportJob",
+            "action": "StartAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetImportJobs": {
+        "CancelVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "ListReadSetImportJobs",
+            "action": "CancelVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteReadSet": {
+        "AcceptShare": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteReadSet",
+            "action": "AcceptShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferences": {
+        "GetRun": {
             "access_level": "Undocumented",
-            "action": "ListReferences",
+            "action": "GetRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRunGroup": {
+        "DeleteReferenceStore": {
             "access_level": "Undocumented",
-            "action": "DeleteRunGroup",
+            "action": "DeleteReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetExportJobs": {
+        "UpdateVariantStore": {
             "access_level": "Undocumented",
-            "action": "ListReadSetExportJobs",
+            "action": "UpdateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationImportJob": {
+        "GetReadSetMetadata": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationImportJob",
+            "action": "GetReadSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunTasks": {
+        "UpdateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "ListRunTasks",
+            "action": "UpdateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStoreVersion": {
+        "ListAnnotationImportJobs": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStoreVersion",
+            "action": "ListAnnotationImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetExportJob": {
+        "GetAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "StartReadSetExportJob",
+            "action": "GetAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetMetadata": {
+        "CreateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "GetReadSetMetadata",
+            "action": "CreateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteShare": {
+        "CreateRunGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteShare",
+            "action": "CreateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStoreVersions": {
+        "GetAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStoreVersions",
+            "action": "GetAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceStores": {
+        "ListReadSetUploadParts": {
             "access_level": "Undocumented",
-            "action": "ListReferenceStores",
+            "action": "ListReadSetUploadParts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShares": {
+        "CancelRun": {
             "access_level": "Undocumented",
-            "action": "ListShares",
+            "action": "CancelRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetImportJob": {
+        "ListSequenceStores": {
             "access_level": "Undocumented",
-            "action": "StartReadSetImportJob",
+            "action": "ListSequenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStore": {
+        "GetReadSet": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStore",
+            "action": "GetReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRunGroup": {
+        "BatchDeleteReadSet": {
             "access_level": "Undocumented",
-            "action": "UpdateRunGroup",
+            "action": "BatchDeleteReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSet": {
+        "StartVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReadSet",
+            "action": "StartVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStore": {
+        "GetReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStore",
+            "action": "GetReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantStores": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListVariantStores",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetActivationJob": {
+        "ListRuns": {
             "access_level": "Undocumented",
-            "action": "GetReadSetActivationJob",
+            "action": "ListRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStoreVersions": {
+        "ListReadSetImportJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStoreVersions",
+            "action": "ListReadSetImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkflow": {
+        "ListReadSetExportJobs": {
             "access_level": "Undocumented",
-            "action": "GetWorkflow",
+            "action": "ListReadSetExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartVariantImportJob": {
+        "GetVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "StartVariantImportJob",
+            "action": "GetVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkflows": {
+        "StartReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "ListWorkflows",
+            "action": "StartReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRuns": {
+        "ListReferences": {
             "access_level": "Undocumented",
-            "action": "ListRuns",
+            "action": "ListReferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAnnotationImportJob": {
+        "DeleteSequenceStore": {
             "access_level": "Undocumented",
-            "action": "StartAnnotationImportJob",
+            "action": "DeleteSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVariantStore": {
+        "CreateSequenceStore": {
             "access_level": "Undocumented",
-            "action": "CreateVariantStore",
+            "action": "CreateSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSequenceStores": {
+        "ListReferenceImportJobs": {
             "access_level": "Undocumented",
-            "action": "ListSequenceStores",
+            "action": "ListReferenceImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListRunGroups": {
             "access_level": "Undocumented",
             "action": "ListRunGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AbortMultipartReadSetUpload": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "AbortMultipartReadSetUpload",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRunGroup": {
+        "GetReferenceMetadata": {
             "access_level": "Undocumented",
-            "action": "CreateRunGroup",
+            "action": "GetReferenceMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorkflow": {
+        "DeleteRunGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteWorkflow",
+            "action": "DeleteRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunGroup": {
+        "StartReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "GetRunGroup",
+            "action": "StartReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CompleteMultipartReadSetUpload": {
+        "DeleteAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "CompleteMultipartReadSetUpload",
+            "action": "DeleteAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetReferenceStore": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStoreVersion": {
+        "StartReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStoreVersion",
+            "action": "StartReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReference": {
+        "GetSequenceStore": {
             "access_level": "Undocumented",
-            "action": "DeleteReference",
+            "action": "GetSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptShare": {
+        "DeleteRun": {
             "access_level": "Undocumented",
-            "action": "AcceptShare",
+            "action": "DeleteRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetActivationJobs": {
+        "GetWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListReadSetActivationJobs",
+            "action": "GetWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStores": {
+        "ListReadSetActivationJobs": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStores",
+            "action": "ListReadSetActivationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSequenceStore": {
+        "CancelAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "GetSequenceStore",
+            "action": "CancelAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShare": {
+        "ListReadSets": {
             "access_level": "Undocumented",
-            "action": "GetShare",
+            "action": "ListReadSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStoreVersion": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStoreVersion",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSequenceStore": {
+        "GetReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "CreateSequenceStore",
+            "action": "GetReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMultipartReadSetUpload": {
+        "UploadReadSetPart": {
             "access_level": "Undocumented",
-            "action": "CreateMultipartReadSetUpload",
+            "action": "UploadReadSetPart",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelAnnotationImportJob": {
+        "AbortMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "CancelAnnotationImportJob",
+            "action": "AbortMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationImportJobs": {
+        "CreateVariantStore": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationImportJobs",
+            "action": "CreateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadReadSetPart": {
+        "UpdateWorkflow": {
             "access_level": "Undocumented",
-            "action": "UploadReadSetPart",
+            "action": "UpdateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceImportJob": {
+        "ListWorkflows": {
             "access_level": "Undocumented",
-            "action": "GetReferenceImportJob",
+            "action": "ListWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceStore": {
+        "ListShares": {
             "access_level": "Undocumented",
-            "action": "GetReferenceStore",
+            "action": "ListShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateShare": {
+        "DeleteAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "CreateShare",
+            "action": "DeleteAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetActivationJob": {
+        "StartRun": {
             "access_level": "Undocumented",
-            "action": "StartReadSetActivationJob",
+            "action": "StartRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReferenceImportJob": {
+        "CreateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "StartReferenceImportJob",
+            "action": "CreateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelRun": {
+        "UpdateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "CancelRun",
+            "action": "UpdateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceMetadata": {
+        "GetShare": {
             "access_level": "Undocumented",
-            "action": "GetReferenceMetadata",
+            "action": "GetShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantImportJobs": {
+        "UpdateRunGroup": {
             "access_level": "Undocumented",
-            "action": "ListVariantImportJobs",
+            "action": "UpdateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateReferenceStore": {
+        "ListRunTasks": {
             "access_level": "Undocumented",
-            "action": "CreateReferenceStore",
+            "action": "ListRunTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSets": {
+        "DeleteReference": {
             "access_level": "Undocumented",
-            "action": "ListReadSets",
+            "action": "DeleteReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStore": {
+        "CreateWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStore",
+            "action": "CreateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRun": {
+        "GetReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "StartRun",
+            "action": "GetReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateVariantStore": {
+        "ListReferenceStores": {
             "access_level": "Undocumented",
-            "action": "UpdateVariantStore",
+            "action": "ListReferenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteWorkflow": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorkflow": {
+        "GetVariantStore": {
             "access_level": "Undocumented",
-            "action": "CreateWorkflow",
+            "action": "GetVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMultipartReadSetUploads": {
+        "GetAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "ListMultipartReadSetUploads",
+            "action": "GetAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceImportJobs": {
+        "GetRunTask": {
             "access_level": "Undocumented",
-            "action": "ListReferenceImportJobs",
+            "action": "GetRunTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReferenceStore": {
+        "DeleteVariantStore": {
             "access_level": "Undocumented",
-            "action": "DeleteReferenceStore",
+            "action": "DeleteVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetExportJob": {
+        "StartReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReadSetExportJob",
+            "action": "StartReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetUploadParts": {
+        "ListAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "ListReadSetUploadParts",
+            "action": "ListAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSequenceStore": {
+        "CreateReferenceStore": {
             "access_level": "Undocumented",
-            "action": "DeleteSequenceStore",
+            "action": "CreateReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunTask": {
+        "GetReference": {
             "access_level": "Undocumented",
-            "action": "GetRunTask",
+            "action": "GetReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStore": {
+        "GetRunGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStore",
+            "action": "GetRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "one": {
-        "GetDeviceInstance": {
+        "CreateDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstance",
+            "action": "CreateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSite": {
+        "CreateDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateSite",
+            "action": "CreateDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSiteAddress": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetSiteAddress",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSite": {
+        "DeleteDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteSite",
+            "action": "DeleteDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RebootDevice": {
+        "GetSiteAddress": {
             "access_level": "Undocumented",
-            "action": "RebootDevice",
+            "action": "GetSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteAssociatedDevice": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteAssociatedDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSites": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "ListSites",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstance": {
+        "CreateDeviceActivationQrCode": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstance",
+            "action": "CreateDeviceActivationQrCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDeviceInstance": {
+        "GetSite": {
             "access_level": "Undocumented",
-            "action": "UpdateDeviceInstance",
+            "action": "GetSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDeviceConfigurationTemplate": {
+        "ListDeviceConfigurationTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdateDeviceConfigurationTemplate",
+            "action": "ListDeviceConfigurationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceConfigurationTemplate": {
+        "ListSites": {
             "access_level": "Undocumented",
-            "action": "GetDeviceConfigurationTemplate",
+            "action": "ListSites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListDeviceInstances": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListDeviceInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstanceConfiguration": {
+        "CreateSite": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstanceConfiguration",
+            "action": "CreateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "GetDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "GetDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceConfigurationTemplates": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "ListDeviceConfigurationTemplates",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSite": {
+        "UpdateSiteAddress": {
             "access_level": "Undocumented",
-            "action": "UpdateSite",
+            "action": "UpdateSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstanceConfiguration": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstanceConfiguration",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "DeleteDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "DeleteDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceConfigurationTemplate": {
+        "UpdateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceConfigurationTemplate",
+            "action": "UpdateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceConfigurationTemplate": {
+        "DeleteSite": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceConfigurationTemplate",
+            "action": "DeleteSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSite": {
+        "UpdateDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "GetSite",
+            "action": "UpdateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceActivationQrCode": {
+        "CreateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceActivationQrCode",
+            "action": "CreateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssociatedDevice": {
+        "UpdateSite": {
             "access_level": "Undocumented",
-            "action": "DeleteAssociatedDevice",
+            "action": "UpdateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceInstances": {
+        "RebootDevice": {
             "access_level": "Undocumented",
-            "action": "ListDeviceInstances",
+            "action": "RebootDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSiteAddress": {
+        "GetDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateSiteAddress",
+            "action": "GetDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "opsworks": {
@@ -118570,129 +118570,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "GetPipelineChangeProgress": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePipeline": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePipeline": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Ingest": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelines": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipeline": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipeline",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelineBlueprints": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetPipeline": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -119355,333 +119355,333 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "partnercentral-account-management": {
-        "AssociatePartnerUser": {
+        "AssociatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "AssociatePartnerUser",
+            "action": "AssociatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisassociatePartnerUser": {
             "access_level": "Undocumented",
             "action": "DisassociatePartnerUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociatePartnerAccount": {
+        "AssociatePartnerUser": {
             "access_level": "Undocumented",
-            "action": "AssociatePartnerAccount",
+            "action": "AssociatePartnerUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payment-cryptography": {
-        "GenerateCardValidationData": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "GenerateCardValidationData",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyPinData": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAlias": {
+        "GetAlias": {
             "access_level": "Undocumented",
-            "action": "DeleteAlias",
+            "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPublicKeyCertificate": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAlias": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "CreateAlias",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAlias": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetAlias",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "GenerateCardValidationData": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ExportKey": {
+        "VerifyMac": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopKeyUsage": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyMac": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "VerifyMac",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "CreateAlias": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TranslatePinData": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "TranslatePinData",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "ListAliases": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "DeleteAlias": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "DeleteAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "TranslatePinData": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAliases": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "ListAliases",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "CreatePaymentInstrument": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentStatus": {
+        "DeletePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "GetPaymentStatus",
+            "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
             "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePaymentInstrument": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "DeletePaymentInstrument",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPaymentPreferences": {
+        "GetPaymentStatus": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "MakePayment": {
             "access_level": "Undocumented",
@@ -119689,209 +119689,209 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "pca-connector-ad": {
-        "GetServicePrincipalName": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetServicePrincipalName",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplateGroupAccessControlEntry": {
+        "UpdateTemplate": {
             "access_level": "Undocumented",
-            "action": "GetTemplateGroupAccessControlEntry",
+            "action": "UpdateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplate": {
+        "GetServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "CreateTemplate",
+            "action": "GetServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConnector": {
+        "DeleteDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "GetConnector",
+            "action": "DeleteDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTemplateGroupAccessControlEntry": {
+        "GetConnector": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplateGroupAccessControlEntry",
+            "action": "GetConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplate": {
+        "ListConnectors": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplate",
+            "action": "ListConnectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnector": {
+        "CreateDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "DeleteConnector",
+            "action": "CreateDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnector": {
+        "CreateTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateConnector",
+            "action": "CreateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplateGroupAccessControlEntry": {
+        "GetTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateTemplateGroupAccessControlEntry",
+            "action": "GetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServicePrincipalName": {
+        "ListServicePrincipalNames": {
             "access_level": "Undocumented",
-            "action": "DeleteServicePrincipalName",
+            "action": "ListServicePrincipalNames",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConnectors": {
+        "UpdateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "ListConnectors",
+            "action": "UpdateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDirectoryRegistration": {
+        "DeleteTemplate": {
             "access_level": "Undocumented",
-            "action": "GetDirectoryRegistration",
+            "action": "DeleteTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDirectoryRegistration": {
+        "ListDirectoryRegistrations": {
             "access_level": "Undocumented",
-            "action": "DeleteDirectoryRegistration",
+            "action": "ListDirectoryRegistrations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServicePrincipalNames": {
+        "ListTemplates": {
             "access_level": "Undocumented",
-            "action": "ListServicePrincipalNames",
+            "action": "ListTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDirectoryRegistration": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateDirectoryRegistration",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplateGroupAccessControlEntry": {
+        "ListTemplateGroupAccessControlEntries": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplateGroupAccessControlEntry",
+            "action": "ListTemplateGroupAccessControlEntries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplates": {
+        "GetDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "ListTemplates",
+            "action": "GetDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplate": {
+        "CreateConnector": {
             "access_level": "Undocumented",
-            "action": "GetTemplate",
+            "action": "CreateConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplateGroupAccessControlEntries": {
+        "CreateServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "ListTemplateGroupAccessControlEntries",
+            "action": "CreateServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTemplate": {
+        "GetTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplate",
+            "action": "GetTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDirectoryRegistrations": {
+        "DeleteServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "ListDirectoryRegistrations",
+            "action": "DeleteServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServicePrincipalName": {
+        "DeleteConnector": {
             "access_level": "Undocumented",
-            "action": "CreateServicePrincipalName",
+            "action": "DeleteConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -123221,579 +123221,579 @@
             "orphan": false,
             "resources": [
                 "purchase-order"
             ]
         }
     },
     "q": {
-        "StartTroubleshootingAnalysis": {
+        "GetConversation": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingAnalysis",
+            "action": "GetConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConversation": {
+        "PassRequest": {
             "access_level": "Undocumented",
-            "action": "GetConversation",
+            "action": "PassRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTroubleshootingResolutionExplanation": {
+        "GetTroubleshootingResults": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingResolutionExplanation",
+            "action": "GetTroubleshootingResults",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartConversation": {
+        "UpdateTroubleshootingCommandResult": {
             "access_level": "Undocumented",
-            "action": "StartConversation",
+            "action": "UpdateTroubleshootingCommandResult",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendMessage": {
+        "StartConversation": {
             "access_level": "Undocumented",
-            "action": "SendMessage",
+            "action": "StartConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRequest": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "PassRequest",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentityMetadata": {
+        "SendMessage": {
             "access_level": "Undocumented",
-            "action": "GetIdentityMetadata",
+            "action": "SendMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTroubleshootingCommandResult": {
+        "StartTroubleshootingAnalysis": {
             "access_level": "Undocumented",
-            "action": "UpdateTroubleshootingCommandResult",
+            "action": "StartTroubleshootingAnalysis",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "StartTroubleshootingResolutionExplanation": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "StartTroubleshootingResolutionExplanation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTroubleshootingResults": {
+        "GetIdentityMetadata": {
             "access_level": "Undocumented",
-            "action": "GetTroubleshootingResults",
+            "action": "GetIdentityMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qbusiness": {
-        "CreatePlugin": {
+        "DeleteChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreatePlugin",
+            "action": "DeleteChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConversation": {
+        "GetRetriever": {
             "access_level": "Undocumented",
-            "action": "DeleteConversation",
+            "action": "GetRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChatControlsConfiguration": {
+        "CreateApplication": {
             "access_level": "Undocumented",
-            "action": "DeleteChatControlsConfiguration",
+            "action": "CreateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPlugin": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetPlugin",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "DeleteApplication": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "DeleteApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDocuments": {
+        "GetPlugin": {
             "access_level": "Undocumented",
-            "action": "ListDocuments",
+            "action": "GetPlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Chat": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "Chat",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserLicenses": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "RemoveUserLicenses",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopDataSourceSyncJob": {
+        "ListWebExperiences": {
             "access_level": "Undocumented",
-            "action": "StopDataSourceSyncJob",
+            "action": "ListWebExperiences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchPutDocument": {
+        "DeleteConversation": {
             "access_level": "Undocumented",
-            "action": "BatchPutDocument",
+            "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "AddUserLicenses": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "AddUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWebExperiences": {
+        "ListUserLicenses": {
             "access_level": "Undocumented",
-            "action": "ListWebExperiences",
+            "action": "ListUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "BatchPutDocument": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "BatchPutDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePlugin": {
+        "UpdateIndex": {
             "access_level": "Undocumented",
-            "action": "DeletePlugin",
+            "action": "UpdateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "CreateIndex": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "CreateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApplication": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateApplication",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteDocument": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteDocument",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "UpdateWebExperience": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "UpdateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdatePlugin": {
             "access_level": "Undocumented",
             "action": "UpdatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWebExperience": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "UpdateWebExperience",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndex": {
+        "GetChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetIndex",
+            "action": "GetChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "ListApplications": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "ListApplications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChatControlsConfiguration": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "GetChatControlsConfiguration",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRetriever": {
+        "CreatePlugin": {
             "access_level": "Undocumented",
-            "action": "GetRetriever",
+            "action": "CreatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "GetIndex": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "GetIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMessages": {
+        "ListDocuments": {
             "access_level": "Undocumented",
-            "action": "ListMessages",
+            "action": "ListDocuments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIndex": {
+        "GetWebExperience": {
             "access_level": "Undocumented",
-            "action": "CreateIndex",
+            "action": "GetWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRetriever": {
+        "PutGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateRetriever",
+            "action": "PutGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChatSync": {
+        "RemoveUserLicenses": {
             "access_level": "Undocumented",
-            "action": "ChatSync",
+            "action": "RemoveUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserLicenses": {
+        "UpdateApplication": {
             "access_level": "Undocumented",
-            "action": "AddUserLicenses",
+            "action": "UpdateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceSyncJobs": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceSyncJobs",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "ChatSync": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "ChatSync",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRetrievers": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "ListRetrievers",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPlugins": {
+        "CreateRetriever": {
             "access_level": "Undocumented",
-            "action": "ListPlugins",
+            "action": "CreateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateWebExperience": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserLicenses": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListUserLicenses",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWebExperience": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateWebExperience",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceSyncJob": {
+        "ListMessages": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceSyncJob",
+            "action": "ListMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "DeleteIndex": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "DeleteIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIndex": {
+        "BatchDeleteDocument": {
             "access_level": "Undocumented",
-            "action": "DeleteIndex",
+            "action": "BatchDeleteDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicense": {
+        "ListIndices": {
             "access_level": "Undocumented",
-            "action": "CreateLicense",
+            "action": "ListIndices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRetriever": {
+        "StartDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "DeleteRetriever",
+            "action": "StartDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroup": {
+        "CreateLicense": {
             "access_level": "Undocumented",
-            "action": "PutGroup",
+            "action": "CreateLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "DeleteWebExperience": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "DeleteWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApplication": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "UpdateApplication",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIndices": {
+        "UpdateChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListIndices",
+            "action": "UpdateChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetLicense": {
             "access_level": "Undocumented",
             "action": "GetLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "StopDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "StopDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "UpdateRetriever": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "UpdateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWebExperience": {
+        "ListRetrievers": {
             "access_level": "Undocumented",
-            "action": "DeleteWebExperience",
+            "action": "ListRetrievers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChatControlsConfiguration": {
+        "DeletePlugin": {
             "access_level": "Undocumented",
-            "action": "UpdateChatControlsConfiguration",
+            "action": "DeletePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFeedback": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "ListPlugins": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "ListPlugins",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIndex": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateIndex",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWebExperience": {
+        "ListDataSourceSyncJobs": {
             "access_level": "Undocumented",
-            "action": "GetWebExperience",
+            "action": "ListDataSourceSyncJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApplications": {
+        "DeleteRetriever": {
             "access_level": "Undocumented",
-            "action": "ListApplications",
+            "action": "DeleteRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRetriever": {
+        "Chat": {
             "access_level": "Undocumented",
-            "action": "CreateRetriever",
+            "action": "Chat",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetApplication": {
             "access_level": "Undocumented",
             "action": "GetApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApplication": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteApplication",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qldb": {
@@ -126250,281 +126250,281 @@
             "orphan": false,
             "resources": [
                 "vpcconnection"
             ]
         }
     },
     "ram": {
-        "DeletePermission": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteResourceShare": {
             "access_level": "Undocumented",
             "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -131906,557 +131906,557 @@
             "orphan": false,
             "resources": [
                 "streamprocessor"
             ]
         }
     },
     "repostspace": {
-        "SendInvites": {
+        "ListSpaces": {
             "access_level": "Undocumented",
-            "action": "SendInvites",
+            "action": "ListSpaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSpaces": {
+        "RegisterAdmin": {
             "access_level": "Undocumented",
-            "action": "ListSpaces",
+            "action": "RegisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterAdmin": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeregisterAdmin",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterAdmin": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "RegisterAdmin",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSpace": {
+        "DeleteSpace": {
             "access_level": "Undocumented",
-            "action": "CreateSpace",
+            "action": "DeleteSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateSpace": {
             "access_level": "Undocumented",
             "action": "UpdateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "SendInvites": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "SendInvites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSpace": {
+        "CreateSpace": {
             "access_level": "Undocumented",
-            "action": "GetSpace",
+            "action": "CreateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeregisterAdmin": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeregisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSpace": {
+        "GetSpace": {
             "access_level": "Undocumented",
-            "action": "DeleteSpace",
+            "action": "GetSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resiliencehub": {
-        "DescribeAppAssessment": {
+        "DeleteAppAssessment": {
             "access_level": "Undocumented",
-            "action": "DescribeAppAssessment",
+            "action": "DeleteAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAssessment": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAssessment",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionAppComponents": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionAppComponents",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDraftAppVersionTemplate": {
+        "ListAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "PutDraftAppVersionTemplate",
+            "action": "ListAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResource": {
+        "CreateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResource",
+            "action": "CreateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionResource": {
+        "BatchUpdateRecommendationStatus": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionResource",
+            "action": "BatchUpdateRecommendationStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchUpdateRecommendationStatus": {
+        "ListUnsupportedAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "BatchUpdateRecommendationStatus",
+            "action": "ListUnsupportedAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PublishAppVersion": {
+        "DescribeAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "PublishAppVersion",
+            "action": "DescribeAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeResiliencyPolicy": {
+        "DescribeAppVersion": {
             "access_level": "Undocumented",
-            "action": "DescribeResiliencyPolicy",
+            "action": "DescribeAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "DeleteAppInputSource": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "DeleteAppInputSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResiliencyPolicy": {
+        "UpdateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "CreateResiliencyPolicy",
+            "action": "UpdateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionAppComponent": {
+        "DescribeAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionAppComponent",
+            "action": "DescribeAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResourceMappings": {
+        "CreateRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResourceMappings",
+            "action": "CreateRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersions": {
+        "DescribeApp": {
             "access_level": "Undocumented",
-            "action": "ListAppVersions",
+            "action": "DescribeApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApp": {
+        "ImportResourcesToDraftAppVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateApp",
+            "action": "ImportResourcesToDraftAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppInputSource": {
+        "RemoveDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "DeleteAppInputSource",
+            "action": "RemoveDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResourcesResolutionStatus": {
+        "CreateApp": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResourcesResolutionStatus",
+            "action": "CreateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessmentComplianceDrifts": {
+        "UpdateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessmentComplianceDrifts",
+            "action": "UpdateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessments": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessments",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResolveAppVersionResources": {
+        "CreateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ResolveAppVersionResources",
+            "action": "CreateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportResourcesToDraftAppVersion": {
+        "ListAppAssessments": {
             "access_level": "Undocumented",
-            "action": "ImportResourcesToDraftAppVersion",
+            "action": "ListAppAssessments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRecommendationTemplate": {
+        "ListAppComponentCompliances": {
             "access_level": "Undocumented",
-            "action": "DeleteRecommendationTemplate",
+            "action": "ListAppComponentCompliances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveDraftAppVersionResourceMappings": {
+        "ListResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "RemoveDraftAppVersionResourceMappings",
+            "action": "ListResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResiliencyPolicy": {
+        "ListSuggestedResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteResiliencyPolicy",
+            "action": "ListSuggestedResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionTemplate": {
+        "ListAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionTemplate",
+            "action": "ListAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersion": {
+        "ListAppAssessmentComplianceDrifts": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersion",
+            "action": "ListAppAssessmentComplianceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSuggestedResiliencyPolicies": {
+        "PublishAppVersion": {
             "access_level": "Undocumented",
-            "action": "ListSuggestedResiliencyPolicies",
+            "action": "PublishAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionResource": {
+        "ListAppInputSources": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionResource",
+            "action": "ListAppInputSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersion": {
+        "AddDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersion",
+            "action": "AddDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppAssessment": {
+        "UpdateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "StartAppAssessment",
+            "action": "UpdateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddDraftAppVersionResourceMappings": {
+        "DescribeResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "AddDraftAppVersionResourceMappings",
+            "action": "DescribeResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionAppComponent": {
+        "StartAppAssessment": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionAppComponent",
+            "action": "StartAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAlarmRecommendations": {
+        "DescribeAppAssessment": {
             "access_level": "Undocumented",
-            "action": "ListAlarmRecommendations",
+            "action": "DescribeAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResiliencyPolicies": {
+        "DescribeAppVersionResourcesResolutionStatus": {
             "access_level": "Undocumented",
-            "action": "ListResiliencyPolicies",
+            "action": "DescribeAppVersionResourcesResolutionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionResource": {
+        "DescribeDraftAppVersionResourcesImportStatus": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionResource",
+            "action": "DescribeDraftAppVersionResourcesImportStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeApp": {
+        "DeleteAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "DescribeApp",
+            "action": "DeleteAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApps": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListApps",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeDraftAppVersionResourcesImportStatus": {
+        "ListAppComponentRecommendations": {
             "access_level": "Undocumented",
-            "action": "DescribeDraftAppVersionResourcesImportStatus",
+            "action": "ListAppComponentRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentRecommendations": {
+        "ListApps": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentRecommendations",
+            "action": "ListApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRecommendationTemplate": {
+        "ListTestRecommendations": {
             "access_level": "Undocumented",
-            "action": "CreateRecommendationTemplate",
+            "action": "ListTestRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUnsupportedAppVersionResources": {
+        "UpdateApp": {
             "access_level": "Undocumented",
-            "action": "ListUnsupportedAppVersionResources",
+            "action": "UpdateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionAppComponent": {
+        "ListRecommendationTemplates": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionAppComponent",
+            "action": "ListRecommendationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppInputSources": {
+        "ListAlarmRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListAppInputSources",
+            "action": "ListAlarmRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListAppVersionAppComponents": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListAppVersionAppComponents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentCompliances": {
+        "DeleteAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentCompliances",
+            "action": "DeleteAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResources": {
+        "PutDraftAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResources",
+            "action": "PutDraftAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionAppComponent": {
+        "ListAppVersions": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionAppComponent",
+            "action": "ListAppVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSopRecommendations": {
             "access_level": "Undocumented",
             "action": "ListSopRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationTemplates": {
+        "CreateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationTemplates",
+            "action": "CreateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTestRecommendations": {
+        "DeleteRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "ListTestRecommendations",
+            "action": "DeleteRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResiliencyPolicy": {
+        "DescribeAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "UpdateResiliencyPolicy",
+            "action": "DescribeAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApp": {
+        "UpdateAppVersion": {
             "access_level": "Undocumented",
-            "action": "CreateApp",
+            "action": "UpdateAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ResolveAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ResolveAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer": {
-        "ListResourceTypes": {
+        "ListTags": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "ListTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTags": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "ListTags",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer-2": {
@@ -135410,41 +135410,33 @@
             "condition_keys": [],
             "description": "Grants permission to get all the domain-related billing records for the current AWS account for a specified period",
             "orphan": false,
             "resources": []
         }
     },
     "route53profiles": {
-        "GetProfileAssociation": {
-            "access_level": "Undocumented",
-            "action": "GetProfileAssociation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "DisassociateProfile": {
+        "ListProfileAssociations": {
             "access_level": "Undocumented",
-            "action": "DisassociateProfile",
+            "action": "ListProfileAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfileResourceAssociations": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListProfileResourceAssociations",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateProfile": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetProfile": {
             "access_level": "Undocumented",
@@ -135458,89 +135450,97 @@
             "access_level": "Undocumented",
             "action": "DeleteProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfileResourceAssociation": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetProfileResourceAssociation",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListProfileResourceAssociations": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListProfileResourceAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisassociateResourceFromProfile": {
             "access_level": "Undocumented",
             "action": "DisassociateResourceFromProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceToProfile": {
+        "GetProfileAssociation": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceToProfile",
+            "action": "GetProfileAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProfileResourceAssociation": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateProfileResourceAssociation",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListProfiles": {
             "access_level": "Undocumented",
             "action": "ListProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfileAssociations": {
+        "GetProfileResourceAssociation": {
             "access_level": "Undocumented",
-            "action": "ListProfileAssociations",
+            "action": "GetProfileResourceAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AssociateProfile": {
             "access_level": "Undocumented",
             "action": "AssociateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProfile": {
+        "DisassociateProfile": {
             "access_level": "Undocumented",
-            "action": "CreateProfile",
+            "action": "DisassociateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "AssociateResourceToProfile": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "AssociateResourceToProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateProfileResourceAssociation": {
+            "access_level": "Undocumented",
+            "action": "UpdateProfileResourceAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "route53resolver": {
@@ -140560,65 +140560,65 @@
             "orphan": false,
             "resources": [
                 "object"
             ]
         }
     },
     "s3express": {
-        "PutBucketPolicy": {
+        "DeleteBucket": {
             "access_level": "Undocumented",
-            "action": "PutBucketPolicy",
+            "action": "DeleteBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBucket": {
+        "DeleteBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateBucket",
+            "action": "DeleteBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBucketPolicy": {
+        "ListAllMyDirectoryBuckets": {
             "access_level": "Undocumented",
-            "action": "GetBucketPolicy",
+            "action": "ListAllMyDirectoryBuckets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "PutBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "PutBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllMyDirectoryBuckets": {
+        "CreateBucket": {
             "access_level": "Undocumented",
-            "action": "ListAllMyDirectoryBuckets",
+            "action": "CreateBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBucketPolicy": {
+        "GetBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteBucketPolicy",
+            "action": "GetBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBucket": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "DeleteBucket",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sagemaker": {
@@ -145399,137 +145399,137 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "CreateSSOApplication": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBillOfMaterialsImportJob": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "CreateBillOfMaterialsImportJob",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillOfMaterialsImportJob": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "GetBillOfMaterialsImportJob",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataIntegrationEvent": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "SendDataIntegrationEvent",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "SendDataIntegrationEvent": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "SendDataIntegrationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "CreateBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "CreateBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "GetBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "GetBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -156562,25 +156562,25 @@
             "access_level": "Undocumented",
             "action": "OpenControlChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataChannel": {
+        "CreateControlChannel": {
             "access_level": "Undocumented",
-            "action": "CreateDataChannel",
+            "action": "CreateControlChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateControlChannel": {
+        "CreateDataChannel": {
             "access_level": "Undocumented",
-            "action": "CreateControlChannel",
+            "action": "CreateDataChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "OpenDataChannel": {
             "access_level": "Undocumented",
@@ -161412,145 +161412,145 @@
             "orphan": false,
             "resources": [
                 "adapter"
             ]
         }
     },
     "thinclient": {
-        "GetEnvironment": {
-            "access_level": "Undocumented",
-            "action": "GetEnvironment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "GetSoftwareSet": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetSoftwareSet",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeregisterDevice": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeregisterDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateDevice": {
             "access_level": "Undocumented",
             "action": "UpdateDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSoftwareSet": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSoftwareSet",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDevices": {
             "access_level": "Undocumented",
             "action": "ListDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetDevice": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSoftwareSets": {
+        "DeleteDevice": {
             "access_level": "Undocumented",
-            "action": "ListSoftwareSets",
+            "action": "DeleteDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterDevice": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeregisterDevice",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListEnvironments": {
             "access_level": "Undocumented",
             "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDevice": {
+        "GetSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "DeleteDevice",
+            "action": "GetSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteEnvironment": {
             "access_level": "Undocumented",
             "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "ListDeviceSessions": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "ListDeviceSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceSessions": {
+        "UpdateSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "ListDeviceSessions",
+            "action": "UpdateSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDevice": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetDevice",
+            "action": "UpdateEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListSoftwareSets": {
+            "access_level": "Undocumented",
+            "action": "ListSoftwareSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "timestream": {
@@ -161900,97 +161900,97 @@
             "orphan": false,
             "resources": [
                 "table"
             ]
         }
     },
     "timestream-influxdb": {
-        "CreateDbParameterGroup": {
+        "GetDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "CreateDbParameterGroup",
+            "action": "GetDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDbInstance": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateDbInstance",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteDbInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDbInstance": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDbInstance",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDbInstance": {
+        "CreateDbInstance": {
             "access_level": "Undocumented",
-            "action": "GetDbInstance",
+            "action": "CreateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDbInstances": {
             "access_level": "Undocumented",
             "action": "ListDbInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDbParameterGroup": {
+        "ListDbParameterGroups": {
             "access_level": "Undocumented",
-            "action": "GetDbParameterGroup",
+            "action": "ListDbParameterGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDbParameterGroups": {
+        "UpdateDbInstance": {
             "access_level": "Undocumented",
-            "action": "ListDbParameterGroups",
+            "action": "UpdateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDbInstance": {
+        "GetDbInstance": {
             "access_level": "Undocumented",
-            "action": "CreateDbInstance",
+            "action": "GetDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "tiros": {
@@ -162032,185 +162032,169 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "PutSolNetworkPackageContent": {
-            "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "UpdateSolFunctionPackage": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
             "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
             "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
             "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSolNetworkInstances": {
             "access_level": "Undocumented",
             "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
-            "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
         "ListSolFunctionInstances": {
             "access_level": "Undocumented",
             "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UntagResource": {
             "access_level": "Undocumented",
@@ -162224,81 +162208,97 @@
             "access_level": "Undocumented",
             "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetSolNetworkOperation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ValidateSolFunctionPackageContent": {
+            "access_level": "Undocumented",
+            "action": "ValidateSolFunctionPackageContent",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListSolFunctionPackages": {
+            "access_level": "Undocumented",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -163998,81 +163998,81 @@
             "condition_keys": [],
             "description": "Grants permission to update the risk status in AWS Trusted Advisor Priority",
             "orphan": false,
             "resources": []
         }
     },
     "ts": {
-        "GetExecution": {
+        "ListTools": {
             "access_level": "Undocumented",
-            "action": "GetExecution",
+            "action": "ListTools",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "GetExecution": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTools": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTools",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExecutionOutput": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetExecutionOutput",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTool": {
+        "GetExecutionOutput": {
             "access_level": "Undocumented",
-            "action": "GetTool",
+            "action": "GetExecutionOutput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartExecution": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetTool": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetTool",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExecution": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "StartExecution",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "vendor-insights": {
@@ -164358,201 +164358,201 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "verifiedpermissions": {
-        "CreatePolicy": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPolicies": {
             "access_level": "Undocumented",
             "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentitySource": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyTemplate": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyTemplate",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyStores": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "ListPolicyStores",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdatePolicyStore": {
             "access_level": "Undocumented",
             "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyTemplate": {
+        "GetPolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdentitySources": {
+        "IsAuthorized": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "IsAuthorized",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "CreateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
             "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "ListPolicyStores": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdentitySource": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "CreateIdentitySource",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "ListPolicyTemplates": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "ListPolicyTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
             "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorized": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "IsAuthorized",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateIdentitySource": {
             "access_level": "Undocumented",
             "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyStore": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "voiceid": {
@@ -168514,353 +168514,353 @@
             "orphan": false,
             "resources": [
                 "network"
             ]
         }
     },
     "wisdom": {
-        "SearchContent": {
-            "access_level": "Undocumented",
-            "action": "SearchContent",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "GetRecommendations": {
+        "ListQuickResponses": {
             "access_level": "Undocumented",
-            "action": "GetRecommendations",
+            "action": "ListQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveKnowledgeBaseTemplateUri": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "RemoveKnowledgeBaseTemplateUri",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteContent": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistantAssociation": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "GetAssistantAssociation",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "ListContents": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "ListContents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "CreateAssistant": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "CreateAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyRecommendationsReceived": {
+        "ListAssistants": {
             "access_level": "Undocumented",
-            "action": "NotifyRecommendationsReceived",
+            "action": "ListAssistants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteContent": {
+        "DeleteQuickResponse": {
             "access_level": "Undocumented",
-            "action": "DeleteContent",
+            "action": "DeleteQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchQuickResponses": {
+        "DeleteAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "SearchQuickResponses",
+            "action": "DeleteAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContent": {
+        "GetRecommendations": {
             "access_level": "Undocumented",
-            "action": "GetContent",
+            "action": "GetRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateContent": {
+        "CreateAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateContent",
+            "action": "CreateAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKnowledgeBase": {
+        "GetAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "GetAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQuickResponse": {
+        "QueryAssistant": {
             "access_level": "Undocumented",
-            "action": "GetQuickResponse",
+            "action": "QueryAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListContents": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListContents",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportJobs": {
+        "UpdateKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "ListImportJobs",
+            "action": "UpdateKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistantAssociation": {
+        "StartContentUpload": {
             "access_level": "Undocumented",
-            "action": "CreateAssistantAssociation",
+            "action": "StartContentUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQuickResponse": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "UpdateQuickResponse",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistant": {
+        "SearchContent": {
             "access_level": "Undocumented",
-            "action": "CreateAssistant",
+            "action": "SearchContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateContent": {
             "access_level": "Undocumented",
             "action": "UpdateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "GetContent": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "GetContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImportJob": {
+        "UpdateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "DeleteImportJob",
+            "action": "UpdateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetContentSummary": {
             "access_level": "Undocumented",
             "action": "GetContentSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistant": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistant",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSessions": {
+        "CreateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "SearchSessions",
+            "action": "CreateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistantAssociation": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistantAssociation",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQuickResponse": {
+        "DeleteAssistant": {
             "access_level": "Undocumented",
-            "action": "CreateQuickResponse",
+            "action": "DeleteAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQuickResponse": {
+        "GetAssistant": {
             "access_level": "Undocumented",
-            "action": "DeleteQuickResponse",
+            "action": "GetAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "StartImportJob": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "StartImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuickResponses": {
+        "NotifyRecommendationsReceived": {
             "access_level": "Undocumented",
-            "action": "ListQuickResponses",
+            "action": "NotifyRecommendationsReceived",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "QueryAssistant": {
+        "SearchQuickResponses": {
             "access_level": "Undocumented",
-            "action": "QueryAssistant",
+            "action": "SearchQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFeedback": {
+        "CreateContent": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "CreateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetImportJob": {
             "access_level": "Undocumented",
             "action": "GetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "ListImportJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "ListImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBaseTemplateUri": {
+        "ListAssistantAssociations": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBaseTemplateUri",
+            "action": "ListAssistantAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistantAssociations": {
+        "SearchSessions": {
             "access_level": "Undocumented",
-            "action": "ListAssistantAssociations",
+            "action": "SearchSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistants": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListAssistants",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistant": {
+        "RemoveKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "GetAssistant",
+            "action": "RemoveKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContentUpload": {
+        "DeleteImportJob": {
             "access_level": "Undocumented",
-            "action": "StartContentUpload",
+            "action": "DeleteImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportJob": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "StartImportJob",
+            "action": "GetKnowledgeBase",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetQuickResponse": {
+            "access_level": "Undocumented",
+            "action": "GetQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "workdocs": {
```

### Comparing `iam_actions-1.2.20240428/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240429/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240429/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/generate/generate.py` & `iam_actions-1.2.20240429/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240429/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240429/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/generate/services.py` & `iam_actions-1.2.20240429/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/policies.json` & `iam_actions-1.2.20240429/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240429/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/iam_actions/services.json` & `iam_actions-1.2.20240429/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240428/pyproject.toml` & `iam_actions-1.2.20240429/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240428"
+version = "1.2.20240429"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240428/setup.py` & `iam_actions-1.2.20240429/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240428',
+    'version': '1.2.20240429',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240428/PKG-INFO` & `iam_actions-1.2.20240429/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240428
+Version: 1.2.20240429
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

