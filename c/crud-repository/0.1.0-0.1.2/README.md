# Comparing `tmp/crud_repository-0.1.0.tar.gz` & `tmp/crud_repository-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crud_repository-0.1.0.tar", last modified: Tue Apr 30 18:56:45 2024, max compression
+gzip compressed data, was "crud_repository-0.1.2.tar", last modified: Tue Apr 30 19:20:33 2024, max compression
```

## Comparing `crud_repository-0.1.0.tar` & `crud_repository-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.572821 crud_repository-0.1.0/
--rw-r--r--   0 dalexander   (501) staff       (20)     1073 2024-04-12 07:44:52.000000 crud_repository-0.1.0/LICENSE
--rw-r--r--   0 dalexander   (501) staff       (20)      293 2024-04-30 09:31:25.000000 crud_repository-0.1.0/MANIFEST.in
--rw-r--r--   0 dalexander   (501) staff       (20)    14488 2024-04-30 18:56:45.572533 crud_repository-0.1.0/PKG-INFO
--rw-r--r--   0 dalexander   (501) staff       (20)    11941 2024-04-30 05:34:15.000000 crud_repository-0.1.0/README.md
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.571686 crud_repository-0.1.0/crud_repository.egg-info/
--rw-r--r--   0 dalexander   (501) staff       (20)    14488 2024-04-30 18:56:45.000000 crud_repository-0.1.0/crud_repository.egg-info/PKG-INFO
--rw-r--r--   0 dalexander   (501) staff       (20)      741 2024-04-30 18:56:45.000000 crud_repository-0.1.0/crud_repository.egg-info/SOURCES.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 18:56:45.000000 crud_repository-0.1.0/crud_repository.egg-info/dependency_links.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 16:58:54.000000 crud_repository-0.1.0/crud_repository.egg-info/not-zip-safe
--rw-r--r--   0 dalexander   (501) staff       (20)      140 2024-04-30 18:56:45.000000 crud_repository-0.1.0/crud_repository.egg-info/requires.txt
--rw-r--r--   0 dalexander   (501) staff       (20)        4 2024-04-30 18:56:45.000000 crud_repository-0.1.0/crud_repository.egg-info/top_level.txt
--rw-r--r--   0 dalexander   (501) staff       (20)     1445 2024-04-30 16:58:44.000000 crud_repository-0.1.0/pyproject.toml
--rw-r--r--   0 dalexander   (501) staff       (20)      281 2024-04-30 18:56:45.573673 crud_repository-0.1.0/setup.cfg
--rw-r--r--   0 dalexander   (501) staff       (20)      850 2024-04-30 18:56:22.000000 crud_repository-0.1.0/setup.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.561000 crud_repository-0.1.0/src/
--rw-r--r--   0 dalexander   (501) staff       (20)     3194 2024-04-30 01:09:48.000000 crud_repository-0.1.0/src/__config__.py
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-30 01:00:42.000000 crud_repository-0.1.0/src/__init__.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.562212 crud_repository-0.1.0/src/db/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-09 20:51:28.000000 crud_repository-0.1.0/src/db/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2129 2024-04-24 16:01:46.000000 crud_repository-0.1.0/src/db/factory.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1415 2024-04-24 01:01:37.000000 crud_repository-0.1.0/src/db/idatabase.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.563352 crud_repository-0.1.0/src/db/mariadb/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:13.000000 crud_repository-0.1.0/src/db/mariadb/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2510 2024-04-30 00:14:45.000000 crud_repository-0.1.0/src/db/mariadb/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.564272 crud_repository-0.1.0/src/db/mysql/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:26.000000 crud_repository-0.1.0/src/db/mysql/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2279 2024-04-30 00:14:45.000000 crud_repository-0.1.0/src/db/mysql/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.565215 crud_repository-0.1.0/src/db/postgres/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:03.000000 crud_repository-0.1.0/src/db/postgres/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1877 2024-04-30 00:14:45.000000 crud_repository-0.1.0/src/db/postgres/db.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.566241 crud_repository-0.1.0/src/model/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 17:00:08.000000 crud_repository-0.1.0/src/model/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)      190 2024-04-09 20:58:35.000000 crud_repository-0.1.0/src/model/base.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.569425 crud_repository-0.1.0/src/my_logger/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-15 08:17:30.000000 crud_repository-0.1.0/src/my_logger/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1973 2024-04-24 22:03:32.000000 crud_repository-0.1.0/src/my_logger/formatters.py
--rw-r--r--   0 dalexander   (501) staff       (20)     5131 2024-04-24 22:03:32.000000 crud_repository-0.1.0/src/my_logger/handlers.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1742 2024-04-26 00:51:10.000000 crud_repository-0.1.0/src/my_logger/logger.py
--rw-r--r--   0 dalexander   (501) staff       (20)     1515 2024-04-24 22:03:32.000000 crud_repository-0.1.0/src/my_logger/monitor.py
-drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 18:56:45.570685 crud_repository-0.1.0/src/repo/
--rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 03:50:05.000000 crud_repository-0.1.0/src/repo/__init__.py
--rw-r--r--   0 dalexander   (501) staff       (20)     2953 2024-04-29 23:49:54.000000 crud_repository-0.1.0/src/repo/repository.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.205770 crud_repository-0.1.2/
+-rw-r--r--   0 dalexander   (501) staff       (20)     1073 2024-04-12 07:44:52.000000 crud_repository-0.1.2/LICENSE
+-rw-r--r--   0 dalexander   (501) staff       (20)      293 2024-04-30 09:31:25.000000 crud_repository-0.1.2/MANIFEST.in
+-rw-r--r--   0 dalexander   (501) staff       (20)     6684 2024-04-30 19:20:33.205578 crud_repository-0.1.2/PKG-INFO
+-rw-r--r--   0 dalexander   (501) staff       (20)     4137 2024-04-30 19:06:00.000000 crud_repository-0.1.2/PYPI.md
+-rw-r--r--   0 dalexander   (501) staff       (20)    11941 2024-04-30 05:34:15.000000 crud_repository-0.1.2/README.md
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.204522 crud_repository-0.1.2/crud_repository.egg-info/
+-rw-r--r--   0 dalexander   (501) staff       (20)     6684 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/PKG-INFO
+-rw-r--r--   0 dalexander   (501) staff       (20)      749 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 dalexander   (501) staff       (20)        1 2024-04-30 19:13:57.000000 crud_repository-0.1.2/crud_repository.egg-info/not-zip-safe
+-rw-r--r--   0 dalexander   (501) staff       (20)      140 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/requires.txt
+-rw-r--r--   0 dalexander   (501) staff       (20)        4 2024-04-30 19:20:33.000000 crud_repository-0.1.2/crud_repository.egg-info/top_level.txt
+-rw-r--r--   0 dalexander   (501) staff       (20)     1443 2024-04-30 19:17:44.000000 crud_repository-0.1.2/pyproject.toml
+-rw-r--r--   0 dalexander   (501) staff       (20)      281 2024-04-30 19:20:33.206565 crud_repository-0.1.2/setup.cfg
+-rw-r--r--   0 dalexander   (501) staff       (20)      818 2024-04-30 19:20:19.000000 crud_repository-0.1.2/setup.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.186556 crud_repository-0.1.2/src/
+-rw-r--r--   0 dalexander   (501) staff       (20)     3194 2024-04-30 01:09:48.000000 crud_repository-0.1.2/src/__config__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-30 01:00:42.000000 crud_repository-0.1.2/src/__init__.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.188488 crud_repository-0.1.2/src/db/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-09 20:51:28.000000 crud_repository-0.1.2/src/db/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     2129 2024-04-24 16:01:46.000000 crud_repository-0.1.2/src/db/factory.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1415 2024-04-24 01:01:37.000000 crud_repository-0.1.2/src/db/idatabase.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.189857 crud_repository-0.1.2/src/db/mariadb/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:13.000000 crud_repository-0.1.2/src/db/mariadb/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     2510 2024-04-30 00:14:45.000000 crud_repository-0.1.2/src/db/mariadb/db.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.191341 crud_repository-0.1.2/src/db/mysql/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:26.000000 crud_repository-0.1.2/src/db/mysql/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     2279 2024-04-30 00:14:45.000000 crud_repository-0.1.2/src/db/mysql/db.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.193518 crud_repository-0.1.2/src/db/postgres/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-13 19:42:03.000000 crud_repository-0.1.2/src/db/postgres/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1877 2024-04-30 00:14:45.000000 crud_repository-0.1.2/src/db/postgres/db.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.196282 crud_repository-0.1.2/src/model/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 17:00:08.000000 crud_repository-0.1.2/src/model/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)      190 2024-04-09 20:58:35.000000 crud_repository-0.1.2/src/model/base.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.201662 crud_repository-0.1.2/src/my_logger/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-04-15 08:17:30.000000 crud_repository-0.1.2/src/my_logger/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1973 2024-04-24 22:03:32.000000 crud_repository-0.1.2/src/my_logger/formatters.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     5131 2024-04-24 22:03:32.000000 crud_repository-0.1.2/src/my_logger/handlers.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1742 2024-04-26 00:51:10.000000 crud_repository-0.1.2/src/my_logger/logger.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     1515 2024-04-24 22:03:32.000000 crud_repository-0.1.2/src/my_logger/monitor.py
+drwxr-xr-x   0 dalexander   (501) staff       (20)        0 2024-04-30 19:20:33.203281 crud_repository-0.1.2/src/repo/
+-rw-r--r--   0 dalexander   (501) staff       (20)        0 2024-03-29 03:50:05.000000 crud_repository-0.1.2/src/repo/__init__.py
+-rw-r--r--   0 dalexander   (501) staff       (20)     2953 2024-04-29 23:49:54.000000 crud_repository-0.1.2/src/repo/repository.py
```

### Comparing `crud_repository-0.1.0/LICENSE` & `crud_repository-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/PKG-INFO` & `crud_repository-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,7 @@
-Metadata-Version: 2.1
-Name: crud_repository
-Version: 0.1.0
-Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
-Home-page: https://github.com/dellius-alexander/CRUDRepository.git
-Author: Dellius Alexander
-Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
-Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
-License: MIT License
-        
-        Copyright (c) 2024 Dellius Alexander
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/dellius-alexander/CRUDRepository.git
-Keywords: crud-repository,database,model,abstraction
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: sqlalchemy>=2.0.29
-Requires-Dist: psycopg2-binary>=2.9.9
-Requires-Dist: python-dotenv>=1.0.1
-Requires-Dist: colorlog>=6.4.1
-Requires-Dist: cryptography>=42.0.5
-Requires-Dist: pymysql>=1.1.0
-Requires-Dist: SQLAlchemy-Utils>=0.41.2
-
 [![Build test and deploy to package repository](https://github.com/dellius-alexander/CRUDRepository/actions/workflows/deploy.yml/badge.svg?branch=main)](https://github.com/dellius-alexander/CRUDRepository/actions/workflows/deploy.yml)
 
 ---
 
 # CRUD Repository
 
 ---
```

### Comparing `crud_repository-0.1.0/crud_repository.egg-info/SOURCES.txt` & `crud_repository-0.1.2/crud_repository.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 MANIFEST.in
+PYPI.md
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 crud_repository.egg-info/PKG-INFO
 crud_repository.egg-info/SOURCES.txt
 crud_repository.egg-info/dependency_links.txt
```

### Comparing `crud_repository-0.1.0/pyproject.toml` & `crud_repository-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crud_repository"
-version = "0.1.0"
+version = "0.1.2"
 description = "The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases."
 authors = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"},
   {email = "info@hyfisolutions.com"},
 ]
 maintainers = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"}
 ]
