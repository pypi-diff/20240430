# Comparing `tmp/hypercoast-0.1.2.tar.gz` & `tmp/hypercoast-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercoast-0.1.2.tar", last modified: Thu Apr 25 17:52:46 2024, max compression
+gzip compressed data, was "hypercoast-0.1.3.tar", last modified: Tue Apr 30 15:26:03 2024, max compression
```

## Comparing `hypercoast-0.1.2.tar` & `hypercoast-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.047348 hypercoast-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.051348 hypercoast-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.051348 hypercoast-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 17:52:31.000000 hypercoast-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-25 17:52:31.000000 hypercoast-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 17:52:46.055348 hypercoast-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 17:52:31.000000 hypercoast-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/emit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/examples/emit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/ui.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    37734 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/emit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-25 17:52:31.000000 hypercoast-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 17:52:31.000000 hypercoast-0.1.2/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-25 17:52:31.000000 hypercoast-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 17:52:31.000000 hypercoast-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 17:52:31.000000 hypercoast-0.1.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:52:46.055348 hypercoast-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 17:52:31.000000 hypercoast-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-25 17:52:31.000000 hypercoast-0.1.2/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.636089 hypercoast-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.624090 hypercoast-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.628090 hypercoast-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.628090 hypercoast-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.636089 hypercoast-0.1.3/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 15:25:53.000000 hypercoast-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-30 15:25:53.000000 hypercoast-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-30 15:26:03.636089 hypercoast-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-30 15:25:53.000000 hypercoast-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.632089 hypercoast-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/emit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.632089 hypercoast-0.1.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/examples/emit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.632089 hypercoast-0.1.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/pace.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/ui.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.632089 hypercoast-0.1.3/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/emit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/pace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-30 15:25:53.000000 hypercoast-0.1.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 15:25:53.000000 hypercoast-0.1.3/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-30 15:25:53.000000 hypercoast-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 15:25:53.000000 hypercoast-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 15:25:53.000000 hypercoast-0.1.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:26:03.636089 hypercoast-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.636089 hypercoast-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 15:25:53.000000 hypercoast-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 15:25:53.000000 hypercoast-0.1.3/tests/test_hypercoast.py
```

### Comparing `hypercoast-0.1.2/.github/workflows/docs-build.yml` & `hypercoast-0.1.3/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/.github/workflows/docs.yml` & `hypercoast-0.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/.github/workflows/installation.yml` & `hypercoast-0.1.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/.github/workflows/macos.yml` & `hypercoast-0.1.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/.github/workflows/pypi.yml` & `hypercoast-0.1.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/.github/workflows/ubuntu.yml` & `hypercoast-0.1.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/.github/workflows/windows.yml` & `hypercoast-0.1.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/.gitignore` & `hypercoast-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/.pre-commit-config.yaml` & `hypercoast-0.1.3/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             types: [python]
           - id: trailing-whitespace
           - id: requirements-txt-fixer
           - id: check-added-large-files
             args: ["--maxkb=500"]
 
     - repo: https://github.com/psf/black
-      rev: 24.4.0
+      rev: 24.4.2
       hooks:
           - id: black-jupyter
             language_version: python3.11
 
     # - repo: https://github.com/codespell-project/codespell
     #   rev: v2.2.6
     #   hooks:
```

### Comparing `hypercoast-0.1.2/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.1.3/HyperCoast.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -44,15 +44,20 @@
 **A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
