# Comparing `tmp/journeylib-1.0.0.tar.gz` & `tmp/journeylib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journeylib-1.0.0.tar", last modified: Tue Apr 30 07:19:08 2024, max compression
+gzip compressed data, was "journeylib-1.0.1.tar", last modified: Tue Apr 30 09:18:30 2024, max compression
```

## Comparing `journeylib-1.0.0.tar` & `journeylib-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 07:19:07.992721 journeylib-1.0.0/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      409 2024-04-30 07:19:07.990302 journeylib-1.0.0/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       57 2024-04-18 11:07:57.000000 journeylib-1.0.0/README.md
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 07:19:07.794607 journeylib-1.0.0/journeylib/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-1.0.0/journeylib/__init__.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      845 2024-04-30 07:17:48.000000 journeylib-1.0.0/journeylib/funciones.py
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 07:19:07.947096 journeylib-1.0.0/journeylib.egg-info/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      409 2024-04-30 07:19:07.000000 journeylib-1.0.0/journeylib.egg-info/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      201 2024-04-30 07:19:07.000000 journeylib-1.0.0/journeylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-04-30 07:19:07.000000 journeylib-1.0.0/journeylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-04-30 07:19:07.000000 journeylib-1.0.0/journeylib.egg-info/top_level.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-04-30 07:19:07.996230 journeylib-1.0.0/setup.cfg
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1347 2024-04-30 07:18:32.000000 journeylib-1.0.0/setup.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 09:18:30.201031 journeylib-1.0.1/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      409 2024-04-30 09:18:30.201031 journeylib-1.0.1/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       57 2024-04-18 11:07:57.000000 journeylib-1.0.1/README.md
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 09:18:29.939325 journeylib-1.0.1/journeylib/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-1.0.1/journeylib/__init__.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      820 2024-04-30 09:12:36.000000 journeylib-1.0.1/journeylib/funciones.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 09:18:30.151466 journeylib-1.0.1/journeylib.egg-info/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      409 2024-04-30 09:18:29.000000 journeylib-1.0.1/journeylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      234 2024-04-30 09:18:29.000000 journeylib-1.0.1/journeylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-04-30 09:18:29.000000 journeylib-1.0.1/journeylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-04-30 09:18:29.000000 journeylib-1.0.1/journeylib.egg-info/requires.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-04-30 09:18:29.000000 journeylib-1.0.1/journeylib.egg-info/top_level.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-04-30 09:18:30.208092 journeylib-1.0.1/setup.cfg
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-04-30 09:17:50.000000 journeylib-1.0.1/setup.py
```

### Comparing `journeylib-1.0.0/setup.py` & `journeylib-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.0' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
+VERSION = '1.0.1' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
 PACKAGE_NAME = 'journeylib' #Nombre de la libreria
 AUTHOR = 'Equipo JourneyGen UPM' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'f.gonzalez.lopez@alumnos.upm.es' #Modificar con vuestros datos
 URL = 'https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Libreria para gestionar datos del historico del proyecto GPTravel' #Descripción corta
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-      #'pymupdf'
+    'fastapi',
+    'requests'
       ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

