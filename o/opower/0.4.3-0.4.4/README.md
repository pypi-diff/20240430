# Comparing `tmp/opower-0.4.3.tar.gz` & `tmp/opower-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opower-0.4.3.tar", last modified: Wed Apr  3 19:15:47 2024, max compression
+gzip compressed data, was "opower-0.4.4.tar", last modified: Tue Apr 30 04:46:19 2024, max compression
```

## Comparing `opower-0.4.3.tar` & `opower-0.4.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.551893 opower-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 19:15:42.000000 opower-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-03 19:15:47.551893 opower-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-03 19:15:42.000000 opower-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 19:15:42.000000 opower-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 19:15:47.551893 opower-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.547893 opower-0.4.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-03 19:15:42.000000 opower-0.4.3/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.547893 opower-0.4.3/src/opower/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21364 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/opower.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.551893 opower-0.4.3/src/opower/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/aepbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/aepohio.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/aeptexas.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/appalachianpower.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/atlanticcityelectric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/bge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/coautilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/comed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/coned.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/delmarva.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/duquesnelight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/enmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/evergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/exelon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/indianamichiganpower.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/kentuckypower.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/oru.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/peco.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/pepco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/pge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/portlandgeneral.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/pse.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/psoklahoma.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/scl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/smud.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/swepco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.551893 opower-0.4.3/src/opower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.551893 opower-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 19:15:42.000000 opower-0.4.3/tests/test_opower.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:19.378263 opower-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 04:46:14.000000 opower-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-30 04:46:19.378263 opower-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-30 04:46:14.000000 opower-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-30 04:46:14.000000 opower-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-30 04:46:19.378263 opower-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:19.370263 opower-0.4.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-30 04:46:14.000000 opower-0.4.4/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:19.370263 opower-0.4.4/src/opower/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21364 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/opower.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:19.378263 opower-0.4.4/src/opower/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/aepbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/aepohio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/aeptexas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/appalachianpower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/atlanticcityelectric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/bge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/coautilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/comed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/coned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/delmarva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/duquesnelight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/enmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/evergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/exelon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/indianamichiganpower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/kentuckypower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/oru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/peco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/pepco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/pge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/portlandgeneral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/psoklahoma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/scl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/smud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-30 04:46:14.000000 opower-0.4.4/src/opower/utilities/swepco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:19.378263 opower-0.4.4/src/opower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-30 04:46:19.000000 opower-0.4.4/src/opower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-30 04:46:19.000000 opower-0.4.4/src/opower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 04:46:19.000000 opower-0.4.4/src/opower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 04:46:19.000000 opower-0.4.4/src/opower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 04:46:19.000000 opower-0.4.4/src/opower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:19.378263 opower-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 04:46:14.000000 opower-0.4.4/tests/test_opower.py
```

### Comparing `opower-0.4.3/LICENSE` & `opower-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/PKG-INFO` & `opower-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opower-0.4.3/README.md` & `opower-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/pyproject.toml` & `opower-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opower"
-version = "0.4.3"
+version = "0.4.4"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `opower-0.4.3/src/demo.py` & `opower-0.4.4/src/demo.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/__init__.py` & `opower-0.4.4/src/opower/__init__.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/opower.py` & `opower-0.4.4/src/opower/opower.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/aepbase.py` & `opower-0.4.4/src/opower/utilities/aepbase.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/atlanticcityelectric.py` & `opower-0.4.4/src/opower/utilities/atlanticcityelectric.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/base.py` & `opower-0.4.4/src/opower/utilities/base.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/bge.py` & `opower-0.4.4/src/opower/utilities/bge.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/coautilities.py` & `opower-0.4.4/src/opower/utilities/coautilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,16 @@
             data=hidden_inputs,
             raise_for_status=True,
         ) as response:
             html = await response.text()
             action_url, hidden_inputs = get_form_action_url_and_hidden_inputs(html)
             assert set(hidden_inputs.keys()) == {"opentoken"}
 
+        session.cookie_jar.update_cookies({"dssPortalCW": "1"})
+
         # Getting success token
         async with session.post(
             action_url,
             headers={"User-Agent": USER_AGENT},
             data=hidden_inputs,
             allow_redirects=False,
             raise_for_status=True,
```

### Comparing `opower-0.4.3/src/opower/utilities/comed.py` & `opower-0.4.4/src/opower/utilities/comed.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/coned.py` & `opower-0.4.4/src/opower/utilities/coned.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/delmarva.py` & `opower-0.4.4/src/opower/utilities/delmarva.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/duquesnelight.py` & `opower-0.4.4/src/opower/utilities/duquesnelight.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/enmax.py` & `opower-0.4.4/src/opower/utilities/enmax.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/evergy.py` & `opower-0.4.4/src/opower/utilities/evergy.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/exelon.py` & `opower-0.4.4/src/opower/utilities/exelon.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/helpers.py` & `opower-0.4.4/src/opower/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/oru.py` & `opower-0.4.4/src/opower/utilities/oru.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/peco.py` & `opower-0.4.4/src/opower/utilities/peco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/pepco.py` & `opower-0.4.4/src/opower/utilities/pepco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/pge.py` & `opower-0.4.4/src/opower/utilities/pge.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/portlandgeneral.py` & `opower-0.4.4/src/opower/utilities/portlandgeneral.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/pse.py` & `opower-0.4.4/src/opower/utilities/pse.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/psoklahoma.py` & `opower-0.4.4/src/opower/utilities/psoklahoma.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/scl.py` & `opower-0.4.4/src/opower/utilities/scl.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/smud.py` & `opower-0.4.4/src/opower/utilities/smud.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower/utilities/swepco.py` & `opower-0.4.4/src/opower/utilities/swepco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.3/src/opower.egg-info/PKG-INFO` & `opower-0.4.4/src/opower.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opower-0.4.3/src/opower.egg-info/SOURCES.txt` & `opower-0.4.4/src/opower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

