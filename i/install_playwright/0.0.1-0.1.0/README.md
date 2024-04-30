# Comparing `tmp/install_playwright-0.0.1.tar.gz` & `tmp/install_playwright-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install_playwright-0.0.1.tar", max compression
+gzip compressed data, was "install_playwright-0.1.0.tar", max compression
```

## Comparing `install_playwright-0.0.1.tar` & `install_playwright-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-12-18 16:17:55.553229 install_playwright-0.0.1/LICENSE
--rw-r--r--   0        0        0     1548 2023-12-18 16:17:55.553229 install_playwright-0.0.1/README.md
--rw-r--r--   0        0        0     1013 2023-12-18 16:17:55.553229 install_playwright-0.0.1/install_playwright/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 16:17:55.553229 install_playwright-0.0.1/install_playwright/py.typed
--rw-r--r--   0        0        0     1805 2023-12-18 16:17:55.553229 install_playwright-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 install_playwright-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-30 02:40:19.372224 install_playwright-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1548 2024-04-30 02:40:19.372224 install_playwright-0.1.0/README.md
+-rw-r--r--   0        0        0     1118 2024-04-30 02:40:19.372224 install_playwright-0.1.0/install_playwright/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 02:40:19.372224 install_playwright-0.1.0/install_playwright/py.typed
+-rw-r--r--   0        0        0     1818 2024-04-30 02:40:19.376224 install_playwright-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 install_playwright-0.1.0/PKG-INFO
```

### Comparing `install_playwright-0.0.1/LICENSE` & `install_playwright-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `install_playwright-0.0.1/README.md` & `install_playwright-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `install_playwright-0.0.1/install_playwright/__init__.py` & `install_playwright-0.1.0/install_playwright/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 import subprocess
+from typing import TYPE_CHECKING
 
 from playwright._impl._driver import compute_driver_executable, get_driver_env
-from playwright.async_api import BrowserType as AsyncBrowserType
-from playwright.sync_api import BrowserType as SyncBrowserType
 
-__version__ = "0.0.1"
+if TYPE_CHECKING:
+    from playwright.async_api import BrowserType as AsyncBrowserType
+    from playwright.sync_api import BrowserType as SyncBrowserType
+
+__version__ = "0.1.0"
 __all__ = ["install"]
 
 
 def install(
     browser_type: SyncBrowserType | AsyncBrowserType,
     *,
     with_deps: bool = False,
@@ -20,17 +23,16 @@
     Args:
         browser_type (SyncBrowserType | AsyncBrowserType): `BrowserType` object. Example: `p.chrome`
         with_deps (bool, optional): install with dependencies. Defaults to `False`.
 
     Returns:
         bool: succeeded or failed
     """
-    driver_executable = str(compute_driver_executable())
-
-    args = [driver_executable, "install", browser_type.name]
+    driver_executable, driver_cli = compute_driver_executable()
+    args = [driver_executable, driver_cli, "install", browser_type.name]
 
     if with_deps:
         args.append("--with-deps")
 
-    proc = subprocess.run(args, env=get_driver_env(), capture_output=True, text=True)
+    proc = subprocess.run(args, env=get_driver_env(), capture_output=True, text=True, check=False)  # noqa: S603
 
     return proc.returncode == 0
```

### Comparing `install_playwright-0.0.1/pyproject.toml` & `install_playwright-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 description = "Execute `playwright install` from Python"
 keywords = ["playwright", "install", "browser"]
 name = "install_playwright"
 packages = [{include = "install_playwright"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/install-playwright-python"
-version = "0.0.1"
+version = "0.1.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 playwright = "^1.9"
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.991,<1.8"
+mypy = ">=0.991,<1.10"
 pre-commit = ">=2.20,<4.0"
 taskipy = "^1.10.3"
-pytest = "^7.4.3"
-pytest-cov = "^4.1.0"
+pytest = ">=7.4.3,<9.0.0"
+pytest-cov = ">=4.1,<6.0"
 
 [tool.black]
 line-length = 120
 target-version = ['py39']
 
 [tool.ruff]
 select = ["ALL"]
```

### Comparing `install_playwright-0.0.1/PKG-INFO` & `install_playwright-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install_playwright
-Version: 0.0.1
+Version: 0.1.0
 Summary: Execute `playwright install` from Python
 Home-page: https://github.com/eggplants/install-playwright-python
 License: MIT
 Keywords: playwright,install,browser
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.8,<4
```

