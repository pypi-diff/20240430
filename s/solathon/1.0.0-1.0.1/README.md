# Comparing `tmp/solathon-1.0.0.tar.gz` & `tmp/solathon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solathon-1.0.0.tar", max compression
+gzip compressed data, was "solathon-1.0.1.tar", max compression
```

## Comparing `solathon-1.0.0.tar` & `solathon-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1050 2024-04-16 13:48:37.758737 solathon-1.0.0/LICENSE
--rw-r--r--   0        0        0     1428 2024-04-16 14:15:10.734716 solathon-1.0.0/README.md
--rw-r--r--   0        0        0     1135 2024-04-16 14:15:34.950535 solathon-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      213 2024-04-16 14:31:44.119135 solathon-1.0.0/solathon/__init__.py
--rw-r--r--   0        0        0    18172 2024-04-16 14:31:07.234418 solathon-1.0.0/solathon/async_client.py
--rw-r--r--   0        0        0    26417 2024-04-16 14:11:21.518429 solathon-1.0.0/solathon/client.py
--rw-r--r--   0        0        0       20 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/__init__.py
--rw-r--r--   0        0        0     3004 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/http.py
--rw-r--r--   0        0        0     5146 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/instructions.py
--rw-r--r--   0        0        0     3040 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/layouts.py
--rw-r--r--   0        0        0     6280 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/message.py
--rw-r--r--   0        0        0     4602 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/account_info.py
--rw-r--r--   0        0        0     6669 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/block.py
--rw-r--r--   0        0        0      778 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/cluster_node.py
--rw-r--r--   0        0        0     1426 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/epoch.py
--rw-r--r--   0        0        0     1750 2024-04-16 13:48:37.765736 solathon-1.0.0/solathon/core/types/inflation.py
--rw-r--r--   0        0        0     2395 2024-04-16 14:28:08.682787 solathon-1.0.0/solathon/keypair.py
--rw-r--r--   0        0        0     1222 2024-04-16 14:21:14.602960 solathon-1.0.0/solathon/publickey.py
--rw-r--r--   0        0        0      286 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/create_qr.py
--rw-r--r--   0        0        0     5128 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/create_transfer.py
--rw-r--r--   0        0        0     3129 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/encode_url.py
--rw-r--r--   0        0        0     3044 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/fetch_transaction.py
--rw-r--r--   0        0        0     1148 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/find_reference.py
--rw-r--r--   0        0        0     2592 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/parse_url.py
--rw-r--r--   0        0        0     3053 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/qr-logo.png
--rw-r--r--   0        0        0      914 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/types.py
--rw-r--r--   0        0        0     3507 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/solana_pay/validate_transfer.py
--rw-r--r--   0        0        0    11293 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/transaction.py
--rw-r--r--   0        0        0     2150 2024-04-16 13:48:37.766737 solathon-1.0.0/solathon/utils.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 solathon-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2024-04-16 13:48:37.758737 solathon-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1428 2024-04-16 14:15:10.734716 solathon-1.0.1/README.md
+-rw-r--r--   0        0        0     1135 2024-04-30 07:31:50.886527 solathon-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      213 2024-04-30 07:31:33.987671 solathon-1.0.1/solathon/__init__.py
+-rw-r--r--   0        0        0    18172 2024-04-16 14:31:07.234418 solathon-1.0.1/solathon/async_client.py
+-rw-r--r--   0        0        0    26868 2024-04-30 07:30:12.369363 solathon-1.0.1/solathon/client.py
+-rw-r--r--   0        0        0       20 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/__init__.py
+-rw-r--r--   0        0        0     3004 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/http.py
+-rw-r--r--   0        0        0     5146 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/instructions.py
+-rw-r--r--   0        0        0     3040 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/layouts.py
+-rw-r--r--   0        0        0     6280 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/message.py
+-rw-r--r--   0        0        0     4602 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/account_info.py
+-rw-r--r--   0        0        0     6787 2024-04-30 07:30:30.435210 solathon-1.0.1/solathon/core/types/block.py
+-rw-r--r--   0        0        0      778 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/cluster_node.py
+-rw-r--r--   0        0        0     1426 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/epoch.py
+-rw-r--r--   0        0        0     1750 2024-04-16 13:48:37.765736 solathon-1.0.1/solathon/core/types/inflation.py
+-rw-r--r--   0        0        0     2395 2024-04-16 14:28:08.682787 solathon-1.0.1/solathon/keypair.py
+-rw-r--r--   0        0        0     1222 2024-04-16 14:21:14.602960 solathon-1.0.1/solathon/publickey.py
+-rw-r--r--   0        0        0      286 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/create_qr.py
+-rw-r--r--   0        0        0     5128 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/create_transfer.py
+-rw-r--r--   0        0        0     3129 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/encode_url.py
+-rw-r--r--   0        0        0     3044 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/fetch_transaction.py
+-rw-r--r--   0        0        0     1148 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/find_reference.py
+-rw-r--r--   0        0        0     2592 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/parse_url.py
+-rw-r--r--   0        0        0     3053 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/qr-logo.png
+-rw-r--r--   0        0        0      914 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/types.py
+-rw-r--r--   0        0        0     3507 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/solana_pay/validate_transfer.py
+-rw-r--r--   0        0        0    11293 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/transaction.py
+-rw-r--r--   0        0        0     2150 2024-04-16 13:48:37.766737 solathon-1.0.1/solathon/utils.py
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 solathon-1.0.1/PKG-INFO
```

### Comparing `solathon-1.0.0/LICENSE` & `solathon-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/README.md` & `solathon-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/pyproject.toml` & `solathon-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solathon"
-version = "1.0.0"
+version = "1.0.1"
 description = "High performance, easy to use and feature-rich Solana SDK for Python."
 license = "MIT"
 authors = ["GitBolt"]
 readme = "README.md"
 repository = "https://github.com/GitBolt/solathon"
 keywords = ["solana", "web3", "sdk", "blockchain", "crypto"]
 classifiers = [
```

### Comparing `solathon-1.0.0/solathon/async_client.py` & `solathon-1.0.1/solathon/async_client.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/client.py` & `solathon-1.0.1/solathon/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -688,28 +688,39 @@
             ],
         )
         if self.clean_response:
             return response["value"]
         return response
 
     def get_transaction(
-        self, signature: Text, commitment: Optional[Commitment] = None
+        self,
+        signature: Text,
+        max_supported_transaction_version: Optional[int] = 0,
+        commitment: Optional[Commitment] = None,
     ) -> RPCResponse[TransactionElementType] | TransactionElement:
         """
         Sends a request to the Solana RPC endpoint to retrieve a transaction by its signature.
 
         Args:
             signature (str): The signature of the transaction to retrieve.
             commitment (Commitment, optional): The level of commitment desired when querying state.
+            max_supported_transaction_version (int, optional): Set the max transaction version to return in responses
 
         Returns:
             RPCResponse: The response from the Solana RPC endpoint.
         """
         response = self.build_and_send_request(
-            "getTransaction", [signature, commitment]
+            "getTransaction",
+            [
+                signature,
+                {
+                    "commitment": commitment,
+                    "maxSupportedTransactionVersion": max_supported_transaction_version,
+                },
+            ],
         )
         if self.clean_response:
             if response == None:
                 raise ValueError("Transaction not found")
             return TransactionElement(response)
         return response
 
