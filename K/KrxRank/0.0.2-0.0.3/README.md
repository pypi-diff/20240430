# Comparing `tmp/krxrank-0.0.2.tar.gz` & `tmp/krxrank-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krxrank-0.0.2.tar", last modified: Mon Apr 29 21:51:40 2024, max compression
+gzip compressed data, was "krxrank-0.0.3.tar", last modified: Mon Apr 29 22:03:31 2024, max compression
```

## Comparing `krxrank-0.0.2.tar` & `krxrank-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 21:51:40.572963 krxrank-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-04-29 19:37:30.000000 krxrank-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1673 2024-04-29 21:51:40.571962 krxrank-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2024-04-29 20:42:29.000000 krxrank-0.0.2/README.md
--rw-rw-rw-   0        0        0      487 2024-04-29 21:51:28.000000 krxrank-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 21:51:40.572963 krxrank-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 21:51:40.540261 krxrank-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 21:51:40.548004 krxrank-0.0.2/src/KrxRank/
--rw-rw-rw-   0        0        0       21 2024-04-29 19:48:12.000000 krxrank-0.0.2/src/KrxRank/__init__.py
--rw-rw-rw-   0        0        0     3119 2024-04-29 19:48:12.000000 krxrank-0.0.2/src/KrxRank/etc.py
--rw-rw-rw-   0        0        0    22537 2024-04-29 19:48:12.000000 krxrank-0.0.2/src/KrxRank/rank.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:51:40.570962 krxrank-0.0.2/src/KrxRank.egg-info/
--rw-rw-rw-   0        0        0     1673 2024-04-29 21:51:40.000000 krxrank-0.0.2/src/KrxRank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-29 21:51:40.000000 krxrank-0.0.2/src/KrxRank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 21:51:40.000000 krxrank-0.0.2/src/KrxRank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 21:51:40.000000 krxrank-0.0.2/src/KrxRank.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 22:03:31.052602 krxrank-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 19:37:30.000000 krxrank-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1673 2024-04-29 22:03:31.051602 krxrank-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-04-29 20:42:29.000000 krxrank-0.0.3/README.md
+-rw-rw-rw-   0        0        0      479 2024-04-29 22:02:20.000000 krxrank-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 22:03:31.052602 krxrank-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 22:03:31.019572 krxrank-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:03:31.026579 krxrank-0.0.3/src/KrxRank/
+-rw-rw-rw-   0        0        0       21 2024-04-29 19:48:12.000000 krxrank-0.0.3/src/KrxRank/__init__.py
+-rw-rw-rw-   0        0        0     3119 2024-04-29 19:48:12.000000 krxrank-0.0.3/src/KrxRank/etc.py
+-rw-rw-rw-   0        0        0    22537 2024-04-29 19:48:12.000000 krxrank-0.0.3/src/KrxRank/rank.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:03:31.049599 krxrank-0.0.3/src/KrxRank.egg-info/
+-rw-rw-rw-   0        0        0     1673 2024-04-29 22:03:31.000000 krxrank-0.0.3/src/KrxRank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-29 22:03:31.000000 krxrank-0.0.3/src/KrxRank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 22:03:31.000000 krxrank-0.0.3/src/KrxRank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 22:03:31.000000 krxrank-0.0.3/src/KrxRank.egg-info/top_level.txt
```

### Comparing `krxrank-0.0.2/LICENSE` & `krxrank-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `krxrank-0.0.2/PKG-INFO` & `krxrank-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KrxRank
-Version: 0.0.2
+Version: 0.0.3
 Summary: KRX 정보데이터시스템 순위 통계 데이터 얻어오기
 Author-email: FinPro <finpro1224@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `krxrank-0.0.2/README.md` & `krxrank-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `krxrank-0.0.2/src/KrxRank/etc.py` & `krxrank-0.0.3/src/KrxRank/etc.py`

 * *Files identical despite different names*

### Comparing `krxrank-0.0.2/src/KrxRank/rank.py` & `krxrank-0.0.3/src/KrxRank/rank.py`

 * *Files identical despite different names*

### Comparing `krxrank-0.0.2/src/KrxRank.egg-info/PKG-INFO` & `krxrank-0.0.3/src/KrxRank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KrxRank
-Version: 0.0.2
+Version: 0.0.3
 Summary: KRX 정보데이터시스템 순위 통계 데이터 얻어오기
 Author-email: FinPro <finpro1224@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

