# Comparing `tmp/tox_uv-1.7.0.tar.gz` & `tmp/tox_uv-1.8.0.tar.gz`

## Comparing `tox_uv-1.7.0.tar` & `tox_uv-1.8.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tox_uv-1.7.0/src/tox_uv/__init__.py
--rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 tox_uv-1.7.0/src/tox_uv/_installer.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tox_uv-1.7.0/src/tox_uv/_package.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tox_uv-1.7.0/src/tox_uv/_run.py
--rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 tox_uv-1.7.0/src/tox_uv/_venv.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 tox_uv-1.7.0/src/tox_uv/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_uv-1.7.0/src/tox_uv/py.typed
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tox_uv-1.7.0/src/tox_uv/version.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/conftest.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/test_tox_uv_api.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/test_tox_uv_installer.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/test_tox_uv_package.py
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/test_tox_uv_venv.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/test_version.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox_uv-1.7.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_uv-1.7.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_uv-1.7.0/LICENSE
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 tox_uv-1.7.0/README.md
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 tox_uv-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 tox_uv-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/__init__.py
+-rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_installer.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_package.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_run.py
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_venv.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/_venv_query.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/py.typed
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tox_uv-1.8.0/src/tox_uv/version.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/conftest.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_tox_uv_api.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_tox_uv_installer.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_tox_uv_package.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_tox_uv_venv.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/test_version.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox_uv-1.8.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_uv-1.8.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_uv-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 tox_uv-1.8.0/README.md
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 tox_uv-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 tox_uv-1.8.0/PKG-INFO
```

### Comparing `tox_uv-1.7.0/src/tox_uv/_installer.py` & `tox_uv-1.8.0/src/tox_uv/_installer.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/src/tox_uv/_package.py` & `tox_uv-1.8.0/src/tox_uv/_package.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/src/tox_uv/_run.py` & `tox_uv-1.8.0/src/tox_uv/_run.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/src/tox_uv/_venv.py` & `tox_uv-1.8.0/src/tox_uv/_venv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 """GitHub Actions integration."""
 
 from __future__ import annotations
 
+import json
 import sys
 from abc import ABC
+from functools import cached_property
+
+if sys.version_info >= (3, 9):  # pragma: no cover (py39+)
+    from importlib.resources import as_file, files
+else:  # pragma: no cover (py38+)
+    from importlib_resources import as_file, files
+
+
 from pathlib import Path
 from platform import python_implementation
 from typing import TYPE_CHECKING, Any, cast
 
 from tox.execute.local_sub_process import LocalSubProcessExecutor
 from tox.execute.request import StdinSource
 from tox.tox_env.python.api import Python, PythonInfo, VersionInfo
@@ -22,14 +31,15 @@
     from tox.tox_env.installer import Installer
 
 
 class UvVenv(Python, ABC):
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         self._executor: Execute | None = None
         self._installer: UvInstaller | None = None
+        self._created = False
         super().__init__(create_args)
 
     def register_config(self) -> None:
         super().register_config()
         desc = "add seed packages to the created venv"
         self.conf.add_config(keys=["uv_seed"], of_type=bool, default=False, desc=desc)
 
@@ -108,30 +118,29 @@
         env.append("UV_*")  # accept uv env vars
         if sys.platform == "darwin":  # pragma: darwin cover
             env.append("MACOSX_DEPLOYMENT_TARGET")  # needed for macOS binary builds
         env.append("PKG_CONFIG_PATH")  # needed for binary builds
         return env
 
     def create_python_env(self) -> None:
