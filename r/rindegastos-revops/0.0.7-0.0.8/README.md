# Comparing `tmp/rindegastos_revops-0.0.7.tar.gz` & `tmp/rindegastos_revops-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rindegastos_revops-0.0.7.tar", last modified: Thu Apr 25 17:02:11 2024, max compression
+gzip compressed data, was "rindegastos_revops-0.0.8.tar", last modified: Tue Apr 30 14:57:46 2024, max compression
```

## Comparing `rindegastos_revops-0.0.7.tar` & `rindegastos_revops-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.576367 rindegastos_revops-0.0.7/
--rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-25 17:02:11.576247 rindegastos_revops-0.0.7/PKG-INFO
--rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 14:06:12.000000 rindegastos_revops-0.0.7/README.md
--rw-r--r--   0 joseizam   (501) staff       (20)       86 2024-04-23 14:09:38.000000 rindegastos_revops-0.0.7/pyproject.toml
--rw-r--r--   0 joseizam   (501) staff       (20)      678 2024-04-25 17:02:11.576699 rindegastos_revops-0.0.7/setup.cfg
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.569960 rindegastos_revops-0.0.7/src/
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.571400 rindegastos_revops-0.0.7/src/rindegastos_revops/
--rw-r--r--   0 joseizam   (501) staff       (20)       26 2024-04-23 20:44:59.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/__init__.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.572436 rindegastos_revops-0.0.7/src/rindegastos_revops/data_engineering/
--rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 19:00:35.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/data_engineering/__init__.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.572697 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/
--rw-r--r--   0 joseizam   (501) staff       (20)       47 2024-04-23 20:44:40.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/__init__.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.574001 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/
--rw-r--r--   0 joseizam   (501) staff       (20)      133 2024-04-24 14:22:46.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)      129 2024-04-23 16:54:01.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/dates.py
--rw-r--r--   0 joseizam   (501) staff       (20)      183 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/file_name.py
--rw-r--r--   0 joseizam   (501) staff       (20)      273 2024-04-24 19:30:42.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/get_dataframe.py
--rw-r--r--   0 joseizam   (501) staff       (20)      932 2024-04-25 15:39:09.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/hubspot.py
--rw-r--r--   0 joseizam   (501) staff       (20)     2025 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.574183 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/
--rw-r--r--   0 joseizam   (501) staff       (20)       36 2024-04-23 20:45:30.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/__init__.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.574532 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/companies/
--rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 20:43:33.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/companies/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)     1894 2024-04-25 16:56:52.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/companies/search.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.574837 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/contacts/
--rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 20:44:10.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/contacts/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)     1881 2024-04-25 16:57:00.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/contacts/search.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.575137 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/deals/
--rw-r--r--   0 joseizam   (501) staff       (20)       20 2024-04-25 15:13:41.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/deals/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)     1883 2024-04-25 16:57:12.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/deals/search.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.575468 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/tickets/
--rw-r--r--   0 joseizam   (501) staff       (20)       20 2024-04-25 15:38:33.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/tickets/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)     1889 2024-04-25 16:57:21.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/tickets/search.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.575772 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/properties/
--rw-r--r--   0 joseizam   (501) staff       (20)       23 2024-04-23 21:07:41.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/properties/__init__.py
--rw-r--r--   0 joseizam   (501) staff       (20)      800 2024-04-24 19:57:32.000000 rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/properties/read_all.py
-drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-25 17:02:11.575995 rindegastos_revops-0.0.7/src/rindegastos_revops.egg-info/
--rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-25 17:02:11.000000 rindegastos_revops-0.0.7/src/rindegastos_revops.egg-info/PKG-INFO
--rw-r--r--   0 joseizam   (501) staff       (20)     1410 2024-04-25 17:02:11.000000 rindegastos_revops-0.0.7/src/rindegastos_revops.egg-info/SOURCES.txt
--rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-25 17:02:11.000000 rindegastos_revops-0.0.7/src/rindegastos_revops.egg-info/dependency_links.txt
--rw-r--r--   0 joseizam   (501) staff       (20)       16 2024-04-25 17:02:11.000000 rindegastos_revops-0.0.7/src/rindegastos_revops.egg-info/requires.txt
--rw-r--r--   0 joseizam   (501) staff       (20)       19 2024-04-25 17:02:11.000000 rindegastos_revops-0.0.7/src/rindegastos_revops.egg-info/top_level.txt
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.903019 rindegastos_revops-0.0.8/
+-rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-30 14:57:46.902942 rindegastos_revops-0.0.8/PKG-INFO
+-rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 14:06:12.000000 rindegastos_revops-0.0.8/README.md
+-rw-r--r--   0 joseizam   (501) staff       (20)       86 2024-04-23 14:09:38.000000 rindegastos_revops-0.0.8/pyproject.toml
+-rw-r--r--   0 joseizam   (501) staff       (20)      678 2024-04-30 14:57:46.903384 rindegastos_revops-0.0.8/setup.cfg
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.892722 rindegastos_revops-0.0.8/src/
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.894130 rindegastos_revops-0.0.8/src/rindegastos_revops/
+-rw-r--r--   0 joseizam   (501) staff       (20)       26 2024-04-23 20:44:59.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.895932 rindegastos_revops-0.0.8/src/rindegastos_revops/data_engineering/
+-rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-23 19:00:35.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/data_engineering/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      458 2024-04-26 13:36:10.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/data_engineering/pandas_helpers.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.896490 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/
+-rw-r--r--   0 joseizam   (501) staff       (20)       47 2024-04-23 20:44:40.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.898728 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/
+-rw-r--r--   0 joseizam   (501) staff       (20)      133 2024-04-24 14:22:46.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      129 2024-04-23 16:54:01.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/dates.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      183 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/file_name.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      273 2024-04-24 19:30:42.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/get_dataframe.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1027 2024-04-30 14:14:54.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/hubspot.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     2025 2024-04-23 15:11:06.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.898969 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/
+-rw-r--r--   0 joseizam   (501) staff       (20)       36 2024-04-23 20:45:30.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/__init__.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.899675 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/companies/
+-rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 20:43:33.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/companies/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1894 2024-04-25 16:56:52.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/companies/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.900115 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/contacts/
+-rw-r--r--   0 joseizam   (501) staff       (20)       21 2024-04-23 20:44:10.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/contacts/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1881 2024-04-25 16:57:00.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/contacts/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.900921 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/deals/
+-rw-r--r--   0 joseizam   (501) staff       (20)       20 2024-04-25 15:13:41.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/deals/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1883 2024-04-25 16:57:12.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/deals/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.901391 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/tickets/
+-rw-r--r--   0 joseizam   (501) staff       (20)       20 2024-04-25 15:38:33.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/tickets/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)     1889 2024-04-25 16:57:21.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/tickets/search.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.901725 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/users/
+-rw-r--r--   0 joseizam   (501) staff       (20)        0 2024-04-30 13:22:22.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/users/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      710 2024-04-30 14:27:05.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/users/all.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.902273 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/properties/
+-rw-r--r--   0 joseizam   (501) staff       (20)       23 2024-04-23 21:07:41.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/properties/__init__.py
+-rw-r--r--   0 joseizam   (501) staff       (20)      800 2024-04-24 19:57:32.000000 rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/properties/read_all.py
+drwxr-xr-x   0 joseizam   (501) staff       (20)        0 2024-04-30 14:57:46.902670 rindegastos_revops-0.0.8/src/rindegastos_revops.egg-info/
+-rw-r--r--   0 joseizam   (501) staff       (20)      538 2024-04-30 14:57:46.000000 rindegastos_revops-0.0.8/src/rindegastos_revops.egg-info/PKG-INFO
+-rw-r--r--   0 joseizam   (501) staff       (20)     1585 2024-04-30 14:57:46.000000 rindegastos_revops-0.0.8/src/rindegastos_revops.egg-info/SOURCES.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)        1 2024-04-30 14:57:46.000000 rindegastos_revops-0.0.8/src/rindegastos_revops.egg-info/dependency_links.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)       16 2024-04-30 14:57:46.000000 rindegastos_revops-0.0.8/src/rindegastos_revops.egg-info/requires.txt
+-rw-r--r--   0 joseizam   (501) staff       (20)       19 2024-04-30 14:57:46.000000 rindegastos_revops-0.0.8/src/rindegastos_revops.egg-info/top_level.txt
```

### Comparing `rindegastos_revops-0.0.7/PKG-INFO` & `rindegastos_revops-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rindegastos_revops
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple sdk for revops packages
 Home-page: https://github.com/joigmz/rindegastos_revops
 Author: Jose Izam
 Author-email: jose.izam99@gmail.com
 Project-URL: Bug Tracker, https://github.com/joigmz/rindegastos_revops
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rindegastos_revops-0.0.7/setup.cfg` & `rindegastos_revops-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rindegastos_revops
-version = 0.0.7
+version = 0.0.8
 author = Jose Izam
 author_email = jose.izam99@gmail.com
 description = Simple sdk for revops packages
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/joigmz/rindegastos_revops
 project_urls =
