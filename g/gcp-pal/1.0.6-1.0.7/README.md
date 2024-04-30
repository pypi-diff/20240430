# Comparing `tmp/gcp_pal-1.0.6.tar.gz` & `tmp/gcp_pal-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-1.0.6.tar", max compression
+gzip compressed data, was "gcp_pal-1.0.7.tar", max compression
```

## Comparing `gcp_pal-1.0.6.tar` & `gcp_pal-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    25269 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/README.md
--rw-r--r--   0        0        0      810 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31402 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13855 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-29 08:56:51.366821 gcp_pal-1.0.6/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    12490 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/firestore.py
--rw-r--r--   0        0        0     3170 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/project.py
--rw-r--r--   0        0        0     1674 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6975 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17133 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       82 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0      935 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/utils/lazy_loader.py
--rw-r--r--   0        0        0    11431 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0     1017 2024-04-29 08:56:51.370821 gcp_pal-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    25718 1970-01-01 00:00:00.000000 gcp_pal-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    28062 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/README.md
+-rw-r--r--   0        0        0      865 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31457 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13920 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0     1094 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    24859 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/dataplex.py
+-rw-r--r--   0        0        0    12490 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     3170 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/project.py
+-rw-r--r--   0        0        0     1674 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6975 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17224 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    11431 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0     1051 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    28511 1970-01-01 00:00:00.000000 gcp_pal-1.0.7/PKG-INFO
```

### Comparing `gcp_pal-1.0.6/README.md` & `gcp_pal-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,52 @@
 [x] Logging Module
 [x] Secret Manager Module
 [x] Cloud Scheduler Module
 [x] Add examples
 [x] Publish to PyPI
 [x] Tests
 [x] Project Module
+[x] Dataplex Module
 ...
 -->
 
 # GCP Pal Library
 
 The `gcp-pal` library provides a set of utilities for interacting with Google Cloud Platform (GCP) services, streamlining the process of implementing GCP functionalities within your Python applications.
 
 The utilities are designed to work with the `google-cloud` Python libraries, providing a more user-friendly and intuitive interface for common tasks.
 
