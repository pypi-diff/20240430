# Comparing `tmp/leap_data_management_utils-0.0.5.tar.gz` & `tmp/leap_data_management_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_data_management_utils-0.0.5.tar", last modified: Mon Apr 22 21:52:23 2024, max compression
+gzip compressed data, was "leap_data_management_utils-0.0.6.tar", last modified: Tue Apr 30 19:54:19 2024, max compression
```

## Comparing `leap_data_management_utils-0.0.5.tar` & `leap_data_management_utils-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:52:23.215291 leap_data_management_utils-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:52:23.211290 leap_data_management_utils-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:52:23.211290 leap_data_management_utils-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/.github/workflows/catalog-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-22 21:52:23.215291 leap_data_management_utils-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:52:23.211290 leap_data_management_utils-0.0.5/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/ci/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:52:23.211290 leap_data_management_utils-0.0.5/leap_data_management_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 21:52:23.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/cmip_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/cmip_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:52:23.211290 leap_data_management_utils-0.0.5/leap_data_management_utils/testing_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:52:23.215291 leap_data_management_utils-0.0.5/leap_data_management_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/tests/test_cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/leap_data_management_utils/tests/test_data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:52:23.215291 leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-22 21:52:23.000000 leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-22 21:52:23.000000 leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:52:23.000000 leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 21:52:23.000000 leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 21:52:23.000000 leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 21:52:23.000000 leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-22 21:52:12.000000 leap_data_management_utils-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 21:52:23.215291 leap_data_management_utils-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.215972 leap_data_management_utils-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.215972 leap_data_management_utils-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.github/workflows/catalog-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.215972 leap_data_management_utils-0.0.6/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/ci/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/leap_data_management_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/leap_data_management_utils/testing_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/leap_data_management_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/tests/test_cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/leap_data_management_utils/tests/test_data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 19:54:19.000000 leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-30 19:54:07.000000 leap_data_management_utils-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:54:19.219972 leap_data_management_utils-0.0.6/setup.cfg
```

### Comparing `leap_data_management_utils-0.0.5/.github/workflows/catalog-ci.yaml` & `leap_data_management_utils-0.0.6/.github/workflows/catalog-ci.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/.github/workflows/release.yaml` & `leap_data_management_utils-0.0.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/.gitignore` & `leap_data_management_utils-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/.pre-commit-config.yaml` & `leap_data_management_utils-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/LICENSE` & `leap_data_management_utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/PKG-INFO` & `leap_data_management_utils-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -19,20 +19,24 @@
 Requires-Dist: apache-beam
 Requires-Dist: cftime
 Requires-Dist: db_dtypes
 Requires-Dist: google-api-core
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: pandas
 Requires-Dist: pangeo-forge-esgf
+Requires-Dist: pangeo-forge-recipes
 Requires-Dist: pydantic-core
 Requires-Dist: pydantic>=2
 Requires-Dist: pyyaml
 Requires-Dist: ruamel.yaml
 Requires-Dist: universal-pathlib
 Requires-Dist: xarray
 Requires-Dist: zarr
 Provides-Extra: test
-Requires-Dist: pre-commit; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: dev
+Requires-Dist: leap-data-leap_data_management_utils[test]; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
 # LEAP Data Management Utils
 
 This Repo is intended to be installed via the `requirements.txt` during recipe execution in `pangeo-forge-recipes`. It currently contains beam transforms to log information into BigQuery tables. Additional shared utilities and checks that are commonly used between LEAP pangeo-forge-feedstocks can live here.
