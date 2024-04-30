# Comparing `tmp/depot_api-1.0.4.tar.gz` & `tmp/depot_api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depot_api-1.0.4.tar", last modified: Fri Apr 19 12:45:56 2024, max compression
+gzip compressed data, was "depot_api-1.0.7.tar", last modified: Tue Apr 30 13:07:27 2024, max compression
```

## Comparing `depot_api-1.0.4.tar` & `depot_api-1.0.7.tar`

### file list

```diff
@@ -1,43 +1,53 @@
--rw-r--r--   0        0        0     5878 2024-04-19 12:38:33.227535 depot_api-1.0.4/README.md
--rw-r--r--   0        0        0     1474 2024-04-19 12:38:33.236855 depot_api-1.0.4/depot_api/__init__.py
--rw-r--r--   0        0        0       97 2024-04-19 12:38:33.238227 depot_api-1.0.4/depot_api/api/__init__.py
--rw-r--r--   0        0        0   159078 2024-04-19 12:38:33.219404 depot_api-1.0.4/depot_api/api/default_api.py
--rw-r--r--   0        0        0    25761 2024-04-19 12:38:33.242557 depot_api-1.0.4/depot_api/api_client.py
--rw-r--r--   0        0        0      652 2024-04-19 12:38:33.243026 depot_api-1.0.4/depot_api/api_response.py
--rw-r--r--   0        0        0    14735 2024-04-19 12:38:33.236127 depot_api-1.0.4/depot_api/configuration.py
--rw-r--r--   0        0        0     5972 2024-04-19 12:38:33.239537 depot_api-1.0.4/depot_api/exceptions.py
--rw-r--r--   0        0        0      926 2024-04-19 12:38:33.237708 depot_api-1.0.4/depot_api/models/__init__.py
--rw-r--r--   0        0        0     4826 2024-04-19 12:38:33.145632 depot_api-1.0.4/depot_api/models/client_id.py
--rw-r--r--   0        0        0     4850 2024-04-19 12:38:33.152608 depot_api-1.0.4/depot_api/models/client_secret.py
--rw-r--r--   0        0        0     3049 2024-04-15 14:00:46.761397 depot_api-1.0.4/depot_api/models/cluster.py
--rw-r--r--   0        0        0     2716 2024-04-19 12:38:33.159082 depot_api-1.0.4/depot_api/models/cluster_in.py
--rw-r--r--   0        0        0     4897 2024-04-19 12:38:33.164777 depot_api-1.0.4/depot_api/models/grant_type.py
--rw-r--r--   0        0        0     2978 2024-04-19 12:38:33.169450 depot_api-1.0.4/depot_api/models/http_validation_error.py
--rw-r--r--   0        0        0     4801 2024-04-19 12:38:33.173154 depot_api-1.0.4/depot_api/models/id.py
--rw-r--r--   0        0        0     3427 2024-04-18 08:54:32.098926 depot_api-1.0.4/depot_api/models/job_instance.py
--rw-r--r--   0        0        0     2948 2024-04-19 12:38:33.176100 depot_api-1.0.4/depot_api/models/job_instance_in.py
--rw-r--r--   0        0        0     3056 2024-04-19 12:38:33.179079 depot_api-1.0.4/depot_api/models/provider.py
--rw-r--r--   0        0        0     2988 2024-04-18 08:54:32.122496 depot_api-1.0.4/depot_api/models/repository.py
--rw-r--r--   0        0        0     3199 2024-04-18 08:54:32.125437 depot_api-1.0.4/depot_api/models/repository_out.py
--rw-r--r--   0        0        0     3079 2024-04-19 12:38:33.182146 depot_api-1.0.4/depot_api/models/validation_error.py
--rw-r--r--   0        0        0     4901 2024-04-19 12:38:33.184861 depot_api-1.0.4/depot_api/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0        0 2024-04-19 12:38:33.233735 depot_api-1.0.4/depot_api/py.typed
--rw-r--r--   0        0        0     9227 2024-04-19 12:38:33.244552 depot_api-1.0.4/depot_api/rest.py
--rw-r--r--   0        0        0     1868 2024-04-19 12:45:56.459860 depot_api-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 12:38:33.239878 depot_api-1.0.4/test/__init__.py
--rw-r--r--   0        0        0     1276 2024-04-18 20:09:02.454188 depot_api-1.0.4/test/test_client_id.py
--rw-r--r--   0        0        0     1324 2024-04-18 20:09:02.466568 depot_api-1.0.4/test/test_client_secret.py
--rw-r--r--   0        0        0     1509 2024-04-15 14:00:46.763230 depot_api-1.0.4/test/test_cluster.py
--rw-r--r--   0        0        0     1685 2024-04-16 05:26:03.952432 depot_api-1.0.4/test/test_cluster_in.py
--rw-r--r--   0        0        0     3543 2024-04-15 14:00:46.839817 depot_api-1.0.4/test/test_default_api.py
--rw-r--r--   0        0        0     1288 2024-04-18 20:09:02.478374 depot_api-1.0.4/test/test_grant_type.py
--rw-r--r--   0        0        0     1698 2024-04-15 14:00:46.769812 depot_api-1.0.4/test/test_http_validation_error.py
--rw-r--r--   0        0        0     1203 2024-04-15 14:00:46.780645 depot_api-1.0.4/test/test_id.py
--rw-r--r--   0        0        0     1663 2024-04-15 14:00:46.785728 depot_api-1.0.4/test/test_job_instance.py
--rw-r--r--   0        0        0     1732 2024-04-18 06:49:32.731307 depot_api-1.0.4/test/test_job_instance_in.py
--rw-r--r--   0        0        0     1526 2024-04-15 14:00:46.790366 depot_api-1.0.4/test/test_provider.py
--rw-r--r--   0        0        0     1569 2024-04-15 14:00:46.793463 depot_api-1.0.4/test/test_repository.py
--rw-r--r--   0        0        0     2371 2024-04-15 14:00:46.796985 depot_api-1.0.4/test/test_repository_out.py
--rw-r--r--   0        0        0     1609 2024-04-15 14:00:46.800103 depot_api-1.0.4/test/test_validation_error.py
--rw-r--r--   0        0        0     1458 2024-04-15 14:00:46.802999 depot_api-1.0.4/test/test_validation_error_loc_inner.py
--rw-r--r--   0        0        0     6594 1970-01-01 00:00:00.000000 depot_api-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7628 2024-04-30 11:01:54.696567 depot_api-1.0.7/README.md
+-rw-r--r--   0        0        0     1579 2024-04-30 11:01:54.720574 depot_api-1.0.7/depot_api/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-30 11:01:54.722210 depot_api-1.0.7/depot_api/api/__init__.py
+-rw-r--r--   0        0        0   257139 2024-04-30 11:01:54.654214 depot_api-1.0.7/depot_api/api/default_api.py
+-rw-r--r--   0        0        0    25761 2024-04-30 11:01:54.727516 depot_api-1.0.7/depot_api/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-30 11:01:54.728128 depot_api-1.0.7/depot_api/api_response.py
+-rw-r--r--   0        0        0    14735 2024-04-30 11:01:54.719388 depot_api-1.0.7/depot_api/configuration.py
+-rw-r--r--   0        0        0     5972 2024-04-30 11:01:54.723817 depot_api-1.0.7/depot_api/exceptions.py
+-rw-r--r--   0        0        0     1031 2024-04-30 11:01:54.721577 depot_api-1.0.7/depot_api/models/__init__.py
+-rw-r--r--   0        0        0     4826 2024-04-30 11:01:54.502071 depot_api-1.0.7/depot_api/models/client_id.py
+-rw-r--r--   0        0        0     4850 2024-04-30 11:01:54.511995 depot_api-1.0.7/depot_api/models/client_secret.py
+-rw-r--r--   0        0        0     3049 2024-04-15 14:00:46.761397 depot_api-1.0.7/depot_api/models/cluster.py
+-rw-r--r--   0        0        0     2716 2024-04-30 11:01:54.519862 depot_api-1.0.7/depot_api/models/cluster_in.py
+-rw-r--r--   0        0        0     4897 2024-04-30 11:01:54.526646 depot_api-1.0.7/depot_api/models/grant_type.py
+-rw-r--r--   0        0        0     2978 2024-04-30 11:01:54.535113 depot_api-1.0.7/depot_api/models/http_validation_error.py
+-rw-r--r--   0        0        0     4801 2024-04-30 11:01:54.541423 depot_api-1.0.7/depot_api/models/id.py
+-rw-r--r--   0        0        0     3427 2024-04-18 08:54:32.098926 depot_api-1.0.7/depot_api/models/job_instance.py
+-rw-r--r--   0        0        0     2948 2024-04-30 11:01:54.548015 depot_api-1.0.7/depot_api/models/job_instance_in.py
+-rw-r--r--   0        0        0     4838 2024-04-30 09:34:16.126240 depot_api-1.0.7/depot_api/models/private_key.py
+-rw-r--r--   0        0        0     3056 2024-04-30 11:01:54.553912 depot_api-1.0.7/depot_api/models/provider.py
+-rw-r--r--   0        0        0     4832 2024-04-30 09:34:16.126948 depot_api-1.0.7/depot_api/models/public_key.py
+-rw-r--r--   0        0        0     2988 2024-04-18 08:54:32.122496 depot_api-1.0.7/depot_api/models/repository.py
+-rw-r--r--   0        0        0     2650 2024-04-30 11:01:54.560586 depot_api-1.0.7/depot_api/models/repository_in.py
+-rw-r--r--   0        0        0     4856 2024-04-30 09:34:16.127862 depot_api-1.0.7/depot_api/models/repository_key.py
+-rw-r--r--   0        0        0     3199 2024-04-18 08:54:32.125437 depot_api-1.0.7/depot_api/models/repository_out.py
+-rw-r--r--   0        0        0     2715 2024-04-30 11:01:54.568091 depot_api-1.0.7/depot_api/models/ssh_key_in.py
+-rw-r--r--   0        0        0     3079 2024-04-30 11:01:54.572631 depot_api-1.0.7/depot_api/models/validation_error.py
+-rw-r--r--   0        0        0     4901 2024-04-30 11:01:54.576452 depot_api-1.0.7/depot_api/models/validation_error_loc_inner.py
+-rw-r--r--   0        0        0        0 2024-04-30 11:01:54.716503 depot_api-1.0.7/depot_api/py.typed
+-rw-r--r--   0        0        0     9227 2024-04-30 11:01:54.729580 depot_api-1.0.7/depot_api/rest.py
+-rw-r--r--   0        0        0     1919 2024-04-30 13:07:27.717369 depot_api-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 11:01:54.724655 depot_api-1.0.7/test/__init__.py
+-rw-r--r--   0        0        0     1276 2024-04-18 20:09:02.454188 depot_api-1.0.7/test/test_client_id.py
+-rw-r--r--   0        0        0     1324 2024-04-18 20:09:02.466568 depot_api-1.0.7/test/test_client_secret.py
+-rw-r--r--   0        0        0     1509 2024-04-15 14:00:46.763230 depot_api-1.0.7/test/test_cluster.py
+-rw-r--r--   0        0        0     1685 2024-04-16 05:26:03.952432 depot_api-1.0.7/test/test_cluster_in.py
+-rw-r--r--   0        0        0     3543 2024-04-15 14:00:46.839817 depot_api-1.0.7/test/test_default_api.py
+-rw-r--r--   0        0        0     1288 2024-04-18 20:09:02.478374 depot_api-1.0.7/test/test_grant_type.py
+-rw-r--r--   0        0        0     1698 2024-04-15 14:00:46.769812 depot_api-1.0.7/test/test_http_validation_error.py
+-rw-r--r--   0        0        0     1203 2024-04-15 14:00:46.780645 depot_api-1.0.7/test/test_id.py
+-rw-r--r--   0        0        0     1663 2024-04-15 14:00:46.785728 depot_api-1.0.7/test/test_job_instance.py
+-rw-r--r--   0        0        0     1732 2024-04-18 06:49:32.731307 depot_api-1.0.7/test/test_job_instance_in.py
+-rw-r--r--   0        0        0     1300 2024-04-30 09:34:16.145205 depot_api-1.0.7/test/test_private_key.py
+-rw-r--r--   0        0        0     1526 2024-04-15 14:00:46.790366 depot_api-1.0.7/test/test_provider.py
+-rw-r--r--   0        0        0     1288 2024-04-30 09:34:16.149824 depot_api-1.0.7/test/test_public_key.py
+-rw-r--r--   0        0        0     1569 2024-04-15 14:00:46.793463 depot_api-1.0.7/test/test_repository.py
+-rw-r--r--   0        0        0     1513 2024-04-30 09:34:16.155031 depot_api-1.0.7/test/test_repository_in.py
+-rw-r--r--   0        0        0     1336 2024-04-30 09:34:16.157940 depot_api-1.0.7/test/test_repository_key.py
+-rw-r--r--   0        0        0     2371 2024-04-15 14:00:46.796985 depot_api-1.0.7/test/test_repository_out.py
+-rw-r--r--   0        0        0     1528 2024-04-30 09:34:16.159968 depot_api-1.0.7/test/test_ssh_key_in.py
+-rw-r--r--   0        0        0     1609 2024-04-15 14:00:46.800103 depot_api-1.0.7/test/test_validation_error.py
+-rw-r--r--   0        0        0     1458 2024-04-15 14:00:46.802999 depot_api-1.0.7/test/test_validation_error_loc_inner.py
+-rw-r--r--   0        0        0     8369 1970-01-01 00:00:00.000000 depot_api-1.0.7/PKG-INFO
```

### Comparing `depot_api-1.0.4/README.md` & `depot_api-1.0.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -89,40 +89,52 @@
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *DefaultApi* | [**create_cluster_clusters_post**](docs/DefaultApi.md#create_cluster_clusters_post) | **POST** /clusters/ | Create Cluster
 *DefaultApi* | [**create_job_instance_job_instances_post**](docs/DefaultApi.md#create_job_instance_job_instances_post) | **POST** /job_instances/ | Create Job Instance
+*DefaultApi* | [**create_managed_ssh_key_managed_ssh_keys_post**](docs/DefaultApi.md#create_managed_ssh_key_managed_ssh_keys_post) | **POST** /managed_ssh_keys/ | Create Managed Ssh Key
 *DefaultApi* | [**create_provider_providers_post**](docs/DefaultApi.md#create_provider_providers_post) | **POST** /providers/ | Create Provider
+*DefaultApi* | [**create_repository_repositories_post**](docs/DefaultApi.md#create_repository_repositories_post) | **POST** /repositories/ | Create Repository
+*DefaultApi* | [**create_ssh_key_ssh_keys_post**](docs/DefaultApi.md#create_ssh_key_ssh_keys_post) | **POST** /ssh_keys/ | Create Ssh Key
 *DefaultApi* | [**delete_cluster_clusters_cluster_id_delete**](docs/DefaultApi.md#delete_cluster_clusters_cluster_id_delete) | **DELETE** /clusters/{cluster_id} | Delete Cluster
 *DefaultApi* | [**delete_job_instance_job_instances_job_instance_id_delete**](docs/DefaultApi.md#delete_job_instance_job_instances_job_instance_id_delete) | **DELETE** /job_instances/{job_instance_id} | Delete Job Instance
 *DefaultApi* | [**delete_provider_providers_provider_id_delete**](docs/DefaultApi.md#delete_provider_providers_provider_id_delete) | **DELETE** /providers/{provider_id} | Delete Provider
+*DefaultApi* | [**delete_ssh_key_ssh_keys_key_name_delete**](docs/DefaultApi.md#delete_ssh_key_ssh_keys_key_name_delete) | **DELETE** /ssh_keys/{key_name} | Delete Ssh Key
+*DefaultApi* | [**get_managed_ssh_key_managed_ssh_keys_get**](docs/DefaultApi.md#get_managed_ssh_key_managed_ssh_keys_get) | **GET** /managed_ssh_keys/ | Get Managed Ssh Key
 *DefaultApi* | [**list_clusters_clusters_get**](docs/DefaultApi.md#list_clusters_clusters_get) | **GET** /clusters/ | List Clusters
 *DefaultApi* | [**list_job_instances_job_instances_get**](docs/DefaultApi.md#list_job_instances_job_instances_get) | **GET** /job_instances/ | List Job Instances
 *DefaultApi* | [**list_providers_providers_get**](docs/DefaultApi.md#list_providers_providers_get) | **GET** /providers/ | List Providers
 *DefaultApi* | [**list_providers_types_provider_types_get**](docs/DefaultApi.md#list_providers_types_provider_types_get) | **GET** /provider_types/ | List Providers Types
+*DefaultApi* | [**list_repositories_repositories_get**](docs/DefaultApi.md#list_repositories_repositories_get) | **GET** /repositories/ | List Repositories
+*DefaultApi* | [**list_ssh_keys_ssh_keys_get**](docs/DefaultApi.md#list_ssh_keys_ssh_keys_get) | **GET** /ssh_keys/ | List Ssh Keys
 *DefaultApi* | [**login_token_post**](docs/DefaultApi.md#login_token_post) | **POST** /token | Login
 *DefaultApi* | [**read_cluster_clusters_cluster_id_get**](docs/DefaultApi.md#read_cluster_clusters_cluster_id_get) | **GET** /clusters/{cluster_id} | Read Cluster
 *DefaultApi* | [**read_job_instance_job_instances_job_instance_id_get**](docs/DefaultApi.md#read_job_instance_job_instances_job_instance_id_get) | **GET** /job_instances/{job_instance_id} | Read Job Instance
 *DefaultApi* | [**read_log_logs_job_instance_id_get**](docs/DefaultApi.md#read_log_logs_job_instance_id_get) | **GET** /logs/{job_instance_id} | Read Log
 *DefaultApi* | [**read_provider_providers_provider_id_get**](docs/DefaultApi.md#read_provider_providers_provider_id_get) | **GET** /providers/{provider_id} | Read Provider
+*DefaultApi* | [**read_repository_by_name_repositories_by_name_get**](docs/DefaultApi.md#read_repository_by_name_repositories_by_name_get) | **GET** /repositories/by_name/ | Read Repository By Name
+*DefaultApi* | [**read_ssh_key_by_name_ssh_keys_by_name_get**](docs/DefaultApi.md#read_ssh_key_by_name_ssh_keys_by_name_get) | **GET** /ssh_keys/by_name/ | Read Ssh Key By Name
 *DefaultApi* | [**read_users_me_users_me_get**](docs/DefaultApi.md#read_users_me_users_me_get) | **GET** /users/me | Read Users Me
+*DefaultApi* | [**update_repository_repositories_by_name_patch**](docs/DefaultApi.md#update_repository_repositories_by_name_patch) | **PATCH** /repositories/by_name/ | Update Repository
 
 
 ## Documentation For Models
 
  - [ClientId](docs/ClientId.md)
  - [ClientSecret](docs/ClientSecret.md)
  - [ClusterIn](docs/ClusterIn.md)
  - [GrantType](docs/GrantType.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
  - [Id](docs/Id.md)
  - [JobInstanceIn](docs/JobInstanceIn.md)
  - [Provider](docs/Provider.md)
+ - [RepositoryIn](docs/RepositoryIn.md)
+ - [SshKeyIn](docs/SshKeyIn.md)
  - [ValidationError](docs/ValidationError.md)
  - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
```

### Comparing `depot_api-1.0.4/depot_api/__init__.py` & `depot_api-1.0.7/depot_api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,9 +35,11 @@
 from depot_api.models.client_secret import ClientSecret
 from depot_api.models.cluster_in import ClusterIn
 from depot_api.models.grant_type import GrantType
 from depot_api.models.http_validation_error import HTTPValidationError
 from depot_api.models.id import Id
 from depot_api.models.job_instance_in import JobInstanceIn
 from depot_api.models.provider import Provider
+from depot_api.models.repository_in import RepositoryIn
+from depot_api.models.ssh_key_in import SshKeyIn
 from depot_api.models.validation_error import ValidationError
 from depot_api.models.validation_error_loc_inner import ValidationErrorLocInner
```

### Comparing `depot_api-1.0.4/depot_api/api/default_api.py` & `depot_api-1.0.7/depot_api/api/default_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from typing import Optional
 from depot_api.models.client_id import ClientId
 from depot_api.models.client_secret import ClientSecret
 from depot_api.models.cluster_in import ClusterIn
 from depot_api.models.grant_type import GrantType
 from depot_api.models.job_instance_in import JobInstanceIn
 from depot_api.models.provider import Provider
+from depot_api.models.repository_in import RepositoryIn
+from depot_api.models.ssh_key_in import SshKeyIn
 
 from depot_api.api_client import ApiClient, RequestSerialized
 from depot_api.api_response import ApiResponse
 from depot_api.rest import RESTResponseType
 
 
 class DefaultApi:
@@ -582,14 +584,274 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def create_managed_ssh_key_managed_ssh_keys_post(
+        self,
+        service: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Create Managed Ssh Key
+
+
+        :param service: (required)
+        :type service: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_managed_ssh_key_managed_ssh_keys_post_serialize(
+            service=service,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def create_managed_ssh_key_managed_ssh_keys_post_with_http_info(
+        self,
+        service: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Create Managed Ssh Key
+
+
+        :param service: (required)
+        :type service: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_managed_ssh_key_managed_ssh_keys_post_serialize(
+            service=service,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def create_managed_ssh_key_managed_ssh_keys_post_without_preload_content(
+        self,
+        service: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Create Managed Ssh Key
+
+
+        :param service: (required)
+        :type service: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_managed_ssh_key_managed_ssh_keys_post_serialize(
+            service=service,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _create_managed_ssh_key_managed_ssh_keys_post_serialize(
+        self,
+        service,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if service is not None:
+            
+            _query_params.append(('service', service))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/managed_ssh_keys/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def create_provider_providers_post(
         self,
         provider: Provider,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -853,14 +1115,556 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def create_repository_repositories_post(
+        self,
+        repository_in: RepositoryIn,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Create Repository
+
+
+        :param repository_in: (required)
+        :type repository_in: RepositoryIn
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_repository_repositories_post_serialize(
+            repository_in=repository_in,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def create_repository_repositories_post_with_http_info(
+        self,
+        repository_in: RepositoryIn,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Create Repository
+
+
+        :param repository_in: (required)
+        :type repository_in: RepositoryIn
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_repository_repositories_post_serialize(
+            repository_in=repository_in,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def create_repository_repositories_post_without_preload_content(
+        self,
+        repository_in: RepositoryIn,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Create Repository
+
+
+        :param repository_in: (required)
+        :type repository_in: RepositoryIn
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_repository_repositories_post_serialize(
+            repository_in=repository_in,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _create_repository_repositories_post_serialize(
+        self,
+        repository_in,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if repository_in is not None:
+            _body_params = repository_in
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/repositories/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def create_ssh_key_ssh_keys_post(
+        self,
+        ssh_key_in: SshKeyIn,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Create Ssh Key
+
+
+        :param ssh_key_in: (required)
+        :type ssh_key_in: SshKeyIn
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_ssh_key_ssh_keys_post_serialize(
+            ssh_key_in=ssh_key_in,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def create_ssh_key_ssh_keys_post_with_http_info(
+        self,
+        ssh_key_in: SshKeyIn,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Create Ssh Key
+
+
+        :param ssh_key_in: (required)
+        :type ssh_key_in: SshKeyIn
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_ssh_key_ssh_keys_post_serialize(
+            ssh_key_in=ssh_key_in,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def create_ssh_key_ssh_keys_post_without_preload_content(
+        self,
+        ssh_key_in: SshKeyIn,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Create Ssh Key
+
+
+        :param ssh_key_in: (required)
+        :type ssh_key_in: SshKeyIn
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_ssh_key_ssh_keys_post_serialize(
+            ssh_key_in=ssh_key_in,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _create_ssh_key_ssh_keys_post_serialize(
+        self,
+        ssh_key_in,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if ssh_key_in is not None:
+            _body_params = ssh_key_in
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/ssh_keys/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def delete_cluster_clusters_cluster_id_delete(
         self,
         cluster_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -1627,14 +2431,532 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def delete_ssh_key_ssh_keys_key_name_delete(
+        self,
+        key_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Delete Ssh Key
+
+
+        :param key_name: (required)
+        :type key_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_ssh_key_ssh_keys_key_name_delete_serialize(
+            key_name=key_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def delete_ssh_key_ssh_keys_key_name_delete_with_http_info(
+        self,
+        key_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Delete Ssh Key
+
+
+        :param key_name: (required)
+        :type key_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_ssh_key_ssh_keys_key_name_delete_serialize(
+            key_name=key_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def delete_ssh_key_ssh_keys_key_name_delete_without_preload_content(
+        self,
+        key_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Delete Ssh Key
+
+
+        :param key_name: (required)
+        :type key_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_ssh_key_ssh_keys_key_name_delete_serialize(
+            key_name=key_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _delete_ssh_key_ssh_keys_key_name_delete_serialize(
+        self,
+        key_name,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if key_name is not None:
+            _path_params['key_name'] = key_name
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='DELETE',
+            resource_path='/ssh_keys/{key_name}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def get_managed_ssh_key_managed_ssh_keys_get(
+        self,
+        service: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Get Managed Ssh Key
+
+
+        :param service: (required)
+        :type service: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_managed_ssh_key_managed_ssh_keys_get_serialize(
+            service=service,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def get_managed_ssh_key_managed_ssh_keys_get_with_http_info(
+        self,
+        service: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Get Managed Ssh Key
+
+
+        :param service: (required)
+        :type service: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_managed_ssh_key_managed_ssh_keys_get_serialize(
+            service=service,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def get_managed_ssh_key_managed_ssh_keys_get_without_preload_content(
+        self,
+        service: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Get Managed Ssh Key
+
+
+        :param service: (required)
+        :type service: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_managed_ssh_key_managed_ssh_keys_get_serialize(
+            service=service,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _get_managed_ssh_key_managed_ssh_keys_get_serialize(
+        self,
+        service,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if service is not None:
+            
+            _query_params.append(('service', service))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/managed_ssh_keys/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def list_clusters_clusters_get(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -2587,14 +3909,494 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def list_repositories_repositories_get(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """List Repositories
+
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._list_repositories_repositories_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def list_repositories_repositories_get_with_http_info(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """List Repositories
+
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._list_repositories_repositories_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def list_repositories_repositories_get_without_preload_content(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """List Repositories
+
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._list_repositories_repositories_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _list_repositories_repositories_get_serialize(
+        self,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/repositories/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def list_ssh_keys_ssh_keys_get(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """List Ssh Keys
+
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._list_ssh_keys_ssh_keys_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def list_ssh_keys_ssh_keys_get_with_http_info(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """List Ssh Keys
+
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._list_ssh_keys_ssh_keys_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def list_ssh_keys_ssh_keys_get_without_preload_content(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """List Ssh Keys
+
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._list_ssh_keys_ssh_keys_get_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _list_ssh_keys_ssh_keys_get_serialize(
+        self,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/ssh_keys/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def login_token_post(
         self,
         username: StrictStr,
         password: StrictStr,
         grant_type: Optional[GrantType] = None,
         scope: Optional[StrictStr] = None,
         client_id: Optional[ClientId] = None,
@@ -3964,14 +5766,534 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def read_repository_by_name_repositories_by_name_get(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Read Repository By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_repository_by_name_repositories_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def read_repository_by_name_repositories_by_name_get_with_http_info(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Read Repository By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_repository_by_name_repositories_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def read_repository_by_name_repositories_by_name_get_without_preload_content(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Read Repository By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_repository_by_name_repositories_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _read_repository_by_name_repositories_by_name_get_serialize(
+        self,
+        name,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if name is not None:
+            
+            _query_params.append(('name', name))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/repositories/by_name/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def read_ssh_key_by_name_ssh_keys_by_name_get(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Read Ssh Key By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_ssh_key_by_name_ssh_keys_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def read_ssh_key_by_name_ssh_keys_by_name_get_with_http_info(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Read Ssh Key By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_ssh_key_by_name_ssh_keys_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def read_ssh_key_by_name_ssh_keys_by_name_get_without_preload_content(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Read Ssh Key By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_ssh_key_by_name_ssh_keys_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _read_ssh_key_by_name_ssh_keys_by_name_get_serialize(
+        self,
+        name,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if name is not None:
+            
+            _query_params.append(('name', name))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/ssh_keys/by_name/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def read_users_me_users_me_get(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -4195,13 +6517,290 @@
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def update_repository_repositories_by_name_patch(
+        self,
+        repository_url: StrictStr,
+        ssh_key_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Update Repository
+
+
+        :param repository_url: (required)
+        :type repository_url: str
+        :param ssh_key_name: (required)
+        :type ssh_key_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._update_repository_repositories_by_name_patch_serialize(
+            repository_url=repository_url,
+            ssh_key_name=ssh_key_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def update_repository_repositories_by_name_patch_with_http_info(
+        self,
+        repository_url: StrictStr,
+        ssh_key_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Update Repository
+
+
+        :param repository_url: (required)
+        :type repository_url: str
+        :param ssh_key_name: (required)
+        :type ssh_key_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._update_repository_repositories_by_name_patch_serialize(
+            repository_url=repository_url,
+            ssh_key_name=ssh_key_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def update_repository_repositories_by_name_patch_without_preload_content(
+        self,
+        repository_url: StrictStr,
+        ssh_key_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Update Repository
+
+
+        :param repository_url: (required)
+        :type repository_url: str
+        :param ssh_key_name: (required)
+        :type ssh_key_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._update_repository_repositories_by_name_patch_serialize(
+            repository_url=repository_url,
+            ssh_key_name=ssh_key_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _update_repository_repositories_by_name_patch_serialize(
+        self,
+        repository_url,
+        ssh_key_name,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if repository_url is not None:
+            
+            _query_params.append(('repository_url', repository_url))
+            
+        if ssh_key_name is not None:
+            
+            _query_params.append(('ssh_key_name', ssh_key_name))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='PATCH',
+            resource_path='/repositories/by_name/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `depot_api-1.0.4/depot_api/api_client.py` & `depot_api-1.0.7/depot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/api_response.py` & `depot_api-1.0.7/depot_api/api_response.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/configuration.py` & `depot_api-1.0.7/depot_api/configuration.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/exceptions.py` & `depot_api-1.0.7/depot_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/__init__.py` & `depot_api-1.0.7/depot_api/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,9 +18,11 @@
 from depot_api.models.client_secret import ClientSecret
 from depot_api.models.cluster_in import ClusterIn
 from depot_api.models.grant_type import GrantType
 from depot_api.models.http_validation_error import HTTPValidationError
 from depot_api.models.id import Id
 from depot_api.models.job_instance_in import JobInstanceIn
 from depot_api.models.provider import Provider
+from depot_api.models.repository_in import RepositoryIn
+from depot_api.models.ssh_key_in import SshKeyIn
 from depot_api.models.validation_error import ValidationError
 from depot_api.models.validation_error_loc_inner import ValidationErrorLocInner
```

### Comparing `depot_api-1.0.4/depot_api/models/client_id.py` & `depot_api-1.0.7/depot_api/models/client_id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/client_secret.py` & `depot_api-1.0.7/depot_api/models/client_secret.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/cluster.py` & `depot_api-1.0.7/depot_api/models/cluster.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/cluster_in.py` & `depot_api-1.0.7/depot_api/models/cluster_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/grant_type.py` & `depot_api-1.0.7/depot_api/models/grant_type.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/http_validation_error.py` & `depot_api-1.0.7/depot_api/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/id.py` & `depot_api-1.0.7/depot_api/models/id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/job_instance.py` & `depot_api-1.0.7/depot_api/models/job_instance.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/job_instance_in.py` & `depot_api-1.0.7/depot_api/models/job_instance_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/provider.py` & `depot_api-1.0.7/depot_api/models/provider.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/repository.py` & `depot_api-1.0.7/depot_api/models/repository.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/repository_out.py` & `depot_api-1.0.7/depot_api/models/repository_out.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/validation_error.py` & `depot_api-1.0.7/depot_api/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/models/validation_error_loc_inner.py` & `depot_api-1.0.7/depot_api/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/depot_api/rest.py` & `depot_api-1.0.7/depot_api/rest.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/pyproject.toml` & `depot_api-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -56,30 +56,31 @@
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 authors = [
     { name = "OpenAPI Generator Community", email = "team@openapitools.org" },
-    { name = "CodeDepot Team", email = "contact@codedepot.ai" },
+    { name = "OpenAPI Generator community", email = "team@openapitools.org" },
+    { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 requires-python = "<4.0,>=3.7"
 dependencies = [
     "urllib3>=1.25.3",
     "python-dateutil>=2.8.2",
     "pydantic>=2",
     "typing-extensions>=4.7.1",
     "pydantic >= 2",
     "python-dateutil",
     "typing-extensions >= 4.7.1",
     "urllib3 >= 1.25.3, < 2.1.0",
 ]
 name = "depot-api"
-version = "1.0.4"
-description = "FastAPI client for the Depot API"
+version = "1.0.7"
+description = "Depot API"
 readme = "README.md"
 keywords = [
     "OpenAPI",
     "OpenAPI-Generator",
     "FastAPI",
 ]
```

### Comparing `depot_api-1.0.4/test/test_client_id.py` & `depot_api-1.0.7/test/test_client_id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_client_secret.py` & `depot_api-1.0.7/test/test_client_secret.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_cluster.py` & `depot_api-1.0.7/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_cluster_in.py` & `depot_api-1.0.7/test/test_cluster_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_default_api.py` & `depot_api-1.0.7/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_grant_type.py` & `depot_api-1.0.7/test/test_grant_type.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_http_validation_error.py` & `depot_api-1.0.7/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_id.py` & `depot_api-1.0.7/test/test_id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_job_instance.py` & `depot_api-1.0.7/test/test_job_instance.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_job_instance_in.py` & `depot_api-1.0.7/test/test_job_instance_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_provider.py` & `depot_api-1.0.7/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_repository.py` & `depot_api-1.0.7/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_repository_out.py` & `depot_api-1.0.7/test/test_repository_out.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_validation_error.py` & `depot_api-1.0.7/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/test/test_validation_error_loc_inner.py` & `depot_api-1.0.7/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.4/PKG-INFO` & `depot_api-1.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: depot-api
-Version: 1.0.4
-Summary: FastAPI client for the Depot API
+Version: 1.0.7
+Summary: Depot API
 Keywords: OpenAPI,OpenAPI-Generator,FastAPI
-Author-Email: OpenAPI Generator Community <team@openapitools.org>, CodeDepot Team <contact@codedepot.ai>
+Author-Email: OpenAPI Generator Community <team@openapitools.org>, OpenAPI Generator community <team@openapitools.org>, CodeDepot <contact@codedepot.ai>
 License: NoLicense
 Project-URL: Repository, https://github.com/GIT_USER_ID/GIT_REPO_ID
 Project-URL: Homepage, https://codedepot.ai
 Requires-Python: <4.0,>=3.7
 Requires-Dist: urllib3>=1.25.3
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pydantic>=2
@@ -109,40 +109,52 @@
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *DefaultApi* | [**create_cluster_clusters_post**](docs/DefaultApi.md#create_cluster_clusters_post) | **POST** /clusters/ | Create Cluster
 *DefaultApi* | [**create_job_instance_job_instances_post**](docs/DefaultApi.md#create_job_instance_job_instances_post) | **POST** /job_instances/ | Create Job Instance
+*DefaultApi* | [**create_managed_ssh_key_managed_ssh_keys_post**](docs/DefaultApi.md#create_managed_ssh_key_managed_ssh_keys_post) | **POST** /managed_ssh_keys/ | Create Managed Ssh Key
 *DefaultApi* | [**create_provider_providers_post**](docs/DefaultApi.md#create_provider_providers_post) | **POST** /providers/ | Create Provider
+*DefaultApi* | [**create_repository_repositories_post**](docs/DefaultApi.md#create_repository_repositories_post) | **POST** /repositories/ | Create Repository
+*DefaultApi* | [**create_ssh_key_ssh_keys_post**](docs/DefaultApi.md#create_ssh_key_ssh_keys_post) | **POST** /ssh_keys/ | Create Ssh Key
 *DefaultApi* | [**delete_cluster_clusters_cluster_id_delete**](docs/DefaultApi.md#delete_cluster_clusters_cluster_id_delete) | **DELETE** /clusters/{cluster_id} | Delete Cluster
 *DefaultApi* | [**delete_job_instance_job_instances_job_instance_id_delete**](docs/DefaultApi.md#delete_job_instance_job_instances_job_instance_id_delete) | **DELETE** /job_instances/{job_instance_id} | Delete Job Instance
 *DefaultApi* | [**delete_provider_providers_provider_id_delete**](docs/DefaultApi.md#delete_provider_providers_provider_id_delete) | **DELETE** /providers/{provider_id} | Delete Provider
+*DefaultApi* | [**delete_ssh_key_ssh_keys_key_name_delete**](docs/DefaultApi.md#delete_ssh_key_ssh_keys_key_name_delete) | **DELETE** /ssh_keys/{key_name} | Delete Ssh Key
+*DefaultApi* | [**get_managed_ssh_key_managed_ssh_keys_get**](docs/DefaultApi.md#get_managed_ssh_key_managed_ssh_keys_get) | **GET** /managed_ssh_keys/ | Get Managed Ssh Key
 *DefaultApi* | [**list_clusters_clusters_get**](docs/DefaultApi.md#list_clusters_clusters_get) | **GET** /clusters/ | List Clusters
 *DefaultApi* | [**list_job_instances_job_instances_get**](docs/DefaultApi.md#list_job_instances_job_instances_get) | **GET** /job_instances/ | List Job Instances
 *DefaultApi* | [**list_providers_providers_get**](docs/DefaultApi.md#list_providers_providers_get) | **GET** /providers/ | List Providers
 *DefaultApi* | [**list_providers_types_provider_types_get**](docs/DefaultApi.md#list_providers_types_provider_types_get) | **GET** /provider_types/ | List Providers Types
+*DefaultApi* | [**list_repositories_repositories_get**](docs/DefaultApi.md#list_repositories_repositories_get) | **GET** /repositories/ | List Repositories
+*DefaultApi* | [**list_ssh_keys_ssh_keys_get**](docs/DefaultApi.md#list_ssh_keys_ssh_keys_get) | **GET** /ssh_keys/ | List Ssh Keys
 *DefaultApi* | [**login_token_post**](docs/DefaultApi.md#login_token_post) | **POST** /token | Login
 *DefaultApi* | [**read_cluster_clusters_cluster_id_get**](docs/DefaultApi.md#read_cluster_clusters_cluster_id_get) | **GET** /clusters/{cluster_id} | Read Cluster
 *DefaultApi* | [**read_job_instance_job_instances_job_instance_id_get**](docs/DefaultApi.md#read_job_instance_job_instances_job_instance_id_get) | **GET** /job_instances/{job_instance_id} | Read Job Instance
 *DefaultApi* | [**read_log_logs_job_instance_id_get**](docs/DefaultApi.md#read_log_logs_job_instance_id_get) | **GET** /logs/{job_instance_id} | Read Log
 *DefaultApi* | [**read_provider_providers_provider_id_get**](docs/DefaultApi.md#read_provider_providers_provider_id_get) | **GET** /providers/{provider_id} | Read Provider
+*DefaultApi* | [**read_repository_by_name_repositories_by_name_get**](docs/DefaultApi.md#read_repository_by_name_repositories_by_name_get) | **GET** /repositories/by_name/ | Read Repository By Name
+*DefaultApi* | [**read_ssh_key_by_name_ssh_keys_by_name_get**](docs/DefaultApi.md#read_ssh_key_by_name_ssh_keys_by_name_get) | **GET** /ssh_keys/by_name/ | Read Ssh Key By Name
 *DefaultApi* | [**read_users_me_users_me_get**](docs/DefaultApi.md#read_users_me_users_me_get) | **GET** /users/me | Read Users Me
+*DefaultApi* | [**update_repository_repositories_by_name_patch**](docs/DefaultApi.md#update_repository_repositories_by_name_patch) | **PATCH** /repositories/by_name/ | Update Repository
 
 
 ## Documentation For Models
 
  - [ClientId](docs/ClientId.md)
  - [ClientSecret](docs/ClientSecret.md)
  - [ClusterIn](docs/ClusterIn.md)
  - [GrantType](docs/GrantType.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
  - [Id](docs/Id.md)
  - [JobInstanceIn](docs/JobInstanceIn.md)
  - [Provider](docs/Provider.md)
+ - [RepositoryIn](docs/RepositoryIn.md)
+ - [SshKeyIn](docs/SshKeyIn.md)
  - [ValidationError](docs/ValidationError.md)
  - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
```

