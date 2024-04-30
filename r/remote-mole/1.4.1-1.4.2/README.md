# Comparing `tmp/remote_mole-1.4.1.tar.gz` & `tmp/remote_mole-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote_mole-1.4.1.tar", last modified: Wed Apr 24 21:53:07 2024, max compression
+gzip compressed data, was "remote_mole-1.4.2.tar", last modified: Tue Apr 30 18:20:00 2024, max compression
```

## Comparing `remote_mole-1.4.1.tar` & `remote_mole-1.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.267799 remote_mole-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    34451 2024-04-24 21:52:23.000000 remote_mole-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      865 2024-04-24 21:53:07.265798 remote_mole-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      534 2024-04-24 21:52:23.000000 remote_mole-1.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 21:53:07.267799 remote_mole-1.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-24 21:52:23.000000 remote_mole-1.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.249798 remote_mole-1.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.252798 remote_mole-1.4.1/src/remote_mole/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.259798 remote_mole-1.4.1/src/remote_mole/_internal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.260799 remote_mole-1.4.1/src/remote_mole/_internal/platforms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/platforms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.261798 remote_mole-1.4.1/src/remote_mole/_internal/platforms/discord/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/platforms/discord/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7349 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/platforms/discord/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.263799 remote_mole-1.4.1/src/remote_mole/_internal/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/services/lxi.py
--rw-rw-rw-   0 root         (0) root         (0)     2525 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/services/ngrok.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.264798 remote_mole-1.4.1/src/remote_mole/setup/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/setup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4201 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/setup/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.259798 remote_mole-1.4.1/src/remote_mole.egg-info/
--rw-r--r--   0 root         (0) root         (0)      865 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      661 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.345984 remote_mole-1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34451 2024-04-30 18:18:57.000000 remote_mole-1.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-30 18:20:00.342984 remote_mole-1.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      534 2024-04-30 18:18:57.000000 remote_mole-1.4.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 18:20:00.345984 remote_mole-1.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-30 18:18:57.000000 remote_mole-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.321984 remote_mole-1.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.324984 remote_mole-1.4.2/src/remote_mole/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.334984 remote_mole-1.4.2/src/remote_mole/_internal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/_internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.335984 remote_mole-1.4.2/src/remote_mole/_internal/platforms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/_internal/platforms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.337984 remote_mole-1.4.2/src/remote_mole/_internal/platforms/discord/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/_internal/platforms/discord/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7363 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/_internal/platforms/discord/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.339984 remote_mole-1.4.2/src/remote_mole/_internal/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/_internal/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/_internal/services/lxi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/_internal/services/ngrok.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.341984 remote_mole-1.4.2/src/remote_mole/setup/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/setup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4201 2024-04-30 18:18:57.000000 remote_mole-1.4.2/src/remote_mole/setup/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:20:00.333984 remote_mole-1.4.2/src/remote_mole.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-30 18:19:59.000000 remote_mole-1.4.2/src/remote_mole.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-30 18:20:00.000000 remote_mole-1.4.2/src/remote_mole.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 18:19:59.000000 remote_mole-1.4.2/src/remote_mole.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-30 18:19:59.000000 remote_mole-1.4.2/src/remote_mole.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-30 18:19:59.000000 remote_mole-1.4.2/src/remote_mole.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-30 18:19:59.000000 remote_mole-1.4.2/src/remote_mole.egg-info/top_level.txt
```

### Comparing `remote_mole-1.4.1/LICENSE` & `remote_mole-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.1/PKG-INFO` & `remote_mole-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote_mole
-Version: 1.4.1
+Version: 1.4.2
 Summary: Create moles on remote setups.
 Home-page: http://packages.python.org/remote_mole
 Author: ACESRG
 Author-email: aces.rg@gmail.com
 License: GPLv3
 Keywords: bots ssh jupyter ngrok discord
 Platform: UNKNOWN
```

### Comparing `remote_mole-1.4.1/README.md` & `remote_mole-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.1/setup.py` & `remote_mole-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="remote_mole",
-    version="1.4.1",
+    version="1.4.2",
     author="ACESRG",
     author_email="aces.rg@gmail.com",
     description=("Create moles on remote setups."),
     license="GPLv3",
     keywords="bots ssh jupyter ngrok discord",
     url="http://packages.python.org/remote_mole",
     packages=[
```

### Comparing `remote_mole-1.4.1/src/remote_mole/_internal/platforms/discord/daemon.py` & `remote_mole-1.4.2/src/remote_mole/_internal/platforms/discord/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         )
     elif tunnel_type == 'custom':
         return _format_string_as_code(
             f'The port 1209 was open on: {tunnel.address}'
         )
     elif tunnel_type == 'vnc':
         return _format_string_as_code(
-            f'You can access the device vnc on: {tunnel.address}'
+            f'You can access the device vnc on: {tunnel.address}:{tunnel.port}'
         )
     else:
         return _format_string_as_code(
             f'The port was open on: {tunnel.address}'
         )
```

### Comparing `remote_mole-1.4.1/src/remote_mole/_internal/services/lxi.py` & `remote_mole-1.4.2/src/remote_mole/_internal/services/lxi.py`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.1/src/remote_mole/_internal/services/ngrok.py` & `remote_mole-1.4.2/src/remote_mole/_internal/services/ngrok.py`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.1/src/remote_mole/setup/entrypoint.py` & `remote_mole-1.4.2/src/remote_mole/setup/entrypoint.py`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.1/src/remote_mole.egg-info/PKG-INFO` & `remote_mole-1.4.2/src/remote_mole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-mole
-Version: 1.4.1
+Version: 1.4.2
 Summary: Create moles on remote setups.
 Home-page: http://packages.python.org/remote_mole
 Author: ACESRG
 Author-email: aces.rg@gmail.com
 License: GPLv3
 Keywords: bots ssh jupyter ngrok discord
 Platform: UNKNOWN
```

### Comparing `remote_mole-1.4.1/src/remote_mole.egg-info/SOURCES.txt` & `remote_mole-1.4.2/src/remote_mole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

