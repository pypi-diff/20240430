# Comparing `tmp/omniconfig-0.1.2.tar.gz` & `tmp/omniconfig-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniconfig-0.1.2.tar", max compression
+gzip compressed data, was "omniconfig-0.1.3.tar", max compression
```

## Comparing `omniconfig-0.1.2.tar` & `omniconfig-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34523 2024-04-22 18:56:40.046281 omniconfig-0.1.2/LICENSE
--rw-r--r--   0        0        0     6478 2024-04-23 23:38:25.410432 omniconfig-0.1.2/README.md
--rw-r--r--   0        0        0      370 2024-04-23 23:47:53.317428 omniconfig-0.1.2/omniconfig/__init__.py
--rw-r--r--   0        0        0    17446 2024-04-22 19:39:16.088184 omniconfig-0.1.2/omniconfig/args.py
--rw-r--r--   0        0        0    13422 2024-04-23 21:56:49.634348 omniconfig-0.1.2/omniconfig/configclass.py
--rw-r--r--   0        0        0    10024 2024-04-23 23:28:39.099346 omniconfig-0.1.2/omniconfig/parser.py
--rw-r--r--   0        0        0     6473 2024-04-23 23:47:20.369254 omniconfig-0.1.2/omniconfig/utils.py
--rw-r--r--   0        0        0       89 2024-04-23 23:29:25.575591 omniconfig-0.1.2/omniconfig/version.py
--rw-r--r--   0        0        0      858 2024-04-23 23:29:19.059557 omniconfig-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7127 1970-01-01 00:00:00.000000 omniconfig-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-22 18:56:40.046281 omniconfig-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6478 2024-04-28 06:53:26.458810 omniconfig-0.1.3/README.md
+-rw-r--r--   0        0        0      391 2024-04-30 21:33:49.203985 omniconfig-0.1.3/omniconfig/__init__.py
+-rw-r--r--   0        0        0    17446 2024-04-28 06:53:26.502810 omniconfig-0.1.3/omniconfig/args.py
+-rw-r--r--   0        0        0    14702 2024-04-30 21:25:09.580828 omniconfig-0.1.3/omniconfig/configclass.py
+-rw-r--r--   0        0        0     9495 2024-04-30 21:30:31.694785 omniconfig-0.1.3/omniconfig/parser.py
+-rw-r--r--   0        0        0     6473 2024-04-28 06:53:26.510810 omniconfig-0.1.3/omniconfig/utils.py
+-rw-r--r--   0        0        0       89 2024-04-30 21:34:02.868068 omniconfig-0.1.3/omniconfig/version.py
+-rw-r--r--   0        0        0      858 2024-04-30 21:35:53.460740 omniconfig-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7127 1970-01-01 00:00:00.000000 omniconfig-0.1.3/PKG-INFO
```

### Comparing `omniconfig-0.1.2/LICENSE` & `omniconfig-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.2/README.md` & `omniconfig-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.2/omniconfig/args.py` & `omniconfig-0.1.3/omniconfig/args.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.2/omniconfig/configclass.py` & `omniconfig-0.1.3/omniconfig/configclass.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 from enum import Enum
 from inspect import signature
 from typing import Any, Callable, Type, TypeVar
 
 import docstring_parser
 
 from .args import Arguments, _format_prefix_to_flag
