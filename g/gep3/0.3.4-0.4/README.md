# Comparing `tmp/gep3-0.3.4.tar.gz` & `tmp/gep3-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gep3-0.3.4.tar", last modified: Wed Apr 24 04:10:29 2024, max compression
+gzip compressed data, was "gep3-0.4.tar", last modified: Mon Apr 29 23:53:47 2024, max compression
```

## Comparing `gep3-0.3.4.tar` & `gep3-0.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.084082 gep3-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 04:10:22.000000 gep3-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-24 04:10:29.084082 gep3-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 04:10:22.000000 gep3-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 04:10:22.000000 gep3-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-24 04:10:29.084082 gep3-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.076082 gep3-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.080082 gep3-0.3.4/src/ccid/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-24 04:10:22.000000 gep3-0.3.4/src/ccid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-24 04:10:22.000000 gep3-0.3.4/src/ccid/bulk_in_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-24 04:10:22.000000 gep3-0.3.4/src/ccid/bulk_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-24 04:10:22.000000 gep3-0.3.4/src/ccid/bulk_out_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-24 04:10:22.000000 gep3-0.3.4/src/ccid/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.080082 gep3-0.3.4/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:22.000000 gep3-0.3.4/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-24 04:10:22.000000 gep3-0.3.4/src/common/ber.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-24 04:10:22.000000 gep3-0.3.4/src/common/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-24 04:10:22.000000 gep3-0.3.4/src/common/bitstr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-24 04:10:22.000000 gep3-0.3.4/src/common/hstr.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 04:10:22.000000 gep3-0.3.4/src/common/intlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-24 04:10:22.000000 gep3-0.3.4/src/common/parserc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-24 04:10:22.000000 gep3-0.3.4/src/common/str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.080082 gep3-0.3.4/src/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:22.000000 gep3-0.3.4/src/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-04-24 04:10:22.000000 gep3-0.3.4/src/crypto/des.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-24 04:10:22.000000 gep3-0.3.4/src/crypto/modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.080082 gep3-0.3.4/src/emv/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 04:10:22.000000 gep3-0.3.4/src/emv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-24 04:10:22.000000 gep3-0.3.4/src/emv/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-24 04:10:22.000000 gep3-0.3.4/src/emv/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 04:10:22.000000 gep3-0.3.4/src/emv/dsc.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-24 04:10:22.000000 gep3-0.3.4/src/emv/key_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-24 04:10:22.000000 gep3-0.3.4/src/emv/records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.084082 gep3-0.3.4/src/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:22.000000 gep3-0.3.4/src/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 04:10:22.000000 gep3-0.3.4/src/examples/emv_key_derivation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-24 04:10:22.000000 gep3-0.3.4/src/examples/evc_cvc3.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-24 04:10:22.000000 gep3-0.3.4/src/examples/evc_dcvv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.084082 gep3-0.3.4/src/gep3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-24 04:10:29.000000 gep3-0.3.4/src/gep3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-24 04:10:29.000000 gep3-0.3.4/src/gep3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:10:29.000000 gep3-0.3.4/src/gep3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 04:10:29.000000 gep3-0.3.4/src/gep3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 04:10:29.000000 gep3-0.3.4/src/gep3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.084082 gep3-0.3.4/src/globalplatform/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-24 04:10:22.000000 gep3-0.3.4/src/globalplatform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-24 04:10:22.000000 gep3-0.3.4/src/globalplatform/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-24 04:10:22.000000 gep3-0.3.4/src/globalplatform/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.084082 gep3-0.3.4/src/iso7816/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 04:10:22.000000 gep3-0.3.4/src/iso7816/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20583 2024-04-24 04:10:22.000000 gep3-0.3.4/src/iso7816/apdu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-24 04:10:22.000000 gep3-0.3.4/src/iso7816/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-24 04:10:22.000000 gep3-0.3.4/src/iso7816/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.084082 gep3-0.3.4/src/multos/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 04:10:22.000000 gep3-0.3.4/src/multos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 04:10:22.000000 gep3-0.3.4/src/multos/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-24 04:10:22.000000 gep3-0.3.4/src/multos/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:29.084082 gep3-0.3.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:10:22.000000 gep3-0.3.4/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-24 04:10:22.000000 gep3-0.3.4/src/tests/test_common_ber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-24 04:10:22.000000 gep3-0.3.4/src/tests/test_crypto_des.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 23:53:38.000000 gep3-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-29 23:53:47.480560 gep3-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 23:53:38.000000 gep3-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 23:53:38.000000 gep3-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-29 23:53:47.480560 gep3-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.472560 gep3-0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/ccid/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/bulk_in_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/bulk_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/bulk_out_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-29 23:53:38.000000 gep3-0.4/src/ccid/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:38.000000 gep3-0.4/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-29 23:53:38.000000 gep3-0.4/src/common/ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-04-29 23:53:38.000000 gep3-0.4/src/common/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-29 23:53:38.000000 gep3-0.4/src/common/bitstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-29 23:53:38.000000 gep3-0.4/src/common/hstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-29 23:53:38.000000 gep3-0.4/src/common/intlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-29 23:53:38.000000 gep3-0.4/src/common/parserc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-29 23:53:38.000000 gep3-0.4/src/common/str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:38.000000 gep3-0.4/src/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29456 2024-04-29 23:53:38.000000 gep3-0.4/src/crypto/des.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-29 23:53:38.000000 gep3-0.4/src/crypto/modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/emv/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/key_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-29 23:53:38.000000 gep3-0.4/src/emv/records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.476560 gep3-0.4/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:38.000000 gep3-0.4/src/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-29 23:53:38.000000 gep3-0.4/src/examples/emv_key_derivation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-29 23:53:38.000000 gep3-0.4/src/examples/evc_cvc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-29 23:53:38.000000 gep3-0.4/src/examples/evc_dcvv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/gep3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 23:53:47.000000 gep3-0.4/src/gep3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/globalplatform/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-29 23:53:38.000000 gep3-0.4/src/globalplatform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-29 23:53:38.000000 gep3-0.4/src/globalplatform/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-29 23:53:38.000000 gep3-0.4/src/globalplatform/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/iso7816/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-29 23:53:38.000000 gep3-0.4/src/iso7816/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16507 2024-04-29 23:53:38.000000 gep3-0.4/src/iso7816/apdu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-29 23:53:38.000000 gep3-0.4/src/iso7816/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-29 23:53:38.000000 gep3-0.4/src/iso7816/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/multos/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 23:53:38.000000 gep3-0.4/src/multos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-29 23:53:38.000000 gep3-0.4/src/multos/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-29 23:53:38.000000 gep3-0.4/src/multos/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:47.480560 gep3-0.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:53:38.000000 gep3-0.4/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-29 23:53:38.000000 gep3-0.4/src/tests/test_common_ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-29 23:53:38.000000 gep3-0.4/src/tests/test_crypto_des.py
```

### Comparing `gep3-0.3.4/LICENSE` & `gep3-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/PKG-INFO` & `gep3-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.3.4
+Version: 0.4
 Summary: Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 Home-page: https://github.com/spochic/gep3
 Author: Sebastien Pochic
 Author-email: spochic@gmail.com
 Project-URL: Bug Tracker, https://github.com/spochic/gep3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gep3-0.3.4/setup.cfg` & `gep3-0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gep3
