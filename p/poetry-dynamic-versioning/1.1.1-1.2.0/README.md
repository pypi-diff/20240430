# Comparing `tmp/poetry_dynamic_versioning-1.1.1.tar.gz` & `tmp/poetry_dynamic_versioning-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_dynamic_versioning-1.1.1.tar", max compression
+gzip compressed data, was "poetry_dynamic_versioning-1.2.0.tar", max compression
```

## Comparing `poetry_dynamic_versioning-1.1.1.tar` & `poetry_dynamic_versioning-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    14121 2023-10-27 05:33:51.250306 poetry_dynamic_versioning-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2021-12-24 01:49:41.427292 poetry_dynamic_versioning-1.1.1/LICENSE
--rw-r--r--   0        0        0    17202 2023-10-27 05:25:02.336274 poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/__init__.py
--rw-r--r--   0        0        0      409 2023-06-12 16:10:01.487305 poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/__main__.py
--rw-r--r--   0        0        0      119 2023-02-21 03:15:22.704013 poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/backend.py
--rw-r--r--   0        0        0     3783 2023-08-21 03:34:20.335230 poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/cli.py
--rw-r--r--   0        0        0     1776 2023-08-21 02:56:59.654177 poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/patch.py
--rw-r--r--   0        0        0     5731 2023-06-29 15:51:30.898970 poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/plugin.py
--rw-r--r--   0        0        0     1796 2023-10-27 05:33:55.762171 poetry_dynamic_versioning-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    16176 2023-10-01 13:59:45.145490 poetry_dynamic_versioning-1.1.1/README.md
--rw-r--r--   0        0        0        0 2021-12-24 01:49:41.429292 poetry_dynamic_versioning-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0       22 2021-12-24 01:49:41.430292 poetry_dynamic_versioning-1.1.1/tests/dependency-classic/dependency_classic/__init__.py
--rw-r--r--   0        0        0      117 2021-12-24 01:49:41.430292 poetry_dynamic_versioning-1.1.1/tests/dependency-classic/setup.py
--rw-r--r--   0        0        0       22 2023-10-01 13:37:46.946853 poetry_dynamic_versioning-1.1.1/tests/dependency-dynamic/dependency_dynamic/__init__.py
--rw-r--r--   0        0        0      276 2023-10-27 04:51:06.780634 poetry_dynamic_versioning-1.1.1/tests/dependency-dynamic/pyproject.toml
--rw-r--r--   0        0        0       22 2021-12-24 01:49:41.431293 poetry_dynamic_versioning-1.1.1/tests/dependency-static/dependency_static/__init__.py
--rw-r--r--   0        0        0      227 2022-09-05 08:46:04.436946 poetry_dynamic_versioning-1.1.1/tests/dependency-static/pyproject.toml
--rw-r--r--   0        0        0        8 2023-08-17 17:06:47.459015 poetry_dynamic_versioning-1.1.1/tests/project/docs/version.txt
--rw-r--r--   0        0        0       79 2023-08-17 17:06:47.460167 poetry_dynamic_versioning-1.1.1/tests/project/project/__init__.py
--rw-r--r--   0        0        0      659 2023-08-17 17:06:47.460167 poetry_dynamic_versioning-1.1.1/tests/project/pyproject.toml
--rw-r--r--   0        0        0     8818 2023-08-17 17:06:10.662827 poetry_dynamic_versioning-1.1.1/tests/test_integration.py
--rw-r--r--   0        0        0     7824 2023-10-01 13:59:19.680868 poetry_dynamic_versioning-1.1.1/tests/test_unit.py
--rw-r--r--   0        0        0    17691 1970-01-01 00:00:00.000000 poetry_dynamic_versioning-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    14526 2023-12-02 14:47:35.948286 poetry_dynamic_versioning-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2021-12-24 01:49:41.427292 poetry_dynamic_versioning-1.2.0/LICENSE
+-rw-r--r--   0        0        0    20717 2023-12-02 14:26:02.121075 poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/__init__.py
+-rw-r--r--   0        0        0      409 2023-06-12 16:10:01.487305 poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/__main__.py
+-rw-r--r--   0        0        0      119 2023-02-21 03:15:22.704013 poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/backend.py
+-rw-r--r--   0        0        0     3663 2023-12-02 07:59:50.665171 poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/cli.py
+-rw-r--r--   0        0        0     1776 2023-08-21 02:56:59.654177 poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/patch.py
+-rw-r--r--   0        0        0     5731 2023-12-02 14:11:46.317585 poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/plugin.py
+-rw-r--r--   0        0        0     1835 2023-12-02 14:47:31.305929 poetry_dynamic_versioning-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16581 2023-12-02 08:03:55.730745 poetry_dynamic_versioning-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2021-12-24 01:49:41.429292 poetry_dynamic_versioning-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       22 2021-12-24 01:49:41.430292 poetry_dynamic_versioning-1.2.0/tests/dependency-classic/dependency_classic/__init__.py
+-rw-r--r--   0        0        0      117 2021-12-24 01:49:41.430292 poetry_dynamic_versioning-1.2.0/tests/dependency-classic/setup.py
+-rw-r--r--   0        0        0       22 2023-12-02 14:22:56.183385 poetry_dynamic_versioning-1.2.0/tests/dependency-dynamic/dependency_dynamic/__init__.py
+-rw-r--r--   0        0        0      276 2023-12-02 14:23:07.016565 poetry_dynamic_versioning-1.2.0/tests/dependency-dynamic/pyproject.toml
+-rw-r--r--   0        0        0       22 2021-12-24 01:49:41.431293 poetry_dynamic_versioning-1.2.0/tests/dependency-static/dependency_static/__init__.py
+-rw-r--r--   0        0        0      227 2022-09-05 08:46:04.436946 poetry_dynamic_versioning-1.2.0/tests/dependency-static/pyproject.toml
+-rw-r--r--   0        0        0        8 2023-12-02 07:32:08.932020 poetry_dynamic_versioning-1.2.0/tests/project/docs/version.txt
+-rw-r--r--   0        0        0       79 2023-12-02 07:32:08.932020 poetry_dynamic_versioning-1.2.0/tests/project/project/__init__.py
+-rw-r--r--   0        0        0      659 2023-12-02 07:32:08.947725 poetry_dynamic_versioning-1.2.0/tests/project/pyproject.toml
+-rw-r--r--   0        0        0     9133 2023-12-02 07:59:50.665171 poetry_dynamic_versioning-1.2.0/tests/test_integration.py
+-rw-r--r--   0        0        0     7850 2023-12-02 13:49:24.976830 poetry_dynamic_versioning-1.2.0/tests/test_unit.py
+-rw-r--r--   0        0        0    18096 1970-01-01 00:00:00.000000 poetry_dynamic_versioning-1.2.0/PKG-INFO
```

### Comparing `poetry_dynamic_versioning-1.1.1/CHANGELOG.md` & `poetry_dynamic_versioning-1.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## v1.2.0 (2023-12-02)
+
+* Added:
+  * `initial-content-jinja` option in `tool.poetry-dynamic-versioning.files` section.
+* Fixed:
+  * Line ending style was not preserved in some cases because of the default behavior of `pathlib.Path.read_text`.
+    To avoid this, `pathlib.Path.read_bytes` is used instead now.
+    ([Contributed by nardi](https://github.com/mtkennerly/poetry-dynamic-versioning/pull/157))
+
 ## v1.1.1 (2023-10-27)
 
 * Fixed:
   * Custom substitutions in pyproject.toml weren't cleaned up correctly.
     This was because the plugin would record the "original" content of the file
     after the `version` and `enable` fields had already been changed.
     Now, substitutions are reverted first before reverting `version` and `enable`.
```

### Comparing `poetry_dynamic_versioning-1.1.1/LICENSE` & `poetry_dynamic_versioning-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/__init__.py` & `poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,122 @@
 import subprocess
 import sys
 import textwrap
 from importlib import import_module
 from pathlib import Path
 from typing import Mapping, MutableMapping, Optional, Sequence, Tuple, Union
 
+import jinja2
 import tomlkit
+from dunamai import (
+    bump_version,
+    check_version,
+    Concern,
+    Pattern,
+    serialize_pep440,
+    serialize_pvp,
+    serialize_semver,
+    Style,
+    Vcs,
+    Version,
+)
 
 _BYPASS_ENV = "POETRY_DYNAMIC_VERSIONING_BYPASS"
 _OVERRIDE_ENV = "POETRY_DYNAMIC_VERSIONING_OVERRIDE"
 
+if sys.version_info >= (3, 8):
+    from typing import TypedDict
+
+    _SubstitutionPattern = TypedDict(
+        "_SubstitutionPattern",
+        {
+            "value": str,
+            "mode": Optional[str],
+        },
+    )
+
+    _SubstitutionFolder = TypedDict(
+        "_SubstitutionFolder",
+        {
+            "path": str,
+            "files": Optional[Sequence[str]],
+            "patterns": Optional[Sequence[Union[str, _SubstitutionPattern]]],
+        },
+    )
+
+    _Substitution = TypedDict(
+        "_Substitution",
+        {
+            "files": Sequence[str],
+            "patterns": Sequence[Union[str, _SubstitutionPattern]],
+            "folders": Sequence[_SubstitutionFolder],
+        },
+    )
+
+    _File = TypedDict(
+        "_File",
+        {
+            "persistent-substitution": Optional[bool],
+            "initial-content": Optional[str],
+            "initial-content-jinja": Optional[str],
+        },
+    )
+
+    _JinjaImport = TypedDict(
+        "_JinjaImport",
+        {
+            "module": str,
+            "item": Optional[str],
+        },
+    )
+
+    _Config = TypedDict(
+        "_Config",
+        {
+            "enable": bool,
+            "vcs": str,
+            "dirty": bool,
+            "pattern": Optional[str],
+            "latest-tag": bool,
+            "substitution": _Substitution,
+            "files": Mapping[str, _File],
+            "style": Optional[str],
+            "metadata": Optional[bool],
+            "format": Optional[str],
+            "format-jinja": Optional[str],
+            "format-jinja-imports": Sequence[_JinjaImport],
+            "bump": bool,
+            "tagged-metadata": bool,
+            "full-commit": bool,
+            "tag-branch": Optional[str],
+            "tag-dir": str,
+            "strict": bool,
+            "fix-shallow-repository": bool,
+        },
+    )
+else:
+
+    class _Config(Mapping):
+        pass
+
 
 class _ProjectState:
     def __init__(
         self,
         path: Path,
         original_version: str,
         version: str,
-        substitutions: MutableMapping[Path, str] = None,
+        substitutions: Optional[MutableMapping[Path, str]] = None,
     ) -> None:
         self.path = path
         self.original_version = original_version
         self.version = version
-        self.substitutions = {} if substitutions is None else substitutions
+        self.substitutions = (
+            {} if substitutions is None else substitutions
+        )  # type: MutableMapping[Path, str]
 
 
 class _State:
     def __init__(self) -> None:
         self.patched_core_poetry_create = False
         self.cli_mode = False
         self.projects = {}  # type: MutableMapping[str, _ProjectState]
@@ -63,24 +153,24 @@
 class _FolderConfig:
     def __init__(self, path: Path, files: Sequence[str], patterns: Sequence[_SubPattern]):
         self.path = path
         self.files = files
         self.patterns = patterns
 
     @staticmethod
-    def from_config(config: Mapping, root: Path) -> Sequence["_FolderConfig"]:
+    def from_config(config: _Config, root: Path) -> Sequence["_FolderConfig"]:
         files = config["substitution"]["files"]
         patterns = _SubPattern.from_config(config["substitution"]["patterns"])
 
         main = _FolderConfig(root, files, patterns)
         extra = [
             _FolderConfig(
                 root / x["path"],
-                x.get("files", files),
-                _SubPattern.from_config(x["patterns"]) if "patterns" in x else patterns,
+                x["files"] if x["files"] is not None else files,
+                _SubPattern.from_config(x["patterns"]) if x["patterns"] is not None else patterns,
             )
             for x in config["substitution"]["folders"]
         ]
 
         return [main, *extra]
 
 
@@ -128,29 +218,29 @@
         if isinstance(value, dict) and key in base and isinstance(base[key], dict):
             result[key] = _deep_merge_dicts(base[key], value)
         else:
             result[key] = value
     return result
 
 
-def _find_higher_file(*names: str, start: Path = None) -> Optional[Path]:
+def _find_higher_file(*names: str, start: Optional[Path] = None) -> Optional[Path]:
     # Note: We need to make sure we get a pathlib object. Many tox poetry
     # helpers will pass us a string and not a pathlib object. See issue #40.
     if start is None:
         start = Path.cwd()
     elif not isinstance(start, Path):
         start = Path(start)
     for level in [start, *start.parents]:
         for name in names:
             if (level / name).is_file():
                 return level / name
     return None
 
 
-def _get_pyproject_path(start: Path = None) -> Optional[Path]:
+def _get_pyproject_path(start: Optional[Path] = None) -> Optional[Path]:
     return _find_higher_file("pyproject.toml", start=start)
 
 
 def _get_pyproject_path_from_poetry(pyproject) -> Path:
     # poetry-core 1.6.0+:
     recommended = getattr(pyproject, "path", None)
     # poetry-core <1.6.0:
@@ -160,33 +250,57 @@
         return recommended
     elif legacy:
         return legacy
     else:
         raise RuntimeError("Unable to determine pyproject.toml path from Poetry instance")
 
 
-def _get_config(local: Mapping) -> Mapping:
-    return _deep_merge_dicts(_default_config(), local)["tool"]["poetry-dynamic-versioning"]
+def _get_config(local: Mapping) -> _Config:
+    def initialize(data, key):
+        if isinstance(data, dict) and key not in data:
+            data[key] = None
+
+    if isinstance(local, tomlkit.TOMLDocument):
+        local = local.unwrap()
+
+    merged = _deep_merge_dicts(_default_config(), local)["tool"][
+        "poetry-dynamic-versioning"
+    ]  # type: _Config
+
+    # Add default values so we don't have to worry about missing keys
+    for x in merged["files"].values():
+        initialize(x, "initial-content")
+        initialize(x, "initial-content-jinja")
+        initialize(x, "persistent-substitution")
+    for x in merged["format-jinja-imports"]:
+        initialize(x, "item")
+    for x in merged["substitution"]["folders"]:
+        initialize(x, "files")
+        initialize(x, "patterns")
+    for x in merged["substitution"]["patterns"]:
+        initialize(x, "mode")
 
+    return merged
 
-def _get_config_from_path(start: Path = None) -> Mapping:
+
+def _get_config_from_path(start: Optional[Path] = None) -> Mapping:
     pyproject_path = _get_pyproject_path(start)
     if pyproject_path is None:
         return _default_config()["tool"]["poetry-dynamic-versioning"]
-    pyproject = tomlkit.parse(pyproject_path.read_text(encoding="utf-8"))
+    pyproject = tomlkit.parse(pyproject_path.read_bytes().decode("utf-8"))
     result = _get_config(pyproject)
     return result
 
 
 def _validate_config(config: Optional[Mapping] = None) -> Sequence[str]:
     if config is None:
         pyproject_path = _get_pyproject_path()
         if pyproject_path is None:
             raise RuntimeError("Unable to find pyproject.toml")
-        config = tomlkit.parse(pyproject_path.read_text(encoding="utf-8"))
+        config = tomlkit.parse(pyproject_path.read_bytes().decode("utf-8"))
 
     return _validate_config_section(
         config.get("tool", {}).get("poetry-dynamic-versioning", {}),
         _default_config()["tool"]["poetry-dynamic-versioning"],
         ["tool", "poetry-dynamic-versioning"],
     )
 
@@ -217,14 +331,53 @@
 
 def _format_timestamp(value: Optional[dt.datetime]) -> Optional[str]:
     if value is None:
         return None
     return value.strftime("%Y%m%d%H%M%S")
 
 
+def _render_jinja(
+    version: Version, template: str, config: _Config, extra: Optional[Mapping] = None
+) -> str:
+    if extra is None:
+        extra = {}
+
+    if config["bump"] and version.distance > 0:
+        version = version.bump()
+    default_context = {
+        "base": version.base,
+        "version": version,
+        "stage": version.stage,
+        "revision": version.revision,
+        "distance": version.distance,
+        "commit": version.commit,
+        "dirty": version.dirty,
+        "branch": version.branch,
+        "branch_escaped": _escape_branch(version.branch),
+        "timestamp": _format_timestamp(version.timestamp),
+        "env": os.environ,
+        "bump_version": bump_version,
+        "tagged_metadata": version.tagged_metadata,
+        "serialize_pep440": serialize_pep440,
+        "serialize_pvp": serialize_pvp,
+        "serialize_semver": serialize_semver,
+        **extra,
+    }
+    custom_context = {}  # type: dict
+    for entry in config["format-jinja-imports"]:
+        if "module" in entry:
+            module = import_module(entry["module"])
+            if entry["item"] is not None:
+                custom_context[entry["item"]] = getattr(module, entry["item"])
+            else:
+                custom_context[entry["module"]] = module
+    serialized = jinja2.Template(template).render(**default_context, **custom_context)
+    return serialized
+
+
 def _run_cmd(command: str, codes: Sequence[int] = (0,)) -> Tuple[int, str]:
     result = subprocess.run(
         shlex.split(command),
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
     )
     output = result.stdout.decode().strip()
@@ -254,52 +407,39 @@
     bypass = env.get(_BYPASS_ENV)
     if bypass is not None:
         return bypass
 
     return None
 
 
-def _get_version_from_dunamai(vcs, pattern, config, *, strict: Optional[bool] = None):
-    from dunamai import Version
-
+def _get_version_from_dunamai(
+    vcs: Vcs, pattern: Union[str, Pattern], config: _Config, *, strict: Optional[bool] = None
+) -> Version:
     return Version.from_vcs(
         vcs,
         pattern,
         config["latest-tag"],
         config["tag-dir"],
         config["tag-branch"],
         config["full-commit"],
         config["strict"] if strict is None else strict,
     )
 
 
-def _get_version(config: Mapping, name: Optional[str] = None) -> str:
+def _get_version(config: _Config, name: Optional[str] = None) -> Tuple[str, Version]:
     override = _get_override_version(name)
     if override is not None:
-        return override
-
-    import jinja2
-    from dunamai import (
-        bump_version,
-        check_version,
-        Concern,
-        Pattern,
-        serialize_pep440,
-        serialize_pvp,
-        serialize_semver,
-        Style,
-        Vcs,
-    )
+        return (override, Version.parse(override))
 
     vcs = Vcs(config["vcs"])
-    style = config["style"]
-    if style is not None:
-        style = Style(style)
+    style = Style(config["style"]) if config["style"] is not None else None
 
-    pattern = config["pattern"] if config["pattern"] is not None else Pattern.Default
+    pattern = (
+        config["pattern"] if config["pattern"] is not None else Pattern.Default
+    )  # type: Union[str, Pattern]
 
     if config["fix-shallow-repository"]:
         # We start without strict so we can inspect the concerns.
         version = _get_version_from_dunamai(vcs, pattern, config, strict=False)
         retry = config["strict"]
 
         if Concern.ShallowRepository in version.concerns and version.vcs == Vcs.Git:
@@ -311,58 +451,28 @@
     else:
         version = _get_version_from_dunamai(vcs, pattern, config)
 
     for concern in version.concerns:
         print("Warning: {}".format(concern.message()), file=sys.stderr)
 
     if config["format-jinja"]:
-        if config["bump"] and version.distance > 0:
-            version = version.bump()
-        default_context = {
-            "base": version.base,
-            "version": version,
-            "stage": version.stage,
-            "revision": version.revision,
-            "distance": version.distance,
-            "commit": version.commit,
-            "dirty": version.dirty,
-            "branch": version.branch,
-            "branch_escaped": _escape_branch(version.branch),
-            "timestamp": _format_timestamp(version.timestamp),
-            "env": os.environ,
-            "bump_version": bump_version,
-            "tagged_metadata": version.tagged_metadata,
-            "serialize_pep440": serialize_pep440,
-            "serialize_pvp": serialize_pvp,
-            "serialize_semver": serialize_semver,
-        }
-        custom_context = {}  # type: dict
-        for entry in config["format-jinja-imports"]:
-            if "module" in entry:
-                module = import_module(entry["module"])
-                if "item" in entry:
-                    custom_context[entry["item"]] = getattr(module, entry["item"])
-                else:
-                    custom_context[entry["module"]] = module
-        serialized = jinja2.Template(config["format-jinja"]).render(
-            **default_context, **custom_context
-        )
+        serialized = _render_jinja(version, config["format-jinja"], config)
         if style is not None:
             check_version(serialized, style)
     else:
         serialized = version.serialize(
             metadata=config["metadata"],
             dirty=config["dirty"],
             format=config["format"],
             style=style,
             bump=config["bump"],
             tagged_metadata=config["tagged-metadata"],
         )
 
-    return serialized
+    return (serialized, version)
 
 
 def _substitute_version(name: str, version: str, folders: Sequence[_FolderConfig]) -> None:
     if _state.projects[name].substitutions:
         # Already ran; don't need to repeat.
         return
 
@@ -373,15 +483,15 @@
             for match in folder.path.glob(str(file_glob)):
                 resolved = match.resolve()
                 if resolved in files:
                     continue
                 files[resolved] = folder
 
     for file, config in files.items():
-        original_content = file.read_text(encoding="utf-8")
+        original_content = file.read_bytes().decode("utf-8")
         new_content = _substitute_version_in_text(version, original_content, config.patterns)
         if original_content != new_content:
             _state.projects[name].substitutions[file] = original_content
             file.write_bytes(new_content.encode("utf-8"))
 
 
 def _substitute_version_in_text(version: str, content: str, patterns: Sequence[_SubPattern]) -> str:
@@ -411,17 +521,17 @@
             pattern.value, r"\g<1>{}\g<2>".format(insert), new_content, flags=re.MULTILINE
         )
 
     return new_content
 
 
 def _apply_version(
-    version: str, config: Mapping, pyproject_path: Path, retain: bool = False
+    version: str, instance: Version, config: _Config, pyproject_path: Path, retain: bool = False
 ) -> None:
-    pyproject = tomlkit.parse(pyproject_path.read_text(encoding="utf-8"))
+    pyproject = tomlkit.parse(pyproject_path.read_bytes().decode("utf-8"))
 
     pyproject["tool"]["poetry"]["version"] = version  # type: ignore
 
     # Disable the plugin in case we're building a source distribution,
     # which won't have access to the VCS info at install time.
     # We revert this later when we deactivate.
     if not retain and not _state.cli_mode:
@@ -429,15 +539,28 @@
 
     pyproject_path.write_bytes(tomlkit.dumps(pyproject).encode("utf-8"))
 
     name = pyproject["tool"]["poetry"]["name"]  # type: ignore
 
     for file_name, file_info in config["files"].items():
         full_file = pyproject_path.parent.joinpath(file_name)
-        if "initial-content" in file_info:
+
+        if file_info["initial-content-jinja"] is not None:
+            if not full_file.parent.exists():
+                full_file.parent.mkdir()
+            initial = textwrap.dedent(
+                _render_jinja(
+                    instance,
+                    file_info["initial-content-jinja"],
+                    config,
+                    {"formatted_version": version},
+                )
+            )
+            full_file.write_bytes(initial.encode("utf-8"))
+        elif file_info["initial-content"] is not None:
             if not full_file.parent.exists():
                 full_file.parent.mkdir()
             initial = textwrap.dedent(file_info["initial-content"])
             full_file.write_bytes(initial.encode("utf-8"))
 
     _substitute_version(
         name,  # type: ignore
@@ -462,15 +585,15 @@
 
     if pyproject_path is None:
         pyproject_path = _get_pyproject_path()
         if pyproject_path is None:
             raise RuntimeError("Unable to find pyproject.toml")
 
     if pyproject is None:
-        pyproject = tomlkit.parse(pyproject_path.read_text(encoding="utf-8"))
+        pyproject = tomlkit.parse(pyproject_path.read_bytes().decode("utf-8"))
 
     if name is None or original is None:
         name = pyproject["tool"]["poetry"]["name"]
         original = pyproject["tool"]["poetry"]["version"]
         if name in _state.projects:
             return name
 
@@ -478,47 +601,47 @@
     if not config["enable"] and not force:
         return name if name in _state.projects else None
 
     initial_dir = Path.cwd()
     target_dir = pyproject_path.parent
     os.chdir(str(target_dir))
     try:
-        version = _get_version(config, name)
+        version, instance = _get_version(config, name)
     finally:
         os.chdir(str(initial_dir))
 
     # Condition will always be true, but it makes Mypy happy.
     if name is not None and original is not None:
         _state.projects[name] = _ProjectState(pyproject_path, original, version)
         if io:
-            _apply_version(version, config, pyproject_path, retain)
+            _apply_version(version, instance, config, pyproject_path, retain)
 
     return name
 
 
 def _revert_version(retain: bool = False) -> None:
     for project, state in _state.projects.items():
-        pyproject = tomlkit.parse(state.path.read_text(encoding="utf-8"))
+        pyproject = tomlkit.parse(state.path.read_bytes().decode("utf-8"))
 
         if state.substitutions:
             config = _get_config(pyproject)
 
             persistent = []
             for file, file_info in config["files"].items():
-                if file_info.get("persistent-substitution"):
+                if file_info["persistent-substitution"]:
                     persistent.append(state.path.parent.joinpath(file))
 
             for file, content in state.substitutions.items():
                 if file in persistent:
                     continue
 
                 file.write_bytes(content.encode("utf-8"))
 
             # Reread pyproject.toml in case the substitutions affected it.
-            pyproject = tomlkit.parse(state.path.read_text(encoding="utf-8"))
+            pyproject = tomlkit.parse(state.path.read_bytes().decode("utf-8"))
 
         pyproject["tool"]["poetry"]["version"] = state.original_version  # type: ignore
 
         if not retain and not _state.cli_mode:
             pyproject["tool"]["poetry-dynamic-versioning"]["enable"] = True  # type: ignore
 
         state.path.write_bytes(tomlkit.dumps(pyproject).encode("utf-8"))
```

### Comparing `poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/cli.py` & `poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import argparse
-import sys
-from typing import (
-    Mapping,
-    Optional,
-)
-
-import tomlkit
-
-from poetry_dynamic_versioning import (
-    _get_and_apply_version,
-    _get_pyproject_path,
-    _state,
-    _validate_config,
-)
-
-_DEFAULT_REQUIRES = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
-_DEFAULT_BUILD_BACKEND = "poetry_dynamic_versioning.backend"
-
-
-class Key:
-    tool = "tool"
-    pdv = "poetry-dynamic-versioning"
-    enable = "enable"
-    build_system = "build-system"
-    requires = "requires"
-    build_backend = "build-backend"
-
-
-class Command:
-    dv = "dynamic-versioning"
-    enable = "enable"
-    dv_enable = "{} {}".format(dv, enable)
-
-
-class Help:
-    main = (
-        "Apply the dynamic version to all relevant files and leave the changes in-place."
-        " This allows you to activate the plugin behavior on demand and inspect the result."
-        " Your configuration will be detected from pyproject.toml as normal."
-    )
-    enable = (
-        "Update pyproject.toml to enable the plugin using a typical configuration."
-        " The output may not be suitable for more complex use cases."
-    )
-
-
-def parse_args(argv=None) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(description=Help.main)
-
-    subparsers = parser.add_subparsers(dest="cmd", title="subcommands")
-    subparsers.add_parser(Command.enable, help=Help.enable)
-
-    return parser.parse_args(argv)
-
-
-def validate(*, standalone: bool, config: Optional[Mapping] = None) -> None:
-    errors = _validate_config(config)
-    if errors:
-        if standalone:
-            print("Configuration issues:", file=sys.stderr)
-        else:
-            print("poetry-dynamic-versioning configuration issues:", file=sys.stderr)
-        for error in errors:
-            print("  - {}".format(error), file=sys.stderr)
-
-
-def apply(*, standalone: bool) -> None:
-    validate(standalone=standalone)
-
-    name = _get_and_apply_version(retain=True, force=True)
-    if not name:
-        raise RuntimeError("Unable to determine a dynamic version")
-
-    if standalone:
-        report_apply(name)
-
-
-def report_apply(name: str) -> None:
-    print("Version: {}".format(_state.projects[name].version), file=sys.stderr)
-    if _state.projects[name].substitutions:
-        print("Files with substitutions:", file=sys.stderr)
-        for file_name in _state.projects[name].substitutions:
-            print("  - {}".format(file_name), file=sys.stderr)
-    else:
-        print("Files with substitutions: none", file=sys.stderr)
-
-
-def enable() -> None:
-    pyproject_path = _get_pyproject_path()
-    if pyproject_path is None:
-        raise RuntimeError("Unable to find pyproject.toml")
-    config = tomlkit.parse(pyproject_path.read_text(encoding="utf-8"))
-
-    config = _enable_in_doc(config)
-    pyproject_path.write_bytes(tomlkit.dumps(config).encode("utf-8"))
-
-
-def _enable_in_doc(doc: tomlkit.TOMLDocument) -> tomlkit.TOMLDocument:
-    pdv_table = tomlkit.table().add(Key.enable, True)
-    tool_table = tomlkit.table().add(Key.pdv, pdv_table)
-
-    if doc.get(Key.tool) is None:
-        doc.add(Key.tool, tool_table)
-    elif doc[Key.tool].get(Key.pdv) is None:  # type: ignore
-        doc[Key.tool].add(Key.pdv, pdv_table)  # type: ignore
-    else:
-        doc[Key.tool][Key.pdv].update(pdv_table)  # type: ignore
-
-    build_system_table = (
-        tomlkit.table()
-        .add(Key.requires, _DEFAULT_REQUIRES)
-        .add(Key.build_backend, _DEFAULT_BUILD_BACKEND)
-    )
-
-    if doc.get(Key.build_system) is None:
-        doc.add(Key.build_system, build_system_table)
-    else:
-        doc[Key.build_system].update(build_system_table)  # type: ignore
-
-    return doc
+import argparse
+import sys
+from typing import (
+    Mapping,
+    Optional,
+)
+
+import tomlkit
+
+from poetry_dynamic_versioning import (
+    _get_and_apply_version,
+    _get_pyproject_path,
+    _state,
+    _validate_config,
+)
+
+_DEFAULT_REQUIRES = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+_DEFAULT_BUILD_BACKEND = "poetry_dynamic_versioning.backend"
+
+
+class Key:
+    tool = "tool"
+    pdv = "poetry-dynamic-versioning"
+    enable = "enable"
+    build_system = "build-system"
+    requires = "requires"
+    build_backend = "build-backend"
+
+
+class Command:
+    dv = "dynamic-versioning"
+    enable = "enable"
+    dv_enable = "{} {}".format(dv, enable)
+
+
+class Help:
+    main = (
+        "Apply the dynamic version to all relevant files and leave the changes in-place."
+        " This allows you to activate the plugin behavior on demand and inspect the result."
+        " Your configuration will be detected from pyproject.toml as normal."
+    )
+    enable = (
+        "Update pyproject.toml to enable the plugin using a typical configuration."
+        " The output may not be suitable for more complex use cases."
+    )
+
+
+def parse_args(argv=None) -> argparse.Namespace:
+    parser = argparse.ArgumentParser(description=Help.main)
+
+    subparsers = parser.add_subparsers(dest="cmd", title="subcommands")
+    subparsers.add_parser(Command.enable, help=Help.enable)
+
+    return parser.parse_args(argv)
+
+
+def validate(*, standalone: bool, config: Optional[Mapping] = None) -> None:
+    errors = _validate_config(config)
+    if errors:
+        if standalone:
+            print("Configuration issues:", file=sys.stderr)
+        else:
+            print("poetry-dynamic-versioning configuration issues:", file=sys.stderr)
+        for error in errors:
+            print("  - {}".format(error), file=sys.stderr)
+
+
+def apply(*, standalone: bool) -> None:
+    validate(standalone=standalone)
+
+    name = _get_and_apply_version(retain=True, force=True)
+    if not name:
+        raise RuntimeError("Unable to determine a dynamic version")
+
+    if standalone:
+        report_apply(name)
+
+
+def report_apply(name: str) -> None:
+    print("Version: {}".format(_state.projects[name].version), file=sys.stderr)
+    if _state.projects[name].substitutions:
+        print("Files with substitutions:", file=sys.stderr)
+        for file_name in _state.projects[name].substitutions:
+            print("  - {}".format(file_name), file=sys.stderr)
+    else:
+        print("Files with substitutions: none", file=sys.stderr)
+
+
+def enable() -> None:
+    pyproject_path = _get_pyproject_path()
+    if pyproject_path is None:
+        raise RuntimeError("Unable to find pyproject.toml")
+    config = tomlkit.parse(pyproject_path.read_bytes().decode("utf-8"))
+
+    config = _enable_in_doc(config)
+    pyproject_path.write_bytes(tomlkit.dumps(config).encode("utf-8"))
+
+
+def _enable_in_doc(doc: tomlkit.TOMLDocument) -> tomlkit.TOMLDocument:
+    pdv_table = tomlkit.table().add(Key.enable, True)
+    tool_table = tomlkit.table().add(Key.pdv, pdv_table)
+
+    if doc.get(Key.tool) is None:
+        doc.add(Key.tool, tool_table)
+    elif doc[Key.tool].get(Key.pdv) is None:  # type: ignore
+        doc[Key.tool].add(Key.pdv, pdv_table)  # type: ignore
+    else:
+        doc[Key.tool][Key.pdv].update(pdv_table)  # type: ignore
+
+    build_system_table = (
+        tomlkit.table()
+        .add(Key.requires, _DEFAULT_REQUIRES)
+        .add(Key.build_backend, _DEFAULT_BUILD_BACKEND)
+    )
+
+    if doc.get(Key.build_system) is None:
+        doc.add(Key.build_system, build_system_table)
+    else:
+        doc[Key.build_system].update(build_system_table)  # type: ignore
+
+    return doc
```

### Comparing `poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/patch.py` & `poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/patch.py`

 * *Files identical despite different names*

### Comparing `poetry_dynamic_versioning-1.1.1/poetry_dynamic_versioning/plugin.py` & `poetry_dynamic_versioning-1.2.0/poetry_dynamic_versioning/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_dynamic_versioning-1.1.1/pyproject.toml` & `poetry_dynamic_versioning-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-dynamic-versioning"
-version = "1.1.1"
+version = "1.2.0"
 description = "Plugin for Poetry to enable dynamic versioning based on VCS tags"
 license = "MIT"
 authors = ["Matthew T. Kennerly <mtkennerly@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/mtkennerly/poetry-dynamic-versioning"
 keywords = ["poetry", "plugin", "version", "versioning", "dynamic"]
 classifiers = [
@@ -47,14 +47,17 @@
 
 [tool.poetry.plugins."poetry.application.plugin"]
 poetry-dynamic-versioning = "poetry_dynamic_versioning.plugin:DynamicVersioningPlugin"
 
 [tool.black]
 line-length = 100
 
+[tool.mypy]
+allow_redefinition = true
+
 [tool.ruff]
 line-length = 100
 extend-select = ["W605", "N"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `poetry_dynamic_versioning-1.1.1/README.md` & `poetry_dynamic_versioning-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -256,14 +256,21 @@
   * `persistent-substitution` (boolean, optional):
     If true, then do not revert any substitutions applied to this file.
     This is primarily useful for editable installs, if you need the version to remain in a file ignored by your VCS.
   * `initial-content` (string, optional):
     Set the file content before the substitution phase.
     The file will be created or overwritten as necessary.
     Common leading whitespace will be stripped from each line.
+  * `initial-content-jinja` (string, optional):
+    Same as `initial-content`, but using Jinja formatting.
+    If both options are set, this one takes priority.
+    You can use the same imports from `format-jinja-imports` and the same variables from `format-jinja`,
+    with this additional variable:
+
+    * `formatted_version` (string) - version formatted by either the `format` or `format-jinja` option
 
   Example:
 
   ```toml
   [tool.poetry-dynamic-versioning.files."package/_version.py"]
   persistent-substitution = true
   initial-content = """
```

### Comparing `poetry_dynamic_versioning-1.1.1/tests/project/pyproject.toml` & `poetry_dynamic_versioning-1.2.0/tests/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_dynamic_versioning-1.1.1/tests/test_integration.py` & `poetry_dynamic_versioning-1.2.0/tests/test_integration.py`

 * *Files 13% similar despite different names*

```diff
@@ -84,109 +84,121 @@
 def test_plugin_enabled():
     run("poetry build", where=DUMMY)
     artifact = next(DUMMY_DIST.glob("*.whl"))
     assert DUMMY_VERSION not in artifact.name
 
 
 def test_plugin_disabled():
-    data = DUMMY_PYPROJECT.read_text("utf8")
+    data = DUMMY_PYPROJECT.read_bytes().decode("utf-8")
     data = data.replace("enable = true", "enable = false")
     DUMMY_PYPROJECT.write_bytes(data.encode("utf-8"))
 
     run("poetry build", where=DUMMY)
     artifact = next(DUMMY_DIST.glob("*.whl"))
     assert DUMMY_VERSION in artifact.name
 
 
 def test_plugin_disabled_without_plugin_section():
-    data = DUMMY_PYPROJECT.read_text("utf8")
+    data = DUMMY_PYPROJECT.read_bytes().decode("utf-8")
     data = data.replace("[tool.poetry-dynamic-versioning]", "[tool.poetry-dynamic-versioning-x]")
     DUMMY_PYPROJECT.write_bytes(data.encode("utf-8"))
 
     run("poetry build", where=DUMMY)
     artifact = next(DUMMY_DIST.glob("*.whl"))
     assert DUMMY_VERSION in artifact.name
 
 
 def test_plugin_disabled_without_pyproject_file():
     delete(DUMMY_PYPROJECT)
     run("poetry --help", where=DUMMY)
 
 
 def test_invalid_config_for_vcs():
-    data = DUMMY_PYPROJECT.read_text("utf8")
+    data = DUMMY_PYPROJECT.read_bytes().decode("utf-8")
     data = data.replace('vcs = "git"', 'vcs = "invalid"')
     DUMMY_PYPROJECT.write_bytes(data.encode("utf-8"))
 
     run("poetry build", where=DUMMY, codes=[1])
 
 
 def test_keep_pyproject_modifications():
     package = "cachy"
     # Using --optional to avoid actually installing the package
     run(f"poetry add --optional {package}", where=DUMMY)
     # Make sure pyproject.toml contains the new package dependency
-    data = DUMMY_PYPROJECT.read_text("utf8")
+    data = DUMMY_PYPROJECT.read_bytes().decode("utf-8")
     assert package in data
 
 
 def test_poetry_run():
     # The original version is restored before the command runs:
     run(f"poetry run grep 'version = \"{DUMMY_VERSION}\"' pyproject.toml", where=DUMMY)
     # Make sure original version number is still in place:
-    data = DUMMY_PYPROJECT.read_text("utf8")
+    data = DUMMY_PYPROJECT.read_bytes().decode("utf-8")
     assert f'version = "{DUMMY_VERSION}"' in data
 
 
 @pytest.mark.skipif("CI" in os.environ, reason="Avoid error: 'Inappropriate ioctl for device'")
 def test_poetry_shell():
     # Make sure original version number is still in place afterwards:
     run("poetry shell", where=DUMMY)
-    data = DUMMY_PYPROJECT.read_text("utf8")
+    data = DUMMY_PYPROJECT.read_bytes().decode("utf-8")
     assert f'version = "{DUMMY_VERSION}"' in data
 
 
 def test_plugin_cli_mode_and_substitution():
     run("poetry dynamic-versioning", where=DUMMY)
     # Changes persist after the command is done:
-    assert f'version = "{DUMMY_VERSION}"' not in DUMMY_PYPROJECT.read_text("utf8")
-    assert '__version__: str = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_text("utf8")
-    assert '__version__ = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_text("utf8")
+    assert f'version = "{DUMMY_VERSION}"' not in DUMMY_PYPROJECT.read_bytes().decode("utf-8")
+    assert '__version__: str = "0.0.0"' not in (
+        DUMMY / "project" / "__init__.py"
+    ).read_bytes().decode("utf-8")
+    assert '__version__ = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_bytes().decode(
+        "utf-8"
+    )
     assert "__version_tuple__ = (0, 0, 0)" not in (DUMMY / "project" / "__init__.py").read_text(
         "utf8"
     )
-    assert "<0.0.0>" not in (DUMMY / "project" / "__init__.py").read_text("utf8")
+    assert "<0.0.0>" not in (DUMMY / "project" / "__init__.py").read_bytes().decode("utf-8")
 
 
 def test_standalone_cli_mode_and_substitution():
     run("poetry-dynamic-versioning", where=DUMMY)
     # Changes persist after the command is done:
-    assert f'version = "{DUMMY_VERSION}"' not in DUMMY_PYPROJECT.read_text("utf8")
-    assert '__version__: str = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_text("utf8")
-    assert '__version__ = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_text("utf8")
+    assert f'version = "{DUMMY_VERSION}"' not in DUMMY_PYPROJECT.read_bytes().decode("utf-8")
+    assert '__version__: str = "0.0.0"' not in (
+        DUMMY / "project" / "__init__.py"
+    ).read_bytes().decode("utf-8")
+    assert '__version__ = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_bytes().decode(
+        "utf-8"
+    )
     assert "__version_tuple__ = (0, 0, 0)" not in (DUMMY / "project" / "__init__.py").read_text(
         "utf8"
     )
-    assert "<0.0.0>" not in (DUMMY / "project" / "__init__.py").read_text("utf8")
+    assert "<0.0.0>" not in (DUMMY / "project" / "__init__.py").read_bytes().decode("utf-8")
 
 
 def test_cli_mode_and_substitution_without_enable():
-    data = DUMMY_PYPROJECT.read_text("utf8")
+    data = DUMMY_PYPROJECT.read_bytes().decode("utf-8")
     data = data.replace("enable = true", "enable = false")
     DUMMY_PYPROJECT.write_bytes(data.encode("utf-8"))
 
     run("poetry dynamic-versioning", where=DUMMY)
     # Changes persist after the command is done:
-    assert f'version = "{DUMMY_VERSION}"' not in DUMMY_PYPROJECT.read_text("utf8")
-    assert '__version__: str = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_text("utf8")
-    assert '__version__ = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_text("utf8")
+    assert f'version = "{DUMMY_VERSION}"' not in DUMMY_PYPROJECT.read_bytes().decode("utf-8")
+    assert '__version__: str = "0.0.0"' not in (
+        DUMMY / "project" / "__init__.py"
+    ).read_bytes().decode("utf-8")
+    assert '__version__ = "0.0.0"' not in (DUMMY / "project" / "__init__.py").read_bytes().decode(
+        "utf-8"
+    )
     assert "__version_tuple__ = (0, 0, 0)" not in (DUMMY / "project" / "__init__.py").read_text(
         "utf8"
     )
-    assert "<0.0.0>" not in (DUMMY / "project" / "__init__.py").read_text("utf8")
+    assert "<0.0.0>" not in (DUMMY / "project" / "__init__.py").read_bytes().decode("utf-8")
 
 
 def test_cli_mode_plus_build_will_disable_plugin():
     run("poetry dynamic-versioning", where=DUMMY)
     run("poetry build", where=DUMMY)
     artifact = next(DUMMY_DIST.glob("*.tar.gz"))
     with tarfile.open(artifact, "r:gz") as f:
@@ -206,15 +218,15 @@
 
 
 def test_poetry_core_as_build_system():
     project = ROOT / "tests" / "dependency-dynamic"
     dist = project / "dist"
     pyproject = project / "pyproject.toml"
 
-    data = pyproject.read_text("utf8")
+    data = pyproject.read_bytes().decode("utf-8")
     data = re.sub(
         r"requires = .*",
         'requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]',
         data,
     )
     data = re.sub(
         r"build-backend = .*",
@@ -225,15 +237,15 @@
 
     run("pip wheel . --no-build-isolation --wheel-dir dist", where=project)
     artifact = next(dist.glob("*.whl"))
     assert DEPENDENCY_DYNAMIC_VERSION not in artifact.name
 
 
 def test_bumping_enabled():
-    data = DUMMY_PYPROJECT.read_text("utf8")
+    data = DUMMY_PYPROJECT.read_bytes().decode("utf-8")
     data = data.replace('vcs = "git"', "bump = true")
     data = data.replace('style = "semver"', 'style = "pep440"')
     DUMMY_PYPROJECT.write_bytes(data.encode("utf-8"))
 
     run("poetry build", where=DUMMY)
     artifact = next(DUMMY_DIST.glob("*.whl"))
     assert DUMMY_VERSION not in artifact.name
```

### Comparing `poetry_dynamic_versioning-1.1.1/tests/test_unit.py` & `poetry_dynamic_versioning-1.2.0/tests/test_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     config = plugin._get_config_from_path(root / "tests" / "project")
     assert config["vcs"] == "git"
     assert config["style"] == "semver"
     assert config["tag-dir"] == "alt/tags"
 
 
 def test__get_version__defaults(config):
-    assert plugin._get_version(config) == Version.from_git().serialize()
+    assert plugin._get_version(config)[0] == Version.from_git().serialize()
 
 
 def test__get_version__invalid_vcs(config):
     config["vcs"] = "invalid"
     with pytest.raises(ValueError):
         plugin._get_version(config)
 
@@ -64,34 +64,34 @@
     with pytest.raises(ValueError):
         plugin._get_version(config)
 
 
 def test__get_version__format_jinja(config):
     os.environ["FOO"] = "foo"
     config["format-jinja"] = "{% if true %}v1+{{ env['FOO'] }}{% endif %}"
-    assert plugin._get_version(config) == "v1+foo"
+    assert plugin._get_version(config)[0] == "v1+foo"
 
 
 def test__get_version__format_jinja_with_enforced_style(config):
     config["format-jinja"] = "{% if true %}1+jinja{% endif %}"
     config["style"] = "pvp"
     with pytest.raises(ValueError):
         plugin._get_version(config)
 
 
 def test__get_version__format_jinja_imports_with_module_only(config):
     config["format-jinja"] = "{{ math.pow(2, 2) }}"
-    config["format-jinja-imports"] = [{"module": "math"}]
-    assert plugin._get_version(config) == "4.0"
+    config["format-jinja-imports"] = [{"module": "math", "item": None}]
+    assert plugin._get_version(config)[0] == "4.0"
 
 
 def test__get_version__format_jinja_imports_with_module_and_item(config):
     config["format-jinja"] = "{{ pow(2, 3) }}"
     config["format-jinja-imports"] = [{"module": "math", "item": "pow"}]
-    assert plugin._get_version(config) == "8.0"
+    assert plugin._get_version(config)[0] == "8.0"
 
 
 def test__get_override_version__bypass():
     env = {plugin._BYPASS_ENV: "0.1.0"}
     assert plugin._get_override_version(None, env) == "0.1.0"
     assert plugin._get_override_version("foo", env) == "0.1.0"
```

### Comparing `poetry_dynamic_versioning-1.1.1/PKG-INFO` & `poetry_dynamic_versioning-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-dynamic-versioning
-Version: 1.1.1
+Version: 1.2.0
 Summary: Plugin for Poetry to enable dynamic versioning based on VCS tags
 Home-page: https://github.com/mtkennerly/poetry-dynamic-versioning
 License: MIT
 Keywords: poetry,plugin,version,versioning,dynamic
 Author: Matthew T. Kennerly
 Author-email: mtkennerly@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -290,14 +290,21 @@
   * `persistent-substitution` (boolean, optional):
     If true, then do not revert any substitutions applied to this file.
     This is primarily useful for editable installs, if you need the version to remain in a file ignored by your VCS.
   * `initial-content` (string, optional):
     Set the file content before the substitution phase.
     The file will be created or overwritten as necessary.
     Common leading whitespace will be stripped from each line.
+  * `initial-content-jinja` (string, optional):
+    Same as `initial-content`, but using Jinja formatting.
+    If both options are set, this one takes priority.
+    You can use the same imports from `format-jinja-imports` and the same variables from `format-jinja`,
+    with this additional variable:
+
+    * `formatted_version` (string) - version formatted by either the `format` or `format-jinja` option
 
   Example:
 
   ```toml
   [tool.poetry-dynamic-versioning.files."package/_version.py"]
   persistent-substitution = true
   initial-content = """
```

