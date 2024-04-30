# Comparing `tmp/aiotx-0.0.2.tar.gz` & `tmp/aiotx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.0.2.tar", last modified: Tue Apr 30 05:51:29 2024, max compression
+gzip compressed data, was "aiotx-0.0.3.tar", last modified: Tue Apr 30 06:12:55 2024, max compression
```

## Comparing `aiotx-0.0.2.tar` & `aiotx-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:51:29.774702 aiotx-0.0.2/
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     3078 2024-04-30 05:29:10.000000 aiotx-0.0.2/.gitignore
--rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)     3070 2024-04-30 05:51:29.774702 aiotx-0.0.2/PKG-INFO
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     1636 2024-04-30 05:49:52.000000 aiotx-0.0.2/README.md
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:51:29.774702 aiotx-0.0.2/aiotx/
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:34:42.000000 aiotx-0.0.2/aiotx/__init__.py
-drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:51:29.774702 aiotx-0.0.2/aiotx.egg-info/
--rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)     3070 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/PKG-INFO
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      216 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/SOURCES.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        1 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/dependency_links.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       93 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/requires.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        6 2024-04-30 05:51:29.000000 aiotx-0.0.2/aiotx.egg-info/top_level.txt
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      419 2024-04-30 05:38:25.000000 aiotx-0.0.2/pyproject.toml
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      114 2024-04-30 05:51:29.778702 aiotx-0.0.2/setup.cfg
--rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     1769 2024-04-30 05:51:10.000000 aiotx-0.0.2/setup.py
+drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     3086 2024-04-30 06:07:18.000000 aiotx-0.0.3/.gitignore
+-rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)     3088 2024-04-30 06:12:55.671593 aiotx-0.0.3/PKG-INFO
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     1654 2024-04-30 06:05:14.000000 aiotx-0.0.3/README.md
+drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/aiotx/
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 05:57:05.000000 aiotx-0.0.3/aiotx/__init__.py
+drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/aiotx/clients/
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      291 2024-04-30 06:08:28.000000 aiotx-0.0.3/aiotx/clients/__init__.py
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      187 2024-04-30 06:08:35.000000 aiotx-0.0.3/aiotx/clients/_bitcoin_base_client.py
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      186 2024-04-30 06:08:46.000000 aiotx-0.0.3/aiotx/clients/_evm_base_client.py
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       86 2024-04-30 06:11:46.000000 aiotx-0.0.3/aiotx/exceptions.py
+drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/aiotx/types/
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       59 2024-04-30 06:06:35.000000 aiotx-0.0.3/aiotx/types/__init__.py
+drwxrwxr-x   0 oleksandr  (1000) oleksandr  (1000)        0 2024-04-30 06:12:55.671593 aiotx-0.0.3/aiotx.egg-info/
+-rw-r--r--   0 oleksandr  (1000) oleksandr  (1000)     3088 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/PKG-INFO
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      358 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        1 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)       93 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/requires.txt
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)        6 2024-04-30 06:12:55.000000 aiotx-0.0.3/aiotx.egg-info/top_level.txt
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      419 2024-04-30 05:38:25.000000 aiotx-0.0.3/pyproject.toml
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)      114 2024-04-30 06:12:55.675593 aiotx-0.0.3/setup.cfg
+-rw-rw-r--   0 oleksandr  (1000) oleksandr  (1000)     1769 2024-04-30 06:12:20.000000 aiotx-0.0.3/setup.py
```

### Comparing `aiotx-0.0.2/.gitignore` & `aiotx-0.0.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+.vscode/
```

### Comparing `aiotx-0.0.2/PKG-INFO` & `aiotx-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.0.2
+Version: 0.0.3
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -49,25 +49,25 @@
 pip install aiotx
 ```
 
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
-from aiotx import AioTxClient
+from aiotx import AioTxBSCClient
 
 async def main():
-    client = AioTxClient(node_url="https://example.com")
+    bsc_client = AioTxBSCClient(node_url="https://example.com")
     
     # Create a new wallet
-    wallet = await client.create_wallet()
+    wallet = await bsc_client.create_wallet()
     print(f"Wallet address: {wallet.address}")
     
     # Retrieve the wallet balance
-    balance = await client.get_balance(wallet.address)
+    balance = await bsc_client.get_balance(wallet.address)
     print(f"Wallet balance: {balance}")
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
```

### Comparing `aiotx-0.0.2/README.md` & `aiotx-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 pip install aiotx
 ```
 
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
-from aiotx import AioTxClient
+from aiotx import AioTxBSCClient
 
 async def main():
-    client = AioTxClient(node_url="https://example.com")
+    bsc_client = AioTxBSCClient(node_url="https://example.com")
     
     # Create a new wallet
-    wallet = await client.create_wallet()
+    wallet = await bsc_client.create_wallet()
     print(f"Wallet address: {wallet.address}")
     
     # Retrieve the wallet balance
-    balance = await client.get_balance(wallet.address)
+    balance = await bsc_client.get_balance(wallet.address)
     print(f"Wallet balance: {balance}")
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
```

### Comparing `aiotx-0.0.2/aiotx.egg-info/PKG-INFO` & `aiotx-0.0.3/aiotx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.0.2
+Version: 0.0.3
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -49,25 +49,25 @@
 pip install aiotx
 ```
 
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
-from aiotx import AioTxClient
+from aiotx import AioTxBSCClient
 
 async def main():
-    client = AioTxClient(node_url="https://example.com")
+    bsc_client = AioTxBSCClient(node_url="https://example.com")
     
     # Create a new wallet
-    wallet = await client.create_wallet()
+    wallet = await bsc_client.create_wallet()
     print(f"Wallet address: {wallet.address}")
     
     # Retrieve the wallet balance
-    balance = await client.get_balance(wallet.address)
+    balance = await bsc_client.get_balance(wallet.address)
     print(f"Wallet balance: {balance}")
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
```

### Comparing `aiotx-0.0.2/setup.py` & `aiotx-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "wallet",
         "transaction",
     ],
     use_scm_version=True,
     description="An asynchronous library for interacting with various cryptocurrencies and blockchains",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(exclude=("tests", "scripts")),
     package_data={
         "aiotx": ["py.typed"],
     },
     setup_requires=[
         "setuptools_scm",
     ],
```

