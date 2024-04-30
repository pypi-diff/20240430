# Comparing `tmp/ql_cq-1.8.0.tar.gz` & `tmp/ql_cq-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ql_cq-1.8.0.tar", max compression
+gzip compressed data, was "ql_cq-1.9.0.tar", max compression
```

## Comparing `ql_cq-1.8.0.tar` & `ql_cq-1.9.0.tar`

### file list

```diff
@@ -1,49 +1,47 @@
--rw-r--r--   0        0        0      584 2024-03-02 15:21:48.173504 ql_cq-1.8.0/LICENSE.txt
--rw-r--r--   0        0        0     3498 2024-03-02 15:21:48.173504 ql_cq-1.8.0/README.md
--rw-r--r--   0        0        0        0 2024-03-02 15:21:48.173504 ql_cq-1.8.0/cq/__init__.py
--rw-r--r--   0        0        0      422 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checker.py
--rw-r--r--   0        0        0        0 2024-03-02 15:21:48.173504 ql_cq-1.8.0/cq/checkers/__init__.py
--rw-r--r--   0        0        0     1144 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/git.py
--rw-r--r--   0        0        0     1561 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/init.py
--rw-r--r--   0        0        0     1239 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/isort.py
--rw-r--r--   0        0        0      542 2024-03-02 15:21:48.173504 ql_cq-1.8.0/cq/checkers/isort_config.py
--rw-r--r--   0        0        0     1273 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/mypy.py
--rw-r--r--   0        0        0     1554 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/orange.py
--rw-r--r--   0        0        0     1484 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/pyflakes.py
--rw-r--r--   0        0        0     4868 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/pylint.py
--rw-r--r--   0        0        0    13842 2024-03-02 15:21:48.173504 ql_cq-1.8.0/cq/checkers/pylintrc
--rw-r--r--   0        0        0     8589 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/regex.py
--rw-r--r--   0        0        0     7865 2024-03-18 17:38:10.288221 ql_cq-1.8.0/cq/checkers/requirements.py
--rw-r--r--   0        0        0      867 2024-03-19 08:01:56.033523 ql_cq-1.8.0/cq/checkers/ruff.py
--rw-r--r--   0        0        0     2615 2024-03-19 08:01:56.033523 ql_cq-1.8.0/cq/checkers/safety.py
--rw-r--r--   0        0        0     1000 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/setup.py
--rw-r--r--   0        0        0       23 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/checkers/test/data/formatted.txt
--rw-r--r--   0        0        0      117 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/checkers/test/data/isort.txt
--rw-r--r--   0        0        0       24 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/checkers/test/data/not-formatted.txt
--rw-r--r--   0        0        0     1062 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/checkers/test/test_git.py
--rw-r--r--   0        0        0     2486 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/checkers/test/test_init.py
--rw-r--r--   0        0        0      657 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/checkers/test/test_isort.py
--rw-r--r--   0        0        0      903 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/test/test_mypy.py
--rw-r--r--   0        0        0     1352 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/test/test_orange.py
--rw-r--r--   0        0        0      952 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/test/test_pyflakes.py
--rw-r--r--   0        0        0      991 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/test/test_pylint.py
--rw-r--r--   0        0        0     4361 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/checkers/test/test_regex.py
--rw-r--r--   0        0        0     3677 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/checkers/test/test_requirements.py
--rw-r--r--   0        0        0      933 2024-03-19 08:01:56.033523 ql_cq-1.8.0/cq/checkers/test/test_ruff.py
--rw-r--r--   0        0        0     2498 2024-03-18 17:16:06.971997 ql_cq-1.8.0/cq/checkers/test/test_safety.py
--rw-r--r--   0        0        0      160 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixer.py
--rw-r--r--   0        0        0        0 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/__init__.py
--rw-r--r--   0        0        0      400 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/isort_fixer.py
--rw-r--r--   0        0        0      271 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/orange.py
--rw-r--r--   0        0        0      307 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/test/data/isort-result.txt
--rw-r--r--   0        0        0      305 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/test/data/isort-test.txt
--rw-r--r--   0        0        0       23 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/test/data/orange-result.txt
--rw-r--r--   0        0        0       24 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/test/data/orange-test.txt
--rw-r--r--   0        0        0      576 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/test/test_isort_fixer.py
--rw-r--r--   0        0        0      577 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/fixers/test/test_orange_fixer.py
--rw-r--r--   0        0        0     6811 2024-03-19 08:01:56.033523 ql_cq-1.8.0/cq/main.py
--rw-r--r--   0        0        0     1033 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/test/test_cq.py
--rw-r--r--   0        0        0     1778 2024-03-02 15:21:48.177504 ql_cq-1.8.0/cq/test/test_utils.py
--rw-r--r--   0        0        0     2602 2024-03-19 08:01:56.033523 ql_cq-1.8.0/cq/utils.py
--rw-r--r--   0        0        0     1098 2024-03-19 08:02:20.381263 ql_cq-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 ql_cq-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      584 2024-03-02 15:21:48.173504 ql_cq-1.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     3274 2024-04-30 14:54:25.767989 ql_cq-1.9.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-02 15:21:48.173504 ql_cq-1.9.0/cq/__init__.py
+-rw-r--r--   0        0        0      422 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checker.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:21:48.173504 ql_cq-1.9.0/cq/checkers/__init__.py
+-rw-r--r--   0        0        0     1144 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/git.py
+-rw-r--r--   0        0        0     1561 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/init.py
+-rw-r--r--   0        0        0     1239 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/isort.py
+-rw-r--r--   0        0        0      542 2024-03-02 15:21:48.173504 ql_cq-1.9.0/cq/checkers/isort_config.py
+-rw-r--r--   0        0        0     1273 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/mypy.py
+-rw-r--r--   0        0        0     1554 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/orange.py
+-rw-r--r--   0        0        0     1484 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/pyflakes.py
+-rw-r--r--   0        0        0     4868 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/pylint.py
+-rw-r--r--   0        0        0    13842 2024-03-02 15:21:48.173504 ql_cq-1.9.0/cq/checkers/pylintrc
+-rw-r--r--   0        0        0     8589 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/regex.py
+-rw-r--r--   0        0        0      867 2024-03-19 08:01:56.033523 ql_cq-1.9.0/cq/checkers/ruff.py
+-rw-r--r--   0        0        0     2615 2024-04-30 15:07:42.289982 ql_cq-1.9.0/cq/checkers/safety.py
+-rw-r--r--   0        0        0     1000 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/setup.py
+-rw-r--r--   0        0        0       23 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/checkers/test/data/formatted.txt
+-rw-r--r--   0        0        0      117 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/checkers/test/data/isort.txt
+-rw-r--r--   0        0        0       24 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/checkers/test/data/not-formatted.txt
+-rw-r--r--   0        0        0     1062 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/checkers/test/test_git.py
+-rw-r--r--   0        0        0     2486 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/checkers/test/test_init.py
+-rw-r--r--   0        0        0      657 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/checkers/test/test_isort.py
+-rw-r--r--   0        0        0      903 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/test/test_mypy.py
+-rw-r--r--   0        0        0     1352 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/test/test_orange.py
+-rw-r--r--   0        0        0      952 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/test/test_pyflakes.py
+-rw-r--r--   0        0        0      991 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/test/test_pylint.py
+-rw-r--r--   0        0        0     4361 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/checkers/test/test_regex.py
+-rw-r--r--   0        0        0      933 2024-03-19 08:01:56.033523 ql_cq-1.9.0/cq/checkers/test/test_ruff.py
+-rw-r--r--   0        0        0     2498 2024-03-18 17:16:06.971997 ql_cq-1.9.0/cq/checkers/test/test_safety.py
+-rw-r--r--   0        0        0      160 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixer.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/__init__.py
+-rw-r--r--   0        0        0      400 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/isort_fixer.py
+-rw-r--r--   0        0        0      271 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/orange.py
+-rw-r--r--   0        0        0      307 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/test/data/isort-result.txt
+-rw-r--r--   0        0        0      305 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/test/data/isort-test.txt
+-rw-r--r--   0        0        0       23 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/test/data/orange-result.txt
+-rw-r--r--   0        0        0       24 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/test/data/orange-test.txt
+-rw-r--r--   0        0        0      576 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/test/test_isort_fixer.py
+-rw-r--r--   0        0        0      577 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/fixers/test/test_orange_fixer.py
+-rw-r--r--   0        0        0     6655 2024-04-30 14:54:25.767989 ql_cq-1.9.0/cq/main.py
+-rw-r--r--   0        0        0     1033 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/test/test_cq.py
+-rw-r--r--   0        0        0     1778 2024-03-02 15:21:48.177504 ql_cq-1.9.0/cq/test/test_utils.py
+-rw-r--r--   0        0        0     2602 2024-03-19 08:01:56.033523 ql_cq-1.9.0/cq/utils.py
+-rw-r--r--   0        0        0     1098 2024-04-30 15:07:54.145753 ql_cq-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4367 1970-01-01 00:00:00.000000 ql_cq-1.9.0/PKG-INFO
```

### Comparing `ql_cq-1.8.0/LICENSE.txt` & `ql_cq-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/README.md` & `ql_cq-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -57,16 +57,14 @@
 
 ## Checkers
 - [`pylint`](https://www.pylint.org/) - comprehensive linter
 - [`mypy`](http://mypy-lang.org/) - checks python typing
 - [`pyflakes-ext`](https://pypi.org/project/pyflakes-ext/) - another general linter
 - `grammar_nazi` - grammar/spelling errors
 - `dumb_style_checker` - basic python mistakes (e.g. use of print in a library)
-- `requirements_setup_compatibility` - validation of version compatibility between setup.py and requirements.txt
-- [`requirements-validator`](https://pip.pypa.io/en/latest/reference/pip_check/) - requirements.txt validation
 - [`setup_check`](https://docs.python.org/3/distutils/examples.html#checking-a-package) - setup.py validator
 - `branch_name_check` - check whether current branch name comply with Quantlane standards
 - [`orange`](https://gitlab.com/quantlane/meta/orange) - code formatter based on `black`
 - [`isort`](https://github.com/PyCQA/isort) - isort your imports, so you don't have to
 - [`safety`](https://github.com/pyupio/safety) - checks installed dependencies for known security vulnerabilities
 
 ## Fixers
```

### Comparing `ql_cq-1.8.0/cq/checkers/git.py` & `ql_cq-1.9.0/cq/checkers/git.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/init.py` & `ql_cq-1.9.0/cq/checkers/init.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/isort.py` & `ql_cq-1.9.0/cq/checkers/isort.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/isort_config.py` & `ql_cq-1.9.0/cq/checkers/isort_config.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/mypy.py` & `ql_cq-1.9.0/cq/checkers/mypy.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/orange.py` & `ql_cq-1.9.0/cq/checkers/orange.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/pyflakes.py` & `ql_cq-1.9.0/cq/checkers/pyflakes.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/pylint.py` & `ql_cq-1.9.0/cq/checkers/pylint.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/pylintrc` & `ql_cq-1.9.0/cq/checkers/pylintrc`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/regex.py` & `ql_cq-1.9.0/cq/checkers/regex.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/ruff.py` & `ql_cq-1.9.0/cq/checkers/ruff.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/safety.py` & `ql_cq-1.9.0/cq/checkers/safety.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/setup.py` & `ql_cq-1.9.0/cq/checkers/setup.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_git.py` & `ql_cq-1.9.0/cq/checkers/test/test_git.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_init.py` & `ql_cq-1.9.0/cq/checkers/test/test_init.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_isort.py` & `ql_cq-1.9.0/cq/checkers/test/test_isort.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_mypy.py` & `ql_cq-1.9.0/cq/checkers/test/test_mypy.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_orange.py` & `ql_cq-1.9.0/cq/checkers/test/test_orange.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_pyflakes.py` & `ql_cq-1.9.0/cq/checkers/test/test_pyflakes.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_pylint.py` & `ql_cq-1.9.0/cq/checkers/test/test_pylint.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_regex.py` & `ql_cq-1.9.0/cq/checkers/test/test_regex.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_ruff.py` & `ql_cq-1.9.0/cq/checkers/test/test_ruff.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/checkers/test/test_safety.py` & `ql_cq-1.9.0/cq/checkers/test/test_safety.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/fixers/test/test_isort_fixer.py` & `ql_cq-1.9.0/cq/fixers/test/test_isort_fixer.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/fixers/test/test_orange_fixer.py` & `ql_cq-1.9.0/cq/fixers/test/test_orange_fixer.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/main.py` & `ql_cq-1.9.0/cq/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,28 @@
 import cq.checkers.init
 import cq.checkers.isort
 import cq.checkers.mypy
 import cq.checkers.orange
 import cq.checkers.pyflakes
 import cq.checkers.pylint
 import cq.checkers.regex
-import cq.checkers.requirements
 import cq.checkers.ruff
 import cq.checkers.safety
 import cq.checkers.setup
 import cq.fixer
 import cq.fixers.isort_fixer
 import cq.fixers.orange
 
 
 checkers: List[cq.checker.Checker] = [
 	cq.checkers.pylint.PylintChecker(),
 	cq.checkers.mypy.MypyChecker(),
 	cq.checkers.pyflakes.PyflakesExtChecker(),
 	cq.checkers.regex.GrammarNaziChecker(),
 	cq.checkers.regex.DumbStyleChecker(),
-	cq.checkers.requirements.RequirementsSetupCompatiblityChecker(),
-	cq.checkers.requirements.RequirementsvalidatorChecker(),
 	cq.checkers.setup.SetupChecker(),
 	cq.checkers.git.BranchNameChecker(),
 	cq.checkers.init.InitChecker(),
 	cq.checkers.orange.OrangeChecker(),
 	cq.checkers.isort.IsortChecker(),
 	cq.checkers.safety.SafetyChecker(),
 	cq.checkers.ruff.RuffChecker(),
```

### Comparing `ql_cq-1.8.0/cq/test/test_cq.py` & `ql_cq-1.9.0/cq/test/test_cq.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/test/test_utils.py` & `ql_cq-1.9.0/cq/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/cq/utils.py` & `ql_cq-1.9.0/cq/utils.py`

 * *Files identical despite different names*

### Comparing `ql_cq-1.8.0/pyproject.toml` & `ql_cq-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ql-cq"
-version = "1.8.0"
+version = "1.9.0"
 description = "Code quality checker"
 authors = ["Quantlane <code@quantlane.com>"]
 license = "Apache License, Version 2.0"
 homepage = "https://gitlab.com/quantlane/meta/cq"
 readme = "README.md"
 packages = [
     { include = "cq" },
```

### Comparing `ql_cq-1.8.0/PKG-INFO` & `ql_cq-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ql-cq
-Version: 1.8.0
+Version: 1.9.0
 Summary: Code quality checker
 Home-page: https://gitlab.com/quantlane/meta/cq
 License: Apache License, Version 2.0
 Author: Quantlane
 Author-email: code@quantlane.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -86,16 +86,14 @@
 
 ## Checkers
 - [`pylint`](https://www.pylint.org/) - comprehensive linter
 - [`mypy`](http://mypy-lang.org/) - checks python typing
 - [`pyflakes-ext`](https://pypi.org/project/pyflakes-ext/) - another general linter
 - `grammar_nazi` - grammar/spelling errors
 - `dumb_style_checker` - basic python mistakes (e.g. use of print in a library)
-- `requirements_setup_compatibility` - validation of version compatibility between setup.py and requirements.txt
-- [`requirements-validator`](https://pip.pypa.io/en/latest/reference/pip_check/) - requirements.txt validation
 - [`setup_check`](https://docs.python.org/3/distutils/examples.html#checking-a-package) - setup.py validator
 - `branch_name_check` - check whether current branch name comply with Quantlane standards
 - [`orange`](https://gitlab.com/quantlane/meta/orange) - code formatter based on `black`
 - [`isort`](https://github.com/PyCQA/isort) - isort your imports, so you don't have to
 - [`safety`](https://github.com/pyupio/safety) - checks installed dependencies for known security vulnerabilities
 
 ## Fixers
```

