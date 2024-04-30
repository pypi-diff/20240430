# Comparing `tmp/crud_repository-0.1.2.tar.gz` & `tmp/crud_repository-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crud_repository-0.1.2.tar", last modified: Tue Apr 30 19:20:33 2024, max compression
+gzip compressed data, was "crud_repository-0.1.3.tar", last modified: Tue Apr 30 19:23:47 2024, max compression
```

## Comparing `crud_repository-0.1.2.tar` & `crud_repository-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.205770 crud_repository-0.1.2/
--rw-r--r--   0 dalexander   (501) staff       (20)     1073 2024-04-12 07:44:52.000000 crud_repository-0.1.2/LICENSE
--rw-r--r--   0 dalexander   (501) staff       (20)      293 2024-04-30 09:31:25.000000 crud_repository-0.1.2/MANIFEST.in
--rw-r--r--   0 dalexander   (501) staff       (20)     6684 2024-04-30 19:20:33.205578 crud_repository-0.1.2/PKG-INFO
--rw-r--r--   0 dalexander   (501) staff       (20)     4137 2024-04-30 19:06:00.000000 crud_repository-0.1.2/PYPI.md
--rw-r--r--   0 dalexander   (501) staff       (20)    11941 2024-04-30 05:34:15.000000 crud_repository-0.1.2/README.md
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.204522 crud_repository-0.1.2/crud_repository.egg-info/
--rw-r--r--   0 dalexander   (501) staff       (20)     6684 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/PKG-INFO
--rw-r--r--   0 dalexander   (501) staff       (20)      749 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/SOURCES.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/dependency_links.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 19:13:57.000000 crud_repository-0.1.2/crud_repository.egg-info/not-zip-safe
--rw-r--r--   0 dalexander   (501) staff       (20)      140 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/requires.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        4 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/top_level.txt
--rw-r--r--   0 dalexander   (501) staff       (20)     1443 2024-04-30 19:17:44.000000 crud_repository-0.1.2/pyproject.toml
--rw-r--r--   0 dalexander   (501) staff       (20)      281 2024-04-30 19:20:33.206565 crud_repository-0.1.2/setup.cfg
--rw-r--r--   0 dalexander   (501) staff       (20)      818 2024-04-30 19:20:19.000000 crud_repository-0.1.2/setup.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.186556 crud_repository-0.1.2/src/
--rw-r--r--   0 dalexander   (501) staff       (20)     3194 2024-04-30 01:09:48.000000 crud_repository-0.1.2/src/__config__.py
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-30 01:00:42.000000 crud_repository-0.1.2/src/__init__.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.188488 crud_repository-0.1.2/src/db/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-09 20:51:28.000000 crud_repository-0.1.2/src/db/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2129 2024-04-24 16:01:46.000000 crud_repository-0.1.2/src/db/factory.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1415 2024-04-24 01:01:37.000000 crud_repository-0.1.2/src/db/idatabase.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.189857 crud_repository-0.1.2/src/db/mariadb/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:13.000000 crud_repository-0.1.2/src/db/mariadb/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2510 2024-04-30 00:14:45.000000 crud_repository-0.1.2/src/db/mariadb/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.191341 crud_repository-0.1.2/src/db/mysql/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:26.000000 crud_repository-0.1.2/src/db/mysql/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2279 2024-04-30 00:14:45.000000 crud_repository-0.1.2/src/db/mysql/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.193518 crud_repository-0.1.2/src/db/postgres/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:03.000000 crud_repository-0.1.2/src/db/postgres/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1877 2024-04-30 00:14:45.000000 crud_repository-0.1.2/src/db/postgres/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.196282 crud_repository-0.1.2/src/model/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 17:00:08.000000 crud_repository-0.1.2/src/model/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)      190 2024-04-09 20:58:35.000000 crud_repository-0.1.2/src/model/base.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.201662 crud_repository-0.1.2/src/my_logger/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-15 08:17:30.000000 crud_repository-0.1.2/src/my_logger/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1973 2024-04-24 22:03:32.000000 crud_repository-0.1.2/src/my_logger/formatters.py
--rw-r--r--   0 dalexander   (501) staff       (20)     5131 2024-04-24 22:03:32.000000 crud_repository-0.1.2/src/my_logger/handlers.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1742 2024-04-26 00:51:10.000000 crud_repository-0.1.2/src/my_logger/logger.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1515 2024-04-24 22:03:32.000000 crud_repository-0.1.2/src/my_logger/monitor.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.203281 crud_repository-0.1.2/src/repo/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 03:50:05.000000 crud_repository-0.1.2/src/repo/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2953 2024-04-29 23:49:54.000000 crud_repository-0.1.2/src/repo/repository.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.397499 crud_repository-0.1.3/
+-rw-r--r--   0 dalexander   (501) staff       (20)     1073 2024-04-12 07:44:52.000000 crud_repository-0.1.3/LICENSE
+-rw-r--r--   0 dalexander   (501) staff       (20)      293 2024-04-30 09:31:25.000000 crud_repository-0.1.3/MANIFEST.in
+-rw-r--r--   0 dalexander   (501) staff       (20)     6746 2024-04-30 19:23:47.397264 crud_repository-0.1.3/PKG-INFO
+-rw-r--r--   0 dalexander   (501) staff       (20)     4199 2024-04-30 19:23:29.000000 crud_repository-0.1.3/PYPI.md
+-rw-r--r--   0 dalexander   (501) staff       (20)    12003 2024-04-30 19:23:29.000000 crud_repository-0.1.3/README.md
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.396369 crud_repository-0.1.3/crud_repository.egg-info/
+-rw-r--r--   0 dalexander   (501) staff       (20)     6746 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/PKG-INFO
+-rw-r--r--   0 dalexander   (501) staff       (20)      749 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 19:13:57.000000 crud_repository-0.1.3/crud_repository.egg-info/not-zip-safe
+-rw-r--r--   0 dalexander   (501) staff       (20)      140 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/requires.txt
+-rw-r--r--   0 dalexander   (501) staff       (20)        4 2024-04-30 19:23:47.000000 crud_repository-0.1.3/crud_repository.egg-info/top_level.txt
+-rw-r--r--   0 dalexander   (501) staff       (20)     1443 2024-04-30 19:23:29.000000 crud_repository-0.1.3/pyproject.toml
+-rw-r--r--   0 dalexander   (501) staff       (20)      281 2024-04-30 19:23:47.398157 crud_repository-0.1.3/setup.cfg
+-rw-r--r--   0 dalexander   (501) staff       (20)      818 2024-04-30 19:20:19.000000 crud_repository-0.1.3/setup.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.383691 crud_repository-0.1.3/src/
+-rw-r--r--   0 dalexander   (501) staff       (20)     3194 2024-04-30 01:09:48.000000 crud_repository-0.1.3/src/__config__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-30 01:00:42.000000 crud_repository-0.1.3/src/__init__.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.385470 crud_repository-0.1.3/src/db/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-09 20:51:28.000000 crud_repository-0.1.3/src/db/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     2129 2024-04-24 16:01:46.000000 crud_repository-0.1.3/src/db/factory.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1415 2024-04-24 01:01:37.000000 crud_repository-0.1.3/src/db/idatabase.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.386750 crud_repository-0.1.3/src/db/mariadb/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:13.000000 crud_repository-0.1.3/src/db/mariadb/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     2510 2024-04-30 00:14:45.000000 crud_repository-0.1.3/src/db/mariadb/db.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.388035 crud_repository-0.1.3/src/db/mysql/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:26.000000 crud_repository-0.1.3/src/db/mysql/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     2279 2024-04-30 00:14:45.000000 crud_repository-0.1.3/src/db/mysql/db.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.389118 crud_repository-0.1.3/src/db/postgres/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:03.000000 crud_repository-0.1.3/src/db/postgres/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1877 2024-04-30 00:14:45.000000 crud_repository-0.1.3/src/db/postgres/db.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.390365 crud_repository-0.1.3/src/model/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 17:00:08.000000 crud_repository-0.1.3/src/model/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)      190 2024-04-09 20:58:35.000000 crud_repository-0.1.3/src/model/base.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.393981 crud_repository-0.1.3/src/my_logger/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-15 08:17:30.000000 crud_repository-0.1.3/src/my_logger/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1973 2024-04-24 22:03:32.000000 crud_repository-0.1.3/src/my_logger/formatters.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     5131 2024-04-24 22:03:32.000000 crud_repository-0.1.3/src/my_logger/handlers.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1742 2024-04-26 00:51:10.000000 crud_repository-0.1.3/src/my_logger/logger.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1515 2024-04-24 22:03:32.000000 crud_repository-0.1.3/src/my_logger/monitor.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:23:47.395210 crud_repository-0.1.3/src/repo/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 03:50:05.000000 crud_repository-0.1.3/src/repo/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     2953 2024-04-29 23:49:54.000000 crud_repository-0.1.3/src/repo/repository.py
```

### Comparing `crud_repository-0.1.2/LICENSE` & `crud_repository-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/PKG-INFO` & `crud_repository-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.2
+Version: 0.1.3
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
         
