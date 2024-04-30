# Comparing `tmp/django_environment_config-0.0.3.tar.gz` & `tmp/django_environment_config-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_environment_config-0.0.3.tar", max compression
+gzip compressed data, was "django_environment_config-0.0.4.tar", max compression
```

## Comparing `django_environment_config-0.0.3.tar` & `django_environment_config-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2705 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/LICENSE
--rw-r--r--   0        0        0     2148 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/README.md
--rw-r--r--   0        0        0       64 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/__init__.py
--rw-r--r--   0        0        0     3206 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/base.py
--rw-r--r--   0        0        0      364 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/constants.py
--rw-r--r--   0        0        0      901 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/errors.py
--rw-r--r--   0        0        0        0 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/py.typed
--rw-r--r--   0        0        0     1210 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/typing.py
--rw-r--r--   0        0        0    11566 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/env_config/values.py
--rw-r--r--   0        0        0     8706 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/pytest_plugin/__init__.py
--rw-r--r--   0        0        0      792 2024-04-29 11:00:57.074359 django_environment_config-0.0.3/pytest_plugin/hooks.py
--rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 django_environment_config-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2705 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2148 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/README.md
+-rw-r--r--   0        0        0       64 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config/__init__.py
+-rw-r--r--   0        0        0     3373 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config/base.py
+-rw-r--r--   0        0        0      364 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config/constants.py
+-rw-r--r--   0        0        0      901 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config/errors.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config/py.typed
+-rw-r--r--   0        0        0     1210 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config/typing.py
+-rw-r--r--   0        0        0    11566 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config/values.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config_pytest_plugin/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/env_config_pytest_plugin/hooks.py
+-rw-r--r--   0        0        0     8728 2024-04-29 12:52:33.937581 django_environment_config-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 django_environment_config-0.0.4/PKG-INFO
```

### Comparing `django_environment_config-0.0.3/LICENSE` & `django_environment_config-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.3/README.md` & `django_environment_config-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.3/env_config/base.py` & `django_environment_config-0.0.4/env_config/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import inspect
 import os
 from typing import TYPE_CHECKING
 
 from django.utils.functional import classproperty
 from dotenv import dotenv_values
+from dotenv.main import find_dotenv
 
 from .constants import ENV_NAME, Undefined
 
 if TYPE_CHECKING:
     from dotenv.main import StrPath
 
     from .typing import Any
@@ -25,15 +26,15 @@
     def __init_subclass__(
         cls,
         *,
         dotenv_path: StrPath | None | Undefined = Undefined,
     ) -> None:
         env: str | None = os.environ.get(ENV_NAME)
         if env is None:  # pragma: no cover
-            msg = f"Environment variable {ENV_NAME!r} must be set before subclassing {cls.__name__!r}"
+            msg = f"Environment variable {ENV_NAME!r} must be set before subclassing 'Environment'"
             raise ValueError(msg)
 
         if cls.__name__ != env:
             return
 
         # If not given, set it to `None` so that `python-dotenv` will use
         # `dotenv.main.find_dotenv` to find the `.env` file automatically.
@@ -52,16 +53,18 @@
         setattr(cls, f"_{cls.__name__}__dotenv_path", dotenv_path)
 
         cls.pre_setup()
         cls.setup(stack_level=2)
         cls.post_setup()
 
     @staticmethod
-    def load_dotenv(*, dotenv_path: StrPath | None = None) -> dict[str, str]:
+    def load_dotenv(*, dotenv_path: StrPath | None = None) -> dict[str, str]:  # pragma: no cover
         """Load the `.env` file and return the values."""
+        if dotenv_path is None:
+            dotenv_path = find_dotenv(raise_error_if_not_found=True, usecwd=True)
         return dotenv_values(dotenv_path=dotenv_path)
 
     @classmethod
     def pre_setup(cls) -> None:
         """
         Hook for doing additional setup before the settings have been loaded,
         but after the `.env` file has been loaded.
```

### Comparing `django_environment_config-0.0.3/env_config/errors.py` & `django_environment_config-0.0.4/env_config/errors.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.3/env_config/typing.py` & `django_environment_config-0.0.4/env_config/typing.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.3/env_config/values.py` & `django_environment_config-0.0.4/env_config/values.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.3/pyproject.toml` & `django_environment_config-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "django-environment-config"
-version = "0.0.3"
+version = "0.0.4"
 description = "Configure django settings for multiple environments."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "env_config" },
-    { include = "pytest_plugin" },
+    { include = "env_config_pytest_plugin" },
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mrthearman.github.io/django-environment-config"
 repository = "https://github.com/MrThearMan/django-environment-config"
 keywords = [
     "django",
@@ -72,15 +72,15 @@
 django-stubs = "4.2.7"
 
 [tool.poetry.extras]
 db = ["dj-database-url"]
 cache = ["django-cache-url"]
 
 [tool.poetry.plugins.pytest11]
-django_environment_config = "pytest_plugin.hooks"
+django_environment_config = "env_config_pytest_plugin.hooks"
 
 [tool.ruff]
 fix = true
 unsafe-fixes = true
 line-length = 120
 extend-exclude = [
     "tests/*",
```

### Comparing `django_environment_config-0.0.3/pytest_plugin/hooks.py` & `django_environment_config-0.0.4/env_config_pytest_plugin/hooks.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.3/PKG-INFO` & `django_environment_config-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-environment-config
-Version: 0.0.3
+Version: 0.0.4
 Summary: Configure django settings for multiple environments.
 Home-page: https://mrthearman.github.io/django-environment-config
 License: MIT
 Keywords: django,configuration,settings,environment,env,config
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.10,<4
```

