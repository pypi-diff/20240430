# Comparing `tmp/deploy-time-build-0.3.19.tar.gz` & `tmp/deploy-time-build-0.3.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploy-time-build-0.3.19.tar", last modified: Fri Apr 26 15:25:25 2024, max compression
+gzip compressed data, was "deploy-time-build-0.3.20.tar", last modified: Tue Apr 30 13:57:31 2024, max compression
```

## Comparing `deploy-time-build-0.3.19.tar` & `deploy-time-build-0.3.20.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:25:25.437469 deploy-time-build-0.3.19/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-04-26 15:25:25.437469 deploy-time-build-0.3.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:25:25.437469 deploy-time-build-0.3.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:25:25.433469 deploy-time-build-0.3.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:25:25.433469 deploy-time-build-0.3.19/src/deploy_time_build/
--rw-r--r--   0 runner    (1001) docker     (127)    62190 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/src/deploy_time_build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:25:25.437469 deploy-time-build-0.3.19/src/deploy_time_build/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/src/deploy_time_build/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   334704 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/src/deploy_time_build/_jsii/deploy-time-build@0.3.19.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:25:15.000000 deploy-time-build-0.3.19/src/deploy_time_build/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:25:25.433469 deploy-time-build-0.3.19/src/deploy_time_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-04-26 15:25:25.000000 deploy-time-build-0.3.19/src/deploy_time_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-26 15:25:25.000000 deploy-time-build-0.3.19/src/deploy_time_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:25:25.000000 deploy-time-build-0.3.19/src/deploy_time_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 15:25:25.000000 deploy-time-build-0.3.19/src/deploy_time_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 15:25:25.000000 deploy-time-build-0.3.19/src/deploy_time_build.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:57:31.330385 deploy-time-build-0.3.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-30 13:57:31.330385 deploy-time-build-0.3.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:57:31.330385 deploy-time-build-0.3.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:57:31.326385 deploy-time-build-0.3.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:57:31.330385 deploy-time-build-0.3.20/src/deploy_time_build/
+-rw-r--r--   0 runner    (1001) docker     (127)    62230 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/src/deploy_time_build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:57:31.330385 deploy-time-build-0.3.20/src/deploy_time_build/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/src/deploy_time_build/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   334730 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/src/deploy_time_build/_jsii/deploy-time-build@0.3.20.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:57:20.000000 deploy-time-build-0.3.20/src/deploy_time_build/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:57:31.330385 deploy-time-build-0.3.20/src/deploy_time_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-30 13:57:31.000000 deploy-time-build-0.3.20/src/deploy_time_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-30 13:57:31.000000 deploy-time-build-0.3.20/src/deploy_time_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:57:31.000000 deploy-time-build-0.3.20/src/deploy_time_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 13:57:31.000000 deploy-time-build-0.3.20/src/deploy_time_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 13:57:31.000000 deploy-time-build-0.3.20/src/deploy_time_build.egg-info/top_level.txt
```

### Comparing `deploy-time-build-0.3.19/LICENSE` & `deploy-time-build-0.3.20/LICENSE`

 * *Files identical despite different names*

### Comparing `deploy-time-build-0.3.19/PKG-INFO` & `deploy-time-build-0.3.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploy-time-build
-Version: 0.3.19
+Version: 0.3.20
 Summary: Build during CDK deployment.
 Home-page: https://github.com/tmokmss/deploy-time-build.git
 Author: tmokmss<tomookam@live.jp>
 License: MIT
 Project-URL: Source, https://github.com/tmokmss/deploy-time-build.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -171,15 +171,15 @@
 new FargateTaskDefinition(this, 'TaskDefinition', {
     runtimePlatform: { cpuArchitecture: CpuArchitecture.ARM64 }
 }).addContainer('main', {
     image: armImage.toEcsDockerImageCode(),
 });
 ```
 
-The third argument (props) are the super set of DockerImageAsset's properties. You can additionally set `tag` and `repository`.
+The third argument (props) are a superset of DockerImageAsset's properties. You can set a few additional properties such as `tag`, `repository`, and `zstdCompression`.
 
 ### Build SOCI index for a container image
 
 [Seekable OCI (SOCI)](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/) is a way to help start tasks faster for Amazon ECS tasks on Fargate 1.4.0. You can build and push a SOCI index using the `SociIndexBuild` construct.
 
 ![soci-architecture](imgs/soci-architecture.png)
```

