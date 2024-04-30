# Comparing `tmp/monisha-0.0.59.tar.gz` & `tmp/monisha-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.59.tar", last modified: Thu Apr 25 13:26:43 2024, max compression
+gzip compressed data, was "monisha-0.0.60.tar", last modified: Tue Apr 30 06:23:29 2024, max compression
```

## Comparing `monisha-0.0.59.tar` & `monisha-0.0.60.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.623930 monisha-0.0.59/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-25 13:26:36.000000 monisha-0.0.59/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.619930 monisha-0.0.59/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.623930 monisha-0.0.59/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function18.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.623930 monisha-0.0.59/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 13:26:43.623930 monisha-0.0.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 13:26:36.000000 monisha-0.0.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.623930 monisha-0.0.59/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:26:43.623930 monisha-0.0.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-25 13:26:36.000000 monisha-0.0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.563874 monisha-0.0.60/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 06:23:21.000000 monisha-0.0.60/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.555874 monisha-0.0.60/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.559874 monisha-0.0.60/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function18.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.559874 monisha-0.0.60/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 06:23:29.563874 monisha-0.0.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 06:23:21.000000 monisha-0.0.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.559874 monisha-0.0.60/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:23:29.563874 monisha-0.0.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 06:23:21.000000 monisha-0.0.60/setup.py
```

### Comparing `monisha-0.0.59/LICENSE` & `monisha-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/__init__.py` & `monisha-0.0.60/Monisha/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 appname = "monisha"
-version = "0.0.59"
+version = "0.0.60"
 
-install = ["python-magic"]
+install = ["hachoir"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

### Comparing `monisha-0.0.59/Monisha/functions/__init__.py` & `monisha-0.0.60/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function01.py` & `monisha-0.0.60/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function02.py` & `monisha-0.0.60/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function03.py` & `monisha-0.0.60/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function06.py` & `monisha-0.0.60/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function07.py` & `monisha-0.0.60/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function10.py` & `monisha-0.0.60/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function14.py` & `monisha-0.0.60/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function15.py` & `monisha-0.0.60/Monisha/functions/function15.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,23 @@
         self.filesize = kwargs.get('filesize', 0)
         self.location = kwargs.get('location', None)
 
 #=================================================================================================
 
 class Location:
 
+    async def get00(dlocation, files=[]):
+        for patho in sorted(os.listdir(dlocation)):
+            filez = os.path.join(dlocation, patho)
+            files.append(filez)
+
+        return files
+
+#=================================================================================================
+
     async def get01(flocation, exo):
         try:
             location = str(flocation)
             filesize = int(os.path.getsize(location))
             return Messages(location=location, filesize=filesize)
         except Exception:
             pass
```

### Comparing `monisha-0.0.59/Monisha/functions/function16.py` & `monisha-0.0.60/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function17.py` & `monisha-0.0.60/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/functions/function18.py` & `monisha-0.0.60/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/Monisha/scripts/es.py` & `monisha-0.0.60/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/PKG-INFO` & `monisha-0.0.60/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.59
+Version: 0.0.60
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
@@ -15,12 +15,12 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python-magic
+Requires-Dist: hachoir
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.59 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.60 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-python-magic
+hachoir
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.59/monisha.egg-info/PKG-INFO` & `monisha-0.0.60/monisha.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.59
+Version: 0.0.60
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
@@ -15,12 +15,12 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python-magic
+Requires-Dist: hachoir
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.59 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.60 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-python-magic
+hachoir
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.59/monisha.egg-info/SOURCES.txt` & `monisha-0.0.60/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.59/setup.py` & `monisha-0.0.60/setup.py`

 * *Files identical despite different names*

