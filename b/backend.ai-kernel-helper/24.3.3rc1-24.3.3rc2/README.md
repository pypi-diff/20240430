# Comparing `tmp/backend.ai-kernel-helper-24.3.3rc1.tar.gz` & `tmp/backend.ai-kernel-helper-24.3.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-helper-24.3.3rc1.tar", last modified: Mon Apr 29 16:32:28 2024, max compression
+gzip compressed data, was "backend.ai-kernel-helper-24.3.3rc2.tar", last modified: Tue Apr 30 06:26:19 2024, max compression
```

## Comparing `backend.ai-kernel-helper-24.3.3rc1.tar` & `backend.ai-kernel-helper-24.3.3rc2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.620598 backend.ai-kernel-helper-24.3.3rc1/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-29 16:32:28.620598 backend.ai-kernel-helper-24.3.3rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.616598 backend.ai-kernel-helper-24.3.3rc1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.616598 backend.ai-kernel-helper-24.3.3rc1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.616598 backend.ai-kernel-helper-24.3.3rc1/ai/backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/ai/backend/helpers/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/ai/backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/ai/backend/helpers/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:32:28.620598 backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:32:28.620598 backend.ai-kernel-helper-24.3.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-29 16:32:28.000000 backend.ai-kernel-helper-24.3.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:19.735783 backend.ai-kernel-helper-24.3.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-30 06:26:19.735783 backend.ai-kernel-helper-24.3.3rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:19.735783 backend.ai-kernel-helper-24.3.3rc2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:19.735783 backend.ai-kernel-helper-24.3.3rc2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:19.735783 backend.ai-kernel-helper-24.3.3rc2/ai/backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/ai/backend/helpers/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/ai/backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/ai/backend/helpers/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:26:19.735783 backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:26:19.735783 backend.ai-kernel-helper-24.3.3rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-30 06:26:19.000000 backend.ai-kernel-helper-24.3.3rc2/setup.py
```

### Comparing `backend.ai-kernel-helper-24.3.3rc1/PKG-INFO` & `backend.ai-kernel-helper-24.3.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 24.3.3rc1
+Version: 24.3.3rc2
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-helper-24.3.3rc1/ai/backend/helpers/package.py` & `backend.ai-kernel-helper-24.3.3rc2/ai/backend/helpers/package.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-24.3.3rc1/backend.ai_kernel_helper.egg-info/PKG-INFO` & `backend.ai-kernel-helper-24.3.3rc2/backend.ai_kernel_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 24.3.3rc1
+Version: 24.3.3rc2
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-helper-24.3.3rc1/backend_shim.py` & `backend.ai-kernel-helper-24.3.3rc2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-24.3.3rc1/setup.py` & `backend.ai-kernel-helper-24.3.3rc2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,11 +40,11 @@
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

