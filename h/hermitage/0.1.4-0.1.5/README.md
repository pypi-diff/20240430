# Comparing `tmp/hermitage-0.1.4.tar.gz` & `tmp/hermitage-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage-0.1.4.tar", max compression
+gzip compressed data, was "hermitage-0.1.5.tar", max compression
```

## Comparing `hermitage-0.1.4.tar` & `hermitage-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       46 2024-04-15 11:34:36.787863 hermitage-0.1.4/README.md
--rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.4/hermitage/__init__.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.4/hermitage/definition/__init__.py
--rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.4/hermitage/definition/contracts.py
--rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.4/hermitage/mappers/__init__.py
--rw-r--r--   0        0        0     1235 2024-04-24 07:28:43.056982 hermitage-0.1.4/hermitage/mappers/invoice.py
--rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.4/hermitage/parsers/__init__.py
--rw-r--r--   0        0        0     2836 2024-04-13 13:20:31.671188 hermitage-0.1.4/hermitage/parsers/query.py
--rw-r--r--   0        0        0      361 2024-04-24 07:29:35.528391 hermitage-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-04-15 11:34:36.787863 hermitage-0.1.5/README.md
+-rw-r--r--   0        0        0      257 2024-04-13 13:50:37.630467 hermitage-0.1.5/hermitage/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.5/hermitage/definition/__init__.py
+-rw-r--r--   0        0        0    11820 2024-04-13 13:19:43.140011 hermitage-0.1.5/hermitage/definition/contracts.py
+-rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.5/hermitage/mappers/__init__.py
+-rw-r--r--   0        0        0     1235 2024-04-24 07:28:43.056982 hermitage-0.1.5/hermitage/mappers/invoice.py
+-rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.5/hermitage/parsers/__init__.py
+-rw-r--r--   0        0        0     2836 2024-04-13 13:20:31.671188 hermitage-0.1.5/hermitage/parsers/query.py
+-rw-r--r--   0        0        0      361 2024-04-29 15:53:32.455489 hermitage-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.1.5/PKG-INFO
```

### Comparing `hermitage-0.1.4/hermitage/definition/contracts.py` & `hermitage-0.1.5/hermitage/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.4/hermitage/mappers/invoice.py` & `hermitage-0.1.5/hermitage/mappers/invoice.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.4/hermitage/parsers/query.py` & `hermitage-0.1.5/hermitage/parsers/query.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.1.4/PKG-INFO` & `hermitage-0.1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: hermitage
-Version: 0.1.4
+Version: 0.1.5
 Summary: Universal storage access framework
 Home-page: https://github.com/smairon/hermitage
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: zodchy (>=0.1.0,<0.2.0)
+Requires-Dist: zodchy (>=0.2.3,<0.3.0)
 Project-URL: Repository, https://github.com/smairon/hermitage
 Description-Content-Type: text/markdown
 
 # Hermitage
 Universal storage access framework
```

