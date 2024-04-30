# Comparing `tmp/automvs-0.0.2.tar.gz` & `tmp/automvs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.0.2.tar", last modified: Tue Jan 23 17:11:51 2024, max compression
+gzip compressed data, was "automvs-0.0.3.tar", last modified: Tue Apr 30 16:17:49 2024, max compression
```

## Comparing `automvs-0.0.2.tar` & `automvs-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-01-23 17:11:51.646511 automvs-0.0.2/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-01-23 16:37:21.000000 automvs-0.0.2/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     1449 2024-01-23 17:11:51.646511 automvs-0.0.2/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      956 2023-04-29 00:15:17.000000 automvs-0.0.2/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-01-23 17:11:51.646511 automvs-0.0.2/automvs/
--rw-rw-r--   0 phil      (1000) phil      (1000)    18527 2024-01-23 17:11:37.000000 automvs-0.0.2/automvs/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-01-23 17:11:51.646511 automvs-0.0.2/automvs.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1449 2024-01-23 17:11:51.000000 automvs-0.0.2/automvs.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-01-23 17:11:51.000000 automvs-0.0.2/automvs.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-01-23 17:11:51.000000 automvs-0.0.2/automvs.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-01-23 17:11:51.000000 automvs-0.0.2/automvs.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-01-23 17:11:51.646511 automvs-0.0.2/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-01-23 17:11:48.000000 automvs-0.0.2/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-30 16:17:49.364480 automvs-0.0.3/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.3/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-04-30 16:17:49.364480 automvs-0.0.3/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.3/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-30 16:17:49.364480 automvs-0.0.3/automvs/
+-rw-rw-r--   0 phil      (1000) phil      (1000)    19020 2024-04-30 16:16:50.000000 automvs-0.0.3/automvs/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-30 16:17:49.364480 automvs-0.0.3/automvs.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-04-30 16:17:49.000000 automvs-0.0.3/automvs.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-04-30 16:17:49.000000 automvs-0.0.3/automvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-04-30 16:17:49.000000 automvs-0.0.3/automvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-04-30 16:17:49.000000 automvs-0.0.3/automvs.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-04-30 16:17:49.364480 automvs-0.0.3/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-04-30 16:16:55.000000 automvs-0.0.3/setup.py
```

### Comparing `automvs-0.0.2/LICENSE` & `automvs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `automvs-0.0.2/PKG-INFO` & `automvs-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,8 +40,7 @@
     build.send_herc('devinit 170 tape/zdlib1.het')
     build.wait_for_string("IEF238D SMP4P44 - REPLY DEVICE NAME OR 'CANCEL'.")
     build.send_reply('170')
     build.send_oper("$DU")
 finally:
     build.quit_hercules()
 ```
-
```

### Comparing `automvs-0.0.2/README.md` & `automvs-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `automvs-0.0.2/automvs/__init__.py` & `automvs-0.0.3/automvs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     This library allows the use of MVS/CE in an automated fashion. This can
     be used for deploying XMI files, pushing out updates, building software,
     creating custom MVS deployments.
 
     Using this library requires a recent version of hercules SDL and MVS/CE.
 """
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 __author__ = 'Philip Young'
 __license__ = "GPL"
 
 # Copyright (c) 2021, Philip Young
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -475,7 +475,14 @@
         self.check_maxcc(jobname)
         
 
     def change_to_mvsce(self):
         self.logger.debug("[AUTOMATION] Changing to MVS/CE Folder {}".format(self.mvsce_location))
         os.chdir(self.mvsce_location)
 
+    def change_punchcard_output(self,path):
+        self.logger.debug("[AUTOMATION] Changing 3525 Punchcard output location to: '{}'".format(path))
+        if not os.path.exists(os.path.dirname(path)): 
+            self.logger.debug("[AUTOMATION] Punchcard folder '{}' does not exist".format(path))
+            raise Exception("Punchcard folder '{}' does no exist".format(path))
+        self.send_herc(command='detach d')
+        self.send_herc(command='attach d 3525 {} ebcdic'.format(path))
```

### Comparing `automvs-0.0.2/automvs.egg-info/PKG-INFO` & `automvs-0.0.3/automvs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,8 +40,7 @@
     build.send_herc('devinit 170 tape/zdlib1.het')
     build.wait_for_string("IEF238D SMP4P44 - REPLY DEVICE NAME OR 'CANCEL'.")
     build.send_reply('170')
     build.send_oper("$DU")
 finally:
     build.quit_hercules()
 ```
-
```

### Comparing `automvs-0.0.2/setup.py` & `automvs-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='automvs',
-    version='0.0.2',    
+    version='0.0.3',    
     description='Python library for MVS/CE automation',
     url='https://github.com/MVS-sysgen/automvs',
     author='Philip Young',
     author_email='mainframed767@gmail.com',
     license='MIT',
     packages=['automvs'],
     install_requires=[],
```

