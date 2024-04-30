# Comparing `tmp/pycomus-1.0.4.tar.gz` & `tmp/pycomus-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycomus-1.0.4.tar", last modified: Tue Apr 30 01:53:54 2024, max compression
+gzip compressed data, was "pycomus-1.1.tar", last modified: Tue Apr 30 01:59:17 2024, max compression
```

## Comparing `pycomus-1.0.4.tar` & `pycomus-1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.870367 pycomus-1.0.4/
--rw-rw-rw-   0        0        0     5166 2024-04-30 01:53:54.869351 pycomus-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.868322 pycomus-1.0.4/PyCOMUS.egg-info/
--rw-rw-rw-   0        0        0     5166 2024-04-30 01:53:54.000000 pycomus-1.0.4/PyCOMUS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1919 2024-04-30 01:53:54.000000 pycomus-1.0.4/PyCOMUS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 01:53:54.000000 pycomus-1.0.4/PyCOMUS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-30 01:53:54.000000 pycomus-1.0.4/PyCOMUS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4684 2024-04-18 01:48:26.000000 pycomus-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.316623 pycomus-1.0.4/RestfulApi/
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.318170 pycomus-1.0.4/RestfulApi/ComusApi/
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.354480 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/
--rw-rw-rw-   0        0        0        0 2024-03-18 00:44:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/__init__.py
--rw-rw-rw-   0        0        0      409 2024-03-18 00:44:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/asgi.py
--rw-rw-rw-   0        0        0     3930 2024-03-18 03:23:34.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/settings.py
--rw-rw-rw-   0        0        0      825 2024-03-18 00:54:12.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/urls.py
--rw-rw-rw-   0        0        0      409 2024-03-18 00:44:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.402192 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/
--rw-rw-rw-   0        0        0        0 2024-03-18 00:44:50.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-18 00:44:50.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/admin.py
--rw-rw-rw-   0        0        0      154 2024-03-18 07:41:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.408379 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/
--rw-rw-rw-   0        0        0     2954 2024-03-18 07:41:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      413 2024-03-18 07:41:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/0002_alter_comusctrlparsmodel_comus_dis_uuid.py
--rw-rw-rw-   0        0        0     1512 2024-03-18 07:41:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/0003_comusoutparsmodel.py
--rw-rw-rw-   0        0        0        0 2024-03-18 00:44:50.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/__init__.py
--rw-rw-rw-   0        0        0     2658 2024-03-18 08:09:54.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/models.py
--rw-rw-rw-   0        0        0     6044 2024-03-18 07:47:07.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/serializers.py
--rw-rw-rw-   0        0        0       63 2024-03-18 00:44:50.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/tests.py
--rw-rw-rw-   0        0        0      386 2024-03-18 07:32:07.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/urls.py
--rw-rw-rw-   0        0        0     5789 2024-03-18 08:07:45.000000 pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/views.py
--rw-rw-rw-   0        0        0        0 2024-03-18 03:39:00.000000 pycomus-1.0.4/RestfulApi/ComusApi/__init__.py
--rw-rw-rw-   0        0        0      686 2024-03-18 00:44:19.000000 pycomus-1.0.4/RestfulApi/ComusApi/manage.py
--rw-rw-rw-   0        0        0        0 2024-03-18 03:39:00.000000 pycomus-1.0.4/RestfulApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.408892 pycomus-1.0.4/pycomus/
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.466366 pycomus-1.0.4/pycomus/ComusDis/
--rw-rw-rw-   0        0        0     1813 2024-03-04 03:24:27.000000 pycomus-1.0.4/pycomus/ComusDis/CONSTANTS.py
--rw-rw-rw-   0        0        0    21568 2024-04-30 01:45:25.000000 pycomus-1.0.4/pycomus/ComusDis/CmsDis.py
--rw-rw-rw-   0        0        0    26311 2024-04-29 01:57:32.000000 pycomus-1.0.4/pycomus/ComusDis/CmsGridPars.py
--rw-rw-rw-   0        0        0     4842 2024-04-29 01:49:54.000000 pycomus-1.0.4/pycomus/ComusDis/CmsMd.py
--rw-rw-rw-   0        0        0     6648 2024-04-29 01:49:54.000000 pycomus-1.0.4/pycomus/ComusDis/CmsOutPars.py
--rw-rw-rw-   0        0        0    12197 2024-04-29 01:49:54.000000 pycomus-1.0.4/pycomus/ComusDis/CmsPars.py
--rw-rw-rw-   0        0        0     5597 2024-04-29 01:59:01.000000 pycomus-1.0.4/pycomus/ComusDis/CmsTime.py
--rw-rw-rw-   0        0        0      389 2024-02-07 03:08:10.000000 pycomus-1.0.4/pycomus/ComusDis/GridCell.py
--rw-rw-rw-   0        0        0      670 2024-02-05 03:51:34.000000 pycomus-1.0.4/pycomus/ComusDis/GridLyr.py
--rw-rw-rw-   0        0        0      221 2024-04-30 01:49:26.000000 pycomus-1.0.4/pycomus/ComusDis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.672317 pycomus-1.0.4/pycomus/Package/
--rw-rw-rw-   0        0        0     7972 2024-04-29 02:07:48.000000 pycomus-1.0.4/pycomus/Package/CDRN.py
--rw-rw-rw-   0        0        0    10485 2024-04-29 02:07:52.000000 pycomus-1.0.4/pycomus/Package/CEVT.py
--rw-rw-rw-   0        0        0     8343 2024-04-29 02:08:21.000000 pycomus-1.0.4/pycomus/Package/CGHB.py
--rw-rw-rw-   0        0        0     6240 2024-04-29 02:09:29.000000 pycomus-1.0.4/pycomus/Package/CHFB.py
--rw-rw-rw-   0        0        0     6132 2024-04-29 02:12:07.000000 pycomus-1.0.4/pycomus/Package/CIBS.py
--rw-rw-rw-   0        0        0    21602 2024-04-29 02:32:25.000000 pycomus-1.0.4/pycomus/Package/CLAK.py
--rw-rw-rw-   0        0        0     6632 2024-04-29 02:17:59.000000 pycomus-1.0.4/pycomus/Package/CRCH.py
--rw-rw-rw-   0        0        0     5371 2024-04-29 02:19:25.000000 pycomus-1.0.4/pycomus/Package/CREG.py
--rw-rw-rw-   0        0        0    15899 2024-04-29 02:33:20.000000 pycomus-1.0.4/pycomus/Package/CRES.py
--rw-rw-rw-   0        0        0     9861 2024-04-29 02:40:00.000000 pycomus-1.0.4/pycomus/Package/CRIV.py
--rw-rw-rw-   0        0        0     7323 2024-04-29 02:43:07.000000 pycomus-1.0.4/pycomus/Package/CSHB.py
--rw-rw-rw-   0        0        0    46089 2024-04-29 02:57:18.000000 pycomus-1.0.4/pycomus/Package/CSTR.py
--rw-rw-rw-   0        0        0    23849 2024-04-29 03:05:02.000000 pycomus-1.0.4/pycomus/Package/CSUB.py
--rw-rw-rw-   0        0        0     7702 2024-04-29 03:06:22.000000 pycomus-1.0.4/pycomus/Package/CWEL.py
--rw-rw-rw-   0        0        0      392 2024-02-22 01:12:55.000000 pycomus-1.0.4/pycomus/Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:53:54.867289 pycomus-1.0.4/pycomus/Utils/
--rw-rw-rw-   0        0        0     9516 2024-04-18 01:34:14.000000 pycomus-1.0.4/pycomus/Utils/BoundaryCheck.py
--rw-rw-rw-   0        0        0     1813 2024-03-04 03:24:27.000000 pycomus-1.0.4/pycomus/Utils/CONSTANTS.py
--rw-rw-rw-   0        0        0    19768 2024-03-15 02:33:52.000000 pycomus-1.0.4/pycomus/Utils/LinuxCheckParams.so
--rw-rw-rw-   0        0        0  2516512 2024-03-15 01:34:26.000000 pycomus-1.0.4/pycomus/Utils/LinuxComus.so
--rw-rw-rw-   0        0        0     5703 2024-04-29 03:23:40.000000 pycomus-1.0.4/pycomus/Utils/Map.py
--rw-rw-rw-   0        0        0    15272 2024-04-29 03:45:14.000000 pycomus-1.0.4/pycomus/Utils/ReadData.py
--rw-rw-rw-   0        0        0    13824 2024-02-05 02:25:25.000000 pycomus-1.0.4/pycomus/Utils/WinCheckParams.dll
--rw-rw-rw-   0        0        0   757760 2024-03-14 09:00:49.000000 pycomus-1.0.4/pycomus/Utils/WinComus.dll
--rw-rw-rw-   0        0        0       61 2024-03-05 07:43:35.000000 pycomus-1.0.4/pycomus/Utils/__init__.py
--rw-rw-rw-   0        0        0      172 2024-02-01 02:11:48.000000 pycomus-1.0.4/pycomus/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-30 01:53:54.870378 pycomus-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      948 2024-04-30 01:51:51.000000 pycomus-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.948591 pycomus-1.1/
+-rw-rw-rw-   0        0        0     5164 2024-04-30 01:59:17.947591 pycomus-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.946591 pycomus-1.1/PyCOMUS.egg-info/
+-rw-rw-rw-   0        0        0     5164 2024-04-30 01:59:17.000000 pycomus-1.1/PyCOMUS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2024-04-30 01:59:17.000000 pycomus-1.1/PyCOMUS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 01:59:17.000000 pycomus-1.1/PyCOMUS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-30 01:59:17.000000 pycomus-1.1/PyCOMUS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4684 2024-04-18 01:48:26.000000 pycomus-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.888756 pycomus-1.1/RestfulApi/
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.889782 pycomus-1.1/RestfulApi/ComusApi/
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.893381 pycomus-1.1/RestfulApi/ComusApi/ComusApi/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:44:19.000000 pycomus-1.1/RestfulApi/ComusApi/ComusApi/__init__.py
+-rw-rw-rw-   0        0        0      409 2024-03-18 00:44:19.000000 pycomus-1.1/RestfulApi/ComusApi/ComusApi/asgi.py
+-rw-rw-rw-   0        0        0     3930 2024-03-18 03:23:34.000000 pycomus-1.1/RestfulApi/ComusApi/ComusApi/settings.py
+-rw-rw-rw-   0        0        0      825 2024-03-18 00:54:12.000000 pycomus-1.1/RestfulApi/ComusApi/ComusApi/urls.py
+-rw-rw-rw-   0        0        0      409 2024-03-18 00:44:19.000000 pycomus-1.1/RestfulApi/ComusApi/ComusApi/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.899705 pycomus-1.1/RestfulApi/ComusApi/ComusDis/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:44:50.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-18 00:44:50.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/admin.py
+-rw-rw-rw-   0        0        0      154 2024-03-18 07:41:19.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.902868 pycomus-1.1/RestfulApi/ComusApi/ComusDis/migrations/
+-rw-rw-rw-   0        0        0     2954 2024-03-18 07:41:19.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      413 2024-03-18 07:41:19.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/migrations/0002_alter_comusctrlparsmodel_comus_dis_uuid.py
+-rw-rw-rw-   0        0        0     1512 2024-03-18 07:41:19.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/migrations/0003_comusoutparsmodel.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:44:50.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2658 2024-03-18 08:09:54.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/models.py
+-rw-rw-rw-   0        0        0     6044 2024-03-18 07:47:07.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/serializers.py
+-rw-rw-rw-   0        0        0       63 2024-03-18 00:44:50.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/tests.py
+-rw-rw-rw-   0        0        0      386 2024-03-18 07:32:07.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/urls.py
+-rw-rw-rw-   0        0        0     5789 2024-03-18 08:07:45.000000 pycomus-1.1/RestfulApi/ComusApi/ComusDis/views.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 03:39:00.000000 pycomus-1.1/RestfulApi/ComusApi/__init__.py
+-rw-rw-rw-   0        0        0      686 2024-03-18 00:44:19.000000 pycomus-1.1/RestfulApi/ComusApi/manage.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 03:39:00.000000 pycomus-1.1/RestfulApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.903901 pycomus-1.1/pycomus/
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.912127 pycomus-1.1/pycomus/ComusDis/
+-rw-rw-rw-   0        0        0     1813 2024-03-04 03:24:27.000000 pycomus-1.1/pycomus/ComusDis/CONSTANTS.py
+-rw-rw-rw-   0        0        0    21676 2024-04-30 01:59:05.000000 pycomus-1.1/pycomus/ComusDis/CmsDis.py
+-rw-rw-rw-   0        0        0    26311 2024-04-29 01:57:32.000000 pycomus-1.1/pycomus/ComusDis/CmsGridPars.py
+-rw-rw-rw-   0        0        0     4842 2024-04-29 01:49:54.000000 pycomus-1.1/pycomus/ComusDis/CmsMd.py
+-rw-rw-rw-   0        0        0     6648 2024-04-29 01:49:54.000000 pycomus-1.1/pycomus/ComusDis/CmsOutPars.py
+-rw-rw-rw-   0        0        0    12197 2024-04-29 01:49:54.000000 pycomus-1.1/pycomus/ComusDis/CmsPars.py
+-rw-rw-rw-   0        0        0     5597 2024-04-29 01:59:01.000000 pycomus-1.1/pycomus/ComusDis/CmsTime.py
+-rw-rw-rw-   0        0        0      389 2024-02-07 03:08:10.000000 pycomus-1.1/pycomus/ComusDis/GridCell.py
+-rw-rw-rw-   0        0        0      670 2024-02-05 03:51:34.000000 pycomus-1.1/pycomus/ComusDis/GridLyr.py
+-rw-rw-rw-   0        0        0      221 2024-04-30 01:49:26.000000 pycomus-1.1/pycomus/ComusDis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.925595 pycomus-1.1/pycomus/Package/
+-rw-rw-rw-   0        0        0     7972 2024-04-29 02:07:48.000000 pycomus-1.1/pycomus/Package/CDRN.py
+-rw-rw-rw-   0        0        0    10485 2024-04-29 02:07:52.000000 pycomus-1.1/pycomus/Package/CEVT.py
+-rw-rw-rw-   0        0        0     8343 2024-04-29 02:08:21.000000 pycomus-1.1/pycomus/Package/CGHB.py
+-rw-rw-rw-   0        0        0     6240 2024-04-29 02:09:29.000000 pycomus-1.1/pycomus/Package/CHFB.py
+-rw-rw-rw-   0        0        0     6132 2024-04-29 02:12:07.000000 pycomus-1.1/pycomus/Package/CIBS.py
+-rw-rw-rw-   0        0        0    21602 2024-04-29 02:32:25.000000 pycomus-1.1/pycomus/Package/CLAK.py
+-rw-rw-rw-   0        0        0     6632 2024-04-29 02:17:59.000000 pycomus-1.1/pycomus/Package/CRCH.py
+-rw-rw-rw-   0        0        0     5371 2024-04-29 02:19:25.000000 pycomus-1.1/pycomus/Package/CREG.py
+-rw-rw-rw-   0        0        0    15899 2024-04-29 02:33:20.000000 pycomus-1.1/pycomus/Package/CRES.py
+-rw-rw-rw-   0        0        0     9861 2024-04-29 02:40:00.000000 pycomus-1.1/pycomus/Package/CRIV.py
+-rw-rw-rw-   0        0        0     7323 2024-04-29 02:43:07.000000 pycomus-1.1/pycomus/Package/CSHB.py
+-rw-rw-rw-   0        0        0    46089 2024-04-29 02:57:18.000000 pycomus-1.1/pycomus/Package/CSTR.py
+-rw-rw-rw-   0        0        0    23849 2024-04-29 03:05:02.000000 pycomus-1.1/pycomus/Package/CSUB.py
+-rw-rw-rw-   0        0        0     7702 2024-04-29 03:06:22.000000 pycomus-1.1/pycomus/Package/CWEL.py
+-rw-rw-rw-   0        0        0      392 2024-02-22 01:12:55.000000 pycomus-1.1/pycomus/Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 01:59:17.945591 pycomus-1.1/pycomus/Utils/
+-rw-rw-rw-   0        0        0     9516 2024-04-18 01:34:14.000000 pycomus-1.1/pycomus/Utils/BoundaryCheck.py
+-rw-rw-rw-   0        0        0     1813 2024-03-04 03:24:27.000000 pycomus-1.1/pycomus/Utils/CONSTANTS.py
+-rw-rw-rw-   0        0        0    19768 2024-03-15 02:33:52.000000 pycomus-1.1/pycomus/Utils/LinuxCheckParams.so
+-rw-rw-rw-   0        0        0  2516512 2024-03-15 01:34:26.000000 pycomus-1.1/pycomus/Utils/LinuxComus.so
+-rw-rw-rw-   0        0        0     5703 2024-04-29 03:23:40.000000 pycomus-1.1/pycomus/Utils/Map.py
+-rw-rw-rw-   0        0        0    15272 2024-04-29 03:45:14.000000 pycomus-1.1/pycomus/Utils/ReadData.py
+-rw-rw-rw-   0        0        0    13824 2024-02-05 02:25:25.000000 pycomus-1.1/pycomus/Utils/WinCheckParams.dll
+-rw-rw-rw-   0        0        0   757760 2024-03-14 09:00:49.000000 pycomus-1.1/pycomus/Utils/WinComus.dll
+-rw-rw-rw-   0        0        0       61 2024-03-05 07:43:35.000000 pycomus-1.1/pycomus/Utils/__init__.py
+-rw-rw-rw-   0        0        0      172 2024-02-01 02:11:48.000000 pycomus-1.1/pycomus/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 01:59:17.948591 pycomus-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-04-30 01:59:15.000000 pycomus-1.1/setup.py
```

### Comparing `pycomus-1.0.4/PKG-INFO` & `pycomus-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCOMUS
-Version: 1.0.4
+Version: 1.1
 Summary: A Python library for invoking the COMUS model for groundwater numerical simulation.
 Home-page: https://github.com/ZhenjiangWuHydro/PyCOMUS
 Author: Zhenjiang Wu
 Author-email: zhenjiangwu613@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycomus-1.0.4/PyCOMUS.egg-info/PKG-INFO` & `pycomus-1.1/PyCOMUS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCOMUS
