# Comparing `tmp/neuro_config_client-24.4.1.tar.gz` & `tmp/neuro_config_client-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro_config_client-24.4.1.tar", last modified: Sun Apr 28 16:45:59 2024, max compression
+gzip compressed data, was "neuro_config_client-24.4.2.tar", last modified: Tue Apr 30 15:42:49 2024, max compression
```

## Comparing `neuro_config_client-24.4.1.tar` & `neuro_config_client-24.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:45:59.267490 neuro_config_client-24.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:45:59.263490 neuro_config_client-24.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.github/actionlint-matcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:45:59.267490 neuro_config_client-24.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.github/workflows/remove-automerge.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.github/workflows/setup-automerge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-28 16:45:59.267490 neuro_config_client-24.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:45:59.267490 neuro_config_client-24.4.1/neuro_config_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/neuro_config_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/neuro_config_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/neuro_config_client/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    42485 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/neuro_config_client/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/neuro_config_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:45:59.267490 neuro_config_client-24.4.1/neuro_config_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-28 16:45:59.000000 neuro_config_client-24.4.1/neuro_config_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-28 16:45:59.000000 neuro_config_client-24.4.1/neuro_config_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:45:59.000000 neuro_config_client-24.4.1/neuro_config_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:45:59.000000 neuro_config_client-24.4.1/neuro_config_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-28 16:45:59.000000 neuro_config_client-24.4.1/neuro_config_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-28 16:45:59.000000 neuro_config_client-24.4.1/neuro_config_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-28 16:45:59.267490 neuro_config_client-24.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:45:59.267490 neuro_config_client-24.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    70969 2024-04-28 16:45:50.000000 neuro_config_client-24.4.1/tests/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:42:49.029633 neuro_config_client-24.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:42:49.025633 neuro_config_client-24.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.github/actionlint-matcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:42:49.029633 neuro_config_client-24.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.github/workflows/remove-automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.github/workflows/setup-automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 15:42:49.029633 neuro_config_client-24.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:42:49.029633 neuro_config_client-24.4.2/neuro_config_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/neuro_config_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/neuro_config_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13474 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/neuro_config_client/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42447 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/neuro_config_client/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/neuro_config_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:42:49.029633 neuro_config_client-24.4.2/neuro_config_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 15:42:48.000000 neuro_config_client-24.4.2/neuro_config_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 15:42:49.000000 neuro_config_client-24.4.2/neuro_config_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:42:48.000000 neuro_config_client-24.4.2/neuro_config_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:42:48.000000 neuro_config_client-24.4.2/neuro_config_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 15:42:48.000000 neuro_config_client-24.4.2/neuro_config_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 15:42:48.000000 neuro_config_client-24.4.2/neuro_config_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-30 15:42:49.029633 neuro_config_client-24.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:42:49.029633 neuro_config_client-24.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    70969 2024-04-30 15:42:38.000000 neuro_config_client-24.4.2/tests/test_factories.py
```

### Comparing `neuro_config_client-24.4.1/.github/workflows/ci.yaml` & `neuro_config_client-24.4.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/.github/workflows/remove-automerge.yml` & `neuro_config_client-24.4.2/.github/workflows/remove-automerge.yml`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/.github/workflows/setup-automerge.yml` & `neuro_config_client-24.4.2/.github/workflows/setup-automerge.yml`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/.gitignore` & `neuro_config_client-24.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/.pre-commit-config.yaml` & `neuro_config_client-24.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/LICENSE` & `neuro_config_client-24.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/PKG-INFO` & `neuro_config_client-24.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-config-client
-Version: 24.4.1
+Version: 24.4.2
 Summary: Internal client for Neu.ro config service
 Home-page: https://github.com/neuro-inc/neuro-config-client
 License: Apache 2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `neuro_config_client-24.4.1/neuro_config_client/__init__.py` & `neuro_config_client-24.4.2/neuro_config_client/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/neuro_config_client/client.py` & `neuro_config_client-24.4.2/neuro_config_client/client.py`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/neuro_config_client/entities.py` & `neuro_config_client-24.4.2/neuro_config_client/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,17 +477,17 @@
 @dataclass(frozen=True)
 class ResourcePoolType:
     name: str
     min_size: int = 0
     max_size: int = 1
     idle_size: int = 0
     cpu: float = 1.0
-    available_cpu: float = 1.0
+    available_cpu: float = 1.0  # TODO: deprecated, use cpu instead
     memory: int = 2**30  # 1gb
-    available_memory: int = 2**30  # 1gb
+    available_memory: int = 2**30  # TODO: deprecated, use memory instead
     disk_size: int = 150 * 2**30  # 150gb
     nvidia_gpu: int | None = None
     amd_gpu: int | None = None
     intel_gpu: int | None = None
     price: Decimal = Decimal()
     currency: str | None = None
     tpu: TPUResource | None = None
```

### Comparing `neuro_config_client-24.4.1/neuro_config_client/factories.py` & `neuro_config_client-24.4.2/neuro_config_client/factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,25 +247,25 @@
             ],
         )
 
     def create_resource_pool_type(self, payload: dict[str, Any]) -> ResourcePoolType:
         tpu = None
         if payload.get("tpu"):
             tpu = self.create_tpu_resource(payload["tpu"])
+        cpu = payload.get("cpu", ResourcePoolType.cpu)
+        memory = payload.get("memory", ResourcePoolType.memory)
         return ResourcePoolType(
             name=payload["name"],
             min_size=payload.get("min_size", ResourcePoolType.min_size),
             max_size=payload.get("max_size", ResourcePoolType.max_size),
             idle_size=payload.get("idle_size", ResourcePoolType.idle_size),
-            cpu=payload.get("cpu", ResourcePoolType.cpu),
-            available_cpu=payload.get("available_cpu", ResourcePoolType.available_cpu),
-            memory=payload.get("memory", ResourcePoolType.memory),
-            available_memory=payload.get(
-                "available_memory", ResourcePoolType.available_memory
-            ),
+            cpu=cpu,
+            available_cpu=payload.get("available_cpu") or cpu,
+            memory=memory,
+            available_memory=payload.get("available_memory") or memory,
             nvidia_gpu=payload.get("nvidia_gpu"),
             amd_gpu=payload.get("amd_gpu"),
             intel_gpu=payload.get("intel_gpu"),
             price=Decimal(payload.get("price", ResourcePoolType.price)),
             currency=payload.get("currency"),
             tpu=tpu,
             is_preemptible=payload.get(
```

### Comparing `neuro_config_client-24.4.1/neuro_config_client.egg-info/PKG-INFO` & `neuro_config_client-24.4.2/neuro_config_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-config-client
-Version: 24.4.1
+Version: 24.4.2
 Summary: Internal client for Neu.ro config service
 Home-page: https://github.com/neuro-inc/neuro-config-client
 License: Apache 2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `neuro_config_client-24.4.1/neuro_config_client.egg-info/SOURCES.txt` & `neuro_config_client-24.4.2/neuro_config_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/setup.cfg` & `neuro_config_client-24.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `neuro_config_client-24.4.1/tests/test_factories.py` & `neuro_config_client-24.4.2/tests/test_factories.py`

 * *Files identical despite different names*

