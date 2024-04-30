# Comparing `tmp/deepl_cli-0.6.0.tar.gz` & `tmp/deepl_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepl_cli-0.6.0.tar", max compression
+gzip compressed data, was "deepl_cli-0.7.0.tar", max compression
```

## Comparing `deepl_cli-0.6.0.tar` & `deepl_cli-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-12-23 08:58:37.268481 deepl_cli-0.6.0/LICENSE
--rw-r--r--   0        0        0     2638 2023-12-23 08:58:37.268481 deepl_cli-0.6.0/README.md
--rw-r--r--   0        0        0      107 2023-12-23 08:58:37.268481 deepl_cli-0.6.0/deepl/__init__.py
--rw-r--r--   0        0        0     6739 2023-12-23 08:58:37.268481 deepl_cli-0.6.0/deepl/deepl.py
--rw-r--r--   0        0        0     3876 2023-12-23 08:58:37.268481 deepl_cli-0.6.0/deepl/main.py
--rw-r--r--   0        0        0        0 2023-12-23 08:58:37.268481 deepl_cli-0.6.0/deepl/py.typed
--rw-r--r--   0        0        0     1922 2023-12-23 08:58:37.272481 deepl_cli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 deepl_cli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-30 03:21:40.990771 deepl_cli-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2638 2024-04-30 03:21:40.990771 deepl_cli-0.7.0/README.md
+-rw-r--r--   0        0        0      107 2024-04-30 03:21:40.990771 deepl_cli-0.7.0/deepl/__init__.py
+-rw-r--r--   0        0        0     6983 2024-04-30 03:21:40.990771 deepl_cli-0.7.0/deepl/deepl.py
+-rw-r--r--   0        0        0     3876 2024-04-30 03:21:40.990771 deepl_cli-0.7.0/deepl/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 03:21:40.990771 deepl_cli-0.7.0/deepl/py.typed
+-rw-r--r--   0        0        0     1829 2024-04-30 03:21:40.990771 deepl_cli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 deepl_cli-0.7.0/PKG-INFO
```

### Comparing `deepl_cli-0.6.0/LICENSE` & `deepl_cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepl_cli-0.6.0/README.md` & `deepl_cli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `deepl_cli-0.6.0/deepl/deepl.py` & `deepl_cli-0.7.0/deepl/deepl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+from functools import partial
 from typing import TYPE_CHECKING, Any, ClassVar
 from urllib.parse import quote
 
 from install_playwright import install
 from playwright._impl._errors import Error as PlaywrightError
 from playwright.async_api import async_playwright
 
@@ -92,16 +93,17 @@
     async def __translate(self, script: str) -> str:
         """Throw a request."""
         async with async_playwright() as p:
             # Dry run
             try:
                 browser = await self.__get_browser(p)
             except PlaywrightError as e:
-                if "Executable doesn't exist at" in e.message:
+                if "playwright install" in e.message:
                     print("Installing browser executable. This may take some time.")  # noqa: T201
+                    await asyncio.get_event_loop().run_in_executor(None, partial(install, p.chromium, with_deps=True))
                     await asyncio.get_event_loop().run_in_executor(None, install, p.chromium)
                     browser = await self.__get_browser(p)
                 else:
                     raise
 
             page = await browser.new_page()
             page.set_default_timeout(self.timeout)
@@ -127,18 +129,18 @@
                 msg = f"Maybe Time limit exceeded. ({self.timeout} ms)"
                 raise DeepLCLIPageLoadError(msg) from e
 
             if self.use_dom_submit:
                 # banner prevents clicking on language buttons, close the banner first
                 await page.click("button[data-testid=cookie-banner-lax-close-button]")
                 # select input / output language
-                await page.click("button[data-testid=translator-source-lang-btn]")
-                await page.click(f"button[data-testid=translator-lang-option-{self.fr_lang}]")
-                await page.click("button[data-testid=translator-target-lang-btn]")
-                await page.click(f"button[data-testid=translator-lang-option-{self.to_lang}]")
+                await page.locator("button[data-testid=translator-source-lang-btn]").dispatch_event("click")
+                await page.locator(f"button[data-testid=translator-lang-option-{self.fr_lang}]").dispatch_event("click")
+                await page.locator("button[data-testid=translator-target-lang-btn]").dispatch_event("click")
+                await page.locator(f"button[data-testid=translator-lang-option-{self.to_lang}]").dispatch_event("click")
                 # fill in the form of translating script
                 await page.fill("div[aria-labelledby=translation-source-heading]", script)
 
             # Wait for translation to complete
             try:
                 await page.wait_for_function(
                     """
```

