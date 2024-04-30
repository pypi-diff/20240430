# Comparing `tmp/azurefunctions-extensions-bindings-blob-1.0.0a1.tar.gz` & `tmp/azurefunctions_extensions_bindings_blob-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurefunctions-extensions-bindings-blob-1.0.0a1.tar", last modified: Thu Apr 11 00:15:19 2024, max compression
+gzip compressed data, was "azurefunctions_extensions_bindings_blob-1.0.0b1.tar", last modified: Tue Apr 30 20:13:59 2024, max compression
```

## Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1.tar` & `azurefunctions_extensions_bindings_blob-1.0.0b1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:19.045160 azurefunctions-extensions-bindings-blob-1.0.0a1/
--rw-rw-rw-   0        0        0     1093 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/LICENSE
--rw-rw-rw-   0        0        0       91 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     7556 2024-04-11 00:15:19.043160 azurefunctions-extensions-bindings-blob-1.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     6334 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:18.943004 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:18.943004 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:18.944007 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:18.981846 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/
--rw-rw-rw-   0        0        0      446 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/__init__.py
--rw-rw-rw-   0        0        0     1367 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/blobClient.py
--rw-rw-rw-   0        0        0     1539 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/blobClientConverter.py
--rw-rw-rw-   0        0        0     1319 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/containerClient.py
--rw-rw-rw-   0        0        0     1547 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/storageStreamDownloader.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:19.041154 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions_extensions_bindings_blob.egg-info/
--rw-rw-rw-   0        0        0     7556 2024-04-11 00:15:18.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions_extensions_bindings_blob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      906 2024-04-11 00:15:18.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions_extensions_bindings_blob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 00:15:18.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions_extensions_bindings_blob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2024-04-11 00:15:18.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions_extensions_bindings_blob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-11 00:15:18.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions_extensions_bindings_blob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1507 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:18.947006 azurefunctions-extensions-bindings-blob-1.0.0a1/samples/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:19.026188 azurefunctions-extensions-bindings-blob-1.0.0a1/samples/blob_samples_blobclient/
--rw-rw-rw-   0        0        0     1734 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/samples/blob_samples_blobclient/function_app.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:19.027760 azurefunctions-extensions-bindings-blob-1.0.0a1/samples/blob_samples_containerclient/
--rw-rw-rw-   0        0        0     1617 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/samples/blob_samples_containerclient/function_app.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:19.028762 azurefunctions-extensions-bindings-blob-1.0.0a1/samples/blob_samples_storagestreamdownloader/
--rw-rw-rw-   0        0        0     1736 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/samples/blob_samples_storagestreamdownloader/function_app.py
--rw-rw-rw-   0        0        0       42 2024-04-11 00:15:19.045160 azurefunctions-extensions-bindings-blob-1.0.0a1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 00:15:19.037156 azurefunctions-extensions-bindings-blob-1.0.0a1/tests/
--rw-rw-rw-   0        0        0      519 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/tests/__init__.py
--rw-rw-rw-   0        0        0     6580 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/tests/test_blobclient.py
--rw-rw-rw-   0        0        0     6708 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/tests/test_containerclient.py
--rw-rw-rw-   0        0        0     6786 2024-04-11 00:14:42.000000 azurefunctions-extensions-bindings-blob-1.0.0a1/tests/test_ssd.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.973619 azurefunctions_extensions_bindings_blob-1.0.0b1/
+-rw-rw-rw-   0        0        0     1093 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7650 2024-04-30 20:13:59.972625 azurefunctions_extensions_bindings_blob-1.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     6428 2024-04-30 18:50:12.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.900874 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.901873 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.901873 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.927165 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/
+-rw-rw-rw-   0        0        0      446 2024-04-30 18:50:12.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/__init__.py
+-rw-rw-rw-   0        0        0     1367 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/blobClient.py
+-rw-rw-rw-   0        0        0     1539 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/blobClientConverter.py
+-rw-rw-rw-   0        0        0     1319 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/containerClient.py
+-rw-rw-rw-   0        0        0     1547 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/storageStreamDownloader.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.969614 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions_extensions_bindings_blob.egg-info/
+-rw-rw-rw-   0        0        0     7650 2024-04-30 20:13:59.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions_extensions_bindings_blob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2024-04-30 20:13:59.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions_extensions_bindings_blob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 20:13:59.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions_extensions_bindings_blob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2024-04-30 20:13:59.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions_extensions_bindings_blob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-30 20:13:59.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions_extensions_bindings_blob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1507 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.907408 azurefunctions_extensions_bindings_blob-1.0.0b1/samples/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.961315 azurefunctions_extensions_bindings_blob-1.0.0b1/samples/blob_samples_blobclient/
+-rw-rw-rw-   0        0        0     1748 2024-04-30 18:50:12.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/samples/blob_samples_blobclient/function_app.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.962315 azurefunctions_extensions_bindings_blob-1.0.0b1/samples/blob_samples_containerclient/
+-rw-rw-rw-   0        0        0     1615 2024-04-30 18:50:12.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/samples/blob_samples_containerclient/function_app.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.963316 azurefunctions_extensions_bindings_blob-1.0.0b1/samples/blob_samples_storagestreamdownloader/
+-rw-rw-rw-   0        0        0     1734 2024-04-30 18:50:12.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/samples/blob_samples_storagestreamdownloader/function_app.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 20:13:59.973619 azurefunctions_extensions_bindings_blob-1.0.0b1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 20:13:59.967615 azurefunctions_extensions_bindings_blob-1.0.0b1/tests/
+-rw-rw-rw-   0        0        0      519 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/tests/__init__.py
+-rw-rw-rw-   0        0        0     6580 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/tests/test_blobclient.py
+-rw-rw-rw-   0        0        0     6708 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/tests/test_containerclient.py
+-rw-rw-rw-   0        0        0     6786 2024-04-23 20:16:13.000000 azurefunctions_extensions_bindings_blob-1.0.0b1/tests/test_ssd.py
```

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/LICENSE` & `azurefunctions_extensions_bindings_blob-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/PKG-INFO` & `azurefunctions_extensions_bindings_blob-1.0.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurefunctions-extensions-bindings-blob
-Version: 1.0.0a1
+Version: 1.0.0b1
 Summary: Blob Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,49 +15,48 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: azurefunctions-extensions-base
