# Comparing `tmp/mllm-0.1.5.tar.gz` & `tmp/mllm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllm-0.1.5.tar", max compression
+gzip compressed data, was "mllm-0.1.6.tar", max compression
```

## Comparing `mllm-0.1.5.tar` & `mllm-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.5/LICENSE
--rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.5/README.md
--rw-r--r--   0        0        0      149 2024-04-29 21:17:19.261017 mllm-0.1.5/mllm/__init__.py
--rw-r--r--   0        0        0     1981 2024-04-27 22:13:37.479726 mllm-0.1.5/mllm/db/conn.py
--rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.5/mllm/db/models.py
--rw-r--r--   0        0        0      846 2024-04-29 21:16:16.874384 mllm-0.1.5/mllm/models.py
--rw-r--r--   0        0        0     5605 2024-04-29 21:16:42.671629 mllm-0.1.5/mllm/prompt.py
--rw-r--r--   0        0        0     8299 2024-04-29 21:17:12.773037 mllm-0.1.5/mllm/router.py
--rw-r--r--   0        0        0      793 2024-04-29 21:17:15.851578 mllm-0.1.5/mllm/util.py
--rw-r--r--   0        0        0      390 2024-04-29 21:17:25.763718 mllm-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.6/README.md
+-rw-r--r--   0        0        0      149 2024-04-29 21:17:19.261017 mllm-0.1.6/mllm/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-30 02:56:14.276096 mllm-0.1.6/mllm/db/conn.py
+-rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.6/mllm/db/models.py
+-rw-r--r--   0        0        0      846 2024-04-29 21:16:16.874384 mllm-0.1.6/mllm/models.py
+-rw-r--r--   0        0        0     5605 2024-04-30 21:03:51.206117 mllm-0.1.6/mllm/prompt.py
+-rw-r--r--   0        0        0     8299 2024-04-29 21:17:12.773037 mllm-0.1.6/mllm/router.py
+-rw-r--r--   0        0        0      793 2024-04-29 21:17:15.851578 mllm-0.1.6/mllm/util.py
+-rw-r--r--   0        0        0      390 2024-04-30 21:04:07.909036 mllm-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.6/PKG-INFO
```

### Comparing `mllm-0.1.5/LICENSE` & `mllm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mllm-0.1.5/README.md` & `mllm-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mllm-0.1.5/mllm/db/conn.py` & `mllm-0.1.6/mllm/db/conn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import time
 
 from sqlalchemy import create_engine, Engine
 from sqlalchemy.orm import sessionmaker
 
 from .models import Base
 
 
@@ -32,17 +33,22 @@
         client_encoding="utf8",
     )
 
     return engine
 
 
 def get_sqlite_conn() -> Engine:
-    print("connecting to local sqlite db ./data/prompts.db")
-    os.makedirs(os.path.dirname("./data/prompts.db"), exist_ok=True)
-    engine = create_engine("sqlite:///./data/prompts.db")
+    db_name = os.environ.get("MLLM_DB_NAME", "prompts.db")
+    db_path = os.environ.get("MLLM_DB_PATH", "./.data")
+    db_test = os.environ.get("MLLM_DB_TEST", "false") == "true"
+    if db_test:
+        db_name = f"mllm_test_{int(time.time())}.db"
+    print(f"\nconnecting to local sqlite db ./data/{db_name}")
+    os.makedirs(os.path.dirname(f"{db_path}/{db_name}"), exist_ok=True)
+    engine = create_engine(f"sqlite:///{db_path}/{db_name}")
     return engine
 
 
 if DB_TYPE == "postgres":
     engine = get_pg_conn()
 else:
     engine = get_sqlite_conn()
```

### Comparing `mllm-0.1.5/mllm/db/models.py` & `mllm-0.1.6/mllm/db/models.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.5/mllm/models.py` & `mllm-0.1.6/mllm/models.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.5/mllm/prompt.py` & `mllm-0.1.6/mllm/prompt.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.5/mllm/router.py` & `mllm-0.1.6/mllm/router.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.5/mllm/util.py` & `mllm-0.1.6/mllm/util.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.5/PKG-INFO` & `mllm-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllm
-Version: 0.1.5
+Version: 0.1.6
 Summary: Multimodal Large Language Models
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