-version = 0.3.4
+version = 0.4
 author = Sebastien Pochic
 author_email = spochic@gmail.com
 description = Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spochic/gep3
 project_urls =
```

### Comparing `gep3-0.3.4/src/ccid/__init__.py` & `gep3-0.4/src/ccid/__init__.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/ccid/bulk_in_messages.py` & `gep3-0.4/src/ccid/bulk_in_messages.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/ccid/bulk_message.py` & `gep3-0.4/src/ccid/bulk_message.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/ccid/bulk_out_messages.py` & `gep3-0.4/src/ccid/bulk_out_messages.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/ccid/descriptors.py` & `gep3-0.4/src/ccid/descriptors.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/common/ber.py` & `gep3-0.4/src/common/ber.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/common/bitstr.py` & `gep3-0.4/src/common/bitstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/common/hstr.py` & `gep3-0.4/src/common/hstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/common/intlist.py` & `gep3-0.4/src/common/intlist.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/common/parserc.py` & `gep3-0.4/src/common/parserc.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/common/str.py` & `gep3-0.4/src/common/str.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/crypto/modes.py` & `gep3-0.4/src/crypto/modes.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/emv/commands.py` & `gep3-0.4/src/emv/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from enum import StrEnum
 
 # Third party imports
 
 # Local application imports
 # from common.ber import encode
 from common.binary import ByteString