-readme = {file = "README.md", content-type = "text/markdown"}
+readme = {file = "PYPI.md", content-type = "text/markdown"}
 keywords = ["crud-repository", "database", "model", "abstraction"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

### Comparing `crud_repository-0.1.0/setup.py` & `crud_repository-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """
 This module is used for packaging the CRUDRepository project.
 """
-import os
-
 from setuptools import setup, find_packages
 from pathlib import Path
 
 # --------------------------------------------------------------
 setup(
     name="crud_repository",
-    version="0.1.3",
     url="https://github.com/dellius-alexander/CRUDRepository.git",
     author="Dellius Alexander",
     author_email="dalexander@hyfisolutions.com",
     description="The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.",
     packages=find_packages(
         exclude=["tests", "*.tests", "*.tests.*", "tests.*", "dist", "build", "logs"]
     ),
```

### Comparing `crud_repository-0.1.0/src/__config__.py` & `crud_repository-0.1.2/src/__config__.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/db/factory.py` & `crud_repository-0.1.2/src/db/factory.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/db/idatabase.py` & `crud_repository-0.1.2/src/db/idatabase.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/db/mariadb/db.py` & `crud_repository-0.1.2/src/db/mariadb/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/db/mysql/db.py` & `crud_repository-0.1.2/src/db/mysql/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/db/postgres/db.py` & `crud_repository-0.1.2/src/db/postgres/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/my_logger/formatters.py` & `crud_repository-0.1.2/src/my_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/my_logger/handlers.py` & `crud_repository-0.1.2/src/my_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/my_logger/logger.py` & `crud_repository-0.1.2/src/my_logger/logger.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/my_logger/monitor.py` & `crud_repository-0.1.2/src/my_logger/monitor.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.0/src/repo/repository.py` & `crud_repository-0.1.2/src/repo/repository.py`

 * *Files identical despite different names*

