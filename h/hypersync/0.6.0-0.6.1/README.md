# Comparing `tmp/hypersync-0.6.0.tar.gz` & `tmp/hypersync-0.6.1.tar.gz`

## Comparing `hypersync-0.6.0.tar` & `hypersync-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 hypersync-0.6.0/Cargo.toml
--rw-r--r--   0     1001      127     2983 2024-04-20 23:46:42.000000 hypersync-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0     1001      127      699 2024-04-20 23:46:42.000000 hypersync-0.6.0/.gitignore
--rw-r--r--   0     1001      127    16725 2024-04-20 23:46:42.000000 hypersync-0.6.0/LICENSE
--rw-r--r--   0     1001      127      137 2024-04-20 23:46:42.000000 hypersync-0.6.0/README.md
--rw-r--r--   0     1001      127     4840 2024-04-20 23:46:42.000000 hypersync-0.6.0/erc20.abi.json
--rw-r--r--   0     1001      127     3232 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/all-erc20.py
--rw-r--r--   0     1001      127      959 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/simple-blocks-and-transaction-hashes.py
--rw-r--r--   0     1001      127      902 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/simple-blocks-and-transactions.py
--rw-r--r--   0     1001      127     1201 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/simple-logs-of-event.py
--rw-r--r--   0     1001      127      935 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/simple-logs.py
--rw-r--r--   0     1001      127     2694 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/top-usdt.py
--rw-r--r--   0     1001      127     5558 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/wallet.py
--rw-r--r--   0     1001      127     1906 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/watch.py
--rw-r--r--   0     1001      127     9132 2024-04-20 23:46:42.000000 hypersync-0.6.0/hypersync/__init__.py
--rw-r--r--   0     1001      127     2752 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/config.rs
--rw-r--r--   0     1001      127     4241 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/decode.rs
--rw-r--r--   0     1001      127    13235 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/from_arrow.rs
--rw-r--r--   0     1001      127    20356 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/lib.rs
--rw-r--r--   0     1001      127     7062 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/query.rs
--rw-r--r--   0     1001      127     6949 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/types.rs
--rw-r--r--   0     1001      127     9152 2024-04-20 23:46:42.000000 hypersync-0.6.0/test.py
--rw-r--r--   0     1001      127    82944 2024-04-20 23:46:42.000000 hypersync-0.6.0/Cargo.lock
--rw-r--r--   0     1001      127      604 2024-04-20 23:46:42.000000 hypersync-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 hypersync-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 hypersync-0.6.1/Cargo.toml
+-rw-r--r--   0     1001      127     2983 2024-04-30 03:40:33.000000 hypersync-0.6.1/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      699 2024-04-30 03:40:33.000000 hypersync-0.6.1/.gitignore
+-rw-r--r--   0     1001      127    16725 2024-04-30 03:40:33.000000 hypersync-0.6.1/LICENSE
+-rw-r--r--   0     1001      127      137 2024-04-30 03:40:33.000000 hypersync-0.6.1/README.md
+-rw-r--r--   0     1001      127     4840 2024-04-30 03:40:33.000000 hypersync-0.6.1/erc20.abi.json
+-rw-r--r--   0     1001      127     3232 2024-04-30 03:40:33.000000 hypersync-0.6.1/examples/all-erc20.py
+-rw-r--r--   0     1001      127      959 2024-04-30 03:40:33.000000 hypersync-0.6.1/examples/simple-blocks-and-transaction-hashes.py
+-rw-r--r--   0     1001      127      902 2024-04-30 03:40:33.000000 hypersync-0.6.1/examples/simple-blocks-and-transactions.py
+-rw-r--r--   0     1001      127     1201 2024-04-30 03:40:33.000000 hypersync-0.6.1/examples/simple-logs-of-event.py
+-rw-r--r--   0     1001      127      935 2024-04-30 03:40:33.000000 hypersync-0.6.1/examples/simple-logs.py
+-rw-r--r--   0     1001      127     2694 2024-04-30 03:40:33.000000 hypersync-0.6.1/examples/top-usdt.py
+-rw-r--r--   0     1001      127     5558 2024-04-30 03:40:33.000000 hypersync-0.6.1/examples/wallet.py
+-rw-r--r--   0     1001      127     1906 2024-04-30 03:40:33.000000 hypersync-0.6.1/examples/watch.py
+-rw-r--r--   0     1001      127     9132 2024-04-30 03:40:33.000000 hypersync-0.6.1/hypersync/__init__.py
+-rw-r--r--   0     1001      127     2752 2024-04-30 03:40:33.000000 hypersync-0.6.1/src/config.rs
+-rw-r--r--   0     1001      127     4241 2024-04-30 03:40:33.000000 hypersync-0.6.1/src/decode.rs
+-rw-r--r--   0     1001      127    13235 2024-04-30 03:40:33.000000 hypersync-0.6.1/src/from_arrow.rs
+-rw-r--r--   0     1001      127    20356 2024-04-30 03:40:33.000000 hypersync-0.6.1/src/lib.rs
+-rw-r--r--   0     1001      127     7062 2024-04-30 03:40:33.000000 hypersync-0.6.1/src/query.rs
+-rw-r--r--   0     1001      127     6949 2024-04-30 03:40:33.000000 hypersync-0.6.1/src/types.rs
+-rw-r--r--   0     1001      127     9152 2024-04-30 03:40:33.000000 hypersync-0.6.1/test.py
+-rw-r--r--   0     1001      127    82946 2024-04-30 03:40:33.000000 hypersync-0.6.1/Cargo.lock
+-rw-r--r--   0     1001      127      604 2024-04-30 03:40:33.000000 hypersync-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 hypersync-0.6.1/PKG-INFO
```

### Comparing `hypersync-0.6.0/Cargo.toml` & `hypersync-0.6.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "hypersync"
-version = "0.6.0"
+version = "0.6.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "hypersync"
 crate-type = ["cdylib"]