-from iso7816.apdu import CommandApdu, CommandField, create_command_APDU
+from iso7816.apdu import CommandApdu
+from iso7816.encodings import Lc, Le
 
 
 # Enum Definitions
 class ApplicationIdentifier(StrEnum):
     Mastercard = 'A0000000041010'
     Visa = 'A0000000031010'
     Maestro = 'A00000000410103060'
@@ -29,34 +30,37 @@
     PINTryCounter = '9F17'
     LogFormat = '9F4F'
 
 
 # Command APDUs defined by EMV
 class Select(CommandApdu):
     def __init__(self, aid: ByteString):
-        super().__init__(ByteString(
-            F'00A40400{len(aid):02X}') + aid + ByteString('00'))
+        header = ByteString('00A40400').blocks(1)
+        super().__init__(*header,  data_field=aid, Ne=256)
 
 
 def SELECT(aid: ByteString | ApplicationIdentifier) -> Select:
-    """SELECT(): generate CommandApdu for SELECT command
+    """SELECT(): generate CommandApdu for SELECT command (EMV)
     """
-    if isinstance(aid, ApplicationIdentifier):
-        return Select(ByteString(aid.value))
-    elif isinstance(aid, ByteString):
-        return Select(aid)
-    else:
-        raise TypeError(
-            F"emv.SELECT(): aid should be of type ByteString or ApplicationIdentifier, received: {type(aid)}")
+    match aid:
+        case ApplicationIdentifier():
+            application_identifier = ByteString(aid.value)
+        case ByteString():
+            application_identifier = aid
+        case _:
+            raise TypeError(
+                F"SELECT(): aid should be of type ByteString or ApplicationIdentifier, received: {type(aid)}")
+
+    return Select(application_identifier)
 
 
 class GetProcessingOptions(CommandApdu):
     def __init__(self, pdol: ByteString):
-        super().__init__(ByteString(
-            F'80A80000{len(pdol):02X}') + pdol + ByteString('00'))
+        header = ByteString('80A80000').blocks(1)
+        super().__init__(*header, data_field=pdol, Ne=256)
 
 
 def GET_PROCESSING_OPTIONS(pdol: ByteString | None) -> GetProcessingOptions:
     """GET_PROCESSING_OPTIONS(): generate APDU for GET PROCESSING OPTIONS command
     """
     if pdol:
         return GetProcessingOptions(pdol)
@@ -65,26 +69,28 @@
 
 
 GPO = GET_PROCESSING_OPTIONS
 
 
 class ReadRecord(CommandApdu):
     def __init__(self, SFI: int, record: int):
-        super().__init__(ByteString(F"00B2{record:02X}{SFI*8+4}00"))
+        header = ByteString(F"00B2{record:02X}{SFI*8+4}00").blocks(1)
+        super().__init__(*header, data_field=None, Ne=None)
 
 
 def READ_RECORD(SFI: int, record: int) -> ReadRecord:
     """READ_RECORD(): generate APDU for READ RECORD command
     """
     return ReadRecord(SFI, record)
 
 
 class GetData(CommandApdu):
     def __init__(self, tag: ByteString):
-        super().__init__(ByteString(F'80CA{tag}00'))
+        header = ByteString(F"80CA{tag}").blocks(1)
+        super().__init__(*header, data_field=None, Ne=256)
 
 
 def GET_DATA(tag: ByteString | GetDataObject) -> GetData:
     """GET_DATA: generate APDU for GET DATA command
     """
     if isinstance(tag, GetDataObject):
         if len(tag.value) == 2:
```

### Comparing `gep3-0.3.4/src/emv/data.py` & `gep3-0.4/src/emv/data.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/emv/dsc.py` & `gep3-0.4/src/emv/dsc.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/emv/key_management.py` & `gep3-0.4/src/emv/key_management.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/emv/records.py` & `gep3-0.4/src/emv/records.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/examples/emv_key_derivation.py` & `gep3-0.4/src/examples/emv_key_derivation.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/examples/evc_cvc3.py` & `gep3-0.4/src/examples/evc_cvc3.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/examples/evc_dcvv.py` & `gep3-0.4/src/examples/evc_dcvv.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/gep3.egg-info/PKG-INFO` & `gep3-0.4/src/gep3.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.3.4
+Version: 0.4
 Summary: Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 Home-page: https://github.com/spochic/gep3
 Author: Sebastien Pochic
 Author-email: spochic@gmail.com
 Project-URL: Bug Tracker, https://github.com/spochic/gep3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gep3-0.3.4/src/gep3.egg-info/SOURCES.txt` & `gep3-0.4/src/gep3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/globalplatform/encodings.py` & `gep3-0.4/src/globalplatform/encodings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """encodings.py
 """
 
 # Standard library imports
-from enum import Enum
+from enum import Enum, StrEnum, IntEnum
 
 # Third party imports
 
 # Local application imports
+from common.binary import ByteString
 from common.hstr import clean as _clean
 
 
 # Enum Definitions
-class SecureMessaging(Enum):
-    No = 'No secure messaging'
-    GlobalPlatform = 'Secure messaging - GlobalPlatform proprietary'
-    Iso7816 = 'Secure messaging - ISO7816 standard, command header not processed (no C-MAC)'
-    Iso7816_CMAC = 'Secure messaging - ISO7816 standard, command header authenticated (C-MAC)'
+class SecureMessaging(IntEnum):
+    No = 0x0
+    GlobalPlatform = 0x4
+    Iso7816 = 0x8
+    Iso7816_CMAC = 0xC
 
 
-class CardPersonalizationLifeCycleData(Enum):
+class CardPersonalizationLifeCycleData(StrEnum):
     ICFabricator = "IC Fabricator"
     ICType = "IC Type"
     OperatingSystemIdentifier = "Operating System Identifier"
     OperatingSystemReleaseDate = "Operating System Release Date"
     OperatingSystemReleaseLevel = "Operating System Release Level"
     ICFabricationDate = "IC Fabrication Date"
     ICSerialNumber = "IC Serial Number"
@@ -36,96 +37,84 @@
     ICPrePersonalizationEquipmentIdentifier = "IC Pre-Personalization Equipment Identifier"
     ICPersonalizer = "IC Personalizer"
     ICPersonalizationDate = "IC Personalization Date"
     ICPersonalizationEquipmentIdentifier = "IC Personalization Equipment Identifier"
 
 
 # Class Definitions
-class CLA:
+class ClassByte(ByteString):
     def __init__(self, secure_messaging: SecureMessaging, logical_channel: int):
-        if (logical_channel < 0) or (logical_channel > 19):
-            raise ValueError(
-                F'Logical channel number out of bound: should be in [0;19], received {logical_channel}')
+        match logical_channel:
+            case logical_channel if logical_channel < 0:
+                raise ValueError(
+                    F'Logical channel number out of bound: should be in [0;19], received {logical_channel}')
+
+            case logical_channel if logical_channel <= 3:
+                # CLA Byte Coding according to Table 11-11
+                _class_byte = 0x80
+                _class_byte += secure_messaging
+                _class_byte += logical_channel
+
+            case logical_channel if logical_channel <= 19:
+                # CLA Byte Coding according to Table 11-12
+                _class_byte = 0xC0 if secure_messaging == SecureMessaging.No else 0xE0
+                _class_byte += 4 + logical_channel
+
+            case _:
+                raise ValueError(
+                    F'Logical channel number out of bound: should be in [0;19], received {logical_channel}')
+
+        super().__init__(_class_byte)
 
-        self.__logical_channel = logical_channel
         self.__secure_messaging = secure_messaging
+        self.__logical_channel = logical_channel
 
-    @classmethod
-    def from_value(cls, CLA: int):
-        if (CLA < 0x00) or (CLA > 0xFF):
-            raise ValueError(
-                F'Class byte should out of bound: should be 2 bytes, received {CLA:X}')
-
-        secure_messaging: SecureMessaging
-        logical_channel: int
-
-        # Testing b7
-        if CLA & 0x40 == 0x00:
-            # CLA Byte Coding according to Table 11-11
-            # Testing b4-b3
-            match CLA & 0x0C:
-                case 0x00:
-                    secure_messaging = SecureMessaging.No
-                case 0x04:
-                    secure_messaging = SecureMessaging.GlobalPlatform
-                case 0x08:
-                    secure_messaging = SecureMessaging.Iso7816
-                case 0x0C:
-                    secure_messaging = SecureMessaging.Iso7816_CMAC
-                case _:
-                    # This should not happen
-                    raise ArithmeticError(
-                        F'CLA.from_value() error: CLA = {CLA:02X}')
-
-            logical_channel = CLA & 0x03
-
-        else:
-            # CLA Byte Coding according to Table 11-12
-            # Testing b6
-            if CLA & 0x20 == 0x00:
-                secure_messaging = SecureMessaging.No
-            else:
-                secure_messaging = SecureMessaging.GlobalPlatform
-
-            logical_channel = CLA & 0x0F
-
-        return cls(secure_messaging, logical_channel)
-
-    @classmethod
-    def from_string(cls, CLA: str):
-        return cls.from_value(int(_clean(CLA), 16))
+    @property
+    def secure_messaging(self) -> SecureMessaging:
+        return self.__secure_messaging
 
     @property
-    def value(self) -> int:
-        CLA = 0x00
+    def logical_channel(self) -> int:
+        return self.__logical_channel
 
-        if self.__logical_channel <= 3:
-            # CLA Byte Coding according to Table 11-11
-            CLA += 0x80 + self.__logical_channel
-            match self.__secure_messaging:
-                case SecureMessaging.No:
-                    CLA += 0x00
-                case SecureMessaging.GlobalPlatform:
-                    CLA += 0x04
-                case SecureMessaging.Iso7816:
-                    CLA += 0x08
-                case SecureMessaging.Iso7816_CMAC:
-                    CLA += 0x0C
-
-        else:
-            # CLA Byte Coding according to Table 11-12
-            CLA += 0xC0 + self.__logical_channel
-            if self.__secure_messaging != SecureMessaging.No:
-                CLA += 0x20
 
-        return CLA
+def CLA(value: int | str | ByteString) -> ClassByte:
+    """CLA(): creates a GlobalPlatform-compliant CLA Byte
+    """
+    match value:
+        case int():
+            class_byte = ByteString(value)
+        case str():
+            class_byte = ByteString(value)
+        case ByteString():
+            class_byte = value
+
+        case _:
+            raise TypeError(
+                F"CLA()| type {type(value)} not supported for argument value")
+
+    if len(class_byte) != 1:
+        raise ValueError(
+            F"CLA()| expecting 1 byte, received {class_byte} bytes")
+
+    if class_byte.is_bit_unset(8):
+        # GP CLA Byte must have b8 set
+        raise ValueError(F"CLA(): expecting b8 = 1, received {class_byte}")
+
+    if class_byte.is_bit_unset(7):
+        # CLA Byte Coding according to Table 11-11
+        secure_messaging = SecureMessaging(int(class_byte.mask(0x0C)))
+        logical_channel = int(class_byte.mask(0x03))
+    else:
+        # CLA Byte Coding according to Table 11-12
+        secure_messaging = SecureMessaging.No if class_byte.is_bit_unset(
+            6) else SecureMessaging.GlobalPlatform
+        logical_channel = 4 + int(class_byte.mask(0x0F))
 
-    @property
-    def string(self) -> str:
-        return F"{self.value:02X}"
+    return ClassByte(secure_messaging, logical_channel)
 
 
 class CPLC:
     def __init__(self, data: str):
         cplc_data = _clean(
             data, "globalplatform.encodings.CPLC.__init__()", "data")
         if len(cplc_data) != 84:
```

### Comparing `gep3-0.3.4/src/multos/commands.py` & `gep3-0.4/src/multos/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/multos/encodings.py` & `gep3-0.4/src/multos/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/tests/test_common_ber.py` & `gep3-0.4/src/tests/test_common_ber.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3.4/src/tests/test_crypto_des.py` & `gep3-0.4/src/tests/test_crypto_des.py`

 * *Files identical despite different names*