-Version: 1.0.4
+Version: 1.1
 Summary: A Python library for invoking the COMUS model for groundwater numerical simulation.
 Home-page: https://github.com/ZhenjiangWuHydro/PyCOMUS
 Author: Zhenjiang Wu
 Author-email: zhenjiangwu613@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycomus-1.0.4/PyCOMUS.egg-info/SOURCES.txt` & `pycomus-1.1/PyCOMUS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/README.md` & `pycomus-1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/settings.py` & `pycomus-1.1/RestfulApi/ComusApi/ComusApi/settings.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/RestfulApi/ComusApi/ComusApi/urls.py` & `pycomus-1.1/RestfulApi/ComusApi/ComusApi/urls.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/0001_initial.py` & `pycomus-1.1/RestfulApi/ComusApi/ComusDis/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/migrations/0003_comusoutparsmodel.py` & `pycomus-1.1/RestfulApi/ComusApi/ComusDis/migrations/0003_comusoutparsmodel.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/models.py` & `pycomus-1.1/RestfulApi/ComusApi/ComusDis/models.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/serializers.py` & `pycomus-1.1/RestfulApi/ComusApi/ComusDis/serializers.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/RestfulApi/ComusApi/ComusDis/views.py` & `pycomus-1.1/RestfulApi/ComusApi/ComusDis/views.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/RestfulApi/ComusApi/manage.py` & `pycomus-1.1/RestfulApi/ComusApi/manage.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/ComusDis/CONSTANTS.py` & `pycomus-1.1/pycomus/ComusDis/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/ComusDis/CmsDis.py` & `pycomus-1.1/pycomus/ComusDis/CmsDis.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # Version: 1.0.0
 # Author: Zhenjiang Wu
 # Description: Set COMUS Model LPF Or BCF Layer Property.
 # --------------------------------------------------------------
 import os
 from typing import List, Union, Tuple
 