```

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils/catalog.py` & `leap_data_management_utils-0.0.6/leap_data_management_utils/catalog.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,42 @@
 import argparse
 import json
 import traceback
 
 import pydantic
 import pydantic_core
+import requests
 import upath
 import yaml
 
 
+def s3_to_https(s3_url: str) -> str:
+    # Split the URL into its components
+    s3_parts = s3_url.split('/')
+
+    # Get the bucket name from the first part of the URL
+    bucket_name = s3_parts[2]
+
+    # Join the remaining parts of the URL to form the path to the file
+    path = '/'.join(s3_parts[3:])
+
+    # Return the HTTPS URL in the desired format
+    return f'https://{bucket_name}.s3.amazonaws.com/{path}'
+
+
+def gs_to_https(gs_url: str) -> str:
+    return gs_url.replace('gs://', 'https://storage.googleapis.com/')
+
+
 class Store(pydantic.BaseModel):
     id: str = pydantic.Field(..., description='ID of the store')
     name: str = pydantic.Field(None, description='Name of the store')
     url: str = pydantic.Field(..., description='URL of the store')
     rechunking: list[dict[str, str]] | None = pydantic.Field(None, alias='ncviewjs:rechunking')
+    public: bool | None = pydantic.Field(None, description='Whether the store is public')
 
 
 class Link(pydantic.BaseModel):
     label: str = pydantic.Field(..., description='Label of the link')
     url: str = pydantic.Field(..., description='URL of the link')
 
 
@@ -114,14 +134,18 @@
     errors = []
     valid = []
     catalog = []
 
     for feedstock in feedstocks:
         try:
             feed = Feedstock.from_yaml(convert_to_raw_github_url(feedstock))
+            print('🔄 Checking stores')
+            for index, store in enumerate(feed.stores):
+                print(f'  🚦 {store.id} ({index + 1}/{len(feed.stores)})')
+                feed.stores[index].public = is_store_public(store.rechunking or store.url)
             valid.append({'feedstock': str(feedstock), 'status': 'valid'})
             catalog.append(feed)
         except Exception:
             errors.append({'feedstock': str(feedstock), 'traceback': traceback.format_exc()})
 
     valid_report = format_report('✅ Valid feedstocks:', valid)
     invalid_report = format_report('❌ Invalid feedstocks:', errors, include_traceback=True)
@@ -132,14 +156,42 @@
 
     if errors:
         raise ValidationError('Validation failed')
 
     return catalog
 
 
+def is_store_public(store) -> bool:
+    try:
+        if store.startswith('s3://'):
+            url = s3_to_https(store)
+
+        elif store.startswith('gs://'):
+            url = gs_to_https(store)
+        else:
+            url = store
+
+        url = url.strip('/')
+
+        path = f'{url}/.zmetadata'
+
+        response = requests.get(path)
+        response.raise_for_status()
+        return True
+    except requests.exceptions.HTTPError as e:
+        if e.response.status_code == 404:
+            print(f'Resource not found at {path}.')
+        else:
+            print(f'HTTP error {e.response.status_code} for {path}.')
+        return False
+    except Exception as e:
+        print(f'An error occurred while checking if store {store} is public: {str(e)}')
+        return False
+
+
 def validate(args):
     if args.single:
         # If single file path is provided, validate just this one feedstock
         try:
             _ = Feedstock.from_yaml(convert_to_raw_github_url(args.single))
             print(
                 format_report(
```

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils/cmip_catalog.py` & `leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_catalog.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils/cmip_testing.py` & `leap_data_management_utils-0.0.6/leap_data_management_utils/cmip_testing.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils/cmip_transforms.py` & `leap_data_management_utils-0.0.6/leap_data_management_utils/data_management_transforms.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,217 @@
-"""
-utils that are specific to CMIP data management
-"""
+# Note: All of this code was written by Julius Busecke and copied from this feedstock:
+# https://github.com/leap-stc/cmip6-leap-feedstock/blob/main/feedstock/recipe.py#L262
 
-import datetime
+import subprocess
 from dataclasses import dataclass
+from datetime import datetime, timezone
+from typing import Optional
 
 import apache_beam as beam
 import zarr
+from google.api_core.exceptions import NotFound
 from google.cloud import bigquery
+from ruamel.yaml import YAML
 
