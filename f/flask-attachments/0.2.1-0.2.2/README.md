# Comparing `tmp/flask_attachments-0.2.1.tar.gz` & `tmp/flask_attachments-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr  9 22:33:47 2024, max compression
+gzip compressed data, last modified: Mon Apr 29 22:23:32 2024, max compression
```

## Comparing `flask_attachments-0.2.1.tar` & `flask_attachments-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      247 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/__about__.py
--rw-r--r--   0        0        0      372 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/__init__.py
--rw-r--r--   0        0        0      411 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/_version.py
--rw-r--r--   0        0        0     6566 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/cli.py
--rw-r--r--   0        0        0     3850 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/compression.py
--rw-r--r--   0        0        0     7419 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/extension.py
--rw-r--r--   0        0        0    12035 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/models.py
--rw-r--r--   0        0        0        0 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/py.typed
--rw-r--r--   0        0        0     2989 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/services.py
--rw-r--r--   0        0        0     1153 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/views.py
--rw-r--r--   0        0        0     1223 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/.gitignore
--rw-r--r--   0        0        0       98 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/AUTHORS.rst
--rw-r--r--   0        0        0     1502 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/LICENSE
--rw-r--r--   0        0        0      814 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/README.md
--rw-r--r--   0        0        0     2384 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1791 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      247 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/__about__.py
+-rw-r--r--   0        0        0      372 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/_version.py
+-rw-r--r--   0        0        0     6566 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/cli.py
+-rw-r--r--   0        0        0     3850 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/compression.py
+-rw-r--r--   0        0        0     7419 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/extension.py
+-rw-r--r--   0        0        0    12041 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/models.py
+-rw-r--r--   0        0        0        0 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/py.typed
+-rw-r--r--   0        0        0     2989 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/services.py
+-rw-r--r--   0        0        0     1153 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/src/flask_attachments/views.py
+-rw-r--r--   0        0        0     1223 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/.gitignore
+-rw-r--r--   0        0        0       98 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1502 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/LICENSE
+-rw-r--r--   0        0        0      814 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/README.md
+-rw-r--r--   0        0        0     2399 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1791 2024-04-29 22:23:32.000000 flask_attachments-0.2.2/PKG-INFO
```

### Comparing `flask_attachments-0.2.1/src/flask_attachments/cli.py` & `flask_attachments-0.2.2/src/flask_attachments/cli.py`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.1/src/flask_attachments/compression.py` & `flask_attachments-0.2.2/src/flask_attachments/compression.py`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.1/src/flask_attachments/extension.py` & `flask_attachments-0.2.2/src/flask_attachments/extension.py`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.1/src/flask_attachments/models.py` & `flask_attachments-0.2.2/src/flask_attachments/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     def download_link(self) -> str:
         """Url for downloading the file"""
         return url_for("attachments.download", id=self.id)
 
     @classmethod
     def from_file(
         cls,
-        file: os.PathLike[str],
+        file: str | os.PathLike[str],
         content_type: str | None = None,
         compression: CompressionAlgorithm | str | None = None,
         digest_algorithm: str | None = None,
     ) -> "Attachment":
         """Create a new attachment by reading a file from disk"""
 
         if content_type is None:
```

### Comparing `flask_attachments-0.2.1/src/flask_attachments/services.py` & `flask_attachments-0.2.2/src/flask_attachments/services.py`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.1/src/flask_attachments/views.py` & `flask_attachments-0.2.2/src/flask_attachments/views.py`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.1/.gitignore` & `flask_attachments-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.1/LICENSE` & `flask_attachments-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.1/README.md` & `flask_attachments-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.1/pyproject.toml` & `flask_attachments-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 Homepage = "https://github.com/alexrudy/flask_attachments"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements/base.in"]
 
 [tool.hatch.version]
 source = "vcs"
-raw-options = { local_scheme = "no-local-version" }
+
+[tool.hatch.version.raw-options]
+local_scheme = "no-local-version"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/flask_attachments/_version.py"
 
-
 [tool.hatch.build.targets.sdist]
 include = ["src/flask_attachments"]
 exclude = [
     "tests/*",
     "docs/*",
     ".*",
     "build/*",
```

### Comparing `flask_attachments-0.2.1/PKG-INFO` & `flask_attachments-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flask-attachments
-Version: 0.2.1
+Version: 0.2.2
 Summary: Flask Attachments provides a way to integrate arbitrary media with SQLAlchemy in a Flask website.
 Project-URL: Homepage, https://github.com/alexrudy/flask_attachments
 Author-email: Alex Rudy <opensource@alexrudy.net>
 License-Expression: BSD-3-Clause
 License-File: AUTHORS.rst
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
```