```

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/hubspot.py` & `rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/hubspot.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,22 @@
     CONTACTS_SEARCH = "objects/contacts/search"
     # Companies
     COMPANIES_SEARCH = "objects/companies/search"
     # Deals
     DEALS_SEARCH = "objects/deals/search"
     # Tickets
     TICKETS_SEARCH = "objects/tickets/search"
+    # Users
+    USERS_ALL = "objects/users"
     # Properties
     PROPERTIES_CONTACTS_READ_ALL = "properties/contacts"
     PROPERTIES_COMPANIES_READ_ALL = "properties/companies"
     PROPERTIES_DEALS_READ_ALL = "properties/deals"
     PROPERTIES_TICKETS_READ_ALL = "properties/tickets"
+    PROPERTIES_USERS_READ_ALL = "properties/users"
 
 
 class HubspotConnectorApi:
     def __init__(self, hubspot_api_key):
         self.base_url = "https://api.hubapi.com/crm/v3"
 
         self.headers = {
```

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py` & `rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/helpers/properties_selection.py`

 * *Files identical despite different names*

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/companies/search.py` & `rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/companies/search.py`

 * *Files identical despite different names*

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/contacts/search.py` & `rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/contacts/search.py`

 * *Files identical despite different names*

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/deals/search.py` & `rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/deals/search.py`

 * *Files identical despite different names*

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/objects/tickets/search.py` & `rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/objects/tickets/search.py`

 * *Files identical despite different names*

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops/hubspot_api/properties/read_all.py` & `rindegastos_revops-0.0.8/src/rindegastos_revops/hubspot_api/properties/read_all.py`

 * *Files identical despite different names*

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops.egg-info/PKG-INFO` & `rindegastos_revops-0.0.8/src/rindegastos_revops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rindegastos_revops
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple sdk for revops packages
 Home-page: https://github.com/joigmz/rindegastos_revops
 Author: Jose Izam
 Author-email: jose.izam99@gmail.com
 Project-URL: Bug Tracker, https://github.com/joigmz/rindegastos_revops
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rindegastos_revops-0.0.7/src/rindegastos_revops.egg-info/SOURCES.txt` & `rindegastos_revops-0.0.8/src/rindegastos_revops.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/rindegastos_revops/__init__.py
 src/rindegastos_revops.egg-info/PKG-INFO
 src/rindegastos_revops.egg-info/SOURCES.txt
 src/rindegastos_revops.egg-info/dependency_links.txt
 src/rindegastos_revops.egg-info/requires.txt
 src/rindegastos_revops.egg-info/top_level.txt
 src/rindegastos_revops/data_engineering/__init__.py
