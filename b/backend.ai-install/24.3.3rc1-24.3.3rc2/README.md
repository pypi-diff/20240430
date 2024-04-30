# Comparing `tmp/backend.ai-install-24.3.3rc1.tar.gz` & `tmp/backend.ai-install-24.3.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-install-24.3.3rc1.tar", last modified: Mon Apr 29 16:32:28 2024, max compression
+gzip compressed data, was "backend.ai-install-24.3.3rc2.tar", last modified: Tue Apr 30 06:26:17 2024, max compression
```

## Comparing `backend.ai-install-24.3.3rc1.tar` & `backend.ai-install-24.3.3rc2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.248594 backend.ai-install-24.3.3rc1/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-29 16:32:28.248594 backend.ai-install-24.3.3rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.240594 backend.ai-install-24.3.3rc1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.240594 backend.ai-install-24.3.3rc1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.244594 backend.ai-install-24.3.3rc1/ai/backend/install/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/app.tcss
--rw-r--r--   0 runner    (1001) docker     (127)    21404 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.244594 backend.ai-install-24.3.3rc1/ai/backend/install/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/configs/agent.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/configs/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/configs/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/configs/manager.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/configs/storage-proxy.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/configs/webserver.conf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)    46366 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.244594 backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-keypairs.json
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-resource-presets.json
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-session-templates.json
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-set-user-main-access-keys.json
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-users.json
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/http.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/tomltool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/ai/backend/install/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.248594 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-29 16:32:28.000000 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-29 16:32:28.000000 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:28.000000 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 16:32:28.000000 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:28.000000 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:28.000000 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-29 16:32:28.000000 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-29 16:32:28.000000 backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:32:28.248594 backend.ai-install-24.3.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-29 16:32:27.000000 backend.ai-install-24.3.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.447754 backend.ai-install-24.3.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-30 06:26:17.447754 backend.ai-install-24.3.3rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.435753 backend.ai-install-24.3.3rc2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.435753 backend.ai-install-24.3.3rc2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.439753 backend.ai-install-24.3.3rc2/ai/backend/install/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/app.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)    21404 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.443753 backend.ai-install-24.3.3rc2/ai/backend/install/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/configs/agent.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/configs/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/configs/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/configs/manager.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/configs/storage-proxy.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/configs/webserver.conf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46366 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.443753 backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-keypairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-resource-presets.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-session-templates.json
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-set-user-main-access-keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-users.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/tomltool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/ai/backend/install/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:17.447754 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-30 06:26:17.000000 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-30 06:26:17.000000 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:17.000000 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 06:26:17.000000 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:17.000000 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:17.000000 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-30 06:26:17.000000 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-30 06:26:17.000000 backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:26:17.447754 backend.ai-install-24.3.3rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-30 06:26:16.000000 backend.ai-install-24.3.3rc2/setup.py
```

### Comparing `backend.ai-install-24.3.3rc1/PKG-INFO` & `backend.ai-install-24.3.3rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-install
-Version: 24.3.3rc1
+Version: 24.3.3rc2
 Summary: Backend.AI Installer
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiotools~=1.7.0
 Requires-Dist: asyncpg>=0.27.0
-Requires-Dist: backend.ai-common==24.03.3rc1
-Requires-Dist: backend.ai-plugin==24.03.3rc1
+Requires-Dist: backend.ai-common==24.03.3rc2
+Requires-Dist: backend.ai-plugin==24.03.3rc2
 Requires-Dist: click~=8.1.7
 Requires-Dist: pydantic~=2.6.4
 Requires-Dist: python-dateutil>=2.8
 Requires-Dist: rich~=13.6
 Requires-Dist: textual~=0.56.3
 Requires-Dist: tomlkit~=0.12.4
 Requires-Dist: types-aiofiles
```

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/app.tcss` & `backend.ai-install-24.3.3rc2/ai/backend/install/app.tcss`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/cli.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/common.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/common.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/configs/agent.toml` & `backend.ai-install-24.3.3rc2/ai/backend/install/configs/agent.toml`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/configs/alembic.ini` & `backend.ai-install-24.3.3rc2/ai/backend/install/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/configs/docker-compose.yml` & `backend.ai-install-24.3.3rc2/ai/backend/install/configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/configs/manager.toml` & `backend.ai-install-24.3.3rc2/ai/backend/install/configs/manager.toml`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/configs/storage-proxy.toml` & `backend.ai-install-24.3.3rc2/ai/backend/install/configs/storage-proxy.toml`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/configs/webserver.conf` & `backend.ai-install-24.3.3rc2/ai/backend/install/configs/webserver.conf`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/context.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/dev.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/dev.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/docker.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-keypairs.json` & `backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-keypairs.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-resource-presets.json` & `backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-resource-presets.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-session-templates.json` & `backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-session-templates.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-set-user-main-access-keys.json` & `backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-set-user-main-access-keys.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/fixtures/example-users.json` & `backend.ai-install-24.3.3rc2/ai/backend/install/fixtures/example-users.json`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/http.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/http.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/tomltool.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/tomltool.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/types.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/ai/backend/install/widgets.py` & `backend.ai-install-24.3.3rc2/ai/backend/install/widgets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/PKG-INFO` & `backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-install
-Version: 24.3.3rc1
+Version: 24.3.3rc2
 Summary: Backend.AI Installer
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiotools~=1.7.0
 Requires-Dist: asyncpg>=0.27.0
-Requires-Dist: backend.ai-common==24.03.3rc1
-Requires-Dist: backend.ai-plugin==24.03.3rc1
+Requires-Dist: backend.ai-common==24.03.3rc2
+Requires-Dist: backend.ai-plugin==24.03.3rc2
 Requires-Dist: click~=8.1.7
 Requires-Dist: pydantic~=2.6.4
 Requires-Dist: python-dateutil>=2.8
 Requires-Dist: rich~=13.6
 Requires-Dist: textual~=0.56.3
 Requires-Dist: tomlkit~=0.12.4
 Requires-Dist: types-aiofiles
```

### Comparing `backend.ai-install-24.3.3rc1/backend.ai_install.egg-info/SOURCES.txt` & `backend.ai-install-24.3.3rc2/backend.ai_install.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/backend_shim.py` & `backend.ai-install-24.3.3rc2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-install-24.3.3rc1/setup.py` & `backend.ai-install-24.3.3rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
         ],
     },
     'install_requires': (
         'aiofiles~=23.2.1',
         'aiohttp~=3.9.1',
         'aiotools~=1.7.0',
         'asyncpg>=0.27.0',
-        """backend.ai-common==24.03.3rc1
+        """backend.ai-common==24.03.3rc2
 """,
-        """backend.ai-plugin==24.03.3rc1
+        """backend.ai-plugin==24.03.3rc2
 """,
         'click~=8.1.7',
         'pydantic~=2.6.4',
         'python-dateutil>=2.8',
         'rich~=13.6',
         'textual~=0.56.3',
         'tomlkit~=0.12.4',
@@ -110,11 +110,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.3rc1
+    'version': """24.03.3rc2
 """,
     'zip_safe': False,
 })
```

