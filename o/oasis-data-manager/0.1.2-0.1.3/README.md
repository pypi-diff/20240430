# Comparing `tmp/oasis-data-manager-0.1.2.tar.gz` & `tmp/oasis-data-manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasis-data-manager-0.1.2.tar", last modified: Thu Feb 29 14:26:36 2024, max compression
+gzip compressed data, was "oasis-data-manager-0.1.3.tar", last modified: Tue Apr 30 15:02:46 2024, max compression
```

## Comparing `oasis-data-manager-0.1.2.tar` & `oasis-data-manager-0.1.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.976858 oasis-data-manager-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-29 14:26:36.976858 oasis-data-manager-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.972858 oasis-data-manager-0.1.2/oasis_data_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.972858 oasis-data-manager-0.1.2/oasis_data_manager/complex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/complex/complex.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1220 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/complex/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.972858 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.972858 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/backends/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/backends/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/df_reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.972858 oasis-data-manager-0.1.2/oasis_data_manager/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.972858 oasis-data-manager-0.1.2/oasis_data_manager/filestore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.976858 oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10587 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/aws_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5354 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/azure_abfs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12971 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1242 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/filestore.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/oasis_data_manager/filestore/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:26:36.972858 oasis-data-manager-0.1.2/oasis_data_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-29 14:26:36.000000 oasis-data-manager-0.1.2/oasis_data_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-02-29 14:26:36.000000 oasis-data-manager-0.1.2/oasis_data_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 14:26:36.000000 oasis-data-manager-0.1.2/oasis_data_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-29 14:26:36.000000 oasis-data-manager-0.1.2/oasis_data_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-29 14:26:36.000000 oasis-data-manager-0.1.2/oasis_data_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/requirements-package.in
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-29 14:26:36.976858 oasis-data-manager-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-29 14:26:30.000000 oasis-data-manager-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.682872 oasis-data-manager-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-30 15:02:46.682872 oasis-data-manager-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.678872 oasis-data-manager-0.1.3/oasis_data_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.678872 oasis-data-manager-0.1.3/oasis_data_manager/complex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/complex/complex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1220 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/complex/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.682872 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.682872 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/backends/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/backends/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/df_reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.682872 oasis-data-manager-0.1.3/oasis_data_manager/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.682872 oasis-data-manager-0.1.3/oasis_data_manager/filestore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.682872 oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10636 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/aws_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5354 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/azure_abfs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13597 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1242 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/filestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/oasis_data_manager/filestore/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:02:46.678872 oasis-data-manager-0.1.3/oasis_data_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-30 15:02:46.000000 oasis-data-manager-0.1.3/oasis_data_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 15:02:46.000000 oasis-data-manager-0.1.3/oasis_data_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:02:46.000000 oasis-data-manager-0.1.3/oasis_data_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 15:02:46.000000 oasis-data-manager-0.1.3/oasis_data_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 15:02:46.000000 oasis-data-manager-0.1.3/oasis_data_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/requirements-package.in
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 15:02:46.682872 oasis-data-manager-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-30 15:02:44.000000 oasis-data-manager-0.1.3/setup.py
```

### Comparing `oasis-data-manager-0.1.2/LICENSE` & `oasis-data-manager-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/PKG-INFO` & `oasis-data-manager-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasis-data-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: UNKNOWN
 Home-page: https://github.com/OasisLMF/OasisDataManager
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/complex/complex.py` & `oasis-data-manager-0.1.3/oasis_data_manager/complex/complex.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/complex/examples.py` & `oasis-data-manager-0.1.3/oasis_data_manager/complex/examples.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/config.py` & `oasis-data-manager-0.1.3/oasis_data_manager/config.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/df_reader/backends/base.py` & `oasis-data-manager-0.1.3/oasis_data_manager/df_reader/backends/base.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/df_reader/backends/dask.py` & `oasis-data-manager-0.1.3/oasis_data_manager/df_reader/backends/dask.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/df_reader/backends/pandas.py` & `oasis-data-manager-0.1.3/oasis_data_manager/df_reader/backends/pandas.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/df_reader/config.py` & `oasis-data-manager-0.1.3/oasis_data_manager/df_reader/config.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/df_reader/reader.py` & `oasis-data-manager-0.1.3/oasis_data_manager/df_reader/reader.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/errors/__init__.py` & `oasis-data-manager-0.1.3/oasis_data_manager/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/aws_s3.py` & `oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/aws_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
             "key": self.access_key,
             "secret": self.secret_key,
             "token": self.security_token,
             "use_ssl": self.use_ssl,
             "s3_additional_kwargs": s3_additional_kwargs,
             "client_kwargs": {
                 "endpoint_url": self.endpoint_url,
+                "region_name": self.region_name,
             },
         }
 
     def _strip_signing_parameters(self, url):
         """Duplicated Unsiged URLs from Django-Stroage
 
         Method from: https://github.com/jschneier/django-storages/blob/master/storages/backends/s3boto3.py
```

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/azure_abfs.py` & `oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/azure_abfs.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/base.py` & `oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,16 @@
         ----------
         :param suffix: Set the filename extension
         :type suffix: str
 
         :return: filename string
         :rtype str
         """
