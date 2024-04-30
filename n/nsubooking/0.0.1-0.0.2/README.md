# Comparing `tmp/nsubooking-0.0.1.tar.gz` & `tmp/nsubooking-0.0.2.tar.gz`

## Comparing `nsubooking-0.0.1.tar` & `nsubooking-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nsubooking-0.0.1/nsubooking/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 nsubooking-0.0.1/nsubooking/app.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 nsubooking-0.0.1/nsubooking/configure.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 nsubooking-0.0.1/nsubooking/driver.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 nsubooking-0.0.1/nsubooking/event.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 nsubooking-0.0.1/nsubooking/logger.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nsubooking-0.0.1/nsubooking/loop.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 nsubooking-0.0.1/nsubooking/settings.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 nsubooking-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nsubooking-0.0.1/LICENSE
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 nsubooking-0.0.1/README.md
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 nsubooking-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nsubooking-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nsubooking-0.0.2/nsubooking/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 nsubooking-0.0.2/nsubooking/app.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 nsubooking-0.0.2/nsubooking/configure.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 nsubooking-0.0.2/nsubooking/driver.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 nsubooking-0.0.2/nsubooking/event.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 nsubooking-0.0.2/nsubooking/logger.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nsubooking-0.0.2/nsubooking/loop.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 nsubooking-0.0.2/nsubooking/settings.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 nsubooking-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nsubooking-0.0.2/LICENSE
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nsubooking-0.0.2/README.md
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 nsubooking-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 nsubooking-0.0.2/PKG-INFO
```

### Comparing `nsubooking-0.0.1/nsubooking/event.py` & `nsubooking-0.0.2/nsubooking/event.py`

 * *Files identical despite different names*

### Comparing `nsubooking-0.0.1/nsubooking/logger.py` & `nsubooking-0.0.2/nsubooking/logger.py`

 * *Files identical despite different names*

### Comparing `nsubooking-0.0.1/nsubooking/loop.py` & `nsubooking-0.0.2/nsubooking/loop.py`

 * *Files identical despite different names*

### Comparing `nsubooking-0.0.1/nsubooking/settings.py` & `nsubooking-0.0.2/nsubooking/settings.py`

 * *Files identical despite different names*

### Comparing `nsubooking-0.0.1/.gitignore` & `nsubooking-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nsubooking-0.0.1/LICENSE` & `nsubooking-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nsubooking-0.0.1/README.md` & `nsubooking-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,45 @@
-**Automatic booking of washing machines at NSU.**
--------------------------------------------------
+# Automatic booking of washing machines at NSU.
 
 This package provides the opportunity for booking washing machine in NSU dormitories.
 
-For use this package you need tu setup your envirement variables first.
+## Installation
+
+`pip install nsubooking`
+
+## Setting env
+
+For use this package you need tu setup your envirement variables.
 
 You can do that with `.env` file in root directory or `export $var = data`.
 
 **You need folowing envirement variables:**
+
 - EMAIL (required) - email of your booking account.
 - PASSWORD (required) - password of your booking account.
 - PAGE_LIVE_TIME (nonrequired) - time between bookings.
 - BOOK_WAIT (nonrequired) - time between page reloads while waiting available machines.
 
-**You can use this package in two scenarios:**
-- Application mode:
-  1. Clone repo to your machine.
-  2. Install `requirements.txt` locate in  root directory.
-  3. Run `manage.py` file locate in  root directory.
-- Package mode:
-  Following...
+## Quickstart
+
+To quickstart try following code:
+
+```python
+from nsubooking import run
+
+
+if __name__ == 'main':
+  run()
+```
+
+To inject app to async loop you can also use:
+
+```python
+from nsubooking import run_loop
+import asyncio
+
+
+if __name__ == 'main':
+  asyncio.run(run_loop())
+```
+
+**But in this case logger will not configured.**
```

### Comparing `nsubooking-0.0.1/pyproject.toml` & `nsubooking-0.0.2/pyproject.toml`

 * *Files identical despite different names*