-from GridCell import GridCell
-from GridLyr import LpfLayers, BcfLayers
-from CONSTANTS import LPF_LYR_FILE_NAME, BCF_LYR_FILE_NAME, LPF_LYR_PKG_NAME, BCF_LYR_PKG_NAME, \
+import pycomus
+from pycomus.ComusDis.GridCell import GridCell
+from pycomus.ComusDis.GridLyr import LpfLayers, BcfLayers
+from pycomus.Utils.CONSTANTS import LPF_LYR_FILE_NAME, BCF_LYR_FILE_NAME, LPF_LYR_PKG_NAME, BCF_LYR_PKG_NAME, \
     GRID_SPACE_FILE_NAME, CON_PKG_NAME
 
 
 class ComusDis:
     """
     Base Class
     """
@@ -196,15 +197,15 @@
     """
 
     def __init__(self, model, num_lyr: int = 1, num_row: int = 1, num_col: int = 1,
                  row_space: Union[float, int, List[float]] = 1, col_space: Union[float, int, List[float]] = 1,
                  x_coord: float = 0, y_coord: float = 0, lyr_type: List[int] = None, lyr_cbd: List[int] = None,
                  lyr_ibs: List[int] = None):
         super().__init__(model, num_lyr, num_row, num_col, x_coord, y_coord, row_space, col_space)
-        cms_pars = model.package[CON_PKG_NAME]
+        cms_pars: pycomus.ComusConPars = model.package[CON_PKG_NAME]
         if cms_pars.intblkm == 1:
             raise ValueError("In BCF format has been selected, it is not possible to add layers in LPF format.")
         if not lyr_type:
             lyr_type: List[int] = [0] * num_lyr
         if not lyr_cbd:
             lyr_cbd: List[int] = [0] * num_lyr
         if not lyr_ibs:
@@ -257,15 +258,15 @@
         Example:
         --------
         >>> import pycomus
         >>> model1 = pycomus.ComusModel(model_name="test")
         >>> modelDis = pycomus.ComusDisLpf.load(model1, "./InputFiles/CtrlPar.in", "./InputFiles/GrdSpace.in", "./InputFiles/LpfLyr.in")
         """
         # Check INTBLKM
