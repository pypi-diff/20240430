# Comparing `tmp/kframe-0.2.3.dev8901407152.tar.gz` & `tmp/kframe-0.2.3rc1.tar.gz`

## Comparing `kframe-0.2.3.dev8901407152.tar` & `kframe-0.2.3rc1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.coverage
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.tool-versions
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/CHANGELOG.md
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.github/workflows/dev_ci.yml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.github/workflows/main_release.yml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.github/workflows/qa_cd.yml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.github/workflows/qa_ci.yml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/src/kframe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/src/kframe/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/src/kframe/config/configattr.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/tests/test_secretattr.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/.gitignore
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/LICENSE.txt
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/README.md
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/pyproject.toml
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 kframe-0.2.3.dev8901407152/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.tool-versions
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/dev_ci.yml
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/qa_cd.yml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.github/workflows/qa_ci.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/tests/test_secretattr.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/.gitignore
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/LICENSE.txt
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/README.md
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 kframe-0.2.3rc1/PKG-INFO
```

### Comparing `kframe-0.2.3.dev8901407152/CHANGELOG.md` & `kframe-0.2.3rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/.github/workflows/dev_ci.yml` & `kframe-0.2.3rc1/.github/workflows/dev_ci.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/.github/workflows/main_ci.yml` & `kframe-0.2.3rc1/.github/workflows/main_ci.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/.github/workflows/main_pre_release.yml` & `kframe-0.2.3rc1/.github/workflows/main_pre_release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -56,16 +56,14 @@
     - name: Run tests
       run: hatch run cov
 
     - name: Build
       run: hatch build
 
     - name: Publish
-      run: hatch publish --user __token__ --yes
-      env:
-        HATCH_INDEX_AUTH: ${{ secrets.PYPI_TOKEN }}
+      run: hatch publish --user __token__
```

### Comparing `kframe-0.2.3.dev8901407152/.github/workflows/main_release.yml` & `kframe-0.2.3rc1/.github/workflows/main_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/.github/workflows/qa_cd.yml` & `kframe-0.2.3rc1/.github/workflows/qa_cd.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/.github/workflows/qa_ci.yml` & `kframe-0.2.3rc1/.github/workflows/qa_ci.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/src/kframe/config/configattr.py` & `kframe-0.2.3rc1/src/kframe/config/configattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/src/kframe/config/configentity.py` & `kframe-0.2.3rc1/src/kframe/config/configentity.py`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/tests/test_secretattr.py` & `kframe-0.2.3rc1/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/LICENSE.txt` & `kframe-0.2.3rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/README.md` & `kframe-0.2.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `kframe-0.2.3.dev8901407152/pyproject.toml` & `kframe-0.2.3rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.2.3.dev8901407152"
+version = "0.2.3rc1"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
@@ -24,17 +24,17 @@
   "Operating System :: MacOS",
 ]
 dependencies = [
 ]
 
 [project.urls]
 # TODO: Update these URLs
-Documentation = "https://github.com/kaeus-sgarcia/kframe#readme"
-Issues = "https://github.com/kaeus-sgarcia/kframe/issues"
-Source = "https://github.com/kaeus-sgarcia/kframe"
+Documentation = "https://github.com/unknown/kframe#readme"
+Issues = "https://github.com/unknown/kframe/issues"
+Source = "https://github.com/unknown/kframe"
 
 # Development environment
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "ruff",
```

### Comparing `kframe-0.2.3.dev8901407152/PKG-INFO` & `kframe-0.2.3rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.2.3.dev8901407152
+Version: 0.2.3rc1
 Summary: Kaeus development framework
-Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
-Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
-Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
+Project-URL: Documentation, https://github.com/unknown/kframe#readme
+Project-URL: Issues, https://github.com/unknown/kframe/issues
+Project-URL: Source, https://github.com/unknown/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
```