-from leap_data_management_utils.data_management_transforms import BQInterface
+yaml = YAML(typ='safe')
 
 
-@dataclass
-class IIDEntry:
-    """Single row/entry for an iid
-    :param iid: CMIP6 instance id
-    :param store: URL to zarr store
-    """
+def get_github_commit_url() -> Optional[str]:
+    """Get the GitHub commit URL for the current commit"""
+    # Get GitHub Server URL
+    github_server_url = 'https://github.com'
 
-    iid: str
-    store: str  # TODO: should this allow other objects?
-    retracted: bool
-    tests_passed: bool
+    # Get the repository's remote origin URL
+    try:
+        repo_origin_url = subprocess.check_output(
+            ['git', 'config', '--get', 'remote.origin.url'], text=True
+        ).strip()
 
-    # Check if the iid conforms to a schema
-    def __post_init__(self):
-        schema = 'mip_era.activity_id.institution_id.source_id.experiment_id.member_id.table_id.variable_id.grid_label.version'
-        facets = self.iid.split('.')
-        if len(facets) != len(schema.split('.')):
-            raise ValueError(f'IID does not conform to CMIP6 {schema =}. Got {self.iid =}')
-        assert self.store.startswith('gs://')
-        assert self.retracted in [True, False]
-        assert self.tests_passed in [True, False]
+        # Extract the repository path from the remote URL
+        repository_path = repo_origin_url.split('github.com/')[-1].replace('.git', '')
 
-        # TODO: Check each facet with the controlled CMIP vocabulary
+        # Get the current commit SHA
+        commit_sha = subprocess.check_output(['git', 'rev-parse', 'HEAD'], text=True).strip()
 
-        # TODO Check store validity?
+        # Construct the GitHub commit URL
+        git_url_hash = f'{github_server_url}/{repository_path}/commit/{commit_sha}'
 
+        # Output the GitHub commit URL
+        return git_url_hash
 
-@dataclass
-class IIDResult:
-    """Class to handle the results pertaining to a single IID."""
+    except subprocess.CalledProcessError as e:
+        print('Error executing Git command:', e)
+        return None
 
-    results: bigquery.table.RowIterator
-    iid: str
 
-    def __post_init__(self):
-        if self.results.total_rows > 0:
-            self.exists = True
-            self.rows = [r for r in self.results]
-            self.latest_row = self.rows[0]
-        else:
-            self.exists = False
+def get_catalog_store_urls(catalog_yaml_path: str) -> dict[str, str]:
+    with open(catalog_yaml_path) as f:
+        catalog_meta = yaml.load(f)
+    return {d['id']: d['url'] for d in catalog_meta['stores']}
 
 
-class CMIPBQInterface(BQInterface):
+@dataclass
+class BQInterface:
     """Class to read/write information from BigQuery table
     :param table_id: BigQuery table ID
     :param client: BigQuery client object
     :param result_limit: Maximum number of results to return from query
     """
 
+    table_id: str
+    client: Optional[bigquery.client.Client] = None
+    result_limit: Optional[int] = 10
+    schema: Optional[list] = None
+
     def __post_init__(self):
         # TODO how do I handle the schema? This class could be used for any table, but for
         # TODO this specific case I want to prescribe the schema
         # for now just hardcode it
         if not self.schema:
             self.schema = [
-                bigquery.SchemaField('instance_id', 'STRING', mode='REQUIRED'),
-                bigquery.SchemaField('store', 'STRING', mode='REQUIRED'),
+                bigquery.SchemaField('dataset_id', 'STRING', mode='REQUIRED'),
+                bigquery.SchemaField('dataset_url', 'STRING', mode='REQUIRED'),
                 bigquery.SchemaField('timestamp', 'TIMESTAMP', mode='REQUIRED'),
-                bigquery.SchemaField('retracted', 'BOOL', mode='REQUIRED'),
-                bigquery.SchemaField('tests_passed', 'BOOL', mode='REQUIRED'),
             ]
