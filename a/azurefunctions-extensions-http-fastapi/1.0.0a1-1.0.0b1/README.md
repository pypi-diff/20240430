# Comparing `tmp/azurefunctions-extensions-http-fastapi-1.0.0a1.tar.gz` & `tmp/azurefunctions_extensions_http_fastapi-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurefunctions-extensions-http-fastapi-1.0.0a1.tar", last modified: Thu Apr 11 00:09:34 2024, max compression
+gzip compressed data, was "azurefunctions_extensions_http_fastapi-1.0.0b1.tar", last modified: Tue Apr 30 20:18:54 2024, max compression
```

## Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1.tar` & `azurefunctions_extensions_http_fastapi-1.0.0b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.783025 azurefunctions-extensions-http-fastapi-1.0.0a1/
--rw-rw-rw-   0        0        0     1093 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/LICENSE
--rw-rw-rw-   0        0        0       91 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     6430 2024-04-11 00:09:34.782025 azurefunctions-extensions-http-fastapi-1.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     5104 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.637048 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.638048 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions/extensions/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.638048 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions/extensions/http/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.673047 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions/extensions/http/fastapi/
--rw-rw-rw-   0        0        0      627 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions/extensions/http/fastapi/__init__.py
--rw-rw-rw-   0        0        0     4505 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions/extensions/http/fastapi/web.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.779027 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions_extensions_http_fastapi.egg-info/
--rw-rw-rw-   0        0        0     6430 2024-04-11 00:09:34.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions_extensions_http_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2024-04-11 00:09:34.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions_extensions_http_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 00:09:34.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions_extensions_http_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2024-04-11 00:09:34.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions_extensions_http_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-11 00:09:34.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions_extensions_http_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1608 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.641047 azurefunctions-extensions-http-fastapi-1.0.0a1/samples/
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.732248 azurefunctions-extensions-http-fastapi-1.0.0a1/samples/fastapi_samples_streaming_download/
--rw-rw-rw-   0        0        0     1017 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/samples/fastapi_samples_streaming_download/function_app.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.744247 azurefunctions-extensions-http-fastapi-1.0.0a1/samples/fastapi_samples_streaming_upload/
--rw-rw-rw-   0        0        0     1031 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/samples/fastapi_samples_streaming_upload/function_app.py
--rw-rw-rw-   0        0        0       42 2024-04-11 00:09:34.784027 azurefunctions-extensions-http-fastapi-1.0.0a1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 00:09:34.775024 azurefunctions-extensions-http-fastapi-1.0.0a1/tests/
--rw-rw-rw-   0        0        0      519 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/tests/__init__.py
--rw-rw-rw-   0        0        0     8678 2024-04-11 00:08:04.000000 azurefunctions-extensions-http-fastapi-1.0.0a1/tests/test_web.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.665885 azurefunctions_extensions_http_fastapi-1.0.0b1/
+-rw-rw-rw-   0        0        0     1093 2024-04-11 14:42:57.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-04-11 14:42:57.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6519 2024-04-30 20:18:54.664373 azurefunctions_extensions_http_fastapi-1.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     5193 2024-04-30 20:18:12.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.540641 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.540641 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions/extensions/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.540641 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions/extensions/http/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.571201 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions/extensions/http/fastapi/
+-rw-rw-rw-   0        0        0      627 2024-04-30 20:18:12.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions/extensions/http/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     4505 2024-04-11 14:42:57.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions/extensions/http/fastapi/web.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.661373 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions_extensions_http_fastapi.egg-info/
+-rw-rw-rw-   0        0        0     6519 2024-04-30 20:18:54.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions_extensions_http_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2024-04-30 20:18:54.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions_extensions_http_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 20:18:54.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions_extensions_http_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2024-04-30 20:18:54.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions_extensions_http_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-30 20:18:54.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions_extensions_http_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1608 2024-04-23 22:06:27.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.542636 azurefunctions_extensions_http_fastapi-1.0.0b1/samples/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.623782 azurefunctions_extensions_http_fastapi-1.0.0b1/samples/fastapi_samples_streaming_download/
+-rw-rw-rw-   0        0        0     1017 2024-04-11 14:42:57.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/samples/fastapi_samples_streaming_download/function_app.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.635323 azurefunctions_extensions_http_fastapi-1.0.0b1/samples/fastapi_samples_streaming_upload/
+-rw-rw-rw-   0        0        0     1031 2024-04-11 14:42:57.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/samples/fastapi_samples_streaming_upload/function_app.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 20:18:54.666890 azurefunctions_extensions_http_fastapi-1.0.0b1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 20:18:54.657374 azurefunctions_extensions_http_fastapi-1.0.0b1/tests/
+-rw-rw-rw-   0        0        0      519 2024-04-11 14:42:57.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/tests/__init__.py
+-rw-rw-rw-   0        0        0     8678 2024-04-11 14:42:57.000000 azurefunctions_extensions_http_fastapi-1.0.0b1/tests/test_web.py
```

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/LICENSE` & `azurefunctions_extensions_http_fastapi-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/PKG-INFO` & `azurefunctions_extensions_http_fastapi-1.0.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurefunctions-extensions-http-fastapi
-Version: 1.0.0a1
+Version: 1.0.0b1
 Summary: FastApi Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,52 +15,51 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azurefunctions.extensions.base
