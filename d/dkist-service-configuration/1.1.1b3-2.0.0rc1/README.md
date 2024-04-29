# Comparing `tmp/dkist-service-configuration-1.1.1b3.tar.gz` & `tmp/dkist_service_configuration-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-service-configuration-1.1.1b3.tar", last modified: Fri Dec 15 17:19:34 2023, max compression
+gzip compressed data, was "dkist_service_configuration-2.0.0rc1.tar", last modified: Mon Apr 29 20:25:42 2024, max compression
```

## Comparing `dkist-service-configuration-1.1.1b3.tar` & `dkist_service_configuration-2.0.0rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-15 17:19:34.307795 dkist-service-configuration-1.1.1b3/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1892 2023-12-15 17:19:34.307795 dkist-service-configuration-1.1.1b3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1274 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-15 17:19:34.303795 dkist-service-configuration-1.1.1b3/dkist_service_configuration/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-15 17:19:34.303795 dkist-service-configuration-1.1.1b3/dkist_service_configuration/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1701 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration/tests/test_settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-15 17:19:34.307795 dkist-service-configuration-1.1.1b3/dkist_service_configuration.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1892 2023-12-15 17:19:34.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-12-15 17:19:34.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-12-15 17:19:34.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-12-15 17:19:34.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-12-15 17:19:34.000000 dkist-service-configuration-1.1.1b3/dkist_service_configuration.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-12-15 17:19:34.307795 dkist-service-configuration-1.1.1b3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-12-15 17:19:18.000000 dkist-service-configuration-1.1.1b3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1934 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/test_settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1934 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      631 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/setup.py
```

### Comparing `dkist-service-configuration-1.1.1b3/.gitignore` & `dkist_service_configuration-2.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.1.1b3/.pre-commit-config.yaml` & `dkist_service_configuration-2.0.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.1.1b3/LICENSE` & `dkist_service_configuration-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.1.1b3/PKG-INFO` & `dkist_service_configuration-2.0.0rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 1.1.1b3
+Version: 2.0.0rc1
 Summary: Configuration support for DKIST services
 Home-page: https://bitbucket.org/dkistdc/dkist_service_configuration/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: loguru
-Requires-Dist: pydantic[dotenv]<2.0
+Requires-Dist: pydantic-settings
+Requires-Dist: pydantic[dotenv]>2.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 dkist-service-configuration
 ===========================
 
@@ -44,15 +45,15 @@
 Examples
 --------
 
 **config.py**
 
 .. code:: python
 
