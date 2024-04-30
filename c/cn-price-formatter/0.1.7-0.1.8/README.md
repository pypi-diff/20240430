# Comparing `tmp/cn_price_formatter-0.1.7.tar.gz` & `tmp/cn_price_formatter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cn_price_formatter-0.1.7.tar", last modified: Mon Feb  5 14:12:15 2024, max compression
+gzip compressed data, was "cn_price_formatter-0.1.8.tar", last modified: Tue Apr 30 15:15:08 2024, max compression
```

## Comparing `cn_price_formatter-0.1.7.tar` & `cn_price_formatter-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 usmantahir  (1000) usmantahir  (1000)        0 2024-02-05 14:12:15.064803 cn_price_formatter-0.1.7/
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)      221 2024-02-05 14:12:15.064803 cn_price_formatter-0.1.7/PKG-INFO
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)     2606 2024-01-31 17:44:10.000000 cn_price_formatter-0.1.7/README.md
-drwxrwxr-x   0 usmantahir  (1000) usmantahir  (1000)        0 2024-02-05 14:12:15.064803 cn_price_formatter-0.1.7/cn_price_formatter/
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)        0 2024-01-31 16:43:10.000000 cn_price_formatter-0.1.7/cn_price_formatter/__init__.py
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)    18630 2024-02-05 14:11:14.000000 cn_price_formatter-0.1.7/cn_price_formatter/price_formatter.py
-drwxrwxr-x   0 usmantahir  (1000) usmantahir  (1000)        0 2024-02-05 14:12:15.064803 cn_price_formatter-0.1.7/cn_price_formatter.egg-info/
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)      221 2024-02-05 14:12:15.000000 cn_price_formatter-0.1.7/cn_price_formatter.egg-info/PKG-INFO
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)      443 2024-02-05 14:12:15.000000 cn_price_formatter-0.1.7/cn_price_formatter.egg-info/SOURCES.txt
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)        1 2024-02-05 14:12:15.000000 cn_price_formatter-0.1.7/cn_price_formatter.egg-info/dependency_links.txt
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)       25 2024-02-05 14:12:15.000000 cn_price_formatter-0.1.7/cn_price_formatter.egg-info/top_level.txt
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)       38 2024-02-05 14:12:15.064803 cn_price_formatter-0.1.7/setup.cfg
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)      399 2024-02-05 14:11:20.000000 cn_price_formatter-0.1.7/setup.py
-drwxrwxr-x   0 usmantahir  (1000) usmantahir  (1000)        0 2024-02-05 14:12:15.064803 cn_price_formatter-0.1.7/tests/
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)        0 2024-01-31 16:45:21.000000 cn_price_formatter-0.1.7/tests/__init__.py
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)     2768 2024-02-03 13:01:10.000000 cn_price_formatter-0.1.7/tests/didatravel_test_price_formatter.py
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)     2842 2024-02-03 13:01:10.000000 cn_price_formatter-0.1.7/tests/exp_test_price_formatter.py
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)     3740 2024-02-03 13:01:10.000000 cn_price_formatter-0.1.7/tests/hp_price_formatter.py
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)     2046 2024-02-03 13:01:10.000000 cn_price_formatter-0.1.7/tests/rakuten_price_formatter.py
--rw-rw-r--   0 usmantahir  (1000) usmantahir  (1000)     4979 2024-02-03 13:01:10.000000 cn_price_formatter-0.1.7/tests/ratehawk_price_formatter.py
+drwxrwxr-x   0 asadsaqlain  (1000) asadsaqlain  (1000)        0 2024-04-30 15:15:08.290398 cn_price_formatter-0.1.8/
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)      296 2024-04-30 15:15:08.290398 cn_price_formatter-0.1.8/PKG-INFO
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)     2606 2024-02-12 14:57:53.000000 cn_price_formatter-0.1.8/README.md
+drwxrwxr-x   0 asadsaqlain  (1000) asadsaqlain  (1000)        0 2024-04-30 15:15:08.290398 cn_price_formatter-0.1.8/cn_price_formatter/
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)        0 2024-02-12 14:57:53.000000 cn_price_formatter-0.1.8/cn_price_formatter/__init__.py
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)    18819 2024-04-29 15:05:48.000000 cn_price_formatter-0.1.8/cn_price_formatter/price_formatter.py
+drwxrwxr-x   0 asadsaqlain  (1000) asadsaqlain  (1000)        0 2024-04-30 15:15:08.290398 cn_price_formatter-0.1.8/cn_price_formatter.egg-info/
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)      296 2024-04-30 15:15:08.000000 cn_price_formatter-0.1.8/cn_price_formatter.egg-info/PKG-INFO
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)      443 2024-04-30 15:15:08.000000 cn_price_formatter-0.1.8/cn_price_formatter.egg-info/SOURCES.txt
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)        1 2024-04-30 15:15:08.000000 cn_price_formatter-0.1.8/cn_price_formatter.egg-info/dependency_links.txt
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)       25 2024-04-30 15:15:08.000000 cn_price_formatter-0.1.8/cn_price_formatter.egg-info/top_level.txt
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)       38 2024-04-30 15:15:08.290398 cn_price_formatter-0.1.8/setup.cfg
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)      399 2024-04-30 15:12:59.000000 cn_price_formatter-0.1.8/setup.py
+drwxrwxr-x   0 asadsaqlain  (1000) asadsaqlain  (1000)        0 2024-04-30 15:15:08.290398 cn_price_formatter-0.1.8/tests/
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)        0 2024-02-12 14:57:53.000000 cn_price_formatter-0.1.8/tests/__init__.py
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)     2768 2024-02-12 14:57:53.000000 cn_price_formatter-0.1.8/tests/didatravel_test_price_formatter.py
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)     2842 2024-02-12 14:57:53.000000 cn_price_formatter-0.1.8/tests/exp_test_price_formatter.py
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)     3740 2024-02-12 14:57:53.000000 cn_price_formatter-0.1.8/tests/hp_price_formatter.py
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)     2046 2024-02-12 14:57:53.000000 cn_price_formatter-0.1.8/tests/rakuten_price_formatter.py
+-rw-rw-r--   0 asadsaqlain  (1000) asadsaqlain  (1000)     4979 2024-04-29 15:03:38.000000 cn_price_formatter-0.1.8/tests/ratehawk_price_formatter.py
```

### Comparing `cn_price_formatter-0.1.7/README.md` & `cn_price_formatter-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cn_price_formatter-0.1.7/cn_price_formatter/price_formatter.py` & `cn_price_formatter-0.1.8/cn_price_formatter/price_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,14 +285,15 @@
                     # Check pay at property taxes
                     taxes_data = payments.get('tax_data', [])
                     if taxes_data:
                         for tax_data in taxes_data.get('taxes', []):
                             try:
                                 if tax_data.get('included_by_supplier', True):
                                     partner_tax += float(tax_data.get('amount', 0))
