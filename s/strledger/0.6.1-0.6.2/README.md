# Comparing `tmp/strledger-0.6.1.tar.gz` & `tmp/strledger-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strledger-0.6.1.tar", max compression
+gzip compressed data, was "strledger-0.6.2.tar", max compression
```

## Comparing `strledger-0.6.1.tar` & `strledger-0.6.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 09:34:52.502126 strledger-0.6.1/LICENSE
--rw-r--r--   0        0        0     1188 2024-04-23 12:41:53.731085 strledger-0.6.1/README.md
--rw-r--r--   0        0        0     1375 2024-04-23 12:41:53.731954 strledger-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      120 2024-04-23 12:41:53.732265 strledger-0.6.1/strledger/__init__.py
--rw-r--r--   0        0        0     9195 2024-04-23 09:34:52.505783 strledger-0.6.1/strledger/cli.py
--rw-r--r--   0        0        0     7066 2024-04-23 09:34:52.505980 strledger-0.6.1/strledger/core.py
--rw-r--r--   0        0        0        0 2024-04-23 09:34:52.506030 strledger-0.6.1/strledger/py.typed
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 strledger-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 09:34:52.502126 strledger-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1188 2024-04-23 12:41:53.731085 strledger-0.6.2/README.md
+-rw-r--r--   0        0        0     1375 2024-04-30 09:08:33.374138 strledger-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-04-30 09:08:37.476327 strledger-0.6.2/strledger/__init__.py
+-rw-r--r--   0        0        0    10249 2024-04-30 09:08:11.685426 strledger-0.6.2/strledger/cli.py
+-rw-r--r--   0        0        0     7066 2024-04-23 09:34:52.505980 strledger-0.6.2/strledger/core.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:34:52.506030 strledger-0.6.2/strledger/py.typed
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 strledger-0.6.2/PKG-INFO
```

### Comparing `strledger-0.6.1/LICENSE` & `strledger-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strledger-0.6.1/README.md` & `strledger-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `strledger-0.6.1/pyproject.toml` & `strledger-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strledger"
-version = "0.6.1"
+version = "0.6.2"
 description = "Sign Stellar Transaction with Ledger on the command line."
 authors = ["overcat <4catcode@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/overcat/strledger"
 repository = "https://github.com/overcat/strledger"
 documentation = "https://github.com/overcat/strledger"
```

### Comparing `strledger-0.6.1/strledger/cli.py` & `strledger-0.6.2/strledger/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from urllib.parse import urljoin
 
 import click
 from ledgerwallet import __version__ as ledger_wallet_version
 from ledgerwallet import utils
 from ledgerwallet.client import CommException
 from stellar_sdk import (
+    DecoratedSignature,
     Network,
     parse_transaction_envelope_from_xdr,
     Server,
     TransactionEnvelope,
     FeeBumpTransactionEnvelope,
 )
 from stellar_sdk.xdr import HashIDPreimage
@@ -90,14 +91,20 @@
     "--keypair-index",
     type=int,
     required=False,
     help="Keypair Index.",
     default=DEFAULT_KEYPAIR_INDEX,
     show_default=True,
 )
+@click.option(
+    "-a",
+    "--hash-signing",
+    is_flag=True,
+    help="Only send the hash to the device for signing.",
+)
 @click.option("-s", "--submit", is_flag=True, help="Submit to Stellar Network.")
 @click.option(
     "-u",
     "--horizon-url",
     type=str,
     required=False,
     help="Horizon Server URL.",
@@ -107,14 +114,15 @@
 @click.argument("transaction_envelope")
 @click.pass_obj
 def sign_transaction(
     get_client: Callable[[], StrLedger],
     network_passphrase: str,
     transaction_envelope: str,
     keypair_index: int,
+    hash_signing: bool,
     submit: bool,
     horizon_url: str,
 ):
     """Sign a base64-encoded transaction envelope.
 
     For testnet transactions, use the following network passphrase:
     'Test SDF Network ; September 2015'
@@ -133,30 +141,50 @@
         )
         sys.exit(1)
     tx_hash = te.hash_hex()
     echo_normal(f"Network Passphrase: {network_passphrase}")
     echo_normal(f"Transaction Hash: {tx_hash}")
     echo_normal("Please confirm this transaction on Ledger.")
 
-    try:
-        assert isinstance(te, (TransactionEnvelope, FeeBumpTransactionEnvelope))
-        client.sign_transaction(transaction_envelope=te, keypair_index=keypair_index)
-    except CommException as e:
-        if e.sw == SW.DENY:
-            echo_error("The request to sign the transaction was denied.")
-        elif e.sw == SW.UNKNOWN_OP:
-            echo_error("The transaction contains unsupported operation(s).")
-        elif e.sw == SW.UNKNOWN_ENVELOPE_TYPE:
-            echo_error(
-                "The transaction contains unsupported transaction envelope type."
+    if hash_signing:
+        try:
+            signature = client.sign_transaction_hash(tx_hash, keypair_index)
+        except CommException as e:
+            if e.sw == SW.TX_HASH_SIGNING_MODE_NOT_ENABLED:
+                echo_error(
+                    "Hash signing is not enabled on this device.\n"
+                    "Please enable it on the device and try again."
+                )
+            elif e.sw == SW.DENY:
+                echo_error("The request to sign the transaction hash was denied.")
+                sys.exit(1)
+            else:
+                raise e
+        keypair = client.get_keypair(keypair_index=keypair_index)
+        decorated_signature = DecoratedSignature(keypair.signature_hint(), signature)
+        te.signatures.append(decorated_signature)
+    else:
+        try:
+            assert isinstance(te, (TransactionEnvelope, FeeBumpTransactionEnvelope))
+            client.sign_transaction(
+                transaction_envelope=te, keypair_index=keypair_index
             )
-        else:
-            echo_error(f"Unknown exception, you can the problem here: {__issue__}")
-            raise
-        sys.exit(1)
+        except CommException as e:
+            if e.sw == SW.DENY:
+                echo_error("The request to sign the transaction was denied.")
+            elif e.sw == SW.UNKNOWN_OP:
+                echo_error("The transaction contains unsupported operation(s).")
+            elif e.sw == SW.UNKNOWN_ENVELOPE_TYPE:
+                echo_error(
+                    "The transaction contains unsupported transaction envelope type."
+                )
+            else:
+                echo_error(f"Unknown exception, you can the problem here: {__issue__}")
+                raise
+            sys.exit(1)
 
     echo_success("Signed successfully.")
     echo_success("Base64-encoded signed transaction envelope:")
     echo_success(te.to_xdr())
     if submit:
         echo_normal("Submitting to the network...")
         server = Server(horizon_url)
```

### Comparing `strledger-0.6.1/strledger/core.py` & `strledger-0.6.2/strledger/core.py`

 * *Files identical despite different names*

### Comparing `strledger-0.6.1/PKG-INFO` & `strledger-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strledger
-Version: 0.6.1
+Version: 0.6.2
 Summary: Sign Stellar Transaction with Ledger on the command line.
 Home-page: https://github.com/overcat/strledger
 License: MIT
 Keywords: stellar,ledger
 Author: overcat
 Author-email: 4catcode@gmail.com
 Requires-Python: >=3.8,<4.0
```