+src/rindegastos_revops/data_engineering/pandas_helpers.py
 src/rindegastos_revops/hubspot_api/__init__.py
 src/rindegastos_revops/hubspot_api/helpers/__init__.py
 src/rindegastos_revops/hubspot_api/helpers/dates.py
 src/rindegastos_revops/hubspot_api/helpers/file_name.py
 src/rindegastos_revops/hubspot_api/helpers/get_dataframe.py
 src/rindegastos_revops/hubspot_api/helpers/hubspot.py
 src/rindegastos_revops/hubspot_api/helpers/properties_selection.py
@@ -20,9 +21,11 @@
 src/rindegastos_revops/hubspot_api/objects/companies/search.py
 src/rindegastos_revops/hubspot_api/objects/contacts/__init__.py
 src/rindegastos_revops/hubspot_api/objects/contacts/search.py
 src/rindegastos_revops/hubspot_api/objects/deals/__init__.py
 src/rindegastos_revops/hubspot_api/objects/deals/search.py
 src/rindegastos_revops/hubspot_api/objects/tickets/__init__.py
 src/rindegastos_revops/hubspot_api/objects/tickets/search.py
+src/rindegastos_revops/hubspot_api/objects/users/__init__.py
+src/rindegastos_revops/hubspot_api/objects/users/all.py
 src/rindegastos_revops/hubspot_api/properties/__init__.py
 src/rindegastos_revops/hubspot_api/properties/read_all.py
```

