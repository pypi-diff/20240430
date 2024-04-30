# Comparing `tmp/cdk-sops-secrets-1.6.9.tar.gz` & `tmp/cdk-sops-secrets-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.6.9.tar", last modified: Thu Feb 29 06:13:44 2024, max compression
+gzip compressed data, was "cdk-sops-secrets-1.7.0.tar", last modified: Mon Apr 29 12:41:26 2024, max compression
```

## Comparing `cdk-sops-secrets-1.6.9.tar` & `cdk-sops-secrets-1.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:13:44.660661 cdk-sops-secrets-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-02-29 06:13:44.660661 cdk-sops-secrets-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 06:13:44.660661 cdk-sops-secrets-1.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:13:44.648661 cdk-sops-secrets-1.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:13:44.648661 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)    76283 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:13:44.648661 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  8962620 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.6.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 06:13:33.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:13:44.648661 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-02-29 06:13:44.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-29 06:13:44.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 06:13:44.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-29 06:13:44.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 06:13:44.000000 cdk-sops-secrets-1.6.9/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:41:26.517570 cdk-sops-secrets-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-29 12:41:26.517570 cdk-sops-secrets-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:41:26.517570 cdk-sops-secrets-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:41:26.505570 cdk-sops-secrets-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:41:26.505570 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76606 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:41:26.505570 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  8963934 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.7.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:41:14.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:41:26.505570 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-29 12:41:26.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-29 12:41:26.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:41:26.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-29 12:41:26.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 12:41:26.000000 cdk-sops-secrets-1.7.0/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.6.9/LICENSE` & `cdk-sops-secrets-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.6.9/PKG-INFO` & `cdk-sops-secrets-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.6.9
+Version: 1.7.0
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -151,14 +151,24 @@
 
 ### It does not work, what can I do?
 
 Even if this construct has some unit and integration tests performed, there can be bugs and issues. As everything is performed by a cloudformation custom resource provider, a good starting point is the log of the corresponding lambda function. It should be located in your AWS Account under Cloudwatch -> Log groups:
 
 `/aws/lambda/<YOUR-STACK-NAME>-SingletonLambdaSopsSyncProvider<SOMETHINGsomething1234>`
 
