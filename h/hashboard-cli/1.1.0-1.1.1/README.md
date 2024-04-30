# Comparing `tmp/hashboard_cli-1.1.0.tar.gz` & `tmp/hashboard_cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashboard_cli-1.1.0.tar", last modified: Thu Apr 25 19:09:29 2024, max compression
+gzip compressed data, was "hashboard_cli-1.1.1.tar", last modified: Tue Apr 30 15:42:37 2024, max compression
```

## Comparing `hashboard_cli-1.1.0.tar` & `hashboard_cli-1.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.845770 hashboard_cli-1.1.0/
--rw-r--r--   0 elagulsen   (501) staff       (20)    11357 2023-08-14 18:27:21.000000 hashboard_cli-1.1.0/LICENSE
--rw-r--r--   0 elagulsen   (501) staff       (20)      924 2024-04-25 19:09:29.845704 hashboard_cli-1.1.0/PKG-INFO
--rw-r--r--   0 elagulsen   (501) staff       (20)      141 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/README.md
--rw-r--r--   0 elagulsen   (501) staff       (20)      104 2023-08-15 19:32:06.000000 hashboard_cli-1.1.0/pyproject.toml
--rw-r--r--   0 elagulsen   (501) staff       (20)      878 2024-04-25 19:09:29.846019 hashboard_cli-1.1.0/setup.cfg
--rw-r--r--   0 elagulsen   (501) staff       (20)       38 2023-08-14 18:27:21.000000 hashboard_cli-1.1.0/setup.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.838716 hashboard_cli-1.1.0/src/
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.841271 hashboard_cli-1.1.0/src/hashboard/
--rw-r--r--   0 elagulsen   (501) staff       (20)       18 2024-04-25 19:09:12.000000 hashboard_cli-1.1.0/src/hashboard/__init__.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.841518 hashboard_cli-1.1.0/src/hashboard/api/
--rw-r--r--   0 elagulsen   (501) staff       (20)    14949 2024-04-25 19:09:12.000000 hashboard_cli-1.1.0/src/hashboard/api/__init__.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.842143 hashboard_cli-1.1.0/src/hashboard/api/access_keys/
--rw-r--r--   0 elagulsen   (501) staff       (20)        0 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/api/access_keys/__init__.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     4227 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/api/access_keys/browser_auth.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     4409 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/api/access_keys/existing_user.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     2143 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/api/access_keys/utils.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.842538 hashboard_cli-1.1.0/src/hashboard/api/analytics/
--rw-r--r--   0 elagulsen   (501) staff       (20)      900 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/api/analytics/__init__.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     4003 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/api/analytics/cli_with_tracking.py
--rw-r--r--   0 elagulsen   (501) staff       (20)       20 2024-04-12 14:43:11.000000 hashboard_cli-1.1.0/src/hashboard/api/analytics/events.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.843049 hashboard_cli-1.1.0/src/hashboard/api/datasource/
--rw-r--r--   0 elagulsen   (501) staff       (20)        0 2024-04-19 17:47:42.000000 hashboard_cli-1.1.0/src/hashboard/api/datasource/__init__.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     9994 2024-04-25 19:09:12.000000 hashboard_cli-1.1.0/src/hashboard/api/datasource/datasource_cli.py
--rw-r--r--   0 elagulsen   (501) staff       (20)    10025 2024-04-25 19:09:12.000000 hashboard_cli-1.1.0/src/hashboard/api/datasource/utils.py
--rw-r--r--   0 elagulsen   (501) staff       (20)    38873 2024-04-25 15:48:11.000000 hashboard_cli-1.1.0/src/hashboard/cli.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      346 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/constants.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     1744 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/credentials.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     3843 2024-04-16 15:20:55.000000 hashboard_cli-1.1.0/src/hashboard/filesystem.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      597 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/session.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.843985 hashboard_cli-1.1.0/src/hashboard/utils/
--rw-r--r--   0 elagulsen   (501) staff       (20)        0 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/__init__.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      665 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/cli.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     1977 2024-04-16 15:20:55.000000 hashboard_cli-1.1.0/src/hashboard/utils/config.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      230 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/env.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     2922 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/utils/grn.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      941 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/input_validation.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     1468 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/resource.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.845394 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/
--rw-r--r--   0 elagulsen   (501) staff       (20)      924 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/PKG-INFO
--rw-r--r--   0 elagulsen   (501) staff       (20)     1224 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 elagulsen   (501) staff       (20)        1 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 elagulsen   (501) staff       (20)       42 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/entry_points.txt
--rw-r--r--   0 elagulsen   (501) staff       (20)      138 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/requires.txt
--rw-r--r--   0 elagulsen   (501) staff       (20)       10 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/top_level.txt
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.845217 hashboard_cli-1.1.0/tests/
--rw-r--r--   0 elagulsen   (501) staff       (20)      310 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/tests/test_cli.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     1534 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/tests/test_credentials.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     3890 2024-04-16 15:20:55.000000 hashboard_cli-1.1.0/tests/test_filesystem.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      668 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/tests/test_hashboard_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.996304 hashboard_cli-1.1.1/
+-rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 hashboard_cli-1.1.1/LICENSE
+-rw-r--r--   0 anixon     (501) staff       (20)      924 2024-04-30 15:42:37.996247 hashboard_cli-1.1.1/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      141 2023-09-29 18:00:46.000000 hashboard_cli-1.1.1/README.md
+-rw-r--r--   0 anixon     (501) staff       (20)      104 2023-08-30 15:47:31.000000 hashboard_cli-1.1.1/pyproject.toml
+-rw-r--r--   0 anixon     (501) staff       (20)      878 2024-04-30 15:42:37.996575 hashboard_cli-1.1.1/setup.cfg
+-rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 hashboard_cli-1.1.1/setup.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.988758 hashboard_cli-1.1.1/src/
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.991011 hashboard_cli-1.1.1/src/hashboard/
+-rw-r--r--   0 anixon     (501) staff       (20)       18 2024-04-30 15:41:53.000000 hashboard_cli-1.1.1/src/hashboard/__init__.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.991280 hashboard_cli-1.1.1/src/hashboard/api/
+-rw-r--r--   0 anixon     (501) staff       (20)    15394 2024-04-30 14:54:57.000000 hashboard_cli-1.1.1/src/hashboard/api/__init__.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.992023 hashboard_cli-1.1.1/src/hashboard/api/access_keys/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/api/access_keys/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4227 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/api/access_keys/browser_auth.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4409 2024-03-18 20:02:56.000000 hashboard_cli-1.1.1/src/hashboard/api/access_keys/existing_user.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2143 2024-03-18 20:02:56.000000 hashboard_cli-1.1.1/src/hashboard/api/access_keys/utils.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.992712 hashboard_cli-1.1.1/src/hashboard/api/analytics/
+-rw-r--r--   0 anixon     (501) staff       (20)      900 2023-09-29 18:00:46.000000 hashboard_cli-1.1.1/src/hashboard/api/analytics/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4003 2023-09-29 18:00:46.000000 hashboard_cli-1.1.1/src/hashboard/api/analytics/cli_with_tracking.py
+-rw-r--r--   0 anixon     (501) staff       (20)       20 2024-04-16 20:21:42.000000 hashboard_cli-1.1.1/src/hashboard/api/analytics/events.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.993247 hashboard_cli-1.1.1/src/hashboard/api/datasource/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2024-04-22 20:51:24.000000 hashboard_cli-1.1.1/src/hashboard/api/datasource/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)     9994 2024-04-26 20:17:46.000000 hashboard_cli-1.1.1/src/hashboard/api/datasource/datasource_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)    10025 2024-04-26 20:17:46.000000 hashboard_cli-1.1.1/src/hashboard/api/datasource/utils.py
+-rw-r--r--   0 anixon     (501) staff       (20)    39341 2024-04-30 14:54:57.000000 hashboard_cli-1.1.1/src/hashboard/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)      346 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/constants.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1744 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     3843 2024-04-16 20:21:42.000000 hashboard_cli-1.1.1/src/hashboard/filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      597 2023-09-29 18:00:46.000000 hashboard_cli-1.1.1/src/hashboard/session.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.994389 hashboard_cli-1.1.1/src/hashboard/utils/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)      665 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1977 2024-04-16 20:21:42.000000 hashboard_cli-1.1.1/src/hashboard/utils/config.py
+-rw-r--r--   0 anixon     (501) staff       (20)      230 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/env.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2922 2023-11-06 18:51:09.000000 hashboard_cli-1.1.1/src/hashboard/utils/grn.py
+-rw-r--r--   0 anixon     (501) staff       (20)      941 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/input_validation.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1468 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/resource.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.995855 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/
+-rw-r--r--   0 anixon     (501) staff       (20)      924 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)     1224 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        1 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       42 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anixon     (501) staff       (20)      138 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/requires.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       10 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.995684 hashboard_cli-1.1.1/tests/
+-rw-r--r--   0 anixon     (501) staff       (20)      310 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/tests/test_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1534 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/tests/test_credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     3890 2024-04-16 20:21:42.000000 hashboard_cli-1.1.1/tests/test_filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      668 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/tests/test_hashboard_api.py
```

### Comparing `hashboard_cli-1.1.0/LICENSE` & `hashboard_cli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/PKG-INFO` & `hashboard_cli-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashboard_cli-1.1.0/setup.cfg` & `hashboard_cli-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/api/__init__.py` & `hashboard_cli-1.1.1/src/hashboard/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,17 @@
         session, project_id, build_spec, deploy, allow_dangerous_empty_build
     )
 
 
 def get_datasources(s: Session, project_id: str) -> list:
     """Queries and formats datasources"""
     query = _get_data_connections(s, project_id)
