# Comparing `tmp/journeylib-0.1.1.tar.gz` & `tmp/journeylib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journeylib-0.1.1.tar", last modified: Thu Apr 25 11:23:55 2024, max compression
+gzip compressed data, was "journeylib-1.0.0.tar", last modified: Tue Apr 30 07:19:08 2024, max compression
```

## Comparing `journeylib-0.1.1.tar` & `journeylib-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-25 11:23:55.278169 journeylib-0.1.1/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      409 2024-04-25 11:23:55.269761 journeylib-0.1.1/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       57 2024-04-18 11:07:57.000000 journeylib-0.1.1/README.md
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-25 11:23:55.111265 journeylib-0.1.1/journeylib/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-0.1.1/journeylib/__init__.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      731 2024-04-25 11:15:19.000000 journeylib-0.1.1/journeylib/funciones.py
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-25 11:23:55.236725 journeylib-0.1.1/journeylib.egg-info/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      409 2024-04-25 11:23:54.000000 journeylib-0.1.1/journeylib.egg-info/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      201 2024-04-25 11:23:54.000000 journeylib-0.1.1/journeylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-04-25 11:23:54.000000 journeylib-0.1.1/journeylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-04-25 11:23:54.000000 journeylib-0.1.1/journeylib.egg-info/top_level.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-04-25 11:23:55.278169 journeylib-0.1.1/setup.cfg
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1347 2024-04-25 11:23:29.000000 journeylib-0.1.1/setup.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 07:19:07.992721 journeylib-1.0.0/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      409 2024-04-30 07:19:07.990302 journeylib-1.0.0/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       57 2024-04-18 11:07:57.000000 journeylib-1.0.0/README.md
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 07:19:07.794607 journeylib-1.0.0/journeylib/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-1.0.0/journeylib/__init__.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      845 2024-04-30 07:17:48.000000 journeylib-1.0.0/journeylib/funciones.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-04-30 07:19:07.947096 journeylib-1.0.0/journeylib.egg-info/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      409 2024-04-30 07:19:07.000000 journeylib-1.0.0/journeylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      201 2024-04-30 07:19:07.000000 journeylib-1.0.0/journeylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-04-30 07:19:07.000000 journeylib-1.0.0/journeylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-04-30 07:19:07.000000 journeylib-1.0.0/journeylib.egg-info/top_level.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-04-30 07:19:07.996230 journeylib-1.0.0/setup.cfg
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1347 2024-04-30 07:18:32.000000 journeylib-1.0.0/setup.py
```

### Comparing `journeylib-0.1.1/setup.py` & `journeylib-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.1' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
+VERSION = '1.0.0' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
 PACKAGE_NAME = 'journeylib' #Nombre de la libreria
 AUTHOR = 'Equipo JourneyGen UPM' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'f.gonzalez.lopez@alumnos.upm.es' #Modificar con vuestros datos
 URL = 'https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Libreria para gestionar datos del historico del proyecto GPTravel' #Descripción corta
```

