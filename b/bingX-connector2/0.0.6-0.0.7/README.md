# Comparing `tmp/bingX-connector2-0.0.6.tar.gz` & `tmp/bingX-connector2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingX-connector2-0.0.6.tar", last modified: Tue Apr  2 18:01:05 2024, max compression
+gzip compressed data, was "bingX-connector2-0.0.7.tar", last modified: Mon Apr 29 22:44:33 2024, max compression
```

## Comparing `bingX-connector2-0.0.6.tar` & `bingX-connector2-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)    35149 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/LICENSE
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     6481 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/PKG-INFO
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     5980 2024-03-09 12:46:00.000000 bingX-connector2-0.0.6/README.md
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.949060 bingX-connector2-0.0.6/bingX/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       99 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     2389 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/api.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      786 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/error.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.949060 bingX-connector2-0.0.6/bingX/perpetual/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)        0 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/__init__.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX/perpetual/v1/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1771 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/Perpetual.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       88 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      940 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/account.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     4492 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/market.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1299 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/other.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     9036 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/trade.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX/perpetual/v2/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1732 2024-03-04 13:41:22.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/Perpetual.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       88 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1761 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/account.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     4357 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/market.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     9337 2024-04-02 17:59:26.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/trade.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX/spot/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1316 2024-03-04 13:41:10.000000 bingX-connector2-0.0.6/bingX/spot/Spot.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       62 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1412 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/market.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1305 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/other.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     3703 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/trade.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     3261 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/transfer.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX/standard/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      778 2024-03-04 13:41:00.000000 bingX-connector2-0.0.6/bingX/standard/Standard.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       78 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/standard/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1438 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/standard/trade.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX_connector2.egg-info/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     6481 2024-04-02 18:01:05.000000 bingX-connector2-0.0.6/bingX_connector2.egg-info/PKG-INFO
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      852 2024-04-02 18:01:05.000000 bingX-connector2-0.0.6/bingX_connector2.egg-info/SOURCES.txt
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)        1 2024-04-02 18:01:05.000000 bingX-connector2-0.0.6/bingX_connector2.egg-info/dependency_links.txt
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       12 2024-04-02 18:01:05.000000 bingX-connector2-0.0.6/bingX_connector2.egg-info/top_level.txt
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       38 2024-04-02 18:01:05.955727 bingX-connector2-0.0.6/setup.cfg
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      853 2024-04-02 18:00:41.000000 bingX-connector2-0.0.6/setup.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/tests/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)        0 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/tests/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1694 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/tests/test_spot.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      674 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/tests/test_standard.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.780742 bingX-connector2-0.0.7/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)    35149 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/LICENSE
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     6481 2024-04-29 22:44:33.780742 bingX-connector2-0.0.7/PKG-INFO
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     5980 2024-03-09 12:46:00.000000 bingX-connector2-0.0.7/README.md
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.777408 bingX-connector2-0.0.7/bingX/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       99 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     2389 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/api.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      786 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/error.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.777408 bingX-connector2-0.0.7/bingX/perpetual/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)        0 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/perpetual/__init__.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.777408 bingX-connector2-0.0.7/bingX/perpetual/v1/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1771 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/perpetual/v1/Perpetual.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       88 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/perpetual/v1/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      936 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/perpetual/v1/account.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     4472 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/perpetual/v1/market.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1293 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/perpetual/v1/other.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     9000 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/perpetual/v1/trade.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.777408 bingX-connector2-0.0.7/bingX/perpetual/v2/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1732 2024-03-04 13:41:22.000000 bingX-connector2-0.0.7/bingX/perpetual/v2/Perpetual.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       88 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/perpetual/v2/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1755 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/perpetual/v2/account.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     4339 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/perpetual/v2/market.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     9307 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/perpetual/v2/trade.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.777408 bingX-connector2-0.0.7/bingX/spot/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1316 2024-03-04 13:41:10.000000 bingX-connector2-0.0.7/bingX/spot/Spot.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       62 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/spot/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1406 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/spot/market.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1299 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/spot/other.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     3691 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/spot/trade.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     3253 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/spot/transfer.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.777408 bingX-connector2-0.0.7/bingX/standard/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      778 2024-03-04 13:41:00.000000 bingX-connector2-0.0.7/bingX/standard/Standard.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       78 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/bingX/standard/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1432 2024-04-29 22:43:53.000000 bingX-connector2-0.0.7/bingX/standard/trade.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.777408 bingX-connector2-0.0.7/bingX_connector2.egg-info/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     6481 2024-04-29 22:44:33.000000 bingX-connector2-0.0.7/bingX_connector2.egg-info/PKG-INFO
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      852 2024-04-29 22:44:33.000000 bingX-connector2-0.0.7/bingX_connector2.egg-info/SOURCES.txt
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)        1 2024-04-29 22:44:33.000000 bingX-connector2-0.0.7/bingX_connector2.egg-info/dependency_links.txt
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       12 2024-04-29 22:44:33.000000 bingX-connector2-0.0.7/bingX_connector2.egg-info/top_level.txt
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       38 2024-04-29 22:44:33.780742 bingX-connector2-0.0.7/setup.cfg
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      853 2024-04-29 22:44:01.000000 bingX-connector2-0.0.7/setup.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-29 22:44:33.777408 bingX-connector2-0.0.7/tests/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)        0 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/tests/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1694 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/tests/test_spot.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      674 2024-03-04 13:27:08.000000 bingX-connector2-0.0.7/tests/test_standard.py
```

### Comparing `bingX-connector2-0.0.6/LICENSE` & `bingX-connector2-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/PKG-INFO` & `bingX-connector2-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingX-connector2
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple connector to BingX Public API
 Home-page: https://github.com/demonarch/bingX-connector-python
 Author: Ming119
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `bingX-connector2-0.0.6/README.md` & `bingX-connector2-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/bingX/api.py` & `bingX-connector2-0.0.7/bingX/api.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/bingX/error.py` & `bingX-connector2-0.0.7/bingX/error.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v1/Perpetual.py` & `bingX-connector2-0.0.7/bingX/perpetual/v1/Perpetual.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v1/account.py` & `bingX-connector2-0.0.7/bingX/perpetual/v1/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     https://bingx-api.github.io/docs/swap/account-api.html#_1-get-perpetual-swap-account-asset-information
     '''
     res = self.post("/api/v1/user/getBalance", params={
         "currency": currency,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def positions(self,
     symbol: str,
 ) -> dict:
     ''' Perpetual Swap Positions
     POST /api/v1/user/getPositions
@@ -29,9 +29,9 @@
     https://bingx-api.github.io/docs/swap/account-api.html#_2-perpetual-swap-positions
     '''
     res = self.post("/api/v1/user/getPositions", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
```

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v1/market.py` & `bingX-connector2-0.0.7/bingX/perpetual/v1/market.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     GET /api/v1/market/getAllContracts
 
     https://bingx-api.github.io/docs/swap/market-api.html#_1-contract-information
     '''
     res = self.get("/api/v1/market/getAllContracts")
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def latest_price(self,
     symbol: str,
 ) -> dict:
     ''' Get Latest Price of a Trading Pair
     GET /api/v1/market/getLatestPrice