-        base = self.base_python.version_info
-        version_spec = (
-            sys.executable
-            if (base.major, base.minor) == sys.version_info[:2]
-            else f"{base.major}.{base.minor}"
-            if base.minor
-            else f"{base.major}"
-        )
+        base, imp = self.base_python.version_info, self.base_python.impl_lower
+        if (base.major, base.minor) == sys.version_info[:2] and (sys.implementation.name.lower() == imp):
+            version_spec = sys.executable
+        else:
+            uv_imp = "python" if (imp and imp == "cpython") else imp
+            version_spec = f"{uv_imp or ''}{base.major}.{base.minor}" if base.minor else f"{uv_imp or ''}{base.major}"
         cmd: list[str] = [self.uv, "venv", "-p", version_spec]
         if self.options.verbosity > 2:  # noqa: PLR2004
             cmd.append("-v")
         if self.conf["uv_seed"]:
             cmd.append("--seed")
         cmd.append(str(self.venv_dir))
         outcome = self.execute(cmd, stdin=StdinSource.OFF, run_id="venv", show=None)
         outcome.assert_success()
+        self._created = True
 
     @property
     def _allow_externals(self) -> list[str]:
         result = super()._allow_externals
         result.append(self.uv)
         return result
 
@@ -148,15 +157,40 @@
         suffix = ".exe" if sys.platform == "win32" else ""
         return self.env_bin_dir() / f"python{suffix}"
 
     def env_site_package_dir(self) -> Path:
         if sys.platform == "win32":  # pragma: win32 cover
             return self.venv_dir / "Lib" / "site-packages"
         else:  # pragma: win32 no cover # noqa: RET505
-            assert self.base_python.version_info.major is not None  # noqa: S101
-            assert self.base_python.version_info.minor is not None  # noqa: S101
-            return self.venv_dir / "lib" / f"python{self.base_python.version_dot}" / "site-packages"
+            py = self._py_info
+            impl = "pypy" if py.implementation == "pypy" else "python"
+            return self.venv_dir / "lib" / f"{impl}{py.version_dot}" / "site-packages"
+
+    @cached_property
+    def _py_info(self) -> PythonInfo:  # pragma: win32 no cover
+        if not (self._created or self.env_dir.exists()):  # called during config, no environment setup
+            self.create_python_env()
+            self._paths = self.prepend_env_var_path()
+        with as_file(files("tox_uv") / "_venv_query.py") as filename:
+            cmd = [str(self.env_python()), str(filename)]
+            outcome = self.execute(cmd, stdin=StdinSource.OFF, run_id="venv-query", show=False)
+        outcome.assert_success()
+        res = json.loads(outcome.out)
+        return PythonInfo(
+            implementation=res["implementation"],
+            version_info=VersionInfo(
+                major=res["version_info"][0],
+                minor=res["version_info"][1],
+                micro=res["version_info"][2],
+                releaselevel=res["version_info"][3],
+                serial=res["version_info"][4],
+            ),
+            version=res["version"],
+            is_64=res["is_64"],
+            platform=sys.platform,
+            extra={},
+        )
 
 
 __all__ = [
     "UvVenv",
 ]
```

### Comparing `tox_uv-1.7.0/src/tox_uv/plugin.py` & `tox_uv-1.8.0/src/tox_uv/plugin.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/tests/test_tox_uv_api.py` & `tox_uv-1.8.0/tests/test_tox_uv_api.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/tests/test_tox_uv_installer.py` & `tox_uv-1.8.0/tests/test_tox_uv_installer.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/tests/test_tox_uv_package.py` & `tox_uv-1.8.0/tests/test_tox_uv_package.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/tests/test_tox_uv_venv.py` & `tox_uv-1.8.0/tests/test_tox_uv_venv.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,25 +75,41 @@
     result.assert_success()
 
     exe = "python.exe" if sys.platform == "win32" else "python"
     env_bin_dir = str(project.path / ".tox" / "py" / ".venv" / ("Scripts" if sys.platform == "win32" else "bin") / exe)
     assert env_bin_dir in result.out
 
 