-from .utils import CONFIG_SUFFIXES, format_scope_and_prefix, parse_field_type, remove_suffix
+from .utils import (
+    CONFIG_SUFFIXES,
+    dump_toml,
+    dump_yaml,
+    format_scope_and_prefix,
+    parse_field_type,
+    remove_suffix,
+)
 
 __all__ = [
     "configclass",
     "get_arguments",
     "from_dict",
     "ARGPARSE_ARGS",
     "ARGPARSE_KWARGS",
@@ -47,14 +54,16 @@
     _set_field_docs(cls)
     if not hasattr(cls, "get_arguments"):
         setattr(cls, "get_arguments", classmethod(get_arguments))
     if not hasattr(cls, "from_dict"):
         setattr(cls, "from_dict", classmethod(from_dict))
     if not hasattr(cls, "formatted_str"):
         setattr(cls, "formatted_str", formatted_str)
+    if not hasattr(cls, "dump"):
+        setattr(cls, "dump", dump)
     return cls
 
 
 def _set_field_docs(cls) -> None:
     """Set field docs from the docstring of a config dataclass."""
     doc: str = cls.__doc__
     fields = getattr(cls, _FIELDS)  # include both fields and initvars
@@ -231,44 +240,44 @@
                 )
                 _kwargs["type"] = field_type
         # add to parser
         parser.add_argument(*_flags, **_kwargs)
     return parser
 
 
-def from_dict(cls: Type[_T], /, parsed_args: dict[str, Any], **defaults) -> _T:
+def from_dict(cls: Type[_T], /, parsed_args: dict[str, Any], **overwrites) -> _T:
     """Create a config dataclass from formatted parsed arguments dict.
 
     Args:
         cls (Type[_T@configclass]): Config dataclass type.
         parsed_args (dict[str, Any]): Formatted parsed arguments dict from `Arguments.to_dict`.
-        **defaults: Overwrite values for the config dataclass.
+        **overwrites: Overwrite values for the config dataclass.
 
     Returns:
         _T@configclass: The config dataclass instance.
     """
     if hasattr(cls, "update_from_dict"):
-        parsed_args, defaults = cls.update_from_dict(parsed_args=parsed_args, defaults=defaults)
+        parsed_args, overwrites = cls.update_from_dict(parsed_args=parsed_args, overwrites=overwrites)
     fields = _get_init_fields(cls)
     kwargs = {}
     for field in fields:
-        if field.name in defaults:
-            kwargs[field.name] = defaults[field.name]
+        if field.name in overwrites:
+            kwargs[field.name] = overwrites[field.name]
         elif field.name in parsed_args:
             field_type, field_type_optional = parse_field_type(field.type)
             if hasattr(field_type, "from_dict"):
                 if field_type_optional and not parsed_args.get(f"enable_{field.name}", False):
                     kwargs[field.name] = None
                 else:
                     _kwargs: dict[str, Any] = field.metadata.get(ARGPARSE_KWARGS, {})
                     _prefix = _kwargs.get("prefix", remove_suffix(field.name, CONFIG_SUFFIXES))
                     _n = len(_prefix) + (1 if _prefix else 0)
                     kwargs[field.name] = field_type.from_dict(
                         parsed_args[field.name],
-                        **{k[_n:]: v for k, v in defaults.items() if k.startswith(_prefix)},
+                        **{k[_n:]: v for k, v in overwrites.items() if k.startswith(_prefix)},
                     )
             else:
                 kwargs[field.name] = parsed_args[field.name]
     return cls(**kwargs)
 
 
 def formatted_str(self: _T, /, indent: int = 2, level: int = 0) -> str:
@@ -291,14 +300,51 @@
         if hasattr(value, "formatted_str"):
             s += f"\n{_}{field.name}={value.formatted_str(indent=indent, level=level)},"
         else:
             s += f"\n{_}{field.name}={value},"
     return s[:-1] + ")"
 
 