```

### Comparing `hypersync-0.6.0/.github/workflows/publish.yml` & `hypersync-0.6.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/.gitignore` & `hypersync-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/LICENSE` & `hypersync-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/erc20.abi.json` & `hypersync-0.6.1/erc20.abi.json`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/examples/all-erc20.py` & `hypersync-0.6.1/examples/all-erc20.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/examples/simple-blocks-and-transaction-hashes.py` & `hypersync-0.6.1/examples/simple-blocks-and-transaction-hashes.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/examples/simple-blocks-and-transactions.py` & `hypersync-0.6.1/examples/simple-blocks-and-transactions.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/examples/simple-logs-of-event.py` & `hypersync-0.6.1/examples/simple-logs-of-event.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/examples/simple-logs.py` & `hypersync-0.6.1/examples/simple-logs.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/examples/top-usdt.py` & `hypersync-0.6.1/examples/top-usdt.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/examples/wallet.py` & `hypersync-0.6.1/examples/wallet.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/examples/watch.py` & `hypersync-0.6.1/examples/watch.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/hypersync/__init__.py` & `hypersync-0.6.1/hypersync/__init__.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/src/config.rs` & `hypersync-0.6.1/src/config.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/src/decode.rs` & `hypersync-0.6.1/src/decode.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/src/from_arrow.rs` & `hypersync-0.6.1/src/from_arrow.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/src/lib.rs` & `hypersync-0.6.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/src/query.rs` & `hypersync-0.6.1/src/query.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/src/types.rs` & `hypersync-0.6.1/src/types.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/test.py` & `hypersync-0.6.1/test.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/Cargo.lock` & `hypersync-0.6.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
  "alloy-primitives",
  "alloy-sol-type-parser",
  "alloy-sol-types",
  "const-hex",
  "itoa",
  "serde",
  "serde_json",
- "winnow 0.6.6",
+ "winnow 0.6.7",
 ]
 
 [[package]]
 name = "alloy-json-abi"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24ed0f2a6c3a1c947b4508522a53a190dba8f94dcd4e3e1a5af945a498e78f2f"
@@ -141,15 +141,15 @@
 
 [[package]]
 name = "alloy-sol-type-parser"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0045cc89524e1451ccf33e8581355b6027ac7c6e494bb02959d4213ad0d8e91d"
 dependencies = [
- "winnow 0.6.6",
+ "winnow 0.6.7",
 ]
 
 [[package]]
 name = "alloy-sol-types"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad09ec5853fa700d12d778ad224dcdec636af424d29fad84fb9a2f16a5b0ef09"
@@ -916,17 +916,17 @@
 checksum = "a2a2b11eda1d40935b26cf18f6833c526845ae8c41e58d09af6adeb6f0269183"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fastrange-rs"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e90a1392cd6ec5ebe42ccaf251f2b7ba6be654c377f05c913f3898bfb2172512"
 
@@ -961,17 +961,17 @@
  "rand",
  "rustc-hex",
  "static_assertions",
 ]
 
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
@@ -1147,17 +1147,17 @@
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
 dependencies = [
  "ahash",
  "allocator-api2",
  "rayon",
 ]
 
 [[package]]
@@ -1272,15 +1272,15 @@
  "rustls",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
 name = "hypersync"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-json-abi",
  "alloy-primitives",
  "anyhow",
  "dict_derive",
  "env_logger",
@@ -1372,17 +1372,17 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -1420,17 +1420,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
@@ -1438,17 +1438,17 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
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
@@ -1618,33 +1618,33 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
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
 name = "parquet-format-safe"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
@@ -2057,17 +2057,17 @@
 checksum = "d25bf25ec5ae4a3f1b92f929810509a2f53d7dca2f50b794ff57e3face536c8f"
 dependencies = [
  "rand_core",
 ]
 
 [[package]]
 name = "raw-cpuid"
-version = "11.0.1"
+version = "11.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
+checksum = "e29830cbb1290e404f24c73af91c5d8d631ce7e128691e9477556b540cd01ecd"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "rayon"
 version = "1.10.0"
@@ -2086,19 +2086,19 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
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
@@ -2260,30 +2260,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver 1.0.22",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.11"
+version = "0.21.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fecbfb7b1444f477b345853b1fce097a2c6fb637b2bfb87e6bc5db0f043fae4"
+checksum = "3f56a14d1f48b391359b22f731fd4bd7e43c97f3c50eee276f3aa09c94784d3e"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -2382,26 +2382,26 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -2462,17 +2462,17 @@
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "skar-client"
-version = "0.18.0"
+version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0ef43bae6c714fa1ed747532a809c9415328f7be7f054d3cf8ea9847b9cd057"
+checksum = "279662d9dc05cc56b73e8f011c97cc673781ca8fec683c9cca592d977835e2b6"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-json-abi",
  "anyhow",
  "arrayvec",
  "capnp",
  "faster-hex",
@@ -2564,17 +2564,17 @@
 name = "snap"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b6b67fb9a61334225b5b790716f609cd58395f895b3fe8b328786812a40bc3b"
 
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
 name = "spin"
@@ -3206,17 +3206,17 @@
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.6.6"
+version = "0.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
+checksum = "14b9415ee827af173ebb3f15f9083df5a122eb93572ec28741fb153356ea2578"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
@@ -3280,32 +3280,32 @@
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "7.0.0"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `hypersync-0.6.0/pyproject.toml` & `hypersync-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hypersync-0.6.0/PKG-INFO` & `hypersync-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hypersync
-Version: 0.6.0
+Version: 0.6.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: strenum >=0.4.15, <0.4.16
```

