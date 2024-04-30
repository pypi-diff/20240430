# Comparing `tmp/dotlink-2.0b1.tar.gz` & `tmp/dotlink-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotlink-2.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dotlink-2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dotlink-2.0b1.tar` & `dotlink-2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      180 2023-11-13 20:25:37.851662 dotlink-2.0b1/.flake8
--rw-r--r--   0        0        0     1241 2022-08-24 06:05:13.105426 dotlink-2.0b1/.gitignore
--rw-r--r--   0        0        0       50 2023-11-09 03:22:13.341003 dotlink-2.0b1/.mailmap
--rw-r--r--   0        0        0     2807 2023-11-13 20:49:18.129003 dotlink-2.0b1/CHANGELOG.md
--rw-r--r--   0        0        0     3216 2022-08-24 06:05:30.030426 dotlink-2.0b1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      765 2022-08-24 06:05:30.033964 dotlink-2.0b1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1076 2023-11-09 03:25:11.466041 dotlink-2.0b1/LICENSE
--rw-r--r--   0        0        0     1522 2023-11-13 20:48:55.524419 dotlink-2.0b1/README.md
--rw-r--r--   0        0        0      201 2023-11-13 20:25:37.851963 dotlink-2.0b1/dotlink/__init__.py
--rw-r--r--   0        0        0      129 2023-11-13 20:25:37.852221 dotlink-2.0b1/dotlink/__main__.py
--rw-r--r--   0        0        0      156 2023-11-13 20:49:18.135218 dotlink-2.0b1/dotlink/__version__.py
--rw-r--r--   0        0        0     2561 2023-11-13 20:25:37.852425 dotlink-2.0b1/dotlink/actions.py
--rw-r--r--   0        0        0     1958 2023-11-13 20:38:34.674732 dotlink-2.0b1/dotlink/cli.py
--rw-r--r--   0        0        0     3696 2023-11-13 20:25:37.852832 dotlink-2.0b1/dotlink/core.py
--rw-r--r--   0        0        0        0 2023-11-13 20:25:37.852860 dotlink-2.0b1/dotlink/tests/__init__.py
--rw-r--r--   0        0        0     7409 2023-11-13 20:25:37.853243 dotlink-2.0b1/dotlink/tests/actions.py
--rw-r--r--   0        0        0     3486 2023-11-13 20:25:37.853324 dotlink-2.0b1/dotlink/tests/core.py
--rw-r--r--   0        0        0      128 2023-11-13 20:25:37.853499 dotlink-2.0b1/dotlink/tests/smoke.py
--rw-r--r--   0        0        0     1449 2023-11-13 20:25:37.853693 dotlink-2.0b1/dotlink/tests/types.py
--rw-r--r--   0        0        0      398 2023-11-13 20:25:37.853820 dotlink-2.0b1/dotlink/tests/util.py
--rw-r--r--   0        0        0     2038 2023-11-13 20:25:37.854082 dotlink-2.0b1/dotlink/types.py
--rw-r--r--   0        0        0      346 2023-11-13 20:25:37.854204 dotlink-2.0b1/dotlink/util.py
--rw-r--r--   0        0        0       14 2023-11-13 20:25:37.854340 dotlink-2.0b1/example/dotlink
--rw-r--r--   0        0        0      551 2023-11-13 20:25:37.854590 dotlink-2.0b1/makefile
--rw-r--r--   0        0        0     1167 2023-11-13 20:25:37.854825 dotlink-2.0b1/pyproject.toml
--rw-r--r--   0        0        0     2535 1970-01-01 00:00:00.000000 dotlink-2.0b1/PKG-INFO
+-rw-r--r--   0        0        0      189 2024-04-30 03:07:39.470713 dotlink-2.1/.flake8
+-rw-r--r--   0        0        0     1241 2024-04-30 03:07:39.471461 dotlink-2.1/.gitignore
+-rw-r--r--   0        0        0       50 2024-04-30 03:07:39.471567 dotlink-2.1/.mailmap
+-rw-r--r--   0        0        0     3521 2024-04-30 06:24:47.466958 dotlink-2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3216 2024-04-30 03:07:39.471819 dotlink-2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      765 2024-04-30 03:07:39.471924 dotlink-2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1076 2024-04-30 03:07:39.472035 dotlink-2.1/LICENSE
+-rw-r--r--   0        0        0     1522 2024-04-30 03:07:39.472147 dotlink-2.1/README.md
+-rw-r--r--   0        0        0      201 2024-04-30 03:07:39.472322 dotlink-2.1/dotlink/__init__.py
+-rw-r--r--   0        0        0      129 2024-04-30 03:07:39.472429 dotlink-2.1/dotlink/__main__.py
+-rw-r--r--   0        0        0      154 2024-04-30 06:24:47.476050 dotlink-2.1/dotlink/__version__.py
+-rw-r--r--   0        0        0     3471 2024-04-30 03:07:39.472659 dotlink-2.1/dotlink/actions.py
+-rw-r--r--   0        0        0     1980 2024-04-30 03:07:39.472772 dotlink-2.1/dotlink/cli.py
+-rw-r--r--   0        0        0     5146 2024-04-30 04:50:41.441003 dotlink-2.1/dotlink/core.py
+-rw-r--r--   0        0        0        0 2024-04-30 03:07:39.472998 dotlink-2.1/dotlink/tests/__init__.py
+-rw-r--r--   0        0        0     9893 2024-04-30 03:07:39.473296 dotlink-2.1/dotlink/tests/actions.py
+-rw-r--r--   0        0        0     4704 2024-04-30 04:50:41.441264 dotlink-2.1/dotlink/tests/core.py
+-rw-r--r--   0        0        0      124 2024-04-30 03:07:39.473527 dotlink-2.1/dotlink/tests/smoke.py
+-rw-r--r--   0        0        0     1934 2024-04-30 04:50:41.441541 dotlink-2.1/dotlink/tests/types.py
+-rw-r--r--   0        0        0      694 2024-04-30 04:50:41.442250 dotlink-2.1/dotlink/tests/util.py
+-rw-r--r--   0        0        0     2466 2024-04-30 04:50:41.442491 dotlink-2.1/dotlink/types.py
+-rw-r--r--   0        0        0      516 2024-04-30 04:50:41.442734 dotlink-2.1/dotlink/util.py
+-rw-r--r--   0        0        0       14 2024-04-30 03:07:39.474129 dotlink-2.1/example/dotlink
+-rw-r--r--   0        0        0      551 2024-04-30 03:07:39.474240 dotlink-2.1/makefile
+-rw-r--r--   0        0        0     1180 2024-04-30 04:50:41.442842 dotlink-2.1/pyproject.toml
+-rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 dotlink-2.1/PKG-INFO
```

### Comparing `dotlink-2.0b1/.gitignore` & `dotlink-2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dotlink-2.0b1/CHANGELOG.md` & `dotlink-2.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,48 @@
 dotlink
 =======
 
 [![Generated by attribution][attribution-badge]][attribution-url]
 
 
