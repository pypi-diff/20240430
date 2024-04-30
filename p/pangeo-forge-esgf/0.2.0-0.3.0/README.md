# Comparing `tmp/pangeo-forge-esgf-0.2.0.tar.gz` & `tmp/pangeo_forge_esgf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-esgf-0.2.0.tar", last modified: Tue Apr  2 19:14:55 2024, max compression
+gzip compressed data, was "pangeo_forge_esgf-0.3.0.tar", last modified: Tue Apr 30 15:33:24 2024, max compression
```

## Comparing `pangeo-forge-esgf-0.2.0.tar` & `pangeo_forge_esgf-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.311452 pangeo-forge-esgf-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.311452 pangeo-forge-esgf-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.github/workflows/pythonpublish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.311452 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17813 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/recipe_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_recipe_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 19:14:55.000000 pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:14:55.315451 pangeo-forge-esgf-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-02 19:14:44.000000 pangeo-forge-esgf-0.2.0/test_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:33:24.855017 pangeo_forge_esgf-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:33:24.851017 pangeo_forge_esgf-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:33:24.851017 pangeo_forge_esgf-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/.github/workflows/pythonpublish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-30 15:33:24.855017 pangeo_forge_esgf-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:33:24.855017 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 15:33:24.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17813 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/recipe_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:33:24.855017 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/tests/test_recipe_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:33:24.855017 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-30 15:33:24.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 15:33:24.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:33:24.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 15:33:24.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 15:33:24.000000 pangeo_forge_esgf-0.3.0/pangeo_forge_esgf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:33:24.855017 pangeo_forge_esgf-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-30 15:33:11.000000 pangeo_forge_esgf-0.3.0/test_script.py
```

### Comparing `pangeo-forge-esgf-0.2.0/.github/dependabot.yml` & `pangeo_forge_esgf-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/.github/workflows/ci.yaml` & `pangeo_forge_esgf-0.3.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/.github/workflows/pythonpublish.yaml` & `pangeo_forge_esgf-0.3.0/.github/workflows/pythonpublish.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/.gitignore` & `pangeo_forge_esgf-0.3.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -131,7 +131,8 @@
 test_beam.ipynb
 test_DAMIP_feedstock_with_beam_refactor.ipynb
 test_esgf-pyclient.ipynb
 test_refactor.ipynb
 test_refactor.py
 test_script copy.py
 pangeo_forge_esgf/recipe_inputs_old.py
+.vscode/settings.json
```

### Comparing `pangeo-forge-esgf-0.2.0/.pre-commit-config.yaml` & `pangeo_forge_esgf-0.3.0/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 autoupdate_schedule: quarterly
 default_language_version:
     python: python3.9
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.3.5
+    rev: v0.4.2
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v1.9.0'  # Use the sha / tag you want to point at
+    rev: 'v1.10.0'  # Use the sha / tag you want to point at
     hooks:
     -   id: mypy
         additional_dependencies: ["types-requests"]
         exclude: "test_script.py"
```

### Comparing `pangeo-forge-esgf-0.2.0/LICENSE` & `pangeo_forge_esgf-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/PKG-INFO` & `pangeo_forge_esgf-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-esgf
-Version: 0.2.0
+Version: 0.3.0
 Summary: Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge
 Author-email: Julius Busecke <julius@ldeo.columbia.edu>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/jbusecke/pangeo-forge-esgf
 Project-URL: Tracker, https://github.com/jbusecke/pangeo-forge-esgf/issues
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-esgf-0.2.0/README.md` & `pangeo_forge_esgf-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/__init__.py` & `pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/__init__.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/recipe_inputs.py` & `pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/recipe_inputs.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_parsing.py` & `pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/tests/test_parsing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 from pangeo_forge_esgf.parsing import parse_instance_ids
 import pytest
 
 
-def test_readme_example():
+def test_unparsable_iid():
+    parse_iids = [
+        "Some.random.*.*.crap.*.that.we.[cannot, will_not].parse",
+    ]
+    iids = []
+    for piid in parse_iids:
+        with pytest.warns(UserWarning):
+            iids.extend(parse_instance_ids(piid))
+    iids
+
+    assert len(iids) == 0
+
+
+@pytest.mark.parametrize(
+    "search_nodes", [None, ["https://esgf-node.llnl.gov/esg-search/search"]]
+)
+def test_readme_example(search_nodes):
     # This is possibly flaky (due to the dependence on the ESGF API)
     parse_iids = [
         "CMIP6.PMIP.*.*.lgm.*.*.[uo,vo].*.*",
     ]
     iids = []
     for piid in parse_iids:
-        iids.extend(parse_instance_ids(piid))
+        iids.extend(parse_instance_ids(piid, search_nodes))
     iids
 
     # I expect at least these iids to be parsed
     # (there might be new ones that are added at a later point)
     expected_iids = [
         "CMIP6.PMIP.MIROC.MIROC-ES2L.lgm.r1i1p1f2.Omon.uo.gn.v20191002",
         "CMIP6.PMIP.AWI.AWI-ESM-1-1-LR.lgm.r1i1p1f1.Odec.uo.gn.v20200212",
@@ -27,14 +43,22 @@
         "CMIP6.PMIP.MPI-M.MPI-ESM1-2-LR.lgm.r1i1p1f1.Omon.vo.gn.v20190710",
     ]
 
     for iid in expected_iids:
         assert iid in iids
 
 
+def test_deprecation_warning():
+    iid = ["CMIP6.PMIP.*.*.lgm.*.*.uo.*.*"]
+    with pytest.warns(DeprecationWarning):
+        parse_instance_ids(
+            iid[0], search_node="https://esgf-node.llnl.gov/esg-search/search"
+        )
+
+
 @pytest.mark.parametrize(
     "facet_iid, expected",
     [
         ("a.b.c.d", ["a.b.c.d"]),
         ("a.[b1, b2].c.[d1, d2]", ["a.b1.c.d1", "a.b1.c.d2", "a.b2.c.d1", "a.b2.c.d2"]),
         ("a.[b1, b2].c.d", ["a.b1.c.d", "a.b2.c.d"]),
         ("a.b.c.[d1, d2]", ["a.b.c.d1", "a.b.c.d2"]),
```

### Comparing `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf/tests/test_recipe_inputs.py` & `pangeo_forge_esgf-0.3.0/pangeo_forge_esgf/tests/test_recipe_inputs.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/PKG-INFO` & `pangeo_forge_esgf-0.3.0/pangeo_forge_esgf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-esgf
-Version: 0.2.0
+Version: 0.3.0
 Summary: Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge
 Author-email: Julius Busecke <julius@ldeo.columbia.edu>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/jbusecke/pangeo-forge-esgf
 Project-URL: Tracker, https://github.com/jbusecke/pangeo-forge-esgf/issues
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-esgf-0.2.0/pangeo_forge_esgf.egg-info/SOURCES.txt` & `pangeo_forge_esgf-0.3.0/pangeo_forge_esgf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/pyproject.toml` & `pangeo_forge_esgf-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-esgf-0.2.0/test_script.py` & `pangeo_forge_esgf-0.3.0/test_script.py`

 * *Files identical despite different names*