@@ -25,15 +25,15 @@
     https://bingx-api.github.io/docs/swap/market-api.html#_2-get-latest-price-of-a-trading-pair
     '''
     res = self.get("/api/v1/market/getLatestPrice", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def market_depth(self,
     symbol: str,
     level:  int = None,
 ) -> dict:
     ''' Get Market Depth
@@ -43,15 +43,15 @@
     '''
     res = self.get("/api/v1/market/getMarketDepth", params={
         "symbol": symbol,
         "level":  level,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def latest_trade(self,
     symbol: str,
 ) -> dict:
     ''' The latest Trade of a Trading Pair
     GET /api/v1/market/getMarketTrades
@@ -59,15 +59,15 @@
     https://bingx-api.github.io/docs/swap/market-api.html#_4-the-latest-trade-of-a-trading-pair
     '''
     res = self.get("/api/v1/market/getMarketTrades", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def current_funding_rate(self,
     symbol: str,
 ) -> dict:
     ''' Current Funding Rate
     GET /api/v1/market/getLatestFunding
@@ -75,15 +75,15 @@
     https://bingx-api.github.io/docs/swap/market-api.html#_5-current-funding-rate
     '''
     res = self.get("/api/v1/market/getLatestFunding", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def funding_rate_history(self,
     symbol: str,
 ) -> dict:
     ''' Funding Rate History
     GET /api/v1/market/getHistoryFunding
