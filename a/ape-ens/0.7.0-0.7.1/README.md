# Comparing `tmp/ape-ens-0.7.0.tar.gz` & `tmp/ape-ens-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ens-0.7.0.tar", last modified: Tue Dec 19 01:50:31 2023, max compression
+gzip compressed data, was "ape-ens-0.7.1.tar", last modified: Tue Apr 30 14:29:02 2024, max compression
```

## Comparing `ape-ens-0.7.0.tar` & `ape-ens-0.7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:50:31.671809 ape-ens-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:50:31.667809 ape-ens-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:50:31.671809 ape-ens-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:50:31.671809 ape-ens-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-19 01:49:36.000000 ape-ens-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-12-19 01:49:36.000000 ape-ens-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-19 01:49:36.000000 ape-ens-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2023-12-19 01:50:31.671809 ape-ens-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2023-12-19 01:49:36.000000 ape-ens-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:50:31.671809 ape-ens-0.7.0/ape_ens/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-19 01:49:36.000000 ape-ens-0.7.0/ape_ens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2023-12-19 01:49:36.000000 ape-ens-0.7.0/ape_ens/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 01:49:36.000000 ape-ens-0.7.0/ape_ens/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:50:31.671809 ape-ens-0.7.0/ape_ens/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-19 01:49:36.000000 ape-ens-0.7.0/ape_ens/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-12-19 01:49:36.000000 ape-ens-0.7.0/ape_ens/utils/namehash.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-19 01:50:31.000000 ape-ens-0.7.0/ape_ens/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:50:31.671809 ape-ens-0.7.0/ape_ens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2023-12-19 01:50:31.000000 ape-ens-0.7.0/ape_ens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-12-19 01:50:31.000000 ape-ens-0.7.0/ape_ens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 01:50:31.000000 ape-ens-0.7.0/ape_ens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 01:50:31.000000 ape-ens-0.7.0/ape_ens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-12-19 01:50:31.000000 ape-ens-0.7.0/ape_ens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-19 01:50:31.000000 ape-ens-0.7.0/ape_ens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-12-19 01:49:36.000000 ape-ens-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-19 01:50:31.675809 ape-ens-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2023-12-19 01:49:36.000000 ape-ens-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 01:50:31.671809 ape-ens-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 01:49:36.000000 ape-ens-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2023-12-19 01:49:36.000000 ape-ens-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-12-19 01:49:36.000000 ape-ens-0.7.0/tests/test_ens.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-19 01:49:36.000000 ape-ens-0.7.0/tests/test_namehash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 14:28:09.000000 ape-ens-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-30 14:28:09.000000 ape-ens-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-30 14:28:09.000000 ape-ens-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-30 14:29:02.758334 ape-ens-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-30 14:28:09.000000 ape-ens-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/ape_ens/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/ape_ens/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-30 14:28:09.000000 ape-ens-0.7.1/ape_ens/utils/namehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/ape_ens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 14:29:02.000000 ape-ens-0.7.1/ape_ens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 14:28:09.000000 ape-ens-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 14:29:02.758334 ape-ens-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-30 14:28:09.000000 ape-ens-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:29:02.758334 ape-ens-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:28:09.000000 ape-ens-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-30 14:28:09.000000 ape-ens-0.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 14:28:09.000000 ape-ens-0.7.1/tests/test_ens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 14:28:09.000000 ape-ens-0.7.1/tests/test_namehash.py
```

### Comparing `ape-ens-0.7.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-ens-0.7.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-ens-0.7.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-ens-0.7.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.github/release-drafter.yml` & `ape-ens-0.7.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.github/workflows/commit.yaml` & `ape-ens-0.7.1/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.github/workflows/publish.yaml` & `ape-ens-0.7.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.github/workflows/test.yaml` & `ape-ens-0.7.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.github/workflows/title.yaml` & `ape-ens-0.7.1/.github/workflows/title.yaml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.gitignore` & `ape-ens-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/.pre-commit-config.yaml` & `ape-ens-0.7.1/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.0
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-ens-0.7.0/CONTRIBUTING.md` & `ape-ens-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/LICENSE` & `ape-ens-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/PKG-INFO` & `ape-ens-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ens
-Version: 0.7.0
+Version: 0.7.1
 Summary: ape-ens: Ape plugin for ENS argument conversion and contracts
 Home-page: https://github.com/ApeWorX/ape-ens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-ens-0.7.0/README.md` & `ape-ens-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/ape_ens/converter.py` & `ape-ens-0.7.1/ape_ens/converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ape.api import ConverterAPI
 from ape.exceptions import NetworkError, ProviderError
 from ape.logging import logger
 from ape.types import AddressType
 from ape.utils import cached_property
 from ape_ethereum.provider import Web3Provider
