# Comparing `tmp/crud_repository-0.1.3.tar.gz` & `tmp/crud_repository-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crud_repository-0.1.3.tar", last modified: Tue Apr 30 19:23:47 2024, max compression
+gzip compressed data, was "crud_repository-0.1.5.tar", last modified: Tue Apr 30 20:50:53 2024, max compression
```

## Comparing `crud_repository-0.1.3.tar` & `crud_repository-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.397499 crud_repository-0.1.3/
--rw-r--r--   0 dalexander   (501) staff       (20)     1073 2024-04-12 07:44:52.000000 crud_repository-0.1.3/LICENSE
--rw-r--r--   0 dalexander   (501) staff       (20)      293 2024-04-30 09:31:25.000000 crud_repository-0.1.3/MANIFEST.in
--rw-r--r--   0 dalexander   (501) staff       (20)     6746 2024-04-30 19:23:47.397264 crud_repository-0.1.3/PKG-INFO
--rw-r--r--   0 dalexander   (501) staff       (20)     4199 2024-04-30 19:23:29.000000 crud_repository-0.1.3/PYPI.md
--rw-r--r--   0 dalexander   (501) staff       (20)    12003 2024-04-30 19:23:29.000000 crud_repository-0.1.3/README.md
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.396369 crud_repository-0.1.3/crud_repository.egg-info/
--rw-r--r--   0 dalexander   (501) staff       (20)     6746 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/PKG-INFO
--rw-r--r--   0 dalexander   (501) staff       (20)      749 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/SOURCES.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/dependency_links.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 19:13:57.000000 crud_repository-0.1.3/crud_repository.egg-info/not-zip-safe
--rw-r--r--   0 dalexander   (501) staff       (20)      140 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/requires.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        4 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/top_level.txt
--rw-r--r--   0 dalexander   (501) staff       (20)     1443 2024-04-30 19:23:29.000000 crud_repository-0.1.3/pyproject.toml
--rw-r--r--   0 dalexander   (501) staff       (20)      281 2024-04-30 19:23:47.398157 crud_repository-0.1.3/setup.cfg
--rw-r--r--   0 dalexander   (501) staff       (20)      818 2024-04-30 19:20:19.000000 crud_repository-0.1.3/setup.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.383691 crud_repository-0.1.3/src/
--rw-r--r--   0 dalexander   (501) staff       (20)     3194 2024-04-30 01:09:48.000000 crud_repository-0.1.3/src/__config__.py
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-30 01:00:42.000000 crud_repository-0.1.3/src/__init__.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.385470 crud_repository-0.1.3/src/db/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-09 20:51:28.000000 crud_repository-0.1.3/src/db/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2129 2024-04-24 16:01:46.000000 crud_repository-0.1.3/src/db/factory.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1415 2024-04-24 01:01:37.000000 crud_repository-0.1.3/src/db/idatabase.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.386750 crud_repository-0.1.3/src/db/mariadb/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:13.000000 crud_repository-0.1.3/src/db/mariadb/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2510 2024-04-30 00:14:45.000000 crud_repository-0.1.3/src/db/mariadb/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.388035 crud_repository-0.1.3/src/db/mysql/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:26.000000 crud_repository-0.1.3/src/db/mysql/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2279 2024-04-30 00:14:45.000000 crud_repository-0.1.3/src/db/mysql/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.389118 crud_repository-0.1.3/src/db/postgres/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:03.000000 crud_repository-0.1.3/src/db/postgres/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1877 2024-04-30 00:14:45.000000 crud_repository-0.1.3/src/db/postgres/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.390365 crud_repository-0.1.3/src/model/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 17:00:08.000000 crud_repository-0.1.3/src/model/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)      190 2024-04-09 20:58:35.000000 crud_repository-0.1.3/src/model/base.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.393981 crud_repository-0.1.3/src/my_logger/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-15 08:17:30.000000 crud_repository-0.1.3/src/my_logger/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1973 2024-04-24 22:03:32.000000 crud_repository-0.1.3/src/my_logger/formatters.py
--rw-r--r--   0 dalexander   (501) staff       (20)     5131 2024-04-24 22:03:32.000000 crud_repository-0.1.3/src/my_logger/handlers.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1742 2024-04-26 00:51:10.000000 crud_repository-0.1.3/src/my_logger/logger.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1515 2024-04-24 22:03:32.000000 crud_repository-0.1.3/src/my_logger/monitor.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.395210 crud_repository-0.1.3/src/repo/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 03:50:05.000000 crud_repository-0.1.3/src/repo/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2953 2024-04-29 23:49:54.000000 crud_repository-0.1.3/src/repo/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.294226 crud_repository-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 20:50:45.000000 crud_repository-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-30 20:50:45.000000 crud_repository-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-04-30 20:50:53.294226 crud_repository-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-30 20:50:45.000000 crud_repository-0.1.5/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-30 20:50:45.000000 crud_repository-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.294226 crud_repository-0.1.5/crud_repository.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-04-30 20:50:53.000000 crud_repository-0.1.5/crud_repository.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-30 20:50:53.000000 crud_repository-0.1.5/crud_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:50:53.000000 crud_repository-0.1.5/crud_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:50:53.000000 crud_repository-0.1.5/crud_repository.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-30 20:50:53.000000 crud_repository-0.1.5/crud_repository.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 20:50:53.000000 crud_repository-0.1.5/crud_repository.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-30 20:50:51.000000 crud_repository-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 20:50:53.294226 crud_repository-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 20:50:45.000000 crud_repository-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.290226 crud_repository-0.1.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.290226 crud_repository-0.1.5/src/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/idatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.294226 crud_repository-0.1.5/src/db/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/mariadb/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.294226 crud_repository-0.1.5/src/db/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/mysql/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.294226 crud_repository-0.1.5/src/db/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/db/postgres/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.294226 crud_repository-0.1.5/src/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.294226 crud_repository-0.1.5/src/my_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/my_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/my_logger/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/my_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/my_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/my_logger/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:53.294226 crud_repository-0.1.5/src/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-30 20:50:45.000000 crud_repository-0.1.5/src/repo/repository.py
```

### Comparing `crud_repository-0.1.3/LICENSE` & `crud_repository-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/PKG-INFO` & `crud_repository-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.3
+Version: 0.1.5
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
```

### Comparing `crud_repository-0.1.3/PYPI.md` & `crud_repository-0.1.5/PYPI.md`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/README.md` & `crud_repository-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/crud_repository.egg-info/PKG-INFO` & `crud_repository-0.1.5/crud_repository.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.3
+Version: 0.1.5
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
```

