# Comparing `tmp/cachext-1.2.0-py3-none-any.whl.zip` & `tmp/cachext-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5990 bytes, number of entries: 9
--rw-r--r--  2.0 unx       22 b- defN 22-Jul-26 06:06 cachext/__init__.py
--rw-r--r--  2.0 unx     9269 b- defN 22-Jul-26 06:06 cachext/backends.py
--rw-r--r--  2.0 unx     3274 b- defN 22-Jul-26 06:06 cachext/cache.py
--rw-r--r--  2.0 unx     2059 b- defN 22-Jul-26 06:06 cachext/exts.py
--rw-r--r--  2.0 unx     1064 b- defN 22-Jul-26 06:07 cachext-1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1625 b- defN 22-Jul-26 06:07 cachext-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-26 06:07 cachext-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Jul-26 06:07 cachext-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      680 b- defN 22-Jul-26 06:07 cachext-1.2.0.dist-info/RECORD
-9 files, 18093 bytes uncompressed, 4828 bytes compressed:  73.3%
+Zip file size: 6083 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-30 02:50 cachext/__init__.py
+-rw-r--r--  2.0 unx     9384 b- defN 24-Apr-30 02:50 cachext/backends.py
+-rw-r--r--  2.0 unx     3274 b- defN 24-Apr-30 02:50 cachext/cache.py
+-rw-r--r--  2.0 unx     2174 b- defN 24-Apr-30 02:50 cachext/exts.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-30 02:50 cachext-1.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1656 b- defN 24-Apr-30 02:50 cachext-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 02:50 cachext-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-30 02:50 cachext-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      680 b- defN 24-Apr-30 02:50 cachext-1.2.1.dist-info/RECORD
+9 files, 18354 bytes uncompressed, 4921 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: cachext/cache.py
 Comment: 
 
 Filename: cachext/exts.py
 Comment: 
 
-Filename: cachext-1.2.0.dist-info/LICENSE
+Filename: cachext-1.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: cachext-1.2.0.dist-info/METADATA
+Filename: cachext-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: cachext-1.2.0.dist-info/WHEEL
+Filename: cachext-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: cachext-1.2.0.dist-info/top_level.txt
+Filename: cachext-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cachext-1.2.0.dist-info/RECORD
+Filename: cachext-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cachext/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.2.0'
+__version__ = '1.2.1'
```

## cachext/backends.py

```diff
@@ -64,14 +64,16 @@
         raise NotImplementedError
 
 
 class Redis(BaseBackend):
 
     def __init__(self, prefix=None, default_ttl=600, **kwargs):
         import redis
+        from opentelemetry.instrumentation.redis import RedisInstrumentor
+        RedisInstrumentor().instrument()
         self._client = redis.StrictRedis(**kwargs)
         self.prefix = prefix
         self.default_ttl = default_ttl
 
     def get(self, key):
         key = self.trans_key(key)
         v = self._client.get(key)
```

## cachext/exts.py

```diff
@@ -43,14 +43,16 @@
 
     def __init__(self, ns='REDIS_'):
         self._client = None
         self.ns = ns
 
     def init_app(self, app):
         import redis
+        from opentelemetry.instrumentation.redis import RedisInstrumentor
+        RedisInstrumentor().instrument()
         opts = app.config.get_namespace(self.ns)
         self._pool = redis.ConnectionPool(**opts)
         self._client = redis.StrictRedis(connection_pool=self._pool)
 
     def __getattr__(self, name):
         return getattr(self._client, name)
```

## Comparing `cachext-1.2.0.dist-info/LICENSE` & `cachext-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cachext-1.2.0.dist-info/METADATA` & `cachext-1.2.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: cachext
-Version: 1.2.0
+Version: 1.2.1
 Summary: cache extension for sea/flask
 Home-page: https://github.com/shanbay/cachext
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: MIT
 Keywords: cache,flask,sea
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 License-File: LICENSE
+Requires-Dist: opentelemetry.instrumentation.redis
 
 # [Home Page](https://shanbay.github.io/cachext/)
 
 [![](https://img.shields.io/travis/shanbay/cachext.svg?style=flat-square)](https://travis-ci.org/shanbay/cachext)
 [![Maintainability](https://api.codeclimate.com/v1/badges/774db211d37720bb2599/maintainability)](https://codeclimate.com/github/shanbay/cachext/maintainability)
 [![Coverage Status](https://coveralls.io/repos/github/shanbay/cachext/badge.svg?branch=master)](https://coveralls.io/github/shanbay/cachext?branch=master)
 [![](https://img.shields.io/pypi/v/cachext.svg)](https://github.com/shanbay/cachext)
 [![](https://img.shields.io/pypi/pyversions/cachext.svg)](https://github.com/shanbay/cachext)
 [![](https://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://shanbay.mit-license.org)
-
-
```

