# Comparing `tmp/pyreqwest_impersonate-0.3.1.tar.gz` & `tmp/pyreqwest_impersonate-0.3.2.tar.gz`

## Comparing `pyreqwest_impersonate-0.3.1.tar` & `pyreqwest_impersonate-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.1/Cargo.toml
--rw-r--r--   0     1001      127     4854 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/.gitignore
--rw-r--r--   0     1001      127     7758 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/README.md
--rw-r--r--   0     1001      127      271 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/1_threads.csv
--rw-r--r--   0     1001      127      273 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/4_threads.csv
--rw-r--r--   0     1001      127      343 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/README.md
--rw-r--r--   0     1001      127     3299 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/benchmark.py
--rw-r--r--   0     1001      127       83 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/requirements.txt
--rw-r--r--   0     1001      127      799 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/server.py
--rw-r--r--   0     1001      127    23737 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/src/lib.rs
--rw-r--r--   0     1001      127     3033 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/src/response.rs
--rw-r--r--   0     1001      127     3922 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/tests/test_client.py
--rw-r--r--   0     1001      127     5573 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/tests/test_defs.py
--rw-r--r--   0     1001      127    41713 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8827 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      127     4854 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/.gitignore
+-rw-r--r--   0     1001      127     7808 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/README.md
+-rw-r--r--   0     1001      127      273 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/1_threads.csv
+-rw-r--r--   0     1001      127      273 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/4_threads.csv
+-rw-r--r--   0     1001      127      343 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/README.md
+-rw-r--r--   0     1001      127     3299 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/benchmark.py
+-rw-r--r--   0     1001      127       83 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      799 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/benchmark/server.py
+-rw-r--r--   0     1001      127    23737 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      127     3033 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/src/response.rs
+-rw-r--r--   0     1001      127     3830 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/tests/test_client.py
+-rw-r--r--   0     1001      127     5370 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/tests/test_defs.py
+-rw-r--r--   0     1001      127    41944 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-04-30 12:05:28.000000 pyreqwest_impersonate-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8877 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.2/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.3.1/Cargo.toml` & `pyreqwest_impersonate-0.3.2/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.3.1"
+version = "0.3.2"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
```

### Comparing `pyreqwest_impersonate-0.3.1/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.3.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.1/.gitignore` & `pyreqwest_impersonate-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.1/README.md` & `pyreqwest_impersonate-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,18 @@
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
         impersonate (str, optional): Entity to impersonate. Example: "chrome_123". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123"
-            Safari: "safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5","safari_17_2_1"
+            Safari: "safari_ios_17_2","safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5",
+                "safari_17_2_1","safari17_4_1"
             OkHttp: "okhttp_3_9","okhttp_3_11","okhttp_3_13","okhttp_3_14","okhttp_4_9","okhttp_4_10","okhttp_5"
