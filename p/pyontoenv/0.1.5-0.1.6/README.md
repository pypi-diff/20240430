# Comparing `tmp/pyontoenv-0.1.5.tar.gz` & `tmp/pyontoenv-0.1.6.tar.gz`

## Comparing `pyontoenv-0.1.5.tar` & `pyontoenv-0.1.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0     1001      127      776 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/Cargo.toml
--rw-r--r--   0     1001      127     5324 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/config.rs
--rw-r--r--   0     1001      127     2180 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/consts.rs
--rw-r--r--   0     1001      127     3267 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/doctor.rs
--rw-r--r--   0     1001      127      350 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/errors.rs
--rw-r--r--   0     1001      127    38576 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/lib.rs
--rw-r--r--   0     1001      127    13633 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/ontology.rs
--rw-r--r--   0     1001      127     3521 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/policy.rs
--rw-r--r--   0     1001      127     4646 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/transform.rs
--rw-r--r--   0     1001      127     6428 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/util.rs
--rw-r--r--   0     1001      127  1689944 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/Brick-1.3.ttl
--rw-r--r--   0     1001      127     1248 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model
--rw-r--r--   0     1001      127      321 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model.n3
--rw-r--r--   0     1001      127      537 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model.nt
--rw-r--r--   0     1001      127     1248 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model.ttl
--rw-r--r--   0     1001      127      789 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model.xml
--rw-r--r--   0     1001      127      909 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   146214 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0     1001      127    30521 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   163975 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0     1001      127  1323794 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127    17472 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127  1456008 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127   104496 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0     1001      127  1255550 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/bacnet.ttl
--rw-r--r--   0     1001      127    44502 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/brickpatches.ttl
--rw-r--r--   0     1001      127    81761 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/rec.ttl
--rw-r--r--   0     1001      127     4069 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/recimports.ttl
--rw-r--r--   0     1001      127    11876 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/ref-schema.ttl
--rw-r--r--   0     1001      127     1160 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data2/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data2/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data2/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data2/ont4.ttl
--rw-r--r--   0     1001      127     1248 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model
--rw-r--r--   0     1001      127      321 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model.n3
--rw-r--r--   0     1001      127      537 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model.nt
--rw-r--r--   0     1001      127     1248 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model.ttl
--rw-r--r--   0     1001      127      789 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model.xml
--rw-r--r--   0     1001      127  1689944 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
--rw-r--r--   0     1001      127     1160 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v1/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v1/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v1/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v1/ont4.ttl
--rw-r--r--   0     1001      127     1135 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v2/ont3.ttl
--rw-r--r--   0     1001      127     1129 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v2/ont5.ttl
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.5/python/Cargo.toml
--rw-r--r--   0     1001      127     2886 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/.gitignore
--rw-r--r--   0     1001      127      731 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/README.md
--rw-r--r--   0     1001      127       71 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/build.rs
--rw-r--r--   0     1001      127     5241 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/poetry.lock
--rw-r--r--   0     1001      127       71 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/requirements.dev.txt
--rw-r--r--   0     1001      127    14479 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/src/lib.rs
--rw-r--r--   0     1001      127      694 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/test.py
--rw-r--r--   0     1001      127    73924 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/Cargo.lock
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 pyontoenv-0.1.5/Cargo.toml
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 pyontoenv-0.1.5/PKG-INFO
+-rw-r--r--   0     1001      127      776 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/Cargo.toml
+-rw-r--r--   0     1001      127     5324 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/config.rs
+-rw-r--r--   0     1001      127     2180 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/consts.rs
+-rw-r--r--   0     1001      127     3267 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/doctor.rs
+-rw-r--r--   0     1001      127      350 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/errors.rs
+-rw-r--r--   0     1001      127    38576 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/lib.rs
+-rw-r--r--   0     1001      127    13633 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/ontology.rs
+-rw-r--r--   0     1001      127     3521 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/policy.rs
+-rw-r--r--   0     1001      127     4646 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/transform.rs
+-rw-r--r--   0     1001      127     6428 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/util.rs
+-rw-r--r--   0     1001      127  1689944 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/Brick-1.3.ttl
+-rw-r--r--   0     1001      127     1248 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model
+-rw-r--r--   0     1001      127      321 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model.n3
+-rw-r--r--   0     1001      127      537 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model.nt
+-rw-r--r--   0     1001      127     1248 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model.ttl
+-rw-r--r--   0     1001      127      789 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model.xml
+-rw-r--r--   0     1001      127      909 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   146214 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0     1001      127    30521 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   163975 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0     1001      127  1323794 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127    17472 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127  1456008 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127   104496 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0     1001      127  1255550 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/bacnet.ttl
+-rw-r--r--   0     1001      127    44502 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/brickpatches.ttl
+-rw-r--r--   0     1001      127    81761 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/rec.ttl
+-rw-r--r--   0     1001      127     4069 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/recimports.ttl
+-rw-r--r--   0     1001      127    11876 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/ref-schema.ttl
+-rw-r--r--   0     1001      127     1160 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data2/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data2/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data2/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data2/ont4.ttl
+-rw-r--r--   0     1001      127     1248 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model
+-rw-r--r--   0     1001      127      321 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model.n3
+-rw-r--r--   0     1001      127      537 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model.nt
+-rw-r--r--   0     1001      127     1248 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model.ttl
+-rw-r--r--   0     1001      127      789 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model.xml
+-rw-r--r--   0     1001      127  1689944 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
+-rw-r--r--   0     1001      127     1160 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v1/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v1/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v1/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v1/ont4.ttl
+-rw-r--r--   0     1001      127     1135 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v2/ont3.ttl
+-rw-r--r--   0     1001      127     1129 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v2/ont5.ttl
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.6/python/Cargo.toml
+-rw-r--r--   0     1001      127     2886 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/.gitignore
+-rw-r--r--   0     1001      127      731 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/README.md
+-rw-r--r--   0     1001      127       71 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/build.rs
+-rw-r--r--   0     1001      127     5241 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/poetry.lock
+-rw-r--r--   0     1001      127       71 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/requirements.dev.txt
+-rw-r--r--   0     1001      127    14479 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/src/lib.rs
+-rw-r--r--   0     1001      127      694 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/test.py
+-rw-r--r--   0     1001      127    73218 2024-04-29 19:46:26.000000 pyontoenv-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 pyontoenv-0.1.6/Cargo.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 pyontoenv-0.1.6/PKG-INFO
```

### Comparing `pyontoenv-0.1.5/lib/Cargo.toml` & `pyontoenv-0.1.6/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/src/config.rs` & `pyontoenv-0.1.6/lib/src/config.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/src/consts.rs` & `pyontoenv-0.1.6/lib/src/consts.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/src/doctor.rs` & `pyontoenv-0.1.6/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/src/lib.rs` & `pyontoenv-0.1.6/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/src/ontology.rs` & `pyontoenv-0.1.6/lib/src/ontology.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/src/policy.rs` & `pyontoenv-0.1.6/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/src/transform.rs` & `pyontoenv-0.1.6/lib/src/transform.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/src/util.rs` & `pyontoenv-0.1.6/lib/src/util.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/Brick-1.3.ttl` & `pyontoenv-0.1.6/lib/tests/data/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/model` & `pyontoenv-0.1.6/lib/tests/data/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/model.nt` & `pyontoenv-0.1.6/lib/tests/data/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/model.ttl` & `pyontoenv-0.1.6/lib/tests/data/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/model.xml` & `pyontoenv-0.1.6/lib/tests/data/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/bacnet.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/brickpatches.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/rec.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/recimports.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data/support/ref-schema.ttl` & `pyontoenv-0.1.6/lib/tests/data/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data2/ont1.ttl` & `pyontoenv-0.1.6/lib/tests/data2/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data2/ont2.ttl` & `pyontoenv-0.1.6/lib/tests/data2/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data2/ont3.ttl` & `pyontoenv-0.1.6/lib/tests/data2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/data2/ont4.ttl` & `pyontoenv-0.1.6/lib/tests/data2/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/fileendings/model` & `pyontoenv-0.1.6/lib/tests/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/fileendings/model.nt` & `pyontoenv-0.1.6/lib/tests/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/fileendings/model.ttl` & `pyontoenv-0.1.6/lib/tests/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/fileendings/model.xml` & `pyontoenv-0.1.6/lib/tests/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.6/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/updates/v1/ont1.ttl` & `pyontoenv-0.1.6/lib/tests/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/updates/v1/ont2.ttl` & `pyontoenv-0.1.6/lib/tests/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/updates/v1/ont3.ttl` & `pyontoenv-0.1.6/lib/tests/updates/v1/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/updates/v1/ont4.ttl` & `pyontoenv-0.1.6/lib/tests/updates/v1/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/updates/v2/ont3.ttl` & `pyontoenv-0.1.6/lib/tests/updates/v2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/lib/tests/updates/v2/ont5.ttl` & `pyontoenv-0.1.6/lib/tests/updates/v2/ont5.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/python/Cargo.toml` & `pyontoenv-0.1.6/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/python/.github/workflows/CI.yml` & `pyontoenv-0.1.6/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/python/.gitignore` & `pyontoenv-0.1.6/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/python/README.md` & `pyontoenv-0.1.6/python/README.md`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/python/poetry.lock` & `pyontoenv-0.1.6/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/python/src/lib.rs` & `pyontoenv-0.1.6/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/python/test.py` & `pyontoenv-0.1.6/python/test.py`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.5/Cargo.lock` & `pyontoenv-0.1.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -553,29 +553,14 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
-name = "foreign-types"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
-dependencies = [
- "foreign-types-shared",
-]
-
-[[package]]
-name = "foreign-types-shared"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
-
-[[package]]
 name = "form_urlencoded"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
