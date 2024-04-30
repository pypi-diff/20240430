# Comparing `tmp/aiotx-0.0.3.tar.gz` & `tmp/aiotx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.0.3.tar", last modified: Tue Apr 30 06:12:55 2024, max compression
+gzip compressed data, was "aiotx-0.0.6.tar", last modified: Tue Apr 30 06:30:09 2024, max compression
```

## Comparing `aiotx-0.0.3.tar` & `aiotx-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     3086 2024-04-30 06:07:18.000000 aiotx-0.0.3/.gitignore
--rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)     3088 2024-04-30 06:12:55.671593 aiotx-0.0.3/PKG-INFO
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     1654 2024-04-30 06:05:14.000000 aiotx-0.0.3/README.md
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/aiotx/
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:57:05.000000 aiotx-0.0.3/aiotx/__init__.py
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/aiotx/clients/
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      291 2024-04-30 06:08:28.000000 aiotx-0.0.3/aiotx/clients/__init__.py
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      187 2024-04-30 06:08:35.000000 aiotx-0.0.3/aiotx/clients/_bitcoin_base_client.py
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      186 2024-04-30 06:08:46.000000 aiotx-0.0.3/aiotx/clients/_evm_base_client.py
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       86 2024-04-30 06:11:46.000000 aiotx-0.0.3/aiotx/exceptions.py
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/aiotx/types/
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       59 2024-04-30 06:06:35.000000 aiotx-0.0.3/aiotx/types/__init__.py
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/aiotx.egg-info/
--rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)     3088 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/PKG-INFO
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      358 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/SOURCES.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        1 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/dependency_links.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       93 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/requires.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        6 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/top_level.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      419 2024-04-30 05:38:25.000000 aiotx-0.0.3/pyproject.toml
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      114 2024-04-30 06:12:55.675593 aiotx-0.0.3/setup.cfg
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     1769 2024-04-30 06:12:20.000000 aiotx-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.364729 aiotx-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.364729 aiotx-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 06:30:04.000000 aiotx-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-30 06:30:04.000000 aiotx-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-30 06:30:04.000000 aiotx-0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-30 06:30:09.368729 aiotx-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-30 06:30:04.000000 aiotx-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/clients/_bitcoin_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 06:30:04.000000 aiotx-0.0.6/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:30:09.368729 aiotx-0.0.6/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 06:30:09.000000 aiotx-0.0.6/aiotx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-30 06:30:04.000000 aiotx-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 06:30:09.368729 aiotx-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-30 06:30:04.000000 aiotx-0.0.6/setup.py
```

### Comparing `aiotx-0.0.3/.gitignore` & `aiotx-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-0.0.3/PKG-INFO` & `aiotx-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.0.3
+Version: 0.0.6
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `aiotx-0.0.3/README.md` & `aiotx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aiotx-0.0.3/aiotx.egg-info/PKG-INFO` & `aiotx-0.0.6/aiotx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.0.3
+Version: 0.0.6
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `aiotx-0.0.3/setup.py` & `aiotx-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         "wallet",
         "transaction",
     ],
     use_scm_version=True,
     description="An asynchronous library for interacting with various cryptocurrencies and blockchains",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    version="0.0.3",
     packages=find_packages(exclude=("tests", "scripts")),
     package_data={
         "aiotx": ["py.typed"],
     },
     setup_requires=[
         "setuptools_scm",
     ],
```