### Comparing `crud_repository-0.1.3/crud_repository.egg-info/SOURCES.txt` & `crud_repository-0.1.5/crud_repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/pyproject.toml` & `crud_repository-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crud_repository"
-version = "0.1.3"
+version = "0.1.5"
 description = "The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases."
 authors = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"},
   {email = "info@hyfisolutions.com"},
 ]
 maintainers = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"}
```

### Comparing `crud_repository-0.1.3/setup.py` & `crud_repository-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/__config__.py` & `crud_repository-0.1.5/src/__config__.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/db/factory.py` & `crud_repository-0.1.5/src/db/factory.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/db/idatabase.py` & `crud_repository-0.1.5/src/db/idatabase.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/db/mariadb/db.py` & `crud_repository-0.1.5/src/db/mariadb/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/db/mysql/db.py` & `crud_repository-0.1.5/src/db/mysql/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/db/postgres/db.py` & `crud_repository-0.1.5/src/db/postgres/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/my_logger/formatters.py` & `crud_repository-0.1.5/src/my_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/my_logger/handlers.py` & `crud_repository-0.1.5/src/my_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/my_logger/logger.py` & `crud_repository-0.1.5/src/my_logger/logger.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/my_logger/monitor.py` & `crud_repository-0.1.5/src/my_logger/monitor.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.3/src/repo/repository.py` & `crud_repository-0.1.5/src/repo/repository.py`

 * *Files identical despite different names*