+                                    room_rate = room_rate - float(tax_data.get('amount', 0))
                                 else:
                                     # due_at_property += float(tax_data.get('amount', 0))
                                     due_at_property.append({
                                         'name' : tax_data['name'],
                                         'amount': float(tax_data.get('amount', 0)),
                                         'currency': tax_data.get('currency_code', '')
                                     }) 
@@ -329,16 +330,17 @@
             if key not in data:
                 raise ValueError(f"Missing key '{key}' in the JSON data.")
 
         
                    
         
     
-
-        base_rate = data["TotalPrice"]
+        no_of_rooms = data['no_of_rooms']
+        base_rate = data["TotalPrice"] * no_of_rooms
+        # base_rate = data["TotalPrice"]
         number_of_nights = len(data['PriceList'])
         totalPrice = base_rate
         self.base_rate = base_rate
         self.partner_total = base_rate
         self.cn_fees = self.get_total_cn_fee()
         self.total = self.partner_total + self.cn_fees
         self.total_tax = self.cn_fees
```

### Comparing `cn_price_formatter-0.1.7/tests/didatravel_test_price_formatter.py` & `cn_price_formatter-0.1.8/tests/didatravel_test_price_formatter.py`

 * *Files identical despite different names*

### Comparing `cn_price_formatter-0.1.7/tests/exp_test_price_formatter.py` & `cn_price_formatter-0.1.8/tests/exp_test_price_formatter.py`

 * *Files identical despite different names*

### Comparing `cn_price_formatter-0.1.7/tests/hp_price_formatter.py` & `cn_price_formatter-0.1.8/tests/hp_price_formatter.py`

 * *Files identical despite different names*

### Comparing `cn_price_formatter-0.1.7/tests/rakuten_price_formatter.py` & `cn_price_formatter-0.1.8/tests/rakuten_price_formatter.py`

 * *Files identical despite different names*

### Comparing `cn_price_formatter-0.1.7/tests/ratehawk_price_formatter.py` & `cn_price_formatter-0.1.8/tests/ratehawk_price_formatter.py`

 * *Files identical despite different names*

