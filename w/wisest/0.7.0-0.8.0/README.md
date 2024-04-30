# Comparing `tmp/wisest-0.7.0-py3-none-any.whl.zip` & `tmp/wisest-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 6517 bytes, number of entries: 12
+Zip file size: 6659 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      452 b- defN 80-Jan-01 00:00 wise/__init__.py
 -rw-r--r--  2.0 unx     1252 b- defN 80-Jan-01 00:00 wise/cli.py
 -rw-r--r--  2.0 unx      771 b- defN 80-Jan-01 00:00 wise/cost.py
--rw-r--r--  2.0 unx      672 b- defN 80-Jan-01 00:00 wise/currency.py
+-rw-r--r--  2.0 unx      583 b- defN 80-Jan-01 00:00 wise/currency.py
 -rw-r--r--  2.0 unx     2157 b- defN 80-Jan-01 00:00 wise/method.py
--rw-r--r--  2.0 unx     3587 b- defN 80-Jan-01 00:00 wise/price.py
--rw-r--r--  2.0 unx     1825 b- defN 80-Jan-01 00:00 wise/rate.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      546 b- defN 80-Jan-01 00:00 wisest-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.7.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      873 b- defN 16-Jan-01 00:00 wisest-0.7.0.dist-info/RECORD
-12 files, 13326 bytes uncompressed, 5081 bytes compressed:  61.9%
+-rw-r--r--  2.0 unx     3493 b- defN 80-Jan-01 00:00 wise/price.py
+-rw-r--r--  2.0 unx     1707 b- defN 80-Jan-01 00:00 wise/rate.py
+-rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 wise/request.py
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 wisest-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.8.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      943 b- defN 16-Jan-01 00:00 wisest-0.8.0.dist-info/RECORD
+13 files, 13172 bytes uncompressed, 5117 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -15,23 +15,26 @@
 
 Filename: wise/price.py
 Comment: 
 
 Filename: wise/rate.py
 Comment: 
 
-Filename: wisest-0.7.0.dist-info/LICENSE
+Filename: wise/request.py
 Comment: 
 
-Filename: wisest-0.7.0.dist-info/METADATA
+Filename: wisest-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: wisest-0.7.0.dist-info/WHEEL
+Filename: wisest-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: wisest-0.7.0.dist-info/entry_points.txt
+Filename: wisest-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: wisest-0.7.0.dist-info/RECORD
+Filename: wisest-0.8.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: wisest-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wise/currency.py

```diff
@@ -1,25 +1,22 @@
 from __future__ import annotations
 
-import requests
 from pydantic import BaseModel
 from pydantic import Field
-from requests.utils import default_headers
 
-default_timeout = 10
+from .request import get
 
 
 class CurrencyRequest(BaseModel):
     def do(self) -> list[Currency]:
-        resp = requests.get(
+        resp = get(
             url="https://wise.com/gateway/v1/currencies",
-            headers=default_headers(),
-            timeout=default_timeout,
         )
-        return [Currency(**c) for c in resp.json()]
+        resp.raise_for_status()
+        return [Currency.model_validate(data) for data in resp.json()]
 
 
 class Currency(BaseModel):
     code: str
     symbol: str
     name: str
     country_keywords: list[str] = Field(alias="countryKeywords")
```

## wise/price.py

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
-import requests
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import field_validator
-from requests.utils import default_headers
 
-default_timeout = 10
+from .request import get
 
 
 class Price(BaseModel):
     price_set_id: int = Field(validation_alias="priceSetId")
     source_amount: float = Field(validation_alias="sourceAmount")
     target_amount: float = Field(validation_alias="targetAmount")
     pay_in_method: str = Field(validation_alias="payInMethod")
@@ -44,21 +42,20 @@
     def upper(cls, s: str) -> str:
         return s.upper()
 
     def do(self) -> list[Price]:
         # https://wise.com/gb/pricing/receive
         # https://wise.com/gb/pricing/send-money
 
-        resp = requests.get(
-            url="http://wise.com/gateway/v1/price",
+        resp = get(
+            url="https://wise.com/gateway/v1/price",
             params=self.model_dump(exclude_none=True, by_alias=True),
-            headers=default_headers(),
-            timeout=default_timeout,
         )
-        return [Price(**data) for data in resp.json()]
+        resp.raise_for_status()
+        return [Price.model_validate(data) for data in resp.json()]
 
 
 def find_price(
     prices: list[Price],
     pay_in_method: str = "VISA_CREDIT",
     pay_out_method: str = "BALANCE",
 ) -> Price:
```

## wise/rate.py

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 
-import requests
 from pydantic import BaseModel
 from pydantic import field_validator
-from requests.utils import default_headers
 
-default_timeout = 10
+from .request import get
 
 
 # {"source":"EUR","target":"USD","value":1.05425,"time":1697653800557}
 class Rate(BaseModel):
     source: str
     target: str
     value: float
@@ -42,21 +40,20 @@
 
 
 class RateRequest(BaseModel):
     source: str
     target: str
 
     def do(self) -> Rate:
-        resp = requests.get(
+        resp = get(
             "https://wise.com/rates/live",
             params=self.model_dump(),
-            headers=default_headers(),
-            timeout=default_timeout,
         )
-        return Rate(**resp.json())
+        resp.raise_for_status()
+        return Rate.model_validate(resp.json())
 
 
 def query_rate(source: str, target: str) -> Rate:
     return RateRequest(source=source, target=target).do()
 
 
 # https://wise.com/rates/history?source=EUR&target=USD&length=10&resolution=daily&unit=day
@@ -64,14 +61,13 @@
     source: str
     target: str
     length: int
     resolution: Resolution
     unit: Unit
 
     def do(self) -> list[Rate]:
-        resp = requests.get(
+        resp = get(
             url="https://wise.com/rates/history",
-            params=self.model_dump(),
-            headers=default_headers(),
-            timeout=default_timeout,
+            params=self.model_dump(mode="json"),
         )
-        return [Rate(**r) for r in resp.json()]
+        resp.raise_for_status()
+        return [Rate.model_validate(data) for data in resp.json()]
```

## Comparing `wisest-0.7.0.dist-info/LICENSE` & `wisest-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wisest-0.7.0.dist-info/METADATA` & `wisest-0.8.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wisest
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
```

