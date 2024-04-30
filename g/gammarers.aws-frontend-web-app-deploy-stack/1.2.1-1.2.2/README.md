# Comparing `tmp/gammarers.aws-frontend-web-app-deploy-stack-1.2.1.tar.gz` & `tmp/gammarers.aws-frontend-web-app-deploy-stack-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-frontend-web-app-deploy-stack-1.2.1.tar", last modified: Wed Apr 24 10:22:56 2024, max compression
+gzip compressed data, was "gammarers.aws-frontend-web-app-deploy-stack-1.2.2.tar", last modified: Tue Apr 30 19:13:37 2024, max compression
```

## Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1.tar` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:22:56.982319 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-24 10:22:56.982319 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:22:56.982319 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:22:56.982319 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:22:56.982319 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:22:56.982319 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/aws_frontend_web_app_deploy_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:22:56.982319 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36128 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:22:43.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:22:56.982319 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-24 10:22:56.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 10:22:56.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:22:56.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 10:22:56.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 10:22:56.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.464958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.464958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36124 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:13:26.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:13:37.468958 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 19:13:37.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1/LICENSE` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1/PKG-INFO` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-frontend-web-app-deploy-stack
-Version: 1.2.1
+Version: 1.2.2
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1/README.md` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1/setup.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-frontend-web-app-deploy-stack",
-    "version": "1.2.1",
+    "version": "1.2.2",
     "description": "This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_frontend_web_app_deploy_stack",
         "gammarers.aws_frontend_web_app_deploy_stack._jsii"
     ],
     "package_data": {
         "gammarers.aws_frontend_web_app_deploy_stack._jsii": [
-            "aws-frontend-web-app-deploy-stack@1.2.1.jsii.tgz"
+            "aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz"
         ],
         "gammarers.aws_frontend_web_app_deploy_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 import gammarers.aws_secure_cloudfront_origin_bucket._jsii
 import gammarers.aws_secure_frontend_web_app_cloudfront_distribution._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-frontend-web-app-deploy-stack",
-    "1.2.1",
+    "1.2.2",
     __name__[0:-6],
-    "aws-frontend-web-app-deploy-stack@1.2.1.jsii.tgz",
+    "aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-frontend-web-app-deploy-stack
-Version: 1.2.1
+Version: 1.2.2
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.1/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.2/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
 src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
 src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
 src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
-src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.1.jsii.tgz
+src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.2.jsii.tgz
```