+### I get errors with dotenv formatted files
+
+Only very basic dotenv syntax is working right now. Only single line values are accepted. The format must match:
+
+```dotenv
+key=value
+```
+
+comments must be a single line, not after value assignments.
+
 ### Error getting data key: 0 successful groups required, got 0
 
 This error message (and failed sync) is related to the  mozilla/sops issues [#948](https://github.com/mozilla/sops/issues/948) and [#634](https://github.com/mozilla/sops/issues/634). You must not create your secret with the `--aws-profile` flag. This profile will be written to your sops filed and is required in every runtime environment. You have to define the profile to use via the environment variable `AWS_PROFILE` instead, to avoid this.
 
 ### Asset of sync lambda not found
 
 The lambda asset code is generated relative to the path of the index.ts in this package. With tools like nx this can lead to wrong results, so that the asset could not be found.
```

### Comparing `cdk-sops-secrets-1.6.9/README.md` & `cdk-sops-secrets-1.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -128,14 +128,24 @@
 
 ### It does not work, what can I do?
 
 Even if this construct has some unit and integration tests performed, there can be bugs and issues. As everything is performed by a cloudformation custom resource provider, a good starting point is the log of the corresponding lambda function. It should be located in your AWS Account under Cloudwatch -> Log groups:
 
 `/aws/lambda/<YOUR-STACK-NAME>-SingletonLambdaSopsSyncProvider<SOMETHINGsomething1234>`
 
+### I get errors with dotenv formatted files
+
+Only very basic dotenv syntax is working right now. Only single line values are accepted. The format must match:
+
+```dotenv
+key=value
+```
+
+comments must be a single line, not after value assignments.
+
 ### Error getting data key: 0 successful groups required, got 0
 
 This error message (and failed sync) is related to the  mozilla/sops issues [#948](https://github.com/mozilla/sops/issues/948) and [#634](https://github.com/mozilla/sops/issues/634). You must not create your secret with the `--aws-profile` flag. This profile will be written to your sops filed and is required in every runtime environment. You have to define the profile to use via the environment variable `AWS_PROFILE` instead, to avoid this.
 
 ### Asset of sync lambda not found
 
 The lambda asset code is generated relative to the path of the index.ts in this package. With tools like nx this can lead to wrong results, so that the asset could not be found.
```

### Comparing `cdk-sops-secrets-1.6.9/setup.py` & `cdk-sops-secrets-1.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.6.9",
+    "version": "1.7.0",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<markus.siebert@deutschebahn.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.6.9.jsii.tgz"
+            "cdk-sops-secrets@1.7.0.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.1.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.94.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-sops-secrets-1.6.9/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.7.0/src/cdk_sops_secrets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,24 @@
 
 ### It does not work, what can I do?
 
 Even if this construct has some unit and integration tests performed, there can be bugs and issues. As everything is performed by a cloudformation custom resource provider, a good starting point is the log of the corresponding lambda function. It should be located in your AWS Account under Cloudwatch -> Log groups:
 
 `/aws/lambda/<YOUR-STACK-NAME>-SingletonLambdaSopsSyncProvider<SOMETHINGsomething1234>`
 
+### I get errors with dotenv formatted files
+
+Only very basic dotenv syntax is working right now. Only single line values are accepted. The format must match:
+
+```dotenv
+key=value
+```
+
+comments must be a single line, not after value assignments.
+
 ### Error getting data key: 0 successful groups required, got 0
 
 This error message (and failed sync) is related to the  mozilla/sops issues [#948](https://github.com/mozilla/sops/issues/948) and [#634](https://github.com/mozilla/sops/issues/634). You must not create your secret with the `--aws-profile` flag. This profile will be written to your sops filed and is required in every runtime environment. You have to define the profile to use via the environment variable `AWS_PROFILE` instead, to avoid this.
 
 ### Asset of sync lambda not found
 
 The lambda asset code is generated relative to the path of the index.ts in this package. With tools like nx this can lead to wrong results, so that the asset could not be found.
@@ -183,14 +193,17 @@
 * [isotoma/sops-secretsmanager-cdk](https://github.com/isotoma/sops-secretsmanager-cdk): Does nearly the same. Uses CustomResource, wraps the sops CLI, does not support flatten. Found it after I published my solution to NPM :-/
 * [taimos/secretsmanager-versioning](https://github.com/taimos/secretsmanager-versioning): Different approach on the same problem. This is a CLI tool with very nice integration into CDK and also handles git versioning information.
 
 ## License
 
 The Apache-2.0 license. Please have a look at the [LICENSE](LICENSE) and [LICENSE-3RD-PARTY](LICENSE-3RD-PARTY).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cdk-sops-secrets-1.6.9/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.7.0/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.6.9
+Version: 1.7.0
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -151,14 +151,24 @@
 
 ### It does not work, what can I do?
 
 Even if this construct has some unit and integration tests performed, there can be bugs and issues. As everything is performed by a cloudformation custom resource provider, a good starting point is the log of the corresponding lambda function. It should be located in your AWS Account under Cloudwatch -> Log groups:
 
 `/aws/lambda/<YOUR-STACK-NAME>-SingletonLambdaSopsSyncProvider<SOMETHINGsomething1234>`
 
+### I get errors with dotenv formatted files
+
+Only very basic dotenv syntax is working right now. Only single line values are accepted. The format must match:
+
+```dotenv
+key=value
+```
+
+comments must be a single line, not after value assignments.
+
 ### Error getting data key: 0 successful groups required, got 0
 
 This error message (and failed sync) is related to the  mozilla/sops issues [#948](https://github.com/mozilla/sops/issues/948) and [#634](https://github.com/mozilla/sops/issues/634). You must not create your secret with the `--aws-profile` flag. This profile will be written to your sops filed and is required in every runtime environment. You have to define the profile to use via the environment variable `AWS_PROFILE` instead, to avoid this.
 
 ### Asset of sync lambda not found
 
 The lambda asset code is generated relative to the path of the index.ts in this package. With tools like nx this can lead to wrong results, so that the asset could not be found.
```