-        cms_pars = model.package[CON_PKG_NAME]
+        cms_pars: pycomus.ComusConPars = model.package[CON_PKG_NAME]
         if cms_pars.intblkm == 1:
             raise ValueError("In BCF format has been selected, it is not possible to add layers in LPF format.")
 
         # Check Control Params
         num_lyr, num_row, num_col, x_coord, y_coord = ComusDis._load_control_params(ctrl_params_file)
 
         # Check Grid Space Params
```

### Comparing `pycomus-1.0.4/pycomus/ComusDis/CmsGridPars.py` & `pycomus-1.1/pycomus/ComusDis/CmsGridPars.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/ComusDis/CmsMd.py` & `pycomus-1.1/pycomus/ComusDis/CmsMd.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/ComusDis/CmsOutPars.py` & `pycomus-1.1/pycomus/ComusDis/CmsOutPars.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/ComusDis/CmsPars.py` & `pycomus-1.1/pycomus/ComusDis/CmsPars.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/ComusDis/CmsTime.py` & `pycomus-1.1/pycomus/ComusDis/CmsTime.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/ComusDis/GridLyr.py` & `pycomus-1.1/pycomus/ComusDis/GridLyr.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CDRN.py` & `pycomus-1.1/pycomus/Package/CDRN.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CEVT.py` & `pycomus-1.1/pycomus/Package/CEVT.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CGHB.py` & `pycomus-1.1/pycomus/Package/CGHB.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CHFB.py` & `pycomus-1.1/pycomus/Package/CHFB.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CIBS.py` & `pycomus-1.1/pycomus/Package/CIBS.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CLAK.py` & `pycomus-1.1/pycomus/Package/CLAK.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CRCH.py` & `pycomus-1.1/pycomus/Package/CRCH.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CREG.py` & `pycomus-1.1/pycomus/Package/CREG.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CRES.py` & `pycomus-1.1/pycomus/Package/CRES.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CRIV.py` & `pycomus-1.1/pycomus/Package/CRIV.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CSHB.py` & `pycomus-1.1/pycomus/Package/CSHB.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CSTR.py` & `pycomus-1.1/pycomus/Package/CSTR.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CSUB.py` & `pycomus-1.1/pycomus/Package/CSUB.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Package/CWEL.py` & `pycomus-1.1/pycomus/Package/CWEL.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Utils/BoundaryCheck.py` & `pycomus-1.1/pycomus/Utils/BoundaryCheck.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Utils/CONSTANTS.py` & `pycomus-1.1/pycomus/Utils/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Utils/LinuxCheckParams.so` & `pycomus-1.1/pycomus/Utils/LinuxCheckParams.so`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Utils/LinuxComus.so` & `pycomus-1.1/pycomus/Utils/LinuxComus.so`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Utils/Map.py` & `pycomus-1.1/pycomus/Utils/Map.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Utils/ReadData.py` & `pycomus-1.1/pycomus/Utils/ReadData.py`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Utils/WinCheckParams.dll` & `pycomus-1.1/pycomus/Utils/WinCheckParams.dll`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/pycomus/Utils/WinComus.dll` & `pycomus-1.1/pycomus/Utils/WinComus.dll`

 * *Files identical despite different names*

### Comparing `pycomus-1.0.4/setup.py` & `pycomus-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyCOMUS",
-    version="1.0.4",
+    version="1.1",
     author="Zhenjiang Wu",
     author_email="zhenjiangwu613@gmail.com",
     description="A Python library for invoking the COMUS model for groundwater numerical simulation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ZhenjiangWuHydro/PyCOMUS",
     packages=setuptools.find_packages(exclude=['Example*', 'tests*', 'docs*', 'build*', 'dist*', '.idea*', '.gitignore', 'README.md','ComusModel','paper','CheckParam']),
```