@@ -841,24 +826,25 @@
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
-name = "hyper-tls"
-version = "0.5.0"
+name = "hyper-rustls"
+version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6183ddfa99b85da61a140bea0efc93fdf56ceaa041b37d553518030827f9905"
+checksum = "8d78e1e73ec14cf7375674f74d7dde185c8206fd9dea6fb6295e8a98098aaa97"
 dependencies = [
- "bytes",
+ "futures-util",
+ "http",
  "hyper",
- "native-tls",
+ "rustls",
  "tokio",
- "tokio-native-tls",
+ "tokio-rustls",
 ]
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
@@ -1348,32 +1334,14 @@
 [[package]]
 name = "mown"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7627d8bbeb17edbf1c3f74b21488e4af680040da89713b4217d0010e9cbd97e"
 
 [[package]]
-name = "native-tls"
-version = "0.2.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
-dependencies = [
- "lazy_static",
- "libc",
- "log",
- "openssl",
- "openssl-probe",
- "openssl-sys",
- "schannel",
- "security-framework",
- "security-framework-sys",
- "tempfile",
-]
-
-[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
@@ -1407,15 +1375,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1433,69 +1401,25 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
 ]
 
 [[package]]
-name = "openssl"
-version = "0.10.64"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
-dependencies = [
- "bitflags 2.5.0",
- "cfg-if",
- "foreign-types",
- "libc",
- "once_cell",
- "openssl-macros",
- "openssl-sys",
-]
-
-[[package]]
-name = "openssl-macros"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.60",
-]
-
-[[package]]
-name = "openssl-probe"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
-
-[[package]]
-name = "openssl-sys"
-version = "0.9.102"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
-dependencies = [
- "cc",
- "libc",
- "pkg-config",
- "vcpkg",
-]
-
-[[package]]
 name = "oxigraph"
 version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3285d2243e62417ee2cabeae86d3dcc07cfb7e5eaf1cd94b799d4f68f3d3a149"
 dependencies = [
  "digest",
  "getrandom",
@@ -1661,20 +1585,14 @@
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
-name = "pkg-config"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
-
-[[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "powerfmt"
@@ -1801,15 +1719,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
@@ -1974,40 +1892,71 @@
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "hyper",
- "hyper-tls",
+ "hyper-rustls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
- "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
+ "rustls",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "system-configuration",
  "tokio",
- "tokio-native-tls",
+ "tokio-rustls",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
+ "webpki-roots",
  "winreg",
 ]
 
 [[package]]
+name = "ring"
+version = "0.16.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
+dependencies = [
+ "cc",
+ "libc",
+ "once_cell",
+ "spin 0.5.2",
+ "untrusted 0.7.1",
+ "web-sys",
+ "winapi",
+]
+
+[[package]]
+name = "ring"
+version = "0.17.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "getrandom",
+ "libc",
+ "spin 0.9.8",
+ "untrusted 0.9.0",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "rio_api"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1924fa1f0e6d851f9b73b3c569e607c368a0d92995d99d563ad7bf1414696603"
 
 [[package]]
 name = "rio_turtle"
@@ -2054,23 +2003,45 @@
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "rustls"
+version = "0.21.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+dependencies = [
+ "log",
+ "ring 0.17.8",
+ "rustls-webpki",
+ "sct",
+]
+
+[[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
  "base64 0.21.7",
 ]
 
 [[package]]
+name = "rustls-webpki"
+version = "0.101.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
+dependencies = [
+ "ring 0.17.8",
+ "untrusted 0.9.0",
+]
+
+[[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "ryu-js"
@@ -2090,49 +2061,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "schannel"
-version = "0.1.23"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
-dependencies = [
- "windows-sys 0.52.0",
-]
-
-[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "security-framework"
-version = "2.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
-dependencies = [
- "bitflags 1.3.2",
- "core-foundation",
- "core-foundation-sys",
- "libc",
- "security-framework-sys",
-]
-
-[[package]]
-name = "security-framework-sys"
-version = "2.10.0"
+name = "sct"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
+checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
 dependencies = [
- "core-foundation-sys",
- "libc",
+ "ring 0.16.20",
+ "untrusted 0.7.1",
 ]
 
 [[package]]
 name = "serde"
 version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
@@ -2303,14 +2252,26 @@
  "oxiri",
  "oxrdf",
  "peg",
  "rand 0.8.5",
 ]
 
 [[package]]
+name = "spin"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
+
+[[package]]
+name = "spin"
+version = "0.9.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
+
+[[package]]
 name = "static-iref"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9786d4b8e9e5423fe85c57a826d7e0f0774746149a2ccd21e2104ff74b71ce7"
 dependencies = [
  "iref",
 ]
@@ -2488,20 +2449,20 @@
  "mio",
  "pin-project-lite",
  "socket2",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "tokio-native-tls"
-version = "0.3.1"
+name = "tokio-rustls"
+version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
+checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "native-tls",
+ "rustls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
 version = "0.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2576,14 +2537,26 @@
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "untrusted"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
+
+[[package]]
+name = "untrusted"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
+
+[[package]]
 name = "url"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
@@ -2599,20 +2572,14 @@
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
-name = "vcpkg"
-version = "0.2.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
-
-[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
@@ -2712,14 +2679,20 @@
 checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "webpki-roots"
+version = "0.25.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5f20c57d8d7db6d3b86154206ae5d8fba62dd39573114de97c2cb0578251f8e1"
+
+[[package]]
 name = "which"
 version = "4.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87ba24419a2078cd2b0f2ede2691b6c66d8e47836da3b6db8265ebad47afbfc7"
 dependencies = [
  "either",
  "home",
```

### Comparing `pyontoenv-0.1.5/Cargo.toml` & `pyontoenv-0.1.6/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.5"
+version = "0.1.6"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
+readme = "README.md"
 
 [workspace.dependencies]
 anyhow = "1.0.79"
 regex = "1.10.3"
 walkdir = "2.4.0"
-reqwest = { version = "0.11", features = ["blocking", "json"] }
+reqwest = { version = "0.11", features = ["blocking", "json", "rustls-tls"], default-features = false }
 json-ld = "0.15.1"
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 env_logger = "0.11.1"
 log = "0.4.20"
 serde_regex = "1.1.0"
 glob = "0.3.1"
```

### Comparing `pyontoenv-0.1.5/pyproject.toml` & `pyontoenv-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.5"
+version = "0.1.6"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyontoenv-0.1.5/PKG-INFO` & `pyontoenv-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyontoenv
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Command line tool to manage ontologies and their imports in a local environment
 Home-Page: https://github.com/gtfierro/ontoenv-rs
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
```

