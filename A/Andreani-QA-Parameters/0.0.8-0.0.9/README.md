# Comparing `tmp/Andreani_QA_Parameters-0.0.8.tar.gz` & `tmp/Andreani_QA_Parameters-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Parameters-0.0.8.tar", last modified: Fri Aug  4 19:29:11 2023, max compression
+gzip compressed data, was "Andreani_QA_Parameters-0.0.9.tar", last modified: Tue Aug  8 19:32:57 2023, max compression
```

## Comparing `Andreani_QA_Parameters-0.0.8.tar` & `Andreani_QA_Parameters-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 19:29:11.097780 Andreani_QA_Parameters-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-08-04 19:29:11.086084 Andreani_QA_Parameters-0.0.8/Andreani_QA_Parameters.egg-info/
--rw-rw-rw-   0        0        0      278 2023-08-04 19:29:10.000000 Andreani_QA_Parameters-0.0.8/Andreani_QA_Parameters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-08-04 19:29:11.000000 Andreani_QA_Parameters-0.0.8/Andreani_QA_Parameters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 19:29:10.000000 Andreani_QA_Parameters-0.0.8/Andreani_QA_Parameters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-04 19:29:10.000000 Andreani_QA_Parameters-0.0.8/Andreani_QA_Parameters.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 19:29:11.093350 Andreani_QA_Parameters-0.0.8/Andreani_QA_parameters/
--rw-rw-rw-   0        0        0     2753 2023-08-04 18:20:53.000000 Andreani_QA_Parameters-0.0.8/Andreani_QA_parameters/Parameters.py
--rw-rw-rw-   0        0        0       36 2023-07-17 18:24:05.000000 Andreani_QA_Parameters-0.0.8/Andreani_QA_parameters/__init__.py
--rw-rw-rw-   0        0        0      278 2023-08-04 19:29:11.096361 Andreani_QA_Parameters-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 19:29:11.097780 Andreani_QA_Parameters-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1183 2023-08-04 19:26:15.000000 Andreani_QA_Parameters-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:32:57.985913 Andreani_QA_Parameters-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-08-08 19:32:57.967023 Andreani_QA_Parameters-0.0.9/Andreani_QA_Parameters.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-08-08 19:32:57.000000 Andreani_QA_Parameters-0.0.9/Andreani_QA_Parameters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-08-08 19:32:57.000000 Andreani_QA_Parameters-0.0.9/Andreani_QA_Parameters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 19:32:57.000000 Andreani_QA_Parameters-0.0.9/Andreani_QA_Parameters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-08 19:32:57.000000 Andreani_QA_Parameters-0.0.9/Andreani_QA_Parameters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 19:32:57.978529 Andreani_QA_Parameters-0.0.9/Andreani_QA_parameters/
+-rw-rw-rw-   0        0        0     2800 2023-08-08 19:31:31.000000 Andreani_QA_Parameters-0.0.9/Andreani_QA_parameters/Parameters.py
+-rw-rw-rw-   0        0        0       36 2023-07-17 18:24:05.000000 Andreani_QA_Parameters-0.0.9/Andreani_QA_parameters/__init__.py
+-rw-rw-rw-   0        0        0      278 2023-08-08 19:32:57.984506 Andreani_QA_Parameters-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Parameters-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 19:32:57.987067 Andreani_QA_Parameters-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2023-08-08 19:31:31.000000 Andreani_QA_Parameters-0.0.9/setup.py
```

### Comparing `Andreani_QA_Parameters-0.0.8/Andreani_QA_parameters/Parameters.py` & `Andreani_QA_Parameters-0.0.9/Andreani_QA_parameters/Parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import platform
+import sys
 
 
 class Parameters:
     # CONFIGURACION PATH Y TESTCASE
     current_path = os.path.abspath(os.path.join(os.getcwd(), "../.."))
+    sys.path.append(current_path)
     file_name_stored = None
     env = None
 
     # CONFIGURACION PARA UTILIZAR CSV DESDE SHAREPOINT
     #sharepoint_data_jmeter=None
 
     # CONFIGURACION FORMATO DE FECHA
```

### Comparing `Andreani_QA_Parameters-0.0.8/setup.py` & `Andreani_QA_Parameters-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.8'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.9'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'Andreani_QA_Parameters'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Parametros + Encriptor para ejecución de casos automatizados'  # Descripción corta
```