-def test_uv_env_site_package_dir(tox_project: ToxProjectCreator) -> None:
+def test_uv_env_site_package_dir_run(tox_project: ToxProjectCreator) -> None:
     project = tox_project({"tox.ini": "[testenv]\npackage=skip\ncommands=python -c 'print(\"{envsitepackagesdir}\")'"})
     result = project.run("-vv")
     result.assert_success()
 
     env_dir = project.path / ".tox" / "py" / ".venv"
     ver = sys.version_info
     if sys.platform == "win32":  # pragma: win32 cover
         path = str(env_dir / "Lib" / "site-packages")
     else:  # pragma: win32 no cover
-        path = str(env_dir / "lib" / f"python{ver.major}.{ver.minor}" / "site-packages")
+        impl = "pypy" if sys.implementation.name.lower() == "pypy" else "python"
+        path = str(env_dir / "lib" / f"{impl}{ver.major}.{ver.minor}" / "site-packages")
+    assert path in result.out
+
+
+def test_uv_env_site_package_dir_conf(tox_project: ToxProjectCreator) -> None:
+    project = tox_project({"tox.ini": "[testenv]\npackage=skip\ncommands={envsitepackagesdir}"})
+    result = project.run("c", "-e", "py", "-k", "commands")
+    result.assert_success()
+
+    env_dir = project.path / ".tox" / "py" / ".venv"
+    ver = sys.version_info
+    if sys.platform == "win32":  # pragma: win32 cover
+        path = str(env_dir / "Lib" / "site-packages")
+    else:  # pragma: win32 no cover
+        impl = "pypy" if sys.implementation.name.lower() == "pypy" else "python"
+        path = str(env_dir / "lib" / f"{impl}{ver.major}.{ver.minor}" / "site-packages")
     assert path in result.out
 
 
 def test_uv_env_python_not_in_path(tox_project: ToxProjectCreator) -> None:
     # Make sure there is no pythonX.Y in the search path
     ver = sys.version_info
     exe_ext = ".exe" if sys.platform == "win32" else ""
```

### Comparing `tox_uv-1.7.0/tests/demo_pkg_inline/build.py` & `tox_uv-1.8.0/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/LICENSE` & `tox_uv-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/README.md` & `tox_uv-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tox_uv-1.7.0/pyproject.toml` & `tox_uv-1.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.4",
-  "hatchling>=1.21.1",
+  "hatchling>=1.24.2",
 ]
 
 [project]
 name = "tox-uv"
 description = "Integration of uv with tox."
 readme = "README.md"
 keywords = [
   "environments",
   "isolated",
   "testing",
   "virtual",
 ]
 license = "MIT"
-maintainers = [{ name = "Bernát Gábor", email = "gaborjbernat@gmail.com" }]
+maintainers = [
+  { name = "Bernát Gábor", email = "gaborjbernat@gmail.com" },
+]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
@@ -34,44 +36,56 @@
   "Topic :: Software Development :: Libraries",
   "Topic :: System",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "packaging>=23.2",
-  "tox<5,>=4.14",
-  "uv<1,>=0.1.15",
+  'importlib_resources>=6.4; python_version < "3.9"',
+  "packaging>=24",
+  "tox<5,>=4.15",
+  "uv<1,>=0.1.39",
 ]
 optional-dependencies.test = [
   "covdefaults>=2.3",
   "devpi-process>=1",
-  "pytest>=8.0.2",
-  "pytest-cov>=4.1",
-  "pytest-mock>=3.12",
+  "pytest>=8.2",
+  "pytest-cov>=5",
+  "pytest-mock>=3.14",
 ]
+urls.Changelog = "https://github.com/tox-dev/tox-uv/releases"
 urls.Documentation = "https://github.com/tox-dev/tox-uv#tox-uv"
 urls.Homepage = "https://github.com/tox-dev/tox-uv"
 urls.Source = "https://github.com/tox-dev/tox-uv"
 urls.Tracker = "https://github.com/tox-dev/tox-uv/issues"
 entry-points.tox = {"tox-uv" = "tox_uv.plugin"}
 
 [tool.hatch]
 build.hooks.vcs.version-file = "src/tox_uv/version.py"