### Comparing `deploy-time-build-0.3.19/README.md` & `deploy-time-build-0.3.20/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 new FargateTaskDefinition(this, 'TaskDefinition', {
     runtimePlatform: { cpuArchitecture: CpuArchitecture.ARM64 }
 }).addContainer('main', {
     image: armImage.toEcsDockerImageCode(),
 });
 ```
 
-The third argument (props) are the super set of DockerImageAsset's properties. You can additionally set `tag` and `repository`.
+The third argument (props) are a superset of DockerImageAsset's properties. You can set a few additional properties such as `tag`, `repository`, and `zstdCompression`.
 
 ### Build SOCI index for a container image
 
 [Seekable OCI (SOCI)](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/) is a way to help start tasks faster for Amazon ECS tasks on Fargate 1.4.0. You can build and push a SOCI index using the `SociIndexBuild` construct.
 
 ![soci-architecture](imgs/soci-architecture.png)
```

### Comparing `deploy-time-build-0.3.19/setup.py` & `deploy-time-build-0.3.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "deploy-time-build",
-    "version": "0.3.19",
+    "version": "0.3.20",
     "description": "Build during CDK deployment.",
     "license": "MIT",
     "url": "https://github.com/tmokmss/deploy-time-build.git",
     "long_description_content_type": "text/markdown",
     "author": "tmokmss<tomookam@live.jp>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "deploy_time_build",
         "deploy_time_build._jsii"
     ],
     "package_data": {
         "deploy_time_build._jsii": [
-            "deploy-time-build@0.3.19.jsii.tgz"
+            "deploy-time-build@0.3.20.jsii.tgz"
         ],
         "deploy_time_build": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `deploy-time-build-0.3.19/src/deploy_time_build/__init__.py` & `deploy-time-build-0.3.20/src/deploy_time_build/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 new FargateTaskDefinition(this, 'TaskDefinition', {
     runtimePlatform: { cpuArchitecture: CpuArchitecture.ARM64 }
 }).addContainer('main', {
     image: armImage.toEcsDockerImageCode(),
 });
 ```
 
-The third argument (props) are the super set of DockerImageAsset's properties. You can additionally set `tag` and `repository`.
+The third argument (props) are a superset of DockerImageAsset's properties. You can set a few additional properties such as `tag`, `repository`, and `zstdCompression`.
 
 ### Build SOCI index for a container image
 
 [Seekable OCI (SOCI)](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/) is a way to help start tasks faster for Amazon ECS tasks on Fargate 1.4.0. You can build and push a SOCI index using the `SociIndexBuild` construct.
 
 ![soci-architecture](imgs/soci-architecture.png)
```

### Comparing `deploy-time-build-0.3.19/src/deploy_time_build.egg-info/PKG-INFO` & `deploy-time-build-0.3.20/src/deploy_time_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploy-time-build
-Version: 0.3.19
+Version: 0.3.20
 Summary: Build during CDK deployment.
 Home-page: https://github.com/tmokmss/deploy-time-build.git
 Author: tmokmss<tomookam@live.jp>
 License: MIT
 Project-URL: Source, https://github.com/tmokmss/deploy-time-build.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -171,15 +171,15 @@
 new FargateTaskDefinition(this, 'TaskDefinition', {
     runtimePlatform: { cpuArchitecture: CpuArchitecture.ARM64 }
 }).addContainer('main', {
     image: armImage.toEcsDockerImageCode(),
 });
 ```
 
-The third argument (props) are the super set of DockerImageAsset's properties. You can additionally set `tag` and `repository`.
+The third argument (props) are a superset of DockerImageAsset's properties. You can set a few additional properties such as `tag`, `repository`, and `zstdCompression`.
 
 ### Build SOCI index for a container image
 
 [Seekable OCI (SOCI)](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/) is a way to help start tasks faster for Amazon ECS tasks on Fargate 1.4.0. You can build and push a SOCI index using the `SociIndexBuild` construct.
 
 ![soci-architecture](imgs/soci-architecture.png)
```

