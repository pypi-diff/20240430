# Comparing `tmp/pytest_pyodide-0.56.2.tar.gz` & `tmp/pytest_pyodide-0.57.0.tar.gz`

## Comparing `pytest_pyodide-0.56.2.tar` & `pytest_pyodide-0.57.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/.flake8
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/CHANGELOG.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/COMPATIBILITY.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/conftest.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/.github/FUNDING.yml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/.github/codecov.yml
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/.github/workflows/build.yaml
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/.github/workflows/main.yaml
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/.github/workflows/testall.yaml
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/examples/test_install_package.py
--rw-r--r--   0        0        0    93002 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/__init__.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/_decorator_in_pyodide.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/copy_files_to_pyodide.py
--rw-r--r--   0        0        0    16308 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/decorator.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/doctest.py
--rw-r--r--   0        0        0    10962 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/fixture.py
--rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/hook.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/hypothesis.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/node_test_driver.js
--rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/run_tests_inside_pyodide.py
--rw-r--r--   0        0        0    18965 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/runner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/server.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/utils.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/_templates/module_test.html
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/_templates/module_webworker_dev.js
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/_templates/test.html
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pytest_pyodide/_templates/webworker_dev.js
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_ci.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_copy_files.py
--rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_decorator.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_doctest.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_fixture.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_jsassert.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_marker.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_options.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_run_in_pyodide.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_server.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_testing.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/test_webworker.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/datafiles/in_pyodide_tests.py
--rw-r--r--   0        0        0     9613 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/utils/build_test_matrix.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/LICENSE
--rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/README.md
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/pyproject.toml
--rw-r--r--   0        0        0    30497 2020-02-02 00:00:00.000000 pytest_pyodide-0.56.2/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/.flake8
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/CHANGELOG.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/COMPATIBILITY.md
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/conftest.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/.github/codecov.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/.github/workflows/testall.yaml
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/examples/test_install_package.py
+-rw-r--r--   0        0        0    93002 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/__init__.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/_decorator_in_pyodide.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/copy_files_to_pyodide.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/decorator.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/doctest.py
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/fixture.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/hook.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/hypothesis.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/node_test_driver.js
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/run_tests_inside_pyodide.py
+-rw-r--r--   0        0        0    19245 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/runner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/server.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/utils.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/_templates/module_test.html
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/_templates/module_webworker_dev.js
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/_templates/test.html
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pytest_pyodide/_templates/webworker_dev.js
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_ci.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_copy_files.py
+-rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_decorator.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_doctest.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_fixture.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_jsassert.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_marker.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_options.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_run_in_pyodide.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_server.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_testing.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/test_webworker.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/datafiles/in_pyodide_tests.py
+-rw-r--r--   0        0        0     9613 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl
+-rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/utils/build_test_matrix.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/LICENSE
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/README.md
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/pyproject.toml
+-rw-r--r--   0        0        0    30503 2020-02-02 00:00:00.000000 pytest_pyodide-0.57.0/PKG-INFO
```

### Comparing `pytest_pyodide-0.56.2/.pre-commit-config.yaml` & `pytest_pyodide-0.57.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/CHANGELOG.md` & `pytest_pyodide-0.57.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## [0.57.0] - 2024-04-30
+
+- Fixed safari compatibility with Selenium 4.20
+  [#135](https://github.com/pyodide/pytest-pyodide/pull/135)
 
 ## [0.56.1] - 2023-12-09
 
 - Fixed a bug in webworker test template files.
   [#127](https://github.com/pyodide/pytest-pyodide/pull/127)
 
 ## [0.56.0] - 2023-12-09
```

### Comparing `pytest_pyodide-0.56.2/COMPATIBILITY.md` & `pytest_pyodide-0.57.0/COMPATIBILITY.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Compatible Pyodide versions
 
 Following versions of pytest-pyodide and Pyodide are tested in CI.
 Other versions may work, however with no guarantee.
 
 | pytest-pyodide | Tested Pyodide versions |
-| -------------- | ----------------------- |
-| main branch    | 0.23.4, 0.24.1          |
+|----------------|-------------------------|
+| main branch    | 0.23.4, 0.24.1, 0.25.1  |
+| 0.57.*         | 0.23.4, 0.24.1, 0.25.1  |
 | 0.56.*         | 0.23.4, 0.24.1          |
 | 0.55.*         | 0.23.4, 0.24.1          |
 | 0.54.*         | 0.23.4, 0.24.1          |
 | 0.53.*         | 0.23.2, 0.22.0          |
 | 0.52.*         | 0.23.2, 0.22.0          |
 | 0.51.*         | 0.23.2, 0.22.0, 0.21.3  |
 | 0.50.*         | 0.22.0, 0.21.3          |
```

### Comparing `pytest_pyodide-0.56.2/.github/workflows/build.yaml` & `pytest_pyodide-0.57.0/.github/workflows/build.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   test:
       uses: ./.github/workflows/testall.yaml
       with:
         build-artifact-name: none
         build-artifact-path: none
-        pyodide-versions: "0.24.1,0.23.4"
+        pyodide-versions: "0.25.1,0.24.1,0.23.4"
 
   deploy:
     runs-on: ubuntu-20.04
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     environment: PyPi-deploy
     steps:
       - uses: actions/checkout@v3
```

### Comparing `pytest_pyodide-0.56.2/.github/workflows/main.yaml` & `pytest_pyodide-0.57.0/.github/workflows/main.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,16 @@
       - name: Install pytest-pyodide
         shell: bash -l {0}
         run: |
           if [ -d "pytest_pyodide" ]; then
             # Currently we only install the package for dependencies.
             # We then uninstall it otherwise tests fails due to pytest hook being
             # registered twice.
-              ${{needs.get_versions.outputs.pythonexec}} -m pip install ".[test]"
+            # temporarily pin pytest version (https://github.com/pyodide/pytest-pyodide/pull/133#issuecomment-2081412407)
+              ${{needs.get_versions.outputs.pythonexec}} -m pip install ".[test]" "pytest<8.0.0"
           else
               ${{needs.get_versions.outputs.pythonexec}} -m pip install pytest-pyodide
           fi
       - name: Run tests
         shell: bash -l {0}
         run: |
           pytest -v \
```

### Comparing `pytest_pyodide-0.56.2/.github/workflows/testall.yaml` & `pytest_pyodide-0.57.0/.github/workflows/testall.yaml`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/examples/test_install_package.py` & `pytest_pyodide-0.57.0/examples/test_install_package.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl` & `pytest_pyodide-0.57.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/__init__.py` & `pytest_pyodide-0.57.0/pytest_pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/_decorator_in_pyodide.py` & `pytest_pyodide-0.57.0/pytest_pyodide/_decorator_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/copy_files_to_pyodide.py` & `pytest_pyodide-0.57.0/pytest_pyodide/copy_files_to_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/decorator.py` & `pytest_pyodide-0.57.0/pytest_pyodide/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .runner import _BrowserBaseRunner
 from .utils import package_is_built as _package_is_built
 
 MaybeAsyncFuncDef = ast.FunctionDef | ast.AsyncFunctionDef
 
 
 def package_is_built(package_name: str):
-    return _package_is_built(package_name, pytest.pyodide_dist_dir)  # type: ignore[arg-type]
+    return _package_is_built(package_name, pytest.pyodide_dist_dir)
 
 
 class SeleniumType(Protocol):
     JavascriptException: type
     browser: str
 
     def load_package(self, pkgs: str | list[str]):
@@ -431,14 +431,15 @@
 
         statements, funcdef = _locate_funcdef(module_ast, f)
         inner_funcdef = prepare_inner_funcdef(funcdef)
         statements.append(inner_funcdef)
         new_ast_module = ast.Module(statements, type_ignores=[])
 
         wrapper = _create_outer_func(self._run, funcdef, f)
+        functools.update_wrapper(wrapper, f)
 
         # Store information needed by self._code_template
         self._mod = new_ast_module
         self._module_filename = module_filename
         self._func_name = f.__name__
         self._async_func = isinstance(funcdef, ast.AsyncFunctionDef)
         return wrapper
```

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/doctest.py` & `pytest_pyodide-0.57.0/pytest_pyodide/doctest.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/fixture.py` & `pytest_pyodide-0.57.0/pytest_pyodide/fixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 # browser name: (attr_name, flags)
                 "firefox": ("firefox", FIREFOX_FLAGS),
                 "chrome": ("chromium", CHROME_FLAGS),
                 # TODO: enable webkit
                 # "webkit": (),
             }
             try:
-                for runtime in runtimes:  # type: ignore[attr-defined]
+                for runtime in runtimes:
                     if runtime not in supported_browsers:
                         pytest.exit(
                             f"Unsupported runtime for playwright: {runtime}",
                             returncode=1,
                         )
 
                     attr_name, flags = supported_browsers[runtime]
```

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/hook.py` & `pytest_pyodide-0.57.0/pytest_pyodide/hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     config.option.dist_dir = Path(config.option.dist_dir).resolve()
     run_host, runtimes = _filter_runtimes(config.option.runtime)
 
     if not hasattr(pytest, "pyodide_options_stack"):
         pytest.pyodide_options_stack = []
     else:
-        pytest.pyodide_options_stack.append(  # type:ignore[attr-defined]
+        pytest.pyodide_options_stack.append(
             [
                 pytest.pyodide_run_host_test,
                 pytest.pyodide_runtimes,
                 pytest.pyodide_dist_dir,
             ]
         )
     pytest.pyodide_run_host_test = run_host
```

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/hypothesis.py` & `pytest_pyodide-0.57.0/pytest_pyodide/hypothesis.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/node_test_driver.js` & `pytest_pyodide-0.57.0/pytest_pyodide/node_test_driver.js`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/run_tests_inside_pyodide.py` & `pytest_pyodide-0.57.0/pytest_pyodide/run_tests_inside_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/runner.py` & `pytest_pyodide-0.57.0/pytest_pyodide/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,25 +461,33 @@
 # often causes unexpected errors. So we make a global webdriver instance and
 # reuse it.
 GLOBAL_SAFARI_WEBDRIVER = None
 
 
 @pytest.fixture(scope="session", autouse=True)
 def use_global_safari_service():
-    if "safari" in pytest.pyodide_runtimes:  # type: ignore[operator]
+    if "safari" in pytest.pyodide_runtimes:
         global GLOBAL_SAFARI_WEBDRIVER
 
         from selenium.webdriver.common.driver_finder import DriverFinder
         from selenium.webdriver.safari.options import Options
         from selenium.webdriver.safari.service import Service
 
         GLOBAL_SAFARI_WEBDRIVER = Service(reuse_service=True)
-        GLOBAL_SAFARI_WEBDRIVER.path = DriverFinder.get_path(
-            GLOBAL_SAFARI_WEBDRIVER, Options()
-        )
+
+        try:
+            # selenium >= 4.20
+            # https://github.com/SeleniumHQ/selenium/pull/13387
+            finder = DriverFinder(GLOBAL_SAFARI_WEBDRIVER, Options())
+            browser_path = finder.get_driver_path()
+        except Exception:
+            # selenium < 4.20
+            browser_path = DriverFinder.get_path(GLOBAL_SAFARI_WEBDRIVER, Options())
+
+        GLOBAL_SAFARI_WEBDRIVER.path = browser_path
         GLOBAL_SAFARI_WEBDRIVER.start()
 
         try:
             yield GLOBAL_SAFARI_WEBDRIVER
         finally:
             GLOBAL_SAFARI_WEBDRIVER.stop()
     else:
```

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/server.py` & `pytest_pyodide-0.57.0/pytest_pyodide/server.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/utils.py` & `pytest_pyodide-0.57.0/pytest_pyodide/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/_templates/module_test.html` & `pytest_pyodide-0.57.0/pytest_pyodide/_templates/module_test.html`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/_templates/module_webworker_dev.js` & `pytest_pyodide-0.57.0/pytest_pyodide/_templates/module_webworker_dev.js`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/_templates/test.html` & `pytest_pyodide-0.57.0/pytest_pyodide/_templates/test.html`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/pytest_pyodide/_templates/webworker_dev.js` & `pytest_pyodide-0.57.0/pytest_pyodide/_templates/webworker_dev.js`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_ci.py` & `pytest_pyodide-0.57.0/tests/test_ci.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_copy_files.py` & `pytest_pyodide-0.57.0/tests/test_copy_files.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_decorator.py` & `pytest_pyodide-0.57.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_doctest.py` & `pytest_pyodide-0.57.0/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_fixture.py` & `pytest_pyodide-0.57.0/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_jsassert.py` & `pytest_pyodide-0.57.0/tests/test_jsassert.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_options.py` & `pytest_pyodide-0.57.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_run_in_pyodide.py` & `pytest_pyodide-0.57.0/tests/test_run_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_server.py` & `pytest_pyodide-0.57.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/test_testing.py` & `pytest_pyodide-0.57.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/datafiles/in_pyodide_tests.py` & `pytest_pyodide-0.57.0/tests/datafiles/in_pyodide_tests.py`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl` & `pytest_pyodide-0.57.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/utils/build_test_matrix.py` & `pytest_pyodide-0.57.0/utils/build_test_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import json
 
 DEFAULT_OS = "ubuntu-20.04, macos-11"
 DEFAULT_RUNNER = "selenium, playwright"
 DEFAULT_BROWSER = "chrome, firefox, node, safari, host"
 DEFAULT_CHROME_VERSION = "latest"
 DEFAULT_FIREFOX_VERSION = "latest"
-DEFAULT_NODE_VERSION = "18, 20"
+DEFAULT_NODE_VERSION = "20"
 DEFAULT_PLAYWRIGHT_VERSION = (
     "1.22.0"  # TODO: versions > 1.22.0 have firefox performance issue
 )
 
 
 @dataclasses.dataclass
 class TestConfig:
```

### Comparing `pytest_pyodide-0.56.2/LICENSE` & `pytest_pyodide-0.57.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_pyodide-0.56.2/README.md` & `pytest_pyodide-0.57.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # pytest-pyodide
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pytest-pyodide.svg)](https://pypi.org/project/pytest-pyodide/)
-![GHA](https://github.com/pyodide/pytest-pyodide/actions/workflows/main.yml/badge.svg)
+![GHA](https://github.com/pyodide/pytest-pyodide/actions/workflows/build.yml/badge.svg)
 [![codecov](https://codecov.io/gh/pyodide/pytest-pyodide/branch/main/graph/badge.svg?token=U7tWHpJj5c)](https://codecov.io/gh/pyodide/pytest-pyodide)
 
 
 Pytest plugin for testing applications that use Pyodide
 
 ## Installation
 
 pytest-pyodide requires Python 3.10+ and can be installed with
 ```
 pip install pytest-pyodide
 ```
-You would also one at least one of the following runtimes,
+You would also need one at least one of the following runtimes:
  - Chrome and chromedriver
  - Firefox and geckodriver
  - Safari and safaridriver
  - node v18+
 
 ## Github Reusable workflow
```

### Comparing `pytest_pyodide-0.56.2/pyproject.toml` & `pytest_pyodide-0.57.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 source = "vcs"
 
 [tool.mypy]
 python_version = "3.10"
 show_error_codes = true
 warn_unreachable = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
+disable_error_code = ["attr-defined"]
 
 # Strict checks
 warn_unused_configs = true
 check_untyped_defs = true
 disallow_subclassing_any = false
 no_implicit_optional = true
 warn_redundant_casts = true
```

### Comparing `pytest_pyodide-0.56.2/PKG-INFO` & `pytest_pyodide-0.57.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pytest-pyodide
-Version: 0.56.2
+Version: 0.57.0
 Summary: Pytest plugin for testing applications that use Pyodide
 Project-URL: Homepage, https://github.com/pyodide/pytest-pyodide
 Project-URL: Repository, https://github.com/pyodide/pytest-pyodide
 Project-URL: Changelog, https://github.com/pyodide/pytest-pyodide/blob/main/CHANGELOG.md
 License: Mozilla Public License Version 2.0
         ==================================
         
@@ -396,27 +396,27 @@
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: requests; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pytest-pyodide
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pytest-pyodide.svg)](https://pypi.org/project/pytest-pyodide/)
-![GHA](https://github.com/pyodide/pytest-pyodide/actions/workflows/main.yml/badge.svg)
+![GHA](https://github.com/pyodide/pytest-pyodide/actions/workflows/build.yml/badge.svg)
 [![codecov](https://codecov.io/gh/pyodide/pytest-pyodide/branch/main/graph/badge.svg?token=U7tWHpJj5c)](https://codecov.io/gh/pyodide/pytest-pyodide)
 
 
 Pytest plugin for testing applications that use Pyodide
 
 ## Installation
 
 pytest-pyodide requires Python 3.10+ and can be installed with
 ```
 pip install pytest-pyodide
 ```
-You would also one at least one of the following runtimes,
+You would also need one at least one of the following runtimes:
  - Chrome and chromedriver
  - Firefox and geckodriver
  - Safari and safaridriver
  - node v18+
 
 ## Github Reusable workflow
```