@@ -91,15 +91,15 @@
     https://bingx-api.github.io/docs/swap/market-api.html#_6-funding-rate-history
     '''
     res = self.get("/api/v1/market/getHistoryFunding", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def kline_data(self,
     symbol:    str,
     klineType: str,
 ) -> dict:
     ''' Get K-Line Data
@@ -109,15 +109,15 @@
     '''
     res = self.get("/api/v1/market/getLatestKline", params={
         "symbol":    symbol,
         "klineType": klineType,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def kline_data_history(self,
     symbol:    str,
     klineType: str,
     startTs:   int,
     endTs:     int,
@@ -131,15 +131,15 @@
         "symbol":    symbol,
         "klineType": klineType,
         "startTs":   startTs,
         "endTs":     endTs,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def open_positions(self,
     symbol: str,
 ) -> dict:
     ''' Get Swap Open Positions
     GET /api/v1/market/getOpenPositions
@@ -147,15 +147,15 @@
     https://bingx-api.github.io/docs/swap/market-api.html#_9-get-swap-open-positions
     '''
     res = self.get("/api/v1/market/getOpenPositions", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def ticker(self,
     symbol: str = None,
 ) -> dict:
     ''' Get Ticker
     GET /api/v1/market/getTicker
@@ -163,9 +163,9 @@
     https://bingx-api.github.io/docs/swap/market-api.html#_10-get-ticker
     '''
     res = self.get("/api/v1/market/getTicker", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
```

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v1/other.py` & `bingX-connector2-0.0.7/bingX/perpetual/v1/other.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     POST /api/v1/user/auth/userDataStream
 
     https://bingx-api.github.io/docs/swap/other-interface.html#generate-listen-key
     '''
     res = self.post("/api/v1/user/auth/userDataStream")
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
 
 def extend_listen_key(self,
     listenKey: str,
 ) -> dict:
     ''' Extend Listen Key
     PUT /api/v1/user/auth/userDataStream
@@ -25,15 +25,15 @@
     https://bingx-api.github.io/docs/swap/other-interface.html#extend-listen-key-validity-period
     '''
     res = self.put("/api/v1/user/auth/userDataStream", params={
         "listenKey": listenKey,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
 
 def delete_listen_key(self,
     listenKey: str,
 ) -> dict:
     ''' Delete Listen Key
     DELETE /api/v1/user/auth/userDataStream
@@ -41,9 +41,9 @@
     https://bingx-api.github.io/docs/swap/other-interface.html#delete-listen-key
     '''
     res = self.delete("/api/v1/user/auth/userDataStream", params={
         "listenKey": listenKey,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
```

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v1/trade.py` & `bingX-connector2-0.0.7/bingX/perpetual/v1/trade.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "tradeType":        tradeType,
         "action":           action,
         "takerProfitPrice": takerProfitPrice,
         "stopLossPrice":    stopLossPrice,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def close_position(self,
     symbol:     str,
     positionId: str,
 ) -> dict:
     ''' One-Click Close Position
@@ -46,27 +46,27 @@
     '''
     res = self.post("/api/v1/user/oneClickClosePosition", params={
         "symbol":     symbol,
         "positionId": positionId,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def close_all_positions(self) -> dict:
     ''' One-Click Close All Positions
     POST /api/v1/user/oneClickCloseAllPositions
 
     https://bingx-api.github.io/docs/swap/trade-api.html#_3-one-click-close-all-positions
     '''
     res = self.post("/api/v1/user/oneClickCloseAllPositions")
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def cancel_order(self,
     symbol:  str,
     orderId: str,
 ) -> dict:
     ''' Cancel an Order
@@ -74,15 +74,15 @@
     '''
     res = self.post("/api/v1/user/cancelOrder", params={
         "symbol":  symbol,
         "orderId": orderId,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def cancel_orders(self,
     symbol:   str,
     orderIds: List[str],
 ) -> dict:
     ''' Cancel Multiple Orders
@@ -92,27 +92,27 @@
     '''
     res = self.post("/api/v1/user/batchCancelOrders", params={
         "symbol": symbol,
         "oids":   orderIds,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def cancel_all_orders(self) -> dict:
     ''' Cancel All Orders
     POST /api/v1/user/cancelAll
 
     https://bingx-api.github.io/docs/swap/trade-api.html#_6-cancel-all-orders
     '''
     res = self.post("/api/v1/user/cancelAll")
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def unfilled_order_acquisition(self,
     symbol: str,
 ) -> dict:
     ''' Unfilled Order Acquisition
     POST /api/v1/user/pendingOrders
@@ -120,15 +120,15 @@
     https://bingx-api.github.io/docs/swap/trade-api.html#_7-unfilled-order-acquisition
     '''
     res = self.post("/api/v1/user/pendingOrders", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def order_details(self,
     symbol:  str,
     orderId: str,
 ) -> dict:
     ''' Query Order Details
@@ -138,15 +138,15 @@
     '''
     res = self.post("/api/v1/user/orderInfo", params={
         "symbol":  symbol,
         "orderId": orderId,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def margin_mode(self,
     symbol: str,
 ) -> dict:
     ''' Query Margin Mode
     POST /api/v1/user/getMarginMode
@@ -154,15 +154,15 @@
     https://bingx-api.github.io/docs/swap/trade-api.html#_9-query-margin-mode
     '''
     res = self.post("/api/v1/user/getMarginMode", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def switch_margin_mode(self,
     symbol:     str,
     marginMode: str,
 ) -> dict:
     ''' Switch Margin Mode
@@ -172,15 +172,15 @@
     '''
     res = self.post("/api/v1/user/setMarginMode", params={
         "symbol":     symbol,
         "marginMode": marginMode,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def leverage(self,
     symbol: str,
 ) -> dict:
     ''' Query Leverage
     POST /api/v1/user/getLeverage
@@ -188,15 +188,15 @@
     https://bingx-api.github.io/docs/swap/trade-api.html#_11-query-leverage
     '''
     res = self.post("/api/v1/user/getLeverage", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def switch_leverage(self,
     symbol:   str,
     side:     str,
     leverage: int,
 ) -> dict:
@@ -208,15 +208,15 @@
     res = self.post("/api/v1/user/setLeverage", params={
         "symbol":   symbol,
         "side":     side,
         "leverage": leverage,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
 
 def force_orders(self,
     symbol:        str,
     autoCloseType: str,
     lastOrderId:   int,
     length:        int,
@@ -230,15 +230,15 @@
         "symbol":        symbol,
         "autoCloseType": autoCloseType,
         "lastOrderId":   lastOrderId,
         "length":        length,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def orders_history(self,
     symbol:      str,
     lastOrderId: int,
     length:      int,
 ) -> dict:
@@ -250,15 +250,15 @@
     res = self.post("/api/v1/user/historyOrders", params={
         "symbol":      symbol,
         "lastOrderId": lastOrderId,
         "length":      length,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def place_a_stop_order(self,
     positionId:      str,
     entrustVolume:   float,
     orderId:         str   = None,
     stopLossPrice:   float = None,
@@ -274,15 +274,15 @@
         "orderId":         orderId,
         "stopLossPrice":   stopLossPrice,
         "takeProfitPrice": takeProfitPrice,
         "entrustVolume":   entrustVolume,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def cancel_stop_order(self,
     orderId: str,
 ) -> dict:
     ''' Cancel a Stop Order
     POST /api/v1/user/cancelStopOrder
@@ -290,15 +290,15 @@
     https://bingx-api.github.io/docs/swap/trade-api.html#_16-cancel-stop-order
     '''
     res = self.post("/api/v1/user/cancelStopOrder", params={
         "orderId": orderId,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def stop_orders(self,
     symbol: str,
 ) -> dict:
     ''' Query Stop Orders
     POST /api/v1/user/pendingStopOrders
@@ -306,15 +306,15 @@
     https://bingx-api.github.io/docs/swap/trade-api.html#_17-query-stop-orders
     '''
     res = self.post("/api/v1/user/pendingStopOrders", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def stop_orders_history(self,
     symbol:      str,
     lastOrderId: int,
     length:      int,
 ) -> dict:
@@ -326,9 +326,9 @@
     res = self.post("/api/v1/user/historyStopOrders", params={
         "symbol":      symbol,
         "lastOrderId": lastOrderId,
         "length":      length,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
```

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v2/Perpetual.py` & `bingX-connector2-0.0.7/bingX/perpetual/v2/Perpetual.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v2/account.py` & `bingX-connector2-0.0.7/bingX/perpetual/v2/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     https://bingx-api.github.io/docs/swapV2/account-api.html#_1-get-perpetual-swap-account-asset-information
     '''
     res = self.get("/openApi/swap/v2/user/balance", params={
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def positions(self,
     symbol: str,
     recvWindow: int = None,
 ) -> dict:
     ''' Perpetual Swap Positions
@@ -31,15 +31,15 @@
     '''
     res = self.get("/openApi/swap/v2/user/positions", params={
         "symbol": symbol,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def income(self,
     symbol: str = None,
     incomeType: str = None,
     startTime: int = None,
     endTime: int = None,
@@ -57,9 +57,9 @@
         "startTime": startTime,
         "endTime": endTime,
         "limit": limit,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
```

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v2/market.py` & `bingX-connector2-0.0.7/bingX/perpetual/v2/market.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     GET /openApi/swap/v2/quote/contracts
 
     https://bingx-api.github.io/docs/swapV2/market-api.html#_1-contract-information
     '''
     res = self.get("/openApi/swap/v2/quote/contracts")
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def latest_price(self,
     symbol: str = None,
 ) -> dict:
     ''' Get Latest Price of a Trading Pair
     GET /openApi/swap/v2/quote/price
@@ -25,15 +25,15 @@
     https://bingx-api.github.io/docs/swapV2/market-api.html#_2-get-latest-price-of-a-trading-pair
     '''
     res = self.get("/openApi/swap/v2/quote/price", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def market_depth(self,
     symbol: str,
     limit:  int = None,
 ) -> dict:
     ''' Get Market Depth
@@ -43,15 +43,15 @@
     '''
     res = self.get("/openApi/swap/v2/quote/depth", params={
         "symbol": symbol,
         "limit":  limit,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def latest_trade(self,
     symbol: str,
     limit:  int = None,
 ) -> dict:
     ''' The latest Trade of a Trading Pair
@@ -61,15 +61,15 @@
     '''
     res = self.get("/openApi/swap/v2/quote/trades", params={
         "symbol": symbol,
         "limit":  limit,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def current_funding_rate(self,
     symbol: str = None,
 ) -> dict:
     ''' Current Funding Rate
     GET /openApi/swap/v2/quote/premiumIndex
@@ -77,15 +77,15 @@
     https://bingx-api.github.io/docs/swapV2/market-api.html#_5-current-funding-rate
     '''
     res = self.get("/openApi/swap/v2/quote/premiumIndex", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def funding_rate_history(self,
     symbol:    str,
     startTime: int = None,
     endTime:   int = None,
     limit:     int = None,
@@ -99,15 +99,15 @@
         "symbol":    symbol,
         "startTime": startTime,
         "endTime":   endTime,
         "limit":     limit,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def kline(self,
     symbol:    str,
     interval:  str,
     startTime: int = None,
     endTime:   int = None,
@@ -123,15 +123,15 @@
         "interval":  interval,
         "startTime": startTime,
         "endTime":   endTime,
         "limit":     limit,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def get_open_positions(self,
     symbol: str,
 ) -> dict:
     ''' Get Swap Open Positions
     GET /openApi/swap/v2/quote/openInterest
@@ -139,15 +139,15 @@
     https://bingx-api.github.io/docs/swapV2/market-api.html#_8-get-swap-open-positions
     '''
     res = self.get("/openApi/swap/v2/quote/openInterest", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def ticker(self,
     symbol: str = None,
 ) -> dict:
     ''' Get Ticker
     GET /openApi/swap/v2/quote/ticker
@@ -155,9 +155,9 @@
     https://bingx-api.github.io/docs/swapV2/market-api.html#_9-get-ticker
     '''
     res = self.get("/openApi/swap/v2/quote/ticker", params={
         "symbol": symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
```

### Comparing `bingX-connector2-0.0.6/bingX/perpetual/v2/trade.py` & `bingX-connector2-0.0.7/bingX/perpetual/v2/trade.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         "recvWindow":   recvWindow,
 
         "takeProfit":  "{\"type\": \"TAKE_PROFIT_MARKET\", \"stopPrice\": %TAKE_PROFIT%,\"price\": %TAKE_PROFIT%,\"workingType\":\"MARK_PRICE\"}".replace("%TAKE_PROFIT%", str(takeProfit)) if takeProfit else None,
         "stopLoss":    "{\"type\": \"STOP_MARKET\", \"stopPrice\": %STOP_LOSS%,\"price\": %STOP_LOSS%,\"workingType\":\"MARK_PRICE\"}".replace("%STOP_LOSS%", str(stopLoss)) if stopLoss else None,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def bulk_order(self,
     batchOrders: List,
     recvWindow:  int = None,
 ) -> dict:
     ''' Bulk order
@@ -52,15 +52,15 @@
     '''
     res = self.post("/openApi/swap/v2/trade/batchOrders", params={
         "batchOrders": batchOrders,
         "recvWindow":  recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def close_all_positions(self,
     recvWindow: int = None,
 ) -> dict:
     ''' One-Click Close All Positions
     POST /openApi/swap/v2/trade/closeAllPositions
@@ -68,15 +68,15 @@
     https://bingx-api.github.io/docs/swapV2/trade-api.html#_3-one-click-close-all-positions
     '''
     res = self.post("/openApi/swap/v2/trade/closeAllPositions", params={
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def cancel_order(self,
     orderId:    int,
     symbol:     str,
     recvWindow: int = None,
 ) -> dict:
@@ -88,15 +88,15 @@
     res = self.delete("/openApi/swap/v2/trade/order", params={
         "orderId":    orderId,
         "symbol":     symbol,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def cancel_orders(self,
     symbol:      str,
     orderIdList: List[int],
     recvWindow:  int = None,
 ) -> dict:
@@ -108,15 +108,15 @@
     res = self.delete("/openApi/swap/v2/trade/batchOrders", params={
         "symbol":      symbol,
         "orderIdList": orderIdList,
         "recvWindow":  recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def cancel_all_orders(self,
     symbol:     str,
     recvWindow: int = None,
 ) -> dict:
     ''' Cancel All Orders
@@ -126,15 +126,15 @@
     '''
     res = self.post("/openApi/swap/v2/trade/allOpenOrders", params={
         "symbol":     symbol,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def current_orders(self,
     symbol:     str,
     recvWindow: int = None,
 ) -> dict:
     ''' Query all current pending orders
@@ -144,15 +144,15 @@
     '''
     res = self.get("/openApi/swap/v2/trade/openOrders", params={
         "symbol":     symbol,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def order(self,
     symbol:     str,
     orderId:    int,
     recvWindow: int = None,
 ) -> dict:
@@ -164,15 +164,15 @@
     res = self.get("/openApi/swap/v2/trade/order", params={
         "symbol":     symbol,
         "orderId":    orderId,
         "recvWindow": recvWindow,
     })
     
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def margin_mode(self,
     symbol:     str,
     recvWindow: int = None,
 ) -> dict:
     ''' Query Margin Mode
@@ -182,15 +182,15 @@
     '''
     res = self.get("/openApi/swap/v2/trade/marginType", params={
         "symbol":     symbol,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def switch_margin_mode(self,
     symbol:     str,
     marginType: str,
     recvWindow: int = None,
 ) -> dict:
@@ -202,15 +202,15 @@
     res = self.post("/openApi/swap/v2/trade/marginType", params={
         "symbol":     symbol,
         "marginType": marginType,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res  # No "data" return? 
 
 def leverage(self,
     symbol:     str,
     recvWindow: int = None,
 ) -> dict:
     ''' Query Leverage
@@ -220,15 +220,15 @@
     '''
     res = self.get("/openApi/swap/v2/trade/leverage", params={
         "symbol":     symbol,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def switch_leverage(self,
     symbol:     str,
     side:       str,
     leverage:   int,
     recvWindow: int = None,
@@ -242,15 +242,15 @@
         "symbol":     symbol,
         "side":       side,
         "leverage":   leverage,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def force_orders(self,
     symbol:        str = None,
     autoCloseType: str = None,
     startTime:     int = None,
     endTime:       int = None,
@@ -268,15 +268,15 @@
         "startTime":     startTime,
         "endTime":       endTime,
         "limit":         limit,
         "recvWindow":    recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def orders_history(self,
     symbol:     str,
     orderId:    int = None,
     startTime:  int = None,
     endTime:    int = None,
@@ -294,15 +294,15 @@
         "startTime":  startTime,
         "endTime":    endTime,
         "limit":      limit,
         "recvWindow": recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def adjust_isolated_margin(self,
     symbol:       str,
     amount:       float,
     type:         int,
     positionSide: str = None,
@@ -318,9 +318,9 @@
         "amount":       amount,
         "type":         type,
         "positionSide": positionSide,
         "recvWindow":   recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res  # no "data" return?
```

### Comparing `bingX-connector2-0.0.6/bingX/spot/Spot.py` & `bingX-connector2-0.0.7/bingX/spot/Spot.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/bingX/spot/market.py` & `bingX-connector2-0.0.7/bingX/spot/market.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     https://bingx-api.github.io/docs/spot/market-interface.html#query-symbols
     '''
     res = self.get('/openApi/spot/v1/common/symbols', params={
         'symbol': symbol,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def trades(self,
     symbol: str,
     limit:  int = None,
 ) -> dict:
     ''' Query transaction records
@@ -31,15 +31,15 @@
     '''
     res = self.get('/openApi/spot/v1/market/trades', params={
         'symbol': symbol,
         'limit':  limit,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def depth(self,
     symbol: str,
     limit:  int = None,
 ) -> dict:
     ''' Query depth information
@@ -49,9 +49,9 @@
     '''
     res = self.get('/openApi/spot/v1/market/depth', params={
         'symbol': symbol,
         'limit':  limit,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
```

### Comparing `bingX-connector2-0.0.6/bingX/spot/other.py` & `bingX-connector2-0.0.7/bingX/spot/other.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     POST /openApi/user/auth/userDataStream
 
     https://bingx-api.github.io/docs/spot/other-interface.html#generate-listen-key
     '''
     res = self.post('/openApi/user/auth/userDataStream')
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
 
 def extend_listen_key(self,
     listenKey: str,
 ) -> None:
     ''' Extend Listen Key Validity period
     PUT /openApi/user/auth/userDataStream
@@ -25,15 +25,15 @@
     https://bingx-api.github.io/docs/spot/other-interface.html#extend-listen-key-validity-period
     '''
     res = self.put('/openApi/user/auth/userDataStream', params={
         'listenKey': listenKey,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
 
 def delete_listen_key(self,
     listenKey: str,
 ) -> None:
     ''' Delete Listen Key
     DELETE /openApi/user/auth/userDataStream
@@ -41,9 +41,9 @@
     https://bingx-api.github.io/docs/spot/other-interface.html#delete-listen-key
     '''
     res = self.delete('/openApi/user/auth/userDataStream', params={
         'listenKey': listenKey,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
```

### Comparing `bingX-connector2-0.0.6/bingX/spot/trade.py` & `bingX-connector2-0.0.7/bingX/spot/trade.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         'quantity':      quantity,
         'quoteOrderQty': quoteOrderQty,
         'price':         price,
         'recvWindow':    recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def cancel_order(self,
     symbol:     str,
     orderId:    int,
     recvWindow: int = None,
 ) -> dict:
@@ -47,15 +47,15 @@
     res = self.post('/openApi/spot/v1/trade/cancel', params={
         'symbol':     symbol,
         'orderId':    orderId,
         'recvWindow': recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def order(self,
     symbol:     str,
     orderId:    int,
     recvWindow: int = None,
 ) -> dict:
@@ -67,15 +67,15 @@
     res = self.get('/openApi/spot/v1/trade/query', params={
         'symbol':     symbol,
         'orderId':    orderId,
         'recvWindow': recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def open_orders(self,   
     symbol:     str,
     recvWindow: int = None,
 ) -> dict:
     ''' Query Open Orders
@@ -85,15 +85,15 @@
     '''
     res = self.get('/openApi/spot/v1/trade/openOrders', params={
         'symbol':     symbol,
         'recvWindow': recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def order_history(self,
     symbol:     str,
     orderId:    int = None,
     startTime:  int = None,
     endTime:    int = None,
@@ -113,15 +113,15 @@
         'endTime':    endTime,
         'pageIndex':  pageIndex,
         'pageSize':   pageSize,
         'recvWindow': recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def assets(self,
     recvWindow: int = None,
 ) -> dict:
     ''' Query Assets
     GET /openApi/spot/v1/account/balance
@@ -129,9 +129,9 @@
     https://bingx-api.github.io/docs/spot/trade-interface.html#query-assets
     '''
     res = self.get('/openApi/spot/v1/account/balance', params={
         'recvWindow': recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
```

### Comparing `bingX-connector2-0.0.6/bingX/spot/transfer.py` & `bingX-connector2-0.0.7/bingX/spot/transfer.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         'type':       type,
         'asset':      asset,
         'amount':     amount,
         'recvWindow': recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
 
 def transfer_history(self,
     type:       str,
     startTime:  int   = None,
     endTime:    int   = None,
     current:    int   = None,
@@ -45,15 +45,15 @@
         'endTime':    endTime,
         'current':    current,
         'size':       size,
         'recvWindow': recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
 
 def deposit_history(self,
     coin:       str = None,
     status:     int = None,
     startTime:  int = None,
     endTime:    int = None,
@@ -73,15 +73,15 @@
         'endTime':    endTime,
         'offset':     offset,
         'limit':      limit,
         'recvWindow': recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
 
 def withdraw_history(self,
     coin:            str = None,
     withdrawOrderId: str = None,
     status:          int = None,
     startTime:       int = None,
@@ -103,9 +103,9 @@
         'endTime':         endTime,
         'offset':          offset,
         'limit':           limit,
         'recvWindow':      recvWindow,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res
```

### Comparing `bingX-connector2-0.0.6/bingX/standard/Standard.py` & `bingX-connector2-0.0.7/bingX/standard/Standard.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/bingX/standard/trade.py` & `bingX-connector2-0.0.7/bingX/standard/trade.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     GET /openApi/contract/v1/allPosition
 
     https://bingx-api.github.io/docs/standard/contract-interface.html#position
     '''
     res = self.get("/openApi/contract/v1/allPosition")
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def order_history(self,
     symbol:    str,
     orderId:   int = None,
     startTime: int = None,
     endTime:   int = None,
@@ -33,21 +33,21 @@
         "orderId":   orderId,
         "startTime": startTime,
         "endTime":   endTime,
         "limit":     limit,
     })
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
 
 def balance(self) -> dict:
     ''' Query standard contract balance
     GET /openApi/contract/v1/balance
 
     https://bingx-api.github.io/docs/standard/contract-interface.html#query-standard-contract-balance
     '''
     res = self.get("/openApi/contract/v1/balance")
 
     if 'code' in res and res['code']:
-        raise ClientError(res['code'], res['msg'])
+        raise Exception(res['code'], res['msg'])
     return res['data']
```

### Comparing `bingX-connector2-0.0.6/bingX_connector2.egg-info/PKG-INFO` & `bingX-connector2-0.0.7/bingX_connector2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingX-connector2
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple connector to BingX Public API
 Home-page: https://github.com/demonarch/bingX-connector-python
 Author: Ming119
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `bingX-connector2-0.0.6/bingX_connector2.egg-info/SOURCES.txt` & `bingX-connector2-0.0.7/bingX_connector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/setup.py` & `bingX-connector2-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 NAME = "bingX-connector2"
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 AUTHOR = "Ming119"
 URL = "https://github.com/demonarch/bingX-connector-python"
 
 setuptools.setup(
     name=NAME,
     version=VERSION,
     author=AUTHOR,
```

### Comparing `bingX-connector2-0.0.6/tests/test_spot.py` & `bingX-connector2-0.0.7/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.6/tests/test_standard.py` & `bingX-connector2-0.0.7/tests/test_standard.py`

 * *Files identical despite different names*