-Requires-Dist: fastapi==0.110.0
-Requires-Dist: uvicorn==0.28.0
-Requires-Dist: pydantic==2.6.4
+Requires-Dist: azurefunctions-extensions-base
+Requires-Dist: fastapi==0.110.1
+Requires-Dist: uvicorn==0.29.0
+Requires-Dist: pydantic==2.7.1
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-instafail; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
-# Azure Functions Extension FastApi library for Python
+# Azure Functions Extensions Http FastApi library for Python
 This library contains HttpV2 extensions for FastApi Request/Response types to use in your function app code. 
 
 [Source code](https://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-http-fastapi)
-| Package (PyPi)
-| Package (Conda)
+| [Package (PyPi)](https://pypi.org/project/azurefunctions-extensions-http-fastapi/)
 | API reference documentation
 | Product documentation
 | [Samples](hhttps://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-http-fastapi/samples)
 
 
 ## Getting started
 
 ### Prerequisites
 * Python 3.8 or later is required to use this package. For more details, please read our page on [Python Functions version support policy](https://learn.microsoft.com/en-us/azure/azure-functions/functions-versions?tabs=isolated-process%2Cv4&pivots=programming-language-python#languages).
 
 
 ### Instructions
 1. Follow the guide to [create an app](https://learn.microsoft.com/en-us/azure/azure-functions/create-first-function-cli-python?tabs=windows%2Cbash%2Cazure-cli%2Cbrowser).
 2. Ensure your app is using programming model v2 and contains a http trigger function.
-3. Add azurefunctions-extensions-http-fastapi to your requirement.txt
-4. Import Request and different types of responses from azure.functions.extensions.fastapi in your httptrigger functions.
-5. Change the request and response types to ones imported from azure.functions.extensions.fastapi.
+3. Add ```azurefunctions-extensions-http-fastapi``` to your requirements.txt
+4. Import Request and different types of responses from ```azurefunctions.extensions.http.fastapi``` in your HttpTrigger functions.
+5. Change the request and response types to ones imported from ```azurefunctions.extensions.http.fastapi```.
 6. Run your function app and try it out!
 
 ### Bind to the FastApi-type
-The Azure Functions Extension FastApi library for Python allows you to create a function app with FastApi Request or Response types. When your function runs, you will receive the request of FastApi Request type and you can return a FastApi response type instance. FastApi is one of top popular python web framework which provides elegant and powerful request/response types and functionalities to users. With this integration, you are empowered to use request/response the same way as using them in native FastApi. A good example is you can do http streaming upload and streaming download now! Feel free to check out [Fastapi doc] for further reference (https://fastapi.tiangolo.com/reference/responses/?h=custom)
+The Azure Functions Extensions Http FastApi library for Python allows you to create a function app with FastApi Request or Response types. When your function runs, you will receive the request of FastApi Request type and you can return a FastApi response type instance. FastApi is one of top popular python web framework which provides elegant and powerful request/response types and functionalities to users. With this integration, you are empowered to use request/response the same way as using them in native FastApi. A good example is you can do http streaming upload and streaming download now! Feel free to check out [Fastapi doc](https://fastapi.tiangolo.com/reference/responses/?h=custom) for further reference. 
 
 
 ```python
 # This Azure Function receives streaming data from a client and processes it in real-time.
 # It demonstrates streaming upload capabilities for scenarios such as uploading large files,
 # processing continuous data streams, or handling IoT device data.
```

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/README.md` & `azurefunctions_extensions_http_fastapi-1.0.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# Azure Functions Extension FastApi library for Python
+# Azure Functions Extensions Http FastApi library for Python
 This library contains HttpV2 extensions for FastApi Request/Response types to use in your function app code. 
 
 [Source code](https://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-http-fastapi)
-| Package (PyPi)
-| Package (Conda)
+| [Package (PyPi)](https://pypi.org/project/azurefunctions-extensions-http-fastapi/)
 | API reference documentation
 | Product documentation
 | [Samples](hhttps://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-http-fastapi/samples)
 
 
 ## Getting started
 
 ### Prerequisites
 * Python 3.8 or later is required to use this package. For more details, please read our page on [Python Functions version support policy](https://learn.microsoft.com/en-us/azure/azure-functions/functions-versions?tabs=isolated-process%2Cv4&pivots=programming-language-python#languages).
 
 
 ### Instructions
 1. Follow the guide to [create an app](https://learn.microsoft.com/en-us/azure/azure-functions/create-first-function-cli-python?tabs=windows%2Cbash%2Cazure-cli%2Cbrowser).
 2. Ensure your app is using programming model v2 and contains a http trigger function.
-3. Add azurefunctions-extensions-http-fastapi to your requirement.txt
-4. Import Request and different types of responses from azure.functions.extensions.fastapi in your httptrigger functions.
-5. Change the request and response types to ones imported from azure.functions.extensions.fastapi.
+3. Add ```azurefunctions-extensions-http-fastapi``` to your requirements.txt
+4. Import Request and different types of responses from ```azurefunctions.extensions.http.fastapi``` in your HttpTrigger functions.
+5. Change the request and response types to ones imported from ```azurefunctions.extensions.http.fastapi```.
 6. Run your function app and try it out!
 
 ### Bind to the FastApi-type
-The Azure Functions Extension FastApi library for Python allows you to create a function app with FastApi Request or Response types. When your function runs, you will receive the request of FastApi Request type and you can return a FastApi response type instance. FastApi is one of top popular python web framework which provides elegant and powerful request/response types and functionalities to users. With this integration, you are empowered to use request/response the same way as using them in native FastApi. A good example is you can do http streaming upload and streaming download now! Feel free to check out [Fastapi doc] for further reference (https://fastapi.tiangolo.com/reference/responses/?h=custom)
+The Azure Functions Extensions Http FastApi library for Python allows you to create a function app with FastApi Request or Response types. When your function runs, you will receive the request of FastApi Request type and you can return a FastApi response type instance. FastApi is one of top popular python web framework which provides elegant and powerful request/response types and functionalities to users. With this integration, you are empowered to use request/response the same way as using them in native FastApi. A good example is you can do http streaming upload and streaming download now! Feel free to check out [Fastapi doc](https://fastapi.tiangolo.com/reference/responses/?h=custom) for further reference. 
 
 
 ```python
 # This Azure Function receives streaming data from a client and processes it in real-time.
 # It demonstrates streaming upload capabilities for scenarios such as uploading large files,
 # processing continuous data streams, or handling IoT device data.
```

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions/extensions/http/fastapi/__init__.py` & `azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions/extensions/http/fastapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
     "RedirectResponse",
     "JSONResponse",
     "UJSONResponse",
     "ORJSONResponse",
     "FileResponse",
 ]
 
-__version__ = "1.0.0a1"
+__version__ = "1.0.0b1"
```

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions/extensions/http/fastapi/web.py` & `azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions/extensions/http/fastapi/web.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions_extensions_http_fastapi.egg-info/PKG-INFO` & `azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions_extensions_http_fastapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurefunctions-extensions-http-fastapi
-Version: 1.0.0a1
+Version: 1.0.0b1
 Summary: FastApi Python worker extension for Azure Functions.
 Author-email: "Azure Functions team at Microsoft Corp." <azurefunctions@microsoft.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,52 +15,51 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azurefunctions.extensions.base
-Requires-Dist: fastapi==0.110.0
-Requires-Dist: uvicorn==0.28.0
-Requires-Dist: pydantic==2.6.4
+Requires-Dist: azurefunctions-extensions-base
+Requires-Dist: fastapi==0.110.1
+Requires-Dist: uvicorn==0.29.0
+Requires-Dist: pydantic==2.7.1
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-instafail; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
-# Azure Functions Extension FastApi library for Python
+# Azure Functions Extensions Http FastApi library for Python
 This library contains HttpV2 extensions for FastApi Request/Response types to use in your function app code. 
 
 [Source code](https://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-http-fastapi)
-| Package (PyPi)
-| Package (Conda)
+| [Package (PyPi)](https://pypi.org/project/azurefunctions-extensions-http-fastapi/)
 | API reference documentation
 | Product documentation
 | [Samples](hhttps://github.com/Azure/azure-functions-python-extensions/tree/main/azurefunctions-extensions-http-fastapi/samples)
 
 
 ## Getting started
 
 ### Prerequisites
 * Python 3.8 or later is required to use this package. For more details, please read our page on [Python Functions version support policy](https://learn.microsoft.com/en-us/azure/azure-functions/functions-versions?tabs=isolated-process%2Cv4&pivots=programming-language-python#languages).
 
 
 ### Instructions
 1. Follow the guide to [create an app](https://learn.microsoft.com/en-us/azure/azure-functions/create-first-function-cli-python?tabs=windows%2Cbash%2Cazure-cli%2Cbrowser).
 2. Ensure your app is using programming model v2 and contains a http trigger function.
-3. Add azurefunctions-extensions-http-fastapi to your requirement.txt
-4. Import Request and different types of responses from azure.functions.extensions.fastapi in your httptrigger functions.
-5. Change the request and response types to ones imported from azure.functions.extensions.fastapi.
+3. Add ```azurefunctions-extensions-http-fastapi``` to your requirements.txt
+4. Import Request and different types of responses from ```azurefunctions.extensions.http.fastapi``` in your HttpTrigger functions.
+5. Change the request and response types to ones imported from ```azurefunctions.extensions.http.fastapi```.
 6. Run your function app and try it out!
 
 ### Bind to the FastApi-type
-The Azure Functions Extension FastApi library for Python allows you to create a function app with FastApi Request or Response types. When your function runs, you will receive the request of FastApi Request type and you can return a FastApi response type instance. FastApi is one of top popular python web framework which provides elegant and powerful request/response types and functionalities to users. With this integration, you are empowered to use request/response the same way as using them in native FastApi. A good example is you can do http streaming upload and streaming download now! Feel free to check out [Fastapi doc] for further reference (https://fastapi.tiangolo.com/reference/responses/?h=custom)
+The Azure Functions Extensions Http FastApi library for Python allows you to create a function app with FastApi Request or Response types. When your function runs, you will receive the request of FastApi Request type and you can return a FastApi response type instance. FastApi is one of top popular python web framework which provides elegant and powerful request/response types and functionalities to users. With this integration, you are empowered to use request/response the same way as using them in native FastApi. A good example is you can do http streaming upload and streaming download now! Feel free to check out [Fastapi doc](https://fastapi.tiangolo.com/reference/responses/?h=custom) for further reference. 
 
 
 ```python
 # This Azure Function receives streaming data from a client and processes it in real-time.
 # It demonstrates streaming upload capabilities for scenarios such as uploading large files,
 # processing continuous data streams, or handling IoT device data.
```

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/azurefunctions_extensions_http_fastapi.egg-info/SOURCES.txt` & `azurefunctions_extensions_http_fastapi-1.0.0b1/azurefunctions_extensions_http_fastapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/pyproject.toml` & `azurefunctions_extensions_http_fastapi-1.0.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -61,21 +61,21 @@
 000003c0: 5765 6220 456e 7669 726f 6e6d 656e 7427  Web Environment'
 000003d0: 2c0d 0a20 2020 2020 2020 2027 4465 7665  ,..        'Deve
 000003e0: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
 000003f0: 3a20 3520 2d20 5072 6f64 7563 7469 6f6e  : 5 - Production
 00000400: 2f53 7461 626c 6527 2c0d 0a20 2020 205d  /Stable',..    ]
 00000410: 0d0a 6465 7065 6e64 656e 6369 6573 203d  ..dependencies =
 00000420: 205b 0d0a 2020 2020 2020 2020 2761 7a75   [..        'azu
-00000430: 7265 6675 6e63 7469 6f6e 732e 6578 7465  refunctions.exte
-00000440: 6e73 696f 6e73 2e62 6173 6527 2c0d 0a20  nsions.base',.. 
+00000430: 7265 6675 6e63 7469 6f6e 732d 6578 7465  refunctions-exte
+00000440: 6e73 696f 6e73 2d62 6173 6527 2c0d 0a20  nsions-base',.. 
 00000450: 2020 2020 2020 2027 6661 7374 6170 693d         'fastapi=
-00000460: 3d30 2e31 3130 2e30 272c 0d0a 2020 2020  =0.110.0',..    
+00000460: 3d30 2e31 3130 2e31 272c 0d0a 2020 2020  =0.110.1',..    
 00000470: 2020 2020 2775 7669 636f 726e 3d3d 302e      'uvicorn==0.
-00000480: 3238 2e30 272c 0d0a 2020 2020 2020 2020  28.0',..        
-00000490: 2770 7964 616e 7469 633d 3d32 2e36 2e34  'pydantic==2.6.4
+00000480: 3239 2e30 272c 0d0a 2020 2020 2020 2020  29.0',..        
+00000490: 2770 7964 616e 7469 633d 3d32 2e37 2e31  'pydantic==2.7.1
 000004a0: 272c 0d0a 2020 2020 5d0d 0a0d 0a5b 7072  ',..    ]....[pr
 000004b0: 6f6a 6563 742e 6f70 7469 6f6e 616c 2d64  oject.optional-d
 000004c0: 6570 656e 6465 6e63 6965 735d 0d0a 6465  ependencies]..de
 000004d0: 7620 3d20 5b0d 0a20 2020 2027 7079 7465  v = [..    'pyte
 000004e0: 7374 272c 0d0a 2020 2020 2770 7974 6573  st',..    'pytes
 000004f0: 742d 636f 7627 2c0d 0a20 2020 2027 636f  t-cov',..    'co
 00000500: 7665 7261 6765 272c 0d0a 2020 2020 2770  verage',..    'p
```

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/samples/fastapi_samples_streaming_download/function_app.py` & `azurefunctions_extensions_http_fastapi-1.0.0b1/samples/fastapi_samples_streaming_download/function_app.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/samples/fastapi_samples_streaming_upload/function_app.py` & `azurefunctions_extensions_http_fastapi-1.0.0b1/samples/fastapi_samples_streaming_upload/function_app.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/tests/__init__.py` & `azurefunctions_extensions_http_fastapi-1.0.0b1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `azurefunctions-extensions-http-fastapi-1.0.0a1/tests/test_web.py` & `azurefunctions_extensions_http_fastapi-1.0.0b1/tests/test_web.py`

 * *Files identical despite different names*

