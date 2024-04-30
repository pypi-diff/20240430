# Comparing `tmp/datarecipe-1.2.8.tar.gz` & `tmp/datarecipe-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarecipe-1.2.8.tar", last modified: Mon Mar 18 09:21:02 2024, max compression
+gzip compressed data, was "datarecipe-1.2.9.tar", last modified: Mon Mar 18 09:38:42 2024, max compression
```

## Comparing `datarecipe-1.2.8.tar` & `datarecipe-1.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 09:21:02.112097 datarecipe-1.2.8/
--rw-rw-rw-   0        0        0     1068 2023-09-19 08:06:14.000000 datarecipe-1.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3255 2024-03-18 09:21:02.112097 datarecipe-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2822 2023-09-25 07:53:58.000000 datarecipe-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 09:21:02.110096 datarecipe-1.2.8/datarecipe/
--rw-rw-rw-   0        0        0      261 2024-02-12 13:55:18.000000 datarecipe-1.2.8/datarecipe/__init__.py
--rw-rw-rw-   0        0        0     3080 2024-03-18 09:20:56.000000 datarecipe-1.2.8/datarecipe/common_tools.py
--rw-rw-rw-   0        0        0     1128 2023-11-28 07:47:48.000000 datarecipe-1.2.8/datarecipe/examine.py
--rw-rw-rw-   0        0        0     4613 2024-02-18 15:46:39.000000 datarecipe-1.2.8/datarecipe/mysql.py
-drwxrwxrwx   0        0        0        0 2024-03-18 09:21:02.111097 datarecipe-1.2.8/datarecipe.egg-info/
--rw-rw-rw-   0        0        0     3255 2024-03-18 09:21:02.000000 datarecipe-1.2.8/datarecipe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-03-18 09:21:02.000000 datarecipe-1.2.8/datarecipe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 09:21:02.000000 datarecipe-1.2.8/datarecipe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-18 09:21:02.000000 datarecipe-1.2.8/datarecipe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 09:21:02.112097 datarecipe-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-03-18 09:21:01.000000 datarecipe-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-18 09:38:42.696399 datarecipe-1.2.9/
+-rw-rw-rw-   0        0        0     1068 2023-09-19 08:06:14.000000 datarecipe-1.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3255 2024-03-18 09:38:42.696399 datarecipe-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2822 2023-09-25 07:53:58.000000 datarecipe-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-18 09:38:42.694400 datarecipe-1.2.9/datarecipe/
+-rw-rw-rw-   0        0        0      261 2024-02-12 13:55:18.000000 datarecipe-1.2.9/datarecipe/__init__.py
+-rw-rw-rw-   0        0        0     2965 2024-03-18 09:38:33.000000 datarecipe-1.2.9/datarecipe/common_tools.py
+-rw-rw-rw-   0        0        0     1128 2023-11-28 07:47:48.000000 datarecipe-1.2.9/datarecipe/examine.py
+-rw-rw-rw-   0        0        0     4613 2024-02-18 15:46:39.000000 datarecipe-1.2.9/datarecipe/mysql.py
+drwxrwxrwx   0        0        0        0 2024-03-18 09:38:42.696399 datarecipe-1.2.9/datarecipe.egg-info/
+-rw-rw-rw-   0        0        0     3255 2024-03-18 09:38:42.000000 datarecipe-1.2.9/datarecipe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-03-18 09:38:42.000000 datarecipe-1.2.9/datarecipe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-18 09:38:42.000000 datarecipe-1.2.9/datarecipe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-03-18 09:38:42.000000 datarecipe-1.2.9/datarecipe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-18 09:38:42.696399 datarecipe-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-03-18 09:38:42.000000 datarecipe-1.2.9/setup.py
```

### Comparing `datarecipe-1.2.8/LICENSE.txt` & `datarecipe-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarecipe-1.2.8/PKG-INFO` & `datarecipe-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarecipe
-Version: 1.2.8
+Version: 1.2.9
 Summary: A recipe for every data baker
 Home-page: https://github.com/Adward-Chen/databaker/tree/main
 Author: Hanfan Chen
 Author-email: HanfanC@outlook.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datarecipe-1.2.8/README.md` & `datarecipe-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `datarecipe-1.2.8/datarecipe/common_tools.py` & `datarecipe-1.2.9/datarecipe/common_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             server.sendmail(send_email_address, receive_email_address, msg.as_string())
     elif type=='TLS':
         with smtplib.SMTP(smtp_address, smtp_port) as server:
             server.starttls()  # 升级连接到TLS
             server.login(send_email_address, send_email_password)
             server.sendmail(send_email_address, receive_email_address, msg.as_string())
 
-def local_to_df(path, partial_file_name, skip_rows = None, keep_file_name=False, sheet_num=1, encoding='auto', sep=','):
+def local_to_df(path, partial_file_name, skip_rows=0, keep_file_name=False, sheet_num=1, encoding='auto', sep=','):
     all_data = pd.DataFrame()
 
     # 获取匹配的文件列表，并为其添加进度条
     file_list = list(glob.glob(f"{path}/**/*{partial_file_name}*.*", recursive=True))
     
     for file_name in tqdm(file_list, desc="Processing Files"):
         _, file_extension = os.path.splitext(file_name)
@@ -36,20 +36,17 @@
         # 识别文件编码类型
         if encoding=='auto':
             with open(file_name, 'rb') as file:
                 result = chardet.detect(file.read())
                 encoding = result['encoding']
         
         if file_extension == "csv":
-            if skip_rows:
-                file_data = pd.read_csv(file_name, encoding=encoding, skiprows=skip_rows, sep=sep)
-            else:
-                file_data = pd.read_csv(file_name, encoding=encoding, sep=sep)
+            file_data = pd.read_csv(file_name, encoding=encoding, skiprows=skip_rows, sep=sep)
         elif file_extension == "xlsx":
-            file_data = pd.read_excel(file_name, sheet_name=sheet_num - 1)
+            file_data = pd.read_excel(file_name, sheet_name=sheet_num - 1, skiprows=skip_rows)
         else:
             continue  # Skip unsupported file types
 
         if keep_file_name:
             file_data["file_name"] = str(file_name)
 
         all_data = pd.concat([all_data, file_data])
```

### Comparing `datarecipe-1.2.8/datarecipe/examine.py` & `datarecipe-1.2.9/datarecipe/examine.py`

 * *Files identical despite different names*

### Comparing `datarecipe-1.2.8/datarecipe/mysql.py` & `datarecipe-1.2.9/datarecipe/mysql.py`

 * *Files identical despite different names*

### Comparing `datarecipe-1.2.8/datarecipe.egg-info/PKG-INFO` & `datarecipe-1.2.9/datarecipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarecipe
-Version: 1.2.8
+Version: 1.2.9
 Summary: A recipe for every data baker
 Home-page: https://github.com/Adward-Chen/databaker/tree/main
 Author: Hanfan Chen
 Author-email: HanfanC@outlook.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datarecipe-1.2.8/setup.py` & `datarecipe-1.2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="datarecipe",
-  version="1.2.8",
+  version="1.2.9",
   author="Hanfan Chen",
   author_email="HanfanC@outlook.com",
   description="A recipe for every data baker",
   long_description=long_description,
   long_description_content_type="markdown",
   url="https://github.com/Adward-Chen/databaker/tree/main",
   packages=setuptools.find_packages(),
```