@@ -734,14 +745,15 @@
                     f"Failed to fetch data from RPC endpoint. Error {res['error']['code']}: {res['error']['message']}"
                 )
 
             if (
                 isinstance(res["result"], dict)
                 or isinstance(res["result"], list)
                 or isinstance(res["result"], str)
+                or isinstance(res["result"], int)
                 or res["result"] == None
             ):
                 return res["result"]
             else:
                 raise RPCRequestError(
                     f"Invalid response from RPC endpoint. Expected types dict | list | str, got {type(res['result']).__name__}"
                 )
```

### Comparing `solathon-1.0.0/solathon/core/http.py` & `solathon-1.0.1/solathon/core/http.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/core/instructions.py` & `solathon-1.0.1/solathon/core/instructions.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/core/layouts.py` & `solathon-1.0.1/solathon/core/layouts.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/core/message.py` & `solathon-1.0.1/solathon/core/message.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/core/types/__init__.py` & `solathon-1.0.1/solathon/core/types/__init__.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/core/types/account_info.py` & `solathon-1.0.1/solathon/core/types/account_info.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/core/types/block.py` & `solathon-1.0.1/solathon/core/types/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,18 @@
     '''
     Convert Transaction JSON to Class
     '''
     def __init__(self, response: TransactionElementType) -> None:
         self.meta = Meta(response['meta'])
         self.transaction = Transaction(response['transaction'])
 
+    def __repr__(self) -> str:
+        return f"TransactionElement(signatures={self.transaction.signatures!r})"
+
+    
 class BlockType(TypedDict):
     '''
     JSON Response type of Block Information received by RPC
     '''
     blockHeight: int
     blockTime: None
     blockhash: str
```

### Comparing `solathon-1.0.0/solathon/core/types/cluster_node.py` & `solathon-1.0.1/solathon/core/types/cluster_node.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/core/types/epoch.py` & `solathon-1.0.1/solathon/core/types/epoch.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/core/types/inflation.py` & `solathon-1.0.1/solathon/core/types/inflation.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/keypair.py` & `solathon-1.0.1/solathon/keypair.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/publickey.py` & `solathon-1.0.1/solathon/publickey.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/create_qr.py` & `solathon-1.0.1/solathon/solana_pay/create_qr.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/create_transfer.py` & `solathon-1.0.1/solathon/solana_pay/create_transfer.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/encode_url.py` & `solathon-1.0.1/solathon/solana_pay/encode_url.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/fetch_transaction.py` & `solathon-1.0.1/solathon/solana_pay/fetch_transaction.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/find_reference.py` & `solathon-1.0.1/solathon/solana_pay/find_reference.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/parse_url.py` & `solathon-1.0.1/solathon/solana_pay/parse_url.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/qr-logo.png` & `solathon-1.0.1/solathon/solana_pay/qr-logo.png`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/types.py` & `solathon-1.0.1/solathon/solana_pay/types.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/solana_pay/validate_transfer.py` & `solathon-1.0.1/solathon/solana_pay/validate_transfer.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/transaction.py` & `solathon-1.0.1/solathon/transaction.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/solathon/utils.py` & `solathon-1.0.1/solathon/utils.py`

 * *Files identical despite different names*

### Comparing `solathon-1.0.0/PKG-INFO` & `solathon-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solathon
-Version: 1.0.0
+Version: 1.0.1
 Summary: High performance, easy to use and feature-rich Solana SDK for Python.
 Home-page: https://github.com/GitBolt/solathon
 License: MIT
 Keywords: solana,web3,sdk,blockchain,crypto
 Author: GitBolt
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solathon Version: 1.0.0 Summary: High performance,
+Metadata-Version: 2.1 Name: solathon Version: 1.0.1 Summary: High performance,
 easy to use and feature-rich Solana SDK for Python. Home-page: https://
 github.com/GitBolt/solathon License: MIT Keywords:
 solana,web3,sdk,blockchain,crypto Author: GitBolt Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

