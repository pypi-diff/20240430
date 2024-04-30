# Comparing `tmp/DevOpsAPI-0.2.0a7.tar.gz` & `tmp/devopsapi-0.2.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DevOpsAPI-0.2.0a7.tar", last modified: Wed Nov 22 17:04:10 2023, max compression
+gzip compressed data, was "devopsapi-0.2.0a8.tar", last modified: Tue Apr 30 14:51:52 2024, max compression
```

## Comparing `DevOpsAPI-0.2.0a7.tar` & `devopsapi-0.2.0a8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:04:10.644317 DevOpsAPI-0.2.0a7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:04:10.640318 DevOpsAPI-0.2.0a7/DevOpsAPI/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/DevOpsAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/DevOpsAPI/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/DevOpsAPI/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/DevOpsAPI/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/DevOpsAPI/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/DevOpsAPI/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/DevOpsAPI/wi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:04:10.644317 DevOpsAPI-0.2.0a7/DevOpsAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-11-22 17:04:10.000000 DevOpsAPI-0.2.0a7/DevOpsAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-11-22 17:04:10.000000 DevOpsAPI-0.2.0a7/DevOpsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 17:04:10.000000 DevOpsAPI-0.2.0a7/DevOpsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-22 17:04:10.000000 DevOpsAPI-0.2.0a7/DevOpsAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-22 17:04:10.000000 DevOpsAPI-0.2.0a7/DevOpsAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-11-22 17:04:10.644317 DevOpsAPI-0.2.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-22 17:04:10.644317 DevOpsAPI-0.2.0a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:04:10.644317 DevOpsAPI-0.2.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/tests/test_testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/tests/test_testrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-11-22 17:04:03.000000 DevOpsAPI-0.2.0a7/tests/test_workitems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:51:52.370890 devopsapi-0.2.0a8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:51:52.370890 devopsapi-0.2.0a8/DevOpsAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/DevOpsAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/DevOpsAPI/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/DevOpsAPI/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/DevOpsAPI/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/DevOpsAPI/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/DevOpsAPI/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/DevOpsAPI/wi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:51:52.370890 devopsapi-0.2.0a8/DevOpsAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 14:51:52.000000 devopsapi-0.2.0a8/DevOpsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 14:51:52.000000 devopsapi-0.2.0a8/DevOpsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:51:52.000000 devopsapi-0.2.0a8/DevOpsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 14:51:52.000000 devopsapi-0.2.0a8/DevOpsAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 14:51:52.000000 devopsapi-0.2.0a8/DevOpsAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 14:51:52.370890 devopsapi-0.2.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 14:51:52.370890 devopsapi-0.2.0a8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:51:52.370890 devopsapi-0.2.0a8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/tests/test_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/tests/test_testrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-30 14:51:46.000000 devopsapi-0.2.0a8/tests/test_workitems.py
```

### Comparing `DevOpsAPI-0.2.0a7/DevOpsAPI/api.py` & `devopsapi-0.2.0a8/DevOpsAPI/api.py`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/DevOpsAPI/base.py` & `devopsapi-0.2.0a8/DevOpsAPI/base.py`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/DevOpsAPI/connection.py` & `devopsapi-0.2.0a8/DevOpsAPI/connection.py`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/DevOpsAPI/projects.py` & `devopsapi-0.2.0a8/DevOpsAPI/projects.py`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/DevOpsAPI/testing.py` & `devopsapi-0.2.0a8/DevOpsAPI/testing.py`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/DevOpsAPI/wi.py` & `devopsapi-0.2.0a8/DevOpsAPI/wi.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,23 @@
 
     def as_xml(self):
         return Step._template.format(self.action, self.result)
 
     def __str__(self):
         return f"Step: action: {self.action}, result: {self.result}"
 
-    _template = """
-        <step id=\"2\" type=\"ValidateStep\">
-            <parameterizedString isformatted=\"true\">{}</parameterizedString>
-            <parameterizedString isformatted=\"true\">{}</parameterizedString><description/>
-        </step>"""
+    _template = re.sub(r"\n", "", """
+<step type=\"ActionStep\">
+<parameterizedString isformatted=\"true\">
+&lt;DIV&gt;&lt;P&gt;{}&lt;/P&gt;&lt;/DIV&gt;
+</parameterizedString>
+<parameterizedString isformatted=\"true\">
+&lt;DIV&gt;&lt;P&gt;{}&lt;/P&gt;&lt;/DIV&gt;
+</parameterizedString><description/>
+</step>""")
 
 
 class WorkItem:
     def __init__(self, connection, id=None, json=None):
         self._c = connection
 
         if id:
@@ -155,15 +159,15 @@
     @Steps.setter
     def Steps(self, steps):
         strsteps = [step.as_xml() for step in steps]
         stepxml = f'<steps>{"".join(strsteps)}</steps>'
 
         patches = Patches()
         patches.append(Patch(Ops.add, "Microsoft.VSTS.TCM.Steps", stepxml))
-        response = self._c.patch(f"wit/workitems/{self.id}", patches.json(), is_json=True)
+        response = self._c.patch(f"wit/workitems/{self.id}", json=patches.json(), is_json=True)
         response.raise_for_status()
         self.update()
 
     def delete(self):
         response = self._c.delete(f"test/testcases/{self.id}")
         response.raise_for_status()
 
@@ -200,15 +204,14 @@
     def __init__(self, operation, field, value):
         self.operation = operation
         self.field = field
         self.value = value
 
     def json(self):
         result = {
-            "from": None,
             "op": self.operation,
             "path": f"/fields/{self.field}",
             "value": self.value
         }
         return result
```

### Comparing `DevOpsAPI-0.2.0a7/DevOpsAPI.egg-info/PKG-INFO` & `devopsapi-0.2.0a8/DevOpsAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DevOpsAPI
-Version: 0.2.0a7
+Version: 0.2.0a8
 Summary: A simple object-oriented python interface to the DevOps REST API
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/acre-bdd/DevOpsAPI
 Project-URL: Bug Tracker, https://github.com/acre-bdd/DevOpsAPI/issues
 Project-URL: Documentation, https://acre-bdd.github.io/DevOpsAPI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DevOpsAPI-0.2.0a7/LICENSE` & `devopsapi-0.2.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/PKG-INFO` & `devopsapi-0.2.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DevOpsAPI
-Version: 0.2.0a7
+Version: 0.2.0a8
 Summary: A simple object-oriented python interface to the DevOps REST API
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/acre-bdd/DevOpsAPI
 Project-URL: Bug Tracker, https://github.com/acre-bdd/DevOpsAPI/issues
 Project-URL: Documentation, https://acre-bdd.github.io/DevOpsAPI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DevOpsAPI-0.2.0a7/README.md` & `devopsapi-0.2.0a8/README.md`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/pyproject.toml` & `devopsapi-0.2.0a8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "DevOpsAPI"
-version = "0.2.0a7"
+version = "0.2.0a8"
 description="A simple object-oriented python interface to the DevOps REST API"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `DevOpsAPI-0.2.0a7/tests/test_testcase.py` & `devopsapi-0.2.0a8/tests/test_testcase.py`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/tests/test_testrun.py` & `devopsapi-0.2.0a8/tests/test_testrun.py`

 * *Files identical despite different names*

### Comparing `DevOpsAPI-0.2.0a7/tests/test_workitems.py` & `devopsapi-0.2.0a8/tests/test_workitems.py`

 * *Files identical despite different names*