-        super().__post_init__()
+        if self.client is None:
+            self.client = bigquery.Client()
+
+        # check if table exists, otherwise create it
+        try:
+            self._get_table()
+        except NotFound:
+            self.create_table()
+
+    def create_table(self) -> bigquery.table.Table:
+        """Create the table if it does not exist"""
+        print(f'Creating {self.table_id =}')
+        table = bigquery.Table(self.table_id, schema=self.schema)
+        self.client.create_table(table)  # Make an API request.
+
+    def _get_table(self) -> bigquery.table.Table:
+        """Get the table object"""
+        return self.client.get_table(self.table_id)
+
+    def insert(self, fields: dict = {}):
+        timestamp = datetime.now().isoformat()
 
-    def _get_timestamp(self) -> str:
-        """Get the current timestamp"""
-        return datetime.datetime.utcnow().isoformat()
-
-    def insert_iid(self, IID_entry):
-        """Insert a row into the table for a given IID_entry object"""
-        fields = {
-            'instance_id': IID_entry.iid,
-            'store': IID_entry.store,
-            'retracted': IID_entry.retracted,
-            'tests_passed': IID_entry.tests_passed,
-            'timestamp': self._get_timestamp(),
-        }
-        self.insert(fields)
-
-    def insert_multiple_iids(self, IID_entries: list[IIDEntry]):
-        """Insert multiple rows into the table for a given list of IID_entry objects"""
-        # FIXME This repeats a bunch of code from the parent class .insert() method
-        timestamp = self._get_timestamp()
         rows_to_insert = [
-            {
-                'instance_id': IID_entry.iid,
-                'store': IID_entry.store,
-                'retracted': IID_entry.retracted,
-                'tests_passed': IID_entry.tests_passed,
-                'timestamp': timestamp,
-            }
-            for IID_entry in IID_entries
+            fields | {'timestamp': timestamp}  # timestamp is always overridden
         ]
+
         errors = self.client.insert_rows_json(self._get_table(), rows_to_insert)
         if errors:
             raise RuntimeError(f'Error inserting row: {errors}')
 
-    def _get_iid_results(self, iid: str) -> IIDResult:
-        # keep this in case I ever need the row index again...
-        # query = f"""
-        # WITH table_with_index AS (SELECT *, ROW_NUMBER() OVER ()-1 as row_index FROM `{self.table_id}`)
-        # SELECT *
-        # FROM `table_with_index`
-        # WHERE instance_id='{iid}'
-        # """
-        """Get the full result object for a given iid"""
+    def catalog_insert(self, dataset_id: str, dataset_url: str, extra_fields: dict = {}):
+        rows_to_insert = [
+            {
+                'dataset_id': dataset_id,
+                'dataset_url': dataset_url,
+            }
+            | extra_fields
+        ]
+        self.insert(rows_to_insert)
+
+    def _get_query_job(self, query: str) -> bigquery.job.query.QueryJob:
+        return self.client.query(query)
+
+    def get_all(self) -> list[bigquery.table.Row]:
+        """Get all rows in the table"""
         query = f"""
-        SELECT *
-        FROM `{self.table_id}`
-        WHERE instance_id='{iid}'
-        ORDER BY timestamp DESC
-        LIMIT {self.result_limit}
-        """
-        results = self._get_query_job(
-            query
-        ).result()  # TODO: `.result()` is waiting for the query. Should I do this here?
-        return IIDResult(results, iid)
-
-    def iid_exists(self, iid: str) -> bool:
-        """Check if iid exists in the table"""
-        return self._get_iid_results(iid).exists
-
-    def iid_list_exists(self, iids: list[str]) -> list[str]:
-        """More efficient way to check if a list of iids exists in the table
-        Passes the entire list to a single SQL query.
-        Returns a list of iids that exist in the table
-        Only supports list up to 10k elements. If you want to check more, you should
-        work in batches:
-        ```
-        iids = df['instance_id'].tolist()
-        iids_in_bq = []
-        batchsize = 10000
-        iid_batches = [iids[i : i + batchsize] for i in range(0, len(iids), batchsize)]
-        for iids_batch in tqdm(iid_batches):
-            iids_in_bq_batch = bq.iid_list_exists(iids_batch)
-            iids_in_bq.extend(iids_in_bq_batch)
-        ```
+        SELECT * FROM {self.table_id};
         """
