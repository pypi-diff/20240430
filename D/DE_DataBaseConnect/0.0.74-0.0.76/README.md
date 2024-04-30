# Comparing `tmp/DE_DataBaseConnect-0.0.74.tar.gz` & `tmp/de_databaseconnect-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DE_DataBaseConnect-0.0.74.tar", last modified: Wed May 31 17:22:04 2023, max compression
+gzip compressed data, was "de_databaseconnect-0.0.76.tar", max compression
```

## Comparing `DE_DataBaseConnect-0.0.74.tar` & `de_databaseconnect-0.0.76.tar`

### file list

```diff
@@ -1,12 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 17:22:04.553067 DE_DataBaseConnect-0.0.74/
--rw-rw-rw-   0        0        0    17270 2023-05-31 17:21:53.000000 DE_DataBaseConnect-0.0.74/DE_DataBase.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:22:04.540102 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-31 17:22:03.000000 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-31 17:22:03.000000 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 17:22:03.000000 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 17:22:03.000000 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.74/Licence.txt
--rw-rw-rw-   0        0        0      307 2023-05-31 17:22:04.553067 DE_DataBaseConnect-0.0.74/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.74/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 17:22:04.562044 DE_DataBaseConnect-0.0.74/setup.cfg
--rw-rw-rw-   0        0        0      327 2023-05-31 17:21:59.000000 DE_DataBaseConnect-0.0.74/setup.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:24:30.466226 de_databaseconnect-0.0.76/DE_DataBaseConnect/de_databaseconnect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:24:30.473208 de_databaseconnect-0.0.76/DE_DataBaseConnect/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 18:24:30.479194 de_databaseconnect-0.0.76/DE_DataBaseConnect/tests/__init__.py
+-rw-r--r--   0        0        0     1088 2022-08-23 21:32:43.000000 de_databaseconnect-0.0.76/Licence.txt
+-rw-r--r--   0        0        0      292 2024-04-30 18:28:26.382612 de_databaseconnect-0.0.76/pyproject.toml
+-rw-r--r--   0        0        0      829 2022-08-23 21:32:43.000000 de_databaseconnect-0.0.76/README.md
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 de_databaseconnect-0.0.76/PKG-INFO
```

### Comparing `DE_DataBaseConnect-0.0.74/Licence.txt` & `de_databaseconnect-0.0.76/Licence.txt`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.74/README.md` & `de_databaseconnect-0.0.76/README.md`

 * *Files identical despite different names*