-    data_sources = [[d['name'], d['subType'], d['id']] for d in query["data"]["dataConnections"]]
+    data_sources = [
+        [d["name"], d["subType"], d["id"]] for d in query["data"]["dataConnections"]
+    ]
     return data_sources
 
 
 def clear_model_cache(s: Session, model_id: str) -> str:
     """Clears the cache for the specified model"""
     return _graphql_query(
         s,
@@ -144,26 +146,39 @@
     )["data"]["pullResource"]
     res["configs"] = [
         Resource.from_dict(json.loads(string)) for string in res["configs"]
     ]
     return res
 
 
+def build_fetch_timeout_error(build_id):
+    def error_func(status_code):
+        if status_code == 401:
+            raise ClickException(
+                f"The Hashboard CLI client has timed out but your request is still running on our server. Please check the build page to view build progress: {build_details_uri(build_id)}"
+            )
+        elif status_code != 200:
+            raise ClickException("Unexpected error received from the Hashboard server.")
+
+    return error_func
+
+
 def fetch_build_status(s: Session, build_id):
     return _graphql_query(
         s,
         """
         query fetchBuild($buildId: String!){
             fetchBuild (buildId: $buildId){
                 id,
                 status, 
             }
         }
         """,
         {"buildId": build_id},
+        custom_status_response_func=build_fetch_timeout_error(build_id),
     )
 
 
 def fetch_build(s: Session, build_id):
     return _graphql_query(
         s,
         """
@@ -179,14 +194,15 @@
                 },
                 warnings,
                 errors
             }
         }
         """,
         {"buildId": build_id},
+        custom_status_response_func=build_fetch_timeout_error(build_id),
     )
 
 
 def apply_preview_build(s: Session, preview_build_id):
     return _graphql_query(
         s,
         """
@@ -260,15 +276,15 @@
             }
         }
         """,
         {
             "projectId": project_id,
             "buildSpec": build_spec,
             "deploy": deploy,
-            "allowEmptyBuild": allow_dangerous_empty_build
+            "allowEmptyBuild": allow_dangerous_empty_build,
         },
     )
 
 
 def _get_data_connections(session: Session, project_id: str) -> dict:
     query = _graphql_query(
         session,
@@ -297,87 +313,88 @@
             }
         }
         """,
         {"datasourceId": datasource_id},
     )
     return query
 
+
 def create_data_source(session: Session, datasource: dict) -> dict:
     # Assumes that error handling occurs a level up
     return _graphql_query(
         session,
         """
         mutation AddDatasource($datasource: DatasourceInput!) {
           addDatasource(datasource: $datasource) {
             id
           }
         }
         """,
         {"datasource": datasource},
     )["data"]["addDatasource"]["id"]
 
+
 def update_data_source(session: Session, datasource: dict) -> dict:
     # Assumes that error handling occurs a level up
     return _graphql_query(
         session,
         """
         mutation UpdateDatasource($datasource: DatasourceInput!) {
           updateDatasource(datasource: $datasource) {
             id
           }
         }
         """,
         {"datasource": datasource},
     )["data"]["updateDatasource"]["id"]
 
+
 def test_data_source(session: Session, datasource_name: str, project_id: str) -> bool:
     return _graphql_query(
         session,
         """
         query TestDatasourceByName($name: String!, $projectId: String!) {
             testDatasourceByName(name: $name, projectId: $projectId) 
         }
         """,
         {"name": datasource_name, "projectId": project_id},
     )["data"]["testDatasourceByName"]
 
+
 def get_tables(s: Session, datasource_id: str) -> Dict[str, Dict[str, str]]:
     """Queries and formats table from datasource"""
     query = _get_table_data(s, datasource_id)
     tables = _parse_table_data(query)
     return tables
 
 
-preview_uri = lambda build_results, query_name="createBuild": click.style(
-    f"{HASHBOARD_BASE_URI}/app/?build={build_results['data'][query_name]['id']}",
-    underline=True,
-)
-
-build_details_uri = lambda build_results, query_name="createBuild": click.style(
-    f"{HASHBOARD_BASE_URI}/app/p/builds/{build_results['data'][query_name]['id']}",
+build_details_uri = lambda id: click.style(
+    f"{HASHBOARD_BASE_URI}/app/p/builds/{id}",
     underline=True,
 )
 
-preview_model_uri = (
-    lambda model_id, build_results, query_name="modelPreviewBuildFromGleanDb": f"{HASHBOARD_BASE_URI}/app/m/{model_id}?build={build_results['data'][query_name]['id']}"
-)
 
-
-def _graphql_query(session: Session, query: str, variables: dict):
+def _graphql_query(
+    session: Session, query: str, variables: dict, custom_status_response_func=None
+):
     r = session.post(
         HASHBOARD_BASE_URI + "/graphql/",
         json={"query": query, "variables": variables},
         headers={"Glean-CLI-Version": VERSION},
     )
-    if r.status_code == 504:
-        raise ClickException(
-            f"The Hashboard CLI client has timed out but your request is still running on our server. Please check your project's build page in a few minutes to see build results: {HASHBOARD_BASE_URI}/app/p/data-ops"
-        )
-    elif r.status_code != 200:
-        raise ClickException("Unexpected error received from the Hashboard server.")
+    if custom_status_response_func:
+        custom_status_response_func(r.status_code)
+    else:
+        # This 504 status should only be encountered by legacy build commands
+        if r.status_code == 504:
+            raise ClickException(
+                f"The Hashboard CLI client has timed out but your request is still running on our server. Please check your project's build page in a few minutes to see build results: {HASHBOARD_BASE_URI}/app/p/data-ops"
+            )
+        elif r.status_code != 200:
+            raise ClickException("Unexpected error received from the Hashboard server.")
 
     results = r.json()
     graphql_exceptions = results.get("errors")
     if (
         graphql_exceptions
         and isinstance(graphql_exceptions[0], dict)
         and graphql_exceptions[0].get("message")
@@ -448,8 +465,7 @@
         HASHBOARD_BASE_URI + f"/export/{endpoint}",
         data=json.dumps(data),
         headers={"Glean-CLI-Version": VERSION, **additional_headers},
     )
     if r.status_code != 200:
         raise ClickException("Unexpected error received from the Hashboard server.")
     return r.text
-
```

### Comparing `hashboard_cli-1.1.0/src/hashboard/api/access_keys/browser_auth.py` & `hashboard_cli-1.1.1/src/hashboard/api/access_keys/browser_auth.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/api/access_keys/existing_user.py` & `hashboard_cli-1.1.1/src/hashboard/api/access_keys/existing_user.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/api/access_keys/utils.py` & `hashboard_cli-1.1.1/src/hashboard/api/access_keys/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/api/analytics/__init__.py` & `hashboard_cli-1.1.1/src/hashboard/api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/api/analytics/cli_with_tracking.py` & `hashboard_cli-1.1.1/src/hashboard/api/analytics/cli_with_tracking.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/api/datasource/datasource_cli.py` & `hashboard_cli-1.1.1/src/hashboard/api/datasource/datasource_cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/api/datasource/utils.py` & `hashboard_cli-1.1.1/src/hashboard/api/datasource/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/cli.py` & `hashboard_cli-1.1.1/src/hashboard/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,28 +408,43 @@
         deploy_completed = _poll_for_build_status(deploy_id)
         _echo_async_build_results(deploy_completed)
 
     click.echo("")
     click.echo(click.style("✅ Deploy complete.", fg="bright_green"))
 
 
+def spinning_cursor():
+    while True:
+        for cursor in "|/-\\":
+            yield cursor
+
+
 def _poll_for_build_status(build_id):
     s = get_current_session()
-    click.echo("Compiling resources ", nl=False)
-    for i in range(300):  # arbitrary upper limit
-        click.echo(".", nl=False)
-        # TODO Add error handling here
-        partial_build = fetch_build_status(s, build_id)
-        if ("errors" in partial_build and partial_build["errors"]) or partial_build[
-            "data"
-        ]["fetchBuild"]["status"] == "completed":
-            click.echo()
-            build = fetch_build(s, build_id)
-            return build
-        time.sleep(10)
+
+    spinner = spinning_cursor()
+    is_running = False
+    for i in range(3000):  # arbitrary upper limit
+        click.echo("\r" + next(spinner), nl=False)
+        if not i % 10:
+            click.echo("\b ", nl=False)
+            sys.stdout.flush()
+            partial_build = fetch_build_status(s, build_id)
+            if ("errors" in partial_build and partial_build["errors"]) or partial_build[
+                "data"
+            ]["fetchBuild"]["status"] == "completed":
+                build = fetch_build(s, build_id)
+                return build
+            elif (
+                partial_build["data"]["fetchBuild"]["status"] == "running"
+                and not is_running
+            ):
+                click.echo("\bBuilding resources... ")
+                is_running = True
+        time.sleep(0.5)
     click.echo("Error fetching build, max attempt.", fg="red")
     click.get_current_context().exit(1)
 
 
 @cli.command(cls=CommandWithTracking)
 @click.argument("database")
 @click.pass_context
@@ -831,21 +846,22 @@
         _echo_build_errors_and_exit(
             [
                 e["extensions"]["userMessage"]
                 for e in build_results["errors"]
                 if "extensions" in e and "userMessage" in e["extensions"]
             ]
         )
-    created_build_results = build_results["data"][query_name]
+    created_build_id = build_results["data"][query_name]
 
     click.echo(
-        click.style("📦 Build ", fg="bright_green")
-        + click.style(created_build_results, bold=True)
-        + click.style(" started running successfully.", fg="bright_green")
+        click.style("\n📦 Build ", fg="white")
+        + click.style(created_build_id, bold=True)
+        + click.style(" queued, waiting to start", fg="white")
     )
+    click.echo(f"Follow build in web app: {build_details_uri(created_build_id)}")
     click.echo("")
 
 
 def _get_empty_status_groups():
     return {
         "modelBundles": [],
         "metrics": [],
@@ -949,15 +965,15 @@
     click.echo("")
 
     if created_build_results["warnings"]:
         _echo_build_warnings(created_build_results["warnings"])
 
     _echo_build_resources(created_build_results["resources"], deploy)
     click.echo("")
-    click.echo(f"Details: {build_details_uri(build_results, query_name=query_name)}")
+    click.echo(f"Details: {build_details_uri(build_results['data'][query_name]['id'])}")
 
 
 def _echo_pull_errors_and_exit(errors: List[str]):
     click.echo("")
     click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――", fg="red")
     click.echo("❗ Errors encountered when pulling resources")
     click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――", fg="red")
```

### Comparing `hashboard_cli-1.1.0/src/hashboard/credentials.py` & `hashboard_cli-1.1.1/src/hashboard/credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/filesystem.py` & `hashboard_cli-1.1.1/src/hashboard/filesystem.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/session.py` & `hashboard_cli-1.1.1/src/hashboard/session.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/utils/cli.py` & `hashboard_cli-1.1.1/src/hashboard/utils/cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/utils/config.py` & `hashboard_cli-1.1.1/src/hashboard/utils/config.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/utils/grn.py` & `hashboard_cli-1.1.1/src/hashboard/utils/grn.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/utils/input_validation.py` & `hashboard_cli-1.1.1/src/hashboard/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard/utils/resource.py` & `hashboard_cli-1.1.1/src/hashboard/utils/resource.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/src/hashboard_cli.egg-info/PKG-INFO` & `hashboard_cli-1.1.1/src/hashboard_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashboard_cli-1.1.0/src/hashboard_cli.egg-info/SOURCES.txt` & `hashboard_cli-1.1.1/src/hashboard_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/tests/test_credentials.py` & `hashboard_cli-1.1.1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/tests/test_filesystem.py` & `hashboard_cli-1.1.1/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.0/tests/test_hashboard_api.py` & `hashboard_cli-1.1.1/tests/test_hashboard_api.py`

 * *Files identical despite different names*

