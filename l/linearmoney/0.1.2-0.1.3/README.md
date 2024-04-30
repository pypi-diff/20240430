# Comparing `tmp/linearmoney-0.1.2.tar.gz` & `tmp/linearmoney-0.1.3.tar.gz`

## Comparing `linearmoney-0.1.2.tar` & `linearmoney-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/_utils.py
--rw-r--r--   0        0        0    13168 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/cache.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/currencies.json
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/data.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/exceptions.py
--rw-r--r--   0        0        0  3144518 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/locales.json
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/mixins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/py.typed
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/resources.py
--rw-r--r--   0        0        0    13242 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/scalar.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/supported_iso_codes.json
--rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 linearmoney-0.1.2/src/linearmoney/vector.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 linearmoney-0.1.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 linearmoney-0.1.2/LICENSE
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 linearmoney-0.1.2/README.md
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 linearmoney-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 linearmoney-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/_utils.py
+-rw-r--r--   0        0        0    13168 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/cache.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/cldr_version.json
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/currencies.json
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/data.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/exceptions.py
+-rw-r--r--   0        0        0  3144508 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/locales.json
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/mixins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/py.typed
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/resources.py
+-rw-r--r--   0        0        0    13242 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/scalar.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/supported_iso_codes.json
+-rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/vector.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 linearmoney-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 linearmoney-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 linearmoney-0.1.3/README.md
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 linearmoney-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 linearmoney-0.1.3/PKG-INFO
```

### Comparing `linearmoney-0.1.2/src/linearmoney/_utils.py` & `linearmoney-0.1.3/src/linearmoney/_utils.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/src/linearmoney/cache.py` & `linearmoney-0.1.3/src/linearmoney/cache.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/src/linearmoney/currencies.json` & `linearmoney-0.1.3/src/linearmoney/currencies.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9832589285714286%*

 * *Differences: {"'AMD'": "{'cash_places': 0}",*

 * * "'COP'": "{'cash_places': 0}",*

 * * "'CRC'": "{'cash_places': 0}",*

 * * "'CZK'": "{'cash_places': 0}",*

 * * "'GYD'": "{'cash_places': 0}",*

 * * "'HUF'": "{'cash_places': 0}",*

 * * "'IDR'": "{'cash_places': 0}",*

 * * "'MNT'": "{'cash_places': 0}",*

 * * "'MUR'": "{'cash_places': 0}",*

 * * "'NOK'": "{'cash_places': 0}",*

 * * "'PKR'": "{'cash_places': 0}",*

 * * "'SEK'": "{'cash_places': 0}",*

 * * "'TWD'": "{'cash_places': 0}",*

 * * "'TZS'": "{'cash_places': 0}",*

 * * "'UZS'": "{'cash_places': 0}"}*

```diff
@@ -9,15 +9,15 @@
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
         "places": 0
     },
     "AMD": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "BHD": {
         "cash_denomination": 0,
         "cash_places": 3,
         "denomination": 0,
@@ -51,27 +51,27 @@
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
         "places": 0
     },
     "COP": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "CRC": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "CZK": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "DEFAULT": {
         "cash_denomination": 0,
         "cash_places": 2,
         "denomination": 0,
@@ -93,27 +93,27 @@
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
         "places": 0
     },
     "GYD": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "HUF": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "IDR": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "IQD": {
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
@@ -195,39 +195,39 @@
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
         "places": 0
     },
     "MNT": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "MUR": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "NOK": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "OMR": {
         "cash_denomination": 0,
         "cash_places": 3,
         "denomination": 0,
         "places": 3
     },
     "PKR": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "PYG": {
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
@@ -243,15 +243,15 @@
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
         "places": 0
     },
     "SEK": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "SLE": {
         "cash_denomination": 0,
         "cash_places": 2,
         "denomination": 0,
@@ -273,33 +273,33 @@
         "cash_denomination": 0,
         "cash_places": 3,
         "denomination": 0,
         "places": 3
     },
     "TWD": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "TZS": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "UGX": {
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
         "places": 0
     },
     "UZS": {
         "cash_denomination": 0,
-        "cash_places": 2,
+        "cash_places": 0,
         "denomination": 0,
         "places": 2
     },
     "VND": {
         "cash_denomination": 0,
         "cash_places": 0,
         "denomination": 0,
```

