# Comparing `tmp/roktools-6.1.1.tar.gz` & `tmp/roktools-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roktools-6.1.1.tar", max compression
+gzip compressed data, was "roktools-6.1.2.tar", max compression
```

## Comparing `roktools-6.1.1.tar` & `roktools-6.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-04-15 14:24:20.442323 roktools-6.1.1/LICENSE
--rw-r--r--   0        0        0     1665 2024-04-15 14:24:20.442323 roktools-6.1.1/README.md
--rw-r--r--   0        0        0     1162 2024-04-15 14:24:20.442323 roktools-6.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-15 14:24:20.442323 roktools-6.1.1/roktools/__init__.py
--rw-r--r--   0        0        0     4509 2024-04-15 14:24:20.442323 roktools-6.1.1/roktools/cl.py
--rw-r--r--   0        0        0      133 2024-04-15 14:24:20.442323 roktools-6.1.1/roktools/constants.py
--rw-r--r--   0        0        0      491 2024-04-15 14:24:20.442323 roktools-6.1.1/roktools/decorator.py
--rw-r--r--   0        0        0      933 2024-04-15 14:24:20.442323 roktools-6.1.1/roktools/file.py
--rw-r--r--   0        0        0    33628 2024-04-15 14:24:20.442323 roktools-6.1.1/roktools/geodetic.py
--rw-r--r--   0        0        0        0 2024-04-15 14:24:20.490322 roktools-6.1.1/roktools/gnss/__init__.py
--rw-r--r--   0        0        0     1884 2024-04-15 14:24:20.442323 roktools-6.1.1/roktools/gnss/edit.py
--rw-r--r--   0        0        0     1644 2024-04-15 14:24:20.442323 roktools-6.1.1/roktools/gnss/observables.py
--rw-r--r--   0        0        0     1244 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/gnss/residuals.py
--rw-r--r--   0        0        0     9505 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/gnss/types.py
--rw-r--r--   0        0        0     1479 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/logger.py
--rw-r--r--   0        0        0        0 2024-04-15 14:24:20.490322 roktools-6.1.1/roktools/orbit/__init__.py
--rw-r--r--   0        0        0     1745 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/orbit/kepler.py
--rw-r--r--   0        0        0     5905 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/orbit/tle.py
--rw-r--r--   0        0        0        0 2024-04-15 14:24:20.490322 roktools-6.1.1/roktools/parsers/rtklib/__init__,py
--rw-r--r--   0        0        0     5459 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/parsers/rtklib/stats.py
--rw-r--r--   0        0        0    31188 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/rinex.py
--rwxr-xr-x   0        0        0     1084 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/stats.py
--rwxr-xr-x   0        0        0     1598 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/tensorial.py
--rw-r--r--   0        0        0    11178 2024-04-15 14:24:20.446323 roktools-6.1.1/roktools/time.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-30 07:25:56.872515 roktools-6.1.2/LICENSE
+-rw-r--r--   0        0        0     1665 2024-04-30 07:25:56.872515 roktools-6.1.2/README.md
+-rw-r--r--   0        0        0     1162 2024-04-30 07:25:56.872515 roktools-6.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/__init__.py
+-rw-r--r--   0        0        0     4509 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/cl.py
+-rw-r--r--   0        0        0      133 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/constants.py
+-rw-r--r--   0        0        0      491 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/decorator.py
+-rw-r--r--   0        0        0      933 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/file.py
+-rw-r--r--   0        0        0    33628 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/geodetic.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:25:56.924515 roktools-6.1.2/roktools/gnss/__init__.py
+-rw-r--r--   0        0        0     1884 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/gnss/edit.py
+-rw-r--r--   0        0        0     1644 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/gnss/observables.py
+-rw-r--r--   0        0        0     1244 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/gnss/residuals.py
+-rw-r--r--   0        0        0     9505 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/gnss/types.py
+-rw-r--r--   0        0        0     1479 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/logger.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:25:56.924515 roktools-6.1.2/roktools/orbit/__init__.py
+-rw-r--r--   0        0        0     1745 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/orbit/kepler.py
+-rw-r--r--   0        0        0     5905 2024-04-30 07:25:56.872515 roktools-6.1.2/roktools/orbit/tle.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:25:56.924515 roktools-6.1.2/roktools/parsers/rtklib/__init__,py
+-rw-r--r--   0        0        0     5459 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/parsers/rtklib/stats.py
+-rw-r--r--   0        0        0    31199 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/rinex.py
+-rwxr-xr-x   0        0        0     1084 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/stats.py
+-rwxr-xr-x   0        0        0     1598 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/tensorial.py
+-rw-r--r--   0        0        0    11178 2024-04-30 07:25:56.876515 roktools-6.1.2/roktools/time.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.1.2/PKG-INFO
```

### Comparing `roktools-6.1.1/LICENSE` & `roktools-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/README.md` & `roktools-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/pyproject.toml` & `roktools-6.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roktools"
-version = "6.1.1"
+version = "6.1.2"
 description = "Package with utilities and tools for GNSS data processing"
 authors = ["Rokubun <info@rokubun.cat>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `roktools-6.1.1/roktools/cl.py` & `roktools-6.1.2/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/file.py` & `roktools-6.1.2/roktools/file.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/geodetic.py` & `roktools-6.1.2/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/gnss/edit.py` & `roktools-6.1.2/roktools/gnss/edit.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/gnss/observables.py` & `roktools-6.1.2/roktools/gnss/observables.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/gnss/residuals.py` & `roktools-6.1.2/roktools/gnss/residuals.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/gnss/types.py` & `roktools-6.1.2/roktools/gnss/types.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/logger.py` & `roktools-6.1.2/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/orbit/kepler.py` & `roktools-6.1.2/roktools/orbit/kepler.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/orbit/tle.py` & `roktools-6.1.2/roktools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/parsers/rtklib/stats.py` & `roktools-6.1.2/roktools/parsers/rtklib/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/rinex.py` & `roktools-6.1.2/roktools/rinex.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
         if observable_value.lli != 0:
             self.slip = 1
             self.flags = '00000100'
 
     def aslist(self) -> list:
 
-        return [self.epoch, self.sat.constellation, self.sat, str(self.channel),
+        return [self.epoch, self.sat.constellation.value, str(self.sat), str(self.channel),
                 f'{self.sat}{self.channel}', self.range, self.phase, self.doppler, self.snr, self.flags, self.slip]
 
     @staticmethod
     def get_list_fieldnames() -> List[str]:
         return ["epoch", "constellation", "sat", "channel", "signal", "range", "phase", "doppler", "snr", "flag", "slip"]
```

### Comparing `roktools-6.1.1/roktools/stats.py` & `roktools-6.1.2/roktools/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/tensorial.py` & `roktools-6.1.2/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/roktools/time.py` & `roktools-6.1.2/roktools/time.py`

 * *Files identical despite different names*

### Comparing `roktools-6.1.1/PKG-INFO` & `roktools-6.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 6.1.1
+Version: 6.1.2
 Summary: Package with utilities and tools for GNSS data processing
 Author: Rokubun
 Author-email: info@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

