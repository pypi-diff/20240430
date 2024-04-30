# Comparing `tmp/speedtab-0.2.1.8.tar.gz` & `tmp/speedtab-0.2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.2.1.8.tar", max compression
+gzip compressed data, was "speedtab-0.2.1.9.tar", max compression
```

## Comparing `speedtab-0.2.1.8.tar` & `speedtab-0.2.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2024-04-22 14:44:54.149278 speedtab-0.2.1.8/pyproject.toml
--rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.8/speedtab/__init__.py
--rw-r--r--   0        0        0    88064 2024-04-22 14:44:39.537125 speedtab-0.2.1.8/speedtab/client.py
--rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.8/speedtab/enums.py
--rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.8/speedtab/formats.py
--rw-r--r--   0        0        0      783 2024-04-22 14:45:02.220885 speedtab-0.2.1.8/setup.py
--rw-r--r--   0        0        0      808 2024-04-22 14:45:02.221886 speedtab-0.2.1.8/PKG-INFO
+-rw-r--r--   0        0        0      567 2024-04-22 14:48:24.759600 speedtab-0.2.1.9/pyproject.toml
+-rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.9/speedtab/__init__.py
+-rw-r--r--   0        0        0    88073 2024-04-22 14:48:24.699600 speedtab-0.2.1.9/speedtab/client.py
+-rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.9/speedtab/enums.py
+-rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.9/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2024-04-22 14:48:54.819719 speedtab-0.2.1.9/setup.py
+-rw-r--r--   0        0        0      808 2024-04-22 14:48:54.819719 speedtab-0.2.1.9/PKG-INFO
```

### Comparing `speedtab-0.2.1.8/pyproject.toml` & `speedtab-0.2.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.2.1.8"
+version = "0.2.1.9"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.2.1.8/speedtab/client.py` & `speedtab-0.2.1.9/speedtab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
                         'requests': batch_update_list
                     }}).execute()
 
             if batch_update_data_list:
                 self.connect_v4.spreadsheets().values().batchUpdate(**{
                     'spreadsheetId': self.spreadsheet_id,
                     'body': {
-                        'valueInputOption': 'USER_ENTERED',
+                        'valueInputOption': self.value_input_option,
                         'data': batch_update_data_list,
                     }}).execute()
         if batch_update_chart_list:
             self.connect_v4.spreadsheets().batchUpdate(**{
                 'spreadsheetId': self.spreadsheet_id,
                 'body': {
                     'requests': batch_update_chart_list
```

### Comparing `speedtab-0.2.1.8/speedtab/enums.py` & `speedtab-0.2.1.9/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.8/speedtab/formats.py` & `speedtab-0.2.1.9/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.8/setup.py` & `speedtab-0.2.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.2.1.8',
+    'version': '0.2.1.9',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.2.1.8/PKG-INFO` & `speedtab-0.2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.2.1.8
+Version: 0.2.1.9
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