-build.targets.sdist.include = ["/src", "/tests"]
+build.targets.sdist.include = [
+  "/src",
+  "/tests",
+]
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 target-version = "py38"
-lint.isort = { known-first-party = ["tox_uv", "tests"], required-imports = ["from __future__ import annotations"] }
-lint.select = ["ALL"]
+lint.isort = { known-first-party = [
+  "tox_uv",
+  "tests",
+], required-imports = [
+  "from __future__ import annotations",
+] }
+lint.select = [
+  "ALL",
+]
 lint.ignore = [
   "ANN101", # Missing type annotation for `self` in method
   "D301",   #  Use `r"""` if any backslashes in a docstring
   "D205",   # 1 blank line required between summary line and description
   "D401",   # First line of docstring should be in imperative mood
   "D203",   # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
   "D212",   # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
@@ -99,18 +113,38 @@
 builtin = "clear,usage,en-GB_to_en-US"
 write-changes = true
 count = true
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
-paths.source = ["src", ".tox/*/.venv/lib/*/site-packages", ".tox\\*\\.venv\\Lib\\site-packages", "**/src", "**\\src"]
-paths.other = [".", "*/tox_uv", "*\\tox_uv"]
+paths.source = [
+  "src",
+  ".tox/*/.venv/lib/*/site-packages",
+  ".tox\\*\\.venv\\Lib\\site-packages",
+  "**/src",
+  "**\\src",
+]
+paths.other = [
+  ".",
+  "*/tox_uv",
+  "*\\tox_uv",
+]
+report.omit = [
+  "src/tox_uv/_venv_query.py",
+]
 report.fail_under = 100
 run.parallel = true
-run.plugins = ["covdefaults"]
+run.plugins = [
+  "covdefaults",
+]
 
 [tool.mypy]
 python_version = "3.11"
 show_error_codes = true
 strict = true
-overrides = [{ module = ["virtualenv.*", "uv.*"], ignore_missing_imports = true }]
+overrides = [
+  { module = [
+    "virtualenv.*",
+    "uv.*",
+  ], ignore_missing_imports = true },
+]
```

### Comparing `tox_uv-1.7.0/PKG-INFO` & `tox_uv-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: tox-uv
-Version: 1.7.0
+Version: 1.8.0
 Summary: Integration of uv with tox.
+Project-URL: Changelog, https://github.com/tox-dev/tox-uv/releases
 Project-URL: Documentation, https://github.com/tox-dev/tox-uv#tox-uv
 Project-URL: Homepage, https://github.com/tox-dev/tox-uv
 Project-URL: Source, https://github.com/tox-dev/tox-uv
 Project-URL: Tracker, https://github.com/tox-dev/tox-uv/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -21,23 +22,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System
 Requires-Python: >=3.8
-Requires-Dist: packaging>=23.2
-Requires-Dist: tox<5,>=4.14
-Requires-Dist: uv<1,>=0.1.15
+Requires-Dist: importlib-resources>=6.4; python_version < '3.9'
+Requires-Dist: packaging>=24
+Requires-Dist: tox<5,>=4.15
+Requires-Dist: uv<1,>=0.1.39
 Provides-Extra: test
 Requires-Dist: covdefaults>=2.3; extra == 'test'
 Requires-Dist: devpi-process>=1; extra == 'test'
-Requires-Dist: pytest-cov>=4.1; extra == 'test'
-Requires-Dist: pytest-mock>=3.12; extra == 'test'
-Requires-Dist: pytest>=8.0.2; extra == 'test'
+Requires-Dist: pytest-cov>=5; extra == 'test'
+Requires-Dist: pytest-mock>=3.14; extra == 'test'
+Requires-Dist: pytest>=8.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 # tox-uv
 
 [![PyPI version](https://badge.fury.io/py/tox-uv.svg)](https://badge.fury.io/py/tox-uv)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/tox-uv.svg)](https://pypi.python.org/pypi/tox-uv/)
 [![check](https://github.com/tox-dev/tox-uv/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/tox-uv/actions/workflows/check.yml)
```