-        assert len(iids) <= 10000
+        results = self._get_query_job(query)
+        return results.to_dataframe()
 
-        # source: https://stackoverflow.com/questions/26441928/how-do-i-check-if-multiple-values-exists-in-database
+    def get_latest(self) -> list[bigquery.table.Row]:
+        """Get the latest row for all iids in the table"""
+        # adopted from https://stackoverflow.com/a/1313293
         query = f"""
-        SELECT instance_id, store
-        FROM {self.table_id}
-        WHERE instance_id IN ({",".join([f"'{iid}'" for iid in iids])})
+        WITH ranked_iids AS (
+        SELECT i.*, ROW_NUMBER() OVER (PARTITION BY instance_id ORDER BY timestamp DESC) AS rn
+        FROM {self.table_id} AS i
+        )
+        SELECT * FROM ranked_iids WHERE rn = 1;
         """
-        results = self._get_query_job(query).result()
-        # this is a full row iterator, for now just return the iids
-        return list(set([r['instance_id'] for r in results]))
+        results = self._get_query_job(query)
+        return results.to_dataframe().drop(columns=['rn'])
 
 
 # ----------------------------------------------------------------------------------------------
 # apache Beam stages
 # ----------------------------------------------------------------------------------------------
 
 
 @dataclass
-class LogCMIPToBigQuery(beam.PTransform):
-    """
-    Logging stage for data written to zarr store
-    """
-
-    iid: str
+class RegisterDatasetToCatalog(beam.PTransform):
     table_id: str
-    retracted: bool = False
-    tests_passed: bool = False
+    dataset_id: str
 
-    def _log_to_bigquery(self, store: zarr.storage.FSStore) -> zarr.storage.FSStore:
-        bq_interface = CMIPBQInterface(table_id=self.table_id)
-        iid_entry = IIDEntry(
-            iid=self.iid,
-            store='gs://' + store.path,  # TODO: Get the full store path from the store object
-            retracted=self.retracted,
-            tests_passed=self.tests_passed,
-        )
-        bq_interface.insert_iid(iid_entry)
+    def _register_dataset_to_catalog(self, store: zarr.storage.FSStore) -> zarr.storage.FSStore:
+        bq_interface = BQInterface(table_id=self.table_id)
+        bq_interface.catalog_insert(dataset_id=self.dataset_id, dataset_url=store.path)
         return store
 
     def expand(self, pcoll: beam.PCollection) -> beam.PCollection:
-        return pcoll | beam.Map(self._log_to_bigquery)
+        return pcoll | beam.Map(self._register_dataset_to_catalog)
+
+
+@dataclass
+class Copy(beam.PTransform):
+    """Copy a store to a new location. If the target input is False, do nothing."""
+
+    target: str
+
+    def _copy(self, store: zarr.storage.FSStore) -> zarr.storage.FSStore:
+        import os
+
+        import gcsfs
+        import zarr
+
+        # We do need the gs:// prefix?
+        # TODO: Determine this dynamically from zarr.storage.FSStore
+        source = f'gs://{os.path.normpath(store.path)}/'  # FIXME more elegant. `.copytree` needs trailing slash
+        if self.target is False:
+            # dont do anything
+            return store
+        else:
+            fs = gcsfs.GCSFileSystem()  # FIXME: How can we generalize this?
+            fs.cp(source, self.target, recursive=True)
+            # return a new store with the new path that behaves exactly like the input
+            # to this stage (so we can slot this stage right before testing/logging stages)
+            return zarr.storage.FSStore(self.target)
+
+    def expand(self, pcoll: beam.PCollection) -> beam.PCollection:
+        return pcoll | 'Copying Store' >> beam.Map(self._copy)
+
+
+@dataclass
+class InjectAttrs(beam.PTransform):
+    inject_attrs: dict = None
+    add_provenance: bool = True
+
+    # add a post_init method to add the provenance attributes
+    def __post_init__(self):
+        if self.inject_attrs is None:
+            self.inject_attrs = {}
+
+        if self.add_provenance:
+            git_url_hash = get_github_commit_url()
+            timestamp = datetime.now(timezone.utc).isoformat()
+            provenance_dict = {
+                'pangeo_forge_build_git_hash': git_url_hash,
+                'pangeo_forge_build_timestamp': timestamp,
+            }
+            self.inject_attrs.update(provenance_dict)
+
+    def _update_zarr_attrs(self, store: zarr.storage.FSStore) -> zarr.storage.FSStore:
+        # TODO: Can we get a warning here if the store does not exist?
+        attrs = zarr.open(store, mode='a').attrs
+        attrs.update(self.inject_attrs)
+        # ? Should we consolidate here? We are explicitly doing that later...
+        return store
+
+    def expand(
+        self, pcoll: beam.PCollection[zarr.storage.FSStore]
+    ) -> beam.PCollection[zarr.storage.FSStore]:
+        return pcoll | 'Injecting Attributes' >> beam.Map(self._update_zarr_attrs)
```

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb` & `leap_data_management_utils-0.0.6/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils/tests/test_cmip_transforms.py` & `leap_data_management_utils-0.0.6/leap_data_management_utils/tests/test_cmip_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils/tests/test_data_management_transforms.py` & `leap_data_management_utils-0.0.6/leap_data_management_utils/tests/test_data_management_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/PKG-INFO` & `leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -19,20 +19,24 @@
 Requires-Dist: apache-beam
 Requires-Dist: cftime
 Requires-Dist: db_dtypes
 Requires-Dist: google-api-core
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: pandas
 Requires-Dist: pangeo-forge-esgf
+Requires-Dist: pangeo-forge-recipes
 Requires-Dist: pydantic-core
 Requires-Dist: pydantic>=2
 Requires-Dist: pyyaml
 Requires-Dist: ruamel.yaml
 Requires-Dist: universal-pathlib
 Requires-Dist: xarray
 Requires-Dist: zarr
 Provides-Extra: test
-Requires-Dist: pre-commit; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: dev
+Requires-Dist: leap-data-leap_data_management_utils[test]; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
 # LEAP Data Management Utils
 
 This Repo is intended to be installed via the `requirements.txt` during recipe execution in `pangeo-forge-recipes`. It currently contains beam transforms to log information into BigQuery tables. Additional shared utilities and checks that are commonly used between LEAP pangeo-forge-feedstocks can live here.
```

### Comparing `leap_data_management_utils-0.0.5/leap_data_management_utils.egg-info/SOURCES.txt` & `leap_data_management_utils-0.0.6/leap_data_management_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 .github/dependabot.yml
 .github/workflows/catalog-ci.yaml
+.github/workflows/ci.yaml
 .github/workflows/release.yaml
 ci/environment.yaml
 leap_data_management_utils/__init__.py
 leap_data_management_utils/_version.py
 leap_data_management_utils/catalog.py
 leap_data_management_utils/cmip_catalog.py
 leap_data_management_utils/cmip_testing.py
```

### Comparing `leap_data_management_utils-0.0.5/pyproject.toml` & `leap_data_management_utils-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,26 +25,32 @@
     "apache-beam",
     "cftime",
     "db_dtypes",
     "google-api-core",
     "google-cloud-bigquery",
     "pandas",
     "pangeo-forge-esgf",
+    "pangeo-forge-recipes",
     "pydantic-core",
     "pydantic>=2",
     "pyyaml",
     "ruamel.yaml",
     "universal-pathlib",
     "xarray",
     "zarr",
 ]
 
 [project.optional-dependencies]
 test = [
-    "pre-commit",
+    "pytest"
+]
+
+dev = [
+    "leap-data-leap_data_management_utils[test]",
+    "pre-commit"
 ]
 
 
 [project.scripts]
 leap-catalog = "leap_data_management_utils.catalog:main"
```