### Comparing `linearmoney-0.1.2/src/linearmoney/data.py` & `linearmoney-0.1.3/src/linearmoney/data.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/src/linearmoney/exceptions.py` & `linearmoney-0.1.3/src/linearmoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/src/linearmoney/locales.json` & `linearmoney-0.1.3/src/linearmoney/locales.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9922570654277982%*

 * *Differences: {"'accounting'": "{'ar_BH': {'negative_symbol_space': 1, 'positive_symbol_space': 1}, 'ar_DJ': "*

 * *                 "{'negative_symbol_space': 1, 'positive_symbol_space': 1}, 'ar_EG': "*

 * *                 "{'negative_symbol_space': 1, 'positive_symbol_space': 1}, 'ar_ER': "*

 * *                 "{'negative_symbol_space': 1, 'positive_symbol_space': 1}, 'ar_IL': "*

 * *                 "{'negative_symbol_space': 1, 'positive_symbol_space': 1}, 'ar_IQ': "*

 * *                 "{'negative_symbol_space': 1, 'positive_symbol_spa […]*

```diff
@@ -1127,22 +1127,22 @@
             "local_currency_code": "BHD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_DJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -1408,22 +1408,22 @@
             "local_currency_code": "DJF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_DZ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -1970,22 +1970,22 @@
             "local_currency_code": "EGP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_EH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -2532,22 +2532,22 @@
             "local_currency_code": "ERN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_IL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -2813,22 +2813,22 @@
             "local_currency_code": "ILS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_IQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -3094,22 +3094,22 @@
             "local_currency_code": "IQD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_JO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -3375,22 +3375,22 @@
             "local_currency_code": "JOD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_KM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -3656,22 +3656,22 @@
             "local_currency_code": "KMF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_KW": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -3937,22 +3937,22 @@
             "local_currency_code": "KWD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_LB": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -4218,22 +4218,22 @@
             "local_currency_code": "LBP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_LY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -5061,22 +5061,22 @@
             "local_currency_code": "MRU",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_OM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -5342,22 +5342,22 @@
             "local_currency_code": "OMR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_PS": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -5623,22 +5623,22 @@
             "local_currency_code": "ILS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_QA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -5904,22 +5904,22 @@
             "local_currency_code": "QAR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -6185,22 +6185,22 @@
             "local_currency_code": "SAR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -6466,22 +6466,22 @@
             "local_currency_code": "SDG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -6747,22 +6747,22 @@
             "local_currency_code": "SOS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SS": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -7028,22 +7028,22 @@
             "local_currency_code": "SSP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -7309,22 +7309,22 @@
             "local_currency_code": "SYP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_TD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -7590,22 +7590,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_TN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -8152,22 +8152,22 @@
             "local_currency_code": "YER",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "as_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -8629,22 +8629,22 @@
             "local_currency_code": "AZN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "be_BY": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -8815,22 +8815,22 @@
             "local_currency_code": "BYN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "bg_BG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "Af",
@@ -9106,22 +9106,22 @@
             "local_currency_code": "BGN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "bn_BD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -10023,22 +10023,22 @@
             "local_currency_code": "BAM",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ca_AD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -10344,22 +10344,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ca_ES": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -10665,22 +10665,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ca_FR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -10986,22 +10986,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ca_IT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -11307,22 +11307,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "chr_US": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -11816,22 +11816,22 @@
             "local_currency_code": "CZK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "cy_GB": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -12393,22 +12393,22 @@
             "local_currency_code": "DKK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "da_GL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -12687,22 +12687,22 @@
             "local_currency_code": "DKK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "de_AT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -13335,22 +13335,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "de_CH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -13983,22 +13983,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "de_IT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -14307,22 +14307,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "de_LI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -14955,22 +14955,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "dsb_DE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -15167,22 +15167,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "el_CY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -15459,22 +15459,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "el_GR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -15751,22 +15751,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_AE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -18359,22 +18359,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_BI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -22597,22 +22597,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_DG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -23249,22 +23249,22 @@
             "local_currency_code": "DKK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_DM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -24227,22 +24227,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_FJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -42157,22 +42157,22 @@
             "local_currency_code": "SEK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_SG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -43135,22 +43135,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_SL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -53001,22 +53001,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "es_EC": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -53605,22 +53605,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "es_GQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -54813,22 +54813,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "es_MX": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -56323,22 +56323,22 @@
             "local_currency_code": "PHP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "es_PR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -56925,15 +56925,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "PYG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -58431,22 +58431,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "eu_ES": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -58757,22 +58757,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fa_AF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -59594,22 +59594,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fil_PH": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -60090,22 +60090,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_BF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -60393,22 +60393,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_BI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -60696,22 +60696,22 @@
             "local_currency_code": "BIF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_BJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -60999,22 +60999,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_BL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -61302,22 +61302,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -61605,22 +61605,22 @@
             "local_currency_code": "CAD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -61908,22 +61908,22 @@
             "local_currency_code": "CDF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -62211,22 +62211,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -62514,22 +62514,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -62817,22 +62817,22 @@
             "local_currency_code": "CHF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -63120,22 +63120,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -63423,22 +63423,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_DJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -63726,22 +63726,22 @@
             "local_currency_code": "DJF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_DZ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -64029,22 +64029,22 @@
             "local_currency_code": "DZD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_FR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -64332,22 +64332,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -64635,22 +64635,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -64938,22 +64938,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -65241,22 +65241,22 @@
             "local_currency_code": "GNF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GP": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -65544,22 +65544,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -65847,22 +65847,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_HT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -66150,22 +66150,22 @@
             "local_currency_code": "HTG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_KM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -66453,22 +66453,22 @@
             "local_currency_code": "KMF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_LU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -66756,22 +66756,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -67059,22 +67059,22 @@
             "local_currency_code": "MAD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MC": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -67362,22 +67362,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -67665,22 +67665,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -67968,22 +67968,22 @@
             "local_currency_code": "MGA",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_ML": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -68271,22 +68271,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -68574,22 +68574,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -68877,22 +68877,22 @@
             "local_currency_code": "MRU",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -69180,22 +69180,22 @@
             "local_currency_code": "MUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_NC": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -69483,22 +69483,22 @@
             "local_currency_code": "XPF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_NE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -69786,22 +69786,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_PF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -70089,22 +70089,22 @@
             "local_currency_code": "XPF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_PM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -70392,22 +70392,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_RE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -70695,22 +70695,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_RW": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -70998,22 +70998,22 @@
             "local_currency_code": "RWF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_SC": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -71301,22 +71301,22 @@
             "local_currency_code": "SCR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_SN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -71604,22 +71604,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_SY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -71907,22 +71907,22 @@
             "local_currency_code": "SYP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_TD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -72210,22 +72210,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_TG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -72513,22 +72513,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_TN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -72816,22 +72816,22 @@
             "local_currency_code": "TND",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_VU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -73119,22 +73119,22 @@
             "local_currency_code": "VUV",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_WF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -73422,22 +73422,22 @@
             "local_currency_code": "XPF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_YT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -73725,22 +73725,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ga_GB": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -74877,22 +74877,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "gu_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -75887,22 +75887,22 @@
             "local_currency_code": "ILS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u200e-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u200e+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hi_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -76423,22 +76423,22 @@
             "local_currency_code": "BAM",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hr_HR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -76745,22 +76745,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hsb_DE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -76957,22 +76957,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hu_HU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -77267,22 +77267,22 @@
             "local_currency_code": "HUF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hy_AM": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -77454,22 +77454,22 @@
             "local_currency_code": "AMD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "id_ID": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -78206,22 +78206,22 @@
             "local_currency_code": "ISK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "it_CH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -78798,22 +78798,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "it_SM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -79094,22 +79094,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "it_VA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -79390,22 +79390,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ja_JP": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -80167,22 +80167,22 @@
             "local_currency_code": "GEL",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "kk_KZ": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -80353,22 +80353,22 @@
             "local_currency_code": "KZT",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "km_KH": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -82038,22 +82038,22 @@
             "local_currency_code": "KGS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "lo_LA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -82679,22 +82679,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "lv_LV": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -82910,22 +82910,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "mk_MK": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -83161,22 +83161,22 @@
             "local_currency_code": "MKD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ml_IN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -88457,22 +88457,22 @@
             "local_currency_code": "NOK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "no_NO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -89465,22 +89465,22 @@
             "local_currency_code": "PLN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ps_AF": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -90154,22 +90154,22 @@
             "local_currency_code": "AOA",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_BR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -90796,22 +90796,22 @@
             "local_currency_code": "CHF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_CV": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -91117,22 +91117,22 @@
             "local_currency_code": "CVE",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_GQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -91438,22 +91438,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_GW": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -91759,22 +91759,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_LU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -92080,22 +92080,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_MO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -92401,22 +92401,22 @@
             "local_currency_code": "MOP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_MZ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -92722,22 +92722,22 @@
             "local_currency_code": "MZN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_PT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -93043,22 +93043,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_ST": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -93364,22 +93364,22 @@
             "local_currency_code": "STN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_TL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -93685,22 +93685,22 @@
             "local_currency_code": "USD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ro_MD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -93958,22 +93958,22 @@
             "local_currency_code": "MDL",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ro_RO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -94231,22 +94231,22 @@
             "local_currency_code": "RON",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_BY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -94532,22 +94532,22 @@
             "local_currency_code": "BYN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_KG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -94833,22 +94833,22 @@
             "local_currency_code": "KGS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_KZ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -95134,22 +95134,22 @@
             "local_currency_code": "KZT",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_MD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -95435,22 +95435,22 @@
             "local_currency_code": "MDL",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_RU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -95736,22 +95736,22 @@
             "local_currency_code": "RUB",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_UA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -96037,22 +96037,22 @@
             "local_currency_code": "UAH",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sd_PK": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -96222,22 +96222,22 @@
             "local_currency_code": "PKR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "si_LK": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -96733,22 +96733,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sl_SI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -97032,22 +97032,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "so_DJ": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -97998,22 +97998,22 @@
             "local_currency_code": "ALL",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sq_MK": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "AFN",
                 "ALL": "Lek\u00eb",
                 "AMD": "AMD",
@@ -98184,22 +98184,22 @@
             "local_currency_code": "MKD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sq_XK": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "AFN",
                 "ALL": "Lek\u00eb",
                 "AMD": "AMD",
@@ -98370,22 +98370,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sr_BA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -98675,22 +98675,22 @@
             "local_currency_code": "BAM",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sr_ME": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -98980,22 +98980,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sr_RS": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -99285,22 +99285,22 @@
             "local_currency_code": "RSD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sr_XK": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -99590,22 +99590,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 0,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sv_AX": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -99915,22 +99915,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sv_FI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -100240,22 +100240,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sv_SE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -100565,22 +100565,22 @@
             "local_currency_code": "SEK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sw_CD": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -102773,22 +102773,22 @@
             "local_currency_code": "TMT",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "tr_CY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -103722,22 +103722,22 @@
             "local_currency_code": "UAH",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ur_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -104609,22 +104609,22 @@
             "local_currency_code": "VND",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "yo_BJ": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -108309,22 +108309,22 @@
             "local_currency_code": "AED",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u200e-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u200e+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_BH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -108590,22 +108590,22 @@
             "local_currency_code": "BHD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_DJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -108871,22 +108871,22 @@
             "local_currency_code": "DJF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_DZ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -109152,22 +109152,22 @@
             "local_currency_code": "DZD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u200e-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u200e+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_EG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -109433,22 +109433,22 @@
             "local_currency_code": "EGP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_EH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -109714,22 +109714,22 @@
             "local_currency_code": "MAD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u200e-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u200e+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_ER": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -109995,22 +109995,22 @@
             "local_currency_code": "ERN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_IL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -110276,22 +110276,22 @@
             "local_currency_code": "ILS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_IQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -110557,22 +110557,22 @@
             "local_currency_code": "IQD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_JO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -110838,22 +110838,22 @@
             "local_currency_code": "JOD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_KM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -111119,22 +111119,22 @@
             "local_currency_code": "KMF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_KW": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -111400,22 +111400,22 @@
             "local_currency_code": "KWD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_LB": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -111681,22 +111681,22 @@
             "local_currency_code": "LBP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_LY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -111962,22 +111962,22 @@
             "local_currency_code": "LYD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u200e-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u200e+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_MA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -112243,22 +112243,22 @@
             "local_currency_code": "MAD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u200e-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u200e+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_MR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -112524,22 +112524,22 @@
             "local_currency_code": "MRU",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_OM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -112805,22 +112805,22 @@
             "local_currency_code": "OMR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_PS": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -113086,22 +113086,22 @@
             "local_currency_code": "ILS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_QA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -113367,22 +113367,22 @@
             "local_currency_code": "QAR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -113648,22 +113648,22 @@
             "local_currency_code": "SAR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -113929,22 +113929,22 @@
             "local_currency_code": "SDG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -114210,22 +114210,22 @@
             "local_currency_code": "SOS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SS": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -114491,22 +114491,22 @@
             "local_currency_code": "SSP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_SY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -114772,22 +114772,22 @@
             "local_currency_code": "SYP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_TD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -115053,22 +115053,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_TN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -115334,22 +115334,22 @@
             "local_currency_code": "TND",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u200e-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u200e+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ar_YE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "\u062f.\u0625.\u200f",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -115615,22 +115615,22 @@
             "local_currency_code": "YER",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "as_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -116094,22 +116094,22 @@
             "local_currency_code": "AZN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "be_BY": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -116280,22 +116280,22 @@
             "local_currency_code": "BYN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "bg_BG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "Af",
@@ -116571,22 +116571,22 @@
             "local_currency_code": "BGN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "bn_BD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -117488,22 +117488,22 @@
             "local_currency_code": "BAM",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ca_AD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -117809,22 +117809,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ca_ES": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -118130,22 +118130,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ca_FR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -118451,22 +118451,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ca_IT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -118772,22 +118772,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "chr_US": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -119281,22 +119281,22 @@
             "local_currency_code": "CZK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "cy_GB": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -119858,22 +119858,22 @@
             "local_currency_code": "DKK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "da_GL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -120152,22 +120152,22 @@
             "local_currency_code": "DKK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "de_AT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -120800,22 +120800,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "de_CH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -121448,22 +121448,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "de_IT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -121772,22 +121772,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "de_LI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -122420,22 +122420,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "dsb_DE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -122632,22 +122632,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "el_CY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -122924,22 +122924,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "el_GR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -123216,22 +123216,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_AE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -125824,22 +125824,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_BI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -130062,22 +130062,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_DG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -130714,22 +130714,22 @@
             "local_currency_code": "DKK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_DM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -131692,22 +131692,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_FJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -145058,15 +145058,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -149624,22 +149624,22 @@
             "local_currency_code": "SEK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_SG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -150602,22 +150602,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "en_SL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -160468,22 +160468,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "es_EC": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -161072,22 +161072,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "es_GQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -162280,22 +162280,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "es_MX": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -163790,22 +163790,22 @@
             "local_currency_code": "PHP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "es_PR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -164392,15 +164392,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "PYG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -165898,22 +165898,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "eu_ES": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -166224,22 +166224,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fa_AF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -167061,22 +167061,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fil_PH": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -167557,22 +167557,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_BF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -167860,22 +167860,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_BI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -168163,22 +168163,22 @@
             "local_currency_code": "BIF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_BJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -168466,22 +168466,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_BL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -168769,22 +168769,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -169072,22 +169072,22 @@
             "local_currency_code": "CAD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -169375,22 +169375,22 @@
             "local_currency_code": "CDF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -169678,22 +169678,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -169981,22 +169981,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -170284,22 +170284,22 @@
             "local_currency_code": "CHF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -170587,22 +170587,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_CM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -170890,22 +170890,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_DJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -171193,22 +171193,22 @@
             "local_currency_code": "DJF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_DZ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -171496,22 +171496,22 @@
             "local_currency_code": "DZD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_FR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -171799,22 +171799,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -172102,22 +172102,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -172405,22 +172405,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -172708,22 +172708,22 @@
             "local_currency_code": "GNF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GP": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -173011,22 +173011,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_GQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -173314,22 +173314,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_HT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -173617,22 +173617,22 @@
             "local_currency_code": "HTG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_KM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -173920,22 +173920,22 @@
             "local_currency_code": "KMF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_LU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -174223,22 +174223,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -174526,22 +174526,22 @@
             "local_currency_code": "MAD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MC": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -174829,22 +174829,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -175132,22 +175132,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -175435,22 +175435,22 @@
             "local_currency_code": "MGA",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_ML": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -175738,22 +175738,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -176041,22 +176041,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -176344,22 +176344,22 @@
             "local_currency_code": "MRU",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_MU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -176647,22 +176647,22 @@
             "local_currency_code": "MUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_NC": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -176950,22 +176950,22 @@
             "local_currency_code": "XPF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_NE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -177253,22 +177253,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_PF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -177556,22 +177556,22 @@
             "local_currency_code": "XPF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_PM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -177859,22 +177859,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_RE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -178162,22 +178162,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_RW": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -178465,22 +178465,22 @@
             "local_currency_code": "RWF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_SC": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -178768,22 +178768,22 @@
             "local_currency_code": "SCR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_SN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -179071,22 +179071,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_SY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -179374,22 +179374,22 @@
             "local_currency_code": "SYP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_TD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -179677,22 +179677,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_TG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -179980,22 +179980,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_TN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -180283,22 +180283,22 @@
             "local_currency_code": "TND",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_VU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -180586,22 +180586,22 @@
             "local_currency_code": "VUV",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_WF": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -180889,22 +180889,22 @@
             "local_currency_code": "XPF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "fr_YT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -181192,22 +181192,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ga_GB": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -182344,22 +182344,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "gu_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -183354,22 +183354,22 @@
             "local_currency_code": "ILS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u200e-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u200e+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hi_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -183890,22 +183890,22 @@
             "local_currency_code": "BAM",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hr_HR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -184212,22 +184212,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hsb_DE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -184424,22 +184424,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hu_HU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -184734,22 +184734,22 @@
             "local_currency_code": "HUF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "hy_AM": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -184921,22 +184921,22 @@
             "local_currency_code": "AMD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "id_ID": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -185673,22 +185673,22 @@
             "local_currency_code": "ISK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "it_CH": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -186265,22 +186265,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "it_SM": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -186561,22 +186561,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "it_VA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -186857,22 +186857,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ja_JP": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -187634,22 +187634,22 @@
             "local_currency_code": "GEL",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "kk_KZ": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -187820,22 +187820,22 @@
             "local_currency_code": "KZT",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "km_KH": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -189505,22 +189505,22 @@
             "local_currency_code": "KGS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "lo_LA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -190146,22 +190146,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "lv_LV": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -190377,22 +190377,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "mk_MK": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -190628,22 +190628,22 @@
             "local_currency_code": "MKD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ml_IN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -192290,22 +192290,22 @@
             "local_currency_code": "MMK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "nb_NO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -192614,22 +192614,22 @@
             "local_currency_code": "NOK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "nb_SJ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -192938,22 +192938,22 @@
             "local_currency_code": "NOK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ne_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -193642,15 +193642,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "AWG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -193968,15 +193968,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -194294,15 +194294,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "USD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -194620,15 +194620,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "ANG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -194946,15 +194946,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -195272,15 +195272,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "SRD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -195598,15 +195598,15 @@
             "decimal_separator": ",",
             "grouping_separator": ".",
             "local_currency_code": "ANG",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
-            "negative_sign_position": -1,
+            "negative_sign_position": 1,
             "negative_symbol_before": true,
             "negative_symbol_space": 0,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
@@ -195924,22 +195924,22 @@
             "local_currency_code": "NOK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "no_NO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -196248,22 +196248,22 @@
             "local_currency_code": "NOK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "or_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -196934,22 +196934,22 @@
             "local_currency_code": "PLN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ps_AF": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -197623,22 +197623,22 @@
             "local_currency_code": "AOA",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_BR": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -198265,22 +198265,22 @@
             "local_currency_code": "CHF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_CV": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -198586,22 +198586,22 @@
             "local_currency_code": "CVE",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_GQ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -198907,22 +198907,22 @@
             "local_currency_code": "XAF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_GW": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -199228,22 +199228,22 @@
             "local_currency_code": "XOF",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_LU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -199549,22 +199549,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_MO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -199870,22 +199870,22 @@
             "local_currency_code": "MOP",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_MZ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -200191,22 +200191,22 @@
             "local_currency_code": "MZN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_PT": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -200512,22 +200512,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_ST": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -200833,22 +200833,22 @@
             "local_currency_code": "STN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "pt_TL": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -201154,22 +201154,22 @@
             "local_currency_code": "USD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ro_MD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -201427,22 +201427,22 @@
             "local_currency_code": "MDL",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ro_RO": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
@@ -201700,22 +201700,22 @@
             "local_currency_code": "RON",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_BY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -202001,22 +202001,22 @@
             "local_currency_code": "BYN",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_KG": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -202302,22 +202302,22 @@
             "local_currency_code": "KGS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_KZ": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -202603,22 +202603,22 @@
             "local_currency_code": "KZT",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_MD": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -202904,22 +202904,22 @@
             "local_currency_code": "MDL",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_RU": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -203205,22 +203205,22 @@
             "local_currency_code": "RUB",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ru_UA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -203506,22 +203506,22 @@
             "local_currency_code": "UAH",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sd_PK": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -203691,22 +203691,22 @@
             "local_currency_code": "PKR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u061c-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "\u061c+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "si_LK": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -204202,22 +204202,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sl_SI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -204501,22 +204501,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "so_DJ": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -205467,22 +205467,22 @@
             "local_currency_code": "ALL",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sq_MK": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "AFN",
                 "ALL": "Lek\u00eb",
                 "AMD": "AMD",
@@ -205653,22 +205653,22 @@
             "local_currency_code": "MKD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sq_XK": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "AFN",
                 "ALL": "Lek\u00eb",
                 "AMD": "AMD",
@@ -205839,22 +205839,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sr_BA": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -206144,22 +206144,22 @@
             "local_currency_code": "BAM",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sr_ME": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -206449,22 +206449,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sr_RS": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -206754,22 +206754,22 @@
             "local_currency_code": "RSD",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sr_XK": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -207059,22 +207059,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sv_AX": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -207384,22 +207384,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sv_FI": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -207709,22 +207709,22 @@
             "local_currency_code": "EUR",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sv_SE": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -208034,22 +208034,22 @@
             "local_currency_code": "SEK",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "\u2212",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "sw_CD": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -210248,22 +210248,22 @@
             "local_currency_code": "TMT",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "tr_CY": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -211197,22 +211197,22 @@
             "local_currency_code": "UAH",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "ur_IN": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
@@ -211769,22 +211769,22 @@
             "local_currency_code": "UZS",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "vi_VN": {
             "currency_symbols": {
                 "ADP": "ADP",
                 "AED": "AED",
                 "AFA": "AFA",
                 "AFN": "\u060b",
@@ -212086,22 +212086,22 @@
             "local_currency_code": "VND",
             "negative_grouping": [
                 3
             ],
             "negative_sign": "-",
             "negative_sign_position": 1,
             "negative_symbol_before": false,
-            "negative_symbol_space": 0,
+            "negative_symbol_space": 1,
             "positive_grouping": [
                 3
             ],
             "positive_sign": "+",
             "positive_sign_position": -1,
             "positive_symbol_before": false,
-            "positive_symbol_space": 0
+            "positive_symbol_space": 1
         },
         "yo_BJ": {
             "currency_symbols": {
                 "AED": "AED",
                 "AFN": "\u060b",
                 "ALL": "ALL",
                 "AMD": "\u058f",
```

### Comparing `linearmoney-0.1.2/src/linearmoney/mixins.py` & `linearmoney-0.1.3/src/linearmoney/mixins.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/src/linearmoney/resources.py` & `linearmoney-0.1.3/src/linearmoney/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 import importlib.resources
 from os import PathLike
 from typing import Literal, Any, TypeAlias
 
 import linearmoney as lm
 
 ResourceName: TypeAlias = (
-    Literal["locales"] | Literal["currencies"] | Literal["supported_iso_codes"]
+    Literal["locales"]
+    | Literal["currencies"]
+    | Literal["supported_iso_codes"]
+    | Literal["cldr_version"]
 )
 
 
 def _load_json_resource(res_path: str | PathLike) -> dict:
     with open(res_path, "r") as json_file:
         return json.load(json_file)
```

### Comparing `linearmoney-0.1.2/src/linearmoney/scalar.py` & `linearmoney-0.1.3/src/linearmoney/scalar.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/src/linearmoney/supported_iso_codes.json` & `linearmoney-0.1.3/src/linearmoney/supported_iso_codes.json`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/src/linearmoney/vector.py` & `linearmoney-0.1.3/src/linearmoney/vector.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/LICENSE` & `linearmoney-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.2/README.md` & `linearmoney-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -56,20 +56,17 @@
 ```
 
 From source:
 
 ```bash
 git clone https://github.com/GrammAcc/linearmoney
 cd linearmoney
-poetry build
+python -m build .
 ```
 
-See the [poetry installation](https://python-poetry.org/docs/#installation) docs if
-you don't have poetry installed yet.
-
 Then to install (virtual environment recommended):
 
 ```bash
 pip install path/to/cloned/repo
 ```
 
 ## Basic Usage
@@ -108,22 +105,26 @@
 
 See the [Recipes](https://grammacc.github.io/linearmoney/recipes.html)
 section of the user guide for
 some examples of how to mitigate the verbosity of the library and other helpful patterns.
 
 ## Contributing
 
-This project is in early development and is not yet accepting PRs. Once a contributing
-workflow and CI pipeline are setup, we will start accepting public PRs.
+Contributions are greatly appreciated!
+
+See the [contributing guidelines](/CONTRIBUTING.md) to get started.
 
 ## Roadmap
 
 Version 1.0.0:
 - [ ] Redesign locale/formatting data structure
+  - [#15](https://github.com/GrammAcc/linearmoney/issues/15)
 - [ ] Redesign caching system
 - [ ] Higher-order serialization interface
   - [ ] Serialization/deserialization of forex vectors
 - [ ] Recipes to add
   - [ ] Use-cases without vectors
-- [ ] Refactor CLDR data processing script
+- [x] Refactor CLDR data processing script
   - [#11](https://github.com/GrammAcc/linearmoney/issues/11)
-- [ ] Add contributing guidelines and setup CI
+- [x] Add contributing guidelines and setup CI
+  - [x] Contributing guidelines
+  - [x] CI workflow
```

### Comparing `linearmoney-0.1.2/pyproject.toml` & `linearmoney-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -42,16 +42,14 @@
 include = ["src"]
 
 # This is needed for hatchling to find the version in the package __init__.py file.
 # See https://github.com/pypa/hatch/issues/981#issuecomment-1743631364
 [tool.hatch.build.targets.wheel]
 packages = ["src/linearmoney"]
 
-[tool.hatch.publish.index]
-disable = true
 
 [tool.hatch.envs.default]
 python = "3.12"
 
 [tool.hatch.envs.default.scripts]
 ci = [
     "hatch run test:suite",
@@ -133,14 +131,22 @@
     "pdoc 'linearmoney' --docformat='google' --output-directory='documentation/md/api_reference' --template-directory='documentation/pdoc_templates'",
     "mkdocs build -f documentation/mkdocs.yml",
 ]
 serve = "python documentation/serve.py"
 test-prose = "pytest --doctest-glob='*.md' README.md documentation"
 test-in-source = "python documentation/run_doctests.py"
 
+[tool.hatch.envs.cldr]
+description = "CLDR data tooling"
+detached = true
+
+[tool.hatch.envs.cldr.scripts]
+build = "python process_cldr_data.py"
+test = "python tests/cldr/check_data.py"
+
 
 [tool.pytest.ini_options]
 log_file="testsuite.log"
 log_file_level="DEBUG"
 addopts = "--import-mode=importlib --show-capture=no --ignore=cldr-json"
```

### Comparing `linearmoney-0.1.2/PKG-INFO` & `linearmoney-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: linearmoney
-Version: 0.1.2
+Version: 0.1.3
 Summary: Full multi-currency support for python.
 Project-URL: homepage, https://github.com/GrammAcc/linearmoney
 Project-URL: bug_tracker, https://github.com/GrammAcc/linearmoney/issues
 Project-URL: documentation, https://grammacc.github.io/linearmoney
 Project-URL: repository, https://github.com/GrammAcc/linearmoney
 Author-email: GrammAcc <grammaticallyacceptable@grammacc.dev>
 Maintainer-email: GrammAcc <grammaticallyacceptable@grammacc.dev>
@@ -77,20 +77,17 @@
 ```
 
 From source:
 
 ```bash
 git clone https://github.com/GrammAcc/linearmoney
 cd linearmoney
-poetry build
+python -m build .
 ```
 
-See the [poetry installation](https://python-poetry.org/docs/#installation) docs if
-you don't have poetry installed yet.
-
 Then to install (virtual environment recommended):
 
 ```bash
 pip install path/to/cloned/repo
 ```
 
 ## Basic Usage
@@ -129,22 +126,26 @@
 
 See the [Recipes](https://grammacc.github.io/linearmoney/recipes.html)
 section of the user guide for
 some examples of how to mitigate the verbosity of the library and other helpful patterns.
 
 ## Contributing
 
-This project is in early development and is not yet accepting PRs. Once a contributing
-workflow and CI pipeline are setup, we will start accepting public PRs.
+Contributions are greatly appreciated!
+
+See the [contributing guidelines](/CONTRIBUTING.md) to get started.
 
 ## Roadmap
 
 Version 1.0.0:
 - [ ] Redesign locale/formatting data structure
+  - [#15](https://github.com/GrammAcc/linearmoney/issues/15)
 - [ ] Redesign caching system
 - [ ] Higher-order serialization interface
   - [ ] Serialization/deserialization of forex vectors
 - [ ] Recipes to add
   - [ ] Use-cases without vectors
-- [ ] Refactor CLDR data processing script
+- [x] Refactor CLDR data processing script
   - [#11](https://github.com/GrammAcc/linearmoney/issues/11)
-- [ ] Add contributing guidelines and setup CI
+- [x] Add contributing guidelines and setup CI
+  - [x] Contributing guidelines
+  - [x] CI workflow
```

