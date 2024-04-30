# Comparing `tmp/carreiras-commons-0.0.7.tar.gz` & `tmp/carreiras-commons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carreiras-commons-0.0.7.tar", last modified: Fri Feb  9 12:25:55 2024, max compression
+gzip compressed data, was "carreiras-commons-0.0.9.tar", last modified: Fri Feb  9 19:10:04 2024, max compression
```

## Comparing `carreiras-commons-0.0.7.tar` & `carreiras-commons-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 israelbrancomendonca   (501) staff       (20)        0 2024-02-09 12:25:55.660537 carreiras-commons-0.0.7/
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)       36 2024-02-08 11:47:19.000000 carreiras-commons-0.0.7/LICENSE.txt
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      923 2024-02-09 12:25:55.660621 carreiras-commons-0.0.7/PKG-INFO
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      549 2024-02-08 11:47:19.000000 carreiras-commons-0.0.7/README.md
-drwxr-xr-x   0 israelbrancomendonca   (501) staff       (20)        0 2024-02-09 12:25:55.659628 carreiras-commons-0.0.7/carreiras_commons/
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      294 2024-02-08 11:47:19.000000 carreiras-commons-0.0.7/carreiras_commons/__init__.py
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      958 2024-02-09 12:24:36.000000 carreiras-commons-0.0.7/carreiras_commons/config.py
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      953 2024-02-09 12:24:36.000000 carreiras-commons-0.0.7/carreiras_commons/messaging_email.py
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      983 2024-02-09 12:24:36.000000 carreiras-commons-0.0.7/carreiras_commons/messaging_notificacao.py
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      979 2024-02-09 12:24:36.000000 carreiras-commons-0.0.7/carreiras_commons/messaging_notificacao_admin.py
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      547 2024-02-09 12:24:36.000000 carreiras-commons-0.0.7/carreiras_commons/notificacao_adm_enum.py
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      982 2024-02-08 13:02:15.000000 carreiras-commons-0.0.7/carreiras_commons/notificacao_enum.py
-drwxr-xr-x   0 israelbrancomendonca   (501) staff       (20)        0 2024-02-09 12:25:55.660405 carreiras-commons-0.0.7/carreiras_commons.egg-info/
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      923 2024-02-09 12:25:55.000000 carreiras-commons-0.0.7/carreiras_commons.egg-info/PKG-INFO
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      471 2024-02-09 12:25:55.000000 carreiras-commons-0.0.7/carreiras_commons.egg-info/SOURCES.txt
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)        1 2024-02-09 12:25:55.000000 carreiras-commons-0.0.7/carreiras_commons.egg-info/dependency_links.txt
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)       18 2024-02-09 12:25:55.000000 carreiras-commons-0.0.7/carreiras_commons.egg-info/top_level.txt
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      106 2024-02-09 12:25:55.660853 carreiras-commons-0.0.7/setup.cfg
--rw-r--r--   0 israelbrancomendonca   (501) staff       (20)     1041 2024-02-09 12:25:44.000000 carreiras-commons-0.0.7/setup.py
+drwxr-xr-x   0 israelbrancomendonca   (501) staff       (20)        0 2024-02-09 19:10:04.962382 carreiras-commons-0.0.9/
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)       36 2024-02-08 11:47:19.000000 carreiras-commons-0.0.9/LICENSE.txt
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      923 2024-02-09 19:10:04.962468 carreiras-commons-0.0.9/PKG-INFO
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      549 2024-02-08 11:47:19.000000 carreiras-commons-0.0.9/README.md
+drwxr-xr-x   0 israelbrancomendonca   (501) staff       (20)        0 2024-02-09 19:10:04.961529 carreiras-commons-0.0.9/carreiras_commons/
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      294 2024-02-08 11:47:19.000000 carreiras-commons-0.0.9/carreiras_commons/__init__.py
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)     1193 2024-02-09 19:09:35.000000 carreiras-commons-0.0.9/carreiras_commons/config.py
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      953 2024-02-09 12:24:36.000000 carreiras-commons-0.0.9/carreiras_commons/messaging_email.py
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      983 2024-02-09 12:24:36.000000 carreiras-commons-0.0.9/carreiras_commons/messaging_notificacao.py
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      979 2024-02-09 12:24:36.000000 carreiras-commons-0.0.9/carreiras_commons/messaging_notificacao_admin.py
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      547 2024-02-09 12:24:36.000000 carreiras-commons-0.0.9/carreiras_commons/notificacao_adm_enum.py
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      982 2024-02-08 13:02:15.000000 carreiras-commons-0.0.9/carreiras_commons/notificacao_enum.py
+drwxr-xr-x   0 israelbrancomendonca   (501) staff       (20)        0 2024-02-09 19:10:04.962243 carreiras-commons-0.0.9/carreiras_commons.egg-info/
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      923 2024-02-09 19:10:04.000000 carreiras-commons-0.0.9/carreiras_commons.egg-info/PKG-INFO
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      471 2024-02-09 19:10:04.000000 carreiras-commons-0.0.9/carreiras_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)        1 2024-02-09 19:10:04.000000 carreiras-commons-0.0.9/carreiras_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)       18 2024-02-09 19:10:04.000000 carreiras-commons-0.0.9/carreiras_commons.egg-info/top_level.txt
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)      106 2024-02-09 19:10:04.962705 carreiras-commons-0.0.9/setup.cfg
+-rw-r--r--   0 israelbrancomendonca   (501) staff       (20)     1041 2024-02-09 19:10:01.000000 carreiras-commons-0.0.9/setup.py
```

### Comparing `carreiras-commons-0.0.7/PKG-INFO` & `carreiras-commons-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carreiras-commons
-Version: 0.0.7
+Version: 0.0.9
 Summary: Common functions to carreiras projects
 Home-page: https://dev.azure.com/TITBrasil/Carreiras/_git/CARREIRAS-COMMON
 Author: HYTI
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Carreiras/_git/CARREIRAS-COMMON
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Carreiras/_git/CARREIRAS-COMMON
```

### Comparing `carreiras-commons-0.0.7/README.md` & `carreiras-commons-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `carreiras-commons-0.0.7/carreiras_commons/config.py` & `carreiras-commons-0.0.9/carreiras_commons/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 RABBITMQ_HOST = getenv('RABBITMQ_HOST', 'localhost')
 RABBITMQ_PORT = getenv('RABBITMQ_PORT', '5672')
 RABBITMQ_EXCHANGE = getenv('RABBITMQ_EXCHANGE', '')
 RABBITMQ_QUEUE_EMAIL = getenv('RABBITMQ_QUEUE', 'email')
 RABBITMQ_QUEUE_NOTIFICACAO = getenv('RABBITMQ_QUEUE', 'notificacoes')
 RABBITMQ_QUEUE_NOTIFICACAO_ADMIN = getenv('RABBITMQ_QUEUE', 'notificacoes_admin')
 
+SMTP_SERVER =  getenv('SMTP_SERVER', "smtp.gmail.com")
+SMTP_PORT = getenv('SMTP_PORT', 587)
+SMTP_USUERNAME = getenv('SMTP_USUERNAME', "teste@gmail.com") 
+SMTP_PASSWORD = getenv('SMTP_PASSWORD', "123") 
+SENDER_EMAIL = getenv('SENDER_EMAIL', "teste@gmail.com")  
+
 DEBUG = getenv('DEBUG',True)
 PORT = getenv('PORT',9090)
 
-DATABASE_PASSAOWRD = urllib.parse.quote_plus( getenv('DATABASE_PASSAOWRD', "U#aBrpd5873P!@sdRCMQW"))
-DATABASE_USER = getenv('DATABASE_USER', 'postgres')
-DATABASE_HOST = getenv('DATABASE_HOST', '20.83.136.185')
+DATABASE_PASSAOWRD = urllib.parse.quote_plus( getenv('DATABASE_PASSAOWRD', "123"))
+DATABASE_USER = getenv('DATABASE_USER', 'root')
+DATABASE_HOST = getenv('DATABASE_HOST', 'localhost')
 DATABASE_PORT = getenv('DATABASE_PORT', '5432')
-DATABASE_NAME = getenv('DATABASE_NAME', 'carreiras')
+DATABASE_NAME = getenv('DATABASE_NAME', 'bd')
 SQLALCHEMY_DATABASE_URI = f"postgresql://{DATABASE_USER}:{DATABASE_PASSAOWRD}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}"
 SQLALCHEMY_TRACK_MODIFICATIONS = False
```

