# Comparing `tmp/aioli_sdk-0.2.2rc0.tar.gz` & `tmp/aioli_sdk-0.2.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli_sdk-0.2.2rc0.tar", last modified: Mon Apr 29 17:19:02 2024, max compression
+gzip compressed data, was "aioli_sdk-0.2.3.dev0.tar", last modified: Mon Apr 29 18:41:55 2024, max compression
```

## Comparing `aioli_sdk-0.2.2rc0.tar` & `aioli_sdk-0.2.3.dev0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.646988 aioli_sdk-0.2.2rc0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-04-29 17:19:02.646988 aioli_sdk-0.2.2rc0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.638988 aioli_sdk-0.2.2rc0/aioli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.638988 aioli_sdk-0.2.2rc0/aioli/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14908 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7705 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.638988 aioli_sdk-0.2.2rc0/aioli/cli/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28285 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.638988 aioli_sdk-0.2.2rc0/aioli/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.638988 aioli_sdk-0.2.2rc0/aioli/common/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/api/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/requests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/common/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/aioli/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.646988 aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-04-29 17:19:02.000000 aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2447 2024-04-29 17:19:02.000000 aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-29 17:19:02.000000 aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-29 17:19:02.000000 aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-29 17:19:00.000000 aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-29 17:19:02.000000 aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-29 17:19:02.000000 aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.642988 aioli_sdk-0.2.2rc0/aiolirest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.642988 aioli_sdk-0.2.2rc0/aiolirest/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22812 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    84658 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10514 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91192 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/packaged_models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54370 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43081 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105943 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/templates_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61884 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25049 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/api_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14924 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5596 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:19:02.646988 aioli_sdk-0.2.2rc0/aiolirest/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2221 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3383 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/auto_scaling_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3985 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3661 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7355 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/deployment_model_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5067 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4883 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2787 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3774 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/event_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2641 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2535 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/model_auth_token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/observability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6064 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/packaged_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5498 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/packaged_model_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2939 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3365 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/resources_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2835 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3295 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/security.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2648 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5201 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5027 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3931 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3386 2024-04-29 17:18:58.000000 aioli_sdk-0.2.2rc0/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8439 2024-04-29 17:18:59.000000 aioli_sdk-0.2.2rc0/aiolirest/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-29 17:19:02.646988 aioli_sdk-0.2.2rc0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-04-29 17:13:44.000000 aioli_sdk-0.2.2rc0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.654555 aioli_sdk-0.2.3.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-04-29 18:41:55.654555 aioli_sdk-0.2.3.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.646555 aioli_sdk-0.2.3.dev0/aioli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.646555 aioli_sdk-0.2.3.dev0/aioli/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14908 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7705 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/sso.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.646555 aioli_sdk-0.2.3.dev0/aioli/cli/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28285 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/test/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/cli/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.646555 aioli_sdk-0.2.3.dev0/aioli/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.646555 aioli_sdk-0.2.3.dev0/aioli/common/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/api/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/api/authentication.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/api/certs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/api/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/declarative_argparse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/requests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/common/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/aioli/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.654555 aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-04-29 18:41:55.000000 aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2447 2024-04-29 18:41:55.000000 aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-29 18:41:55.000000 aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-29 18:41:55.000000 aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-29 18:41:53.000000 aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-29 18:41:55.000000 aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-29 18:41:55.000000 aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.650555 aioli_sdk-0.2.3.dev0/aiolirest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3160 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.650555 aioli_sdk-0.2.3.dev0/aiolirest/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/authentication_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/deployments_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/information_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/packaged_models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54371 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/registries_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/roles_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/templates_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api/users_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/api_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:55.650555 aioli_sdk-0.2.3.dev0/aiolirest/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/auto_scaling_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/autoscaling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/configuration_resources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/deployment_model_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/deployment_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4884 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/deployment_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/error_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/event_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/failure_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/login_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/login_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/model_auth_token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/observability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6065 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/packaged_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5499 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/packaged_model_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/resource_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/resources_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/role_assignment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/role_assignments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/security.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/success_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5202 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/trained_model_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5028 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/trained_model_registry_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/user_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/models/user_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-04-29 18:41:51.000000 aioli_sdk-0.2.3.dev0/aiolirest/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-29 18:41:55.654555 aioli_sdk-0.2.3.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-04-29 18:35:44.000000 aioli_sdk-0.2.3.dev0/setup.py
```

### Comparing `aioli_sdk-0.2.2rc0/PKG-INFO` & `aioli_sdk-0.2.3.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.2rc0
+Version: 0.2.3.dev0
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/_util.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/cli.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/deployment.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/errors.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/model.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/model.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/registry.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/registry.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/render.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/render.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/role.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/sso.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/test/conftest.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/test/test_cli.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/user.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/cli/version.py` & `aioli_sdk-0.2.3.dev0/aioli/cli/version.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/api/authentication.py` & `aioli_sdk-0.2.3.dev0/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/api/certs.py` & `aioli_sdk-0.2.3.dev0/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/api/errors.py` & `aioli_sdk-0.2.3.dev0/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/api/request.py` & `aioli_sdk-0.2.3.dev0/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/check.py` & `aioli_sdk-0.2.3.dev0/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/constants.py` & `aioli_sdk-0.2.3.dev0/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/declarative_argparse.py` & `aioli_sdk-0.2.3.dev0/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/requests.py` & `aioli_sdk-0.2.3.dev0/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/common/util.py` & `aioli_sdk-0.2.3.dev0/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli/util.py` & `aioli_sdk-0.2.3.dev0/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/PKG-INFO` & `aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.2rc0
+Version: 0.2.3.dev0
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.2rc0/aioli_sdk.egg-info/SOURCES.txt` & `aioli_sdk-0.2.3.dev0/aioli_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/__init__.py` & `aioli_sdk-0.2.3.dev0/aiolirest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api/authentication_api.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api/deployments_api.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api/deployments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api/information_api.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api/information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api/packaged_models_api.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api/packaged_models_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api/registries_api.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api/registries_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api/roles_api.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api/roles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api/templates_api.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api/users_api.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api_client.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/api_response.py` & `aioli_sdk-0.2.3.dev0/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/configuration.py` & `aioli_sdk-0.2.3.dev0/aiolirest/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.2.2-rc0\n"\
+               "Version of the API: 0.2.3-dev0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/exceptions.py` & `aioli_sdk-0.2.3.dev0/aiolirest/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/__init__.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/auto_scaling_template.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/auto_scaling_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/autoscaling.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/autoscaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/configuration_resources.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/configuration_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/deployment.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/deployment_model_version.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/deployment_model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/deployment_request.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/deployment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/deployment_state.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/deployment_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/error_response.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/event_info.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/event_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/failure_info.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/failure_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/login_request.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/login_response.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/login_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/model_auth_token.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/model_auth_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/observability.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/observability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/packaged_model.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/packaged_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/packaged_model_request.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/packaged_model_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/resource_profile.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/resource_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/resources_template.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/resources_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/role.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/role_assignment.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/role_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/role_assignments.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/role_assignments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/security.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/success_response.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/success_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/trained_model_registry.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/trained_model_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/trained_model_registry_request.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/trained_model_registry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/user.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/user_patch_request.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/user_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/models/user_request.py` & `aioli_sdk-0.2.3.dev0/aiolirest/models/user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/aiolirest/rest.py` & `aioli_sdk-0.2.3.dev0/aiolirest/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.2-rc0
+    The version of the OpenAPI document: 0.2.3-dev0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.2rc0/setup.py` & `aioli_sdk-0.2.3.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.2.2-rc0",
+    version="0.2.3-dev0",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