-Source code: **https://github.com/VitaminB16/gcp-pal**
-PyPI: **https://pypi.org/project/gcp-pal/**
+- Source code: **https://github.com/VitaminB16/gcp-pal**
+- PyPI: **https://pypi.org/project/gcp-pal/**
+
+---
+
+## Table of Contents
+
+| Section Link | Module Class |
+|--------------|-------------|
+| [Installation](#installation) |  |
+| [Configuration](#configuration) |  |
+| [Firestore Module](#firestore-module) | `gcp_pal.Firestore` |
+| [PubSub Module](#pubsub-module) | `gcp_pal.PubSub` |
+| [Request Module](#request-module) | `gcp_pal.Request` |
+| [BigQuery Module](#bigquery-module) | `gcp_pal.BigQuery` |
+| [Storage Module](#storage-module) | `gcp_pal.Storage` |
+| [Parquet Module](#parquet-module) | `gcp_pal.Parquet` |
+| [Schema Module](#schema-module) | `gcp_pal.Schema` |
+| [Cloud Functions Module](#cloud-functions-module) | `gcp_pal.CloudFunctions` |
+| [Docker Module](#docker-module) | `gcp_pal.Docker` |
+| [Cloud Run Module](#cloud-run-module) | `gcp_pal.CloudRun` |
+| [Logging Module](#logging-module) | `gcp_pal.Logging` |
+| [Secret Manager Module](#secret-manager-module) | `gcp_pal.SecretManager` |
+| [Cloud Scheduler Module](#cloud-scheduler-module) | `gcp_pal.CloudScheduler` |
+| [Project Module](#project-module) | `gcp_pal.Project` |
+| [Dataplex Module](#dataplex-module) | `gcp_pal.Dataplex` |
+
+
 
 ---
 
 ## Installation
 
 The package is available on PyPI as `gcp-pal`. To install with `pip`:
 
@@ -1023,8 +1050,78 @@
 
 To obtain the project number use the `number` method:
 
 ```python
 project_number = Project("project-name").number()
 print(project_number)
 # Output: "1234567890"
-```
+```
+
+
+---
+
+## Dataplex Module
+
+The Dataplex module in the `gcp-pal` library allows you to interact with Dataplex services.
+
+### Initializing Dataplex
+
+Import the Dataplex class from the `gcp_pal` module:
+
+```python
+from gcp_pal import Dataplex
+```
+
+### Listing Dataplex objects
+
+The Dataplex module supports listing all lakes, zones, and assets within a Dataplex instance:
+
+```python
+lakes = Dataplex().ls()
+print(lakes)
+# Output: ['lake1', 'lake2']
+zones = Dataplex("lake1").ls()
+print(zones)
+# Output: ['zone1', 'zone2']
+assets = Dataplex("lake1/zone1").ls()
+print(assets)
+# Output: ['asset1', 'asset2']
+```
+
+### Creating Dataplex objects
+
+To create a lake, zone, or asset within a Dataplex instance, use the `create_lake`, `create_zone`, and `create_asset` methods.
+
+To create a lake:
+
+```python
+Dataplex("lake1").create_lake()
+# Output: Lake "lake1" created
+```
+
+To create a zone (zone type and location type are required):
+
+```python
+Dataplex("lake1/zone1").create_zone(zone_type="raw", location_type="single-region")
+# Output: Zone "zone1" created in Lake "lake1"
+```
+
+To create an asset (asset source and asset type are required):
+
+```python
+Dataplex("lake1/zone1").create_asset(asset_source="dataset_name", asset_type="bigquery")
+# Output: Asset "asset1" created in Zone "zone1" of Lake "lake1"
+```
+
+### Deleting Dataplex objects
+
+Deleting objects can be done using a single `delete` method:
+
+```python
+Dataplex("lake1/zone1/asset1").delete()
+# Output: Asset "asset1" deleted
+Dataplax("lake1/zone1").delete()
+# Output: Zone "zone1" and all its assets deleted
+Dataplex("lake1").delete()
+# Output: Lake "lake1" and all its zones and assets deleted
+```
+
```

### Comparing `gcp_pal-1.0.6/gcp_pal/__init__.py` & `gcp_pal-1.0.7/gcp_pal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 PubSub = LazyLoader("gcp_pal.pubsub", "PubSub")
 Logging = LazyLoader("gcp_pal.pylogging", "Logging")
 Request = LazyLoader("gcp_pal.request", "Request")
 Schema = LazyLoader("gcp_pal.schema", "Schema")
 Storage = LazyLoader("gcp_pal.storage", "Storage")
 Parquet = LazyLoader("gcp_pal.storage", "Parquet")
 SecretManager = LazyLoader("gcp_pal.secretmanager", "SecretManager")
-Project = LazyLoader("gcp_pal.project", "Project")
+Project = LazyLoader("gcp_pal.project", "Project")
+Dataplex = LazyLoader("gcp_pal.dataplex", "Dataplex")
```

### Comparing `gcp_pal-1.0.6/gcp_pal/bigquery.py` & `gcp_pal-1.0.7/gcp_pal/bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,19 +173,19 @@
         if self.project and self.dataset:
             self.dataset_id = f"{self.project}.{self.dataset}"
 
         if not self.project:
             raise ValueError("Project ID not specified.")
         if not self.dataset and self.table:
             raise ValueError("Table name specified without dataset.")
-        if self.project in BigQuery._clients:
-            self.client = BigQuery._clients[self.project]
+        if self.location in BigQuery._clients.get(self.project, {}):
+            self.client = BigQuery._clients[self.project][self.location]
         else:
             self.client = bigquery.Client(project=self.project, location=self.location)
-            BigQuery._clients[self.project] = self.client
+            BigQuery._clients[self.project] = {self.location: self.client}
 
     def __repr__(self):
         return f"BigQuery({self.table_id})"
 
     def query(self, sql, job_config=None, schema=None, to_dataframe=False, params=None):
         """
         Executes a query against BigQuery.
```

### Comparing `gcp_pal-1.0.6/gcp_pal/cloudfunctions.py` & `gcp_pal-1.0.7/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/cloudrun.py` & `gcp_pal-1.0.7/gcp_pal/cloudrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,19 +38,22 @@
             name = name.split("/")[-1]
         self.name = name
         self.full_name = f"{self.parent}/{self.type}s/{self.name}"
         self.image_url = None
 
         if self.project in CloudRun._client:
             self.client = CloudRun._client[self.project]
-            self.jobs_client = CloudRun._jobs_client[self.project]
         else:
             self.client = run_v2.ServicesClient()
-            self.jobs_client = run_v2.JobsClient()
             CloudRun._client[self.project] = self.client
+
+        if self.project in CloudRun._jobs_client:
+            self.jobs_client = CloudRun._jobs_client[self.project]
+        else:
+            self.jobs_client = run_v2.JobsClient()
             CloudRun._jobs_client[self.project] = self.jobs_client
 
     def ls_jobs(self, active_only=False, full_id=False):
         """
         List all jobs in the project.
         """
         jobs = self.jobs_client.list_jobs(parent=self.parent)
```

### Comparing `gcp_pal-1.0.6/gcp_pal/cloudscheduler.py` & `gcp_pal-1.0.7/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/config/vars.py` & `gcp_pal-1.0.7/gcp_pal/config/vars.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 PYPI_NAMES = {
+    "gcsfs": "gcsfs",
     "google.auth": "google-auth",
     "google.oauth2": "google-auth-oauthlib",
     "google.cloud.core": "google-cloud-core",
+    "google.cloud.run_v1": "google-cloud-run",
+    "google.cloud.run_v2": "google-cloud-run",
     "google.cloud.storage": "google-cloud-storage",
     "google.cloud.logging": "google-cloud-logging",
     "google.cloud.pubsub_v1": "google-cloud-pubsub",
     "google.cloud.bigquery": "google-cloud-bigquery",
     "google.cloud.firestore": "google-cloud-firestore",
+    "google.cloud.dataplex_v1": "google-cloud-dataplex",
     "google.cloud.functions_v1": "google-cloud-functions",
     "google.cloud.functions_v2": "google-cloud-functions",
     "google.cloud.scheduler_v1": "google-cloud-scheduler",
     "google.cloud.secretmanager": "google-cloud-secret-manager",
     "google.cloud.resource_manager": "google-cloud-resource-manager",
     "google.cloud.resourcemanager_v3": "google-cloud-resource-manager",
-    "google.cloud.run_v1": "google-cloud-run",
-    "google.cloud.run_v2": "google-cloud-run",
-    "gcsfs": "gcsfs",
     "pyarrow": "pyarrow",
     "pandas": "pandas",
     "pandas_gbq": "pandas-gbq",
     "docker": "docker",
     "yaml": "pyyaml",
 }
```

### Comparing `gcp_pal-1.0.6/gcp_pal/firestore.py` & `gcp_pal-1.0.7/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/project.py` & `gcp_pal-1.0.7/gcp_pal/project.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/pubsub.py` & `gcp_pal-1.0.7/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/pydocker.py` & `gcp_pal-1.0.7/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/pylogging.py` & `gcp_pal-1.0.7/gcp_pal/pylogging.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/request.py` & `gcp_pal-1.0.7/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/schema.py` & `gcp_pal-1.0.7/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/secretmanager.py` & `gcp_pal-1.0.7/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/storage/parquet.py` & `gcp_pal-1.0.7/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/storage/storage.py` & `gcp_pal-1.0.7/gcp_pal/storage/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,23 @@
         self.bucket_path = self.fs_prefix + self.bucket_name
         if self.bucket_name == "":
             self.bucket_name = None
             self.bucket_path = None
 
         self.ref_type = self._ref_type()
 
-        if self.project in Storage._clients:
-            self.fs = Storage._clients[self.project]
+        if self.location in Storage._clients.get(self.project, {}):
+            self.fs = Storage._clients[self.project][self.location]
         else:
             self.fs = gcsfs.GCSFileSystem(
                 project=self.project,
                 default_location=self.location,
                 cache_timeout=0,
             )
-            Storage._clients[self.project] = self.fs
+            Storage._clients[self.project] = {self.location: self.fs}
 
     def __repr__(self):
         """
         String representation of the class.
 
         Examples:
         - `Storage("bucket_name")` -> `Storage(gs://bucket_name)`
@@ -479,34 +479,34 @@
         path = self._suffix_path(path)
         bucket_name = path[len(self.fs_prefix) :].split("/")[0]
         path = path[len(bucket_name) + 1 :]
         bucket = Bucket(bucket_name, self.project)
         return Blob(path, bucket)
 
 
-if __name__ == "__main__":
-    import pyarrow as pa
-    import pyarrow.parquet as pq
-    import pandas as pd
-
-    success = {}
-    bucket_name = f"test_bucket_vita_1324"
-    Storage(bucket_name).create()
-
-    df = pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
-    partition_cols = ["a"]
-    file_name = f"gs://{bucket_name}/file.parquet"
-    table = pa.Table.from_pandas(df)
-    pq.write_to_dataset(
-        table, file_name, partition_cols=partition_cols, basename_template="{i}.parquet"
-    )
-    print(file_name)
-    print(Storage(file_name).isfile())
-    print(Storage(file_name).isfile("a=1"))
-    exit()
+# if __name__ == "__main__":
+#     import pyarrow as pa
+#     import pyarrow.parquet as pq
+#     import pandas as pd
+
+#     success = {}
+#     bucket_name = f"test_bucket_vita_1324"
+#     Storage(bucket_name).create()
+
+#     df = pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+#     partition_cols = ["a"]
+#     file_name = f"gs://{bucket_name}/file.parquet"
+#     table = pa.Table.from_pandas(df)
+#     pq.write_to_dataset(
+#         table, file_name, partition_cols=partition_cols, basename_template="{i}.parquet"
+#     )
+#     print(file_name)
+#     print(Storage(file_name).isfile())
+#     print(Storage(file_name).isfile("a=1"))
+#     exit()
 
 if __name__ == "__main__":
     print(Storage("bucket_name").bucket_name == "bucket_name")
     print(Storage("gs://bucket_name").bucket_name == "bucket_name")
     print(Storage("bucket_name/file").bucket_name == "bucket_name")
     print(Storage("gs://bucket_name/file").bucket_name == "bucket_name")
     print(Storage("gs://bucket_name").path == "gs://bucket_name")
```

### Comparing `gcp_pal-1.0.6/gcp_pal/utils/lazy_loader.py` & `gcp_pal-1.0.7/gcp_pal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/gcp_pal/utils/utils.py` & `gcp_pal-1.0.7/gcp_pal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.6/pyproject.toml` & `gcp_pal-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "1.0.6"
+version = "1.0.7"
 description = "Set of utilities for interacting with Google Cloud Platform"
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
@@ -30,11 +30,12 @@
 docker = "^7.0.0"
 google-cloud-run = "^0.10.5"
 pyyaml = "^6.0.1"
 google-cloud-secret-manager = "^2.19.0"
 google-cloud-scheduler = "^2.13.3"
 google-cloud-logging = "^3.10.0"
 google-cloud-resource-manager = "^1.12.3"
+google-cloud-dataplex = "^1.13.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gcp_pal-1.0.6/PKG-INFO` & `gcp_pal-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 1.0.6
+Version: 1.0.7
 Summary: Set of utilities for interacting with Google Cloud Platform
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,25 +26,52 @@
 [x] Logging Module
 [x] Secret Manager Module
 [x] Cloud Scheduler Module
 [x] Add examples
 [x] Publish to PyPI
 [x] Tests
 [x] Project Module
+[x] Dataplex Module
 ...
 -->
 
 # GCP Pal Library
 
 The `gcp-pal` library provides a set of utilities for interacting with Google Cloud Platform (GCP) services, streamlining the process of implementing GCP functionalities within your Python applications.
 
 The utilities are designed to work with the `google-cloud` Python libraries, providing a more user-friendly and intuitive interface for common tasks.
 
-Source code: **https://github.com/VitaminB16/gcp-pal**
-PyPI: **https://pypi.org/project/gcp-pal/**
+- Source code: **https://github.com/VitaminB16/gcp-pal**
+- PyPI: **https://pypi.org/project/gcp-pal/**
+
+---
+
+## Table of Contents
+
+| Section Link | Module Class |
+|--------------|-------------|
+| [Installation](#installation) |  |
+| [Configuration](#configuration) |  |
+| [Firestore Module](#firestore-module) | `gcp_pal.Firestore` |
+| [PubSub Module](#pubsub-module) | `gcp_pal.PubSub` |
+| [Request Module](#request-module) | `gcp_pal.Request` |
+| [BigQuery Module](#bigquery-module) | `gcp_pal.BigQuery` |
+| [Storage Module](#storage-module) | `gcp_pal.Storage` |
+| [Parquet Module](#parquet-module) | `gcp_pal.Parquet` |
+| [Schema Module](#schema-module) | `gcp_pal.Schema` |
+| [Cloud Functions Module](#cloud-functions-module) | `gcp_pal.CloudFunctions` |
+| [Docker Module](#docker-module) | `gcp_pal.Docker` |
+| [Cloud Run Module](#cloud-run-module) | `gcp_pal.CloudRun` |
+| [Logging Module](#logging-module) | `gcp_pal.Logging` |
+| [Secret Manager Module](#secret-manager-module) | `gcp_pal.SecretManager` |
+| [Cloud Scheduler Module](#cloud-scheduler-module) | `gcp_pal.CloudScheduler` |
+| [Project Module](#project-module) | `gcp_pal.Project` |
+| [Dataplex Module](#dataplex-module) | `gcp_pal.Dataplex` |
+
+
 
 ---
 
 ## Installation
 
 The package is available on PyPI as `gcp-pal`. To install with `pip`:
 
@@ -1037,7 +1064,78 @@
 To obtain the project number use the `number` method:
 
 ```python
 project_number = Project("project-name").number()
 print(project_number)
 # Output: "1234567890"
 ```
+
+
+---
+
+## Dataplex Module
+
+The Dataplex module in the `gcp-pal` library allows you to interact with Dataplex services.
+
+### Initializing Dataplex
+
+Import the Dataplex class from the `gcp_pal` module:
+
+```python
+from gcp_pal import Dataplex
+```
+
+### Listing Dataplex objects
+
+The Dataplex module supports listing all lakes, zones, and assets within a Dataplex instance:
+
+```python
+lakes = Dataplex().ls()
+print(lakes)
+# Output: ['lake1', 'lake2']
+zones = Dataplex("lake1").ls()
+print(zones)
+# Output: ['zone1', 'zone2']
+assets = Dataplex("lake1/zone1").ls()
+print(assets)
+# Output: ['asset1', 'asset2']
+```
+
+### Creating Dataplex objects
+
+To create a lake, zone, or asset within a Dataplex instance, use the `create_lake`, `create_zone`, and `create_asset` methods.
+
+To create a lake:
+
+```python
+Dataplex("lake1").create_lake()
+# Output: Lake "lake1" created
+```
+
+To create a zone (zone type and location type are required):
+
+```python
+Dataplex("lake1/zone1").create_zone(zone_type="raw", location_type="single-region")
+# Output: Zone "zone1" created in Lake "lake1"
+```
+
+To create an asset (asset source and asset type are required):
+
+```python
+Dataplex("lake1/zone1").create_asset(asset_source="dataset_name", asset_type="bigquery")
+# Output: Asset "asset1" created in Zone "zone1" of Lake "lake1"
+```
+
+### Deleting Dataplex objects
+
+Deleting objects can be done using a single `delete` method:
+
+```python
+Dataplex("lake1/zone1/asset1").delete()
+# Output: Asset "asset1" deleted
+Dataplax("lake1/zone1").delete()
+# Output: Zone "zone1" and all its assets deleted
+Dataplex("lake1").delete()
+# Output: Lake "lake1" and all its zones and assets deleted
+```
+
+
```

