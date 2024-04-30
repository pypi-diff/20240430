# Comparing `tmp/SleepHarmonizer-0.1.4.tar.gz` & `tmp/SleepHarmonizer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SleepHarmonizer-0.1.4.tar", last modified: Wed Apr 24 10:19:26 2024, max compression
+gzip compressed data, was "SleepHarmonizer-0.1.5.tar", last modified: Tue Apr 30 07:14:23 2024, max compression
```

## Comparing `SleepHarmonizer-0.1.4.tar` & `SleepHarmonizer-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 10:19:26.759562 SleepHarmonizer-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9049 2024-04-24 10:19:26.758562 SleepHarmonizer-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8562 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 10:19:26.753562 SleepHarmonizer-0.1.4/SleepHarmonizer/
--rw-rw-rw-   0 root         (0) root         (0)     4184 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/EDFWriter.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/PSGEventManager.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6744 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 10:19:26.754562 SleepHarmonizer-0.1.4/SleepHarmonizer/phases/
--rw-rw-rw-   0 root         (0) root         (0)     4077 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/phases/Export.py
--rw-rw-rw-   0 root         (0) root         (0)     3547 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/phases/LoadData.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/phases/Setup.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/phases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 10:19:26.756562 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/
--rwxrwxrwx   0 root         (0) root         (0)    12683 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/AliceRMLLoader.py
--rw-rw-rw-   0 root         (0) root         (0)    11246 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/AliceTextReportLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     4568 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     8335 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py
--rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/DominoErgLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     7126 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/RecordLoaderAlice.py
--rw-rw-rw-   0 root         (0) root         (0)     5374 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/RecordLoaderDomino.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/RecordLoaderTest.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 10:19:26.754562 SleepHarmonizer-0.1.4/SleepHarmonizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9049 2024-04-24 10:19:26.000000 SleepHarmonizer-0.1.4/SleepHarmonizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1217 2024-04-24 10:19:26.000000 SleepHarmonizer-0.1.4/SleepHarmonizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 10:19:26.000000 SleepHarmonizer-0.1.4/SleepHarmonizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      153 2024-04-24 10:19:26.000000 SleepHarmonizer-0.1.4/SleepHarmonizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-24 10:19:26.000000 SleepHarmonizer-0.1.4/SleepHarmonizer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 10:19:26.759562 SleepHarmonizer-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-04-24 10:18:53.000000 SleepHarmonizer-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 10:19:26.756562 SleepHarmonizer-0.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 10:19:26.758562 SleepHarmonizer-0.1.4/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/tests/unit/test_Export.py
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/tests/unit/test_LoadData.py
--rwxrwxrwx   0 root         (0) root         (0)     1016 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/tests/unit/test_Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/tests/unit/test_Setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-24 10:18:52.000000 SleepHarmonizer-0.1.4/tests/unit/test_SignalPreprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.352892 SleepHarmonizer-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9049 2024-04-30 07:14:23.352892 SleepHarmonizer-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8562 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.347894 SleepHarmonizer-0.1.5/SleepHarmonizer/
+-rw-rw-rw-   0 root         (0) root         (0)     4184 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/EDFWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/PSGEventManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6744 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.349893 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/
+-rw-rw-rw-   0 root         (0) root         (0)     4077 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/Export.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/LoadData.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/Setup.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.350893 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/
+-rwxrwxrwx   0 root         (0) root         (0)    12683 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/AliceRMLLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)    11246 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/AliceTextReportLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     4568 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     8335 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoErgLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7126 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderAlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5374 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderDomino.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderTest.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.348894 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9049 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 07:14:23.352892 SleepHarmonizer-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-04-30 07:13:50.000000 SleepHarmonizer-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.351893 SleepHarmonizer-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.352892 SleepHarmonizer-0.1.5/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_Export.py
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_LoadData.py
+-rwxrwxrwx   0 root         (0) root         (0)     1016 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_Setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_SignalPreprocessing.py
```

### Comparing `SleepHarmonizer-0.1.4/LICENSE` & `SleepHarmonizer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/PKG-INFO` & `SleepHarmonizer-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SleepHarmonizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Plugin and stand alone tool to harmonize sleep related data
 Home-page: https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SleepHarmonizer-0.1.4/README.md` & `SleepHarmonizer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/EDFWriter.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/EDFWriter.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/PSGEventManager.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/PSGEventManager.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/Plugin.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/Plugin.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/SignalPreprocessing.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/config.yaml` & `SleepHarmonizer-0.1.5/SleepHarmonizer/config.yaml`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/phases/Export.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/phases/Export.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/phases/LoadData.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/phases/LoadData.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,16 @@
         recordLoader = RecordLoader.get()
 
         if dataName == "metadata":
             allRecordIds = recordLoader.getRecordList()
             if len(allRecordIds) == 0:
                 raise Exception("No records found. Check your recordLoader config and your dataversion config.")
             metadata = self.getMetadata(allRecordIds)
+            if not self.getConfig("dataIsFinal", False):
+                self.logWarning("metadata is not final (flag dataIsFinal not set), so the metadata is not saved")
             self.project.registerData("metadata", metadata, save=self.getConfig("dataIsFinal", False))
         elif dataName == "allDBRecordIds":
             datasetConfig = self.getConfig("dataversion")
 
             if datasetConfig["recordIds"] is not None:
                 recordIds = {r: [r] for r in datasetConfig["recordIds"]}
             else:
```

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/AliceRMLLoader.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/AliceRMLLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/AliceTextReportLoader.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/AliceTextReportLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/DominoErgLoader.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoErgLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/RecordLoaderAlice.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderAlice.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/RecordLoaderDomino.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderDomino.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer/recordloaders/RecordLoaderTest.py` & `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderTest.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer.egg-info/PKG-INFO` & `SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SleepHarmonizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Plugin and stand alone tool to harmonize sleep related data
 Home-page: https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SleepHarmonizer-0.1.4/SleepHarmonizer.egg-info/SOURCES.txt` & `SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/setup.py` & `SleepHarmonizer-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SleepHarmonizer",
-    version="v0.1.4"[1:],
+    version="v0.1.5"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Plugin and stand alone tool to harmonize sleep related data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer",
     packages=setuptools.find_packages(),
```

### Comparing `SleepHarmonizer-0.1.4/tests/unit/test_Export.py` & `SleepHarmonizer-0.1.5/tests/unit/test_Export.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/tests/unit/test_LoadData.py` & `SleepHarmonizer-0.1.5/tests/unit/test_LoadData.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/tests/unit/test_Plugin.py` & `SleepHarmonizer-0.1.5/tests/unit/test_Plugin.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.4/tests/unit/test_SignalPreprocessing.py` & `SleepHarmonizer-0.1.5/tests/unit/test_SignalPreprocessing.py`

 * *Files identical despite different names*