@@ -81,14 +81,20 @@
 In summary, CRUDRepository is a flexible and extensible 
 foundation for Python applications that require database interactions, 
 abstracting the complexities of direct database access and providing a 
 clear and simple interface for performing CRUD operations.
 
 ---
 
+## Installation
+    
+```bash
+pip install crud-repository
+```
+
 ## Code Example Usage
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from src.db.factory import DatabaseFactory
 from typing import Optional
```

### Comparing `crud_repository-0.1.2/PYPI.md` & `crud_repository-0.1.3/PYPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 In summary, CRUDRepository is a flexible and extensible 
 foundation for Python applications that require database interactions, 
 abstracting the complexities of direct database access and providing a 
 clear and simple interface for performing CRUD operations.
 
 ---
 
+## Installation
+    
+```bash
+pip install crud-repository
+```
+
 ## Code Example Usage
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from src.db.factory import DatabaseFactory
 from typing import Optional
```

### Comparing `crud_repository-0.1.2/README.md` & `crud_repository-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,20 @@
 gets a session from the `DatabaseFactory` which creates an instance of either `PostgreSQLDatabase`, 
 `MySQLDatabase`, or `MariaDBDatabase` based on the provided configuration. The `Repository` 
 then performs the operation on the user in the session, and commits the session. The result 
 of the operation is then returned to the client.
 
 ---
 
