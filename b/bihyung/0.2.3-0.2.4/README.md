# Comparing `tmp/bihyung-0.2.3.tar.gz` & `tmp/bihyung-0.2.4.tar.gz`

## Comparing `bihyung-0.2.3.tar` & `bihyung-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 bihyung-0.2.3/bihyung/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-04-29 05:19:59.000000 bihyung-0.2.3/bihyung/.gitignore
--rw-r--r--   0     1001      127      426 2024-04-29 05:19:59.000000 bihyung-0.2.3/bihyung/langchain_example.py
--rw-r--r--   0     1001      127     4056 2024-04-29 05:19:59.000000 bihyung-0.2.3/bihyung/src/lib.rs
--rw-r--r--   0     1001      127   102173 2024-04-29 05:19:59.000000 bihyung-0.2.3/Cargo.lock
--rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 bihyung-0.2.3/Cargo.toml
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 bihyung-0.2.4/bihyung/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-04-30 03:32:42.000000 bihyung-0.2.4/bihyung/.gitignore
+-rw-r--r--   0     1001      127      426 2024-04-30 03:32:42.000000 bihyung-0.2.4/bihyung/langchain_example.py
+-rw-r--r--   0     1001      127     4056 2024-04-30 03:32:42.000000 bihyung-0.2.4/bihyung/src/lib.rs
+-rw-r--r--   0     1001      127   102173 2024-04-30 03:32:42.000000 bihyung-0.2.4/Cargo.lock
+-rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 bihyung-0.2.4/Cargo.toml
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.2.4/PKG-INFO
```

### Comparing `bihyung-0.2.3/bihyung/.gitignore` & `bihyung-0.2.4/bihyung/.gitignore`

 * *Files identical despite different names*

### Comparing `bihyung-0.2.3/bihyung/src/lib.rs` & `bihyung-0.2.4/bihyung/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.2.3/Cargo.lock` & `bihyung-0.2.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bihyung"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "enum_dispatch",
  "llm-daemon 0.2.0",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
  "tracing",
@@ -1683,15 +1683,15 @@
  "tracing",
  "tracing-subscriber",
  "url",
 ]
 
 [[package]]
 name = "llm-daemon"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "anyhow",
  "async-trait",
  "axum",
  "criterion",
  "daemonize",
  "futures",
```

