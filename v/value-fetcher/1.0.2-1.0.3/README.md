# Comparing `tmp/value_fetcher-1.0.2.tar.gz` & `tmp/value_fetcher-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "value_fetcher-1.0.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `value_fetcher-1.0.2.tar` & `value_fetcher-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-01-22 19:54:17.587999 value_fetcher-1.0.2/LICENSE
--rw-r--r--   0        0        0     3091 2023-01-22 19:54:17.587999 value_fetcher-1.0.2/README.md
--rw-r--r--   0        0        0      801 2023-01-22 19:54:17.587999 value_fetcher-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      103 2023-01-22 19:54:17.587999 value_fetcher-1.0.2/src/value_fetcher/__init__.py
--rw-r--r--   0        0        0     2885 2023-01-22 19:54:17.587999 value_fetcher-1.0.2/src/value_fetcher/aws.py
--rw-r--r--   0        0        0     4938 2023-01-22 19:54:17.587999 value_fetcher-1.0.2/src/value_fetcher/base.py
--rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 value_fetcher-1.0.2/setup.py
--rw-r--r--   0        0        0     3775 1970-01-01 00:00:00.000000 value_fetcher-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/.github/workflows/validate.yml
+-rwxr-xr-x   0        0        0      574 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/scripts/validate.sh
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/src/value_fetcher/__init__.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/src/value_fetcher/aws.py
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/src/value_fetcher/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/tests/test_aws.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/tests/test_base.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/tests/test_base_aws_parameter_store.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/tests/test_base_aws_secrets_manager.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/tests/test_base_env_vars.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/tests/utils.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/README.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 value_fetcher-1.0.3/PKG-INFO
```

### Comparing `value_fetcher-1.0.2/LICENSE` & `value_fetcher-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `value_fetcher-1.0.2/README.md` & `value_fetcher-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `value_fetcher-1.0.2/src/value_fetcher/aws.py` & `value_fetcher-1.0.3/src/value_fetcher/aws.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,77 +4,75 @@
   - Secrets Manager to fetch secret values
 """
 
 import logging
 import boto3
 import botocore
 
+
 class Aws:
     """
     Fetch parameters and send emails.
     """
+
     def __init__(self) -> None:
         # Prepare AWS clients
-        self.ssm = boto3.client('ssm')
-        self.secretsmanager = boto3.client('secretsmanager')
+        self.ssm = boto3.client("ssm")
+        self.secretsmanager = boto3.client("secretsmanager")
 
     def get_parameter_value(self, name) -> str:
         """
         Fetch encrypted parameters from Systems Manager (SSM) Parameter Store
         https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html
         """
 
         value = None
 
-        logging.debug('Fetching AWS SSM Parameter Store parameter: %s', name)
+        logging.debug("Fetching AWS SSM Parameter Store parameter: %s", name)
         try:
-            response = self.ssm.get_parameter(
-                Name=name,
-                WithDecryption=True
-            )
-            if 'Parameter' in response:
-                if 'Value' in response['Parameter']:
-                    value = response['Parameter']['Value']
+            response = self.ssm.get_parameter(Name=name, WithDecryption=True)
+            if "Parameter" in response:
+                if "Value" in response["Parameter"]:
+                    value = response["Parameter"]["Value"]
         except (
             botocore.exceptions.ClientError,
             botocore.exceptions.NoCredentialsError,
             self.ssm.exceptions.InternalServerError,
             self.ssm.exceptions.InvalidKeyId,
             self.ssm.exceptions.ParameterNotFound,
             self.ssm.exceptions.ParameterVersionNotFound,
         ) as exception:
-            logging.warning('Unable to retrieve AWS SSM Parameter value for name %s', name)
+            logging.warning("AWS SSM Parameter fetch failed: %s", name)
             logging.warning(exception)
 
         return value
 
-
     def get_secret_value(self, name) -> str:
         """
         Fetch encrypted secret from Secrets Manager
         https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html
         """
 
         value = None
-        logging.debug('Fetching AWS Secrets Manager secret: %s', name)
+        logging.debug("Fetching AWS Secrets Manager secret: %s", name)
 
         try:
             response = self.secretsmanager.get_secret_value(SecretId=name)
-            if 'SecretString' in response:
-                value = response['SecretString']
-            elif 'SecretBinary' in response:
-                value = response['SecretBinary']
+            if "SecretString" in response:
+                value = response["SecretString"]
+            elif "SecretBinary" in response:
+                value = response["SecretBinary"]
                 if isinstance(value, bytes):
-                    value = value.decode('utf-8')
+                    value = value.decode("utf-8")
         except (
             botocore.exceptions.ClientError,
             botocore.exceptions.NoCredentialsError,
             self.secretsmanager.exceptions.ResourceNotFoundException,
             self.secretsmanager.exceptions.InvalidParameterException,
             self.secretsmanager.exceptions.InvalidRequestException,
             self.secretsmanager.exceptions.DecryptionFailure,
             self.secretsmanager.exceptions.InternalServiceError,
         ) as exception:
-            logging.warning('Unable to retrieve AWS Secrets Manager value for name %s', name)
+            logging.warning("AWS Secrets Manager fetch failed: %s", name)
             logging.warning(exception)
 
         return value
```

### Comparing `value_fetcher-1.0.2/src/value_fetcher/base.py` & `value_fetcher-1.0.3/src/value_fetcher/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,132 +10,133 @@
 from .aws import Aws
 
 
 class ValueFetcher:
     """
     Configuration provider class
     """
+
     def __init__(self, env_defaults: dict = None) -> None:
         self.env_defaults = env_defaults
 
     def get(self, key: str) -> str:
         """
         Given a key name MY_VAL, check for a source env var e.g. MY_VAL_SOURCE.
         Raises exception if source does not match list of known services.
         """
         # Make the provided name all-uppercase
         key = key.upper()
 
         if not isinstance(key, str) or len(key) == 0:
-            message = 'Invalid key name provided'
+            message = "Invalid key name provided"
             logging.critical(message)
             logging.critical(key)
             raise ValueError(message)
 
-        logging.debug('Retrieving value for key %s', key)
-        source = os.environ.get(f'{key}_SOURCE', 'env').lower()
-        logging.debug('%s source: %s', key, source)
+        logging.debug("Retrieving value for key %s", key)
+        source = os.environ.get(f"{key}_SOURCE", "env").lower()
+        logging.debug("%s source: %s", key, source)
         # Get value from environment variable
-        if source == 'env':
+        if source == "env":
             return self.get_from_env(key)
 
         # Get value from AWS SSM parameter store
-        if source == 'aws_ssm_parameter_store':
+        if source == "aws_ssm_parameter_store":
             return self.get_from_aws_ssm_parameter_store(key)
 
         # Get value from AWS Secrets Manager
-        if source == 'aws_secrets_manager':
+        if source == "aws_secrets_manager":
             return self.get_from_aws_secrets_manager(key)
 
-        message = f'Unknown source {source}'
+        message = f"Unknown source {source}"
         logging.critical(message)
         raise ValueError(message)
 
-
     def get_from_env(self, key) -> str:
         """
         Fetch a value from environment variables, using a default if available.
         If value is empty and cannot be found in defaults, raise exception.
         """
 
         if not isinstance(key, str) or len(key) == 0:
-            message = 'Missing or empty environment key'
+            message = "Missing or empty environment key"
             logging.critical(message)
             logging.critical(key)
             raise ValueError(message)
 
-        logging.debug('Checking environment for key: %s', key)
-        value = os.environ.get(key, '').strip()
+        logging.debug("Checking environment for key: %s", key)
+        value = os.environ.get(key, "").strip()
         if not isinstance(value, str) or len(value) == 0:
-            if isinstance(self.env_defaults, dict) and key in self.env_defaults:
-                logging.debug('Using default value for environment variable: %s', key)
-                value = self.env_defaults[key]
+            defaults = self.env_defaults
+            if isinstance(defaults, dict) and key in defaults:
+                logging.debug("Using default value for env var: %s", key)
+                value = defaults[key]
             else:
-                message = f'Missing or empty environment value for {key}'
+                message = f"Missing or empty environment value for {key}"
                 logging.critical(message)
                 raise ValueError(message)
 
         return value
 
-
     def get_from_aws_ssm_parameter_store(self, key: str) -> str:
         """
         Fetch a value from AWS SSM Parameter store.
