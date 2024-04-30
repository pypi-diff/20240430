# Comparing `tmp/snakemake_storage_plugin_sharepoint-0.2.3.tar.gz` & `tmp/snakemake_storage_plugin_sharepoint-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_sharepoint-0.2.3.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_sharepoint-0.2.4.tar", max compression
```

## Comparing `snakemake_storage_plugin_sharepoint-0.2.3.tar` & `snakemake_storage_plugin_sharepoint-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1058 2024-04-29 19:13:59.807533 snakemake_storage_plugin_sharepoint-0.2.3/LICENSE
--rw-r--r--   0        0        0      119 2024-04-29 19:13:59.807533 snakemake_storage_plugin_sharepoint-0.2.3/README.md
--rw-r--r--   0        0        0      958 2024-04-29 19:13:59.807533 snakemake_storage_plugin_sharepoint-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      322 2024-04-29 19:13:59.807533 snakemake_storage_plugin_sharepoint-0.2.3/snakemake_storage_plugin_sharepoint/__init__.py
--rw-r--r--   0        0        0     6810 2024-04-29 19:13:59.807533 snakemake_storage_plugin_sharepoint-0.2.3/snakemake_storage_plugin_sharepoint/object.py
--rw-r--r--   0        0        0     2561 2024-04-29 19:13:59.807533 snakemake_storage_plugin_sharepoint-0.2.3/snakemake_storage_plugin_sharepoint/provider.py
--rw-r--r--   0        0        0     4367 2024-04-29 19:13:59.807533 snakemake_storage_plugin_sharepoint-0.2.3/snakemake_storage_plugin_sharepoint/settings.py
--rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 snakemake_storage_plugin_sharepoint-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/LICENSE
+-rw-r--r--   0        0        0      119 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/README.md
+-rw-r--r--   0        0        0      958 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      322 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/__init__.py
+-rw-r--r--   0        0        0     6810 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/object.py
+-rw-r--r--   0        0        0     2561 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/provider.py
+-rw-r--r--   0        0        0     4367 2024-04-30 20:32:51.687547 snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/settings.py
+-rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 snakemake_storage_plugin_sharepoint-0.2.4/PKG-INFO
```

### Comparing `snakemake_storage_plugin_sharepoint-0.2.3/LICENSE` & `snakemake_storage_plugin_sharepoint-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_sharepoint-0.2.3/pyproject.toml` & `snakemake_storage_plugin_sharepoint-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-storage-plugin-sharepoint"
-version = "0.2.3"
+version = "0.2.4"
 description = "Snakemake storage plugin for reading and writing files on Microsoft SharePoint."
 authors = [
     "Hugo Lapre <hugo.lapre@brabantwater.nl>",
 ]
 readme = "README.md"
 repository = "https://github.com/Hugovdberg/snakemake-storage-plugin-sharepoint"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/sharepoint.html"
```

### Comparing `snakemake_storage_plugin_sharepoint-0.2.3/snakemake_storage_plugin_sharepoint/object.py` & `snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/object.py`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_sharepoint-0.2.3/snakemake_storage_plugin_sharepoint/provider.py` & `snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/provider.py`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_sharepoint-0.2.3/snakemake_storage_plugin_sharepoint/settings.py` & `snakemake_storage_plugin_sharepoint-0.2.4/snakemake_storage_plugin_sharepoint/settings.py`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_sharepoint-0.2.3/PKG-INFO` & `snakemake_storage_plugin_sharepoint-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-storage-plugin-sharepoint
-Version: 0.2.3
+Version: 0.2.4
 Summary: Snakemake storage plugin for reading and writing files on Microsoft SharePoint.
 Home-page: https://github.com/Hugovdberg/snakemake-storage-plugin-sharepoint
 License: MIT
 Keywords: snakemake,plugin,storage,sharepoint
 Author: Hugo Lapre
 Author-email: hugo.lapre@brabantwater.nl
 Requires-Python: >=3.11,<4.0
```