-            Edge: "edge_99","edge_101","edge_120"
+            Edge: "edge_99","edge_101","edge_122"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is False.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
          
     """
```

### Comparing `pyreqwest_impersonate-0.3.1/benchmark/benchmark.py` & `pyreqwest_impersonate-0.3.2/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.1/benchmark/server.py` & `pyreqwest_impersonate-0.3.2/benchmark/server.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.1/src/lib.rs` & `pyreqwest_impersonate-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.1/src/response.rs` & `pyreqwest_impersonate-0.3.2/src/response.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.1/tests/test_client.py` & `pyreqwest_impersonate-0.3.2/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from time import sleep
-from urllib.parse import parse_qs
 
 from pyreqwest_impersonate import Client
 
 
 def retry(max_retries=3, delay=1):
     def decorator(func):
         def wrapper(*args, **kwargs):
@@ -96,16 +95,15 @@
     )
     assert response.status_code == 200
     json_data = response.json()
     assert json_data["method"] == "POST"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
-    received_data_dict = parse_qs(json_data["data"])
-    assert received_data_dict == {"key1": ["value1"], "key2": ["value2"]}
+    assert json_data["form"] == {"key1": "value1", "key2": "value2"}
 
 
 @retry()
 def test_client_impersonate():
     client = Client(impersonate="chrome_123", verify=False)
     response = client.get("https://tls.peet.ws/api/all")
     assert response.status_code == 200
```

### Comparing `pyreqwest_impersonate-0.3.1/tests/test_defs.py` & `pyreqwest_impersonate-0.3.2/tests/test_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from time import sleep
-from urllib.parse import parse_qs
 
 import pyreqwest_impersonate as pri
 
 
 def retry(max_retries=3, delay=1):
     def decorator(func):
         def wrapper(*args, **kwargs):
@@ -115,16 +114,16 @@
     )
     assert response.status_code == 200
     json_data = response.json()
     assert json_data["method"] == "POST"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
-    received_data_dict = parse_qs(json_data["data"])
-    assert received_data_dict == {"key1": ["value1"], "key2": ["value2"]}
+    assert json_data["form"] == {"key1": "value1", "key2": "value2"}
+    
 
 
 @retry()
 def test_patch():
     auth_bearer = "bearerXXXXXXXXXXXXXXXXXXXX"
     headers = {"X-Test": "test"}
     params = {"x": "aaa", "y": "bbb"}
@@ -138,16 +137,15 @@
     )
     assert response.status_code == 200
     json_data = response.json()
     assert json_data["method"] == "PATCH"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
-    received_data_dict = parse_qs(json_data["data"])
-    assert received_data_dict == {"key1": ["value1"], "key2": ["value2"]}
+    assert json_data["form"] == {"key1": "value1", "key2": "value2"}
 
 
 @retry()
 def test_put():
     auth_bearer = "bearerXXXXXXXXXXXXXXXXXXXX"
     headers = {"X-Test": "test"}
     params = {"x": "aaa", "y": "bbb"}
@@ -161,9 +159,8 @@
     )
     assert response.status_code == 200
     json_data = response.json()
     assert json_data["method"] == "PUT"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
-    received_data_dict = parse_qs(json_data["data"])
-    assert received_data_dict == {"key1": ["value1"], "key2": ["value2"]}
+    assert json_data["form"] == {"key1": "value1", "key2": "value2"}
```

### Comparing `pyreqwest_impersonate-0.3.1/Cargo.lock` & `pyreqwest_impersonate-0.3.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,19 @@
 name = "antidote"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34fde25430d87a9388dadbe6e34d7f72a462c8b43ac8d309b42b0a8505d7e2a5"
 
 [[package]]
 name = "async-compression"
-version = "0.4.8"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07dbbf24db18d609b1462965249abdf49129ccad073ec257da372adc83259c60"
+checksum = "4e9eabd7a98fe442131a17c316bd9349c43695e49e730c3c8e12cfb5f4da2693"
 dependencies = [
- "brotli 4.0.0",
+ "brotli 5.0.0",
  "flate2",
  "futures-core",
  "memchr",
  "pin-project-lite",
  "tokio",
 ]
 
@@ -154,38 +154,38 @@
  "alloc-no-stdlib",
  "alloc-stdlib",
  "brotli-decompressor 2.5.1",
 ]
 
 [[package]]
 name = "brotli"
-version = "4.0.0"
+version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "125740193d7fee5cc63ab9e16c2fdc4e07c74ba755cc53b327d6ea029e9fc569"
+checksum = "19483b140a7ac7174d34b5a581b406c64f84da5409d3e09cf4fff604f9270e67"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
- "brotli-decompressor 3.0.0",
+ "brotli-decompressor 4.0.0",
 ]
 
 [[package]]
 name = "brotli-decompressor"
 version = "2.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e2e4afe60d7dd600fdd3de8d0f08c2b7ec039712e3b6137ff98b7004e82de4f"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "brotli-decompressor"
-version = "3.0.0"
+version = "4.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65622a320492e09b5e0ac436b14c54ff68199bac392d0e89a6832c4518eea525"
+checksum = "e6221fe77a248b9117d431ad93761222e1cf8ff282d9d1d5d9f53d6299a1cf76"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
@@ -197,17 +197,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.92"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
 dependencies = [
@@ -321,17 +321,17 @@
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -452,17 +452,17 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -623,26 +623,26 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
@@ -654,17 +654,17 @@
 checksum = "47186c6da4d81ca383c7c47c1bfc80f4b95f4720514d860a5407aaf4233f9588"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -768,33 +768,33 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -821,17 +821,17 @@
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psl-types"
 version = "2.0.11"
@@ -846,17 +846,17 @@
 dependencies = [
  "idna 0.3.0",
  "psl-types",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -864,60 +864,60 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "encoding_rs",
  "pyo3",
  "pythonize",
  "reqwest-impersonate",
  "serde_json",
 ]
@@ -939,19 +939,19 @@
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -977,17 +977,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest-impersonate"
-version = "0.11.69"
+version = "0.11.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca713112440b818dade748d74fef3965a8c058e2eb735333bac5a1bdbb59cdd4"
+checksum = "5b725314a794f526bac22292a10e2bf581cbea5ebd527fa3032e2cfd829068be"
 dependencies = [
  "async-compression",
  "base64",
  "boring-imp",
  "boring-sys-imp",
  "bytes",
  "cookie",
@@ -1047,37 +1047,37 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1111,27 +1111,27 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1159,26 +1159,26 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1472,15 +1472,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1492,110 +1492,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
```

### Comparing `pyreqwest_impersonate-0.3.1/pyproject.toml` & `pyreqwest_impersonate-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.1/PKG-INFO` & `pyreqwest_impersonate-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -75,17 +75,18 @@
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
         impersonate (str, optional): Entity to impersonate. Example: "chrome_123". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123"
-            Safari: "safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5","safari_17_2_1"
+            Safari: "safari_ios_17_2","safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5",
+                "safari_17_2_1","safari17_4_1"
             OkHttp: "okhttp_3_9","okhttp_3_11","okhttp_3_13","okhttp_3_14","okhttp_4_9","okhttp_4_10","okhttp_5"
-            Edge: "edge_99","edge_101","edge_120"
+            Edge: "edge_99","edge_101","edge_122"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is False.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
          
     """
```

