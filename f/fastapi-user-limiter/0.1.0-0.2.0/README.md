# Comparing `tmp/fastapi_user_limiter-0.1.0.tar.gz` & `tmp/fastapi_user_limiter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_limiter-0.1.0.tar", last modified: Wed Apr 24 13:30:43 2024, max compression
+gzip compressed data, was "fastapi_user_limiter-0.2.0.tar", last modified: Tue Apr 30 13:04:11 2024, max compression
```

## Comparing `fastapi_user_limiter-0.1.0.tar` & `fastapi_user_limiter-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:30:43.843367 fastapi_user_limiter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 13:30:43.843367 fastapi_user_limiter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 13:30:26.000000 fastapi_user_limiter-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 13:30:26.000000 fastapi_user_limiter-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:30:43.843367 fastapi_user_limiter-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:30:43.843367 fastapi_user_limiter-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:30:43.843367 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:30:26.000000 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-24 13:30:26.000000 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:30:43.843367 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 13:30:43.000000 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-24 13:30:43.000000 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:30:43.000000 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 13:30:43.000000 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 13:30:43.000000 fastapi_user_limiter-0.1.0/src/fastapi_user_limiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 13:04:03.000000 fastapi_user_limiter-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 13:04:03.000000 fastapi_user_limiter-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:03.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-30 13:04:03.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/top_level.txt
```

### Comparing `fastapi_user_limiter-0.1.0/PKG-INFO` & `fastapi_user_limiter-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,59 @@
-Metadata-Version: 2.1
-Name: fastapi_user_limiter
-Version: 0.1.0
-Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
-Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
-Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
-Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Requires-Dist: fastapi[all]
-Requires-Dist: redis
-
 # FastAPI rate limiter
 
 This package adds a rate limiter to FastAPI using Redis.
 
 ## Installation
 
 First install Redis, then install the package using:
 ```
 pip install fastapi-user-limiter
 ```
 
 ## Usage
 
-An example of how to use the rate limiter can be found in `example.py`:
+You can use the `rate_limit` decorator to put a single rate limit on an endpoint:
 
-```
+```python
 from fastapi_user_limiter.limiter import RateLimiter, rate_limit
 from fastapi import FastAPI, Request
 
+app = FastAPI()
+rate_limiter = RateLimiter()
+
+# 2 requests max per 5 seconds
+@app.get("/single")
+@rate_limit(rate_limiter, 2, 5)
+async def read_single(request: Request):
+    return {"Hello": "World"}
+
+```
+
+To put multiple rate limits on the same endpoint (with different window size and maximum request counts), use the
+`multi_rate_limit` decorator. Each `multi_rate_limit` decorator on a particular endpoint requires an ID as its first arg.
+This ID must be unique among the `multi_rate_limit` decorators on that endpoint:
+
+```python
+from fastapi_user_limiter.limiter import RateLimiter, multi_rate_limit
+from fastapi import FastAPI, Request
 
 app = FastAPI()
 rate_limiter = RateLimiter()
 
 
-@app.get("/")
-@rate_limit(rate_limiter, 5, 60)
-async def read_root(request: Request):
-    return {"Hello": "World"}
+# 1 request max per second, 3 requests max per 10 seconds
+@app.get("/multi")
+@multi_rate_limit(1, rate_limiter, 1, 1)
+@multi_rate_limit(2, rate_limiter, 3, 10)
+async def read_multi(request: Request):
+    return {"Hello": "There"}
 ```
 
-Every endpoint handler with the rate limiter decorator needs to have `request` (of type `fastapi.Request`) as its first argument.
+The aforementioned examples can be found in `example.py` (use ` uvicorn example:app --reload` to run).
+
+
+**NOTE**: Every endpoint handler with the rate limiter decorator needs to have `request` (of type `fastapi.Request`)
+as its first argument.
 
 ## Future features
 
 The package will soon have the additional feature of allowing each user account to have a different rate limit for each endpoint.
```

### Comparing `fastapi_user_limiter-0.1.0/pyproject.toml` & `fastapi_user_limiter-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi_user_limiter"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Rate-limiter for FastAPI with the possibility of user-based rate limits"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_user_limiter-0.1.0/src/fastapi_user_limiter.egg-info/PKG-INFO` & `fastapi_user_limiter-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.1.0
+Version: 0.2.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,29 +22,53 @@
 First install Redis, then install the package using:
 ```
 pip install fastapi-user-limiter
 ```
 
 ## Usage
 
-An example of how to use the rate limiter can be found in `example.py`:
+You can use the `rate_limit` decorator to put a single rate limit on an endpoint:
 
-```
+```python
 from fastapi_user_limiter.limiter import RateLimiter, rate_limit
 from fastapi import FastAPI, Request
 
+app = FastAPI()
+rate_limiter = RateLimiter()
+
+# 2 requests max per 5 seconds
+@app.get("/single")
+@rate_limit(rate_limiter, 2, 5)
+async def read_single(request: Request):
+    return {"Hello": "World"}
+
+```
+
+To put multiple rate limits on the same endpoint (with different window size and maximum request counts), use the
+`multi_rate_limit` decorator. Each `multi_rate_limit` decorator on a particular endpoint requires an ID as its first arg.
+This ID must be unique among the `multi_rate_limit` decorators on that endpoint:
+
+```python
+from fastapi_user_limiter.limiter import RateLimiter, multi_rate_limit
+from fastapi import FastAPI, Request
 
 app = FastAPI()
 rate_limiter = RateLimiter()
 
 
-@app.get("/")
-@rate_limit(rate_limiter, 5, 60)
-async def read_root(request: Request):
-    return {"Hello": "World"}
+# 1 request max per second, 3 requests max per 10 seconds
+@app.get("/multi")
+@multi_rate_limit(1, rate_limiter, 1, 1)
+@multi_rate_limit(2, rate_limiter, 3, 10)
+async def read_multi(request: Request):
+    return {"Hello": "There"}
 ```
 
-Every endpoint handler with the rate limiter decorator needs to have `request` (of type `fastapi.Request`) as its first argument.
+The aforementioned examples can be found in `example.py` (use ` uvicorn example:app --reload` to run).
+
+
+**NOTE**: Every endpoint handler with the rate limiter decorator needs to have `request` (of type `fastapi.Request`)
+as its first argument.
 
 ## Future features
 
 The package will soon have the additional feature of allowing each user account to have a different rate limit for each endpoint.
```