-Requires-Dist: azure-storage-blob==12.19.0
+Requires-Dist: azure-storage-blob==12.19.1
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-instafail; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
-# Azure Functions Extension Blob library for Python
+# Azure Functions Extensions Bindings Blob library for Python
 This library allows Blob Trigger and Blob Input bindings in Python Function Apps to recognize and bind to client types from the
 Azure Storage Blob sdk.
 
 Blob client types can be generated from:
 
 * Blob Triggers
 * Blob Input
 
 [Source code](https://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-bindings-blob)
-| Package (PyPi)
-| Package (Conda)
+[Package (PyPi)](https://pypi.org/project/azurefunctions-extensions-bindings-blob/)
 | API reference documentation
 | Product documentation
 | [Samples](hhttps://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-bindings-blob/samples)
 
 
 ## Getting started
 
 ### Prerequisites
 * Python 3.9 or later is required to use this package. For more details, please read our page on [Python Functions version support policy](https://learn.microsoft.com/en-us/azure/azure-functions/functions-versions?tabs=isolated-process%2Cv4&pivots=programming-language-python#languages).
 
 * You must have an [Azure subscription](https://azure.microsoft.com/free/) and an
 [Azure storage account](https://docs.microsoft.com/azure/storage/common/storage-account-overview) to use this package.
 
 ### Install the package
-Install the Azure Functions Extension Blob library for Python with pip:
+Install the Azure Functions Extensions Bindings Blob library for Python with pip:
 
 ```bash
 pip install azurefunctions-extensions-bindings-blob
 ```
 
 ### Create a storage account
 If you wish to create a new storage account, you can use the
@@ -71,15 +70,15 @@
 az group create --name my-resource-group --location westus2
 
 # Create the storage account
 az storage account create -n my-storage-account-name -g my-resource-group
 ```
 
 ### Bind to the SDK-type
-The Azure Functions Extension Blob library for Python allows you to create a function app with a Blob Trigger or
+The Azure Functions Extensions Bindings Blob library for Python allows you to create a function app with a Blob Trigger or
 Blob Input and define the type as a BlobClient, ContainerClient, or StorageStreamDownloader. Instead of receiving
 an InputStream, when the function is executed, the type returned will be the defined SDK-type and have all of the
 properties and methods available as seen in the Azure Storage Blob library for Python.
 
 
 ```python
 import logging
@@ -88,25 +87,25 @@
 
 @app.blob_trigger(arg_name="client",
                   path="PATH/TO/BLOB",
                   connection="AzureWebJobsStorage")
 def blob_trigger(client: blob.BlobClient):
     logging.info(f"Python blob trigger function processed blob \n"
                  f"Properties: {client.get_blob_properties()}\n"
-                 f"Blob content: {client.download_blob(encoding="utf-8").readall()}")
+                 f"Blob content head: {client.download_blob(encoding="utf-8").read(size=1)}")
 
 
 @app.route(route="file")
 @app.blob_input(arg_name="client",
                 path="PATH/TO/BLOB",
                 connection="AzureWebJobsStorage")
 def blob_input(req: func.HttpRequest, client: blob.BlobClient):
     logging.info(f"Python blob input function processed blob \n"
                  f"Properties: {client.get_blob_properties()}\n"
-                 f"Blob content: {client.download_blob(encoding="utf-8").readall()}")
+                 f"Blob content head: {client.download_blob(encoding="utf-8").read(size=1)}")
 ```
 
 ## Troubleshooting
 ### General
 The SDK-types raise exceptions defined in [Azure Core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md).
 
 This list can be used for reference to catch thrown exceptions. To get the specific error code of the exception, use the `error_code` attribute, i.e, `exception.error_code`.
```

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/README.md` & `azurefunctions_extensions_bindings_blob-1.0.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# Azure Functions Extension Blob library for Python
+# Azure Functions Extensions Bindings Blob library for Python
 This library allows Blob Trigger and Blob Input bindings in Python Function Apps to recognize and bind to client types from the
 Azure Storage Blob sdk.
 
 Blob client types can be generated from:
 
 * Blob Triggers
 * Blob Input
 
 [Source code](https://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-bindings-blob)
-| Package (PyPi)
-| Package (Conda)
+[Package (PyPi)](https://pypi.org/project/azurefunctions-extensions-bindings-blob/)
 | API reference documentation
 | Product documentation
 | [Samples](hhttps://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-bindings-blob/samples)
 
 
 ## Getting started
 
 ### Prerequisites
 * Python 3.9 or later is required to use this package. For more details, please read our page on [Python Functions version support policy](https://learn.microsoft.com/en-us/azure/azure-functions/functions-versions?tabs=isolated-process%2Cv4&pivots=programming-language-python#languages).
 
 * You must have an [Azure subscription](https://azure.microsoft.com/free/) and an
 [Azure storage account](https://docs.microsoft.com/azure/storage/common/storage-account-overview) to use this package.
 
 ### Install the package
-Install the Azure Functions Extension Blob library for Python with pip:
+Install the Azure Functions Extensions Bindings Blob library for Python with pip:
 
 ```bash
 pip install azurefunctions-extensions-bindings-blob
 ```
 
 ### Create a storage account
 If you wish to create a new storage account, you can use the
@@ -42,15 +41,15 @@
 az group create --name my-resource-group --location westus2
 
 # Create the storage account
 az storage account create -n my-storage-account-name -g my-resource-group
 ```
 
 ### Bind to the SDK-type
-The Azure Functions Extension Blob library for Python allows you to create a function app with a Blob Trigger or
+The Azure Functions Extensions Bindings Blob library for Python allows you to create a function app with a Blob Trigger or
 Blob Input and define the type as a BlobClient, ContainerClient, or StorageStreamDownloader. Instead of receiving
 an InputStream, when the function is executed, the type returned will be the defined SDK-type and have all of the
 properties and methods available as seen in the Azure Storage Blob library for Python.
 
 
 ```python
 import logging
@@ -59,25 +58,25 @@
 
 @app.blob_trigger(arg_name="client",
                   path="PATH/TO/BLOB",
                   connection="AzureWebJobsStorage")
 def blob_trigger(client: blob.BlobClient):
     logging.info(f"Python blob trigger function processed blob \n"
                  f"Properties: {client.get_blob_properties()}\n"
-                 f"Blob content: {client.download_blob(encoding="utf-8").readall()}")
+                 f"Blob content head: {client.download_blob(encoding="utf-8").read(size=1)}")
 
 
 @app.route(route="file")
 @app.blob_input(arg_name="client",
                 path="PATH/TO/BLOB",
                 connection="AzureWebJobsStorage")
 def blob_input(req: func.HttpRequest, client: blob.BlobClient):
     logging.info(f"Python blob input function processed blob \n"
                  f"Properties: {client.get_blob_properties()}\n"
-                 f"Blob content: {client.download_blob(encoding="utf-8").readall()}")
+                 f"Blob content head: {client.download_blob(encoding="utf-8").read(size=1)}")
 ```
 
 ## Troubleshooting
 ### General
 The SDK-types raise exceptions defined in [Azure Core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md).
 
 This list can be used for reference to catch thrown exceptions. To get the specific error code of the exception, use the `error_code` attribute, i.e, `exception.error_code`.
```

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/blobClient.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/blobClient.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/blobClientConverter.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/blobClientConverter.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/containerClient.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/containerClient.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions/extensions/bindings/blob/storageStreamDownloader.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions/extensions/bindings/blob/storageStreamDownloader.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions_extensions_bindings_blob.egg-info/PKG-INFO` & `azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions_extensions_bindings_blob.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurefunctions-extensions-bindings-blob
-Version: 1.0.0a1
+Version: 1.0.0b1
 Summary: Blob Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,49 +15,48 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: azurefunctions-extensions-base
-Requires-Dist: azure-storage-blob==12.19.0
+Requires-Dist: azure-storage-blob==12.19.1
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-instafail; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
-# Azure Functions Extension Blob library for Python
+# Azure Functions Extensions Bindings Blob library for Python
 This library allows Blob Trigger and Blob Input bindings in Python Function Apps to recognize and bind to client types from the
 Azure Storage Blob sdk.
 
 Blob client types can be generated from:
 
 * Blob Triggers
 * Blob Input
 
 [Source code](https://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-bindings-blob)
-| Package (PyPi)
-| Package (Conda)
+[Package (PyPi)](https://pypi.org/project/azurefunctions-extensions-bindings-blob/)
 | API reference documentation
 | Product documentation
 | [Samples](hhttps://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-bindings-blob/samples)
 
 
 ## Getting started
 
 ### Prerequisites
 * Python 3.9 or later is required to use this package. For more details, please read our page on [Python Functions version support policy](https://learn.microsoft.com/en-us/azure/azure-functions/functions-versions?tabs=isolated-process%2Cv4&pivots=programming-language-python#languages).
 
 * You must have an [Azure subscription](https://azure.microsoft.com/free/) and an
 [Azure storage account](https://docs.microsoft.com/azure/storage/common/storage-account-overview) to use this package.
 
 ### Install the package
-Install the Azure Functions Extension Blob library for Python with pip:
+Install the Azure Functions Extensions Bindings Blob library for Python with pip:
 
 ```bash
 pip install azurefunctions-extensions-bindings-blob
 ```
 
 ### Create a storage account
 If you wish to create a new storage account, you can use the
@@ -71,15 +70,15 @@
 az group create --name my-resource-group --location westus2
 
 # Create the storage account
 az storage account create -n my-storage-account-name -g my-resource-group
 ```
 
 ### Bind to the SDK-type
-The Azure Functions Extension Blob library for Python allows you to create a function app with a Blob Trigger or
+The Azure Functions Extensions Bindings Blob library for Python allows you to create a function app with a Blob Trigger or
 Blob Input and define the type as a BlobClient, ContainerClient, or StorageStreamDownloader. Instead of receiving
 an InputStream, when the function is executed, the type returned will be the defined SDK-type and have all of the
 properties and methods available as seen in the Azure Storage Blob library for Python.
 
 
 ```python
 import logging
@@ -88,25 +87,25 @@
 
 @app.blob_trigger(arg_name="client",
                   path="PATH/TO/BLOB",
                   connection="AzureWebJobsStorage")
 def blob_trigger(client: blob.BlobClient):
     logging.info(f"Python blob trigger function processed blob \n"
                  f"Properties: {client.get_blob_properties()}\n"
-                 f"Blob content: {client.download_blob(encoding="utf-8").readall()}")
+                 f"Blob content head: {client.download_blob(encoding="utf-8").read(size=1)}")
 
 
 @app.route(route="file")
 @app.blob_input(arg_name="client",
                 path="PATH/TO/BLOB",
                 connection="AzureWebJobsStorage")
 def blob_input(req: func.HttpRequest, client: blob.BlobClient):
     logging.info(f"Python blob input function processed blob \n"
                  f"Properties: {client.get_blob_properties()}\n"
-                 f"Blob content: {client.download_blob(encoding="utf-8").readall()}")
+                 f"Blob content head: {client.download_blob(encoding="utf-8").read(size=1)}")
 ```
 
 ## Troubleshooting
 ### General
 The SDK-types raise exceptions defined in [Azure Core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md).
 
 This list can be used for reference to catch thrown exceptions. To get the specific error code of the exception, use the `error_code` attribute, i.e, `exception.error_code`.
```

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/azurefunctions_extensions_bindings_blob.egg-info/SOURCES.txt` & `azurefunctions_extensions_bindings_blob-1.0.0b1/azurefunctions_extensions_bindings_blob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/pyproject.toml` & `azurefunctions_extensions_bindings_blob-1.0.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 000003c0: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
 000003d0: 626c 6527 2c0d 0a20 2020 205d 0d0a 6465  ble',..    ]..de
 000003e0: 7065 6e64 656e 6369 6573 203d 205b 0d0a  pendencies = [..
 000003f0: 2020 2020 2761 7a75 7265 6675 6e63 7469      'azurefuncti
 00000400: 6f6e 732d 6578 7465 6e73 696f 6e73 2d62  ons-extensions-b
 00000410: 6173 6527 2c0d 0a20 2020 2027 617a 7572  ase',..    'azur
 00000420: 652d 7374 6f72 6167 652d 626c 6f62 3d3d  e-storage-blob==
-00000430: 3132 2e31 392e 3027 0d0a 2020 2020 5d0d  12.19.0'..    ].
+00000430: 3132 2e31 392e 3127 0d0a 2020 2020 5d0d  12.19.1'..    ].
 00000440: 0a0d 0a5b 7072 6f6a 6563 742e 6f70 7469  ...[project.opti
 00000450: 6f6e 616c 2d64 6570 656e 6465 6e63 6965  onal-dependencie
 00000460: 735d 0d0a 6465 7620 3d20 5b0d 0a20 2020  s]..dev = [..   
 00000470: 2027 7079 7465 7374 272c 0d0a 2020 2020   'pytest',..    
 00000480: 2770 7974 6573 742d 636f 7627 2c0d 0a20  'pytest-cov',.. 
 00000490: 2020 2027 636f 7665 7261 6765 272c 0d0a     'coverage',..
 000004a0: 2020 2020 2770 7974 6573 742d 696e 7374      'pytest-inst
```

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/samples/blob_samples_blobclient/function_app.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/samples/blob_samples_containerclient/function_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,43 +10,37 @@
 
 import azure.functions as func
 import azurefunctions.extensions.bindings.blob as blob
 
 app = func.FunctionApp(http_auth_level=func.AuthLevel.ANONYMOUS)
 
 """
-FOLDER: blob_samples_blobclient
+FOLDER: blob_samples_containerclient
 DESCRIPTION:
-    These samples demonstrate how to obtain a BlobClient from a Blob Trigger
+    These samples demonstrate how to obtain a ContainerClient from a Blob Trigger
     or Blob Input function app binding.
 USAGE:
     Set the environment variables with your own values before running the
     sample:
     1) AzureWebJobsStorage - the connection string to your storage account
 
-    Set PATH/TO/BLOB to the path to the blob you want to trigger or serve as
+    Set CONTAINER to the path to the container you want to trigger or serve as
     input to the function.
 """
 
 
-@app.blob_trigger(
-    arg_name="client", path="PATH/TO/BLOB", connection="AzureWebJobsStorage"
-)
-def blob_trigger(client: blob.BlobClient):
+@app.blob_trigger(arg_name="client", path="CONTAINER", connection="AzureWebJobsStorage")
+def blob_trigger(client: blob.ContainerClient):
     logging.info(
         f"Python blob trigger function processed blob \n"
-        f"Properties: {client.get_blob_properties()}\n"
-        f"Blob content: {client.download_blob().readall()}"
+        f"Properties: {client.get_container_properties()}\n"
     )
 
 
 @app.route(route="file")
-@app.blob_input(
-    arg_name="client", path="PATH/TO/BLOB", connection="AzureWebJobsStorage"
-)
+@app.blob_input(arg_name="client", path="CONTAINER", connection="AzureWebJobsStorage")
 def blob_input(req: func.HttpRequest, client: blob.BlobClient):
     logging.info(
-        f"Python blob trigger function processed blob \n"
-        f"Properties: {client.get_blob_properties()}\n"
-        f"Blob content: {client.download_blob().readall()}"
+        f"Python blob input function processed blob \n"
+        f"Properties: {client.get_container_properties()}\n"
     )
     return "ok"
```

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/samples/blob_samples_storagestreamdownloader/function_app.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/samples/blob_samples_storagestreamdownloader/function_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,11 +42,11 @@
 @app.route(route="file")
 @app.blob_input(
     arg_name="stream", path="PATH/TO/BLOB", connection="AzureWebJobsStorage"
 )
 def blob_input(req: func.HttpRequest, stream: blob.StorageStreamDownloader):
     for chunk in stream.chunks():
         logging.info(
-            f"Python blob trigger function processed blob chunk \n"
+            f"Python blob input function processed blob chunk \n"
             f"Chunk: {chunk.decode()}"
         )
     return "ok"
```

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/tests/__init__.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/tests/test_blobclient.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/tests/test_blobclient.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/tests/test_containerclient.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/tests/test_containerclient.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-bindings-blob-1.0.0a1/tests/test_ssd.py` & `azurefunctions_extensions_bindings_blob-1.0.0b1/tests/test_ssd.py`

 * *Files identical despite different names*

