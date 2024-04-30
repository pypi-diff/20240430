# Comparing `tmp/brainsight-0.1.0.tar.gz` & `tmp/brainsight-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainsight-0.1.0.tar", max compression
+gzip compressed data, was "brainsight-0.2.0.tar", max compression
```

## Comparing `brainsight-0.1.0.tar` & `brainsight-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,16 @@
--rw-r--r--   0        0        0      129 2024-04-18 12:41:09.120946 brainsight-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-18 12:46:46.330548 brainsight-0.1.0/brainsight/__ini__.py
--rw-r--r--   0        0        0      415 2024-04-18 12:46:44.458928 brainsight-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 brainsight-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      129 2024-04-18 12:41:09.120946 brainsight-0.2.0/README.md
+-rw-r--r--   0        0        0       45 2024-04-30 10:14:15.902680 brainsight-0.2.0/brainsight/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 10:14:15.903321 brainsight-0.2.0/brainsight/modules/__init__.py
+-rw-r--r--   0        0        0     5358 2024-04-30 10:14:15.915624 brainsight-0.2.0/brainsight/modules/base_module.py
+-rw-r--r--   0        0        0      152 2024-04-30 10:14:15.923627 brainsight-0.2.0/brainsight/modules/defaults.py
+-rw-r--r--   0        0        0    10161 2024-04-30 10:14:15.930088 brainsight-0.2.0/brainsight/modules/lfp.py
+-rw-r--r--   0        0        0    10933 2024-04-30 10:14:15.932340 brainsight-0.2.0/brainsight/modules/periodogram.py
+-rw-r--r--   0        0        0    10110 2024-04-30 10:14:15.935576 brainsight-0.2.0/brainsight/modules/spectrogram.py
+-rw-r--r--   0        0        0     2384 2024-04-30 10:14:48.059214 brainsight-0.2.0/brainsight/modules/utils.py
+-rw-r--r--   0        0        0       88 2024-04-30 10:14:15.941331 brainsight-0.2.0/brainsight/types/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-30 10:14:15.944821 brainsight-0.2.0/brainsight/types/dataset.py
+-rw-r--r--   0        0        0     4438 2024-04-30 10:14:15.947662 brainsight-0.2.0/brainsight/types/signal.py
+-rw-r--r--   0        0        0      355 2024-04-30 10:14:15.950683 brainsight-0.2.0/brainsight/types/utils.py
+-rw-r--r--   0        0        0      499 2024-04-30 10:14:15.953952 brainsight-0.2.0/brainsight/utils/mappings.py
+-rw-r--r--   0        0        0      430 2024-04-30 10:15:22.785875 brainsight-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 brainsight-0.2.0/PKG-INFO
```

### Comparing `brainsight-0.1.0/PKG-INFO` & `brainsight-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: brainsight
-Version: 0.1.0
+Version: 0.2.0
 Summary: Analysis toolkit for brain activity data.
 Author: MMT Analytics
 Author-email: analytics@machinemedicine.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<6.1)
 Requires-Dist: colorcet (>=3.1.0,<3.2.0)
 Requires-Dist: matplotlib (>=3.8.3,<3.9.0)
+Requires-Dist: mne (>=1.7.0,<1.8.0)
 Requires-Dist: numpy (>=1.26.1,<1.27.0)
 Requires-Dist: scipy (>=1.11.3,<1.12.0)
 Description-Content-Type: text/markdown
 
 # BrainSight #
 
 Analysis toolkit for brain activity data.
```