+from web3.exceptions import CannotHandleRequest
 from web3.main import ENS
 
 
 class ENSConversions(ConverterAPI):
     """Converts ENS names like `my-name.eth` to `0xAbCd...1234`"""
 
     address_cache: Dict[str, AddressType] = {}
@@ -23,30 +24,36 @@
             and provider.network.name in ("mainnet", "mainnet-fork")
             and provider.network.ecosystem.name == "ethereum"
         ):
             return provider
 
         # Connect to mainnet for ENS resolution
         # NOTE: May not work unless the user configures their default mainnet provider.
-        provider = self.network_manager.get_provider_from_choice("ethereum:mainnet")
-        if not isinstance(provider, Web3Provider):
+        ecosystem = self.network_manager.get_ecosystem("ethereum")
+        mainnet = ecosystem.get_network("mainnet")
+        if not (provider := mainnet.default_provider):
+            return None
+
+        elif not isinstance(provider, Web3Provider):
             logger.warning(
                 "Unable to connect to mainnet provider to "
                 "perform ENS lookup (must be a Web3Provider)"
             )
             return None
 
-        try:
-            provider.connect()
-        except ProviderError:
-            logger.warning(
-                "Unable to connect to mainnet provider to perform ENS lookup. "
-                "Try changing your default mainnet provider."
-            )
-            return None
+        if not provider.is_connected:
+            # Connect if needed.
+            try:
+                provider.connect()
+            except ProviderError:
+                logger.warning(
+                    "Unable to connect to mainnet provider to perform ENS lookup. "
+                    "Try changing your default mainnet provider."
+                )
+                return None
 
         return provider
 
     def is_convertible(self, value: Any) -> bool:
         if not isinstance(value, str):
             return False
 
@@ -61,39 +68,42 @@
 
         else:
             try:
                 provider = self.mainnet_provider
                 if not provider:
                     return False
 
-                ens = provider.web3.ens
-                if not ens:
+                elif not (ens := provider.web3.ens):
                     return False
 
-                address = ens.address(value)
+                try:
+                    address = ens.address(value)
+                except CannotHandleRequest:
+                    # Either this is not actually mainnet or our head is
+                    # pointed before ENS existed.
+                    return False
 
                 if address is not None:
                     self.address_cache[value] = address
                     return True
 
                 return False
+
             except (NetworkError, ProviderError):
                 return False
 
     def convert(self, value: str) -> AddressType:
         if value in self.address_cache:
             return self.address_cache[value]
 
-        provider = self.mainnet_provider
-        if not provider:
+        elif not (provider := self.mainnet_provider):
             # Should never get here.
             raise ValueError(f"Unable to convert ENS value '{value}'.")
 
         # TODO: Switch to using ENS SDK
-        ens = provider.web3.ens
-        if not ens:
+        if not (ens := provider.web3.ens):
             # Should never get here.
             raise ValueError(f"Unable to convert ENS value '{value}'.")
 
         address = ens.address(value)
         self.address_cache[value] = address
         return address
```

### Comparing `ape-ens-0.7.0/ape_ens/utils/namehash.py` & `ape-ens-0.7.1/ape_ens/utils/namehash.py`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/ape_ens.egg-info/PKG-INFO` & `ape-ens-0.7.1/ape_ens.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ens
-Version: 0.7.0
+Version: 0.7.1
 Summary: ape-ens: Ape plugin for ENS argument conversion and contracts
 Home-page: https://github.com/ApeWorX/ape-ens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-ens-0.7.0/ape_ens.egg-info/SOURCES.txt` & `ape-ens-0.7.1/ape_ens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/ape_ens.egg-info/requires.txt` & `ape-ens-0.7.1/ape_ens.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 ape-polygon
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
@@ -33,21 +33,21 @@
 
 [doc]
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-ens-0.7.0/pyproject.toml` & `ape-ens-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.7.0/setup.py` & `ape-ens-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "ape-polygon",  # For testing against another network named 'mainnet'
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
-        "flake8>=6.1.0,<7",  # Style linter
+        "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
         "Sphinx>=6.1.3,<7",  # Documentation generator
```

### Comparing `ape-ens-0.7.0/tests/conftest.py` & `ape-ens-0.7.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,7 +104,13 @@
     mainnet.set_default_provider("mock-mainnet")
     mainnet_fork.set_default_provider("mock-mainnet-fork")
     polygon_mainnet.set_default_provider("mock-polygon-mainnet")
 
     yield ens
 
     delete_caches()
+
+
+@pytest.fixture
+def mainnet_provider(converter):
+    _ = converter.is_convertible("test.eth")  # Set mainnet_provider
+    return converter.__dict__["mainnet_provider"]
```

### Comparing `ape-ens-0.7.0/tests/test_namehash.py` & `ape-ens-0.7.1/tests/test_namehash.py`

 * *Files identical despite different names*

