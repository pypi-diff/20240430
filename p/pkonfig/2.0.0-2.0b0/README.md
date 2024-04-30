# Comparing `tmp/pkonfig-2.0.0.tar.gz` & `tmp/pkonfig-2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkonfig-2.0.0.tar", max compression
+gzip compressed data, was "pkonfig-2.0b0.tar", last modified: Sun Mar 12 06:25:22 2023, max compression
```

## Comparing `pkonfig-2.0.0.tar` & `pkonfig-2.0b0.tar`

### file list

```diff
@@ -1,16 +1,50 @@
--rw-r--r--   0        0        0     1072 2024-04-30 13:28:33.870947 pkonfig-2.0.0/LICENSE
--rw-r--r--   0        0        0    19535 2024-04-30 13:28:33.870947 pkonfig-2.0.0/README.md
--rw-r--r--   0        0        0      348 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/__init__.py
--rw-r--r--   0        0        0     2193 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/config.py
--rw-r--r--   0        0        0      227 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/errors.py
--rw-r--r--   0        0        0     6025 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/fields.py
--rw-r--r--   0        0        0      491 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/storage/__init__.py
--rw-r--r--   0        0        0     3004 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/storage/base.py
--rw-r--r--   0        0        0     1281 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/storage/dot_env.py
--rw-r--r--   0        0        0      809 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/storage/env.py
--rw-r--r--   0        0        0     1150 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/storage/ini.py
--rw-r--r--   0        0        0      195 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/storage/json.py
--rw-r--r--   0        0        0      553 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/storage/toml.py
--rw-r--r--   0        0        0      222 2024-04-30 13:28:33.870947 pkonfig-2.0.0/pkonfig/storage/yaml_.py
--rw-r--r--   0        0        0     3668 2024-04-30 13:28:47.790994 pkonfig-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    20966 1970-01-01 00:00:00.000000 pkonfig-2.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.670579 pkonfig-2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-12 06:25:12.000000 pkonfig-2.0b0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.666578 pkonfig-2.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.666578 pkonfig-2.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-12 06:25:12.000000 pkonfig-2.0b0/.github/workflows/code-quality.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-12 06:25:12.000000 pkonfig-2.0b0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-12 06:25:12.000000 pkonfig-2.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21029 2023-03-12 06:25:12.000000 pkonfig-2.0b0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-12 06:25:12.000000 pkonfig-2.0b0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-12 06:25:12.000000 pkonfig-2.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20222 2023-03-12 06:25:22.670579 pkonfig-2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-12 06:25:12.000000 pkonfig-2.0b0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    30599 2023-03-12 06:25:12.000000 pkonfig-2.0b0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-03-12 06:25:12.000000 pkonfig-2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.666578 pkonfig-2.0b0/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:12.000000 pkonfig-2.0b0/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-12 06:25:12.000000 pkonfig-2.0b0/benchmark/pydantic_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.666578 pkonfig-2.0b0/pkonfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.670579 pkonfig-2.0b0/pkonfig/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/storage/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pkonfig/storage/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.666578 pkonfig-2.0b0/pkonfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20222 2023-03-12 06:25:22.000000 pkonfig-2.0b0/pkonfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-12 06:25:22.000000 pkonfig-2.0b0/pkonfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 06:25:22.000000 pkonfig-2.0b0/pkonfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-12 06:25:22.000000 pkonfig-2.0b0/pkonfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-12 06:25:22.000000 pkonfig-2.0b0/pkonfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-12 06:25:12.000000 pkonfig-2.0b0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-03-12 06:25:12.000000 pkonfig-2.0b0/python_version_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-12 06:25:22.670579 pkonfig-2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-12 06:25:12.000000 pkonfig-2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.670579 pkonfig-2.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:22.670579 pkonfig-2.0b0/tests/test_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_storage/test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_storage/test.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_storage/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_storage/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_storage/test_dot_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-12 06:25:12.000000 pkonfig-2.0b0/tests/test_storage/test_optional.py
```

### Comparing `pkonfig-2.0.0/LICENSE` & `pkonfig-2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pkonfig-2.0.0/README.md` & `pkonfig-2.0b0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 [![Code Style - isort](https://img.shields.io/badge/Code%20Style-isort-%231674b1)](https://pycqa.github.io/isort/)
 [![codecov](https://codecov.io/github/ngladkikh/pkonfig/branch/main/graph/badge.svg?token=VDRSB1XUFH)](https://codecov.io/github/ngladkikh/pkonfig)
 
 ## Prerequisites
 
 - Pythonic configuration management helpers.
 - Multiple sources of configs (environment variables, dotenv files, YAML, JSON, TOML, INI)
-  with agile order configuration.
+with agile order configuration.
 - Configs validation mechanics based on type hints or user defined classes.
 - Minimal external dependencies.
 - Follow [Fail-fast](https://en.wikipedia.org/wiki/Fail-fast) principle.
 - Autocomplete in modern IDEs.
 
 ## Features
 
-- User defined config source order: Define the order in which PKonfig looks for configuration values.
-- Multilevel configs for environment variables and dotenv config sources: Allows for more granular control over configuration values.
-- Custom aliases for fields or groups of configs: Create custom aliases for configuration values to make them easier to reference in code.
-- Configs type casting: Automatically cast configuration values to the correct data type.
-- Config values validation based on type and/or value: Validate configuration values to ensure they meet specific requirements.
-- High performance: Designed to be fast and efficient.
-- Extendable API: Easily extend PKonfig to meet your specific needs.
+- User defined config source order.
+- Multilevel configs for environment variables and dotenv config sources.
+- Custom aliases for fields or groups of configs.
+- Configs type casting
+- Config values validation based on type and/or value.
+- High performance.
+- Extendable API.
 
 ## Installation
 
 To install basic PKonfig without YAML and TOML support run:
 
 ```bash
 pip install pkonfig
@@ -54,49 +54,46 @@
 
 And if both TOML and YAML is needed:
 
 ```bash
 pip install pkonfig[toml,yaml]
 ```
 
-For production no __.env__ files are needed but proper environment variables should be set.
-In case some of required variables missing __ConfigValueNotFoundError__ exception raised while __AppConfig__
+For production no __.env__ files are needed but propper environment variables should be set.
+In case some of required variables missing __KeyError__ exception raised while __AppConfig__
 instantiation.
 
 ## Quickstart
 
-The Config class is a Pythonic configuration management helper designed
-to provide a simple way of managing multiple sources of configuration values in your application.
 The most basic usage example when environment variables are used for production
 environment and DotEnv files are used for local development.
 
 Create __config__ module __config.py__:
 
 ```python
-from typing import Literal
-from pkonfig import Config, LogLevel, Choice, Str, Int
-from pkonfig.storage import Env
-from pkonfig import DotEnv
+from pkonfig import Config, Env, LogLevel, Choice, Storage
+from storage import DotEnv
 
 
 class PG(Config):
-    host: str = Str("localhost")
-    port: int = Int(5432)
-    user: str = Str("postgres")
-    password: str = Str("postgres")
+  host = "localhost"
+  port = 5432
+  user = "postgres"
+  password = "postgres"
 
 
 class AppConfig(Config):
-    db1 = PG()
-    db2 = PG()
-    log_level: int = LogLevel("INFO")
-    env: Literal["local", "prod", "test"] = Choice(["local", "prod", "test"], default="prod")
+  db1 = PG()
+  db2 = PG()
+  log_level = LogLevel("INFO")
+  env = Choice(["local", "prod", "test"], default="prod")
 
 
-config = AppConfig(DotEnv(".env"), Env())
+storage = Storage(DotEnv(".env", missing_ok=True), Env())
+config = AppConfig(storage)
 ```
 
 For local development create DotEnv file in root app folder __.env__:
 
 ```dotenv
 APP_DB1_HOST=10.10.10.10
 APP_DB1_USER=user
@@ -106,77 +103,66 @@
 ```
 
 Then elsewhere in app you could run:
 
 ```python
 from config import config
 
-print(config.env)           # 'local'
+print(config.env)           # local
 print(config.log_level)     # 20
-print(config.db.host)       # 'localhost'
+print(config.db.host)       # localhost
 print(config.db.port)       # 5432
-print(config.db.user)       # 'postgres'
-print(config.db.password)   # 'postgres'
+print(config.db.user)       # postgres
+print(config.db.password)   # postgres
 ```
 
 ## Usage
 
 ### Config sources
 
 __PKonfig__ implements several config sources out of the box.
-Use `DictStorage` if some defaults should be stored from code rather than from field default values:
-
-```python
-from pkonfig import Config, Str, DictStorage
-
-
-class AppConfig(Config):
-    foo: str = Str()    # foo has no default value and raise an exception if value not found in storage
-
-
-CONFIG = AppConfig(DictStorage(foo="baz"))
-print(CONFIG.foo)   # 'baz'
-```
+All config sources implement `Mapping` protocol and default values could be set up during initialization.
 
 #### Environment variables
 
 The most common way to configure application is environment variables.
 To parse environment variables and store values in multilevel structure class `Env` could be used.
-Common pattern is naming variables with multiple words describing the exact purpose
+Common pattern is naming variables with multiple words describing the exact purpose 
 more precise: __PG_HOST__, __PG_PORT__ and __REDIS_HOST__, __REDIS_PORT__ could be treated as two groups:
 
 - PG
-    - HOST
-    - PORT
+  - HOST
+  - PORT
 - REDIS
-    - HOST
-    - PORT
+  - HOST
+  - PORT
 
 PKonfig respects this convention so that `Env` has two optional arguments:
 
 - `delimiter` string that will be used to split configuration levels taken from keys;
 - `prefix` string that is used to identify keys that are related to the given app and omit everything else.
 
 ```python
 from os import environ
-from pkonfig.storage import Env
+from pkonfig import Env
+
 
 environ["APP_OUTER"] = "foo"
 environ["APP_INNER_KEY"] = "baz"
 environ["NOPE"] = "qwe"
 
-source = Env(delimiter="_", prefix="APP")
+source = Env(delimiter="_", prefix="APP", some_key="some")
 
-print(source[("outer",)])  # foo
-print(source[("inner", "key")])  # baz
-print(source[("nope",)])  # raises KeyError
+print(source[("outer",)])          # foo
+print(source[("inner", "key")])    # baz
+print(source[("nope",)])           # raises KeyError
 ```
 
 `Env` ignores key cases and ignores all keys starting not from __prefix__.
-To change this behaviour set __prefix__ to `None` or an empty string.
+To change this behaviour set __prefix__ to `None`.
 In this case you will get all key value pairs:
 
 ```python
 from os import environ
 from pkonfig import Env
 
 environ["NOPE"] = "qwe"
@@ -190,53 +176,54 @@
 
 In the same manner as environment variables DotEnv files could be used.
 `DotEnv` requires file name as a string or a path and also accepts `delimiter` and `prefix` optional arguments.
 `missing_ok` argument defines whether `DotEnv` raises exception when given file not found.
 When file not found and `missing_ok` is set `DotEnv` contains empty dictionary.
 
 ```python
-from pkonfig import DotEnv
+
+from storage import DotEnv
 
 config_source = DotEnv("test.env", delimiter="_", prefix="APP", missing_ok=True)
 ```
 
 #### Ini
 
-__INI__ files are quite common and class `Ini`
-is build on top of [`configparser.ConfigParser`](https://docs.python.org/3/library/configparser.html).
+__INI__ files are quite common and class `Ini` 
+is build on top of [`configparser.ConfigParser`](https://docs.python.org/3/library/configparser.html):
+
+```python
+
+from storage import Ini
 
-**config.ini** file example:
+storage = Ini("config.ini", missing_ok=False)
+print(storage[("bitbucket.org", "User")])  # hg
+print(storage[("bitbucket.org", "ServerAliveInterval")])  # 45
+```
+
+In case when __config.ini__:
 
 ```ini
 [DEFAULT]
 ServerAliveInterval = 45
 
 [bitbucket.org]
 User = hg
 ```
 
-Then in Python code:
-
-```python
-from pkonfig.storage import Ini
-
-storage = Ini("config.ini", missing_ok=False)
-print(storage[("bitbucket.org", "User")])  # hg
-print(storage[("bitbucket.org", "ServerAliveInterval")])  # 45
-```
-
 `Ini` also accepts `missing_ok` argument to ignore missing file.
 Most of `ConfigParser` arguments are also accepted to modify parser behaviour.
 
 #### Json
 
 `Json` class uses `json.load` to read given JSON file and respects `missing_ok` argument:
 
 ```python
-from pkonfig.storage import Json
+
+from storage import Json
 
 storage = Json("config.json", missing_ok=False)
 ```
 
 #### Yaml
 
 To parse YAML files [PyYaml](https://pyyaml.org/wiki/PyYAMLDocumentation) could be used wrapped with `Yaml` class:
@@ -261,108 +248,107 @@
 ### Source order
 
 Any source for `BaseConfig` should implement `Mapper` protocol.
 So it is easy to implement custom or combine existing implementations.
 Recommended way to combine multiple sources of configs is `ChainMap`:
 
 ```python
-from pkonfig import Config, Env, Yaml, DotEnv, Str
-
-
-class AppConfig(Config):
-    foo: str = Str()
+from pkonfig import Env, Yaml, Storage
+from storage import DotEnv
 
-
-config = AppConfig(
-    DotEnv("test.env", missing_ok=True),
-    Env(),
-    Yaml("base_config.yaml"),
+config_source = Storage(
+  DotEnv("test.env", missing_ok=True),
+  Env(),
+  Yaml("base_config.yaml")
 )
 ```
 
-In this example we created `AppConfig` that looks for key until finds one in the given mappers sequence.
+In this example we created `ChainMap` that looks for key until finds one in the given mappers sequence.
 The first one source for configs is **test.env** file that might not exist and could be used for local development only.
-Then environment variables are used as the second one config source.
-The last one is **base_config.yaml** that should exist or `FileNotFoundError` exception raised.
-You can customize source order.
+Environment variables are used as the second one config source.
+Dotenv file will be preferred source in this example.
+The last one source is **base_config.yaml** that should exist or `FileNotFoundError` exception raised.
+
+You can customize source order in this way or even create your own logic implementing
+`Mapper` protocol.
 
 ### Config
 
 To implement application config class user should inherit from `pkonfig.config.Config` class and define
 required fields:
 
 ```python
-from pkonfig import Config, Float, Int, DictStorage
+from pkonfig import Config
 
 
 class AppConfig(Config):
-    foo: float = Float()
-    baz: int = Int()
+    foo: float
+    baz: int
 
 
-config = AppConfig(DictStorage(**{"foo": "0.33", "baz": 1}))
+storage = {"foo": "0.33", "baz": 1}
+config = AppConfig(storage)
 
 print(config.foo)   # 0.33
 print(config.baz)   # 1
 ```
 
 To build more granular config structure:
 
 ```python
-from pkonfig import Config, DictStorage, Float, Int, Str
+from pkonfig import Config
 
 
 class Inner(Config):
-    key: str = Str()
+    key: str
 
 
 class AppConfig(Config):
     inner = Inner()
-    foo: float = Float()
-    baz: int = Int()
+    foo: float
+    baz: int
 
 
-storage = DictStorage(
-    **{
-        "foo": "0.33",
-        "baz": 1,
-        "inner": {"key": "value"}
-    }
-)
+storage = {
+    "foo": "0.33", 
+    "baz": 1, 
+    "inner": {"key": "value"}
+}
 config = AppConfig(storage)
 
 print(config.inner.key)   # value
 ```
 
 ### Multilevel Config
 
 Grouping might be useful when there are lots of config parameters.
-To achieve this `Config` class should be inherited like:
+To achieve this `EmbeddedConfig` class should be inherited:
 
 ```python
-from pkonfig import Config, DotEnv, Str, Int
+from pkonfig import Config
+from storage import DotEnv
 
 
 class PgConfig(Config):
-    host: str = Str("localhost")
-    port: int = Int(5432)
+  host: str
+  port: int = 5432
 
 
 class RedisConfig(Config):
-    host: str = Str("localhost")
-    port: int = Int(6379)
+  host: str
+  port: int = 6379
 
 
 class AppConfig(Config):
-    pg = PgConfig()
-    redis = RedisConfig()
+  pg = PgConfig()
+  redis = RedisConfig()
 
 
 config = AppConfig(
-    DotEnv(".env", delimiter="__", prefix="APP")
+  DotEnv(".env", delimiter="__", prefix="APP")
 )
 
 print(config.pg.host)  # db_host
 print(config.pg.port)  # 6432
 print(config.redis.host)  # redis
 ```
 
@@ -372,34 +358,35 @@
 APP__PG__PORT=6432
 APP__REDIS__HOST=redis
 ```
 In this example we customized delimiter with two underscores, default is '**_**'.
 
 ### Aliases
 
-All __Config__ fields accept __alias__ argument.
+All __Config__ fields accept __alias__ argument. 
 When storage class searches for config attribute in its source either attribute
 name is used or alias when it is set.
 
 __config.py__:
 
 ```python
-from pkonfig import Config, Int, Str, DotEnv
+from pkonfig import Config, Int, Str
+from storage import DotEnv
 
 
 class HostConfig(Config):
-    host: str = Str("localhost")
-    port: int = Int(5432)
-    user: str = Str("user")
-    password = Str(alias="pass")
+  host: str
+  port: int
+  user: str
+  password = Str(alias="pass")
 
 
 class AppConfig(Config):
-    pg = HostConfig(alias="db")
-    foo_baz = Int(alias="my_alias")
+  pg = HostConfig(alias="db")
+  foo_baz = Int(alias="my_alias")
 
 
 config = AppConfig(DotEnv(".env", delimiter="__"))
 ```
 
 __.env__ content:
 
@@ -408,15 +395,15 @@
 APP__DB__PORT=6432
 APP__DB__PASS=password
 APP__DB__USER=postgres
 APP__MY_ALIAS=123
 ```
 
 In this example storage will seek in dotenv file parameters named by given alias.
-Elsewhere in the app:
+Elsewhere in an app:
 
 ```python
 from config import config
 
 
 print(config.foo_baz)       # 123
 print(config.pg.password)   # password
@@ -437,102 +424,131 @@
 class AppConfig(Config):
     foo: str
     baz: int
     flag: bool
     file: Path
 ```
 
+#### Using default values:
+
+```python
+from pathlib import Path
+from pkonfig import Config
+
+
+class AppConfig(Config):
+    foo = "some"
+    baz = 1
+    flag = False
+    file = Path("some.text")
+```
+
+Given values will be used as default values.
+
+#### Using PKonfig fields directly
+
+```python
+from pkonfig import Config, PathField, Str, Int, Bool
+
+
+class AppConfig(Config):
+    foo = Str()
+    baz = Int()
+    flag = Bool()
+    file = PathField()
+```
+
 #### Caching
 
 All __PKonfig__ field types are Python descriptors that are responsible for type casting and data validation.
 In most cases there is no need to do this job every time the value is accessed.
 To avoid undesirable calculations caching is used.
-So that type casting and validation is done only once during `Config` object initialization.
+So that type casting and validation is done only once 
+during `Config` object initialization.
+In case when configuration may change during application lifecycle user may disable this behaviour:
+
+```python
+from pkonfig import Config, Int
+
+
+class AppConfig(Config):
+    attr = Int(no_cache=True)
+```
+
+In given example `attr` will do type casting and validation every time this attribute is accessed.
 
 #### Default values
 
 If value is not set in config source user can use default value.
 `None` could be used as default value:
 
 ```python
-from pkonfig import Config, Int, Str, DictStorage
+from pkonfig import Config, Int, Str
 
 
 class AppConfig(Config):
     int_attr = Int(None)
     str_attr = Str(None)
 
-config = AppConfig(DictStorage())
+config = AppConfig({})
 print(config.str_attr)    # None
 print(config.int_attr)    # None
 ```
 
-When `None` is default value the field is treated as nullable.
+When `None` is default value field is treated as nullable.
 
 #### Field nullability
 
 To handle type casting and validation fields should not be nullable.
 In case `None` is a valid value and should be used without casting and validation
 option `nullable` could be set:
 
 ```python
-from pkonfig import Int, Config, DictStorage
+from pkonfig import Int, Config
 
 
 class AppConfig(Config):
     int_attr = Int(nullable=True)
 
-config = AppConfig(DictStorage(int_attr=None))
+config = AppConfig(dict(int_attr=None))
 print(config.int_attr)    # None
 ```
 
-In this example when `None` comes from storage type casting and validation is omitted.
-
-By default, fields are treated as not nullable:
-
-```python
-from pkonfig import Int, Config, DictStorage
-
-
-class AppConfig(Config):
-    int_attr = Int(default=1)
-
-config = AppConfig(DictStorage(int_attr=None))  # ValueError("Not nullable") is raised here
-```
+In this example `None` comes from storage and type casting is omitted.
 
 ### Custom descriptor or property
 
 ```python
-from pkonfig import Config, Bool, DictStorage, Str
+from pkonfig import Config
 
 
 class AppConfig(Config):
-    flag: bool = Bool(True)
-    baz: str = Str("test")
-
+    flag = True
+    baz = "test"
+    
     @property
     def value(self):
-        return self.flag and self.baz == "test"
+        return self.flag and self.baz == "test" 
 
 
-config = AppConfig(DictStorage())
+config = AppConfig({})
 print(config.value)  # True
 ```
 
 ### Custom field types
 
 User can customize how field validation and casting is done.
 The recommended way is to implement `validate` method:
 
 ```python
 from pkonfig import Config, Int
 
 
 class OnlyPositive(Int):
-    def validate(self, value) -> None:
+    def validate(self, value):
         if value < 0:
             raise ValueError("Only positive values accepted")
 
 
 class AppConfig(Config):
     positive = OnlyPositive()
 ```
@@ -540,15 +556,14 @@
 Custom type casting is also available.
 To achieve this user should inherit abstract class `Field` and implement method `cast`:
 
 ```python
 from typing import List
 from pkonfig import Field
 
-
 class ListOfStrings(Field):
     def cast(self, value: str) -> List[str]:
         return value.split(",")
 ```
 
 ### Available fields
 
@@ -558,14 +573,16 @@
 - int -> `Int`
 - float -> `Float`
 - Decimal -> `DecimalField`
 - str -> `Str`
 - bytes -> `Byte`
 - bytearray -> `ByteArray`
 
+The only reason to use this types directly is customising field nullability and cache policy.
+
 #### PathField
 
 Basic path type that is parental for other two types and is used when you define field using `pathlib.Path`.
 This type raises `FileNotFoundError` exception during initialization if given path doesn't exist:
 
 ```python
 from pkonfig import Config, PathField
@@ -588,110 +605,145 @@
 
 #### EnumField
 
 This field uses custom enum to validate input and cast it to given `Enum`:
 
 ```python
 from enum import Enum
-from pkonfig import Config, EnumField, DictStorage, Int
+from pkonfig import Config, EnumField
 
 
 class UserType(Enum):
-    guest = Int(1)
-    user = Int(2)
-    admin = Int(3)
+    guest = 1
+    user = 2
+    admin = 3
 
 
 class AppConfig(Config):
     user_type = EnumField(UserType)
 
 
-config = AppConfig(DictStorage(user_type="admin"))
+config = AppConfig({"user_type": "admin"})
 print(config.user_type is UserType.admin)  # True
 ```
 
 #### LogLevel
 
 `LogLevel` field is useful to define `logging` level through configs.
-`LogLevel` accepts strings that define log level and casts
+`LogLevel` accepts strings that define log level and casts 
 that string to `logging` level integer value:
 
 ```python
 import logging
-from pkonfig import Config, LogLevel, DictStorage
+from pkonfig import Config, LogLevel
 
 
 class AppConfig(Config):
     some_level = LogLevel()
     another_level = LogLevel()
 
 
 config = AppConfig(
-    DictStorage(
-        some_level="info",
-        another_level="Debug",
-    )
+    {
+        "some_level": "info",
+        "another_level": "Debug",
+    }
 )
 
 print(config.some_level)        # 20
 print(config.another_level)     # 10
 
 print(config.another_level is logging.DEBUG)     # True
 ```
 
 #### Choice
 
 `Choice` field validates that config value is a member of the given sequence and also does optional type casting:
 
 ```python
-from pkonfig import Config, Choice, DictStorage
+from pkonfig import Config, Choice
 
 
 class AppConfig(Config):
     one_of_attr = Choice([10, 100], cast_function=int)
 
 
-config = AppConfig(DictStorage(one_of_attr="10"))
+config = AppConfig({"one_of_attr": "10"})
 print(config.one_of_attr == 10)  # True
 
-config = AppConfig(DictStorage(one_of_attr="2"))    # raises TypeError exception
+config = AppConfig({"one_of_attr": "2"})    # raises TypeError exception
 ```
 
 When `cast_function` is not given raw values from storage are used.
 
 #### DebugFlag
 
 `DebugFlag` helps to set widely used __debug__ option.
 `DebugFlag` ignores value case and treats __'true'__ string as `True` and any other value as `False`:
 
 ```python
-from pkonfig import Config, Bool, DictStorage
+from pkonfig import Config, DebugFlag
 
 
 class AppConfig(Config):
-    lower_case = Bool()
-    upper_case = Bool()
-    random_string = Bool()
+    lower_case = DebugFlag()
+    upper_case = DebugFlag()
+    random_string = DebugFlag()
 
 
 config = AppConfig(
-    DictStorage(
-        lower_case="true",
-        upper_case="TRUE",
-        random_string="foo",
-    )
+  {
+    "lower_case": "true",
+    "upper_case": "TRUE",
+    "random_string": "foo",
+  }
 )
 print(config.lower_case)        # True
 print(config.upper_case)        # True
 print(config.random_string)     # False
 ```
 
+### Types to Fields mapping
+
+All fields for `BaseConfig` children classes are converted to descriptors internally.
+Class `pkonfig.config.DefaultMapper` defines how field types will be replaced with descriptors.
+This mapping is used by default:
+```
+{
+    bool: Bool,
+    int: Int,
+    float: Float,
+    str: Str,
+    bytes: Byte,
+    bytearray: ByteArray,
+    Path: PathField,
+    Decimal: DecimalField,
+}
+```
+
+When field type is not found in this mapper it is ignored and won't be taken from storage source while resolving.
+
+User can modify default mapper giving dictionary of types and appropriate fields:
+
+```python
+from decimal import Decimal
+from pkonfig import Config, DefaultMapper, DecimalField
+
+
+class AppConfig(Config):
+    _mapper = DefaultMapper({float: DecimalField})
+    foo: float
+
+config = AppConfig(dict(foo=1/3))
+assert isinstance(config.foo, Decimal)  # True
+```
+
 ### Per-environment config files
 
-When your app is configured with different configuration files
+When your app is configured with different configuration files 
 and each file is used only in an appropriate environment you can create a function
 to find which file should be used:
 
 ```python
 from pkonfig import Env, Config, Choice
 
 
@@ -701,24 +753,24 @@
     "local": "configs/local.yaml",
 }
 
 
 def get_config_file():
     class _Config(Config):
         env = Choice(
-            ["prod", "local", "staging"],
-            cast_function=str.lower,
-            default="prod"
+          ["prod", "local", "staging"], 
+          cast_function=str.lower,
+          default="prod"
         )
-
+    
     _config = _Config(Env())
     return CONFIG_FILES[_config.env]
 ```
 
-__get_config_file__ uses environment variables and predefined config files paths
+__get_config_file__ uses environment variables and predefined config files pathes
 to check whether __APP_ENV__ var is set, validate this variable and return appropriate
 config file name.
 Then actual application configuration:
 
 ```python
 from pkonfig import Env, Yaml, Config, Choice
 
@@ -729,51 +781,27 @@
     "local": "configs/local.yaml",
 }
 
 
 def get_config_file():
     class _Config(Config):
         env = Choice(
-            ["prod", "local", "staging"],
-            cast_function=str.lower,
-            default="prod"
+          ["prod", "local", "staging"], 
+          cast_function=str.lower,
+          default="prod"
         )
-
+    
     _config = _Config(Env())
     return CONFIG_FILES[_config.env]
 
 
 class AppConfig(Config):
     env = Choice(
-        ["prod", "local", "staging"],
+        ["prod", "local", "staging"], 
         cast_function=str.lower,
         default="prod"
     )
     ...
 
 
 config = AppConfig(Env(), Yaml(get_config_file()))
 ```
-
-### Fail fast
-
-Very often it is helpful to check app configs existence and validate values before the app does something.
-To achieve this `Config` class runs `check` as the last step in it's `__init__` method.
-`check` recursively gets from storage and verifies all defined config attributes.
-When this behaviour is not desirable for some reason user can set flag `fail_fast` to `False`:
-
-```python
-from pkonfig import Config, DotEnv, ConfigValueNotFoundError
-
-
-class AppConfig(Config):
-    foo: str
-
-
-try:
-    config = AppConfig(DotEnv(".env"))
-except ConfigValueNotFoundError as exc:
-    print(exc)  # config.foo not found
-
-config = AppConfig(DotEnv(".env"), fail_fast=False) # No error raised
-config.foo  # This line actually causes `config.foo not found` exception
-```
```

### Comparing `pkonfig-2.0.0/pkonfig/storage/env.py` & `pkonfig-2.0b0/pkonfig/storage/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 import os
-from typing import Any
+from typing import Any, Optional, Tuple
 
-from pkonfig.storage.base import (
-    DEFAULT_DELIMITER,
-    DEFAULT_PREFIX,
-    BaseStorage,
-    DictStorage,
-    EnvKeyConverter,
-    InternalKey,
-)
+from pkonfig.base import BaseStorage, InternalKey, Storage
 
+DEFAULT_PREFIX = "APP"
+DEFAULT_DELIMITER = "_"
 
-class Env(BaseStorage):
+
+class EnvMixin:
+    # pylint: disable=too-few-public-methods
 
     def __init__(
+        self, delimiter=DEFAULT_DELIMITER, prefix=Optional[DEFAULT_PREFIX]
+    ) -> None:
+        self.prefix = prefix
+        self.delimiter = delimiter
+
+    def to_key(self, internal_key: InternalKey) -> str:
+        if self.prefix:
+            return self.delimiter.join((self.prefix, *internal_key))
+        return self.delimiter.join(internal_key)
+
+
+class Env(BaseStorage, EnvMixin):
+    def __init__(
         self, delimiter=DEFAULT_DELIMITER, prefix=DEFAULT_PREFIX, **defaults
     ) -> None:
-        super().__init__()
-        self._converter = EnvKeyConverter(prefix=prefix, delimiter=delimiter)
-        self._default = DictStorage(**defaults)
+        super().__init__(delimiter=delimiter, prefix=prefix)
+        self.default = Storage(defaults)
 
-    def __getitem__(self, key: InternalKey) -> Any:
-        str_key = self._converter.to_key(key)
+    def __getitem__(self, key: Tuple[str, ...]) -> Any:
+        str_key = self.to_key(key)
         upper_str_key = str_key.upper()
         if upper_str_key in os.environ:
             return os.environ[upper_str_key]
 
         if str_key in os.environ:
             return os.environ[str_key]
 
-        return self._default[key]
+        return self.default[key]
+
+    def __len__(self) -> int:
+        return len(os.environ)
```

### Comparing `pkonfig-2.0.0/PKG-INFO` & `pkonfig-2.0b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: pkonfig
-Version: 2.0.0
+Version: 2.0b0
 Summary: Pythonic agile application configuration helpers
-License: MIT
-Keywords: config,configuration,configurations,settings,env,environment,environments,dotenv,application,python-config,yaml,toml,ini
+Home-page: https://github.com/ngladkikh/pkonfig
 Author: Nikita Gladkikh
 Author-email: gladkikh.nikita@gmail.com
-Requires-Python: >=3.9,<4.0
+Maintainer: Nikita Gladkikh
+Maintainer-email: gladkikh.nikita@gmail.com
+License: MIT
+Keywords: config,configuration,configurations,settings,env,environment,environments,dotenv,application,python-config,yaml,toml,ini
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Provides-Extra: toml
-Provides-Extra: yaml
-Requires-Dist: pyyaml ; extra == "yaml"
-Requires-Dist: tomli ; (python_version < "3.11") and (extra == "toml")
-Project-URL: documentation, https://github.com/ngladkikh/pkonfig
-Project-URL: homepage, https://github.com/ngladkikh/pkonfig
-Project-URL: repository, https://github.com/ngladkikh/pkonfig
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: yaml
+Provides-Extra: toml
+License-File: LICENSE
 
 # PKonfig
 
 __P__ stands for __Python__.
 
 [![pypi](https://img.shields.io/pypi/v/pkonfig.svg)](https://pypi.python.org/pypi/pkonfig)
 [![downloads](https://img.shields.io/pypi/dm/pkonfig)](https://pepy.tech/project/pkonfig)
@@ -44,29 +45,29 @@
 [![Code Style - isort](https://img.shields.io/badge/Code%20Style-isort-%231674b1)](https://pycqa.github.io/isort/)
 [![codecov](https://codecov.io/github/ngladkikh/pkonfig/branch/main/graph/badge.svg?token=VDRSB1XUFH)](https://codecov.io/github/ngladkikh/pkonfig)
 
 ## Prerequisites
 
 - Pythonic configuration management helpers.
 - Multiple sources of configs (environment variables, dotenv files, YAML, JSON, TOML, INI)
-  with agile order configuration.
+with agile order configuration.
 - Configs validation mechanics based on type hints or user defined classes.
 - Minimal external dependencies.
 - Follow [Fail-fast](https://en.wikipedia.org/wiki/Fail-fast) principle.
 - Autocomplete in modern IDEs.
 
 ## Features
 
-- User defined config source order: Define the order in which PKonfig looks for configuration values.
-- Multilevel configs for environment variables and dotenv config sources: Allows for more granular control over configuration values.
-- Custom aliases for fields or groups of configs: Create custom aliases for configuration values to make them easier to reference in code.
-- Configs type casting: Automatically cast configuration values to the correct data type.
-- Config values validation based on type and/or value: Validate configuration values to ensure they meet specific requirements.
-- High performance: Designed to be fast and efficient.
-- Extendable API: Easily extend PKonfig to meet your specific needs.
+- User defined config source order.
+- Multilevel configs for environment variables and dotenv config sources.
+- Custom aliases for fields or groups of configs.
+- Configs type casting
+- Config values validation based on type and/or value.
+- High performance.
+- Extendable API.
 
 ## Installation
 
 To install basic PKonfig without YAML and TOML support run:
 
 ```bash
 pip install pkonfig
@@ -86,49 +87,46 @@
 
 And if both TOML and YAML is needed:
 
 ```bash
 pip install pkonfig[toml,yaml]
 ```
 
-For production no __.env__ files are needed but proper environment variables should be set.
-In case some of required variables missing __ConfigValueNotFoundError__ exception raised while __AppConfig__
+For production no __.env__ files are needed but propper environment variables should be set.
+In case some of required variables missing __KeyError__ exception raised while __AppConfig__
 instantiation.
 
 ## Quickstart
 
-The Config class is a Pythonic configuration management helper designed
-to provide a simple way of managing multiple sources of configuration values in your application.
 The most basic usage example when environment variables are used for production
 environment and DotEnv files are used for local development.
 
 Create __config__ module __config.py__:
 
 ```python
-from typing import Literal
-from pkonfig import Config, LogLevel, Choice, Str, Int
-from pkonfig.storage import Env
-from pkonfig import DotEnv
+from pkonfig import Config, Env, LogLevel, Choice, Storage
+from storage import DotEnv
 
 
 class PG(Config):
-    host: str = Str("localhost")
-    port: int = Int(5432)
-    user: str = Str("postgres")
-    password: str = Str("postgres")
+  host = "localhost"
+  port = 5432
+  user = "postgres"
+  password = "postgres"
 
 
 class AppConfig(Config):
-    db1 = PG()
-    db2 = PG()
-    log_level: int = LogLevel("INFO")
-    env: Literal["local", "prod", "test"] = Choice(["local", "prod", "test"], default="prod")
+  db1 = PG()
+  db2 = PG()
+  log_level = LogLevel("INFO")
+  env = Choice(["local", "prod", "test"], default="prod")
 
 
-config = AppConfig(DotEnv(".env"), Env())
+storage = Storage(DotEnv(".env", missing_ok=True), Env())
+config = AppConfig(storage)
 ```
 
 For local development create DotEnv file in root app folder __.env__:
 
 ```dotenv
 APP_DB1_HOST=10.10.10.10
 APP_DB1_USER=user
@@ -138,77 +136,66 @@
 ```
 
 Then elsewhere in app you could run:
 
 ```python
 from config import config
 
-print(config.env)           # 'local'
+print(config.env)           # local
 print(config.log_level)     # 20
-print(config.db.host)       # 'localhost'
+print(config.db.host)       # localhost
 print(config.db.port)       # 5432
-print(config.db.user)       # 'postgres'
-print(config.db.password)   # 'postgres'
+print(config.db.user)       # postgres
+print(config.db.password)   # postgres
 ```
 
 ## Usage
 
 ### Config sources
 
 __PKonfig__ implements several config sources out of the box.
-Use `DictStorage` if some defaults should be stored from code rather than from field default values:
-
-```python
-from pkonfig import Config, Str, DictStorage
-
-
-class AppConfig(Config):
-    foo: str = Str()    # foo has no default value and raise an exception if value not found in storage
-
-
-CONFIG = AppConfig(DictStorage(foo="baz"))
-print(CONFIG.foo)   # 'baz'
-```
+All config sources implement `Mapping` protocol and default values could be set up during initialization.
 
 #### Environment variables
 
 The most common way to configure application is environment variables.
 To parse environment variables and store values in multilevel structure class `Env` could be used.
-Common pattern is naming variables with multiple words describing the exact purpose
+Common pattern is naming variables with multiple words describing the exact purpose 
 more precise: __PG_HOST__, __PG_PORT__ and __REDIS_HOST__, __REDIS_PORT__ could be treated as two groups:
 
 - PG
-    - HOST
-    - PORT
+  - HOST
+  - PORT
 - REDIS
-    - HOST
-    - PORT
+  - HOST
+  - PORT
 
 PKonfig respects this convention so that `Env` has two optional arguments:
 
 - `delimiter` string that will be used to split configuration levels taken from keys;
 - `prefix` string that is used to identify keys that are related to the given app and omit everything else.
 
 ```python
 from os import environ
-from pkonfig.storage import Env
+from pkonfig import Env
+
 
 environ["APP_OUTER"] = "foo"
 environ["APP_INNER_KEY"] = "baz"
 environ["NOPE"] = "qwe"
 
-source = Env(delimiter="_", prefix="APP")
+source = Env(delimiter="_", prefix="APP", some_key="some")
 
-print(source[("outer",)])  # foo
-print(source[("inner", "key")])  # baz
-print(source[("nope",)])  # raises KeyError
+print(source[("outer",)])          # foo
+print(source[("inner", "key")])    # baz
+print(source[("nope",)])           # raises KeyError
 ```
 
 `Env` ignores key cases and ignores all keys starting not from __prefix__.
-To change this behaviour set __prefix__ to `None` or an empty string.
+To change this behaviour set __prefix__ to `None`.
 In this case you will get all key value pairs:
 
 ```python
 from os import environ
 from pkonfig import Env
 
 environ["NOPE"] = "qwe"
@@ -222,53 +209,54 @@
 
 In the same manner as environment variables DotEnv files could be used.
 `DotEnv` requires file name as a string or a path and also accepts `delimiter` and `prefix` optional arguments.
 `missing_ok` argument defines whether `DotEnv` raises exception when given file not found.
 When file not found and `missing_ok` is set `DotEnv` contains empty dictionary.
 
 ```python
-from pkonfig import DotEnv
+
+from storage import DotEnv
 
 config_source = DotEnv("test.env", delimiter="_", prefix="APP", missing_ok=True)
 ```
 
 #### Ini
 
-__INI__ files are quite common and class `Ini`
-is build on top of [`configparser.ConfigParser`](https://docs.python.org/3/library/configparser.html).
+__INI__ files are quite common and class `Ini` 
+is build on top of [`configparser.ConfigParser`](https://docs.python.org/3/library/configparser.html):
+
+```python
 
-**config.ini** file example:
+from storage import Ini
+
+storage = Ini("config.ini", missing_ok=False)
+print(storage[("bitbucket.org", "User")])  # hg
+print(storage[("bitbucket.org", "ServerAliveInterval")])  # 45
+```
+
+In case when __config.ini__:
 
 ```ini
 [DEFAULT]
 ServerAliveInterval = 45
 
 [bitbucket.org]
 User = hg
 ```
 
-Then in Python code:
-
-```python
-from pkonfig.storage import Ini
-
-storage = Ini("config.ini", missing_ok=False)
-print(storage[("bitbucket.org", "User")])  # hg
-print(storage[("bitbucket.org", "ServerAliveInterval")])  # 45
-```
-
 `Ini` also accepts `missing_ok` argument to ignore missing file.
 Most of `ConfigParser` arguments are also accepted to modify parser behaviour.
 
 #### Json
 
 `Json` class uses `json.load` to read given JSON file and respects `missing_ok` argument:
 
 ```python
-from pkonfig.storage import Json
+
+from storage import Json
 
 storage = Json("config.json", missing_ok=False)
 ```
 
 #### Yaml
 
 To parse YAML files [PyYaml](https://pyyaml.org/wiki/PyYAMLDocumentation) could be used wrapped with `Yaml` class:
@@ -293,108 +281,107 @@
 ### Source order
 
 Any source for `BaseConfig` should implement `Mapper` protocol.
 So it is easy to implement custom or combine existing implementations.
 Recommended way to combine multiple sources of configs is `ChainMap`:
 
 ```python
-from pkonfig import Config, Env, Yaml, DotEnv, Str
-
-
-class AppConfig(Config):
-    foo: str = Str()
-
+from pkonfig import Env, Yaml, Storage
+from storage import DotEnv
 
-config = AppConfig(
-    DotEnv("test.env", missing_ok=True),
-    Env(),
-    Yaml("base_config.yaml"),
+config_source = Storage(
+  DotEnv("test.env", missing_ok=True),
+  Env(),
+  Yaml("base_config.yaml")
 )
 ```
 
-In this example we created `AppConfig` that looks for key until finds one in the given mappers sequence.
+In this example we created `ChainMap` that looks for key until finds one in the given mappers sequence.
 The first one source for configs is **test.env** file that might not exist and could be used for local development only.
-Then environment variables are used as the second one config source.
-The last one is **base_config.yaml** that should exist or `FileNotFoundError` exception raised.
-You can customize source order.
+Environment variables are used as the second one config source.
+Dotenv file will be preferred source in this example.
+The last one source is **base_config.yaml** that should exist or `FileNotFoundError` exception raised.
+
+You can customize source order in this way or even create your own logic implementing
+`Mapper` protocol.
 
 ### Config
 
 To implement application config class user should inherit from `pkonfig.config.Config` class and define
 required fields:
 
 ```python
-from pkonfig import Config, Float, Int, DictStorage
+from pkonfig import Config
 
 
 class AppConfig(Config):
-    foo: float = Float()
-    baz: int = Int()
+    foo: float
+    baz: int
 
 
-config = AppConfig(DictStorage(**{"foo": "0.33", "baz": 1}))
+storage = {"foo": "0.33", "baz": 1}
+config = AppConfig(storage)
 
 print(config.foo)   # 0.33
 print(config.baz)   # 1
 ```
 
 To build more granular config structure:
 
 ```python
-from pkonfig import Config, DictStorage, Float, Int, Str
+from pkonfig import Config
 
 
 class Inner(Config):
-    key: str = Str()
+    key: str
 
 
 class AppConfig(Config):
     inner = Inner()
-    foo: float = Float()
-    baz: int = Int()
+    foo: float
+    baz: int
 
 
-storage = DictStorage(
-    **{
-        "foo": "0.33",
-        "baz": 1,
-        "inner": {"key": "value"}
-    }
-)
+storage = {
+    "foo": "0.33", 
+    "baz": 1, 
+    "inner": {"key": "value"}
+}
 config = AppConfig(storage)
 
 print(config.inner.key)   # value
 ```
 
 ### Multilevel Config
 
 Grouping might be useful when there are lots of config parameters.
-To achieve this `Config` class should be inherited like:
+To achieve this `EmbeddedConfig` class should be inherited:
 
 ```python
-from pkonfig import Config, DotEnv, Str, Int
+from pkonfig import Config
+from storage import DotEnv
 
 
 class PgConfig(Config):
-    host: str = Str("localhost")
-    port: int = Int(5432)
+  host: str
+  port: int = 5432
 
 
 class RedisConfig(Config):
-    host: str = Str("localhost")
-    port: int = Int(6379)
+  host: str
+  port: int = 6379
 
 
 class AppConfig(Config):
-    pg = PgConfig()
-    redis = RedisConfig()
+  pg = PgConfig()
+  redis = RedisConfig()
 
 
 config = AppConfig(
-    DotEnv(".env", delimiter="__", prefix="APP")
+  DotEnv(".env", delimiter="__", prefix="APP")
 )
 
 print(config.pg.host)  # db_host
 print(config.pg.port)  # 6432
 print(config.redis.host)  # redis
 ```
 
@@ -404,34 +391,35 @@
 APP__PG__PORT=6432
 APP__REDIS__HOST=redis
 ```
 In this example we customized delimiter with two underscores, default is '**_**'.
 
 ### Aliases
 
-All __Config__ fields accept __alias__ argument.
+All __Config__ fields accept __alias__ argument. 
 When storage class searches for config attribute in its source either attribute
 name is used or alias when it is set.
 
 __config.py__:
 
 ```python
-from pkonfig import Config, Int, Str, DotEnv
+from pkonfig import Config, Int, Str
+from storage import DotEnv
 
 
 class HostConfig(Config):
-    host: str = Str("localhost")
-    port: int = Int(5432)
-    user: str = Str("user")
-    password = Str(alias="pass")
+  host: str
+  port: int
+  user: str
+  password = Str(alias="pass")
 
 
 class AppConfig(Config):
-    pg = HostConfig(alias="db")
-    foo_baz = Int(alias="my_alias")
+  pg = HostConfig(alias="db")
+  foo_baz = Int(alias="my_alias")
 
 
 config = AppConfig(DotEnv(".env", delimiter="__"))
 ```
 
 __.env__ content:
 
@@ -440,15 +428,15 @@
 APP__DB__PORT=6432
 APP__DB__PASS=password
 APP__DB__USER=postgres
 APP__MY_ALIAS=123
 ```
 
 In this example storage will seek in dotenv file parameters named by given alias.
-Elsewhere in the app:
+Elsewhere in an app:
 
 ```python
 from config import config
 
 
 print(config.foo_baz)       # 123
 print(config.pg.password)   # password
@@ -469,102 +457,131 @@
 class AppConfig(Config):
     foo: str
     baz: int
     flag: bool
     file: Path
 ```
 
+#### Using default values:
+
+```python
+from pathlib import Path
+from pkonfig import Config
+
+
+class AppConfig(Config):
+    foo = "some"
+    baz = 1
+    flag = False
+    file = Path("some.text")
+```
+
+Given values will be used as default values.
+
+#### Using PKonfig fields directly
+
+```python
+from pkonfig import Config, PathField, Str, Int, Bool
+
+
+class AppConfig(Config):
+    foo = Str()
+    baz = Int()
+    flag = Bool()
+    file = PathField()
+```
+
 #### Caching
 
 All __PKonfig__ field types are Python descriptors that are responsible for type casting and data validation.
 In most cases there is no need to do this job every time the value is accessed.
 To avoid undesirable calculations caching is used.
-So that type casting and validation is done only once during `Config` object initialization.
+So that type casting and validation is done only once 
+during `Config` object initialization.
+In case when configuration may change during application lifecycle user may disable this behaviour:
+
+```python
+from pkonfig import Config, Int
+
+
+class AppConfig(Config):
+    attr = Int(no_cache=True)
+```
+
+In given example `attr` will do type casting and validation every time this attribute is accessed.
 
 #### Default values
 
 If value is not set in config source user can use default value.
 `None` could be used as default value:
 
 ```python
-from pkonfig import Config, Int, Str, DictStorage
+from pkonfig import Config, Int, Str
 
 
 class AppConfig(Config):
     int_attr = Int(None)
     str_attr = Str(None)
 
-config = AppConfig(DictStorage())
+config = AppConfig({})
 print(config.str_attr)    # None
 print(config.int_attr)    # None
 ```
 
-When `None` is default value the field is treated as nullable.
+When `None` is default value field is treated as nullable.
 
 #### Field nullability
 
 To handle type casting and validation fields should not be nullable.
 In case `None` is a valid value and should be used without casting and validation
 option `nullable` could be set:
 
 ```python
-from pkonfig import Int, Config, DictStorage
+from pkonfig import Int, Config
 
 
 class AppConfig(Config):
     int_attr = Int(nullable=True)
 
-config = AppConfig(DictStorage(int_attr=None))
+config = AppConfig(dict(int_attr=None))
 print(config.int_attr)    # None
 ```
 
-In this example when `None` comes from storage type casting and validation is omitted.
-
-By default, fields are treated as not nullable:
-
-```python
-from pkonfig import Int, Config, DictStorage
-
-
-class AppConfig(Config):
-    int_attr = Int(default=1)
-
-config = AppConfig(DictStorage(int_attr=None))  # ValueError("Not nullable") is raised here
-```
+In this example `None` comes from storage and type casting is omitted.
 
 ### Custom descriptor or property
 
 ```python
-from pkonfig import Config, Bool, DictStorage, Str
+from pkonfig import Config
 
 
 class AppConfig(Config):
-    flag: bool = Bool(True)
-    baz: str = Str("test")
-
+    flag = True
+    baz = "test"
+    
     @property
     def value(self):
-        return self.flag and self.baz == "test"
+        return self.flag and self.baz == "test" 
 
 
-config = AppConfig(DictStorage())
+config = AppConfig({})
 print(config.value)  # True
 ```
 
 ### Custom field types
 
 User can customize how field validation and casting is done.
 The recommended way is to implement `validate` method:
 
 ```python
 from pkonfig import Config, Int
 
 
 class OnlyPositive(Int):
-    def validate(self, value) -> None:
+    def validate(self, value):
         if value < 0:
             raise ValueError("Only positive values accepted")
 
 
 class AppConfig(Config):
     positive = OnlyPositive()
 ```
@@ -572,15 +589,14 @@
 Custom type casting is also available.
 To achieve this user should inherit abstract class `Field` and implement method `cast`:
 
 ```python
 from typing import List
 from pkonfig import Field
 
-
 class ListOfStrings(Field):
     def cast(self, value: str) -> List[str]:
         return value.split(",")
 ```
 
 ### Available fields
 
@@ -590,14 +606,16 @@
 - int -> `Int`
 - float -> `Float`
 - Decimal -> `DecimalField`
 - str -> `Str`
 - bytes -> `Byte`
 - bytearray -> `ByteArray`
 
+The only reason to use this types directly is customising field nullability and cache policy.
+
 #### PathField
 
 Basic path type that is parental for other two types and is used when you define field using `pathlib.Path`.
 This type raises `FileNotFoundError` exception during initialization if given path doesn't exist:
 
 ```python
 from pkonfig import Config, PathField
@@ -620,110 +638,145 @@
 
 #### EnumField
 
 This field uses custom enum to validate input and cast it to given `Enum`:
 
 ```python
 from enum import Enum
-from pkonfig import Config, EnumField, DictStorage, Int
+from pkonfig import Config, EnumField
 
 
 class UserType(Enum):
-    guest = Int(1)
-    user = Int(2)
-    admin = Int(3)
+    guest = 1
+    user = 2
+    admin = 3
 
 
 class AppConfig(Config):
     user_type = EnumField(UserType)
 
 
-config = AppConfig(DictStorage(user_type="admin"))
+config = AppConfig({"user_type": "admin"})
 print(config.user_type is UserType.admin)  # True
 ```
 
 #### LogLevel
 
 `LogLevel` field is useful to define `logging` level through configs.
-`LogLevel` accepts strings that define log level and casts
+`LogLevel` accepts strings that define log level and casts 
 that string to `logging` level integer value:
 
 ```python
 import logging
-from pkonfig import Config, LogLevel, DictStorage
+from pkonfig import Config, LogLevel
 
 
 class AppConfig(Config):
     some_level = LogLevel()
     another_level = LogLevel()
 
 
 config = AppConfig(
-    DictStorage(
-        some_level="info",
-        another_level="Debug",
-    )
+    {
+        "some_level": "info",
+        "another_level": "Debug",
+    }
 )
 
 print(config.some_level)        # 20
 print(config.another_level)     # 10
 
 print(config.another_level is logging.DEBUG)     # True
 ```
 
 #### Choice
 
 `Choice` field validates that config value is a member of the given sequence and also does optional type casting:
 
 ```python
-from pkonfig import Config, Choice, DictStorage
+from pkonfig import Config, Choice
 
 
 class AppConfig(Config):
     one_of_attr = Choice([10, 100], cast_function=int)
 
 
-config = AppConfig(DictStorage(one_of_attr="10"))
+config = AppConfig({"one_of_attr": "10"})
 print(config.one_of_attr == 10)  # True
 
-config = AppConfig(DictStorage(one_of_attr="2"))    # raises TypeError exception
+config = AppConfig({"one_of_attr": "2"})    # raises TypeError exception
 ```
 
 When `cast_function` is not given raw values from storage are used.
 
 #### DebugFlag
 
 `DebugFlag` helps to set widely used __debug__ option.
 `DebugFlag` ignores value case and treats __'true'__ string as `True` and any other value as `False`:
 
 ```python
-from pkonfig import Config, Bool, DictStorage
+from pkonfig import Config, DebugFlag
 
 
 class AppConfig(Config):
-    lower_case = Bool()
-    upper_case = Bool()
-    random_string = Bool()
+    lower_case = DebugFlag()
+    upper_case = DebugFlag()
+    random_string = DebugFlag()
 
 
 config = AppConfig(
-    DictStorage(
-        lower_case="true",
-        upper_case="TRUE",
-        random_string="foo",
-    )
+  {
+    "lower_case": "true",
+    "upper_case": "TRUE",
+    "random_string": "foo",
+  }
 )
 print(config.lower_case)        # True
 print(config.upper_case)        # True
 print(config.random_string)     # False
 ```
 
+### Types to Fields mapping
+
+All fields for `BaseConfig` children classes are converted to descriptors internally.
+Class `pkonfig.config.DefaultMapper` defines how field types will be replaced with descriptors.
+This mapping is used by default:
+```
+{
+    bool: Bool,
+    int: Int,
+    float: Float,
+    str: Str,
+    bytes: Byte,
+    bytearray: ByteArray,
+    Path: PathField,
+    Decimal: DecimalField,
+}
+```
+
+When field type is not found in this mapper it is ignored and won't be taken from storage source while resolving.
+
+User can modify default mapper giving dictionary of types and appropriate fields:
+
+```python
+from decimal import Decimal
+from pkonfig import Config, DefaultMapper, DecimalField
+
+
+class AppConfig(Config):
+    _mapper = DefaultMapper({float: DecimalField})
+    foo: float
+
+config = AppConfig(dict(foo=1/3))
+assert isinstance(config.foo, Decimal)  # True
+```
+
 ### Per-environment config files
 
-When your app is configured with different configuration files
+When your app is configured with different configuration files 
 and each file is used only in an appropriate environment you can create a function
 to find which file should be used:
 
 ```python
 from pkonfig import Env, Config, Choice
 
 
@@ -733,24 +786,24 @@
     "local": "configs/local.yaml",
 }
 
 
 def get_config_file():
     class _Config(Config):
         env = Choice(
-            ["prod", "local", "staging"],
-            cast_function=str.lower,
-            default="prod"
+          ["prod", "local", "staging"], 
+          cast_function=str.lower,
+          default="prod"
         )
-
+    
     _config = _Config(Env())
     return CONFIG_FILES[_config.env]
 ```
 
-__get_config_file__ uses environment variables and predefined config files paths
+__get_config_file__ uses environment variables and predefined config files pathes
 to check whether __APP_ENV__ var is set, validate this variable and return appropriate
 config file name.
 Then actual application configuration:
 
 ```python
 from pkonfig import Env, Yaml, Config, Choice
 
@@ -761,51 +814,27 @@
     "local": "configs/local.yaml",
 }
 
 
 def get_config_file():
     class _Config(Config):
         env = Choice(
-            ["prod", "local", "staging"],
-            cast_function=str.lower,
-            default="prod"
+          ["prod", "local", "staging"], 
+          cast_function=str.lower,
+          default="prod"
         )
-
+    
     _config = _Config(Env())
     return CONFIG_FILES[_config.env]
 
 
 class AppConfig(Config):
     env = Choice(
-        ["prod", "local", "staging"],
+        ["prod", "local", "staging"], 
         cast_function=str.lower,
         default="prod"
     )
     ...
 
 
 config = AppConfig(Env(), Yaml(get_config_file()))
 ```
-
-### Fail fast
-
-Very often it is helpful to check app configs existence and validate values before the app does something.
-To achieve this `Config` class runs `check` as the last step in it's `__init__` method.
-`check` recursively gets from storage and verifies all defined config attributes.
-When this behaviour is not desirable for some reason user can set flag `fail_fast` to `False`:
-
-```python
-from pkonfig import Config, DotEnv, ConfigValueNotFoundError
-
-
-class AppConfig(Config):
-    foo: str
-
-
-try:
-    config = AppConfig(DotEnv(".env"))
-except ConfigValueNotFoundError as exc:
-    print(exc)  # config.foo not found
-
-config = AppConfig(DotEnv(".env"), fail_fast=False) # No error raised
-config.foo  # This line actually causes `config.foo not found` exception
-```
```