### Comparing `deepl_cli-0.6.0/deepl/main.py` & `deepl_cli-0.7.0/deepl/main.py`

 * *Files identical despite different names*

### Comparing `deepl_cli-0.6.0/pyproject.toml` & `deepl_cli-0.7.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# poetry self add poetry-bumpversion
-
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = [
   "poetry-core",
 ]
 
 [tool]
@@ -19,66 +17,61 @@
 description = "DeepL Translator CLI without API Key"
 keywords = ["deepl", "translate", "cli"]
 name = "deepl_cli"
 packages = [{include = "deepl"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/deepl-cli"
-version = "0.6.0"
+version = "0.7.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-install-playwright = "^0.0.0"
-playwright = "^1.31.1"
+install-playwright = "^0.1.0"
+playwright = "^1.43.0"
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.991,<1.8"
+mypy = ">=0.991,<1.11"
 pre-commit = ">=2.20,<4.0"
 taskipy = "^1.10.3"
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-pytest-asyncio = "^0.21.0"
+pytest = ">=7.2.2,<9.0.0"
+pytest-cov = ">=4,<6"
+pytest-asyncio = ">=0.21,<0.24"
 
 [tool.poetry.scripts]
 deepl = "deepl.main:main"
 
 [tool.black]
 line-length = 120
 target-version = ['py39']
 
-[tool.ruff]
-select = ["ALL"]
-ignore = ["D", "ANN101"]
-line-length = 120
-
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 18
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "main.py" = [
   "T201", # `print` found
 ]
 "tests/test_*.py" = [
   "INP001",  # File tests/test_*.py is part of an implicit namespace package. Add an __init__.py.
   "S101", # Use of assert detected
 ]
 "examples/*.py" = [
   "INP001",  # File tests/test_*.py is part of an implicit namespace package. Add an __init__.py.
   "T201", # `print` found
 ]
 
-[tool.isort]
-profile = "black"
-
 [tool.mypy]
 pretty = true
 python_version = "3.9"
 show_error_codes = true
 strict = true
 
-[tool.poetry_bumpversion.file."deepl/__init__.py"]
+[tool.lint.ruff]
+select = ["ALL"]
+ignore = ["D", "ANN101"]
+line-length = 120
 
 [tool.taskipy.tasks]
 test = "pytest --cov=deepl --cov-report=term"
 "test:ci" = "task test --cov-report=xml:cov.xml"
 lint = "pre-commit run -a"
 profile = "python -m cProfile"
```

### Comparing `deepl_cli-0.6.0/PKG-INFO` & `deepl_cli-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepl_cli
-Version: 0.6.0
+Version: 0.7.0
 Summary: DeepL Translator CLI without API Key
 Home-page: https://github.com/eggplants/deepl-cli
 License: MIT
 Keywords: deepl,translate,cli
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.8,<4
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: install-playwright (>=0.0.0,<0.0.1)
-Requires-Dist: playwright (>=1.31.1,<2.0.0)
+Requires-Dist: install-playwright (>=0.1.0,<0.2.0)
+Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Project-URL: Repository, https://github.com/eggplants/deepl-cli
 Description-Content-Type: text/markdown
 
 # deepl-cli
 
 [![Release Package](
   <https://github.com/eggplants/deepl-cli/workflows/Release%20Package/badge.svg>
```