+## Installation
+    
+```bash
+pip install crud-repository
+```
+
 ## Code Example Usage
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from src.db.factory import DatabaseFactory
 from typing import Optional
```

### Comparing `crud_repository-0.1.2/crud_repository.egg-info/PKG-INFO` & `crud_repository-0.1.3/crud_repository.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.2
+Version: 0.1.3
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
         
@@ -81,14 +81,20 @@
 In summary, CRUDRepository is a flexible and extensible 
 foundation for Python applications that require database interactions, 
 abstracting the complexities of direct database access and providing a 
 clear and simple interface for performing CRUD operations.
 
 ---
 
+## Installation
+    
+```bash
+pip install crud-repository
+```
+
 ## Code Example Usage
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from src.db.factory import DatabaseFactory
 from typing import Optional
```

### Comparing `crud_repository-0.1.2/crud_repository.egg-info/SOURCES.txt` & `crud_repository-0.1.3/crud_repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/pyproject.toml` & `crud_repository-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crud_repository"
-version = "0.1.2"
+version = "0.1.3"
 description = "The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases."
 authors = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"},
   {email = "info@hyfisolutions.com"},
 ]
 maintainers = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"}
```

### Comparing `crud_repository-0.1.2/setup.py` & `crud_repository-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/__config__.py` & `crud_repository-0.1.3/src/__config__.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/db/factory.py` & `crud_repository-0.1.3/src/db/factory.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/db/idatabase.py` & `crud_repository-0.1.3/src/db/idatabase.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/db/mariadb/db.py` & `crud_repository-0.1.3/src/db/mariadb/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/db/mysql/db.py` & `crud_repository-0.1.3/src/db/mysql/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/db/postgres/db.py` & `crud_repository-0.1.3/src/db/postgres/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/my_logger/formatters.py` & `crud_repository-0.1.3/src/my_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/my_logger/handlers.py` & `crud_repository-0.1.3/src/my_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/my_logger/logger.py` & `crud_repository-0.1.3/src/my_logger/logger.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/my_logger/monitor.py` & `crud_repository-0.1.3/src/my_logger/monitor.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.2/src/repo/repository.py` & `crud_repository-0.1.3/src/repo/repository.py`

 * *Files identical despite different names*

