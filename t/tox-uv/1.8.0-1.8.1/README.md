# Comparing `tmp/tox_uv-1.8.0.tar.gz` & `tmp/tox_uv-1.8.1.tar.gz`

## Comparing `tox_uv-1.8.0.tar` & `tox_uv-1.8.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/__init__.py
--rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_installer.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_package.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_run.py
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_venv.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_venv_query.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/py.typed
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/version.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/conftest.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_tox_uv_api.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_tox_uv_installer.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_tox_uv_package.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_tox_uv_venv.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_version.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_uv-1.8.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_uv-1.8.0/LICENSE
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 tox_uv-1.8.0/README.md
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 tox_uv-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 tox_uv-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/__init__.py
+-rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/_installer.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/_package.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/_run.py
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/_venv.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/_venv_query.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/py.typed
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tox_uv-1.8.1/src/tox_uv/version.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/conftest.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/test_tox_uv_api.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/test_tox_uv_installer.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/test_tox_uv_package.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/test_tox_uv_venv.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/test_version.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox_uv-1.8.1/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_uv-1.8.1/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_uv-1.8.1/LICENSE
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 tox_uv-1.8.1/README.md
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 tox_uv-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 tox_uv-1.8.1/PKG-INFO
```

### Comparing `tox_uv-1.8.0/src/tox_uv/_installer.py` & `tox_uv-1.8.1/src/tox_uv/_installer.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/src/tox_uv/_package.py` & `tox_uv-1.8.1/src/tox_uv/_package.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/src/tox_uv/_run.py` & `tox_uv-1.8.1/src/tox_uv/_run.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/src/tox_uv/_venv.py` & `tox_uv-1.8.1/src/tox_uv/_venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         else:  # pragma: win32 no cover # noqa: RET505
             py = self._py_info
             impl = "pypy" if py.implementation == "pypy" else "python"
             return self.venv_dir / "lib" / f"{impl}{py.version_dot}" / "site-packages"
 
     @cached_property
     def _py_info(self) -> PythonInfo:  # pragma: win32 no cover
-        if not (self._created or self.env_dir.exists()):  # called during config, no environment setup
+        if not self._created and not self.env_python().exists():  # called during config, no environment setup
             self.create_python_env()
             self._paths = self.prepend_env_var_path()
         with as_file(files("tox_uv") / "_venv_query.py") as filename:
             cmd = [str(self.env_python()), str(filename)]
             outcome = self.execute(cmd, stdin=StdinSource.OFF, run_id="venv-query", show=False)
         outcome.assert_success()
         res = json.loads(outcome.out)
```

### Comparing `tox_uv-1.8.0/src/tox_uv/plugin.py` & `tox_uv-1.8.1/src/tox_uv/plugin.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/tests/test_tox_uv_api.py` & `tox_uv-1.8.1/tests/test_tox_uv_api.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/tests/test_tox_uv_installer.py` & `tox_uv-1.8.1/tests/test_tox_uv_installer.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/tests/test_tox_uv_package.py` & `tox_uv-1.8.1/tests/test_tox_uv_package.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/tests/test_tox_uv_venv.py` & `tox_uv-1.8.1/tests/test_tox_uv_venv.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/tests/demo_pkg_inline/build.py` & `tox_uv-1.8.1/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/LICENSE` & `tox_uv-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/README.md` & `tox_uv-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/pyproject.toml` & `tox_uv-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.0/PKG-INFO` & `tox_uv-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tox-uv
-Version: 1.8.0
+Version: 1.8.1
 Summary: Integration of uv with tox.
 Project-URL: Changelog, https://github.com/tox-dev/tox-uv/releases
 Project-URL: Documentation, https://github.com/tox-dev/tox-uv#tox-uv
 Project-URL: Homepage, https://github.com/tox-dev/tox-uv
 Project-URL: Source, https://github.com/tox-dev/tox-uv
 Project-URL: Tracker, https://github.com/tox-dev/tox-uv/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
```