--   Visualize hyperspectral data
--   Analyze hyperspectral data
--
+-   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit/), [PACE](https://pace.gsfc.nasa.gov/))
+-   Interactive extraction and visualization of spectral signatures
+-   Saving spectral signatures as CSV files
+
 ## Demo
 
 -   Visualizing spectral signature interactively
 
 ![](https://i.imgur.com/zeyABMq.gif)
+
+## Acknowledgement
+
+This projects draws inspiration and adapts source code from the [nasa/EMIT-Data-Resources](https://github.com/nasa/EMIT-Data-Resources) repository. Credit goes to the original authors.
```

### Comparing `hypercoast-0.1.2/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.1.3/HyperCoast.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,18 +30,20 @@
 docs/common.md
 docs/contributing.md
 docs/emit.md
 docs/faq.md
 docs/hypercoast.md
 docs/index.md
 docs/installation.md
+docs/pace.md
 docs/ui.md
 docs/usage.md
 docs/examples/emit.ipynb
 docs/overrides/main.html
 hypercoast/__init__.py
 hypercoast/common.py
 hypercoast/emit.py
 hypercoast/hypercoast.py
+hypercoast/pace.py
 hypercoast/ui.py
 tests/__init__.py
 tests/test_hypercoast.py
```

### Comparing `hypercoast-0.1.2/LICENSE` & `hypercoast-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/PKG-INFO` & `hypercoast-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -44,15 +44,20 @@
 **A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
--   Visualize hyperspectral data
--   Analyze hyperspectral data
--
+-   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit/), [PACE](https://pace.gsfc.nasa.gov/))
+-   Interactive extraction and visualization of spectral signatures
+-   Saving spectral signatures as CSV files
+
 ## Demo
 
 -   Visualizing spectral signature interactively
 
 ![](https://i.imgur.com/zeyABMq.gif)
+
+## Acknowledgement
+
+This projects draws inspiration and adapts source code from the [nasa/EMIT-Data-Resources](https://github.com/nasa/EMIT-Data-Resources) repository. Credit goes to the original authors.
```

### Comparing `hypercoast-0.1.2/README.md` & `hypercoast-0.1.3/docs/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-# HyperCoast
+# Welcome to hypercoast
 
-[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/HyperCoast/blob/main)
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
 [![image](https://static.pepy.tech/badge/hypercoast)](https://pepy.tech/project/hypercoast)
 [![image](https://img.shields.io/conda/vn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
 [![Conda Recipe](https://img.shields.io/badge/recipe-hypercoast-green.svg)](https://github.com/conda-forge/hypercoast-feedstock)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
 
 **A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
--   Visualize hyperspectral data
--   Analyze hyperspectral data
--
+-   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit/), [PACE](https://pace.gsfc.nasa.gov/))
+-   Interactive extraction and visualization of spectral signatures
+-   Saving spectral signatures as CSV files
+
 ## Demo
 
 -   Visualizing spectral signature interactively
 
 ![](https://i.imgur.com/zeyABMq.gif)
+
+## Acknowledgement
+
+This projects draws inspiration and adapts source code from the [nasa/EMIT-Data-Resources](https://github.com/nasa/EMIT-Data-Resources) repository. Credit goes to the original authors.
```

### Comparing `hypercoast-0.1.2/docs/contributing.md` & `hypercoast-0.1.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/docs/examples/emit.ipynb` & `hypercoast-0.1.3/docs/examples/emit.ipynb`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/docs/installation.md` & `hypercoast-0.1.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/hypercoast/common.py` & `hypercoast-0.1.3/hypercoast/common.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/hypercoast/emit.py` & `hypercoast-0.1.3/hypercoast/emit.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 Some source code is adapted from https://github.com/nasa/EMIT-Data-Resources.
 Credits to the original authors, including Erik Bolch, Alex Leigh, and others.
 
 """
 
 import os
 import xarray as xr
-import hvplot.xarray
 import numpy as np
 import geopandas as gpd
 
 
 def read_emit(filepath, ortho=True, wavelengths=None, method="nearest", **kwargs):
     """
     Opens an EMIT dataset from a file path and assigns new coordinates to it.
@@ -96,14 +95,16 @@
         options (dict, optional): Additional options to be passed to `hvplot.line`. Defaults to {}.
         **kwargs: Additional keyword arguments to be passed to `hvplot.line`.
 
     Returns:
         hvplot.Plot: The line plot of the reflectance data.
     """
 
+    import hvplot.xarray
+
     if ortho == True:
         if longitude is None or latitude is None:
             raise ValueError(
                 "Longitude and Latitude must be provided for orthorectified data."
             )
     else:
         if downtrack is None or crosstrack is None:
@@ -178,14 +179,16 @@
         title (str, optional): The title of the plot. If None, a default title will be generated. Defaults to None.
         options (dict, optional): Additional options to be passed to `hvplot.image`. Defaults to {}.
         **kwargs: Additional keyword arguments to be passed to `hvplot.image`.
 
     Returns:
         hvplot.Plot: The image plot of the reflectance data at the specified wavelengths.
     """
+    import hvplot.xarray
+
     if isinstance(ds, str):
         ds = read_emit(ds, ortho=ortho)
     example = ds.sel(wavelengths=wavelengths, method=method)
 
     if title is None:
         title = f"Reflectance at {example.wavelengths.values:.3f} {example.wavelengths.units}"
```

### Comparing `hypercoast-0.1.2/hypercoast/hypercoast.py` & `hypercoast-0.1.3/hypercoast/hypercoast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Main module."""
 
 import ipyleaflet
 import leafmap
 import xarray as xr
 from .common import download_file
 from .emit import read_emit, plot_emit, viz_emit, emit_to_netcdf, emit_to_image
+from .pace import *
 
 
 class Map(leafmap.Map):
     """
     A class that extends leafmap.Map to provide additional functionality for hypercoast.
 
     Attributes:
```

### Comparing `hypercoast-0.1.2/hypercoast/ui.py` & `hypercoast-0.1.3/hypercoast/ui.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.2/mkdocs.yml` & `hypercoast-0.1.3/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -81,8 +81,9 @@
     - Report Issues: https://github.com/opengeos/HyperCoast/issues
     - Examples:
           - examples/emit.ipynb
     - API Reference:
           - common module: common.md
           - emit module: emit.md
           - hypercoast module: hypercoast.md
+          - pace module: pace.md
           - ui module: ui.md
```

### Comparing `hypercoast-0.1.2/pyproject.toml` & `hypercoast-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HyperCoast"
-version = "0.1.2"
+version = "0.1.3"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package for processing hyperspectral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.1.2"
+current_version = "0.1.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