+v2.1
+----
+
+Feature release
+
+- Add support for including another repo via URL (#19)
+- Allow selecting repo branch/tag/revision with url `#fragment` (#19)
+- Cache cloned repos by URL, repo name, and target ref (#19)
+
+```text
+$ git shortlog -s v2.0...v2.1
+     2	Amethyst Reese
+     8	dependabot[bot]
+```
+
+
+v2.0
+----
+
+Major release
+
+- Total rewrite, using Python 3.8 syntax features
+- Changed config format to `dest [= src]`
+- Changed config filename to `.dotlink` or `dotlink`
+- Use click for CLI arg parsing
+- Use modern Python features and metadata
+- Support for `--plan` or `--dry-run`
+- Dropped `--rsync` option in favor of new ssh+tar stream
+
+```text
+$ git shortlog -s v2.0b1...v2.0
+     3	Amethyst Reese
+```
+
+
 v2.0b1
 ------
 
 Beta release
 
 - Total rewrite
 - Changed config format to `dest [= src]`
```

### Comparing `dotlink-2.0b1/CODE_OF_CONDUCT.md` & `dotlink-2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dotlink-2.0b1/CONTRIBUTING.md` & `dotlink-2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dotlink-2.0b1/LICENSE` & `dotlink-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dotlink-2.0b1/README.md` & `dotlink-2.1/README.md`

 * *Files identical despite different names*

### Comparing `dotlink-2.0b1/dotlink/actions.py` & `dotlink-2.1/dotlink/actions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # Copyright Amethyst Reese
 # Licensed under the MIT license
 
 from __future__ import annotations
 
+import logging
 import shutil
-
+import tarfile
 from dataclasses import dataclass
+from io import BytesIO
 from pathlib import Path
 from typing import Any, Generator
 
 from .types import Target
+from .util import run
+
+LOG = logging.getLogger(__name__)
 
 
 @dataclass
 class Plan:
     actions: list[Action]
 
     def __str__(self) -> str:
@@ -91,7 +96,37 @@
 class Deploy(Action):
     def __init__(self, src: Path, target: Target) -> None:
         self.src = src
         self.target = target
 
     def print(self) -> str:
         return f"{self.src} -> {self.target}"
+
+
+class SSHTarball(Deploy):
+    def prepare(self) -> None:
+        if not self.src.is_dir():
+            raise RuntimeError(f"{self.src} is not a directory")
+
+        if not self.target.remote:
+            raise ValueError(f"target {self.target} is not remote")
+
+    def execute(self) -> None:
+        stream = BytesIO()
+        with tarfile.open(mode="w|gz", fileobj=stream) as tf:
+            tf.add(self.src, arcname=".")
+
+        stream.seek(0)
+        self.data = stream.read()
+        LOG.debug("tarball compressed size %d bytes", len(self.data))
+
+        run(
+            "ssh",
+            self.target.address,
+            "tar",
+            "-xz",
+            "-f-",
+            "-C",
+            self.target.path.as_posix(),
+            input=self.data,
+            encoding=None,
+        )
```

### Comparing `dotlink-2.0b1/dotlink/cli.py` & `dotlink-2.1/dotlink/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,7 +69,8 @@
     )
 
     if dry_run:
         print(plan)
     else:
         for action in plan.execute():
             print(action)
+        print("done")
```

### Comparing `dotlink-2.0b1/dotlink/tests/core.py` & `dotlink-2.1/dotlink/tests/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from textwrap import dedent
 from unittest import TestCase
 from unittest.mock import Mock, patch
 
 from dotlink import core
-from dotlink.types import Config, InvalidPlan
+from dotlink.types import Config, InvalidPlan, Source
 
 
 class CoreTest(TestCase):
     def setUp(self) -> None:
         td = TemporaryDirectory()
         self.addCleanup(td.cleanup)
         self.dir = Path(td.name).resolve()
@@ -105,10 +105,38 @@
                 core.generate_config(self.dir / "invalid")
 
         with self.subTest("include missing"):
             (self.dir / "invalid" / "dotlink").write_text("@bar\n")
             with self.assertRaisesRegex(InvalidPlan, "bar not found"):
                 core.generate_config(self.dir / "invalid")
 
+    @patch("dotlink.core.user_cache_dir")
+    def test_repo_cache_dir(self, ucd_mock: Mock) -> None:
+        with TemporaryDirectory() as td:
+            tdp = Path(td) / "dotlink"
+            ucd_mock.return_value = tdp.as_posix()
+
+            for source_str, expected in (
+                ("", None),
+                ("foo/bar", None),
+                ("https://github.com/amyreese/dotfiles.git", tdp / "d45a-dotfiles"),
+                (
+                    "https://github.com/amyreese/dotfiles.git#feature-branch",
+                    tdp / "d45a-dotfiles-feature-branch",
+                ),
+                ("https://github.com/actions/checkout", tdp / "0f8a-checkout"),
+                (
+                    "https://github.com/actions/checkout#main",
+                    tdp / "0f8a-checkout-main",
+                ),
+            ):
+                with self.subTest(source_str):
+                    source = Source.parse(source_str)
+                    if expected is None:
+                        with self.assertRaises(AssertionError):
+                            core.repo_cache_dir(source)
+                    else:
+                        self.assertEqual(expected, core.repo_cache_dir(source))
+
     @patch("dotlink.core.run")
     def test_prepare_source(self, run_mock: Mock) -> None:
         pass
```

### Comparing `dotlink-2.0b1/dotlink/tests/types.py` & `dotlink-2.1/dotlink/tests/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,17 +8,34 @@
 
 
 class TypesTest(TestCase):
     def test_source(self) -> None:
         for value, expected in (
             ("", Source(path=Path(""))),
             (".", Source(path=Path("."))),
-            ("/foo/bar", Source(path=Path("/foo/bar"))),
-            ("git://github.com/a/b", Source(url="git://github.com/a/b")),
-            ("https://github.com/a/b.git", Source(url="https://github.com/a/b.git")),
+            (
+                "/foo/bar",
+                Source(path=Path("/foo/bar"), stem="bar"),
+            ),
+            (
+                "git://github.com/a/b",
+                Source(url="git://github.com/a/b", stem="b"),
+            ),
+            (
+                "https://github.com/a/b.git",
+                Source(url="https://github.com/a/b.git", stem="b"),
+            ),
+            (
+                "git://github.com/a/b#main",
+                Source(url="git://github.com/a/b", stem="b", ref="main"),
+            ),
+            (
+                "https://github.com/a/b.git#abc123",
+                Source(url="https://github.com/a/b.git", stem="b", ref="abc123"),
+            ),
         ):
             with self.subTest(value):
                 assert Source.parse(value) == expected
 
     def test_target(self) -> None:
         for value, expected in (
             ("", Target(path=Path(""))),
```

### Comparing `dotlink-2.0b1/dotlink/types.py` & `dotlink-2.1/dotlink/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     re.X,
 )
 
 Pair: TypeAlias = Tuple[Path, Path]
 URL: TypeAlias = str
 
 
-class InvalidPlan(ValueError):
-    ...
+class InvalidPlan(ValueError): ...
 
 
 class Method(Enum):
     symlink = auto()
     copy = auto()
 
 
@@ -43,34 +42,47 @@
     includes: Sequence[Config] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
 class Source:
     path: Path | None = None
     url: URL | None = None
+    ref: str = ""
+    stem: str = ""
 
     @classmethod
-    def parse(cls, value: str) -> Self:
+    def parse(cls, value: str, root: Path | None = None) -> Self:
         url = urlparse(value)
         if url.scheme and url.netloc:
-            return cls(url=URL(value))
+            return cls(
+                url=URL(url._replace(fragment="").geturl()),
+                ref=url.fragment,
+                stem=Path(url.path).stem,
+            )
+        path = Path(value)
+        if root:
+            return cls(path=root / path, stem=path.stem)
         else:
-            return cls(path=Path(value))
+            return cls(path=path, stem=path.stem)
 
 
 @dataclass(frozen=True)
 class Target:
     path: Path
     host: str | None = None
     user: str | None = None
 
     @property
     def remote(self) -> bool:
         return self.host is not None
 
+    @property
+    def address(self) -> str:
+        return f"{self.user}@{self.host}" if self.user else (self.host or "")
+
     def __str__(self) -> str:
         if self.host:
             if self.user:
                 return f"{self.user}@{self.host}:{self.path}"
             else:
                 return f"{self.host}:{self.path}"
         else:
```

### Comparing `dotlink-2.0b1/makefile` & `dotlink-2.1/makefile`

 * *Files identical despite different names*

### Comparing `dotlink-2.0b1/pyproject.toml` & `dotlink-2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     "Operating System :: OS Independent",
     "Topic :: Utilities",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 dependencies = [
     "click >= 8",
-    "rich >= 12",
+    "platformdirs >= 4",
     "typing_extensions >= 4",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "attribution==1.6.2",
-    "black==23.11.0",
-    "flake8==6.1.0",
+    "attribution==1.7.1",
+    "black==24.4.2",
+    "flake8==7.0.0",
     "flit==3.9.0",
-    "mypy==1.6.1",
-    "pytest==7.4.3",
-    "usort==1.0.7",
-    "ufmt==2.3.0",
+    "mypy==1.10.0",
+    "pytest==8.2.0",
+    "usort==1.0.8.post1",
+    "ufmt==2.5.1",
 ]
 
 [project.scripts]
 dotlink = "dotlink.cli:main"
 
 [project.urls]
 home-page = "https://github.com/amyreese/dotlink"
```

### Comparing `dotlink-2.0b1/PKG-INFO` & `dotlink-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: dotlink
-Version: 2.0b1
+Version: 2.1
 Summary: Automate deployment of dotfiles to local paths or remote hosts
 Author-email: Amethyst Reese <amy@noswap.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Dist: click >= 8
-Requires-Dist: rich >= 12
+Requires-Dist: platformdirs >= 4
 Requires-Dist: typing_extensions >= 4
-Requires-Dist: attribution==1.6.2 ; extra == "dev"
-Requires-Dist: black==23.11.0 ; extra == "dev"
-Requires-Dist: flake8==6.1.0 ; extra == "dev"
+Requires-Dist: attribution==1.7.1 ; extra == "dev"
+Requires-Dist: black==24.4.2 ; extra == "dev"
+Requires-Dist: flake8==7.0.0 ; extra == "dev"
 Requires-Dist: flit==3.9.0 ; extra == "dev"
-Requires-Dist: mypy==1.6.1 ; extra == "dev"
-Requires-Dist: pytest==7.4.3 ; extra == "dev"
-Requires-Dist: usort==1.0.7 ; extra == "dev"
-Requires-Dist: ufmt==2.3.0 ; extra == "dev"
+Requires-Dist: mypy==1.10.0 ; extra == "dev"
+Requires-Dist: pytest==8.2.0 ; extra == "dev"
+Requires-Dist: usort==1.0.8.post1 ; extra == "dev"
+Requires-Dist: ufmt==2.5.1 ; extra == "dev"
 Project-URL: Github, https://github.com/amyreese/dotlink
 Project-URL: home-page, https://github.com/amyreese/dotlink
 Provides-Extra: dev
 
 dotlink
 =======
```

