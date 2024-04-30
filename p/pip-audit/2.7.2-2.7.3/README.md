# Comparing `tmp/pip_audit-2.7.2.tar.gz` & `tmp/pip_audit-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_audit-2.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pip_audit-2.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_audit-2.7.2.tar` & `pip_audit-2.7.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10174 2024-02-29 16:06:23.784848 pip_audit-2.7.2/LICENSE
--rw-r--r--   0        0        0    24406 2024-02-29 16:06:23.784848 pip_audit-2.7.2/README.md
--rw-r--r--   0        0        0       53 2024-02-29 16:06:23.784848 pip_audit-2.7.2/pip_audit/__init__.py
--rw-r--r--   0        0        0      144 2024-02-29 16:06:23.784848 pip_audit-2.7.2/pip_audit/__main__.py
--rw-r--r--   0        0        0     3158 2024-02-29 16:06:23.784848 pip_audit-2.7.2/pip_audit/_audit.py
--rw-r--r--   0        0        0     6223 2024-02-29 16:06:23.784848 pip_audit-2.7.2/pip_audit/_cache.py
--rw-r--r--   0        0        0    21239 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_cli.py
--rw-r--r--   0        0        0      579 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_dependency_source/__init__.py
--rw-r--r--   0        0        0     1738 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_dependency_source/interface.py
--rw-r--r--   0        0        0     6919 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_dependency_source/pip.py
--rw-r--r--   0        0        0     5698 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_dependency_source/pyproject.py
--rw-r--r--   0        0        0    15353 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_dependency_source/requirement.py
--rw-r--r--   0        0        0     3683 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_fix.py
--rw-r--r--   0        0        0      380 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_format/__init__.py
--rw-r--r--   0        0        0     5685 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_format/columns.py
--rw-r--r--   0        0        0     2803 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_format/cyclonedx.py
--rw-r--r--   0        0        0     1119 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_format/interface.py
--rw-r--r--   0        0        0     3458 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_format/json.py
--rw-r--r--   0        0        0     5155 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_format/markdown.py
--rw-r--r--   0        0        0      536 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_service/__init__.py
--rw-r--r--   0        0        0     5265 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_service/interface.py
--rw-r--r--   0        0        0     5898 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_service/osv.py
--rw-r--r--   0        0        0     5047 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_service/pypi.py
--rw-r--r--   0        0        0     8716 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_state.py
--rw-r--r--   0        0        0     2345 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_subprocess.py
--rw-r--r--   0        0        0      662 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_util.py
--rw-r--r--   0        0        0     8406 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pip_audit/_virtual_env.py
--rw-r--r--   0        0        0     2926 2024-02-29 16:06:23.788848 pip_audit-2.7.2/pyproject.toml
--rw-r--r--   0        0        0    26495 1970-01-01 00:00:00.000000 pip_audit-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-04-30 19:27:30.362503 pip_audit-2.7.3/LICENSE
+-rw-r--r--   0        0        0    24477 2024-04-30 19:27:30.362503 pip_audit-2.7.3/README.md
+-rw-r--r--   0        0        0       53 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/__main__.py
+-rw-r--r--   0        0        0     3163 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_audit.py
+-rw-r--r--   0        0        0     6223 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_cache.py
+-rw-r--r--   0        0        0    21239 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_cli.py
+-rw-r--r--   0        0        0      579 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_dependency_source/__init__.py
+-rw-r--r--   0        0        0     1739 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_dependency_source/interface.py
+-rw-r--r--   0        0        0     6919 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_dependency_source/pip.py
+-rw-r--r--   0        0        0     5691 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_dependency_source/pyproject.py
+-rw-r--r--   0        0        0    15179 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_dependency_source/requirement.py
+-rw-r--r--   0        0        0     3684 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_fix.py
+-rw-r--r--   0        0        0      380 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_format/__init__.py
+-rw-r--r--   0        0        0     5685 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_format/columns.py
+-rw-r--r--   0        0        0     2804 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_format/cyclonedx.py
+-rw-r--r--   0        0        0     1120 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_format/interface.py
+-rw-r--r--   0        0        0     3459 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_format/json.py
+-rw-r--r--   0        0        0     5155 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_format/markdown.py
+-rw-r--r--   0        0        0      536 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_service/__init__.py
+-rw-r--r--   0        0        0     5265 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_service/interface.py
+-rw-r--r--   0        0        0     5899 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_service/osv.py
+-rw-r--r--   0        0        0     5048 2024-04-30 19:27:30.362503 pip_audit-2.7.3/pip_audit/_service/pypi.py
+-rw-r--r--   0        0        0     8717 2024-04-30 19:27:30.366503 pip_audit-2.7.3/pip_audit/_state.py
+-rw-r--r--   0        0        0     2270 2024-04-30 19:27:30.366503 pip_audit-2.7.3/pip_audit/_subprocess.py
+-rw-r--r--   0        0        0      662 2024-04-30 19:27:30.366503 pip_audit-2.7.3/pip_audit/_util.py
+-rw-r--r--   0        0        0     8406 2024-04-30 19:27:30.366503 pip_audit-2.7.3/pip_audit/_virtual_env.py
+-rw-r--r--   0        0        0     3139 2024-04-30 19:27:30.366503 pip_audit-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0    26610 1970-01-01 00:00:00.000000 pip_audit-2.7.3/PKG-INFO
```

### Comparing `pip_audit-2.7.2/LICENSE` & `pip_audit-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/README.md` & `pip_audit-2.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 `pip-audit` has [`pre-commit`](https://pre-commit.com/) support.
 
 For example, using `pip-audit` via `pre-commit` to audit a requirements file:
 
 ```yaml
   - repo: https://github.com/pypa/pip-audit
-    rev: v2.7.2
+    rev: v2.7.3
     hooks:
       -   id: pip-audit
           args: ["-r", "requirements.txt"]
 
 ci:
   # Leave pip-audit to only run locally and not in CI
   # pre-commit.ci does not allow network calls
@@ -464,17 +464,18 @@
 * [`pip`'s `keyring` authentication](https://pip.pypa.io/en/stable/topics/authentication/#keyring-support)
   **is** supported, but in a limited fashion: `pip-audit` uses the `subprocess` keyring provider,
   since audits happen in isolated virtual environments. The `subprocess` provider in turn
   is subject to additional restrictions (such as a required username);
   [`pip`'s documentation](https://pip.pypa.io/en/stable/topics/authentication/#using-keyring-as-a-command-line-application)
   explains these in depth.
 
-In practice, this means that authenticated third-party indices that **don't** take
-a username, like Google Artifact Registry, are currently **unsupported** by `pip-audit`.
-See [#742](https://github.com/pypa/pip-audit/issues/742) for more details.
+In addition to the above, some third-party indices have required, hard-coded usernames.
+For example, for Google Artifact registry, the hard-coded username is `oauth2accesstoken`.
+See [#742](https://github.com/pypa/pip-audit/issues/742) and
+[pip#11971](https://github.com/pypa/pip/issues/11971) for additional context.
 
 ## Tips and Tricks
 
 ### Running against a `pipenv` project
 
 `pipenv` uses both a `Pipfile` and `Pipfile.lock` file to track and freeze dependencies
 instead of a `requirements.txt` file. `pip-audit` cannot process the `Pipfile[.lock]`
```

### Comparing `pip_audit-2.7.2/pip_audit/_audit.py` & `pip_audit-2.7.3/pip_audit/_audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Core auditing APIs.
 """
+
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from typing import Iterator
 
 from pip_audit._dependency_source import DependencySource
@@ -58,15 +59,15 @@
         `PYSEC`-identified results are given priority over other results.
         """
         specs = source.collect()
 
         if self._options.dry_run:
             # Drain the iterator in dry-run mode.
             logger.info(f"Dry run: would have audited {len(list(specs))} packages")
-            return {}
+            yield from ()
         else:
             for dep, vulns in self._service.query_all(specs):
                 unique_vulns: list[VulnerabilityResult] = []
                 seen_aliases: set[str] = set()
 
                 # First pass, add all PYSEC vulnerabilities and track their
                 # alias sets.
```

### Comparing `pip_audit-2.7.2/pip_audit/_cache.py` & `pip_audit-2.7.3/pip_audit/_cache.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_cli.py` & `pip_audit-2.7.3/pip_audit/_cli.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_dependency_source/__init__.py` & `pip_audit-2.7.3/pip_audit/_dependency_source/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_dependency_source/interface.py` & `pip_audit-2.7.3/pip_audit/_dependency_source/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Interfaces for interacting with "dependency sources", i.e. sources
 of fully resolved Python dependency trees.
 """
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Iterator
 
 from pip_audit._fix import ResolvedFixVersion
 from pip_audit._service import Dependency
```

### Comparing `pip_audit-2.7.2/pip_audit/_dependency_source/pip.py` & `pip_audit-2.7.3/pip_audit/_dependency_source/pip.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_dependency_source/pyproject.py` & `pip_audit-2.7.3/pip_audit/_dependency_source/pyproject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Collect dependencies from `pyproject.toml` files.
 """
+
 from __future__ import annotations
 
 import logging
 import os
 from pathlib import Path
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from typing import Iterator
@@ -137,16 +138,16 @@
                     req.specifier = SpecifierSet(f"=={fix_version.version}")
                     deps[i] = str(req)
                 assert req.marker is None or req.marker.evaluate()
 
             # Now dump the new edited TOML to the temporary file.
             toml.dump(pyproject_data, tmp)
 
-            # And replace the original `pyproject.toml` file.
-            os.replace(tmp.name, self.filename)
+        # And replace the original `pyproject.toml` file.
+        os.replace(tmp.name, self.filename)
 
 
 class PyProjectSourceError(DependencySourceError):
     """A `pyproject.toml` specific `DependencySourceError`."""
 
     pass
```

### Comparing `pip_audit-2.7.2/pip_audit/_dependency_source/requirement.py` & `pip_audit-2.7.3/pip_audit/_dependency_source/requirement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Collect dependencies from one or more `requirements.txt`-formatted files.
 """
 
 from __future__ import annotations
 
 import logging
-import os
 import re
 import shutil
 from contextlib import ExitStack
 from pathlib import Path
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from typing import IO, Iterator
 
@@ -189,15 +188,15 @@
         """
         Fixes a dependency version for this `RequirementSource`.
         """
         with ExitStack() as stack:
             # Make temporary copies of the existing requirements files. If anything goes wrong, we
             # want to copy them back into place and undo any partial application of the fix.
             tmp_files: list[IO[str]] = [
-                stack.enter_context(NamedTemporaryFile(mode="w")) for _ in self._filenames
+                stack.enter_context(NamedTemporaryFile(mode="r+")) for _ in self._filenames
             ]
             for filename, tmp_file in zip(self._filenames, tmp_files):
                 with filename.open("r") as f:
                     shutil.copyfileobj(f, tmp_file)
 
             try:
                 # Now fix the files inplace
@@ -216,15 +215,15 @@
 
     def _fix_file(self, filename: Path, fix_version: ResolvedFixVersion) -> None:
         # Reparse the requirements file. We want to rewrite each line to the new requirements file
         # and only modify the lines that we're fixing.
         #
         # This time we're using the `RequirementsFile.parse` API instead of `Requirements.from_file`
         # since we want to access each line sequentially in order to rewrite the file.
-        reqs = list(RequirementsFile.parse(filename=str(filename)))
+        reqs = list(RequirementsFile.parse(filename=filename.as_posix()))
 
         # Check ahead of time for anything invalid in the requirements file since we don't want to
         # encounter this while writing out the file. Check for duplicate requirements and lines that
         # failed to parse.
         req_names: set[str] = set()
         for req in reqs:
             if (
@@ -274,18 +273,17 @@
                     file=f,
                 )
                 print(f"{fix_version.dep.canonical_name}=={fix_version.version}", file=f)
 
     def _recover_files(self, tmp_files: list[IO[str]]) -> None:
         for filename, tmp_file in zip(self._filenames, tmp_files):
             try:
-                os.replace(tmp_file.name, filename)
-                # We need to tinker with the internals to prevent the file wrapper from attempting
-                # to remove the temporary file like in the regular case.
-                tmp_file._closer.delete = False  # type: ignore[attr-defined]
+                tmp_file.seek(0)
+                with filename.open("w") as f:
+                    shutil.copyfileobj(tmp_file, f)
             except Exception as e:
                 # Not much we can do at this point since we're already handling an exception. Just
                 # log the error and try to recover the rest of the files.
                 logger.warning(f"encountered an exception during file recovery: {e}")
                 continue
 
     def _collect_preresolved_deps(
```

### Comparing `pip_audit-2.7.2/pip_audit/_fix.py` & `pip_audit-2.7.3/pip_audit/_fix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functionality for resolving fixed versions of dependencies.
 """
+
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from typing import Any, Iterator, cast
 
 from packaging.version import Version
```

### Comparing `pip_audit-2.7.2/pip_audit/_format/columns.py` & `pip_audit-2.7.3/pip_audit/_format/columns.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_format/cyclonedx.py` & `pip_audit-2.7.3/pip_audit/_format/cyclonedx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functionality for formatting vulnerability results using the CycloneDX SBOM format.
 """
+
 from __future__ import annotations
 
 import enum
 import logging
 from typing import cast
 
 from cyclonedx import output
```

### Comparing `pip_audit-2.7.2/pip_audit/_format/interface.py` & `pip_audit-2.7.3/pip_audit/_format/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Interfaces for formatting vulnerability results into a string representation.
 """
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
 import pip_audit._fix as fix
 import pip_audit._service as service
```

### Comparing `pip_audit-2.7.2/pip_audit/_format/json.py` & `pip_audit-2.7.3/pip_audit/_format/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functionality for formatting vulnerability results as an array of JSON objects.
 """
+
 from __future__ import annotations
 
 import json
 from typing import Any, cast
 
 import pip_audit._fix as fix
 import pip_audit._service as service
```

### Comparing `pip_audit-2.7.2/pip_audit/_format/markdown.py` & `pip_audit-2.7.3/pip_audit/_format/markdown.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_service/__init__.py` & `pip_audit-2.7.3/pip_audit/_service/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_service/interface.py` & `pip_audit-2.7.3/pip_audit/_service/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_service/osv.py` & `pip_audit-2.7.3/pip_audit/_service/osv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functionality for using the [OSV](https://osv.dev/) API as a `VulnerabilityService`.
 """
+
 from __future__ import annotations
 
 import json
 import logging
 from pathlib import Path
 from typing import Any, cast
```

### Comparing `pip_audit-2.7.2/pip_audit/_service/pypi.py` & `pip_audit-2.7.3/pip_audit/_service/pypi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Functionality for using the [PyPI](https://warehouse.pypa.io/api-reference/json.html)
 API as a `VulnerabilityService`.
 """
+
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 from typing import cast
 
 import requests
```

### Comparing `pip_audit-2.7.2/pip_audit/_state.py` & `pip_audit-2.7.3/pip_audit/_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Interfaces for for propagating feedback from the API to provide responsive progress indicators as
 well as a progress spinner implementation for use with CLI applications.
 """
+
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from logging.handlers import MemoryHandler
 from typing import Any, Sequence
```

### Comparing `pip_audit-2.7.2/pip_audit/_subprocess.py` & `pip_audit-2.7.3/pip_audit/_subprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,17 +48,16 @@
     stderr = b""
 
     # NOTE: We use `poll()` to control this loop instead of the `read()` call
     # to prevent deadlocks. Similarly, `read(size)` will return an empty bytes
     # once `stdout` hits EOF, so we don't have to worry about that blocking.
     while not terminated:
         terminated = process.poll() is not None
-        # NOTE(ww): Buffer size chosen arbitrarily here and below.
-        stdout += process.stdout.read(4096)  # type: ignore
-        stderr += process.stderr.read(4096)  # type: ignore
+        stdout += process.stdout.read()  # type: ignore
+        stderr += process.stderr.read()  # type: ignore
         state.update_state(
             f"Running {pretty_args}",
             stdout.decode(errors="replace") if log_stdout else None,
         )
 
     if process.returncode != 0:
         raise CalledProcessError(
```

### Comparing `pip_audit-2.7.2/pip_audit/_util.py` & `pip_audit-2.7.3/pip_audit/_util.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pip_audit/_virtual_env.py` & `pip_audit-2.7.3/pip_audit/_virtual_env.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.7.2/pyproject.toml` & `pip_audit-2.7.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Security",
 ]
 dependencies = [
     "CacheControl[filecache] >= 0.13.0",
-    "cyclonedx-python-lib >= 5,< 7",
+    "cyclonedx-python-lib >= 5,< 8",
     "html5lib>=1.1",
     "packaging>=23.0.0",                 # https://github.com/pypa/pip-audit/issues/464
     "pip-api>=0.0.28",
     "pip-requirements-parser>=32.0.0",
     "requests >= 2.31.0",
     "rich>=12.4",
     "toml>=0.10",
@@ -45,15 +45,18 @@
     "pretend",
     "pytest",
     "pytest-cov",
 ]
 lint = [
     # NOTE(ww): ruff is under active development, so we pin conservatively here
     # and let Dependabot periodically perform this update.
-    "ruff < 0.2.3",
+    "ruff < 0.4.3",
+    # HACK(ww): interrogate needs setuptools to provide `pkg_resources` on Python 3.12+;
+    # remove this when https://github.com/econchick/interrogate/issues/164 is resolved.
+    "setuptools",
     "interrogate",
     "mypy",
     "types-html5lib",
     "types-requests",
     "types-toml",
 ]
 doc = ["pdoc"]
@@ -92,11 +95,13 @@
 warn_unused_ignores = true
 
 [tool.bump]
 input = "pip_audit/__init__.py"
 reset = true
 
 [tool.ruff]
+line-length = 100
+
+[tool.ruff.lint]
 # Never enforce `E501` (line length violations).
 ignore = ["E501"]
 select = ["E", "F", "I", "W", "UP"]
-line-length = 100
```

### Comparing `pip_audit-2.7.2/PKG-INFO` & `pip_audit-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_audit
-Version: 2.7.2
+Version: 2.7.3
 Summary: A tool for scanning Python environments for known vulnerabilities
 Author-email: Alex Cameron <alex.cameron@trailofbits.com>, Dustin Ingram <di@python.org>, William Woodruff <william@trailofbits.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,27 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Requires-Dist: CacheControl[filecache] >= 0.13.0
-Requires-Dist: cyclonedx-python-lib >= 5,< 7
+Requires-Dist: cyclonedx-python-lib >= 5,< 8
 Requires-Dist: html5lib>=1.1
 Requires-Dist: packaging>=23.0.0
 Requires-Dist: pip-api>=0.0.28
 Requires-Dist: pip-requirements-parser>=32.0.0
 Requires-Dist: requests >= 2.31.0
 Requires-Dist: rich>=12.4
 Requires-Dist: toml>=0.10
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: bump>=1.3.2 ; extra == "dev"
 Requires-Dist: pip-audit[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
-Requires-Dist: ruff < 0.2.3 ; extra == "lint"
+Requires-Dist: ruff < 0.4.3 ; extra == "lint"
+Requires-Dist: setuptools ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: types-html5lib ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: types-toml ; extra == "lint"
 Requires-Dist: coverage[toml] ~= 7.0, != 7.3.3 ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
@@ -151,15 +152,15 @@
 
 `pip-audit` has [`pre-commit`](https://pre-commit.com/) support.
 
 For example, using `pip-audit` via `pre-commit` to audit a requirements file:
 
 ```yaml
   - repo: https://github.com/pypa/pip-audit
-    rev: v2.7.2
+    rev: v2.7.3
     hooks:
       -   id: pip-audit
           args: ["-r", "requirements.txt"]
 
 ci:
   # Leave pip-audit to only run locally and not in CI
   # pre-commit.ci does not allow network calls
@@ -513,17 +514,18 @@
 * [`pip`'s `keyring` authentication](https://pip.pypa.io/en/stable/topics/authentication/#keyring-support)
   **is** supported, but in a limited fashion: `pip-audit` uses the `subprocess` keyring provider,
   since audits happen in isolated virtual environments. The `subprocess` provider in turn
   is subject to additional restrictions (such as a required username);
   [`pip`'s documentation](https://pip.pypa.io/en/stable/topics/authentication/#using-keyring-as-a-command-line-application)
   explains these in depth.
 
-In practice, this means that authenticated third-party indices that **don't** take
-a username, like Google Artifact Registry, are currently **unsupported** by `pip-audit`.
-See [#742](https://github.com/pypa/pip-audit/issues/742) for more details.
+In addition to the above, some third-party indices have required, hard-coded usernames.
+For example, for Google Artifact registry, the hard-coded username is `oauth2accesstoken`.
+See [#742](https://github.com/pypa/pip-audit/issues/742) and
+[pip#11971](https://github.com/pypa/pip/issues/11971) for additional context.
 
 ## Tips and Tricks
 
 ### Running against a `pipenv` project
 
 `pipenv` uses both a `Pipfile` and `Pipfile.lock` file to track and freeze dependencies
 instead of a `requirements.txt` file. `pip-audit` cannot process the `Pipfile[.lock]`
```