-    from dkist_service_configuration import logger
+    from dkist_service_configuration.logging import logger
     from dkist_service_configuration import MeshServiceConfigurationBase
     logger.debug('hello world)
     class NewConfiguration(MeshServiceConfigurationBase):
         username: str = "me"
         password: str = "pass"
     new_configuration = NewConfiguration()
     new_configuration.log_configurations()
```

### Comparing `dkist-service-configuration-1.1.1b3/README.rst` & `dkist_service_configuration-2.0.0rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 Examples
 --------
 
 **config.py**
 
 .. code:: python
 
-    from dkist_service_configuration import logger
+    from dkist_service_configuration.logging import logger
     from dkist_service_configuration import MeshServiceConfigurationBase
     logger.debug('hello world)
     class NewConfiguration(MeshServiceConfigurationBase):
         username: str = "me"
         password: str = "pass"
     new_configuration = NewConfiguration()
     new_configuration.log_configurations()
```

### Comparing `dkist-service-configuration-1.1.1b3/bitbucket-pipelines.yml` & `dkist_service_configuration-2.0.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.1.1b3/dkist_service_configuration/logging.py` & `dkist_service_configuration-2.0.0rc1/dkist_service_configuration/logging.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.1.1b3/dkist_service_configuration/settings.py` & `dkist_service_configuration-2.0.0rc1/dkist_service_configuration/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,62 @@
 """
 Wrapper for retrieving configurations and safely logging their retrieval
 """
 import re
 
 from pydantic import BaseModel
-from pydantic import BaseSettings
 from pydantic import Field
+from pydantic_settings import BaseSettings
+from pydantic_settings import SettingsConfigDict
 
 from dkist_service_configuration.logging import logger
 
 
 class ConfigurationBase(BaseSettings):
     """Settings base which logs configured settings while censoring secrets"""
 
-    log_level: str = Field("INFO", env="LOGURU_LEVEL")
-    # env -> validation_alias in pydantic 2.x
+    log_level: str = Field(default="INFO", validation_alias="LOGURU_LEVEL")
 
-    class Config:
-        env_file = ".env"
-        env_file_encoding = "utf-8"
-
-    # model_config = SettingsConfigDict(env_file=".env", env_file_encoding="utf-8") in pydantic 2.x
+    model_config = SettingsConfigDict(env_file=".env", env_file_encoding="utf-8")
 
     @staticmethod
     def _is_secret(field_name: str) -> bool:
         for pattern in ("pass", "secret", "token"):
             if re.search(pattern, field_name):
                 return True
         return False
 
     def log_configurations(self):
-        for field_name in self.__fields__:  # __fields__ -> model_fields in pydantic 2.x
+        for field_name in self.model_fields:
             if self._is_secret(field_name=field_name):
                 logger.info(f"{field_name}: <CENSORED>")
             else:
                 logger.info(f"{field_name}: {getattr(self, field_name)}")
 
 
 class MeshService(BaseModel):
     """Model of the metadata for a node in the service mesh"""
 
-    host: str = Field(..., alias="mesh_address")
-    port: int = Field(..., alias="mesh_port")
+    host: str = Field(default=..., alias="mesh_address")
+    port: int = Field(default=..., alias="mesh_port")
 
 
 DEFAULT_MESH_SERVICE = MeshService(mesh_address="127.0.0.1", mesh_port=0)
 
 
 class MeshServiceConfigurationBase(ConfigurationBase):
     """
     Settings base for services using a mesh configuration to define connections in the form
     {
         "upstream_service_name": {"mesh_address": "localhost", "mesh_port": 6742}
     }
     """
 
     service_mesh: dict[str, MeshService] = Field(
-        default_factory=dict, env="MESH_CONFIG"
-    )  # env -> validation_alias when going to pydantic 2.x
+        default_factory=dict, validation_alias="MESH_CONFIG"
+    )
 
     def service_mesh_detail(
         self, service_name: str, default_mesh_service: MeshService = DEFAULT_MESH_SERVICE
     ) -> MeshService:
         mesh_service = self.service_mesh.get(service_name) or default_mesh_service
         return mesh_service
```

### Comparing `dkist-service-configuration-1.1.1b3/dkist_service_configuration/tests/test_settings.py` & `dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.1.1b3/dkist_service_configuration.egg-info/PKG-INFO` & `dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 1.1.1b3
+Version: 2.0.0rc1
 Summary: Configuration support for DKIST services
 Home-page: https://bitbucket.org/dkistdc/dkist_service_configuration/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: loguru
-Requires-Dist: pydantic[dotenv]<2.0
+Requires-Dist: pydantic-settings
+Requires-Dist: pydantic[dotenv]>2.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 dkist-service-configuration
 ===========================
 
@@ -44,15 +45,15 @@
 Examples
 --------
 
 **config.py**
 
 .. code:: python
 
-    from dkist_service_configuration import logger
+    from dkist_service_configuration.logging import logger
     from dkist_service_configuration import MeshServiceConfigurationBase
     logger.debug('hello world)
     class NewConfiguration(MeshServiceConfigurationBase):
         username: str = "me"
         password: str = "pass"
     new_configuration = NewConfiguration()
     new_configuration.log_configurations()
```

### Comparing `dkist-service-configuration-1.1.1b3/dkist_service_configuration.egg-info/SOURCES.txt` & `dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.1.1b3/setup.cfg` & `dkist_service_configuration-2.0.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
 	loguru
-	pydantic[dotenv] < 2.0
+	pydantic-settings
+	pydantic[dotenv] > 2.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 
 [tool:pytest]
```

