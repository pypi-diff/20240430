# Comparing `tmp/inoopa_utils-2.9.7.tar.gz` & `tmp/inoopa_utils-2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inoopa_utils-2.9.7.tar", max compression
+gzip compressed data, was "inoopa_utils-2.9.8.tar", max compression
```

## Comparing `inoopa_utils-2.9.7.tar` & `inoopa_utils-2.9.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      953 2024-03-11 12:17:35.204315 inoopa_utils-2.9.7/README.md
--rw-r--r--   0        0        0        0 2024-04-22 08:46:46.594963 inoopa_utils-2.9.7/inoopa_utils/__init__.py
--rw-r--r--   0        0        0     1781 2024-03-08 11:42:35.645264 inoopa_utils-2.9.7/inoopa_utils/address_parser.py
--rw-r--r--   0        0        0     6238 2024-03-08 11:42:34.540729 inoopa_utils-2.9.7/inoopa_utils/batch_processing.py
--rw-r--r--   0        0        0        0 2024-03-08 11:43:03.997156 inoopa_utils-2.9.7/inoopa_utils/custom_types/__init__.py
--rw-r--r--   0        0        0     9103 2024-04-29 14:08:17.458618 inoopa_utils-2.9.7/inoopa_utils/custom_types/companies.py
--rw-r--r--   0        0        0      801 2024-03-08 11:43:06.928124 inoopa_utils-2.9.7/inoopa_utils/custom_types/decision_makers.py
--rw-r--r--   0        0        0      117 2024-03-08 11:43:11.918631 inoopa_utils-2.9.7/inoopa_utils/custom_types/exceptions.py
--rw-r--r--   0        0        0     2352 2024-04-26 10:34:01.198648 inoopa_utils-2.9.7/inoopa_utils/custom_types/typesense_schemas.py
--rw-r--r--   0        0        0      358 2024-03-08 11:43:09.416778 inoopa_utils-2.9.7/inoopa_utils/custom_types/websites.py
--rw-r--r--   0        0        0     1720 2024-03-08 11:42:33.437130 inoopa_utils-2.9.7/inoopa_utils/inoopa_logging.py
--rw-r--r--   0        0        0    16195 2024-03-08 11:42:26.507548 inoopa_utils-2.9.7/inoopa_utils/mongodb_helpers.py
--rw-r--r--   0        0        0     3207 2024-03-27 14:28:43.391739 inoopa_utils-2.9.7/inoopa_utils/openai_helpers.py
--rw-r--r--   0        0        0     4243 2024-03-08 11:42:32.029627 inoopa_utils-2.9.7/inoopa_utils/rabbitmq_helpers.py
--rw-r--r--   0        0        0     4871 2024-03-08 11:42:30.821464 inoopa_utils-2.9.7/inoopa_utils/sql_helpers.py
--rw-r--r--   0        0        0      427 2023-11-06 09:54:38.711474 inoopa_utils-2.9.7/inoopa_utils/tests/test_logging.py
--rw-r--r--   0        0        0      627 2023-11-06 12:56:31.343962 inoopa_utils-2.9.7/inoopa_utils/tests/test_rabbitmq.py
--rw-r--r--   0        0        0    11383 2024-04-26 10:43:04.588471 inoopa_utils-2.9.7/inoopa_utils/typesense_helpers.py
--rw-r--r--   0        0        0        0 2023-11-06 00:28:42.240779 inoopa_utils-2.9.7/inoopa_utils/utils/__init__.py
--rw-r--r--   0        0        0      368 2024-03-08 11:43:44.438533 inoopa_utils-2.9.7/inoopa_utils/utils/env_variables_helper.py
--rw-r--r--   0        0        0      144 2024-03-08 11:43:22.052184 inoopa_utils-2.9.7/inoopa_utils/utils/exceptions.py
--rw-r--r--   0        0        0      663 2024-04-30 14:17:06.269687 inoopa_utils-2.9.7/pyproject.toml
--rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 inoopa_utils-2.9.7/PKG-INFO
+-rw-r--r--   0        0        0      953 2024-03-11 12:17:35.204315 inoopa_utils-2.9.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 08:46:46.594963 inoopa_utils-2.9.8/inoopa_utils/__init__.py
+-rw-r--r--   0        0        0     1781 2024-03-08 11:42:35.645264 inoopa_utils-2.9.8/inoopa_utils/address_parser.py
+-rw-r--r--   0        0        0     6238 2024-03-08 11:42:34.540729 inoopa_utils-2.9.8/inoopa_utils/batch_processing.py
+-rw-r--r--   0        0        0        0 2024-03-08 11:43:03.997156 inoopa_utils-2.9.8/inoopa_utils/custom_types/__init__.py
+-rw-r--r--   0        0        0     9103 2024-04-29 14:08:17.458618 inoopa_utils-2.9.8/inoopa_utils/custom_types/companies.py
+-rw-r--r--   0        0        0      801 2024-03-08 11:43:06.928124 inoopa_utils-2.9.8/inoopa_utils/custom_types/decision_makers.py
+-rw-r--r--   0        0        0      117 2024-03-08 11:43:11.918631 inoopa_utils-2.9.8/inoopa_utils/custom_types/exceptions.py
+-rw-r--r--   0        0        0     2352 2024-04-26 10:34:01.198648 inoopa_utils-2.9.8/inoopa_utils/custom_types/typesense_schemas.py
+-rw-r--r--   0        0        0      358 2024-03-08 11:43:09.416778 inoopa_utils-2.9.8/inoopa_utils/custom_types/websites.py
+-rw-r--r--   0        0        0     1720 2024-03-08 11:42:33.437130 inoopa_utils-2.9.8/inoopa_utils/inoopa_logging.py
+-rw-r--r--   0        0        0    16195 2024-03-08 11:42:26.507548 inoopa_utils-2.9.8/inoopa_utils/mongodb_helpers.py
+-rw-r--r--   0        0        0     3207 2024-03-27 14:28:43.391739 inoopa_utils-2.9.8/inoopa_utils/openai_helpers.py
+-rw-r--r--   0        0        0     4243 2024-03-08 11:42:32.029627 inoopa_utils-2.9.8/inoopa_utils/rabbitmq_helpers.py
+-rw-r--r--   0        0        0     4871 2024-03-08 11:42:30.821464 inoopa_utils-2.9.8/inoopa_utils/sql_helpers.py
+-rw-r--r--   0        0        0      427 2023-11-06 09:54:38.711474 inoopa_utils-2.9.8/inoopa_utils/tests/test_logging.py
+-rw-r--r--   0        0        0      627 2023-11-06 12:56:31.343962 inoopa_utils-2.9.8/inoopa_utils/tests/test_rabbitmq.py
+-rw-r--r--   0        0        0    11383 2024-04-26 10:43:04.588471 inoopa_utils-2.9.8/inoopa_utils/typesense_helpers.py
+-rw-r--r--   0        0        0        0 2023-11-06 00:28:42.240779 inoopa_utils-2.9.8/inoopa_utils/utils/__init__.py
+-rw-r--r--   0        0        0      368 2024-03-08 11:43:44.438533 inoopa_utils-2.9.8/inoopa_utils/utils/env_variables_helper.py
+-rw-r--r--   0        0        0      144 2024-03-08 11:43:22.052184 inoopa_utils-2.9.8/inoopa_utils/utils/exceptions.py
+-rw-r--r--   0        0        0      664 2024-04-30 14:19:44.219766 inoopa_utils-2.9.8/pyproject.toml
+-rw-r--r--   0        0        0     2015 1970-01-01 00:00:00.000000 inoopa_utils-2.9.8/PKG-INFO
```

### Comparing `inoopa_utils-2.9.7/README.md` & `inoopa_utils-2.9.8/README.md`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/address_parser.py` & `inoopa_utils-2.9.8/inoopa_utils/address_parser.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/batch_processing.py` & `inoopa_utils-2.9.8/inoopa_utils/batch_processing.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/custom_types/companies.py` & `inoopa_utils-2.9.8/inoopa_utils/custom_types/companies.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/custom_types/decision_makers.py` & `inoopa_utils-2.9.8/inoopa_utils/custom_types/decision_makers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/custom_types/typesense_schemas.py` & `inoopa_utils-2.9.8/inoopa_utils/custom_types/typesense_schemas.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/inoopa_logging.py` & `inoopa_utils-2.9.8/inoopa_utils/inoopa_logging.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/mongodb_helpers.py` & `inoopa_utils-2.9.8/inoopa_utils/mongodb_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/openai_helpers.py` & `inoopa_utils-2.9.8/inoopa_utils/openai_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/rabbitmq_helpers.py` & `inoopa_utils-2.9.8/inoopa_utils/rabbitmq_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/sql_helpers.py` & `inoopa_utils-2.9.8/inoopa_utils/sql_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/tests/test_rabbitmq.py` & `inoopa_utils-2.9.8/inoopa_utils/tests/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/inoopa_utils/typesense_helpers.py` & `inoopa_utils-2.9.8/inoopa_utils/typesense_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.7/pyproject.toml` & `inoopa_utils-2.9.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "inoopa_utils"
 description = "Collection of utils used at Inoopa."
-version = "2.9.7"
+version = "2.9.8"
 authors = ["Dev Inoopa <dev@inoopa.com>"]
 packages = [{ include = "inoopa_utils" }]
 repository = "https://bitbucket.org/inoopa/inoopa_utils/"
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 iniconfig = "^2.0.0"
 openai = "^1.14.3"
 pandas = "^2.0.3"
-pendulum = "^2.1.2"
+pendulum = ">=2.1.2"
 PyMySQL = "^1.0.0"
 python-dotenv = "1.0.0"
 rabbitpy = "^2.0.1"
 SQLAlchemy = "^2.0.0"
 tiktoken = "^0.6.0"
 typesense = "^0.18.0"
 pymongo = "^4.6.1"
```

### Comparing `inoopa_utils-2.9.7/PKG-INFO` & `inoopa_utils-2.9.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inoopa_utils
-Version: 2.9.7
+Version: 2.9.8
 Summary: Collection of utils used at Inoopa.
 Home-page: https://bitbucket.org/inoopa/inoopa_utils/
 Author: Dev Inoopa
 Author-email: dev@inoopa.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyMySQL (>=1.0.0,<2.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.0,<3.0.0)
 Requires-Dist: boto3 (>=1.34.18,<2.0.0)
 Requires-Dist: iniconfig (>=2.0.0,<3.0.0)
 Requires-Dist: openai (>=1.14.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: pendulum (>=2.1.2)
 Requires-Dist: pymongo (>=4.6.1,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: rabbitpy (>=2.0.1,<3.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: typesense (>=0.18.0,<0.19.0)
 Project-URL: Repository, https://bitbucket.org/inoopa/inoopa_utils/
```