-        If the parameter name is not configured by an environment variable, try the provided key.
+        If the parameter name is not configured by an environment variable,
+        try the provided key.
         """
 
         if not isinstance(key, str) or len(key) == 0:
-            message = 'Missing or empty AWS SSM Parameter Store key'
+            message = "Missing or empty AWS SSM Parameter Store key"
             logging.critical(message)
             raise ValueError(message)
 
-        name_key = f'{key}_PARAMETER_STORE_NAME'
+        name_key = f"{key}_PARAMETER_STORE_NAME"
 
-        logging.debug('Checking environment for AWS SSM Parameter name: %s', name_key)
+        logging.debug("Checking env for AWS SSM Parameter %s", name_key)
         try:
             name = self.get_from_env(name_key)
-            logging.debug('Using parameter name %s', name)
+            logging.debug("Using parameter name %s", name)
         except ValueError as exception:
             logging.debug(exception)
-            logging.debug('Using key name for parameter %s', key)
+            logging.debug("Using key name for parameter %s", key)
             name = key
 
         aws = Aws()
         value = aws.get_parameter_value(name)
         if not isinstance(value, str) or len(value) == 0:
-            message = f'Missing or empty AWS SSM Parameter Store value for {name}'
+            message = f"Missing or empty AWS SSM Parameter Store {name}"
             logging.critical(message)
             raise ValueError(message)
 
         return value
 
-
     def get_from_aws_secrets_manager(self, key: str) -> str:
         """
         Fetch a value from AWS Secrets Manager.