+        if suffix.startswith('.'):
+            suffix = suffix[1:]
         return "{}.{}".format(uuid.uuid4().hex, suffix)
 
     def _is_valid_url(self, url):
         """Check if a String is a valid url
 
         Parameters
         ----------
@@ -242,14 +244,21 @@
 
         :param subdir: Store a file under this sub directory path
         :type  subdir: str
 
         :return: Absolute filepath to stored Object
         :rtype str
         """
+        # null ref given
+        if not reference:
+            if required:
+                raise MissingInputsException(reference)
+            else:
+                return None
+
         target = os.path.abspath(
             os.path.join(output_path, subdir) if subdir else output_path
         )
 
         if os.path.isdir(target):
             fname = reference
             if self._is_valid_url(reference):
@@ -294,25 +303,31 @@
         :return: access storage reference returned from self._store_file, self._store_dir
                  This will either be a pre-signed URL or absolute filepath
         :rtype str
         """
         if not reference:
             return None
 
-        ext = "tar.gz" if not suffix else suffix
-        filename = filename if filename else self._get_unique_filename(ext)
-        storage_path = os.path.join(subdir, filename) if subdir else filename
-
-        self.fs.mkdirs(os.path.dirname(storage_path), exist_ok=True)
-
         if os.path.isfile(reference):
-            self.logger.info("Store file: {} -> {}".format(reference, storage_path))
-            self.fs.put(reference, storage_path)
-            return storage_path
+            ext = "".join(Path(reference).suffixes) if not suffix else suffix
+            filename = filename if filename else self._get_unique_filename(ext)
+            storage_path = subdir if subdir else ''
+            self.fs.mkdirs(os.path.dirname(storage_path), exist_ok=True)
+            storage_location = os.path.join(storage_path, filename)
+
+            self.logger.info("Store file: {} -> {}".format(reference, storage_location))
+            self.fs.put(reference, storage_location)
+            return storage_location
+
         elif os.path.isdir(reference):
+            ext = "tar.gz" if not suffix else suffix
+            filename = filename if filename else self._get_unique_filename(ext)
+            storage_path = os.path.join(subdir, filename) if subdir else filename
+            self.fs.mkdirs(os.path.dirname(storage_path), exist_ok=True)
+
             self.logger.info("Store dir: {} -> {}".format(reference, storage_path))
             with tempfile.NamedTemporaryFile() as f:
                 self.compress(f.name, reference, arcname)
                 self.fs.put(f.name, storage_path)
             return storage_path
         else:
             return None
```

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/filestore/backends/local.py` & `oasis-data-manager-0.1.3/oasis_data_manager/filestore/backends/local.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/filestore/config.py` & `oasis-data-manager-0.1.3/oasis_data_manager/filestore/config.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/filestore/filestore.py` & `oasis-data-manager-0.1.3/oasis_data_manager/filestore/filestore.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager/filestore/log.py` & `oasis-data-manager-0.1.3/oasis_data_manager/filestore/log.py`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager.egg-info/PKG-INFO` & `oasis-data-manager-0.1.3/oasis_data_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasis-data-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: UNKNOWN
 Home-page: https://github.com/OasisLMF/OasisDataManager
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oasis-data-manager-0.1.2/oasis_data_manager.egg-info/SOURCES.txt` & `oasis-data-manager-0.1.3/oasis_data_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oasis-data-manager-0.1.2/setup.py` & `oasis-data-manager-0.1.3/setup.py`

 * *Files identical despite different names*

