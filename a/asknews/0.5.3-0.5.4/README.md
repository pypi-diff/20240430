# Comparing `tmp/asknews-0.5.3-py3-none-any.whl.zip` & `tmp/asknews-0.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 22606 bytes, number of entries: 24
+Zip file size: 22590 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 asknews_sdk/__init__.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 asknews_sdk/api/__init__.py
 -rw-r--r--  2.0 unx     4442 b- defN 80-Jan-01 00:00 asknews_sdk/api/analytics.py
 -rw-r--r--  2.0 unx      170 b- defN 80-Jan-01 00:00 asknews_sdk/api/base.py
 -rw-r--r--  2.0 unx     8439 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
 -rw-r--r--  2.0 unx    11705 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
 -rw-r--r--  2.0 unx    10424 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
@@ -11,16 +11,16 @@
 -rw-r--r--  2.0 unx     2430 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
 -rw-r--r--  2.0 unx     3983 b- defN 80-Jan-01 00:00 asknews_sdk/dto/chat.py
 -rw-r--r--  2.0 unx      606 b- defN 80-Jan-01 00:00 asknews_sdk/dto/error.py
 -rw-r--r--  2.0 unx     1284 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
 -rw-r--r--  2.0 unx      552 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
 -rw-r--r--  2.0 unx     4200 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1414 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
--rw-r--r--  2.0 unx     6302 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
+-rw-r--r--  2.0 unx     6274 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5248 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1583 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.5.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3185 b- defN 80-Jan-01 00:00 asknews-0.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.5.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.5.3.dist-info/RECORD
-24 files, 86373 bytes uncompressed, 19572 bytes compressed:  77.3%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.5.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3185 b- defN 80-Jan-01 00:00 asknews-0.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.5.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.5.4.dist-info/RECORD
+24 files, 86345 bytes uncompressed, 19556 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.5.3.dist-info/LICENSE
+Filename: asknews-0.5.4.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.5.3.dist-info/METADATA
+Filename: asknews-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.5.3.dist-info/WHEEL
+Filename: asknews-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.5.3.dist-info/RECORD
+Filename: asknews-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asknews_sdk/sdk.py

```diff
@@ -18,15 +18,15 @@
     AsyncStoriesAPI,
     NewsAPI,
     AsyncNewsAPI,
     ChatAPI,
     AsyncChatAPI,
 )
 
-DEFAULT_API_BASE_URL = "https://feat-stories-service.review.api.asknews.app"
+DEFAULT_API_BASE_URL = "https://api.asknews.app"
 DEFAULT_TOKEN_URL = "https://auth.asknews.app/oauth2/token"
 
 class AskNewsSDK:
     """
     The AskNews SDK client for communicating with the AskNews API.
 
     Usage:
```

## Comparing `asknews-0.5.3.dist-info/LICENSE` & `asknews-0.5.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.5.3.dist-info/METADATA` & `asknews-0.5.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asknews
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python SDK for AskNews
 Home-page: https://gitlab.com/emergentmethods/asknews/python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `asknews-0.5.3.dist-info/RECORD` & `asknews-0.5.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 asknews_sdk/dto/base.py,sha256=qWmt8bTCSYMFNALZyTEpuQZRu_yesSqJWbJ3maMeqcg,2430
 asknews_sdk/dto/chat.py,sha256=FqrpKuM4jmIvrqoAE3egW8mTAVw3III9mplK-tXDK8M,3983
 asknews_sdk/dto/error.py,sha256=XhOo_lgl9vVHbhUVQiFIUXVaXAexUULjr7Hph5b6Ovc,606
 asknews_sdk/dto/news.py,sha256=vI3CC3rljq9I7T5ivp97KZpbvSeJJzel7b5N3qFEqyo,1284
 asknews_sdk/dto/sentiment.py,sha256=m6d-5mQ0dd4vewj7wF3-IZGLknXHkaKRmdYbyUaYI50,552
 asknews_sdk/dto/stories.py,sha256=lqgKFPo3rOWqJeJWQ5UVAKUc-XHfL8h0Jt46vHSAiKg,4200
 asknews_sdk/errors.py,sha256=F7VncOcrCxM1mYGCqV2NUGDnDnqQWgxhhmXd__-5bK8,1414
-asknews_sdk/sdk.py,sha256=etSaKeGiUIQ2qd1Ek_m86eKTEe7FbAYacUq1UdY1Nd4,6302
+asknews_sdk/sdk.py,sha256=ljfgbkpJT5lW-ATx1eVkPI9WyeJwRSdClwL_puHAkyA,6274
 asknews_sdk/security.py,sha256=C3_-lQMwHNx9E-4GC4LedXofJ2ybZLGQGxIh55nVvks,5248
 asknews_sdk/utils.py,sha256=YAk-0ANXWu7J9PlKCyptXZnlvle4cLXuQWXxjxxWojQ,1583
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.5.3.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.5.3.dist-info/METADATA,sha256=Oos1pkKou2NMaZq481QCEdBNJ5Wp0ceog4_0T5pCcq8,3185
-asknews-0.5.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.5.3.dist-info/RECORD,,
+asknews-0.5.4.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.5.4.dist-info/METADATA,sha256=0sWjEy2wxwl3ijA875r2gG6npLX4dI0c1uFuOiad7Pg,3185
+asknews-0.5.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.5.4.dist-info/RECORD,,
```