-        If the secret name is not configured by an environment variable, use the key directly.
+        If the secret name is not configured by an environment variable,
+        use the key directly.
         """
 
         if not isinstance(key, str) or len(key) == 0:
-            message = 'Missing or empty AWS Secrets Manager key'
+            message = "Missing or empty AWS Secrets Manager key"
             logging.critical(message)
             raise ValueError(message)
 
-        name_key = f'{key}_SECRETS_MANAGER_NAME'
+        name_key = f"{key}_SECRETS_MANAGER_NAME"
 
-        logging.debug('Checking environment for AWS Secret Manager name: %s', name_key)
+        logging.debug("Checking env for AWS Secret Manager %s", name_key)
         try:
             name = self.get_from_env(name_key)
-            logging.debug('Using secret name %s', name)
+            logging.debug("Using secret name %s", name)
         except ValueError as exception:
             logging.debug(exception)
-            logging.debug('Using key name for secret %s', key)
+            logging.debug("Using key name for secret %s", key)
             name = key
 
         aws = Aws()
         value = aws.get_secret_value(name)
         if not isinstance(value, str) or len(value) == 0:
-            message = f'Missing or empty AWS Secrets Manager value for {name}'
+            message = f"Missing or empty AWS Secrets Manager value for {name}"
             logging.critical(message)
             raise ValueError(message)
 
         return value
```

### Comparing `value_fetcher-1.0.2/setup.py` & `value_fetcher-1.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,116 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-package_dir = \
-{'': 'src'}
-
-packages = \
-['value_fetcher']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['boto3>=1.26.27,<2.0.0', 'pyyaml>=6.0,<7.0']
-
-setup_kwargs = {
-    'name': 'value-fetcher',
-    'version': '1.0.2',
-    'description': 'Fetch a value from various sources, e.g AWS Secrets Manager and SSM Parameter Store',
-    'long_description': '# Value fetcher\n## Introduction\nPython module to fetch values from multiple sources with optional defaults, including:\n- Environment variables\n- AWS Systems Manager (SSM) Parameter Store\n- AWS Secrets Manager\n\n## Usage\nInstall the package with the following:\n\n```shell\npip install value-fetcher\n```\n\n### Fetching values directly\nIn this use case, the value fetcher package makes it convenient to fetch values from the supported sources in a consistent and simplified manner.\n```python\nfrom value_fetcher import ValueFetcher\n\n# Instantiate value fetcher class\nfetcher = ValueFetcher()\n\n# Retrieve values from supported AWS sources\nmy_secret = fetcher.get_from_aws_secrets_manager(\'/my/secret/key\')\nmy_param = fetcher.get_from_aws_ssm_parameter_store(\'/my/parameter/key\')\n```\n\n### Configuring source locations dynamically\nIn this use case, environment variables are used to configure the sources for multiple keys.\nThis is useful in more complex applications where lots of values need to be fetched and the source needs to be configured dynamically.\nSee this [contact form handler repository](https://github.com/voquis/aws-lambda-contact-form-handler) for example usage.\n\nEnvironment variables can be appended to the configuration key name, setting the source of the value.\nThese are:\n- `_PARAMETER_STORE_NAME` - for AWS SSM Parameter Store\n- `_SECRETS_MANAGER_NAME` - for AWS Secrets Manager\n\nOne of the available configuration sources for each value must also be set by setting an environment variable ending with `_SOURCE` for the value name:\n- `env` - Environment variables (default)\n- `aws_ssm_parameter_store` - AWS Systems Manager (SSM) Parameter Store\n- `aws_secrets_manager` - AWS Secrets Manager\n\nFor example, to fetch `MY_PARAM` from AWS SSM Parameter Store and `MY_SECRET` from AWS Secrets Manager, consider the following python script (e.g. `app.py`) called subsequently by a shell script:\n\n```python\n# This file is app.py for example\nfrom value_fetcher import ValueFetcher\n\n# Instantiate value fetcher class, with optional defaults if values cannot be found\nfetcher = ValueFetcher({\n    \'MY_PARAM\': \'Default value if none can be found\',\n})\n\n# Retrieve values from supported AWS sources\nmy_secret = fetcher.get(\'MY_SECRET\')\nmy_param = fetcher.get(\'MY_PARAM\')\n\nprint(my_secret)\nprint(my_param)\n```\n\nThe above scripts would be called by the following shell script:\n```shell\n#!/usr/bin/bash\nMY_PARAM_SOURCE="aws_ssm_parameter_store"\nMY_PARAM_PARAMETER_STORE_NAME="/my/parameter/store/key/name"\n\nMY_SECRET_SOURCE="aws_secrets_manager"\nMY_SECRET_SECRETS_MANAGER_NAME="my/secrets/manager/key/name"\n\nexport MY_PARAM_SOURCE MY_PARAM_PARAMETER_STORE_NAME\nexport MY_SECRET_SOURCE MY_SECRET_SECRETS_MANAGER_NAME\n\n# For AWS ensure credentials are available, e.g. with AWS SSO, aws-vault, aws-profile etc.\npython app.py\n```\n\n## Development\nThis project uses Poetry for package management.\nAfter cloning, run:\n```\n./scripts/poetry.sh\n```\nto install dependencies for local development and running tests, etc.\n### Tests\n\nTo run static code analysers and unit tests:\n```\n./scripts/validate.sh\n```\n',
-    'author': 'Voquis Limited',
-    'author_email': 'opensource@voquis.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/voquis/value-fetcher',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.11,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.3
+Name: value-fetcher
+Version: 1.0.3
+Summary: Fetch a value from various sources, e.g AWS Secrets Manager and SSM Parameter Store
+Project-URL: Homepage, https://github.com/voquis/value-fetcher
+Project-URL: Issues, https://github.com/voquis/value-fetcher/issues
+Author-email: Voquis Limited <opensource@voquis.com>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: configuration,parameters,secrets,values
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Requires-Dist: boto3
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: moto; extra == 'dev'
+Requires-Dist: pylint; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
+Description-Content-Type: text/markdown
+
+# Value fetcher
+## Introduction
+Python module to fetch values from multiple sources with optional defaults, including:
+- Environment variables
+- AWS Systems Manager (SSM) Parameter Store
+- AWS Secrets Manager
+
+## Usage
+Install the package with the following:
+
+```shell
+pip install value-fetcher
+```
+
+### Fetching values directly
+In this use case, the value fetcher package makes it convenient to fetch values from the supported sources in a consistent and simplified manner.
+```python
+from value_fetcher import ValueFetcher
+
+# Instantiate value fetcher class
+fetcher = ValueFetcher()
+
+# Retrieve values from supported AWS sources
+my_secret = fetcher.get_from_aws_secrets_manager('/my/secret/key')
+my_param = fetcher.get_from_aws_ssm_parameter_store('/my/parameter/key')
+```
+
+### Configuring source locations dynamically
+In this use case, environment variables are used to configure the sources for multiple keys.
+This is useful in more complex applications where lots of values need to be fetched and the source needs to be configured dynamically.
+See this [contact form handler repository](https://github.com/voquis/aws-lambda-contact-form-handler) for example usage.
+
+Environment variables can be appended to the configuration key name, setting the source of the value.
+These are:
+- `_PARAMETER_STORE_NAME` - for AWS SSM Parameter Store
+- `_SECRETS_MANAGER_NAME` - for AWS Secrets Manager
+
+One of the available configuration sources for each value must also be set by setting an environment variable ending with `_SOURCE` for the value name:
+- `env` - Environment variables (default)
+- `aws_ssm_parameter_store` - AWS Systems Manager (SSM) Parameter Store
+- `aws_secrets_manager` - AWS Secrets Manager
+
+For example, to fetch `MY_PARAM` from AWS SSM Parameter Store and `MY_SECRET` from AWS Secrets Manager, consider the following python script (e.g. `app.py`) called subsequently by a shell script:
+
+```python
+# This file is app.py for example
+from value_fetcher import ValueFetcher
+
+# Instantiate value fetcher class, with optional defaults if values cannot be found
+fetcher = ValueFetcher({
+    'MY_PARAM': 'Default value if none can be found',
+})
+
+# Retrieve values from supported AWS sources
+my_secret = fetcher.get('MY_SECRET')
+my_param = fetcher.get('MY_PARAM')
+
+print(my_secret)
+print(my_param)
+```
+
+The above scripts would be called by the following shell script:
+```shell
+#!/usr/bin/bash
+MY_PARAM_SOURCE="aws_ssm_parameter_store"
+MY_PARAM_PARAMETER_STORE_NAME="/my/parameter/store/key/name"
+
+MY_SECRET_SOURCE="aws_secrets_manager"
+MY_SECRET_SECRETS_MANAGER_NAME="my/secrets/manager/key/name"
+
+export MY_PARAM_SOURCE MY_PARAM_PARAMETER_STORE_NAME
+export MY_SECRET_SOURCE MY_SECRET_SECRETS_MANAGER_NAME
+
+# For AWS ensure credentials are available, e.g. with AWS SSO, aws-vault, aws-profile etc.
+python app.py
+```
+
+## Development
+This project uses Poetry for package management.
+After cloning, run:
+```
+./scripts/poetry.sh
+```
+to install dependencies for local development and running tests, etc.
+### Tests
+
+To run static code analysers and unit tests:
+```
+./scripts/validate.sh
+```
```

