# Comparing `tmp/hawk_scanner-0.3.8.tar.gz` & `tmp/hawk_scanner-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hawk_scanner-0.3.8.tar", last modified: Tue Jan  9 15:28:17 2024, max compression
+gzip compressed data, was "hawk_scanner-0.3.9.tar", last modified: Wed Jan 10 10:02:15 2024, max compression
```

## Comparing `hawk_scanner-0.3.8.tar` & `hawk_scanner-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:28:17.907647 hawk_scanner-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-01-09 15:28:17.907647 hawk_scanner-0.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:28:17.903647 hawk_scanner-0.3.8/hawk_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:28:17.903647 hawk_scanner-0.3.8/hawk_scanner/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/couchdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/firebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/gdrive_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/commands/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:28:17.907647 hawk_scanner-0.3.8/hawk_scanner/internals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18127 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/internals/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    19833 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/hawk_scanner/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:28:17.907647 hawk_scanner-0.3.8/hawk_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-01-09 15:28:17.000000 hawk_scanner-0.3.8/hawk_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-01-09 15:28:17.000000 hawk_scanner-0.3.8/hawk_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 15:28:17.000000 hawk_scanner-0.3.8/hawk_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-09 15:28:17.000000 hawk_scanner-0.3.8/hawk_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 15:28:17.000000 hawk_scanner-0.3.8/hawk_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-09 15:28:17.000000 hawk_scanner-0.3.8/hawk_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-09 15:28:17.000000 hawk_scanner-0.3.8/hawk_scanner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-09 15:28:17.907647 hawk_scanner-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-01-09 15:28:12.000000 hawk_scanner-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 10:02:15.733629 hawk_scanner-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-01-10 10:02:15.733629 hawk_scanner-0.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 10:02:15.729629 hawk_scanner-0.3.9/hawk_scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 10:02:15.729629 hawk_scanner-0.3.9/hawk_scanner/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/couchdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/firebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/gdrive_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/commands/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 10:02:15.733629 hawk_scanner-0.3.9/hawk_scanner/internals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19299 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/internals/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19225 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/hawk_scanner/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 10:02:15.733629 hawk_scanner-0.3.9/hawk_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-01-10 10:02:15.000000 hawk_scanner-0.3.9/hawk_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-01-10 10:02:15.000000 hawk_scanner-0.3.9/hawk_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 10:02:15.000000 hawk_scanner-0.3.9/hawk_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-10 10:02:15.000000 hawk_scanner-0.3.9/hawk_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 10:02:15.000000 hawk_scanner-0.3.9/hawk_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-10 10:02:15.000000 hawk_scanner-0.3.9/hawk_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-10 10:02:15.000000 hawk_scanner-0.3.9/hawk_scanner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-10 10:02:15.733629 hawk_scanner-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-01-10 10:02:07.000000 hawk_scanner-0.3.9/setup.py
```

### Comparing `hawk_scanner-0.3.8/LICENSE` & `hawk_scanner-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hawk_scanner-0.3.8/PKG-INFO` & `hawk_scanner-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawk_scanner
-Version: 0.3.8
+Version: 0.3.9
 Summary: A powerful scanner to scan your Filesystem, S3, MongoDB, MySQL, PostgreSQL, Redis, Slack, Google Cloud Storage and Firebase storage for PII and sensitive data using text and OCR analysis. Hawk-eye can also analyse supports most of the file types like docx, xlsx, pptx, pdf, jpg, png, gif, zip, tar, rar, etc.
 Home-page: https://github.com/rohitcoder/hawk-eye
 Author: Rohit Kumar
 Author-email: 
 License: Apache License 2.0
 Keywords: pii secrets sensitive-data cybersecurity scanner
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hawk_scanner Version: 0.3.8 Summary: A powerful
+Metadata-Version: 2.1 Name: hawk_scanner Version: 0.3.9 Summary: A powerful
 scanner to scan your Filesystem, S3, MongoDB, MySQL, PostgreSQL, Redis, Slack,
 Google Cloud Storage and Firebase storage for PII and sensitive data using text
 and OCR analysis. Hawk-eye can also analyse supports most of the file types
 like docx, xlsx, pptx, pdf, jpg, png, gif, zip, tar, rar, etc. Home-page:
 https://github.com/rohitcoder/hawk-eye Author: Rohit Kumar Author-email:
 License: Apache License 2.0 Keywords: pii secrets sensitive-data cybersecurity
 scanner Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/couchdb.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/couchdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def check_data_patterns(db, patterns, profile_name, database_name):
     results = []
     for doc_id in db:
         document = db[doc_id]
         for field_name, field_value in document.items():
             if field_value:
                 value_str = str(field_value)
-                matches = system.match_strings(value_str)
+                matches = system.analyze_strings(value_str, 'couchdb')
                 if matches:
                     for match in matches:
                         results.append({
                             'host': f"{db.resource.credentials[1]}:{db.resource.credentials[2]}",
                             'database': database_name,
                             'document_id': doc_id,
                             'field': field_name,
@@ -38,40 +38,43 @@
                             'sample_text': match['sample_text'],
                             'profile': profile_name,
                             'data_source': 'couchdb'
                         })
 
     return results
 
-def execute(args):
-    results = []
-    system.print_info(f"Running Checks for CouchDB Sources")
-    connections = system.get_connection()
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        couchdb_config = sources_config.get('couchdb')
-
-        if couchdb_config:
-            patterns = system.get_fingerprint_file()
-
-            for key, config in couchdb_config.items():
-                host = config.get('host')
-                port = config.get('port', 5984)  # default CouchDB port
-                username = config.get('username')
-                password = config.get('password')
-                database = config.get('database')
-
-                if host and username and password and database:
-                    system.print_info(f"Checking CouchDB Profile {key} with host and authentication")
-                else:
-                    system.print_error(f"Incomplete CouchDB configuration for key: {key}")
-                    continue
-
-                db = connect_couchdb(host, port, username, password, database)
-                if db:
-                    results += check_data_patterns(db, patterns, key, database)
+def execute(args, programmatic=False):
+    try:
+        results = []
+        system.print_info(f"Running Checks for CouchDB Sources")
+        connections = system.get_connection(args, programmatic)
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            couchdb_config = sources_config.get('couchdb')
+
+            if couchdb_config:
+                patterns = system.get_fingerprint_file(args, programmatic)
+
+                for key, config in couchdb_config.items():
+                    host = config.get('host')
+                    port = config.get('port', 5984)  # default CouchDB port
+                    username = config.get('username')
+                    password = config.get('password')
+                    database = config.get('database')
+
+                    if host and username and password and database:
+                        system.print_info(f"Checking CouchDB Profile {key} with host and authentication")
+                    else:
+                        system.print_error(f"Incomplete CouchDB configuration for key: {key}")
+                        continue
+
+                    db = connect_couchdb(host, port, username, password, database)
+                    if db:
+                        results += check_data_patterns(db, patterns, key, database)
+            else:
+                system.print_error("No CouchDB connection details found in connection.yml")
         else:
-            system.print_error("No CouchDB connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
+            system.print_error("No 'sources' section found in connection.yml")
+    except Exception as e:
+        system.print_error(f"Failed to execute CouchDB checks with error: {e}")
     return results
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/firebase.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/firebase.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,79 +11,83 @@
         firebase_admin.initialize_app(cred)
         bucket = storage.bucket(bucket_name)
         system.print_info(f"Connected to Firebase bucket: {bucket_name}")
         return bucket
     except Exception as e:
         print(f"Failed to connect to Firebase bucket: {e}")
 
-def execute(args):
-    results = []
-    shouldDownload = True
-    connections = system.get_connection()
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        firebase_config = sources_config.get('firebase')
-
-        if firebase_config:
-            for key, config in firebase_config.items():
-                credentials_file = config.get('credentials_file')
-                bucket_name = config.get('bucket_name')
-                exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
-
-                if credentials_file and bucket_name:
-                    bucket = connect_firebase(credentials_file, bucket_name)
-                    if bucket:
-                        for blob in bucket.list_blobs():
-                            file_name = blob.name
-                            ## get unique etag or hash of file
-                            remote_etag = blob.etag
-                            system.print_debug(f"Remote etag: {remote_etag}")
-
-                            if system.should_exclude_file(file_name, exclude_patterns):
-                                continue
-
-                            file_path = f"data/firebase/{remote_etag}-{file_name}"
-                            os.makedirs(os.path.dirname(file_path), exist_ok=True)
-
-                            if config.get("cache") == True:
-                                if os.path.exists(file_path):
-                                    shouldDownload = False
-                                    local_etag = file_path.split('/')[-1].split('-')[0]
-                                    system.print_debug(f"Local etag: {local_etag}")
-                                    system.print_debug(f"File already exists in cache, using it. You can disable cache by setting 'cache: false' in connection.yml")
-                                    if remote_etag != local_etag:
-                                        system.print_debug(f"File in firebase bucket has changed, downloading it again...")
-                                        shouldDownload = True
-                                    else:
-                                        shouldDownload = False
+def execute(args, programmatic=False):
+    try:
+        results = []
+        shouldDownload = True
+        connections = system.get_connection(args, programmatic)
+        fingerprints = system.get_fingerprint_file(args, programmatic) 
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            firebase_config = sources_config.get('firebase')
+
+            if firebase_config:
+                for key, config in firebase_config.items():
+                    credentials_file = config.get('credentials_file')
+                    bucket_name = config.get('bucket_name')
+                    exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
+
+                    if credentials_file and bucket_name:
+                        bucket = connect_firebase(credentials_file, bucket_name)
+                        if bucket:
+                            for blob in bucket.list_blobs():
+                                file_name = blob.name
+                                ## get unique etag or hash of file
+                                remote_etag = blob.etag
+                                system.print_debug(f"Remote etag: {remote_etag}")
+
+                                if system.should_exclude_file(file_name, exclude_patterns):
+                                    continue
 
-                            if shouldDownload:
                                 file_path = f"data/firebase/{remote_etag}-{file_name}"
-                                system.print_debug(f"Downloading file: {file_name} to {file_path}...")
-                                blob.download_to_filename(file_path)
-                            
-                            matches = system.read_match_strings(file_path, 'google_cloud_storage')
-                            if matches:
-                                for match in matches:
-                                    results.append({
-                                        'bucket': bucket_name,
-                                        'file_path': file_name,
-                                        'pattern_name': match['pattern_name'],
-                                        'matches': match['matches'],
-                                        'sample_text': match['sample_text'],
-                                        'profile': key,
-                                        'data_source': 'firebase'
-                                    })
+                                os.makedirs(os.path.dirname(file_path), exist_ok=True)
+
+                                if config.get("cache") == True:
+                                    if os.path.exists(file_path):
+                                        shouldDownload = False
+                                        local_etag = file_path.split('/')[-1].split('-')[0]
+                                        system.print_debug(f"Local etag: {local_etag}")
+                                        system.print_debug(f"File already exists in cache, using it. You can disable cache by setting 'cache: false' in connection.yml")
+                                        if remote_etag != local_etag:
+                                            system.print_debug(f"File in firebase bucket has changed, downloading it again...")
+                                            shouldDownload = True
+                                        else:
+                                            shouldDownload = False
+
+                                if shouldDownload:
+                                    file_path = f"data/firebase/{remote_etag}-{file_name}"
+                                    system.print_debug(f"Downloading file: {file_name} to {file_path}...")
+                                    blob.download_to_filename(file_path)
+                                
+                                matches = system.analyze_file(file_path, 'google_cloud_storage', connections, fingerprints, programmatic=programmatic)
+                                if matches:
+                                    for match in matches:
+                                        results.append({
+                                            'bucket': bucket_name,
+                                            'file_path': file_name,
+                                            'pattern_name': match['pattern_name'],
+                                            'matches': match['matches'],
+                                            'sample_text': match['sample_text'],
+                                            'profile': key,
+                                            'data_source': 'firebase'
+                                        })
 
+                        else:
+                            system.print_error(f"Failed to connect to Firebase bucket: {bucket_name}")
                     else:
-                        system.print_error(f"Failed to connect to Firebase bucket: {bucket_name}")
-                else:
-                    system.print_error(f"Incomplete Firebase configuration for key: {key}")
+                        system.print_error(f"Incomplete Firebase configuration for key: {key}")
+            else:
+                system.print_error("No Firebase connection details found in connection file")
         else:
-            system.print_error("No Firebase connection details found in connection file")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
-    
-    if config.get("cache") == False:
-        os.system("rm -rf data/firebase")
+            system.print_error("No 'sources' section found in connection.yml")
+        
+        if config.get("cache") == False:
+            os.system("rm -rf data/firebase")
+    except Exception as e:
+        print(f"Failed to connect to Firebase bucket: {e}")
     return results
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/fs.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/fs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,71 @@
-import argparse
+import argparse, os, concurrent.futures, time
 from google.cloud import storage
 from rich.console import Console
 from hawk_scanner.internals import system
-import os
-import concurrent.futures
-import time
 
-def process_file(file_path, key, results):
-    matches = system.read_match_strings(file_path, 'fs')
+def process_file(file_path, key, connections, fingerprints, programmatic=False):
+    matches = system.analyze_file(file_path, 'fs', connections, fingerprints, programmatic=programmatic)
     file_data = system.getFileData(file_path)
+    results = []
     if matches:
         for match in matches:
             results.append({
                 'host': 'This PC',
                 'file_path': file_path,
                 'pattern_name': match['pattern_name'],
                 'matches': match['matches'],
                 'sample_text': match['sample_text'],
                 'profile': key,
                 'data_source': 'fs',
                 'file_data': file_data
             })
+    return results
 
-def execute(args):
-    results = []
-    connections = system.get_connection()
+def execute(args, programmatic=False):
+    try:
+        results = []
+        connections = system.get_connection(args, programmatic)
+        fingerprints = system.get_fingerprint_file(args, programmatic)
 
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        fs_config = sources_config.get('fs')
-        if fs_config:
-            for key, config in fs_config.items():
-                if 'path' not in config:
-                    system.print_error(f"Path not found in fs profile '{key}'")
-                    continue
-                path = config.get('path')
-                if not os.path.exists(path):
-                    system.print_error(f"Path '{path}' does not exist")
-                
-                exclude_patterns = fs_config.get(key, {}).get('exclude_patterns', [])
-                start_time = time.time()
-                files = system.list_all_files_iteratively(path, exclude_patterns)
-                
-                # Use ThreadPoolExecutor for parallel processing
-                file_count = 0
-                with concurrent.futures.ThreadPoolExecutor() as executor:
-                    futures = []
-                    for file_path in files:
-                        file_count += 1
-                        futures.append(executor.submit(process_file, file_path, key, results))
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            fs_config = sources_config.get('fs')
+            if fs_config:
+                for key, config in fs_config.items():
+                    if 'path' not in config:
+                        system.print_error(f"Path not found in fs profile '{key}'")
+                        continue
+                    path = config.get('path')
+                    if not os.path.exists(path):
+                        system.print_error(f"Path '{path}' does not exist")
+                    
+                    exclude_patterns = fs_config.get(key, {}).get('exclude_patterns', [])
+                    start_time = time.time()
+                    files = system.list_all_files_iteratively(path, exclude_patterns)
                     
-                    # Wait for all tasks to complete
-                    concurrent.futures.wait(futures)
-                end_time = time.time()
-                system.print_info(f"Time taken to analyze {file_count} files: {end_time - start_time} seconds")
+                    # Use ThreadPoolExecutor for parallel processing
+                    file_count = 0
+                    with concurrent.futures.ThreadPoolExecutor() as executor:
+                        futures = []
+                        for file_path in files:
+                            file_count += 1
+                            results += process_file(file_path, key, connections, fingerprints, programmatic=programmatic)
+                        
+                        # Wait for all tasks to complete
+                        concurrent.futures.wait(futures)
+                    end_time = time.time()
+                    elapsed_time = round(end_time - start_time, 2)
+                    system.print_info(f"Time taken to analyze {file_count} files: {elapsed_time} seconds")
+            else:
+                system.print_error("No filesystem 'fs' connection details found in connection.yml")
         else:
-            system.print_error("No filesystem 'fs' connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
+            system.print_error("No 'sources' section found in connection.yml")
+    except Exception as e:
+        system.print_error(f"Error in executing filesystem checks: {e}")
     return results
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     # Add your command-line arguments here if needed
     args = parser.parse_args()
     results = execute(args)
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/gcs.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/gcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,76 +18,80 @@
     except Exception as e:
         print(f"Failed to connect to Google Cloud Storage bucket: {e}")
 
 def get_last_update_time(blob):
     # Use Google Cloud Blob's etag as the entity tag (ETag)
     return blob.etag
 
-def execute(args):
-    results = []
-    shouldDownload = True
-    connections = system.get_connection()
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        gcs_config = sources_config.get('gcs')
-
-        if gcs_config:
-            for key, config in gcs_config.items():
-                bucket_name = config.get('bucket_name')
-                exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
-                credentials_file = config.get('credentials_file')
-
-                if bucket_name:
-                    bucket = connect_google_cloud(bucket_name, credentials_file)
-                    if bucket:
-                        for blob in bucket.list_blobs():
-                            file_name = blob.name
-                            ## get unique etag or hash of file
-                            remote_etag = get_last_update_time(blob)
-                            system.print_debug(f"Remote etag: {remote_etag}")
-
-                            if system.should_exclude_file(file_name, exclude_patterns):
-                                continue
-
-                            file_path = f"data/google_cloud_storage/{remote_etag}-{file_name}"
-                            os.makedirs(os.path.dirname(file_path), exist_ok=True)
-
-                            if config.get("cache") == True:
-                                if os.path.exists(file_path):
-                                    shouldDownload = False
-                                    local_etag = file_path.split('/')[-1].split('-')[0]
-                                    system.print_debug(f"Local etag: {local_etag}")
-                                    system.print_debug(f"File already exists in cache, using it. You can disable cache by setting 'cache: false' in connection.yml")
-                                    if remote_etag != local_etag:
-                                        system.print_debug(f"File in Google Cloud Storage bucket has changed, downloading it again...")
-                                        shouldDownload = True
-                                    else:
-                                        shouldDownload = False
+def execute(args, programmatic=False):
+    try:
+        results = []
+        shouldDownload = True
+        connections = system.get_connection(args, programmatic)
+        fingerprints = system.get_fingerprint_file(args, programmatic)
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            gcs_config = sources_config.get('gcs')
+
+            if gcs_config:
+                for key, config in gcs_config.items():
+                    bucket_name = config.get('bucket_name')
+                    exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
+                    credentials_file = config.get('credentials_file')
+
+                    if bucket_name:
+                        bucket = connect_google_cloud(bucket_name, credentials_file)
+                        if bucket:
+                            for blob in bucket.list_blobs():
+                                file_name = blob.name
+                                ## get unique etag or hash of file
+                                remote_etag = get_last_update_time(blob)
+                                system.print_debug(f"Remote etag: {remote_etag}")
+
+                                if system.should_exclude_file(file_name, exclude_patterns):
+                                    continue
+
+                                file_path = f"data/google_cloud_storage/{remote_etag}-{file_name}"
+                                os.makedirs(os.path.dirname(file_path), exist_ok=True)
 
-                            if shouldDownload:
-                                system.print_debug(f"Downloading file: {file_name} to {file_path}...")
-                                blob.download_to_filename(file_path)
-
-                            matches = system.read_match_strings(file_path, 'google_cloud_storage')
-                            if matches:
-                                for match in matches:
-                                    results.append({
-                                        'bucket': bucket_name,
-                                        'file_path': file_name,
-                                        'pattern_name': match['pattern_name'],
-                                        'matches': match['matches'],
-                                        'sample_text': match['sample_text'],
-                                        'profile': key,
-                                        'data_source': 'gcs'
-                                    })
+                                if config.get("cache") == True:
+                                    if os.path.exists(file_path):
+                                        shouldDownload = False
+                                        local_etag = file_path.split('/')[-1].split('-')[0]
+                                        system.print_debug(f"Local etag: {local_etag}")
+                                        system.print_debug(f"File already exists in cache, using it. You can disable cache by setting 'cache: false' in connection.yml")
+                                        if remote_etag != local_etag:
+                                            system.print_debug(f"File in Google Cloud Storage bucket has changed, downloading it again...")
+                                            shouldDownload = True
+                                        else:
+                                            shouldDownload = False
+
+                                if shouldDownload:
+                                    system.print_debug(f"Downloading file: {file_name} to {file_path}...")
+                                    blob.download_to_filename(file_path)
+
+                                matches = system.analyze_file(file_path, 'google_cloud_storage', connections, fingerprints, programmatic=programmatic)
+                                if matches:
+                                    for match in matches:
+                                        results.append({
+                                            'bucket': bucket_name,
+                                            'file_path': file_name,
+                                            'pattern_name': match['pattern_name'],
+                                            'matches': match['matches'],
+                                            'sample_text': match['sample_text'],
+                                            'profile': key,
+                                            'data_source': 'gcs'
+                                        })
+                        else:
+                            system.print_error(f"Failed to connect to Google Cloud Storage bucket: {bucket_name}")
                     else:
-                        system.print_error(f"Failed to connect to Google Cloud Storage bucket: {bucket_name}")
-                else:
-                    system.print_error(f"Incomplete Google Cloud Storage configuration for key: {key}")
+                        system.print_error(f"Incomplete Google Cloud Storage configuration for key: {key}")
+            else:
+                system.print_error("No Google Cloud Storage connection details found in connection.yml")
         else:
-            system.print_error("No Google Cloud Storage connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
-    if config.get("cache") == False:
-        os.system("rm -rf data/google_cloud_storage")
+            system.print_error("No 'sources' section found in connection.yml")
+        if config.get("cache") == False:
+            os.system("rm -rf data/google_cloud_storage")
+    except Exception as e:
+        print(f"Failed to connect to Google Cloud Storage bucket: {e}")
     return results
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/gdrive.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/gdrive.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,87 +61,91 @@
     try:
         file_list = drive.ListFile({'q': f"'root' in parents and title='{folder_name}'"}).GetList() if folder_name else drive.ListFile().GetList()
         return file_list
     except Exception as e:
         print(f"Error listing files: {e}")
         return []
 
-def execute(args):
-    results = []
-    should_download = True
-    connections = system.get_connection()
-    is_cache_enabled = False
-    drive_config = None
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        drive_config = sources_config.get('gdrive')
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
-
-    if drive_config:
-        for key, config in drive_config.items():
-            credentials_file = config.get('credentials_file')
-            folder_name = config.get('folder_name')
-            exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
-            is_cache_enabled = config.get('cache', False)
-            drive = connect_google_drive(credentials_file)
-            if not os.path.exists("data/google_drive"):
-                os.makedirs("data/google_drive")
-            if drive:
-                files = list_files(drive, folder_name=folder_name)
-                for file_obj in files:
-                    download_file(drive, file_obj, "data/google_drive")
-                    file_id = file_obj['id']
-                    file_name = file_obj['title']
-                    if file_obj['mimeType'] == 'application/vnd.google-apps.folder':
-                        continue
-
-                    # Construct file_path with the correct folder structure
-                    parent_folder_ids = file_obj['parents']
-                    folder_path = "data/google_drive"
-                    if parent_folder_ids:
-                        for parent_id in parent_folder_ids:
-                            parent_folder = drive.CreateFile({'id': parent_id['id']})
-                            if parent_folder['title'] == 'My Drive':
-                                continue
-                            folder_path = os.path.join(folder_path, parent_folder['title'])
-
-                    file_path = os.path.join(folder_path, file_name)
-
-                    if system.should_exclude_file(file_name, exclude_patterns):
-                        continue
-
-                    if config.get("cache") and os.path.exists(file_path):
-                        should_download = False
-                        system.print_debug(f"File already exists in cache, using it.")
-                    else:
-                        should_download = True
-
-                    if should_download:
+def execute(args, programmatic=False):
+    try:
+        results = []
+        should_download = True
+        connections = system.get_connection(args, programmatic)
+        fingerprints = system.get_fingerprint_file(args, programmatic)
+
+        is_cache_enabled = False
+        drive_config = None
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            drive_config = sources_config.get('gdrive')
+        else:
+            system.print_error("No 'sources' section found in connection.yml")
+
+        if drive_config:
+            for key, config in drive_config.items():
+                credentials_file = config.get('credentials_file')
+                folder_name = config.get('folder_name')
+                exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
+                is_cache_enabled = config.get('cache', False)
+                drive = connect_google_drive(credentials_file)
+                if not os.path.exists("data/google_drive"):
+                    os.makedirs("data/google_drive")
+                if drive:
+                    files = list_files(drive, folder_name=folder_name)
+                    for file_obj in files:
                         download_file(drive, file_obj, "data/google_drive")
+                        file_id = file_obj['id']
+                        file_name = file_obj['title']
+                        if file_obj['mimeType'] == 'application/vnd.google-apps.folder':
+                            continue
+
+                        # Construct file_path with the correct folder structure
+                        parent_folder_ids = file_obj['parents']
+                        folder_path = "data/google_drive"
+                        if parent_folder_ids:
+                            for parent_id in parent_folder_ids:
+                                parent_folder = drive.CreateFile({'id': parent_id['id']})
+                                if parent_folder['title'] == 'My Drive':
+                                    continue
+                                folder_path = os.path.join(folder_path, parent_folder['title'])
+
+                        file_path = os.path.join(folder_path, file_name)
+
+                        if system.should_exclude_file(file_name, exclude_patterns):
+                            continue
+
+                        if config.get("cache") and os.path.exists(file_path):
+                            should_download = False
+                            system.print_debug(f"File already exists in cache, using it.")
+                        else:
+                            should_download = True
+
+                        if should_download:
+                            download_file(drive, file_obj, "data/google_drive")
+
+                        matches = system.analyze_file(file_path, 'gdrive', connections, fingerprints, programmatic=programmatic)
+                        if matches:
+                            for match in matches:
+                                results.append({
+                                    'file_id': file_id,
+                                    'file_name': file_name,
+                                    'file_path': file_path,
+                                    'pattern_name': match['pattern_name'],
+                                    'matches': match['matches'],
+                                    'sample_text': match['sample_text'],
+                                    'profile': key,
+                                    'data_source': 'gdrive'
+                                })
+                else:
+                    system.print_error("Failed to connect to Google Drive")
+        else:
+            system.print_error("No Google Drive connection details found in connection file")
 
-                    matches = system.read_match_strings(file_path, 'gdrive')
-                    if matches:
-                        for match in matches:
-                            results.append({
-                                'file_id': file_id,
-                                'file_name': file_name,
-                                'file_path': file_path,
-                                'pattern_name': match['pattern_name'],
-                                'matches': match['matches'],
-                                'sample_text': match['sample_text'],
-                                'profile': key,
-                                'data_source': 'gdrive'
-                            })
-            else:
-                system.print_error("Failed to connect to Google Drive")
-    else:
-        system.print_error("No Google Drive connection details found in connection file")
-
-    if not is_cache_enabled:
-        os.system("rm -rf data/google_drive")
-
+        if not is_cache_enabled:
+            os.system("rm -rf data/google_drive")
+    except Exception as e:
+        print(f"Failed to connect to Google Drive: {e}")
     return results
 
 # Call the execute function with the necessary arguments
 # execute(your_args)
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/gdrive_workspace.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/gdrive_workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,81 +77,85 @@
             query += f" and '{impersonate_user}' in owners"
         file_list = drive.files().list(q=query).execute().get('files', [])
         return file_list
     except Exception as e:
         print(f"Error listing files: {e}")
         return []
 
-def execute(args):
-    results = []
-    connections = system.get_connection()
-    is_cache_enabled = False
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        drive_config = sources_config.get('gdrive_workspace')
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
-
-    if drive_config:
-        for key, config in drive_config.items():
-            credentials_file = config.get('credentials_file')
-            impersonate_users = config.get('impersonate_users', [])
-            exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
-            is_cache_enabled = config.get('cache', False)
-
-            for impersonate_user in impersonate_users or [None]:
-                drive = connect_google_drive(credentials_file, impersonate_user)
-                if not os.path.exists("data/google_drive"):
-                    os.makedirs("data/google_drive")
-                if drive:
-                    files = list_files(drive, impersonate_user)
-                    for file_obj in files:
-                        
-                        if 'mimeType' in file_obj and file_obj['mimeType'] == 'application/vnd.google-apps.document' or file_obj['mimeType'] == 'application/vnd.google-apps.spreadsheet' or file_obj['mimeType'] == 'application/vnd.google-apps.presentation' or file_obj['mimeType'] == 'application/vnd.google-apps.drawing' or file_obj['mimeType'] == 'application/vnd.google-apps.script':
-                            file_obj['name'] = file_obj['name'] + '-runtime.pdf'
-
-                        file_id = file_obj['id']
-                        file_name = file_obj['name']
-                        folder_path = "data/google_drive"
-
-                        file_path = os.path.join(folder_path, file_name)
-
-                        if system.should_exclude_file(file_name, exclude_patterns):
-                            continue
-
-                        if config.get("cache") and os.path.exists(file_path):
-                            is_cache_enabled = False
-                            system.print_debug(f"File already exists in cache, using it.")
-                        else:
-                            is_cache_enabled = True
-
-                        if is_cache_enabled:
-                            download_file(drive, file_obj, "data/google_drive/")
-
-                        matches = system.read_match_strings(file_path, 'gdrive_workspace')
-                        file_name = file_name.replace('-runtime.pdf', '')
-                        if matches:
-                            for match in matches:
-                                results.append({
-                                    'file_id': file_id,
-                                    'file_name': file_name,
-                                    'user': impersonate_user,
-                                    'file_path': file_path,
-                                    'pattern_name': match['pattern_name'],
-                                    'matches': match['matches'],
-                                    'sample_text': match['sample_text'],
-                                    'profile': key,
-                                    'data_source': 'gdrive_workspace'
-                                })
-                else:
-                    system.print_error("Failed to connect to Google Drive")
-    else:
-        system.print_error("No Google Drive connection details found in connection file")
-
-    """if not is_cache_enabled:
-        os.system("rm -rf data/google_drive")"""
+def execute(args, programmatic=False):
+    try:
+        results = []
+        connections = system.get_connection(args, programmatic)
+        fingerprints = system.get_fingerprint_file(args, programmatic)
+
+        is_cache_enabled = False
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            drive_config = sources_config.get('gdrive_workspace')
+        else:
+            system.print_error("No 'sources' section found in connection.yml")
+
+        if drive_config:
+            for key, config in drive_config.items():
+                credentials_file = config.get('credentials_file')
+                impersonate_users = config.get('impersonate_users', [])
+                exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
+                is_cache_enabled = config.get('cache', False)
+
+                for impersonate_user in impersonate_users or [None]:
+                    drive = connect_google_drive(credentials_file, impersonate_user)
+                    if not os.path.exists("data/google_drive"):
+                        os.makedirs("data/google_drive")
+                    if drive:
+                        files = list_files(drive, impersonate_user)
+                        for file_obj in files:
+                            
+                            if 'mimeType' in file_obj and file_obj['mimeType'] == 'application/vnd.google-apps.document' or file_obj['mimeType'] == 'application/vnd.google-apps.spreadsheet' or file_obj['mimeType'] == 'application/vnd.google-apps.presentation' or file_obj['mimeType'] == 'application/vnd.google-apps.drawing' or file_obj['mimeType'] == 'application/vnd.google-apps.script':
+                                file_obj['name'] = file_obj['name'] + '-runtime.pdf'
+
+                            file_id = file_obj['id']
+                            file_name = file_obj['name']
+                            folder_path = "data/google_drive"
+
+                            file_path = os.path.join(folder_path, file_name)
+
+                            if system.should_exclude_file(file_name, exclude_patterns):
+                                continue
+
+                            if config.get("cache") and os.path.exists(file_path):
+                                is_cache_enabled = False
+                                system.print_debug(f"File already exists in cache, using it.")
+                            else:
+                                is_cache_enabled = True
+
+                            if is_cache_enabled:
+                                download_file(drive, file_obj, "data/google_drive/")
+
+                            matches = system.analyze_file(file_path, 'gdrive_workspace', connections, fingerprints, programmatic=programmatic)
+                            file_name = file_name.replace('-runtime.pdf', '')
+                            if matches:
+                                for match in matches:
+                                    results.append({
+                                        'file_id': file_id,
+                                        'file_name': file_name,
+                                        'user': impersonate_user,
+                                        'file_path': file_path,
+                                        'pattern_name': match['pattern_name'],
+                                        'matches': match['matches'],
+                                        'sample_text': match['sample_text'],
+                                        'profile': key,
+                                        'data_source': 'gdrive_workspace'
+                                    })
+                    else:
+                        system.print_error("Failed to connect to Google Drive")
+        else:
+            system.print_error("No Google Drive connection details found in connection file")
 
+        """if not is_cache_enabled:
+            os.system("rm -rf data/google_drive")"""
+    except Exception as e:
+        print(f"Error executing gdrive_workspace module: {e}")
     return results
 
 # Call the execute function with the necessary arguments
 # execute(y
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/mongodb.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/mongodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             continue
 
         collection = db[collection_name]
         for document in collection.find().limit(limit_end).skip(limit_start):
             for field_name, field_value in document.items():
                 if field_value:
                     value_str = str(field_value)
-                    matches = system.match_strings(value_str)
+                    matches = system.analyze_strings(value_str)
                     if matches:
                         for match in matches:
                             results.append({
                                 'host': db.client.address[0],
                                 'database': database_name,
                                 'collection': collection_name,
                                 'field': field_name,
@@ -55,50 +55,53 @@
                                 'sample_text': match['sample_text'],
                                 'profile': profile_name,
                                 'data_source': 'mongodb'
                             })
 
     return results
 
-def execute(args):
-    results = []
-    system.print_info(f"Running Checks for MongoDB Sources")
-    connections = system.get_connection()
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        mongodb_config = sources_config.get('mongodb')
-
-        if mongodb_config:
-            patterns = system.get_fingerprint_file()
-
-            for key, config in mongodb_config.items():
-                host = config.get('host')
-                port = config.get('port', 27017)  # default MongoDB port
-                username = config.get('username')
-                password = config.get('password')
-                database = config.get('database')
-                uri = config.get('uri')  # Added support for URI
-                limit_start = config.get('limit_start', 0)
-                limit_end = config.get('limit_end', 500)
-                collections = config.get('collections', [])
-
-                if uri:
-                    system.print_info(f"Checking MongoDB Profile {key} using URI")
-                elif host and username and password and database:
-                    system.print_info(f"Checking MongoDB Profile {key} with host and authentication")
-                else:
-                    system.print_error(f"Incomplete MongoDB configuration for key: {key}")
-                    continue
-
-                db = connect_mongodb(host, port, username, password, database, uri)
-                if db:
-                    results += check_data_patterns(db, patterns, key, database, limit_start=limit_start, limit_end=limit_end, whitelisted_collections=collections)
+def execute(args, programmatic=False):
+    try:
+        results = []
+        system.print_info(f"Running Checks for MongoDB Sources")
+        connections = system.get_connection(args, programmatic)
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            mongodb_config = sources_config.get('mongodb')
+
+            if mongodb_config:
+                patterns = system.get_fingerprint_file(args, programmatic)
+
+                for key, config in mongodb_config.items():
+                    host = config.get('host')
+                    port = config.get('port', 27017)  # default MongoDB port
+                    username = config.get('username')
+                    password = config.get('password')
+                    database = config.get('database')
+                    uri = config.get('uri')  # Added support for URI
+                    limit_start = config.get('limit_start', 0)
+                    limit_end = config.get('limit_end', 500)
+                    collections = config.get('collections', [])
+
+                    if uri:
+                        system.print_info(f"Checking MongoDB Profile {key} using URI")
+                    elif host and username and password and database:
+                        system.print_info(f"Checking MongoDB Profile {key} with host and authentication")
+                    else:
+                        system.print_error(f"Incomplete MongoDB configuration for key: {key}")
+                        continue
+
+                    db = connect_mongodb(host, port, username, password, database, uri)
+                    if db:
+                        results += check_data_patterns(db, patterns, key, database, limit_start=limit_start, limit_end=limit_end, whitelisted_collections=collections)
+            else:
+                system.print_error("No MongoDB connection details found in connection.yml")
         else:
-            system.print_error("No MongoDB connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
+            system.print_error("No 'sources' section found in connection.yml")
+    except Exception as e:
+        system.print_error(f"Failed to run MongoDB checks with error: {e}")
     return results
 
 # Example usage
 if __name__ == "__main__":
     execute(None)
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/mysql.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,46 +60,49 @@
             data_count += 1
 
         table_count += 1
 
     cursor.close()
     return results
 
-def execute(args):
-    results = []
-    system.print_info(f"Running Checks for MySQL Sources")
-    connections = system.get_connection()
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        mysql_config = sources_config.get('mysql')
-
-        if mysql_config:
-            patterns = system.get_fingerprint_file()
-
-            for key, config in mysql_config.items():
-                host = config.get('host')
-                user = config.get('user')
-                port = config.get('port', 3306)  # default port for MySQL
-                password = config.get('password')
-                database = config.get('database')
-                limit_start = config.get('limit_start', 0)
-                limit_end = config.get('limit_end', 500)
-                tables = config.get('tables', [])
-
-                if host and user and database:
-                    system.print_info(f"Checking MySQL Profile {key} and database {database}")
-                    conn = connect_mysql(host, port, user, password, database)
-                    if conn:
-                        results += check_data_patterns(conn, patterns, key, database, limit_start=limit_start, limit_end=limit_end, whitelisted_tables=tables)
-                        conn.close()
-                else:
-                    system.print_error(f"Incomplete MySQL configuration for key: {key}")
+def execute(args, programmatic=False):
+    try:
+        results = []
+        system.print_info(f"Running Checks for MySQL Sources")
+        connections = system.get_connection(args, programmatic)
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            mysql_config = sources_config.get('mysql')
+
+            if mysql_config:
+                patterns = system.get_fingerprint_file(args, programmatic)
+
+                for key, config in mysql_config.items():
+                    host = config.get('host')
+                    user = config.get('user')
+                    port = config.get('port', 3306)  # default port for MySQL
+                    password = config.get('password')
+                    database = config.get('database')
+                    limit_start = config.get('limit_start', 0)
+                    limit_end = config.get('limit_end', 500)
+                    tables = config.get('tables', [])
+
+                    if host and user and database:
+                        system.print_info(f"Checking MySQL Profile {key} and database {database}")
+                        conn = connect_mysql(host, port, user, password, database)
+                        if conn:
+                            results += check_data_patterns(conn, patterns, key, database, limit_start=limit_start, limit_end=limit_end, whitelisted_tables=tables)
+                            conn.close()
+                    else:
+                        system.print_error(f"Incomplete MySQL configuration for key: {key}")
+            else:
+                system.print_error("No MySQL connection details found in connection.yml")
         else:
-            system.print_error("No MySQL connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
+            system.print_error("No 'sources' section found in connection.yml")
+    except Exception as e:
+        system.print_error(f"Failed to run MySQL checks with error: {e}")
     return results
 
 # Example usage
 if __name__ == "__main__":
     execute(None)
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/postgresql.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         columns = [column[0] for column in cursor.description]
 
         data_count = 1
         for row in cursor.fetchall():
             for column, value in zip(columns, row):
                 if value:
                     value_str = str(value)
-                    matches = system.match_strings(value_str)
+                    matches = system.analyze_strings(value_str)
                     if matches:
                         for match in matches:
                             results.append({
                                 'host': conn.dsn,
                                 'database': database_name,
                                 'table': table,
                                 'column': column,
@@ -64,46 +64,49 @@
             data_count += 1
 
         table_count += 1
 
     cursor.close()
     return results
 
-def execute(args):
-    results = []
-    system.print_info(f"Running Checks for PostgreSQL Sources")
-    connections = system.get_connection()
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        postgresql_config = sources_config.get('postgresql')
-
-        if postgresql_config:
-            patterns = system.get_fingerprint_file()
-
-            for key, config in postgresql_config.items():
-                host = config.get('host')
-                user = config.get('user')
-                port = config.get('port', 5432)  # default port for PostgreSQL
-                password = config.get('password')
-                database = config.get('database')
-                limit_start = config.get('limit_start', 0)
-                limit_end = config.get('limit_end', 500)
-                tables = config.get('tables', [])
-
-                if host and user and password and database:
-                    system.print_info(f"Checking PostgreSQL Profile {key}, database {database}")
-                    conn = connect_postgresql(host, port, user, password, database)
-                    if conn:
-                        results += check_data_patterns(conn, patterns, key, database, limit_start=limit_start, limit_end=limit_end, whitelisted_tables=tables)
-                        conn.close()
-                else:
-                    system.print_error(f"Incomplete PostgreSQL configuration for key: {key}")
+def execute(args, programmatic=False):
+    try:
+        results = []
+        system.print_info(f"Running Checks for PostgreSQL Sources")
+        connections = system.get_connection(args, programmatic)
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            postgresql_config = sources_config.get('postgresql')
+
+            if postgresql_config:
+                patterns = system.get_fingerprint_file(args, programmatic)
+
+                for key, config in postgresql_config.items():
+                    host = config.get('host')
+                    user = config.get('user')
+                    port = config.get('port', 5432)  # default port for PostgreSQL
+                    password = config.get('password')
+                    database = config.get('database')
+                    limit_start = config.get('limit_start', 0)
+                    limit_end = config.get('limit_end', 500)
+                    tables = config.get('tables', [])
+
+                    if host and user and password and database:
+                        system.print_info(f"Checking PostgreSQL Profile {key}, database {database}")
+                        conn = connect_postgresql(host, port, user, password, database)
+                        if conn:
+                            results += check_data_patterns(conn, patterns, key, database, limit_start=limit_start, limit_end=limit_end, whitelisted_tables=tables)
+                            conn.close()
+                    else:
+                        system.print_error(f"Incomplete PostgreSQL configuration for key: {key}")
+            else:
+                system.print_error("No PostgreSQL connection details found in connection.yml")
         else:
-            system.print_error("No PostgreSQL connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
+            system.print_error("No 'sources' section found in connection.yml")
+    except Exception as e:
+        system.print_error(f"Failed to run PostgreSQL checks with error: {e}")
     return results
 
 # Example usage
 if __name__ == "__main__":
     execute(None)
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/redis.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,34 +40,37 @@
                         'matches': match['matches'],
                         'sample_text': match['sample_text'],
                         'profile': profile_name,
                         'data_source': 'redis'
                     })
     return results
 
-def execute(args):
-    results = []
-    connections = system.get_connection()
+def execute(args, programmatic=False):
+    try:
+        results = []
+        connections = system.get_connection(args, programmatic)
 
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        redis_config = sources_config.get('redis')
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            redis_config = sources_config.get('redis')
 
-        if redis_config:
-            patterns = system.get_fingerprint_file()
+            if redis_config:
+                patterns = system.get_fingerprint_file(args, programmatic)
 
-            for profile_name, config in redis_config.items():
-                host = config.get('host')
-                port = config.get('port', 6379)
+                for profile_name, config in redis_config.items():
+                    host = config.get('host')
+                    port = config.get('port', 6379)
 
-                if host:
-                    redis_instance = connect_redis(host, port)
-                    if redis_instance:
-                        results = check_data_patterns(redis_instance, patterns, profile_name, host)
-                        redis_instance.close()
-                else:
-                    system.print_error(f"Incomplete Redis configuration for key: {profile_name}")
+                    if host:
+                        redis_instance = connect_redis(host, port)
+                        if redis_instance:
+                            results = check_data_patterns(redis_instance, patterns, profile_name, host)
+                            redis_instance.close()
+                    else:
+                        system.print_error(f"Incomplete Redis configuration for key: {profile_name}")
+            else:
+                system.print_error("No Redis connection details found in connection.yml")
         else:
-            system.print_error("No Redis connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
+            system.print_error("No 'sources' section found in connection.yml")
+    except Exception as e:
+        system.print_error(f"Error: {e}")
     return results
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/s3.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,80 +27,82 @@
     return None
 
 def get_patterns_from_file(file_path):
     with open(file_path, 'r', encoding='utf-8') as file:
         patterns = yaml.safe_load(file)
         return patterns
 
-def execute(args):
-    results = []
-    shouldDownload = True
-    system.print_info(f"Running Checks for S3 Sources")
-    connections = system.get_connection()
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        s3_config = sources_config.get('s3')
-
-        if s3_config:
-            for key, config in s3_config.items():
-                access_key = config.get('access_key')
-                secret_key = config.get('secret_key')
-                bucket_name = config.get('bucket_name')
-                exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
-
-                system.print_info(f"Checking S3 profile: '{key}' with bucket '{bucket_name}'")
-                profile_name = key
-                if access_key and secret_key and bucket_name:
-                    bucket = connect_s3(access_key, secret_key, bucket_name)
-                    if bucket:
-
-                        for obj in bucket.objects.all():
-                            remote_etag = obj.e_tag.replace('"', '')
-                            system.print_debug(f"Remote etag: {remote_etag}")
-                            file_name = obj.key
-                            if system.should_exclude_file(file_name, exclude_patterns):
-                                continue
-
-                            file_path = f"data/s3/{remote_etag}-{file_name}"
-                            os.makedirs(os.path.dirname(file_path), exist_ok=True)
-                            if config.get("cache") == True:
-                                if os.path.exists(file_path):
-                                    shouldDownload = False
-                                    local_etag = file_path.split('/')[-1].split('-')[0]
-                                    system.print_debug(f"Local etag: {local_etag}")
-                                    system.print_debug(f"File already exists in cache, using it. You can disable cache by setting 'cache: false' in connection.yml")
-                                    if remote_etag != local_etag:
-                                        system.print_debug(f"File in S3 bucket has changed, downloading it again...")
-                                        shouldDownload = True
-                                    else:
-                                        shouldDownload = False
+def execute(args, programmatic=False):
+    try:
+        results = []
+        shouldDownload = True
+        system.print_info(f"Running Checks for S3 Sources")
+        connections = system.get_connection(args, programmatic)
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            s3_config = sources_config.get('s3')
+
+            if s3_config:
+                for key, config in s3_config.items():
+                    access_key = config.get('access_key')
+                    secret_key = config.get('secret_key')
+                    bucket_name = config.get('bucket_name')
+                    exclude_patterns = config.get(key, {}).get('exclude_patterns', [])
+
+                    system.print_info(f"Checking S3 profile: '{key}' with bucket '{bucket_name}'")
+                    profile_name = key
+                    if access_key and secret_key and bucket_name:
+                        bucket = connect_s3(access_key, secret_key, bucket_name)
+                        if bucket:
+
+                            for obj in bucket.objects.all():
+                                remote_etag = obj.e_tag.replace('"', '')
+                                system.print_debug(f"Remote etag: {remote_etag}")
+                                file_name = obj.key
+                                if system.should_exclude_file(file_name, exclude_patterns):
+                                    continue
 
-                            if shouldDownload:
                                 file_path = f"data/s3/{remote_etag}-{file_name}"
-                                system.print_debug(f"Downloading file: {file_name} to {file_path}...")
-                                bucket.download_file(file_name, file_path)
-                            
-                            matches = system.read_match_strings(file_path, 'google_cloud_storage')
-                            if matches:
-                                for match in matches:
-                                    results.append({
-                                        'bucket': bucket_name,
-                                        'file_path': file_name,
-                                        'pattern_name': match['pattern_name'],
-                                        'matches': match['matches'],
-                                        'sample_text': match['sample_text'],
-                                        'profile': key,
-                                        'data_source': 's3'
-                                    })
+                                os.makedirs(os.path.dirname(file_path), exist_ok=True)
+                                if config.get("cache") == True:
+                                    if os.path.exists(file_path):
+                                        shouldDownload = False
+                                        local_etag = file_path.split('/')[-1].split('-')[0]
+                                        system.print_debug(f"Local etag: {local_etag}")
+                                        system.print_debug(f"File already exists in cache, using it. You can disable cache by setting 'cache: false' in connection.yml")
+                                        if remote_etag != local_etag:
+                                            system.print_debug(f"File in S3 bucket has changed, downloading it again...")
+                                            shouldDownload = True
+                                        else:
+                                            shouldDownload = False
+
+                                if shouldDownload:
+                                    file_path = f"data/s3/{remote_etag}-{file_name}"
+                                    system.print_debug(f"Downloading file: {file_name} to {file_path}...")
+                                    bucket.download_file(file_name, file_path)
+                                
+                                matches = system.analyze_strings(file_path, 'google_cloud_storage')
+                                if matches:
+                                    for match in matches:
+                                        results.append({
+                                            'bucket': bucket_name,
+                                            'file_path': file_name,
+                                            'pattern_name': match['pattern_name'],
+                                            'matches': match['matches'],
+                                            'sample_text': match['sample_text'],
+                                            'profile': key,
+                                            'data_source': 's3'
+                                        })
 
+                        else:
+                            system.print_error(f"Failed to connect to S3 bucket: {bucket_name}")
                     else:
-                        system.print_error(f"Failed to connect to S3 bucket: {bucket_name}")
-                else:
-                    system.print_error(f"Incomplete S3 configuration for key: {key}")
+                        system.print_error(f"Incomplete S3 configuration for key: {key}")
+            else:
+                system.print_error("No S3 connection details found in connection.yml")
         else:
-            system.print_error("No S3 connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
-    if config.get("cache") == False:
-        os.system("rm -rf data/s3")
+            system.print_error("No 'sources' section found in connection.yml")
+        if config.get("cache") == False:
+            os.system("rm -rf data/s3")
+    except Exception as e:
+        system.print_error(f"Error running S3 checks: {e}")
     return results
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/slack.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,39 +63,41 @@
                                 'data_source': 'slack'
                             })
         return results
     except SlackApiError as e:
         system.print_error(f"Failed to fetch messages from Slack with error: {e.response['error']}")
         return results
 
-def execute(args):
-    results = []
-    system.print_info("Running Checks for Slack Sources")
-    connections = system.get_connection()
-
-    if 'sources' in connections:
-        sources_config = connections['sources']
-        slack_config = sources_config.get('slack')
-
-        if slack_config:
-            patterns = system.get_fingerprint_file()
-
-            for key, config in slack_config.items():
-                token = config.get('token')
-                channel_types = config.get('channel_types', "public_channel,private_channel")
-                channel_names = config.get('channel_names', None)
-
-                if token:
-                    system.print_info(f"Checking Slack Profile {key}")
-                else:
-                    system.print_error(f"Incomplete Slack configuration for key: {key}")
-                    continue
-
-                client = connect_slack(token)
-                if client:
-                    results += check_slack_messages(client, patterns, key, channel_types, channel_names)
+def execute(args, programmatic=False):
+    try:
+        results = []
+        system.print_info("Running Checks for Slack Sources")
+        connections = system.get_connection(args, programmatic)
+
+        if 'sources' in connections:
+            sources_config = connections['sources']
+            slack_config = sources_config.get('slack')
+
+            if slack_config:
+                patterns = system.get_fingerprint_file(args, programmatic)
+
+                for key, config in slack_config.items():
+                    token = config.get('token')
+                    channel_types = config.get('channel_types', "public_channel,private_channel")
+                    channel_names = config.get('channel_names', None)
+
+                    if token:
+                        system.print_info(f"Checking Slack Profile {key}")
+                    else:
+                        system.print_error(f"Incomplete Slack configuration for key: {key}")
+                        continue
+
+                    client = connect_slack(token)
+                    if client:
+                        results += check_slack_messages(client, patterns, key, channel_types, channel_names)
+            else:
+                system.print_error("No Slack connection details found in connection.yml")
         else:
-            system.print_error("No Slack connection details found in connection.yml")
-    else:
-        system.print_error("No 'sources' section found in connection.yml")
-
+            system.print_error("No 'sources' section found in connection.yml")
+    except Exception as e:
+        system.print_error(f"Failed to run Slack checks with error: {e}")
     return results
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/commands/text.py` & `hawk_scanner-0.3.9/hawk_scanner/commands/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 from hawk_scanner.internals import system
 from rich.console import Console
 
 console = Console()
 
 def check_data_patterns(value, patterns, profile_name):
     value_str = str(value)
-    matches = system.match_strings(value_str)
+    matches = system.analyze_strings(value_str)
     results = []
     if matches:
         for match in matches:
             results.append({
                 'pattern_name': match['pattern_name'],
                 'matches': match['matches'],
                 'sample_text': match['sample_text'],
                 'profile': profile_name,
                 'data_source': 'text'
             })
     return results
 
 def execute(args, programmatic=False):
-    results = []
-    system.print_info(f"Running Checks for Simple text")
-    connections = system.get_connection()
-    patterns = system.get_fingerprint_file()
-    
-    if not programmatic:
+    try:
+        results = []
+        system.print_info(f"Running Checks for Simple text")
+        connections = system.get_connection(args, programmatic)
+        patterns = system.get_fingerprint_file(args, programmatic)
         if 'sources' in connections:
             sources_config = connections['sources']
             text_config = sources_config.get('text')
-
             if text_config:
                 for key, config in text_config.items():
                     text = config.get('text', None)
                     results += check_data_patterns(text, patterns, key)
             else:
                 system.print_error("No text connection details found in connection.yml")
         else:
             system.print_error("No 'sources' section found in connection.yml")
-    else:
-        text = args.get('text', None)
-        results += check_data_patterns(text, patterns, 'text')
+    except Exception as e:
+        system.print_error(f"Failed to connect to text with error: {e}")
     return results
 
 # Example usage
 if __name__ == "__main__":
     execute(None)
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/internals/system.py` & `hawk_scanner-0.3.9/hawk_scanner/internals/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,27 @@
 import shutil
 import os, cv2
 import tarfile
 
 # Create a TinyDB instance for storing previous alert hashes
 db = TinyDB('previous_alerts.json')
 
+## Now separate the results by data_source
+data_sources = ['s3', 'mysql', 'redis', 'firebase', 'gcs', 'fs', 'postgresql', 'mongodb', 'slack', 'couchdb', 'gdrive', 'gdrive_workspace', 'text']
+data_sources_option = ['all'] + data_sources
 parser = argparse.ArgumentParser(description='🦅 A powerful scanner to scan your Filesystem, S3, MySQL, PostgreSQL, MongoDB, Redis, Google Cloud Storage and Firebase storage for PII and sensitive data.')
+parser.add_argument('command', nargs='?', choices=data_sources_option, help='Command to execute')
+parser.add_argument('--json', help='Save output to json file')
+parser.add_argument('--debug', action='store_true', help='Enable debug mode')
 parser.add_argument('--connection', action='store', help='YAML Connection file path')
 parser.add_argument('--fingerprint', action='store', help='Override YAML fingerprint file path')
-parser.add_argument('--debug', action='store_true', help='Enable debug mode')
 parser.add_argument('--shutup', action='store_true', help='Suppress the Hawk Eye banner 🫣', default=False)
 
 args, extra_args = parser.parse_known_args()
 
-
 console = Console()
 
 def calculate_msg_hash(msg):
     return hashlib.sha256(msg.encode()).hexdigest()
 
 def print_info(message):
     console.print(f"[yellow][INFO][/yellow] {str(message)}")
@@ -102,52 +106,65 @@
     redacted_middle = "*" * len(middle)
 
     # Concatenate the parts back together
     redacted_string = before_middle + redacted_middle + after_middle
 
     return redacted_string
 
-def get_connection():
-    if args.connection:
-        if os.path.exists(args.connection):
-            with open(args.connection, 'r') as file:
-                connections = yaml.safe_load(file)
-                return connections
+def get_connection(args=None, programmatic=False):
+    try:
+        if args.connection and not programmatic:
+            if os.path.exists(args.connection):
+                with open(args.connection, 'r') as file:
+                    connections = yaml.safe_load(file)
+                    return connections
+            else:
+                print_error(f"Connection file not found: {args.connection}")
+                exit(1)
+        elif programmatic and args.connection:
+            connections = yaml.safe_load(args.connection)
+            return connections
         else:
-            print_error(f"Connection file not found: {args.connection}")
+            print_error(f"Please provide a connection file using --connection flag")
             exit(1)
-    else:
-        print_error(f"Please provide a connection file using --connection flag")
+    except Exception as e:
+        print_error(f"Unable to load connection file: {e}")
         exit(1)
 
-def get_fingerprint_file():
-    if args.fingerprint:
-        if os.path.exists(args.fingerprint):
-            with open(args.fingerprint, 'r') as file:
-                return yaml.safe_load(file)
-        else:
-            print_error(f"Fingerprint file not found: {args.fingerprint}")
-            exit(1)
-    else:
-        file_path = "https://github.com/rohitcoder/hawk-eye/raw/main/fingerprint.yml"
-        try:
-            response = requests.get(file_path, timeout=10)
-            print_info(f"Downloading default fingerprint.yml from {file_path}")
-            if response.status_code == 200:
-                with open('fingerprint.yml', 'wb') as file:
-                    file.write(response.content)
-                return yaml.safe_load(response.content)
+def get_fingerprint_file(args, programmatic=False):
+    try:
+        if args.fingerprint and not programmatic:
+            if os.path.exists(args.fingerprint):
+                with open(args.fingerprint, 'r') as file:
+                    return yaml.safe_load(file)
             else:
+                print_error(f"Fingerprint file not found: {args.fingerprint}")
+                exit(1)
+        elif programmatic and args.fingerprint:
+            return yaml.safe_load(args.fingerprint)
+        else:
+            file_path = "https://github.com/rohitcoder/hawk-eye/raw/main/fingerprint.yml"
+            try:
+                response = requests.get(file_path, timeout=10)
+                print_info(f"Downloading default fingerprint.yml from {file_path}")
+                if response.status_code == 200:
+                    with open('fingerprint.yml', 'wb') as file:
+                        file.write(response.content)
+                    return yaml.safe_load(response.content)
+                else:
+                    print_error(f"Unable to download default fingerprint.yml please provide your own fingerprint file using --fingerprint flag")
+                    exit(1)
+            except Exception as e:
                 print_error(f"Unable to download default fingerprint.yml please provide your own fingerprint file using --fingerprint flag")
                 exit(1)
-        except Exception as e:
-            print_error(f"Unable to download default fingerprint.yml please provide your own fingerprint file using --fingerprint flag")
-            exit(1)
+    except Exception as e:
+        print_error(f"Unable to load fingerprint file: {e}")
+        exit(1)
 
-patterns = get_fingerprint_file()
+patterns = get_fingerprint_file(args)
 
 def print_banner():
     banner = r"""
                                 /T /I
                                 / |/ | .-~/
                             T\ Y  I  |/  /  _
             /T               | \I  |  I  Y.-~/
@@ -179,31 +196,31 @@
                     / .  .  . : | :!        \\
                 (_/  /   | | j-"             ~^~^
                     ~-<_(_.^-~"
     """
     if not args.shutup:
         console.print(banner)
 
-connections = get_connection()
+connections = get_connection(args)
+patterns = get_fingerprint_file(args)
 
-def match_strings(content):
+def analyze_strings(content, connections=connections, patterns=patterns, programmatic=False):
     matched_strings = []
-
+    print_debug(f"Connections: {connections}")
     if 'notify' in connections:
         redacted: bool = connections.get('notify', {}).get('redacted', False)
     else:
         redacted = False
         
     for pattern_name, pattern_regex in patterns.items():
         print_debug(f"Matching pattern: {pattern_name}")
         found = {} 
         ## parse pattern_regex as Regex
         complied_regex = re.compile(pattern_regex, re.IGNORECASE)
         print_debug(f"Regex: {complied_regex}")
-        print_debug(f"Content: {content}")
         matches = re.findall(complied_regex, content)
         print_debug(f"Matches: {matches}")
         if matches:
             print_debug(f"Found {len(matches)} matches for pattern: {pattern_name}")
             found['pattern_name'] = pattern_name
             redacted_matches = []
             if redacted:
@@ -246,26 +263,20 @@
     for root, dirs, files in os.walk(path, topdown=True):
         dirs[:] = [d for d in dirs if not should_exclude_folder(os.path.join(root, d), exclude_patterns)]
 
         for file in files:
             if not should_exclude_file(file, exclude_patterns):
                 yield os.path.join(root, file)
 
-def read_match_strings(file_path, source):
+def analyze_file(file_path, source, connections=None, patterns=None, programmatic=False):
     print_info(f"Scanning file: {file_path}")
     content = ''
-
     try:
-        # Check if the file is an image
-        print(file_path)
         if file_path.lower().endswith(('.png', '.jpg', '.jpeg', '.gif', '.bmp')):
-            print("ocr started for "+file_path)
             content = enhance_and_ocr(file_path)
-            print("texts")
-            print(content)
         # Check if the file is a PDF document
         elif file_path.lower().endswith('.pdf'):
             content = read_pdf(file_path)
         # Check if the file is an office document (Word, Excel, PowerPoint)
         elif file_path.lower().endswith(('.docx', '.xlsx', '.pptx')):
             content = read_office_document(file_path)
         # Check if the file is an archive (zip, rar, tar, tar.gz)
@@ -273,18 +284,18 @@
             content = read_archive(file_path)
         else:
             # For other file types, read content normally
             with open(file_path, 'rb') as file:
                 # Attempt to decode using UTF-8, fallback to 'latin-1' if needed
                 content = file.read().decode('utf-8', errors='replace')
     except Exception as e:
-        print_debug(f"Error in read_match_strings: {e}")
+        print_debug(f"Error in analyze_file: {e}")
         pass
-
-    matched_strings = match_strings(content)
+    matched_strings = analyze_strings(content, connections, patterns, programmatic=programmatic)
+    print_debug(f"Matched strings: {matched_strings}")
     return matched_strings
 
 def read_pdf(file_path):
     content = ''
     try:
         # Read content from PDF document
         with open(file_path, 'rb') as file:
@@ -343,15 +354,15 @@
                 with tarfile.open(file_path, 'r:gz') as tar:
                     tar.extractall(tmp_dir)
 
             # Iterate over all files in the temporary directory
             for root, dirs, files in os.walk(tmp_dir):
                 for file in files:
                     file_path = os.path.join(root, file)
-                    content += read_match_strings(file_path, 'archive')  # Recursively read content
+                    content += analyze_file(file_path, 'archive')  # Recursively read content
 
             # Clean up the temporary directory
             shutil.rmtree(tmp_dir)
     except Exception as e:
         print_debug(f"Error in read_archive: {e}")
     return content
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner/main.py` & `hawk_scanner-0.3.9/hawk_scanner/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     os.system('cls' if os.name == 'nt' else 'clear')
 
 
 clear_screen()
 system.print_banner()
 
 console = Console()
-
-## Now separate the results by data_source
-data_sources = ['s3', 'mysql', 'redis', 'firebase', 'gcs', 'fs', 'postgresql', 'mongodb', 'slack', 'couchdb', 'gdrive', 'gdrive_workspace', 'text']
+args = system.args
 
 def load_command_module(command):
     try:
         module = importlib.import_module(f"hawk_scanner.commands.{command}")
         return module
     except Exception as e:
         print(f"Command '{command}' is not supported. {e} ")
@@ -38,30 +36,23 @@
     results = module.execute(args)
     for result in results:
         final_results.append(result)
     return final_results
 
 
 def main():
-    data_sources_option = ['all'] + data_sources
-    parser = argparse.ArgumentParser(description='CLI Command Executor')
-    parser.add_argument('command', nargs='?', choices=data_sources_option, help='Command to execute')
-    parser.add_argument('--json', help='Save output to json file')
-    parser.add_argument('--debug', action='store_true', help='Enable debug mode')
-
-    args, extra_args = parser.parse_known_args()
     results = []
     if args.command:
         if args.command == 'all':
             commands = data_sources
             for command in commands:
-                for data in execute_command(command, extra_args):
+                for data in execute_command(command, args):
                     results.append(data)
         else:
-            for data in execute_command(args.command, extra_args):
+            for data in execute_command(args.command, args):
                 results.append(data)
     else:
         system.print_error("Please provide a command to execute")
 
     ## GROUP results in grouped_results by datasource by key val
     grouped_results = {}
     for result in results:
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner.egg-info/PKG-INFO` & `hawk_scanner-0.3.9/hawk_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawk_scanner
-Version: 0.3.8
+Version: 0.3.9
 Summary: A powerful scanner to scan your Filesystem, S3, MongoDB, MySQL, PostgreSQL, Redis, Slack, Google Cloud Storage and Firebase storage for PII and sensitive data using text and OCR analysis. Hawk-eye can also analyse supports most of the file types like docx, xlsx, pptx, pdf, jpg, png, gif, zip, tar, rar, etc.
 Home-page: https://github.com/rohitcoder/hawk-eye
 Author: Rohit Kumar
 Author-email: 
 License: Apache License 2.0
 Keywords: pii secrets sensitive-data cybersecurity scanner
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hawk_scanner Version: 0.3.8 Summary: A powerful
+Metadata-Version: 2.1 Name: hawk_scanner Version: 0.3.9 Summary: A powerful
 scanner to scan your Filesystem, S3, MongoDB, MySQL, PostgreSQL, Redis, Slack,
 Google Cloud Storage and Firebase storage for PII and sensitive data using text
 and OCR analysis. Hawk-eye can also analyse supports most of the file types
 like docx, xlsx, pptx, pdf, jpg, png, gif, zip, tar, rar, etc. Home-page:
 https://github.com/rohitcoder/hawk-eye Author: Rohit Kumar Author-email:
 License: Apache License 2.0 Keywords: pii secrets sensitive-data cybersecurity
 scanner Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `hawk_scanner-0.3.8/hawk_scanner.egg-info/SOURCES.txt` & `hawk_scanner-0.3.9/hawk_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hawk_scanner-0.3.8/readme.md` & `hawk_scanner-0.3.9/readme.md`

 * *Files identical despite different names*

### Comparing `hawk_scanner-0.3.8/setup.py` & `hawk_scanner-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = "0.3.8"
+VERSION = "0.3.9"
 
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
```