+def _to_dump_value(value: Any) -> Any:
+    if hasattr(value, "dump"):
+        return value.dump()
+    elif value is None:
+        return None
+    elif isinstance(value, (str, int, float, complex, bool)):
+        return value
+    elif isinstance(value, Enum):
+        return value.name
+    elif isinstance(value, (list, tuple)):
+        return [_to_dump_value(v) for v in value]
+    elif isinstance(value, dict):
+        return {k: _to_dump_value(v) for k, v in value.items()}
+    return str(value)
+
+
+def dump(self: _T, path: str = "") -> dict[str, Any]:
+    """Dump config dict of a config dataclass.
+
+    Args:
+        self: Config dataclass instance.
+        path (str): Path to dump the config dict. Defaults to ``""``.
+
+    Returns:
+        dict[str, Any]: The dict.
+    """
+    rst = {field.name: _to_dump_value(getattr(self, field.name)) for field in _get_init_fields(self.__class__)}
+    if path:
+        if path.endswith(".toml"):
+            dump_toml(rst, path)
+        elif path.endswith(("yaml", "yml")):
+            dump_yaml(rst, path)
+        else:
+            raise ValueError(f"Unsupported file format {path}")
+    return rst
+
+
 def IGNORE_FIELD(parser: Arguments) -> None:
     """Ignore a field when adding arguments to a parser."""
     pass
 
 
 def ADD_PREFIX_BOOL_FIELDS(prefix: str, **defaults) -> Callable[[Arguments], None]:
     """Add boolean fields with same prefix to a parser."""
```

### Comparing `omniconfig-0.1.2/omniconfig/parser.py` & `omniconfig-0.1.3/omniconfig/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Parser class."""
 
 import argparse
 import os
 from typing import Any, Callable, Sequence, Type, TypeVar
 
 from .args import Arguments
-from .utils import dump_yaml, format_scope_and_prefix, load_yaml, update_dict, load_toml, dump_toml
+from .utils import dump_toml, dump_yaml, format_scope_and_prefix, load_toml, load_yaml, update_dict
 
 __all__ = ["ConfigParser"]
 
 
 _T = TypeVar("_T")
 
 
@@ -199,38 +199,24 @@
 
         Returns:
             tuple[dict[str, Any] | Any, dict[str, Any], list[str]]: Configs from the parsed arguments,
                                                                     parsed yaml configs, and unknown arguments.
         """
         return self._parse_args(args=args, namespace=namespace, **defaults)
 
-    def dump_yaml(self, path: str | None = None) -> str | None:
-        """Dump default yaml config file.
+    def dump_default(self, path: str) -> None:
+        """Dump default config file.
 
         Args:
-            path (str | None, optional): Path to dump the yaml file. Defaults to ``None``.
-
-        Returns:
-            str | None: Dumped yaml string if ``path`` is ``None``.
-        """
-        default: dict[str, dict] = {}
-        for scope, (cfg, args, prefix) in self._cfgs.items():
-            default[scope] = args.to_dict(detailed=False)
-        if len(self._cfgs) == 1:
-            default = next(iter(default.values()))
-        return dump_yaml(default, path=path)
-    
-    def dump_toml(self, path: str | None = None) -> str | None:
-        """Dump default toml config file.
-
-        Args:
-            path (str | None, optional): Path to dump the toml file. Defaults to ``None``.
-
-        Returns:
-            str | None: Dumped toml string if ``path`` is ``None``.
+            path (str | None, optional): Path to dump the file.
         """
         default: dict[str, dict] = {}
         for scope, (cfg, args, prefix) in self._cfgs.items():
             default[scope] = args.to_dict(detailed=False)
         if len(self._cfgs) == 1:
             default = next(iter(default.values()))
-        return dump_toml(default, path=path)
+        if path.endswith(("yaml", "yml")):
+            return dump_yaml(default, path=path)
+        elif path.endswith("toml"):
+            return dump_toml(default, path=path)
+        else:
+            raise ValueError(f"unsupported file type {path}")
```

### Comparing `omniconfig-0.1.2/omniconfig/utils.py` & `omniconfig-0.1.3/omniconfig/utils.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.2/pyproject.toml` & `omniconfig-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniconfig"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python package for parsing configurations from YAML and TOML and command-line interface."
 authors = ["Yujun(Xavier) Lin"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10 <4.0"
```

### Comparing `omniconfig-0.1.2/PKG-INFO` & `omniconfig-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniconfig
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for parsing configurations from YAML and TOML and command-line interface.
 License: AGPL-3.0-only
 Author: Yujun(Xavier) Lin
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

