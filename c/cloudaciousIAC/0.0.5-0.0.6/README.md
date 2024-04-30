# Comparing `tmp/cloudaciousiac-0.0.5.tar.gz` & `tmp/cloudaciousiac-0.0.6.tar.gz`

## Comparing `cloudaciousiac-0.0.5.tar` & `cloudaciousiac-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/.pypirc
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/config.cfg
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/setup.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/src/cloudaciousIAC/ContainerImages.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/src/cloudaciousIAC/Naming.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/src/cloudaciousIAC/README.md
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/src/cloudaciousIAC/StackInfo.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/.gitignore
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/.pypirc
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/config.cfg
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/setup.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/src/cloudaciousIAC/ContainerImages.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/src/cloudaciousIAC/Naming.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/src/cloudaciousIAC/README.md
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/src/cloudaciousIAC/StackInfo.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/.gitignore
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cloudaciousiac-0.0.6/PKG-INFO
```

### Comparing `cloudaciousiac-0.0.5/.gitlab-ci.yml` & `cloudaciousiac-0.0.6/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 pypi_prod:
   stage: deploy
   image: python:latest
   before_script:
     - echo $CI_COMMIT_TAG
     - cp .pypirc ~/
+    - cat ~/.pypirc
     - python -m pip install --upgrade build
     - python -m pip install --upgrade twine
   # environment:
   #   name: production
   #   url: https://prod.cloudacious.io
   rules:
     - if: $CI_COMMIT_TAG
```

### Comparing `cloudaciousiac-0.0.5/README.md` & `cloudaciousiac-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cloudaciousiac-0.0.5/setup.py` & `cloudaciousiac-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `cloudaciousiac-0.0.5/src/cloudaciousIAC/ContainerImages.py` & `cloudaciousiac-0.0.6/src/cloudaciousIAC/ContainerImages.py`

 * *Files identical despite different names*

### Comparing `cloudaciousiac-0.0.5/src/cloudaciousIAC/Naming.py` & `cloudaciousiac-0.0.6/src/cloudaciousIAC/Naming.py`

 * *Files identical despite different names*

### Comparing `cloudaciousiac-0.0.5/src/cloudaciousIAC/README.md` & `cloudaciousiac-0.0.6/src/cloudaciousIAC/README.md`

 * *Files identical despite different names*

### Comparing `cloudaciousiac-0.0.5/src/cloudaciousIAC/StackInfo.py` & `cloudaciousiac-0.0.6/src/cloudaciousIAC/StackInfo.py`

 * *Files identical despite different names*

### Comparing `cloudaciousiac-0.0.5/.gitignore` & `cloudaciousiac-0.0.6/.gitignore`

 * *Files identical despite different names*