### Comparing `carreiras-commons-0.0.7/carreiras_commons/messaging_email.py` & `carreiras-commons-0.0.9/carreiras_commons/messaging_email.py`

 * *Files identical despite different names*

### Comparing `carreiras-commons-0.0.7/carreiras_commons/messaging_notificacao.py` & `carreiras-commons-0.0.9/carreiras_commons/messaging_notificacao.py`

 * *Files identical despite different names*

### Comparing `carreiras-commons-0.0.7/carreiras_commons/messaging_notificacao_admin.py` & `carreiras-commons-0.0.9/carreiras_commons/messaging_notificacao_admin.py`

 * *Files identical despite different names*

### Comparing `carreiras-commons-0.0.7/carreiras_commons/notificacao_adm_enum.py` & `carreiras-commons-0.0.9/carreiras_commons/notificacao_adm_enum.py`

 * *Files identical despite different names*

### Comparing `carreiras-commons-0.0.7/carreiras_commons/notificacao_enum.py` & `carreiras-commons-0.0.9/carreiras_commons/notificacao_enum.py`

 * *Files identical despite different names*

### Comparing `carreiras-commons-0.0.7/carreiras_commons.egg-info/PKG-INFO` & `carreiras-commons-0.0.9/carreiras_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carreiras-commons
-Version: 0.0.7
+Version: 0.0.9
 Summary: Common functions to carreiras projects
 Home-page: https://dev.azure.com/TITBrasil/Carreiras/_git/CARREIRAS-COMMON
 Author: HYTI
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Carreiras/_git/CARREIRAS-COMMON
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Carreiras/_git/CARREIRAS-COMMON
```

### Comparing `carreiras-commons-0.0.7/setup.py` & `carreiras-commons-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='carreiras-commons',
-    version='0.0.7',
+    version='0.0.9',
     author='HYTI',
     author_email='contato@titcs.com.br',
     packages=['carreiras_commons'],
     description='Common functions to carreiras projects',
     long_description='Common functions to carreiras projects',
     url='https://dev.azure.com/TITBrasil/Carreiras/_git/CARREIRAS-COMMON',
     project_urls={
```

